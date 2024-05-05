# Comparing `tmp/libvsmbr-python-20240302.tar.gz` & `tmp/libvsmbr-python-20240505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvsmbr-python-20240302.tar", last modified: Sat Mar  2 13:39:42 2024, max compression
+gzip compressed data, was "libvsmbr-python-20240505.tar", last modified: Sun May  5 04:58:33 2024, max compression
```

## Comparing `libvsmbr-python-20240302.tar` & `libvsmbr-python-20240505.tar`

### file list

```diff
@@ -1,729 +1,731 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:40.000000 libvsmbr-20240302/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31392 2024-03-02 06:52:58.000000 libvsmbr-20240302/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-03-02 06:52:46.000000 libvsmbr-20240302/libfdata/libfdata_vector.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/libvsmbr/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1693 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/vsmbr_partition_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8802 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9692 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2151 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_sector_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2919 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2221 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2207 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_partition_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-03-02 06:53:15.000000 libvsmbr-20240302/libvsmbr/libvsmbr_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1755 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_chs_address.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2202 2023-12-03 09:16:46.000000 libvsmbr-20240302/libvsmbr/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11988 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_boot_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42722 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_section_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1100 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1098 2024-03-02 06:53:15.000000 libvsmbr-20240302/libvsmbr/libvsmbr.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3055 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_section_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3696 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1871 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_partition_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4476 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_partition_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5561 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_partition_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4591 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_partition_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5158 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_chs_address.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1843 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2078 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/vsmbr_boot_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8423 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_partition_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2179 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33887 2024-03-02 06:52:58.000000 libvsmbr-20240302/libvsmbr/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25893 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_partition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4000 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_partition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2381 2024-03-02 06:44:24.000000 libvsmbr-20240302/libvsmbr/libvsmbr_boot_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3214 2024-03-02 06:41:40.000000 libvsmbr-20240302/libvsmbr.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-03-02 06:41:40.000000 libvsmbr-20240302/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-03-02 06:52:58.000000 libvsmbr-20240302/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 06:41:40.000000 libvsmbr-20240302/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-03-02 06:52:59.000000 libvsmbr-20240302/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:38.000000 libvsmbr-20240302/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-02 06:52:53.000000 libvsmbr-20240302/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-03-02 06:52:53.000000 libvsmbr-20240302/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-03-02 06:52:53.000000 libvsmbr-20240302/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-03-02 06:52:54.000000 libvsmbr-20240302/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-03-02 06:52:53.000000 libvsmbr-20240302/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:16:46.000000 libvsmbr-20240302/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:39.000000 libvsmbr-20240302/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:39.000000 libvsmbr-20240302/include/libvsmbr/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1799 2024-03-02 06:44:24.000000 libvsmbr-20240302/include/libvsmbr/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2024-03-02 06:53:15.000000 libvsmbr-20240302/include/libvsmbr/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4983 2024-03-02 06:44:24.000000 libvsmbr-20240302/include/libvsmbr/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4852 2024-03-02 06:53:15.000000 libvsmbr-20240302/include/libvsmbr/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-02 06:44:24.000000 libvsmbr-20240302/include/libvsmbr/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-03-02 06:44:24.000000 libvsmbr-20240302/include/libvsmbr/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-02 06:44:24.000000 libvsmbr-20240302/include/libvsmbr/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-03-02 06:53:15.000000 libvsmbr-20240302/include/libvsmbr/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-03-02 06:44:24.000000 libvsmbr-20240302/include/libvsmbr/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11155 2024-03-02 06:44:24.000000 libvsmbr-20240302/include/libvsmbr.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      474 2024-03-02 06:41:40.000000 libvsmbr-20240302/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11155 2024-03-02 06:53:15.000000 libvsmbr-20240302/include/libvsmbr.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26153 2024-03-02 06:52:58.000000 libvsmbr-20240302/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:39.000000 libvsmbr-20240302/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-03-02 06:41:40.000000 libvsmbr-20240302/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-03-02 06:53:15.000000 libvsmbr-20240302/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15432 2024-03-02 06:52:57.000000 libvsmbr-20240302/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16351 2024-03-02 06:53:15.000000 libvsmbr-20240302/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-03-02 06:44:24.000000 libvsmbr-20240302/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23160 2024-03-02 06:52:58.000000 libvsmbr-20240302/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:39.000000 libvsmbr-20240302/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28163 2024-03-02 06:52:58.000000 libvsmbr-20240302/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-02 06:52:38.000000 libvsmbr-20240302/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:40.000000 libvsmbr-20240302/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28636 2024-03-02 06:52:58.000000 libvsmbr-20240302/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-03-02 06:52:44.000000 libvsmbr-20240302/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2023-12-03 09:16:34.000000 libvsmbr-20240302/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:40.000000 libvsmbr-20240302/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31622 2024-03-02 06:52:58.000000 libvsmbr-20240302/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-03-02 06:52:32.000000 libvsmbr-20240302/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:16:34.000000 libvsmbr-20240302/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-03-02 06:52:58.000000 libvsmbr-20240302/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:38.000000 libvsmbr-20240302/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-03-02 06:44:24.000000 libvsmbr-20240302/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:38.000000 libvsmbr-20240302/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-03-02 06:41:40.000000 libvsmbr-20240302/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2190 2024-03-02 06:41:40.000000 libvsmbr-20240302/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-03-02 06:41:40.000000 libvsmbr-20240302/dpkg/libvsmbr-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-03-02 06:41:40.000000 libvsmbr-20240302/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-03-02 06:41:40.000000 libvsmbr-20240302/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-03-02 06:53:15.000000 libvsmbr-20240302/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-03-02 06:41:40.000000 libvsmbr-20240302/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-03-02 06:41:40.000000 libvsmbr-20240302/dpkg/libvsmbr.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-03-02 06:53:15.000000 libvsmbr-20240302/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-03-02 06:41:40.000000 libvsmbr-20240302/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1664789 2024-03-02 06:52:57.000000 libvsmbr-20240302/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-03-02 06:52:58.000000 libvsmbr-20240302/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-03-02 06:52:58.000000 libvsmbr-20240302/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libvsmbr/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8716 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libvsmbr/libvsmbr.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5617 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_tools_signal/vsmbr_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5510 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_notify/vsmbr_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5423 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_error/vsmbr_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5782 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_tools_info_handle/vsmbr_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_partition_type/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5696 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_partition_type/vsmbr_test_partition_type.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_partition_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5699 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_partition_entry/vsmbr_test_partition_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_partition_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5702 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_partition_values/vsmbr_test_partition_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_section_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5696 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_section_values/vsmbr_test_section_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5617 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_tools_output/vsmbr_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5681 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_io_handle/vsmbr_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbrinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbrinfo/vsmbrinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/pyvsmbr/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6383 2024-03-02 06:42:18.000000 libvsmbr-20240302/msvscpp/pyvsmbr/pyvsmbr.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_chs_address/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5687 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_chs_address/vsmbr_test_chs_address.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_boot_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5937 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_boot_record/vsmbr_test_boot_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_partition/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6173 2024-03-02 06:42:18.000000 libvsmbr-20240302/msvscpp/vsmbr_test_partition/vsmbr_test_partition.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6338 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_support/vsmbr_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_sector_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5937 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/vsmbr_test_sector_data/vsmbr_test_sector_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/vsmbr_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6497 2024-03-02 06:42:18.000000 libvsmbr-20240302/msvscpp/vsmbr_test_volume/vsmbr_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21597 2024-03-02 06:52:58.000000 libvsmbr-20240302/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-03-02 06:42:05.000000 libvsmbr-20240302/msvscpp/libcerror/libcerror.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28813 2024-03-02 06:42:18.000000 libvsmbr-20240302/msvscpp/libvsmbr.sln
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      659 2024-03-02 06:41:40.000000 libvsmbr-20240302/libvsmbr.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-03-02 06:44:24.000000 libvsmbr-20240302/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:40.000000 libvsmbr-20240302/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28927 2024-03-02 06:52:58.000000 libvsmbr-20240302/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-03-02 06:52:36.000000 libvsmbr-20240302/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      395 2024-03-02 06:42:18.000000 libvsmbr-20240302/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-03-02 06:52:58.000000 libvsmbr-20240302/INSTALL
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2458 2024-03-02 06:53:15.000000 libvsmbr-20240302/libvsmbr.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:39.000000 libvsmbr-20240302/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30611 2024-03-02 06:52:58.000000 libvsmbr-20240302/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 06:52:34.000000 libvsmbr-20240302/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-02 06:41:40.000000 libvsmbr-20240302/pyproject.toml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/vsmbrtools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2676 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1132 2023-12-03 09:16:44.000000 libvsmbr-20240302/vsmbrtools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22087 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3451 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6879 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29542 2024-03-02 06:52:59.000000 libvsmbr-20240302/vsmbrtools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_libvsmbr.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-02 06:44:24.000000 libvsmbr-20240302/vsmbrtools/vsmbrtools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-03-02 06:41:40.000000 libvsmbr-20240302/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-03-02 06:52:58.000000 libvsmbr-20240302/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-03-02 06:41:40.000000 libvsmbr-20240302/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2024-03-02 06:41:40.000000 libvsmbr-20240302/acinclude.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/pyvsmbr/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2949 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2445 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_partitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23854 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1168 2023-12-03 09:16:47.000000 libvsmbr-20240302/pyvsmbr/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15102 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_libvsmbr.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22357 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_partition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9329 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_partitions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40597 2024-03-02 06:52:59.000000 libvsmbr-20240302/pyvsmbr/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2761 2024-03-02 06:44:24.000000 libvsmbr-20240302/pyvsmbr/pyvsmbr_partition.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:16:34.000000 libvsmbr-20240302/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:39.000000 libvsmbr-20240302/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31017 2024-03-02 06:52:58.000000 libvsmbr-20240302/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-02 06:52:43.000000 libvsmbr-20240302/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-03-02 06:52:59.000000 libvsmbr-20240302/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:40.000000 libvsmbr-20240302/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28205 2024-03-02 06:52:58.000000 libvsmbr-20240302/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-03-02 06:52:41.000000 libvsmbr-20240302/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      372 2023-12-03 09:16:34.000000 libvsmbr-20240302/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      158 2023-12-03 09:16:46.000000 libvsmbr-20240302/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2024-03-02 06:44:24.000000 libvsmbr-20240302/manuals/vsmbrinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5519 2024-03-02 06:44:24.000000 libvsmbr-20240302/manuals/libvsmbr.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25130 2024-03-02 06:52:58.000000 libvsmbr-20240302/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_getopt.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-03-02 06:41:45.000000 libvsmbr-20240302/tests/test_vsmbrinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/pyvsmbr_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_error.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4068 2024-03-02 06:42:42.000000 libvsmbr-20240302/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_libvsmbr.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7449 2024-03-02 06:42:18.000000 libvsmbr-20240302/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12950 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_partition_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59346 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_partition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5686 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/pyvsmbr_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6608 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_rwlock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1833 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_partition_type.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-02 06:41:45.000000 libvsmbr-20240302/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4088 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_rwlock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10125 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_chs_address.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26256 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_boot_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-03-02 06:41:45.000000 libvsmbr-20240302/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9606 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9072 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/pyvsmbr_test_partition.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9326 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_partition_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31131 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62839 2024-03-02 06:52:59.000000 libvsmbr-20240302/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6235 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_section_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14431 2024-03-02 06:44:24.000000 libvsmbr-20240302/tests/vsmbr_test_support.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4186 2024-03-02 06:42:42.000000 libvsmbr-20240302/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2024-03-02 06:44:24.000000 libvsmbr-20240302/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-03-02 06:44:24.000000 libvsmbr-20240302/ossfuzz/ossfuzz_libvsmbr.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2023-12-03 09:16:35.000000 libvsmbr-20240302/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-02 06:44:24.000000 libvsmbr-20240302/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2700 2024-03-02 06:44:24.000000 libvsmbr-20240302/ossfuzz/partition_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32387 2024-03-02 06:52:58.000000 libvsmbr-20240302/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-03-02 06:52:53.000000 libvsmbr-20240302/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:39.000000 libvsmbr-20240302/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28985 2024-03-02 06:52:58.000000 libvsmbr-20240302/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-03-02 06:52:42.000000 libvsmbr-20240302/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:41.000000 libvsmbr-20240302/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-03-02 06:53:15.000000 libvsmbr-20240302/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:16:46.000000 libvsmbr-20240302/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:40.000000 libvsmbr-20240302/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51729 2024-03-02 06:52:58.000000 libvsmbr-20240302/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-03-02 06:52:48.000000 libvsmbr-20240302/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39024 2024-03-02 06:52:58.000000 libvsmbr-20240302/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:39.000000 libvsmbr-20240302/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28039 2024-03-02 06:52:58.000000 libvsmbr-20240302/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-03-02 06:52:39.000000 libvsmbr-20240302/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 13:39:39.000000 libvsmbr-20240302/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-02 06:52:35.000000 libvsmbr-20240302/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27552 2024-03-02 06:52:58.000000 libvsmbr-20240302/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56736 2024-03-02 06:52:55.000000 libvsmbr-20240302/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6985 2024-03-02 06:44:24.000000 libvsmbr-20240302/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-03-02 13:39:42.467626 libvsmbr-20240302/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:30.000000 libvsmbr-20240505/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31956 2024-05-05 04:41:26.000000 libvsmbr-20240505/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-05 04:41:08.000000 libvsmbr-20240505/libfdata/libfdata_vector.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:31.000000 libvsmbr-20240505/libvsmbr/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1693 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/vsmbr_partition_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8802 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9692 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2151 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_sector_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2919 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2221 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2207 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_partition_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-05-05 04:41:43.000000 libvsmbr-20240505/libvsmbr/libvsmbr_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1755 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_chs_address.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2188 2024-05-04 14:51:05.000000 libvsmbr-20240505/libvsmbr/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11988 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_boot_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42722 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_section_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1100 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1098 2024-05-05 04:41:43.000000 libvsmbr-20240505/libvsmbr/libvsmbr.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3055 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_section_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3696 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1871 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_partition_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4476 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_partition_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5561 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_partition_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4591 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_partition_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5158 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_chs_address.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1843 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2078 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/vsmbr_boot_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8423 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_partition_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2179 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34551 2024-05-05 04:41:26.000000 libvsmbr-20240505/libvsmbr/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25893 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_partition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4000 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_partition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2381 2024-05-04 13:23:42.000000 libvsmbr-20240505/libvsmbr/libvsmbr_boot_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3214 2024-05-04 13:23:39.000000 libvsmbr-20240505/libvsmbr.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-04 13:23:39.000000 libvsmbr-20240505/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-05 04:41:26.000000 libvsmbr-20240505/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 13:23:39.000000 libvsmbr-20240505/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-05 04:41:26.000000 libvsmbr-20240505/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:28.000000 libvsmbr-20240505/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-05 04:41:20.000000 libvsmbr-20240505/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-05 04:41:20.000000 libvsmbr-20240505/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-05 04:41:20.000000 libvsmbr-20240505/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-05 04:41:20.000000 libvsmbr-20240505/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-05 04:41:20.000000 libvsmbr-20240505/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:16:46.000000 libvsmbr-20240505/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-04 13:23:44.000000 libvsmbr-20240505/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:28.000000 libvsmbr-20240505/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:28.000000 libvsmbr-20240505/include/libvsmbr/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1799 2024-05-04 13:23:42.000000 libvsmbr-20240505/include/libvsmbr/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2024-05-05 04:41:43.000000 libvsmbr-20240505/include/libvsmbr/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4983 2024-05-04 13:23:42.000000 libvsmbr-20240505/include/libvsmbr/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4852 2024-05-05 04:41:43.000000 libvsmbr-20240505/include/libvsmbr/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-04 13:23:42.000000 libvsmbr-20240505/include/libvsmbr/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-05-04 13:23:42.000000 libvsmbr-20240505/include/libvsmbr/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-04 13:23:42.000000 libvsmbr-20240505/include/libvsmbr/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-05-05 04:41:43.000000 libvsmbr-20240505/include/libvsmbr/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-05-04 13:23:42.000000 libvsmbr-20240505/include/libvsmbr/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11155 2024-05-04 13:23:42.000000 libvsmbr-20240505/include/libvsmbr.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      425 2024-05-04 14:50:28.000000 libvsmbr-20240505/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11155 2024-05-05 04:41:43.000000 libvsmbr-20240505/include/libvsmbr.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26133 2024-05-05 04:41:26.000000 libvsmbr-20240505/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:28.000000 libvsmbr-20240505/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-04 14:50:28.000000 libvsmbr-20240505/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-05-05 04:41:43.000000 libvsmbr-20240505/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15432 2024-05-05 04:41:25.000000 libvsmbr-20240505/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16351 2024-05-05 04:41:43.000000 libvsmbr-20240505/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-04 13:23:41.000000 libvsmbr-20240505/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23167 2024-05-05 04:41:26.000000 libvsmbr-20240505/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:29.000000 libvsmbr-20240505/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28365 2024-05-05 04:41:26.000000 libvsmbr-20240505/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-05 04:40:44.000000 libvsmbr-20240505/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:30.000000 libvsmbr-20240505/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28874 2024-05-05 04:41:26.000000 libvsmbr-20240505/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-05 04:41:05.000000 libvsmbr-20240505/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-05-04 14:52:34.000000 libvsmbr-20240505/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:30.000000 libvsmbr-20240505/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32217 2024-05-05 04:41:26.000000 libvsmbr-20240505/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-05 04:40:25.000000 libvsmbr-20240505/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:16:34.000000 libvsmbr-20240505/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-05 04:41:26.000000 libvsmbr-20240505/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:28.000000 libvsmbr-20240505/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-05-04 13:23:44.000000 libvsmbr-20240505/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:28.000000 libvsmbr-20240505/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-04 13:23:39.000000 libvsmbr-20240505/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2190 2024-05-04 13:23:39.000000 libvsmbr-20240505/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-04 13:23:39.000000 libvsmbr-20240505/dpkg/libvsmbr-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-05-04 13:23:39.000000 libvsmbr-20240505/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-04 13:23:39.000000 libvsmbr-20240505/dpkg/libvsmbr-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-05-04 13:23:39.000000 libvsmbr-20240505/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-05-05 04:41:43.000000 libvsmbr-20240505/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-04 13:23:39.000000 libvsmbr-20240505/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-04 13:23:39.000000 libvsmbr-20240505/dpkg/libvsmbr.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-04 13:23:39.000000 libvsmbr-20240505/dpkg/libvsmbr-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-05-05 04:41:43.000000 libvsmbr-20240505/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-04 13:23:39.000000 libvsmbr-20240505/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1667012 2024-05-05 04:41:24.000000 libvsmbr-20240505/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-05 04:41:26.000000 libvsmbr-20240505/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-05 04:41:26.000000 libvsmbr-20240505/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libvsmbr/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8716 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libvsmbr/libvsmbr.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5617 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_tools_signal/vsmbr_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5510 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_notify/vsmbr_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-04 14:51:51.000000 libvsmbr-20240505/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5423 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_error/vsmbr_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5782 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_tools_info_handle/vsmbr_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_partition_type/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5696 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_partition_type/vsmbr_test_partition_type.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_partition_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5699 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_partition_entry/vsmbr_test_partition_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_partition_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5702 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_partition_values/vsmbr_test_partition_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_section_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5696 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_section_values/vsmbr_test_section_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5617 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_tools_output/vsmbr_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5681 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_io_handle/vsmbr_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbrinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbrinfo/vsmbrinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/pyvsmbr/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6383 2024-05-04 14:48:25.000000 libvsmbr-20240505/msvscpp/pyvsmbr/pyvsmbr.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_chs_address/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5687 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_chs_address/vsmbr_test_chs_address.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_boot_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5937 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_boot_record/vsmbr_test_boot_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_partition/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6173 2024-05-04 14:48:25.000000 libvsmbr-20240505/msvscpp/vsmbr_test_partition/vsmbr_test_partition.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6338 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_support/vsmbr_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_sector_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5937 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/vsmbr_test_sector_data/vsmbr_test_sector_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/vsmbr_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6497 2024-05-04 14:48:25.000000 libvsmbr-20240505/msvscpp/vsmbr_test_volume/vsmbr_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21597 2024-05-05 04:41:26.000000 libvsmbr-20240505/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-04 13:24:19.000000 libvsmbr-20240505/msvscpp/libcerror/libcerror.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28813 2024-05-04 14:48:25.000000 libvsmbr-20240505/msvscpp/libvsmbr.sln
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      659 2024-05-04 13:23:39.000000 libvsmbr-20240505/libvsmbr.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-05-04 13:23:41.000000 libvsmbr-20240505/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:30.000000 libvsmbr-20240505/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29198 2024-05-05 04:41:26.000000 libvsmbr-20240505/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-05 04:40:39.000000 libvsmbr-20240505/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      395 2024-05-04 14:48:30.000000 libvsmbr-20240505/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-05 04:41:26.000000 libvsmbr-20240505/INSTALL
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2458 2024-05-05 04:41:43.000000 libvsmbr-20240505/libvsmbr.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:29.000000 libvsmbr-20240505/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31111 2024-05-05 04:41:26.000000 libvsmbr-20240505/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 04:40:29.000000 libvsmbr-20240505/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-04 13:23:39.000000 libvsmbr-20240505/pyproject.toml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:31.000000 libvsmbr-20240505/vsmbrtools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2676 2024-05-04 14:48:30.000000 libvsmbr-20240505/vsmbrtools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1128 2024-05-04 14:52:04.000000 libvsmbr-20240505/vsmbrtools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22087 2024-05-04 14:48:30.000000 libvsmbr-20240505/vsmbrtools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3451 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6879 2024-05-04 14:48:30.000000 libvsmbr-20240505/vsmbrtools/vsmbrinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29759 2024-05-05 04:41:26.000000 libvsmbr-20240505/vsmbrtools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_libvsmbr.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-04 13:23:43.000000 libvsmbr-20240505/vsmbrtools/vsmbrtools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-05-04 13:23:39.000000 libvsmbr-20240505/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-05 04:41:26.000000 libvsmbr-20240505/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-04 13:23:39.000000 libvsmbr-20240505/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2024-05-04 13:23:39.000000 libvsmbr-20240505/acinclude.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:31.000000 libvsmbr-20240505/pyvsmbr/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2949 2024-05-04 14:48:30.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2445 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_partitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23854 2024-05-04 14:48:30.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-04 14:51:43.000000 libvsmbr-20240505/pyvsmbr/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15102 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_libvsmbr.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22330 2024-05-04 14:48:30.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_partition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9329 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_partitions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40988 2024-05-05 04:41:26.000000 libvsmbr-20240505/pyvsmbr/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2761 2024-05-04 13:23:43.000000 libvsmbr-20240505/pyvsmbr/pyvsmbr_partition.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:16:34.000000 libvsmbr-20240505/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:29.000000 libvsmbr-20240505/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31550 2024-05-05 04:41:26.000000 libvsmbr-20240505/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-05 04:41:00.000000 libvsmbr-20240505/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-05 04:41:26.000000 libvsmbr-20240505/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:30.000000 libvsmbr-20240505/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28396 2024-05-05 04:41:26.000000 libvsmbr-20240505/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-05 04:40:51.000000 libvsmbr-20240505/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      372 2023-12-03 09:16:34.000000 libvsmbr-20240505/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:31.000000 libvsmbr-20240505/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      129 2024-05-04 14:51:35.000000 libvsmbr-20240505/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2024-05-04 13:23:44.000000 libvsmbr-20240505/manuals/vsmbrinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5519 2024-05-04 13:23:44.000000 libvsmbr-20240505/manuals/libvsmbr.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25130 2024-05-05 04:41:26.000000 libvsmbr-20240505/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_getopt.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3289 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/test_vsmbrinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/pyvsmbr_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_error.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4037 2024-05-04 14:49:32.000000 libvsmbr-20240505/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_libvsmbr.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7466 2024-05-04 15:19:34.000000 libvsmbr-20240505/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12950 2024-05-04 14:48:25.000000 libvsmbr-20240505/tests/vsmbr_test_partition_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59346 2024-05-04 14:48:25.000000 libvsmbr-20240505/tests/vsmbr_test_partition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5686 2024-05-04 14:48:30.000000 libvsmbr-20240505/tests/pyvsmbr_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6608 2024-05-04 14:48:25.000000 libvsmbr-20240505/tests/vsmbr_test_rwlock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1833 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_partition_type.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4417 2024-05-04 14:49:17.000000 libvsmbr-20240505/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_rwlock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10125 2024-05-04 14:48:25.000000 libvsmbr-20240505/tests/vsmbr_test_chs_address.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26256 2024-05-04 14:48:25.000000 libvsmbr-20240505/tests/vsmbr_test_boot_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9606 2024-05-04 14:48:25.000000 libvsmbr-20240505/tests/vsmbr_test_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9072 2024-05-04 14:48:30.000000 libvsmbr-20240505/tests/pyvsmbr_test_partition.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9326 2024-05-04 14:48:25.000000 libvsmbr-20240505/tests/vsmbr_test_partition_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31131 2024-05-04 14:48:25.000000 libvsmbr-20240505/tests/vsmbr_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63941 2024-05-05 04:41:26.000000 libvsmbr-20240505/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6235 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_section_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14431 2024-05-04 13:23:44.000000 libvsmbr-20240505/tests/vsmbr_test_support.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4155 2024-05-04 14:49:46.000000 libvsmbr-20240505/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:32.000000 libvsmbr-20240505/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2024-05-04 13:23:42.000000 libvsmbr-20240505/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-05-04 13:23:42.000000 libvsmbr-20240505/ossfuzz/ossfuzz_libvsmbr.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1430 2024-05-04 14:51:16.000000 libvsmbr-20240505/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-04 13:23:42.000000 libvsmbr-20240505/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2700 2024-05-04 13:23:42.000000 libvsmbr-20240505/ossfuzz/partition_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32490 2024-05-05 04:41:26.000000 libvsmbr-20240505/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-05 04:41:20.000000 libvsmbr-20240505/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:29.000000 libvsmbr-20240505/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29293 2024-05-05 04:41:26.000000 libvsmbr-20240505/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-05 04:40:57.000000 libvsmbr-20240505/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:31.000000 libvsmbr-20240505/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-05-05 04:41:43.000000 libvsmbr-20240505/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:16:46.000000 libvsmbr-20240505/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:30.000000 libvsmbr-20240505/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54877 2024-05-05 04:41:26.000000 libvsmbr-20240505/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-05 04:41:15.000000 libvsmbr-20240505/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38970 2024-05-05 04:41:26.000000 libvsmbr-20240505/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:29.000000 libvsmbr-20240505/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28234 2024-05-05 04:41:26.000000 libvsmbr-20240505/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-05 04:40:47.000000 libvsmbr-20240505/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 04:58:28.000000 libvsmbr-20240505/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-05 04:40:32.000000 libvsmbr-20240505/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27701 2024-05-05 04:41:26.000000 libvsmbr-20240505/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56736 2024-05-05 04:41:23.000000 libvsmbr-20240505/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6985 2024-05-05 04:31:44.000000 libvsmbr-20240505/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-05-05 04:58:33.068974 libvsmbr-20240505/PKG-INFO
```

### Comparing `libvsmbr-20240302/libfdata/libfdata_error.h` & `libvsmbr-20240505/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_area.c` & `libvsmbr-20240505/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_stream.h` & `libvsmbr-20240505/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_cache.h` & `libvsmbr-20240505/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_range_list.c` & `libvsmbr-20240505/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_mapped_range.c` & `libvsmbr-20240505/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_libcerror.h` & `libvsmbr-20240505/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_definitions.h` & `libvsmbr-20240505/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libvsmbr-20240302/libfdata/libfdata_list.c` & `libvsmbr-20240505/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_libcdata.h` & `libvsmbr-20240505/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_list.h` & `libvsmbr-20240505/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_list_element.h` & `libvsmbr-20240505/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/Makefile.am` & `libvsmbr-20240505/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
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
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libvsmbr-20240302/libfdata/libfdata_libcnotify.h` & `libvsmbr-20240505/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_extern.h` & `libvsmbr-20240505/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_notify.c` & `libvsmbr-20240505/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_cache.c` & `libvsmbr-20240505/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_stream.c` & `libvsmbr-20240505/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_unused.h` & `libvsmbr-20240505/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_range.h` & `libvsmbr-20240505/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_area.h` & `libvsmbr-20240505/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_error.c` & `libvsmbr-20240505/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_support.h` & `libvsmbr-20240505/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_range.c` & `libvsmbr-20240505/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_mapped_range.h` & `libvsmbr-20240505/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_support.c` & `libvsmbr-20240505/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_list_element.c` & `libvsmbr-20240505/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_segments_array.c` & `libvsmbr-20240505/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_types.h` & `libvsmbr-20240505/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_notify.h` & `libvsmbr-20240505/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_range_list.h` & `libvsmbr-20240505/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_segments_array.h` & `libvsmbr-20240505/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/Makefile.in` & `libvsmbr-20240505/libfdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -506,16 +506,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -539,15 +539,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -759,24 +760,39 @@
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
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -872,17 +888,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsmbr-20240302/libfdata/libfdata_vector.c` & `libvsmbr-20240505/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_libfcache.h` & `libvsmbr-20240505/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfdata/libfdata_vector.h` & `libvsmbr-20240505/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/vsmbr_partition_entry.h` & `libvsmbr-20240505/libvsmbr/vsmbr_partition_entry.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_libcdata.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_sector_data.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_sector_data.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_support.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_libfcache.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_libcnotify.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_sector_data.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_sector_data.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_libcerror.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_extern.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_debug.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_debug.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_definitions.h.in` & `libvsmbr-20240505/libvsmbr/libvsmbr_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_partition_values.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_partition_values.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_libcthreads.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_definitions.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBVSMBR )
 #include <libvsmbr/definitions.h>
 
 /* The definitions in <libvsmbr/definitions.h> are copied here
  * for local use of libvsmbr
  */
 #else
-#define LIBVSMBR_VERSION			20240302
+#define LIBVSMBR_VERSION			20240505
 
 /* The libvsmbr version string
  */
-#define LIBVSMBR_VERSION_STRING			"20240302"
+#define LIBVSMBR_VERSION_STRING			"20240505"
 
 /* The endian definitions
  */
 #define LIBVSMBR_ENDIAN_BIG			_BYTE_STREAM_ENDIAN_BIG
 #define LIBVSMBR_ENDIAN_LITTLE			_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The access flags definitions
```

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_chs_address.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_chs_address.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_notify.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_notify.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/Makefile.am` & `libvsmbr-20240505/libvsmbr/Makefile.am`

 * *Files 6% similar despite different names*

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
@@ -67,21 +67,19 @@
 libvsmbr_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libvsmbr_definitions.h.in \
 	libvsmbr.rc \
 	libvsmbr.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvsmbr_definitions.h \
+	libvsmbr.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libvsmbr_definitions.h
-	-rm -f libvsmbr.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvsmbr ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvsmbr_la_SOURCES)
```

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_boot_record.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_boot_record.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_libfdata.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_libfdata.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_volume.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_volume.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_section_values.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_section_values.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr.rc.in` & `libvsmbr-20240505/libvsmbr/libvsmbr.rc.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr.rc` & `libvsmbr-20240505/libvsmbr/libvsmbr.rc`

 * *Files 23% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Master Boot Record (MBR) volume system format\0"
-      VALUE "FileVersion",		"20240302" "\0"
+      VALUE "FileVersion",		"20240505" "\0"
       VALUE "InternalName",		"libvsmbr.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libvsmbr.dll\0"
       VALUE "ProductName",		"libvsmbr\0"
-      VALUE "ProductVersion",		"20240302" "\0"
+      VALUE "ProductVersion",		"20240505" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libvsmbr/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_section_values.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_section_values.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_error.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_io_handle.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_partition_entry.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_partition_entry.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_libbfio.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_partition_type.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_partition_type.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_debug.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_debug.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_partition_values.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_partition_values.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_volume.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_volume.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_partition_type.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_partition_type.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_chs_address.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_chs_address.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_types.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr.c` & `libvsmbr-20240505/libvsmbr/libvsmbr.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/vsmbr_boot_record.h` & `libvsmbr-20240505/libvsmbr/vsmbr_boot_record.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_partition_entry.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_partition_entry.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_notify.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_notify.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_support.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_unused.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_io_handle.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/Makefile.in` & `libvsmbr-20240505/libvsmbr/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -522,16 +522,16 @@
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
@@ -592,15 +592,18 @@
 
 libvsmbr_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libvsmbr_definitions.h.in \
 	libvsmbr.rc \
 	libvsmbr.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvsmbr_definitions.h \
+	libvsmbr.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -845,24 +848,41 @@
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
+		-rm -f ./$(DEPDIR)/libvsmbr.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_boot_record.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_chs_address.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_debug.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_error.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_notify.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_partition.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_partition_entry.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_partition_type.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_partition_values.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_section_values.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_sector_data.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_support.Plo
+	-rm -f ./$(DEPDIR)/libvsmbr_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -960,19 +980,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvsmbr_definitions.h
-	-rm -f libvsmbr.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvsmbr ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvsmbr_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_libclocale.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_error.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_partition.c` & `libvsmbr-20240505/libvsmbr/libvsmbr_partition.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_partition.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_partition.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr/libvsmbr_boot_record.h` & `libvsmbr-20240505/libvsmbr/libvsmbr_boot_record.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr.spec.in` & `libvsmbr-20240505/libvsmbr.spec.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/COPYING` & `libvsmbr-20240505/COPYING`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/install-sh` & `libvsmbr-20240505/install-sh`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/depcomp` & `libvsmbr-20240505/depcomp`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/libcfile.m4` & `libvsmbr-20240505/m4/libcfile.m4`

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

### Comparing `libvsmbr-20240302/m4/tests.m4` & `libvsmbr-20240505/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/libcpath.m4` & `libvsmbr-20240505/m4/libcpath.m4`

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

### Comparing `libvsmbr-20240302/m4/lib-prefix.m4` & `libvsmbr-20240505/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/progtest.m4` & `libvsmbr-20240505/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/libuna.m4` & `libvsmbr-20240505/m4/libuna.m4`

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

### Comparing `libvsmbr-20240302/m4/gettext.m4` & `libvsmbr-20240505/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/lib-ld.m4` & `libvsmbr-20240505/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/libclocale.m4` & `libvsmbr-20240505/m4/libclocale.m4`

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

### Comparing `libvsmbr-20240302/m4/libcdata.m4` & `libvsmbr-20240505/m4/libcdata.m4`

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

### Comparing `libvsmbr-20240302/m4/libcsplit.m4` & `libvsmbr-20240505/m4/libcsplit.m4`

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

### Comparing `libvsmbr-20240302/m4/common.m4` & `libvsmbr-20240505/m4/common.m4`

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

### Comparing `libvsmbr-20240302/m4/libcthreads.m4` & `libvsmbr-20240505/m4/libcthreads.m4`

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

### Comparing `libvsmbr-20240302/m4/ltversion.m4` & `libvsmbr-20240505/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/ltsugar.m4` & `libvsmbr-20240505/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/libfdata.m4` & `libvsmbr-20240505/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libvsmbr-20240302/m4/host-cpu-c-abi.m4` & `libvsmbr-20240505/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/libtool.m4` & `libvsmbr-20240505/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/po.m4` & `libvsmbr-20240505/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/libcerror.m4` & `libvsmbr-20240505/m4/libcerror.m4`

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

### Comparing `libvsmbr-20240302/m4/libcnotify.m4` & `libvsmbr-20240505/m4/libcnotify.m4`

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

### Comparing `libvsmbr-20240302/m4/libbfio.m4` & `libvsmbr-20240505/m4/libbfio.m4`

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

### Comparing `libvsmbr-20240302/m4/intlmacosx.m4` & `libvsmbr-20240505/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/lt~obsolete.m4` & `libvsmbr-20240505/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/lib-link.m4` & `libvsmbr-20240505/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/iconv.m4` & `libvsmbr-20240505/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/ltoptions.m4` & `libvsmbr-20240505/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/nls.m4` & `libvsmbr-20240505/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/python.m4` & `libvsmbr-20240505/m4/python.m4`

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

### Comparing `libvsmbr-20240302/m4/types.m4` & `libvsmbr-20240505/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/m4/libfcache.m4` & `libvsmbr-20240505/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libvsmbr-20240302/m4/pthread.m4` & `libvsmbr-20240505/m4/pthread.m4`

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

### Comparing `libvsmbr-20240302/include/libvsmbr/definitions.h.in` & `libvsmbr-20240505/include/libvsmbr/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/libvsmbr/definitions.h` & `libvsmbr-20240505/include/libvsmbr/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBVSMBR_DEFINITIONS_H )
 #define _LIBVSMBR_DEFINITIONS_H
 
 #include <libvsmbr/types.h>
 
-#define LIBVSMBR_VERSION		20240302
+#define LIBVSMBR_VERSION		20240505
 
 /* The version string
  */
-#define LIBVSMBR_VERSION_STRING		"20240302"
+#define LIBVSMBR_VERSION_STRING		"20240505"
 
 /* The byte order definitions
  */
 enum LIBVSMBR_ENDIAN
 {
 	LIBVSMBR_ENDIAN_BIG		= (int) 'b',
 	LIBVSMBR_ENDIAN_LITTLE		= (int) 'l',
```

### Comparing `libvsmbr-20240302/include/libvsmbr/types.h.in` & `libvsmbr-20240505/include/libvsmbr/types.h.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/libvsmbr/types.h` & `libvsmbr-20240505/include/libvsmbr/types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/libvsmbr/features.h.in` & `libvsmbr-20240505/include/libvsmbr/features.h.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/libvsmbr/error.h` & `libvsmbr-20240505/include/libvsmbr/error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/libvsmbr/extern.h` & `libvsmbr-20240505/include/libvsmbr/extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/libvsmbr/features.h` & `libvsmbr-20240505/include/libvsmbr/features.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/libvsmbr/codepage.h` & `libvsmbr-20240505/include/libvsmbr/codepage.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/libvsmbr.h.in` & `libvsmbr-20240505/include/libvsmbr.h.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/libvsmbr.h` & `libvsmbr-20240505/include/libvsmbr.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/include/Makefile.in` & `libvsmbr-20240505/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -488,15 +488,20 @@
 
 EXTRA_DIST = \
 	libvsmbr.h.in \
 	libvsmbr/definitions.h.in \
 	libvsmbr/features.h.in \
 	libvsmbr/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvsmbr.h \
+	libvsmbr/definitions.h \
+	libvsmbr/features.h \
+	libvsmbr/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -693,23 +698,25 @@
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
@@ -791,17 +798,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvsmbr.h
-	-rm -f libvsmbr/definitions.h
-	-rm -f libvsmbr/features.h
-	-rm -f libvsmbr/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsmbr-20240302/common/config_borlandc.h` & `libvsmbr-20240505/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/file_stream.h` & `libvsmbr-20240505/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/memory.h` & `libvsmbr-20240505/common/memory.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/byte_stream.h` & `libvsmbr-20240505/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/common.h` & `libvsmbr-20240505/common/common.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/config_winapi.h` & `libvsmbr-20240505/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/system_string.h` & `libvsmbr-20240505/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/types.h.in` & `libvsmbr-20240505/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/types.h` & `libvsmbr-20240505/common/types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/config.h.in` & `libvsmbr-20240505/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/config.h` & `libvsmbr-20240505/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -505,24 +505,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libvsmbr"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libvsmbr 20240302"
+#define PACKAGE_STRING "libvsmbr 20240505"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libvsmbr"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240302"
+#define PACKAGE_VERSION "20240505"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -543,15 +543,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240302"
+#define VERSION "20240505"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libvsmbr-20240302/common/wide_string.h` & `libvsmbr-20240505/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/narrow_string.h` & `libvsmbr-20240505/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/config_msc.h` & `libvsmbr-20240505/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/common/Makefile.in` & `libvsmbr-20240505/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,17 @@
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
@@ -457,15 +459,18 @@
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
@@ -633,23 +638,25 @@
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
@@ -729,15 +736,10 @@
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

### Comparing `libvsmbr-20240302/libclocale/libclocale_wide_string.c` & `libvsmbr-20240505/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/libclocale_support.h` & `libvsmbr-20240505/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/Makefile.am` & `libvsmbr-20240505/libclocale/Makefile.am`

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

### Comparing `libvsmbr-20240302/libclocale/libclocale_definitions.h` & `libvsmbr-20240505/libclocale/libclocale_definitions.h`

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

### Comparing `libvsmbr-20240302/libclocale/libclocale_unused.h` & `libvsmbr-20240505/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/libclocale_libcerror.h` & `libvsmbr-20240505/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/libclocale_locale.h` & `libvsmbr-20240505/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/libclocale_support.c` & `libvsmbr-20240505/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/libclocale_codepage.c` & `libvsmbr-20240505/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/libclocale_locale.c` & `libvsmbr-20240505/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/Makefile.in` & `libvsmbr-20240505/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -487,30 +487,31 @@
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
@@ -713,24 +714,30 @@
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
 
@@ -817,17 +824,14 @@
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

### Comparing `libvsmbr-20240302/libclocale/libclocale_extern.h` & `libvsmbr-20240505/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/libclocale_wide_string.h` & `libvsmbr-20240505/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libclocale/libclocale_codepage.h` & `libvsmbr-20240505/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_libcdata.h` & `libvsmbr-20240505/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_types.h` & `libvsmbr-20240505/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_cache_value.c` & `libvsmbr-20240505/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_unused.h` & `libvsmbr-20240505/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/Makefile.am` & `libvsmbr-20240505/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
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
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libvsmbr-20240302/libfcache/libfcache_support.h` & `libvsmbr-20240505/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_error.h` & `libvsmbr-20240505/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_support.c` & `libvsmbr-20240505/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_cache.h` & `libvsmbr-20240505/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_error.c` & `libvsmbr-20240505/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_libcerror.h` & `libvsmbr-20240505/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_date_time.c` & `libvsmbr-20240505/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_extern.h` & `libvsmbr-20240505/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_cache_value.h` & `libvsmbr-20240505/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/Makefile.in` & `libvsmbr-20240505/libfcache/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -489,16 +489,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -510,15 +510,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -722,24 +723,31 @@
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
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -827,17 +835,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsmbr-20240302/libfcache/libfcache_date_time.h` & `libvsmbr-20240505/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libfcache/libfcache_definitions.h` & `libvsmbr-20240505/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libvsmbr-20240302/libfcache/libfcache_cache.c` & `libvsmbr-20240505/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/Makefile.am` & `libvsmbr-20240505/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 DPKG_FILES = \
 	dpkg/changelog \
 	dpkg/changelog.in \
 	dpkg/compat \
 	dpkg/control \
 	dpkg/copyright \
 	dpkg/rules \
-	dpkg/libvsmbr-dev.install \
 	dpkg/libvsmbr.install \
+	dpkg/libvsmbr-dev.install \
+	dpkg/libvsmbr-python3.install \
+	dpkg/libvsmbr-tools.install \
 	dpkg/source/format
 
 GETTEXT_FILES = \
 	config.rpath \
 	po/Makevars.in
 
 PKGCONFIG_FILES = \
@@ -55,16 +57,23 @@
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
+	libvsmbr.pc \
+	libvsmbr.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libvsmbr.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -85,19 +94,7 @@
 	(cd $(srcdir)/libcpath && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvsmbr && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvsmbr.pc
-	-rm -f libvsmbr.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libvsmbr-20240302/libbfio/libbfio_file_range.h` & `libvsmbr-20240505/libbfio/libbfio_file_range.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_file_range_io_handle.c` & `libvsmbr-20240505/libbfio/libbfio_file_range_io_handle.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_support.c` & `libvsmbr-20240505/libbfio/libbfio_support.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_libcpath.h` & `libvsmbr-20240505/libbfio/libbfio_libcpath.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_error.h` & `libvsmbr-20240505/libbfio/libbfio_error.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_libclocale.h` & `libvsmbr-20240505/libbfio/libbfio_libclocale.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_error.c` & `libvsmbr-20240505/libbfio/libbfio_error.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_libuna.h` & `libvsmbr-20240505/libbfio/libbfio_libuna.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_file_io_handle.h` & `libvsmbr-20240505/libbfio/libbfio_file_io_handle.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_file_pool.h` & `libvsmbr-20240505/libbfio/libbfio_file_pool.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_file_range.c` & `libvsmbr-20240505/libbfio/libbfio_file_range.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_types.h` & `libvsmbr-20240505/libbfio/libbfio_types.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_unused.h` & `libvsmbr-20240505/libbfio/libbfio_unused.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_libcdata.h` & `libvsmbr-20240505/libbfio/libbfio_libcdata.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_file.h` & `libvsmbr-20240505/libbfio/libbfio_file.h`

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

### Comparing `libvsmbr-20240302/libbfio/Makefile.am` & `libvsmbr-20240505/libbfio/Makefile.am`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_libcfile.h` & `libvsmbr-20240505/libbfio/libbfio_libcfile.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_definitions.h` & `libvsmbr-20240505/libbfio/libbfio_definitions.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_codepage.h` & `libvsmbr-20240505/libbfio/libbfio_codepage.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_file_io_handle.c` & `libvsmbr-20240505/libbfio/libbfio_file_io_handle.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_support.h` & `libvsmbr-20240505/libbfio/libbfio_support.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_memory_range.h` & `libvsmbr-20240505/libbfio/libbfio_memory_range.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_file_pool.c` & `libvsmbr-20240505/libbfio/libbfio_file_pool.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_file_range_io_handle.h` & `libvsmbr-20240505/libbfio/libbfio_file_range_io_handle.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_libcthreads.h` & `libvsmbr-20240505/libbfio/libbfio_libcthreads.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_system_string.h` & `libvsmbr-20240505/libbfio/libbfio_system_string.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_memory_range_io_handle.c` & `libvsmbr-20240505/libbfio/libbfio_memory_range_io_handle.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_handle.c` & `libvsmbr-20240505/libbfio/libbfio_handle.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_file.c` & `libvsmbr-20240505/libbfio/libbfio_file.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_handle.h` & `libvsmbr-20240505/libbfio/libbfio_handle.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_memory_range.c` & `libvsmbr-20240505/libbfio/libbfio_memory_range.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_pool.c` & `libvsmbr-20240505/libbfio/libbfio_pool.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_libcerror.h` & `libvsmbr-20240505/libbfio/libbfio_libcerror.h`

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

### Comparing `libvsmbr-20240302/libbfio/Makefile.in` & `libvsmbr-20240505/libbfio/Makefile.in`

 * *Files 7% similar despite different names*

```diff
@@ -507,16 +507,16 @@
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
@@ -547,15 +547,16 @@
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
@@ -766,24 +767,38 @@
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
 
@@ -852,14 +867,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -870,23 +887,22 @@
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

### Comparing `libvsmbr-20240302/libbfio/libbfio_system_string.c` & `libvsmbr-20240505/libbfio/libbfio_system_string.c`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_memory_range_io_handle.h` & `libvsmbr-20240505/libbfio/libbfio_memory_range_io_handle.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_extern.h` & `libvsmbr-20240505/libbfio/libbfio_extern.h`

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

### Comparing `libvsmbr-20240302/libbfio/libbfio_pool.h` & `libvsmbr-20240505/libbfio/libbfio_pool.h`

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

### Comparing `libvsmbr-20240302/config.guess` & `libvsmbr-20240505/config.guess`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/dpkg/copyright` & `libvsmbr-20240505/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/dpkg/control` & `libvsmbr-20240505/dpkg/control`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/dpkg/rules` & `libvsmbr-20240505/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/COPYING.LESSER` & `libvsmbr-20240505/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/configure` & `libvsmbr-20240505/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libvsmbr 20240302.
+# Generated by GNU Autoconf 2.71 for libvsmbr 20240505.
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
 PACKAGE_NAME='libvsmbr'
 PACKAGE_TARNAME='libvsmbr'
-PACKAGE_VERSION='20240302'
-PACKAGE_STRING='libvsmbr 20240302'
+PACKAGE_VERSION='20240505'
+PACKAGE_STRING='libvsmbr 20240505'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libvsmbr.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1611,15 +1611,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libvsmbr 20240302 to adapt to many kinds of systems.
+\`configure' configures libvsmbr 20240505 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1682,15 +1682,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libvsmbr 20240302:";;
+     short | recursive ) echo "Configuration of libvsmbr 20240505:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1912,15 +1912,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libvsmbr configure 20240302
+libvsmbr configure 20240505
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2633,15 +2633,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libvsmbr $as_me 20240302, which was
+It was created by libvsmbr $as_me 20240505, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4122,15 +4122,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libvsmbr'
- VERSION='20240302'
+ VERSION='20240505'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23717,15 +23717,15 @@
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
@@ -24216,15 +24216,16 @@
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
@@ -24366,15 +24367,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24468,15 +24469,15 @@
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
@@ -26108,15 +26109,15 @@
 
 
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
@@ -26170,47 +26171,52 @@
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
@@ -26244,15 +26250,15 @@
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
@@ -26286,15 +26292,15 @@
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
@@ -26329,15 +26335,15 @@
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
@@ -26371,15 +26377,15 @@
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
@@ -26413,15 +26419,15 @@
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
@@ -26455,15 +26461,15 @@
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
@@ -26497,15 +26503,15 @@
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
@@ -26540,15 +26546,15 @@
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
@@ -26582,15 +26588,15 @@
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
@@ -26624,15 +26630,15 @@
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
@@ -26666,15 +26672,15 @@
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
@@ -26708,15 +26714,15 @@
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
@@ -26751,15 +26757,15 @@
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
@@ -26793,15 +26799,15 @@
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
@@ -26835,15 +26841,15 @@
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
@@ -26877,15 +26883,15 @@
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
@@ -26919,15 +26925,15 @@
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
@@ -26962,67 +26968,76 @@
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
 
@@ -27110,15 +27125,15 @@
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
@@ -30889,15 +30904,16 @@
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
@@ -30922,15 +30938,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31000,15 +31016,15 @@
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
@@ -31555,15 +31571,16 @@
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
@@ -31719,15 +31736,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31797,15 +31814,15 @@
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
@@ -32255,15 +32272,16 @@
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
@@ -32318,15 +32336,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32396,15 +32414,15 @@
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
@@ -33119,15 +33137,16 @@
 
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
@@ -33152,15 +33171,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33230,15 +33249,15 @@
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
@@ -40440,15 +40459,16 @@
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
@@ -40473,15 +40493,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40551,15 +40571,15 @@
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
@@ -41740,15 +41760,16 @@
 
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
@@ -42062,15 +42083,15 @@
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
@@ -42140,15 +42161,15 @@
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
@@ -42945,15 +42966,16 @@
 
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
@@ -43143,15 +43165,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43221,15 +43243,15 @@
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
@@ -45339,15 +45361,16 @@
 
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
@@ -45372,15 +45395,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45450,15 +45473,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46370,15 +46393,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46471,15 +46495,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46549,15 +46573,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49837,15 +49861,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49870,15 +49895,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50189,16 +50214,20 @@
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
 
@@ -51197,15 +51226,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libvsmbr $as_me 20240302, which was
+This file was extended by libvsmbr $as_me 20240505, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -51265,15 +51294,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libvsmbr config.status 20240302
+libvsmbr config.status 20240505
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libvsmbr-20240302/compile` & `libvsmbr-20240505/compile`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/missing` & `libvsmbr-20240505/missing`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libfdata/libfdata.vcproj` & `libvsmbr-20240505/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libvsmbr/libvsmbr.vcproj` & `libvsmbr-20240505/msvscpp/libvsmbr/libvsmbr.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_tools_signal/vsmbr_test_tools_signal.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_tools_signal/vsmbr_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_notify/vsmbr_test_notify.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_notify/vsmbr_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libclocale/libclocale.vcproj` & `libvsmbr-20240505/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libfcache/libfcache.vcproj` & `libvsmbr-20240505/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/Makefile.am` & `libvsmbr-20240505/msvscpp/Makefile.am`

 * *Files 24% similar despite different names*

```diff
@@ -31,13 +31,11 @@
 	vsmbr_test_volume/vsmbr_test_volume.vcproj \
 	vsmbrinfo/vsmbrinfo.vcproj \
 	libvsmbr.sln
 
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

### Comparing `libvsmbr-20240302/msvscpp/libbfio/libbfio.vcproj` & `libvsmbr-20240505/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_error/vsmbr_test_error.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_error/vsmbr_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_tools_info_handle/vsmbr_test_tools_info_handle.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_tools_info_handle/vsmbr_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_partition_type/vsmbr_test_partition_type.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_partition_type/vsmbr_test_partition_type.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_partition_entry/vsmbr_test_partition_entry.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_partition_entry/vsmbr_test_partition_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_partition_values/vsmbr_test_partition_values.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_partition_values/vsmbr_test_partition_values.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_section_values/vsmbr_test_section_values.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_section_values/vsmbr_test_section_values.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libcfile/libcfile.vcproj` & `libvsmbr-20240505/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libcdata/libcdata.vcproj` & `libvsmbr-20240505/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_tools_output/vsmbr_test_tools_output.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_tools_output/vsmbr_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_io_handle/vsmbr_test_io_handle.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_io_handle/vsmbr_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbrinfo/vsmbrinfo.vcproj` & `libvsmbr-20240505/msvscpp/vsmbrinfo/vsmbrinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/pyvsmbr/pyvsmbr.vcproj` & `libvsmbr-20240505/msvscpp/pyvsmbr/pyvsmbr.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libcthreads/libcthreads.vcproj` & `libvsmbr-20240505/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_chs_address/vsmbr_test_chs_address.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_chs_address/vsmbr_test_chs_address.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libcpath/libcpath.vcproj` & `libvsmbr-20240505/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_boot_record/vsmbr_test_boot_record.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_boot_record/vsmbr_test_boot_record.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_partition/vsmbr_test_partition.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_partition/vsmbr_test_partition.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_support/vsmbr_test_support.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_support/vsmbr_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_sector_data/vsmbr_test_sector_data.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_sector_data/vsmbr_test_sector_data.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/vsmbr_test_volume/vsmbr_test_volume.vcproj` & `libvsmbr-20240505/msvscpp/vsmbr_test_volume/vsmbr_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libcsplit/libcsplit.vcproj` & `libvsmbr-20240505/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libuna/libuna.vcproj` & `libvsmbr-20240505/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/Makefile.in` & `libvsmbr-20240505/msvscpp/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -460,15 +460,16 @@
 	vsmbr_test_volume/vsmbr_test_volume.vcproj \
 	vsmbrinfo/vsmbrinfo.vcproj \
 	libvsmbr.sln
 
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
@@ -572,23 +573,25 @@
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
@@ -667,13 +670,10 @@
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

### Comparing `libvsmbr-20240302/msvscpp/libcnotify/libcnotify.vcproj` & `libvsmbr-20240505/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libcerror/libcerror.vcproj` & `libvsmbr-20240505/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/msvscpp/libvsmbr.sln` & `libvsmbr-20240505/msvscpp/libvsmbr.sln`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr.pc.in` & `libvsmbr-20240505/libvsmbr.pc.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_extern.h` & `libvsmbr-20240505/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_support.h` & `libvsmbr-20240505/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_unused.h` & `libvsmbr-20240505/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_notify.h` & `libvsmbr-20240505/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_support.c` & `libvsmbr-20240505/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_types.h` & `libvsmbr-20240505/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/Makefile.am` & `libvsmbr-20240505/libcfile/Makefile.am`

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

### Comparing `libvsmbr-20240302/libcfile/libcfile_notify.c` & `libvsmbr-20240505/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_system_string.h` & `libvsmbr-20240505/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_file.h` & `libvsmbr-20240505/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_libcnotify.h` & `libvsmbr-20240505/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_system_string.c` & `libvsmbr-20240505/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_error.h` & `libvsmbr-20240505/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_libcerror.h` & `libvsmbr-20240505/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_file.c` & `libvsmbr-20240505/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_libclocale.h` & `libvsmbr-20240505/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_winapi.h` & `libvsmbr-20240505/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/Makefile.in` & `libvsmbr-20240505/libcfile/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -489,16 +489,16 @@
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
@@ -513,15 +513,16 @@
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
@@ -726,24 +727,32 @@
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
 
@@ -832,17 +841,14 @@
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

### Comparing `libvsmbr-20240302/libcfile/libcfile_error.c` & `libvsmbr-20240505/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_libuna.h` & `libvsmbr-20240505/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_winapi.c` & `libvsmbr-20240505/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcfile/libcfile_definitions.h` & `libvsmbr-20240505/libcfile/libcfile_definitions.h`

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

### Comparing `libvsmbr-20240302/INSTALL` & `libvsmbr-20240505/INSTALL`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libvsmbr.spec` & `libvsmbr-20240505/libvsmbr.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libvsmbr
-Version: 20240302
+Version: 20240505
 Release: 1
 Summary: Library to access the Master Boot Record (MBR) volume system format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libvsmbr
             
@@ -90,10 +90,10 @@
 %files -n libvsmbr-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sat Mar  2 2024 Joachim Metz <joachim.metz@gmail.com> 20240302-1
+* Sun May  5 2024 Joachim Metz <joachim.metz@gmail.com> 20240505-1
 - Auto-generated
```

### Comparing `libvsmbr-20240302/libcdata/libcdata_list_element.h` & `libvsmbr-20240505/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_array.h` & `libvsmbr-20240505/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_definitions.h` & `libvsmbr-20240505/libcdata/libcdata_definitions.h`

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

### Comparing `libvsmbr-20240302/libcdata/libcdata_libcerror.h` & `libvsmbr-20240505/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_unused.h` & `libvsmbr-20240505/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_btree.h` & `libvsmbr-20240505/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_btree.c` & `libvsmbr-20240505/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_support.c` & `libvsmbr-20240505/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_list.c` & `libvsmbr-20240505/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_extern.h` & `libvsmbr-20240505/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_list.h` & `libvsmbr-20240505/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_btree_values_list.h` & `libvsmbr-20240505/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/Makefile.am` & `libvsmbr-20240505/libcdata/Makefile.am`

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

### Comparing `libvsmbr-20240302/libcdata/libcdata_btree_node.h` & `libvsmbr-20240505/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_range_list_value.h` & `libvsmbr-20240505/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_range_list.h` & `libvsmbr-20240505/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_range_list.c` & `libvsmbr-20240505/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_array.c` & `libvsmbr-20240505/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_list_element.c` & `libvsmbr-20240505/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_libcthreads.h` & `libvsmbr-20240505/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_tree_node.h` & `libvsmbr-20240505/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_error.h` & `libvsmbr-20240505/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_types.h` & `libvsmbr-20240505/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_btree_node.c` & `libvsmbr-20240505/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_tree_node.c` & `libvsmbr-20240505/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_support.h` & `libvsmbr-20240505/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/Makefile.in` & `libvsmbr-20240505/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -503,16 +503,16 @@
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
@@ -529,15 +529,16 @@
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
@@ -747,24 +748,37 @@
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
 
@@ -858,17 +872,14 @@
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

### Comparing `libvsmbr-20240302/libcdata/libcdata_range_list_value.c` & `libvsmbr-20240505/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_btree_values_list.c` & `libvsmbr-20240505/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcdata/libcdata_error.c` & `libvsmbr-20240505/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/info_handle.h` & `libvsmbr-20240505/vsmbrtools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_libbfio.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_libuna.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/Makefile.am` & `libvsmbr-20240505/vsmbrtools/Makefile.am`

 * *Files 16% similar despite different names*

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
@@ -36,17 +36,15 @@
 	@LIBUNA_LIBADD@ \
 	../libvsmbr/libvsmbr.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
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
 	@echo "Running splint on vsmbrinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vsmbrinfo_SOURCES)
```

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_getopt.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_getopt.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/info_handle.c` & `libvsmbr-20240505/vsmbrtools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_i18n.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_i18n.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_getopt.c` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_getopt.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_output.c` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_output.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_libclocale.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrinfo.c` & `libvsmbr-20240505/vsmbrtools/vsmbrinfo.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_libcerror.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/Makefile.in` & `libvsmbr-20240505/vsmbrtools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -479,16 +479,16 @@
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
@@ -516,15 +516,16 @@
 	@LIBUNA_LIBADD@ \
 	../libvsmbr/libvsmbr.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
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
@@ -770,23 +771,30 @@
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
+		-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/vsmbrinfo.Po
+	-rm -f ./$(DEPDIR)/vsmbrtools_getopt.Po
+	-rm -f ./$(DEPDIR)/vsmbrtools_output.Po
+	-rm -f ./$(DEPDIR)/vsmbrtools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -874,17 +882,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on vsmbrinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vsmbrinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_output.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_output.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_signal.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_signal.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_libvsmbr.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_libvsmbr.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_libcnotify.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_signal.c` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_signal.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/vsmbrtools/vsmbrtools_unused.h` & `libvsmbr-20240505/vsmbrtools/vsmbrtools_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/config.sub` & `libvsmbr-20240505/config.sub`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/setup.py` & `libvsmbr-20240505/setup.py`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/acinclude.m4` & `libvsmbr-20240505/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_libcerror.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_error.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_integer.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_integer.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_volume.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_volume.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_partitions.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_partitions.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_volume.c` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_volume.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_libclocale.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/Makefile.am` & `libvsmbr-20240505/pyvsmbr/Makefile.am`

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
@@ -41,13 +41,11 @@
 	@LIBBFIO_LIBADD@
 
 pyvsmbr_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyvsmbr_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_libbfio.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr.c` & `libvsmbr-20240505/pyvsmbr/pyvsmbr.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_libvsmbr.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_libvsmbr.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_partition.c` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_partition.c`

 * *Files 1% similar despite different names*

```diff
@@ -49,22 +49,22 @@
 	  "get_volume_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the volume offset." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyvsmbr_partition_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyvsmbr_partition_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyvsmbr_partition_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -77,15 +77,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset." },
 
 	{ "read",
 	  (PyCFunction) pyvsmbr_partition_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "seek",
 	  (PyCFunction) pyvsmbr_partition_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_partitions.c` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_partitions.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_python.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_python.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_error.c` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_unused.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_file_object_io_handle.c` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_integer.c` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_integer.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_file_object_io_handle.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/pyvsmbr/Makefile.in` & `libvsmbr-20240505/pyvsmbr/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -524,16 +524,16 @@
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
@@ -565,15 +565,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyvsmbr_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyvsmbr_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -855,24 +856,33 @@
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
+		-rm -f ./$(DEPDIR)/pyvsmbr_la-pyvsmbr.Plo
+	-rm -f ./$(DEPDIR)/pyvsmbr_la-pyvsmbr_error.Plo
+	-rm -f ./$(DEPDIR)/pyvsmbr_la-pyvsmbr_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyvsmbr_la-pyvsmbr_integer.Plo
+	-rm -f ./$(DEPDIR)/pyvsmbr_la-pyvsmbr_partition.Plo
+	-rm -f ./$(DEPDIR)/pyvsmbr_la-pyvsmbr_partitions.Plo
+	-rm -f ./$(DEPDIR)/pyvsmbr_la-pyvsmbr_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -963,13 +973,10 @@
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

### Comparing `libvsmbr-20240302/pyvsmbr/pyvsmbr_partition.h` & `libvsmbr-20240505/pyvsmbr/pyvsmbr_partition.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/config.rpath` & `libvsmbr-20240505/config.rpath`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_thread.h` & `libvsmbr-20240505/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_read_write_lock.h` & `libvsmbr-20240505/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_thread.c` & `libvsmbr-20240505/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_thread_pool.h` & `libvsmbr-20240505/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_support.h` & `libvsmbr-20240505/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_lock.h` & `libvsmbr-20240505/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_unused.h` & `libvsmbr-20240505/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_lock.c` & `libvsmbr-20240505/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_condition.h` & `libvsmbr-20240505/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_repeating_thread.h` & `libvsmbr-20240505/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/Makefile.am` & `libvsmbr-20240505/libcthreads/Makefile.am`

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

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_support.c` & `libvsmbr-20240505/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_mutex.c` & `libvsmbr-20240505/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_queue.c` & `libvsmbr-20240505/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_mutex.h` & `libvsmbr-20240505/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_types.h` & `libvsmbr-20240505/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_thread_attributes.h` & `libvsmbr-20240505/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_condition.c` & `libvsmbr-20240505/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_error.c` & `libvsmbr-20240505/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_read_write_lock.c` & `libvsmbr-20240505/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_libcerror.h` & `libvsmbr-20240505/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_definitions.h` & `libvsmbr-20240505/libcthreads/libcthreads_definitions.h`

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

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_thread_pool.c` & `libvsmbr-20240505/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_error.h` & `libvsmbr-20240505/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_thread_attributes.c` & `libvsmbr-20240505/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_extern.h` & `libvsmbr-20240505/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_repeating_thread.c` & `libvsmbr-20240505/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcthreads/Makefile.in` & `libvsmbr-20240505/libcthreads/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -507,16 +507,16 @@
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
@@ -531,15 +531,16 @@
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
@@ -749,24 +750,37 @@
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
 
@@ -860,17 +874,14 @@
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

### Comparing `libvsmbr-20240302/libcthreads/libcthreads_queue.h` & `libvsmbr-20240505/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/test-driver` & `libvsmbr-20240505/test-driver`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_support.c` & `libvsmbr-20240505/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_libcerror.h` & `libvsmbr-20240505/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_definitions.h` & `libvsmbr-20240505/libcpath/libcpath_definitions.h`

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

### Comparing `libvsmbr-20240302/libcpath/Makefile.am` & `libvsmbr-20240505/libcpath/Makefile.am`

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

### Comparing `libvsmbr-20240302/libcpath/libcpath_error.c` & `libvsmbr-20240505/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_extern.h` & `libvsmbr-20240505/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_system_string.h` & `libvsmbr-20240505/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_support.h` & `libvsmbr-20240505/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_libcsplit.h` & `libvsmbr-20240505/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_system_string.c` & `libvsmbr-20240505/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_libclocale.h` & `libvsmbr-20240505/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_error.h` & `libvsmbr-20240505/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/Makefile.in` & `libvsmbr-20240505/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -483,16 +483,16 @@
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
@@ -504,15 +504,16 @@
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
@@ -715,24 +716,30 @@
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
 
@@ -819,17 +826,14 @@
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

### Comparing `libvsmbr-20240302/libcpath/libcpath_libuna.h` & `libvsmbr-20240505/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_unused.h` & `libvsmbr-20240505/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_path.c` & `libvsmbr-20240505/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcpath/libcpath_path.h` & `libvsmbr-20240505/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/manuals/vsmbrinfo.1` & `libvsmbr-20240505/manuals/vsmbrinfo.1`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/manuals/libvsmbr.3` & `libvsmbr-20240505/manuals/libvsmbr.3`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/manuals/Makefile.in` & `libvsmbr-20240505/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -463,15 +463,16 @@
 	libvsmbr.3 \
 	vsmbrinfo.1
 
 EXTRA_DIST = \
 	libvsmbr.3 \
 	vsmbrinfo.1
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -664,23 +665,25 @@
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
@@ -762,13 +765,10 @@
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

### Comparing `libvsmbr-20240302/tests/vsmbr_test_libbfio.h` & `libvsmbr-20240505/tests/vsmbr_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_getopt.h` & `libvsmbr-20240505/tests/vsmbr_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/test_vsmbrinfo.sh` & `libvsmbr-20240505/tests/test_vsmbrinfo.sh`

 * *Files 8% similar despite different names*

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
 
 PROFILES=("vsmbrinfo");
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

### Comparing `libvsmbr-20240302/tests/pyvsmbr_test_support.py` & `libvsmbr-20240505/tests/pyvsmbr_test_support.py`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_memory.h` & `libvsmbr-20240505/tests/vsmbr_test_memory.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_tools_signal.c` & `libvsmbr-20240505/tests/vsmbr_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_error.c` & `libvsmbr-20240505/tests/vsmbr_test_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/test_tools.sh` & `libvsmbr-20240505/tests/test_tools.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
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

### Comparing `libvsmbr-20240302/tests/vsmbr_test_libvsmbr.h` & `libvsmbr-20240505/tests/vsmbr_test_libvsmbr.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_unused.h` & `libvsmbr-20240505/tests/vsmbr_test_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_io_handle.c` & `libvsmbr-20240505/tests/vsmbr_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_libclocale.h` & `libvsmbr-20240505/tests/vsmbr_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/Makefile.am` & `libvsmbr-20240505/tests/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
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
@@ -308,13 +308,12 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvsmbr/libvsmbr.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@PTHREAD_LIBADD@
 
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

### Comparing `libvsmbr-20240302/tests/vsmbr_test_partition_values.c` & `libvsmbr-20240505/tests/vsmbr_test_partition_values.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_partition.c` & `libvsmbr-20240505/tests/vsmbr_test_partition.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_functions.h` & `libvsmbr-20240505/tests/vsmbr_test_functions.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/pyvsmbr_test_volume.py` & `libvsmbr-20240505/tests/pyvsmbr_test_volume.py`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_rwlock.c` & `libvsmbr-20240505/tests/vsmbr_test_rwlock.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_tools_output.c` & `libvsmbr-20240505/tests/vsmbr_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_partition_type.c` & `libvsmbr-20240505/tests/vsmbr_test_partition_type.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_libcerror.h` & `libvsmbr-20240505/tests/vsmbr_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/test_python_module.sh` & `libvsmbr-20240505/tests/test_python_module.sh`

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
 TEST_FUNCTIONS_WITH_INPUT="partition volume";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libvsmbr";
+PYTHON_MODULE="pyvsmbr";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvsmbr_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvsmbr_test_${TEST_FUNCTION}.py";
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
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyvsmbr");
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

### Comparing `libvsmbr-20240302/tests/vsmbr_test_rwlock.h` & `libvsmbr-20240505/tests/vsmbr_test_rwlock.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_tools_info_handle.c` & `libvsmbr-20240505/tests/vsmbr_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_libcnotify.h` & `libvsmbr-20240505/tests/vsmbr_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_chs_address.c` & `libvsmbr-20240505/tests/vsmbr_test_chs_address.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_boot_record.c` & `libvsmbr-20240505/tests/vsmbr_test_boot_record.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_getopt.c` & `libvsmbr-20240505/tests/vsmbr_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/test_runner.sh` & `libvsmbr-20240505/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_sector_data.c` & `libvsmbr-20240505/tests/vsmbr_test_sector_data.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/pyvsmbr_test_partition.py` & `libvsmbr-20240505/tests/pyvsmbr_test_partition.py`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_notify.c` & `libvsmbr-20240505/tests/vsmbr_test_notify.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_macros.h` & `libvsmbr-20240505/tests/vsmbr_test_macros.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_partition_entry.c` & `libvsmbr-20240505/tests/vsmbr_test_partition_entry.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_libuna.h` & `libvsmbr-20240505/tests/vsmbr_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_volume.c` & `libvsmbr-20240505/tests/vsmbr_test_volume.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/Makefile.in` & `libvsmbr-20240505/tests/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -811,16 +811,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
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
@@ -1102,16 +1102,18 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvsmbr/libvsmbr.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@PTHREAD_LIBADD@
 
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
@@ -1600,24 +1602,49 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../vsmbrtools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../vsmbrtools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../vsmbrtools/$(DEPDIR)/info_handle.Po
+	-rm -f ../vsmbrtools/$(DEPDIR)/vsmbrtools_output.Po
+	-rm -f ../vsmbrtools/$(DEPDIR)/vsmbrtools_signal.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_boot_record.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_chs_address.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_error.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_functions.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_getopt.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_memory.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_notify.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_partition.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_partition_entry.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_partition_type.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_partition_values.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_rwlock.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_section_values.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_sector_data.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_support.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/vsmbr_test_volume.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1723,13 +1750,10 @@
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

### Comparing `libvsmbr-20240302/tests/vsmbr_test_functions.c` & `libvsmbr-20240505/tests/vsmbr_test_functions.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_memory.c` & `libvsmbr-20240505/tests/vsmbr_test_memory.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_section_values.c` & `libvsmbr-20240505/tests/vsmbr_test_section_values.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/vsmbr_test_support.c` & `libvsmbr-20240505/tests/vsmbr_test_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/tests/test_library.sh` & `libvsmbr-20240505/tests/test_library.sh`

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
 
 LIBRARY_TESTS="boot_record chs_address error io_handle notify partition_entry partition_type partition_values section_values sector_data";
 LIBRARY_TESTS_WITH_INPUT="partition support volume";
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

### Comparing `libvsmbr-20240302/ossfuzz/volume_fuzzer.cc` & `libvsmbr-20240505/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/ossfuzz/ossfuzz_libvsmbr.h` & `libvsmbr-20240505/ossfuzz/ossfuzz_libvsmbr.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/ossfuzz/Makefile.am` & `libvsmbr-20240505/ossfuzz/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
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
 	@LIBCPATH_CPPFLAGS@ \
@@ -48,19 +48,17 @@
 	../libvsmbr/libvsmbr.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on partition_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(partition_fuzzer_SOURCES)
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
```

### Comparing `libvsmbr-20240302/ossfuzz/ossfuzz_libbfio.h` & `libvsmbr-20240505/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/ossfuzz/partition_fuzzer.cc` & `libvsmbr-20240505/ossfuzz/partition_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/ossfuzz/Makefile.in` & `libvsmbr-20240505/ossfuzz/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -507,16 +507,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -554,15 +554,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libvsmbr/libvsmbr.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -809,23 +810,27 @@
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
+		-rm -f ./$(DEPDIR)/partition_fuzzer.Po
+	-rm -f ./$(DEPDIR)/volume_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -910,17 +915,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on partition_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(partition_fuzzer_SOURCES)
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsmbr-20240302/ltmain.sh` & `libvsmbr-20240505/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_narrow_string.c` & `libvsmbr-20240505/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_definitions.h` & `libvsmbr-20240505/libcsplit/libcsplit_definitions.h`

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

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_types.h` & `libvsmbr-20240505/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_wide_split_string.c` & `libvsmbr-20240505/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_support.h` & `libvsmbr-20240505/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/Makefile.am` & `libvsmbr-20240505/libcsplit/Makefile.am`

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

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_libcerror.h` & `libvsmbr-20240505/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_wide_string.c` & `libvsmbr-20240505/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_unused.h` & `libvsmbr-20240505/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_wide_split_string.h` & `libvsmbr-20240505/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_error.c` & `libvsmbr-20240505/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_narrow_split_string.c` & `libvsmbr-20240505/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_extern.h` & `libvsmbr-20240505/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_error.h` & `libvsmbr-20240505/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_support.c` & `libvsmbr-20240505/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_wide_string.h` & `libvsmbr-20240505/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/Makefile.in` & `libvsmbr-20240505/libcsplit/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -493,16 +493,16 @@
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
@@ -511,15 +511,16 @@
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
@@ -724,24 +725,32 @@
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
 
@@ -830,17 +839,14 @@
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

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_narrow_split_string.h` & `libvsmbr-20240505/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcsplit/libcsplit_narrow_string.h` & `libvsmbr-20240505/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/po/remove-potcdate.sin` & `libvsmbr-20240505/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/po/Makefile.in.in` & `libvsmbr-20240505/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/po/en@quot.header` & `libvsmbr-20240505/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/po/en@boldquot.header` & `libvsmbr-20240505/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/po/insert-header.sin` & `libvsmbr-20240505/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/po/Makevars` & `libvsmbr-20240505/po/Makevars`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/po/Makevars.in` & `libvsmbr-20240505/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/po/Rules-quot` & `libvsmbr-20240505/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1251.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf16_string.c` & `libvsmbr-20240505/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_base16_stream.c` & `libvsmbr-20240505/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf8_stream.h` & `libvsmbr-20240505/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_2.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_932.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_dingbats.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf8_string.c` & `libvsmbr-20240505/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_base64_stream.c` & `libvsmbr-20240505/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_error.h` & `libvsmbr-20240505/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_turkish.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_unicode_character.c` & `libvsmbr-20240505/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_gaelic.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_arabic.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_thai.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_874.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_15.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf8_string.h` & `libvsmbr-20240505/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_16.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1255.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf7_stream.c` & `libvsmbr-20240505/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_byte_stream.h` & `libvsmbr-20240505/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_koi8_u.c` & `libvsmbr-20240505/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_unused.h` & `libvsmbr-20240505/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_6.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_14.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_base64_stream.h` & `libvsmbr-20240505/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_error.c` & `libvsmbr-20240505/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_centraleurroman.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_romanian.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_6.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_9.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_russian.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_dingbats.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_15.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_936.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_croatian.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_scsu.h` & `libvsmbr-20240505/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/Makefile.am` & `libvsmbr-20240505/libuna/Makefile.am`

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

### Comparing `libvsmbr-20240302/libuna/libuna_utf32_stream.c` & `libvsmbr-20240505/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_936.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_10.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_roman.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf7_stream.h` & `libvsmbr-20240505/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_3.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_thai.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_farsi.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_ukrainian.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_inuit.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_932.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_874.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_5.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_10.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_definitions.h` & `libvsmbr-20240505/libuna/libuna_definitions.h`

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

### Comparing `libvsmbr-20240302/libuna/libuna_url_stream.h` & `libvsmbr-20240505/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_icelandic.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_koi8_u.h` & `libvsmbr-20240505/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf16_stream.c` & `libvsmbr-20240505/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1253.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_4.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_greek.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_libcerror.h` & `libvsmbr-20240505/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_centraleurroman.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1254.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_13.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_7.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1255.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_unicode_character.h` & `libvsmbr-20240505/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_8.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_13.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_949.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_cyrillic.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_celtic.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_support.h` & `libvsmbr-20240505/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_4.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_949.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf16_stream.h` & `libvsmbr-20240505/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_symbol.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_roman.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1257.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1254.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_950.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_extern.h` & `libvsmbr-20240505/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1256.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_types.h` & `libvsmbr-20240505/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_base32_stream.h` & `libvsmbr-20240505/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1253.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_16.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf8_stream.c` & `libvsmbr-20240505/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1250.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_2.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_support.c` & `libvsmbr-20240505/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_koi8_r.c` & `libvsmbr-20240505/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_5.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf16_string.h` & `libvsmbr-20240505/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf32_string.c` & `libvsmbr-20240505/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_icelandic.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1256.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf32_string.h` & `libvsmbr-20240505/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_romanian.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_8.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_koi8_r.h` & `libvsmbr-20240505/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_cyrillic.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_arabic.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_croatian.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_9.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_greek.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1258.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_7.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/Makefile.in` & `libvsmbr-20240505/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -661,16 +661,16 @@
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
@@ -736,15 +736,16 @@
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
@@ -1006,24 +1007,89 @@
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
 
@@ -1169,17 +1235,14 @@
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

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_3.c` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1250.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_scsu.c` & `libvsmbr-20240505/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1252.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_turkish.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_ukrainian.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_russian.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1258.c` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_celtic.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_byte_stream.c` & `libvsmbr-20240505/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_gaelic.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_utf32_stream.h` & `libvsmbr-20240505/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_symbol.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1257.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_inuit.h` & `libvsmbr-20240505/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_mac_farsi.c` & `libvsmbr-20240505/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_950.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_url_stream.c` & `libvsmbr-20240505/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1251.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_windows_1252.h` & `libvsmbr-20240505/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_codepage_iso_8859_14.h` & `libvsmbr-20240505/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_base16_stream.h` & `libvsmbr-20240505/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libuna/libuna_base32_stream.c` & `libvsmbr-20240505/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/Makefile.in` & `libvsmbr-20240505/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -574,16 +574,18 @@
 DPKG_FILES = \
 	dpkg/changelog \
 	dpkg/changelog.in \
 	dpkg/compat \
 	dpkg/control \
 	dpkg/copyright \
 	dpkg/rules \
-	dpkg/libvsmbr-dev.install \
 	dpkg/libvsmbr.install \
+	dpkg/libvsmbr-dev.install \
+	dpkg/libvsmbr-python3.install \
+	dpkg/libvsmbr-tools.install \
 	dpkg/source/format
 
 GETTEXT_FILES = \
 	config.rpath \
 	po/Makevars.in
 
 PKGCONFIG_FILES = \
@@ -602,16 +604,23 @@
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
+	libvsmbr.pc \
+	libvsmbr.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libvsmbr.pc
 
 all: all-recursive
 
@@ -1028,23 +1037,26 @@
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
 
@@ -1153,22 +1165,10 @@
 	(cd $(srcdir)/libcpath && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvsmbr && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvsmbr.pc
-	-rm -f libvsmbr.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_definitions.h` & `libvsmbr-20240505/libcnotify/libcnotify_definitions.h`

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

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_extern.h` & `libvsmbr-20240505/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_support.c` & `libvsmbr-20240505/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_stream.h` & `libvsmbr-20240505/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/Makefile.am` & `libvsmbr-20240505/libcnotify/Makefile.am`

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

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_unused.h` & `libvsmbr-20240505/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_verbose.h` & `libvsmbr-20240505/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_print.h` & `libvsmbr-20240505/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_stream.c` & `libvsmbr-20240505/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_support.h` & `libvsmbr-20240505/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_verbose.c` & `libvsmbr-20240505/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/Makefile.in` & `libvsmbr-20240505/libcnotify/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -485,30 +485,31 @@
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
@@ -711,24 +712,30 @@
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
 
@@ -815,17 +822,14 @@
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

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_libcerror.h` & `libvsmbr-20240505/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcnotify/libcnotify_print.c` & `libvsmbr-20240505/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/libcerror_system.c` & `libvsmbr-20240505/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/libcerror_error.c` & `libvsmbr-20240505/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/libcerror_extern.h` & `libvsmbr-20240505/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/Makefile.am` & `libvsmbr-20240505/libcerror/Makefile.am`

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

### Comparing `libvsmbr-20240302/libcerror/libcerror_types.h` & `libvsmbr-20240505/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/libcerror_support.h` & `libvsmbr-20240505/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/libcerror_error.h` & `libvsmbr-20240505/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/libcerror_system.h` & `libvsmbr-20240505/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/libcerror_definitions.h` & `libvsmbr-20240505/libcerror/libcerror_definitions.h`

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

### Comparing `libvsmbr-20240302/libcerror/libcerror_support.c` & `libvsmbr-20240505/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/libcerror_unused.h` & `libvsmbr-20240505/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/libcerror/Makefile.in` & `libvsmbr-20240505/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -482,28 +482,29 @@
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
@@ -705,24 +706,29 @@
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
 
@@ -808,17 +814,14 @@
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

### Comparing `libvsmbr-20240302/aclocal.m4` & `libvsmbr-20240505/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libvsmbr-20240302/configure.ac` & `libvsmbr-20240505/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libvsmbr],
- [20240302],
+ [20240505],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libvsmbr.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

