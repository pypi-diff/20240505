# Comparing `tmp/spicelib-1.1.1.tar.gz` & `tmp/spicelib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicelib-1.1.1.tar", last modified: Sun Apr 21 14:58:07 2024, max compression
+gzip compressed data, was "spicelib-1.1.2.tar", last modified: Sun May  5 18:29:47 2024, max compression
```

## Comparing `spicelib-1.1.1.tar` & `spicelib-1.1.2.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.469311 spicelib-1.1.1/
--rw-rw-rw-   0        0        0    35823 2023-09-01 13:27:07.000000 spicelib-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      132 2024-03-10 15:30:59.000000 spicelib-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    67351 2024-04-21 14:58:07.469311 spicelib-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    25240 2024-04-21 13:17:00.000000 spicelib-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.212540 spicelib-1.1.1/examples/
--rw-rw-rw-   0        0        0      798 2023-09-01 13:57:48.000000 spicelib-1.1.1/examples/ltsteps_example.py
--rw-rw-rw-   0        0        0     1142 2023-09-08 09:39:40.000000 spicelib-1.1.1/examples/ngspice_batch.py
--rw-rw-rw-   0        0        0     1708 2024-02-23 21:06:01.000000 spicelib-1.1.1/examples/qspice_example.py
--rw-rw-rw-   0        0        0     3151 2023-09-18 15:59:31.000000 spicelib-1.1.1/examples/raw_plotting.py
--rw-rw-rw-   0        0        0      486 2024-02-25 16:29:46.000000 spicelib-1.1.1/examples/raw_read_example.py
--rw-rw-rw-   0        0        0     4276 2024-02-25 14:48:43.000000 spicelib-1.1.1/examples/raw_write_example.py
--rw-rw-rw-   0        0        0     1833 2024-02-10 22:37:40.000000 spicelib-1.1.1/examples/run_fast_worst_case.py
--rw-rw-rw-   0        0        0     2673 2024-03-16 10:43:35.000000 spicelib-1.1.1/examples/run_montecarlo.py
--rw-rw-rw-   0        0        0     1910 2024-02-02 12:19:23.000000 spicelib-1.1.1/examples/run_sensitivity.py
--rw-rw-rw-   0        0        0     2812 2024-04-21 13:17:00.000000 spicelib-1.1.1/examples/run_worst_case.py
--rw-rw-rw-   0        0        0     2464 2024-03-16 10:41:24.000000 spicelib-1.1.1/examples/sim_client_example.py
--rw-rw-rw-   0        0        0     1479 2024-03-16 10:24:39.000000 spicelib-1.1.1/examples/sim_runner_asc_example.py
--rw-rw-rw-   0        0        0     2867 2024-04-21 13:16:18.000000 spicelib-1.1.1/examples/sim_runner_callback_example.py
--rw-rw-rw-   0        0        0     2732 2023-09-08 09:39:40.000000 spicelib-1.1.1/examples/sim_runner_callback_process_example.py
--rw-rw-rw-   0        0        0     1705 2024-03-16 10:24:39.000000 spicelib-1.1.1/examples/sim_runner_example.py
--rw-rw-rw-   0        0        0     2010 2023-09-08 09:39:40.000000 spicelib-1.1.1/examples/sim_server_example.py
--rw-rw-rw-   0        0        0     1253 2024-02-23 21:30:13.000000 spicelib-1.1.1/examples/sim_stepper_example.py
--rw-rw-rw-   0        0        0      379 2023-09-08 09:39:40.000000 spicelib-1.1.1/examples/spice_editor_example.py
--rw-rw-rw-   0        0        0     1280 2024-04-21 13:16:18.000000 spicelib-1.1.1/examples/sub_circuit_asc_edits.py
--rw-rw-rw-   0        0        0     1302 2024-04-21 13:16:18.000000 spicelib-1.1.1/examples/sub_circuit_edits.py
--rw-rw-rw-   0        0        0     1184 2024-04-21 13:16:18.000000 spicelib-1.1.1/examples/sub_circuit_qsch_edits.py
--rw-rw-rw-   0        0        0     1714 2024-04-21 13:16:18.000000 spicelib-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 14:58:07.470644 spicelib-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.221051 spicelib-1.1.1/spicelib/
--rw-rw-rw-   0        0        0     1741 2024-03-16 10:24:39.000000 spicelib-1.1.1/spicelib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.271704 spicelib-1.1.1/spicelib/client_server/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/client_server/__init__.py
--rw-rw-rw-   0        0        0    10097 2024-02-15 17:23:09.000000 spicelib-1.1.1/spicelib/client_server/sim_client.py
--rw-rw-rw-   0        0        0     8378 2024-02-16 14:22:36.000000 spicelib-1.1.1/spicelib/client_server/sim_server.py
--rw-rw-rw-   0        0        0     6097 2024-02-15 19:28:40.000000 spicelib-1.1.1/spicelib/client_server/srv_sim_runner.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.288114 spicelib-1.1.1/spicelib/editor/
--rw-rw-rw-   0        0        0      123 2023-10-15 17:22:56.000000 spicelib-1.1.1/spicelib/editor/__init__.py
--rw-rw-rw-   0        0        0    23214 2024-04-21 13:17:00.000000 spicelib-1.1.1/spicelib/editor/asc_editor.py
--rw-rw-rw-   0        0        0    11781 2024-04-21 13:16:18.000000 spicelib-1.1.1/spicelib/editor/asy_reader.py
--rw-rw-rw-   0        0        0    19713 2024-04-21 13:17:00.000000 spicelib-1.1.1/spicelib/editor/base_editor.py
--rw-rw-rw-   0        0        0    13201 2024-04-21 13:20:57.000000 spicelib-1.1.1/spicelib/editor/base_schematic.py
--rw-rw-rw-   0        0        0    36329 2024-04-21 13:30:43.000000 spicelib-1.1.1/spicelib/editor/qsch_editor.py
--rw-rw-rw-   0        0        0    47480 2024-04-21 13:17:00.000000 spicelib-1.1.1/spicelib/editor/spice_editor.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.299648 spicelib-1.1.1/spicelib/log/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/log/__init__.py
--rw-rw-rw-   0        0        0    20952 2024-03-02 20:08:05.000000 spicelib-1.1.1/spicelib/log/logfile_data.py
--rw-rw-rw-   0        0        0    25636 2024-03-16 10:24:39.000000 spicelib-1.1.1/spicelib/log/ltsteps.py
--rw-rw-rw-   0        0        0     8183 2024-03-02 20:02:43.000000 spicelib-1.1.1/spicelib/log/qspice_log_reader.py
--rw-rw-rw-   0        0        0     6664 2023-09-01 14:14:09.000000 spicelib-1.1.1/spicelib/log/semi_dev_op_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.312352 spicelib-1.1.1/spicelib/raw/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/raw/__init__.py
--rw-rw-rw-   0        0        0    14833 2023-10-16 19:39:04.000000 spicelib-1.1.1/spicelib/raw/raw_classes.py
--rw-rw-rw-   0        0        0     6197 2023-09-01 23:08:42.000000 spicelib-1.1.1/spicelib/raw/raw_convert.py
--rw-rw-rw-   0        0        0    42506 2024-02-10 22:37:40.000000 spicelib-1.1.1/spicelib/raw/raw_read.py
--rw-rw-rw-   0        0        0    17368 2023-09-01 14:14:09.000000 spicelib-1.1.1/spicelib/raw/raw_write.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.354181 spicelib-1.1.1/spicelib/scripts/
--rw-rw-rw-   0        0        0     9237 2024-04-21 13:16:18.000000 spicelib-1.1.1/spicelib/scripts/asc_to_qsch.py
--rw-rw-rw-   0        0        0     5654 2024-03-09 13:11:41.000000 spicelib-1.1.1/spicelib/scripts/asc_to_qsch_data.xml
--rw-rw-rw-   0        0        0    12544 2024-03-16 10:24:39.000000 spicelib-1.1.1/spicelib/scripts/histogram.py
--rw-rw-rw-   0        0        0     7464 2024-03-16 10:24:39.000000 spicelib-1.1.1/spicelib/scripts/ltsteps.py
--rw-rw-rw-   0        0        0     4479 2023-09-01 22:58:58.000000 spicelib-1.1.1/spicelib/scripts/rawplot.py
--rw-rw-rw-   0        0        0     3502 2024-04-21 13:17:00.000000 spicelib-1.1.1/spicelib/scripts/readme_update.py
--rw-rw-rw-   0        0        0     4295 2024-02-15 10:43:01.000000 spicelib-1.1.1/spicelib/scripts/run_server.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.371041 spicelib-1.1.1/spicelib/sim/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/sim/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-09-08 09:39:40.000000 spicelib-1.1.1/spicelib/sim/process_callback.py
--rw-rw-rw-   0        0        0     8337 2024-02-10 22:37:40.000000 spicelib-1.1.1/spicelib/sim/run_task.py
--rw-rw-rw-   0        0        0    28813 2024-02-16 14:36:38.000000 spicelib-1.1.1/spicelib/sim/sim_runner.py
--rw-rw-rw-   0        0        0    10216 2023-10-19 12:50:05.000000 spicelib-1.1.1/spicelib/sim/sim_stepping.py
--rw-rw-rw-   0        0        0     5757 2023-11-03 11:50:22.000000 spicelib-1.1.1/spicelib/sim/simulator.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.416155 spicelib-1.1.1/spicelib/sim/tookit/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/sim/tookit/__init__.py
--rw-rw-rw-   0        0        0     4800 2023-10-19 16:51:29.000000 spicelib-1.1.1/spicelib/sim/tookit/failure_modes.py
--rw-rw-rw-   0        0        0    14582 2024-02-15 19:51:50.000000 spicelib-1.1.1/spicelib/sim/tookit/fast_worst_case.py
--rw-rw-rw-   0        0        0    12645 2024-03-09 16:55:25.000000 spicelib-1.1.1/spicelib/sim/tookit/montecarlo.py
--rw-rw-rw-   0        0        0    10260 2024-02-15 19:49:53.000000 spicelib-1.1.1/spicelib/sim/tookit/quick_sensitivity_analysis.py
--rw-rw-rw-   0        0        0     9616 2024-02-15 09:14:53.000000 spicelib-1.1.1/spicelib/sim/tookit/sim_analysis.py
--rw-rw-rw-   0        0        0    13777 2024-02-15 19:48:44.000000 spicelib-1.1.1/spicelib/sim/tookit/tolerance_deviations.py
--rw-rw-rw-   0        0        0    13523 2024-02-15 19:49:32.000000 spicelib-1.1.1/spicelib/sim/tookit/worst_case.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.422392 spicelib-1.1.1/spicelib/simulators/
--rw-rw-rw-   0        0        0        0 2023-09-08 09:39:40.000000 spicelib-1.1.1/spicelib/simulators/__init__.py
--rw-rw-rw-   0        0        0    10327 2024-02-10 22:37:40.000000 spicelib-1.1.1/spicelib/simulators/ltspice_simulator.py
--rw-rw-rw-   0        0        0     5355 2023-10-08 21:40:06.000000 spicelib-1.1.1/spicelib/simulators/ngspice_simulator.py
--rw-rw-rw-   0        0        0     6026 2023-11-03 11:49:49.000000 spicelib-1.1.1/spicelib/simulators/qspice_simulator.py
--rw-rw-rw-   0        0        0     8073 2023-10-08 21:40:06.000000 spicelib-1.1.1/spicelib/simulators/xyce_simulator.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.435370 spicelib-1.1.1/spicelib/utils/
--rw-rw-rw-   0        0        0     3811 2024-02-10 22:37:40.000000 spicelib-1.1.1/spicelib/utils/detect_encoding.py
--rw-rw-rw-   0        0        0     1886 2024-04-21 13:16:18.000000 spicelib-1.1.1/spicelib/utils/file_search.py
--rw-rw-rw-   0        0        0     8101 2023-10-01 12:37:22.000000 spicelib-1.1.1/spicelib/utils/sweep_iterators.py
--rw-rw-rw-   0        0        0     1133 2024-04-21 13:16:18.000000 spicelib-1.1.1/spicelib/utils/windows_short_names.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.467834 spicelib-1.1.1/spicelib.egg-info/
--rw-rw-rw-   0        0        0    67351 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2771 2024-04-21 14:58:07.000000 spicelib-1.1.1/spicelib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      330 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       53 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.465827 spicelib-1.1.1/unittests/
--rw-rw-rw-   0        0        0     4093 2023-09-01 21:04:13.000000 spicelib-1.1.1/unittests/sweep_iterators_unittest.py
--rw-rw-rw-   0        0        0     4856 2024-02-11 08:24:38.000000 spicelib-1.1.1/unittests/test_asc_editor.py
--rw-rw-rw-   0        0        0     6573 2024-04-21 13:16:18.000000 spicelib-1.1.1/unittests/test_qsch_editor.py
--rw-rw-rw-   0        0        0    20957 2024-03-16 10:24:39.000000 spicelib-1.1.1/unittests/test_qspice_rawread.py
--rw-rw-rw-   0        0        0     4865 2023-10-19 13:29:57.000000 spicelib-1.1.1/unittests/test_spice_editor.py
--rw-rw-rw-   0        0        0    22930 2024-03-16 10:24:39.000000 spicelib-1.1.1/unittests/test_spicelib.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.109243 spicelib-1.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-09-01 13:27:07.000000 spicelib-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      132 2024-03-10 15:30:59.000000 spicelib-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    67542 2024-05-05 18:29:47.108236 spicelib-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    25431 2024-05-05 15:59:33.000000 spicelib-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.839020 spicelib-1.1.2/examples/
+-rw-rw-rw-   0        0        0      798 2023-09-01 13:57:48.000000 spicelib-1.1.2/examples/ltsteps_example.py
+-rw-rw-rw-   0        0        0     1142 2023-09-08 09:39:40.000000 spicelib-1.1.2/examples/ngspice_batch.py
+-rw-rw-rw-   0        0        0     1708 2024-02-23 21:06:01.000000 spicelib-1.1.2/examples/qspice_example.py
+-rw-rw-rw-   0        0        0     3151 2023-09-18 15:59:31.000000 spicelib-1.1.2/examples/raw_plotting.py
+-rw-rw-rw-   0        0        0      486 2024-02-25 16:29:46.000000 spicelib-1.1.2/examples/raw_read_example.py
+-rw-rw-rw-   0        0        0     4276 2024-02-25 14:48:43.000000 spicelib-1.1.2/examples/raw_write_example.py
+-rw-rw-rw-   0        0        0     2241 2024-05-05 15:55:48.000000 spicelib-1.1.2/examples/run_fast_worst_case.py
+-rw-rw-rw-   0        0        0     2673 2024-03-16 10:43:35.000000 spicelib-1.1.2/examples/run_montecarlo.py
+-rw-rw-rw-   0        0        0     1910 2024-02-02 12:19:23.000000 spicelib-1.1.2/examples/run_sensitivity.py
+-rw-rw-rw-   0        0        0     2812 2024-04-21 13:17:00.000000 spicelib-1.1.2/examples/run_worst_case.py
+-rw-rw-rw-   0        0        0     2464 2024-03-16 10:41:24.000000 spicelib-1.1.2/examples/sim_client_example.py
+-rw-rw-rw-   0        0        0     1479 2024-03-16 10:24:39.000000 spicelib-1.1.2/examples/sim_runner_asc_example.py
+-rw-rw-rw-   0        0        0     2867 2024-04-21 13:16:18.000000 spicelib-1.1.2/examples/sim_runner_callback_example.py
+-rw-rw-rw-   0        0        0     2732 2023-09-08 09:39:40.000000 spicelib-1.1.2/examples/sim_runner_callback_process_example.py
+-rw-rw-rw-   0        0        0     1705 2024-03-16 10:24:39.000000 spicelib-1.1.2/examples/sim_runner_example.py
+-rw-rw-rw-   0        0        0     2010 2023-09-08 09:39:40.000000 spicelib-1.1.2/examples/sim_server_example.py
+-rw-rw-rw-   0        0        0     1253 2024-02-23 21:30:13.000000 spicelib-1.1.2/examples/sim_stepper_example.py
+-rw-rw-rw-   0        0        0      379 2023-09-08 09:39:40.000000 spicelib-1.1.2/examples/spice_editor_example.py
+-rw-rw-rw-   0        0        0     1280 2024-04-21 13:16:18.000000 spicelib-1.1.2/examples/sub_circuit_asc_edits.py
+-rw-rw-rw-   0        0        0     1302 2024-04-21 13:16:18.000000 spicelib-1.1.2/examples/sub_circuit_edits.py
+-rw-rw-rw-   0        0        0     1184 2024-04-21 13:16:18.000000 spicelib-1.1.2/examples/sub_circuit_qsch_edits.py
+-rw-rw-rw-   0        0        0     1714 2024-05-05 15:55:48.000000 spicelib-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:29:47.109243 spicelib-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.840025 spicelib-1.1.2/spicelib/
+-rw-rw-rw-   0        0        0     1741 2024-03-16 10:24:39.000000 spicelib-1.1.2/spicelib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.886121 spicelib-1.1.2/spicelib/client_server/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/client_server/__init__.py
+-rw-rw-rw-   0        0        0    10097 2024-02-15 17:23:09.000000 spicelib-1.1.2/spicelib/client_server/sim_client.py
+-rw-rw-rw-   0        0        0     8378 2024-02-16 14:22:36.000000 spicelib-1.1.2/spicelib/client_server/sim_server.py
+-rw-rw-rw-   0        0        0     6097 2024-02-15 19:28:40.000000 spicelib-1.1.2/spicelib/client_server/srv_sim_runner.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.900761 spicelib-1.1.2/spicelib/editor/
+-rw-rw-rw-   0        0        0      123 2023-10-15 17:22:56.000000 spicelib-1.1.2/spicelib/editor/__init__.py
+-rw-rw-rw-   0        0        0    24463 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/asc_editor.py
+-rw-rw-rw-   0        0        0    13608 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/asy_reader.py
+-rw-rw-rw-   0        0        0    19855 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/base_editor.py
+-rw-rw-rw-   0        0        0    13410 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/base_schematic.py
+-rw-rw-rw-   0        0        0     4065 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/ltspice_utils.py
+-rw-rw-rw-   0        0        0    36418 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/qsch_editor.py
+-rw-rw-rw-   0        0        0    47162 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/spice_editor.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.922097 spicelib-1.1.2/spicelib/log/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/log/__init__.py
+-rw-rw-rw-   0        0        0    20952 2024-03-02 20:08:05.000000 spicelib-1.1.2/spicelib/log/logfile_data.py
+-rw-rw-rw-   0        0        0    25636 2024-03-16 10:24:39.000000 spicelib-1.1.2/spicelib/log/ltsteps.py
+-rw-rw-rw-   0        0        0     8183 2024-03-02 20:02:43.000000 spicelib-1.1.2/spicelib/log/qspice_log_reader.py
+-rw-rw-rw-   0        0        0     6664 2023-09-01 14:14:09.000000 spicelib-1.1.2/spicelib/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.944039 spicelib-1.1.2/spicelib/raw/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/raw/__init__.py
+-rw-rw-rw-   0        0        0    14833 2023-10-16 19:39:04.000000 spicelib-1.1.2/spicelib/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     6197 2023-09-01 23:08:42.000000 spicelib-1.1.2/spicelib/raw/raw_convert.py
+-rw-rw-rw-   0        0        0    42506 2024-02-10 22:37:40.000000 spicelib-1.1.2/spicelib/raw/raw_read.py
+-rw-rw-rw-   0        0        0    17368 2023-09-01 14:14:09.000000 spicelib-1.1.2/spicelib/raw/raw_write.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.986493 spicelib-1.1.2/spicelib/scripts/
+-rw-rw-rw-   0        0        0     9237 2024-04-21 13:16:18.000000 spicelib-1.1.2/spicelib/scripts/asc_to_qsch.py
+-rw-rw-rw-   0        0        0     5654 2024-03-09 13:11:41.000000 spicelib-1.1.2/spicelib/scripts/asc_to_qsch_data.xml
+-rw-rw-rw-   0        0        0    12544 2024-03-16 10:24:39.000000 spicelib-1.1.2/spicelib/scripts/histogram.py
+-rw-rw-rw-   0        0        0     7464 2024-03-16 10:24:39.000000 spicelib-1.1.2/spicelib/scripts/ltsteps.py
+-rw-rw-rw-   0        0        0     4479 2023-09-01 22:58:58.000000 spicelib-1.1.2/spicelib/scripts/rawplot.py
+-rw-rw-rw-   0        0        0     3505 2024-04-28 17:15:15.000000 spicelib-1.1.2/spicelib/scripts/readme_update.py
+-rw-rw-rw-   0        0        0     4295 2024-02-15 10:43:01.000000 spicelib-1.1.2/spicelib/scripts/run_server.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.003037 spicelib-1.1.2/spicelib/sim/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/sim/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-09-08 09:39:40.000000 spicelib-1.1.2/spicelib/sim/process_callback.py
+-rw-rw-rw-   0        0        0     8337 2024-02-10 22:37:40.000000 spicelib-1.1.2/spicelib/sim/run_task.py
+-rw-rw-rw-   0        0        0    28817 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/sim/sim_runner.py
+-rw-rw-rw-   0        0        0    10216 2023-10-19 12:50:05.000000 spicelib-1.1.2/spicelib/sim/sim_stepping.py
+-rw-rw-rw-   0        0        0     5757 2023-11-03 11:50:22.000000 spicelib-1.1.2/spicelib/sim/simulator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.042833 spicelib-1.1.2/spicelib/sim/tookit/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/sim/tookit/__init__.py
+-rw-rw-rw-   0        0        0     4800 2023-10-19 16:51:29.000000 spicelib-1.1.2/spicelib/sim/tookit/failure_modes.py
+-rw-rw-rw-   0        0        0    14582 2024-02-15 19:51:50.000000 spicelib-1.1.2/spicelib/sim/tookit/fast_worst_case.py
+-rw-rw-rw-   0        0        0    12645 2024-03-09 16:55:25.000000 spicelib-1.1.2/spicelib/sim/tookit/montecarlo.py
+-rw-rw-rw-   0        0        0    10260 2024-02-15 19:49:53.000000 spicelib-1.1.2/spicelib/sim/tookit/quick_sensitivity_analysis.py
+-rw-rw-rw-   0        0        0     9616 2024-02-15 09:14:53.000000 spicelib-1.1.2/spicelib/sim/tookit/sim_analysis.py
+-rw-rw-rw-   0        0        0    13777 2024-02-15 19:48:44.000000 spicelib-1.1.2/spicelib/sim/tookit/tolerance_deviations.py
+-rw-rw-rw-   0        0        0    13523 2024-02-15 19:49:32.000000 spicelib-1.1.2/spicelib/sim/tookit/worst_case.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.063164 spicelib-1.1.2/spicelib/simulators/
+-rw-rw-rw-   0        0        0        0 2023-09-08 09:39:40.000000 spicelib-1.1.2/spicelib/simulators/__init__.py
+-rw-rw-rw-   0        0        0    10327 2024-02-10 22:37:40.000000 spicelib-1.1.2/spicelib/simulators/ltspice_simulator.py
+-rw-rw-rw-   0        0        0     5355 2023-10-08 21:40:06.000000 spicelib-1.1.2/spicelib/simulators/ngspice_simulator.py
+-rw-rw-rw-   0        0        0     6026 2023-11-03 11:49:49.000000 spicelib-1.1.2/spicelib/simulators/qspice_simulator.py
+-rw-rw-rw-   0        0        0     8073 2023-10-08 21:40:06.000000 spicelib-1.1.2/spicelib/simulators/xyce_simulator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.068472 spicelib-1.1.2/spicelib/utils/
+-rw-rw-rw-   0        0        0     3811 2024-02-10 22:37:40.000000 spicelib-1.1.2/spicelib/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0     3105 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/utils/file_search.py
+-rw-rw-rw-   0        0        0     8213 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/utils/sweep_iterators.py
+-rw-rw-rw-   0        0        0     2471 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/utils/windows_short_names.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.107236 spicelib-1.1.2/spicelib.egg-info/
+-rw-rw-rw-   0        0        0    67542 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2804 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      330 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       53 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.105230 spicelib-1.1.2/unittests/
+-rw-rw-rw-   0        0        0     4093 2023-09-01 21:04:13.000000 spicelib-1.1.2/unittests/sweep_iterators_unittest.py
+-rw-rw-rw-   0        0        0     4856 2024-02-11 08:24:38.000000 spicelib-1.1.2/unittests/test_asc_editor.py
+-rw-rw-rw-   0        0        0     6573 2024-04-21 13:16:18.000000 spicelib-1.1.2/unittests/test_qsch_editor.py
+-rw-rw-rw-   0        0        0    20957 2024-03-16 10:24:39.000000 spicelib-1.1.2/unittests/test_qspice_rawread.py
+-rw-rw-rw-   0        0        0     4865 2023-10-19 13:29:57.000000 spicelib-1.1.2/unittests/test_spice_editor.py
+-rw-rw-rw-   0        0        0    22930 2024-03-16 10:24:39.000000 spicelib-1.1.2/unittests/test_spicelib.py
```

### Comparing `spicelib-1.1.1/LICENSE` & `spicelib-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/PKG-INFO` & `spicelib-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicelib
-Version: 1.1.1
+Version: 1.1.2
 Summary: A set of tools to Automate Spice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -1185,14 +1185,17 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 1.1.2
+  * Fixes on the readme_update.py script. Was not supporting spaces after the []
+  * Solving issue PyLTspice Issue #138. Hierarchical edits to ASC files are now supported.
 * Version 1.1.1
   * Supporting hierarchical edits on both QSpice and LTspice schematics
   * Skipping the need of the rich library on examples
   * Giving feedback on the search for symbols on the ASC to QSCH conversion
   * Improvement on Documentation
   * Adding examples and unittests on hiearchical edits
   * Giving access to hidden properties (asc_file_path in AscEditor and qsch_file_path in QschEditor)
```

### Comparing `spicelib-1.1.1/README.md` & `spicelib-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -487,14 +487,17 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 1.1.2
+  * Fixes on the readme_update.py script. Was not supporting spaces after the []
+  * Solving issue PyLTspice Issue #138. Hierarchical edits to ASC files are now supported.
 * Version 1.1.1
   * Supporting hierarchical edits on both QSpice and LTspice schematics
   * Skipping the need of the rich library on examples
   * Giving feedback on the search for symbols on the ASC to QSCH conversion
   * Improvement on Documentation
   * Adding examples and unittests on hiearchical edits
   * Giving access to hidden properties (asc_file_path in AscEditor and qsch_file_path in QschEditor)
```

### Comparing `spicelib-1.1.1/examples/ltsteps_example.py` & `spicelib-1.1.2/examples/ltsteps_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/ngspice_batch.py` & `spicelib-1.1.2/examples/ngspice_batch.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/qspice_example.py` & `spicelib-1.1.2/examples/qspice_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/raw_plotting.py` & `spicelib-1.1.2/examples/raw_plotting.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/raw_write_example.py` & `spicelib-1.1.2/examples/raw_write_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/run_fast_worst_case.py` & `spicelib-1.1.2/examples/run_fast_worst_case.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python
+# coding=utf-8
 import logging
 
 import spicelib
 from spicelib import AscEditor, SimRunner  # Imports the class that manipulates the asc file
 from spicelib.sim.tookit.fast_worst_case import FastWorstCaseAnalysis
 from spicelib.simulators.ltspice_simulator import LTspice
 
@@ -26,10 +28,18 @@
 # Finally the netlist is saved to a file
 wca.save_netlist('./testfiles/sallenkey_fwc.asc')
 
 print("=====================================")
 # Now using the second method, where the simulations are ran one by one
 wca.clear_simulation_data()  # Clears the simulation data
 wca.reset_netlist()  # Resets the netlist to the original
-results = wca.run_analysis(measure='fcut')  # Makes the Worst Case Analysis
-print(results)
+nominal, min_value, max_comp_values, max_value, min_comp_values = wca.run_analysis(measure='fcut')  # Makes the Worst Case Analysis
+print("Nominal Value", nominal)
+print("Worst Case Min", min_value)
+print("Min Component Values")
+for comp, value in min_comp_values.items():
+    print(f"    {comp} = {value}")
+print("Worst Case Max", max_value)
+print("Max Component Values")
+for comp, value in max_comp_values.items():
+    print(f"    {comp} = {value}")
 wca.cleanup_files()  # Deletes the temporary files
```

### Comparing `spicelib-1.1.1/examples/run_montecarlo.py` & `spicelib-1.1.2/examples/run_montecarlo.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/run_sensitivity.py` & `spicelib-1.1.2/examples/run_sensitivity.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/run_worst_case.py` & `spicelib-1.1.2/examples/run_worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sim_client_example.py` & `spicelib-1.1.2/examples/sim_client_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sim_runner_asc_example.py` & `spicelib-1.1.2/examples/sim_runner_asc_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sim_runner_callback_example.py` & `spicelib-1.1.2/examples/sim_runner_callback_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sim_runner_callback_process_example.py` & `spicelib-1.1.2/examples/sim_runner_callback_process_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sim_runner_example.py` & `spicelib-1.1.2/examples/sim_runner_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sim_server_example.py` & `spicelib-1.1.2/examples/sim_server_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sim_stepper_example.py` & `spicelib-1.1.2/examples/sim_stepper_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sub_circuit_asc_edits.py` & `spicelib-1.1.2/examples/sub_circuit_asc_edits.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sub_circuit_edits.py` & `spicelib-1.1.2/examples/sub_circuit_edits.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/examples/sub_circuit_qsch_edits.py` & `spicelib-1.1.2/examples/sub_circuit_qsch_edits.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/pyproject.toml` & `spicelib-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "spicelib"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to Automate Spice simulations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `spicelib-1.1.1/spicelib/__init__.py` & `spicelib-1.1.2/spicelib/__init__.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/client_server/sim_client.py` & `spicelib-1.1.2/spicelib/client_server/sim_client.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/client_server/sim_server.py` & `spicelib-1.1.2/spicelib/client_server/sim_server.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/client_server/srv_sim_runner.py` & `spicelib-1.1.2/spicelib/client_server/srv_sim_runner.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/editor/asc_editor.py` & `spicelib-1.1.2/spicelib/editor/asc_editor.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,112 +17,31 @@
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 import os.path
 from pathlib import Path
 from typing import Union, Optional
 import re
 import logging
-from ..utils.file_search import find_file_in_directory
-from .base_editor import BaseEditor, format_eng, ComponentNotFoundError, ParameterNotFoundError, PARAM_REGEX, \
-    UNIQUE_SIMULATION_DOT_INSTRUCTIONS, Component
-from .base_schematic import (BaseSchematic, Point, Line, Text, SchematicComponent, ERotation, HorAlign, VerAlign,
-                             TextTypeEnum, Port)
 
-_logger = logging.getLogger("spicelib.AscEditor")
+from .ltspice_utils import TEXT_REGEX, TEXT_REGEX_X, TEXT_REGEX_Y, TEXT_REGEX_ALIGN, TEXT_REGEX_SIZE, TEXT_REGEX_TYPE, \
+    TEXT_REGEX_TEXT, END_LINE_TERM, ASC_ROTATION_DICT, ASC_INV_ROTATION_DICT, asc_text_align_set, asc_text_align_get
+from .spice_editor import SpiceEditor, SpiceCircuit
+from ..utils.file_search import search_file_in_containers
+from .base_editor import format_eng, ComponentNotFoundError, ParameterNotFoundError, PARAM_REGEX, \
+    UNIQUE_SIMULATION_DOT_INSTRUCTIONS
+from .base_schematic import (BaseSchematic, Point, Line, Text, SchematicComponent, ERotation, TextTypeEnum, Port)
+from .asy_reader import AsyReader
 
-TEXT_REGEX = re.compile(r"TEXT (-?\d+)\s+(-?\d+)\s+(Left|Right|Top|Bottom)\s(\d+)\s*(?P<type>[!;])(?P<text>.*)",
-                        re.IGNORECASE)
-TEXT_REGEX_X = 1
-TEXT_REGEX_Y = 2
-TEXT_REGEX_ALIGN = 3
-TEXT_REGEX_SIZE = 4
-TEXT_REGEX_TYPE = 5
-TEXT_REGEX_TEXT = 6
-
-END_LINE_TERM = "\n"
-
-
-ASC_ROTATION_DICT = {
-    'R0': ERotation.R0,
-    'R90': ERotation.R90,
-    'R180': ERotation.R180,
-    'R270': ERotation.R270,
-    'M0': ERotation.M0,
-    'M90': ERotation.M90,
-    'M180': ERotation.M180,
-    'M270': ERotation.M270,
-}
-
-ASC_INV_ROTATION_DICT = {val: key for key, val in ASC_ROTATION_DICT.items()}
-
-LT_ATTRIBUTE_NUMBERS = {
-    'Prefix': 0,
-    'Type': 1,
-    'Value': 3,
-    'Value2': 123,
-    'SpiceModel': 38,
-    'ModelFile': 'X',
-    'Def_Sub': 'X',
-    'SpiceLine': 39,
-    'SpiceLine2': 40,
-}
-
-LT_ATTRIBUTE_NUMBERS_INV = {val: key for key, val in LT_ATTRIBUTE_NUMBERS.items()}
-
-WEIGHT_CONVERSION_TABLE = ('Thin', 'Normal', 'Thick')
-
-
-def asc_text_align_set(text: Text, alignment: str):
-    if alignment == 'Left':
-        text.textAlignment = HorAlign.LEFT
-        text.verticalAlignment = VerAlign.CENTER
-    elif alignment == 'Center':
-        text.textAlignment = HorAlign.CENTER
-        text.verticalAlignment = VerAlign.CENTER
-    elif alignment == 'Right':
-        text.textAlignment = HorAlign.RIGHT
-        text.verticalAlignment = VerAlign.CENTER
-    elif alignment == 'VTop':
-        text.textAlignment = HorAlign.CENTER
-        text.verticalAlignment = VerAlign.TOP
-    elif alignment == 'VCenter':
-        text.textAlignment = HorAlign.CENTER
-        text.verticalAlignment = VerAlign.CENTER
-    elif alignment == 'VBottom':
-        text.textAlignment = HorAlign.LEFT
-        text.verticalAlignment = VerAlign.BOTTOM
-    else:
-        # Default
-        text.textAlignment = HorAlign.LEFT
-        text.verticalAlignment = VerAlign.CENTER
-    return text
-
-
-def asc_text_align_get(text: Text) -> str:
-    if text.verticalAlignment == VerAlign.CENTER:
-        if text.textAlignment == HorAlign.RIGHT:
-            return 'Right'
-        elif text.textAlignment == HorAlign.CENTER:
-            return 'Center'
-        else:
-            return 'Left'
-    else:
-        if text.verticalAlignment == VerAlign.TOP:
-            return 'VTop'
-        elif text.verticalAlignment == VerAlign.CENTER:
-            return 'VCenter'
-        elif text.verticalAlignment == VerAlign.BOTTOM:
-            return 'VBottom'
-        else:
-            return 'Left'
+_logger = logging.getLogger("spicelib.AscEditor")
 
 
 class AscEditor(BaseSchematic):
     """Class made to update directly the LTspice ASC files"""
     lib_paths = []  # This is a class variable, so it can be shared between all instances.
+    symbol_cache = {}  # This is a class variable, so it can be shared between all instances.
 
     def __init__(self, asc_file: str):
         super().__init__()
         self.version = 4
         self.sheet = "1 0 0"  # Three values are present on the SHEET clause
         self.asc_file_path = Path(asc_file)
         if not self.asc_file_path.exists():
@@ -210,17 +129,18 @@
 
                 elif line.startswith("SYMATTR"):
                     assert component is not None, "Syntax Error: SYMATTR clause without SYMBOL"
                     tag, ref, text = line.split(maxsplit=2)
                     text = text.strip()  # Gets rid of the \n terminator
                     if ref == "InstName":
                         component.reference = text
-                        if component.reference.startswith('X'):  # This is a subcircuit
+                        symbol = self._get_symbol(component.symbol)
+                        if component.reference.startswith('X') or symbol.is_subcircuit():  # This is a subcircuit
                             # then create the attribute "SUBCKT"
-                            component.attributes["_SUBCKT"] = self._get_symbol_circuit(component.symbol)
+                            component.attributes["_SUBCKT"] = self._get_subcircuit(symbol)
                     else:
                         component.attributes[ref] = text
                 elif line.startswith("TEXT"):
                     match = TEXT_REGEX.match(line)
                     if match:
                         text = match.group(TEXT_REGEX_TEXT)
                         X = int(match.group(TEXT_REGEX_X))
@@ -262,18 +182,48 @@
                 else:
                     raise NotImplementedError("Primitive not supported for ASC file\n" 
                                               f'"{line}"')
             if component is not None:
                 assert component.reference is not None, "Component InstName was not given"
                 self.components[component.reference] = component
 
-    def _get_symbol_circuit(self, symbol: str):
-        asc_filename = symbol + os.path.extsep + "asc"
-        asc_path = self._lib_file_find(asc_filename)
-        answer = AscEditor(asc_path)
+    def _get_symbol(self, symbol: str) -> AsyReader:
+        asy_filename = symbol + os.path.extsep + "asy"
+        asy_path = self._asy_file_find(asy_filename)
+        if asy_path is None:
+            raise FileNotFoundError(f"File {asy_filename} not found")
+        answer = AsyReader(asy_path)
+        return answer
+
+    def _get_subcircuit(self, symbol: AsyReader) -> Union[SpiceEditor, 'AscEditor']:
+        # if it is a an ASC file, then we need to read it
+        if symbol.symbol_type == "BLOCK":
+            asc_filename = symbol.get_schematic_file()
+            if asc_filename.exists():
+                asc_path = asc_filename
+            else:
+                asc_path = search_file_in_containers(asc_filename.stem + os.path.extsep + "asc",
+                                                     # The directory where the script is located
+                                                     os.path.split(self.asc_file_path)[0],
+                                                     # The current script directory
+                                                     os.path.curdir,
+                                                     # The library paths
+                                                     *self.lib_paths)
+            if asc_path is None:
+                raise FileNotFoundError(f"File {asc_filename} not found")
+            answer = AscEditor(asc_path)
+        elif symbol.symbol_type == "CELL":
+            model = symbol.get_model()
+            lib = symbol.get_library()
+            lib_path = self._lib_file_find(lib)
+            if lib_path is None:
+                raise FileNotFoundError(f"File {lib} not found")
+            answer = SpiceEditor.find_subckt_in_lib(lib_path, model)
+        else:
+            raise ValueError(f"Symbol type {symbol.symbol_type} not supported")
         return answer
 
     def get_subcircuit(self, reference: str) -> 'AscEditor':
         """Returns an AscEditor file corresponding to the symbol"""
         sub = self.get_component(reference)
         return sub.attributes["_SUBCKT"]
 
@@ -331,26 +281,40 @@
             text = f".param {param}={value}"
             directive = Text(coord=coord, text=text, size=2, type=TextTypeEnum.DIRECTIVE)
             _logger.info(f"Parameter {param} added with value {value}")
             self.directives.append(directive)
         self.updated = True
 
     def set_component_value(self, device: str, value: Union[str, int, float]) -> None:
-        component = self.get_component(device)
-        if "Value" in component.attributes:
-            if isinstance(value, str):
-                value_str = value
-            else:
-                value_str = format_eng(value)
-            component.attributes["Value"] = value_str
-            _logger.info(f"Component {device} updated to {value_str}")
-            self.set_updated(device)
+        """
+        Sets the value of the component
+
+        :param device: The reference of the component
+        :param value: The new value
+        """
+        sub_circuit, ref = self._get_parent(device)
+
+        if sub_circuit != self:  # The component is in a subcircuit
+            if isinstance(sub_circuit, SpiceCircuit):
+                _logger.warning(f"Component {device} is in an Spice subcircuit. "
+                                f"This function may not work as expected.")
+            return sub_circuit.set_component_value(ref, value)
         else:
-            _logger.error(f"Component {device} does not have a Value attribute")
-            raise ComponentNotFoundError(f"Component {device} does not have a Value attribute")
+            component = self.get_component(device)
+            if "Value" in component.attributes:
+                if isinstance(value, str):
+                    value_str = value
+                else:
+                    value_str = format_eng(value)
+                component.attributes["Value"] = value_str
+                _logger.info(f"Component {device} updated to {value_str}")
+                self.set_updated(device)
+            else:
+                _logger.error(f"Component {device} does not have a Value attribute")
+                raise ComponentNotFoundError(f"Component {device} does not have a Value attribute")
 
     def set_element_model(self, element: str, model: str) -> None:
         component = self.get_component(element)
         component.symbol = model
         _logger.info(f"Component {element} updated to {model}")
         self.set_updated(element)
 
@@ -406,32 +370,43 @@
         return min_x, max_y + 24  # Setting the text in the bottom left corner of the canvas
 
     def add_library_paths(self, *paths):
         """Adding paths for searching for symbols and libraries"""
         self.lib_paths.extend(*paths)
 
     def _lib_file_find(self, filename) -> Optional[str]:
-        for sym_root in self.lib_paths + [
-            # os.path.curdir,  # The current script directory
-            os.path.split(self.asc_file_path)[0],  # The directory where the script is located
-            os.path.expanduser(r"~\AppData\Local\LTspice\lib\sym"),
-            os.path.expanduser(r"~\Documents\LtspiceXVII\lib\sym"),
-            # os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\lib.zip"), # TODO: implement this
-        ]:
-            print(f"   {os.path.abspath(sym_root)}")
-            if not os.path.exists(sym_root):  # Skipping invalid paths
-                continue
-            if sym_root.endswith('.zip'):
-                pass
-                # TODO: Using an IO buffer to pass the file to the AsyEditor
-            else:
-                file_found = find_file_in_directory(sym_root, filename)
-                if file_found is not None:
-                    return file_found
-        return None
+        file_found = search_file_in_containers(filename, *self.lib_paths)  # The library paths
+        if file_found is None:
+            file_found = search_file_in_containers(filename,
+                                                   os.path.split(self.asc_file_path)[0],
+                                                   os.path.curdir,  # The current script directory,
+                                                   os.path.split(self.asc_file_path)[0],
+                                                   # The directory where the script is located
+                                                   os.path.expanduser(r"~\AppData\Local\LTspice\lib\sub"),
+                                                   os.path.expanduser(r"~\Documents\LtspiceXVII\lib\sub"),
+                                                   os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\lib.zip"),
+                                                   )
+        return file_found
+
+    def _asy_file_find(self, filename) -> Optional[str]:
+        if filename in self.symbol_cache:
+            return self.symbol_cache[filename]
+        _logger.info(f"Searching for symbol {filename}...")
+        file_found = search_file_in_containers(filename, *self.lib_paths)
+        if file_found is None:
+            file_found = search_file_in_containers(filename,
+                                                   os.path.curdir,  # The current script directory
+                                                   os.path.split(self.asc_file_path)[0],
+                                                   # The directory where the script is located
+                                                   os.path.expanduser(r"~\AppData\Local\LTspice\lib\sym"),
+                                                   os.path.expanduser(r"~\Documents\LtspiceXVII\lib\sym"),
+                                                   )
+        if file_found is not None:
+            self.symbol_cache[filename] = file_found
+        return file_found
 
     def add_instruction(self, instruction: str) -> None:
         # docstring inherited from BaseEditor
         instruction = instruction.strip()  # Clean any end of line terminators
         set_command = instruction.split()[0].upper()
 
         if set_command in UNIQUE_SIMULATION_DOT_INSTRUCTIONS:
```

### Comparing `spicelib-1.1.1/spicelib/editor/asy_reader.py` & `spicelib-1.1.2/spicelib/editor/asy_reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
 import logging
 from collections import OrderedDict
 from pathlib import Path
 from typing import Union
 
 from .base_schematic import Point, Text, TextTypeEnum, Line, Circle, Rectangle, Arc, HorAlign, ERotation, VerAlign
-from .asc_editor import asc_text_align_set, TEXT_REGEX, LT_ATTRIBUTE_NUMBERS, LT_ATTRIBUTE_NUMBERS_INV, \
-    WEIGHT_CONVERSION_TABLE
+from .ltspice_utils import asc_text_align_set
 
 from .qsch_editor import QschTag
 
 _logger = logging.getLogger("spicelib.AsyReader")
 SCALE_X = 6.25
 SCALE_Y = - 6.25
 
@@ -232,7 +231,49 @@
                     attr_dict[k] = v
 
             pin_tag, _ = QschTag.parse(f'«pin ({coord.X * SCALE_X:.0f},{coord.Y * SCALE_Y:.0f}) (0,0)'
                                        f' 1 0 0 0x1000000 -1 "{attr_dict["PinName"]}"»')
             symbol.items.append(pin_tag)
 
         return symbol
+
+    def is_subcircuit(self):
+        return self.symbol_type == 'BLOCK' or self.attributes.get('Prefix') == 'X'
+
+    def get_library(self) -> str:
+        """Returns the library name of the model. If not found, returns None."""
+        # Searching in this exact order
+        for attr in ('ModelFile', 'SpiceModel', 'SpiceLine', 'SpiceLine2', 'Def_Sub', 'Value', 'Value2'):
+            if attr in self.attributes and (self.attributes[attr].endswith('.lib') or
+                        self.attributes[attr].endswith('.sub') or
+                        self.attributes[attr].endswith('.cir')
+            ):
+                return self.attributes[attr]
+        return self.attributes.get('SpiceModel')
+
+    def get_model(self) -> str:
+        """Returns the model name of the component. If not found, returns None."""
+        # Searching in this exact order
+        for attr in ('Value', 'SpiceModel', 'Value2', 'ModelFile', 'SpiceLine', 'SpiceLine2', 'Def_Sub', ):
+            if attr in self.attributes:
+                return self.attributes[attr]
+        raise ValueError("No Value or Value2 attribute found")
+
+    def get_value(self) -> Union[int, float, str]:
+        """
+        Returns the value of the component. If not found, returns None.
+        If found it tries to convert the value to a number. If it fails, it returns the string.
+        """
+        value = self.get_model()
+        try:
+            ans = int(value)
+        except ValueError:
+            try:
+                ans = float(value)
+            except ValueError:
+                ans = value.strip()  # Removes the leading trailing spaces
+        return ans
+
+    def get_schematic_file(self):
+        assert self._asy_file_path.suffix == '.asy', "File is not an asy file"
+        assert self.symbol_type == 'BLOCK', "File is not a subcircuit"
+        return self._asy_file_path.with_suffix('.asc')
```

### Comparing `spicelib-1.1.1/spicelib/editor/base_editor.py` & `spicelib-1.1.2/spicelib/editor/base_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python
 # coding=utf-8
-
 # -------------------------------------------------------------------------------
 #
 #  ███████╗██████╗ ██╗ ██████╗███████╗██╗     ██╗██████╗
 #  ██╔════╝██╔══██╗██║██╔════╝██╔════╝██║     ██║██╔══██╗
 #  ███████╗██████╔╝██║██║     █████╗  ██║     ██║██████╔╝
 #  ╚════██║██╔═══╝ ██║██║     ██╔══╝  ██║     ██║██╔══██╗
 #  ███████║██║     ██║╚██████╗███████╗███████╗██║██████╔╝
@@ -14,21 +12,29 @@
 # Purpose:     Abstract class that defines the protocol for the editors
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
+__author__ = "Nuno Brum"
+__version__ = "0.1.0"
+
+
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from math import floor, log
 from pathlib import Path
 from typing import Union
 import logging
 
+
+__author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
+__copyright__ = "Copyright 2021, Fribourg Switzerland"
+
 _logger = logging.getLogger("spicelib.BaseEditor")
 
 SUBCKT_DIVIDER = ':'  #: This controls the sub-circuit divider when setting component values inside sub-circuits.
 # Ex: Editor.set_component_value('XU1:R1', '1k')
 
 UNIQUE_SIMULATION_DOT_INSTRUCTIONS = ('.AC', '.DC', '.TRAN', '.NOISE', '.DC', '.TF')
 SPICE_DOT_INSTRUCTIONS = (
```

### Comparing `spicelib-1.1.1/spicelib/editor/base_schematic.py` & `spicelib-1.1.2/spicelib/editor/base_schematic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-#!/usr/bin/env python
 # coding=utf-8
-import abc
-import dataclasses
-import enum
 # -------------------------------------------------------------------------------
 #
 #  ███████╗██████╗ ██╗ ██████╗███████╗██╗     ██╗██████╗
 #  ██╔════╝██╔══██╗██║██╔════╝██╔════╝██║     ██║██╔══██╗
 #  ███████╗██████╔╝██║██║     █████╗  ██║     ██║██████╔╝
 #  ╚════██║██╔═══╝ ██║██║     ██╔══╝  ██║     ██║██╔══██╗
 #  ███████║██║     ██║╚██████╗███████╗███████╗██║██████╔╝
 #  ╚══════╝╚═╝     ╚═╝ ╚═════╝╚══════╝╚══════╝╚═╝╚═════╝
 #
-# Name:        base_editor.py
-# Purpose:     Abstract class that defines the protocol for the editors
+# Name:        base_schematic.py
+# Purpose:     Base classes for schematic editors
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
 
+import dataclasses
+import enum
 from typing import List, Callable, Union
 from collections import OrderedDict
 import logging
 from .base_editor import BaseEditor, Component, ComponentNotFoundError, SUBCKT_DIVIDER
 
+__author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
+__copyright__ = "Copyright 2021, Fribourg Switzerland"
+
 _logger = logging.getLogger("spicelib.BaseSchematic")
 
 
 class ERotation(enum.IntEnum):
     """Component Rotation Enum"""
     R0 = 0  # 0 Rotation
     R45 = 45  # 45 Rotation
@@ -283,18 +284,21 @@
 
         :param reference: The reference of the component
         :return: The SchematicComponent object
         :raises ComponentNotFoundError: If the component is not found.
         """
         sub_circuit, ref = self._get_parent(reference)
 
-        if ref not in sub_circuit.components:
-            _logger.error(f"Component {reference} not found")
-            raise ComponentNotFoundError(f"Component {reference} not found in Schematic file")
-        return sub_circuit.components[ref]
+        if sub_circuit != self:  # The component is in a subcircuit
+            return sub_circuit.get_component(ref)
+        else:
+            if ref not in sub_circuit.components:
+                _logger.error(f"Component {reference} not found")
+                raise ComponentNotFoundError(f"Component {reference} not found in Schematic file")
+            return sub_circuit.components[ref]
 
     def get_component_position(self, reference: str) -> (Point, ERotation):
         """Returns the position and rotation of the component"""
         comp = self.get_component(reference)
         return comp.position, comp.rotation
 
     def set_component_position(self, reference: str, position: Point, rotation: ERotation) -> None:
```

### Comparing `spicelib-1.1.1/spicelib/editor/qsch_editor.py` & `spicelib-1.1.2/spicelib/editor/qsch_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # coding=utf-8
 # -------------------------------------------------------------------------------
 #
 #  ███████╗██████╗ ██╗ ██████╗███████╗██╗     ██╗██████╗
 #  ██╔════╝██╔══██╗██║██╔════╝██╔════╝██║     ██║██╔══██╗
 #  ███████╗██████╔╝██║██║     █████╗  ██║     ██║██████╔╝
 #  ╚════██║██╔═══╝ ██║██║     ██╔══╝  ██║     ██║██╔══██╗
@@ -27,14 +26,17 @@
 from .base_editor import (
     format_eng, ComponentNotFoundError, ParameterNotFoundError,
     PARAM_REGEX, UNIQUE_SIMULATION_DOT_INSTRUCTIONS
 )
 from .base_schematic import BaseSchematic, SchematicComponent, Point, ERotation, Line, Text, TextTypeEnum
 from ..utils.file_search import find_file_in_directory
 
+__author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
+__copyright__ = "Copyright 2021, Fribourg Switzerland"
+
 __all__ = ('QschEditor', )
 
 _logger = logging.getLogger("qspice.QschEditor")
 
 QSCH_HEADER = (255, 216, 255, 219)
```

### Comparing `spicelib-1.1.1/spicelib/editor/spice_editor.py` & `spicelib-1.1.2/spicelib/editor/spice_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,16 @@
     # Frequency Noise Analysis (FRA) wiggler
     # pattern = r'^@(\d+)\s+(\w+)\s+(\w+)(?:\s+delay=(\d+\w+))?(?:\s+fstart=(\d+\w+))?(?:\s+fend=(\d+\w+))?(?:\s+oct=(\d+))?(?:\s+fcoarse=(\d+\w+))?(?:\s+nmax=(\d+\w+))?\s+(\d+)\s+(\d+\w+)\s+(\d+)(?:\s+pp0=(\d+\.\d+))?(?:\s+pp1=(\d+\.\d+))?(?:\s+f0=(\d+\w+))?(?:\s+f1=(\d+\w+))?(?:\s+tavgmin=(\d+\w+))?(?:\s+tsettle=(\d+\w+))?(?:\s+acmag=(\d+))?$'
     'Ã': r"^(?P<designator>Ã\w+)(?P<nodes>(\s+\S+){16})\s+(?P<value>.*)(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",  # QSPICE Unique component Ã
     '¥': r"^(?P<designator>¥\w+)(?P<nodes>(\s+\S+){16})\s+(?P<value>.*)(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",  # QSPICE Unique component ¥
     '€': r"^(?P<designator>€\w+)(?P<nodes>(\s+\S+){32})\s+(?P<value>.*)(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",  # QSPICE Unique component €
     '£': r"^(?P<designator>£\w+)(?P<nodes>(\s+\S+){64})\s+(?P<value>.*)(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",  # QSPICE Unique component £
     'Ø': r"^(?P<designator>Ø\w+)(?P<nodes>(\s+\S+){1,99})\s+(?P<value>.*)(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",  # QSPICE Unique component Ø
-    '×': r"^(?P<designator>×\w+)(?P<nodes>(\s+\S+){4,16})\s+(?P<value>.*)(?P<params>(\w+\s+){1,8})\s*\\?$",  # QSPICE Unique component ×
+    '×': r"^(?P<designator>×\w+)(?P<nodes>(\s+\S+){4,16})\s+(?P<value>.*)(?P<params>(\w+\s+){1,8})\s*\\?$",  # QSPICE proprietaty component ×
+    'Ö': r"^(?P<designator>Ö\w+)(?P<nodes>(\s+\S+){5})\s+(?P<params>.*)\s*\\?$",  # LTspice proprietary component Ö
 }
 
 SUBCKT_CLAUSE_FIND = r"^.SUBCKT\s+"
 
 # Code Optimization objects, avoiding repeated compilation of regular expressions
 component_replace_regexs = {prefix: re.compile(pattern, re.IGNORECASE) for prefix, pattern in REPLACE_REGXES.items()}
 subckt_regex = re.compile(r"^.SUBCKT\s+(?P<name>\w+)", re.IGNORECASE)
@@ -117,15 +118,15 @@
                     return "*"
                 elif ch == '.':  # this is a directive
                     j = i + 1
                     while j < len(line) and (line[j] not in (' ', '\t', '\r', '\n')):
                         j += 1
                     return line[i:j].upper()
                 else:
-                    raise SyntaxError('Unrecognized command in line "%s"' % line)
+                    raise SyntaxError('Unrecognized command in line "%s" of file %s' % line)
     elif isinstance(line, SpiceCircuit):
         return ".SUBCKT"
     else:
         raise SyntaxError('Unrecognized command in line "{}"'.format(line))
 
 
 def _first_token_upped(line):
@@ -260,51 +261,36 @@
         regex = component_replace_regexs['X']  # The sub-circuit instance regex
         m = regex.search(sub_circuit_instance)
         if m:
             subcircuit_name = m.group('value')  # last_token of the line before Params:
         else:
             raise UnrecognizedSyntaxError(sub_circuit_instance, REPLACE_REGXES['X'])
 
-        line_no = 0
-        libs_list = []
-        sub_circuit = None
-        while line_no < len(self.netlist):
-            line = self.netlist[line_no]
-            if isinstance(line, SpiceCircuit):
-                if line.name() == subcircuit_name:
-                    sub_circuit = line  # The circuit was already found
-                    break
-            else:
+        # Search for the sub-circuit in the netlist
+        sub_circuit = SpiceEditor.find_subckt_in_lib(self.circuit_file, subcircuit_name)
+
+        if sub_circuit is None:  # If it was not found in the netlist, search on the declared libraries
+            # If we reached here is because the subcircuit was not found. Search for it in declared libraries
+            for line in self.netlist:
                 m = lib_inc_regex.match(line)
-                if m:  # For compatibility issues not using the walruss operator here
-                    libs_list.append(m.group(2))
-            line_no += 1
-        if sub_circuit is None:
-            # If we reached here is because the subciruit was not found. Search for it in declared libraries
-            libs_list_full_path = []
-            for lib in libs_list:
-                if os.path.exists(lib):
-                    libs_list_full_path.append(lib)
-                    continue
-                # TODO: This changes dependend of the simulator being used.
-                lib_filename = os.path.join(os.path.expanduser('~'), "Documents\\LTspiceXVII\\lib\\sub", lib)
-                if os.path.exists(lib_filename):
-                    libs_list_full_path.append(lib)
-                    continue
-                for path in LibSearchPaths:
-                    lib_filename = os.path.join(path, lib)
-                    if os.path.exists(lib_filename):
-                        libs_list_full_path.append(lib_filename)
-                        continue
-
-            # If it reached here, we have a valid lib_filename
-            for lib_path in libs_list_full_path:
-                sub_circuit = SpiceEditor.find_subckt_in_lib(lib_path, subcircuit_name)
-                if sub_circuit:
-                    break
+                if m:  # If it is a library include
+                    lib = m.group(2)
+                    if os.path.exists(lib):
+                        lib_filename = os.path.join(os.path.expanduser('~'), "Documents\\LTspiceXVII\\lib\\sub", lib)
+                        if os.path.exists(lib_filename):
+                            sub_circuit = SpiceEditor.find_subckt_in_lib(lib_filename, subcircuit_name)
+                            if sub_circuit:
+                                break
+                    for path in LibSearchPaths:
+                        lib_filename = os.path.join(path, lib)
+                        if os.path.exists(lib_filename):
+                            sub_circuit = SpiceEditor.find_subckt_in_lib(lib_filename, subcircuit_name)
+                            if sub_circuit:
+                                break
+
         if sub_circuit:
             if SUBCKT_DIVIDER in instance_name:
                 return sub_circuit.get_subcircuit(sub_subckts)
             else:
                 return sub_circuit
         else:
             # The search was not successful
@@ -467,15 +453,15 @@
         :raises: ComponentNotFoundError - In case the component is not found
         :raises: UnrecognizedSyntaxError when the line doesn't match the expected REGEX.
         :raises: NotImplementedError if there isn't an associated regular expression for the component prefix.
         """
         component_info = self.get_component_info(reference)
         component = Component()
         component.reference = reference
-        component.nodes = component_info['nodes']
+        component.ports = component_info['nodes'].split()
         for attr in component_info:
             if attr not in ('designator', 'nodes'):
                 component.attributes[attr] = component_info[attr]
         return component
 
     def get_component_attribute(self, reference: str, attribute: str) -> Optional[str]:
         """
```

### Comparing `spicelib-1.1.1/spicelib/log/logfile_data.py` & `spicelib-1.1.2/spicelib/log/logfile_data.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/log/ltsteps.py` & `spicelib-1.1.2/spicelib/log/ltsteps.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/log/qspice_log_reader.py` & `spicelib-1.1.2/spicelib/log/qspice_log_reader.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/log/semi_dev_op_reader.py` & `spicelib-1.1.2/spicelib/log/semi_dev_op_reader.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/raw/raw_classes.py` & `spicelib-1.1.2/spicelib/raw/raw_classes.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/raw/raw_convert.py` & `spicelib-1.1.2/spicelib/raw/raw_convert.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/raw/raw_read.py` & `spicelib-1.1.2/spicelib/raw/raw_read.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/raw/raw_write.py` & `spicelib-1.1.2/spicelib/raw/raw_write.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/scripts/asc_to_qsch.py` & `spicelib-1.1.2/spicelib/scripts/asc_to_qsch.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/scripts/asc_to_qsch_data.xml` & `spicelib-1.1.2/spicelib/scripts/asc_to_qsch_data.xml`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/scripts/histogram.py` & `spicelib-1.1.2/spicelib/scripts/histogram.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/scripts/ltsteps.py` & `spicelib-1.1.2/spicelib/scripts/ltsteps.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/scripts/rawplot.py` & `spicelib-1.1.2/spicelib/scripts/rawplot.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/scripts/readme_update.py` & `spicelib-1.1.2/spicelib/scripts/readme_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 except FileNotFoundError:
     print("File not found")
     exit(1)
 except Exception as e:
     print(f"Error reading file: {e}")
     exit(1)
 print(f"{len(readme_md)} lines read")
-in_statement_regex = re.compile(r"-- in (?P<path>.*?)(?P<loc>\s\[.*\])?$")
+in_statement_regex = re.compile(r"-- in (?P<path>.*?)(?P<loc>\s\[.*\])?\s*$")
 
 block_start = -1
 line_no = 0
 # detect python code blocks
 while line_no < len(readme_md):
     line = readme_md[line_no]
     if "```python" in line:
```

### Comparing `spicelib-1.1.1/spicelib/scripts/run_server.py` & `spicelib-1.1.2/spicelib/scripts/run_server.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/process_callback.py` & `spicelib-1.1.2/spicelib/sim/process_callback.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/run_task.py` & `spicelib-1.1.2/spicelib/sim/run_task.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/sim_runner.py` & `spicelib-1.1.2/spicelib/sim/sim_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,17 +189,17 @@
             self.simulator = simulator
         else:
             raise TypeError("Invalid simulator type.")
         _logger.info("SimRunner initialized")
 
     def __del__(self):
         """Class Destructor : Closes Everything"""
-        _logger.debug("Waiting for all spawned sim_tasks to finish.")
+        # _logger.debug("Waiting for all spawned sim_tasks to finish.")
         self.wait_completion(abort_all_on_timeout=True)  # Kill all pending simulations
-        _logger.debug("Exiting SimRunner")
+        # _logger.debug("Exiting SimRunner")
 
     def set_simulator(self, spice_tool: Type[Simulator]) -> None:
         """
         Manually overriding the simulator to be used.
 
         :param spice_tool: String containing the path to the spice tool to be used, or alternatively the Simulator
             object.
```

### Comparing `spicelib-1.1.1/spicelib/sim/sim_stepping.py` & `spicelib-1.1.2/spicelib/sim/sim_stepping.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/simulator.py` & `spicelib-1.1.2/spicelib/sim/simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/tookit/failure_modes.py` & `spicelib-1.1.2/spicelib/sim/tookit/failure_modes.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/tookit/fast_worst_case.py` & `spicelib-1.1.2/spicelib/sim/tookit/fast_worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/tookit/montecarlo.py` & `spicelib-1.1.2/spicelib/sim/tookit/montecarlo.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/tookit/quick_sensitivity_analysis.py` & `spicelib-1.1.2/spicelib/sim/tookit/quick_sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/tookit/sim_analysis.py` & `spicelib-1.1.2/spicelib/sim/tookit/sim_analysis.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/tookit/tolerance_deviations.py` & `spicelib-1.1.2/spicelib/sim/tookit/tolerance_deviations.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/sim/tookit/worst_case.py` & `spicelib-1.1.2/spicelib/sim/tookit/worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/simulators/ltspice_simulator.py` & `spicelib-1.1.2/spicelib/simulators/ltspice_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/simulators/ngspice_simulator.py` & `spicelib-1.1.2/spicelib/simulators/ngspice_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/simulators/qspice_simulator.py` & `spicelib-1.1.2/spicelib/simulators/qspice_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/simulators/xyce_simulator.py` & `spicelib-1.1.2/spicelib/simulators/xyce_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/utils/detect_encoding.py` & `spicelib-1.1.2/spicelib/utils/detect_encoding.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/spicelib/utils/sweep_iterators.py` & `spicelib-1.1.2/spicelib/utils/sweep_iterators.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 # Licence:     refer to the LICENSE file
 #
 # -------------------------------------------------------------------------------
 
 import math
 from typing import Union, Optional, Iterable
 
+__author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
+__copyright__ = "Copyright 2021, Fribourg Switzerland"
+
 __all__ = ['sweep', 'sweep_n', 'sweep_log', 'sweep_log_n']
 
+
 class BaseIterator(object):
     """Common implementation to all Iterator classes"""
 
     def __init__(self, start: Union[int, float], stop: Optional[Union[int, float]] = None, step: Union[int, float] = 1):
         if stop is None:
             self.stop = start
             self.start = 0
@@ -93,15 +97,14 @@
         [0.3, 0.5, 0.7, 0.9000000000000001, 1.1]
         >>> list(sweep_n(15, -15, 13))
         [15, 12.5, 10.0, 7.5, 5.0, 2.5, 0.0, -2.5, -5.0, -7.5, -10.0, -12.5, -15.0]
         """
     return sweep(start, stop, (stop-start)/(N-1))
 
 
-
 class sweep_log(BaseIterator):
     """
     Generator function to be used in logarithmic sweeps.
     Advantages towards the range python built-in functions_
     - Supports floating point arguments
     - Supports both up and down sweeps.
     Usage:
```

### Comparing `spicelib-1.1.1/spicelib.egg-info/PKG-INFO` & `spicelib-1.1.2/spicelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicelib
-Version: 1.1.1
+Version: 1.1.2
 Summary: A set of tools to Automate Spice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -1185,14 +1185,17 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 1.1.2
+  * Fixes on the readme_update.py script. Was not supporting spaces after the []
+  * Solving issue PyLTspice Issue #138. Hierarchical edits to ASC files are now supported.
 * Version 1.1.1
   * Supporting hierarchical edits on both QSpice and LTspice schematics
   * Skipping the need of the rich library on examples
   * Giving feedback on the search for symbols on the ASC to QSCH conversion
   * Improvement on Documentation
   * Adding examples and unittests on hiearchical edits
   * Giving access to hidden properties (asc_file_path in AscEditor and qsch_file_path in QschEditor)
```

### Comparing `spicelib-1.1.1/spicelib.egg-info/SOURCES.txt` & `spicelib-1.1.2/spicelib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 spicelib/client_server/sim_server.py
 spicelib/client_server/srv_sim_runner.py
 spicelib/editor/__init__.py
 spicelib/editor/asc_editor.py
 spicelib/editor/asy_reader.py
 spicelib/editor/base_editor.py
 spicelib/editor/base_schematic.py
+spicelib/editor/ltspice_utils.py
 spicelib/editor/qsch_editor.py
 spicelib/editor/spice_editor.py
 spicelib/log/__init__.py
 spicelib/log/logfile_data.py
 spicelib/log/ltsteps.py
 spicelib/log/qspice_log_reader.py
 spicelib/log/semi_dev_op_reader.py
```

### Comparing `spicelib-1.1.1/unittests/sweep_iterators_unittest.py` & `spicelib-1.1.2/unittests/sweep_iterators_unittest.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/unittests/test_asc_editor.py` & `spicelib-1.1.2/unittests/test_asc_editor.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/unittests/test_qsch_editor.py` & `spicelib-1.1.2/unittests/test_qsch_editor.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/unittests/test_qspice_rawread.py` & `spicelib-1.1.2/unittests/test_qspice_rawread.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/unittests/test_spice_editor.py` & `spicelib-1.1.2/unittests/test_spice_editor.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.1/unittests/test_spicelib.py` & `spicelib-1.1.2/unittests/test_spicelib.py`

 * *Files identical despite different names*

