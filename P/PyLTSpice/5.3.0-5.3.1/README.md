# Comparing `tmp/pyltspice-5.3.0.tar.gz` & `tmp/pyltspice-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyltspice-5.3.0.tar", last modified: Sun Apr 21 15:06:40 2024, max compression
+gzip compressed data, was "pyltspice-5.3.1.tar", last modified: Sun May  5 18:30:40 2024, max compression
```

## Comparing `pyltspice-5.3.0.tar` & `pyltspice-5.3.1.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.839309 pyltspice-5.3.0/
--rw-rw-rw-   0        0        0    35823 2023-08-06 15:17:19.000000 pyltspice-5.3.0/LICENSE
--rw-rw-rw-   0        0        0    69160 2024-04-21 15:06:40.839309 pyltspice-5.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.786970 pyltspice-5.3.0/PyLTSpice/
--rw-rw-rw-   0        0        0      789 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/Histogram.py
--rw-rw-rw-   0        0        0      809 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/LTSteps.py
--rw-rw-rw-   0        0        0     1856 2024-03-16 09:47:29.000000 pyltspice-5.3.0/PyLTSpice/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.795539 pyltspice-5.3.0/PyLTSpice/editor/
--rw-rw-rw-   0        0        0        0 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/editor/__init__.py
--rw-rw-rw-   0        0        0      904 2024-03-16 09:13:46.000000 pyltspice-5.3.0/PyLTSpice/editor/asc_editor.py
--rw-rw-rw-   0        0        0     1797 2024-03-16 09:13:46.000000 pyltspice-5.3.0/PyLTSpice/editor/spice_editor.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.800124 pyltspice-5.3.0/PyLTSpice/log/
--rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 pyltspice-5.3.0/PyLTSpice/log/__init__.py
--rw-rw-rw-   0        0        0      638 2024-03-16 09:16:16.000000 pyltspice-5.3.0/PyLTSpice/log/logfile_data.py
--rw-rw-rw-   0        0        0      728 2024-03-16 09:13:46.000000 pyltspice-5.3.0/PyLTSpice/log/ltsteps.py
--rw-rw-rw-   0        0        0      788 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/log/semi_dev_op_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.804375 pyltspice-5.3.0/PyLTSpice/raw/
--rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 pyltspice-5.3.0/PyLTSpice/raw/__init__.py
--rw-rw-rw-   0        0        0      813 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/raw/raw_classes.py
--rw-rw-rw-   0        0        0     9473 2024-03-16 09:14:55.000000 pyltspice-5.3.0/PyLTSpice/raw/raw_read.py
--rw-rw-rw-   0        0        0      870 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/raw/raw_write.py
--rw-rw-rw-   0        0        0      775 2023-10-16 16:10:21.000000 pyltspice-5.3.0/PyLTSpice/rawplot.py
--rw-rw-rw-   0        0        0      775 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/run_server.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.811574 pyltspice-5.3.0/PyLTSpice/sim/
--rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 pyltspice-5.3.0/PyLTSpice/sim/__init__.py
--rw-rw-rw-   0        0        0     1096 2024-03-16 09:16:49.000000 pyltspice-5.3.0/PyLTSpice/sim/ltspice_simulator.py
--rw-rw-rw-   0        0        0      797 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/sim/process_callback.py
--rw-rw-rw-   0        0        0    10830 2024-03-16 09:18:04.000000 pyltspice-5.3.0/PyLTSpice/sim/sim_batch.py
--rw-rw-rw-   0        0        0     7807 2024-03-16 09:18:04.000000 pyltspice-5.3.0/PyLTSpice/sim/sim_runner.py
--rw-rw-rw-   0        0        0     1618 2024-03-16 09:18:04.000000 pyltspice-5.3.0/PyLTSpice/sim/sim_stepping.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.814899 pyltspice-5.3.0/PyLTSpice/sim/tookit/
--rw-rw-rw-   0        0        0      766 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/sim/tookit/montecarlo.py
--rw-rw-rw-   0        0        0      771 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/sim/tookit/worst_case.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.818113 pyltspice-5.3.0/PyLTSpice/utils/
--rw-rw-rw-   0        0        0     1067 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/utils/detect_encoding.py
--rw-rw-rw-   0        0        0     4387 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/utils/sweep_iterators.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.837193 pyltspice-5.3.0/PyLTSpice.egg-info/
--rw-rw-rw-   0        0        0    69160 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1396 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       48 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    27231 2024-04-21 15:05:37.000000 pyltspice-5.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.831531 pyltspice-5.3.0/examples/
--rw-rw-rw-   0        0        0      799 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/ltsteps_example.py
--rw-rw-rw-   0        0        0     3152 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/raw_plotting.py
--rw-rw-rw-   0        0        0     3939 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/raw_write_example.py
--rw-rw-rw-   0        0        0     2449 2024-02-23 21:07:51.000000 pyltspice-5.3.0/examples/run_montecarlo.py
--rw-rw-rw-   0        0        0     1544 2024-02-15 09:12:22.000000 pyltspice-5.3.0/examples/run_worst_case.py
--rw-rw-rw-   0        0        0     1354 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_runner_asc_example.py
--rw-rw-rw-   0        0        0     2535 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_runner_callback_example.py
--rw-rw-rw-   0        0        0     2740 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_runner_callback_process_example.py
--rw-rw-rw-   0        0        0     1759 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_runner_example.py
--rw-rw-rw-   0        0        0     1175 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_stepper_example.py
--rw-rw-rw-   0        0        0      251 2024-02-15 09:34:35.000000 pyltspice-5.3.0/examples/spice_editor_example.py
--rw-rw-rw-   0        0        0     1095 2024-04-21 15:05:37.000000 pyltspice-5.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 15:06:40.840317 pyltspice-5.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.835547 pyltspice-5.3.0/unittests/
--rw-rw-rw-   0        0        0     6054 2023-09-02 12:26:10.000000 pyltspice-5.3.0/unittests/sweep_iterators_unittest.py
--rw-rw-rw-   0        0        0     3178 2024-04-21 15:05:37.000000 pyltspice-5.3.0/unittests/test_asc_editor.py
--rw-rw-rw-   0        0        0    19390 2024-03-10 16:30:27.000000 pyltspice-5.3.0/unittests/test_pyltspice.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.776052 pyltspice-5.3.1/
+-rw-rw-rw-   0        0        0    35823 2023-08-06 15:17:19.000000 pyltspice-5.3.1/LICENSE
+-rw-rw-rw-   0        0        0    70587 2024-05-05 18:30:40.776052 pyltspice-5.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.721049 pyltspice-5.3.1/PyLTSpice/
+-rw-rw-rw-   0        0        0      789 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/Histogram.py
+-rw-rw-rw-   0        0        0      809 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/LTSteps.py
+-rw-rw-rw-   0        0        0     1856 2024-03-16 09:47:29.000000 pyltspice-5.3.1/PyLTSpice/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.729615 pyltspice-5.3.1/PyLTSpice/editor/
+-rw-rw-rw-   0        0        0        0 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/editor/__init__.py
+-rw-rw-rw-   0        0        0      904 2024-03-16 09:13:46.000000 pyltspice-5.3.1/PyLTSpice/editor/asc_editor.py
+-rw-rw-rw-   0        0        0     1797 2024-03-16 09:13:46.000000 pyltspice-5.3.1/PyLTSpice/editor/spice_editor.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.734083 pyltspice-5.3.1/PyLTSpice/log/
+-rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 pyltspice-5.3.1/PyLTSpice/log/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-16 09:16:16.000000 pyltspice-5.3.1/PyLTSpice/log/logfile_data.py
+-rw-rw-rw-   0        0        0      728 2024-03-16 09:13:46.000000 pyltspice-5.3.1/PyLTSpice/log/ltsteps.py
+-rw-rw-rw-   0        0        0      788 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.739089 pyltspice-5.3.1/PyLTSpice/raw/
+-rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 pyltspice-5.3.1/PyLTSpice/raw/__init__.py
+-rw-rw-rw-   0        0        0      813 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     9473 2024-03-16 09:14:55.000000 pyltspice-5.3.1/PyLTSpice/raw/raw_read.py
+-rw-rw-rw-   0        0        0      870 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/raw/raw_write.py
+-rw-rw-rw-   0        0        0      775 2023-10-16 16:10:21.000000 pyltspice-5.3.1/PyLTSpice/rawplot.py
+-rw-rw-rw-   0        0        0      775 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/run_server.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.746159 pyltspice-5.3.1/PyLTSpice/sim/
+-rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 pyltspice-5.3.1/PyLTSpice/sim/__init__.py
+-rw-rw-rw-   0        0        0     1096 2024-03-16 09:16:49.000000 pyltspice-5.3.1/PyLTSpice/sim/ltspice_simulator.py
+-rw-rw-rw-   0        0        0      797 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/sim/process_callback.py
+-rw-rw-rw-   0        0        0    10830 2024-03-16 09:18:04.000000 pyltspice-5.3.1/PyLTSpice/sim/sim_batch.py
+-rw-rw-rw-   0        0        0     7807 2024-03-16 09:18:04.000000 pyltspice-5.3.1/PyLTSpice/sim/sim_runner.py
+-rw-rw-rw-   0        0        0     1618 2024-03-16 09:18:04.000000 pyltspice-5.3.1/PyLTSpice/sim/sim_stepping.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.749165 pyltspice-5.3.1/PyLTSpice/sim/tookit/
+-rw-rw-rw-   0        0        0      766 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/sim/tookit/montecarlo.py
+-rw-rw-rw-   0        0        0      771 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/sim/tookit/worst_case.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.751490 pyltspice-5.3.1/PyLTSpice/utils/
+-rw-rw-rw-   0        0        0     1067 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0     4387 2023-10-16 16:04:02.000000 pyltspice-5.3.1/PyLTSpice/utils/sweep_iterators.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.774052 pyltspice-5.3.1/PyLTSpice.egg-info/
+-rw-rw-rw-   0        0        0    70587 2024-05-05 18:30:40.000000 pyltspice-5.3.1/PyLTSpice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1459 2024-05-05 18:30:40.000000 pyltspice-5.3.1/PyLTSpice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:30:40.000000 pyltspice-5.3.1/PyLTSpice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 18:30:40.000000 pyltspice-5.3.1/PyLTSpice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       48 2024-05-05 18:30:40.000000 pyltspice-5.3.1/PyLTSpice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    28658 2024-05-05 18:22:47.000000 pyltspice-5.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.768460 pyltspice-5.3.1/examples/
+-rw-rw-rw-   0        0        0      799 2023-09-02 12:26:10.000000 pyltspice-5.3.1/examples/ltsteps_example.py
+-rw-rw-rw-   0        0        0     3152 2023-09-02 12:26:10.000000 pyltspice-5.3.1/examples/raw_plotting.py
+-rw-rw-rw-   0        0        0      463 2024-04-28 16:26:16.000000 pyltspice-5.3.1/examples/raw_read_example.py
+-rw-rw-rw-   0        0        0     4884 2024-04-28 16:57:18.000000 pyltspice-5.3.1/examples/raw_write_example.py
+-rw-rw-rw-   0        0        0     2449 2024-02-23 21:07:51.000000 pyltspice-5.3.1/examples/run_montecarlo.py
+-rw-rw-rw-   0        0        0     1544 2024-02-15 09:12:22.000000 pyltspice-5.3.1/examples/run_worst_case.py
+-rw-rw-rw-   0        0        0     1354 2023-09-02 12:26:10.000000 pyltspice-5.3.1/examples/sim_runner_asc_example.py
+-rw-rw-rw-   0        0        0     2605 2024-05-05 18:22:47.000000 pyltspice-5.3.1/examples/sim_runner_callback_example.py
+-rw-rw-rw-   0        0        0     2740 2023-09-02 12:26:10.000000 pyltspice-5.3.1/examples/sim_runner_callback_process_example.py
+-rw-rw-rw-   0        0        0     1759 2023-09-02 12:26:10.000000 pyltspice-5.3.1/examples/sim_runner_example.py
+-rw-rw-rw-   0        0        0     1175 2023-09-02 12:26:10.000000 pyltspice-5.3.1/examples/sim_stepper_example.py
+-rw-rw-rw-   0        0        0      251 2024-02-15 09:34:35.000000 pyltspice-5.3.1/examples/spice_editor_example.py
+-rw-rw-rw-   0        0        0     1280 2024-04-21 13:16:18.000000 pyltspice-5.3.1/examples/sub_circuit_asc_edits.py
+-rw-rw-rw-   0        0        0     1095 2024-05-05 18:22:47.000000 pyltspice-5.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:30:40.777051 pyltspice-5.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 18:30:40.773046 pyltspice-5.3.1/unittests/
+-rw-rw-rw-   0        0        0     6054 2023-09-02 12:26:10.000000 pyltspice-5.3.1/unittests/sweep_iterators_unittest.py
+-rw-rw-rw-   0        0        0     3178 2024-04-21 15:05:37.000000 pyltspice-5.3.1/unittests/test_asc_editor.py
+-rw-rw-rw-   0        0        0    19390 2024-03-10 16:30:27.000000 pyltspice-5.3.1/unittests/test_pyltspice.py
```

### Comparing `pyltspice-5.3.0/LICENSE` & `pyltspice-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PKG-INFO` & `pyltspice-5.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2050 794c  : 2.1..Name: PyL
 00000020: 5453 7069 6365 0d0a 5665 7273 696f 6e3a  TSpice..Version:
-00000030: 2035 2e33 2e30 0d0a 5375 6d6d 6172 793a   5.3.0..Summary:
+00000030: 2035 2e33 2e31 0d0a 5375 6d6d 6172 793a   5.3.1..Summary:
 00000040: 2041 2073 6574 206f 6620 746f 6f6c 7320   A set of tools 
 00000050: 746f 2041 7574 6f6d 6174 6520 4c54 5370  to Automate LTSp
 00000060: 6963 6520 7369 6d75 6c61 7469 6f6e 730d  ice simulations.
 00000070: 0a41 7574 686f 722d 656d 6169 6c3a 204e  .Author-email: N
 00000080: 756e 6f20 4272 756d 203c 6d65 406e 756e  uno Brum <me@nun
 00000090: 6f62 7275 6d2e 636f 6d3e 0d0a 4c69 6365  obrum.com>..Lice
 000000a0: 6e73 653a 2020 2020 2020 2020 2020 2020  nse:            
@@ -2614,15 +2614,15 @@
 0000a350: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
 0000a360: 3e3d 332e 380d 0a44 6573 6372 6970 7469  >=3.8..Descripti
 0000a370: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
 0000a380: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
 0000a390: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
 0000a3a0: 4345 4e53 450d 0a52 6571 7569 7265 732d  CENSE..Requires-
 0000a3b0: 4469 7374 3a20 7370 6963 656c 6962 3e3d  Dist: spicelib>=
-0000a3c0: 312e 312e 310d 0a0d 0a23 2052 4541 444d  1.1.1....# READM
+0000a3c0: 312e 312e 320d 0a0d 0a23 2052 4541 444d  1.1.2....# READM
 0000a3d0: 4520 230d 0a0d 0a50 794c 5453 7069 6365  E #....PyLTSpice
 0000a3e0: 2069 7320 6120 746f 6f6c 6368 6169 6e20   is a toolchain 
 0000a3f0: 6f66 2070 7974 686f 6e20 7574 696c 6974  of python utilit
 0000a400: 6965 7320 6465 7369 676e 2074 6f20 696e  ies design to in
 0000a410: 7465 7261 6374 2077 6974 6820 4c54 5370  teract with LTSp
 0000a420: 6963 6520 456c 6563 7472 6f6e 6963 2053  ice Electronic S
 0000a430: 696d 756c 6174 6f72 2e0d 0a49 7420 6973  imulator...It is
@@ -2840,1484 +2840,1573 @@
 0000b170: 746c 6962 2070 6c6f 740d 0a0d 0a60 6060  tlib plot....```
 0000b180: 7079 7468 6f6e 0d0a 6672 6f6d 2050 794c  python..from PyL
 0000b190: 5453 7069 6365 2069 6d70 6f72 7420 5261  TSpice import Ra
 0000b1a0: 7752 6561 640d 0a0d 0a66 726f 6d20 6d61  wRead....from ma
 0000b1b0: 7470 6c6f 746c 6962 2069 6d70 6f72 7420  tplotlib import 
 0000b1c0: 7079 706c 6f74 2061 7320 706c 740d 0a0d  pyplot as plt...
 0000b1d0: 0a4c 5452 203d 2052 6177 5265 6164 2822  .LTR = RawRead("
-0000b1e0: 5452 414e 202d 2053 5445 502e 7261 7722  TRAN - STEP.raw"
-0000b1f0: 290d 0a0d 0a70 7269 6e74 284c 5452 2e67  )....print(LTR.g
-0000b200: 6574 5f74 7261 6365 5f6e 616d 6573 2829  et_trace_names()
-0000b210: 290d 0a70 7269 6e74 284c 5452 2e67 6574  )..print(LTR.get
-0000b220: 5f72 6177 5f70 726f 7065 7274 7928 2929  _raw_property())
-0000b230: 0d0a 0d0a 4952 3120 3d20 4c54 522e 6765  ....IR1 = LTR.ge
-0000b240: 745f 7472 6163 6528 2249 2852 3129 2229  t_trace("I(R1)")
-0000b250: 0d0a 7820 3d20 4c54 522e 6765 745f 7472  ..x = LTR.get_tr
-0000b260: 6163 6528 2774 696d 6527 2920 2023 2047  ace('time')  # G
-0000b270: 6574 7320 7468 6520 7469 6d65 2061 7869  ets the time axi
-0000b280: 730d 0a73 7465 7073 203d 204c 5452 2e67  s..steps = LTR.g
-0000b290: 6574 5f73 7465 7073 2829 0d0a 666f 7220  et_steps()..for 
-0000b2a0: 7374 6570 2069 6e20 7261 6e67 6528 6c65  step in range(le
-0000b2b0: 6e28 7374 6570 7329 293a 0d0a 2020 2020  n(steps)):..    
-0000b2c0: 2320 7072 696e 7428 7374 6570 735b 7374  # print(steps[st
-0000b2d0: 6570 5d29 0d0a 2020 2020 706c 742e 706c  ep])..    plt.pl
-0000b2e0: 6f74 2878 2e67 6574 5f77 6176 6528 7374  ot(x.get_wave(st
-0000b2f0: 6570 292c 2049 5231 2e67 6574 5f77 6176  ep), IR1.get_wav
-0000b300: 6528 7374 6570 292c 206c 6162 656c 3d73  e(step), label=s
-0000b310: 7465 7073 5b73 7465 705d 290d 0a0d 0a70  teps[step])....p
-0000b320: 6c74 2e6c 6567 656e 6428 2920 2023 206f  lt.legend()  # o
-0000b330: 7264 6572 2061 206c 6567 656e 640d 0a70  rder a legend..p
-0000b340: 6c74 2e73 686f 7728 290d 0a60 6060 2020  lt.show()..```  
-0000b350: 200d 0a0d 0a23 2323 2052 6177 5772 6974   ....### RawWrit
-0000b360: 6520 2323 230d 0a0d 0a54 6865 2066 6f6c  e ###....The fol
-0000b370: 6c6f 7769 6e67 2065 7861 6d70 6c65 2077  lowing example w
-0000b380: 7269 7465 7320 6120 5241 5720 6669 6c65  rites a RAW file
-0000b390: 2077 6974 6820 6120 3320 6d69 6c6c 6973   with a 3 millis
-0000b3a0: 6563 6f6e 6473 2074 7261 6e73 6965 6e74  econds transient
-0000b3b0: 2073 696d 756c 6174 696f 6e20 7369 6e65   simulation sine
-0000b3c0: 2077 6974 6820 6120 3130 6b48 7a20 616e   with a 10kHz an
-0000b3d0: 6420 6120 636f 7369 6e65 2077 6974 680d  d a cosine with.
-0000b3e0: 0a39 2e39 3937 6b48 7a0d 0a0d 0a60 6060  .9.997kHz....```
-0000b3f0: 7079 7468 6f6e 0d0a 696d 706f 7274 206e  python..import n
-0000b400: 756d 7079 2061 7320 6e70 0d0a 6672 6f6d  umpy as np..from
-0000b410: 2050 794c 5453 7069 6365 2069 6d70 6f72   PyLTSpice impor
-0000b420: 7420 5472 6163 652c 2052 6177 5772 6974  t Trace, RawWrit
-0000b430: 650d 0a0d 0a4c 5720 3d20 5261 7757 7269  e....LW = RawWri
-0000b440: 7465 2866 6173 7461 6363 6573 3d46 616c  te(fastacces=Fal
-0000b450: 7365 290d 0a74 7820 3d20 5472 6163 6528  se)..tx = Trace(
-0000b460: 2774 696d 6527 2c20 6e70 2e61 7261 6e67  'time', np.arang
-0000b470: 6528 302e 302c 2033 652d 332c 2039 3937  e(0.0, 3e-3, 997
-0000b480: 452d 3131 2929 0d0a 7679 203d 2054 7261  E-11))..vy = Tra
-0000b490: 6365 2827 4e30 3031 272c 206e 702e 7369  ce('N001', np.si
-0000b4a0: 6e28 3220 2a20 6e70 2e70 6920 2a20 7478  n(2 * np.pi * tx
-0000b4b0: 2e64 6174 6120 2a20 3130 3030 3029 290d  .data * 10000)).
-0000b4c0: 0a76 7a20 3d20 5472 6163 6528 274e 3030  .vz = Trace('N00
-0000b4d0: 3227 2c20 6e70 2e63 6f73 2832 202a 206e  2', np.cos(2 * n
-0000b4e0: 702e 7069 202a 2074 782e 6461 7461 202a  p.pi * tx.data *
-0000b4f0: 2039 3937 3029 290d 0a4c 572e 6164 645f   9970))..LW.add_
-0000b500: 7472 6163 6528 7478 290d 0a4c 572e 6164  trace(tx)..LW.ad
-0000b510: 645f 7472 6163 6528 7679 290d 0a4c 572e  d_trace(vy)..LW.
-0000b520: 6164 645f 7472 6163 6528 767a 290d 0a4c  add_trace(vz)..L
-0000b530: 572e 7361 7665 2822 7465 7374 655f 736e  W.save("teste_sn
-0000b540: 6970 7065 7431 2e72 6177 2229 0d0a 6060  ippet1.raw")..``
-0000b550: 6020 2020 0d0a 0d0a 2323 2320 5370 6963  `   ....### Spic
-0000b560: 6545 6469 746f 722c 2041 7363 4564 6974  eEditor, AscEdit
-0000b570: 6f72 2061 6e64 2053 696d 5275 6e6e 6572  or and SimRunner
-0000b580: 2e70 7920 2323 230d 0a0d 0a54 6869 7320  .py ###....This 
-0000b590: 6d6f 6475 6c65 2069 7320 7573 6564 2074  module is used t
-0000b5a0: 6f20 6c61 756e 6368 204c 5453 5069 6365  o launch LTSPice
-0000b5b0: 2073 696d 756c 6174 696f 6e73 2e20 5265   simulations. Re
-0000b5c0: 7375 6c74 7320 7468 656e 2063 616e 2062  sults then can b
-0000b5d0: 6520 7072 6f63 6573 7365 6420 7769 7468  e processed with
-0000b5e0: 2065 6974 6865 7220 7468 6520 5261 7752   either the RawR
-0000b5f0: 6561 6420 6f72 2077 6974 6820 7468 650d  ead or with the.
-0000b600: 0a4c 5453 7465 7073 206d 6f64 756c 6520  .LTSteps module 
-0000b610: 746f 2072 6561 6420 7468 6520 6c6f 6720  to read the log 
-0000b620: 6669 6c65 2077 6869 6368 2063 616e 2063  file which can c
-0000b630: 6f6e 7461 696e 202e 4d45 4153 2072 6573  ontain .MEAS res
-0000b640: 756c 7473 2e0d 0a0d 0a54 6865 2073 6372  ults.....The scr
-0000b650: 6970 7420 7769 6c6c 2066 6972 7374 6c79  ipt will firstly
-0000b660: 2069 6e76 6f6b 6520 7468 6520 4c54 5370   invoke the LTSp
-0000b670: 6963 6520 696e 2063 6f6d 6d61 6e64 206c  ice in command l
-0000b680: 696e 6520 746f 2067 656e 6572 6174 6520  ine to generate 
-0000b690: 6120 6e65 746c 6973 742c 2061 6e64 2074  a netlist, and t
-0000b6a0: 6865 6e20 7468 6973 206e 6574 6c69 7374  hen this netlist
-0000b6b0: 2063 616e 2062 6520 7570 6461 7465 640d   can be updated.
-0000b6c0: 0a64 6972 6563 746c 7920 6279 2074 6865  .directly by the
-0000b6d0: 2073 6372 6970 742c 2069 6e20 6f72 6465   script, in orde
-0000b6e0: 7220 746f 2063 6861 6e67 6520 636f 6d70  r to change comp
-0000b6f0: 6f6e 656e 7420 7661 6c75 6573 2c20 7061  onent values, pa
-0000b700: 7261 6d65 7465 7273 206f 7220 7369 6d75  rameters or simu
-0000b710: 6c61 7469 6f6e 2063 6f6d 6d61 6e64 732e  lation commands.
-0000b720: 0d0a 0d0a 4865 7265 2066 6f6c 6c6f 7773  ....Here follows
-0000b730: 2061 6e20 6578 616d 706c 6520 6f66 206f   an example of o
-0000b740: 7065 7261 7469 6f6e 2e0d 0a0d 0a60 6060  peration.....```
-0000b750: 7079 7468 6f6e 0d0a 6672 6f6d 2050 794c  python..from PyL
-0000b760: 5453 7069 6365 2069 6d70 6f72 7420 5369  TSpice import Si
-0000b770: 6d52 756e 6e65 720d 0a66 726f 6d20 5079  mRunner..from Py
-0000b780: 4c54 5370 6963 6520 696d 706f 7274 2053  LTSpice import S
-0000b790: 7069 6365 4564 6974 6f72 0d0a 0d0a 2320  piceEditor....# 
-0000b7a0: 7365 6c65 6374 2073 7069 6365 206d 6f64  select spice mod
-0000b7b0: 656c 0d0a 4c54 4320 3d20 5369 6d52 756e  el..LTC = SimRun
-0000b7c0: 6e65 7228 6f75 7470 7574 5f66 6f6c 6465  ner(output_folde
-0000b7d0: 723d 272e 2f74 656d 7027 290d 0a4c 5443  r='./temp')..LTC
-0000b7e0: 2e63 7265 6174 655f 6e65 746c 6973 7428  .create_netlist(
-0000b7f0: 2742 6174 6368 5f54 6573 742e 6173 6327  'Batch_Test.asc'
-0000b800: 290d 0a6e 6574 6c69 7374 203d 2053 7069  )..netlist = Spi
-0000b810: 6365 4564 6974 6f72 2827 4261 7463 685f  ceEditor('Batch_
-0000b820: 5465 7374 2e6e 6574 2729 0d0a 2320 7365  Test.net')..# se
-0000b830: 7420 6465 6661 756c 7420 6172 6775 6d65  t default argume
-0000b840: 6e74 730d 0a6e 6574 6c69 7374 2e73 6574  nts..netlist.set
-0000b850: 5f70 6172 616d 6574 6572 7328 7265 733d  _parameters(res=
-0000b860: 302c 2063 6170 3d31 3030 652d 362c 2072  0, cap=100e-6, r
-0000b870: 756e 3d2d 3129 0d0a 6e65 746c 6973 742e  un=-1)..netlist.
-0000b880: 7365 745f 636f 6d70 6f6e 656e 745f 7661  set_component_va
-0000b890: 6c75 6528 2752 3227 2c20 2732 6b27 2920  lue('R2', '2k') 
-0000b8a0: 2023 204d 6f64 6966 7969 6e67 2074 6865   # Modifying the
-0000b8b0: 2076 616c 7565 206f 6620 6120 7265 7369   value of a resi
-0000b8c0: 7374 6f72 0d0a 6e65 746c 6973 742e 7365  stor..netlist.se
-0000b8d0: 745f 636f 6d70 6f6e 656e 745f 7661 6c75  t_component_valu
-0000b8e0: 6528 2752 3127 2c20 2734 6b27 290d 0a6e  e('R1', '4k')..n
-0000b8f0: 6574 6c69 7374 2e73 6574 5f65 6c65 6d65  etlist.set_eleme
-0000b900: 6e74 5f6d 6f64 656c 2827 5633 272c 2022  nt_model('V3', "
-0000b910: 5349 4e45 2830 2031 2033 6b20 3020 3020  SINE(0 1 3k 0 0 
-0000b920: 3029 2229 2020 2320 4d6f 6469 6679 696e  0)")  # Modifyin
-0000b930: 6720 7468 650d 0a6e 6574 6c69 7374 2e73  g the..netlist.s
-0000b940: 6574 5f63 6f6d 706f 6e65 6e74 5f76 616c  et_component_val
-0000b950: 7565 2827 5855 313a 4332 272c 2032 3065  ue('XU1:C2', 20e
-0000b960: 2d31 3229 2020 2320 6d6f 6469 6679 696e  -12)  # modifyin
-0000b970: 6720 6120 6465 6669 6e65 2073 696d 756c  g a define simul
-0000b980: 6174 696f 6e0d 0a6e 6574 6c69 7374 2e61  ation..netlist.a
-0000b990: 6464 5f69 6e73 7472 7563 7469 6f6e 7328  dd_instructions(
-0000b9a0: 0d0a 2020 2020 223b 2053 696d 756c 6174  ..    "; Simulat
-0000b9b0: 696f 6e20 7365 7474 696e 6773 222c 0d0a  ion settings",..
-0000b9c0: 2020 2020 222e 7361 7665 2056 2856 696e      ".save V(Vin
-0000b9d0: 2920 4928 5231 2922 2c0d 0a29 0d0a 0d0a  ) I(R1)",..)....
-0000b9e0: 666f 7220 6f70 616d 7020 696e 2028 2741  for opamp in ('A
-0000b9f0: 4437 3132 272c 2027 4144 3832 3027 293a  D712', 'AD820'):
-0000ba00: 0d0a 2020 2020 6e65 746c 6973 742e 7365  ..    netlist.se
-0000ba10: 745f 656c 656d 656e 745f 6d6f 6465 6c28  t_element_model(
-0000ba20: 2758 5531 272c 206f 7061 6d70 290d 0a20  'XU1', opamp).. 
-0000ba30: 2020 2066 6f72 2073 7570 706c 795f 766f     for supply_vo
-0000ba40: 6c74 6167 6520 696e 2028 352c 2031 302c  ltage in (5, 10,
-0000ba50: 2031 3529 3a0d 0a20 2020 2020 2020 206e   15):..        n
-0000ba60: 6574 6c69 7374 2e73 6574 5f63 6f6d 706f  etlist.set_compo
-0000ba70: 6e65 6e74 5f76 616c 7565 2827 5631 272c  nent_value('V1',
-0000ba80: 2073 7570 706c 795f 766f 6c74 6167 6529   supply_voltage)
-0000ba90: 0d0a 2020 2020 2020 2020 6e65 746c 6973  ..        netlis
-0000baa0: 742e 7365 745f 636f 6d70 6f6e 656e 745f  t.set_component_
-0000bab0: 7661 6c75 6528 2756 3227 2c20 2d73 7570  value('V2', -sup
-0000bac0: 706c 795f 766f 6c74 6167 6529 0d0a 2020  ply_voltage)..  
-0000bad0: 2020 2020 2020 7072 696e 7428 2273 696d        print("sim
-0000bae0: 756c 6174 696e 6720 4f70 416d 7022 2c20  ulating OpAmp", 
-0000baf0: 6f70 616d 702c 2022 566f 6c74 6167 6522  opamp, "Voltage"
-0000bb00: 2c20 7375 7070 6c79 5f76 6f6c 7461 6765  , supply_voltage
-0000bb10: 290d 0a20 2020 2020 2020 204c 5443 2e72  )..        LTC.r
-0000bb20: 756e 286e 6574 6c69 7374 290d 0a0d 0a66  un(netlist)....f
-0000bb30: 6f72 2072 6177 2c20 6c6f 6720 696e 204c  or raw, log in L
-0000bb40: 5443 3a0d 0a20 2020 2070 7269 6e74 2822  TC:..    print("
-0000bb50: 5261 7720 6669 6c65 3a20 2573 2c20 4c6f  Raw file: %s, Lo
-0000bb60: 6720 6669 6c65 3a20 2573 2220 2520 2872  g file: %s" % (r
-0000bb70: 6177 2c20 6c6f 6729 290d 0a20 2020 2023  aw, log))..    #
-0000bb80: 2064 6f20 736f 6d65 7468 696e 6720 7769   do something wi
-0000bb90: 7468 2074 6865 2064 6174 610d 0a20 2020  th the data..   
-0000bba0: 2023 2072 6177 5f64 6174 6120 3d20 5261   # raw_data = Ra
-0000bbb0: 7752 6561 6428 7261 7729 0d0a 2020 2020  wRead(raw)..    
-0000bbc0: 2320 6c6f 675f 6461 7461 203d 204c 5453  # log_data = LTS
-0000bbd0: 7465 7073 286c 6f67 290d 0a20 2020 2023  teps(log)..    #
-0000bbe0: 202e 2e2e 0d0a 0d0a 6e65 746c 6973 742e   .......netlist.
-0000bbf0: 7265 7365 745f 6e65 746c 6973 7428 290d  reset_netlist().
-0000bc00: 0a6e 6574 6c69 7374 2e61 6464 5f69 6e73  .netlist.add_ins
-0000bc10: 7472 7563 7469 6f6e 7328 0d0a 2020 2020  tructions(..    
-0000bc20: 223b 2053 696d 756c 6174 696f 6e20 7365  "; Simulation se
-0000bc30: 7474 696e 6773 222c 0d0a 2020 2020 222e  ttings",..    ".
-0000bc40: 6163 2064 6563 2033 3020 3130 2031 4d65  ac dec 30 10 1Me
-0000bc50: 6722 2c0d 0a20 2020 2022 2e6d 6561 7320  g",..    ".meas 
-0000bc60: 4143 2047 6169 6e20 4d41 5820 6d61 6728  AC Gain MAX mag(
-0000bc70: 5628 6f75 7429 2920 3b20 6669 6e64 2074  V(out)) ; find t
-0000bc80: 6865 2070 6561 6b20 7265 7370 6f6e 7365  he peak response
-0000bc90: 2061 6e64 2063 616c 6c20 6974 2022 2247   and call it ""G
-0000bca0: 6169 6e22 2222 2c0d 0a20 2020 2022 2e6d  ain""",..    ".m
-0000bcb0: 6561 7320 4143 2046 6375 7420 5452 4947  eas AC Fcut TRIG
-0000bcc0: 206d 6167 2856 286f 7574 2929 3d47 6169   mag(V(out))=Gai
-0000bcd0: 6e2f 7371 7274 2832 2920 4641 4c4c 3d6c  n/sqrt(2) FALL=l
-0000bce0: 6173 7422 0d0a 290d 0a0d 0a23 2053 696d  ast"..)....# Sim
-0000bcf0: 2053 7461 7469 7374 6963 730d 0a70 7269   Statistics..pri
-0000bd00: 6e74 2827 5375 6363 6573 7366 756c 2f54  nt('Successful/T
-0000bd10: 6f74 616c 2053 696d 756c 6174 696f 6e73  otal Simulations
-0000bd20: 3a20 2720 2b20 7374 7228 4c54 432e 6f6b  : ' + str(LTC.ok
-0000bd30: 5369 6d29 202b 2027 2f27 202b 2073 7472  Sim) + '/' + str
-0000bd40: 284c 5443 2e72 756e 6e6f 2929 0d0a 0d0a  (LTC.runno))....
-0000bd50: 656e 7465 7220 3d20 696e 7075 7428 2250  enter = input("P
-0000bd60: 7265 7373 2065 6e74 6572 2074 6f20 6465  ress enter to de
-0000bd70: 6c65 7465 2063 7265 6174 6564 2066 696c  lete created fil
-0000bd80: 6573 2229 0d0a 6966 2065 6e74 6572 203d  es")..if enter =
-0000bd90: 3d20 2727 3a0d 0a20 2020 204c 5443 2e66  = '':..    LTC.f
-0000bda0: 696c 655f 636c 6561 6e75 7028 290d 0a60  ile_cleanup()..`
-0000bdb0: 6060 0d0a 0d0a 5468 6520 6578 616d 706c  ``....The exampl
-0000bdc0: 6520 6162 6f76 6520 6973 2075 7369 6e67  e above is using
-0000bdd0: 2074 6865 2053 7069 6365 4564 6974 6f72   the SpiceEditor
-0000bde0: 2074 6f20 6372 6561 7465 2061 6e64 206d   to create and m
-0000bdf0: 6f64 6966 7920 6120 7370 6963 6520 6e65  odify a spice ne
-0000be00: 746c 6973 742c 2062 7574 2069 7420 6973  tlist, but it is
-0000be10: 2061 6c73 6f20 706f 7373 6962 6c65 2074   also possible t
-0000be20: 6f20 7573 6520 7468 650d 0a41 7363 4564  o use the..AscEd
-0000be30: 6974 6f72 2074 6f20 6469 7265 6374 6c79  itor to directly
-0000be40: 206d 6f64 6966 7920 7468 6520 2e61 7363   modify the .asc
-0000be50: 2066 696c 652e 2054 6865 2065 6469 7465   file. The edite
-0000be60: 6420 2e61 7363 2066 696c 6520 6361 6e20  d .asc file can 
-0000be70: 7468 656e 2062 6520 6f70 656e 6564 2062  then be opened b
-0000be80: 7920 7468 6520 4c54 5370 6963 6520 4755  y the LTSpice GU
-0000be90: 4920 616e 6420 7468 650d 0a73 696d 756c  I and the..simul
-0000bea0: 6174 696f 6e20 6361 6e20 6265 2072 756e  ation can be run
-0000beb0: 2066 726f 6d20 7468 6572 652e 0d0a 0d0a   from there.....
-0000bec0: 2323 2320 5369 6d75 6c61 7469 6f6e 2041  ### Simulation A
-0000bed0: 6e61 6c79 7369 7320 546f 6f6c 6b69 7420  nalysis Toolkit 
-0000bee0: 2323 230d 0a0d 0a54 6865 2041 7363 4564  ###....The AscEd
-0000bef0: 6974 6f72 2063 616e 2062 6520 7573 6564  itor can be used
-0000bf00: 2077 6974 6820 7468 6520 5369 6d75 6c61   with the Simula
-0000bf10: 7469 6f6e 2041 6e61 6c79 7369 7320 546f  tion Analysis To
-0000bf20: 6f6c 6b69 7420 746f 2070 6572 666f 726d  olkit to perform
-0000bf30: 204d 6f6e 7465 2043 6172 6c6f 206f 7220   Monte Carlo or 
-0000bf40: 576f 7374 2043 6173 6520 7369 6d75 6c61  Wost Case simula
-0000bf50: 7469 6f6e 732e 0d0a 5468 6573 6520 7369  tions...These si
-0000bf60: 6d75 6c61 7469 6f6e 7320 6361 6e20 6569  mulations can ei
-0000bf70: 7468 6572 2062 6520 646f 6e65 206f 6e20  ther be done on 
-0000bf80: 7468 6520 4c54 5370 6963 6520 4755 4920  the LTSpice GUI 
-0000bf90: 6f72 2075 7369 6e67 2074 6865 2052 756e  or using the Run
-0000bfa0: 6e65 7220 436c 6173 7320 6465 7363 7269  ner Class descri
-0000bfb0: 6265 6420 6162 6f76 652e 0d0a 0d0a 4c65  bed above.....Le
-0000bfc0: 7427 7320 636f 6e73 6964 6572 2074 6865  t's consider the
-0000bfd0: 2066 6f6c 6c6f 7769 6e67 2063 6972 6375   following circu
-0000bfe0: 6974 3a0d 0a0d 0a21 5b53 616c 6c65 6e2d  it:....![Sallen-
-0000bff0: 4b65 7920 416d 706c 6966 6965 725d 282e  Key Amplifier](.
-0000c000: 2f64 6f63 2f6d 6f64 756c 6573 2f73 616c  /doc/modules/sal
-0000c010: 6c65 6e6b 6579 2e70 6e67 2022 5361 6c6c  lenkey.png "Sall
-0000c020: 656e 2d4b 6579 2041 6d70 6c69 6669 6572  en-Key Amplifier
-0000c030: 2229 0d0a 0d0a 5768 656e 2070 6572 666f  ")....When perfo
-0000c040: 726d 696e 6720 6120 4d6f 6e74 6520 4361  rming a Monte Ca
-0000c050: 726c 6f20 7369 6d75 6c61 7469 6f6e 206f  rlo simulation o
-0000c060: 6e20 7468 6973 2063 6972 6375 6974 2c20  n this circuit, 
-0000c070: 7765 206e 6565 6420 746f 206d 616e 7561  we need to manua
-0000c080: 6c6c 7920 6d6f 6469 6679 2074 6865 2076  lly modify the v
-0000c090: 616c 7565 206f 6620 6561 6368 2063 6f6d  alue of each com
-0000c0a0: 706f 6e65 6e74 2c20 0d0a 616e 6420 7468  ponent, ..and th
-0000c0b0: 656e 2061 6464 2074 6865 202e 7374 6570  en add the .step
-0000c0c0: 2063 6f6d 6d61 6e64 2066 6f72 206d 616b   command for mak
-0000c0d0: 696e 6720 7365 7665 7261 6c20 7275 6e73  ing several runs
-0000c0e0: 206f 6e20 7468 6520 7361 6d65 2063 6972   on the same cir
-0000c0f0: 6375 6974 2e20 0d0a 546f 2073 696d 706c  cuit. ..To simpl
-0000c100: 6966 7920 7468 6973 2070 726f 6365 7373  ify this process
-0000c110: 2c20 7468 6520 4173 6345 6469 746f 7220  , the AscEditor 
-0000c120: 636c 6173 7320 6361 6e20 6265 2075 7365  class can be use
-0000c130: 6420 6173 2065 7865 6d70 6c69 6669 6564  d as exemplified
-0000c140: 2062 656c 6f77 3a0d 0a0d 0a60 6060 7079   below:....```py
-0000c150: 7468 6f6e 0d0a 6672 6f6d 2050 794c 5453  thon..from PyLTS
-0000c160: 7069 6365 2069 6d70 6f72 7420 4173 6345  pice import AscE
-0000c170: 6469 746f 722c 2053 696d 5275 6e6e 6572  ditor, SimRunner
-0000c180: 2020 2320 496d 706f 7274 7320 7468 6520    # Imports the 
-0000c190: 636c 6173 7320 7468 6174 206d 616e 6970  class that manip
-0000c1a0: 756c 6174 6573 2074 6865 2061 7363 2066  ulates the asc f
-0000c1b0: 696c 650d 0a66 726f 6d20 5079 4c54 5370  ile..from PyLTSp
-0000c1c0: 6963 652e 7369 6d2e 746f 6f6b 6974 2e6d  ice.sim.tookit.m
-0000c1d0: 6f6e 7465 6361 726c 6f20 696d 706f 7274  ontecarlo import
-0000c1e0: 204d 6f6e 7465 6361 726c 6f20 2023 2049   Montecarlo  # I
-0000c1f0: 6d70 6f72 7473 2074 6865 204d 6f6e 7465  mports the Monte
-0000c200: 6361 726c 6f20 746f 6f6c 6b69 7420 636c  carlo toolkit cl
-0000c210: 6173 730d 0a0d 0a73 616c 6c65 6e6b 6579  ass....sallenkey
-0000c220: 203d 2041 7363 4564 6974 6f72 2822 2e2f   = AscEditor("./
-0000c230: 7465 7374 6669 6c65 732f 7361 6c6c 656e  testfiles/sallen
-0000c240: 6b65 792e 6173 6322 2920 2023 2052 6561  key.asc")  # Rea
-0000c250: 6473 2074 6865 2061 7363 2066 696c 6520  ds the asc file 
-0000c260: 696e 746f 206d 656d 6f72 790d 0a72 756e  into memory..run
-0000c270: 6e65 7220 3d20 5369 6d52 756e 6e65 7228  ner = SimRunner(
-0000c280: 6f75 7470 7574 5f66 6f6c 6465 723d 272e  output_folder='.
-0000c290: 2f74 656d 705f 6d63 2729 2020 2320 496e  /temp_mc')  # In
-0000c2a0: 7374 616e 7469 6174 6573 2074 6865 2072  stantiates the r
-0000c2b0: 756e 6e65 7220 636c 6173 732c 2077 6974  unner class, wit
-0000c2c0: 6820 7468 6520 6f75 7470 7574 2066 6f6c  h the output fol
-0000c2d0: 6465 7220 616c 7265 6164 7920 7365 740d  der already set.
-0000c2e0: 0a6d 6320 3d20 4d6f 6e74 6563 6172 6c6f  .mc = Montecarlo
-0000c2f0: 2873 616c 6c65 6e6b 6579 2c20 7275 6e6e  (sallenkey, runn
-0000c300: 6572 2920 2023 2049 6e73 7461 6e74 6961  er)  # Instantia
-0000c310: 7465 7320 7468 6520 4d6f 6e74 6563 6172  tes the Montecar
-0000c320: 6c6f 2063 6c61 7373 2c20 7769 7468 2074  lo class, with t
-0000c330: 6865 2061 7363 2066 696c 6520 616c 7265  he asc file alre
-0000c340: 6164 7920 696e 206d 656d 6f72 790d 0a0d  ady in memory...
-0000c350: 0a23 2054 6865 2066 6f6c 6c6f 7769 6e67  .# The following
-0000c360: 206c 696e 6573 2073 6574 2074 6865 2064   lines set the d
-0000c370: 6566 6175 6c74 2074 6f6c 6572 616e 6365  efault tolerance
-0000c380: 7320 666f 7220 7468 6520 636f 6d70 6f6e  s for the compon
-0000c390: 656e 7473 0d0a 6d63 2e73 6574 5f74 6f6c  ents..mc.set_tol
-0000c3a0: 6572 616e 6365 2827 5227 2c20 302e 3031  erance('R', 0.01
-0000c3b0: 2920 2023 2031 2520 746f 6c65 7261 6e63  )  # 1% toleranc
-0000c3c0: 652c 2064 6566 6175 6c74 2064 6973 7472  e, default distr
-0000c3d0: 6962 7574 696f 6e20 6973 2075 6e69 666f  ibution is unifo
-0000c3e0: 726d 0d0a 6d63 2e73 6574 5f74 6f6c 6572  rm..mc.set_toler
-0000c3f0: 616e 6365 2827 4327 2c20 302e 312c 2064  ance('C', 0.1, d
-0000c400: 6973 7472 6962 7574 696f 6e3d 2775 6e69  istribution='uni
-0000c410: 666f 726d 2729 2020 2320 3130 2520 746f  form')  # 10% to
-0000c420: 6c65 7261 6e63 652c 2065 7870 6c69 6369  lerance, explici
-0000c430: 7420 756e 6966 6f72 6d20 6469 7374 7269  t uniform distri
-0000c440: 6275 7469 6f6e 0d0a 6d63 2e73 6574 5f74  bution..mc.set_t
-0000c450: 6f6c 6572 616e 6365 2827 5627 2c20 302e  olerance('V', 0.
-0000c460: 312c 2064 6973 7472 6962 7574 696f 6e3d  1, distribution=
-0000c470: 276e 6f72 6d61 6c27 2920 2023 2031 3025  'normal')  # 10%
-0000c480: 2074 6f6c 6572 616e 6365 2c20 6275 7420   tolerance, but 
-0000c490: 7573 696e 6720 6120 6e6f 726d 616c 2064  using a normal d
-0000c4a0: 6973 7472 6962 7574 696f 6e0d 0a0d 0a23  istribution....#
-0000c4b0: 2053 6f6d 6520 636f 6d70 6f6e 656e 7473   Some components
-0000c4c0: 2063 616e 2068 6176 6520 6120 6469 6666   can have a diff
-0000c4d0: 6572 656e 7420 746f 6c65 7261 6e63 650d  erent tolerance.
-0000c4e0: 0a6d 632e 7365 745f 746f 6c65 7261 6e63  .mc.set_toleranc
-0000c4f0: 6528 2752 3127 2c20 302e 3035 2920 2023  e('R1', 0.05)  #
-0000c500: 2035 2520 746f 6c65 7261 6e63 6520 666f   5% tolerance fo
-0000c510: 7220 5231 206f 6e6c 792e 2054 6869 7320  r R1 only. This 
-0000c520: 6f6e 6c79 206f 7665 7272 6964 6573 2074  only overrides t
-0000c530: 6865 2064 6566 6175 6c74 2074 6f6c 6572  he default toler
-0000c540: 616e 6365 2066 6f72 2052 310d 0a0d 0a23  ance for R1....#
-0000c550: 2054 6f6c 6572 616e 6365 7320 6361 6e20   Tolerances can 
-0000c560: 6265 2073 6574 2066 6f72 2070 6172 616d  be set for param
-0000c570: 6574 6572 7320 6173 2077 656c 6c0d 0a6d  eters as well..m
-0000c580: 632e 7365 745f 7061 7261 6d65 7465 725f  c.set_parameter_
-0000c590: 6465 7669 6174 696f 6e28 2756 6f73 272c  deviation('Vos',
-0000c5a0: 2033 652d 342c 2035 652d 332c 2027 756e   3e-4, 5e-3, 'un
-0000c5b0: 6966 6f72 6d27 2920 2023 2054 6865 206b  iform')  # The k
-0000c5c0: 6579 776f 7264 2027 6469 7374 7269 6275  eyword 'distribu
-0000c5d0: 7469 6f6e 2720 6973 206f 7074 696f 6e61  tion' is optiona
-0000c5e0: 6c0d 0a6d 632e 7072 6570 6172 655f 7465  l..mc.prepare_te
-0000c5f0: 7374 6265 6e63 6828 6e75 6d5f 7275 6e73  stbench(num_runs
-0000c600: 3d31 3030 3029 2020 2320 5072 6570 6172  =1000)  # Prepar
-0000c610: 6573 2074 6865 2074 6573 7462 656e 6368  es the testbench
-0000c620: 2066 6f72 2031 3030 3020 7369 6d75 6c61   for 1000 simula
-0000c630: 7469 6f6e 730d 0a0d 0a23 2046 696e 616c  tions....# Final
-0000c640: 6c79 2074 6865 206e 6574 6c69 7374 2069  ly the netlist i
-0000c650: 7320 7361 7665 6420 746f 2061 2066 696c  s saved to a fil
-0000c660: 650d 0a6d 632e 7361 7665 5f6e 6574 6c69  e..mc.save_netli
-0000c670: 7374 2827 2e2f 7465 7374 6669 6c65 732f  st('./testfiles/
-0000c680: 7361 6c6c 656e 6b65 795f 6d63 2e6e 6574  sallenkey_mc.net
-0000c690: 2729 0d0a 0d0a 6d63 2e72 756e 2831 3030  ')....mc.run(100
-0000c6a0: 2920 2023 2052 756e 7320 7468 6520 7369  )  # Runs the si
-0000c6b0: 6d75 6c61 7469 6f6e 2077 6974 6820 7370  mulation with sp
-0000c6c0: 6c69 7473 206f 6620 3130 3020 7275 6e73  lits of 100 runs
-0000c6d0: 2065 6163 680d 0a6c 6f67 7320 3d20 6d63   each..logs = mc
-0000c6e0: 2e72 6561 645f 6c6f 6766 696c 6573 2829  .read_logfiles()
-0000c6f0: 2020 2023 2052 6561 6473 2074 6865 206c     # Reads the l
-0000c700: 6f67 2066 696c 6573 2061 6e64 2073 746f  og files and sto
-0000c710: 7265 7320 7468 6520 7265 7375 6c74 7320  res the results 
-0000c720: 696e 2074 6865 2072 6573 756c 7473 2061  in the results a
-0000c730: 7474 7269 6275 7465 0d0a 6c6f 6773 2e65  ttribute..logs.e
-0000c740: 7870 6f72 745f 6461 7461 2827 2e2f 7465  xport_data('./te
-0000c750: 6d70 5f6d 632f 6461 7461 2e63 7376 2729  mp_mc/data.csv')
-0000c760: 2020 2320 4578 706f 7274 7320 7468 6520    # Exports the 
-0000c770: 6461 7461 2074 6f20 6120 6373 7620 6669  data to a csv fi
-0000c780: 6c65 0d0a 6c6f 6773 2e70 6c6f 745f 6869  le..logs.plot_hi
-0000c790: 7374 6f67 7261 6d28 2766 6375 7427 2920  stogram('fcut') 
-0000c7a0: 2023 2050 6c6f 7473 2074 6865 2068 6973   # Plots the his
-0000c7b0: 746f 6772 616d 7320 666f 7220 7468 6520  tograms for the 
-0000c7c0: 7265 7375 6c74 730d 0a6d 632e 636c 6561  results..mc.clea
-0000c7d0: 6e75 705f 6669 6c65 7328 2920 2023 2044  nup_files()  # D
-0000c7e0: 656c 6574 6573 2074 6865 2074 656d 706f  eletes the tempo
-0000c7f0: 7261 7279 2066 696c 6573 0d0a 6060 600d  rary files..```.
-0000c800: 0a57 6865 6e20 6f70 656e 696e 6720 7468  .When opening th
-0000c810: 6520 6372 6561 7465 6420 7361 6c6c 656e  e created sallen
-0000c820: 6b65 795f 6d63 2e6e 6574 2066 696c 652c  key_mc.net file,
-0000c830: 2077 6520 6361 6e20 7365 6520 7468 6174   we can see that
-0000c840: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-0000c850: 6972 6375 6974 2e0d 0a0d 0a21 5b53 616c  ircuit.....![Sal
-0000c860: 6c65 6e2d 4b65 7920 416d 706c 6966 6965  len-Key Amplifie
-0000c870: 7220 7769 7468 204d 6f6e 7465 6361 726c  r with Montecarl
-0000c880: 6f5d 282e 2f64 6f63 2f6d 6f64 756c 6573  o](./doc/modules
-0000c890: 2f73 616c 6c65 6e6b 6579 5f6d 632e 706e  /sallenkey_mc.pn
-0000c8a0: 6720 2253 616c 6c65 6e2d 4b65 7920 416d  g "Sallen-Key Am
-0000c8b0: 706c 6966 6965 7220 7769 7468 204d 6f6e  plifier with Mon
-0000c8c0: 7465 6361 726c 6f22 290d 0a0d 0a54 6865  tecarlo")....The
-0000c8d0: 2066 6f6c 6c6f 7769 6e67 2075 7064 6174   following updat
-0000c8e0: 6573 2077 6572 6520 6d61 6465 2074 6f20  es were made to 
-0000c8f0: 7468 6520 6369 7263 7569 743a 0d0a 2d20  the circuit:..- 
-0000c900: 5468 6520 7661 6c75 6520 6f66 2065 6163  The value of eac
-0000c910: 6820 636f 6d70 6f6e 656e 7420 7761 7320  h component was 
-0000c920: 7265 706c 6163 6564 2062 7920 6120 6675  replaced by a fu
-0000c930: 6e63 7469 6f6e 2074 6861 7420 6765 6e65  nction that gene
-0000c940: 7261 7465 7320 6120 7261 6e64 6f6d 2076  rates a random v
-0000c950: 616c 7565 2077 6974 6869 6e20 7468 6520  alue within the 
-0000c960: 7370 6563 6966 6965 6420 746f 6c65 7261  specified tolera
-0000c970: 6e63 652e 0d0a 2d20 5468 6520 2e73 7465  nce...- The .ste
-0000c980: 7020 7061 7261 6d20 7275 6e20 636f 6d6d  p param run comm
-0000c990: 616e 6420 7761 7320 6164 6465 6420 746f  and was added to
-0000c9a0: 2074 6865 206e 6574 6c69 7374 2e20 5374   the netlist. St
-0000c9b0: 6172 7473 2061 7420 2d31 2077 6869 6368  arts at -1 which
-0000c9c0: 2069 7427 7320 7468 6520 6e6f 6d69 6e61   it's the nomina
-0000c9d0: 6c20 7661 6c75 6520 7369 6d75 6c61 7469  l value simulati
-0000c9e0: 6f6e 2c20 616e 6420 0d0a 6669 6e69 7368  on, and ..finish
-0000c9f0: 6573 2074 6861 7420 7468 6520 6e75 6d62  es that the numb
-0000ca00: 6572 206f 6620 7369 6d75 6c61 7469 6f6e  er of simulation
-0000ca10: 7320 7370 6563 6966 6965 6420 696e 2074  s specified in t
-0000ca20: 6865 2070 7265 7061 7265 5f74 6573 7462  he prepare_testb
-0000ca30: 656e 6368 2829 206d 6574 686f 642e 0d0a  ench() method...
-0000ca40: 2d20 4120 6465 6661 756c 7420 7661 6c75  - A default valu
-0000ca50: 6520 666f 7220 7468 6520 7275 6e20 7061  e for the run pa
-0000ca60: 7261 6d65 7465 7220 7761 7320 6164 6465  rameter was adde
-0000ca70: 642e 2054 6869 7320 6973 2075 7365 6675  d. This is usefu
-0000ca80: 6c20 6966 2074 6865 202e 7374 6570 2070  l if the .step p
-0000ca90: 6172 616d 2072 756e 2069 7320 636f 6d6d  aram run is comm
-0000caa0: 656e 7465 6420 6f75 742e 0d0a 2d20 5468  ented out...- Th
-0000cab0: 6520 5231 2074 6f6c 6572 616e 6365 2069  e R1 tolerance i
-0000cac0: 7320 6469 6666 6572 656e 7420 6672 6f6d  s different from
-0000cad0: 2074 6865 206f 7468 6572 2072 6573 6973   the other resis
-0000cae0: 746f 7273 2e20 5468 6973 2069 7320 6265  tors. This is be
-0000caf0: 6361 7573 6520 7468 6520 746f 6c65 7261  cause the tolera
-0000cb00: 6e63 6520 7761 7320 6578 706c 6963 6974  nce was explicit
-0000cb10: 6c79 2073 6574 2066 6f72 2052 312e 0d0a  ly set for R1...
-0000cb20: 2d20 5468 6520 566f 7320 7061 7261 6d65  - The Vos parame
-0000cb30: 7465 7220 7761 7320 6164 6465 6420 746f  ter was added to
-0000cb40: 2074 6865 202e 7061 7261 6d20 6c69 7374   the .param list
-0000cb50: 2e20 5468 6973 2069 7320 6265 6361 7573  . This is becaus
-0000cb60: 6520 7468 6520 7061 7261 6d65 7465 7220  e the parameter 
-0000cb70: 7761 7320 6578 706c 6963 6974 6c79 2073  was explicitly s
-0000cb80: 6574 2075 7369 6e67 2074 6865 0d0a 7365  et using the..se
-0000cb90: 745f 7061 7261 6d65 7465 725f 6465 7669  t_parameter_devi
-0000cba0: 6174 696f 6e20 6d65 7468 6f64 2e0d 0a2d  ation method...-
-0000cbb0: 2046 756e 6374 696f 6e73 2075 746f 6c2c   Functions utol,
-0000cbc0: 206e 746f 6c20 616e 6420 7572 6e67 2077   ntol and urng w
-0000cbd0: 6572 6520 6164 6465 6420 746f 2074 6865  ere added to the
-0000cbe0: 202e 6675 6e63 206c 6973 742e 2054 6865   .func list. The
-0000cbf0: 7365 2066 756e 6374 696f 6e73 2061 7265  se functions are
-0000cc00: 2075 7365 6420 746f 2067 656e 6572 6174   used to generat
-0000cc10: 6520 7261 6e64 6f6d 2076 616c 7565 732e  e random values.
-0000cc20: 0d0a 556e 6966 6f72 6d20 6469 7374 7269  ..Uniform distri
-0000cc30: 6275 7469 6f6e 7320 7573 6520 7468 6520  butions use the 
-0000cc40: 4c54 5370 6963 6520 6275 696c 742d 696e  LTSpice built-in
-0000cc50: 206d 6328 782c 2074 6f6c 2920 616e 6420   mc(x, tol) and 
-0000cc60: 666c 6174 2878 2920 6675 6e63 7469 6f6e  flat(x) function
-0000cc70: 732c 2077 6869 6c65 206e 6f72 6d61 6c20  s, while normal 
-0000cc80: 6469 7374 7269 6275 7469 6f6e 7320 7573  distributions us
-0000cc90: 6520 7468 6520 0d0a 6761 7573 7328 7829  e the ..gauss(x)
-0000cca0: 2066 756e 6374 696f 6e2e 0d0a 0d0a 5369   function.....Si
-0000ccb0: 6d69 6c61 726c 792c 2074 6865 2077 6f72  milarly, the wor
-0000ccc0: 7374 2063 6173 6520 616e 616c 7973 6973  st case analysis
-0000ccd0: 2063 616e 2061 6c73 6f20 6265 2073 6574   can also be set
-0000cce0: 7570 2062 7920 7573 696e 6720 7468 6520  up by using the 
-0000ccf0: 636c 6173 7320 576f 7273 7443 6173 6541  class WorstCaseA
-0000cd00: 6e61 6c79 7369 732c 2061 7320 6578 656d  nalysis, as exem
-0000cd10: 706c 6966 6965 6420 6265 6c6f 773a 0d0a  plified below:..
-0000cd20: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-0000cd30: 6d20 5079 4c54 5370 6963 6520 696d 706f  m PyLTSpice impo
-0000cd40: 7274 2041 7363 4564 6974 6f72 2c20 5369  rt AscEditor, Si
-0000cd50: 6d52 756e 6e65 7220 2023 2049 6d70 6f72  mRunner  # Impor
-0000cd60: 7473 2074 6865 2063 6c61 7373 2074 6861  ts the class tha
-0000cd70: 7420 6d61 6e69 7075 6c61 7465 7320 7468  t manipulates th
-0000cd80: 6520 6173 6320 6669 6c65 0d0a 6672 6f6d  e asc file..from
-0000cd90: 2050 794c 5453 7069 6365 2e73 696d 2e74   PyLTSpice.sim.t
-0000cda0: 6f6f 6b69 742e 776f 7273 745f 6361 7365  ookit.worst_case
-0000cdb0: 2069 6d70 6f72 7420 576f 7273 7443 6173   import WorstCas
-0000cdc0: 6541 6e61 6c79 7369 730d 0a0d 0a73 616c  eAnalysis....sal
-0000cdd0: 6c65 6e6b 6579 203d 2041 7363 4564 6974  lenkey = AscEdit
-0000cde0: 6f72 2822 2e2f 7465 7374 6669 6c65 732f  or("./testfiles/
-0000cdf0: 7361 6c6c 656e 6b65 792e 6173 6322 2920  sallenkey.asc") 
-0000ce00: 2023 2052 6561 6473 2074 6865 2061 7363   # Reads the asc
-0000ce10: 2066 696c 6520 696e 746f 206d 656d 6f72   file into memor
-0000ce20: 790d 0a72 756e 6e65 7220 3d20 5369 6d52  y..runner = SimR
-0000ce30: 756e 6e65 7228 6f75 7470 7574 5f66 6f6c  unner(output_fol
-0000ce40: 6465 723d 272e 2f74 656d 705f 7763 6127  der='./temp_wca'
-0000ce50: 2920 2023 2049 6e73 7461 6e74 6961 7465  )  # Instantiate
-0000ce60: 7320 7468 6520 7275 6e6e 6572 2063 6c61  s the runner cla
-0000ce70: 7373 2c20 7769 7468 2074 6865 206f 7574  ss, with the out
-0000ce80: 7075 7420 666f 6c64 6572 2061 6c72 6561  put folder alrea
-0000ce90: 6479 2073 6574 0d0a 7763 6120 3d20 576f  dy set..wca = Wo
-0000cea0: 7273 7443 6173 6541 6e61 6c79 7369 7328  rstCaseAnalysis(
-0000ceb0: 7361 6c6c 656e 6b65 792c 2072 756e 6e65  sallenkey, runne
-0000cec0: 7229 2020 2320 496e 7374 616e 7469 6174  r)  # Instantiat
-0000ced0: 6573 2074 6865 2057 6f72 7374 2043 6173  es the Worst Cas
-0000cee0: 6520 416e 616c 7973 6973 2063 6c61 7373  e Analysis class
-0000cef0: 0d0a 0d0a 2320 5468 6520 666f 6c6c 6f77  ....# The follow
-0000cf00: 696e 6720 6c69 6e65 7320 7365 7420 7468  ing lines set th
-0000cf10: 6520 6465 6661 756c 7420 746f 6c65 7261  e default tolera
-0000cf20: 6e63 6573 2066 6f72 2074 6865 2063 6f6d  nces for the com
-0000cf30: 706f 6e65 6e74 730d 0a77 6361 2e73 6574  ponents..wca.set
-0000cf40: 5f74 6f6c 6572 616e 6365 2827 5227 2c20  _tolerance('R', 
-0000cf50: 302e 3031 2920 2023 2031 2520 746f 6c65  0.01)  # 1% tole
-0000cf60: 7261 6e63 650d 0a77 6361 2e73 6574 5f74  rance..wca.set_t
-0000cf70: 6f6c 6572 616e 6365 2827 4327 2c20 302e  olerance('C', 0.
-0000cf80: 3129 2020 2320 3130 2520 746f 6c65 7261  1)  # 10% tolera
-0000cf90: 6e63 650d 0a77 6361 2e73 6574 5f74 6f6c  nce..wca.set_tol
-0000cfa0: 6572 616e 6365 2827 5627 2c20 302e 3129  erance('V', 0.1)
-0000cfb0: 2020 2320 3130 2520 746f 6c65 7261 6e63    # 10% toleranc
-0000cfc0: 652e 2046 6f72 2057 6f72 7374 2043 6173  e. For Worst Cas
-0000cfd0: 6520 616e 616c 7973 6973 2c20 7468 6520  e analysis, the 
-0000cfe0: 6469 7374 7269 6275 7469 6f6e 2069 7320  distribution is 
-0000cff0: 6972 7265 6c65 7661 6e74 0d0a 0d0a 2320  irrelevant....# 
-0000d000: 536f 6d65 2063 6f6d 706f 6e65 6e74 7320  Some components 
-0000d010: 6361 6e20 6861 7665 2061 2064 6966 6665  can have a diffe
-0000d020: 7265 6e74 2074 6f6c 6572 616e 6365 0d0a  rent tolerance..
-0000d030: 7763 612e 7365 745f 746f 6c65 7261 6e63  wca.set_toleranc
-0000d040: 6528 2752 3127 2c20 302e 3035 2920 2023  e('R1', 0.05)  #
-0000d050: 2035 2520 746f 6c65 7261 6e63 6520 666f   5% tolerance fo
-0000d060: 7220 5231 206f 6e6c 792e 2054 6869 7320  r R1 only. This 
-0000d070: 6f6e 6c79 206f 7665 7272 6964 6573 2074  only overrides t
-0000d080: 6865 2064 6566 6175 6c74 2074 6f6c 6572  he default toler
-0000d090: 616e 6365 2066 6f72 2052 310d 0a0d 0a23  ance for R1....#
-0000d0a0: 2054 6f6c 6572 616e 6365 7320 6361 6e20   Tolerances can 
-0000d0b0: 6265 2073 6574 2066 6f72 2070 6172 616d  be set for param
-0000d0c0: 6574 6572 7320 6173 2077 656c 6c2e 0d0a  eters as well...
-0000d0d0: 7763 612e 7365 745f 7061 7261 6d65 7465  wca.set_paramete
-0000d0e0: 725f 6465 7669 6174 696f 6e28 2756 6f73  r_deviation('Vos
-0000d0f0: 272c 2033 652d 342c 2035 652d 3329 0d0a  ', 3e-4, 5e-3)..
-0000d100: 0d0a 2320 4669 6e61 6c6c 7920 7468 6520  ..# Finally the 
-0000d110: 6e65 746c 6973 7420 6973 2073 6176 6564  netlist is saved
-0000d120: 2074 6f20 6120 6669 6c65 0d0a 7763 612e   to a file..wca.
-0000d130: 7361 7665 5f6e 6574 6c69 7374 2827 2e2f  save_netlist('./
-0000d140: 7465 7374 6669 6c65 732f 7361 6c6c 656e  testfiles/sallen
-0000d150: 6b65 795f 7763 2e61 7363 2729 0d0a 0d0a  key_wc.asc')....
-0000d160: 0d0a 7763 612e 7275 6e28 2920 2023 2052  ..wca.run()  # R
-0000d170: 756e 7320 7468 6520 7369 6d75 6c61 7469  uns the simulati
-0000d180: 6f6e 2077 6974 6820 7370 6c69 7473 206f  on with splits o
-0000d190: 6620 3130 3020 7275 6e73 2065 6163 680d  f 100 runs each.
-0000d1a0: 0a6c 6f67 7320 3d20 7763 612e 7265 6164  .logs = wca.read
-0000d1b0: 5f6c 6f67 6669 6c65 7328 2920 2020 2320  _logfiles()   # 
-0000d1c0: 5265 6164 7320 7468 6520 6c6f 6720 6669  Reads the log fi
-0000d1d0: 6c65 7320 616e 6420 7374 6f72 6573 2074  les and stores t
-0000d1e0: 6865 2072 6573 756c 7473 2069 6e20 7468  he results in th
-0000d1f0: 6520 7265 7375 6c74 7320 6174 7472 6962  e results attrib
-0000d200: 7574 650d 0a6c 6f67 732e 6578 706f 7274  ute..logs.export
-0000d210: 5f64 6174 6128 272e 2f74 656d 705f 7763  _data('./temp_wc
-0000d220: 612f 6461 7461 2e63 7376 2729 2020 2320  a/data.csv')  # 
-0000d230: 4578 706f 7274 7320 7468 6520 6461 7461  Exports the data
-0000d240: 2074 6f20 6120 6373 7620 6669 6c65 0d0a   to a csv file..
-0000d250: 0d0a 7072 696e 7428 2257 6f72 7374 2063  ..print("Worst c
-0000d260: 6173 6520 7265 7375 6c74 733a 2229 0d0a  ase results:")..
-0000d270: 666f 7220 7061 7261 6d20 696e 2028 2766  for param in ('f
-0000d280: 6375 7427 2c20 2766 6375 745f 4652 4f4d  cut', 'fcut_FROM
-0000d290: 2729 3a0d 0a20 2020 2070 7269 6e74 2866  '):..    print(f
-0000d2a0: 227b 7061 7261 6d7d 3a20 6d69 6e3a 7b6c  "{param}: min:{l
-0000d2b0: 6f67 732e 6d69 6e5f 6d65 6173 7572 655f  ogs.min_measure_
-0000d2c0: 7661 6c75 6528 7061 7261 6d29 7d20 6d61  value(param)} ma
-0000d2d0: 783a 7b6c 6f67 732e 6d61 785f 6d65 6173  x:{logs.max_meas
-0000d2e0: 7572 655f 7661 6c75 6528 7061 7261 6d29  ure_value(param)
-0000d2f0: 7d22 290d 0a0d 0a77 6361 2e63 6c65 616e  }")....wca.clean
-0000d300: 7570 5f66 696c 6573 2829 2020 2320 4465  up_files()  # De
-0000d310: 6c65 7465 7320 7468 6520 7465 6d70 6f72  letes the tempor
-0000d320: 6172 7920 6669 6c65 730d 0a60 6060 0d0a  ary files..```..
-0000d330: 5768 656e 206f 7065 6e69 6e67 2074 6865  When opening the
-0000d340: 2063 7265 6174 6564 2073 616c 6c65 6e6b   created sallenk
-0000d350: 6579 5f77 632e 6e65 7420 6669 6c65 2c20  ey_wc.net file, 
-0000d360: 7765 2063 616e 2073 6565 2074 6861 7420  we can see that 
-0000d370: 7468 6520 666f 6c6c 6f77 696e 6720 6369  the following ci
-0000d380: 7263 7569 742e 0d0a 0d0a 215b 5361 6c6c  rcuit.....![Sall
-0000d390: 656e 2d4b 6579 2041 6d70 6c69 6669 6572  en-Key Amplifier
-0000d3a0: 2077 6974 6820 5743 415d 282e 2f64 6f63   with WCA](./doc
-0000d3b0: 2f6d 6f64 756c 6573 2f73 616c 6c65 6e6b  /modules/sallenk
-0000d3c0: 6579 5f77 632e 706e 6720 2253 616c 6c65  ey_wc.png "Salle
-0000d3d0: 6e2d 4b65 7920 416d 706c 6966 6965 7220  n-Key Amplifier 
-0000d3e0: 7769 7468 2057 4341 2229 0d0a 0d0a 5468  with WCA")....Th
-0000d3f0: 6520 666f 6c6c 6f77 696e 6720 7570 6461  e following upda
-0000d400: 7465 7320 7765 7265 206d 6164 6520 746f  tes were made to
-0000d410: 2074 6865 2063 6972 6375 6974 3a0d 0a2d   the circuit:..-
-0000d420: 2054 6865 2076 616c 7565 206f 6620 6561   The value of ea
-0000d430: 6368 2063 6f6d 706f 6e65 6e74 2077 6173  ch component was
-0000d440: 2072 6570 6c61 6365 6420 6279 2061 2066   replaced by a f
-0000d450: 756e 6374 696f 6e20 7468 6174 2067 656e  unction that gen
-0000d460: 6572 6174 6573 2061 206e 6f6d 696e 616c  erates a nominal
-0000d470: 2c20 6d69 6e69 6d75 6d20 616e 6420 6d61  , minimum and ma
-0000d480: 7869 6d75 6d20 7661 6c75 6520 6465 7065  ximum value depe
-0000d490: 6e64 696e 670d 0a6f 6e20 7468 6520 7275  nding..on the ru
-0000d4a0: 6e20 7061 7261 6d65 7465 7220 616e 6420  n parameter and 
-0000d4b0: 6973 2061 7373 6967 6e65 6420 6120 756e  is assigned a un
-0000d4c0: 6971 7565 2069 6e64 6578 206e 756d 6265  ique index numbe
-0000d4d0: 722e 2028 5231 3d30 2c20 566f 733d 312c  r. (R1=0, Vos=1,
-0000d4e0: 2052 323d 322c 202e 2e2e 2056 323d 372c   R2=2, ... V2=7,
-0000d4f0: 2056 494e 3d38 290d 0a54 6865 2075 6e69   VIN=8)..The uni
-0000d500: 7175 6520 6e75 6d62 6572 2063 6f72 7265  que number corre
-0000d510: 7370 6f6e 6473 2074 6f20 7468 6520 6269  sponds to the bi
-0000d520: 7420 706f 7369 7469 6f6e 206f 6620 7468  t position of th
-0000d530: 6520 7275 6e20 7061 7261 6d65 7465 722e  e run parameter.
-0000d540: 2042 6974 2030 2063 6f72 7265 7370 6f6e   Bit 0 correspon
-0000d550: 6473 2074 6f20 7468 6520 6d69 6e69 6d75  ds to the minimu
-0000d560: 6d20 7661 6c75 6520 616e 640d 0a62 6974  m value and..bit
-0000d570: 2031 2063 6f72 7265 7370 6f6e 6473 2074   1 corresponds t
-0000d580: 6f20 7468 6520 6d61 7869 6d75 6d20 7661  o the maximum va
-0000d590: 6c75 652e 2043 616c 6375 6c61 7469 6e67  lue. Calculating
-0000d5a0: 2061 6c6c 2070 6f73 7369 626c 6520 7065   all possible pe
-0000d5b0: 726d 7574 6174 696f 6e73 206f 6620 6d61  rmutations of ma
-0000d5c0: 7869 6d75 6d20 616e 6420 6d69 6e69 6d75  ximum and minimu
-0000d5d0: 6d20 7661 6c75 6573 2066 6f72 2065 6163  m values for eac
-0000d5e0: 680d 0a63 6f6d 706f 6e65 6e74 2c20 7765  h..component, we
-0000d5f0: 2067 6574 2032 2a2a 3920 3d20 3531 3220   get 2**9 = 512 
-0000d600: 706f 7373 6962 6c65 2063 6f6d 6269 6e61  possible combina
-0000d610: 7469 6f6e 732e 2054 6869 7320 6d61 7073  tions. This maps
-0000d620: 2069 6e74 6f20 6120 3920 6269 7420 6269   into a 9 bit bi
-0000d630: 6e61 7279 206e 756d 6265 722c 2077 6869  nary number, whi
-0000d640: 6368 2069 7320 7468 6520 7275 6e20 7061  ch is the run pa
-0000d650: 7261 6d65 7465 722e 0d0a 2d20 5468 6520  rameter...- The 
-0000d660: 2e73 7465 7020 7061 7261 6d20 7275 6e20  .step param run 
-0000d670: 636f 6d6d 616e 6420 7761 7320 6164 6465  command was adde
-0000d680: 6420 746f 2074 6865 206e 6574 6c69 7374  d to the netlist
-0000d690: 2e20 4974 2073 7461 7274 7320 6174 202d  . It starts at -
-0000d6a0: 3120 7768 6963 6820 6974 2773 2074 6865  1 which it's the
-0000d6b0: 206e 6f6d 696e 616c 2076 616c 7565 2073   nominal value s
-0000d6c0: 696d 756c 6174 696f 6e2c 2074 6865 6e20  imulation, then 
-0000d6d0: 300d 0a77 6869 6368 2063 6f72 7265 7370  0..which corresp
-0000d6e0: 6f6e 6473 2074 6f20 7468 6520 6d69 6e69  onds to the mini
-0000d6f0: 6d75 6d20 7661 6c75 6520 666f 7220 6561  mum value for ea
-0000d700: 6368 2063 6f6d 706f 6e65 6e74 2c20 7468  ch component, th
-0000d710: 656e 2069 7420 6d61 6b65 7320 616c 6c20  en it makes all 
-0000d720: 636f 6d62 696e 6174 696f 6e73 206f 6620  combinations of 
-0000d730: 6d69 6e69 6d75 6d20 616e 6420 6d61 7869  minimum and maxi
-0000d740: 6d75 6d20 7661 6c75 6573 200d 0a75 6e74  mum values ..unt
-0000d750: 696c 2035 3131 2c20 7768 6963 6820 6973  il 511, which is
-0000d760: 2074 6865 2073 696d 756c 6174 696f 6e20   the simulation 
-0000d770: 7769 7468 2061 6c6c 206d 6178 696d 756d  with all maximum
-0000d780: 2076 616c 7565 732e 0d0a 2d20 4120 6465   values...- A de
-0000d790: 6661 756c 7420 7661 6c75 6520 666f 7220  fault value for 
-0000d7a0: 7468 6520 7275 6e20 7061 7261 6d65 7465  the run paramete
-0000d7b0: 7220 7761 7320 6164 6465 642e 2054 6869  r was added. Thi
-0000d7c0: 7320 6973 2075 7365 6675 6c20 6966 2074  s is useful if t
-0000d7d0: 6865 202e 7374 6570 2070 6172 616d 2072  he .step param r
-0000d7e0: 756e 2069 7320 636f 6d6d 656e 7465 6420  un is commented 
-0000d7f0: 6f75 742e 0d0a 2d20 5468 6520 5231 2074  out...- The R1 t
-0000d800: 6f6c 6572 616e 6365 2069 7320 6469 6666  olerance is diff
-0000d810: 6572 656e 7420 6672 6f6d 2074 6865 206f  erent from the o
-0000d820: 7468 6572 2072 6573 6973 746f 7273 2e20  ther resistors. 
-0000d830: 5468 6973 2069 7320 6265 6361 7573 6520  This is because 
-0000d840: 7468 6520 746f 6c65 7261 6e63 6520 7761  the tolerance wa
-0000d850: 7320 6578 706c 6963 6974 6c79 2073 6574  s explicitly set
-0000d860: 2066 6f72 2052 312e 0d0a 2d20 5468 6520   for R1...- The 
-0000d870: 7763 2829 2066 756e 6374 696f 6e20 6973  wc() function is
-0000d880: 2061 6464 6564 2074 6f20 7468 6520 6369   added to the ci
-0000d890: 7263 7569 742e 2054 6869 7320 6675 6e63  rcuit. This func
-0000d8a0: 7469 6f6e 2069 7320 7573 6564 2074 6f20  tion is used to 
-0000d8b0: 6361 6c63 756c 6174 6520 7468 6520 776f  calculate the wo
-0000d8c0: 7273 7420 6361 7365 2076 616c 7565 2066  rst case value f
-0000d8d0: 6f72 2065 6163 6820 636f 6d70 6f6e 656e  or each componen
-0000d8e0: 742c 0d0a 6769 7665 6e20 6120 746f 6c65  t,..given a tole
-0000d8f0: 7261 6e63 6520 7661 6c75 6520 616e 6420  rance value and 
-0000d900: 6974 7320 7265 7370 6563 7469 7665 2069  its respective i
-0000d910: 6e64 6578 2e0d 0a2d 2054 6865 2077 6331  ndex...- The wc1
-0000d920: 2829 2066 756e 6374 696f 6e20 6973 2061  () function is a
-0000d930: 6464 6564 2074 6f20 7468 6520 6369 7263  dded to the circ
-0000d940: 7569 742e 2054 6869 7320 6675 6e63 7469  uit. This functi
-0000d950: 6f6e 2069 7320 7573 6564 2074 6f20 6361  on is used to ca
-0000d960: 6c63 756c 6174 6520 7468 6520 776f 7273  lculate the wors
-0000d970: 7420 6361 7365 2076 616c 7565 2066 6f72  t case value for
-0000d980: 2065 6163 6820 636f 6d70 6f6e 656e 742c   each component,
-0000d990: 0d0a 6769 7665 6e20 6120 6d69 6e69 6d75  ..given a minimu
-0000d9a0: 6d20 616e 6420 6d61 7869 6d75 6d20 7661  m and maximum va
-0000d9b0: 6c75 6520 616e 6420 6974 7320 7265 7370  lue and its resp
-0000d9c0: 6563 7469 7665 2069 6e64 6578 2e0d 0a0d  ective index....
-0000d9d0: 0a23 2323 204c 5453 7465 7073 2e70 7920  .### LTSteps.py 
-0000d9e0: 2323 230d 0a0d 0a54 6869 7320 6d6f 6475  ###....This modu
-0000d9f0: 6c65 2064 6566 696e 6573 2061 2063 6c61  le defines a cla
-0000da00: 7373 2074 6861 7420 6361 6e20 6265 2075  ss that can be u
-0000da10: 7365 6420 746f 2070 6172 7365 204c 5453  sed to parse LTS
-0000da20: 7069 6365 206c 6f67 2066 696c 6573 2077  pice log files w
-0000da30: 6865 7265 2074 6865 2069 6e66 6f72 6d61  here the informa
-0000da40: 7469 6f6e 2061 626f 7574 202e 5354 4550  tion about .STEP
-0000da50: 2069 6e66 6f72 6d61 7469 6f6e 2069 730d   information is.
-0000da60: 0a77 7269 7474 656e 2e20 5468 6572 6520  .written. There 
-0000da70: 6172 6520 7477 6f20 706f 7373 6962 6c65  are two possible
-0000da80: 2075 7361 6765 7320 6f66 2074 6869 7320   usages of this 
-0000da90: 6d6f 6475 6c65 2c20 6569 7468 6572 2070  module, either p
-0000daa0: 726f 6772 616d 6d61 7469 6361 6c6c 7920  rogrammatically 
-0000dab0: 6279 2069 6d70 6f72 7469 6e67 2074 6865  by importing the
-0000dac0: 206d 6f64 756c 6520 616e 6420 7468 656e   module and then
-0000dad0: 0d0a 6163 6365 7373 696e 6720 6461 7461  ..accessing data
-0000dae0: 2074 6872 6f75 6768 2074 6865 2063 6c61   through the cla
-0000daf0: 7373 2061 7320 6578 656d 706c 6966 6965  ss as exemplifie
-0000db00: 6420 6865 7265 3a0d 0a0d 0a60 6060 7079  d here:....```py
-0000db10: 7468 6f6e 0d0a 6672 6f6d 2050 794c 5453  thon..from PyLTS
-0000db20: 7069 6365 2e6c 6f67 2e6c 7473 7465 7073  pice.log.ltsteps
-0000db30: 2069 6d70 6f72 7420 4c54 5370 6963 654c   import LTSpiceL
-0000db40: 6f67 5265 6164 6572 0d0a 0d0a 6461 7461  ogReader....data
-0000db50: 203d 204c 5453 7069 6365 4c6f 6752 6561   = LTSpiceLogRea
-0000db60: 6465 7228 2242 6174 6368 5f54 6573 745f  der("Batch_Test_
-0000db70: 4144 3832 305f 3135 2e6c 6f67 2229 0d0a  AD820_15.log")..
-0000db80: 0d0a 7072 696e 7428 224e 756d 6265 7220  ..print("Number 
-0000db90: 6f66 2073 7465 7073 2020 3a22 2c20 6461  of steps  :", da
-0000dba0: 7461 2e73 7465 705f 636f 756e 7429 0d0a  ta.step_count)..
-0000dbb0: 7374 6570 5f6e 616d 6573 203d 2064 6174  step_names = dat
-0000dbc0: 612e 6765 745f 7374 6570 5f76 6172 7328  a.get_step_vars(
-0000dbd0: 290d 0a6d 6561 735f 6e61 6d65 7320 3d20  )..meas_names = 
-0000dbe0: 6461 7461 2e67 6574 5f6d 6561 7375 7265  data.get_measure
-0000dbf0: 5f6e 616d 6573 2829 0d0a 0d0a 2320 5072  _names()....# Pr
-0000dc00: 696e 7469 6e67 2048 6561 6465 7273 0d0a  inting Headers..
-0000dc10: 7072 696e 7428 2720 272e 6a6f 696e 285b  print(' '.join([
-0000dc20: 6622 7b73 7465 703a 3135 737d 2220 666f  f"{step:15s}" fo
-0000dc30: 7220 7374 6570 2069 6e20 7374 6570 5f6e  r step in step_n
-0000dc40: 616d 6573 5d29 2c20 656e 643d 2727 2920  ames]), end='') 
-0000dc50: 2023 2050 7269 6e74 2073 7465 7073 206e   # Print steps n
-0000dc60: 616d 6573 2077 6974 6820 6e6f 206e 6577  ames with no new
-0000dc70: 206c 696e 650d 0a70 7269 6e74 2827 2027   line..print(' '
-0000dc80: 2e6a 6f69 6e28 5b66 227b 6e61 6d65 3a31  .join([f"{name:1
-0000dc90: 3573 7d22 2066 6f72 206e 616d 6520 696e  5s}" for name in
-0000dca0: 206d 6561 735f 6e61 6d65 735d 292c 2065   meas_names]), e
-0000dcb0: 6e64 3d27 5c6e 2729 0d0a 2320 5072 696e  nd='\n')..# Prin
-0000dcc0: 7469 6e67 2064 6174 610d 0a66 6f72 2069  ting data..for i
-0000dcd0: 2069 6e20 7261 6e67 6528 6461 7461 2e73   in range(data.s
-0000dce0: 7465 705f 636f 756e 7429 3a0d 0a20 2020  tep_count):..   
-0000dcf0: 2070 7269 6e74 2827 2027 2e6a 6f69 6e28   print(' '.join(
-0000dd00: 5b66 227b 6461 7461 5b73 7465 705d 5b69  [f"{data[step][i
-0000dd10: 5d3a 3135 7d22 2066 6f72 2073 7465 7020  ]:15}" for step 
-0000dd20: 696e 2073 7465 705f 6e61 6d65 735d 292c  in step_names]),
-0000dd30: 2065 6e64 3d27 2729 2020 2320 5072 696e   end='')  # Prin
-0000dd40: 7420 7374 6570 7320 6e61 6d65 7320 7769  t steps names wi
-0000dd50: 7468 206e 6f20 6e65 7720 6c69 6e65 0d0a  th no new line..
-0000dd60: 2020 2020 7072 696e 7428 2720 272e 6a6f      print(' '.jo
-0000dd70: 696e 285b 6622 7b64 6174 615b 6e61 6d65  in([f"{data[name
-0000dd80: 5d5b 695d 3a31 357d 2220 666f 7220 6e61  ][i]:15}" for na
-0000dd90: 6d65 2069 6e20 6d65 6173 5f6e 616d 6573  me in meas_names
-0000dda0: 5d29 2c20 656e 643d 275c 6e27 2920 2023  ]), end='\n')  #
-0000ddb0: 2050 7269 6e74 2048 6561 6465 720d 0a0d   Print Header...
-0000ddc0: 0a70 7269 6e74 2822 546f 7461 6c20 6e75  .print("Total nu
-0000ddd0: 6d62 6572 206f 6620 6d65 6173 7572 6573  mber of measures
-0000dde0: 2066 6f75 6e64 203a 222c 2064 6174 612e   found :", data.
-0000ddf0: 6d65 6173 7572 655f 636f 756e 7429 0d0a  measure_count)..
-0000de00: 6060 600d 0a0d 0a54 6865 2073 6563 6f6e  ```....The secon
-0000de10: 6420 706f 7373 6962 696c 6974 7920 6973  d possibility is
-0000de20: 2074 6f20 7573 6520 7468 6520 6d6f 6475   to use the modu
-0000de30: 6c65 2064 6972 6563 746c 7920 6f6e 2074  le directly on t
-0000de40: 6865 2063 6f6d 6d61 6e64 206c 696e 650d  he command line.
-0000de50: 0a0d 0a23 2043 6f6d 6d61 6e64 204c 696e  ...# Command Lin
-0000de60: 6520 496e 7465 7266 6163 6520 230d 0a0d  e Interface #...
-0000de70: 0a23 2323 206c 7473 7465 7073 2e65 7865  .### ltsteps.exe
-0000de80: 2023 2323 0d0a 0d0a 5468 6520 3c66 696c   ###....The <fil
-0000de90: 656e 616d 653e 2063 616e 2062 6520 6569  ename> can be ei
-0000dea0: 7468 6572 2062 6520 6120 6c6f 6720 6669  ther be a log fi
-0000deb0: 6c65 2028 2e6c 6f67 292c 2061 2064 6174  le (.log), a dat
-0000dec0: 6120 6578 706f 7274 2066 696c 6520 282e  a export file (.
-0000ded0: 7478 7429 206f 7220 6120 6d65 6173 7572  txt) or a measur
-0000dee0: 656d 656e 7420 6f75 7470 7574 2066 696c  ement output fil
-0000def0: 6520 282e 6d65 6173 290d 0a54 6869 7320  e (.meas)..This 
-0000df00: 7769 6c6c 2070 726f 6365 7373 2061 6c6c  will process all
-0000df10: 2074 6865 2064 6174 6120 616e 6420 6578   the data and ex
-0000df20: 706f 7274 2069 7420 6175 746f 6d61 7469  port it automati
-0000df30: 6361 6c6c 7920 696e 746f 2061 2074 6578  cally into a tex
-0000df40: 7420 6669 6c65 2077 6974 6820 7468 6520  t file with the 
-0000df50: 6578 7465 6e73 696f 6e20 2874 6c6f 672c  extension (tlog,
-0000df60: 2074 7376 2c20 746d 6561 7329 0d0a 7768   tsv, tmeas)..wh
-0000df70: 6572 6520 7468 6520 6461 7461 2072 6561  ere the data rea
-0000df80: 6420 6973 2066 6f72 6d61 7474 6564 2069  d is formatted i
-0000df90: 6e74 6f20 6120 6d6f 7265 2063 6f6e 7665  nto a more conve
-0000dfa0: 6e69 656e 7420 7461 6220 7365 7061 7261  nient tab separa
-0000dfb0: 7465 6420 666f 726d 6174 2e20 496e 2063  ted format. In c
-0000dfc0: 6173 6520 7468 6520 3c6c 6f67 6669 6c65  ase the <logfile
-0000dfd0: 3e20 6973 206e 6f74 2070 726f 7669 6465  > is not provide
-0000dfe0: 642c 2074 6865 0d0a 7363 7269 7074 2077  d, the..script w
-0000dff0: 696c 6c20 7363 616e 2074 6865 2064 6972  ill scan the dir
-0000e000: 6563 746f 7279 2061 6e64 2070 726f 6365  ectory and proce
-0000e010: 7373 2074 6865 206e 6577 6573 7420 6c6f  ss the newest lo
-0000e020: 672c 2074 7874 206f 7220 6f75 7420 6669  g, txt or out fi
-0000e030: 6c65 2066 6f75 6e64 2e0d 0a0d 0a23 2323  le found.....###
-0000e040: 2068 6973 746f 6772 616d 2e65 7865 2023   histogram.exe #
-0000e050: 2323 0d0a 0d0a 5468 6973 206d 6f64 756c  ##....This modul
-0000e060: 6520 7573 6573 2074 6865 2064 6174 6120  e uses the data 
-0000e070: 696e 7369 6465 206f 6e20 7468 6520 6669  inside on the fi
-0000e080: 6c65 6e61 6d65 2074 6f20 7072 6f64 7563  lename to produc
-0000e090: 6520 6120 6869 7374 6f67 7261 6d20 696d  e a histogram im
-0000e0a0: 6167 652e 0d0a 0d0a 6060 600d 0a55 7361  age.....```..Usa
-0000e0b0: 6765 3a20 4869 7374 6f67 7261 6d2e 7079  ge: Histogram.py
-0000e0c0: 205b 6f70 7469 6f6e 735d 204c 4f47 5f46   [options] LOG_F
-0000e0d0: 494c 4520 5452 4143 450d 0a0d 0a4f 7074  ILE TRACE....Opt
-0000e0e0: 696f 6e73 3a0d 0a20 202d 2d76 6572 7369  ions:..  --versi
-0000e0f0: 6f6e 2020 2020 2020 2020 2020 2020 2073  on             s
-0000e100: 686f 7720 7072 6f67 7261 6d27 7320 7665  how program's ve
-0000e110: 7273 696f 6e20 6e75 6d62 6572 2061 6e64  rsion number and
-0000e120: 2065 7869 740d 0a20 202d 682c 202d 2d68   exit..  -h, --h
-0000e130: 656c 7020 2020 2020 2020 2020 2020 2073  elp            s
-0000e140: 686f 7720 7468 6973 2068 656c 7020 6d65  how this help me
-0000e150: 7373 6167 6520 616e 6420 6578 6974 0d0a  ssage and exit..
-0000e160: 2020 2d73 2053 4947 4d41 2c20 2d2d 7369    -s SIGMA, --si
-0000e170: 676d 613d 5349 474d 410d 0a20 2020 2020  gma=SIGMA..     
-0000e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e190: 2020 2053 6967 6d61 2074 6f20 6265 2075     Sigma to be u
-0000e1a0: 7365 6420 696e 2074 6865 2064 6973 7472  sed in the distr
-0000e1b0: 6962 7574 696f 6e20 6669 742e 2044 6566  ibution fit. Def
-0000e1c0: 6175 6c74 3d33 0d0a 2020 2d6e 204e 4249  ault=3..  -n NBI
-0000e1d0: 4e53 2c20 2d2d 6e62 696e 733d 4e42 494e  NS, --nbins=NBIN
-0000e1e0: 530d 0a20 2020 2020 2020 2020 2020 2020  S..             
-0000e1f0: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
-0000e200: 7220 6f66 2062 696e 7320 746f 2062 6520  r of bins to be 
-0000e210: 7573 6564 2069 6e20 7468 6520 6869 7374  used in the hist
-0000e220: 6f67 7261 6d2e 2044 6566 6175 6c74 3d32  ogram. Default=2
-0000e230: 300d 0a20 202d 6320 4649 4c54 4552 532c  0..  -c FILTERS,
-0000e240: 202d 2d63 6f6e 6469 7469 6f6e 3d46 494c   --condition=FIL
-0000e250: 5445 5253 0d0a 2020 2020 2020 2020 2020  TERS..          
-0000e260: 2020 2020 2020 2020 2020 2020 2020 4669                Fi
-0000e270: 6c74 6572 2063 6f6e 6469 7469 6f6e 2077  lter condition w
-0000e280: 7269 7465 6e20 696e 2070 7974 686f 6e2e  riten in python.
-0000e290: 204d 6f72 6520 7468 616e 206f 6e65 0d0a   More than one..
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2b0: 2020 2020 2020 2020 6578 7072 6573 7369          expressi
-0000e2c0: 6f6e 2063 616e 2062 6520 6164 6465 6420  on can be added 
-0000e2d0: 6275 7420 6561 6368 2065 7870 7265 7373  but each express
-0000e2e0: 696f 6e20 7368 6f75 6c64 2062 650d 0a20  ion should be.. 
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e300: 2020 2020 2020 2070 7265 6365 6465 6420         preceded 
-0000e310: 6279 202d 632e 2045 5841 4d50 4c45 3a20  by -c. EXAMPLE: 
-0000e320: 2d63 2056 284e 3030 3129 3e34 202d 6320  -c V(N001)>4 -c 
-0000e330: 7061 7261 6d65 7465 723d 3d31 0d0a 2020  parameter==1..  
-0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e350: 2020 2020 2020 2d63 2020 4928 5631 293c        -c  I(V1)<
-0000e360: 302e 350d 0a20 202d 6620 464f 524d 4154  0.5..  -f FORMAT
-0000e370: 2c20 2d2d 666f 726d 6174 3d46 4f52 4d41  , --format=FORMA
-0000e380: 540d 0a20 2020 2020 2020 2020 2020 2020  T..             
-0000e390: 2020 2020 2020 2020 2020 2046 6f72 6d61             Forma
-0000e3a0: 7420 7374 7269 6e67 2066 6f72 2074 6865  t string for the
-0000e3b0: 2058 2061 7869 732e 2045 7861 6d70 6c65   X axis. Example
-0000e3c0: 3a20 2d66 2025 332e 3466 0d0a 2020 2d74  : -f %3.4f..  -t
-0000e3d0: 2054 4954 4c45 2c20 2d2d 7469 746c 653d   TITLE, --title=
-0000e3e0: 5449 544c 450d 0a20 2020 2020 2020 2020  TITLE..         
-0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000e400: 6974 6c65 2074 6f20 6170 7065 6172 206f  itle to appear o
-0000e410: 6e20 7468 6520 746f 7020 6f66 2074 6865  n the top of the
-0000e420: 2068 6973 746f 6772 616d 2e0d 0a20 202d   histogram...  -
-0000e430: 7220 5241 4e47 452c 202d 2d72 616e 6765  r RANGE, --range
-0000e440: 3d52 414e 4745 0d0a 2020 2020 2020 2020  =RANGE..        
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 5261 6e67 6520 6f66 2074 6865 2058 2061  Range of the X a
-0000e470: 7869 7320 746f 2075 7365 2066 6f72 2074  xis to use for t
-0000e480: 6865 2068 6973 746f 6772 616d 2069 6e20  he histogram in 
-0000e490: 7468 650d 0a20 2020 2020 2020 2020 2020  the..           
-0000e4a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000e4b0: 6d20 6d69 6e3a 6d61 782e 2045 7861 6d70  m min:max. Examp
-0000e4c0: 6c65 3a20 2d72 202d 313a 310d 0a20 202d  le: -r -1:1..  -
-0000e4d0: 432c 202d 2d63 6c69 7062 6f61 7264 2020  C, --clipboard  
-0000e4e0: 2020 2020 2049 6620 7468 6520 6461 7461       If the data
-0000e4f0: 2066 726f 6d20 7468 6520 636c 6970 626f   from the clipbo
-0000e500: 6172 6420 6973 2074 6f20 6265 2075 7365  ard is to be use
-0000e510: 642e 0d0a 2020 2d69 2049 4d41 4745 4649  d...  -i IMAGEFI
-0000e520: 4c45 2c20 2d2d 696d 6167 653d 494d 4147  LE, --image=IMAG
-0000e530: 4546 494c 450d 0a20 2020 2020 2020 2020  EFILE..         
-0000e540: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-0000e550: 616d 6520 6f66 2074 6865 2069 6d61 6765  ame of the image
-0000e560: 2046 696c 652e 2065 7874 656e 7369 6f6e   File. extension
-0000e570: 2027 706e 6727 2020 2020 0d0a 6060 600d   'png'    ..```.
-0000e580: 0a0d 0a23 2323 2072 6177 636f 6e76 6572  ...### rawconver
-0000e590: 742e 6578 6520 2323 230d 0a0d 0a41 2074  t.exe ###....A t
-0000e5a0: 6f6f 6c20 746f 2063 6f6e 7665 7274 202e  ool to convert .
-0000e5b0: 7261 7720 6669 6c65 7320 696e 746f 2063  raw files into c
-0000e5c0: 7376 206f 7220 4578 6365 6c20 6669 6c65  sv or Excel file
-0000e5d0: 732e 0d0a 0d0a 6060 600d 0a55 7361 6765  s.....```..Usage
-0000e5e0: 3a20 7261 775f 636f 6e76 6572 742e 6578  : raw_convert.ex
-0000e5f0: 6520 5b6f 7074 696f 6e73 5d20 3c72 6177  e [options] <raw
-0000e600: 6669 6c65 3e20 3c74 7261 6365 5f6c 6973  file> <trace_lis
-0000e610: 743e 0d0a 0d0a 4f70 7469 6f6e 733a 0d0a  t>....Options:..
-0000e620: 2020 2d2d 7665 7273 696f 6e20 2020 2020    --version     
-0000e630: 2020 2020 2020 2020 7368 6f77 2070 726f          show pro
-0000e640: 6772 616d 2773 2076 6572 7369 6f6e 206e  gram's version n
-0000e650: 756d 6265 7220 616e 6420 6578 6974 0d0a  umber and exit..
-0000e660: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
-0000e670: 2020 2020 2020 2020 7368 6f77 2074 6869          show thi
-0000e680: 7320 6865 6c70 206d 6573 7361 6765 2061  s help message a
-0000e690: 6e64 2065 7869 740d 0a20 202d 6f20 4649  nd exit..  -o FI
-0000e6a0: 4c45 2c20 2d2d 6f75 7470 7574 3d46 494c  LE, --output=FIL
-0000e6b0: 450d 0a20 2020 2020 2020 2020 2020 2020  E..             
-0000e6c0: 2020 2020 2020 2020 2020 204f 7574 7075             Outpu
-0000e6d0: 7420 6669 6c65 206e 616d 652e 2055 7365  t file name. Use
-0000e6e0: 202e 6373 7620 666f 7220 4353 5620 6f75   .csv for CSV ou
-0000e6f0: 7470 7574 2c20 2e78 6c73 7820 666f 720d  tput, .xlsx for.
-0000e700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e710: 2020 2020 2020 2020 2045 7863 656c 206f           Excel o
-0000e720: 7574 7075 740d 0a20 202d 632c 202d 2d63  utput..  -c, --c
-0000e730: 6c69 7062 6f61 7264 2020 2020 2020 204f  lipboard       O
-0000e740: 7574 7075 7420 746f 2063 6c69 7062 6f61  utput to clipboa
-0000e750: 7264 0d0a 2020 2d76 2c20 2d2d 7665 7262  rd..  -v, --verb
-0000e760: 6f73 6520 2020 2020 2020 2020 5665 7262  ose         Verb
-0000e770: 6f73 6520 6f75 7470 7574 0d0a 2020 2d73  ose output..  -s
-0000e780: 2053 4550 4152 4154 4f52 2c20 2d2d 7365   SEPARATOR, --se
-0000e790: 703d 5345 5041 5241 544f 520d 0a20 2020  p=SEPARATOR..   
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7b0: 2020 2020 2056 616c 7565 2073 6570 6172       Value separ
-0000e7c0: 6174 6f72 2066 6f72 2043 5356 206f 7574  ator for CSV out
-0000e7d0: 7075 742e 2044 6566 6175 6c74 3a20 225c  put. Default: "\
-0000e7e0: 7422 203c 5441 423e 0d0a 2020 2020 2020  t" <TAB>..      
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e800: 2020 4578 616d 706c 653a 202d 6420 223b    Example: -d ";
-0000e810: 220d 0a60 6060 0d0a 0d0a 2323 2320 7275  "..```....### ru
-0000e820: 6e5f 7365 7276 6572 2e65 7865 2023 2323  n_server.exe ###
-0000e830: 0d0a 0d0a 5468 6973 2063 6f6d 6d61 6e64  ....This command
-0000e840: 206c 696e 6520 746f 6f6c 2077 6173 206d   line tool was m
-0000e850: 6f76 6564 2074 6f20 7468 6520 7370 6963  oved to the spic
-0000e860: 656c 6962 2070 6163 6b61 6765 2e0d 0a0d  elib package....
-0000e870: 0a23 2323 2053 656d 6944 6576 4f70 5265  .### SemiDevOpRe
-0000e880: 6164 6572 2e70 7920 2323 230d 0a0d 0a54  ader.py ###....T
-0000e890: 6869 7320 6d6f 6475 6c65 2069 7320 7573  his module is us
-0000e8a0: 6564 2074 6f20 7265 6164 2066 726f 6d20  ed to read from 
-0000e8b0: 4c54 5370 6963 6520 6c6f 6720 6669 6c65  LTSpice log file
-0000e8c0: 7320 5365 6d69 636f 6e64 7563 746f 7220  s Semiconductor 
-0000e8d0: 4465 7669 6365 7320 4f70 6572 6174 696e  Devices Operatin
-0000e8e0: 6720 506f 696e 7420 496e 666f 726d 6174  g Point Informat
-0000e8f0: 696f 6e2e 2041 206d 6f72 6520 6465 7461  ion. A more deta
-0000e900: 696c 6564 0d0a 646f 6375 6d65 6e74 6174  iled..documentat
-0000e910: 696f 6e20 6973 2064 6972 6563 746c 7920  ion is directly 
-0000e920: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
-0000e930: 736f 7572 6365 2066 696c 6520 646f 6373  source file docs
-0000e940: 7472 696e 6773 2e0d 0a0d 0a23 2320 4465  trings.....## De
-0000e950: 6275 6720 4c6f 6767 696e 670d 0a0d 0a54  bug Logging....T
-0000e960: 6865 206c 6962 7261 7279 2075 7365 7320  he library uses 
-0000e970: 7468 6520 7374 616e 6461 7264 2060 6c6f  the standard `lo
-0000e980: 6767 696e 6760 206d 6f64 756c 652e 2054  gging` module. T
-0000e990: 6872 6565 2063 6f6e 7665 6e69 656e 6365  hree convenience
-0000e9a0: 2066 756e 6374 696f 6e73 2068 6176 6520   functions have 
-0000e9b0: 6265 656e 2061 6464 6564 2066 6f72 2065  been added for e
-0000e9c0: 6173 696c 7920 6368 616e 6769 6e67 206c  asily changing l
-0000e9d0: 6f67 6769 6e67 0d0a 7365 7474 696e 6773  ogging..settings
-0000e9e0: 2061 6372 6f73 7320 7468 6520 656e 7469   across the enti
-0000e9f0: 7265 206c 6962 7261 7279 2e20 6050 794c  re library. `PyL
-0000ea00: 5453 7069 6365 2e61 6c6c 5f6c 6f67 6765  TSpice.all_logge
-0000ea10: 7273 2829 6020 7265 7475 726e 7320 6120  rs()` returns a 
-0000ea20: 6c69 7374 206f 6620 616c 6c20 7468 6520  list of all the 
-0000ea30: 6c6f 6767 6572 2773 0d0a 6e61 6d65 732c  logger's..names,
-0000ea40: 2060 5079 4c54 5370 6963 652e 7365 745f   `PyLTSpice.set_
-0000ea50: 6c6f 675f 6c65 7665 6c28 6c6f 6767 696e  log_level(loggin
-0000ea60: 672e 4445 4255 4729 600d 0a77 6f75 6c64  g.DEBUG)`..would
-0000ea70: 2073 6574 2074 6865 206c 6962 7261 7279   set the library
-0000ea80: 2773 206c 6f67 6769 6e67 206c 6576 656c  's logging level
-0000ea90: 2074 6f20 6465 6275 672c 2061 6e64 2060   to debug, and `
-0000eaa0: 5079 4c54 5370 6963 652e 6164 645f 6c6f  PyLTSpice.add_lo
-0000eab0: 675f 6861 6e64 6c65 7228 6d79 5f68 616e  g_handler(my_han
-0000eac0: 646c 6572 2960 2077 6f75 6c64 2061 6464  dler)` would add
-0000ead0: 2060 6d79 5f68 616e 646c 6572 6020 6173   `my_handler` as
-0000eae0: 2061 0d0a 6861 6e64 6c65 7220 666f 720d   a..handler for.
-0000eaf0: 0a61 6c6c 206c 6f67 6765 7273 2e0d 0a0d  .all loggers....
-0000eb00: 0a23 2323 2053 696e 676c 6520 4d6f 6475  .### Single Modu
-0000eb10: 6c65 204c 6f67 6769 6e67 0d0a 0d0a 4974  le Logging....It
-0000eb20: 2069 7320 616c 736f 2070 6f73 7369 626c   is also possibl
-0000eb30: 6520 746f 2073 6574 2074 6865 206c 6f67  e to set the log
-0000eb40: 6769 6e67 2073 6574 7469 6e67 7320 666f  ging settings fo
-0000eb50: 7220 6120 7369 6e67 6c65 206d 6f64 756c  r a single modul
-0000eb60: 6520 6279 2075 7369 6e67 2069 7473 206e  e by using its n
-0000eb70: 616d 6520 6163 7175 6972 6564 2066 726f  ame acquired fro
-0000eb80: 6d0d 0a74 6865 2060 5079 4c54 5370 6963  m..the `PyLTSpic
-0000eb90: 652e 616c 6c5f 6c6f 6767 6572 7328 2960  e.all_loggers()`
-0000eba0: 0d0a 6675 6e63 7469 6f6e 2e20 466f 7220  ..function. For 
-0000ebb0: 6578 616d 706c 653a 0d0a 0d0a 6060 6070  example:....```p
-0000ebc0: 7974 686f 6e0d 0a69 6d70 6f72 7420 6c6f  ython..import lo
-0000ebd0: 6767 696e 670d 0a0d 0a6c 6f67 6769 6e67  gging....logging
-0000ebe0: 2e62 6173 6963 436f 6e66 6967 286c 6576  .basicConfig(lev
-0000ebf0: 656c 3d6c 6f67 6769 6e67 2e49 4e46 4f29  el=logging.INFO)
-0000ec00: 2020 2320 5365 7420 7570 2074 6865 2072    # Set up the r
-0000ec10: 6f6f 7420 6c6f 6767 6572 2066 6972 7374  oot logger first
-0000ec20: 0d0a 0d0a 696d 706f 7274 2050 794c 5453  ....import PyLTS
-0000ec30: 7069 6365 2020 2320 496d 706f 7274 2050  pice  # Import P
-0000ec40: 794c 5453 7069 6365 2074 6f20 7365 7420  yLTSpice to set 
-0000ec50: 7468 6520 6c6f 6767 696e 6720 6c65 7665  the logging leve
-0000ec60: 6c73 0d0a 0d0a 5079 4c54 5370 6963 652e  ls....PyLTSpice.
-0000ec70: 7365 745f 6c6f 675f 6c65 7665 6c28 6c6f  set_log_level(lo
-0000ec80: 6767 696e 672e 4445 4255 4729 2020 2320  gging.DEBUG)  # 
-0000ec90: 5365 7420 5079 4c54 5370 6963 6527 7320  Set PyLTSpice's 
-0000eca0: 676c 6f62 616c 206c 6f67 206c 6576 656c  global log level
-0000ecb0: 0d0a 6c6f 6767 696e 672e 6765 744c 6f67  ..logging.getLog
-0000ecc0: 6765 7228 2250 794c 5453 7069 6365 2e52  ger("PyLTSpice.R
-0000ecd0: 6177 5265 6164 2229 2e6c 6576 656c 203d  awRead").level =
-0000ece0: 206c 6f67 6769 6e67 2e57 4152 4e49 4e47   logging.WARNING
-0000ecf0: 2020 2320 5365 7420 7468 6520 6c6f 6720    # Set the log 
-0000ed00: 6c65 7665 6c20 666f 7220 6f6e 6c79 2052  level for only R
-0000ed10: 6177 5265 6164 2074 6f20 7761 726e 696e  awRead to warnin
-0000ed20: 670d 0a60 6060 0d0a 0d0a 576f 756c 6420  g..```....Would 
-0000ed30: 7365 7420 6f6e 6c79 2060 5079 4c54 5370  set only `PyLTSp
-0000ed40: 6963 652e 5261 7752 6561 6460 2066 696c  ice.RawRead` fil
-0000ed50: 6527 7320 6c6f 6767 696e 6720 6c65 7665  e's logging leve
-0000ed60: 6c20 746f 2077 6172 6e69 6e67 2077 6869  l to warning whi
-0000ed70: 6c65 2074 6865 206f 7468 6572 206d 6f64  le the other mod
-0000ed80: 756c 6573 2077 6f75 6c64 2072 656d 6169  ules would remai
-0000ed90: 6e20 6174 2064 6562 7567 206c 6576 656c  n at debug level
-0000eda0: 2e0d 0a5f 4d61 6b65 2073 7572 6520 746f  ..._Make sure to
-0000edb0: 2069 6e69 7469 616c 697a 6520 7468 6520   initialize the 
-0000edc0: 726f 6f74 206c 6f67 6765 7220 6265 666f  root logger befo
-0000edd0: 7265 2069 6d70 6f72 7469 6e67 2074 6865  re importing the
-0000ede0: 206c 6962 7261 7279 2074 6f20 6265 2061   library to be a
-0000edf0: 626c 6520 746f 2073 6565 2074 6865 206c  ble to see the l
-0000ee00: 6f67 732e 5f0d 0a0d 0a23 2320 546f 2077  ogs._....## To w
-0000ee10: 686f 6d20 646f 2049 2074 616c 6b20 746f  hom do I talk to
-0000ee20: 3f20 2323 0d0a 0d0a 2a20 546f 6f6c 7320  ? ##....* Tools 
-0000ee30: 7765 6273 6974 6520 3a20 5b68 7474 7073  website : [https
-0000ee40: 3a2f 2f77 7777 2e6e 756e 6f62 7275 6d2e  ://www.nunobrum.
-0000ee50: 636f 6d2f 7079 6c74 7370 6963 652e 6874  com/pyltspice.ht
-0000ee60: 6d6c 5d28 6874 7470 733a 2f2f 7777 772e  ml](https://www.
-0000ee70: 6e75 6e6f 6272 756d 2e63 6f6d 2f70 796c  nunobrum.com/pyl
-0000ee80: 7473 7069 6365 2e68 746d 6c29 0d0a 2a20  tspice.html)..* 
-0000ee90: 5265 706f 206f 776e 6572 203a 205b 6d65  Repo owner : [me
-0000eea0: 406e 756e 6f62 7275 6d2e 636f 6d5d 286d  @nunobrum.com](m
-0000eeb0: 6169 6c74 6f3a 6d65 406e 756e 6f62 7275  ailto:me@nunobru
-0000eec0: 6d2e 636f 6d29 0d0a 2a20 416c 7465 726e  m.com)..* Altern
-0000eed0: 6174 6976 6520 636f 6e74 6163 7420 3a20  ative contact : 
-0000eee0: 5b6e 756e 6f2e 6272 756d 4067 6d61 696c  [nuno.brum@gmail
-0000eef0: 2e63 6f6d 5d28 6d61 696c 746f 3a6e 756e  .com](mailto:nun
-0000ef00: 6f2e 6272 756d 4067 6d61 696c 2e63 6f6d  o.brum@gmail.com
-0000ef10: 290d 0a0d 0a23 2320 4869 7374 6f72 7920  )....## History 
-0000ef20: 2323 0d0a 2a20 5665 7273 696f 6e20 352e  ##..* Version 5.
-0000ef30: 332e 300d 0a20 202a 2048 6965 7261 7263  3.0..  * Hierarc
-0000ef40: 6869 6361 6c20 5375 7070 6f72 7420 2841  hical Support (A
-0000ef50: 6c69 676e 696e 6720 7769 7468 2074 6865  ligning with the
-0000ef60: 2073 7069 6365 6c69 6220 312e 312e 3129   spicelib 1.1.1)
-0000ef70: 0d0a 2a20 5665 7273 696f 6e20 352e 322e  ..* Version 5.2.
-0000ef80: 330d 0a20 202a 2055 7064 6174 696e 6720  3..  * Updating 
-0000ef90: 6c6f 6767 6572 7320 746f 2075 7365 2074  loggers to use t
-0000efa0: 6865 2022 7370 6963 656c 6962 2220 4944  he "spicelib" ID
-0000efb0: 732e 0d0a 2020 2a20 4669 7869 6e67 2061  s...  * Fixing a
-0000efc0: 7574 6f64 6f63 2065 7272 6f72 730d 0a20  utodoc errors.. 
-0000efd0: 202a 2043 6f72 7265 6374 696e 6720 5665   * Correcting Ve
-0000efe0: 7273 696f 6e20 7265 6665 7265 6e63 6573  rsion references
-0000eff0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 352e  ....* Version 5.
-0000f000: 322e 320d 0a20 202a 2046 6978 6573 206f  2.2..  * Fixes o
-0000f010: 6e20 7468 6520 756e 6974 7465 7374 7320  n the unittests 
-0000f020: 6166 7465 7220 7468 6520 7370 6963 656c  after the spicel
-0000f030: 6962 2075 7064 6174 6520 746f 2031 2e30  ib update to 1.0
-0000f040: 2e34 0d0a 0d0a 2a20 5665 7273 696f 6e20  .4....* Version 
-0000f050: 352e 322e 310d 0a20 202a 2043 6f72 7265  5.2.1..  * Corre
-0000f060: 6374 696f 6e20 6f6e 2074 6865 2072 756e  ction on the run
-0000f070: 5f6d 6f6e 7465 6361 726c 6f2e 7079 2061  _montecarlo.py a
-0000f080: 6e64 2072 756e 5f77 6f72 7374 5f63 6173  nd run_worst_cas
-0000f090: 652e 7079 2065 7861 6d70 6c65 732e 0d0a  e.py examples...
-0000f0a0: 2020 2a20 4669 7865 7320 6f6e 2074 6865    * Fixes on the
-0000f0b0: 2073 7069 6365 6c69 6220 2856 6572 7369   spicelib (Versi
-0000f0c0: 6f6e 2031 2e30 2e33 290d 0a0d 0a2a 2056  on 1.0.3)....* V
-0000f0d0: 6572 7369 6f6e 2035 2e32 0d0a 2020 2a20  ersion 5.2..  * 
-0000f0e0: 5369 6d41 6e61 6c79 7369 7320 7375 7070  SimAnalysis supp
-0000f0f0: 6f72 7469 6e67 2062 6f74 6820 5173 7069  orting both Qspi
-0000f100: 6365 2061 6e64 204c 5453 7069 6365 206c  ce and LTSpice l
-0000f110: 6f67 6669 6c65 732e 0d0a 2020 2a20 4661  ogfiles...  * Fa
-0000f120: 7374 576f 7273 7443 6173 6541 6e61 6c79  stWorstCaseAnaly
-0000f130: 7369 7320 616c 676f 7269 7468 6d20 696d  sis algorithm im
-0000f140: 706c 656d 656e 7465 640d 0a20 202a 2046  plemented..  * F
-0000f150: 6978 206f 6e20 7468 6520 6c6f 6720 7265  ix on the log re
-0000f160: 6164 696e 6720 6f66 2066 6f75 7269 6572  ading of fourier
-0000f170: 2064 6174 612e 0d0a 0d0a 2a20 5665 7273   data.....* Vers
-0000f180: 696f 6e20 352e 310d 0a20 202a 2049 6d70  ion 5.1..  * Imp
-0000f190: 6f72 7461 6e74 2042 7567 6669 7820 6f6e  ortant Bugfix on
-0000f1a0: 2074 6865 204c 5443 6f6d 706c 6578 2063   the LTComplex c
-0000f1b0: 6c61 7373 2e0d 0a20 202a 2046 6978 6573  lass...  * Fixes
-0000f1c0: 2061 6e64 2065 6e68 616e 6369 6e67 2074   and enhancing t
-0000f1d0: 6865 2061 6e61 6c79 7369 7320 746f 6f6c  he analysis tool
-0000f1e0: 6b69 742e 0d0a 2020 2a20 4465 7072 6563  kit...  * Deprec
-0000f1f0: 6174 696e 6720 5370 6963 6545 6469 746f  ating SpiceEdito
-0000f200: 722e 7772 6974 655f 6e65 746c 6973 7420  r.write_netlist 
-0000f210: 696e 2066 6176 6f75 7220 6f66 2073 6176  in favour of sav
-0000f220: 655f 6e65 746c 6973 7428 290d 0a0d 0a2a  e_netlist()....*
-0000f230: 2056 6572 7369 6f6e 2035 2e30 0d0a 2020   Version 5.0..  
-0000f240: 2a20 4d61 6b69 6e67 2074 6869 7320 6c69  * Making this li
-0000f250: 6272 6172 7920 6465 7065 6e64 656e 7420  brary dependent 
-0000f260: 6f6e 2073 7069 6365 6c69 6220 7768 696c  on spicelib whil
-0000f270: 6520 7472 7969 6e67 2074 6f20 6d61 696e  e trying to main
-0000f280: 7461 696e 2062 6163 6b77 6172 6420 636f  tain backward co
-0000f290: 6d70 6174 6962 696c 6974 7920 6173 206d  mpatibility as m
-0000f2a0: 7563 6820 6173 2070 6f73 7369 626c 652e  uch as possible.
-0000f2b0: 200d 0a20 2050 794c 5473 7069 6365 2077   ..  PyLTspice w
-0000f2c0: 696c 6c20 6265 206b 6570 7420 616c 6976  ill be kept aliv
-0000f2d0: 6520 616e 6420 6974 7320 7570 6461 7465  e and its update
-0000f2e0: 2077 696c 6c20 6265 206c 696e 6b65 6420   will be linked 
-0000f2f0: 746f 2074 6865 2073 7069 6365 6c69 622e  to the spicelib.
-0000f300: 2054 6865 206d 6169 6e20 6469 6666 6572   The main differ
-0000f310: 656e 6365 2069 7320 7468 6174 2075 7369  ence is that usi
-0000f320: 6e67 0d0a 2020 5079 4c54 7370 6963 6520  ng..  PyLTspice 
-0000f330: 7769 6c6c 2061 7665 7274 2074 6865 206e  will avert the n
-0000f340: 6565 6420 6f66 2068 6176 696e 6720 746f  eed of having to
-0000f350: 2073 656c 6563 7420 6120 7369 6d75 6c61   select a simula
-0000f360: 746f 7220 696e 2061 6c6c 2072 756e 2063  tor in all run c
-0000f370: 6f6d 6d61 6e64 732e 0d0a 0d0a 2a20 5665  ommands.....* Ve
-0000f380: 7273 696f 6e20 342e 312e 320d 0a20 202a  rsion 4.1.2..  *
-0000f390: 2041 6464 696e 6720 7375 7070 6f72 7420   Adding support 
-0000f3a0: 666f 7220 7468 6520 6e65 7720 5153 5049  for the new QSPI
-0000f3b0: 4345 2073 696d 756c 6174 6f72 0d0a 2020  CE simulator..  
-0000f3c0: 2a20 496d 7072 6f76 696e 6720 7468 6520  * Improving the 
-0000f3d0: 7469 6d65 6f75 7420 6d65 6368 616e 6973  timeout mechanis
-0000f3e0: 6d20 6f6e 2074 6865 2053 696d 5275 6e6e  m on the SimRunn
-0000f3f0: 6572 2063 6c61 7373 0d0a 2020 2a20 4d69  er class..  * Mi
-0000f400: 6e6f 7220 6275 6720 6669 7865 730d 0a0d  nor bug fixes...
-0000f410: 0a2a 2056 6572 7369 6f6e 2034 2e31 2e31  .* Version 4.1.1
-0000f420: 0d0a 2020 2a20 436f 6d70 6c65 7469 6e67  ..  * Completing
-0000f430: 2074 6865 2057 6f72 7374 2d43 6173 6520   the Worst-Case 
-0000f440: 416e 616c 7973 6973 2066 756e 6374 696f  Analysis functio
-0000f450: 6e73 2e20 4164 6469 6e67 2061 2064 6564  ns. Adding a ded
-0000f460: 6963 6174 6564 2065 7861 6d70 6c65 2066  icated example f
-0000f470: 6f72 2069 742e 0d0a 2020 2a20 5265 6661  or it...  * Refa
-0000f480: 6374 6f72 696e 6720 7468 6520 4c54 5370  ctoring the LTSp
-0000f490: 6963 654c 6f67 5265 6164 6572 2063 6c61  iceLogReader cla
-0000f4a0: 7373 2069 6e20 6f72 6465 7220 746f 2075  ss in order to u
-0000f4b0: 7365 2069 7420 6f6e 2074 6865 2041 6e61  se it on the Ana
-0000f4c0: 6c79 7369 7320 746f 6f6c 6b69 740d 0a0d  lysis toolkit...
-0000f4d0: 0a2a 2056 6572 7369 6f6e 2034 2e31 2e30  .* Version 4.1.0
-0000f4e0: 202a 2872 6571 7569 7265 7320 5079 7468   *(requires Pyth
-0000f4f0: 6f6e 2033 2e38 206f 7220 6869 6768 6572  on 3.8 or higher
-0000f500: 292a 0d0a 2020 2020 2a20 4164 6469 6e67  )*..    * Adding
-0000f510: 2061 206e 6577 2063 6c61 7373 2074 6f20   a new class to 
-0000f520: 6d61 6e69 7075 6c61 7465 2064 6972 6563  manipulate direc
-0000f530: 746c 7920 7468 6520 2e61 7363 2066 696c  tly the .asc fil
-0000f540: 6573 2e0d 0a20 2020 202a 204d 6f64 6966  es...    * Modif
-0000f550: 7969 6e67 2061 6c6c 2074 6865 206f 7468  ying all the oth
-0000f560: 6572 2063 6c61 7373 6573 2069 6e20 6f72  er classes in or
-0000f570: 6465 7220 746f 2075 7365 2074 6865 206e  der to use the n
-0000f580: 6577 2063 6c61 7373 2e0d 0a20 2020 202a  ew class...    *
-0000f590: 2041 6464 696e 6720 636c 6173 7365 7320   Adding classes 
-0000f5a0: 746f 2070 6572 666f 726d 204d 6f6e 7465  to perform Monte
-0000f5b0: 6361 726c 6f20 616e 6420 776f 7273 7420  carlo and worst 
-0000f5c0: 6361 7365 2061 6e61 6c79 7369 7320 2854  case analysis (T
-0000f5d0: 6861 6e6b 7320 746f 2040 6d76 616e 7269  hanks to @mvanri
-0000f5e0: 6574 2066 6f72 2068 6973 2073 7461 7274  et for his start
-0000f5f0: 696e 6720 7468 6973 292e 0d0a 2020 2020  ing this)...    
-0000f600: 2a20 5265 6d6f 7669 6e67 2074 6865 2064  * Removing the d
-0000f610: 6570 7265 6361 7465 6420 4c54 5370 6963  eprecated LTSpic
-0000f620: 655f 5261 7752 6561 642e 7079 2c20 4c54  e_RawRead.py, LT
-0000f630: 5370 6963 655f 5261 7757 7269 7465 2e70  Spice_RawWrite.p
-0000f640: 7920 616e 6420 4c54 5370 6963 6542 6174  y and LTSpiceBat
-0000f650: 6368 2e70 7920 6669 6c65 7320 616e 6420  ch.py files and 
-0000f660: 7265 7370 6563 7469 7665 2063 6c61 7373  respective class
-0000f670: 6573 2e0d 0a20 2020 202a 2052 6573 7472  es...    * Restr
-0000f680: 7563 7475 7265 6420 7468 6520 666f 6c64  uctured the fold
-0000f690: 6572 2073 7472 7563 7475 7265 2074 6f20  er structure to 
-0000f6a0: 6265 206d 6f72 6520 696e 206c 696e 6520  be more in line 
-0000f6b0: 7769 7468 2074 6865 2050 7974 686f 6e20  with the Python 
-0000f6c0: 7374 616e 6461 7264 732e 0d0a 2020 2020  standards...    
-0000f6d0: 2a20 4164 6465 6420 616e 2045 7861 6d70  * Added an Examp
-0000f6e0: 6c65 7320 666f 6c64 6572 2077 6974 6820  les folder with 
-0000f6f0: 736f 6d65 2065 7861 6d70 6c65 7320 6f6e  some examples on
-0000f700: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
-0000f710: 6c69 6272 6172 792e 0d0a 0d0a 2a20 5665  library.....* Ve
-0000f720: 7273 696f 6e20 342e 302e 360d 0a20 2020  rsion 4.0.6..   
-0000f730: 202a 2046 6978 696e 6720 6973 7375 6520   * Fixing issue 
-0000f740: 7769 7468 2074 6865 2077 7269 7465 5f6e  with the write_n
-0000f750: 6574 6c69 7374 2829 2066 756e 6374 696f  etlist() functio
-0000f760: 6e20 7768 656e 2072 6563 6569 7669 6e67  n when receiving
-0000f770: 2061 2073 7472 696e 6720 696e 7374 6561   a string instea
-0000f780: 6420 6f66 2061 2070 6174 686c 6962 2e50  d of a pathlib.P
-0000f790: 6174 6820 6f62 6a65 6374 2e0d 0a20 2020  ath object...   
-0000f7a0: 202a 2043 6861 6e67 696e 6720 7468 6520   * Changing the 
-0000f7b0: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
-0000f7c0: 6f6e 2066 6f72 2074 6865 2072 6573 6973  on for the resis
-0000f7d0: 746f 7220 696e 206f 7264 6572 2074 6f20  tor in order to 
-0000f7e0: 6163 6365 7074 2074 6865 2052 3d20 7072  accept the R= pr
-0000f7f0: 6566 6978 206f 6e20 7468 6520 7661 6c75  efix on the valu
-0000f800: 6573 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  es.....* Version
-0000f810: 2034 2e30 2e35 0d0a 2020 2020 2a20 4163   4.0.5..    * Ac
-0000f820: 6365 7074 696e 6720 6669 7865 7320 6672  cepting fixes fr
-0000f830: 6f6d 2061 616e 6173 2d73 6179 6564 4047  om aanas-sayed@G
-0000f840: 6974 4875 6220 7468 6174 2066 6978 6573  itHub that fixes
-0000f850: 2069 7373 7565 7320 7769 7468 2072 756e   issues with run
-0000f860: 6e69 6e67 2074 6865 204c 5453 7069 6365  ning the LTSpice
-0000f870: 2069 6e20 4c69 6e75 782e 0d0a 0d0a 2a20   in Linux.....* 
-0000f880: 5665 7273 696f 6e20 342e 302e 340d 0a20  Version 4.0.4.. 
-0000f890: 2020 202a 2049 6d70 726f 7665 6420 7573     * Improved us
-0000f8a0: 6167 6520 6f66 2074 6865 206c 6f67 6769  age of the loggi
-0000f8b0: 6e67 206c 6962 7261 7279 2e20 2854 6861  ng library. (Tha
-0000f8c0: 6e6b 7320 4054 5370 7265 6368 2066 6f72  nks @TSprech for
-0000f8d0: 2076 6173 746c 7920 696d 7072 6f76 696e   vastly improvin
-0000f8e0: 6720 7468 6520 6c6f 6767 696e 6729 0d0a  g the logging)..
-0000f8f0: 2020 2020 2a20 496e 636c 7564 6564 2052      * Included R
-0000f900: 756e 5461 736b 206e 756d 6265 7220 696e  unTask number in
-0000f910: 2074 6865 206c 6f67 206d 6573 7361 6765   the log message
-0000f920: 732e 0d0a 2020 2020 2a20 496e 636c 7564  s...    * Includ
-0000f930: 6564 206d 696c 6c69 7365 636f 6e64 7320  ed milliseconds 
-0000f940: 696e 2074 6865 2074 696d 6520 656c 6170  in the time elap
-0000f950: 7365 6420 6361 6c63 756c 6174 696f 6e2e  sed calculation.
-0000f960: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
-0000f970: 302e 330d 0a20 2020 202a 2046 6978 696e  0.3..    * Fixin
-0000f980: 6720 6973 7375 6520 696e 2065 6c61 7073  g issue in elaps
-0000f990: 6564 2074 696d 6520 6361 6c63 756c 6174  ed time calculat
-0000f9a0: 696f 6e2e 0d0a 2020 2020 2a20 4669 7869  ion...    * Fixi
-0000f9b0: 6e67 2069 7373 7565 2077 6974 6820 7468  ng issue with th
-0000f9c0: 6520 696d 706f 7274 206f 6620 4c54 5370  e import of LTSp
-0000f9d0: 6963 654c 6f67 5265 6164 6572 2066 726f  iceLogReader fro
-0000f9e0: 6d20 4c54 5374 6570 732e 7079 0d0a 0d0a  m LTSteps.py....
-0000f9f0: 2a20 5665 7273 696f 6e20 342e 302e 320d  * Version 4.0.2.
-0000fa00: 0a20 2020 202a 2043 6861 6e67 696e 6720  .    * Changing 
-0000fa10: 6c69 7374 206f 6620 4c69 6272 6172 7920  list of Library 
-0000fa20: 6465 7065 6e64 656e 6369 6573 2e0d 0a0d  dependencies....
-0000fa30: 0a2a 2056 6572 7369 6f6e 2034 2e30 2e31  .* Version 4.0.1
-0000fa40: 0d0a 2020 2020 2a20 4275 6720 6669 7820  ..    * Bug fix 
-0000fa50: 6f6e 2043 4c49 2066 6f72 2074 6865 2048  on CLI for the H
-0000fa60: 6973 746f 6772 616d 2e70 7920 616e 6420  istogram.py and 
-0000fa70: 4c54 5374 6570 732e 7079 0d0a 0d0a 2a20  LTSteps.py....* 
-0000fa80: 5665 7273 696f 6e20 342e 302e 300d 0a20  Version 4.0.0.. 
-0000fa90: 2020 202a 2053 6570 6172 6174 696e 6720     * Separating 
-0000faa0: 7468 6520 5369 6d43 6f6d 6d61 6e64 6572  the SimCommander
-0000fab0: 2069 6e74 6f20 7477 6f20 7365 7061 7261   into two separa
-0000fac0: 7465 2063 6c61 7373 6573 2c20 6f6e 6520  te classes, one 
-0000fad0: 666f 7220 7468 6520 7370 6963 6520 6e65  for the spice ne
-0000fae0: 746c 6973 7420 6564 6974 696e 6720 2853  tlist editing (S
-0000faf0: 7069 6365 4564 6974 6f72 2920 616e 6420  piceEditor) and 
-0000fb00: 616e 6f74 6865 720d 0a20 2020 2020 2066  another..      f
-0000fb10: 6f72 2074 6865 2073 696d 756c 6174 696f  or the simulatio
-0000fb20: 6e20 6578 6563 7574 696f 6e20 2853 696d  n execution (Sim
-0000fb30: 5275 6e6e 6572 292e 0d0a 2020 2020 2a20  Runner)...    * 
-0000fb40: 496d 706c 656d 656e 7469 6e67 2073 696d  Implementing sim
-0000fb50: 756c 6174 696f 6e20 7365 7276 6572 2074  ulation server t
-0000fb60: 6f20 616c 6c6f 7720 666f 7220 7265 6d6f  o allow for remo
-0000fb70: 7465 2073 696d 756c 6174 696f 6e20 6578  te simulation ex
-0000fb80: 6563 7574 696f 6e20 616e 6420 7468 6520  ecution and the 
-0000fb90: 7265 7370 6563 7469 7665 2063 6c69 656e  respective clien
-0000fba0: 742e 0d0a 2020 2020 2a20 5375 7070 6f72  t...    * Suppor
-0000fbb0: 7469 6e67 2057 6967 676c 6572 2065 6c65  ting Wiggler ele
-0000fbc0: 6d65 6e74 2069 6e20 7468 6520 6e65 7720  ment in the new 
-0000fbd0: 4c54 5370 6963 6558 5649 492e 0d0a 2020  LTSpiceXVII...  
-0000fbe0: 2020 2a20 5265 6e61 6d69 6e67 2061 6c6c    * Renaming all
-0000fbf0: 2066 696c 6573 2069 6e74 6f20 6c6f 7765   files into lowe
-0000fc00: 7263 6173 652e 0d0a 2020 2020 2a20 4372  rcase...    * Cr
-0000fc10: 6561 7469 6e67 2045 7272 6f72 2063 6c61  eating Error cla
-0000fc20: 7373 6573 2066 6f72 2062 6574 7465 7220  sses for better 
-0000fc30: 6572 726f 7220 6861 6e64 6c69 6e67 2e0d  error handling..
-0000fc40: 0a20 2020 202a 2041 6464 696e 6720 7375  .    * Adding su
-0000fc50: 7070 6f72 7420 666f 7220 6f74 6865 7220  pport for other 
-0000fc60: 7369 6d75 6c61 746f 7273 2028 6578 3a20  simulators (ex: 
-0000fc70: 6e67 7370 6963 6529 2077 6865 7265 2074  ngspice) where t
-0000fc80: 6865 2073 696d 756c 6174 6f72 2069 7320  he simulator is 
-0000fc90: 6465 6669 6e65 6420 6279 2061 2063 6c61  defined by a cla
-0000fca0: 7373 2e20 5468 6973 0d0a 2020 2020 2020  ss. This..      
-0000fcb0: 7375 7070 6f72 7420 636c 6173 7320 6e65  support class ne
-0000fcc0: 6564 7320 746f 2062 6520 6120 7375 6263  eds to be a subc
-0000fcd0: 6c61 7373 206f 6620 7468 6520 6162 7374  lass of the abst
-0000fce0: 7261 6374 2063 6c61 7373 2053 696d 756c  ract class Simul
-0000fcf0: 6174 6f72 2e0d 0a20 2020 202a 2045 6e6f  ator...    * Eno
-0000fd00: 726d 6f75 7320 696d 7072 6f76 656d 656e  rmous improvemen
-0000fd10: 7420 696e 2074 6865 2064 6f63 756d 656e  t in the documen
-0000fd20: 7461 7469 6f6e 206f 6620 7468 6520 636f  tation of the co
-0000fd30: 6465 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  de.....* Version
-0000fd40: 2033 2e30 0d0a 2020 2020 2a20 456c 696d   3.0..    * Elim
-0000fd50: 696e 6174 696e 6720 7468 6520 4c54 5370  inating the LTSp
-0000fd60: 6963 6520 7072 6566 6978 6573 2066 726f  ice prefixes fro
-0000fd70: 6d20 6669 6c65 7320 616e 6420 636c 6173  m files and clas
-0000fd80: 7365 732e 0d0a 2020 2020 2a20 4164 6f70  ses...    * Adop
-0000fd90: 7469 6e67 2074 6865 206c 6f77 6572 6361  ting the lowerca
-0000fda0: 7365 2063 6f6e 7665 6e74 696f 6e20 666f  se convention fo
-0000fdb0: 7220 6669 6c65 6e61 6d65 732e 0d0a 0d0a  r filenames.....
-0000fdc0: 2a20 5665 7273 696f 6e20 322e 332e 310d  * Version 2.3.1.
-0000fdd0: 0a20 2020 202a 2042 7567 2066 6978 206f  .    * Bug fix o
-0000fde0: 6e20 7468 6520 7061 7261 6d65 7465 7220  n the parameter 
-0000fdf0: 7265 706c 6163 656d 656e 742e 0d0a 0d0a  replacement.....
-0000fe00: 2a20 5665 7273 696f 6e20 322e 330d 0a20  * Version 2.3.. 
-0000fe10: 2020 202a 2053 7570 706f 7274 696e 6720     * Supporting 
-0000fe20: 7468 6520 6372 6561 7469 6f6e 206f 6620  the creation of 
-0000fe30: 5241 5720 4e6f 6973 6520 416e 616c 7973  RAW Noise Analys
-0000fe40: 6973 0d0a 2020 2020 2a20 4275 6720 4669  is..    * Bug Fi
-0000fe50: 7865 7320 2853 6565 2047 6974 4875 6220  xes (See GitHub 
-0000fe60: 4c6f 6729 0d0a 0d0a 2a20 5665 7273 696f  Log)....* Versio
-0000fe70: 6e20 322e 320d 0a20 2020 202a 204d 616b  n 2.2..    * Mak
-0000fe80: 696e 6720 6e75 6d70 7920 6173 2061 2072  ing numpy as a r
-0000fe90: 6571 7569 7265 6d65 6e74 2061 6e64 2065  equirement and e
-0000fea0: 6c69 6d69 6e61 7469 6e67 2061 6c6c 2063  liminating all c
-0000feb0: 6f64 6520 7468 6174 2061 766f 6964 6564  ode that avoided
-0000fec0: 2074 6865 2075 7365 206f 6620 6e75 6d70   the use of nump
-0000fed0: 790d 0a20 2020 202a 2055 7369 6e67 206e  y..    * Using n
-0000fee0: 6577 2070 6163 6b61 6769 6e67 2074 6f6f  ew packaging too
-0000fef0: 6c0d 0a20 2020 202a 2046 6978 6573 206f  l..    * Fixes o
-0000ff00: 6e20 7468 6520 4c54 5370 6963 655f 5261  n the LTSpice_Ra
-0000ff10: 7757 7269 7465 0d0a 2020 2020 2a20 4669  wWrite..    * Fi
-0000ff20: 7865 7320 696e 2074 6865 2068 616e 646c  xes in the handl
-0000ff30: 696e 6720 6f66 2073 7465 7070 6564 206f  ing of stepped o
-0000ff40: 7065 7261 7469 6e67 2070 6f69 6e74 2073  perating point s
-0000ff50: 696d 756c 6174 696f 6e73 0d0a 0d0a 2a20  imulations....* 
-0000ff60: 5665 7273 696f 6e20 322e 310d 0a20 2020  Version 2.1..   
-0000ff70: 202a 2041 646f 7074 696e 6720 6d69 6e69   * Adopting mini
-0000ff80: 6d75 6d20 7079 7468 6f6e 2076 6572 7369  mum python versi
-0000ff90: 6f6e 2033 2e37 0d0a 2020 2020 2a20 5374  on 3.7..    * St
-0000ffa0: 6172 7469 6e67 2074 6f20 7573 6520 756e  arting to use un
-0000ffb0: 6974 2074 6573 7473 2074 6f20 7661 6c69  it tests to vali
-0000ffc0: 6461 7465 2061 6c6c 206d 6f64 756c 6573  date all modules
-0000ffd0: 2061 6e64 2069 6d70 726f 7669 6e67 2074   and improving t
-0000ffe0: 6573 7462 656e 6368 6573 0d0a 2020 2020  estbenches..    
-0000fff0: 2a20 436f 6d70 6174 6962 696c 6974 7920  * Compatibility 
-00010000: 7769 7468 204e 4753 7069 6365 0d0a 2020  with NGSpice..  
-00010010: 2020 2a20 4176 6f69 6469 6e67 2074 6865    * Avoiding the
-00010020: 2075 7365 206f 6620 7365 7475 702e 7079   use of setup.py
-00010030: 2061 7320 7065 7220 5045 5035 3137 2061   as per PEP517 a
-00010040: 6e64 2050 4550 3531 380d 0a20 2020 202a  nd PEP518..    *
-00010050: 2042 7567 2046 6978 6573 2028 5365 6520   Bug Fixes (See 
-00010060: 4769 7448 7562 206c 6f67 2066 6f72 206d  GitHub log for m
-00010070: 6f72 6520 696e 666f 726d 6174 696f 6e29  ore information)
-00010080: 0d0a 2020 2020 2a20 496d 7072 6f76 656d  ..    * Improvem
-00010090: 656e 7473 206f 6e20 7468 6520 6d61 6e61  ents on the mana
-000100a0: 6765 6d65 6e74 206f 6620 7374 6570 7065  gement of steppe
-000100b0: 6420 6461 7461 2069 6e20 7468 6520 4c54  d data in the LT
-000100c0: 5370 6963 655f 5261 7752 6561 642e 7079  Spice_RawRead.py
-000100d0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 322e  ....* Version 2.
-000100e0: 302e 320d 0a20 2020 202a 2049 6d70 726f  0.2..    * Impro
-000100f0: 7665 6d65 6e74 7320 6f6e 2045 6e63 6f64  vements on Encod
-00010100: 696e 6720 6465 7465 6374 696f 6e0d 0a0d  ing detection...
-00010110: 0a2a 2056 6572 7369 6f6e 2032 2e30 0d0a  .* Version 2.0..
-00010120: 2020 2020 2a20 496e 7465 726e 6174 696f      * Internatio
-00010130: 6e61 6c20 5375 7070 6f72 7420 7573 696e  nal Support usin
-00010140: 6720 7468 6520 636f 7272 6563 7420 656e  g the correct en
-00010150: 636f 6469 6e67 2077 6865 6e20 6c6f 6164  coding when load
-00010160: 696e 6720 6c6f 6720 6669 6c65 732e 0d0a  ing log files...
-00010170: 2020 2020 2a20 436f 6465 204f 7074 696d      * Code Optim
-00010180: 697a 6174 696f 6e73 206f 6e20 7468 6520  izations on the 
-00010190: 4c54 5370 6963 655f 5261 7752 6561 6465  LTSpice_RawReade
-000101a0: 7220 7468 6174 2061 6c6c 6f77 2066 6173  r that allow fas
-000101b0: 7465 7220 6461 7461 206c 6f61 6469 6e67  ter data loading
-000101c0: 2e0d 0a20 2020 202a 2049 6d70 726f 7669  ...    * Improvi
-000101d0: 6e67 2074 6865 2066 756e 6374 696f 6e61  ng the functiona
-000101e0: 6c69 7479 206f 6e20 7468 6520 4c54 5370  lity on the LTSp
-000101f0: 6963 655f 5261 7757 7269 7465 722e 7079  ice_RawWriter.py
-00010200: 0d0a 2020 2020 2a20 4164 6469 6e67 2073  ..    * Adding s
-00010210: 7570 706f 7274 2074 6f20 6564 6974 696e  upport to editin
-00010220: 6720 636f 6d70 6f6e 656e 7473 2069 6e73  g components ins
-00010230: 6964 6520 7375 6263 6972 6375 6974 7320  ide subcircuits 
-00010240: 282e 7375 6263 6b74 290d 0a20 2020 202a  (.subckt)..    *
-00010250: 2053 7570 706f 7274 696e 6720 7265 7369   Supporting resi
-00010260: 7374 6f72 7320 7769 7468 204d 6f64 656c  stors with Model
-00010270: 2044 6566 696e 6974 696f 6e73 0d0a 2020   Definitions..  
-00010280: 2020 2a20 4669 7869 6e67 2070 726f 626c    * Fixing probl
-00010290: 656d 2077 6974 6820 4c54 5370 6963 654c  em with LTSpiceL
-000102a0: 6f67 5265 6164 6572 2074 6861 7420 776f  ogReader that wo
-000102b0: 756c 6420 7265 7475 726e 206d 6573 7365  uld return messe
-000102c0: 6420 7570 2064 6174 610d 0a20 2020 202a  d up data..    *
-000102d0: 2046 6978 696e 6720 7072 6f62 6c65 6d20   Fixing problem 
-000102e0: 7769 7468 2072 6570 6c61 6369 6e67 2074  with replacing t
-000102f0: 6865 2066 696c 6520 6578 7465 6e73 696f  he file extensio
-00010300: 6e20 696e 2063 6572 7461 696e 206e 616d  n in certain nam
-00010310: 6573 0d0a 2020 2020 2a20 436f 7272 6563  es..    * Correc
-00010320: 7469 6e67 2070 726f 626c 656d 2077 6974  ting problem wit
-00010330: 6820 6465 7072 6563 6174 696f 6e73 206f  h deprecations o
-00010340: 6e20 7468 6520 6e75 6d70 7920 6675 6e63  n the numpy func
-00010350: 7469 6f6e 7320 7573 6564 2062 7920 7468  tions used by th
-00010360: 6520 4869 7374 6f67 7261 6d2e 7079 0d0a  e Histogram.py..
-00010370: 2020 2020 2a20 4164 6469 6e67 2062 6163      * Adding bac
-00010380: 6b20 7468 6520 5245 4144 4d45 2e6d 6420  k the README.md 
-00010390: 7468 6174 2073 6f6d 6568 6f77 2077 6173  that somehow was
-000103a0: 2064 656c 6574 6564 0d0a 0d0a 2a20 5665   deleted....* Ve
-000103b0: 7273 696f 6e20 312e 390d 0a20 2020 202a  rsion 1.9..    *
-000103c0: 2041 6464 696e 6720 7375 7070 6f72 7420   Adding support 
-000103d0: 666f 7220 c2b5 2063 6861 7261 6374 6572  for .. character
-000103e0: 2069 6e20 7468 6520 5370 6963 6545 6469   in the SpiceEdi
-000103f0: 746f 722e 0d0a 2020 2020 2a20 4164 6469  tor...    * Addi
-00010400: 6e67 2067 6574 5f63 6f6d 706f 6e65 6e74  ng get_component
-00010410: 5f66 6c6f 6174 7661 6c75 6528 2920 6d65  _floatvalue() me
-00010420: 7468 6f64 2069 6e20 7468 6520 6e65 746c  thod in the netl
-00010430: 6973 7420 6d61 6e69 7075 6c61 7469 6e67  ist manipulating
-00010440: 2063 6c61 7373 2074 6861 7420 6861 6e64   class that hand
-00010450: 6c65 7320 7468 6520 636f 6e76 6572 7369  les the conversi
-00010460: 6f6e 206f 6620 6e75 6d65 7269 630d 0a20  on of numeric.. 
-00010470: 2020 2020 2066 6965 6c64 7320 696e 746f       fields into
-00010480: 2061 2066 6c6f 6174 2e20 5468 6973 2066   a float. This f
-00010490: 756e 6374 696f 6e20 7461 6b65 7320 696e  unction takes in
-000104a0: 746f 2061 6363 6f75 6e74 2074 6865 2065  to account the e
-000104b0: 6e67 696e 6565 7269 6e67 2071 7561 6c69  ngineering quali
-000104c0: 6669 6572 7320 276b 2720 666f 7220 6b69  fiers 'k' for ki
-000104d0: 6c6f 732c 2027 6d27 206f 7220 6d69 6c69  los, 'm' or mili
-000104e0: 732c 0d0a 2020 2020 2020 2775 2720 6f72  s,..      'u' or
-000104f0: 2027 c2b5 2720 666f 7220 6d69 6372 6f6e   '..' for micron
-00010500: 732c 2027 6e27 2066 6f72 206e 616e 6f73  s, 'n' for nanos
-00010510: 2c20 2766 2720 666f 7220 6665 6d74 6f73  , 'f' for femtos
-00010520: 2061 6e64 2027 4d65 6727 2066 6f72 204d   and 'Meg' for M
-00010530: 6567 6173 2e0d 0a0d 0a2a 2056 6572 7369  egas.....* Versi
-00010540: 6f6e 2031 2e38 0d0a 2020 2020 2a20 556e  on 1.8..    * Un
-00010550: 6966 6f72 6d69 6e67 204c 6963 656e 7365  iforming License
-00010560: 2072 6566 6572 656e 6365 2061 6372 6f73   reference acros
-00010570: 7320 6669 6c65 7320 616e 6420 696d 7072  s files and impr
-00010580: 6f76 656d 656e 7473 206f 6e20 7468 6520  ovements on the 
-00010590: 646f 6375 6d65 6e74 6174 696f 6e0d 0a20  documentation.. 
-000105a0: 2020 202a 2041 6e20 656e 6f72 6d6f 7573     * An enormous
-000105b0: 2061 6e64 2077 686f 6c65 6865 6172 7465   and wholehearte
-000105c0: 6420 7468 616e 6b73 2074 6f20 406c 7068  d thanks to @lph
-000105d0: 6572 7220 666f 7220 7468 6520 696d 7072  err for the impr
-000105e0: 6f76 656d 656e 7473 2069 6e20 7468 6520  ovements in the 
-000105f0: 646f 6375 6d65 6e74 6174 696f 6e2e 0d0a  documentation...
-00010600: 2020 2020 2a20 4275 6766 6978 206f 6e20      * Bugfix on 
-00010610: 7468 6520 6164 645f 4c54 7370 6963 6552  the add_LTspiceR
-00010620: 756e 436d 644c 696e 6553 7769 7463 6865  unCmdLineSwitche
-00010630: 7328 2920 3b20 5375 7070 6f72 7469 6e67  s() ; Supporting
-00010640: 202e 7061 7261 6d20 6e61 6d65 2076 616c   .param name val
-00010650: 7565 2066 6f72 6d61 740d 0a20 2020 202a  ue format..    *
-00010660: 2041 6c6c 6f77 696e 6720 7468 6520 4c54   Allowing the LT
-00010670: 5370 6963 6552 6177 5265 6164 2074 6f20  SpiceRawRead to 
-00010680: 7072 6f63 6565 6420 7768 656e 2074 6865  proceed when the
-00010690: 206c 6f67 2066 696c 6520 6361 6e27 7420   log file can't 
-000106a0: 6265 2066 6f75 6e64 206f 7220 7768 656e  be found or when
-000106b0: 2074 6865 7265 2061 7265 2070 726f 626c   there are probl
-000106c0: 656d 7320 7265 6164 696e 6720 6974 2e0d  ems reading it..
-000106d0: 0a2a 2056 6572 7369 6f6e 2031 2e37 0d0a  .* Version 1.7..
-000106e0: 2020 2020 2a20 5275 6e6e 696e 6720 696e      * Running in
-000106f0: 204c 696e 7578 2075 6e64 6572 2077 696e   Linux under win
-00010700: 6520 6973 206e 6f77 2070 6f73 7369 626c  e is now possibl
-00010710: 650d 0a0d 0a2a 2056 6572 7369 6f6e 2031  e....* Version 1
-00010720: 2e36 0d0a 2020 2020 2a20 4164 6469 6e67  .6..    * Adding
-00010730: 204c 5453 7069 6365 5f52 6177 5772 6974   LTSpice_RawWrit
-00010740: 652e 2041 6464 696e 6720 646f 6375 6d65  e. Adding docume
-00010750: 6e74 6174 696f 6e2e 0d0a 0d0a 2a20 5665  ntation.....* Ve
-00010760: 7273 696f 6e20 312e 350d 0a20 2020 202a  rsion 1.5..    *
-00010770: 2053 6d61 6c6c 2066 6978 6573 2061 6e64   Small fixes and
-00010780: 2069 6d70 726f 7665 6d65 6e74 7320 6f6e   improvements on
-00010790: 2074 6865 2063 6c61 7373 2075 7361 6765   the class usage
-000107a0: 2e20 4e6f 2061 6464 6564 2066 6561 7475  . No added featu
-000107b0: 7265 730d 0a0d 0a2a 2056 6572 7369 6f6e  res....* Version
-000107c0: 2031 2e34 0d0a 2020 2020 2a20 4164 6469   1.4..    * Addi
-000107d0: 6e67 2074 6865 204c 5453 7069 6365 5f53  ng the LTSpice_S
-000107e0: 656d 6944 6576 4f70 5265 6164 6572 206d  emiDevOpReader m
-000107f0: 6f64 756c 650d 0a20 2020 202a 2052 652d  odule..    * Re-
-00010800: 656e 6162 6c69 6e67 2074 6865 2048 6973  enabling the His
-00010810: 746f 6772 616d 2066 756e 6374 696f 6e73  togram functions
-00010820: 2077 6869 6368 2077 6865 7265 2064 6973   which where dis
-00010830: 6162 6c65 6420 6279 206d 6973 7461 6b65  abled by mistake
-00010840: 2e0d 0a0d 0a2a 2056 6572 7369 6f6e 2031  .....* Version 1
-00010850: 2e33 0d0a 2020 2020 2a20 4275 6720 6669  .3..    * Bug fi
-00010860: 7865 7320 6f6e 2074 6865 2053 7069 6365  xes on the Spice
-00010870: 4564 6974 6f72 2043 6c61 7373 0d0a 0d0a  Editor Class....
-00010880: 2a20 5665 7273 696f 6e20 312e 320d 0a20  * Version 1.2.. 
-00010890: 2020 202a 2052 4541 444d 452e 6d64 3a0d     * README.md:.
-000108a0: 0a20 2020 2020 2041 6464 696e 6720 6c69  .      Adding li
-000108b0: 6e6b 2074 6f20 7265 6164 7468 6564 6f63  nk to readthedoc
-000108c0: 7320 646f 6375 6d65 6e74 6174 696f 6e0d  s documentation.
-000108d0: 0a20 2020 202a 2041 6c6c 2066 696c 6573  .    * All files
-000108e0: 3a0d 0a20 2020 2020 2043 6f6d 7072 6568  :..      Compreh
-000108f0: 656e 7369 7665 2064 6f63 756d 656e 7461  ensive documenta
-00010900: 7469 6f6e 206f 6e20 686f 7720 746f 2075  tion on how to u
-00010910: 7365 2065 6163 6820 6d6f 6475 6c65 0d0a  se each module..
-00010920: 0d0a 2a20 5665 7273 696f 6e20 312e 310d  ..* Version 1.1.
-00010930: 0a20 2020 202a 2052 4541 444d 452e 6d64  .    * README.md
-00010940: 3a0d 0a20 2020 2020 2055 7064 6174 6564  :..      Updated
-00010950: 2074 6865 2064 6573 6372 6970 7469 6f6e   the description
-00010960: 0d0a 2020 2020 2a20 4c54 5370 6963 6542  ..    * LTSpiceB
-00010970: 6174 6368 2e70 793a 0d0a 2020 2020 2020  atch.py:..      
-00010980: 436f 7272 6563 7465 6420 7468 6520 6e61  Corrected the na
-00010990: 6d65 206f 6620 7468 6520 7265 7475 726e  me of the return
-000109a0: 6564 2072 6177 2066 696c 652e 0d0a 2020  ed raw file...  
-000109b0: 2020 2a20 4164 6465 6420 636f 6d6d 656e    * Added commen
-000109c0: 7473 2074 6872 6f75 6768 6f75 7420 7468  ts throughout th
-000109d0: 6520 636f 6465 2061 6e64 2063 6c65 616e  e code and clean
-000109e0: 7570 0d0a 0d0a 2a20 5665 7273 696f 6e20  up....* Version 
-000109f0: 312e 300d 0a20 2020 202a 204c 5453 7069  1.0..    * LTSpi
-00010a00: 6365 4261 7463 682e 7079 3a5c 0d0a 2020  ceBatch.py:\..  
-00010a10: 2020 2020 496d 706c 656d 656e 7465 6420      Implemented 
-00010a20: 6120 6e65 7720 6170 7072 6f61 6368 2028  a new approach (
-00010a30: 4e4f 5420 4241 434b 5741 5244 5320 434f  NOT BACKWARDS CO
-00010a40: 4d50 4154 4942 4c45 292c 2074 6861 7420  MPATIBLE), that 
-00010a50: 6176 6f69 6473 2074 6865 2075 7361 6765  avoids the usage
-00010a60: 206f 6620 7468 6520 7369 6d5f 7365 7474   of the sim_sett
-00010a70: 696e 6773 2e69 6e63 2066 696c 652e 0d0a  ings.inc file...
-00010a80: 2020 2020 2020 416e 6420 616c 6c6f 7773        And allows
-00010a90: 2074 6f20 6d6f 6469 6679 206e 6f74 206f   to modify not o
-00010aa0: 6e6c 7920 7061 7261 6d65 7465 7273 2c20  nly parameters, 
-00010ab0: 6275 7420 616c 736f 206d 6f64 656c 7320  but also models 
-00010ac0: 616e 6420 6576 656e 2074 6865 2073 696d  and even the sim
-00010ad0: 756c 6174 696f 6e20 636f 6d6d 616e 6473  ulation commands
-00010ae0: 2e0d 0a20 2020 202a 204c 5453 7069 6365  ...    * LTSpice
-00010af0: 5f52 6177 5265 6164 2e70 793a 5c0d 0a20  _RawRead.py:\.. 
-00010b00: 2020 2020 2041 6464 6564 2074 6865 2067       Added the g
-00010b10: 6574 5f74 696d 655f 6178 6973 206d 6574  et_time_axis met
-00010b20: 686f 6420 746f 2074 6865 2052 6177 5265  hod to the RawRe
-00010b30: 6164 2063 6c61 7373 2074 6f20 6176 6f69  ad class to avoi
-00010b40: 6420 7468 6520 7072 6f62 6c65 6d73 2077  d the problems w
-00010b50: 6974 6820 6e65 6761 7469 7665 2076 616c  ith negative val
-00010b60: 7565 7320 6f6e 2074 696d 6520 6178 6973  ues on time axis
-00010b70: 2c0d 0a20 2020 2020 2077 6865 6e20 326e  ,..      when 2n
-00010b80: 6420 6f72 6465 7220 636f 6d70 7265 7373  d order compress
-00010b90: 696f 6e20 6973 2065 6e61 626c 6564 2069  ion is enabled i
-00010ba0: 6e20 4c54 5370 6963 652e 0d0a 2020 2020  n LTSpice...    
-00010bb0: 2a20 4c54 5374 6570 732e 7079 3a5c 0d0a  * LTSteps.py:\..
-00010bc0: 2020 2020 2020 4d6f 6469 6669 6564 2074        Modified t
-00010bd0: 6865 204c 5453 7465 7073 2c20 736f 2069  he LTSteps, so i
-00010be0: 7420 6361 6e20 616c 736f 2072 6561 6420  t can also read 
-00010bf0: 6d65 6173 7572 656d 656e 7473 206f 6e20  measurements on 
-00010c00: 6c6f 6720 6669 6c65 7320 7769 7468 6f75  log files withou
-00010c10: 7420 616e 7920 7374 6570 7320 646f 6e65  t any steps done
-00010c20: 2e0d 0a0d 0a2a 2056 6572 7369 6f6e 2030  .....* Version 0
-00010c30: 2e36 0d0a 2020 2a20 4869 7374 6f67 7261  .6..  * Histogra
-00010c40: 6d2e 7079 206e 6f77 2068 6173 2061 6e20  m.py now has an 
-00010c50: 6f70 7469 6f6e 2074 6f20 6d61 6b65 2074  option to make t
-00010c60: 6865 2068 6973 746f 6772 616d 2064 6972  he histogram dir
-00010c70: 6563 746c 7920 6672 6f6d 2076 616c 7565  ectly from value
-00010c80: 7320 7374 6f72 6564 2069 6e20 7468 6520  s stored in the 
-00010c90: 636c 6970 626f 6172 640d 0a0d 0a2a 2056  clipboard....* V
-00010ca0: 6572 7369 6f6e 2030 2e35 0d0a 2020 2a20  ersion 0.5..  * 
-00010cb0: 5468 6520 4c54 5370 6963 655f 5261 7752  The LTSpice_RawR
-00010cc0: 6561 6465 722e 7079 206e 6f77 2075 7365  eader.py now use
-00010cd0: 7320 7468 6520 6073 7472 7563 742e 756e  s the `struct.un
-00010ce0: 7061 636b 6020 6675 6e63 7469 6f6e 2066  pack` function f
-00010cf0: 6f72 2061 2066 6173 7465 7220 6578 6563  or a faster exec
-00010d00: 7574 696f 6e0d 0a0d 0a2a 2056 6572 7369  ution....* Versi
-00010d10: 6f6e 2030 2e34 0d0a 2020 2a20 4164 6465  on 0.4..  * Adde
-00010d20: 6420 4c54 5370 6963 6542 6174 6368 2e70  d LTSpiceBatch.p
-00010d30: 7920 746f 2074 6865 2063 6f6c 6c65 6374  y to the collect
-00010d40: 696f 6e20 6f66 2074 6f6f 6c73 0d0a 0d0a  ion of tools....
-00010d50: 2a20 5665 7273 696f 6e20 302e 330d 0a20  * Version 0.3.. 
-00010d60: 202a 2041 2076 6572 7369 6f6e 206f 6620   * A version of 
-00010d70: 4c54 5374 6570 7320 7468 6174 2063 616e  LTSteps that can
-00010d80: 2062 6520 696d 706f 7274 6564 2074 6f20   be imported to 
-00010d90: 7573 6520 696e 2061 2068 6967 6865 7220  use in a higher 
-00010da0: 6c65 7665 6c20 7363 7269 7074 0d0a 0d0a  level script....
-00010db0: 2a20 5665 7273 696f 6e20 302e 320d 0a20  * Version 0.2.. 
-00010dc0: 202a 2041 6464 696e 6720 4c54 5374 6570   * Adding LTStep
-00010dd0: 732e 7079 2061 6e64 2048 6973 746f 6772  s.py and Histogr
-00010de0: 616d 2e70 790d 0a0d 0a2a 2056 6572 7369  am.py....* Versi
-00010df0: 6f6e 2030 2e31 200d 0a20 202a 2046 6972  on 0.1 ..  * Fir
-00010e00: 7374 2063 6f6d 6d69 7420 746f 2074 6865  st commit to the
-00010e10: 2062 6974 6275 636b 6574 2072 6570 6f73   bitbucket repos
-00010e20: 6974 6f72 792e 0d0a                      itory...
+0000b1e0: 2e2f 7465 7374 6669 6c65 732f 5452 414e  ./testfiles/TRAN
+0000b1f0: 202d 2053 5445 502e 7261 7722 290d 0a0d   - STEP.raw")...
+0000b200: 0a70 7269 6e74 284c 5452 2e67 6574 5f74  .print(LTR.get_t
+0000b210: 7261 6365 5f6e 616d 6573 2829 290d 0a70  race_names())..p
+0000b220: 7269 6e74 284c 5452 2e67 6574 5f72 6177  rint(LTR.get_raw
+0000b230: 5f70 726f 7065 7274 7928 2929 0d0a 0d0a  _property())....
+0000b240: 4952 3120 3d20 4c54 522e 6765 745f 7472  IR1 = LTR.get_tr
+0000b250: 6163 6528 2249 2852 3129 2229 0d0a 7820  ace("I(R1)")..x 
+0000b260: 3d20 4c54 522e 6765 745f 7472 6163 6528  = LTR.get_trace(
+0000b270: 2774 696d 6527 2920 2023 2047 6574 7320  'time')  # Gets 
+0000b280: 7468 6520 7469 6d65 2061 7869 730d 0a73  the time axis..s
+0000b290: 7465 7073 203d 204c 5452 2e67 6574 5f73  teps = LTR.get_s
+0000b2a0: 7465 7073 2829 0d0a 666f 7220 7374 6570  teps()..for step
+0000b2b0: 2069 6e20 7261 6e67 6528 6c65 6e28 7374   in range(len(st
+0000b2c0: 6570 7329 293a 0d0a 2020 2020 2320 7072  eps)):..    # pr
+0000b2d0: 696e 7428 7374 6570 735b 7374 6570 5d29  int(steps[step])
+0000b2e0: 0d0a 2020 2020 706c 742e 706c 6f74 2878  ..    plt.plot(x
+0000b2f0: 2e67 6574 5f77 6176 6528 7374 6570 292c  .get_wave(step),
+0000b300: 2049 5231 2e67 6574 5f77 6176 6528 7374   IR1.get_wave(st
+0000b310: 6570 292c 206c 6162 656c 3d73 7465 7073  ep), label=steps
+0000b320: 5b73 7465 705d 290d 0a0d 0a70 6c74 2e6c  [step])....plt.l
+0000b330: 6567 656e 6428 2920 2023 206f 7264 6572  egend()  # order
+0000b340: 2061 206c 6567 656e 640d 0a70 6c74 2e73   a legend..plt.s
+0000b350: 686f 7728 290d 0a60 6060 0d0a 2d2d 2069  how()..```..-- i
+0000b360: 6e20 6578 616d 706c 6573 2f72 6177 5f72  n examples/raw_r
+0000b370: 6561 645f 6578 616d 706c 652e 7079 2020  ead_example.py  
+0000b380: 200d 0a0d 0a23 2323 2052 6177 5772 6974   ....### RawWrit
+0000b390: 6520 2323 230d 0a0d 0a54 6865 2066 6f6c  e ###....The fol
+0000b3a0: 6c6f 7769 6e67 2065 7861 6d70 6c65 2077  lowing example w
+0000b3b0: 7269 7465 7320 6120 5241 5720 6669 6c65  rites a RAW file
+0000b3c0: 2077 6974 6820 6120 3320 6d69 6c6c 6973   with a 3 millis
+0000b3d0: 6563 6f6e 6473 2074 7261 6e73 6965 6e74  econds transient
+0000b3e0: 2073 696d 756c 6174 696f 6e20 7369 6e65   simulation sine
+0000b3f0: 2077 6974 6820 6120 3130 6b48 7a20 616e   with a 10kHz an
+0000b400: 6420 6120 636f 7369 6e65 2077 6974 680d  d a cosine with.
+0000b410: 0a39 2e39 3937 6b48 7a0d 0a0d 0a60 6060  .9.997kHz....```
+0000b420: 7079 7468 6f6e 0d0a 696d 706f 7274 206e  python..import n
+0000b430: 756d 7079 2061 7320 6e70 0d0a 6672 6f6d  umpy as np..from
+0000b440: 2050 794c 5453 7069 6365 2069 6d70 6f72   PyLTSpice impor
+0000b450: 7420 5261 7752 6561 642c 2054 7261 6365  t RawRead, Trace
+0000b460: 2c20 5261 7757 7269 7465 0d0a 4c57 203d  , RawWrite..LW =
+0000b470: 2052 6177 5772 6974 6528 6661 7374 6163   RawWrite(fastac
+0000b480: 6365 733d 4661 6c73 6529 0d0a 7478 203d  ces=False)..tx =
+0000b490: 2054 7261 6365 2827 7469 6d65 272c 206e   Trace('time', n
+0000b4a0: 702e 6172 616e 6765 2830 2e30 2c20 3365  p.arange(0.0, 3e
+0000b4b0: 2d33 2c20 3939 3745 2d31 3129 290d 0a76  -3, 997E-11))..v
+0000b4c0: 7920 3d20 5472 6163 6528 274e 3030 3127  y = Trace('N001'
+0000b4d0: 2c20 6e70 2e73 696e 2832 202a 206e 702e  , np.sin(2 * np.
+0000b4e0: 7069 202a 2074 782e 6461 7461 202a 2031  pi * tx.data * 1
+0000b4f0: 3030 3030 2929 0d0a 767a 203d 2054 7261  0000))..vz = Tra
+0000b500: 6365 2827 4e30 3032 272c 206e 702e 636f  ce('N002', np.co
+0000b510: 7328 3220 2a20 6e70 2e70 6920 2a20 7478  s(2 * np.pi * tx
+0000b520: 2e64 6174 6120 2a20 3939 3730 2929 0d0a  .data * 9970))..
+0000b530: 4c57 2e61 6464 5f74 7261 6365 2874 7829  LW.add_trace(tx)
+0000b540: 0d0a 4c57 2e61 6464 5f74 7261 6365 2876  ..LW.add_trace(v
+0000b550: 7929 0d0a 4c57 2e61 6464 5f74 7261 6365  y)..LW.add_trace
+0000b560: 2876 7a29 0d0a 4c57 2e73 6176 6528 222e  (vz)..LW.save(".
+0000b570: 2f74 6573 7466 696c 6573 2f74 6573 7465  /testfiles/teste
+0000b580: 5f73 6e69 7070 6574 312e 7261 7722 290d  _snippet1.raw").
+0000b590: 0a60 6060 2020 200d 0a2d 2d20 696e 2065  .```   ..-- in e
+0000b5a0: 7861 6d70 6c65 732f 7261 775f 7772 6974  xamples/raw_writ
+0000b5b0: 655f 6578 616d 706c 652e 7079 205b 5261  e_example.py [Ra
+0000b5c0: 7757 7269 7465 2045 7861 6d70 6c65 5d0d  wWrite Example].
+0000b5d0: 0a0d 0a23 2323 2053 7069 6365 4564 6974  ...### SpiceEdit
+0000b5e0: 6f72 2c20 4173 6345 6469 746f 7220 616e  or, AscEditor an
+0000b5f0: 6420 5369 6d52 756e 6e65 722e 7079 2023  d SimRunner.py #
+0000b600: 2323 0d0a 0d0a 5468 6973 206d 6f64 756c  ##....This modul
+0000b610: 6520 6973 2075 7365 6420 746f 206c 6175  e is used to lau
+0000b620: 6e63 6820 4c54 5350 6963 6520 7369 6d75  nch LTSPice simu
+0000b630: 6c61 7469 6f6e 732e 2052 6573 756c 7473  lations. Results
+0000b640: 2074 6865 6e20 6361 6e20 6265 2070 726f   then can be pro
+0000b650: 6365 7373 6564 2077 6974 6820 6569 7468  cessed with eith
+0000b660: 6572 2074 6865 2052 6177 5265 6164 206f  er the RawRead o
+0000b670: 7220 7769 7468 2074 6865 0d0a 4c54 5374  r with the..LTSt
+0000b680: 6570 7320 6d6f 6475 6c65 2074 6f20 7265  eps module to re
+0000b690: 6164 2074 6865 206c 6f67 2066 696c 6520  ad the log file 
+0000b6a0: 7768 6963 6820 6361 6e20 636f 6e74 6169  which can contai
+0000b6b0: 6e20 2e4d 4541 5320 7265 7375 6c74 732e  n .MEAS results.
+0000b6c0: 0d0a 0d0a 5468 6520 7363 7269 7074 2077  ....The script w
+0000b6d0: 696c 6c20 6669 7273 746c 7920 696e 766f  ill firstly invo
+0000b6e0: 6b65 2074 6865 204c 5453 7069 6365 2069  ke the LTSpice i
+0000b6f0: 6e20 636f 6d6d 616e 6420 6c69 6e65 2074  n command line t
+0000b700: 6f20 6765 6e65 7261 7465 2061 206e 6574  o generate a net
+0000b710: 6c69 7374 2c20 616e 6420 7468 656e 2074  list, and then t
+0000b720: 6869 7320 6e65 746c 6973 7420 6361 6e20  his netlist can 
+0000b730: 6265 2075 7064 6174 6564 0d0a 6469 7265  be updated..dire
+0000b740: 6374 6c79 2062 7920 7468 6520 7363 7269  ctly by the scri
+0000b750: 7074 2c20 696e 206f 7264 6572 2074 6f20  pt, in order to 
+0000b760: 6368 616e 6765 2063 6f6d 706f 6e65 6e74  change component
+0000b770: 2076 616c 7565 732c 2070 6172 616d 6574   values, paramet
+0000b780: 6572 7320 6f72 2073 696d 756c 6174 696f  ers or simulatio
+0000b790: 6e20 636f 6d6d 616e 6473 2e0d 0a0d 0a48  n commands.....H
+0000b7a0: 6572 6520 666f 6c6c 6f77 7320 616e 2065  ere follows an e
+0000b7b0: 7861 6d70 6c65 206f 6620 6f70 6572 6174  xample of operat
+0000b7c0: 696f 6e2e 0d0a 0d0a 6060 6070 7974 686f  ion.....```pytho
+0000b7d0: 6e0d 0a66 726f 6d20 5079 4c54 5370 6963  n..from PyLTSpic
+0000b7e0: 6520 696d 706f 7274 2053 696d 5275 6e6e  e import SimRunn
+0000b7f0: 6572 0d0a 6672 6f6d 2050 794c 5453 7069  er..from PyLTSpi
+0000b800: 6365 2069 6d70 6f72 7420 5370 6963 6545  ce import SpiceE
+0000b810: 6469 746f 720d 0a0d 0a23 2046 6f72 6365  ditor....# Force
+0000b820: 2061 6e6f 7468 6572 2073 696d 756c 6174   another simulat
+0000b830: 696f 720d 0a73 696d 756c 6174 6f72 203d  ior..simulator =
+0000b840: 2072 2243 3a5c 5072 6f67 7261 6d20 4669   r"C:\Program Fi
+0000b850: 6c65 735c 4c54 435c 4c54 7370 6963 6558  les\LTC\LTspiceX
+0000b860: 5649 495c 5856 4949 7836 342e 6578 6522  VII\XVIIx64.exe"
+0000b870: 0d0a 0d0a 2320 7365 6c65 6374 2073 7069  ....# select spi
+0000b880: 6365 206d 6f64 656c 0d0a 4c54 4320 3d20  ce model..LTC = 
+0000b890: 5369 6d52 756e 6e65 7228 6f75 7470 7574  SimRunner(output
+0000b8a0: 5f66 6f6c 6465 723d 272e 2f74 656d 7027  _folder='./temp'
+0000b8b0: 290d 0a4c 5443 2e63 7265 6174 655f 6e65  )..LTC.create_ne
+0000b8c0: 746c 6973 7428 272e 2f74 6573 7466 696c  tlist('./testfil
+0000b8d0: 6573 2f42 6174 6368 5f54 6573 742e 6173  es/Batch_Test.as
+0000b8e0: 6327 290d 0a6e 6574 6c69 7374 203d 2053  c')..netlist = S
+0000b8f0: 7069 6365 4564 6974 6f72 2827 2e2f 7465  piceEditor('./te
+0000b900: 7374 6669 6c65 732f 4261 7463 685f 5465  stfiles/Batch_Te
+0000b910: 7374 2e6e 6574 2729 0d0a 2320 7365 7420  st.net')..# set 
+0000b920: 6465 6661 756c 7420 6172 6775 6d65 6e74  default argument
+0000b930: 730d 0a6e 6574 6c69 7374 2e73 6574 5f70  s..netlist.set_p
+0000b940: 6172 616d 6574 6572 7328 7265 733d 302c  arameters(res=0,
+0000b950: 2063 6170 3d31 3030 652d 3629 0d0a 6e65   cap=100e-6)..ne
+0000b960: 746c 6973 742e 7365 745f 636f 6d70 6f6e  tlist.set_compon
+0000b970: 656e 745f 7661 6c75 6528 2752 3227 2c20  ent_value('R2', 
+0000b980: 2732 6b27 2920 2023 204d 6f64 6966 7969  '2k')  # Modifyi
+0000b990: 6e67 2074 6865 2076 616c 7565 206f 6620  ng the value of 
+0000b9a0: 6120 7265 7369 7374 6f72 0d0a 6e65 746c  a resistor..netl
+0000b9b0: 6973 742e 7365 745f 636f 6d70 6f6e 656e  ist.set_componen
+0000b9c0: 745f 7661 6c75 6528 2752 3127 2c20 2734  t_value('R1', '4
+0000b9d0: 6b27 290d 0a6e 6574 6c69 7374 2e73 6574  k')..netlist.set
+0000b9e0: 5f65 6c65 6d65 6e74 5f6d 6f64 656c 2827  _element_model('
+0000b9f0: 5633 272c 2022 5349 4e45 2830 2031 2033  V3', "SINE(0 1 3
+0000ba00: 6b20 3020 3020 3029 2229 2020 2320 4d6f  k 0 0 0)")  # Mo
+0000ba10: 6469 6679 696e 6720 7468 650d 0a6e 6574  difying the..net
+0000ba20: 6c69 7374 2e73 6574 5f63 6f6d 706f 6e65  list.set_compone
+0000ba30: 6e74 5f76 616c 7565 2827 5855 313a 4332  nt_value('XU1:C2
+0000ba40: 272c 2032 3065 2d31 3229 2020 2320 6d6f  ', 20e-12)  # mo
+0000ba50: 6469 6679 696e 6720 6120 6465 6669 6e65  difying a define
+0000ba60: 2073 696d 756c 6174 696f 6e0d 0a6e 6574   simulation..net
+0000ba70: 6c69 7374 2e61 6464 5f69 6e73 7472 7563  list.add_instruc
+0000ba80: 7469 6f6e 7328 0d0a 2020 2020 223b 2053  tions(..    "; S
+0000ba90: 696d 756c 6174 696f 6e20 7365 7474 696e  imulation settin
+0000baa0: 6773 222c 0d0a 2020 2020 223b 2e70 6172  gs",..    ";.par
+0000bab0: 616d 2072 756e 203d 2030 220d 0a29 0d0a  am run = 0"..)..
+0000bac0: 6e65 746c 6973 742e 7365 745f 7061 7261  netlist.set_para
+0000bad0: 6d65 7465 7228 2772 756e 272c 2030 290d  meter('run', 0).
+0000bae0: 0a0d 0a66 6f72 206f 7061 6d70 2069 6e20  ...for opamp in 
+0000baf0: 2827 4144 3731 3227 2c20 2741 4438 3230  ('AD712', 'AD820
+0000bb00: 2729 3a0d 0a20 2020 206e 6574 6c69 7374  '):..    netlist
+0000bb10: 2e73 6574 5f65 6c65 6d65 6e74 5f6d 6f64  .set_element_mod
+0000bb20: 656c 2827 5855 3127 2c20 6f70 616d 7029  el('XU1', opamp)
+0000bb30: 0d0a 2020 2020 666f 7220 7375 7070 6c79  ..    for supply
+0000bb40: 5f76 6f6c 7461 6765 2069 6e20 2835 2c20  _voltage in (5, 
+0000bb50: 3130 2c20 3135 293a 0d0a 2020 2020 2020  10, 15):..      
+0000bb60: 2020 6e65 746c 6973 742e 7365 745f 636f    netlist.set_co
+0000bb70: 6d70 6f6e 656e 745f 7661 6c75 6528 2756  mponent_value('V
+0000bb80: 3127 2c20 7375 7070 6c79 5f76 6f6c 7461  1', supply_volta
+0000bb90: 6765 290d 0a20 2020 2020 2020 206e 6574  ge)..        net
+0000bba0: 6c69 7374 2e73 6574 5f63 6f6d 706f 6e65  list.set_compone
+0000bbb0: 6e74 5f76 616c 7565 2827 5632 272c 202d  nt_value('V2', -
+0000bbc0: 7375 7070 6c79 5f76 6f6c 7461 6765 290d  supply_voltage).
+0000bbd0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0000bbe0: 7369 6d75 6c61 7469 6e67 204f 7041 6d70  simulating OpAmp
+0000bbf0: 222c 206f 7061 6d70 2c20 2256 6f6c 7461  ", opamp, "Volta
+0000bc00: 6765 222c 2073 7570 706c 795f 766f 6c74  ge", supply_volt
+0000bc10: 6167 6529 0d0a 2020 2020 2020 2020 4c54  age)..        LT
+0000bc20: 432e 7275 6e28 6e65 746c 6973 7429 0d0a  C.run(netlist)..
+0000bc30: 0d0a 666f 7220 7261 772c 206c 6f67 2069  ..for raw, log i
+0000bc40: 6e20 4c54 433a 0d0a 2020 2020 7072 696e  n LTC:..    prin
+0000bc50: 7428 2252 6177 2066 696c 653a 2025 732c  t("Raw file: %s,
+0000bc60: 204c 6f67 2066 696c 653a 2025 7322 2025   Log file: %s" %
+0000bc70: 2028 7261 772c 206c 6f67 2929 0d0a 2020   (raw, log))..  
+0000bc80: 2020 2320 646f 2073 6f6d 6574 6869 6e67    # do something
+0000bc90: 2077 6974 6820 7468 6520 6461 7461 0d0a   with the data..
+0000bca0: 2020 2020 2320 7261 775f 6461 7461 203d      # raw_data =
+0000bcb0: 2052 6177 5265 6164 2872 6177 290d 0a20   RawRead(raw).. 
+0000bcc0: 2020 2023 206c 6f67 5f64 6174 6120 3d20     # log_data = 
+0000bcd0: 4c54 5374 6570 7328 6c6f 6729 0d0a 2020  LTSteps(log)..  
+0000bce0: 2020 2320 2e2e 2e0d 0a0d 0a6e 6574 6c69    # .......netli
+0000bcf0: 7374 2e72 6573 6574 5f6e 6574 6c69 7374  st.reset_netlist
+0000bd00: 2829 0d0a 6e65 746c 6973 742e 6164 645f  ()..netlist.add_
+0000bd10: 696e 7374 7275 6374 696f 6e73 280d 0a20  instructions(.. 
+0000bd20: 2020 2022 3b20 5369 6d75 6c61 7469 6f6e     "; Simulation
+0000bd30: 2073 6574 7469 6e67 7322 2c0d 0a20 2020   settings",..   
+0000bd40: 2022 2e61 6320 6465 6320 3330 2031 3020   ".ac dec 30 10 
+0000bd50: 314d 6567 222c 0d0a 2020 2020 222e 6d65  1Meg",..    ".me
+0000bd60: 6173 2041 4320 4761 696e 204d 4158 206d  as AC Gain MAX m
+0000bd70: 6167 2856 286f 7574 2929 203b 2066 696e  ag(V(out)) ; fin
+0000bd80: 6420 7468 6520 7065 616b 2072 6573 706f  d the peak respo
+0000bd90: 6e73 6520 616e 6420 6361 6c6c 2069 7420  nse and call it 
+0000bda0: 2222 4761 696e 2222 222c 0d0a 2020 2020  ""Gain""",..    
+0000bdb0: 222e 6d65 6173 2041 4320 4663 7574 2054  ".meas AC Fcut T
+0000bdc0: 5249 4720 6d61 6728 5628 6f75 7429 293d  RIG mag(V(out))=
+0000bdd0: 4761 696e 2f73 7172 7428 3229 2046 414c  Gain/sqrt(2) FAL
+0000bde0: 4c3d 6c61 7374 220d 0a29 0d0a 0d0a 2320  L=last"..)....# 
+0000bdf0: 5369 6d20 5374 6174 6973 7469 6373 0d0a  Sim Statistics..
+0000be00: 7072 696e 7428 2753 7563 6365 7373 6675  print('Successfu
+0000be10: 6c2f 546f 7461 6c20 5369 6d75 6c61 7469  l/Total Simulati
+0000be20: 6f6e 733a 2027 202b 2073 7472 284c 5443  ons: ' + str(LTC
+0000be30: 2e6f 6b53 696d 2920 2b20 272f 2720 2b20  .okSim) + '/' + 
+0000be40: 7374 7228 4c54 432e 7275 6e6e 6f29 290d  str(LTC.runno)).
+0000be50: 0a0d 0a65 6e74 6572 203d 2069 6e70 7574  ...enter = input
+0000be60: 2822 5072 6573 7320 656e 7465 7220 746f  ("Press enter to
+0000be70: 2064 656c 6574 6520 6372 6561 7465 6420   delete created 
+0000be80: 6669 6c65 7322 290d 0a69 6620 656e 7465  files")..if ente
+0000be90: 7220 3d3d 2027 273a 0d0a 2020 2020 4c54  r == '':..    LT
+0000bea0: 432e 6669 6c65 5f63 6c65 616e 7570 2829  C.file_cleanup()
+0000beb0: 0d0a 6060 600d 0a2d 2d20 696e 2065 7861  ..```..-- in exa
+0000bec0: 6d70 6c65 732f 7369 6d5f 7275 6e6e 6572  mples/sim_runner
+0000bed0: 5f65 7861 6d70 6c65 2e70 790d 0a0d 0a54  _example.py....T
+0000bee0: 6865 2065 7861 6d70 6c65 2061 626f 7665  he example above
+0000bef0: 2069 7320 7573 696e 6720 7468 6520 5370   is using the Sp
+0000bf00: 6963 6545 6469 746f 7220 746f 2063 7265  iceEditor to cre
+0000bf10: 6174 6520 616e 6420 6d6f 6469 6679 2061  ate and modify a
+0000bf20: 2073 7069 6365 206e 6574 6c69 7374 2c20   spice netlist, 
+0000bf30: 6275 7420 6974 2069 7320 616c 736f 2070  but it is also p
+0000bf40: 6f73 7369 626c 6520 746f 2075 7365 2074  ossible to use t
+0000bf50: 6865 0d0a 4173 6345 6469 746f 7220 746f  he..AscEditor to
+0000bf60: 2064 6972 6563 746c 7920 6d6f 6469 6679   directly modify
+0000bf70: 2074 6865 202e 6173 6320 6669 6c65 2e20   the .asc file. 
+0000bf80: 5468 6520 6564 6974 6564 202e 6173 6320  The edited .asc 
+0000bf90: 6669 6c65 2063 616e 2074 6865 6e20 6265  file can then be
+0000bfa0: 206f 7065 6e65 6420 6279 2074 6865 204c   opened by the L
+0000bfb0: 5453 7069 6365 2047 5549 2061 6e64 2074  TSpice GUI and t
+0000bfc0: 6865 0d0a 7369 6d75 6c61 7469 6f6e 2063  he..simulation c
+0000bfd0: 616e 2062 6520 7275 6e20 6672 6f6d 2074  an be run from t
+0000bfe0: 6865 7265 2e0d 0a0d 0a23 2323 2053 696d  here.....### Sim
+0000bff0: 756c 6174 696f 6e20 416e 616c 7973 6973  ulation Analysis
+0000c000: 2054 6f6f 6c6b 6974 2023 2323 0d0a 0d0a   Toolkit ###....
+0000c010: 5468 6520 4173 6345 6469 746f 7220 6361  The AscEditor ca
+0000c020: 6e20 6265 2075 7365 6420 7769 7468 2074  n be used with t
+0000c030: 6865 2053 696d 756c 6174 696f 6e20 416e  he Simulation An
+0000c040: 616c 7973 6973 2054 6f6f 6c6b 6974 2074  alysis Toolkit t
+0000c050: 6f20 7065 7266 6f72 6d20 4d6f 6e74 6520  o perform Monte 
+0000c060: 4361 726c 6f20 6f72 2057 6f73 7420 4361  Carlo or Wost Ca
+0000c070: 7365 2073 696d 756c 6174 696f 6e73 2e0d  se simulations..
+0000c080: 0a54 6865 7365 2073 696d 756c 6174 696f  .These simulatio
+0000c090: 6e73 2063 616e 2065 6974 6865 7220 6265  ns can either be
+0000c0a0: 2064 6f6e 6520 6f6e 2074 6865 204c 5453   done on the LTS
+0000c0b0: 7069 6365 2047 5549 206f 7220 7573 696e  pice GUI or usin
+0000c0c0: 6720 7468 6520 5275 6e6e 6572 2043 6c61  g the Runner Cla
+0000c0d0: 7373 2064 6573 6372 6962 6564 2061 626f  ss described abo
+0000c0e0: 7665 2e0d 0a0d 0a4c 6574 2773 2063 6f6e  ve.....Let's con
+0000c0f0: 7369 6465 7220 7468 6520 666f 6c6c 6f77  sider the follow
+0000c100: 696e 6720 6369 7263 7569 743a 0d0a 0d0a  ing circuit:....
+0000c110: 215b 5361 6c6c 656e 2d4b 6579 2041 6d70  ![Sallen-Key Amp
+0000c120: 6c69 6669 6572 5d28 2e2f 646f 632f 6d6f  lifier](./doc/mo
+0000c130: 6475 6c65 732f 7361 6c6c 656e 6b65 792e  dules/sallenkey.
+0000c140: 706e 6720 2253 616c 6c65 6e2d 4b65 7920  png "Sallen-Key 
+0000c150: 416d 706c 6966 6965 7222 290d 0a0d 0a57  Amplifier")....W
+0000c160: 6865 6e20 7065 7266 6f72 6d69 6e67 2061  hen performing a
+0000c170: 204d 6f6e 7465 2043 6172 6c6f 2073 696d   Monte Carlo sim
+0000c180: 756c 6174 696f 6e20 6f6e 2074 6869 7320  ulation on this 
+0000c190: 6369 7263 7569 742c 2077 6520 6e65 6564  circuit, we need
+0000c1a0: 2074 6f20 6d61 6e75 616c 6c79 206d 6f64   to manually mod
+0000c1b0: 6966 7920 7468 6520 7661 6c75 6520 6f66  ify the value of
+0000c1c0: 2065 6163 6820 636f 6d70 6f6e 656e 742c   each component,
+0000c1d0: 200d 0a61 6e64 2074 6865 6e20 6164 6420   ..and then add 
+0000c1e0: 7468 6520 2e73 7465 7020 636f 6d6d 616e  the .step comman
+0000c1f0: 6420 666f 7220 6d61 6b69 6e67 2073 6576  d for making sev
+0000c200: 6572 616c 2072 756e 7320 6f6e 2074 6865  eral runs on the
+0000c210: 2073 616d 6520 6369 7263 7569 742e 200d   same circuit. .
+0000c220: 0a54 6f20 7369 6d70 6c69 6679 2074 6869  .To simplify thi
+0000c230: 7320 7072 6f63 6573 732c 2074 6865 2041  s process, the A
+0000c240: 7363 4564 6974 6f72 2063 6c61 7373 2063  scEditor class c
+0000c250: 616e 2062 6520 7573 6564 2061 7320 6578  an be used as ex
+0000c260: 656d 706c 6966 6965 6420 6265 6c6f 773a  emplified below:
+0000c270: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
+0000c280: 726f 6d20 5079 4c54 5370 6963 6520 696d  rom PyLTSpice im
+0000c290: 706f 7274 2041 7363 4564 6974 6f72 2c20  port AscEditor, 
+0000c2a0: 5369 6d52 756e 6e65 7220 2023 2049 6d70  SimRunner  # Imp
+0000c2b0: 6f72 7473 2074 6865 2063 6c61 7373 2074  orts the class t
+0000c2c0: 6861 7420 6d61 6e69 7075 6c61 7465 7320  hat manipulates 
+0000c2d0: 7468 6520 6173 6320 6669 6c65 0d0a 6672  the asc file..fr
+0000c2e0: 6f6d 2050 794c 5453 7069 6365 2e73 696d  om PyLTSpice.sim
+0000c2f0: 2e74 6f6f 6b69 742e 6d6f 6e74 6563 6172  .tookit.montecar
+0000c300: 6c6f 2069 6d70 6f72 7420 4d6f 6e74 6563  lo import Montec
+0000c310: 6172 6c6f 2020 2320 496d 706f 7274 7320  arlo  # Imports 
+0000c320: 7468 6520 4d6f 6e74 6563 6172 6c6f 2074  the Montecarlo t
+0000c330: 6f6f 6c6b 6974 2063 6c61 7373 0d0a 0d0a  oolkit class....
+0000c340: 7361 6c6c 656e 6b65 7920 3d20 4173 6345  sallenkey = AscE
+0000c350: 6469 746f 7228 222e 2f74 6573 7466 696c  ditor("./testfil
+0000c360: 6573 2f73 616c 6c65 6e6b 6579 2e61 7363  es/sallenkey.asc
+0000c370: 2229 2020 2320 5265 6164 7320 7468 6520  ")  # Reads the 
+0000c380: 6173 6320 6669 6c65 2069 6e74 6f20 6d65  asc file into me
+0000c390: 6d6f 7279 0d0a 7275 6e6e 6572 203d 2053  mory..runner = S
+0000c3a0: 696d 5275 6e6e 6572 286f 7574 7075 745f  imRunner(output_
+0000c3b0: 666f 6c64 6572 3d27 2e2f 7465 6d70 5f6d  folder='./temp_m
+0000c3c0: 6327 2920 2023 2049 6e73 7461 6e74 6961  c')  # Instantia
+0000c3d0: 7465 7320 7468 6520 7275 6e6e 6572 2063  tes the runner c
+0000c3e0: 6c61 7373 2c20 7769 7468 2074 6865 206f  lass, with the o
+0000c3f0: 7574 7075 7420 666f 6c64 6572 2061 6c72  utput folder alr
+0000c400: 6561 6479 2073 6574 0d0a 6d63 203d 204d  eady set..mc = M
+0000c410: 6f6e 7465 6361 726c 6f28 7361 6c6c 656e  ontecarlo(sallen
+0000c420: 6b65 792c 2072 756e 6e65 7229 2020 2320  key, runner)  # 
+0000c430: 496e 7374 616e 7469 6174 6573 2074 6865  Instantiates the
+0000c440: 204d 6f6e 7465 6361 726c 6f20 636c 6173   Montecarlo clas
+0000c450: 732c 2077 6974 6820 7468 6520 6173 6320  s, with the asc 
+0000c460: 6669 6c65 2061 6c72 6561 6479 2069 6e20  file already in 
+0000c470: 6d65 6d6f 7279 0d0a 0d0a 2320 5468 6520  memory....# The 
+0000c480: 666f 6c6c 6f77 696e 6720 6c69 6e65 7320  following lines 
+0000c490: 7365 7420 7468 6520 6465 6661 756c 7420  set the default 
+0000c4a0: 746f 6c65 7261 6e63 6573 2066 6f72 2074  tolerances for t
+0000c4b0: 6865 2063 6f6d 706f 6e65 6e74 730d 0a6d  he components..m
+0000c4c0: 632e 7365 745f 746f 6c65 7261 6e63 6528  c.set_tolerance(
+0000c4d0: 2752 272c 2030 2e30 3129 2020 2320 3125  'R', 0.01)  # 1%
+0000c4e0: 2074 6f6c 6572 616e 6365 2c20 6465 6661   tolerance, defa
+0000c4f0: 756c 7420 6469 7374 7269 6275 7469 6f6e  ult distribution
+0000c500: 2069 7320 756e 6966 6f72 6d0d 0a6d 632e   is uniform..mc.
+0000c510: 7365 745f 746f 6c65 7261 6e63 6528 2743  set_tolerance('C
+0000c520: 272c 2030 2e31 2c20 6469 7374 7269 6275  ', 0.1, distribu
+0000c530: 7469 6f6e 3d27 756e 6966 6f72 6d27 2920  tion='uniform') 
+0000c540: 2023 2031 3025 2074 6f6c 6572 616e 6365   # 10% tolerance
+0000c550: 2c20 6578 706c 6963 6974 2075 6e69 666f  , explicit unifo
+0000c560: 726d 2064 6973 7472 6962 7574 696f 6e0d  rm distribution.
+0000c570: 0a6d 632e 7365 745f 746f 6c65 7261 6e63  .mc.set_toleranc
+0000c580: 6528 2756 272c 2030 2e31 2c20 6469 7374  e('V', 0.1, dist
+0000c590: 7269 6275 7469 6f6e 3d27 6e6f 726d 616c  ribution='normal
+0000c5a0: 2729 2020 2320 3130 2520 746f 6c65 7261  ')  # 10% tolera
+0000c5b0: 6e63 652c 2062 7574 2075 7369 6e67 2061  nce, but using a
+0000c5c0: 206e 6f72 6d61 6c20 6469 7374 7269 6275   normal distribu
+0000c5d0: 7469 6f6e 0d0a 0d0a 2320 536f 6d65 2063  tion....# Some c
+0000c5e0: 6f6d 706f 6e65 6e74 7320 6361 6e20 6861  omponents can ha
+0000c5f0: 7665 2061 2064 6966 6665 7265 6e74 2074  ve a different t
+0000c600: 6f6c 6572 616e 6365 0d0a 6d63 2e73 6574  olerance..mc.set
+0000c610: 5f74 6f6c 6572 616e 6365 2827 5231 272c  _tolerance('R1',
+0000c620: 2030 2e30 3529 2020 2320 3525 2074 6f6c   0.05)  # 5% tol
+0000c630: 6572 616e 6365 2066 6f72 2052 3120 6f6e  erance for R1 on
+0000c640: 6c79 2e20 5468 6973 206f 6e6c 7920 6f76  ly. This only ov
+0000c650: 6572 7269 6465 7320 7468 6520 6465 6661  errides the defa
+0000c660: 756c 7420 746f 6c65 7261 6e63 6520 666f  ult tolerance fo
+0000c670: 7220 5231 0d0a 0d0a 2320 546f 6c65 7261  r R1....# Tolera
+0000c680: 6e63 6573 2063 616e 2062 6520 7365 7420  nces can be set 
+0000c690: 666f 7220 7061 7261 6d65 7465 7273 2061  for parameters a
+0000c6a0: 7320 7765 6c6c 0d0a 6d63 2e73 6574 5f70  s well..mc.set_p
+0000c6b0: 6172 616d 6574 6572 5f64 6576 6961 7469  arameter_deviati
+0000c6c0: 6f6e 2827 566f 7327 2c20 3365 2d34 2c20  on('Vos', 3e-4, 
+0000c6d0: 3565 2d33 2c20 2775 6e69 666f 726d 2729  5e-3, 'uniform')
+0000c6e0: 2020 2320 5468 6520 6b65 7977 6f72 6420    # The keyword 
+0000c6f0: 2764 6973 7472 6962 7574 696f 6e27 2069  'distribution' i
+0000c700: 7320 6f70 7469 6f6e 616c 0d0a 6d63 2e70  s optional..mc.p
+0000c710: 7265 7061 7265 5f74 6573 7462 656e 6368  repare_testbench
+0000c720: 286e 756d 5f72 756e 733d 3130 3030 2920  (num_runs=1000) 
+0000c730: 2023 2050 7265 7061 7265 7320 7468 6520   # Prepares the 
+0000c740: 7465 7374 6265 6e63 6820 666f 7220 3130  testbench for 10
+0000c750: 3030 2073 696d 756c 6174 696f 6e73 0d0a  00 simulations..
+0000c760: 0d0a 2320 4669 6e61 6c6c 7920 7468 6520  ..# Finally the 
+0000c770: 6e65 746c 6973 7420 6973 2073 6176 6564  netlist is saved
+0000c780: 2074 6f20 6120 6669 6c65 0d0a 6d63 2e73   to a file..mc.s
+0000c790: 6176 655f 6e65 746c 6973 7428 272e 2f74  ave_netlist('./t
+0000c7a0: 6573 7466 696c 6573 2f73 616c 6c65 6e6b  estfiles/sallenk
+0000c7b0: 6579 5f6d 632e 6e65 7427 290d 0a0d 0a6d  ey_mc.net')....m
+0000c7c0: 632e 7275 6e5f 7465 7374 6265 6e63 6828  c.run_testbench(
+0000c7d0: 7275 6e73 5f70 6572 5f73 696d 3d31 3030  runs_per_sim=100
+0000c7e0: 2920 2023 2052 756e 7320 7468 6520 7369  )  # Runs the si
+0000c7f0: 6d75 6c61 7469 6f6e 2077 6974 6820 7370  mulation with sp
+0000c800: 6c69 7473 206f 6620 3130 3020 7275 6e73  lits of 100 runs
+0000c810: 2065 6163 680d 0a6c 6f67 7320 3d20 6d63   each..logs = mc
+0000c820: 2e72 6561 645f 6c6f 6766 696c 6573 2829  .read_logfiles()
+0000c830: 2020 2023 2052 6561 6473 2074 6865 206c     # Reads the l
+0000c840: 6f67 2066 696c 6573 2061 6e64 2073 746f  og files and sto
+0000c850: 7265 7320 7468 6520 7265 7375 6c74 7320  res the results 
+0000c860: 696e 2074 6865 2072 6573 756c 7473 2061  in the results a
+0000c870: 7474 7269 6275 7465 0d0a 6c6f 6773 2e6f  ttribute..logs.o
+0000c880: 6274 6169 6e5f 616d 706c 6974 7564 655f  btain_amplitude_
+0000c890: 616e 645f 7068 6173 655f 6672 6f6d 5f63  and_phase_from_c
+0000c8a0: 6f6d 706c 6578 5f76 616c 7565 7328 2920  omplex_values() 
+0000c8b0: 2023 2053 706c 6974 7320 7468 6520 636f   # Splits the co
+0000c8c0: 6d70 6c65 7820 7661 6c75 6573 2069 6e74  mplex values int
+0000c8d0: 6f20 7265 616c 2061 6e64 2069 6d61 6769  o real and imagi
+0000c8e0: 6e61 7279 2070 6172 7473 0d0a 6c6f 6773  nary parts..logs
+0000c8f0: 2e65 7870 6f72 745f 6461 7461 2827 2e2f  .export_data('./
+0000c900: 7465 6d70 5f6d 632f 6461 7461 5f74 6573  temp_mc/data_tes
+0000c910: 7462 656e 6368 2e63 7376 2729 2020 2320  tbench.csv')  # 
+0000c920: 4578 706f 7274 7320 7468 6520 6461 7461  Exports the data
+0000c930: 2074 6f20 6120 6373 7620 6669 6c65 0d0a   to a csv file..
+0000c940: 6c6f 6773 2e70 6c6f 745f 6869 7374 6f67  logs.plot_histog
+0000c950: 7261 6d28 2766 6375 7427 2920 2023 2050  ram('fcut')  # P
+0000c960: 6c6f 7473 2074 6865 2068 6973 746f 6772  lots the histogr
+0000c970: 616d 7320 666f 7220 7468 6520 7265 7375  ams for the resu
+0000c980: 6c74 730d 0a6d 632e 636c 6561 6e75 705f  lts..mc.cleanup_
+0000c990: 6669 6c65 7328 2920 2023 2044 656c 6574  files()  # Delet
+0000c9a0: 6573 2074 6865 2074 656d 706f 7261 7279  es the temporary
+0000c9b0: 2066 696c 6573 0d0a 0d0a 7072 696e 7428   files....print(
+0000c9c0: 223d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  "===============
+0000c9d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c9e0: 3d3d 3d3d 3d3d 2229 0d0a 2320 4e6f 7720  ======")..# Now 
+0000c9f0: 7573 696e 6720 7468 6520 7365 636f 6e64  using the second
+0000ca00: 206d 6574 686f 642c 2077 6865 7265 2074   method, where t
+0000ca10: 6865 2073 696d 756c 6174 696f 6e73 2061  he simulations a
+0000ca20: 7265 2072 616e 206f 6e65 2062 7920 6f6e  re ran one by on
+0000ca30: 650d 0a6d 632e 636c 6561 725f 7369 6d75  e..mc.clear_simu
+0000ca40: 6c61 7469 6f6e 5f64 6174 6128 2920 2023  lation_data()  #
+0000ca50: 2043 6c65 6172 7320 7468 6520 7369 6d75   Clears the simu
+0000ca60: 6c61 7469 6f6e 2064 6174 610d 0a6d 632e  lation data..mc.
+0000ca70: 7265 7365 745f 6e65 746c 6973 7428 2920  reset_netlist() 
+0000ca80: 2023 2052 6573 6574 7320 7468 6520 6e65   # Resets the ne
+0000ca90: 746c 6973 7420 746f 2074 6865 206f 7269  tlist to the ori
+0000caa0: 6769 6e61 6c0d 0a6d 632e 7275 6e5f 616e  ginal..mc.run_an
+0000cab0: 616c 7973 6973 286e 756d 5f72 756e 733d  alysis(num_runs=
+0000cac0: 3130 3030 2920 2023 2052 756e 7320 7468  1000)  # Runs th
+0000cad0: 6520 3130 3030 2073 696d 756c 6174 696f  e 1000 simulatio
+0000cae0: 6e73 0d0a 6c6f 6773 203d 206d 632e 7265  ns..logs = mc.re
+0000caf0: 6164 5f6c 6f67 6669 6c65 7328 2920 2020  ad_logfiles()   
+0000cb00: 2320 5265 6164 7320 7468 6520 6c6f 6720  # Reads the log 
+0000cb10: 6669 6c65 7320 616e 6420 7374 6f72 6573  files and stores
+0000cb20: 2074 6865 2072 6573 756c 7473 2069 6e20   the results in 
+0000cb30: 7468 6520 7265 7375 6c74 7320 6174 7472  the results attr
+0000cb40: 6962 7574 650d 0a6c 6f67 732e 6578 706f  ibute..logs.expo
+0000cb50: 7274 5f64 6174 6128 272e 2f74 656d 705f  rt_data('./temp_
+0000cb60: 6d63 2f64 6174 615f 7369 6d73 2e63 7376  mc/data_sims.csv
+0000cb70: 2729 2020 2320 4578 706f 7274 7320 7468  ')  # Exports th
+0000cb80: 6520 6461 7461 2074 6f20 6120 6373 7620  e data to a csv 
+0000cb90: 6669 6c65 0d0a 6c6f 6773 2e70 6c6f 745f  file..logs.plot_
+0000cba0: 6869 7374 6f67 7261 6d28 2766 6375 7427  histogram('fcut'
+0000cbb0: 2920 2023 2050 6c6f 7473 2074 6865 2068  )  # Plots the h
+0000cbc0: 6973 746f 6772 616d 7320 666f 7220 7468  istograms for th
+0000cbd0: 6520 7265 7375 6c74 730d 0a6d 632e 636c  e results..mc.cl
+0000cbe0: 6561 6e75 705f 6669 6c65 7328 2920 2023  eanup_files()  #
+0000cbf0: 2044 656c 6574 6573 2074 6865 2074 656d   Deletes the tem
+0000cc00: 706f 7261 7279 2066 696c 6573 0d0a 0d0a  porary files....
+0000cc10: 6060 600d 0a2d 2d20 696e 2065 7861 6d70  ```..-- in examp
+0000cc20: 6c65 732f 7275 6e5f 6d6f 6e74 6563 6172  les/run_montecar
+0000cc30: 6c6f 2e70 790d 0a0d 0a57 6865 6e20 6f70  lo.py....When op
+0000cc40: 656e 696e 6720 7468 6520 6372 6561 7465  ening the create
+0000cc50: 6420 7361 6c6c 656e 6b65 795f 6d63 2e6e  d sallenkey_mc.n
+0000cc60: 6574 2066 696c 652c 2077 6520 6361 6e20  et file, we can 
+0000cc70: 7365 6520 7468 6174 2074 6865 2066 6f6c  see that the fol
+0000cc80: 6c6f 7769 6e67 2063 6972 6375 6974 2e0d  lowing circuit..
+0000cc90: 0a0d 0a21 5b53 616c 6c65 6e2d 4b65 7920  ...![Sallen-Key 
+0000cca0: 416d 706c 6966 6965 7220 7769 7468 204d  Amplifier with M
+0000ccb0: 6f6e 7465 6361 726c 6f5d 282e 2f64 6f63  ontecarlo](./doc
+0000ccc0: 2f6d 6f64 756c 6573 2f73 616c 6c65 6e6b  /modules/sallenk
+0000ccd0: 6579 5f6d 632e 706e 6720 2253 616c 6c65  ey_mc.png "Salle
+0000cce0: 6e2d 4b65 7920 416d 706c 6966 6965 7220  n-Key Amplifier 
+0000ccf0: 7769 7468 204d 6f6e 7465 6361 726c 6f22  with Montecarlo"
+0000cd00: 290d 0a0d 0a54 6865 2066 6f6c 6c6f 7769  )....The followi
+0000cd10: 6e67 2075 7064 6174 6573 2077 6572 6520  ng updates were 
+0000cd20: 6d61 6465 2074 6f20 7468 6520 6369 7263  made to the circ
+0000cd30: 7569 743a 0d0a 2d20 5468 6520 7661 6c75  uit:..- The valu
+0000cd40: 6520 6f66 2065 6163 6820 636f 6d70 6f6e  e of each compon
+0000cd50: 656e 7420 7761 7320 7265 706c 6163 6564  ent was replaced
+0000cd60: 2062 7920 6120 6675 6e63 7469 6f6e 2074   by a function t
+0000cd70: 6861 7420 6765 6e65 7261 7465 7320 6120  hat generates a 
+0000cd80: 7261 6e64 6f6d 2076 616c 7565 2077 6974  random value wit
+0000cd90: 6869 6e20 7468 6520 7370 6563 6966 6965  hin the specifie
+0000cda0: 6420 746f 6c65 7261 6e63 652e 0d0a 2d20  d tolerance...- 
+0000cdb0: 5468 6520 2e73 7465 7020 7061 7261 6d20  The .step param 
+0000cdc0: 7275 6e20 636f 6d6d 616e 6420 7761 7320  run command was 
+0000cdd0: 6164 6465 6420 746f 2074 6865 206e 6574  added to the net
+0000cde0: 6c69 7374 2e20 5374 6172 7473 2061 7420  list. Starts at 
+0000cdf0: 2d31 2077 6869 6368 2069 7427 7320 7468  -1 which it's th
+0000ce00: 6520 6e6f 6d69 6e61 6c20 7661 6c75 6520  e nominal value 
+0000ce10: 7369 6d75 6c61 7469 6f6e 2c20 616e 6420  simulation, and 
+0000ce20: 0d0a 6669 6e69 7368 6573 2074 6861 7420  ..finishes that 
+0000ce30: 7468 6520 6e75 6d62 6572 206f 6620 7369  the number of si
+0000ce40: 6d75 6c61 7469 6f6e 7320 7370 6563 6966  mulations specif
+0000ce50: 6965 6420 696e 2074 6865 2070 7265 7061  ied in the prepa
+0000ce60: 7265 5f74 6573 7462 656e 6368 2829 206d  re_testbench() m
+0000ce70: 6574 686f 642e 0d0a 2d20 4120 6465 6661  ethod...- A defa
+0000ce80: 756c 7420 7661 6c75 6520 666f 7220 7468  ult value for th
+0000ce90: 6520 7275 6e20 7061 7261 6d65 7465 7220  e run parameter 
+0000cea0: 7761 7320 6164 6465 642e 2054 6869 7320  was added. This 
+0000ceb0: 6973 2075 7365 6675 6c20 6966 2074 6865  is useful if the
+0000cec0: 202e 7374 6570 2070 6172 616d 2072 756e   .step param run
+0000ced0: 2069 7320 636f 6d6d 656e 7465 6420 6f75   is commented ou
+0000cee0: 742e 0d0a 2d20 5468 6520 5231 2074 6f6c  t...- The R1 tol
+0000cef0: 6572 616e 6365 2069 7320 6469 6666 6572  erance is differ
+0000cf00: 656e 7420 6672 6f6d 2074 6865 206f 7468  ent from the oth
+0000cf10: 6572 2072 6573 6973 746f 7273 2e20 5468  er resistors. Th
+0000cf20: 6973 2069 7320 6265 6361 7573 6520 7468  is is because th
+0000cf30: 6520 746f 6c65 7261 6e63 6520 7761 7320  e tolerance was 
+0000cf40: 6578 706c 6963 6974 6c79 2073 6574 2066  explicitly set f
+0000cf50: 6f72 2052 312e 0d0a 2d20 5468 6520 566f  or R1...- The Vo
+0000cf60: 7320 7061 7261 6d65 7465 7220 7761 7320  s parameter was 
+0000cf70: 6164 6465 6420 746f 2074 6865 202e 7061  added to the .pa
+0000cf80: 7261 6d20 6c69 7374 2e20 5468 6973 2069  ram list. This i
+0000cf90: 7320 6265 6361 7573 6520 7468 6520 7061  s because the pa
+0000cfa0: 7261 6d65 7465 7220 7761 7320 6578 706c  rameter was expl
+0000cfb0: 6963 6974 6c79 2073 6574 2075 7369 6e67  icitly set using
+0000cfc0: 2074 6865 0d0a 7365 745f 7061 7261 6d65   the..set_parame
+0000cfd0: 7465 725f 6465 7669 6174 696f 6e20 6d65  ter_deviation me
+0000cfe0: 7468 6f64 2e0d 0a2d 2046 756e 6374 696f  thod...- Functio
+0000cff0: 6e73 2075 746f 6c2c 206e 746f 6c20 616e  ns utol, ntol an
+0000d000: 6420 7572 6e67 2077 6572 6520 6164 6465  d urng were adde
+0000d010: 6420 746f 2074 6865 202e 6675 6e63 206c  d to the .func l
+0000d020: 6973 742e 2054 6865 7365 2066 756e 6374  ist. These funct
+0000d030: 696f 6e73 2061 7265 2075 7365 6420 746f  ions are used to
+0000d040: 2067 656e 6572 6174 6520 7261 6e64 6f6d   generate random
+0000d050: 2076 616c 7565 732e 0d0a 556e 6966 6f72   values...Unifor
+0000d060: 6d20 6469 7374 7269 6275 7469 6f6e 7320  m distributions 
+0000d070: 7573 6520 7468 6520 4c54 5370 6963 6520  use the LTSpice 
+0000d080: 6275 696c 742d 696e 206d 6328 782c 2074  built-in mc(x, t
+0000d090: 6f6c 2920 616e 6420 666c 6174 2878 2920  ol) and flat(x) 
+0000d0a0: 6675 6e63 7469 6f6e 732c 2077 6869 6c65  functions, while
+0000d0b0: 206e 6f72 6d61 6c20 6469 7374 7269 6275   normal distribu
+0000d0c0: 7469 6f6e 7320 7573 6520 7468 6520 0d0a  tions use the ..
+0000d0d0: 6761 7573 7328 7829 2066 756e 6374 696f  gauss(x) functio
+0000d0e0: 6e2e 0d0a 0d0a 5369 6d69 6c61 726c 792c  n.....Similarly,
+0000d0f0: 2074 6865 2077 6f72 7374 2063 6173 6520   the worst case 
+0000d100: 616e 616c 7973 6973 2063 616e 2061 6c73  analysis can als
+0000d110: 6f20 6265 2073 6574 7570 2062 7920 7573  o be setup by us
+0000d120: 696e 6720 7468 6520 636c 6173 7320 576f  ing the class Wo
+0000d130: 7273 7443 6173 6541 6e61 6c79 7369 732c  rstCaseAnalysis,
+0000d140: 2061 7320 6578 656d 706c 6966 6965 6420   as exemplified 
+0000d150: 6265 6c6f 773a 0d0a 0d0a 6060 6070 7974  below:....```pyt
+0000d160: 686f 6e0d 0a66 726f 6d20 5079 4c54 5370  hon..from PyLTSp
+0000d170: 6963 6520 696d 706f 7274 2041 7363 4564  ice import AscEd
+0000d180: 6974 6f72 2c20 5369 6d52 756e 6e65 7220  itor, SimRunner 
+0000d190: 2023 2049 6d70 6f72 7473 2074 6865 2063   # Imports the c
+0000d1a0: 6c61 7373 2074 6861 7420 6d61 6e69 7075  lass that manipu
+0000d1b0: 6c61 7465 7320 7468 6520 6173 6320 6669  lates the asc fi
+0000d1c0: 6c65 0d0a 6672 6f6d 2050 794c 5453 7069  le..from PyLTSpi
+0000d1d0: 6365 2e73 696d 2e74 6f6f 6b69 742e 776f  ce.sim.tookit.wo
+0000d1e0: 7273 745f 6361 7365 2069 6d70 6f72 7420  rst_case import 
+0000d1f0: 576f 7273 7443 6173 6541 6e61 6c79 7369  WorstCaseAnalysi
+0000d200: 730d 0a0d 0a73 616c 6c65 6e6b 6579 203d  s....sallenkey =
+0000d210: 2041 7363 4564 6974 6f72 2822 2e2f 7465   AscEditor("./te
+0000d220: 7374 6669 6c65 732f 7361 6c6c 656e 6b65  stfiles/sallenke
+0000d230: 792e 6173 6322 2920 2023 2052 6561 6473  y.asc")  # Reads
+0000d240: 2074 6865 2061 7363 2066 696c 6520 696e   the asc file in
+0000d250: 746f 206d 656d 6f72 790d 0a72 756e 6e65  to memory..runne
+0000d260: 7220 3d20 5369 6d52 756e 6e65 7228 6f75  r = SimRunner(ou
+0000d270: 7470 7574 5f66 6f6c 6465 723d 272e 2f74  tput_folder='./t
+0000d280: 656d 705f 7763 6127 2920 2023 2049 6e73  emp_wca')  # Ins
+0000d290: 7461 6e74 6961 7465 7320 7468 6520 7275  tantiates the ru
+0000d2a0: 6e6e 6572 2063 6c61 7373 2c20 7769 7468  nner class, with
+0000d2b0: 2074 6865 206f 7574 7075 7420 666f 6c64   the output fold
+0000d2c0: 6572 2061 6c72 6561 6479 2073 6574 0d0a  er already set..
+0000d2d0: 7763 6120 3d20 576f 7273 7443 6173 6541  wca = WorstCaseA
+0000d2e0: 6e61 6c79 7369 7328 7361 6c6c 656e 6b65  nalysis(sallenke
+0000d2f0: 792c 2072 756e 6e65 7229 2020 2320 496e  y, runner)  # In
+0000d300: 7374 616e 7469 6174 6573 2074 6865 2057  stantiates the W
+0000d310: 6f72 7374 2043 6173 6520 416e 616c 7973  orst Case Analys
+0000d320: 6973 2063 6c61 7373 0d0a 0d0a 2320 5468  is class....# Th
+0000d330: 6520 666f 6c6c 6f77 696e 6720 6c69 6e65  e following line
+0000d340: 7320 7365 7420 7468 6520 6465 6661 756c  s set the defaul
+0000d350: 7420 746f 6c65 7261 6e63 6573 2066 6f72  t tolerances for
+0000d360: 2074 6865 2063 6f6d 706f 6e65 6e74 730d   the components.
+0000d370: 0a77 6361 2e73 6574 5f74 6f6c 6572 616e  .wca.set_toleran
+0000d380: 6365 2827 5227 2c20 302e 3031 2920 2023  ce('R', 0.01)  #
+0000d390: 2031 2520 746f 6c65 7261 6e63 650d 0a77   1% tolerance..w
+0000d3a0: 6361 2e73 6574 5f74 6f6c 6572 616e 6365  ca.set_tolerance
+0000d3b0: 2827 4327 2c20 302e 3129 2020 2320 3130  ('C', 0.1)  # 10
+0000d3c0: 2520 746f 6c65 7261 6e63 650d 0a77 6361  % tolerance..wca
+0000d3d0: 2e73 6574 5f74 6f6c 6572 616e 6365 2827  .set_tolerance('
+0000d3e0: 5627 2c20 302e 3129 2020 2320 3130 2520  V', 0.1)  # 10% 
+0000d3f0: 746f 6c65 7261 6e63 652e 2046 6f72 2057  tolerance. For W
+0000d400: 6f72 7374 2043 6173 6520 616e 616c 7973  orst Case analys
+0000d410: 6973 2c20 7468 6520 6469 7374 7269 6275  is, the distribu
+0000d420: 7469 6f6e 2069 7320 6972 7265 6c65 7661  tion is irreleva
+0000d430: 6e74 0d0a 0d0a 2320 536f 6d65 2063 6f6d  nt....# Some com
+0000d440: 706f 6e65 6e74 7320 6361 6e20 6861 7665  ponents can have
+0000d450: 2061 2064 6966 6665 7265 6e74 2074 6f6c   a different tol
+0000d460: 6572 616e 6365 0d0a 7763 612e 7365 745f  erance..wca.set_
+0000d470: 746f 6c65 7261 6e63 6528 2752 3127 2c20  tolerance('R1', 
+0000d480: 302e 3035 2920 2023 2035 2520 746f 6c65  0.05)  # 5% tole
+0000d490: 7261 6e63 6520 666f 7220 5231 206f 6e6c  rance for R1 onl
+0000d4a0: 792e 2054 6869 7320 6f6e 6c79 206f 7665  y. This only ove
+0000d4b0: 7272 6964 6573 2074 6865 2064 6566 6175  rrides the defau
+0000d4c0: 6c74 2074 6f6c 6572 616e 6365 2066 6f72  lt tolerance for
+0000d4d0: 2052 310d 0a0d 0a23 2054 6f6c 6572 616e   R1....# Toleran
+0000d4e0: 6365 7320 6361 6e20 6265 2073 6574 2066  ces can be set f
+0000d4f0: 6f72 2070 6172 616d 6574 6572 7320 6173  or parameters as
+0000d500: 2077 656c 6c2e 0d0a 7763 612e 7365 745f   well...wca.set_
+0000d510: 7061 7261 6d65 7465 725f 6465 7669 6174  parameter_deviat
+0000d520: 696f 6e28 2756 6f73 272c 2033 652d 342c  ion('Vos', 3e-4,
+0000d530: 2035 652d 3329 0d0a 0d0a 2320 4669 6e61   5e-3)....# Fina
+0000d540: 6c6c 7920 7468 6520 6e65 746c 6973 7420  lly the netlist 
+0000d550: 6973 2073 6176 6564 2074 6f20 6120 6669  is saved to a fi
+0000d560: 6c65 0d0a 7763 612e 7361 7665 5f6e 6574  le..wca.save_net
+0000d570: 6c69 7374 2827 2e2f 7465 7374 6669 6c65  list('./testfile
+0000d580: 732f 7361 6c6c 656e 6b65 795f 7763 2e61  s/sallenkey_wc.a
+0000d590: 7363 2729 0d0a 0d0a 7763 612e 7275 6e5f  sc')....wca.run_
+0000d5a0: 7465 7374 6265 6e63 6828 2920 2023 2052  testbench()  # R
+0000d5b0: 756e 7320 7468 6520 7369 6d75 6c61 7469  uns the simulati
+0000d5c0: 6f6e 2077 6974 6820 7370 6c69 7473 206f  on with splits o
+0000d5d0: 6620 3130 3020 7275 6e73 2065 6163 680d  f 100 runs each.
+0000d5e0: 0a0d 0a6c 6f67 7320 3d20 7763 612e 7265  ...logs = wca.re
+0000d5f0: 6164 5f6c 6f67 6669 6c65 7328 2920 2020  ad_logfiles()   
+0000d600: 2320 5265 6164 7320 7468 6520 6c6f 6720  # Reads the log 
+0000d610: 6669 6c65 7320 616e 6420 7374 6f72 6573  files and stores
+0000d620: 2074 6865 2072 6573 756c 7473 2069 6e20   the results in 
+0000d630: 7468 6520 7265 7375 6c74 7320 6174 7472  the results attr
+0000d640: 6962 7574 650d 0a6c 6f67 732e 6578 706f  ibute..logs.expo
+0000d650: 7274 5f64 6174 6128 272e 2f74 656d 705f  rt_data('./temp_
+0000d660: 7763 612f 6461 7461 2e63 7376 2729 2020  wca/data.csv')  
+0000d670: 2320 4578 706f 7274 7320 7468 6520 6461  # Exports the da
+0000d680: 7461 2074 6f20 6120 6373 7620 6669 6c65  ta to a csv file
+0000d690: 0d0a 0d0a 7072 696e 7428 2257 6f72 7374  ....print("Worst
+0000d6a0: 2063 6173 6520 7265 7375 6c74 733a 2229   case results:")
+0000d6b0: 0d0a 666f 7220 7061 7261 6d20 696e 2028  ..for param in (
+0000d6c0: 2766 6375 7427 2c20 2766 6375 745f 4652  'fcut', 'fcut_FR
+0000d6d0: 4f4d 2729 3a0d 0a20 2020 2070 7269 6e74  OM'):..    print
+0000d6e0: 2866 227b 7061 7261 6d7d 3a20 6d69 6e3a  (f"{param}: min:
+0000d6f0: 7b6c 6f67 732e 6d69 6e5f 6d65 6173 7572  {logs.min_measur
+0000d700: 655f 7661 6c75 6528 7061 7261 6d29 7d20  e_value(param)} 
+0000d710: 6d61 783a 7b6c 6f67 732e 6d61 785f 6d65  max:{logs.max_me
+0000d720: 6173 7572 655f 7661 6c75 6528 7061 7261  asure_value(para
+0000d730: 6d29 7d22 290d 0a0d 0a77 6361 2e63 6c65  m)}")....wca.cle
+0000d740: 616e 7570 5f66 696c 6573 2829 2020 2320  anup_files()  # 
+0000d750: 4465 6c65 7465 7320 7468 6520 7465 6d70  Deletes the temp
+0000d760: 6f72 6172 7920 6669 6c65 730d 0a60 6060  orary files..```
+0000d770: 0d0a 2d2d 2069 6e20 6578 616d 706c 6573  ..-- in examples
+0000d780: 2f72 756e 5f77 6f72 7374 5f63 6173 652e  /run_worst_case.
+0000d790: 7079 0d0a 0d0a 5768 656e 206f 7065 6e69  py....When openi
+0000d7a0: 6e67 2074 6865 2063 7265 6174 6564 2073  ng the created s
+0000d7b0: 616c 6c65 6e6b 6579 5f77 632e 6e65 7420  allenkey_wc.net 
+0000d7c0: 6669 6c65 2c20 7765 2063 616e 2073 6565  file, we can see
+0000d7d0: 2074 6861 7420 7468 6520 666f 6c6c 6f77   that the follow
+0000d7e0: 696e 6720 6369 7263 7569 742e 0d0a 0d0a  ing circuit.....
+0000d7f0: 215b 5361 6c6c 656e 2d4b 6579 2041 6d70  ![Sallen-Key Amp
+0000d800: 6c69 6669 6572 2077 6974 6820 5743 415d  lifier with WCA]
+0000d810: 282e 2f64 6f63 2f6d 6f64 756c 6573 2f73  (./doc/modules/s
+0000d820: 616c 6c65 6e6b 6579 5f77 632e 706e 6720  allenkey_wc.png 
+0000d830: 2253 616c 6c65 6e2d 4b65 7920 416d 706c  "Sallen-Key Ampl
+0000d840: 6966 6965 7220 7769 7468 2057 4341 2229  ifier with WCA")
+0000d850: 0d0a 0d0a 5468 6520 666f 6c6c 6f77 696e  ....The followin
+0000d860: 6720 7570 6461 7465 7320 7765 7265 206d  g updates were m
+0000d870: 6164 6520 746f 2074 6865 2063 6972 6375  ade to the circu
+0000d880: 6974 3a0d 0a2d 2054 6865 2076 616c 7565  it:..- The value
+0000d890: 206f 6620 6561 6368 2063 6f6d 706f 6e65   of each compone
+0000d8a0: 6e74 2077 6173 2072 6570 6c61 6365 6420  nt was replaced 
+0000d8b0: 6279 2061 2066 756e 6374 696f 6e20 7468  by a function th
+0000d8c0: 6174 2067 656e 6572 6174 6573 2061 206e  at generates a n
+0000d8d0: 6f6d 696e 616c 2c20 6d69 6e69 6d75 6d20  ominal, minimum 
+0000d8e0: 616e 6420 6d61 7869 6d75 6d20 7661 6c75  and maximum valu
+0000d8f0: 6520 6465 7065 6e64 696e 670d 0a6f 6e20  e depending..on 
+0000d900: 7468 6520 7275 6e20 7061 7261 6d65 7465  the run paramete
+0000d910: 7220 616e 6420 6973 2061 7373 6967 6e65  r and is assigne
+0000d920: 6420 6120 756e 6971 7565 2069 6e64 6578  d a unique index
+0000d930: 206e 756d 6265 722e 2028 5231 3d30 2c20   number. (R1=0, 
+0000d940: 566f 733d 312c 2052 323d 322c 202e 2e2e  Vos=1, R2=2, ...
+0000d950: 2056 323d 372c 2056 494e 3d38 290d 0a54   V2=7, VIN=8)..T
+0000d960: 6865 2075 6e69 7175 6520 6e75 6d62 6572  he unique number
+0000d970: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
+0000d980: 7468 6520 6269 7420 706f 7369 7469 6f6e  the bit position
+0000d990: 206f 6620 7468 6520 7275 6e20 7061 7261   of the run para
+0000d9a0: 6d65 7465 722e 2042 6974 2030 2063 6f72  meter. Bit 0 cor
+0000d9b0: 7265 7370 6f6e 6473 2074 6f20 7468 6520  responds to the 
+0000d9c0: 6d69 6e69 6d75 6d20 7661 6c75 6520 616e  minimum value an
+0000d9d0: 640d 0a62 6974 2031 2063 6f72 7265 7370  d..bit 1 corresp
+0000d9e0: 6f6e 6473 2074 6f20 7468 6520 6d61 7869  onds to the maxi
+0000d9f0: 6d75 6d20 7661 6c75 652e 2043 616c 6375  mum value. Calcu
+0000da00: 6c61 7469 6e67 2061 6c6c 2070 6f73 7369  lating all possi
+0000da10: 626c 6520 7065 726d 7574 6174 696f 6e73  ble permutations
+0000da20: 206f 6620 6d61 7869 6d75 6d20 616e 6420   of maximum and 
+0000da30: 6d69 6e69 6d75 6d20 7661 6c75 6573 2066  minimum values f
+0000da40: 6f72 2065 6163 680d 0a63 6f6d 706f 6e65  or each..compone
+0000da50: 6e74 2c20 7765 2067 6574 2032 2a2a 3920  nt, we get 2**9 
+0000da60: 3d20 3531 3220 706f 7373 6962 6c65 2063  = 512 possible c
+0000da70: 6f6d 6269 6e61 7469 6f6e 732e 2054 6869  ombinations. Thi
+0000da80: 7320 6d61 7073 2069 6e74 6f20 6120 3920  s maps into a 9 
+0000da90: 6269 7420 6269 6e61 7279 206e 756d 6265  bit binary numbe
+0000daa0: 722c 2077 6869 6368 2069 7320 7468 6520  r, which is the 
+0000dab0: 7275 6e20 7061 7261 6d65 7465 722e 0d0a  run parameter...
+0000dac0: 2d20 5468 6520 2e73 7465 7020 7061 7261  - The .step para
+0000dad0: 6d20 7275 6e20 636f 6d6d 616e 6420 7761  m run command wa
+0000dae0: 7320 6164 6465 6420 746f 2074 6865 206e  s added to the n
+0000daf0: 6574 6c69 7374 2e20 4974 2073 7461 7274  etlist. It start
+0000db00: 7320 6174 202d 3120 7768 6963 6820 6974  s at -1 which it
+0000db10: 2773 2074 6865 206e 6f6d 696e 616c 2076  's the nominal v
+0000db20: 616c 7565 2073 696d 756c 6174 696f 6e2c  alue simulation,
+0000db30: 2074 6865 6e20 300d 0a77 6869 6368 2063   then 0..which c
+0000db40: 6f72 7265 7370 6f6e 6473 2074 6f20 7468  orresponds to th
+0000db50: 6520 6d69 6e69 6d75 6d20 7661 6c75 6520  e minimum value 
+0000db60: 666f 7220 6561 6368 2063 6f6d 706f 6e65  for each compone
+0000db70: 6e74 2c20 7468 656e 2069 7420 6d61 6b65  nt, then it make
+0000db80: 7320 616c 6c20 636f 6d62 696e 6174 696f  s all combinatio
+0000db90: 6e73 206f 6620 6d69 6e69 6d75 6d20 616e  ns of minimum an
+0000dba0: 6420 6d61 7869 6d75 6d20 7661 6c75 6573  d maximum values
+0000dbb0: 200d 0a75 6e74 696c 2035 3131 2c20 7768   ..until 511, wh
+0000dbc0: 6963 6820 6973 2074 6865 2073 696d 756c  ich is the simul
+0000dbd0: 6174 696f 6e20 7769 7468 2061 6c6c 206d  ation with all m
+0000dbe0: 6178 696d 756d 2076 616c 7565 732e 0d0a  aximum values...
+0000dbf0: 2d20 4120 6465 6661 756c 7420 7661 6c75  - A default valu
+0000dc00: 6520 666f 7220 7468 6520 7275 6e20 7061  e for the run pa
+0000dc10: 7261 6d65 7465 7220 7761 7320 6164 6465  rameter was adde
+0000dc20: 642e 2054 6869 7320 6973 2075 7365 6675  d. This is usefu
+0000dc30: 6c20 6966 2074 6865 202e 7374 6570 2070  l if the .step p
+0000dc40: 6172 616d 2072 756e 2069 7320 636f 6d6d  aram run is comm
+0000dc50: 656e 7465 6420 6f75 742e 0d0a 2d20 5468  ented out...- Th
+0000dc60: 6520 5231 2074 6f6c 6572 616e 6365 2069  e R1 tolerance i
+0000dc70: 7320 6469 6666 6572 656e 7420 6672 6f6d  s different from
+0000dc80: 2074 6865 206f 7468 6572 2072 6573 6973   the other resis
+0000dc90: 746f 7273 2e20 5468 6973 2069 7320 6265  tors. This is be
+0000dca0: 6361 7573 6520 7468 6520 746f 6c65 7261  cause the tolera
+0000dcb0: 6e63 6520 7761 7320 6578 706c 6963 6974  nce was explicit
+0000dcc0: 6c79 2073 6574 2066 6f72 2052 312e 0d0a  ly set for R1...
+0000dcd0: 2d20 5468 6520 7763 2829 2066 756e 6374  - The wc() funct
+0000dce0: 696f 6e20 6973 2061 6464 6564 2074 6f20  ion is added to 
+0000dcf0: 7468 6520 6369 7263 7569 742e 2054 6869  the circuit. Thi
+0000dd00: 7320 6675 6e63 7469 6f6e 2069 7320 7573  s function is us
+0000dd10: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
+0000dd20: 7468 6520 776f 7273 7420 6361 7365 2076  the worst case v
+0000dd30: 616c 7565 2066 6f72 2065 6163 6820 636f  alue for each co
+0000dd40: 6d70 6f6e 656e 742c 0d0a 6769 7665 6e20  mponent,..given 
+0000dd50: 6120 746f 6c65 7261 6e63 6520 7661 6c75  a tolerance valu
+0000dd60: 6520 616e 6420 6974 7320 7265 7370 6563  e and its respec
+0000dd70: 7469 7665 2069 6e64 6578 2e0d 0a2d 2054  tive index...- T
+0000dd80: 6865 2077 6331 2829 2066 756e 6374 696f  he wc1() functio
+0000dd90: 6e20 6973 2061 6464 6564 2074 6f20 7468  n is added to th
+0000dda0: 6520 6369 7263 7569 742e 2054 6869 7320  e circuit. This 
+0000ddb0: 6675 6e63 7469 6f6e 2069 7320 7573 6564  function is used
+0000ddc0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+0000ddd0: 6520 776f 7273 7420 6361 7365 2076 616c  e worst case val
+0000dde0: 7565 2066 6f72 2065 6163 6820 636f 6d70  ue for each comp
+0000ddf0: 6f6e 656e 742c 0d0a 6769 7665 6e20 6120  onent,..given a 
+0000de00: 6d69 6e69 6d75 6d20 616e 6420 6d61 7869  minimum and maxi
+0000de10: 6d75 6d20 7661 6c75 6520 616e 6420 6974  mum value and it
+0000de20: 7320 7265 7370 6563 7469 7665 2069 6e64  s respective ind
+0000de30: 6578 2e0d 0a0d 0a23 2323 204c 5453 7465  ex.....### LTSte
+0000de40: 7073 2e70 7920 2323 230d 0a0d 0a54 6869  ps.py ###....Thi
+0000de50: 7320 6d6f 6475 6c65 2064 6566 696e 6573  s module defines
+0000de60: 2061 2063 6c61 7373 2074 6861 7420 6361   a class that ca
+0000de70: 6e20 6265 2075 7365 6420 746f 2070 6172  n be used to par
+0000de80: 7365 204c 5453 7069 6365 206c 6f67 2066  se LTSpice log f
+0000de90: 696c 6573 2077 6865 7265 2074 6865 2069  iles where the i
+0000dea0: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+0000deb0: 202e 5354 4550 2069 6e66 6f72 6d61 7469   .STEP informati
+0000dec0: 6f6e 2069 730d 0a77 7269 7474 656e 2e20  on is..written. 
+0000ded0: 5468 6572 6520 6172 6520 7477 6f20 706f  There are two po
+0000dee0: 7373 6962 6c65 2075 7361 6765 7320 6f66  ssible usages of
+0000def0: 2074 6869 7320 6d6f 6475 6c65 2c20 6569   this module, ei
+0000df00: 7468 6572 2070 726f 6772 616d 6d61 7469  ther programmati
+0000df10: 6361 6c6c 7920 6279 2069 6d70 6f72 7469  cally by importi
+0000df20: 6e67 2074 6865 206d 6f64 756c 6520 616e  ng the module an
+0000df30: 6420 7468 656e 0d0a 6163 6365 7373 696e  d then..accessin
+0000df40: 6720 6461 7461 2074 6872 6f75 6768 2074  g data through t
+0000df50: 6865 2063 6c61 7373 2061 7320 6578 656d  he class as exem
+0000df60: 706c 6966 6965 6420 6865 7265 3a0d 0a0d  plified here:...
+0000df70: 0a60 6060 7079 7468 6f6e 0d0a 2321 2f75  .```python..#!/u
+0000df80: 7372 2f62 696e 2f65 6e76 2070 7974 686f  sr/bin/env pytho
+0000df90: 6e0d 0a23 2063 6f64 696e 673d 7574 662d  n..# coding=utf-
+0000dfa0: 380d 0a0d 0a66 726f 6d20 5079 4c54 5370  8....from PyLTSp
+0000dfb0: 6963 652e 6c6f 672e 6c74 7374 6570 7320  ice.log.ltsteps 
+0000dfc0: 696d 706f 7274 204c 5453 7069 6365 4c6f  import LTSpiceLo
+0000dfd0: 6752 6561 6465 720d 0a0d 0a64 6174 6120  gReader....data 
+0000dfe0: 3d20 4c54 5370 6963 654c 6f67 5265 6164  = LTSpiceLogRead
+0000dff0: 6572 2822 2e2f 7465 7374 6669 6c65 732f  er("./testfiles/
+0000e000: 4261 7463 685f 5465 7374 5f41 4438 3230  Batch_Test_AD820
+0000e010: 5f31 352e 6c6f 6722 290d 0a0d 0a70 7269  _15.log")....pri
+0000e020: 6e74 2822 4e75 6d62 6572 206f 6620 7374  nt("Number of st
+0000e030: 6570 7320 203a 222c 2064 6174 612e 7374  eps  :", data.st
+0000e040: 6570 5f63 6f75 6e74 290d 0a73 7465 705f  ep_count)..step_
+0000e050: 6e61 6d65 7320 3d20 6461 7461 2e67 6574  names = data.get
+0000e060: 5f73 7465 705f 7661 7273 2829 0d0a 6d65  _step_vars()..me
+0000e070: 6173 5f6e 616d 6573 203d 2064 6174 612e  as_names = data.
+0000e080: 6765 745f 6d65 6173 7572 655f 6e61 6d65  get_measure_name
+0000e090: 7328 290d 0a0d 0a23 2050 7269 6e74 696e  s()....# Printin
+0000e0a0: 6720 4865 6164 6572 730d 0a70 7269 6e74  g Headers..print
+0000e0b0: 2827 2027 2e6a 6f69 6e28 5b66 227b 7374  (' '.join([f"{st
+0000e0c0: 6570 3a31 3573 7d22 2066 6f72 2073 7465  ep:15s}" for ste
+0000e0d0: 7020 696e 2073 7465 705f 6e61 6d65 735d  p in step_names]
+0000e0e0: 292c 2065 6e64 3d27 2729 2020 2320 5072  ), end='')  # Pr
+0000e0f0: 696e 7420 7374 6570 7320 6e61 6d65 7320  int steps names 
+0000e100: 7769 7468 206e 6f20 6e65 7720 6c69 6e65  with no new line
+0000e110: 0d0a 7072 696e 7428 2720 272e 6a6f 696e  ..print(' '.join
+0000e120: 285b 6622 7b6e 616d 653a 3135 737d 2220  ([f"{name:15s}" 
+0000e130: 666f 7220 6e61 6d65 2069 6e20 6d65 6173  for name in meas
+0000e140: 5f6e 616d 6573 5d29 2c20 656e 643d 275c  _names]), end='\
+0000e150: 6e27 290d 0a23 2050 7269 6e74 696e 6720  n')..# Printing 
+0000e160: 6461 7461 0d0a 666f 7220 6920 696e 2072  data..for i in r
+0000e170: 616e 6765 2864 6174 612e 7374 6570 5f63  ange(data.step_c
+0000e180: 6f75 6e74 293a 0d0a 2020 2020 7072 696e  ount):..    prin
+0000e190: 7428 2720 272e 6a6f 696e 285b 6622 7b64  t(' '.join([f"{d
+0000e1a0: 6174 615b 7374 6570 5d5b 695d 3a31 357d  ata[step][i]:15}
+0000e1b0: 2220 666f 7220 7374 6570 2069 6e20 7374  " for step in st
+0000e1c0: 6570 5f6e 616d 6573 5d29 2c20 656e 643d  ep_names]), end=
+0000e1d0: 2727 2920 2023 2050 7269 6e74 2073 7465  '')  # Print ste
+0000e1e0: 7073 206e 616d 6573 2077 6974 6820 6e6f  ps names with no
+0000e1f0: 206e 6577 206c 696e 650d 0a20 2020 2070   new line..    p
+0000e200: 7269 6e74 2827 2027 2e6a 6f69 6e28 5b66  rint(' '.join([f
+0000e210: 227b 6461 7461 5b6e 616d 655d 5b69 5d3a  "{data[name][i]:
+0000e220: 3135 7d22 2066 6f72 206e 616d 6520 696e  15}" for name in
+0000e230: 206d 6561 735f 6e61 6d65 735d 292c 2065   meas_names]), e
+0000e240: 6e64 3d27 5c6e 2729 2020 2320 5072 696e  nd='\n')  # Prin
+0000e250: 7420 4865 6164 6572 0d0a 0d0a 7072 696e  t Header....prin
+0000e260: 7428 2254 6f74 616c 206e 756d 6265 7220  t("Total number 
+0000e270: 6f66 206d 6561 7375 7265 7320 666f 756e  of measures foun
+0000e280: 6420 3a22 2c20 6461 7461 2e6d 6561 7375  d :", data.measu
+0000e290: 7265 5f63 6f75 6e74 290d 0a60 6060 0d0a  re_count)..```..
+0000e2a0: 2d2d 2069 6e20 6578 616d 706c 6573 2f6c  -- in examples/l
+0000e2b0: 7473 7465 7073 5f65 7861 6d70 6c65 2e70  tsteps_example.p
+0000e2c0: 790d 0a0d 0a54 6865 2073 6563 6f6e 6420  y....The second 
+0000e2d0: 706f 7373 6962 696c 6974 7920 6973 2074  possibility is t
+0000e2e0: 6f20 7573 6520 7468 6520 6d6f 6475 6c65  o use the module
+0000e2f0: 2064 6972 6563 746c 7920 6f6e 2074 6865   directly on the
+0000e300: 2063 6f6d 6d61 6e64 206c 696e 650d 0a0d   command line...
+0000e310: 0a23 2043 6f6d 6d61 6e64 204c 696e 6520  .# Command Line 
+0000e320: 496e 7465 7266 6163 6520 230d 0a0d 0a23  Interface #....#
+0000e330: 2323 206c 7473 7465 7073 2e65 7865 2023  ## ltsteps.exe #
+0000e340: 2323 0d0a 0d0a 5468 6520 3c66 696c 656e  ##....The <filen
+0000e350: 616d 653e 2063 616e 2062 6520 6569 7468  ame> can be eith
+0000e360: 6572 2062 6520 6120 6c6f 6720 6669 6c65  er be a log file
+0000e370: 2028 2e6c 6f67 292c 2061 2064 6174 6120   (.log), a data 
+0000e380: 6578 706f 7274 2066 696c 6520 282e 7478  export file (.tx
+0000e390: 7429 206f 7220 6120 6d65 6173 7572 656d  t) or a measurem
+0000e3a0: 656e 7420 6f75 7470 7574 2066 696c 6520  ent output file 
+0000e3b0: 282e 6d65 6173 290d 0a54 6869 7320 7769  (.meas)..This wi
+0000e3c0: 6c6c 2070 726f 6365 7373 2061 6c6c 2074  ll process all t
+0000e3d0: 6865 2064 6174 6120 616e 6420 6578 706f  he data and expo
+0000e3e0: 7274 2069 7420 6175 746f 6d61 7469 6361  rt it automatica
+0000e3f0: 6c6c 7920 696e 746f 2061 2074 6578 7420  lly into a text 
+0000e400: 6669 6c65 2077 6974 6820 7468 6520 6578  file with the ex
+0000e410: 7465 6e73 696f 6e20 2874 6c6f 672c 2074  tension (tlog, t
+0000e420: 7376 2c20 746d 6561 7329 0d0a 7768 6572  sv, tmeas)..wher
+0000e430: 6520 7468 6520 6461 7461 2072 6561 6420  e the data read 
+0000e440: 6973 2066 6f72 6d61 7474 6564 2069 6e74  is formatted int
+0000e450: 6f20 6120 6d6f 7265 2063 6f6e 7665 6e69  o a more conveni
+0000e460: 656e 7420 7461 6220 7365 7061 7261 7465  ent tab separate
+0000e470: 6420 666f 726d 6174 2e20 496e 2063 6173  d format. In cas
+0000e480: 6520 7468 6520 3c6c 6f67 6669 6c65 3e20  e the <logfile> 
+0000e490: 6973 206e 6f74 2070 726f 7669 6465 642c  is not provided,
+0000e4a0: 2074 6865 0d0a 7363 7269 7074 2077 696c   the..script wil
+0000e4b0: 6c20 7363 616e 2074 6865 2064 6972 6563  l scan the direc
+0000e4c0: 746f 7279 2061 6e64 2070 726f 6365 7373  tory and process
+0000e4d0: 2074 6865 206e 6577 6573 7420 6c6f 672c   the newest log,
+0000e4e0: 2074 7874 206f 7220 6f75 7420 6669 6c65   txt or out file
+0000e4f0: 2066 6f75 6e64 2e0d 0a0d 0a23 2323 2068   found.....### h
+0000e500: 6973 746f 6772 616d 2e65 7865 2023 2323  istogram.exe ###
+0000e510: 0d0a 0d0a 5468 6973 206d 6f64 756c 6520  ....This module 
+0000e520: 7573 6573 2074 6865 2064 6174 6120 696e  uses the data in
+0000e530: 7369 6465 206f 6e20 7468 6520 6669 6c65  side on the file
+0000e540: 6e61 6d65 2074 6f20 7072 6f64 7563 6520  name to produce 
+0000e550: 6120 6869 7374 6f67 7261 6d20 696d 6167  a histogram imag
+0000e560: 652e 0d0a 0d0a 6060 600d 0a55 7361 6765  e.....```..Usage
+0000e570: 3a20 4869 7374 6f67 7261 6d2e 7079 205b  : Histogram.py [
+0000e580: 6f70 7469 6f6e 735d 204c 4f47 5f46 494c  options] LOG_FIL
+0000e590: 4520 5452 4143 450d 0a0d 0a4f 7074 696f  E TRACE....Optio
+0000e5a0: 6e73 3a0d 0a20 202d 2d76 6572 7369 6f6e  ns:..  --version
+0000e5b0: 2020 2020 2020 2020 2020 2020 2073 686f               sho
+0000e5c0: 7720 7072 6f67 7261 6d27 7320 7665 7273  w program's vers
+0000e5d0: 696f 6e20 6e75 6d62 6572 2061 6e64 2065  ion number and e
+0000e5e0: 7869 740d 0a20 202d 682c 202d 2d68 656c  xit..  -h, --hel
+0000e5f0: 7020 2020 2020 2020 2020 2020 2073 686f  p            sho
+0000e600: 7720 7468 6973 2068 656c 7020 6d65 7373  w this help mess
+0000e610: 6167 6520 616e 6420 6578 6974 0d0a 2020  age and exit..  
+0000e620: 2d73 2053 4947 4d41 2c20 2d2d 7369 676d  -s SIGMA, --sigm
+0000e630: 613d 5349 474d 410d 0a20 2020 2020 2020  a=SIGMA..       
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e650: 2053 6967 6d61 2074 6f20 6265 2075 7365   Sigma to be use
+0000e660: 6420 696e 2074 6865 2064 6973 7472 6962  d in the distrib
+0000e670: 7574 696f 6e20 6669 742e 2044 6566 6175  ution fit. Defau
+0000e680: 6c74 3d33 0d0a 2020 2d6e 204e 4249 4e53  lt=3..  -n NBINS
+0000e690: 2c20 2d2d 6e62 696e 733d 4e42 494e 530d  , --nbins=NBINS.
+0000e6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e6b0: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
+0000e6c0: 6f66 2062 696e 7320 746f 2062 6520 7573  of bins to be us
+0000e6d0: 6564 2069 6e20 7468 6520 6869 7374 6f67  ed in the histog
+0000e6e0: 7261 6d2e 2044 6566 6175 6c74 3d32 300d  ram. Default=20.
+0000e6f0: 0a20 202d 6320 4649 4c54 4552 532c 202d  .  -c FILTERS, -
+0000e700: 2d63 6f6e 6469 7469 6f6e 3d46 494c 5445  -condition=FILTE
+0000e710: 5253 0d0a 2020 2020 2020 2020 2020 2020  RS..            
+0000e720: 2020 2020 2020 2020 2020 2020 4669 6c74              Filt
+0000e730: 6572 2063 6f6e 6469 7469 6f6e 2077 7269  er condition wri
+0000e740: 7465 6e20 696e 2070 7974 686f 6e2e 204d  ten in python. M
+0000e750: 6f72 6520 7468 616e 206f 6e65 0d0a 2020  ore than one..  
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
+0000e780: 2063 616e 2062 6520 6164 6465 6420 6275   can be added bu
+0000e790: 7420 6561 6368 2065 7870 7265 7373 696f  t each expressio
+0000e7a0: 6e20 7368 6f75 6c64 2062 650d 0a20 2020  n should be..   
+0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7c0: 2020 2020 2070 7265 6365 6465 6420 6279       preceded by
+0000e7d0: 202d 632e 2045 5841 4d50 4c45 3a20 2d63   -c. EXAMPLE: -c
+0000e7e0: 2056 284e 3030 3129 3e34 202d 6320 7061   V(N001)>4 -c pa
+0000e7f0: 7261 6d65 7465 723d 3d31 0d0a 2020 2020  rameter==1..    
+0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e810: 2020 2020 2d63 2020 4928 5631 293c 302e      -c  I(V1)<0.
+0000e820: 350d 0a20 202d 6620 464f 524d 4154 2c20  5..  -f FORMAT, 
+0000e830: 2d2d 666f 726d 6174 3d46 4f52 4d41 540d  --format=FORMAT.
+0000e840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e850: 2020 2020 2020 2020 2046 6f72 6d61 7420           Format 
+0000e860: 7374 7269 6e67 2066 6f72 2074 6865 2058  string for the X
+0000e870: 2061 7869 732e 2045 7861 6d70 6c65 3a20   axis. Example: 
+0000e880: 2d66 2025 332e 3466 0d0a 2020 2d74 2054  -f %3.4f..  -t T
+0000e890: 4954 4c45 2c20 2d2d 7469 746c 653d 5449  ITLE, --title=TI
+0000e8a0: 544c 450d 0a20 2020 2020 2020 2020 2020  TLE..           
+0000e8b0: 2020 2020 2020 2020 2020 2020 2054 6974               Tit
+0000e8c0: 6c65 2074 6f20 6170 7065 6172 206f 6e20  le to appear on 
+0000e8d0: 7468 6520 746f 7020 6f66 2074 6865 2068  the top of the h
+0000e8e0: 6973 746f 6772 616d 2e0d 0a20 202d 7220  istogram...  -r 
+0000e8f0: 5241 4e47 452c 202d 2d72 616e 6765 3d52  RANGE, --range=R
+0000e900: 414e 4745 0d0a 2020 2020 2020 2020 2020  ANGE..          
+0000e910: 2020 2020 2020 2020 2020 2020 2020 5261                Ra
+0000e920: 6e67 6520 6f66 2074 6865 2058 2061 7869  nge of the X axi
+0000e930: 7320 746f 2075 7365 2066 6f72 2074 6865  s to use for the
+0000e940: 2068 6973 746f 6772 616d 2069 6e20 7468   histogram in th
+0000e950: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000e960: 2020 2020 2020 2020 2020 2066 6f72 6d20             form 
+0000e970: 6d69 6e3a 6d61 782e 2045 7861 6d70 6c65  min:max. Example
+0000e980: 3a20 2d72 202d 313a 310d 0a20 202d 432c  : -r -1:1..  -C,
+0000e990: 202d 2d63 6c69 7062 6f61 7264 2020 2020   --clipboard    
+0000e9a0: 2020 2049 6620 7468 6520 6461 7461 2066     If the data f
+0000e9b0: 726f 6d20 7468 6520 636c 6970 626f 6172  rom the clipboar
+0000e9c0: 6420 6973 2074 6f20 6265 2075 7365 642e  d is to be used.
+0000e9d0: 0d0a 2020 2d69 2049 4d41 4745 4649 4c45  ..  -i IMAGEFILE
+0000e9e0: 2c20 2d2d 696d 6167 653d 494d 4147 4546  , --image=IMAGEF
+0000e9f0: 494c 450d 0a20 2020 2020 2020 2020 2020  ILE..           
+0000ea00: 2020 2020 2020 2020 2020 2020 204e 616d               Nam
+0000ea10: 6520 6f66 2074 6865 2069 6d61 6765 2046  e of the image F
+0000ea20: 696c 652e 2065 7874 656e 7369 6f6e 2027  ile. extension '
+0000ea30: 706e 6727 2020 2020 0d0a 6060 600d 0a0d  png'    ..```...
+0000ea40: 0a23 2323 2072 6177 636f 6e76 6572 742e  .### rawconvert.
+0000ea50: 6578 6520 2323 230d 0a0d 0a41 2074 6f6f  exe ###....A too
+0000ea60: 6c20 746f 2063 6f6e 7665 7274 202e 7261  l to convert .ra
+0000ea70: 7720 6669 6c65 7320 696e 746f 2063 7376  w files into csv
+0000ea80: 206f 7220 4578 6365 6c20 6669 6c65 732e   or Excel files.
+0000ea90: 0d0a 0d0a 6060 600d 0a55 7361 6765 3a20  ....```..Usage: 
+0000eaa0: 7261 775f 636f 6e76 6572 742e 6578 6520  raw_convert.exe 
+0000eab0: 5b6f 7074 696f 6e73 5d20 3c72 6177 6669  [options] <rawfi
+0000eac0: 6c65 3e20 3c74 7261 6365 5f6c 6973 743e  le> <trace_list>
+0000ead0: 0d0a 0d0a 4f70 7469 6f6e 733a 0d0a 2020  ....Options:..  
+0000eae0: 2d2d 7665 7273 696f 6e20 2020 2020 2020  --version       
+0000eaf0: 2020 2020 2020 7368 6f77 2070 726f 6772        show progr
+0000eb00: 616d 2773 2076 6572 7369 6f6e 206e 756d  am's version num
+0000eb10: 6265 7220 616e 6420 6578 6974 0d0a 2020  ber and exit..  
+0000eb20: 2d68 2c20 2d2d 6865 6c70 2020 2020 2020  -h, --help      
+0000eb30: 2020 2020 2020 7368 6f77 2074 6869 7320        show this 
+0000eb40: 6865 6c70 206d 6573 7361 6765 2061 6e64  help message and
+0000eb50: 2065 7869 740d 0a20 202d 6f20 4649 4c45   exit..  -o FILE
+0000eb60: 2c20 2d2d 6f75 7470 7574 3d46 494c 450d  , --output=FILE.
+0000eb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb80: 2020 2020 2020 2020 204f 7574 7075 7420           Output 
+0000eb90: 6669 6c65 206e 616d 652e 2055 7365 202e  file name. Use .
+0000eba0: 6373 7620 666f 7220 4353 5620 6f75 7470  csv for CSV outp
+0000ebb0: 7574 2c20 2e78 6c73 7820 666f 720d 0a20  ut, .xlsx for.. 
+0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebd0: 2020 2020 2020 2045 7863 656c 206f 7574         Excel out
+0000ebe0: 7075 740d 0a20 202d 632c 202d 2d63 6c69  put..  -c, --cli
+0000ebf0: 7062 6f61 7264 2020 2020 2020 204f 7574  pboard       Out
+0000ec00: 7075 7420 746f 2063 6c69 7062 6f61 7264  put to clipboard
+0000ec10: 0d0a 2020 2d76 2c20 2d2d 7665 7262 6f73  ..  -v, --verbos
+0000ec20: 6520 2020 2020 2020 2020 5665 7262 6f73  e         Verbos
+0000ec30: 6520 6f75 7470 7574 0d0a 2020 2d73 2053  e output..  -s S
+0000ec40: 4550 4152 4154 4f52 2c20 2d2d 7365 703d  EPARATOR, --sep=
+0000ec50: 5345 5041 5241 544f 520d 0a20 2020 2020  SEPARATOR..     
+0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec70: 2020 2056 616c 7565 2073 6570 6172 6174     Value separat
+0000ec80: 6f72 2066 6f72 2043 5356 206f 7574 7075  or for CSV outpu
+0000ec90: 742e 2044 6566 6175 6c74 3a20 225c 7422  t. Default: "\t"
+0000eca0: 203c 5441 423e 0d0a 2020 2020 2020 2020   <TAB>..        
+0000ecb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecc0: 4578 616d 706c 653a 202d 6420 223b 220d  Example: -d ";".
+0000ecd0: 0a60 6060 0d0a 0d0a 2323 2320 7275 6e5f  .```....### run_
+0000ece0: 7365 7276 6572 2e65 7865 2023 2323 0d0a  server.exe ###..
+0000ecf0: 0d0a 5468 6973 2063 6f6d 6d61 6e64 206c  ..This command l
+0000ed00: 696e 6520 746f 6f6c 2077 6173 206d 6f76  ine tool was mov
+0000ed10: 6564 2074 6f20 7468 6520 7370 6963 656c  ed to the spicel
+0000ed20: 6962 2070 6163 6b61 6765 2e0d 0a0d 0a23  ib package.....#
+0000ed30: 2323 2053 656d 6944 6576 4f70 5265 6164  ## SemiDevOpRead
+0000ed40: 6572 2e70 7920 2323 230d 0a0d 0a54 6869  er.py ###....Thi
+0000ed50: 7320 6d6f 6475 6c65 2069 7320 7573 6564  s module is used
+0000ed60: 2074 6f20 7265 6164 2066 726f 6d20 4c54   to read from LT
+0000ed70: 5370 6963 6520 6c6f 6720 6669 6c65 7320  Spice log files 
+0000ed80: 5365 6d69 636f 6e64 7563 746f 7220 4465  Semiconductor De
+0000ed90: 7669 6365 7320 4f70 6572 6174 696e 6720  vices Operating 
+0000eda0: 506f 696e 7420 496e 666f 726d 6174 696f  Point Informatio
+0000edb0: 6e2e 2041 206d 6f72 6520 6465 7461 696c  n. A more detail
+0000edc0: 6564 0d0a 646f 6375 6d65 6e74 6174 696f  ed..documentatio
+0000edd0: 6e20 6973 2064 6972 6563 746c 7920 696e  n is directly in
+0000ede0: 636c 7564 6564 2069 6e20 7468 6520 736f  cluded in the so
+0000edf0: 7572 6365 2066 696c 6520 646f 6373 7472  urce file docstr
+0000ee00: 696e 6773 2e0d 0a0d 0a23 2320 4465 6275  ings.....## Debu
+0000ee10: 6720 4c6f 6767 696e 670d 0a0d 0a54 6865  g Logging....The
+0000ee20: 206c 6962 7261 7279 2075 7365 7320 7468   library uses th
+0000ee30: 6520 7374 616e 6461 7264 2060 6c6f 6767  e standard `logg
+0000ee40: 696e 6760 206d 6f64 756c 652e 2054 6872  ing` module. Thr
+0000ee50: 6565 2063 6f6e 7665 6e69 656e 6365 2066  ee convenience f
+0000ee60: 756e 6374 696f 6e73 2068 6176 6520 6265  unctions have be
+0000ee70: 656e 2061 6464 6564 2066 6f72 2065 6173  en added for eas
+0000ee80: 696c 7920 6368 616e 6769 6e67 206c 6f67  ily changing log
+0000ee90: 6769 6e67 0d0a 7365 7474 696e 6773 2061  ging..settings a
+0000eea0: 6372 6f73 7320 7468 6520 656e 7469 7265  cross the entire
+0000eeb0: 206c 6962 7261 7279 2e20 6050 794c 5453   library. `PyLTS
+0000eec0: 7069 6365 2e61 6c6c 5f6c 6f67 6765 7273  pice.all_loggers
+0000eed0: 2829 6020 7265 7475 726e 7320 6120 6c69  ()` returns a li
+0000eee0: 7374 206f 6620 616c 6c20 7468 6520 6c6f  st of all the lo
+0000eef0: 6767 6572 2773 0d0a 6e61 6d65 732c 2060  gger's..names, `
+0000ef00: 5079 4c54 5370 6963 652e 7365 745f 6c6f  PyLTSpice.set_lo
+0000ef10: 675f 6c65 7665 6c28 6c6f 6767 696e 672e  g_level(logging.
+0000ef20: 4445 4255 4729 600d 0a77 6f75 6c64 2073  DEBUG)`..would s
+0000ef30: 6574 2074 6865 206c 6962 7261 7279 2773  et the library's
+0000ef40: 206c 6f67 6769 6e67 206c 6576 656c 2074   logging level t
+0000ef50: 6f20 6465 6275 672c 2061 6e64 2060 5079  o debug, and `Py
+0000ef60: 4c54 5370 6963 652e 6164 645f 6c6f 675f  LTSpice.add_log_
+0000ef70: 6861 6e64 6c65 7228 6d79 5f68 616e 646c  handler(my_handl
+0000ef80: 6572 2960 2077 6f75 6c64 2061 6464 2060  er)` would add `
+0000ef90: 6d79 5f68 616e 646c 6572 6020 6173 2061  my_handler` as a
+0000efa0: 0d0a 6861 6e64 6c65 7220 666f 720d 0a61  ..handler for..a
+0000efb0: 6c6c 206c 6f67 6765 7273 2e0d 0a0d 0a23  ll loggers.....#
+0000efc0: 2323 2053 696e 676c 6520 4d6f 6475 6c65  ## Single Module
+0000efd0: 204c 6f67 6769 6e67 0d0a 0d0a 4974 2069   Logging....It i
+0000efe0: 7320 616c 736f 2070 6f73 7369 626c 6520  s also possible 
+0000eff0: 746f 2073 6574 2074 6865 206c 6f67 6769  to set the loggi
+0000f000: 6e67 2073 6574 7469 6e67 7320 666f 7220  ng settings for 
+0000f010: 6120 7369 6e67 6c65 206d 6f64 756c 6520  a single module 
+0000f020: 6279 2075 7369 6e67 2069 7473 206e 616d  by using its nam
+0000f030: 6520 6163 7175 6972 6564 2066 726f 6d0d  e acquired from.
+0000f040: 0a74 6865 2060 5079 4c54 5370 6963 652e  .the `PyLTSpice.
+0000f050: 616c 6c5f 6c6f 6767 6572 7328 2960 0d0a  all_loggers()`..
+0000f060: 6675 6e63 7469 6f6e 2e20 466f 7220 6578  function. For ex
+0000f070: 616d 706c 653a 0d0a 0d0a 6060 6070 7974  ample:....```pyt
+0000f080: 686f 6e0d 0a69 6d70 6f72 7420 6c6f 6767  hon..import logg
+0000f090: 696e 670d 0a0d 0a6c 6f67 6769 6e67 2e62  ing....logging.b
+0000f0a0: 6173 6963 436f 6e66 6967 286c 6576 656c  asicConfig(level
+0000f0b0: 3d6c 6f67 6769 6e67 2e49 4e46 4f29 2020  =logging.INFO)  
+0000f0c0: 2320 5365 7420 7570 2074 6865 2072 6f6f  # Set up the roo
+0000f0d0: 7420 6c6f 6767 6572 2066 6972 7374 0d0a  t logger first..
+0000f0e0: 0d0a 696d 706f 7274 2050 794c 5453 7069  ..import PyLTSpi
+0000f0f0: 6365 2020 2320 496d 706f 7274 2050 794c  ce  # Import PyL
+0000f100: 5453 7069 6365 2074 6f20 7365 7420 7468  TSpice to set th
+0000f110: 6520 6c6f 6767 696e 6720 6c65 7665 6c73  e logging levels
+0000f120: 0d0a 0d0a 5079 4c54 5370 6963 652e 7365  ....PyLTSpice.se
+0000f130: 745f 6c6f 675f 6c65 7665 6c28 6c6f 6767  t_log_level(logg
+0000f140: 696e 672e 4445 4255 4729 2020 2320 5365  ing.DEBUG)  # Se
+0000f150: 7420 5079 4c54 5370 6963 6527 7320 676c  t PyLTSpice's gl
+0000f160: 6f62 616c 206c 6f67 206c 6576 656c 0d0a  obal log level..
+0000f170: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
+0000f180: 7228 2250 794c 5453 7069 6365 2e52 6177  r("PyLTSpice.Raw
+0000f190: 5265 6164 2229 2e6c 6576 656c 203d 206c  Read").level = l
+0000f1a0: 6f67 6769 6e67 2e57 4152 4e49 4e47 2020  ogging.WARNING  
+0000f1b0: 2320 5365 7420 7468 6520 6c6f 6720 6c65  # Set the log le
+0000f1c0: 7665 6c20 666f 7220 6f6e 6c79 2052 6177  vel for only Raw
+0000f1d0: 5265 6164 2074 6f20 7761 726e 696e 670d  Read to warning.
+0000f1e0: 0a60 6060 0d0a 0d0a 576f 756c 6420 7365  .```....Would se
+0000f1f0: 7420 6f6e 6c79 2060 5079 4c54 5370 6963  t only `PyLTSpic
+0000f200: 652e 5261 7752 6561 6460 2066 696c 6527  e.RawRead` file'
+0000f210: 7320 6c6f 6767 696e 6720 6c65 7665 6c20  s logging level 
+0000f220: 746f 2077 6172 6e69 6e67 2077 6869 6c65  to warning while
+0000f230: 2074 6865 206f 7468 6572 206d 6f64 756c   the other modul
+0000f240: 6573 2077 6f75 6c64 2072 656d 6169 6e20  es would remain 
+0000f250: 6174 2064 6562 7567 206c 6576 656c 2e0d  at debug level..
+0000f260: 0a5f 4d61 6b65 2073 7572 6520 746f 2069  ._Make sure to i
+0000f270: 6e69 7469 616c 697a 6520 7468 6520 726f  nitialize the ro
+0000f280: 6f74 206c 6f67 6765 7220 6265 666f 7265  ot logger before
+0000f290: 2069 6d70 6f72 7469 6e67 2074 6865 206c   importing the l
+0000f2a0: 6962 7261 7279 2074 6f20 6265 2061 626c  ibrary to be abl
+0000f2b0: 6520 746f 2073 6565 2074 6865 206c 6f67  e to see the log
+0000f2c0: 732e 5f0d 0a0d 0a23 2320 546f 2077 686f  s._....## To who
+0000f2d0: 6d20 646f 2049 2074 616c 6b20 746f 3f20  m do I talk to? 
+0000f2e0: 2323 0d0a 0d0a 2a20 546f 6f6c 7320 7765  ##....* Tools we
+0000f2f0: 6273 6974 6520 3a20 5b68 7474 7073 3a2f  bsite : [https:/
+0000f300: 2f77 7777 2e6e 756e 6f62 7275 6d2e 636f  /www.nunobrum.co
+0000f310: 6d2f 7079 6c74 7370 6963 652e 6874 6d6c  m/pyltspice.html
+0000f320: 5d28 6874 7470 733a 2f2f 7777 772e 6e75  ](https://www.nu
+0000f330: 6e6f 6272 756d 2e63 6f6d 2f70 796c 7473  nobrum.com/pylts
+0000f340: 7069 6365 2e68 746d 6c29 0d0a 2a20 5265  pice.html)..* Re
+0000f350: 706f 206f 776e 6572 203a 205b 6d65 406e  po owner : [me@n
+0000f360: 756e 6f62 7275 6d2e 636f 6d5d 286d 6169  unobrum.com](mai
+0000f370: 6c74 6f3a 6d65 406e 756e 6f62 7275 6d2e  lto:me@nunobrum.
+0000f380: 636f 6d29 0d0a 2a20 416c 7465 726e 6174  com)..* Alternat
+0000f390: 6976 6520 636f 6e74 6163 7420 3a20 5b6e  ive contact : [n
+0000f3a0: 756e 6f2e 6272 756d 4067 6d61 696c 2e63  uno.brum@gmail.c
+0000f3b0: 6f6d 5d28 6d61 696c 746f 3a6e 756e 6f2e  om](mailto:nuno.
+0000f3c0: 6272 756d 4067 6d61 696c 2e63 6f6d 290d  brum@gmail.com).
+0000f3d0: 0a0d 0a23 2320 4869 7374 6f72 7920 2323  ...## History ##
+0000f3e0: 0d0a 2a20 5665 7273 696f 6e20 352e 332e  ..* Version 5.3.
+0000f3f0: 310d 0a20 202a 2042 7567 6669 7865 7320  1..  * Bugfixes 
+0000f400: 0d0a 2020 2020 2a20 5570 6461 7465 7320  ..    * Updates 
+0000f410: 6f6e 2074 6865 2052 4541 444d 452e 6d64  on the README.md
+0000f420: 2066 696c 652e 2049 7373 7565 2023 3133   file. Issue #13
+0000f430: 370d 0a20 2020 202a 2048 6965 7261 7263  7..    * Hierarc
+0000f440: 6869 6361 6c20 7375 7070 6f72 7420 6f6e  hical support on
+0000f450: 2041 7363 4564 6974 6f72 2e20 4973 7375   AscEditor. Issu
+0000f460: 6520 2331 3338 0d0a 2020 2a20 5269 6368  e #138..  * Rich
+0000f470: 2066 6f72 6d61 7420 6973 206f 6e6c 7920   format is only 
+0000f480: 7573 6564 2069 6620 7468 6520 7573 6572  used if the user
+0000f490: 2068 6173 2069 7420 616c 7265 6164 7920   has it already 
+0000f4a0: 696e 7374 616c 6c65 642e 2049 7373 7565  installed. Issue
+0000f4b0: 2023 3133 360d 0a2a 2056 6572 7369 6f6e   #136..* Version
+0000f4c0: 2035 2e33 2e30 0d0a 2020 2a20 4869 6572   5.3.0..  * Hier
+0000f4d0: 6172 6368 6963 616c 2053 7570 706f 7274  archical Support
+0000f4e0: 2028 416c 6967 6e69 6e67 2077 6974 6820   (Aligning with 
+0000f4f0: 7468 6520 7370 6963 656c 6962 2031 2e31  the spicelib 1.1
+0000f500: 2e31 290d 0a2a 2056 6572 7369 6f6e 2035  .1)..* Version 5
+0000f510: 2e32 2e33 0d0a 2020 2a20 5570 6461 7469  .2.3..  * Updati
+0000f520: 6e67 206c 6f67 6765 7273 2074 6f20 7573  ng loggers to us
+0000f530: 6520 7468 6520 2273 7069 6365 6c69 6222  e the "spicelib"
+0000f540: 2049 4473 2e0d 0a20 202a 2046 6978 696e   IDs...  * Fixin
+0000f550: 6720 6175 746f 646f 6320 6572 726f 7273  g autodoc errors
+0000f560: 0d0a 2020 2a20 436f 7272 6563 7469 6e67  ..  * Correcting
+0000f570: 2056 6572 7369 6f6e 2072 6566 6572 656e   Version referen
+0000f580: 6365 730d 0a0d 0a2a 2056 6572 7369 6f6e  ces....* Version
+0000f590: 2035 2e32 2e32 0d0a 2020 2a20 4669 7865   5.2.2..  * Fixe
+0000f5a0: 7320 6f6e 2074 6865 2075 6e69 7474 6573  s on the unittes
+0000f5b0: 7473 2061 6674 6572 2074 6865 2073 7069  ts after the spi
+0000f5c0: 6365 6c69 6220 7570 6461 7465 2074 6f20  celib update to 
+0000f5d0: 312e 302e 340d 0a0d 0a2a 2056 6572 7369  1.0.4....* Versi
+0000f5e0: 6f6e 2035 2e32 2e31 0d0a 2020 2a20 436f  on 5.2.1..  * Co
+0000f5f0: 7272 6563 7469 6f6e 206f 6e20 7468 6520  rrection on the 
+0000f600: 7275 6e5f 6d6f 6e74 6563 6172 6c6f 2e70  run_montecarlo.p
+0000f610: 7920 616e 6420 7275 6e5f 776f 7273 745f  y and run_worst_
+0000f620: 6361 7365 2e70 7920 6578 616d 706c 6573  case.py examples
+0000f630: 2e0d 0a20 202a 2046 6978 6573 206f 6e20  ...  * Fixes on 
+0000f640: 7468 6520 7370 6963 656c 6962 2028 5665  the spicelib (Ve
+0000f650: 7273 696f 6e20 312e 302e 3329 0d0a 0d0a  rsion 1.0.3)....
+0000f660: 2a20 5665 7273 696f 6e20 352e 320d 0a20  * Version 5.2.. 
+0000f670: 202a 2053 696d 416e 616c 7973 6973 2073   * SimAnalysis s
+0000f680: 7570 706f 7274 696e 6720 626f 7468 2051  upporting both Q
+0000f690: 7370 6963 6520 616e 6420 4c54 5370 6963  spice and LTSpic
+0000f6a0: 6520 6c6f 6766 696c 6573 2e0d 0a20 202a  e logfiles...  *
+0000f6b0: 2046 6173 7457 6f72 7374 4361 7365 416e   FastWorstCaseAn
+0000f6c0: 616c 7973 6973 2061 6c67 6f72 6974 686d  alysis algorithm
+0000f6d0: 2069 6d70 6c65 6d65 6e74 6564 0d0a 2020   implemented..  
+0000f6e0: 2a20 4669 7820 6f6e 2074 6865 206c 6f67  * Fix on the log
+0000f6f0: 2072 6561 6469 6e67 206f 6620 666f 7572   reading of four
+0000f700: 6965 7220 6461 7461 2e0d 0a0d 0a2a 2056  ier data.....* V
+0000f710: 6572 7369 6f6e 2035 2e31 0d0a 2020 2a20  ersion 5.1..  * 
+0000f720: 496d 706f 7274 616e 7420 4275 6766 6978  Important Bugfix
+0000f730: 206f 6e20 7468 6520 4c54 436f 6d70 6c65   on the LTComple
+0000f740: 7820 636c 6173 732e 0d0a 2020 2a20 4669  x class...  * Fi
+0000f750: 7865 7320 616e 6420 656e 6861 6e63 696e  xes and enhancin
+0000f760: 6720 7468 6520 616e 616c 7973 6973 2074  g the analysis t
+0000f770: 6f6f 6c6b 6974 2e0d 0a20 202a 2044 6570  oolkit...  * Dep
+0000f780: 7265 6361 7469 6e67 2053 7069 6365 4564  recating SpiceEd
+0000f790: 6974 6f72 2e77 7269 7465 5f6e 6574 6c69  itor.write_netli
+0000f7a0: 7374 2069 6e20 6661 766f 7572 206f 6620  st in favour of 
+0000f7b0: 7361 7665 5f6e 6574 6c69 7374 2829 0d0a  save_netlist()..
+0000f7c0: 0d0a 2a20 5665 7273 696f 6e20 352e 300d  ..* Version 5.0.
+0000f7d0: 0a20 202a 204d 616b 696e 6720 7468 6973  .  * Making this
+0000f7e0: 206c 6962 7261 7279 2064 6570 656e 6465   library depende
+0000f7f0: 6e74 206f 6e20 7370 6963 656c 6962 2077  nt on spicelib w
+0000f800: 6869 6c65 2074 7279 696e 6720 746f 206d  hile trying to m
+0000f810: 6169 6e74 6169 6e20 6261 636b 7761 7264  aintain backward
+0000f820: 2063 6f6d 7061 7469 6269 6c69 7479 2061   compatibility a
+0000f830: 7320 6d75 6368 2061 7320 706f 7373 6962  s much as possib
+0000f840: 6c65 2e20 0d0a 2020 5079 4c54 7370 6963  le. ..  PyLTspic
+0000f850: 6520 7769 6c6c 2062 6520 6b65 7074 2061  e will be kept a
+0000f860: 6c69 7665 2061 6e64 2069 7473 2075 7064  live and its upd
+0000f870: 6174 6520 7769 6c6c 2062 6520 6c69 6e6b  ate will be link
+0000f880: 6564 2074 6f20 7468 6520 7370 6963 656c  ed to the spicel
+0000f890: 6962 2e20 5468 6520 6d61 696e 2064 6966  ib. The main dif
+0000f8a0: 6665 7265 6e63 6520 6973 2074 6861 7420  ference is that 
+0000f8b0: 7573 696e 670d 0a20 2050 794c 5473 7069  using..  PyLTspi
+0000f8c0: 6365 2077 696c 6c20 6176 6572 7420 7468  ce will avert th
+0000f8d0: 6520 6e65 6564 206f 6620 6861 7669 6e67  e need of having
+0000f8e0: 2074 6f20 7365 6c65 6374 2061 2073 696d   to select a sim
+0000f8f0: 756c 6174 6f72 2069 6e20 616c 6c20 7275  ulator in all ru
+0000f900: 6e20 636f 6d6d 616e 6473 2e0d 0a0d 0a2a  n commands.....*
+0000f910: 2056 6572 7369 6f6e 2034 2e31 2e32 0d0a   Version 4.1.2..
+0000f920: 2020 2a20 4164 6469 6e67 2073 7570 706f    * Adding suppo
+0000f930: 7274 2066 6f72 2074 6865 206e 6577 2051  rt for the new Q
+0000f940: 5350 4943 4520 7369 6d75 6c61 746f 720d  SPICE simulator.
+0000f950: 0a20 202a 2049 6d70 726f 7669 6e67 2074  .  * Improving t
+0000f960: 6865 2074 696d 656f 7574 206d 6563 6861  he timeout mecha
+0000f970: 6e69 736d 206f 6e20 7468 6520 5369 6d52  nism on the SimR
+0000f980: 756e 6e65 7220 636c 6173 730d 0a20 202a  unner class..  *
+0000f990: 204d 696e 6f72 2062 7567 2066 6978 6573   Minor bug fixes
+0000f9a0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
+0000f9b0: 312e 310d 0a20 202a 2043 6f6d 706c 6574  1.1..  * Complet
+0000f9c0: 696e 6720 7468 6520 576f 7273 742d 4361  ing the Worst-Ca
+0000f9d0: 7365 2041 6e61 6c79 7369 7320 6675 6e63  se Analysis func
+0000f9e0: 7469 6f6e 732e 2041 6464 696e 6720 6120  tions. Adding a 
+0000f9f0: 6465 6469 6361 7465 6420 6578 616d 706c  dedicated exampl
+0000fa00: 6520 666f 7220 6974 2e0d 0a20 202a 2052  e for it...  * R
+0000fa10: 6566 6163 746f 7269 6e67 2074 6865 204c  efactoring the L
+0000fa20: 5453 7069 6365 4c6f 6752 6561 6465 7220  TSpiceLogReader 
+0000fa30: 636c 6173 7320 696e 206f 7264 6572 2074  class in order t
+0000fa40: 6f20 7573 6520 6974 206f 6e20 7468 6520  o use it on the 
+0000fa50: 416e 616c 7973 6973 2074 6f6f 6c6b 6974  Analysis toolkit
+0000fa60: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
+0000fa70: 312e 3020 2a28 7265 7175 6972 6573 2050  1.0 *(requires P
+0000fa80: 7974 686f 6e20 332e 3820 6f72 2068 6967  ython 3.8 or hig
+0000fa90: 6865 7229 2a0d 0a20 2020 202a 2041 6464  her)*..    * Add
+0000faa0: 696e 6720 6120 6e65 7720 636c 6173 7320  ing a new class 
+0000fab0: 746f 206d 616e 6970 756c 6174 6520 6469  to manipulate di
+0000fac0: 7265 6374 6c79 2074 6865 202e 6173 6320  rectly the .asc 
+0000fad0: 6669 6c65 732e 0d0a 2020 2020 2a20 4d6f  files...    * Mo
+0000fae0: 6469 6679 696e 6720 616c 6c20 7468 6520  difying all the 
+0000faf0: 6f74 6865 7220 636c 6173 7365 7320 696e  other classes in
+0000fb00: 206f 7264 6572 2074 6f20 7573 6520 7468   order to use th
+0000fb10: 6520 6e65 7720 636c 6173 732e 0d0a 2020  e new class...  
+0000fb20: 2020 2a20 4164 6469 6e67 2063 6c61 7373    * Adding class
+0000fb30: 6573 2074 6f20 7065 7266 6f72 6d20 4d6f  es to perform Mo
+0000fb40: 6e74 6563 6172 6c6f 2061 6e64 2077 6f72  ntecarlo and wor
+0000fb50: 7374 2063 6173 6520 616e 616c 7973 6973  st case analysis
+0000fb60: 2028 5468 616e 6b73 2074 6f20 406d 7661   (Thanks to @mva
+0000fb70: 6e72 6965 7420 666f 7220 6869 7320 7374  nriet for his st
+0000fb80: 6172 7469 6e67 2074 6869 7329 2e0d 0a20  arting this)... 
+0000fb90: 2020 202a 2052 656d 6f76 696e 6720 7468     * Removing th
+0000fba0: 6520 6465 7072 6563 6174 6564 204c 5453  e deprecated LTS
+0000fbb0: 7069 6365 5f52 6177 5265 6164 2e70 792c  pice_RawRead.py,
+0000fbc0: 204c 5453 7069 6365 5f52 6177 5772 6974   LTSpice_RawWrit
+0000fbd0: 652e 7079 2061 6e64 204c 5453 7069 6365  e.py and LTSpice
+0000fbe0: 4261 7463 682e 7079 2066 696c 6573 2061  Batch.py files a
+0000fbf0: 6e64 2072 6573 7065 6374 6976 6520 636c  nd respective cl
+0000fc00: 6173 7365 732e 0d0a 2020 2020 2a20 5265  asses...    * Re
+0000fc10: 7374 7275 6374 7572 6564 2074 6865 2066  structured the f
+0000fc20: 6f6c 6465 7220 7374 7275 6374 7572 6520  older structure 
+0000fc30: 746f 2062 6520 6d6f 7265 2069 6e20 6c69  to be more in li
+0000fc40: 6e65 2077 6974 6820 7468 6520 5079 7468  ne with the Pyth
+0000fc50: 6f6e 2073 7461 6e64 6172 6473 2e0d 0a20  on standards... 
+0000fc60: 2020 202a 2041 6464 6564 2061 6e20 4578     * Added an Ex
+0000fc70: 616d 706c 6573 2066 6f6c 6465 7220 7769  amples folder wi
+0000fc80: 7468 2073 6f6d 6520 6578 616d 706c 6573  th some examples
+0000fc90: 206f 6e20 686f 7720 746f 2075 7365 2074   on how to use t
+0000fca0: 6865 206c 6962 7261 7279 2e0d 0a0d 0a2a  he library.....*
+0000fcb0: 2056 6572 7369 6f6e 2034 2e30 2e36 0d0a   Version 4.0.6..
+0000fcc0: 2020 2020 2a20 4669 7869 6e67 2069 7373      * Fixing iss
+0000fcd0: 7565 2077 6974 6820 7468 6520 7772 6974  ue with the writ
+0000fce0: 655f 6e65 746c 6973 7428 2920 6675 6e63  e_netlist() func
+0000fcf0: 7469 6f6e 2077 6865 6e20 7265 6365 6976  tion when receiv
+0000fd00: 696e 6720 6120 7374 7269 6e67 2069 6e73  ing a string ins
+0000fd10: 7465 6164 206f 6620 6120 7061 7468 6c69  tead of a pathli
+0000fd20: 622e 5061 7468 206f 626a 6563 742e 0d0a  b.Path object...
+0000fd30: 2020 2020 2a20 4368 616e 6769 6e67 2074      * Changing t
+0000fd40: 6865 2072 6567 756c 6172 2065 7870 7265  he regular expre
+0000fd50: 7373 696f 6e20 666f 7220 7468 6520 7265  ssion for the re
+0000fd60: 7369 7374 6f72 2069 6e20 6f72 6465 7220  sistor in order 
+0000fd70: 746f 2061 6363 6570 7420 7468 6520 523d  to accept the R=
+0000fd80: 2070 7265 6669 7820 6f6e 2074 6865 2076   prefix on the v
+0000fd90: 616c 7565 732e 0d0a 0d0a 2a20 5665 7273  alues.....* Vers
+0000fda0: 696f 6e20 342e 302e 350d 0a20 2020 202a  ion 4.0.5..    *
+0000fdb0: 2041 6363 6570 7469 6e67 2066 6978 6573   Accepting fixes
+0000fdc0: 2066 726f 6d20 6161 6e61 732d 7361 7965   from aanas-saye
+0000fdd0: 6440 4769 7448 7562 2074 6861 7420 6669  d@GitHub that fi
+0000fde0: 7865 7320 6973 7375 6573 2077 6974 6820  xes issues with 
+0000fdf0: 7275 6e6e 696e 6720 7468 6520 4c54 5370  running the LTSp
+0000fe00: 6963 6520 696e 204c 696e 7578 2e0d 0a0d  ice in Linux....
+0000fe10: 0a2a 2056 6572 7369 6f6e 2034 2e30 2e34  .* Version 4.0.4
+0000fe20: 0d0a 2020 2020 2a20 496d 7072 6f76 6564  ..    * Improved
+0000fe30: 2075 7361 6765 206f 6620 7468 6520 6c6f   usage of the lo
+0000fe40: 6767 696e 6720 6c69 6272 6172 792e 2028  gging library. (
+0000fe50: 5468 616e 6b73 2040 5453 7072 6563 6820  Thanks @TSprech 
+0000fe60: 666f 7220 7661 7374 6c79 2069 6d70 726f  for vastly impro
+0000fe70: 7669 6e67 2074 6865 206c 6f67 6769 6e67  ving the logging
+0000fe80: 290d 0a20 2020 202a 2049 6e63 6c75 6465  )..    * Include
+0000fe90: 6420 5275 6e54 6173 6b20 6e75 6d62 6572  d RunTask number
+0000fea0: 2069 6e20 7468 6520 6c6f 6720 6d65 7373   in the log mess
+0000feb0: 6167 6573 2e0d 0a20 2020 202a 2049 6e63  ages...    * Inc
+0000fec0: 6c75 6465 6420 6d69 6c6c 6973 6563 6f6e  luded millisecon
+0000fed0: 6473 2069 6e20 7468 6520 7469 6d65 2065  ds in the time e
+0000fee0: 6c61 7073 6564 2063 616c 6375 6c61 7469  lapsed calculati
+0000fef0: 6f6e 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  on.....* Version
+0000ff00: 2034 2e30 2e33 0d0a 2020 2020 2a20 4669   4.0.3..    * Fi
+0000ff10: 7869 6e67 2069 7373 7565 2069 6e20 656c  xing issue in el
+0000ff20: 6170 7365 6420 7469 6d65 2063 616c 6375  apsed time calcu
+0000ff30: 6c61 7469 6f6e 2e0d 0a20 2020 202a 2046  lation...    * F
+0000ff40: 6978 696e 6720 6973 7375 6520 7769 7468  ixing issue with
+0000ff50: 2074 6865 2069 6d70 6f72 7420 6f66 204c   the import of L
+0000ff60: 5453 7069 6365 4c6f 6752 6561 6465 7220  TSpiceLogReader 
+0000ff70: 6672 6f6d 204c 5453 7465 7073 2e70 790d  from LTSteps.py.
+0000ff80: 0a0d 0a2a 2056 6572 7369 6f6e 2034 2e30  ...* Version 4.0
+0000ff90: 2e32 0d0a 2020 2020 2a20 4368 616e 6769  .2..    * Changi
+0000ffa0: 6e67 206c 6973 7420 6f66 204c 6962 7261  ng list of Libra
+0000ffb0: 7279 2064 6570 656e 6465 6e63 6965 732e  ry dependencies.
+0000ffc0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
+0000ffd0: 302e 310d 0a20 2020 202a 2042 7567 2066  0.1..    * Bug f
+0000ffe0: 6978 206f 6e20 434c 4920 666f 7220 7468  ix on CLI for th
+0000fff0: 6520 4869 7374 6f67 7261 6d2e 7079 2061  e Histogram.py a
+00010000: 6e64 204c 5453 7465 7073 2e70 790d 0a0d  nd LTSteps.py...
+00010010: 0a2a 2056 6572 7369 6f6e 2034 2e30 2e30  .* Version 4.0.0
+00010020: 0d0a 2020 2020 2a20 5365 7061 7261 7469  ..    * Separati
+00010030: 6e67 2074 6865 2053 696d 436f 6d6d 616e  ng the SimComman
+00010040: 6465 7220 696e 746f 2074 776f 2073 6570  der into two sep
+00010050: 6172 6174 6520 636c 6173 7365 732c 206f  arate classes, o
+00010060: 6e65 2066 6f72 2074 6865 2073 7069 6365  ne for the spice
+00010070: 206e 6574 6c69 7374 2065 6469 7469 6e67   netlist editing
+00010080: 2028 5370 6963 6545 6469 746f 7229 2061   (SpiceEditor) a
+00010090: 6e64 2061 6e6f 7468 6572 0d0a 2020 2020  nd another..    
+000100a0: 2020 666f 7220 7468 6520 7369 6d75 6c61    for the simula
+000100b0: 7469 6f6e 2065 7865 6375 7469 6f6e 2028  tion execution (
+000100c0: 5369 6d52 756e 6e65 7229 2e0d 0a20 2020  SimRunner)...   
+000100d0: 202a 2049 6d70 6c65 6d65 6e74 696e 6720   * Implementing 
+000100e0: 7369 6d75 6c61 7469 6f6e 2073 6572 7665  simulation serve
+000100f0: 7220 746f 2061 6c6c 6f77 2066 6f72 2072  r to allow for r
+00010100: 656d 6f74 6520 7369 6d75 6c61 7469 6f6e  emote simulation
+00010110: 2065 7865 6375 7469 6f6e 2061 6e64 2074   execution and t
+00010120: 6865 2072 6573 7065 6374 6976 6520 636c  he respective cl
+00010130: 6965 6e74 2e0d 0a20 2020 202a 2053 7570  ient...    * Sup
+00010140: 706f 7274 696e 6720 5769 6767 6c65 7220  porting Wiggler 
+00010150: 656c 656d 656e 7420 696e 2074 6865 206e  element in the n
+00010160: 6577 204c 5453 7069 6365 5856 4949 2e0d  ew LTSpiceXVII..
+00010170: 0a20 2020 202a 2052 656e 616d 696e 6720  .    * Renaming 
+00010180: 616c 6c20 6669 6c65 7320 696e 746f 206c  all files into l
+00010190: 6f77 6572 6361 7365 2e0d 0a20 2020 202a  owercase...    *
+000101a0: 2043 7265 6174 696e 6720 4572 726f 7220   Creating Error 
+000101b0: 636c 6173 7365 7320 666f 7220 6265 7474  classes for bett
+000101c0: 6572 2065 7272 6f72 2068 616e 646c 696e  er error handlin
+000101d0: 672e 0d0a 2020 2020 2a20 4164 6469 6e67  g...    * Adding
+000101e0: 2073 7570 706f 7274 2066 6f72 206f 7468   support for oth
+000101f0: 6572 2073 696d 756c 6174 6f72 7320 2865  er simulators (e
+00010200: 783a 206e 6773 7069 6365 2920 7768 6572  x: ngspice) wher
+00010210: 6520 7468 6520 7369 6d75 6c61 746f 7220  e the simulator 
+00010220: 6973 2064 6566 696e 6564 2062 7920 6120  is defined by a 
+00010230: 636c 6173 732e 2054 6869 730d 0a20 2020  class. This..   
+00010240: 2020 2073 7570 706f 7274 2063 6c61 7373     support class
+00010250: 206e 6565 6473 2074 6f20 6265 2061 2073   needs to be a s
+00010260: 7562 636c 6173 7320 6f66 2074 6865 2061  ubclass of the a
+00010270: 6273 7472 6163 7420 636c 6173 7320 5369  bstract class Si
+00010280: 6d75 6c61 746f 722e 0d0a 2020 2020 2a20  mulator...    * 
+00010290: 456e 6f72 6d6f 7573 2069 6d70 726f 7665  Enormous improve
+000102a0: 6d65 6e74 2069 6e20 7468 6520 646f 6375  ment in the docu
+000102b0: 6d65 6e74 6174 696f 6e20 6f66 2074 6865  mentation of the
+000102c0: 2063 6f64 652e 0d0a 0d0a 2a20 5665 7273   code.....* Vers
+000102d0: 696f 6e20 332e 300d 0a20 2020 202a 2045  ion 3.0..    * E
+000102e0: 6c69 6d69 6e61 7469 6e67 2074 6865 204c  liminating the L
+000102f0: 5453 7069 6365 2070 7265 6669 7865 7320  TSpice prefixes 
+00010300: 6672 6f6d 2066 696c 6573 2061 6e64 2063  from files and c
+00010310: 6c61 7373 6573 2e0d 0a20 2020 202a 2041  lasses...    * A
+00010320: 646f 7074 696e 6720 7468 6520 6c6f 7765  dopting the lowe
+00010330: 7263 6173 6520 636f 6e76 656e 7469 6f6e  rcase convention
+00010340: 2066 6f72 2066 696c 656e 616d 6573 2e0d   for filenames..
+00010350: 0a0d 0a2a 2056 6572 7369 6f6e 2032 2e33  ...* Version 2.3
+00010360: 2e31 0d0a 2020 2020 2a20 4275 6720 6669  .1..    * Bug fi
+00010370: 7820 6f6e 2074 6865 2070 6172 616d 6574  x on the paramet
+00010380: 6572 2072 6570 6c61 6365 6d65 6e74 2e0d  er replacement..
+00010390: 0a0d 0a2a 2056 6572 7369 6f6e 2032 2e33  ...* Version 2.3
+000103a0: 0d0a 2020 2020 2a20 5375 7070 6f72 7469  ..    * Supporti
+000103b0: 6e67 2074 6865 2063 7265 6174 696f 6e20  ng the creation 
+000103c0: 6f66 2052 4157 204e 6f69 7365 2041 6e61  of RAW Noise Ana
+000103d0: 6c79 7369 730d 0a20 2020 202a 2042 7567  lysis..    * Bug
+000103e0: 2046 6978 6573 2028 5365 6520 4769 7448   Fixes (See GitH
+000103f0: 7562 204c 6f67 290d 0a0d 0a2a 2056 6572  ub Log)....* Ver
+00010400: 7369 6f6e 2032 2e32 0d0a 2020 2020 2a20  sion 2.2..    * 
+00010410: 4d61 6b69 6e67 206e 756d 7079 2061 7320  Making numpy as 
+00010420: 6120 7265 7175 6972 656d 656e 7420 616e  a requirement an
+00010430: 6420 656c 696d 696e 6174 696e 6720 616c  d eliminating al
+00010440: 6c20 636f 6465 2074 6861 7420 6176 6f69  l code that avoi
+00010450: 6465 6420 7468 6520 7573 6520 6f66 206e  ded the use of n
+00010460: 756d 7079 0d0a 2020 2020 2a20 5573 696e  umpy..    * Usin
+00010470: 6720 6e65 7720 7061 636b 6167 696e 6720  g new packaging 
+00010480: 746f 6f6c 0d0a 2020 2020 2a20 4669 7865  tool..    * Fixe
+00010490: 7320 6f6e 2074 6865 204c 5453 7069 6365  s on the LTSpice
+000104a0: 5f52 6177 5772 6974 650d 0a20 2020 202a  _RawWrite..    *
+000104b0: 2046 6978 6573 2069 6e20 7468 6520 6861   Fixes in the ha
+000104c0: 6e64 6c69 6e67 206f 6620 7374 6570 7065  ndling of steppe
+000104d0: 6420 6f70 6572 6174 696e 6720 706f 696e  d operating poin
+000104e0: 7420 7369 6d75 6c61 7469 6f6e 730d 0a0d  t simulations...
+000104f0: 0a2a 2056 6572 7369 6f6e 2032 2e31 0d0a  .* Version 2.1..
+00010500: 2020 2020 2a20 4164 6f70 7469 6e67 206d      * Adopting m
+00010510: 696e 696d 756d 2070 7974 686f 6e20 7665  inimum python ve
+00010520: 7273 696f 6e20 332e 370d 0a20 2020 202a  rsion 3.7..    *
+00010530: 2053 7461 7274 696e 6720 746f 2075 7365   Starting to use
+00010540: 2075 6e69 7420 7465 7374 7320 746f 2076   unit tests to v
+00010550: 616c 6964 6174 6520 616c 6c20 6d6f 6475  alidate all modu
+00010560: 6c65 7320 616e 6420 696d 7072 6f76 696e  les and improvin
+00010570: 6720 7465 7374 6265 6e63 6865 730d 0a20  g testbenches.. 
+00010580: 2020 202a 2043 6f6d 7061 7469 6269 6c69     * Compatibili
+00010590: 7479 2077 6974 6820 4e47 5370 6963 650d  ty with NGSpice.
+000105a0: 0a20 2020 202a 2041 766f 6964 696e 6720  .    * Avoiding 
+000105b0: 7468 6520 7573 6520 6f66 2073 6574 7570  the use of setup
+000105c0: 2e70 7920 6173 2070 6572 2050 4550 3531  .py as per PEP51
+000105d0: 3720 616e 6420 5045 5035 3138 0d0a 2020  7 and PEP518..  
+000105e0: 2020 2a20 4275 6720 4669 7865 7320 2853    * Bug Fixes (S
+000105f0: 6565 2047 6974 4875 6220 6c6f 6720 666f  ee GitHub log fo
+00010600: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+00010610: 6f6e 290d 0a20 2020 202a 2049 6d70 726f  on)..    * Impro
+00010620: 7665 6d65 6e74 7320 6f6e 2074 6865 206d  vements on the m
+00010630: 616e 6167 656d 656e 7420 6f66 2073 7465  anagement of ste
+00010640: 7070 6564 2064 6174 6120 696e 2074 6865  pped data in the
+00010650: 204c 5453 7069 6365 5f52 6177 5265 6164   LTSpice_RawRead
+00010660: 2e70 790d 0a0d 0a2a 2056 6572 7369 6f6e  .py....* Version
+00010670: 2032 2e30 2e32 0d0a 2020 2020 2a20 496d   2.0.2..    * Im
+00010680: 7072 6f76 656d 656e 7473 206f 6e20 456e  provements on En
+00010690: 636f 6469 6e67 2064 6574 6563 7469 6f6e  coding detection
+000106a0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 322e  ....* Version 2.
+000106b0: 300d 0a20 2020 202a 2049 6e74 6572 6e61  0..    * Interna
+000106c0: 7469 6f6e 616c 2053 7570 706f 7274 2075  tional Support u
+000106d0: 7369 6e67 2074 6865 2063 6f72 7265 6374  sing the correct
+000106e0: 2065 6e63 6f64 696e 6720 7768 656e 206c   encoding when l
+000106f0: 6f61 6469 6e67 206c 6f67 2066 696c 6573  oading log files
+00010700: 2e0d 0a20 2020 202a 2043 6f64 6520 4f70  ...    * Code Op
+00010710: 7469 6d69 7a61 7469 6f6e 7320 6f6e 2074  timizations on t
+00010720: 6865 204c 5453 7069 6365 5f52 6177 5265  he LTSpice_RawRe
+00010730: 6164 6572 2074 6861 7420 616c 6c6f 7720  ader that allow 
+00010740: 6661 7374 6572 2064 6174 6120 6c6f 6164  faster data load
+00010750: 696e 672e 0d0a 2020 2020 2a20 496d 7072  ing...    * Impr
+00010760: 6f76 696e 6720 7468 6520 6675 6e63 7469  oving the functi
+00010770: 6f6e 616c 6974 7920 6f6e 2074 6865 204c  onality on the L
+00010780: 5453 7069 6365 5f52 6177 5772 6974 6572  TSpice_RawWriter
+00010790: 2e70 790d 0a20 2020 202a 2041 6464 696e  .py..    * Addin
+000107a0: 6720 7375 7070 6f72 7420 746f 2065 6469  g support to edi
+000107b0: 7469 6e67 2063 6f6d 706f 6e65 6e74 7320  ting components 
+000107c0: 696e 7369 6465 2073 7562 6369 7263 7569  inside subcircui
+000107d0: 7473 2028 2e73 7562 636b 7429 0d0a 2020  ts (.subckt)..  
+000107e0: 2020 2a20 5375 7070 6f72 7469 6e67 2072    * Supporting r
+000107f0: 6573 6973 746f 7273 2077 6974 6820 4d6f  esistors with Mo
+00010800: 6465 6c20 4465 6669 6e69 7469 6f6e 730d  del Definitions.
+00010810: 0a20 2020 202a 2046 6978 696e 6720 7072  .    * Fixing pr
+00010820: 6f62 6c65 6d20 7769 7468 204c 5453 7069  oblem with LTSpi
+00010830: 6365 4c6f 6752 6561 6465 7220 7468 6174  ceLogReader that
+00010840: 2077 6f75 6c64 2072 6574 7572 6e20 6d65   would return me
+00010850: 7373 6564 2075 7020 6461 7461 0d0a 2020  ssed up data..  
+00010860: 2020 2a20 4669 7869 6e67 2070 726f 626c    * Fixing probl
+00010870: 656d 2077 6974 6820 7265 706c 6163 696e  em with replacin
+00010880: 6720 7468 6520 6669 6c65 2065 7874 656e  g the file exten
+00010890: 7369 6f6e 2069 6e20 6365 7274 6169 6e20  sion in certain 
+000108a0: 6e61 6d65 730d 0a20 2020 202a 2043 6f72  names..    * Cor
+000108b0: 7265 6374 696e 6720 7072 6f62 6c65 6d20  recting problem 
+000108c0: 7769 7468 2064 6570 7265 6361 7469 6f6e  with deprecation
+000108d0: 7320 6f6e 2074 6865 206e 756d 7079 2066  s on the numpy f
+000108e0: 756e 6374 696f 6e73 2075 7365 6420 6279  unctions used by
+000108f0: 2074 6865 2048 6973 746f 6772 616d 2e70   the Histogram.p
+00010900: 790d 0a20 2020 202a 2041 6464 696e 6720  y..    * Adding 
+00010910: 6261 636b 2074 6865 2052 4541 444d 452e  back the README.
+00010920: 6d64 2074 6861 7420 736f 6d65 686f 7720  md that somehow 
+00010930: 7761 7320 6465 6c65 7465 640d 0a0d 0a2a  was deleted....*
+00010940: 2056 6572 7369 6f6e 2031 2e39 0d0a 2020   Version 1.9..  
+00010950: 2020 2a20 4164 6469 6e67 2073 7570 706f    * Adding suppo
+00010960: 7274 2066 6f72 20c2 b520 6368 6172 6163  rt for .. charac
+00010970: 7465 7220 696e 2074 6865 2053 7069 6365  ter in the Spice
+00010980: 4564 6974 6f72 2e0d 0a20 2020 202a 2041  Editor...    * A
+00010990: 6464 696e 6720 6765 745f 636f 6d70 6f6e  dding get_compon
+000109a0: 656e 745f 666c 6f61 7476 616c 7565 2829  ent_floatvalue()
+000109b0: 206d 6574 686f 6420 696e 2074 6865 206e   method in the n
+000109c0: 6574 6c69 7374 206d 616e 6970 756c 6174  etlist manipulat
+000109d0: 696e 6720 636c 6173 7320 7468 6174 2068  ing class that h
+000109e0: 616e 646c 6573 2074 6865 2063 6f6e 7665  andles the conve
+000109f0: 7273 696f 6e20 6f66 206e 756d 6572 6963  rsion of numeric
+00010a00: 0d0a 2020 2020 2020 6669 656c 6473 2069  ..      fields i
+00010a10: 6e74 6f20 6120 666c 6f61 742e 2054 6869  nto a float. Thi
+00010a20: 7320 6675 6e63 7469 6f6e 2074 616b 6573  s function takes
+00010a30: 2069 6e74 6f20 6163 636f 756e 7420 7468   into account th
+00010a40: 6520 656e 6769 6e65 6572 696e 6720 7175  e engineering qu
+00010a50: 616c 6966 6965 7273 2027 6b27 2066 6f72  alifiers 'k' for
+00010a60: 206b 696c 6f73 2c20 276d 2720 6f72 206d   kilos, 'm' or m
+00010a70: 696c 6973 2c0d 0a20 2020 2020 2027 7527  ilis,..      'u'
+00010a80: 206f 7220 27c2 b527 2066 6f72 206d 6963   or '..' for mic
+00010a90: 726f 6e73 2c20 276e 2720 666f 7220 6e61  rons, 'n' for na
+00010aa0: 6e6f 732c 2027 6627 2066 6f72 2066 656d  nos, 'f' for fem
+00010ab0: 746f 7320 616e 6420 274d 6567 2720 666f  tos and 'Meg' fo
+00010ac0: 7220 4d65 6761 732e 0d0a 0d0a 2a20 5665  r Megas.....* Ve
+00010ad0: 7273 696f 6e20 312e 380d 0a20 2020 202a  rsion 1.8..    *
+00010ae0: 2055 6e69 666f 726d 696e 6720 4c69 6365   Uniforming Lice
+00010af0: 6e73 6520 7265 6665 7265 6e63 6520 6163  nse reference ac
+00010b00: 726f 7373 2066 696c 6573 2061 6e64 2069  ross files and i
+00010b10: 6d70 726f 7665 6d65 6e74 7320 6f6e 2074  mprovements on t
+00010b20: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00010b30: 0d0a 2020 2020 2a20 416e 2065 6e6f 726d  ..    * An enorm
+00010b40: 6f75 7320 616e 6420 7768 6f6c 6568 6561  ous and wholehea
+00010b50: 7274 6564 2074 6861 6e6b 7320 746f 2040  rted thanks to @
+00010b60: 6c70 6865 7272 2066 6f72 2074 6865 2069  lpherr for the i
+00010b70: 6d70 726f 7665 6d65 6e74 7320 696e 2074  mprovements in t
+00010b80: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00010b90: 2e0d 0a20 2020 202a 2042 7567 6669 7820  ...    * Bugfix 
+00010ba0: 6f6e 2074 6865 2061 6464 5f4c 5473 7069  on the add_LTspi
+00010bb0: 6365 5275 6e43 6d64 4c69 6e65 5377 6974  ceRunCmdLineSwit
+00010bc0: 6368 6573 2829 203b 2053 7570 706f 7274  ches() ; Support
+00010bd0: 696e 6720 2e70 6172 616d 206e 616d 6520  ing .param name 
+00010be0: 7661 6c75 6520 666f 726d 6174 0d0a 2020  value format..  
+00010bf0: 2020 2a20 416c 6c6f 7769 6e67 2074 6865    * Allowing the
+00010c00: 204c 5453 7069 6365 5261 7752 6561 6420   LTSpiceRawRead 
+00010c10: 746f 2070 726f 6365 6564 2077 6865 6e20  to proceed when 
+00010c20: 7468 6520 6c6f 6720 6669 6c65 2063 616e  the log file can
+00010c30: 2774 2062 6520 666f 756e 6420 6f72 2077  't be found or w
+00010c40: 6865 6e20 7468 6572 6520 6172 6520 7072  hen there are pr
+00010c50: 6f62 6c65 6d73 2072 6561 6469 6e67 2069  oblems reading i
+00010c60: 742e 0d0a 2a20 5665 7273 696f 6e20 312e  t...* Version 1.
+00010c70: 370d 0a20 2020 202a 2052 756e 6e69 6e67  7..    * Running
+00010c80: 2069 6e20 4c69 6e75 7820 756e 6465 7220   in Linux under 
+00010c90: 7769 6e65 2069 7320 6e6f 7720 706f 7373  wine is now poss
+00010ca0: 6962 6c65 0d0a 0d0a 2a20 5665 7273 696f  ible....* Versio
+00010cb0: 6e20 312e 360d 0a20 2020 202a 2041 6464  n 1.6..    * Add
+00010cc0: 696e 6720 4c54 5370 6963 655f 5261 7757  ing LTSpice_RawW
+00010cd0: 7269 7465 2e20 4164 6469 6e67 2064 6f63  rite. Adding doc
+00010ce0: 756d 656e 7461 7469 6f6e 2e0d 0a0d 0a2a  umentation.....*
+00010cf0: 2056 6572 7369 6f6e 2031 2e35 0d0a 2020   Version 1.5..  
+00010d00: 2020 2a20 536d 616c 6c20 6669 7865 7320    * Small fixes 
+00010d10: 616e 6420 696d 7072 6f76 656d 656e 7473  and improvements
+00010d20: 206f 6e20 7468 6520 636c 6173 7320 7573   on the class us
+00010d30: 6167 652e 204e 6f20 6164 6465 6420 6665  age. No added fe
+00010d40: 6174 7572 6573 0d0a 0d0a 2a20 5665 7273  atures....* Vers
+00010d50: 696f 6e20 312e 340d 0a20 2020 202a 2041  ion 1.4..    * A
+00010d60: 6464 696e 6720 7468 6520 4c54 5370 6963  dding the LTSpic
+00010d70: 655f 5365 6d69 4465 764f 7052 6561 6465  e_SemiDevOpReade
+00010d80: 7220 6d6f 6475 6c65 0d0a 2020 2020 2a20  r module..    * 
+00010d90: 5265 2d65 6e61 626c 696e 6720 7468 6520  Re-enabling the 
+00010da0: 4869 7374 6f67 7261 6d20 6675 6e63 7469  Histogram functi
+00010db0: 6f6e 7320 7768 6963 6820 7768 6572 6520  ons which where 
+00010dc0: 6469 7361 626c 6564 2062 7920 6d69 7374  disabled by mist
+00010dd0: 616b 652e 0d0a 0d0a 2a20 5665 7273 696f  ake.....* Versio
+00010de0: 6e20 312e 330d 0a20 2020 202a 2042 7567  n 1.3..    * Bug
+00010df0: 2066 6978 6573 206f 6e20 7468 6520 5370   fixes on the Sp
+00010e00: 6963 6545 6469 746f 7220 436c 6173 730d  iceEditor Class.
+00010e10: 0a0d 0a2a 2056 6572 7369 6f6e 2031 2e32  ...* Version 1.2
+00010e20: 0d0a 2020 2020 2a20 5245 4144 4d45 2e6d  ..    * README.m
+00010e30: 643a 0d0a 2020 2020 2020 4164 6469 6e67  d:..      Adding
+00010e40: 206c 696e 6b20 746f 2072 6561 6474 6865   link to readthe
+00010e50: 646f 6373 2064 6f63 756d 656e 7461 7469  docs documentati
+00010e60: 6f6e 0d0a 2020 2020 2a20 416c 6c20 6669  on..    * All fi
+00010e70: 6c65 733a 0d0a 2020 2020 2020 436f 6d70  les:..      Comp
+00010e80: 7265 6865 6e73 6976 6520 646f 6375 6d65  rehensive docume
+00010e90: 6e74 6174 696f 6e20 6f6e 2068 6f77 2074  ntation on how t
+00010ea0: 6f20 7573 6520 6561 6368 206d 6f64 756c  o use each modul
+00010eb0: 650d 0a0d 0a2a 2056 6572 7369 6f6e 2031  e....* Version 1
+00010ec0: 2e31 0d0a 2020 2020 2a20 5245 4144 4d45  .1..    * README
+00010ed0: 2e6d 643a 0d0a 2020 2020 2020 5570 6461  .md:..      Upda
+00010ee0: 7465 6420 7468 6520 6465 7363 7269 7074  ted the descript
+00010ef0: 696f 6e0d 0a20 2020 202a 204c 5453 7069  ion..    * LTSpi
+00010f00: 6365 4261 7463 682e 7079 3a0d 0a20 2020  ceBatch.py:..   
+00010f10: 2020 2043 6f72 7265 6374 6564 2074 6865     Corrected the
+00010f20: 206e 616d 6520 6f66 2074 6865 2072 6574   name of the ret
+00010f30: 7572 6e65 6420 7261 7720 6669 6c65 2e0d  urned raw file..
+00010f40: 0a20 2020 202a 2041 6464 6564 2063 6f6d  .    * Added com
+00010f50: 6d65 6e74 7320 7468 726f 7567 686f 7574  ments throughout
+00010f60: 2074 6865 2063 6f64 6520 616e 6420 636c   the code and cl
+00010f70: 6561 6e75 700d 0a0d 0a2a 2056 6572 7369  eanup....* Versi
+00010f80: 6f6e 2031 2e30 0d0a 2020 2020 2a20 4c54  on 1.0..    * LT
+00010f90: 5370 6963 6542 6174 6368 2e70 793a 5c0d  SpiceBatch.py:\.
+00010fa0: 0a20 2020 2020 2049 6d70 6c65 6d65 6e74  .      Implement
+00010fb0: 6564 2061 206e 6577 2061 7070 726f 6163  ed a new approac
+00010fc0: 6820 284e 4f54 2042 4143 4b57 4152 4453  h (NOT BACKWARDS
+00010fd0: 2043 4f4d 5041 5449 424c 4529 2c20 7468   COMPATIBLE), th
+00010fe0: 6174 2061 766f 6964 7320 7468 6520 7573  at avoids the us
+00010ff0: 6167 6520 6f66 2074 6865 2073 696d 5f73  age of the sim_s
+00011000: 6574 7469 6e67 732e 696e 6320 6669 6c65  ettings.inc file
+00011010: 2e0d 0a20 2020 2020 2041 6e64 2061 6c6c  ...      And all
+00011020: 6f77 7320 746f 206d 6f64 6966 7920 6e6f  ows to modify no
+00011030: 7420 6f6e 6c79 2070 6172 616d 6574 6572  t only parameter
+00011040: 732c 2062 7574 2061 6c73 6f20 6d6f 6465  s, but also mode
+00011050: 6c73 2061 6e64 2065 7665 6e20 7468 6520  ls and even the 
+00011060: 7369 6d75 6c61 7469 6f6e 2063 6f6d 6d61  simulation comma
+00011070: 6e64 732e 0d0a 2020 2020 2a20 4c54 5370  nds...    * LTSp
+00011080: 6963 655f 5261 7752 6561 642e 7079 3a5c  ice_RawRead.py:\
+00011090: 0d0a 2020 2020 2020 4164 6465 6420 7468  ..      Added th
+000110a0: 6520 6765 745f 7469 6d65 5f61 7869 7320  e get_time_axis 
+000110b0: 6d65 7468 6f64 2074 6f20 7468 6520 5261  method to the Ra
+000110c0: 7752 6561 6420 636c 6173 7320 746f 2061  wRead class to a
+000110d0: 766f 6964 2074 6865 2070 726f 626c 656d  void the problem
+000110e0: 7320 7769 7468 206e 6567 6174 6976 6520  s with negative 
+000110f0: 7661 6c75 6573 206f 6e20 7469 6d65 2061  values on time a
+00011100: 7869 732c 0d0a 2020 2020 2020 7768 656e  xis,..      when
+00011110: 2032 6e64 206f 7264 6572 2063 6f6d 7072   2nd order compr
+00011120: 6573 7369 6f6e 2069 7320 656e 6162 6c65  ession is enable
+00011130: 6420 696e 204c 5453 7069 6365 2e0d 0a20  d in LTSpice... 
+00011140: 2020 202a 204c 5453 7465 7073 2e70 793a     * LTSteps.py:
+00011150: 5c0d 0a20 2020 2020 204d 6f64 6966 6965  \..      Modifie
+00011160: 6420 7468 6520 4c54 5374 6570 732c 2073  d the LTSteps, s
+00011170: 6f20 6974 2063 616e 2061 6c73 6f20 7265  o it can also re
+00011180: 6164 206d 6561 7375 7265 6d65 6e74 7320  ad measurements 
+00011190: 6f6e 206c 6f67 2066 696c 6573 2077 6974  on log files wit
+000111a0: 686f 7574 2061 6e79 2073 7465 7073 2064  hout any steps d
+000111b0: 6f6e 652e 0d0a 0d0a 2a20 5665 7273 696f  one.....* Versio
+000111c0: 6e20 302e 360d 0a20 202a 2048 6973 746f  n 0.6..  * Histo
+000111d0: 6772 616d 2e70 7920 6e6f 7720 6861 7320  gram.py now has 
+000111e0: 616e 206f 7074 696f 6e20 746f 206d 616b  an option to mak
+000111f0: 6520 7468 6520 6869 7374 6f67 7261 6d20  e the histogram 
+00011200: 6469 7265 6374 6c79 2066 726f 6d20 7661  directly from va
+00011210: 6c75 6573 2073 746f 7265 6420 696e 2074  lues stored in t
+00011220: 6865 2063 6c69 7062 6f61 7264 0d0a 0d0a  he clipboard....
+00011230: 2a20 5665 7273 696f 6e20 302e 350d 0a20  * Version 0.5.. 
+00011240: 202a 2054 6865 204c 5453 7069 6365 5f52   * The LTSpice_R
+00011250: 6177 5265 6164 6572 2e70 7920 6e6f 7720  awReader.py now 
+00011260: 7573 6573 2074 6865 2060 7374 7275 6374  uses the `struct
+00011270: 2e75 6e70 6163 6b60 2066 756e 6374 696f  .unpack` functio
+00011280: 6e20 666f 7220 6120 6661 7374 6572 2065  n for a faster e
+00011290: 7865 6375 7469 6f6e 0d0a 0d0a 2a20 5665  xecution....* Ve
+000112a0: 7273 696f 6e20 302e 340d 0a20 202a 2041  rsion 0.4..  * A
+000112b0: 6464 6564 204c 5453 7069 6365 4261 7463  dded LTSpiceBatc
+000112c0: 682e 7079 2074 6f20 7468 6520 636f 6c6c  h.py to the coll
+000112d0: 6563 7469 6f6e 206f 6620 746f 6f6c 730d  ection of tools.
+000112e0: 0a0d 0a2a 2056 6572 7369 6f6e 2030 2e33  ...* Version 0.3
+000112f0: 0d0a 2020 2a20 4120 7665 7273 696f 6e20  ..  * A version 
+00011300: 6f66 204c 5453 7465 7073 2074 6861 7420  of LTSteps that 
+00011310: 6361 6e20 6265 2069 6d70 6f72 7465 6420  can be imported 
+00011320: 746f 2075 7365 2069 6e20 6120 6869 6768  to use in a high
+00011330: 6572 206c 6576 656c 2073 6372 6970 740d  er level script.
+00011340: 0a0d 0a2a 2056 6572 7369 6f6e 2030 2e32  ...* Version 0.2
+00011350: 0d0a 2020 2a20 4164 6469 6e67 204c 5453  ..  * Adding LTS
+00011360: 7465 7073 2e70 7920 616e 6420 4869 7374  teps.py and Hist
+00011370: 6f67 7261 6d2e 7079 0d0a 0d0a 2a20 5665  ogram.py....* Ve
+00011380: 7273 696f 6e20 302e 3120 0d0a 2020 2a20  rsion 0.1 ..  * 
+00011390: 4669 7273 7420 636f 6d6d 6974 2074 6f20  First commit to 
+000113a0: 7468 6520 6269 7462 7563 6b65 7420 7265  the bitbucket re
+000113b0: 706f 7369 746f 7279 2e0d 0a              pository...
```

### Comparing `pyltspice-5.3.0/PyLTSpice/Histogram.py` & `pyltspice-5.3.1/PyLTSpice/Histogram.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/LTSteps.py` & `pyltspice-5.3.1/PyLTSpice/LTSteps.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/__init__.py` & `pyltspice-5.3.1/PyLTSpice/__init__.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/editor/asc_editor.py` & `pyltspice-5.3.1/PyLTSpice/editor/asc_editor.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/editor/spice_editor.py` & `pyltspice-5.3.1/PyLTSpice/editor/spice_editor.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/log/logfile_data.py` & `pyltspice-5.3.1/PyLTSpice/log/logfile_data.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/log/ltsteps.py` & `pyltspice-5.3.1/PyLTSpice/log/ltsteps.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/log/semi_dev_op_reader.py` & `pyltspice-5.3.1/PyLTSpice/log/semi_dev_op_reader.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/raw/raw_classes.py` & `pyltspice-5.3.1/PyLTSpice/raw/raw_classes.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/raw/raw_read.py` & `pyltspice-5.3.1/PyLTSpice/raw/raw_read.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/raw/raw_write.py` & `pyltspice-5.3.1/PyLTSpice/raw/raw_write.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/rawplot.py` & `pyltspice-5.3.1/PyLTSpice/rawplot.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/run_server.py` & `pyltspice-5.3.1/PyLTSpice/run_server.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/sim/ltspice_simulator.py` & `pyltspice-5.3.1/PyLTSpice/sim/ltspice_simulator.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/sim/process_callback.py` & `pyltspice-5.3.1/PyLTSpice/sim/process_callback.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/sim/sim_batch.py` & `pyltspice-5.3.1/PyLTSpice/sim/sim_batch.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/sim/sim_runner.py` & `pyltspice-5.3.1/PyLTSpice/sim/sim_runner.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/sim/sim_stepping.py` & `pyltspice-5.3.1/PyLTSpice/sim/sim_stepping.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/sim/tookit/montecarlo.py` & `pyltspice-5.3.1/PyLTSpice/sim/tookit/montecarlo.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/sim/tookit/worst_case.py` & `pyltspice-5.3.1/PyLTSpice/sim/tookit/worst_case.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/utils/detect_encoding.py` & `pyltspice-5.3.1/PyLTSpice/utils/detect_encoding.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice/utils/sweep_iterators.py` & `pyltspice-5.3.1/PyLTSpice/utils/sweep_iterators.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/PyLTSpice.egg-info/PKG-INFO` & `pyltspice-5.3.1/PyLTSpice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2050 794c  : 2.1..Name: PyL
 00000020: 5453 7069 6365 0d0a 5665 7273 696f 6e3a  TSpice..Version:
-00000030: 2035 2e33 2e30 0d0a 5375 6d6d 6172 793a   5.3.0..Summary:
+00000030: 2035 2e33 2e31 0d0a 5375 6d6d 6172 793a   5.3.1..Summary:
 00000040: 2041 2073 6574 206f 6620 746f 6f6c 7320   A set of tools 
 00000050: 746f 2041 7574 6f6d 6174 6520 4c54 5370  to Automate LTSp
 00000060: 6963 6520 7369 6d75 6c61 7469 6f6e 730d  ice simulations.
 00000070: 0a41 7574 686f 722d 656d 6169 6c3a 204e  .Author-email: N
 00000080: 756e 6f20 4272 756d 203c 6d65 406e 756e  uno Brum <me@nun
 00000090: 6f62 7275 6d2e 636f 6d3e 0d0a 4c69 6365  obrum.com>..Lice
 000000a0: 6e73 653a 2020 2020 2020 2020 2020 2020  nse:            
@@ -2614,15 +2614,15 @@
 0000a350: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
 0000a360: 3e3d 332e 380d 0a44 6573 6372 6970 7469  >=3.8..Descripti
 0000a370: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
 0000a380: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
 0000a390: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
 0000a3a0: 4345 4e53 450d 0a52 6571 7569 7265 732d  CENSE..Requires-
 0000a3b0: 4469 7374 3a20 7370 6963 656c 6962 3e3d  Dist: spicelib>=
-0000a3c0: 312e 312e 310d 0a0d 0a23 2052 4541 444d  1.1.1....# READM
+0000a3c0: 312e 312e 320d 0a0d 0a23 2052 4541 444d  1.1.2....# READM
 0000a3d0: 4520 230d 0a0d 0a50 794c 5453 7069 6365  E #....PyLTSpice
 0000a3e0: 2069 7320 6120 746f 6f6c 6368 6169 6e20   is a toolchain 
 0000a3f0: 6f66 2070 7974 686f 6e20 7574 696c 6974  of python utilit
 0000a400: 6965 7320 6465 7369 676e 2074 6f20 696e  ies design to in
 0000a410: 7465 7261 6374 2077 6974 6820 4c54 5370  teract with LTSp
 0000a420: 6963 6520 456c 6563 7472 6f6e 6963 2053  ice Electronic S
 0000a430: 696d 756c 6174 6f72 2e0d 0a49 7420 6973  imulator...It is
@@ -2840,1484 +2840,1573 @@
 0000b170: 746c 6962 2070 6c6f 740d 0a0d 0a60 6060  tlib plot....```
 0000b180: 7079 7468 6f6e 0d0a 6672 6f6d 2050 794c  python..from PyL
 0000b190: 5453 7069 6365 2069 6d70 6f72 7420 5261  TSpice import Ra
 0000b1a0: 7752 6561 640d 0a0d 0a66 726f 6d20 6d61  wRead....from ma
 0000b1b0: 7470 6c6f 746c 6962 2069 6d70 6f72 7420  tplotlib import 
 0000b1c0: 7079 706c 6f74 2061 7320 706c 740d 0a0d  pyplot as plt...
 0000b1d0: 0a4c 5452 203d 2052 6177 5265 6164 2822  .LTR = RawRead("
-0000b1e0: 5452 414e 202d 2053 5445 502e 7261 7722  TRAN - STEP.raw"
-0000b1f0: 290d 0a0d 0a70 7269 6e74 284c 5452 2e67  )....print(LTR.g
-0000b200: 6574 5f74 7261 6365 5f6e 616d 6573 2829  et_trace_names()
-0000b210: 290d 0a70 7269 6e74 284c 5452 2e67 6574  )..print(LTR.get
-0000b220: 5f72 6177 5f70 726f 7065 7274 7928 2929  _raw_property())
-0000b230: 0d0a 0d0a 4952 3120 3d20 4c54 522e 6765  ....IR1 = LTR.ge
-0000b240: 745f 7472 6163 6528 2249 2852 3129 2229  t_trace("I(R1)")
-0000b250: 0d0a 7820 3d20 4c54 522e 6765 745f 7472  ..x = LTR.get_tr
-0000b260: 6163 6528 2774 696d 6527 2920 2023 2047  ace('time')  # G
-0000b270: 6574 7320 7468 6520 7469 6d65 2061 7869  ets the time axi
-0000b280: 730d 0a73 7465 7073 203d 204c 5452 2e67  s..steps = LTR.g
-0000b290: 6574 5f73 7465 7073 2829 0d0a 666f 7220  et_steps()..for 
-0000b2a0: 7374 6570 2069 6e20 7261 6e67 6528 6c65  step in range(le
-0000b2b0: 6e28 7374 6570 7329 293a 0d0a 2020 2020  n(steps)):..    
-0000b2c0: 2320 7072 696e 7428 7374 6570 735b 7374  # print(steps[st
-0000b2d0: 6570 5d29 0d0a 2020 2020 706c 742e 706c  ep])..    plt.pl
-0000b2e0: 6f74 2878 2e67 6574 5f77 6176 6528 7374  ot(x.get_wave(st
-0000b2f0: 6570 292c 2049 5231 2e67 6574 5f77 6176  ep), IR1.get_wav
-0000b300: 6528 7374 6570 292c 206c 6162 656c 3d73  e(step), label=s
-0000b310: 7465 7073 5b73 7465 705d 290d 0a0d 0a70  teps[step])....p
-0000b320: 6c74 2e6c 6567 656e 6428 2920 2023 206f  lt.legend()  # o
-0000b330: 7264 6572 2061 206c 6567 656e 640d 0a70  rder a legend..p
-0000b340: 6c74 2e73 686f 7728 290d 0a60 6060 2020  lt.show()..```  
-0000b350: 200d 0a0d 0a23 2323 2052 6177 5772 6974   ....### RawWrit
-0000b360: 6520 2323 230d 0a0d 0a54 6865 2066 6f6c  e ###....The fol
-0000b370: 6c6f 7769 6e67 2065 7861 6d70 6c65 2077  lowing example w
-0000b380: 7269 7465 7320 6120 5241 5720 6669 6c65  rites a RAW file
-0000b390: 2077 6974 6820 6120 3320 6d69 6c6c 6973   with a 3 millis
-0000b3a0: 6563 6f6e 6473 2074 7261 6e73 6965 6e74  econds transient
-0000b3b0: 2073 696d 756c 6174 696f 6e20 7369 6e65   simulation sine
-0000b3c0: 2077 6974 6820 6120 3130 6b48 7a20 616e   with a 10kHz an
-0000b3d0: 6420 6120 636f 7369 6e65 2077 6974 680d  d a cosine with.
-0000b3e0: 0a39 2e39 3937 6b48 7a0d 0a0d 0a60 6060  .9.997kHz....```
-0000b3f0: 7079 7468 6f6e 0d0a 696d 706f 7274 206e  python..import n
-0000b400: 756d 7079 2061 7320 6e70 0d0a 6672 6f6d  umpy as np..from
-0000b410: 2050 794c 5453 7069 6365 2069 6d70 6f72   PyLTSpice impor
-0000b420: 7420 5472 6163 652c 2052 6177 5772 6974  t Trace, RawWrit
-0000b430: 650d 0a0d 0a4c 5720 3d20 5261 7757 7269  e....LW = RawWri
-0000b440: 7465 2866 6173 7461 6363 6573 3d46 616c  te(fastacces=Fal
-0000b450: 7365 290d 0a74 7820 3d20 5472 6163 6528  se)..tx = Trace(
-0000b460: 2774 696d 6527 2c20 6e70 2e61 7261 6e67  'time', np.arang
-0000b470: 6528 302e 302c 2033 652d 332c 2039 3937  e(0.0, 3e-3, 997
-0000b480: 452d 3131 2929 0d0a 7679 203d 2054 7261  E-11))..vy = Tra
-0000b490: 6365 2827 4e30 3031 272c 206e 702e 7369  ce('N001', np.si
-0000b4a0: 6e28 3220 2a20 6e70 2e70 6920 2a20 7478  n(2 * np.pi * tx
-0000b4b0: 2e64 6174 6120 2a20 3130 3030 3029 290d  .data * 10000)).
-0000b4c0: 0a76 7a20 3d20 5472 6163 6528 274e 3030  .vz = Trace('N00
-0000b4d0: 3227 2c20 6e70 2e63 6f73 2832 202a 206e  2', np.cos(2 * n
-0000b4e0: 702e 7069 202a 2074 782e 6461 7461 202a  p.pi * tx.data *
-0000b4f0: 2039 3937 3029 290d 0a4c 572e 6164 645f   9970))..LW.add_
-0000b500: 7472 6163 6528 7478 290d 0a4c 572e 6164  trace(tx)..LW.ad
-0000b510: 645f 7472 6163 6528 7679 290d 0a4c 572e  d_trace(vy)..LW.
-0000b520: 6164 645f 7472 6163 6528 767a 290d 0a4c  add_trace(vz)..L
-0000b530: 572e 7361 7665 2822 7465 7374 655f 736e  W.save("teste_sn
-0000b540: 6970 7065 7431 2e72 6177 2229 0d0a 6060  ippet1.raw")..``
-0000b550: 6020 2020 0d0a 0d0a 2323 2320 5370 6963  `   ....### Spic
-0000b560: 6545 6469 746f 722c 2041 7363 4564 6974  eEditor, AscEdit
-0000b570: 6f72 2061 6e64 2053 696d 5275 6e6e 6572  or and SimRunner
-0000b580: 2e70 7920 2323 230d 0a0d 0a54 6869 7320  .py ###....This 
-0000b590: 6d6f 6475 6c65 2069 7320 7573 6564 2074  module is used t
-0000b5a0: 6f20 6c61 756e 6368 204c 5453 5069 6365  o launch LTSPice
-0000b5b0: 2073 696d 756c 6174 696f 6e73 2e20 5265   simulations. Re
-0000b5c0: 7375 6c74 7320 7468 656e 2063 616e 2062  sults then can b
-0000b5d0: 6520 7072 6f63 6573 7365 6420 7769 7468  e processed with
-0000b5e0: 2065 6974 6865 7220 7468 6520 5261 7752   either the RawR
-0000b5f0: 6561 6420 6f72 2077 6974 6820 7468 650d  ead or with the.
-0000b600: 0a4c 5453 7465 7073 206d 6f64 756c 6520  .LTSteps module 
-0000b610: 746f 2072 6561 6420 7468 6520 6c6f 6720  to read the log 
-0000b620: 6669 6c65 2077 6869 6368 2063 616e 2063  file which can c
-0000b630: 6f6e 7461 696e 202e 4d45 4153 2072 6573  ontain .MEAS res
-0000b640: 756c 7473 2e0d 0a0d 0a54 6865 2073 6372  ults.....The scr
-0000b650: 6970 7420 7769 6c6c 2066 6972 7374 6c79  ipt will firstly
-0000b660: 2069 6e76 6f6b 6520 7468 6520 4c54 5370   invoke the LTSp
-0000b670: 6963 6520 696e 2063 6f6d 6d61 6e64 206c  ice in command l
-0000b680: 696e 6520 746f 2067 656e 6572 6174 6520  ine to generate 
-0000b690: 6120 6e65 746c 6973 742c 2061 6e64 2074  a netlist, and t
-0000b6a0: 6865 6e20 7468 6973 206e 6574 6c69 7374  hen this netlist
-0000b6b0: 2063 616e 2062 6520 7570 6461 7465 640d   can be updated.
-0000b6c0: 0a64 6972 6563 746c 7920 6279 2074 6865  .directly by the
-0000b6d0: 2073 6372 6970 742c 2069 6e20 6f72 6465   script, in orde
-0000b6e0: 7220 746f 2063 6861 6e67 6520 636f 6d70  r to change comp
-0000b6f0: 6f6e 656e 7420 7661 6c75 6573 2c20 7061  onent values, pa
-0000b700: 7261 6d65 7465 7273 206f 7220 7369 6d75  rameters or simu
-0000b710: 6c61 7469 6f6e 2063 6f6d 6d61 6e64 732e  lation commands.
-0000b720: 0d0a 0d0a 4865 7265 2066 6f6c 6c6f 7773  ....Here follows
-0000b730: 2061 6e20 6578 616d 706c 6520 6f66 206f   an example of o
-0000b740: 7065 7261 7469 6f6e 2e0d 0a0d 0a60 6060  peration.....```
-0000b750: 7079 7468 6f6e 0d0a 6672 6f6d 2050 794c  python..from PyL
-0000b760: 5453 7069 6365 2069 6d70 6f72 7420 5369  TSpice import Si
-0000b770: 6d52 756e 6e65 720d 0a66 726f 6d20 5079  mRunner..from Py
-0000b780: 4c54 5370 6963 6520 696d 706f 7274 2053  LTSpice import S
-0000b790: 7069 6365 4564 6974 6f72 0d0a 0d0a 2320  piceEditor....# 
-0000b7a0: 7365 6c65 6374 2073 7069 6365 206d 6f64  select spice mod
-0000b7b0: 656c 0d0a 4c54 4320 3d20 5369 6d52 756e  el..LTC = SimRun
-0000b7c0: 6e65 7228 6f75 7470 7574 5f66 6f6c 6465  ner(output_folde
-0000b7d0: 723d 272e 2f74 656d 7027 290d 0a4c 5443  r='./temp')..LTC
-0000b7e0: 2e63 7265 6174 655f 6e65 746c 6973 7428  .create_netlist(
-0000b7f0: 2742 6174 6368 5f54 6573 742e 6173 6327  'Batch_Test.asc'
-0000b800: 290d 0a6e 6574 6c69 7374 203d 2053 7069  )..netlist = Spi
-0000b810: 6365 4564 6974 6f72 2827 4261 7463 685f  ceEditor('Batch_
-0000b820: 5465 7374 2e6e 6574 2729 0d0a 2320 7365  Test.net')..# se
-0000b830: 7420 6465 6661 756c 7420 6172 6775 6d65  t default argume
-0000b840: 6e74 730d 0a6e 6574 6c69 7374 2e73 6574  nts..netlist.set
-0000b850: 5f70 6172 616d 6574 6572 7328 7265 733d  _parameters(res=
-0000b860: 302c 2063 6170 3d31 3030 652d 362c 2072  0, cap=100e-6, r
-0000b870: 756e 3d2d 3129 0d0a 6e65 746c 6973 742e  un=-1)..netlist.
-0000b880: 7365 745f 636f 6d70 6f6e 656e 745f 7661  set_component_va
-0000b890: 6c75 6528 2752 3227 2c20 2732 6b27 2920  lue('R2', '2k') 
-0000b8a0: 2023 204d 6f64 6966 7969 6e67 2074 6865   # Modifying the
-0000b8b0: 2076 616c 7565 206f 6620 6120 7265 7369   value of a resi
-0000b8c0: 7374 6f72 0d0a 6e65 746c 6973 742e 7365  stor..netlist.se
-0000b8d0: 745f 636f 6d70 6f6e 656e 745f 7661 6c75  t_component_valu
-0000b8e0: 6528 2752 3127 2c20 2734 6b27 290d 0a6e  e('R1', '4k')..n
-0000b8f0: 6574 6c69 7374 2e73 6574 5f65 6c65 6d65  etlist.set_eleme
-0000b900: 6e74 5f6d 6f64 656c 2827 5633 272c 2022  nt_model('V3', "
-0000b910: 5349 4e45 2830 2031 2033 6b20 3020 3020  SINE(0 1 3k 0 0 
-0000b920: 3029 2229 2020 2320 4d6f 6469 6679 696e  0)")  # Modifyin
-0000b930: 6720 7468 650d 0a6e 6574 6c69 7374 2e73  g the..netlist.s
-0000b940: 6574 5f63 6f6d 706f 6e65 6e74 5f76 616c  et_component_val
-0000b950: 7565 2827 5855 313a 4332 272c 2032 3065  ue('XU1:C2', 20e
-0000b960: 2d31 3229 2020 2320 6d6f 6469 6679 696e  -12)  # modifyin
-0000b970: 6720 6120 6465 6669 6e65 2073 696d 756c  g a define simul
-0000b980: 6174 696f 6e0d 0a6e 6574 6c69 7374 2e61  ation..netlist.a
-0000b990: 6464 5f69 6e73 7472 7563 7469 6f6e 7328  dd_instructions(
-0000b9a0: 0d0a 2020 2020 223b 2053 696d 756c 6174  ..    "; Simulat
-0000b9b0: 696f 6e20 7365 7474 696e 6773 222c 0d0a  ion settings",..
-0000b9c0: 2020 2020 222e 7361 7665 2056 2856 696e      ".save V(Vin
-0000b9d0: 2920 4928 5231 2922 2c0d 0a29 0d0a 0d0a  ) I(R1)",..)....
-0000b9e0: 666f 7220 6f70 616d 7020 696e 2028 2741  for opamp in ('A
-0000b9f0: 4437 3132 272c 2027 4144 3832 3027 293a  D712', 'AD820'):
-0000ba00: 0d0a 2020 2020 6e65 746c 6973 742e 7365  ..    netlist.se
-0000ba10: 745f 656c 656d 656e 745f 6d6f 6465 6c28  t_element_model(
-0000ba20: 2758 5531 272c 206f 7061 6d70 290d 0a20  'XU1', opamp).. 
-0000ba30: 2020 2066 6f72 2073 7570 706c 795f 766f     for supply_vo
-0000ba40: 6c74 6167 6520 696e 2028 352c 2031 302c  ltage in (5, 10,
-0000ba50: 2031 3529 3a0d 0a20 2020 2020 2020 206e   15):..        n
-0000ba60: 6574 6c69 7374 2e73 6574 5f63 6f6d 706f  etlist.set_compo
-0000ba70: 6e65 6e74 5f76 616c 7565 2827 5631 272c  nent_value('V1',
-0000ba80: 2073 7570 706c 795f 766f 6c74 6167 6529   supply_voltage)
-0000ba90: 0d0a 2020 2020 2020 2020 6e65 746c 6973  ..        netlis
-0000baa0: 742e 7365 745f 636f 6d70 6f6e 656e 745f  t.set_component_
-0000bab0: 7661 6c75 6528 2756 3227 2c20 2d73 7570  value('V2', -sup
-0000bac0: 706c 795f 766f 6c74 6167 6529 0d0a 2020  ply_voltage)..  
-0000bad0: 2020 2020 2020 7072 696e 7428 2273 696d        print("sim
-0000bae0: 756c 6174 696e 6720 4f70 416d 7022 2c20  ulating OpAmp", 
-0000baf0: 6f70 616d 702c 2022 566f 6c74 6167 6522  opamp, "Voltage"
-0000bb00: 2c20 7375 7070 6c79 5f76 6f6c 7461 6765  , supply_voltage
-0000bb10: 290d 0a20 2020 2020 2020 204c 5443 2e72  )..        LTC.r
-0000bb20: 756e 286e 6574 6c69 7374 290d 0a0d 0a66  un(netlist)....f
-0000bb30: 6f72 2072 6177 2c20 6c6f 6720 696e 204c  or raw, log in L
-0000bb40: 5443 3a0d 0a20 2020 2070 7269 6e74 2822  TC:..    print("
-0000bb50: 5261 7720 6669 6c65 3a20 2573 2c20 4c6f  Raw file: %s, Lo
-0000bb60: 6720 6669 6c65 3a20 2573 2220 2520 2872  g file: %s" % (r
-0000bb70: 6177 2c20 6c6f 6729 290d 0a20 2020 2023  aw, log))..    #
-0000bb80: 2064 6f20 736f 6d65 7468 696e 6720 7769   do something wi
-0000bb90: 7468 2074 6865 2064 6174 610d 0a20 2020  th the data..   
-0000bba0: 2023 2072 6177 5f64 6174 6120 3d20 5261   # raw_data = Ra
-0000bbb0: 7752 6561 6428 7261 7729 0d0a 2020 2020  wRead(raw)..    
-0000bbc0: 2320 6c6f 675f 6461 7461 203d 204c 5453  # log_data = LTS
-0000bbd0: 7465 7073 286c 6f67 290d 0a20 2020 2023  teps(log)..    #
-0000bbe0: 202e 2e2e 0d0a 0d0a 6e65 746c 6973 742e   .......netlist.
-0000bbf0: 7265 7365 745f 6e65 746c 6973 7428 290d  reset_netlist().
-0000bc00: 0a6e 6574 6c69 7374 2e61 6464 5f69 6e73  .netlist.add_ins
-0000bc10: 7472 7563 7469 6f6e 7328 0d0a 2020 2020  tructions(..    
-0000bc20: 223b 2053 696d 756c 6174 696f 6e20 7365  "; Simulation se
-0000bc30: 7474 696e 6773 222c 0d0a 2020 2020 222e  ttings",..    ".
-0000bc40: 6163 2064 6563 2033 3020 3130 2031 4d65  ac dec 30 10 1Me
-0000bc50: 6722 2c0d 0a20 2020 2022 2e6d 6561 7320  g",..    ".meas 
-0000bc60: 4143 2047 6169 6e20 4d41 5820 6d61 6728  AC Gain MAX mag(
-0000bc70: 5628 6f75 7429 2920 3b20 6669 6e64 2074  V(out)) ; find t
-0000bc80: 6865 2070 6561 6b20 7265 7370 6f6e 7365  he peak response
-0000bc90: 2061 6e64 2063 616c 6c20 6974 2022 2247   and call it ""G
-0000bca0: 6169 6e22 2222 2c0d 0a20 2020 2022 2e6d  ain""",..    ".m
-0000bcb0: 6561 7320 4143 2046 6375 7420 5452 4947  eas AC Fcut TRIG
-0000bcc0: 206d 6167 2856 286f 7574 2929 3d47 6169   mag(V(out))=Gai
-0000bcd0: 6e2f 7371 7274 2832 2920 4641 4c4c 3d6c  n/sqrt(2) FALL=l
-0000bce0: 6173 7422 0d0a 290d 0a0d 0a23 2053 696d  ast"..)....# Sim
-0000bcf0: 2053 7461 7469 7374 6963 730d 0a70 7269   Statistics..pri
-0000bd00: 6e74 2827 5375 6363 6573 7366 756c 2f54  nt('Successful/T
-0000bd10: 6f74 616c 2053 696d 756c 6174 696f 6e73  otal Simulations
-0000bd20: 3a20 2720 2b20 7374 7228 4c54 432e 6f6b  : ' + str(LTC.ok
-0000bd30: 5369 6d29 202b 2027 2f27 202b 2073 7472  Sim) + '/' + str
-0000bd40: 284c 5443 2e72 756e 6e6f 2929 0d0a 0d0a  (LTC.runno))....
-0000bd50: 656e 7465 7220 3d20 696e 7075 7428 2250  enter = input("P
-0000bd60: 7265 7373 2065 6e74 6572 2074 6f20 6465  ress enter to de
-0000bd70: 6c65 7465 2063 7265 6174 6564 2066 696c  lete created fil
-0000bd80: 6573 2229 0d0a 6966 2065 6e74 6572 203d  es")..if enter =
-0000bd90: 3d20 2727 3a0d 0a20 2020 204c 5443 2e66  = '':..    LTC.f
-0000bda0: 696c 655f 636c 6561 6e75 7028 290d 0a60  ile_cleanup()..`
-0000bdb0: 6060 0d0a 0d0a 5468 6520 6578 616d 706c  ``....The exampl
-0000bdc0: 6520 6162 6f76 6520 6973 2075 7369 6e67  e above is using
-0000bdd0: 2074 6865 2053 7069 6365 4564 6974 6f72   the SpiceEditor
-0000bde0: 2074 6f20 6372 6561 7465 2061 6e64 206d   to create and m
-0000bdf0: 6f64 6966 7920 6120 7370 6963 6520 6e65  odify a spice ne
-0000be00: 746c 6973 742c 2062 7574 2069 7420 6973  tlist, but it is
-0000be10: 2061 6c73 6f20 706f 7373 6962 6c65 2074   also possible t
-0000be20: 6f20 7573 6520 7468 650d 0a41 7363 4564  o use the..AscEd
-0000be30: 6974 6f72 2074 6f20 6469 7265 6374 6c79  itor to directly
-0000be40: 206d 6f64 6966 7920 7468 6520 2e61 7363   modify the .asc
-0000be50: 2066 696c 652e 2054 6865 2065 6469 7465   file. The edite
-0000be60: 6420 2e61 7363 2066 696c 6520 6361 6e20  d .asc file can 
-0000be70: 7468 656e 2062 6520 6f70 656e 6564 2062  then be opened b
-0000be80: 7920 7468 6520 4c54 5370 6963 6520 4755  y the LTSpice GU
-0000be90: 4920 616e 6420 7468 650d 0a73 696d 756c  I and the..simul
-0000bea0: 6174 696f 6e20 6361 6e20 6265 2072 756e  ation can be run
-0000beb0: 2066 726f 6d20 7468 6572 652e 0d0a 0d0a   from there.....
-0000bec0: 2323 2320 5369 6d75 6c61 7469 6f6e 2041  ### Simulation A
-0000bed0: 6e61 6c79 7369 7320 546f 6f6c 6b69 7420  nalysis Toolkit 
-0000bee0: 2323 230d 0a0d 0a54 6865 2041 7363 4564  ###....The AscEd
-0000bef0: 6974 6f72 2063 616e 2062 6520 7573 6564  itor can be used
-0000bf00: 2077 6974 6820 7468 6520 5369 6d75 6c61   with the Simula
-0000bf10: 7469 6f6e 2041 6e61 6c79 7369 7320 546f  tion Analysis To
-0000bf20: 6f6c 6b69 7420 746f 2070 6572 666f 726d  olkit to perform
-0000bf30: 204d 6f6e 7465 2043 6172 6c6f 206f 7220   Monte Carlo or 
-0000bf40: 576f 7374 2043 6173 6520 7369 6d75 6c61  Wost Case simula
-0000bf50: 7469 6f6e 732e 0d0a 5468 6573 6520 7369  tions...These si
-0000bf60: 6d75 6c61 7469 6f6e 7320 6361 6e20 6569  mulations can ei
-0000bf70: 7468 6572 2062 6520 646f 6e65 206f 6e20  ther be done on 
-0000bf80: 7468 6520 4c54 5370 6963 6520 4755 4920  the LTSpice GUI 
-0000bf90: 6f72 2075 7369 6e67 2074 6865 2052 756e  or using the Run
-0000bfa0: 6e65 7220 436c 6173 7320 6465 7363 7269  ner Class descri
-0000bfb0: 6265 6420 6162 6f76 652e 0d0a 0d0a 4c65  bed above.....Le
-0000bfc0: 7427 7320 636f 6e73 6964 6572 2074 6865  t's consider the
-0000bfd0: 2066 6f6c 6c6f 7769 6e67 2063 6972 6375   following circu
-0000bfe0: 6974 3a0d 0a0d 0a21 5b53 616c 6c65 6e2d  it:....![Sallen-
-0000bff0: 4b65 7920 416d 706c 6966 6965 725d 282e  Key Amplifier](.
-0000c000: 2f64 6f63 2f6d 6f64 756c 6573 2f73 616c  /doc/modules/sal
-0000c010: 6c65 6e6b 6579 2e70 6e67 2022 5361 6c6c  lenkey.png "Sall
-0000c020: 656e 2d4b 6579 2041 6d70 6c69 6669 6572  en-Key Amplifier
-0000c030: 2229 0d0a 0d0a 5768 656e 2070 6572 666f  ")....When perfo
-0000c040: 726d 696e 6720 6120 4d6f 6e74 6520 4361  rming a Monte Ca
-0000c050: 726c 6f20 7369 6d75 6c61 7469 6f6e 206f  rlo simulation o
-0000c060: 6e20 7468 6973 2063 6972 6375 6974 2c20  n this circuit, 
-0000c070: 7765 206e 6565 6420 746f 206d 616e 7561  we need to manua
-0000c080: 6c6c 7920 6d6f 6469 6679 2074 6865 2076  lly modify the v
-0000c090: 616c 7565 206f 6620 6561 6368 2063 6f6d  alue of each com
-0000c0a0: 706f 6e65 6e74 2c20 0d0a 616e 6420 7468  ponent, ..and th
-0000c0b0: 656e 2061 6464 2074 6865 202e 7374 6570  en add the .step
-0000c0c0: 2063 6f6d 6d61 6e64 2066 6f72 206d 616b   command for mak
-0000c0d0: 696e 6720 7365 7665 7261 6c20 7275 6e73  ing several runs
-0000c0e0: 206f 6e20 7468 6520 7361 6d65 2063 6972   on the same cir
-0000c0f0: 6375 6974 2e20 0d0a 546f 2073 696d 706c  cuit. ..To simpl
-0000c100: 6966 7920 7468 6973 2070 726f 6365 7373  ify this process
-0000c110: 2c20 7468 6520 4173 6345 6469 746f 7220  , the AscEditor 
-0000c120: 636c 6173 7320 6361 6e20 6265 2075 7365  class can be use
-0000c130: 6420 6173 2065 7865 6d70 6c69 6669 6564  d as exemplified
-0000c140: 2062 656c 6f77 3a0d 0a0d 0a60 6060 7079   below:....```py
-0000c150: 7468 6f6e 0d0a 6672 6f6d 2050 794c 5453  thon..from PyLTS
-0000c160: 7069 6365 2069 6d70 6f72 7420 4173 6345  pice import AscE
-0000c170: 6469 746f 722c 2053 696d 5275 6e6e 6572  ditor, SimRunner
-0000c180: 2020 2320 496d 706f 7274 7320 7468 6520    # Imports the 
-0000c190: 636c 6173 7320 7468 6174 206d 616e 6970  class that manip
-0000c1a0: 756c 6174 6573 2074 6865 2061 7363 2066  ulates the asc f
-0000c1b0: 696c 650d 0a66 726f 6d20 5079 4c54 5370  ile..from PyLTSp
-0000c1c0: 6963 652e 7369 6d2e 746f 6f6b 6974 2e6d  ice.sim.tookit.m
-0000c1d0: 6f6e 7465 6361 726c 6f20 696d 706f 7274  ontecarlo import
-0000c1e0: 204d 6f6e 7465 6361 726c 6f20 2023 2049   Montecarlo  # I
-0000c1f0: 6d70 6f72 7473 2074 6865 204d 6f6e 7465  mports the Monte
-0000c200: 6361 726c 6f20 746f 6f6c 6b69 7420 636c  carlo toolkit cl
-0000c210: 6173 730d 0a0d 0a73 616c 6c65 6e6b 6579  ass....sallenkey
-0000c220: 203d 2041 7363 4564 6974 6f72 2822 2e2f   = AscEditor("./
-0000c230: 7465 7374 6669 6c65 732f 7361 6c6c 656e  testfiles/sallen
-0000c240: 6b65 792e 6173 6322 2920 2023 2052 6561  key.asc")  # Rea
-0000c250: 6473 2074 6865 2061 7363 2066 696c 6520  ds the asc file 
-0000c260: 696e 746f 206d 656d 6f72 790d 0a72 756e  into memory..run
-0000c270: 6e65 7220 3d20 5369 6d52 756e 6e65 7228  ner = SimRunner(
-0000c280: 6f75 7470 7574 5f66 6f6c 6465 723d 272e  output_folder='.
-0000c290: 2f74 656d 705f 6d63 2729 2020 2320 496e  /temp_mc')  # In
-0000c2a0: 7374 616e 7469 6174 6573 2074 6865 2072  stantiates the r
-0000c2b0: 756e 6e65 7220 636c 6173 732c 2077 6974  unner class, wit
-0000c2c0: 6820 7468 6520 6f75 7470 7574 2066 6f6c  h the output fol
-0000c2d0: 6465 7220 616c 7265 6164 7920 7365 740d  der already set.
-0000c2e0: 0a6d 6320 3d20 4d6f 6e74 6563 6172 6c6f  .mc = Montecarlo
-0000c2f0: 2873 616c 6c65 6e6b 6579 2c20 7275 6e6e  (sallenkey, runn
-0000c300: 6572 2920 2023 2049 6e73 7461 6e74 6961  er)  # Instantia
-0000c310: 7465 7320 7468 6520 4d6f 6e74 6563 6172  tes the Montecar
-0000c320: 6c6f 2063 6c61 7373 2c20 7769 7468 2074  lo class, with t
-0000c330: 6865 2061 7363 2066 696c 6520 616c 7265  he asc file alre
-0000c340: 6164 7920 696e 206d 656d 6f72 790d 0a0d  ady in memory...
-0000c350: 0a23 2054 6865 2066 6f6c 6c6f 7769 6e67  .# The following
-0000c360: 206c 696e 6573 2073 6574 2074 6865 2064   lines set the d
-0000c370: 6566 6175 6c74 2074 6f6c 6572 616e 6365  efault tolerance
-0000c380: 7320 666f 7220 7468 6520 636f 6d70 6f6e  s for the compon
-0000c390: 656e 7473 0d0a 6d63 2e73 6574 5f74 6f6c  ents..mc.set_tol
-0000c3a0: 6572 616e 6365 2827 5227 2c20 302e 3031  erance('R', 0.01
-0000c3b0: 2920 2023 2031 2520 746f 6c65 7261 6e63  )  # 1% toleranc
-0000c3c0: 652c 2064 6566 6175 6c74 2064 6973 7472  e, default distr
-0000c3d0: 6962 7574 696f 6e20 6973 2075 6e69 666f  ibution is unifo
-0000c3e0: 726d 0d0a 6d63 2e73 6574 5f74 6f6c 6572  rm..mc.set_toler
-0000c3f0: 616e 6365 2827 4327 2c20 302e 312c 2064  ance('C', 0.1, d
-0000c400: 6973 7472 6962 7574 696f 6e3d 2775 6e69  istribution='uni
-0000c410: 666f 726d 2729 2020 2320 3130 2520 746f  form')  # 10% to
-0000c420: 6c65 7261 6e63 652c 2065 7870 6c69 6369  lerance, explici
-0000c430: 7420 756e 6966 6f72 6d20 6469 7374 7269  t uniform distri
-0000c440: 6275 7469 6f6e 0d0a 6d63 2e73 6574 5f74  bution..mc.set_t
-0000c450: 6f6c 6572 616e 6365 2827 5627 2c20 302e  olerance('V', 0.
-0000c460: 312c 2064 6973 7472 6962 7574 696f 6e3d  1, distribution=
-0000c470: 276e 6f72 6d61 6c27 2920 2023 2031 3025  'normal')  # 10%
-0000c480: 2074 6f6c 6572 616e 6365 2c20 6275 7420   tolerance, but 
-0000c490: 7573 696e 6720 6120 6e6f 726d 616c 2064  using a normal d
-0000c4a0: 6973 7472 6962 7574 696f 6e0d 0a0d 0a23  istribution....#
-0000c4b0: 2053 6f6d 6520 636f 6d70 6f6e 656e 7473   Some components
-0000c4c0: 2063 616e 2068 6176 6520 6120 6469 6666   can have a diff
-0000c4d0: 6572 656e 7420 746f 6c65 7261 6e63 650d  erent tolerance.
-0000c4e0: 0a6d 632e 7365 745f 746f 6c65 7261 6e63  .mc.set_toleranc
-0000c4f0: 6528 2752 3127 2c20 302e 3035 2920 2023  e('R1', 0.05)  #
-0000c500: 2035 2520 746f 6c65 7261 6e63 6520 666f   5% tolerance fo
-0000c510: 7220 5231 206f 6e6c 792e 2054 6869 7320  r R1 only. This 
-0000c520: 6f6e 6c79 206f 7665 7272 6964 6573 2074  only overrides t
-0000c530: 6865 2064 6566 6175 6c74 2074 6f6c 6572  he default toler
-0000c540: 616e 6365 2066 6f72 2052 310d 0a0d 0a23  ance for R1....#
-0000c550: 2054 6f6c 6572 616e 6365 7320 6361 6e20   Tolerances can 
-0000c560: 6265 2073 6574 2066 6f72 2070 6172 616d  be set for param
-0000c570: 6574 6572 7320 6173 2077 656c 6c0d 0a6d  eters as well..m
-0000c580: 632e 7365 745f 7061 7261 6d65 7465 725f  c.set_parameter_
-0000c590: 6465 7669 6174 696f 6e28 2756 6f73 272c  deviation('Vos',
-0000c5a0: 2033 652d 342c 2035 652d 332c 2027 756e   3e-4, 5e-3, 'un
-0000c5b0: 6966 6f72 6d27 2920 2023 2054 6865 206b  iform')  # The k
-0000c5c0: 6579 776f 7264 2027 6469 7374 7269 6275  eyword 'distribu
-0000c5d0: 7469 6f6e 2720 6973 206f 7074 696f 6e61  tion' is optiona
-0000c5e0: 6c0d 0a6d 632e 7072 6570 6172 655f 7465  l..mc.prepare_te
-0000c5f0: 7374 6265 6e63 6828 6e75 6d5f 7275 6e73  stbench(num_runs
-0000c600: 3d31 3030 3029 2020 2320 5072 6570 6172  =1000)  # Prepar
-0000c610: 6573 2074 6865 2074 6573 7462 656e 6368  es the testbench
-0000c620: 2066 6f72 2031 3030 3020 7369 6d75 6c61   for 1000 simula
-0000c630: 7469 6f6e 730d 0a0d 0a23 2046 696e 616c  tions....# Final
-0000c640: 6c79 2074 6865 206e 6574 6c69 7374 2069  ly the netlist i
-0000c650: 7320 7361 7665 6420 746f 2061 2066 696c  s saved to a fil
-0000c660: 650d 0a6d 632e 7361 7665 5f6e 6574 6c69  e..mc.save_netli
-0000c670: 7374 2827 2e2f 7465 7374 6669 6c65 732f  st('./testfiles/
-0000c680: 7361 6c6c 656e 6b65 795f 6d63 2e6e 6574  sallenkey_mc.net
-0000c690: 2729 0d0a 0d0a 6d63 2e72 756e 2831 3030  ')....mc.run(100
-0000c6a0: 2920 2023 2052 756e 7320 7468 6520 7369  )  # Runs the si
-0000c6b0: 6d75 6c61 7469 6f6e 2077 6974 6820 7370  mulation with sp
-0000c6c0: 6c69 7473 206f 6620 3130 3020 7275 6e73  lits of 100 runs
-0000c6d0: 2065 6163 680d 0a6c 6f67 7320 3d20 6d63   each..logs = mc
-0000c6e0: 2e72 6561 645f 6c6f 6766 696c 6573 2829  .read_logfiles()
-0000c6f0: 2020 2023 2052 6561 6473 2074 6865 206c     # Reads the l
-0000c700: 6f67 2066 696c 6573 2061 6e64 2073 746f  og files and sto
-0000c710: 7265 7320 7468 6520 7265 7375 6c74 7320  res the results 
-0000c720: 696e 2074 6865 2072 6573 756c 7473 2061  in the results a
-0000c730: 7474 7269 6275 7465 0d0a 6c6f 6773 2e65  ttribute..logs.e
-0000c740: 7870 6f72 745f 6461 7461 2827 2e2f 7465  xport_data('./te
-0000c750: 6d70 5f6d 632f 6461 7461 2e63 7376 2729  mp_mc/data.csv')
-0000c760: 2020 2320 4578 706f 7274 7320 7468 6520    # Exports the 
-0000c770: 6461 7461 2074 6f20 6120 6373 7620 6669  data to a csv fi
-0000c780: 6c65 0d0a 6c6f 6773 2e70 6c6f 745f 6869  le..logs.plot_hi
-0000c790: 7374 6f67 7261 6d28 2766 6375 7427 2920  stogram('fcut') 
-0000c7a0: 2023 2050 6c6f 7473 2074 6865 2068 6973   # Plots the his
-0000c7b0: 746f 6772 616d 7320 666f 7220 7468 6520  tograms for the 
-0000c7c0: 7265 7375 6c74 730d 0a6d 632e 636c 6561  results..mc.clea
-0000c7d0: 6e75 705f 6669 6c65 7328 2920 2023 2044  nup_files()  # D
-0000c7e0: 656c 6574 6573 2074 6865 2074 656d 706f  eletes the tempo
-0000c7f0: 7261 7279 2066 696c 6573 0d0a 6060 600d  rary files..```.
-0000c800: 0a57 6865 6e20 6f70 656e 696e 6720 7468  .When opening th
-0000c810: 6520 6372 6561 7465 6420 7361 6c6c 656e  e created sallen
-0000c820: 6b65 795f 6d63 2e6e 6574 2066 696c 652c  key_mc.net file,
-0000c830: 2077 6520 6361 6e20 7365 6520 7468 6174   we can see that
-0000c840: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-0000c850: 6972 6375 6974 2e0d 0a0d 0a21 5b53 616c  ircuit.....![Sal
-0000c860: 6c65 6e2d 4b65 7920 416d 706c 6966 6965  len-Key Amplifie
-0000c870: 7220 7769 7468 204d 6f6e 7465 6361 726c  r with Montecarl
-0000c880: 6f5d 282e 2f64 6f63 2f6d 6f64 756c 6573  o](./doc/modules
-0000c890: 2f73 616c 6c65 6e6b 6579 5f6d 632e 706e  /sallenkey_mc.pn
-0000c8a0: 6720 2253 616c 6c65 6e2d 4b65 7920 416d  g "Sallen-Key Am
-0000c8b0: 706c 6966 6965 7220 7769 7468 204d 6f6e  plifier with Mon
-0000c8c0: 7465 6361 726c 6f22 290d 0a0d 0a54 6865  tecarlo")....The
-0000c8d0: 2066 6f6c 6c6f 7769 6e67 2075 7064 6174   following updat
-0000c8e0: 6573 2077 6572 6520 6d61 6465 2074 6f20  es were made to 
-0000c8f0: 7468 6520 6369 7263 7569 743a 0d0a 2d20  the circuit:..- 
-0000c900: 5468 6520 7661 6c75 6520 6f66 2065 6163  The value of eac
-0000c910: 6820 636f 6d70 6f6e 656e 7420 7761 7320  h component was 
-0000c920: 7265 706c 6163 6564 2062 7920 6120 6675  replaced by a fu
-0000c930: 6e63 7469 6f6e 2074 6861 7420 6765 6e65  nction that gene
-0000c940: 7261 7465 7320 6120 7261 6e64 6f6d 2076  rates a random v
-0000c950: 616c 7565 2077 6974 6869 6e20 7468 6520  alue within the 
-0000c960: 7370 6563 6966 6965 6420 746f 6c65 7261  specified tolera
-0000c970: 6e63 652e 0d0a 2d20 5468 6520 2e73 7465  nce...- The .ste
-0000c980: 7020 7061 7261 6d20 7275 6e20 636f 6d6d  p param run comm
-0000c990: 616e 6420 7761 7320 6164 6465 6420 746f  and was added to
-0000c9a0: 2074 6865 206e 6574 6c69 7374 2e20 5374   the netlist. St
-0000c9b0: 6172 7473 2061 7420 2d31 2077 6869 6368  arts at -1 which
-0000c9c0: 2069 7427 7320 7468 6520 6e6f 6d69 6e61   it's the nomina
-0000c9d0: 6c20 7661 6c75 6520 7369 6d75 6c61 7469  l value simulati
-0000c9e0: 6f6e 2c20 616e 6420 0d0a 6669 6e69 7368  on, and ..finish
-0000c9f0: 6573 2074 6861 7420 7468 6520 6e75 6d62  es that the numb
-0000ca00: 6572 206f 6620 7369 6d75 6c61 7469 6f6e  er of simulation
-0000ca10: 7320 7370 6563 6966 6965 6420 696e 2074  s specified in t
-0000ca20: 6865 2070 7265 7061 7265 5f74 6573 7462  he prepare_testb
-0000ca30: 656e 6368 2829 206d 6574 686f 642e 0d0a  ench() method...
-0000ca40: 2d20 4120 6465 6661 756c 7420 7661 6c75  - A default valu
-0000ca50: 6520 666f 7220 7468 6520 7275 6e20 7061  e for the run pa
-0000ca60: 7261 6d65 7465 7220 7761 7320 6164 6465  rameter was adde
-0000ca70: 642e 2054 6869 7320 6973 2075 7365 6675  d. This is usefu
-0000ca80: 6c20 6966 2074 6865 202e 7374 6570 2070  l if the .step p
-0000ca90: 6172 616d 2072 756e 2069 7320 636f 6d6d  aram run is comm
-0000caa0: 656e 7465 6420 6f75 742e 0d0a 2d20 5468  ented out...- Th
-0000cab0: 6520 5231 2074 6f6c 6572 616e 6365 2069  e R1 tolerance i
-0000cac0: 7320 6469 6666 6572 656e 7420 6672 6f6d  s different from
-0000cad0: 2074 6865 206f 7468 6572 2072 6573 6973   the other resis
-0000cae0: 746f 7273 2e20 5468 6973 2069 7320 6265  tors. This is be
-0000caf0: 6361 7573 6520 7468 6520 746f 6c65 7261  cause the tolera
-0000cb00: 6e63 6520 7761 7320 6578 706c 6963 6974  nce was explicit
-0000cb10: 6c79 2073 6574 2066 6f72 2052 312e 0d0a  ly set for R1...
-0000cb20: 2d20 5468 6520 566f 7320 7061 7261 6d65  - The Vos parame
-0000cb30: 7465 7220 7761 7320 6164 6465 6420 746f  ter was added to
-0000cb40: 2074 6865 202e 7061 7261 6d20 6c69 7374   the .param list
-0000cb50: 2e20 5468 6973 2069 7320 6265 6361 7573  . This is becaus
-0000cb60: 6520 7468 6520 7061 7261 6d65 7465 7220  e the parameter 
-0000cb70: 7761 7320 6578 706c 6963 6974 6c79 2073  was explicitly s
-0000cb80: 6574 2075 7369 6e67 2074 6865 0d0a 7365  et using the..se
-0000cb90: 745f 7061 7261 6d65 7465 725f 6465 7669  t_parameter_devi
-0000cba0: 6174 696f 6e20 6d65 7468 6f64 2e0d 0a2d  ation method...-
-0000cbb0: 2046 756e 6374 696f 6e73 2075 746f 6c2c   Functions utol,
-0000cbc0: 206e 746f 6c20 616e 6420 7572 6e67 2077   ntol and urng w
-0000cbd0: 6572 6520 6164 6465 6420 746f 2074 6865  ere added to the
-0000cbe0: 202e 6675 6e63 206c 6973 742e 2054 6865   .func list. The
-0000cbf0: 7365 2066 756e 6374 696f 6e73 2061 7265  se functions are
-0000cc00: 2075 7365 6420 746f 2067 656e 6572 6174   used to generat
-0000cc10: 6520 7261 6e64 6f6d 2076 616c 7565 732e  e random values.
-0000cc20: 0d0a 556e 6966 6f72 6d20 6469 7374 7269  ..Uniform distri
-0000cc30: 6275 7469 6f6e 7320 7573 6520 7468 6520  butions use the 
-0000cc40: 4c54 5370 6963 6520 6275 696c 742d 696e  LTSpice built-in
-0000cc50: 206d 6328 782c 2074 6f6c 2920 616e 6420   mc(x, tol) and 
-0000cc60: 666c 6174 2878 2920 6675 6e63 7469 6f6e  flat(x) function
-0000cc70: 732c 2077 6869 6c65 206e 6f72 6d61 6c20  s, while normal 
-0000cc80: 6469 7374 7269 6275 7469 6f6e 7320 7573  distributions us
-0000cc90: 6520 7468 6520 0d0a 6761 7573 7328 7829  e the ..gauss(x)
-0000cca0: 2066 756e 6374 696f 6e2e 0d0a 0d0a 5369   function.....Si
-0000ccb0: 6d69 6c61 726c 792c 2074 6865 2077 6f72  milarly, the wor
-0000ccc0: 7374 2063 6173 6520 616e 616c 7973 6973  st case analysis
-0000ccd0: 2063 616e 2061 6c73 6f20 6265 2073 6574   can also be set
-0000cce0: 7570 2062 7920 7573 696e 6720 7468 6520  up by using the 
-0000ccf0: 636c 6173 7320 576f 7273 7443 6173 6541  class WorstCaseA
-0000cd00: 6e61 6c79 7369 732c 2061 7320 6578 656d  nalysis, as exem
-0000cd10: 706c 6966 6965 6420 6265 6c6f 773a 0d0a  plified below:..
-0000cd20: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-0000cd30: 6d20 5079 4c54 5370 6963 6520 696d 706f  m PyLTSpice impo
-0000cd40: 7274 2041 7363 4564 6974 6f72 2c20 5369  rt AscEditor, Si
-0000cd50: 6d52 756e 6e65 7220 2023 2049 6d70 6f72  mRunner  # Impor
-0000cd60: 7473 2074 6865 2063 6c61 7373 2074 6861  ts the class tha
-0000cd70: 7420 6d61 6e69 7075 6c61 7465 7320 7468  t manipulates th
-0000cd80: 6520 6173 6320 6669 6c65 0d0a 6672 6f6d  e asc file..from
-0000cd90: 2050 794c 5453 7069 6365 2e73 696d 2e74   PyLTSpice.sim.t
-0000cda0: 6f6f 6b69 742e 776f 7273 745f 6361 7365  ookit.worst_case
-0000cdb0: 2069 6d70 6f72 7420 576f 7273 7443 6173   import WorstCas
-0000cdc0: 6541 6e61 6c79 7369 730d 0a0d 0a73 616c  eAnalysis....sal
-0000cdd0: 6c65 6e6b 6579 203d 2041 7363 4564 6974  lenkey = AscEdit
-0000cde0: 6f72 2822 2e2f 7465 7374 6669 6c65 732f  or("./testfiles/
-0000cdf0: 7361 6c6c 656e 6b65 792e 6173 6322 2920  sallenkey.asc") 
-0000ce00: 2023 2052 6561 6473 2074 6865 2061 7363   # Reads the asc
-0000ce10: 2066 696c 6520 696e 746f 206d 656d 6f72   file into memor
-0000ce20: 790d 0a72 756e 6e65 7220 3d20 5369 6d52  y..runner = SimR
-0000ce30: 756e 6e65 7228 6f75 7470 7574 5f66 6f6c  unner(output_fol
-0000ce40: 6465 723d 272e 2f74 656d 705f 7763 6127  der='./temp_wca'
-0000ce50: 2920 2023 2049 6e73 7461 6e74 6961 7465  )  # Instantiate
-0000ce60: 7320 7468 6520 7275 6e6e 6572 2063 6c61  s the runner cla
-0000ce70: 7373 2c20 7769 7468 2074 6865 206f 7574  ss, with the out
-0000ce80: 7075 7420 666f 6c64 6572 2061 6c72 6561  put folder alrea
-0000ce90: 6479 2073 6574 0d0a 7763 6120 3d20 576f  dy set..wca = Wo
-0000cea0: 7273 7443 6173 6541 6e61 6c79 7369 7328  rstCaseAnalysis(
-0000ceb0: 7361 6c6c 656e 6b65 792c 2072 756e 6e65  sallenkey, runne
-0000cec0: 7229 2020 2320 496e 7374 616e 7469 6174  r)  # Instantiat
-0000ced0: 6573 2074 6865 2057 6f72 7374 2043 6173  es the Worst Cas
-0000cee0: 6520 416e 616c 7973 6973 2063 6c61 7373  e Analysis class
-0000cef0: 0d0a 0d0a 2320 5468 6520 666f 6c6c 6f77  ....# The follow
-0000cf00: 696e 6720 6c69 6e65 7320 7365 7420 7468  ing lines set th
-0000cf10: 6520 6465 6661 756c 7420 746f 6c65 7261  e default tolera
-0000cf20: 6e63 6573 2066 6f72 2074 6865 2063 6f6d  nces for the com
-0000cf30: 706f 6e65 6e74 730d 0a77 6361 2e73 6574  ponents..wca.set
-0000cf40: 5f74 6f6c 6572 616e 6365 2827 5227 2c20  _tolerance('R', 
-0000cf50: 302e 3031 2920 2023 2031 2520 746f 6c65  0.01)  # 1% tole
-0000cf60: 7261 6e63 650d 0a77 6361 2e73 6574 5f74  rance..wca.set_t
-0000cf70: 6f6c 6572 616e 6365 2827 4327 2c20 302e  olerance('C', 0.
-0000cf80: 3129 2020 2320 3130 2520 746f 6c65 7261  1)  # 10% tolera
-0000cf90: 6e63 650d 0a77 6361 2e73 6574 5f74 6f6c  nce..wca.set_tol
-0000cfa0: 6572 616e 6365 2827 5627 2c20 302e 3129  erance('V', 0.1)
-0000cfb0: 2020 2320 3130 2520 746f 6c65 7261 6e63    # 10% toleranc
-0000cfc0: 652e 2046 6f72 2057 6f72 7374 2043 6173  e. For Worst Cas
-0000cfd0: 6520 616e 616c 7973 6973 2c20 7468 6520  e analysis, the 
-0000cfe0: 6469 7374 7269 6275 7469 6f6e 2069 7320  distribution is 
-0000cff0: 6972 7265 6c65 7661 6e74 0d0a 0d0a 2320  irrelevant....# 
-0000d000: 536f 6d65 2063 6f6d 706f 6e65 6e74 7320  Some components 
-0000d010: 6361 6e20 6861 7665 2061 2064 6966 6665  can have a diffe
-0000d020: 7265 6e74 2074 6f6c 6572 616e 6365 0d0a  rent tolerance..
-0000d030: 7763 612e 7365 745f 746f 6c65 7261 6e63  wca.set_toleranc
-0000d040: 6528 2752 3127 2c20 302e 3035 2920 2023  e('R1', 0.05)  #
-0000d050: 2035 2520 746f 6c65 7261 6e63 6520 666f   5% tolerance fo
-0000d060: 7220 5231 206f 6e6c 792e 2054 6869 7320  r R1 only. This 
-0000d070: 6f6e 6c79 206f 7665 7272 6964 6573 2074  only overrides t
-0000d080: 6865 2064 6566 6175 6c74 2074 6f6c 6572  he default toler
-0000d090: 616e 6365 2066 6f72 2052 310d 0a0d 0a23  ance for R1....#
-0000d0a0: 2054 6f6c 6572 616e 6365 7320 6361 6e20   Tolerances can 
-0000d0b0: 6265 2073 6574 2066 6f72 2070 6172 616d  be set for param
-0000d0c0: 6574 6572 7320 6173 2077 656c 6c2e 0d0a  eters as well...
-0000d0d0: 7763 612e 7365 745f 7061 7261 6d65 7465  wca.set_paramete
-0000d0e0: 725f 6465 7669 6174 696f 6e28 2756 6f73  r_deviation('Vos
-0000d0f0: 272c 2033 652d 342c 2035 652d 3329 0d0a  ', 3e-4, 5e-3)..
-0000d100: 0d0a 2320 4669 6e61 6c6c 7920 7468 6520  ..# Finally the 
-0000d110: 6e65 746c 6973 7420 6973 2073 6176 6564  netlist is saved
-0000d120: 2074 6f20 6120 6669 6c65 0d0a 7763 612e   to a file..wca.
-0000d130: 7361 7665 5f6e 6574 6c69 7374 2827 2e2f  save_netlist('./
-0000d140: 7465 7374 6669 6c65 732f 7361 6c6c 656e  testfiles/sallen
-0000d150: 6b65 795f 7763 2e61 7363 2729 0d0a 0d0a  key_wc.asc')....
-0000d160: 0d0a 7763 612e 7275 6e28 2920 2023 2052  ..wca.run()  # R
-0000d170: 756e 7320 7468 6520 7369 6d75 6c61 7469  uns the simulati
-0000d180: 6f6e 2077 6974 6820 7370 6c69 7473 206f  on with splits o
-0000d190: 6620 3130 3020 7275 6e73 2065 6163 680d  f 100 runs each.
-0000d1a0: 0a6c 6f67 7320 3d20 7763 612e 7265 6164  .logs = wca.read
-0000d1b0: 5f6c 6f67 6669 6c65 7328 2920 2020 2320  _logfiles()   # 
-0000d1c0: 5265 6164 7320 7468 6520 6c6f 6720 6669  Reads the log fi
-0000d1d0: 6c65 7320 616e 6420 7374 6f72 6573 2074  les and stores t
-0000d1e0: 6865 2072 6573 756c 7473 2069 6e20 7468  he results in th
-0000d1f0: 6520 7265 7375 6c74 7320 6174 7472 6962  e results attrib
-0000d200: 7574 650d 0a6c 6f67 732e 6578 706f 7274  ute..logs.export
-0000d210: 5f64 6174 6128 272e 2f74 656d 705f 7763  _data('./temp_wc
-0000d220: 612f 6461 7461 2e63 7376 2729 2020 2320  a/data.csv')  # 
-0000d230: 4578 706f 7274 7320 7468 6520 6461 7461  Exports the data
-0000d240: 2074 6f20 6120 6373 7620 6669 6c65 0d0a   to a csv file..
-0000d250: 0d0a 7072 696e 7428 2257 6f72 7374 2063  ..print("Worst c
-0000d260: 6173 6520 7265 7375 6c74 733a 2229 0d0a  ase results:")..
-0000d270: 666f 7220 7061 7261 6d20 696e 2028 2766  for param in ('f
-0000d280: 6375 7427 2c20 2766 6375 745f 4652 4f4d  cut', 'fcut_FROM
-0000d290: 2729 3a0d 0a20 2020 2070 7269 6e74 2866  '):..    print(f
-0000d2a0: 227b 7061 7261 6d7d 3a20 6d69 6e3a 7b6c  "{param}: min:{l
-0000d2b0: 6f67 732e 6d69 6e5f 6d65 6173 7572 655f  ogs.min_measure_
-0000d2c0: 7661 6c75 6528 7061 7261 6d29 7d20 6d61  value(param)} ma
-0000d2d0: 783a 7b6c 6f67 732e 6d61 785f 6d65 6173  x:{logs.max_meas
-0000d2e0: 7572 655f 7661 6c75 6528 7061 7261 6d29  ure_value(param)
-0000d2f0: 7d22 290d 0a0d 0a77 6361 2e63 6c65 616e  }")....wca.clean
-0000d300: 7570 5f66 696c 6573 2829 2020 2320 4465  up_files()  # De
-0000d310: 6c65 7465 7320 7468 6520 7465 6d70 6f72  letes the tempor
-0000d320: 6172 7920 6669 6c65 730d 0a60 6060 0d0a  ary files..```..
-0000d330: 5768 656e 206f 7065 6e69 6e67 2074 6865  When opening the
-0000d340: 2063 7265 6174 6564 2073 616c 6c65 6e6b   created sallenk
-0000d350: 6579 5f77 632e 6e65 7420 6669 6c65 2c20  ey_wc.net file, 
-0000d360: 7765 2063 616e 2073 6565 2074 6861 7420  we can see that 
-0000d370: 7468 6520 666f 6c6c 6f77 696e 6720 6369  the following ci
-0000d380: 7263 7569 742e 0d0a 0d0a 215b 5361 6c6c  rcuit.....![Sall
-0000d390: 656e 2d4b 6579 2041 6d70 6c69 6669 6572  en-Key Amplifier
-0000d3a0: 2077 6974 6820 5743 415d 282e 2f64 6f63   with WCA](./doc
-0000d3b0: 2f6d 6f64 756c 6573 2f73 616c 6c65 6e6b  /modules/sallenk
-0000d3c0: 6579 5f77 632e 706e 6720 2253 616c 6c65  ey_wc.png "Salle
-0000d3d0: 6e2d 4b65 7920 416d 706c 6966 6965 7220  n-Key Amplifier 
-0000d3e0: 7769 7468 2057 4341 2229 0d0a 0d0a 5468  with WCA")....Th
-0000d3f0: 6520 666f 6c6c 6f77 696e 6720 7570 6461  e following upda
-0000d400: 7465 7320 7765 7265 206d 6164 6520 746f  tes were made to
-0000d410: 2074 6865 2063 6972 6375 6974 3a0d 0a2d   the circuit:..-
-0000d420: 2054 6865 2076 616c 7565 206f 6620 6561   The value of ea
-0000d430: 6368 2063 6f6d 706f 6e65 6e74 2077 6173  ch component was
-0000d440: 2072 6570 6c61 6365 6420 6279 2061 2066   replaced by a f
-0000d450: 756e 6374 696f 6e20 7468 6174 2067 656e  unction that gen
-0000d460: 6572 6174 6573 2061 206e 6f6d 696e 616c  erates a nominal
-0000d470: 2c20 6d69 6e69 6d75 6d20 616e 6420 6d61  , minimum and ma
-0000d480: 7869 6d75 6d20 7661 6c75 6520 6465 7065  ximum value depe
-0000d490: 6e64 696e 670d 0a6f 6e20 7468 6520 7275  nding..on the ru
-0000d4a0: 6e20 7061 7261 6d65 7465 7220 616e 6420  n parameter and 
-0000d4b0: 6973 2061 7373 6967 6e65 6420 6120 756e  is assigned a un
-0000d4c0: 6971 7565 2069 6e64 6578 206e 756d 6265  ique index numbe
-0000d4d0: 722e 2028 5231 3d30 2c20 566f 733d 312c  r. (R1=0, Vos=1,
-0000d4e0: 2052 323d 322c 202e 2e2e 2056 323d 372c   R2=2, ... V2=7,
-0000d4f0: 2056 494e 3d38 290d 0a54 6865 2075 6e69   VIN=8)..The uni
-0000d500: 7175 6520 6e75 6d62 6572 2063 6f72 7265  que number corre
-0000d510: 7370 6f6e 6473 2074 6f20 7468 6520 6269  sponds to the bi
-0000d520: 7420 706f 7369 7469 6f6e 206f 6620 7468  t position of th
-0000d530: 6520 7275 6e20 7061 7261 6d65 7465 722e  e run parameter.
-0000d540: 2042 6974 2030 2063 6f72 7265 7370 6f6e   Bit 0 correspon
-0000d550: 6473 2074 6f20 7468 6520 6d69 6e69 6d75  ds to the minimu
-0000d560: 6d20 7661 6c75 6520 616e 640d 0a62 6974  m value and..bit
-0000d570: 2031 2063 6f72 7265 7370 6f6e 6473 2074   1 corresponds t
-0000d580: 6f20 7468 6520 6d61 7869 6d75 6d20 7661  o the maximum va
-0000d590: 6c75 652e 2043 616c 6375 6c61 7469 6e67  lue. Calculating
-0000d5a0: 2061 6c6c 2070 6f73 7369 626c 6520 7065   all possible pe
-0000d5b0: 726d 7574 6174 696f 6e73 206f 6620 6d61  rmutations of ma
-0000d5c0: 7869 6d75 6d20 616e 6420 6d69 6e69 6d75  ximum and minimu
-0000d5d0: 6d20 7661 6c75 6573 2066 6f72 2065 6163  m values for eac
-0000d5e0: 680d 0a63 6f6d 706f 6e65 6e74 2c20 7765  h..component, we
-0000d5f0: 2067 6574 2032 2a2a 3920 3d20 3531 3220   get 2**9 = 512 
-0000d600: 706f 7373 6962 6c65 2063 6f6d 6269 6e61  possible combina
-0000d610: 7469 6f6e 732e 2054 6869 7320 6d61 7073  tions. This maps
-0000d620: 2069 6e74 6f20 6120 3920 6269 7420 6269   into a 9 bit bi
-0000d630: 6e61 7279 206e 756d 6265 722c 2077 6869  nary number, whi
-0000d640: 6368 2069 7320 7468 6520 7275 6e20 7061  ch is the run pa
-0000d650: 7261 6d65 7465 722e 0d0a 2d20 5468 6520  rameter...- The 
-0000d660: 2e73 7465 7020 7061 7261 6d20 7275 6e20  .step param run 
-0000d670: 636f 6d6d 616e 6420 7761 7320 6164 6465  command was adde
-0000d680: 6420 746f 2074 6865 206e 6574 6c69 7374  d to the netlist
-0000d690: 2e20 4974 2073 7461 7274 7320 6174 202d  . It starts at -
-0000d6a0: 3120 7768 6963 6820 6974 2773 2074 6865  1 which it's the
-0000d6b0: 206e 6f6d 696e 616c 2076 616c 7565 2073   nominal value s
-0000d6c0: 696d 756c 6174 696f 6e2c 2074 6865 6e20  imulation, then 
-0000d6d0: 300d 0a77 6869 6368 2063 6f72 7265 7370  0..which corresp
-0000d6e0: 6f6e 6473 2074 6f20 7468 6520 6d69 6e69  onds to the mini
-0000d6f0: 6d75 6d20 7661 6c75 6520 666f 7220 6561  mum value for ea
-0000d700: 6368 2063 6f6d 706f 6e65 6e74 2c20 7468  ch component, th
-0000d710: 656e 2069 7420 6d61 6b65 7320 616c 6c20  en it makes all 
-0000d720: 636f 6d62 696e 6174 696f 6e73 206f 6620  combinations of 
-0000d730: 6d69 6e69 6d75 6d20 616e 6420 6d61 7869  minimum and maxi
-0000d740: 6d75 6d20 7661 6c75 6573 200d 0a75 6e74  mum values ..unt
-0000d750: 696c 2035 3131 2c20 7768 6963 6820 6973  il 511, which is
-0000d760: 2074 6865 2073 696d 756c 6174 696f 6e20   the simulation 
-0000d770: 7769 7468 2061 6c6c 206d 6178 696d 756d  with all maximum
-0000d780: 2076 616c 7565 732e 0d0a 2d20 4120 6465   values...- A de
-0000d790: 6661 756c 7420 7661 6c75 6520 666f 7220  fault value for 
-0000d7a0: 7468 6520 7275 6e20 7061 7261 6d65 7465  the run paramete
-0000d7b0: 7220 7761 7320 6164 6465 642e 2054 6869  r was added. Thi
-0000d7c0: 7320 6973 2075 7365 6675 6c20 6966 2074  s is useful if t
-0000d7d0: 6865 202e 7374 6570 2070 6172 616d 2072  he .step param r
-0000d7e0: 756e 2069 7320 636f 6d6d 656e 7465 6420  un is commented 
-0000d7f0: 6f75 742e 0d0a 2d20 5468 6520 5231 2074  out...- The R1 t
-0000d800: 6f6c 6572 616e 6365 2069 7320 6469 6666  olerance is diff
-0000d810: 6572 656e 7420 6672 6f6d 2074 6865 206f  erent from the o
-0000d820: 7468 6572 2072 6573 6973 746f 7273 2e20  ther resistors. 
-0000d830: 5468 6973 2069 7320 6265 6361 7573 6520  This is because 
-0000d840: 7468 6520 746f 6c65 7261 6e63 6520 7761  the tolerance wa
-0000d850: 7320 6578 706c 6963 6974 6c79 2073 6574  s explicitly set
-0000d860: 2066 6f72 2052 312e 0d0a 2d20 5468 6520   for R1...- The 
-0000d870: 7763 2829 2066 756e 6374 696f 6e20 6973  wc() function is
-0000d880: 2061 6464 6564 2074 6f20 7468 6520 6369   added to the ci
-0000d890: 7263 7569 742e 2054 6869 7320 6675 6e63  rcuit. This func
-0000d8a0: 7469 6f6e 2069 7320 7573 6564 2074 6f20  tion is used to 
-0000d8b0: 6361 6c63 756c 6174 6520 7468 6520 776f  calculate the wo
-0000d8c0: 7273 7420 6361 7365 2076 616c 7565 2066  rst case value f
-0000d8d0: 6f72 2065 6163 6820 636f 6d70 6f6e 656e  or each componen
-0000d8e0: 742c 0d0a 6769 7665 6e20 6120 746f 6c65  t,..given a tole
-0000d8f0: 7261 6e63 6520 7661 6c75 6520 616e 6420  rance value and 
-0000d900: 6974 7320 7265 7370 6563 7469 7665 2069  its respective i
-0000d910: 6e64 6578 2e0d 0a2d 2054 6865 2077 6331  ndex...- The wc1
-0000d920: 2829 2066 756e 6374 696f 6e20 6973 2061  () function is a
-0000d930: 6464 6564 2074 6f20 7468 6520 6369 7263  dded to the circ
-0000d940: 7569 742e 2054 6869 7320 6675 6e63 7469  uit. This functi
-0000d950: 6f6e 2069 7320 7573 6564 2074 6f20 6361  on is used to ca
-0000d960: 6c63 756c 6174 6520 7468 6520 776f 7273  lculate the wors
-0000d970: 7420 6361 7365 2076 616c 7565 2066 6f72  t case value for
-0000d980: 2065 6163 6820 636f 6d70 6f6e 656e 742c   each component,
-0000d990: 0d0a 6769 7665 6e20 6120 6d69 6e69 6d75  ..given a minimu
-0000d9a0: 6d20 616e 6420 6d61 7869 6d75 6d20 7661  m and maximum va
-0000d9b0: 6c75 6520 616e 6420 6974 7320 7265 7370  lue and its resp
-0000d9c0: 6563 7469 7665 2069 6e64 6578 2e0d 0a0d  ective index....
-0000d9d0: 0a23 2323 204c 5453 7465 7073 2e70 7920  .### LTSteps.py 
-0000d9e0: 2323 230d 0a0d 0a54 6869 7320 6d6f 6475  ###....This modu
-0000d9f0: 6c65 2064 6566 696e 6573 2061 2063 6c61  le defines a cla
-0000da00: 7373 2074 6861 7420 6361 6e20 6265 2075  ss that can be u
-0000da10: 7365 6420 746f 2070 6172 7365 204c 5453  sed to parse LTS
-0000da20: 7069 6365 206c 6f67 2066 696c 6573 2077  pice log files w
-0000da30: 6865 7265 2074 6865 2069 6e66 6f72 6d61  here the informa
-0000da40: 7469 6f6e 2061 626f 7574 202e 5354 4550  tion about .STEP
-0000da50: 2069 6e66 6f72 6d61 7469 6f6e 2069 730d   information is.
-0000da60: 0a77 7269 7474 656e 2e20 5468 6572 6520  .written. There 
-0000da70: 6172 6520 7477 6f20 706f 7373 6962 6c65  are two possible
-0000da80: 2075 7361 6765 7320 6f66 2074 6869 7320   usages of this 
-0000da90: 6d6f 6475 6c65 2c20 6569 7468 6572 2070  module, either p
-0000daa0: 726f 6772 616d 6d61 7469 6361 6c6c 7920  rogrammatically 
-0000dab0: 6279 2069 6d70 6f72 7469 6e67 2074 6865  by importing the
-0000dac0: 206d 6f64 756c 6520 616e 6420 7468 656e   module and then
-0000dad0: 0d0a 6163 6365 7373 696e 6720 6461 7461  ..accessing data
-0000dae0: 2074 6872 6f75 6768 2074 6865 2063 6c61   through the cla
-0000daf0: 7373 2061 7320 6578 656d 706c 6966 6965  ss as exemplifie
-0000db00: 6420 6865 7265 3a0d 0a0d 0a60 6060 7079  d here:....```py
-0000db10: 7468 6f6e 0d0a 6672 6f6d 2050 794c 5453  thon..from PyLTS
-0000db20: 7069 6365 2e6c 6f67 2e6c 7473 7465 7073  pice.log.ltsteps
-0000db30: 2069 6d70 6f72 7420 4c54 5370 6963 654c   import LTSpiceL
-0000db40: 6f67 5265 6164 6572 0d0a 0d0a 6461 7461  ogReader....data
-0000db50: 203d 204c 5453 7069 6365 4c6f 6752 6561   = LTSpiceLogRea
-0000db60: 6465 7228 2242 6174 6368 5f54 6573 745f  der("Batch_Test_
-0000db70: 4144 3832 305f 3135 2e6c 6f67 2229 0d0a  AD820_15.log")..
-0000db80: 0d0a 7072 696e 7428 224e 756d 6265 7220  ..print("Number 
-0000db90: 6f66 2073 7465 7073 2020 3a22 2c20 6461  of steps  :", da
-0000dba0: 7461 2e73 7465 705f 636f 756e 7429 0d0a  ta.step_count)..
-0000dbb0: 7374 6570 5f6e 616d 6573 203d 2064 6174  step_names = dat
-0000dbc0: 612e 6765 745f 7374 6570 5f76 6172 7328  a.get_step_vars(
-0000dbd0: 290d 0a6d 6561 735f 6e61 6d65 7320 3d20  )..meas_names = 
-0000dbe0: 6461 7461 2e67 6574 5f6d 6561 7375 7265  data.get_measure
-0000dbf0: 5f6e 616d 6573 2829 0d0a 0d0a 2320 5072  _names()....# Pr
-0000dc00: 696e 7469 6e67 2048 6561 6465 7273 0d0a  inting Headers..
-0000dc10: 7072 696e 7428 2720 272e 6a6f 696e 285b  print(' '.join([
-0000dc20: 6622 7b73 7465 703a 3135 737d 2220 666f  f"{step:15s}" fo
-0000dc30: 7220 7374 6570 2069 6e20 7374 6570 5f6e  r step in step_n
-0000dc40: 616d 6573 5d29 2c20 656e 643d 2727 2920  ames]), end='') 
-0000dc50: 2023 2050 7269 6e74 2073 7465 7073 206e   # Print steps n
-0000dc60: 616d 6573 2077 6974 6820 6e6f 206e 6577  ames with no new
-0000dc70: 206c 696e 650d 0a70 7269 6e74 2827 2027   line..print(' '
-0000dc80: 2e6a 6f69 6e28 5b66 227b 6e61 6d65 3a31  .join([f"{name:1
-0000dc90: 3573 7d22 2066 6f72 206e 616d 6520 696e  5s}" for name in
-0000dca0: 206d 6561 735f 6e61 6d65 735d 292c 2065   meas_names]), e
-0000dcb0: 6e64 3d27 5c6e 2729 0d0a 2320 5072 696e  nd='\n')..# Prin
-0000dcc0: 7469 6e67 2064 6174 610d 0a66 6f72 2069  ting data..for i
-0000dcd0: 2069 6e20 7261 6e67 6528 6461 7461 2e73   in range(data.s
-0000dce0: 7465 705f 636f 756e 7429 3a0d 0a20 2020  tep_count):..   
-0000dcf0: 2070 7269 6e74 2827 2027 2e6a 6f69 6e28   print(' '.join(
-0000dd00: 5b66 227b 6461 7461 5b73 7465 705d 5b69  [f"{data[step][i
-0000dd10: 5d3a 3135 7d22 2066 6f72 2073 7465 7020  ]:15}" for step 
-0000dd20: 696e 2073 7465 705f 6e61 6d65 735d 292c  in step_names]),
-0000dd30: 2065 6e64 3d27 2729 2020 2320 5072 696e   end='')  # Prin
-0000dd40: 7420 7374 6570 7320 6e61 6d65 7320 7769  t steps names wi
-0000dd50: 7468 206e 6f20 6e65 7720 6c69 6e65 0d0a  th no new line..
-0000dd60: 2020 2020 7072 696e 7428 2720 272e 6a6f      print(' '.jo
-0000dd70: 696e 285b 6622 7b64 6174 615b 6e61 6d65  in([f"{data[name
-0000dd80: 5d5b 695d 3a31 357d 2220 666f 7220 6e61  ][i]:15}" for na
-0000dd90: 6d65 2069 6e20 6d65 6173 5f6e 616d 6573  me in meas_names
-0000dda0: 5d29 2c20 656e 643d 275c 6e27 2920 2023  ]), end='\n')  #
-0000ddb0: 2050 7269 6e74 2048 6561 6465 720d 0a0d   Print Header...
-0000ddc0: 0a70 7269 6e74 2822 546f 7461 6c20 6e75  .print("Total nu
-0000ddd0: 6d62 6572 206f 6620 6d65 6173 7572 6573  mber of measures
-0000dde0: 2066 6f75 6e64 203a 222c 2064 6174 612e   found :", data.
-0000ddf0: 6d65 6173 7572 655f 636f 756e 7429 0d0a  measure_count)..
-0000de00: 6060 600d 0a0d 0a54 6865 2073 6563 6f6e  ```....The secon
-0000de10: 6420 706f 7373 6962 696c 6974 7920 6973  d possibility is
-0000de20: 2074 6f20 7573 6520 7468 6520 6d6f 6475   to use the modu
-0000de30: 6c65 2064 6972 6563 746c 7920 6f6e 2074  le directly on t
-0000de40: 6865 2063 6f6d 6d61 6e64 206c 696e 650d  he command line.
-0000de50: 0a0d 0a23 2043 6f6d 6d61 6e64 204c 696e  ...# Command Lin
-0000de60: 6520 496e 7465 7266 6163 6520 230d 0a0d  e Interface #...
-0000de70: 0a23 2323 206c 7473 7465 7073 2e65 7865  .### ltsteps.exe
-0000de80: 2023 2323 0d0a 0d0a 5468 6520 3c66 696c   ###....The <fil
-0000de90: 656e 616d 653e 2063 616e 2062 6520 6569  ename> can be ei
-0000dea0: 7468 6572 2062 6520 6120 6c6f 6720 6669  ther be a log fi
-0000deb0: 6c65 2028 2e6c 6f67 292c 2061 2064 6174  le (.log), a dat
-0000dec0: 6120 6578 706f 7274 2066 696c 6520 282e  a export file (.
-0000ded0: 7478 7429 206f 7220 6120 6d65 6173 7572  txt) or a measur
-0000dee0: 656d 656e 7420 6f75 7470 7574 2066 696c  ement output fil
-0000def0: 6520 282e 6d65 6173 290d 0a54 6869 7320  e (.meas)..This 
-0000df00: 7769 6c6c 2070 726f 6365 7373 2061 6c6c  will process all
-0000df10: 2074 6865 2064 6174 6120 616e 6420 6578   the data and ex
-0000df20: 706f 7274 2069 7420 6175 746f 6d61 7469  port it automati
-0000df30: 6361 6c6c 7920 696e 746f 2061 2074 6578  cally into a tex
-0000df40: 7420 6669 6c65 2077 6974 6820 7468 6520  t file with the 
-0000df50: 6578 7465 6e73 696f 6e20 2874 6c6f 672c  extension (tlog,
-0000df60: 2074 7376 2c20 746d 6561 7329 0d0a 7768   tsv, tmeas)..wh
-0000df70: 6572 6520 7468 6520 6461 7461 2072 6561  ere the data rea
-0000df80: 6420 6973 2066 6f72 6d61 7474 6564 2069  d is formatted i
-0000df90: 6e74 6f20 6120 6d6f 7265 2063 6f6e 7665  nto a more conve
-0000dfa0: 6e69 656e 7420 7461 6220 7365 7061 7261  nient tab separa
-0000dfb0: 7465 6420 666f 726d 6174 2e20 496e 2063  ted format. In c
-0000dfc0: 6173 6520 7468 6520 3c6c 6f67 6669 6c65  ase the <logfile
-0000dfd0: 3e20 6973 206e 6f74 2070 726f 7669 6465  > is not provide
-0000dfe0: 642c 2074 6865 0d0a 7363 7269 7074 2077  d, the..script w
-0000dff0: 696c 6c20 7363 616e 2074 6865 2064 6972  ill scan the dir
-0000e000: 6563 746f 7279 2061 6e64 2070 726f 6365  ectory and proce
-0000e010: 7373 2074 6865 206e 6577 6573 7420 6c6f  ss the newest lo
-0000e020: 672c 2074 7874 206f 7220 6f75 7420 6669  g, txt or out fi
-0000e030: 6c65 2066 6f75 6e64 2e0d 0a0d 0a23 2323  le found.....###
-0000e040: 2068 6973 746f 6772 616d 2e65 7865 2023   histogram.exe #
-0000e050: 2323 0d0a 0d0a 5468 6973 206d 6f64 756c  ##....This modul
-0000e060: 6520 7573 6573 2074 6865 2064 6174 6120  e uses the data 
-0000e070: 696e 7369 6465 206f 6e20 7468 6520 6669  inside on the fi
-0000e080: 6c65 6e61 6d65 2074 6f20 7072 6f64 7563  lename to produc
-0000e090: 6520 6120 6869 7374 6f67 7261 6d20 696d  e a histogram im
-0000e0a0: 6167 652e 0d0a 0d0a 6060 600d 0a55 7361  age.....```..Usa
-0000e0b0: 6765 3a20 4869 7374 6f67 7261 6d2e 7079  ge: Histogram.py
-0000e0c0: 205b 6f70 7469 6f6e 735d 204c 4f47 5f46   [options] LOG_F
-0000e0d0: 494c 4520 5452 4143 450d 0a0d 0a4f 7074  ILE TRACE....Opt
-0000e0e0: 696f 6e73 3a0d 0a20 202d 2d76 6572 7369  ions:..  --versi
-0000e0f0: 6f6e 2020 2020 2020 2020 2020 2020 2073  on             s
-0000e100: 686f 7720 7072 6f67 7261 6d27 7320 7665  how program's ve
-0000e110: 7273 696f 6e20 6e75 6d62 6572 2061 6e64  rsion number and
-0000e120: 2065 7869 740d 0a20 202d 682c 202d 2d68   exit..  -h, --h
-0000e130: 656c 7020 2020 2020 2020 2020 2020 2073  elp            s
-0000e140: 686f 7720 7468 6973 2068 656c 7020 6d65  how this help me
-0000e150: 7373 6167 6520 616e 6420 6578 6974 0d0a  ssage and exit..
-0000e160: 2020 2d73 2053 4947 4d41 2c20 2d2d 7369    -s SIGMA, --si
-0000e170: 676d 613d 5349 474d 410d 0a20 2020 2020  gma=SIGMA..     
-0000e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e190: 2020 2053 6967 6d61 2074 6f20 6265 2075     Sigma to be u
-0000e1a0: 7365 6420 696e 2074 6865 2064 6973 7472  sed in the distr
-0000e1b0: 6962 7574 696f 6e20 6669 742e 2044 6566  ibution fit. Def
-0000e1c0: 6175 6c74 3d33 0d0a 2020 2d6e 204e 4249  ault=3..  -n NBI
-0000e1d0: 4e53 2c20 2d2d 6e62 696e 733d 4e42 494e  NS, --nbins=NBIN
-0000e1e0: 530d 0a20 2020 2020 2020 2020 2020 2020  S..             
-0000e1f0: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
-0000e200: 7220 6f66 2062 696e 7320 746f 2062 6520  r of bins to be 
-0000e210: 7573 6564 2069 6e20 7468 6520 6869 7374  used in the hist
-0000e220: 6f67 7261 6d2e 2044 6566 6175 6c74 3d32  ogram. Default=2
-0000e230: 300d 0a20 202d 6320 4649 4c54 4552 532c  0..  -c FILTERS,
-0000e240: 202d 2d63 6f6e 6469 7469 6f6e 3d46 494c   --condition=FIL
-0000e250: 5445 5253 0d0a 2020 2020 2020 2020 2020  TERS..          
-0000e260: 2020 2020 2020 2020 2020 2020 2020 4669                Fi
-0000e270: 6c74 6572 2063 6f6e 6469 7469 6f6e 2077  lter condition w
-0000e280: 7269 7465 6e20 696e 2070 7974 686f 6e2e  riten in python.
-0000e290: 204d 6f72 6520 7468 616e 206f 6e65 0d0a   More than one..
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2b0: 2020 2020 2020 2020 6578 7072 6573 7369          expressi
-0000e2c0: 6f6e 2063 616e 2062 6520 6164 6465 6420  on can be added 
-0000e2d0: 6275 7420 6561 6368 2065 7870 7265 7373  but each express
-0000e2e0: 696f 6e20 7368 6f75 6c64 2062 650d 0a20  ion should be.. 
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e300: 2020 2020 2020 2070 7265 6365 6465 6420         preceded 
-0000e310: 6279 202d 632e 2045 5841 4d50 4c45 3a20  by -c. EXAMPLE: 
-0000e320: 2d63 2056 284e 3030 3129 3e34 202d 6320  -c V(N001)>4 -c 
-0000e330: 7061 7261 6d65 7465 723d 3d31 0d0a 2020  parameter==1..  
-0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e350: 2020 2020 2020 2d63 2020 4928 5631 293c        -c  I(V1)<
-0000e360: 302e 350d 0a20 202d 6620 464f 524d 4154  0.5..  -f FORMAT
-0000e370: 2c20 2d2d 666f 726d 6174 3d46 4f52 4d41  , --format=FORMA
-0000e380: 540d 0a20 2020 2020 2020 2020 2020 2020  T..             
-0000e390: 2020 2020 2020 2020 2020 2046 6f72 6d61             Forma
-0000e3a0: 7420 7374 7269 6e67 2066 6f72 2074 6865  t string for the
-0000e3b0: 2058 2061 7869 732e 2045 7861 6d70 6c65   X axis. Example
-0000e3c0: 3a20 2d66 2025 332e 3466 0d0a 2020 2d74  : -f %3.4f..  -t
-0000e3d0: 2054 4954 4c45 2c20 2d2d 7469 746c 653d   TITLE, --title=
-0000e3e0: 5449 544c 450d 0a20 2020 2020 2020 2020  TITLE..         
-0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000e400: 6974 6c65 2074 6f20 6170 7065 6172 206f  itle to appear o
-0000e410: 6e20 7468 6520 746f 7020 6f66 2074 6865  n the top of the
-0000e420: 2068 6973 746f 6772 616d 2e0d 0a20 202d   histogram...  -
-0000e430: 7220 5241 4e47 452c 202d 2d72 616e 6765  r RANGE, --range
-0000e440: 3d52 414e 4745 0d0a 2020 2020 2020 2020  =RANGE..        
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 5261 6e67 6520 6f66 2074 6865 2058 2061  Range of the X a
-0000e470: 7869 7320 746f 2075 7365 2066 6f72 2074  xis to use for t
-0000e480: 6865 2068 6973 746f 6772 616d 2069 6e20  he histogram in 
-0000e490: 7468 650d 0a20 2020 2020 2020 2020 2020  the..           
-0000e4a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000e4b0: 6d20 6d69 6e3a 6d61 782e 2045 7861 6d70  m min:max. Examp
-0000e4c0: 6c65 3a20 2d72 202d 313a 310d 0a20 202d  le: -r -1:1..  -
-0000e4d0: 432c 202d 2d63 6c69 7062 6f61 7264 2020  C, --clipboard  
-0000e4e0: 2020 2020 2049 6620 7468 6520 6461 7461       If the data
-0000e4f0: 2066 726f 6d20 7468 6520 636c 6970 626f   from the clipbo
-0000e500: 6172 6420 6973 2074 6f20 6265 2075 7365  ard is to be use
-0000e510: 642e 0d0a 2020 2d69 2049 4d41 4745 4649  d...  -i IMAGEFI
-0000e520: 4c45 2c20 2d2d 696d 6167 653d 494d 4147  LE, --image=IMAG
-0000e530: 4546 494c 450d 0a20 2020 2020 2020 2020  EFILE..         
-0000e540: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-0000e550: 616d 6520 6f66 2074 6865 2069 6d61 6765  ame of the image
-0000e560: 2046 696c 652e 2065 7874 656e 7369 6f6e   File. extension
-0000e570: 2027 706e 6727 2020 2020 0d0a 6060 600d   'png'    ..```.
-0000e580: 0a0d 0a23 2323 2072 6177 636f 6e76 6572  ...### rawconver
-0000e590: 742e 6578 6520 2323 230d 0a0d 0a41 2074  t.exe ###....A t
-0000e5a0: 6f6f 6c20 746f 2063 6f6e 7665 7274 202e  ool to convert .
-0000e5b0: 7261 7720 6669 6c65 7320 696e 746f 2063  raw files into c
-0000e5c0: 7376 206f 7220 4578 6365 6c20 6669 6c65  sv or Excel file
-0000e5d0: 732e 0d0a 0d0a 6060 600d 0a55 7361 6765  s.....```..Usage
-0000e5e0: 3a20 7261 775f 636f 6e76 6572 742e 6578  : raw_convert.ex
-0000e5f0: 6520 5b6f 7074 696f 6e73 5d20 3c72 6177  e [options] <raw
-0000e600: 6669 6c65 3e20 3c74 7261 6365 5f6c 6973  file> <trace_lis
-0000e610: 743e 0d0a 0d0a 4f70 7469 6f6e 733a 0d0a  t>....Options:..
-0000e620: 2020 2d2d 7665 7273 696f 6e20 2020 2020    --version     
-0000e630: 2020 2020 2020 2020 7368 6f77 2070 726f          show pro
-0000e640: 6772 616d 2773 2076 6572 7369 6f6e 206e  gram's version n
-0000e650: 756d 6265 7220 616e 6420 6578 6974 0d0a  umber and exit..
-0000e660: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
-0000e670: 2020 2020 2020 2020 7368 6f77 2074 6869          show thi
-0000e680: 7320 6865 6c70 206d 6573 7361 6765 2061  s help message a
-0000e690: 6e64 2065 7869 740d 0a20 202d 6f20 4649  nd exit..  -o FI
-0000e6a0: 4c45 2c20 2d2d 6f75 7470 7574 3d46 494c  LE, --output=FIL
-0000e6b0: 450d 0a20 2020 2020 2020 2020 2020 2020  E..             
-0000e6c0: 2020 2020 2020 2020 2020 204f 7574 7075             Outpu
-0000e6d0: 7420 6669 6c65 206e 616d 652e 2055 7365  t file name. Use
-0000e6e0: 202e 6373 7620 666f 7220 4353 5620 6f75   .csv for CSV ou
-0000e6f0: 7470 7574 2c20 2e78 6c73 7820 666f 720d  tput, .xlsx for.
-0000e700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e710: 2020 2020 2020 2020 2045 7863 656c 206f           Excel o
-0000e720: 7574 7075 740d 0a20 202d 632c 202d 2d63  utput..  -c, --c
-0000e730: 6c69 7062 6f61 7264 2020 2020 2020 204f  lipboard       O
-0000e740: 7574 7075 7420 746f 2063 6c69 7062 6f61  utput to clipboa
-0000e750: 7264 0d0a 2020 2d76 2c20 2d2d 7665 7262  rd..  -v, --verb
-0000e760: 6f73 6520 2020 2020 2020 2020 5665 7262  ose         Verb
-0000e770: 6f73 6520 6f75 7470 7574 0d0a 2020 2d73  ose output..  -s
-0000e780: 2053 4550 4152 4154 4f52 2c20 2d2d 7365   SEPARATOR, --se
-0000e790: 703d 5345 5041 5241 544f 520d 0a20 2020  p=SEPARATOR..   
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7b0: 2020 2020 2056 616c 7565 2073 6570 6172       Value separ
-0000e7c0: 6174 6f72 2066 6f72 2043 5356 206f 7574  ator for CSV out
-0000e7d0: 7075 742e 2044 6566 6175 6c74 3a20 225c  put. Default: "\
-0000e7e0: 7422 203c 5441 423e 0d0a 2020 2020 2020  t" <TAB>..      
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e800: 2020 4578 616d 706c 653a 202d 6420 223b    Example: -d ";
-0000e810: 220d 0a60 6060 0d0a 0d0a 2323 2320 7275  "..```....### ru
-0000e820: 6e5f 7365 7276 6572 2e65 7865 2023 2323  n_server.exe ###
-0000e830: 0d0a 0d0a 5468 6973 2063 6f6d 6d61 6e64  ....This command
-0000e840: 206c 696e 6520 746f 6f6c 2077 6173 206d   line tool was m
-0000e850: 6f76 6564 2074 6f20 7468 6520 7370 6963  oved to the spic
-0000e860: 656c 6962 2070 6163 6b61 6765 2e0d 0a0d  elib package....
-0000e870: 0a23 2323 2053 656d 6944 6576 4f70 5265  .### SemiDevOpRe
-0000e880: 6164 6572 2e70 7920 2323 230d 0a0d 0a54  ader.py ###....T
-0000e890: 6869 7320 6d6f 6475 6c65 2069 7320 7573  his module is us
-0000e8a0: 6564 2074 6f20 7265 6164 2066 726f 6d20  ed to read from 
-0000e8b0: 4c54 5370 6963 6520 6c6f 6720 6669 6c65  LTSpice log file
-0000e8c0: 7320 5365 6d69 636f 6e64 7563 746f 7220  s Semiconductor 
-0000e8d0: 4465 7669 6365 7320 4f70 6572 6174 696e  Devices Operatin
-0000e8e0: 6720 506f 696e 7420 496e 666f 726d 6174  g Point Informat
-0000e8f0: 696f 6e2e 2041 206d 6f72 6520 6465 7461  ion. A more deta
-0000e900: 696c 6564 0d0a 646f 6375 6d65 6e74 6174  iled..documentat
-0000e910: 696f 6e20 6973 2064 6972 6563 746c 7920  ion is directly 
-0000e920: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
-0000e930: 736f 7572 6365 2066 696c 6520 646f 6373  source file docs
-0000e940: 7472 696e 6773 2e0d 0a0d 0a23 2320 4465  trings.....## De
-0000e950: 6275 6720 4c6f 6767 696e 670d 0a0d 0a54  bug Logging....T
-0000e960: 6865 206c 6962 7261 7279 2075 7365 7320  he library uses 
-0000e970: 7468 6520 7374 616e 6461 7264 2060 6c6f  the standard `lo
-0000e980: 6767 696e 6760 206d 6f64 756c 652e 2054  gging` module. T
-0000e990: 6872 6565 2063 6f6e 7665 6e69 656e 6365  hree convenience
-0000e9a0: 2066 756e 6374 696f 6e73 2068 6176 6520   functions have 
-0000e9b0: 6265 656e 2061 6464 6564 2066 6f72 2065  been added for e
-0000e9c0: 6173 696c 7920 6368 616e 6769 6e67 206c  asily changing l
-0000e9d0: 6f67 6769 6e67 0d0a 7365 7474 696e 6773  ogging..settings
-0000e9e0: 2061 6372 6f73 7320 7468 6520 656e 7469   across the enti
-0000e9f0: 7265 206c 6962 7261 7279 2e20 6050 794c  re library. `PyL
-0000ea00: 5453 7069 6365 2e61 6c6c 5f6c 6f67 6765  TSpice.all_logge
-0000ea10: 7273 2829 6020 7265 7475 726e 7320 6120  rs()` returns a 
-0000ea20: 6c69 7374 206f 6620 616c 6c20 7468 6520  list of all the 
-0000ea30: 6c6f 6767 6572 2773 0d0a 6e61 6d65 732c  logger's..names,
-0000ea40: 2060 5079 4c54 5370 6963 652e 7365 745f   `PyLTSpice.set_
-0000ea50: 6c6f 675f 6c65 7665 6c28 6c6f 6767 696e  log_level(loggin
-0000ea60: 672e 4445 4255 4729 600d 0a77 6f75 6c64  g.DEBUG)`..would
-0000ea70: 2073 6574 2074 6865 206c 6962 7261 7279   set the library
-0000ea80: 2773 206c 6f67 6769 6e67 206c 6576 656c  's logging level
-0000ea90: 2074 6f20 6465 6275 672c 2061 6e64 2060   to debug, and `
-0000eaa0: 5079 4c54 5370 6963 652e 6164 645f 6c6f  PyLTSpice.add_lo
-0000eab0: 675f 6861 6e64 6c65 7228 6d79 5f68 616e  g_handler(my_han
-0000eac0: 646c 6572 2960 2077 6f75 6c64 2061 6464  dler)` would add
-0000ead0: 2060 6d79 5f68 616e 646c 6572 6020 6173   `my_handler` as
-0000eae0: 2061 0d0a 6861 6e64 6c65 7220 666f 720d   a..handler for.
-0000eaf0: 0a61 6c6c 206c 6f67 6765 7273 2e0d 0a0d  .all loggers....
-0000eb00: 0a23 2323 2053 696e 676c 6520 4d6f 6475  .### Single Modu
-0000eb10: 6c65 204c 6f67 6769 6e67 0d0a 0d0a 4974  le Logging....It
-0000eb20: 2069 7320 616c 736f 2070 6f73 7369 626c   is also possibl
-0000eb30: 6520 746f 2073 6574 2074 6865 206c 6f67  e to set the log
-0000eb40: 6769 6e67 2073 6574 7469 6e67 7320 666f  ging settings fo
-0000eb50: 7220 6120 7369 6e67 6c65 206d 6f64 756c  r a single modul
-0000eb60: 6520 6279 2075 7369 6e67 2069 7473 206e  e by using its n
-0000eb70: 616d 6520 6163 7175 6972 6564 2066 726f  ame acquired fro
-0000eb80: 6d0d 0a74 6865 2060 5079 4c54 5370 6963  m..the `PyLTSpic
-0000eb90: 652e 616c 6c5f 6c6f 6767 6572 7328 2960  e.all_loggers()`
-0000eba0: 0d0a 6675 6e63 7469 6f6e 2e20 466f 7220  ..function. For 
-0000ebb0: 6578 616d 706c 653a 0d0a 0d0a 6060 6070  example:....```p
-0000ebc0: 7974 686f 6e0d 0a69 6d70 6f72 7420 6c6f  ython..import lo
-0000ebd0: 6767 696e 670d 0a0d 0a6c 6f67 6769 6e67  gging....logging
-0000ebe0: 2e62 6173 6963 436f 6e66 6967 286c 6576  .basicConfig(lev
-0000ebf0: 656c 3d6c 6f67 6769 6e67 2e49 4e46 4f29  el=logging.INFO)
-0000ec00: 2020 2320 5365 7420 7570 2074 6865 2072    # Set up the r
-0000ec10: 6f6f 7420 6c6f 6767 6572 2066 6972 7374  oot logger first
-0000ec20: 0d0a 0d0a 696d 706f 7274 2050 794c 5453  ....import PyLTS
-0000ec30: 7069 6365 2020 2320 496d 706f 7274 2050  pice  # Import P
-0000ec40: 794c 5453 7069 6365 2074 6f20 7365 7420  yLTSpice to set 
-0000ec50: 7468 6520 6c6f 6767 696e 6720 6c65 7665  the logging leve
-0000ec60: 6c73 0d0a 0d0a 5079 4c54 5370 6963 652e  ls....PyLTSpice.
-0000ec70: 7365 745f 6c6f 675f 6c65 7665 6c28 6c6f  set_log_level(lo
-0000ec80: 6767 696e 672e 4445 4255 4729 2020 2320  gging.DEBUG)  # 
-0000ec90: 5365 7420 5079 4c54 5370 6963 6527 7320  Set PyLTSpice's 
-0000eca0: 676c 6f62 616c 206c 6f67 206c 6576 656c  global log level
-0000ecb0: 0d0a 6c6f 6767 696e 672e 6765 744c 6f67  ..logging.getLog
-0000ecc0: 6765 7228 2250 794c 5453 7069 6365 2e52  ger("PyLTSpice.R
-0000ecd0: 6177 5265 6164 2229 2e6c 6576 656c 203d  awRead").level =
-0000ece0: 206c 6f67 6769 6e67 2e57 4152 4e49 4e47   logging.WARNING
-0000ecf0: 2020 2320 5365 7420 7468 6520 6c6f 6720    # Set the log 
-0000ed00: 6c65 7665 6c20 666f 7220 6f6e 6c79 2052  level for only R
-0000ed10: 6177 5265 6164 2074 6f20 7761 726e 696e  awRead to warnin
-0000ed20: 670d 0a60 6060 0d0a 0d0a 576f 756c 6420  g..```....Would 
-0000ed30: 7365 7420 6f6e 6c79 2060 5079 4c54 5370  set only `PyLTSp
-0000ed40: 6963 652e 5261 7752 6561 6460 2066 696c  ice.RawRead` fil
-0000ed50: 6527 7320 6c6f 6767 696e 6720 6c65 7665  e's logging leve
-0000ed60: 6c20 746f 2077 6172 6e69 6e67 2077 6869  l to warning whi
-0000ed70: 6c65 2074 6865 206f 7468 6572 206d 6f64  le the other mod
-0000ed80: 756c 6573 2077 6f75 6c64 2072 656d 6169  ules would remai
-0000ed90: 6e20 6174 2064 6562 7567 206c 6576 656c  n at debug level
-0000eda0: 2e0d 0a5f 4d61 6b65 2073 7572 6520 746f  ..._Make sure to
-0000edb0: 2069 6e69 7469 616c 697a 6520 7468 6520   initialize the 
-0000edc0: 726f 6f74 206c 6f67 6765 7220 6265 666f  root logger befo
-0000edd0: 7265 2069 6d70 6f72 7469 6e67 2074 6865  re importing the
-0000ede0: 206c 6962 7261 7279 2074 6f20 6265 2061   library to be a
-0000edf0: 626c 6520 746f 2073 6565 2074 6865 206c  ble to see the l
-0000ee00: 6f67 732e 5f0d 0a0d 0a23 2320 546f 2077  ogs._....## To w
-0000ee10: 686f 6d20 646f 2049 2074 616c 6b20 746f  hom do I talk to
-0000ee20: 3f20 2323 0d0a 0d0a 2a20 546f 6f6c 7320  ? ##....* Tools 
-0000ee30: 7765 6273 6974 6520 3a20 5b68 7474 7073  website : [https
-0000ee40: 3a2f 2f77 7777 2e6e 756e 6f62 7275 6d2e  ://www.nunobrum.
-0000ee50: 636f 6d2f 7079 6c74 7370 6963 652e 6874  com/pyltspice.ht
-0000ee60: 6d6c 5d28 6874 7470 733a 2f2f 7777 772e  ml](https://www.
-0000ee70: 6e75 6e6f 6272 756d 2e63 6f6d 2f70 796c  nunobrum.com/pyl
-0000ee80: 7473 7069 6365 2e68 746d 6c29 0d0a 2a20  tspice.html)..* 
-0000ee90: 5265 706f 206f 776e 6572 203a 205b 6d65  Repo owner : [me
-0000eea0: 406e 756e 6f62 7275 6d2e 636f 6d5d 286d  @nunobrum.com](m
-0000eeb0: 6169 6c74 6f3a 6d65 406e 756e 6f62 7275  ailto:me@nunobru
-0000eec0: 6d2e 636f 6d29 0d0a 2a20 416c 7465 726e  m.com)..* Altern
-0000eed0: 6174 6976 6520 636f 6e74 6163 7420 3a20  ative contact : 
-0000eee0: 5b6e 756e 6f2e 6272 756d 4067 6d61 696c  [nuno.brum@gmail
-0000eef0: 2e63 6f6d 5d28 6d61 696c 746f 3a6e 756e  .com](mailto:nun
-0000ef00: 6f2e 6272 756d 4067 6d61 696c 2e63 6f6d  o.brum@gmail.com
-0000ef10: 290d 0a0d 0a23 2320 4869 7374 6f72 7920  )....## History 
-0000ef20: 2323 0d0a 2a20 5665 7273 696f 6e20 352e  ##..* Version 5.
-0000ef30: 332e 300d 0a20 202a 2048 6965 7261 7263  3.0..  * Hierarc
-0000ef40: 6869 6361 6c20 5375 7070 6f72 7420 2841  hical Support (A
-0000ef50: 6c69 676e 696e 6720 7769 7468 2074 6865  ligning with the
-0000ef60: 2073 7069 6365 6c69 6220 312e 312e 3129   spicelib 1.1.1)
-0000ef70: 0d0a 2a20 5665 7273 696f 6e20 352e 322e  ..* Version 5.2.
-0000ef80: 330d 0a20 202a 2055 7064 6174 696e 6720  3..  * Updating 
-0000ef90: 6c6f 6767 6572 7320 746f 2075 7365 2074  loggers to use t
-0000efa0: 6865 2022 7370 6963 656c 6962 2220 4944  he "spicelib" ID
-0000efb0: 732e 0d0a 2020 2a20 4669 7869 6e67 2061  s...  * Fixing a
-0000efc0: 7574 6f64 6f63 2065 7272 6f72 730d 0a20  utodoc errors.. 
-0000efd0: 202a 2043 6f72 7265 6374 696e 6720 5665   * Correcting Ve
-0000efe0: 7273 696f 6e20 7265 6665 7265 6e63 6573  rsion references
-0000eff0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 352e  ....* Version 5.
-0000f000: 322e 320d 0a20 202a 2046 6978 6573 206f  2.2..  * Fixes o
-0000f010: 6e20 7468 6520 756e 6974 7465 7374 7320  n the unittests 
-0000f020: 6166 7465 7220 7468 6520 7370 6963 656c  after the spicel
-0000f030: 6962 2075 7064 6174 6520 746f 2031 2e30  ib update to 1.0
-0000f040: 2e34 0d0a 0d0a 2a20 5665 7273 696f 6e20  .4....* Version 
-0000f050: 352e 322e 310d 0a20 202a 2043 6f72 7265  5.2.1..  * Corre
-0000f060: 6374 696f 6e20 6f6e 2074 6865 2072 756e  ction on the run
-0000f070: 5f6d 6f6e 7465 6361 726c 6f2e 7079 2061  _montecarlo.py a
-0000f080: 6e64 2072 756e 5f77 6f72 7374 5f63 6173  nd run_worst_cas
-0000f090: 652e 7079 2065 7861 6d70 6c65 732e 0d0a  e.py examples...
-0000f0a0: 2020 2a20 4669 7865 7320 6f6e 2074 6865    * Fixes on the
-0000f0b0: 2073 7069 6365 6c69 6220 2856 6572 7369   spicelib (Versi
-0000f0c0: 6f6e 2031 2e30 2e33 290d 0a0d 0a2a 2056  on 1.0.3)....* V
-0000f0d0: 6572 7369 6f6e 2035 2e32 0d0a 2020 2a20  ersion 5.2..  * 
-0000f0e0: 5369 6d41 6e61 6c79 7369 7320 7375 7070  SimAnalysis supp
-0000f0f0: 6f72 7469 6e67 2062 6f74 6820 5173 7069  orting both Qspi
-0000f100: 6365 2061 6e64 204c 5453 7069 6365 206c  ce and LTSpice l
-0000f110: 6f67 6669 6c65 732e 0d0a 2020 2a20 4661  ogfiles...  * Fa
-0000f120: 7374 576f 7273 7443 6173 6541 6e61 6c79  stWorstCaseAnaly
-0000f130: 7369 7320 616c 676f 7269 7468 6d20 696d  sis algorithm im
-0000f140: 706c 656d 656e 7465 640d 0a20 202a 2046  plemented..  * F
-0000f150: 6978 206f 6e20 7468 6520 6c6f 6720 7265  ix on the log re
-0000f160: 6164 696e 6720 6f66 2066 6f75 7269 6572  ading of fourier
-0000f170: 2064 6174 612e 0d0a 0d0a 2a20 5665 7273   data.....* Vers
-0000f180: 696f 6e20 352e 310d 0a20 202a 2049 6d70  ion 5.1..  * Imp
-0000f190: 6f72 7461 6e74 2042 7567 6669 7820 6f6e  ortant Bugfix on
-0000f1a0: 2074 6865 204c 5443 6f6d 706c 6578 2063   the LTComplex c
-0000f1b0: 6c61 7373 2e0d 0a20 202a 2046 6978 6573  lass...  * Fixes
-0000f1c0: 2061 6e64 2065 6e68 616e 6369 6e67 2074   and enhancing t
-0000f1d0: 6865 2061 6e61 6c79 7369 7320 746f 6f6c  he analysis tool
-0000f1e0: 6b69 742e 0d0a 2020 2a20 4465 7072 6563  kit...  * Deprec
-0000f1f0: 6174 696e 6720 5370 6963 6545 6469 746f  ating SpiceEdito
-0000f200: 722e 7772 6974 655f 6e65 746c 6973 7420  r.write_netlist 
-0000f210: 696e 2066 6176 6f75 7220 6f66 2073 6176  in favour of sav
-0000f220: 655f 6e65 746c 6973 7428 290d 0a0d 0a2a  e_netlist()....*
-0000f230: 2056 6572 7369 6f6e 2035 2e30 0d0a 2020   Version 5.0..  
-0000f240: 2a20 4d61 6b69 6e67 2074 6869 7320 6c69  * Making this li
-0000f250: 6272 6172 7920 6465 7065 6e64 656e 7420  brary dependent 
-0000f260: 6f6e 2073 7069 6365 6c69 6220 7768 696c  on spicelib whil
-0000f270: 6520 7472 7969 6e67 2074 6f20 6d61 696e  e trying to main
-0000f280: 7461 696e 2062 6163 6b77 6172 6420 636f  tain backward co
-0000f290: 6d70 6174 6962 696c 6974 7920 6173 206d  mpatibility as m
-0000f2a0: 7563 6820 6173 2070 6f73 7369 626c 652e  uch as possible.
-0000f2b0: 200d 0a20 2050 794c 5473 7069 6365 2077   ..  PyLTspice w
-0000f2c0: 696c 6c20 6265 206b 6570 7420 616c 6976  ill be kept aliv
-0000f2d0: 6520 616e 6420 6974 7320 7570 6461 7465  e and its update
-0000f2e0: 2077 696c 6c20 6265 206c 696e 6b65 6420   will be linked 
-0000f2f0: 746f 2074 6865 2073 7069 6365 6c69 622e  to the spicelib.
-0000f300: 2054 6865 206d 6169 6e20 6469 6666 6572   The main differ
-0000f310: 656e 6365 2069 7320 7468 6174 2075 7369  ence is that usi
-0000f320: 6e67 0d0a 2020 5079 4c54 7370 6963 6520  ng..  PyLTspice 
-0000f330: 7769 6c6c 2061 7665 7274 2074 6865 206e  will avert the n
-0000f340: 6565 6420 6f66 2068 6176 696e 6720 746f  eed of having to
-0000f350: 2073 656c 6563 7420 6120 7369 6d75 6c61   select a simula
-0000f360: 746f 7220 696e 2061 6c6c 2072 756e 2063  tor in all run c
-0000f370: 6f6d 6d61 6e64 732e 0d0a 0d0a 2a20 5665  ommands.....* Ve
-0000f380: 7273 696f 6e20 342e 312e 320d 0a20 202a  rsion 4.1.2..  *
-0000f390: 2041 6464 696e 6720 7375 7070 6f72 7420   Adding support 
-0000f3a0: 666f 7220 7468 6520 6e65 7720 5153 5049  for the new QSPI
-0000f3b0: 4345 2073 696d 756c 6174 6f72 0d0a 2020  CE simulator..  
-0000f3c0: 2a20 496d 7072 6f76 696e 6720 7468 6520  * Improving the 
-0000f3d0: 7469 6d65 6f75 7420 6d65 6368 616e 6973  timeout mechanis
-0000f3e0: 6d20 6f6e 2074 6865 2053 696d 5275 6e6e  m on the SimRunn
-0000f3f0: 6572 2063 6c61 7373 0d0a 2020 2a20 4d69  er class..  * Mi
-0000f400: 6e6f 7220 6275 6720 6669 7865 730d 0a0d  nor bug fixes...
-0000f410: 0a2a 2056 6572 7369 6f6e 2034 2e31 2e31  .* Version 4.1.1
-0000f420: 0d0a 2020 2a20 436f 6d70 6c65 7469 6e67  ..  * Completing
-0000f430: 2074 6865 2057 6f72 7374 2d43 6173 6520   the Worst-Case 
-0000f440: 416e 616c 7973 6973 2066 756e 6374 696f  Analysis functio
-0000f450: 6e73 2e20 4164 6469 6e67 2061 2064 6564  ns. Adding a ded
-0000f460: 6963 6174 6564 2065 7861 6d70 6c65 2066  icated example f
-0000f470: 6f72 2069 742e 0d0a 2020 2a20 5265 6661  or it...  * Refa
-0000f480: 6374 6f72 696e 6720 7468 6520 4c54 5370  ctoring the LTSp
-0000f490: 6963 654c 6f67 5265 6164 6572 2063 6c61  iceLogReader cla
-0000f4a0: 7373 2069 6e20 6f72 6465 7220 746f 2075  ss in order to u
-0000f4b0: 7365 2069 7420 6f6e 2074 6865 2041 6e61  se it on the Ana
-0000f4c0: 6c79 7369 7320 746f 6f6c 6b69 740d 0a0d  lysis toolkit...
-0000f4d0: 0a2a 2056 6572 7369 6f6e 2034 2e31 2e30  .* Version 4.1.0
-0000f4e0: 202a 2872 6571 7569 7265 7320 5079 7468   *(requires Pyth
-0000f4f0: 6f6e 2033 2e38 206f 7220 6869 6768 6572  on 3.8 or higher
-0000f500: 292a 0d0a 2020 2020 2a20 4164 6469 6e67  )*..    * Adding
-0000f510: 2061 206e 6577 2063 6c61 7373 2074 6f20   a new class to 
-0000f520: 6d61 6e69 7075 6c61 7465 2064 6972 6563  manipulate direc
-0000f530: 746c 7920 7468 6520 2e61 7363 2066 696c  tly the .asc fil
-0000f540: 6573 2e0d 0a20 2020 202a 204d 6f64 6966  es...    * Modif
-0000f550: 7969 6e67 2061 6c6c 2074 6865 206f 7468  ying all the oth
-0000f560: 6572 2063 6c61 7373 6573 2069 6e20 6f72  er classes in or
-0000f570: 6465 7220 746f 2075 7365 2074 6865 206e  der to use the n
-0000f580: 6577 2063 6c61 7373 2e0d 0a20 2020 202a  ew class...    *
-0000f590: 2041 6464 696e 6720 636c 6173 7365 7320   Adding classes 
-0000f5a0: 746f 2070 6572 666f 726d 204d 6f6e 7465  to perform Monte
-0000f5b0: 6361 726c 6f20 616e 6420 776f 7273 7420  carlo and worst 
-0000f5c0: 6361 7365 2061 6e61 6c79 7369 7320 2854  case analysis (T
-0000f5d0: 6861 6e6b 7320 746f 2040 6d76 616e 7269  hanks to @mvanri
-0000f5e0: 6574 2066 6f72 2068 6973 2073 7461 7274  et for his start
-0000f5f0: 696e 6720 7468 6973 292e 0d0a 2020 2020  ing this)...    
-0000f600: 2a20 5265 6d6f 7669 6e67 2074 6865 2064  * Removing the d
-0000f610: 6570 7265 6361 7465 6420 4c54 5370 6963  eprecated LTSpic
-0000f620: 655f 5261 7752 6561 642e 7079 2c20 4c54  e_RawRead.py, LT
-0000f630: 5370 6963 655f 5261 7757 7269 7465 2e70  Spice_RawWrite.p
-0000f640: 7920 616e 6420 4c54 5370 6963 6542 6174  y and LTSpiceBat
-0000f650: 6368 2e70 7920 6669 6c65 7320 616e 6420  ch.py files and 
-0000f660: 7265 7370 6563 7469 7665 2063 6c61 7373  respective class
-0000f670: 6573 2e0d 0a20 2020 202a 2052 6573 7472  es...    * Restr
-0000f680: 7563 7475 7265 6420 7468 6520 666f 6c64  uctured the fold
-0000f690: 6572 2073 7472 7563 7475 7265 2074 6f20  er structure to 
-0000f6a0: 6265 206d 6f72 6520 696e 206c 696e 6520  be more in line 
-0000f6b0: 7769 7468 2074 6865 2050 7974 686f 6e20  with the Python 
-0000f6c0: 7374 616e 6461 7264 732e 0d0a 2020 2020  standards...    
-0000f6d0: 2a20 4164 6465 6420 616e 2045 7861 6d70  * Added an Examp
-0000f6e0: 6c65 7320 666f 6c64 6572 2077 6974 6820  les folder with 
-0000f6f0: 736f 6d65 2065 7861 6d70 6c65 7320 6f6e  some examples on
-0000f700: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
-0000f710: 6c69 6272 6172 792e 0d0a 0d0a 2a20 5665  library.....* Ve
-0000f720: 7273 696f 6e20 342e 302e 360d 0a20 2020  rsion 4.0.6..   
-0000f730: 202a 2046 6978 696e 6720 6973 7375 6520   * Fixing issue 
-0000f740: 7769 7468 2074 6865 2077 7269 7465 5f6e  with the write_n
-0000f750: 6574 6c69 7374 2829 2066 756e 6374 696f  etlist() functio
-0000f760: 6e20 7768 656e 2072 6563 6569 7669 6e67  n when receiving
-0000f770: 2061 2073 7472 696e 6720 696e 7374 6561   a string instea
-0000f780: 6420 6f66 2061 2070 6174 686c 6962 2e50  d of a pathlib.P
-0000f790: 6174 6820 6f62 6a65 6374 2e0d 0a20 2020  ath object...   
-0000f7a0: 202a 2043 6861 6e67 696e 6720 7468 6520   * Changing the 
-0000f7b0: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
-0000f7c0: 6f6e 2066 6f72 2074 6865 2072 6573 6973  on for the resis
-0000f7d0: 746f 7220 696e 206f 7264 6572 2074 6f20  tor in order to 
-0000f7e0: 6163 6365 7074 2074 6865 2052 3d20 7072  accept the R= pr
-0000f7f0: 6566 6978 206f 6e20 7468 6520 7661 6c75  efix on the valu
-0000f800: 6573 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  es.....* Version
-0000f810: 2034 2e30 2e35 0d0a 2020 2020 2a20 4163   4.0.5..    * Ac
-0000f820: 6365 7074 696e 6720 6669 7865 7320 6672  cepting fixes fr
-0000f830: 6f6d 2061 616e 6173 2d73 6179 6564 4047  om aanas-sayed@G
-0000f840: 6974 4875 6220 7468 6174 2066 6978 6573  itHub that fixes
-0000f850: 2069 7373 7565 7320 7769 7468 2072 756e   issues with run
-0000f860: 6e69 6e67 2074 6865 204c 5453 7069 6365  ning the LTSpice
-0000f870: 2069 6e20 4c69 6e75 782e 0d0a 0d0a 2a20   in Linux.....* 
-0000f880: 5665 7273 696f 6e20 342e 302e 340d 0a20  Version 4.0.4.. 
-0000f890: 2020 202a 2049 6d70 726f 7665 6420 7573     * Improved us
-0000f8a0: 6167 6520 6f66 2074 6865 206c 6f67 6769  age of the loggi
-0000f8b0: 6e67 206c 6962 7261 7279 2e20 2854 6861  ng library. (Tha
-0000f8c0: 6e6b 7320 4054 5370 7265 6368 2066 6f72  nks @TSprech for
-0000f8d0: 2076 6173 746c 7920 696d 7072 6f76 696e   vastly improvin
-0000f8e0: 6720 7468 6520 6c6f 6767 696e 6729 0d0a  g the logging)..
-0000f8f0: 2020 2020 2a20 496e 636c 7564 6564 2052      * Included R
-0000f900: 756e 5461 736b 206e 756d 6265 7220 696e  unTask number in
-0000f910: 2074 6865 206c 6f67 206d 6573 7361 6765   the log message
-0000f920: 732e 0d0a 2020 2020 2a20 496e 636c 7564  s...    * Includ
-0000f930: 6564 206d 696c 6c69 7365 636f 6e64 7320  ed milliseconds 
-0000f940: 696e 2074 6865 2074 696d 6520 656c 6170  in the time elap
-0000f950: 7365 6420 6361 6c63 756c 6174 696f 6e2e  sed calculation.
-0000f960: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
-0000f970: 302e 330d 0a20 2020 202a 2046 6978 696e  0.3..    * Fixin
-0000f980: 6720 6973 7375 6520 696e 2065 6c61 7073  g issue in elaps
-0000f990: 6564 2074 696d 6520 6361 6c63 756c 6174  ed time calculat
-0000f9a0: 696f 6e2e 0d0a 2020 2020 2a20 4669 7869  ion...    * Fixi
-0000f9b0: 6e67 2069 7373 7565 2077 6974 6820 7468  ng issue with th
-0000f9c0: 6520 696d 706f 7274 206f 6620 4c54 5370  e import of LTSp
-0000f9d0: 6963 654c 6f67 5265 6164 6572 2066 726f  iceLogReader fro
-0000f9e0: 6d20 4c54 5374 6570 732e 7079 0d0a 0d0a  m LTSteps.py....
-0000f9f0: 2a20 5665 7273 696f 6e20 342e 302e 320d  * Version 4.0.2.
-0000fa00: 0a20 2020 202a 2043 6861 6e67 696e 6720  .    * Changing 
-0000fa10: 6c69 7374 206f 6620 4c69 6272 6172 7920  list of Library 
-0000fa20: 6465 7065 6e64 656e 6369 6573 2e0d 0a0d  dependencies....
-0000fa30: 0a2a 2056 6572 7369 6f6e 2034 2e30 2e31  .* Version 4.0.1
-0000fa40: 0d0a 2020 2020 2a20 4275 6720 6669 7820  ..    * Bug fix 
-0000fa50: 6f6e 2043 4c49 2066 6f72 2074 6865 2048  on CLI for the H
-0000fa60: 6973 746f 6772 616d 2e70 7920 616e 6420  istogram.py and 
-0000fa70: 4c54 5374 6570 732e 7079 0d0a 0d0a 2a20  LTSteps.py....* 
-0000fa80: 5665 7273 696f 6e20 342e 302e 300d 0a20  Version 4.0.0.. 
-0000fa90: 2020 202a 2053 6570 6172 6174 696e 6720     * Separating 
-0000faa0: 7468 6520 5369 6d43 6f6d 6d61 6e64 6572  the SimCommander
-0000fab0: 2069 6e74 6f20 7477 6f20 7365 7061 7261   into two separa
-0000fac0: 7465 2063 6c61 7373 6573 2c20 6f6e 6520  te classes, one 
-0000fad0: 666f 7220 7468 6520 7370 6963 6520 6e65  for the spice ne
-0000fae0: 746c 6973 7420 6564 6974 696e 6720 2853  tlist editing (S
-0000faf0: 7069 6365 4564 6974 6f72 2920 616e 6420  piceEditor) and 
-0000fb00: 616e 6f74 6865 720d 0a20 2020 2020 2066  another..      f
-0000fb10: 6f72 2074 6865 2073 696d 756c 6174 696f  or the simulatio
-0000fb20: 6e20 6578 6563 7574 696f 6e20 2853 696d  n execution (Sim
-0000fb30: 5275 6e6e 6572 292e 0d0a 2020 2020 2a20  Runner)...    * 
-0000fb40: 496d 706c 656d 656e 7469 6e67 2073 696d  Implementing sim
-0000fb50: 756c 6174 696f 6e20 7365 7276 6572 2074  ulation server t
-0000fb60: 6f20 616c 6c6f 7720 666f 7220 7265 6d6f  o allow for remo
-0000fb70: 7465 2073 696d 756c 6174 696f 6e20 6578  te simulation ex
-0000fb80: 6563 7574 696f 6e20 616e 6420 7468 6520  ecution and the 
-0000fb90: 7265 7370 6563 7469 7665 2063 6c69 656e  respective clien
-0000fba0: 742e 0d0a 2020 2020 2a20 5375 7070 6f72  t...    * Suppor
-0000fbb0: 7469 6e67 2057 6967 676c 6572 2065 6c65  ting Wiggler ele
-0000fbc0: 6d65 6e74 2069 6e20 7468 6520 6e65 7720  ment in the new 
-0000fbd0: 4c54 5370 6963 6558 5649 492e 0d0a 2020  LTSpiceXVII...  
-0000fbe0: 2020 2a20 5265 6e61 6d69 6e67 2061 6c6c    * Renaming all
-0000fbf0: 2066 696c 6573 2069 6e74 6f20 6c6f 7765   files into lowe
-0000fc00: 7263 6173 652e 0d0a 2020 2020 2a20 4372  rcase...    * Cr
-0000fc10: 6561 7469 6e67 2045 7272 6f72 2063 6c61  eating Error cla
-0000fc20: 7373 6573 2066 6f72 2062 6574 7465 7220  sses for better 
-0000fc30: 6572 726f 7220 6861 6e64 6c69 6e67 2e0d  error handling..
-0000fc40: 0a20 2020 202a 2041 6464 696e 6720 7375  .    * Adding su
-0000fc50: 7070 6f72 7420 666f 7220 6f74 6865 7220  pport for other 
-0000fc60: 7369 6d75 6c61 746f 7273 2028 6578 3a20  simulators (ex: 
-0000fc70: 6e67 7370 6963 6529 2077 6865 7265 2074  ngspice) where t
-0000fc80: 6865 2073 696d 756c 6174 6f72 2069 7320  he simulator is 
-0000fc90: 6465 6669 6e65 6420 6279 2061 2063 6c61  defined by a cla
-0000fca0: 7373 2e20 5468 6973 0d0a 2020 2020 2020  ss. This..      
-0000fcb0: 7375 7070 6f72 7420 636c 6173 7320 6e65  support class ne
-0000fcc0: 6564 7320 746f 2062 6520 6120 7375 6263  eds to be a subc
-0000fcd0: 6c61 7373 206f 6620 7468 6520 6162 7374  lass of the abst
-0000fce0: 7261 6374 2063 6c61 7373 2053 696d 756c  ract class Simul
-0000fcf0: 6174 6f72 2e0d 0a20 2020 202a 2045 6e6f  ator...    * Eno
-0000fd00: 726d 6f75 7320 696d 7072 6f76 656d 656e  rmous improvemen
-0000fd10: 7420 696e 2074 6865 2064 6f63 756d 656e  t in the documen
-0000fd20: 7461 7469 6f6e 206f 6620 7468 6520 636f  tation of the co
-0000fd30: 6465 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  de.....* Version
-0000fd40: 2033 2e30 0d0a 2020 2020 2a20 456c 696d   3.0..    * Elim
-0000fd50: 696e 6174 696e 6720 7468 6520 4c54 5370  inating the LTSp
-0000fd60: 6963 6520 7072 6566 6978 6573 2066 726f  ice prefixes fro
-0000fd70: 6d20 6669 6c65 7320 616e 6420 636c 6173  m files and clas
-0000fd80: 7365 732e 0d0a 2020 2020 2a20 4164 6f70  ses...    * Adop
-0000fd90: 7469 6e67 2074 6865 206c 6f77 6572 6361  ting the lowerca
-0000fda0: 7365 2063 6f6e 7665 6e74 696f 6e20 666f  se convention fo
-0000fdb0: 7220 6669 6c65 6e61 6d65 732e 0d0a 0d0a  r filenames.....
-0000fdc0: 2a20 5665 7273 696f 6e20 322e 332e 310d  * Version 2.3.1.
-0000fdd0: 0a20 2020 202a 2042 7567 2066 6978 206f  .    * Bug fix o
-0000fde0: 6e20 7468 6520 7061 7261 6d65 7465 7220  n the parameter 
-0000fdf0: 7265 706c 6163 656d 656e 742e 0d0a 0d0a  replacement.....
-0000fe00: 2a20 5665 7273 696f 6e20 322e 330d 0a20  * Version 2.3.. 
-0000fe10: 2020 202a 2053 7570 706f 7274 696e 6720     * Supporting 
-0000fe20: 7468 6520 6372 6561 7469 6f6e 206f 6620  the creation of 
-0000fe30: 5241 5720 4e6f 6973 6520 416e 616c 7973  RAW Noise Analys
-0000fe40: 6973 0d0a 2020 2020 2a20 4275 6720 4669  is..    * Bug Fi
-0000fe50: 7865 7320 2853 6565 2047 6974 4875 6220  xes (See GitHub 
-0000fe60: 4c6f 6729 0d0a 0d0a 2a20 5665 7273 696f  Log)....* Versio
-0000fe70: 6e20 322e 320d 0a20 2020 202a 204d 616b  n 2.2..    * Mak
-0000fe80: 696e 6720 6e75 6d70 7920 6173 2061 2072  ing numpy as a r
-0000fe90: 6571 7569 7265 6d65 6e74 2061 6e64 2065  equirement and e
-0000fea0: 6c69 6d69 6e61 7469 6e67 2061 6c6c 2063  liminating all c
-0000feb0: 6f64 6520 7468 6174 2061 766f 6964 6564  ode that avoided
-0000fec0: 2074 6865 2075 7365 206f 6620 6e75 6d70   the use of nump
-0000fed0: 790d 0a20 2020 202a 2055 7369 6e67 206e  y..    * Using n
-0000fee0: 6577 2070 6163 6b61 6769 6e67 2074 6f6f  ew packaging too
-0000fef0: 6c0d 0a20 2020 202a 2046 6978 6573 206f  l..    * Fixes o
-0000ff00: 6e20 7468 6520 4c54 5370 6963 655f 5261  n the LTSpice_Ra
-0000ff10: 7757 7269 7465 0d0a 2020 2020 2a20 4669  wWrite..    * Fi
-0000ff20: 7865 7320 696e 2074 6865 2068 616e 646c  xes in the handl
-0000ff30: 696e 6720 6f66 2073 7465 7070 6564 206f  ing of stepped o
-0000ff40: 7065 7261 7469 6e67 2070 6f69 6e74 2073  perating point s
-0000ff50: 696d 756c 6174 696f 6e73 0d0a 0d0a 2a20  imulations....* 
-0000ff60: 5665 7273 696f 6e20 322e 310d 0a20 2020  Version 2.1..   
-0000ff70: 202a 2041 646f 7074 696e 6720 6d69 6e69   * Adopting mini
-0000ff80: 6d75 6d20 7079 7468 6f6e 2076 6572 7369  mum python versi
-0000ff90: 6f6e 2033 2e37 0d0a 2020 2020 2a20 5374  on 3.7..    * St
-0000ffa0: 6172 7469 6e67 2074 6f20 7573 6520 756e  arting to use un
-0000ffb0: 6974 2074 6573 7473 2074 6f20 7661 6c69  it tests to vali
-0000ffc0: 6461 7465 2061 6c6c 206d 6f64 756c 6573  date all modules
-0000ffd0: 2061 6e64 2069 6d70 726f 7669 6e67 2074   and improving t
-0000ffe0: 6573 7462 656e 6368 6573 0d0a 2020 2020  estbenches..    
-0000fff0: 2a20 436f 6d70 6174 6962 696c 6974 7920  * Compatibility 
-00010000: 7769 7468 204e 4753 7069 6365 0d0a 2020  with NGSpice..  
-00010010: 2020 2a20 4176 6f69 6469 6e67 2074 6865    * Avoiding the
-00010020: 2075 7365 206f 6620 7365 7475 702e 7079   use of setup.py
-00010030: 2061 7320 7065 7220 5045 5035 3137 2061   as per PEP517 a
-00010040: 6e64 2050 4550 3531 380d 0a20 2020 202a  nd PEP518..    *
-00010050: 2042 7567 2046 6978 6573 2028 5365 6520   Bug Fixes (See 
-00010060: 4769 7448 7562 206c 6f67 2066 6f72 206d  GitHub log for m
-00010070: 6f72 6520 696e 666f 726d 6174 696f 6e29  ore information)
-00010080: 0d0a 2020 2020 2a20 496d 7072 6f76 656d  ..    * Improvem
-00010090: 656e 7473 206f 6e20 7468 6520 6d61 6e61  ents on the mana
-000100a0: 6765 6d65 6e74 206f 6620 7374 6570 7065  gement of steppe
-000100b0: 6420 6461 7461 2069 6e20 7468 6520 4c54  d data in the LT
-000100c0: 5370 6963 655f 5261 7752 6561 642e 7079  Spice_RawRead.py
-000100d0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 322e  ....* Version 2.
-000100e0: 302e 320d 0a20 2020 202a 2049 6d70 726f  0.2..    * Impro
-000100f0: 7665 6d65 6e74 7320 6f6e 2045 6e63 6f64  vements on Encod
-00010100: 696e 6720 6465 7465 6374 696f 6e0d 0a0d  ing detection...
-00010110: 0a2a 2056 6572 7369 6f6e 2032 2e30 0d0a  .* Version 2.0..
-00010120: 2020 2020 2a20 496e 7465 726e 6174 696f      * Internatio
-00010130: 6e61 6c20 5375 7070 6f72 7420 7573 696e  nal Support usin
-00010140: 6720 7468 6520 636f 7272 6563 7420 656e  g the correct en
-00010150: 636f 6469 6e67 2077 6865 6e20 6c6f 6164  coding when load
-00010160: 696e 6720 6c6f 6720 6669 6c65 732e 0d0a  ing log files...
-00010170: 2020 2020 2a20 436f 6465 204f 7074 696d      * Code Optim
-00010180: 697a 6174 696f 6e73 206f 6e20 7468 6520  izations on the 
-00010190: 4c54 5370 6963 655f 5261 7752 6561 6465  LTSpice_RawReade
-000101a0: 7220 7468 6174 2061 6c6c 6f77 2066 6173  r that allow fas
-000101b0: 7465 7220 6461 7461 206c 6f61 6469 6e67  ter data loading
-000101c0: 2e0d 0a20 2020 202a 2049 6d70 726f 7669  ...    * Improvi
-000101d0: 6e67 2074 6865 2066 756e 6374 696f 6e61  ng the functiona
-000101e0: 6c69 7479 206f 6e20 7468 6520 4c54 5370  lity on the LTSp
-000101f0: 6963 655f 5261 7757 7269 7465 722e 7079  ice_RawWriter.py
-00010200: 0d0a 2020 2020 2a20 4164 6469 6e67 2073  ..    * Adding s
-00010210: 7570 706f 7274 2074 6f20 6564 6974 696e  upport to editin
-00010220: 6720 636f 6d70 6f6e 656e 7473 2069 6e73  g components ins
-00010230: 6964 6520 7375 6263 6972 6375 6974 7320  ide subcircuits 
-00010240: 282e 7375 6263 6b74 290d 0a20 2020 202a  (.subckt)..    *
-00010250: 2053 7570 706f 7274 696e 6720 7265 7369   Supporting resi
-00010260: 7374 6f72 7320 7769 7468 204d 6f64 656c  stors with Model
-00010270: 2044 6566 696e 6974 696f 6e73 0d0a 2020   Definitions..  
-00010280: 2020 2a20 4669 7869 6e67 2070 726f 626c    * Fixing probl
-00010290: 656d 2077 6974 6820 4c54 5370 6963 654c  em with LTSpiceL
-000102a0: 6f67 5265 6164 6572 2074 6861 7420 776f  ogReader that wo
-000102b0: 756c 6420 7265 7475 726e 206d 6573 7365  uld return messe
-000102c0: 6420 7570 2064 6174 610d 0a20 2020 202a  d up data..    *
-000102d0: 2046 6978 696e 6720 7072 6f62 6c65 6d20   Fixing problem 
-000102e0: 7769 7468 2072 6570 6c61 6369 6e67 2074  with replacing t
-000102f0: 6865 2066 696c 6520 6578 7465 6e73 696f  he file extensio
-00010300: 6e20 696e 2063 6572 7461 696e 206e 616d  n in certain nam
-00010310: 6573 0d0a 2020 2020 2a20 436f 7272 6563  es..    * Correc
-00010320: 7469 6e67 2070 726f 626c 656d 2077 6974  ting problem wit
-00010330: 6820 6465 7072 6563 6174 696f 6e73 206f  h deprecations o
-00010340: 6e20 7468 6520 6e75 6d70 7920 6675 6e63  n the numpy func
-00010350: 7469 6f6e 7320 7573 6564 2062 7920 7468  tions used by th
-00010360: 6520 4869 7374 6f67 7261 6d2e 7079 0d0a  e Histogram.py..
-00010370: 2020 2020 2a20 4164 6469 6e67 2062 6163      * Adding bac
-00010380: 6b20 7468 6520 5245 4144 4d45 2e6d 6420  k the README.md 
-00010390: 7468 6174 2073 6f6d 6568 6f77 2077 6173  that somehow was
-000103a0: 2064 656c 6574 6564 0d0a 0d0a 2a20 5665   deleted....* Ve
-000103b0: 7273 696f 6e20 312e 390d 0a20 2020 202a  rsion 1.9..    *
-000103c0: 2041 6464 696e 6720 7375 7070 6f72 7420   Adding support 
-000103d0: 666f 7220 c2b5 2063 6861 7261 6374 6572  for .. character
-000103e0: 2069 6e20 7468 6520 5370 6963 6545 6469   in the SpiceEdi
-000103f0: 746f 722e 0d0a 2020 2020 2a20 4164 6469  tor...    * Addi
-00010400: 6e67 2067 6574 5f63 6f6d 706f 6e65 6e74  ng get_component
-00010410: 5f66 6c6f 6174 7661 6c75 6528 2920 6d65  _floatvalue() me
-00010420: 7468 6f64 2069 6e20 7468 6520 6e65 746c  thod in the netl
-00010430: 6973 7420 6d61 6e69 7075 6c61 7469 6e67  ist manipulating
-00010440: 2063 6c61 7373 2074 6861 7420 6861 6e64   class that hand
-00010450: 6c65 7320 7468 6520 636f 6e76 6572 7369  les the conversi
-00010460: 6f6e 206f 6620 6e75 6d65 7269 630d 0a20  on of numeric.. 
-00010470: 2020 2020 2066 6965 6c64 7320 696e 746f       fields into
-00010480: 2061 2066 6c6f 6174 2e20 5468 6973 2066   a float. This f
-00010490: 756e 6374 696f 6e20 7461 6b65 7320 696e  unction takes in
-000104a0: 746f 2061 6363 6f75 6e74 2074 6865 2065  to account the e
-000104b0: 6e67 696e 6565 7269 6e67 2071 7561 6c69  ngineering quali
-000104c0: 6669 6572 7320 276b 2720 666f 7220 6b69  fiers 'k' for ki
-000104d0: 6c6f 732c 2027 6d27 206f 7220 6d69 6c69  los, 'm' or mili
-000104e0: 732c 0d0a 2020 2020 2020 2775 2720 6f72  s,..      'u' or
-000104f0: 2027 c2b5 2720 666f 7220 6d69 6372 6f6e   '..' for micron
-00010500: 732c 2027 6e27 2066 6f72 206e 616e 6f73  s, 'n' for nanos
-00010510: 2c20 2766 2720 666f 7220 6665 6d74 6f73  , 'f' for femtos
-00010520: 2061 6e64 2027 4d65 6727 2066 6f72 204d   and 'Meg' for M
-00010530: 6567 6173 2e0d 0a0d 0a2a 2056 6572 7369  egas.....* Versi
-00010540: 6f6e 2031 2e38 0d0a 2020 2020 2a20 556e  on 1.8..    * Un
-00010550: 6966 6f72 6d69 6e67 204c 6963 656e 7365  iforming License
-00010560: 2072 6566 6572 656e 6365 2061 6372 6f73   reference acros
-00010570: 7320 6669 6c65 7320 616e 6420 696d 7072  s files and impr
-00010580: 6f76 656d 656e 7473 206f 6e20 7468 6520  ovements on the 
-00010590: 646f 6375 6d65 6e74 6174 696f 6e0d 0a20  documentation.. 
-000105a0: 2020 202a 2041 6e20 656e 6f72 6d6f 7573     * An enormous
-000105b0: 2061 6e64 2077 686f 6c65 6865 6172 7465   and wholehearte
-000105c0: 6420 7468 616e 6b73 2074 6f20 406c 7068  d thanks to @lph
-000105d0: 6572 7220 666f 7220 7468 6520 696d 7072  err for the impr
-000105e0: 6f76 656d 656e 7473 2069 6e20 7468 6520  ovements in the 
-000105f0: 646f 6375 6d65 6e74 6174 696f 6e2e 0d0a  documentation...
-00010600: 2020 2020 2a20 4275 6766 6978 206f 6e20      * Bugfix on 
-00010610: 7468 6520 6164 645f 4c54 7370 6963 6552  the add_LTspiceR
-00010620: 756e 436d 644c 696e 6553 7769 7463 6865  unCmdLineSwitche
-00010630: 7328 2920 3b20 5375 7070 6f72 7469 6e67  s() ; Supporting
-00010640: 202e 7061 7261 6d20 6e61 6d65 2076 616c   .param name val
-00010650: 7565 2066 6f72 6d61 740d 0a20 2020 202a  ue format..    *
-00010660: 2041 6c6c 6f77 696e 6720 7468 6520 4c54   Allowing the LT
-00010670: 5370 6963 6552 6177 5265 6164 2074 6f20  SpiceRawRead to 
-00010680: 7072 6f63 6565 6420 7768 656e 2074 6865  proceed when the
-00010690: 206c 6f67 2066 696c 6520 6361 6e27 7420   log file can't 
-000106a0: 6265 2066 6f75 6e64 206f 7220 7768 656e  be found or when
-000106b0: 2074 6865 7265 2061 7265 2070 726f 626c   there are probl
-000106c0: 656d 7320 7265 6164 696e 6720 6974 2e0d  ems reading it..
-000106d0: 0a2a 2056 6572 7369 6f6e 2031 2e37 0d0a  .* Version 1.7..
-000106e0: 2020 2020 2a20 5275 6e6e 696e 6720 696e      * Running in
-000106f0: 204c 696e 7578 2075 6e64 6572 2077 696e   Linux under win
-00010700: 6520 6973 206e 6f77 2070 6f73 7369 626c  e is now possibl
-00010710: 650d 0a0d 0a2a 2056 6572 7369 6f6e 2031  e....* Version 1
-00010720: 2e36 0d0a 2020 2020 2a20 4164 6469 6e67  .6..    * Adding
-00010730: 204c 5453 7069 6365 5f52 6177 5772 6974   LTSpice_RawWrit
-00010740: 652e 2041 6464 696e 6720 646f 6375 6d65  e. Adding docume
-00010750: 6e74 6174 696f 6e2e 0d0a 0d0a 2a20 5665  ntation.....* Ve
-00010760: 7273 696f 6e20 312e 350d 0a20 2020 202a  rsion 1.5..    *
-00010770: 2053 6d61 6c6c 2066 6978 6573 2061 6e64   Small fixes and
-00010780: 2069 6d70 726f 7665 6d65 6e74 7320 6f6e   improvements on
-00010790: 2074 6865 2063 6c61 7373 2075 7361 6765   the class usage
-000107a0: 2e20 4e6f 2061 6464 6564 2066 6561 7475  . No added featu
-000107b0: 7265 730d 0a0d 0a2a 2056 6572 7369 6f6e  res....* Version
-000107c0: 2031 2e34 0d0a 2020 2020 2a20 4164 6469   1.4..    * Addi
-000107d0: 6e67 2074 6865 204c 5453 7069 6365 5f53  ng the LTSpice_S
-000107e0: 656d 6944 6576 4f70 5265 6164 6572 206d  emiDevOpReader m
-000107f0: 6f64 756c 650d 0a20 2020 202a 2052 652d  odule..    * Re-
-00010800: 656e 6162 6c69 6e67 2074 6865 2048 6973  enabling the His
-00010810: 746f 6772 616d 2066 756e 6374 696f 6e73  togram functions
-00010820: 2077 6869 6368 2077 6865 7265 2064 6973   which where dis
-00010830: 6162 6c65 6420 6279 206d 6973 7461 6b65  abled by mistake
-00010840: 2e0d 0a0d 0a2a 2056 6572 7369 6f6e 2031  .....* Version 1
-00010850: 2e33 0d0a 2020 2020 2a20 4275 6720 6669  .3..    * Bug fi
-00010860: 7865 7320 6f6e 2074 6865 2053 7069 6365  xes on the Spice
-00010870: 4564 6974 6f72 2043 6c61 7373 0d0a 0d0a  Editor Class....
-00010880: 2a20 5665 7273 696f 6e20 312e 320d 0a20  * Version 1.2.. 
-00010890: 2020 202a 2052 4541 444d 452e 6d64 3a0d     * README.md:.
-000108a0: 0a20 2020 2020 2041 6464 696e 6720 6c69  .      Adding li
-000108b0: 6e6b 2074 6f20 7265 6164 7468 6564 6f63  nk to readthedoc
-000108c0: 7320 646f 6375 6d65 6e74 6174 696f 6e0d  s documentation.
-000108d0: 0a20 2020 202a 2041 6c6c 2066 696c 6573  .    * All files
-000108e0: 3a0d 0a20 2020 2020 2043 6f6d 7072 6568  :..      Compreh
-000108f0: 656e 7369 7665 2064 6f63 756d 656e 7461  ensive documenta
-00010900: 7469 6f6e 206f 6e20 686f 7720 746f 2075  tion on how to u
-00010910: 7365 2065 6163 6820 6d6f 6475 6c65 0d0a  se each module..
-00010920: 0d0a 2a20 5665 7273 696f 6e20 312e 310d  ..* Version 1.1.
-00010930: 0a20 2020 202a 2052 4541 444d 452e 6d64  .    * README.md
-00010940: 3a0d 0a20 2020 2020 2055 7064 6174 6564  :..      Updated
-00010950: 2074 6865 2064 6573 6372 6970 7469 6f6e   the description
-00010960: 0d0a 2020 2020 2a20 4c54 5370 6963 6542  ..    * LTSpiceB
-00010970: 6174 6368 2e70 793a 0d0a 2020 2020 2020  atch.py:..      
-00010980: 436f 7272 6563 7465 6420 7468 6520 6e61  Corrected the na
-00010990: 6d65 206f 6620 7468 6520 7265 7475 726e  me of the return
-000109a0: 6564 2072 6177 2066 696c 652e 0d0a 2020  ed raw file...  
-000109b0: 2020 2a20 4164 6465 6420 636f 6d6d 656e    * Added commen
-000109c0: 7473 2074 6872 6f75 6768 6f75 7420 7468  ts throughout th
-000109d0: 6520 636f 6465 2061 6e64 2063 6c65 616e  e code and clean
-000109e0: 7570 0d0a 0d0a 2a20 5665 7273 696f 6e20  up....* Version 
-000109f0: 312e 300d 0a20 2020 202a 204c 5453 7069  1.0..    * LTSpi
-00010a00: 6365 4261 7463 682e 7079 3a5c 0d0a 2020  ceBatch.py:\..  
-00010a10: 2020 2020 496d 706c 656d 656e 7465 6420      Implemented 
-00010a20: 6120 6e65 7720 6170 7072 6f61 6368 2028  a new approach (
-00010a30: 4e4f 5420 4241 434b 5741 5244 5320 434f  NOT BACKWARDS CO
-00010a40: 4d50 4154 4942 4c45 292c 2074 6861 7420  MPATIBLE), that 
-00010a50: 6176 6f69 6473 2074 6865 2075 7361 6765  avoids the usage
-00010a60: 206f 6620 7468 6520 7369 6d5f 7365 7474   of the sim_sett
-00010a70: 696e 6773 2e69 6e63 2066 696c 652e 0d0a  ings.inc file...
-00010a80: 2020 2020 2020 416e 6420 616c 6c6f 7773        And allows
-00010a90: 2074 6f20 6d6f 6469 6679 206e 6f74 206f   to modify not o
-00010aa0: 6e6c 7920 7061 7261 6d65 7465 7273 2c20  nly parameters, 
-00010ab0: 6275 7420 616c 736f 206d 6f64 656c 7320  but also models 
-00010ac0: 616e 6420 6576 656e 2074 6865 2073 696d  and even the sim
-00010ad0: 756c 6174 696f 6e20 636f 6d6d 616e 6473  ulation commands
-00010ae0: 2e0d 0a20 2020 202a 204c 5453 7069 6365  ...    * LTSpice
-00010af0: 5f52 6177 5265 6164 2e70 793a 5c0d 0a20  _RawRead.py:\.. 
-00010b00: 2020 2020 2041 6464 6564 2074 6865 2067       Added the g
-00010b10: 6574 5f74 696d 655f 6178 6973 206d 6574  et_time_axis met
-00010b20: 686f 6420 746f 2074 6865 2052 6177 5265  hod to the RawRe
-00010b30: 6164 2063 6c61 7373 2074 6f20 6176 6f69  ad class to avoi
-00010b40: 6420 7468 6520 7072 6f62 6c65 6d73 2077  d the problems w
-00010b50: 6974 6820 6e65 6761 7469 7665 2076 616c  ith negative val
-00010b60: 7565 7320 6f6e 2074 696d 6520 6178 6973  ues on time axis
-00010b70: 2c0d 0a20 2020 2020 2077 6865 6e20 326e  ,..      when 2n
-00010b80: 6420 6f72 6465 7220 636f 6d70 7265 7373  d order compress
-00010b90: 696f 6e20 6973 2065 6e61 626c 6564 2069  ion is enabled i
-00010ba0: 6e20 4c54 5370 6963 652e 0d0a 2020 2020  n LTSpice...    
-00010bb0: 2a20 4c54 5374 6570 732e 7079 3a5c 0d0a  * LTSteps.py:\..
-00010bc0: 2020 2020 2020 4d6f 6469 6669 6564 2074        Modified t
-00010bd0: 6865 204c 5453 7465 7073 2c20 736f 2069  he LTSteps, so i
-00010be0: 7420 6361 6e20 616c 736f 2072 6561 6420  t can also read 
-00010bf0: 6d65 6173 7572 656d 656e 7473 206f 6e20  measurements on 
-00010c00: 6c6f 6720 6669 6c65 7320 7769 7468 6f75  log files withou
-00010c10: 7420 616e 7920 7374 6570 7320 646f 6e65  t any steps done
-00010c20: 2e0d 0a0d 0a2a 2056 6572 7369 6f6e 2030  .....* Version 0
-00010c30: 2e36 0d0a 2020 2a20 4869 7374 6f67 7261  .6..  * Histogra
-00010c40: 6d2e 7079 206e 6f77 2068 6173 2061 6e20  m.py now has an 
-00010c50: 6f70 7469 6f6e 2074 6f20 6d61 6b65 2074  option to make t
-00010c60: 6865 2068 6973 746f 6772 616d 2064 6972  he histogram dir
-00010c70: 6563 746c 7920 6672 6f6d 2076 616c 7565  ectly from value
-00010c80: 7320 7374 6f72 6564 2069 6e20 7468 6520  s stored in the 
-00010c90: 636c 6970 626f 6172 640d 0a0d 0a2a 2056  clipboard....* V
-00010ca0: 6572 7369 6f6e 2030 2e35 0d0a 2020 2a20  ersion 0.5..  * 
-00010cb0: 5468 6520 4c54 5370 6963 655f 5261 7752  The LTSpice_RawR
-00010cc0: 6561 6465 722e 7079 206e 6f77 2075 7365  eader.py now use
-00010cd0: 7320 7468 6520 6073 7472 7563 742e 756e  s the `struct.un
-00010ce0: 7061 636b 6020 6675 6e63 7469 6f6e 2066  pack` function f
-00010cf0: 6f72 2061 2066 6173 7465 7220 6578 6563  or a faster exec
-00010d00: 7574 696f 6e0d 0a0d 0a2a 2056 6572 7369  ution....* Versi
-00010d10: 6f6e 2030 2e34 0d0a 2020 2a20 4164 6465  on 0.4..  * Adde
-00010d20: 6420 4c54 5370 6963 6542 6174 6368 2e70  d LTSpiceBatch.p
-00010d30: 7920 746f 2074 6865 2063 6f6c 6c65 6374  y to the collect
-00010d40: 696f 6e20 6f66 2074 6f6f 6c73 0d0a 0d0a  ion of tools....
-00010d50: 2a20 5665 7273 696f 6e20 302e 330d 0a20  * Version 0.3.. 
-00010d60: 202a 2041 2076 6572 7369 6f6e 206f 6620   * A version of 
-00010d70: 4c54 5374 6570 7320 7468 6174 2063 616e  LTSteps that can
-00010d80: 2062 6520 696d 706f 7274 6564 2074 6f20   be imported to 
-00010d90: 7573 6520 696e 2061 2068 6967 6865 7220  use in a higher 
-00010da0: 6c65 7665 6c20 7363 7269 7074 0d0a 0d0a  level script....
-00010db0: 2a20 5665 7273 696f 6e20 302e 320d 0a20  * Version 0.2.. 
-00010dc0: 202a 2041 6464 696e 6720 4c54 5374 6570   * Adding LTStep
-00010dd0: 732e 7079 2061 6e64 2048 6973 746f 6772  s.py and Histogr
-00010de0: 616d 2e70 790d 0a0d 0a2a 2056 6572 7369  am.py....* Versi
-00010df0: 6f6e 2030 2e31 200d 0a20 202a 2046 6972  on 0.1 ..  * Fir
-00010e00: 7374 2063 6f6d 6d69 7420 746f 2074 6865  st commit to the
-00010e10: 2062 6974 6275 636b 6574 2072 6570 6f73   bitbucket repos
-00010e20: 6974 6f72 792e 0d0a                      itory...
+0000b1e0: 2e2f 7465 7374 6669 6c65 732f 5452 414e  ./testfiles/TRAN
+0000b1f0: 202d 2053 5445 502e 7261 7722 290d 0a0d   - STEP.raw")...
+0000b200: 0a70 7269 6e74 284c 5452 2e67 6574 5f74  .print(LTR.get_t
+0000b210: 7261 6365 5f6e 616d 6573 2829 290d 0a70  race_names())..p
+0000b220: 7269 6e74 284c 5452 2e67 6574 5f72 6177  rint(LTR.get_raw
+0000b230: 5f70 726f 7065 7274 7928 2929 0d0a 0d0a  _property())....
+0000b240: 4952 3120 3d20 4c54 522e 6765 745f 7472  IR1 = LTR.get_tr
+0000b250: 6163 6528 2249 2852 3129 2229 0d0a 7820  ace("I(R1)")..x 
+0000b260: 3d20 4c54 522e 6765 745f 7472 6163 6528  = LTR.get_trace(
+0000b270: 2774 696d 6527 2920 2023 2047 6574 7320  'time')  # Gets 
+0000b280: 7468 6520 7469 6d65 2061 7869 730d 0a73  the time axis..s
+0000b290: 7465 7073 203d 204c 5452 2e67 6574 5f73  teps = LTR.get_s
+0000b2a0: 7465 7073 2829 0d0a 666f 7220 7374 6570  teps()..for step
+0000b2b0: 2069 6e20 7261 6e67 6528 6c65 6e28 7374   in range(len(st
+0000b2c0: 6570 7329 293a 0d0a 2020 2020 2320 7072  eps)):..    # pr
+0000b2d0: 696e 7428 7374 6570 735b 7374 6570 5d29  int(steps[step])
+0000b2e0: 0d0a 2020 2020 706c 742e 706c 6f74 2878  ..    plt.plot(x
+0000b2f0: 2e67 6574 5f77 6176 6528 7374 6570 292c  .get_wave(step),
+0000b300: 2049 5231 2e67 6574 5f77 6176 6528 7374   IR1.get_wave(st
+0000b310: 6570 292c 206c 6162 656c 3d73 7465 7073  ep), label=steps
+0000b320: 5b73 7465 705d 290d 0a0d 0a70 6c74 2e6c  [step])....plt.l
+0000b330: 6567 656e 6428 2920 2023 206f 7264 6572  egend()  # order
+0000b340: 2061 206c 6567 656e 640d 0a70 6c74 2e73   a legend..plt.s
+0000b350: 686f 7728 290d 0a60 6060 0d0a 2d2d 2069  how()..```..-- i
+0000b360: 6e20 6578 616d 706c 6573 2f72 6177 5f72  n examples/raw_r
+0000b370: 6561 645f 6578 616d 706c 652e 7079 2020  ead_example.py  
+0000b380: 200d 0a0d 0a23 2323 2052 6177 5772 6974   ....### RawWrit
+0000b390: 6520 2323 230d 0a0d 0a54 6865 2066 6f6c  e ###....The fol
+0000b3a0: 6c6f 7769 6e67 2065 7861 6d70 6c65 2077  lowing example w
+0000b3b0: 7269 7465 7320 6120 5241 5720 6669 6c65  rites a RAW file
+0000b3c0: 2077 6974 6820 6120 3320 6d69 6c6c 6973   with a 3 millis
+0000b3d0: 6563 6f6e 6473 2074 7261 6e73 6965 6e74  econds transient
+0000b3e0: 2073 696d 756c 6174 696f 6e20 7369 6e65   simulation sine
+0000b3f0: 2077 6974 6820 6120 3130 6b48 7a20 616e   with a 10kHz an
+0000b400: 6420 6120 636f 7369 6e65 2077 6974 680d  d a cosine with.
+0000b410: 0a39 2e39 3937 6b48 7a0d 0a0d 0a60 6060  .9.997kHz....```
+0000b420: 7079 7468 6f6e 0d0a 696d 706f 7274 206e  python..import n
+0000b430: 756d 7079 2061 7320 6e70 0d0a 6672 6f6d  umpy as np..from
+0000b440: 2050 794c 5453 7069 6365 2069 6d70 6f72   PyLTSpice impor
+0000b450: 7420 5261 7752 6561 642c 2054 7261 6365  t RawRead, Trace
+0000b460: 2c20 5261 7757 7269 7465 0d0a 4c57 203d  , RawWrite..LW =
+0000b470: 2052 6177 5772 6974 6528 6661 7374 6163   RawWrite(fastac
+0000b480: 6365 733d 4661 6c73 6529 0d0a 7478 203d  ces=False)..tx =
+0000b490: 2054 7261 6365 2827 7469 6d65 272c 206e   Trace('time', n
+0000b4a0: 702e 6172 616e 6765 2830 2e30 2c20 3365  p.arange(0.0, 3e
+0000b4b0: 2d33 2c20 3939 3745 2d31 3129 290d 0a76  -3, 997E-11))..v
+0000b4c0: 7920 3d20 5472 6163 6528 274e 3030 3127  y = Trace('N001'
+0000b4d0: 2c20 6e70 2e73 696e 2832 202a 206e 702e  , np.sin(2 * np.
+0000b4e0: 7069 202a 2074 782e 6461 7461 202a 2031  pi * tx.data * 1
+0000b4f0: 3030 3030 2929 0d0a 767a 203d 2054 7261  0000))..vz = Tra
+0000b500: 6365 2827 4e30 3032 272c 206e 702e 636f  ce('N002', np.co
+0000b510: 7328 3220 2a20 6e70 2e70 6920 2a20 7478  s(2 * np.pi * tx
+0000b520: 2e64 6174 6120 2a20 3939 3730 2929 0d0a  .data * 9970))..
+0000b530: 4c57 2e61 6464 5f74 7261 6365 2874 7829  LW.add_trace(tx)
+0000b540: 0d0a 4c57 2e61 6464 5f74 7261 6365 2876  ..LW.add_trace(v
+0000b550: 7929 0d0a 4c57 2e61 6464 5f74 7261 6365  y)..LW.add_trace
+0000b560: 2876 7a29 0d0a 4c57 2e73 6176 6528 222e  (vz)..LW.save(".
+0000b570: 2f74 6573 7466 696c 6573 2f74 6573 7465  /testfiles/teste
+0000b580: 5f73 6e69 7070 6574 312e 7261 7722 290d  _snippet1.raw").
+0000b590: 0a60 6060 2020 200d 0a2d 2d20 696e 2065  .```   ..-- in e
+0000b5a0: 7861 6d70 6c65 732f 7261 775f 7772 6974  xamples/raw_writ
+0000b5b0: 655f 6578 616d 706c 652e 7079 205b 5261  e_example.py [Ra
+0000b5c0: 7757 7269 7465 2045 7861 6d70 6c65 5d0d  wWrite Example].
+0000b5d0: 0a0d 0a23 2323 2053 7069 6365 4564 6974  ...### SpiceEdit
+0000b5e0: 6f72 2c20 4173 6345 6469 746f 7220 616e  or, AscEditor an
+0000b5f0: 6420 5369 6d52 756e 6e65 722e 7079 2023  d SimRunner.py #
+0000b600: 2323 0d0a 0d0a 5468 6973 206d 6f64 756c  ##....This modul
+0000b610: 6520 6973 2075 7365 6420 746f 206c 6175  e is used to lau
+0000b620: 6e63 6820 4c54 5350 6963 6520 7369 6d75  nch LTSPice simu
+0000b630: 6c61 7469 6f6e 732e 2052 6573 756c 7473  lations. Results
+0000b640: 2074 6865 6e20 6361 6e20 6265 2070 726f   then can be pro
+0000b650: 6365 7373 6564 2077 6974 6820 6569 7468  cessed with eith
+0000b660: 6572 2074 6865 2052 6177 5265 6164 206f  er the RawRead o
+0000b670: 7220 7769 7468 2074 6865 0d0a 4c54 5374  r with the..LTSt
+0000b680: 6570 7320 6d6f 6475 6c65 2074 6f20 7265  eps module to re
+0000b690: 6164 2074 6865 206c 6f67 2066 696c 6520  ad the log file 
+0000b6a0: 7768 6963 6820 6361 6e20 636f 6e74 6169  which can contai
+0000b6b0: 6e20 2e4d 4541 5320 7265 7375 6c74 732e  n .MEAS results.
+0000b6c0: 0d0a 0d0a 5468 6520 7363 7269 7074 2077  ....The script w
+0000b6d0: 696c 6c20 6669 7273 746c 7920 696e 766f  ill firstly invo
+0000b6e0: 6b65 2074 6865 204c 5453 7069 6365 2069  ke the LTSpice i
+0000b6f0: 6e20 636f 6d6d 616e 6420 6c69 6e65 2074  n command line t
+0000b700: 6f20 6765 6e65 7261 7465 2061 206e 6574  o generate a net
+0000b710: 6c69 7374 2c20 616e 6420 7468 656e 2074  list, and then t
+0000b720: 6869 7320 6e65 746c 6973 7420 6361 6e20  his netlist can 
+0000b730: 6265 2075 7064 6174 6564 0d0a 6469 7265  be updated..dire
+0000b740: 6374 6c79 2062 7920 7468 6520 7363 7269  ctly by the scri
+0000b750: 7074 2c20 696e 206f 7264 6572 2074 6f20  pt, in order to 
+0000b760: 6368 616e 6765 2063 6f6d 706f 6e65 6e74  change component
+0000b770: 2076 616c 7565 732c 2070 6172 616d 6574   values, paramet
+0000b780: 6572 7320 6f72 2073 696d 756c 6174 696f  ers or simulatio
+0000b790: 6e20 636f 6d6d 616e 6473 2e0d 0a0d 0a48  n commands.....H
+0000b7a0: 6572 6520 666f 6c6c 6f77 7320 616e 2065  ere follows an e
+0000b7b0: 7861 6d70 6c65 206f 6620 6f70 6572 6174  xample of operat
+0000b7c0: 696f 6e2e 0d0a 0d0a 6060 6070 7974 686f  ion.....```pytho
+0000b7d0: 6e0d 0a66 726f 6d20 5079 4c54 5370 6963  n..from PyLTSpic
+0000b7e0: 6520 696d 706f 7274 2053 696d 5275 6e6e  e import SimRunn
+0000b7f0: 6572 0d0a 6672 6f6d 2050 794c 5453 7069  er..from PyLTSpi
+0000b800: 6365 2069 6d70 6f72 7420 5370 6963 6545  ce import SpiceE
+0000b810: 6469 746f 720d 0a0d 0a23 2046 6f72 6365  ditor....# Force
+0000b820: 2061 6e6f 7468 6572 2073 696d 756c 6174   another simulat
+0000b830: 696f 720d 0a73 696d 756c 6174 6f72 203d  ior..simulator =
+0000b840: 2072 2243 3a5c 5072 6f67 7261 6d20 4669   r"C:\Program Fi
+0000b850: 6c65 735c 4c54 435c 4c54 7370 6963 6558  les\LTC\LTspiceX
+0000b860: 5649 495c 5856 4949 7836 342e 6578 6522  VII\XVIIx64.exe"
+0000b870: 0d0a 0d0a 2320 7365 6c65 6374 2073 7069  ....# select spi
+0000b880: 6365 206d 6f64 656c 0d0a 4c54 4320 3d20  ce model..LTC = 
+0000b890: 5369 6d52 756e 6e65 7228 6f75 7470 7574  SimRunner(output
+0000b8a0: 5f66 6f6c 6465 723d 272e 2f74 656d 7027  _folder='./temp'
+0000b8b0: 290d 0a4c 5443 2e63 7265 6174 655f 6e65  )..LTC.create_ne
+0000b8c0: 746c 6973 7428 272e 2f74 6573 7466 696c  tlist('./testfil
+0000b8d0: 6573 2f42 6174 6368 5f54 6573 742e 6173  es/Batch_Test.as
+0000b8e0: 6327 290d 0a6e 6574 6c69 7374 203d 2053  c')..netlist = S
+0000b8f0: 7069 6365 4564 6974 6f72 2827 2e2f 7465  piceEditor('./te
+0000b900: 7374 6669 6c65 732f 4261 7463 685f 5465  stfiles/Batch_Te
+0000b910: 7374 2e6e 6574 2729 0d0a 2320 7365 7420  st.net')..# set 
+0000b920: 6465 6661 756c 7420 6172 6775 6d65 6e74  default argument
+0000b930: 730d 0a6e 6574 6c69 7374 2e73 6574 5f70  s..netlist.set_p
+0000b940: 6172 616d 6574 6572 7328 7265 733d 302c  arameters(res=0,
+0000b950: 2063 6170 3d31 3030 652d 3629 0d0a 6e65   cap=100e-6)..ne
+0000b960: 746c 6973 742e 7365 745f 636f 6d70 6f6e  tlist.set_compon
+0000b970: 656e 745f 7661 6c75 6528 2752 3227 2c20  ent_value('R2', 
+0000b980: 2732 6b27 2920 2023 204d 6f64 6966 7969  '2k')  # Modifyi
+0000b990: 6e67 2074 6865 2076 616c 7565 206f 6620  ng the value of 
+0000b9a0: 6120 7265 7369 7374 6f72 0d0a 6e65 746c  a resistor..netl
+0000b9b0: 6973 742e 7365 745f 636f 6d70 6f6e 656e  ist.set_componen
+0000b9c0: 745f 7661 6c75 6528 2752 3127 2c20 2734  t_value('R1', '4
+0000b9d0: 6b27 290d 0a6e 6574 6c69 7374 2e73 6574  k')..netlist.set
+0000b9e0: 5f65 6c65 6d65 6e74 5f6d 6f64 656c 2827  _element_model('
+0000b9f0: 5633 272c 2022 5349 4e45 2830 2031 2033  V3', "SINE(0 1 3
+0000ba00: 6b20 3020 3020 3029 2229 2020 2320 4d6f  k 0 0 0)")  # Mo
+0000ba10: 6469 6679 696e 6720 7468 650d 0a6e 6574  difying the..net
+0000ba20: 6c69 7374 2e73 6574 5f63 6f6d 706f 6e65  list.set_compone
+0000ba30: 6e74 5f76 616c 7565 2827 5855 313a 4332  nt_value('XU1:C2
+0000ba40: 272c 2032 3065 2d31 3229 2020 2320 6d6f  ', 20e-12)  # mo
+0000ba50: 6469 6679 696e 6720 6120 6465 6669 6e65  difying a define
+0000ba60: 2073 696d 756c 6174 696f 6e0d 0a6e 6574   simulation..net
+0000ba70: 6c69 7374 2e61 6464 5f69 6e73 7472 7563  list.add_instruc
+0000ba80: 7469 6f6e 7328 0d0a 2020 2020 223b 2053  tions(..    "; S
+0000ba90: 696d 756c 6174 696f 6e20 7365 7474 696e  imulation settin
+0000baa0: 6773 222c 0d0a 2020 2020 223b 2e70 6172  gs",..    ";.par
+0000bab0: 616d 2072 756e 203d 2030 220d 0a29 0d0a  am run = 0"..)..
+0000bac0: 6e65 746c 6973 742e 7365 745f 7061 7261  netlist.set_para
+0000bad0: 6d65 7465 7228 2772 756e 272c 2030 290d  meter('run', 0).
+0000bae0: 0a0d 0a66 6f72 206f 7061 6d70 2069 6e20  ...for opamp in 
+0000baf0: 2827 4144 3731 3227 2c20 2741 4438 3230  ('AD712', 'AD820
+0000bb00: 2729 3a0d 0a20 2020 206e 6574 6c69 7374  '):..    netlist
+0000bb10: 2e73 6574 5f65 6c65 6d65 6e74 5f6d 6f64  .set_element_mod
+0000bb20: 656c 2827 5855 3127 2c20 6f70 616d 7029  el('XU1', opamp)
+0000bb30: 0d0a 2020 2020 666f 7220 7375 7070 6c79  ..    for supply
+0000bb40: 5f76 6f6c 7461 6765 2069 6e20 2835 2c20  _voltage in (5, 
+0000bb50: 3130 2c20 3135 293a 0d0a 2020 2020 2020  10, 15):..      
+0000bb60: 2020 6e65 746c 6973 742e 7365 745f 636f    netlist.set_co
+0000bb70: 6d70 6f6e 656e 745f 7661 6c75 6528 2756  mponent_value('V
+0000bb80: 3127 2c20 7375 7070 6c79 5f76 6f6c 7461  1', supply_volta
+0000bb90: 6765 290d 0a20 2020 2020 2020 206e 6574  ge)..        net
+0000bba0: 6c69 7374 2e73 6574 5f63 6f6d 706f 6e65  list.set_compone
+0000bbb0: 6e74 5f76 616c 7565 2827 5632 272c 202d  nt_value('V2', -
+0000bbc0: 7375 7070 6c79 5f76 6f6c 7461 6765 290d  supply_voltage).
+0000bbd0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0000bbe0: 7369 6d75 6c61 7469 6e67 204f 7041 6d70  simulating OpAmp
+0000bbf0: 222c 206f 7061 6d70 2c20 2256 6f6c 7461  ", opamp, "Volta
+0000bc00: 6765 222c 2073 7570 706c 795f 766f 6c74  ge", supply_volt
+0000bc10: 6167 6529 0d0a 2020 2020 2020 2020 4c54  age)..        LT
+0000bc20: 432e 7275 6e28 6e65 746c 6973 7429 0d0a  C.run(netlist)..
+0000bc30: 0d0a 666f 7220 7261 772c 206c 6f67 2069  ..for raw, log i
+0000bc40: 6e20 4c54 433a 0d0a 2020 2020 7072 696e  n LTC:..    prin
+0000bc50: 7428 2252 6177 2066 696c 653a 2025 732c  t("Raw file: %s,
+0000bc60: 204c 6f67 2066 696c 653a 2025 7322 2025   Log file: %s" %
+0000bc70: 2028 7261 772c 206c 6f67 2929 0d0a 2020   (raw, log))..  
+0000bc80: 2020 2320 646f 2073 6f6d 6574 6869 6e67    # do something
+0000bc90: 2077 6974 6820 7468 6520 6461 7461 0d0a   with the data..
+0000bca0: 2020 2020 2320 7261 775f 6461 7461 203d      # raw_data =
+0000bcb0: 2052 6177 5265 6164 2872 6177 290d 0a20   RawRead(raw).. 
+0000bcc0: 2020 2023 206c 6f67 5f64 6174 6120 3d20     # log_data = 
+0000bcd0: 4c54 5374 6570 7328 6c6f 6729 0d0a 2020  LTSteps(log)..  
+0000bce0: 2020 2320 2e2e 2e0d 0a0d 0a6e 6574 6c69    # .......netli
+0000bcf0: 7374 2e72 6573 6574 5f6e 6574 6c69 7374  st.reset_netlist
+0000bd00: 2829 0d0a 6e65 746c 6973 742e 6164 645f  ()..netlist.add_
+0000bd10: 696e 7374 7275 6374 696f 6e73 280d 0a20  instructions(.. 
+0000bd20: 2020 2022 3b20 5369 6d75 6c61 7469 6f6e     "; Simulation
+0000bd30: 2073 6574 7469 6e67 7322 2c0d 0a20 2020   settings",..   
+0000bd40: 2022 2e61 6320 6465 6320 3330 2031 3020   ".ac dec 30 10 
+0000bd50: 314d 6567 222c 0d0a 2020 2020 222e 6d65  1Meg",..    ".me
+0000bd60: 6173 2041 4320 4761 696e 204d 4158 206d  as AC Gain MAX m
+0000bd70: 6167 2856 286f 7574 2929 203b 2066 696e  ag(V(out)) ; fin
+0000bd80: 6420 7468 6520 7065 616b 2072 6573 706f  d the peak respo
+0000bd90: 6e73 6520 616e 6420 6361 6c6c 2069 7420  nse and call it 
+0000bda0: 2222 4761 696e 2222 222c 0d0a 2020 2020  ""Gain""",..    
+0000bdb0: 222e 6d65 6173 2041 4320 4663 7574 2054  ".meas AC Fcut T
+0000bdc0: 5249 4720 6d61 6728 5628 6f75 7429 293d  RIG mag(V(out))=
+0000bdd0: 4761 696e 2f73 7172 7428 3229 2046 414c  Gain/sqrt(2) FAL
+0000bde0: 4c3d 6c61 7374 220d 0a29 0d0a 0d0a 2320  L=last"..)....# 
+0000bdf0: 5369 6d20 5374 6174 6973 7469 6373 0d0a  Sim Statistics..
+0000be00: 7072 696e 7428 2753 7563 6365 7373 6675  print('Successfu
+0000be10: 6c2f 546f 7461 6c20 5369 6d75 6c61 7469  l/Total Simulati
+0000be20: 6f6e 733a 2027 202b 2073 7472 284c 5443  ons: ' + str(LTC
+0000be30: 2e6f 6b53 696d 2920 2b20 272f 2720 2b20  .okSim) + '/' + 
+0000be40: 7374 7228 4c54 432e 7275 6e6e 6f29 290d  str(LTC.runno)).
+0000be50: 0a0d 0a65 6e74 6572 203d 2069 6e70 7574  ...enter = input
+0000be60: 2822 5072 6573 7320 656e 7465 7220 746f  ("Press enter to
+0000be70: 2064 656c 6574 6520 6372 6561 7465 6420   delete created 
+0000be80: 6669 6c65 7322 290d 0a69 6620 656e 7465  files")..if ente
+0000be90: 7220 3d3d 2027 273a 0d0a 2020 2020 4c54  r == '':..    LT
+0000bea0: 432e 6669 6c65 5f63 6c65 616e 7570 2829  C.file_cleanup()
+0000beb0: 0d0a 6060 600d 0a2d 2d20 696e 2065 7861  ..```..-- in exa
+0000bec0: 6d70 6c65 732f 7369 6d5f 7275 6e6e 6572  mples/sim_runner
+0000bed0: 5f65 7861 6d70 6c65 2e70 790d 0a0d 0a54  _example.py....T
+0000bee0: 6865 2065 7861 6d70 6c65 2061 626f 7665  he example above
+0000bef0: 2069 7320 7573 696e 6720 7468 6520 5370   is using the Sp
+0000bf00: 6963 6545 6469 746f 7220 746f 2063 7265  iceEditor to cre
+0000bf10: 6174 6520 616e 6420 6d6f 6469 6679 2061  ate and modify a
+0000bf20: 2073 7069 6365 206e 6574 6c69 7374 2c20   spice netlist, 
+0000bf30: 6275 7420 6974 2069 7320 616c 736f 2070  but it is also p
+0000bf40: 6f73 7369 626c 6520 746f 2075 7365 2074  ossible to use t
+0000bf50: 6865 0d0a 4173 6345 6469 746f 7220 746f  he..AscEditor to
+0000bf60: 2064 6972 6563 746c 7920 6d6f 6469 6679   directly modify
+0000bf70: 2074 6865 202e 6173 6320 6669 6c65 2e20   the .asc file. 
+0000bf80: 5468 6520 6564 6974 6564 202e 6173 6320  The edited .asc 
+0000bf90: 6669 6c65 2063 616e 2074 6865 6e20 6265  file can then be
+0000bfa0: 206f 7065 6e65 6420 6279 2074 6865 204c   opened by the L
+0000bfb0: 5453 7069 6365 2047 5549 2061 6e64 2074  TSpice GUI and t
+0000bfc0: 6865 0d0a 7369 6d75 6c61 7469 6f6e 2063  he..simulation c
+0000bfd0: 616e 2062 6520 7275 6e20 6672 6f6d 2074  an be run from t
+0000bfe0: 6865 7265 2e0d 0a0d 0a23 2323 2053 696d  here.....### Sim
+0000bff0: 756c 6174 696f 6e20 416e 616c 7973 6973  ulation Analysis
+0000c000: 2054 6f6f 6c6b 6974 2023 2323 0d0a 0d0a   Toolkit ###....
+0000c010: 5468 6520 4173 6345 6469 746f 7220 6361  The AscEditor ca
+0000c020: 6e20 6265 2075 7365 6420 7769 7468 2074  n be used with t
+0000c030: 6865 2053 696d 756c 6174 696f 6e20 416e  he Simulation An
+0000c040: 616c 7973 6973 2054 6f6f 6c6b 6974 2074  alysis Toolkit t
+0000c050: 6f20 7065 7266 6f72 6d20 4d6f 6e74 6520  o perform Monte 
+0000c060: 4361 726c 6f20 6f72 2057 6f73 7420 4361  Carlo or Wost Ca
+0000c070: 7365 2073 696d 756c 6174 696f 6e73 2e0d  se simulations..
+0000c080: 0a54 6865 7365 2073 696d 756c 6174 696f  .These simulatio
+0000c090: 6e73 2063 616e 2065 6974 6865 7220 6265  ns can either be
+0000c0a0: 2064 6f6e 6520 6f6e 2074 6865 204c 5453   done on the LTS
+0000c0b0: 7069 6365 2047 5549 206f 7220 7573 696e  pice GUI or usin
+0000c0c0: 6720 7468 6520 5275 6e6e 6572 2043 6c61  g the Runner Cla
+0000c0d0: 7373 2064 6573 6372 6962 6564 2061 626f  ss described abo
+0000c0e0: 7665 2e0d 0a0d 0a4c 6574 2773 2063 6f6e  ve.....Let's con
+0000c0f0: 7369 6465 7220 7468 6520 666f 6c6c 6f77  sider the follow
+0000c100: 696e 6720 6369 7263 7569 743a 0d0a 0d0a  ing circuit:....
+0000c110: 215b 5361 6c6c 656e 2d4b 6579 2041 6d70  ![Sallen-Key Amp
+0000c120: 6c69 6669 6572 5d28 2e2f 646f 632f 6d6f  lifier](./doc/mo
+0000c130: 6475 6c65 732f 7361 6c6c 656e 6b65 792e  dules/sallenkey.
+0000c140: 706e 6720 2253 616c 6c65 6e2d 4b65 7920  png "Sallen-Key 
+0000c150: 416d 706c 6966 6965 7222 290d 0a0d 0a57  Amplifier")....W
+0000c160: 6865 6e20 7065 7266 6f72 6d69 6e67 2061  hen performing a
+0000c170: 204d 6f6e 7465 2043 6172 6c6f 2073 696d   Monte Carlo sim
+0000c180: 756c 6174 696f 6e20 6f6e 2074 6869 7320  ulation on this 
+0000c190: 6369 7263 7569 742c 2077 6520 6e65 6564  circuit, we need
+0000c1a0: 2074 6f20 6d61 6e75 616c 6c79 206d 6f64   to manually mod
+0000c1b0: 6966 7920 7468 6520 7661 6c75 6520 6f66  ify the value of
+0000c1c0: 2065 6163 6820 636f 6d70 6f6e 656e 742c   each component,
+0000c1d0: 200d 0a61 6e64 2074 6865 6e20 6164 6420   ..and then add 
+0000c1e0: 7468 6520 2e73 7465 7020 636f 6d6d 616e  the .step comman
+0000c1f0: 6420 666f 7220 6d61 6b69 6e67 2073 6576  d for making sev
+0000c200: 6572 616c 2072 756e 7320 6f6e 2074 6865  eral runs on the
+0000c210: 2073 616d 6520 6369 7263 7569 742e 200d   same circuit. .
+0000c220: 0a54 6f20 7369 6d70 6c69 6679 2074 6869  .To simplify thi
+0000c230: 7320 7072 6f63 6573 732c 2074 6865 2041  s process, the A
+0000c240: 7363 4564 6974 6f72 2063 6c61 7373 2063  scEditor class c
+0000c250: 616e 2062 6520 7573 6564 2061 7320 6578  an be used as ex
+0000c260: 656d 706c 6966 6965 6420 6265 6c6f 773a  emplified below:
+0000c270: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
+0000c280: 726f 6d20 5079 4c54 5370 6963 6520 696d  rom PyLTSpice im
+0000c290: 706f 7274 2041 7363 4564 6974 6f72 2c20  port AscEditor, 
+0000c2a0: 5369 6d52 756e 6e65 7220 2023 2049 6d70  SimRunner  # Imp
+0000c2b0: 6f72 7473 2074 6865 2063 6c61 7373 2074  orts the class t
+0000c2c0: 6861 7420 6d61 6e69 7075 6c61 7465 7320  hat manipulates 
+0000c2d0: 7468 6520 6173 6320 6669 6c65 0d0a 6672  the asc file..fr
+0000c2e0: 6f6d 2050 794c 5453 7069 6365 2e73 696d  om PyLTSpice.sim
+0000c2f0: 2e74 6f6f 6b69 742e 6d6f 6e74 6563 6172  .tookit.montecar
+0000c300: 6c6f 2069 6d70 6f72 7420 4d6f 6e74 6563  lo import Montec
+0000c310: 6172 6c6f 2020 2320 496d 706f 7274 7320  arlo  # Imports 
+0000c320: 7468 6520 4d6f 6e74 6563 6172 6c6f 2074  the Montecarlo t
+0000c330: 6f6f 6c6b 6974 2063 6c61 7373 0d0a 0d0a  oolkit class....
+0000c340: 7361 6c6c 656e 6b65 7920 3d20 4173 6345  sallenkey = AscE
+0000c350: 6469 746f 7228 222e 2f74 6573 7466 696c  ditor("./testfil
+0000c360: 6573 2f73 616c 6c65 6e6b 6579 2e61 7363  es/sallenkey.asc
+0000c370: 2229 2020 2320 5265 6164 7320 7468 6520  ")  # Reads the 
+0000c380: 6173 6320 6669 6c65 2069 6e74 6f20 6d65  asc file into me
+0000c390: 6d6f 7279 0d0a 7275 6e6e 6572 203d 2053  mory..runner = S
+0000c3a0: 696d 5275 6e6e 6572 286f 7574 7075 745f  imRunner(output_
+0000c3b0: 666f 6c64 6572 3d27 2e2f 7465 6d70 5f6d  folder='./temp_m
+0000c3c0: 6327 2920 2023 2049 6e73 7461 6e74 6961  c')  # Instantia
+0000c3d0: 7465 7320 7468 6520 7275 6e6e 6572 2063  tes the runner c
+0000c3e0: 6c61 7373 2c20 7769 7468 2074 6865 206f  lass, with the o
+0000c3f0: 7574 7075 7420 666f 6c64 6572 2061 6c72  utput folder alr
+0000c400: 6561 6479 2073 6574 0d0a 6d63 203d 204d  eady set..mc = M
+0000c410: 6f6e 7465 6361 726c 6f28 7361 6c6c 656e  ontecarlo(sallen
+0000c420: 6b65 792c 2072 756e 6e65 7229 2020 2320  key, runner)  # 
+0000c430: 496e 7374 616e 7469 6174 6573 2074 6865  Instantiates the
+0000c440: 204d 6f6e 7465 6361 726c 6f20 636c 6173   Montecarlo clas
+0000c450: 732c 2077 6974 6820 7468 6520 6173 6320  s, with the asc 
+0000c460: 6669 6c65 2061 6c72 6561 6479 2069 6e20  file already in 
+0000c470: 6d65 6d6f 7279 0d0a 0d0a 2320 5468 6520  memory....# The 
+0000c480: 666f 6c6c 6f77 696e 6720 6c69 6e65 7320  following lines 
+0000c490: 7365 7420 7468 6520 6465 6661 756c 7420  set the default 
+0000c4a0: 746f 6c65 7261 6e63 6573 2066 6f72 2074  tolerances for t
+0000c4b0: 6865 2063 6f6d 706f 6e65 6e74 730d 0a6d  he components..m
+0000c4c0: 632e 7365 745f 746f 6c65 7261 6e63 6528  c.set_tolerance(
+0000c4d0: 2752 272c 2030 2e30 3129 2020 2320 3125  'R', 0.01)  # 1%
+0000c4e0: 2074 6f6c 6572 616e 6365 2c20 6465 6661   tolerance, defa
+0000c4f0: 756c 7420 6469 7374 7269 6275 7469 6f6e  ult distribution
+0000c500: 2069 7320 756e 6966 6f72 6d0d 0a6d 632e   is uniform..mc.
+0000c510: 7365 745f 746f 6c65 7261 6e63 6528 2743  set_tolerance('C
+0000c520: 272c 2030 2e31 2c20 6469 7374 7269 6275  ', 0.1, distribu
+0000c530: 7469 6f6e 3d27 756e 6966 6f72 6d27 2920  tion='uniform') 
+0000c540: 2023 2031 3025 2074 6f6c 6572 616e 6365   # 10% tolerance
+0000c550: 2c20 6578 706c 6963 6974 2075 6e69 666f  , explicit unifo
+0000c560: 726d 2064 6973 7472 6962 7574 696f 6e0d  rm distribution.
+0000c570: 0a6d 632e 7365 745f 746f 6c65 7261 6e63  .mc.set_toleranc
+0000c580: 6528 2756 272c 2030 2e31 2c20 6469 7374  e('V', 0.1, dist
+0000c590: 7269 6275 7469 6f6e 3d27 6e6f 726d 616c  ribution='normal
+0000c5a0: 2729 2020 2320 3130 2520 746f 6c65 7261  ')  # 10% tolera
+0000c5b0: 6e63 652c 2062 7574 2075 7369 6e67 2061  nce, but using a
+0000c5c0: 206e 6f72 6d61 6c20 6469 7374 7269 6275   normal distribu
+0000c5d0: 7469 6f6e 0d0a 0d0a 2320 536f 6d65 2063  tion....# Some c
+0000c5e0: 6f6d 706f 6e65 6e74 7320 6361 6e20 6861  omponents can ha
+0000c5f0: 7665 2061 2064 6966 6665 7265 6e74 2074  ve a different t
+0000c600: 6f6c 6572 616e 6365 0d0a 6d63 2e73 6574  olerance..mc.set
+0000c610: 5f74 6f6c 6572 616e 6365 2827 5231 272c  _tolerance('R1',
+0000c620: 2030 2e30 3529 2020 2320 3525 2074 6f6c   0.05)  # 5% tol
+0000c630: 6572 616e 6365 2066 6f72 2052 3120 6f6e  erance for R1 on
+0000c640: 6c79 2e20 5468 6973 206f 6e6c 7920 6f76  ly. This only ov
+0000c650: 6572 7269 6465 7320 7468 6520 6465 6661  errides the defa
+0000c660: 756c 7420 746f 6c65 7261 6e63 6520 666f  ult tolerance fo
+0000c670: 7220 5231 0d0a 0d0a 2320 546f 6c65 7261  r R1....# Tolera
+0000c680: 6e63 6573 2063 616e 2062 6520 7365 7420  nces can be set 
+0000c690: 666f 7220 7061 7261 6d65 7465 7273 2061  for parameters a
+0000c6a0: 7320 7765 6c6c 0d0a 6d63 2e73 6574 5f70  s well..mc.set_p
+0000c6b0: 6172 616d 6574 6572 5f64 6576 6961 7469  arameter_deviati
+0000c6c0: 6f6e 2827 566f 7327 2c20 3365 2d34 2c20  on('Vos', 3e-4, 
+0000c6d0: 3565 2d33 2c20 2775 6e69 666f 726d 2729  5e-3, 'uniform')
+0000c6e0: 2020 2320 5468 6520 6b65 7977 6f72 6420    # The keyword 
+0000c6f0: 2764 6973 7472 6962 7574 696f 6e27 2069  'distribution' i
+0000c700: 7320 6f70 7469 6f6e 616c 0d0a 6d63 2e70  s optional..mc.p
+0000c710: 7265 7061 7265 5f74 6573 7462 656e 6368  repare_testbench
+0000c720: 286e 756d 5f72 756e 733d 3130 3030 2920  (num_runs=1000) 
+0000c730: 2023 2050 7265 7061 7265 7320 7468 6520   # Prepares the 
+0000c740: 7465 7374 6265 6e63 6820 666f 7220 3130  testbench for 10
+0000c750: 3030 2073 696d 756c 6174 696f 6e73 0d0a  00 simulations..
+0000c760: 0d0a 2320 4669 6e61 6c6c 7920 7468 6520  ..# Finally the 
+0000c770: 6e65 746c 6973 7420 6973 2073 6176 6564  netlist is saved
+0000c780: 2074 6f20 6120 6669 6c65 0d0a 6d63 2e73   to a file..mc.s
+0000c790: 6176 655f 6e65 746c 6973 7428 272e 2f74  ave_netlist('./t
+0000c7a0: 6573 7466 696c 6573 2f73 616c 6c65 6e6b  estfiles/sallenk
+0000c7b0: 6579 5f6d 632e 6e65 7427 290d 0a0d 0a6d  ey_mc.net')....m
+0000c7c0: 632e 7275 6e5f 7465 7374 6265 6e63 6828  c.run_testbench(
+0000c7d0: 7275 6e73 5f70 6572 5f73 696d 3d31 3030  runs_per_sim=100
+0000c7e0: 2920 2023 2052 756e 7320 7468 6520 7369  )  # Runs the si
+0000c7f0: 6d75 6c61 7469 6f6e 2077 6974 6820 7370  mulation with sp
+0000c800: 6c69 7473 206f 6620 3130 3020 7275 6e73  lits of 100 runs
+0000c810: 2065 6163 680d 0a6c 6f67 7320 3d20 6d63   each..logs = mc
+0000c820: 2e72 6561 645f 6c6f 6766 696c 6573 2829  .read_logfiles()
+0000c830: 2020 2023 2052 6561 6473 2074 6865 206c     # Reads the l
+0000c840: 6f67 2066 696c 6573 2061 6e64 2073 746f  og files and sto
+0000c850: 7265 7320 7468 6520 7265 7375 6c74 7320  res the results 
+0000c860: 696e 2074 6865 2072 6573 756c 7473 2061  in the results a
+0000c870: 7474 7269 6275 7465 0d0a 6c6f 6773 2e6f  ttribute..logs.o
+0000c880: 6274 6169 6e5f 616d 706c 6974 7564 655f  btain_amplitude_
+0000c890: 616e 645f 7068 6173 655f 6672 6f6d 5f63  and_phase_from_c
+0000c8a0: 6f6d 706c 6578 5f76 616c 7565 7328 2920  omplex_values() 
+0000c8b0: 2023 2053 706c 6974 7320 7468 6520 636f   # Splits the co
+0000c8c0: 6d70 6c65 7820 7661 6c75 6573 2069 6e74  mplex values int
+0000c8d0: 6f20 7265 616c 2061 6e64 2069 6d61 6769  o real and imagi
+0000c8e0: 6e61 7279 2070 6172 7473 0d0a 6c6f 6773  nary parts..logs
+0000c8f0: 2e65 7870 6f72 745f 6461 7461 2827 2e2f  .export_data('./
+0000c900: 7465 6d70 5f6d 632f 6461 7461 5f74 6573  temp_mc/data_tes
+0000c910: 7462 656e 6368 2e63 7376 2729 2020 2320  tbench.csv')  # 
+0000c920: 4578 706f 7274 7320 7468 6520 6461 7461  Exports the data
+0000c930: 2074 6f20 6120 6373 7620 6669 6c65 0d0a   to a csv file..
+0000c940: 6c6f 6773 2e70 6c6f 745f 6869 7374 6f67  logs.plot_histog
+0000c950: 7261 6d28 2766 6375 7427 2920 2023 2050  ram('fcut')  # P
+0000c960: 6c6f 7473 2074 6865 2068 6973 746f 6772  lots the histogr
+0000c970: 616d 7320 666f 7220 7468 6520 7265 7375  ams for the resu
+0000c980: 6c74 730d 0a6d 632e 636c 6561 6e75 705f  lts..mc.cleanup_
+0000c990: 6669 6c65 7328 2920 2023 2044 656c 6574  files()  # Delet
+0000c9a0: 6573 2074 6865 2074 656d 706f 7261 7279  es the temporary
+0000c9b0: 2066 696c 6573 0d0a 0d0a 7072 696e 7428   files....print(
+0000c9c0: 223d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  "===============
+0000c9d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c9e0: 3d3d 3d3d 3d3d 2229 0d0a 2320 4e6f 7720  ======")..# Now 
+0000c9f0: 7573 696e 6720 7468 6520 7365 636f 6e64  using the second
+0000ca00: 206d 6574 686f 642c 2077 6865 7265 2074   method, where t
+0000ca10: 6865 2073 696d 756c 6174 696f 6e73 2061  he simulations a
+0000ca20: 7265 2072 616e 206f 6e65 2062 7920 6f6e  re ran one by on
+0000ca30: 650d 0a6d 632e 636c 6561 725f 7369 6d75  e..mc.clear_simu
+0000ca40: 6c61 7469 6f6e 5f64 6174 6128 2920 2023  lation_data()  #
+0000ca50: 2043 6c65 6172 7320 7468 6520 7369 6d75   Clears the simu
+0000ca60: 6c61 7469 6f6e 2064 6174 610d 0a6d 632e  lation data..mc.
+0000ca70: 7265 7365 745f 6e65 746c 6973 7428 2920  reset_netlist() 
+0000ca80: 2023 2052 6573 6574 7320 7468 6520 6e65   # Resets the ne
+0000ca90: 746c 6973 7420 746f 2074 6865 206f 7269  tlist to the ori
+0000caa0: 6769 6e61 6c0d 0a6d 632e 7275 6e5f 616e  ginal..mc.run_an
+0000cab0: 616c 7973 6973 286e 756d 5f72 756e 733d  alysis(num_runs=
+0000cac0: 3130 3030 2920 2023 2052 756e 7320 7468  1000)  # Runs th
+0000cad0: 6520 3130 3030 2073 696d 756c 6174 696f  e 1000 simulatio
+0000cae0: 6e73 0d0a 6c6f 6773 203d 206d 632e 7265  ns..logs = mc.re
+0000caf0: 6164 5f6c 6f67 6669 6c65 7328 2920 2020  ad_logfiles()   
+0000cb00: 2320 5265 6164 7320 7468 6520 6c6f 6720  # Reads the log 
+0000cb10: 6669 6c65 7320 616e 6420 7374 6f72 6573  files and stores
+0000cb20: 2074 6865 2072 6573 756c 7473 2069 6e20   the results in 
+0000cb30: 7468 6520 7265 7375 6c74 7320 6174 7472  the results attr
+0000cb40: 6962 7574 650d 0a6c 6f67 732e 6578 706f  ibute..logs.expo
+0000cb50: 7274 5f64 6174 6128 272e 2f74 656d 705f  rt_data('./temp_
+0000cb60: 6d63 2f64 6174 615f 7369 6d73 2e63 7376  mc/data_sims.csv
+0000cb70: 2729 2020 2320 4578 706f 7274 7320 7468  ')  # Exports th
+0000cb80: 6520 6461 7461 2074 6f20 6120 6373 7620  e data to a csv 
+0000cb90: 6669 6c65 0d0a 6c6f 6773 2e70 6c6f 745f  file..logs.plot_
+0000cba0: 6869 7374 6f67 7261 6d28 2766 6375 7427  histogram('fcut'
+0000cbb0: 2920 2023 2050 6c6f 7473 2074 6865 2068  )  # Plots the h
+0000cbc0: 6973 746f 6772 616d 7320 666f 7220 7468  istograms for th
+0000cbd0: 6520 7265 7375 6c74 730d 0a6d 632e 636c  e results..mc.cl
+0000cbe0: 6561 6e75 705f 6669 6c65 7328 2920 2023  eanup_files()  #
+0000cbf0: 2044 656c 6574 6573 2074 6865 2074 656d   Deletes the tem
+0000cc00: 706f 7261 7279 2066 696c 6573 0d0a 0d0a  porary files....
+0000cc10: 6060 600d 0a2d 2d20 696e 2065 7861 6d70  ```..-- in examp
+0000cc20: 6c65 732f 7275 6e5f 6d6f 6e74 6563 6172  les/run_montecar
+0000cc30: 6c6f 2e70 790d 0a0d 0a57 6865 6e20 6f70  lo.py....When op
+0000cc40: 656e 696e 6720 7468 6520 6372 6561 7465  ening the create
+0000cc50: 6420 7361 6c6c 656e 6b65 795f 6d63 2e6e  d sallenkey_mc.n
+0000cc60: 6574 2066 696c 652c 2077 6520 6361 6e20  et file, we can 
+0000cc70: 7365 6520 7468 6174 2074 6865 2066 6f6c  see that the fol
+0000cc80: 6c6f 7769 6e67 2063 6972 6375 6974 2e0d  lowing circuit..
+0000cc90: 0a0d 0a21 5b53 616c 6c65 6e2d 4b65 7920  ...![Sallen-Key 
+0000cca0: 416d 706c 6966 6965 7220 7769 7468 204d  Amplifier with M
+0000ccb0: 6f6e 7465 6361 726c 6f5d 282e 2f64 6f63  ontecarlo](./doc
+0000ccc0: 2f6d 6f64 756c 6573 2f73 616c 6c65 6e6b  /modules/sallenk
+0000ccd0: 6579 5f6d 632e 706e 6720 2253 616c 6c65  ey_mc.png "Salle
+0000cce0: 6e2d 4b65 7920 416d 706c 6966 6965 7220  n-Key Amplifier 
+0000ccf0: 7769 7468 204d 6f6e 7465 6361 726c 6f22  with Montecarlo"
+0000cd00: 290d 0a0d 0a54 6865 2066 6f6c 6c6f 7769  )....The followi
+0000cd10: 6e67 2075 7064 6174 6573 2077 6572 6520  ng updates were 
+0000cd20: 6d61 6465 2074 6f20 7468 6520 6369 7263  made to the circ
+0000cd30: 7569 743a 0d0a 2d20 5468 6520 7661 6c75  uit:..- The valu
+0000cd40: 6520 6f66 2065 6163 6820 636f 6d70 6f6e  e of each compon
+0000cd50: 656e 7420 7761 7320 7265 706c 6163 6564  ent was replaced
+0000cd60: 2062 7920 6120 6675 6e63 7469 6f6e 2074   by a function t
+0000cd70: 6861 7420 6765 6e65 7261 7465 7320 6120  hat generates a 
+0000cd80: 7261 6e64 6f6d 2076 616c 7565 2077 6974  random value wit
+0000cd90: 6869 6e20 7468 6520 7370 6563 6966 6965  hin the specifie
+0000cda0: 6420 746f 6c65 7261 6e63 652e 0d0a 2d20  d tolerance...- 
+0000cdb0: 5468 6520 2e73 7465 7020 7061 7261 6d20  The .step param 
+0000cdc0: 7275 6e20 636f 6d6d 616e 6420 7761 7320  run command was 
+0000cdd0: 6164 6465 6420 746f 2074 6865 206e 6574  added to the net
+0000cde0: 6c69 7374 2e20 5374 6172 7473 2061 7420  list. Starts at 
+0000cdf0: 2d31 2077 6869 6368 2069 7427 7320 7468  -1 which it's th
+0000ce00: 6520 6e6f 6d69 6e61 6c20 7661 6c75 6520  e nominal value 
+0000ce10: 7369 6d75 6c61 7469 6f6e 2c20 616e 6420  simulation, and 
+0000ce20: 0d0a 6669 6e69 7368 6573 2074 6861 7420  ..finishes that 
+0000ce30: 7468 6520 6e75 6d62 6572 206f 6620 7369  the number of si
+0000ce40: 6d75 6c61 7469 6f6e 7320 7370 6563 6966  mulations specif
+0000ce50: 6965 6420 696e 2074 6865 2070 7265 7061  ied in the prepa
+0000ce60: 7265 5f74 6573 7462 656e 6368 2829 206d  re_testbench() m
+0000ce70: 6574 686f 642e 0d0a 2d20 4120 6465 6661  ethod...- A defa
+0000ce80: 756c 7420 7661 6c75 6520 666f 7220 7468  ult value for th
+0000ce90: 6520 7275 6e20 7061 7261 6d65 7465 7220  e run parameter 
+0000cea0: 7761 7320 6164 6465 642e 2054 6869 7320  was added. This 
+0000ceb0: 6973 2075 7365 6675 6c20 6966 2074 6865  is useful if the
+0000cec0: 202e 7374 6570 2070 6172 616d 2072 756e   .step param run
+0000ced0: 2069 7320 636f 6d6d 656e 7465 6420 6f75   is commented ou
+0000cee0: 742e 0d0a 2d20 5468 6520 5231 2074 6f6c  t...- The R1 tol
+0000cef0: 6572 616e 6365 2069 7320 6469 6666 6572  erance is differ
+0000cf00: 656e 7420 6672 6f6d 2074 6865 206f 7468  ent from the oth
+0000cf10: 6572 2072 6573 6973 746f 7273 2e20 5468  er resistors. Th
+0000cf20: 6973 2069 7320 6265 6361 7573 6520 7468  is is because th
+0000cf30: 6520 746f 6c65 7261 6e63 6520 7761 7320  e tolerance was 
+0000cf40: 6578 706c 6963 6974 6c79 2073 6574 2066  explicitly set f
+0000cf50: 6f72 2052 312e 0d0a 2d20 5468 6520 566f  or R1...- The Vo
+0000cf60: 7320 7061 7261 6d65 7465 7220 7761 7320  s parameter was 
+0000cf70: 6164 6465 6420 746f 2074 6865 202e 7061  added to the .pa
+0000cf80: 7261 6d20 6c69 7374 2e20 5468 6973 2069  ram list. This i
+0000cf90: 7320 6265 6361 7573 6520 7468 6520 7061  s because the pa
+0000cfa0: 7261 6d65 7465 7220 7761 7320 6578 706c  rameter was expl
+0000cfb0: 6963 6974 6c79 2073 6574 2075 7369 6e67  icitly set using
+0000cfc0: 2074 6865 0d0a 7365 745f 7061 7261 6d65   the..set_parame
+0000cfd0: 7465 725f 6465 7669 6174 696f 6e20 6d65  ter_deviation me
+0000cfe0: 7468 6f64 2e0d 0a2d 2046 756e 6374 696f  thod...- Functio
+0000cff0: 6e73 2075 746f 6c2c 206e 746f 6c20 616e  ns utol, ntol an
+0000d000: 6420 7572 6e67 2077 6572 6520 6164 6465  d urng were adde
+0000d010: 6420 746f 2074 6865 202e 6675 6e63 206c  d to the .func l
+0000d020: 6973 742e 2054 6865 7365 2066 756e 6374  ist. These funct
+0000d030: 696f 6e73 2061 7265 2075 7365 6420 746f  ions are used to
+0000d040: 2067 656e 6572 6174 6520 7261 6e64 6f6d   generate random
+0000d050: 2076 616c 7565 732e 0d0a 556e 6966 6f72   values...Unifor
+0000d060: 6d20 6469 7374 7269 6275 7469 6f6e 7320  m distributions 
+0000d070: 7573 6520 7468 6520 4c54 5370 6963 6520  use the LTSpice 
+0000d080: 6275 696c 742d 696e 206d 6328 782c 2074  built-in mc(x, t
+0000d090: 6f6c 2920 616e 6420 666c 6174 2878 2920  ol) and flat(x) 
+0000d0a0: 6675 6e63 7469 6f6e 732c 2077 6869 6c65  functions, while
+0000d0b0: 206e 6f72 6d61 6c20 6469 7374 7269 6275   normal distribu
+0000d0c0: 7469 6f6e 7320 7573 6520 7468 6520 0d0a  tions use the ..
+0000d0d0: 6761 7573 7328 7829 2066 756e 6374 696f  gauss(x) functio
+0000d0e0: 6e2e 0d0a 0d0a 5369 6d69 6c61 726c 792c  n.....Similarly,
+0000d0f0: 2074 6865 2077 6f72 7374 2063 6173 6520   the worst case 
+0000d100: 616e 616c 7973 6973 2063 616e 2061 6c73  analysis can als
+0000d110: 6f20 6265 2073 6574 7570 2062 7920 7573  o be setup by us
+0000d120: 696e 6720 7468 6520 636c 6173 7320 576f  ing the class Wo
+0000d130: 7273 7443 6173 6541 6e61 6c79 7369 732c  rstCaseAnalysis,
+0000d140: 2061 7320 6578 656d 706c 6966 6965 6420   as exemplified 
+0000d150: 6265 6c6f 773a 0d0a 0d0a 6060 6070 7974  below:....```pyt
+0000d160: 686f 6e0d 0a66 726f 6d20 5079 4c54 5370  hon..from PyLTSp
+0000d170: 6963 6520 696d 706f 7274 2041 7363 4564  ice import AscEd
+0000d180: 6974 6f72 2c20 5369 6d52 756e 6e65 7220  itor, SimRunner 
+0000d190: 2023 2049 6d70 6f72 7473 2074 6865 2063   # Imports the c
+0000d1a0: 6c61 7373 2074 6861 7420 6d61 6e69 7075  lass that manipu
+0000d1b0: 6c61 7465 7320 7468 6520 6173 6320 6669  lates the asc fi
+0000d1c0: 6c65 0d0a 6672 6f6d 2050 794c 5453 7069  le..from PyLTSpi
+0000d1d0: 6365 2e73 696d 2e74 6f6f 6b69 742e 776f  ce.sim.tookit.wo
+0000d1e0: 7273 745f 6361 7365 2069 6d70 6f72 7420  rst_case import 
+0000d1f0: 576f 7273 7443 6173 6541 6e61 6c79 7369  WorstCaseAnalysi
+0000d200: 730d 0a0d 0a73 616c 6c65 6e6b 6579 203d  s....sallenkey =
+0000d210: 2041 7363 4564 6974 6f72 2822 2e2f 7465   AscEditor("./te
+0000d220: 7374 6669 6c65 732f 7361 6c6c 656e 6b65  stfiles/sallenke
+0000d230: 792e 6173 6322 2920 2023 2052 6561 6473  y.asc")  # Reads
+0000d240: 2074 6865 2061 7363 2066 696c 6520 696e   the asc file in
+0000d250: 746f 206d 656d 6f72 790d 0a72 756e 6e65  to memory..runne
+0000d260: 7220 3d20 5369 6d52 756e 6e65 7228 6f75  r = SimRunner(ou
+0000d270: 7470 7574 5f66 6f6c 6465 723d 272e 2f74  tput_folder='./t
+0000d280: 656d 705f 7763 6127 2920 2023 2049 6e73  emp_wca')  # Ins
+0000d290: 7461 6e74 6961 7465 7320 7468 6520 7275  tantiates the ru
+0000d2a0: 6e6e 6572 2063 6c61 7373 2c20 7769 7468  nner class, with
+0000d2b0: 2074 6865 206f 7574 7075 7420 666f 6c64   the output fold
+0000d2c0: 6572 2061 6c72 6561 6479 2073 6574 0d0a  er already set..
+0000d2d0: 7763 6120 3d20 576f 7273 7443 6173 6541  wca = WorstCaseA
+0000d2e0: 6e61 6c79 7369 7328 7361 6c6c 656e 6b65  nalysis(sallenke
+0000d2f0: 792c 2072 756e 6e65 7229 2020 2320 496e  y, runner)  # In
+0000d300: 7374 616e 7469 6174 6573 2074 6865 2057  stantiates the W
+0000d310: 6f72 7374 2043 6173 6520 416e 616c 7973  orst Case Analys
+0000d320: 6973 2063 6c61 7373 0d0a 0d0a 2320 5468  is class....# Th
+0000d330: 6520 666f 6c6c 6f77 696e 6720 6c69 6e65  e following line
+0000d340: 7320 7365 7420 7468 6520 6465 6661 756c  s set the defaul
+0000d350: 7420 746f 6c65 7261 6e63 6573 2066 6f72  t tolerances for
+0000d360: 2074 6865 2063 6f6d 706f 6e65 6e74 730d   the components.
+0000d370: 0a77 6361 2e73 6574 5f74 6f6c 6572 616e  .wca.set_toleran
+0000d380: 6365 2827 5227 2c20 302e 3031 2920 2023  ce('R', 0.01)  #
+0000d390: 2031 2520 746f 6c65 7261 6e63 650d 0a77   1% tolerance..w
+0000d3a0: 6361 2e73 6574 5f74 6f6c 6572 616e 6365  ca.set_tolerance
+0000d3b0: 2827 4327 2c20 302e 3129 2020 2320 3130  ('C', 0.1)  # 10
+0000d3c0: 2520 746f 6c65 7261 6e63 650d 0a77 6361  % tolerance..wca
+0000d3d0: 2e73 6574 5f74 6f6c 6572 616e 6365 2827  .set_tolerance('
+0000d3e0: 5627 2c20 302e 3129 2020 2320 3130 2520  V', 0.1)  # 10% 
+0000d3f0: 746f 6c65 7261 6e63 652e 2046 6f72 2057  tolerance. For W
+0000d400: 6f72 7374 2043 6173 6520 616e 616c 7973  orst Case analys
+0000d410: 6973 2c20 7468 6520 6469 7374 7269 6275  is, the distribu
+0000d420: 7469 6f6e 2069 7320 6972 7265 6c65 7661  tion is irreleva
+0000d430: 6e74 0d0a 0d0a 2320 536f 6d65 2063 6f6d  nt....# Some com
+0000d440: 706f 6e65 6e74 7320 6361 6e20 6861 7665  ponents can have
+0000d450: 2061 2064 6966 6665 7265 6e74 2074 6f6c   a different tol
+0000d460: 6572 616e 6365 0d0a 7763 612e 7365 745f  erance..wca.set_
+0000d470: 746f 6c65 7261 6e63 6528 2752 3127 2c20  tolerance('R1', 
+0000d480: 302e 3035 2920 2023 2035 2520 746f 6c65  0.05)  # 5% tole
+0000d490: 7261 6e63 6520 666f 7220 5231 206f 6e6c  rance for R1 onl
+0000d4a0: 792e 2054 6869 7320 6f6e 6c79 206f 7665  y. This only ove
+0000d4b0: 7272 6964 6573 2074 6865 2064 6566 6175  rrides the defau
+0000d4c0: 6c74 2074 6f6c 6572 616e 6365 2066 6f72  lt tolerance for
+0000d4d0: 2052 310d 0a0d 0a23 2054 6f6c 6572 616e   R1....# Toleran
+0000d4e0: 6365 7320 6361 6e20 6265 2073 6574 2066  ces can be set f
+0000d4f0: 6f72 2070 6172 616d 6574 6572 7320 6173  or parameters as
+0000d500: 2077 656c 6c2e 0d0a 7763 612e 7365 745f   well...wca.set_
+0000d510: 7061 7261 6d65 7465 725f 6465 7669 6174  parameter_deviat
+0000d520: 696f 6e28 2756 6f73 272c 2033 652d 342c  ion('Vos', 3e-4,
+0000d530: 2035 652d 3329 0d0a 0d0a 2320 4669 6e61   5e-3)....# Fina
+0000d540: 6c6c 7920 7468 6520 6e65 746c 6973 7420  lly the netlist 
+0000d550: 6973 2073 6176 6564 2074 6f20 6120 6669  is saved to a fi
+0000d560: 6c65 0d0a 7763 612e 7361 7665 5f6e 6574  le..wca.save_net
+0000d570: 6c69 7374 2827 2e2f 7465 7374 6669 6c65  list('./testfile
+0000d580: 732f 7361 6c6c 656e 6b65 795f 7763 2e61  s/sallenkey_wc.a
+0000d590: 7363 2729 0d0a 0d0a 7763 612e 7275 6e5f  sc')....wca.run_
+0000d5a0: 7465 7374 6265 6e63 6828 2920 2023 2052  testbench()  # R
+0000d5b0: 756e 7320 7468 6520 7369 6d75 6c61 7469  uns the simulati
+0000d5c0: 6f6e 2077 6974 6820 7370 6c69 7473 206f  on with splits o
+0000d5d0: 6620 3130 3020 7275 6e73 2065 6163 680d  f 100 runs each.
+0000d5e0: 0a0d 0a6c 6f67 7320 3d20 7763 612e 7265  ...logs = wca.re
+0000d5f0: 6164 5f6c 6f67 6669 6c65 7328 2920 2020  ad_logfiles()   
+0000d600: 2320 5265 6164 7320 7468 6520 6c6f 6720  # Reads the log 
+0000d610: 6669 6c65 7320 616e 6420 7374 6f72 6573  files and stores
+0000d620: 2074 6865 2072 6573 756c 7473 2069 6e20   the results in 
+0000d630: 7468 6520 7265 7375 6c74 7320 6174 7472  the results attr
+0000d640: 6962 7574 650d 0a6c 6f67 732e 6578 706f  ibute..logs.expo
+0000d650: 7274 5f64 6174 6128 272e 2f74 656d 705f  rt_data('./temp_
+0000d660: 7763 612f 6461 7461 2e63 7376 2729 2020  wca/data.csv')  
+0000d670: 2320 4578 706f 7274 7320 7468 6520 6461  # Exports the da
+0000d680: 7461 2074 6f20 6120 6373 7620 6669 6c65  ta to a csv file
+0000d690: 0d0a 0d0a 7072 696e 7428 2257 6f72 7374  ....print("Worst
+0000d6a0: 2063 6173 6520 7265 7375 6c74 733a 2229   case results:")
+0000d6b0: 0d0a 666f 7220 7061 7261 6d20 696e 2028  ..for param in (
+0000d6c0: 2766 6375 7427 2c20 2766 6375 745f 4652  'fcut', 'fcut_FR
+0000d6d0: 4f4d 2729 3a0d 0a20 2020 2070 7269 6e74  OM'):..    print
+0000d6e0: 2866 227b 7061 7261 6d7d 3a20 6d69 6e3a  (f"{param}: min:
+0000d6f0: 7b6c 6f67 732e 6d69 6e5f 6d65 6173 7572  {logs.min_measur
+0000d700: 655f 7661 6c75 6528 7061 7261 6d29 7d20  e_value(param)} 
+0000d710: 6d61 783a 7b6c 6f67 732e 6d61 785f 6d65  max:{logs.max_me
+0000d720: 6173 7572 655f 7661 6c75 6528 7061 7261  asure_value(para
+0000d730: 6d29 7d22 290d 0a0d 0a77 6361 2e63 6c65  m)}")....wca.cle
+0000d740: 616e 7570 5f66 696c 6573 2829 2020 2320  anup_files()  # 
+0000d750: 4465 6c65 7465 7320 7468 6520 7465 6d70  Deletes the temp
+0000d760: 6f72 6172 7920 6669 6c65 730d 0a60 6060  orary files..```
+0000d770: 0d0a 2d2d 2069 6e20 6578 616d 706c 6573  ..-- in examples
+0000d780: 2f72 756e 5f77 6f72 7374 5f63 6173 652e  /run_worst_case.
+0000d790: 7079 0d0a 0d0a 5768 656e 206f 7065 6e69  py....When openi
+0000d7a0: 6e67 2074 6865 2063 7265 6174 6564 2073  ng the created s
+0000d7b0: 616c 6c65 6e6b 6579 5f77 632e 6e65 7420  allenkey_wc.net 
+0000d7c0: 6669 6c65 2c20 7765 2063 616e 2073 6565  file, we can see
+0000d7d0: 2074 6861 7420 7468 6520 666f 6c6c 6f77   that the follow
+0000d7e0: 696e 6720 6369 7263 7569 742e 0d0a 0d0a  ing circuit.....
+0000d7f0: 215b 5361 6c6c 656e 2d4b 6579 2041 6d70  ![Sallen-Key Amp
+0000d800: 6c69 6669 6572 2077 6974 6820 5743 415d  lifier with WCA]
+0000d810: 282e 2f64 6f63 2f6d 6f64 756c 6573 2f73  (./doc/modules/s
+0000d820: 616c 6c65 6e6b 6579 5f77 632e 706e 6720  allenkey_wc.png 
+0000d830: 2253 616c 6c65 6e2d 4b65 7920 416d 706c  "Sallen-Key Ampl
+0000d840: 6966 6965 7220 7769 7468 2057 4341 2229  ifier with WCA")
+0000d850: 0d0a 0d0a 5468 6520 666f 6c6c 6f77 696e  ....The followin
+0000d860: 6720 7570 6461 7465 7320 7765 7265 206d  g updates were m
+0000d870: 6164 6520 746f 2074 6865 2063 6972 6375  ade to the circu
+0000d880: 6974 3a0d 0a2d 2054 6865 2076 616c 7565  it:..- The value
+0000d890: 206f 6620 6561 6368 2063 6f6d 706f 6e65   of each compone
+0000d8a0: 6e74 2077 6173 2072 6570 6c61 6365 6420  nt was replaced 
+0000d8b0: 6279 2061 2066 756e 6374 696f 6e20 7468  by a function th
+0000d8c0: 6174 2067 656e 6572 6174 6573 2061 206e  at generates a n
+0000d8d0: 6f6d 696e 616c 2c20 6d69 6e69 6d75 6d20  ominal, minimum 
+0000d8e0: 616e 6420 6d61 7869 6d75 6d20 7661 6c75  and maximum valu
+0000d8f0: 6520 6465 7065 6e64 696e 670d 0a6f 6e20  e depending..on 
+0000d900: 7468 6520 7275 6e20 7061 7261 6d65 7465  the run paramete
+0000d910: 7220 616e 6420 6973 2061 7373 6967 6e65  r and is assigne
+0000d920: 6420 6120 756e 6971 7565 2069 6e64 6578  d a unique index
+0000d930: 206e 756d 6265 722e 2028 5231 3d30 2c20   number. (R1=0, 
+0000d940: 566f 733d 312c 2052 323d 322c 202e 2e2e  Vos=1, R2=2, ...
+0000d950: 2056 323d 372c 2056 494e 3d38 290d 0a54   V2=7, VIN=8)..T
+0000d960: 6865 2075 6e69 7175 6520 6e75 6d62 6572  he unique number
+0000d970: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
+0000d980: 7468 6520 6269 7420 706f 7369 7469 6f6e  the bit position
+0000d990: 206f 6620 7468 6520 7275 6e20 7061 7261   of the run para
+0000d9a0: 6d65 7465 722e 2042 6974 2030 2063 6f72  meter. Bit 0 cor
+0000d9b0: 7265 7370 6f6e 6473 2074 6f20 7468 6520  responds to the 
+0000d9c0: 6d69 6e69 6d75 6d20 7661 6c75 6520 616e  minimum value an
+0000d9d0: 640d 0a62 6974 2031 2063 6f72 7265 7370  d..bit 1 corresp
+0000d9e0: 6f6e 6473 2074 6f20 7468 6520 6d61 7869  onds to the maxi
+0000d9f0: 6d75 6d20 7661 6c75 652e 2043 616c 6375  mum value. Calcu
+0000da00: 6c61 7469 6e67 2061 6c6c 2070 6f73 7369  lating all possi
+0000da10: 626c 6520 7065 726d 7574 6174 696f 6e73  ble permutations
+0000da20: 206f 6620 6d61 7869 6d75 6d20 616e 6420   of maximum and 
+0000da30: 6d69 6e69 6d75 6d20 7661 6c75 6573 2066  minimum values f
+0000da40: 6f72 2065 6163 680d 0a63 6f6d 706f 6e65  or each..compone
+0000da50: 6e74 2c20 7765 2067 6574 2032 2a2a 3920  nt, we get 2**9 
+0000da60: 3d20 3531 3220 706f 7373 6962 6c65 2063  = 512 possible c
+0000da70: 6f6d 6269 6e61 7469 6f6e 732e 2054 6869  ombinations. Thi
+0000da80: 7320 6d61 7073 2069 6e74 6f20 6120 3920  s maps into a 9 
+0000da90: 6269 7420 6269 6e61 7279 206e 756d 6265  bit binary numbe
+0000daa0: 722c 2077 6869 6368 2069 7320 7468 6520  r, which is the 
+0000dab0: 7275 6e20 7061 7261 6d65 7465 722e 0d0a  run parameter...
+0000dac0: 2d20 5468 6520 2e73 7465 7020 7061 7261  - The .step para
+0000dad0: 6d20 7275 6e20 636f 6d6d 616e 6420 7761  m run command wa
+0000dae0: 7320 6164 6465 6420 746f 2074 6865 206e  s added to the n
+0000daf0: 6574 6c69 7374 2e20 4974 2073 7461 7274  etlist. It start
+0000db00: 7320 6174 202d 3120 7768 6963 6820 6974  s at -1 which it
+0000db10: 2773 2074 6865 206e 6f6d 696e 616c 2076  's the nominal v
+0000db20: 616c 7565 2073 696d 756c 6174 696f 6e2c  alue simulation,
+0000db30: 2074 6865 6e20 300d 0a77 6869 6368 2063   then 0..which c
+0000db40: 6f72 7265 7370 6f6e 6473 2074 6f20 7468  orresponds to th
+0000db50: 6520 6d69 6e69 6d75 6d20 7661 6c75 6520  e minimum value 
+0000db60: 666f 7220 6561 6368 2063 6f6d 706f 6e65  for each compone
+0000db70: 6e74 2c20 7468 656e 2069 7420 6d61 6b65  nt, then it make
+0000db80: 7320 616c 6c20 636f 6d62 696e 6174 696f  s all combinatio
+0000db90: 6e73 206f 6620 6d69 6e69 6d75 6d20 616e  ns of minimum an
+0000dba0: 6420 6d61 7869 6d75 6d20 7661 6c75 6573  d maximum values
+0000dbb0: 200d 0a75 6e74 696c 2035 3131 2c20 7768   ..until 511, wh
+0000dbc0: 6963 6820 6973 2074 6865 2073 696d 756c  ich is the simul
+0000dbd0: 6174 696f 6e20 7769 7468 2061 6c6c 206d  ation with all m
+0000dbe0: 6178 696d 756d 2076 616c 7565 732e 0d0a  aximum values...
+0000dbf0: 2d20 4120 6465 6661 756c 7420 7661 6c75  - A default valu
+0000dc00: 6520 666f 7220 7468 6520 7275 6e20 7061  e for the run pa
+0000dc10: 7261 6d65 7465 7220 7761 7320 6164 6465  rameter was adde
+0000dc20: 642e 2054 6869 7320 6973 2075 7365 6675  d. This is usefu
+0000dc30: 6c20 6966 2074 6865 202e 7374 6570 2070  l if the .step p
+0000dc40: 6172 616d 2072 756e 2069 7320 636f 6d6d  aram run is comm
+0000dc50: 656e 7465 6420 6f75 742e 0d0a 2d20 5468  ented out...- Th
+0000dc60: 6520 5231 2074 6f6c 6572 616e 6365 2069  e R1 tolerance i
+0000dc70: 7320 6469 6666 6572 656e 7420 6672 6f6d  s different from
+0000dc80: 2074 6865 206f 7468 6572 2072 6573 6973   the other resis
+0000dc90: 746f 7273 2e20 5468 6973 2069 7320 6265  tors. This is be
+0000dca0: 6361 7573 6520 7468 6520 746f 6c65 7261  cause the tolera
+0000dcb0: 6e63 6520 7761 7320 6578 706c 6963 6974  nce was explicit
+0000dcc0: 6c79 2073 6574 2066 6f72 2052 312e 0d0a  ly set for R1...
+0000dcd0: 2d20 5468 6520 7763 2829 2066 756e 6374  - The wc() funct
+0000dce0: 696f 6e20 6973 2061 6464 6564 2074 6f20  ion is added to 
+0000dcf0: 7468 6520 6369 7263 7569 742e 2054 6869  the circuit. Thi
+0000dd00: 7320 6675 6e63 7469 6f6e 2069 7320 7573  s function is us
+0000dd10: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
+0000dd20: 7468 6520 776f 7273 7420 6361 7365 2076  the worst case v
+0000dd30: 616c 7565 2066 6f72 2065 6163 6820 636f  alue for each co
+0000dd40: 6d70 6f6e 656e 742c 0d0a 6769 7665 6e20  mponent,..given 
+0000dd50: 6120 746f 6c65 7261 6e63 6520 7661 6c75  a tolerance valu
+0000dd60: 6520 616e 6420 6974 7320 7265 7370 6563  e and its respec
+0000dd70: 7469 7665 2069 6e64 6578 2e0d 0a2d 2054  tive index...- T
+0000dd80: 6865 2077 6331 2829 2066 756e 6374 696f  he wc1() functio
+0000dd90: 6e20 6973 2061 6464 6564 2074 6f20 7468  n is added to th
+0000dda0: 6520 6369 7263 7569 742e 2054 6869 7320  e circuit. This 
+0000ddb0: 6675 6e63 7469 6f6e 2069 7320 7573 6564  function is used
+0000ddc0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+0000ddd0: 6520 776f 7273 7420 6361 7365 2076 616c  e worst case val
+0000dde0: 7565 2066 6f72 2065 6163 6820 636f 6d70  ue for each comp
+0000ddf0: 6f6e 656e 742c 0d0a 6769 7665 6e20 6120  onent,..given a 
+0000de00: 6d69 6e69 6d75 6d20 616e 6420 6d61 7869  minimum and maxi
+0000de10: 6d75 6d20 7661 6c75 6520 616e 6420 6974  mum value and it
+0000de20: 7320 7265 7370 6563 7469 7665 2069 6e64  s respective ind
+0000de30: 6578 2e0d 0a0d 0a23 2323 204c 5453 7465  ex.....### LTSte
+0000de40: 7073 2e70 7920 2323 230d 0a0d 0a54 6869  ps.py ###....Thi
+0000de50: 7320 6d6f 6475 6c65 2064 6566 696e 6573  s module defines
+0000de60: 2061 2063 6c61 7373 2074 6861 7420 6361   a class that ca
+0000de70: 6e20 6265 2075 7365 6420 746f 2070 6172  n be used to par
+0000de80: 7365 204c 5453 7069 6365 206c 6f67 2066  se LTSpice log f
+0000de90: 696c 6573 2077 6865 7265 2074 6865 2069  iles where the i
+0000dea0: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+0000deb0: 202e 5354 4550 2069 6e66 6f72 6d61 7469   .STEP informati
+0000dec0: 6f6e 2069 730d 0a77 7269 7474 656e 2e20  on is..written. 
+0000ded0: 5468 6572 6520 6172 6520 7477 6f20 706f  There are two po
+0000dee0: 7373 6962 6c65 2075 7361 6765 7320 6f66  ssible usages of
+0000def0: 2074 6869 7320 6d6f 6475 6c65 2c20 6569   this module, ei
+0000df00: 7468 6572 2070 726f 6772 616d 6d61 7469  ther programmati
+0000df10: 6361 6c6c 7920 6279 2069 6d70 6f72 7469  cally by importi
+0000df20: 6e67 2074 6865 206d 6f64 756c 6520 616e  ng the module an
+0000df30: 6420 7468 656e 0d0a 6163 6365 7373 696e  d then..accessin
+0000df40: 6720 6461 7461 2074 6872 6f75 6768 2074  g data through t
+0000df50: 6865 2063 6c61 7373 2061 7320 6578 656d  he class as exem
+0000df60: 706c 6966 6965 6420 6865 7265 3a0d 0a0d  plified here:...
+0000df70: 0a60 6060 7079 7468 6f6e 0d0a 2321 2f75  .```python..#!/u
+0000df80: 7372 2f62 696e 2f65 6e76 2070 7974 686f  sr/bin/env pytho
+0000df90: 6e0d 0a23 2063 6f64 696e 673d 7574 662d  n..# coding=utf-
+0000dfa0: 380d 0a0d 0a66 726f 6d20 5079 4c54 5370  8....from PyLTSp
+0000dfb0: 6963 652e 6c6f 672e 6c74 7374 6570 7320  ice.log.ltsteps 
+0000dfc0: 696d 706f 7274 204c 5453 7069 6365 4c6f  import LTSpiceLo
+0000dfd0: 6752 6561 6465 720d 0a0d 0a64 6174 6120  gReader....data 
+0000dfe0: 3d20 4c54 5370 6963 654c 6f67 5265 6164  = LTSpiceLogRead
+0000dff0: 6572 2822 2e2f 7465 7374 6669 6c65 732f  er("./testfiles/
+0000e000: 4261 7463 685f 5465 7374 5f41 4438 3230  Batch_Test_AD820
+0000e010: 5f31 352e 6c6f 6722 290d 0a0d 0a70 7269  _15.log")....pri
+0000e020: 6e74 2822 4e75 6d62 6572 206f 6620 7374  nt("Number of st
+0000e030: 6570 7320 203a 222c 2064 6174 612e 7374  eps  :", data.st
+0000e040: 6570 5f63 6f75 6e74 290d 0a73 7465 705f  ep_count)..step_
+0000e050: 6e61 6d65 7320 3d20 6461 7461 2e67 6574  names = data.get
+0000e060: 5f73 7465 705f 7661 7273 2829 0d0a 6d65  _step_vars()..me
+0000e070: 6173 5f6e 616d 6573 203d 2064 6174 612e  as_names = data.
+0000e080: 6765 745f 6d65 6173 7572 655f 6e61 6d65  get_measure_name
+0000e090: 7328 290d 0a0d 0a23 2050 7269 6e74 696e  s()....# Printin
+0000e0a0: 6720 4865 6164 6572 730d 0a70 7269 6e74  g Headers..print
+0000e0b0: 2827 2027 2e6a 6f69 6e28 5b66 227b 7374  (' '.join([f"{st
+0000e0c0: 6570 3a31 3573 7d22 2066 6f72 2073 7465  ep:15s}" for ste
+0000e0d0: 7020 696e 2073 7465 705f 6e61 6d65 735d  p in step_names]
+0000e0e0: 292c 2065 6e64 3d27 2729 2020 2320 5072  ), end='')  # Pr
+0000e0f0: 696e 7420 7374 6570 7320 6e61 6d65 7320  int steps names 
+0000e100: 7769 7468 206e 6f20 6e65 7720 6c69 6e65  with no new line
+0000e110: 0d0a 7072 696e 7428 2720 272e 6a6f 696e  ..print(' '.join
+0000e120: 285b 6622 7b6e 616d 653a 3135 737d 2220  ([f"{name:15s}" 
+0000e130: 666f 7220 6e61 6d65 2069 6e20 6d65 6173  for name in meas
+0000e140: 5f6e 616d 6573 5d29 2c20 656e 643d 275c  _names]), end='\
+0000e150: 6e27 290d 0a23 2050 7269 6e74 696e 6720  n')..# Printing 
+0000e160: 6461 7461 0d0a 666f 7220 6920 696e 2072  data..for i in r
+0000e170: 616e 6765 2864 6174 612e 7374 6570 5f63  ange(data.step_c
+0000e180: 6f75 6e74 293a 0d0a 2020 2020 7072 696e  ount):..    prin
+0000e190: 7428 2720 272e 6a6f 696e 285b 6622 7b64  t(' '.join([f"{d
+0000e1a0: 6174 615b 7374 6570 5d5b 695d 3a31 357d  ata[step][i]:15}
+0000e1b0: 2220 666f 7220 7374 6570 2069 6e20 7374  " for step in st
+0000e1c0: 6570 5f6e 616d 6573 5d29 2c20 656e 643d  ep_names]), end=
+0000e1d0: 2727 2920 2023 2050 7269 6e74 2073 7465  '')  # Print ste
+0000e1e0: 7073 206e 616d 6573 2077 6974 6820 6e6f  ps names with no
+0000e1f0: 206e 6577 206c 696e 650d 0a20 2020 2070   new line..    p
+0000e200: 7269 6e74 2827 2027 2e6a 6f69 6e28 5b66  rint(' '.join([f
+0000e210: 227b 6461 7461 5b6e 616d 655d 5b69 5d3a  "{data[name][i]:
+0000e220: 3135 7d22 2066 6f72 206e 616d 6520 696e  15}" for name in
+0000e230: 206d 6561 735f 6e61 6d65 735d 292c 2065   meas_names]), e
+0000e240: 6e64 3d27 5c6e 2729 2020 2320 5072 696e  nd='\n')  # Prin
+0000e250: 7420 4865 6164 6572 0d0a 0d0a 7072 696e  t Header....prin
+0000e260: 7428 2254 6f74 616c 206e 756d 6265 7220  t("Total number 
+0000e270: 6f66 206d 6561 7375 7265 7320 666f 756e  of measures foun
+0000e280: 6420 3a22 2c20 6461 7461 2e6d 6561 7375  d :", data.measu
+0000e290: 7265 5f63 6f75 6e74 290d 0a60 6060 0d0a  re_count)..```..
+0000e2a0: 2d2d 2069 6e20 6578 616d 706c 6573 2f6c  -- in examples/l
+0000e2b0: 7473 7465 7073 5f65 7861 6d70 6c65 2e70  tsteps_example.p
+0000e2c0: 790d 0a0d 0a54 6865 2073 6563 6f6e 6420  y....The second 
+0000e2d0: 706f 7373 6962 696c 6974 7920 6973 2074  possibility is t
+0000e2e0: 6f20 7573 6520 7468 6520 6d6f 6475 6c65  o use the module
+0000e2f0: 2064 6972 6563 746c 7920 6f6e 2074 6865   directly on the
+0000e300: 2063 6f6d 6d61 6e64 206c 696e 650d 0a0d   command line...
+0000e310: 0a23 2043 6f6d 6d61 6e64 204c 696e 6520  .# Command Line 
+0000e320: 496e 7465 7266 6163 6520 230d 0a0d 0a23  Interface #....#
+0000e330: 2323 206c 7473 7465 7073 2e65 7865 2023  ## ltsteps.exe #
+0000e340: 2323 0d0a 0d0a 5468 6520 3c66 696c 656e  ##....The <filen
+0000e350: 616d 653e 2063 616e 2062 6520 6569 7468  ame> can be eith
+0000e360: 6572 2062 6520 6120 6c6f 6720 6669 6c65  er be a log file
+0000e370: 2028 2e6c 6f67 292c 2061 2064 6174 6120   (.log), a data 
+0000e380: 6578 706f 7274 2066 696c 6520 282e 7478  export file (.tx
+0000e390: 7429 206f 7220 6120 6d65 6173 7572 656d  t) or a measurem
+0000e3a0: 656e 7420 6f75 7470 7574 2066 696c 6520  ent output file 
+0000e3b0: 282e 6d65 6173 290d 0a54 6869 7320 7769  (.meas)..This wi
+0000e3c0: 6c6c 2070 726f 6365 7373 2061 6c6c 2074  ll process all t
+0000e3d0: 6865 2064 6174 6120 616e 6420 6578 706f  he data and expo
+0000e3e0: 7274 2069 7420 6175 746f 6d61 7469 6361  rt it automatica
+0000e3f0: 6c6c 7920 696e 746f 2061 2074 6578 7420  lly into a text 
+0000e400: 6669 6c65 2077 6974 6820 7468 6520 6578  file with the ex
+0000e410: 7465 6e73 696f 6e20 2874 6c6f 672c 2074  tension (tlog, t
+0000e420: 7376 2c20 746d 6561 7329 0d0a 7768 6572  sv, tmeas)..wher
+0000e430: 6520 7468 6520 6461 7461 2072 6561 6420  e the data read 
+0000e440: 6973 2066 6f72 6d61 7474 6564 2069 6e74  is formatted int
+0000e450: 6f20 6120 6d6f 7265 2063 6f6e 7665 6e69  o a more conveni
+0000e460: 656e 7420 7461 6220 7365 7061 7261 7465  ent tab separate
+0000e470: 6420 666f 726d 6174 2e20 496e 2063 6173  d format. In cas
+0000e480: 6520 7468 6520 3c6c 6f67 6669 6c65 3e20  e the <logfile> 
+0000e490: 6973 206e 6f74 2070 726f 7669 6465 642c  is not provided,
+0000e4a0: 2074 6865 0d0a 7363 7269 7074 2077 696c   the..script wil
+0000e4b0: 6c20 7363 616e 2074 6865 2064 6972 6563  l scan the direc
+0000e4c0: 746f 7279 2061 6e64 2070 726f 6365 7373  tory and process
+0000e4d0: 2074 6865 206e 6577 6573 7420 6c6f 672c   the newest log,
+0000e4e0: 2074 7874 206f 7220 6f75 7420 6669 6c65   txt or out file
+0000e4f0: 2066 6f75 6e64 2e0d 0a0d 0a23 2323 2068   found.....### h
+0000e500: 6973 746f 6772 616d 2e65 7865 2023 2323  istogram.exe ###
+0000e510: 0d0a 0d0a 5468 6973 206d 6f64 756c 6520  ....This module 
+0000e520: 7573 6573 2074 6865 2064 6174 6120 696e  uses the data in
+0000e530: 7369 6465 206f 6e20 7468 6520 6669 6c65  side on the file
+0000e540: 6e61 6d65 2074 6f20 7072 6f64 7563 6520  name to produce 
+0000e550: 6120 6869 7374 6f67 7261 6d20 696d 6167  a histogram imag
+0000e560: 652e 0d0a 0d0a 6060 600d 0a55 7361 6765  e.....```..Usage
+0000e570: 3a20 4869 7374 6f67 7261 6d2e 7079 205b  : Histogram.py [
+0000e580: 6f70 7469 6f6e 735d 204c 4f47 5f46 494c  options] LOG_FIL
+0000e590: 4520 5452 4143 450d 0a0d 0a4f 7074 696f  E TRACE....Optio
+0000e5a0: 6e73 3a0d 0a20 202d 2d76 6572 7369 6f6e  ns:..  --version
+0000e5b0: 2020 2020 2020 2020 2020 2020 2073 686f               sho
+0000e5c0: 7720 7072 6f67 7261 6d27 7320 7665 7273  w program's vers
+0000e5d0: 696f 6e20 6e75 6d62 6572 2061 6e64 2065  ion number and e
+0000e5e0: 7869 740d 0a20 202d 682c 202d 2d68 656c  xit..  -h, --hel
+0000e5f0: 7020 2020 2020 2020 2020 2020 2073 686f  p            sho
+0000e600: 7720 7468 6973 2068 656c 7020 6d65 7373  w this help mess
+0000e610: 6167 6520 616e 6420 6578 6974 0d0a 2020  age and exit..  
+0000e620: 2d73 2053 4947 4d41 2c20 2d2d 7369 676d  -s SIGMA, --sigm
+0000e630: 613d 5349 474d 410d 0a20 2020 2020 2020  a=SIGMA..       
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e650: 2053 6967 6d61 2074 6f20 6265 2075 7365   Sigma to be use
+0000e660: 6420 696e 2074 6865 2064 6973 7472 6962  d in the distrib
+0000e670: 7574 696f 6e20 6669 742e 2044 6566 6175  ution fit. Defau
+0000e680: 6c74 3d33 0d0a 2020 2d6e 204e 4249 4e53  lt=3..  -n NBINS
+0000e690: 2c20 2d2d 6e62 696e 733d 4e42 494e 530d  , --nbins=NBINS.
+0000e6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e6b0: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
+0000e6c0: 6f66 2062 696e 7320 746f 2062 6520 7573  of bins to be us
+0000e6d0: 6564 2069 6e20 7468 6520 6869 7374 6f67  ed in the histog
+0000e6e0: 7261 6d2e 2044 6566 6175 6c74 3d32 300d  ram. Default=20.
+0000e6f0: 0a20 202d 6320 4649 4c54 4552 532c 202d  .  -c FILTERS, -
+0000e700: 2d63 6f6e 6469 7469 6f6e 3d46 494c 5445  -condition=FILTE
+0000e710: 5253 0d0a 2020 2020 2020 2020 2020 2020  RS..            
+0000e720: 2020 2020 2020 2020 2020 2020 4669 6c74              Filt
+0000e730: 6572 2063 6f6e 6469 7469 6f6e 2077 7269  er condition wri
+0000e740: 7465 6e20 696e 2070 7974 686f 6e2e 204d  ten in python. M
+0000e750: 6f72 6520 7468 616e 206f 6e65 0d0a 2020  ore than one..  
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
+0000e780: 2063 616e 2062 6520 6164 6465 6420 6275   can be added bu
+0000e790: 7420 6561 6368 2065 7870 7265 7373 696f  t each expressio
+0000e7a0: 6e20 7368 6f75 6c64 2062 650d 0a20 2020  n should be..   
+0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7c0: 2020 2020 2070 7265 6365 6465 6420 6279       preceded by
+0000e7d0: 202d 632e 2045 5841 4d50 4c45 3a20 2d63   -c. EXAMPLE: -c
+0000e7e0: 2056 284e 3030 3129 3e34 202d 6320 7061   V(N001)>4 -c pa
+0000e7f0: 7261 6d65 7465 723d 3d31 0d0a 2020 2020  rameter==1..    
+0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e810: 2020 2020 2d63 2020 4928 5631 293c 302e      -c  I(V1)<0.
+0000e820: 350d 0a20 202d 6620 464f 524d 4154 2c20  5..  -f FORMAT, 
+0000e830: 2d2d 666f 726d 6174 3d46 4f52 4d41 540d  --format=FORMAT.
+0000e840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e850: 2020 2020 2020 2020 2046 6f72 6d61 7420           Format 
+0000e860: 7374 7269 6e67 2066 6f72 2074 6865 2058  string for the X
+0000e870: 2061 7869 732e 2045 7861 6d70 6c65 3a20   axis. Example: 
+0000e880: 2d66 2025 332e 3466 0d0a 2020 2d74 2054  -f %3.4f..  -t T
+0000e890: 4954 4c45 2c20 2d2d 7469 746c 653d 5449  ITLE, --title=TI
+0000e8a0: 544c 450d 0a20 2020 2020 2020 2020 2020  TLE..           
+0000e8b0: 2020 2020 2020 2020 2020 2020 2054 6974               Tit
+0000e8c0: 6c65 2074 6f20 6170 7065 6172 206f 6e20  le to appear on 
+0000e8d0: 7468 6520 746f 7020 6f66 2074 6865 2068  the top of the h
+0000e8e0: 6973 746f 6772 616d 2e0d 0a20 202d 7220  istogram...  -r 
+0000e8f0: 5241 4e47 452c 202d 2d72 616e 6765 3d52  RANGE, --range=R
+0000e900: 414e 4745 0d0a 2020 2020 2020 2020 2020  ANGE..          
+0000e910: 2020 2020 2020 2020 2020 2020 2020 5261                Ra
+0000e920: 6e67 6520 6f66 2074 6865 2058 2061 7869  nge of the X axi
+0000e930: 7320 746f 2075 7365 2066 6f72 2074 6865  s to use for the
+0000e940: 2068 6973 746f 6772 616d 2069 6e20 7468   histogram in th
+0000e950: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000e960: 2020 2020 2020 2020 2020 2066 6f72 6d20             form 
+0000e970: 6d69 6e3a 6d61 782e 2045 7861 6d70 6c65  min:max. Example
+0000e980: 3a20 2d72 202d 313a 310d 0a20 202d 432c  : -r -1:1..  -C,
+0000e990: 202d 2d63 6c69 7062 6f61 7264 2020 2020   --clipboard    
+0000e9a0: 2020 2049 6620 7468 6520 6461 7461 2066     If the data f
+0000e9b0: 726f 6d20 7468 6520 636c 6970 626f 6172  rom the clipboar
+0000e9c0: 6420 6973 2074 6f20 6265 2075 7365 642e  d is to be used.
+0000e9d0: 0d0a 2020 2d69 2049 4d41 4745 4649 4c45  ..  -i IMAGEFILE
+0000e9e0: 2c20 2d2d 696d 6167 653d 494d 4147 4546  , --image=IMAGEF
+0000e9f0: 494c 450d 0a20 2020 2020 2020 2020 2020  ILE..           
+0000ea00: 2020 2020 2020 2020 2020 2020 204e 616d               Nam
+0000ea10: 6520 6f66 2074 6865 2069 6d61 6765 2046  e of the image F
+0000ea20: 696c 652e 2065 7874 656e 7369 6f6e 2027  ile. extension '
+0000ea30: 706e 6727 2020 2020 0d0a 6060 600d 0a0d  png'    ..```...
+0000ea40: 0a23 2323 2072 6177 636f 6e76 6572 742e  .### rawconvert.
+0000ea50: 6578 6520 2323 230d 0a0d 0a41 2074 6f6f  exe ###....A too
+0000ea60: 6c20 746f 2063 6f6e 7665 7274 202e 7261  l to convert .ra
+0000ea70: 7720 6669 6c65 7320 696e 746f 2063 7376  w files into csv
+0000ea80: 206f 7220 4578 6365 6c20 6669 6c65 732e   or Excel files.
+0000ea90: 0d0a 0d0a 6060 600d 0a55 7361 6765 3a20  ....```..Usage: 
+0000eaa0: 7261 775f 636f 6e76 6572 742e 6578 6520  raw_convert.exe 
+0000eab0: 5b6f 7074 696f 6e73 5d20 3c72 6177 6669  [options] <rawfi
+0000eac0: 6c65 3e20 3c74 7261 6365 5f6c 6973 743e  le> <trace_list>
+0000ead0: 0d0a 0d0a 4f70 7469 6f6e 733a 0d0a 2020  ....Options:..  
+0000eae0: 2d2d 7665 7273 696f 6e20 2020 2020 2020  --version       
+0000eaf0: 2020 2020 2020 7368 6f77 2070 726f 6772        show progr
+0000eb00: 616d 2773 2076 6572 7369 6f6e 206e 756d  am's version num
+0000eb10: 6265 7220 616e 6420 6578 6974 0d0a 2020  ber and exit..  
+0000eb20: 2d68 2c20 2d2d 6865 6c70 2020 2020 2020  -h, --help      
+0000eb30: 2020 2020 2020 7368 6f77 2074 6869 7320        show this 
+0000eb40: 6865 6c70 206d 6573 7361 6765 2061 6e64  help message and
+0000eb50: 2065 7869 740d 0a20 202d 6f20 4649 4c45   exit..  -o FILE
+0000eb60: 2c20 2d2d 6f75 7470 7574 3d46 494c 450d  , --output=FILE.
+0000eb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb80: 2020 2020 2020 2020 204f 7574 7075 7420           Output 
+0000eb90: 6669 6c65 206e 616d 652e 2055 7365 202e  file name. Use .
+0000eba0: 6373 7620 666f 7220 4353 5620 6f75 7470  csv for CSV outp
+0000ebb0: 7574 2c20 2e78 6c73 7820 666f 720d 0a20  ut, .xlsx for.. 
+0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebd0: 2020 2020 2020 2045 7863 656c 206f 7574         Excel out
+0000ebe0: 7075 740d 0a20 202d 632c 202d 2d63 6c69  put..  -c, --cli
+0000ebf0: 7062 6f61 7264 2020 2020 2020 204f 7574  pboard       Out
+0000ec00: 7075 7420 746f 2063 6c69 7062 6f61 7264  put to clipboard
+0000ec10: 0d0a 2020 2d76 2c20 2d2d 7665 7262 6f73  ..  -v, --verbos
+0000ec20: 6520 2020 2020 2020 2020 5665 7262 6f73  e         Verbos
+0000ec30: 6520 6f75 7470 7574 0d0a 2020 2d73 2053  e output..  -s S
+0000ec40: 4550 4152 4154 4f52 2c20 2d2d 7365 703d  EPARATOR, --sep=
+0000ec50: 5345 5041 5241 544f 520d 0a20 2020 2020  SEPARATOR..     
+0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec70: 2020 2056 616c 7565 2073 6570 6172 6174     Value separat
+0000ec80: 6f72 2066 6f72 2043 5356 206f 7574 7075  or for CSV outpu
+0000ec90: 742e 2044 6566 6175 6c74 3a20 225c 7422  t. Default: "\t"
+0000eca0: 203c 5441 423e 0d0a 2020 2020 2020 2020   <TAB>..        
+0000ecb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecc0: 4578 616d 706c 653a 202d 6420 223b 220d  Example: -d ";".
+0000ecd0: 0a60 6060 0d0a 0d0a 2323 2320 7275 6e5f  .```....### run_
+0000ece0: 7365 7276 6572 2e65 7865 2023 2323 0d0a  server.exe ###..
+0000ecf0: 0d0a 5468 6973 2063 6f6d 6d61 6e64 206c  ..This command l
+0000ed00: 696e 6520 746f 6f6c 2077 6173 206d 6f76  ine tool was mov
+0000ed10: 6564 2074 6f20 7468 6520 7370 6963 656c  ed to the spicel
+0000ed20: 6962 2070 6163 6b61 6765 2e0d 0a0d 0a23  ib package.....#
+0000ed30: 2323 2053 656d 6944 6576 4f70 5265 6164  ## SemiDevOpRead
+0000ed40: 6572 2e70 7920 2323 230d 0a0d 0a54 6869  er.py ###....Thi
+0000ed50: 7320 6d6f 6475 6c65 2069 7320 7573 6564  s module is used
+0000ed60: 2074 6f20 7265 6164 2066 726f 6d20 4c54   to read from LT
+0000ed70: 5370 6963 6520 6c6f 6720 6669 6c65 7320  Spice log files 
+0000ed80: 5365 6d69 636f 6e64 7563 746f 7220 4465  Semiconductor De
+0000ed90: 7669 6365 7320 4f70 6572 6174 696e 6720  vices Operating 
+0000eda0: 506f 696e 7420 496e 666f 726d 6174 696f  Point Informatio
+0000edb0: 6e2e 2041 206d 6f72 6520 6465 7461 696c  n. A more detail
+0000edc0: 6564 0d0a 646f 6375 6d65 6e74 6174 696f  ed..documentatio
+0000edd0: 6e20 6973 2064 6972 6563 746c 7920 696e  n is directly in
+0000ede0: 636c 7564 6564 2069 6e20 7468 6520 736f  cluded in the so
+0000edf0: 7572 6365 2066 696c 6520 646f 6373 7472  urce file docstr
+0000ee00: 696e 6773 2e0d 0a0d 0a23 2320 4465 6275  ings.....## Debu
+0000ee10: 6720 4c6f 6767 696e 670d 0a0d 0a54 6865  g Logging....The
+0000ee20: 206c 6962 7261 7279 2075 7365 7320 7468   library uses th
+0000ee30: 6520 7374 616e 6461 7264 2060 6c6f 6767  e standard `logg
+0000ee40: 696e 6760 206d 6f64 756c 652e 2054 6872  ing` module. Thr
+0000ee50: 6565 2063 6f6e 7665 6e69 656e 6365 2066  ee convenience f
+0000ee60: 756e 6374 696f 6e73 2068 6176 6520 6265  unctions have be
+0000ee70: 656e 2061 6464 6564 2066 6f72 2065 6173  en added for eas
+0000ee80: 696c 7920 6368 616e 6769 6e67 206c 6f67  ily changing log
+0000ee90: 6769 6e67 0d0a 7365 7474 696e 6773 2061  ging..settings a
+0000eea0: 6372 6f73 7320 7468 6520 656e 7469 7265  cross the entire
+0000eeb0: 206c 6962 7261 7279 2e20 6050 794c 5453   library. `PyLTS
+0000eec0: 7069 6365 2e61 6c6c 5f6c 6f67 6765 7273  pice.all_loggers
+0000eed0: 2829 6020 7265 7475 726e 7320 6120 6c69  ()` returns a li
+0000eee0: 7374 206f 6620 616c 6c20 7468 6520 6c6f  st of all the lo
+0000eef0: 6767 6572 2773 0d0a 6e61 6d65 732c 2060  gger's..names, `
+0000ef00: 5079 4c54 5370 6963 652e 7365 745f 6c6f  PyLTSpice.set_lo
+0000ef10: 675f 6c65 7665 6c28 6c6f 6767 696e 672e  g_level(logging.
+0000ef20: 4445 4255 4729 600d 0a77 6f75 6c64 2073  DEBUG)`..would s
+0000ef30: 6574 2074 6865 206c 6962 7261 7279 2773  et the library's
+0000ef40: 206c 6f67 6769 6e67 206c 6576 656c 2074   logging level t
+0000ef50: 6f20 6465 6275 672c 2061 6e64 2060 5079  o debug, and `Py
+0000ef60: 4c54 5370 6963 652e 6164 645f 6c6f 675f  LTSpice.add_log_
+0000ef70: 6861 6e64 6c65 7228 6d79 5f68 616e 646c  handler(my_handl
+0000ef80: 6572 2960 2077 6f75 6c64 2061 6464 2060  er)` would add `
+0000ef90: 6d79 5f68 616e 646c 6572 6020 6173 2061  my_handler` as a
+0000efa0: 0d0a 6861 6e64 6c65 7220 666f 720d 0a61  ..handler for..a
+0000efb0: 6c6c 206c 6f67 6765 7273 2e0d 0a0d 0a23  ll loggers.....#
+0000efc0: 2323 2053 696e 676c 6520 4d6f 6475 6c65  ## Single Module
+0000efd0: 204c 6f67 6769 6e67 0d0a 0d0a 4974 2069   Logging....It i
+0000efe0: 7320 616c 736f 2070 6f73 7369 626c 6520  s also possible 
+0000eff0: 746f 2073 6574 2074 6865 206c 6f67 6769  to set the loggi
+0000f000: 6e67 2073 6574 7469 6e67 7320 666f 7220  ng settings for 
+0000f010: 6120 7369 6e67 6c65 206d 6f64 756c 6520  a single module 
+0000f020: 6279 2075 7369 6e67 2069 7473 206e 616d  by using its nam
+0000f030: 6520 6163 7175 6972 6564 2066 726f 6d0d  e acquired from.
+0000f040: 0a74 6865 2060 5079 4c54 5370 6963 652e  .the `PyLTSpice.
+0000f050: 616c 6c5f 6c6f 6767 6572 7328 2960 0d0a  all_loggers()`..
+0000f060: 6675 6e63 7469 6f6e 2e20 466f 7220 6578  function. For ex
+0000f070: 616d 706c 653a 0d0a 0d0a 6060 6070 7974  ample:....```pyt
+0000f080: 686f 6e0d 0a69 6d70 6f72 7420 6c6f 6767  hon..import logg
+0000f090: 696e 670d 0a0d 0a6c 6f67 6769 6e67 2e62  ing....logging.b
+0000f0a0: 6173 6963 436f 6e66 6967 286c 6576 656c  asicConfig(level
+0000f0b0: 3d6c 6f67 6769 6e67 2e49 4e46 4f29 2020  =logging.INFO)  
+0000f0c0: 2320 5365 7420 7570 2074 6865 2072 6f6f  # Set up the roo
+0000f0d0: 7420 6c6f 6767 6572 2066 6972 7374 0d0a  t logger first..
+0000f0e0: 0d0a 696d 706f 7274 2050 794c 5453 7069  ..import PyLTSpi
+0000f0f0: 6365 2020 2320 496d 706f 7274 2050 794c  ce  # Import PyL
+0000f100: 5453 7069 6365 2074 6f20 7365 7420 7468  TSpice to set th
+0000f110: 6520 6c6f 6767 696e 6720 6c65 7665 6c73  e logging levels
+0000f120: 0d0a 0d0a 5079 4c54 5370 6963 652e 7365  ....PyLTSpice.se
+0000f130: 745f 6c6f 675f 6c65 7665 6c28 6c6f 6767  t_log_level(logg
+0000f140: 696e 672e 4445 4255 4729 2020 2320 5365  ing.DEBUG)  # Se
+0000f150: 7420 5079 4c54 5370 6963 6527 7320 676c  t PyLTSpice's gl
+0000f160: 6f62 616c 206c 6f67 206c 6576 656c 0d0a  obal log level..
+0000f170: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
+0000f180: 7228 2250 794c 5453 7069 6365 2e52 6177  r("PyLTSpice.Raw
+0000f190: 5265 6164 2229 2e6c 6576 656c 203d 206c  Read").level = l
+0000f1a0: 6f67 6769 6e67 2e57 4152 4e49 4e47 2020  ogging.WARNING  
+0000f1b0: 2320 5365 7420 7468 6520 6c6f 6720 6c65  # Set the log le
+0000f1c0: 7665 6c20 666f 7220 6f6e 6c79 2052 6177  vel for only Raw
+0000f1d0: 5265 6164 2074 6f20 7761 726e 696e 670d  Read to warning.
+0000f1e0: 0a60 6060 0d0a 0d0a 576f 756c 6420 7365  .```....Would se
+0000f1f0: 7420 6f6e 6c79 2060 5079 4c54 5370 6963  t only `PyLTSpic
+0000f200: 652e 5261 7752 6561 6460 2066 696c 6527  e.RawRead` file'
+0000f210: 7320 6c6f 6767 696e 6720 6c65 7665 6c20  s logging level 
+0000f220: 746f 2077 6172 6e69 6e67 2077 6869 6c65  to warning while
+0000f230: 2074 6865 206f 7468 6572 206d 6f64 756c   the other modul
+0000f240: 6573 2077 6f75 6c64 2072 656d 6169 6e20  es would remain 
+0000f250: 6174 2064 6562 7567 206c 6576 656c 2e0d  at debug level..
+0000f260: 0a5f 4d61 6b65 2073 7572 6520 746f 2069  ._Make sure to i
+0000f270: 6e69 7469 616c 697a 6520 7468 6520 726f  nitialize the ro
+0000f280: 6f74 206c 6f67 6765 7220 6265 666f 7265  ot logger before
+0000f290: 2069 6d70 6f72 7469 6e67 2074 6865 206c   importing the l
+0000f2a0: 6962 7261 7279 2074 6f20 6265 2061 626c  ibrary to be abl
+0000f2b0: 6520 746f 2073 6565 2074 6865 206c 6f67  e to see the log
+0000f2c0: 732e 5f0d 0a0d 0a23 2320 546f 2077 686f  s._....## To who
+0000f2d0: 6d20 646f 2049 2074 616c 6b20 746f 3f20  m do I talk to? 
+0000f2e0: 2323 0d0a 0d0a 2a20 546f 6f6c 7320 7765  ##....* Tools we
+0000f2f0: 6273 6974 6520 3a20 5b68 7474 7073 3a2f  bsite : [https:/
+0000f300: 2f77 7777 2e6e 756e 6f62 7275 6d2e 636f  /www.nunobrum.co
+0000f310: 6d2f 7079 6c74 7370 6963 652e 6874 6d6c  m/pyltspice.html
+0000f320: 5d28 6874 7470 733a 2f2f 7777 772e 6e75  ](https://www.nu
+0000f330: 6e6f 6272 756d 2e63 6f6d 2f70 796c 7473  nobrum.com/pylts
+0000f340: 7069 6365 2e68 746d 6c29 0d0a 2a20 5265  pice.html)..* Re
+0000f350: 706f 206f 776e 6572 203a 205b 6d65 406e  po owner : [me@n
+0000f360: 756e 6f62 7275 6d2e 636f 6d5d 286d 6169  unobrum.com](mai
+0000f370: 6c74 6f3a 6d65 406e 756e 6f62 7275 6d2e  lto:me@nunobrum.
+0000f380: 636f 6d29 0d0a 2a20 416c 7465 726e 6174  com)..* Alternat
+0000f390: 6976 6520 636f 6e74 6163 7420 3a20 5b6e  ive contact : [n
+0000f3a0: 756e 6f2e 6272 756d 4067 6d61 696c 2e63  uno.brum@gmail.c
+0000f3b0: 6f6d 5d28 6d61 696c 746f 3a6e 756e 6f2e  om](mailto:nuno.
+0000f3c0: 6272 756d 4067 6d61 696c 2e63 6f6d 290d  brum@gmail.com).
+0000f3d0: 0a0d 0a23 2320 4869 7374 6f72 7920 2323  ...## History ##
+0000f3e0: 0d0a 2a20 5665 7273 696f 6e20 352e 332e  ..* Version 5.3.
+0000f3f0: 310d 0a20 202a 2042 7567 6669 7865 7320  1..  * Bugfixes 
+0000f400: 0d0a 2020 2020 2a20 5570 6461 7465 7320  ..    * Updates 
+0000f410: 6f6e 2074 6865 2052 4541 444d 452e 6d64  on the README.md
+0000f420: 2066 696c 652e 2049 7373 7565 2023 3133   file. Issue #13
+0000f430: 370d 0a20 2020 202a 2048 6965 7261 7263  7..    * Hierarc
+0000f440: 6869 6361 6c20 7375 7070 6f72 7420 6f6e  hical support on
+0000f450: 2041 7363 4564 6974 6f72 2e20 4973 7375   AscEditor. Issu
+0000f460: 6520 2331 3338 0d0a 2020 2a20 5269 6368  e #138..  * Rich
+0000f470: 2066 6f72 6d61 7420 6973 206f 6e6c 7920   format is only 
+0000f480: 7573 6564 2069 6620 7468 6520 7573 6572  used if the user
+0000f490: 2068 6173 2069 7420 616c 7265 6164 7920   has it already 
+0000f4a0: 696e 7374 616c 6c65 642e 2049 7373 7565  installed. Issue
+0000f4b0: 2023 3133 360d 0a2a 2056 6572 7369 6f6e   #136..* Version
+0000f4c0: 2035 2e33 2e30 0d0a 2020 2a20 4869 6572   5.3.0..  * Hier
+0000f4d0: 6172 6368 6963 616c 2053 7570 706f 7274  archical Support
+0000f4e0: 2028 416c 6967 6e69 6e67 2077 6974 6820   (Aligning with 
+0000f4f0: 7468 6520 7370 6963 656c 6962 2031 2e31  the spicelib 1.1
+0000f500: 2e31 290d 0a2a 2056 6572 7369 6f6e 2035  .1)..* Version 5
+0000f510: 2e32 2e33 0d0a 2020 2a20 5570 6461 7469  .2.3..  * Updati
+0000f520: 6e67 206c 6f67 6765 7273 2074 6f20 7573  ng loggers to us
+0000f530: 6520 7468 6520 2273 7069 6365 6c69 6222  e the "spicelib"
+0000f540: 2049 4473 2e0d 0a20 202a 2046 6978 696e   IDs...  * Fixin
+0000f550: 6720 6175 746f 646f 6320 6572 726f 7273  g autodoc errors
+0000f560: 0d0a 2020 2a20 436f 7272 6563 7469 6e67  ..  * Correcting
+0000f570: 2056 6572 7369 6f6e 2072 6566 6572 656e   Version referen
+0000f580: 6365 730d 0a0d 0a2a 2056 6572 7369 6f6e  ces....* Version
+0000f590: 2035 2e32 2e32 0d0a 2020 2a20 4669 7865   5.2.2..  * Fixe
+0000f5a0: 7320 6f6e 2074 6865 2075 6e69 7474 6573  s on the unittes
+0000f5b0: 7473 2061 6674 6572 2074 6865 2073 7069  ts after the spi
+0000f5c0: 6365 6c69 6220 7570 6461 7465 2074 6f20  celib update to 
+0000f5d0: 312e 302e 340d 0a0d 0a2a 2056 6572 7369  1.0.4....* Versi
+0000f5e0: 6f6e 2035 2e32 2e31 0d0a 2020 2a20 436f  on 5.2.1..  * Co
+0000f5f0: 7272 6563 7469 6f6e 206f 6e20 7468 6520  rrection on the 
+0000f600: 7275 6e5f 6d6f 6e74 6563 6172 6c6f 2e70  run_montecarlo.p
+0000f610: 7920 616e 6420 7275 6e5f 776f 7273 745f  y and run_worst_
+0000f620: 6361 7365 2e70 7920 6578 616d 706c 6573  case.py examples
+0000f630: 2e0d 0a20 202a 2046 6978 6573 206f 6e20  ...  * Fixes on 
+0000f640: 7468 6520 7370 6963 656c 6962 2028 5665  the spicelib (Ve
+0000f650: 7273 696f 6e20 312e 302e 3329 0d0a 0d0a  rsion 1.0.3)....
+0000f660: 2a20 5665 7273 696f 6e20 352e 320d 0a20  * Version 5.2.. 
+0000f670: 202a 2053 696d 416e 616c 7973 6973 2073   * SimAnalysis s
+0000f680: 7570 706f 7274 696e 6720 626f 7468 2051  upporting both Q
+0000f690: 7370 6963 6520 616e 6420 4c54 5370 6963  spice and LTSpic
+0000f6a0: 6520 6c6f 6766 696c 6573 2e0d 0a20 202a  e logfiles...  *
+0000f6b0: 2046 6173 7457 6f72 7374 4361 7365 416e   FastWorstCaseAn
+0000f6c0: 616c 7973 6973 2061 6c67 6f72 6974 686d  alysis algorithm
+0000f6d0: 2069 6d70 6c65 6d65 6e74 6564 0d0a 2020   implemented..  
+0000f6e0: 2a20 4669 7820 6f6e 2074 6865 206c 6f67  * Fix on the log
+0000f6f0: 2072 6561 6469 6e67 206f 6620 666f 7572   reading of four
+0000f700: 6965 7220 6461 7461 2e0d 0a0d 0a2a 2056  ier data.....* V
+0000f710: 6572 7369 6f6e 2035 2e31 0d0a 2020 2a20  ersion 5.1..  * 
+0000f720: 496d 706f 7274 616e 7420 4275 6766 6978  Important Bugfix
+0000f730: 206f 6e20 7468 6520 4c54 436f 6d70 6c65   on the LTComple
+0000f740: 7820 636c 6173 732e 0d0a 2020 2a20 4669  x class...  * Fi
+0000f750: 7865 7320 616e 6420 656e 6861 6e63 696e  xes and enhancin
+0000f760: 6720 7468 6520 616e 616c 7973 6973 2074  g the analysis t
+0000f770: 6f6f 6c6b 6974 2e0d 0a20 202a 2044 6570  oolkit...  * Dep
+0000f780: 7265 6361 7469 6e67 2053 7069 6365 4564  recating SpiceEd
+0000f790: 6974 6f72 2e77 7269 7465 5f6e 6574 6c69  itor.write_netli
+0000f7a0: 7374 2069 6e20 6661 766f 7572 206f 6620  st in favour of 
+0000f7b0: 7361 7665 5f6e 6574 6c69 7374 2829 0d0a  save_netlist()..
+0000f7c0: 0d0a 2a20 5665 7273 696f 6e20 352e 300d  ..* Version 5.0.
+0000f7d0: 0a20 202a 204d 616b 696e 6720 7468 6973  .  * Making this
+0000f7e0: 206c 6962 7261 7279 2064 6570 656e 6465   library depende
+0000f7f0: 6e74 206f 6e20 7370 6963 656c 6962 2077  nt on spicelib w
+0000f800: 6869 6c65 2074 7279 696e 6720 746f 206d  hile trying to m
+0000f810: 6169 6e74 6169 6e20 6261 636b 7761 7264  aintain backward
+0000f820: 2063 6f6d 7061 7469 6269 6c69 7479 2061   compatibility a
+0000f830: 7320 6d75 6368 2061 7320 706f 7373 6962  s much as possib
+0000f840: 6c65 2e20 0d0a 2020 5079 4c54 7370 6963  le. ..  PyLTspic
+0000f850: 6520 7769 6c6c 2062 6520 6b65 7074 2061  e will be kept a
+0000f860: 6c69 7665 2061 6e64 2069 7473 2075 7064  live and its upd
+0000f870: 6174 6520 7769 6c6c 2062 6520 6c69 6e6b  ate will be link
+0000f880: 6564 2074 6f20 7468 6520 7370 6963 656c  ed to the spicel
+0000f890: 6962 2e20 5468 6520 6d61 696e 2064 6966  ib. The main dif
+0000f8a0: 6665 7265 6e63 6520 6973 2074 6861 7420  ference is that 
+0000f8b0: 7573 696e 670d 0a20 2050 794c 5473 7069  using..  PyLTspi
+0000f8c0: 6365 2077 696c 6c20 6176 6572 7420 7468  ce will avert th
+0000f8d0: 6520 6e65 6564 206f 6620 6861 7669 6e67  e need of having
+0000f8e0: 2074 6f20 7365 6c65 6374 2061 2073 696d   to select a sim
+0000f8f0: 756c 6174 6f72 2069 6e20 616c 6c20 7275  ulator in all ru
+0000f900: 6e20 636f 6d6d 616e 6473 2e0d 0a0d 0a2a  n commands.....*
+0000f910: 2056 6572 7369 6f6e 2034 2e31 2e32 0d0a   Version 4.1.2..
+0000f920: 2020 2a20 4164 6469 6e67 2073 7570 706f    * Adding suppo
+0000f930: 7274 2066 6f72 2074 6865 206e 6577 2051  rt for the new Q
+0000f940: 5350 4943 4520 7369 6d75 6c61 746f 720d  SPICE simulator.
+0000f950: 0a20 202a 2049 6d70 726f 7669 6e67 2074  .  * Improving t
+0000f960: 6865 2074 696d 656f 7574 206d 6563 6861  he timeout mecha
+0000f970: 6e69 736d 206f 6e20 7468 6520 5369 6d52  nism on the SimR
+0000f980: 756e 6e65 7220 636c 6173 730d 0a20 202a  unner class..  *
+0000f990: 204d 696e 6f72 2062 7567 2066 6978 6573   Minor bug fixes
+0000f9a0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
+0000f9b0: 312e 310d 0a20 202a 2043 6f6d 706c 6574  1.1..  * Complet
+0000f9c0: 696e 6720 7468 6520 576f 7273 742d 4361  ing the Worst-Ca
+0000f9d0: 7365 2041 6e61 6c79 7369 7320 6675 6e63  se Analysis func
+0000f9e0: 7469 6f6e 732e 2041 6464 696e 6720 6120  tions. Adding a 
+0000f9f0: 6465 6469 6361 7465 6420 6578 616d 706c  dedicated exampl
+0000fa00: 6520 666f 7220 6974 2e0d 0a20 202a 2052  e for it...  * R
+0000fa10: 6566 6163 746f 7269 6e67 2074 6865 204c  efactoring the L
+0000fa20: 5453 7069 6365 4c6f 6752 6561 6465 7220  TSpiceLogReader 
+0000fa30: 636c 6173 7320 696e 206f 7264 6572 2074  class in order t
+0000fa40: 6f20 7573 6520 6974 206f 6e20 7468 6520  o use it on the 
+0000fa50: 416e 616c 7973 6973 2074 6f6f 6c6b 6974  Analysis toolkit
+0000fa60: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
+0000fa70: 312e 3020 2a28 7265 7175 6972 6573 2050  1.0 *(requires P
+0000fa80: 7974 686f 6e20 332e 3820 6f72 2068 6967  ython 3.8 or hig
+0000fa90: 6865 7229 2a0d 0a20 2020 202a 2041 6464  her)*..    * Add
+0000faa0: 696e 6720 6120 6e65 7720 636c 6173 7320  ing a new class 
+0000fab0: 746f 206d 616e 6970 756c 6174 6520 6469  to manipulate di
+0000fac0: 7265 6374 6c79 2074 6865 202e 6173 6320  rectly the .asc 
+0000fad0: 6669 6c65 732e 0d0a 2020 2020 2a20 4d6f  files...    * Mo
+0000fae0: 6469 6679 696e 6720 616c 6c20 7468 6520  difying all the 
+0000faf0: 6f74 6865 7220 636c 6173 7365 7320 696e  other classes in
+0000fb00: 206f 7264 6572 2074 6f20 7573 6520 7468   order to use th
+0000fb10: 6520 6e65 7720 636c 6173 732e 0d0a 2020  e new class...  
+0000fb20: 2020 2a20 4164 6469 6e67 2063 6c61 7373    * Adding class
+0000fb30: 6573 2074 6f20 7065 7266 6f72 6d20 4d6f  es to perform Mo
+0000fb40: 6e74 6563 6172 6c6f 2061 6e64 2077 6f72  ntecarlo and wor
+0000fb50: 7374 2063 6173 6520 616e 616c 7973 6973  st case analysis
+0000fb60: 2028 5468 616e 6b73 2074 6f20 406d 7661   (Thanks to @mva
+0000fb70: 6e72 6965 7420 666f 7220 6869 7320 7374  nriet for his st
+0000fb80: 6172 7469 6e67 2074 6869 7329 2e0d 0a20  arting this)... 
+0000fb90: 2020 202a 2052 656d 6f76 696e 6720 7468     * Removing th
+0000fba0: 6520 6465 7072 6563 6174 6564 204c 5453  e deprecated LTS
+0000fbb0: 7069 6365 5f52 6177 5265 6164 2e70 792c  pice_RawRead.py,
+0000fbc0: 204c 5453 7069 6365 5f52 6177 5772 6974   LTSpice_RawWrit
+0000fbd0: 652e 7079 2061 6e64 204c 5453 7069 6365  e.py and LTSpice
+0000fbe0: 4261 7463 682e 7079 2066 696c 6573 2061  Batch.py files a
+0000fbf0: 6e64 2072 6573 7065 6374 6976 6520 636c  nd respective cl
+0000fc00: 6173 7365 732e 0d0a 2020 2020 2a20 5265  asses...    * Re
+0000fc10: 7374 7275 6374 7572 6564 2074 6865 2066  structured the f
+0000fc20: 6f6c 6465 7220 7374 7275 6374 7572 6520  older structure 
+0000fc30: 746f 2062 6520 6d6f 7265 2069 6e20 6c69  to be more in li
+0000fc40: 6e65 2077 6974 6820 7468 6520 5079 7468  ne with the Pyth
+0000fc50: 6f6e 2073 7461 6e64 6172 6473 2e0d 0a20  on standards... 
+0000fc60: 2020 202a 2041 6464 6564 2061 6e20 4578     * Added an Ex
+0000fc70: 616d 706c 6573 2066 6f6c 6465 7220 7769  amples folder wi
+0000fc80: 7468 2073 6f6d 6520 6578 616d 706c 6573  th some examples
+0000fc90: 206f 6e20 686f 7720 746f 2075 7365 2074   on how to use t
+0000fca0: 6865 206c 6962 7261 7279 2e0d 0a0d 0a2a  he library.....*
+0000fcb0: 2056 6572 7369 6f6e 2034 2e30 2e36 0d0a   Version 4.0.6..
+0000fcc0: 2020 2020 2a20 4669 7869 6e67 2069 7373      * Fixing iss
+0000fcd0: 7565 2077 6974 6820 7468 6520 7772 6974  ue with the writ
+0000fce0: 655f 6e65 746c 6973 7428 2920 6675 6e63  e_netlist() func
+0000fcf0: 7469 6f6e 2077 6865 6e20 7265 6365 6976  tion when receiv
+0000fd00: 696e 6720 6120 7374 7269 6e67 2069 6e73  ing a string ins
+0000fd10: 7465 6164 206f 6620 6120 7061 7468 6c69  tead of a pathli
+0000fd20: 622e 5061 7468 206f 626a 6563 742e 0d0a  b.Path object...
+0000fd30: 2020 2020 2a20 4368 616e 6769 6e67 2074      * Changing t
+0000fd40: 6865 2072 6567 756c 6172 2065 7870 7265  he regular expre
+0000fd50: 7373 696f 6e20 666f 7220 7468 6520 7265  ssion for the re
+0000fd60: 7369 7374 6f72 2069 6e20 6f72 6465 7220  sistor in order 
+0000fd70: 746f 2061 6363 6570 7420 7468 6520 523d  to accept the R=
+0000fd80: 2070 7265 6669 7820 6f6e 2074 6865 2076   prefix on the v
+0000fd90: 616c 7565 732e 0d0a 0d0a 2a20 5665 7273  alues.....* Vers
+0000fda0: 696f 6e20 342e 302e 350d 0a20 2020 202a  ion 4.0.5..    *
+0000fdb0: 2041 6363 6570 7469 6e67 2066 6978 6573   Accepting fixes
+0000fdc0: 2066 726f 6d20 6161 6e61 732d 7361 7965   from aanas-saye
+0000fdd0: 6440 4769 7448 7562 2074 6861 7420 6669  d@GitHub that fi
+0000fde0: 7865 7320 6973 7375 6573 2077 6974 6820  xes issues with 
+0000fdf0: 7275 6e6e 696e 6720 7468 6520 4c54 5370  running the LTSp
+0000fe00: 6963 6520 696e 204c 696e 7578 2e0d 0a0d  ice in Linux....
+0000fe10: 0a2a 2056 6572 7369 6f6e 2034 2e30 2e34  .* Version 4.0.4
+0000fe20: 0d0a 2020 2020 2a20 496d 7072 6f76 6564  ..    * Improved
+0000fe30: 2075 7361 6765 206f 6620 7468 6520 6c6f   usage of the lo
+0000fe40: 6767 696e 6720 6c69 6272 6172 792e 2028  gging library. (
+0000fe50: 5468 616e 6b73 2040 5453 7072 6563 6820  Thanks @TSprech 
+0000fe60: 666f 7220 7661 7374 6c79 2069 6d70 726f  for vastly impro
+0000fe70: 7669 6e67 2074 6865 206c 6f67 6769 6e67  ving the logging
+0000fe80: 290d 0a20 2020 202a 2049 6e63 6c75 6465  )..    * Include
+0000fe90: 6420 5275 6e54 6173 6b20 6e75 6d62 6572  d RunTask number
+0000fea0: 2069 6e20 7468 6520 6c6f 6720 6d65 7373   in the log mess
+0000feb0: 6167 6573 2e0d 0a20 2020 202a 2049 6e63  ages...    * Inc
+0000fec0: 6c75 6465 6420 6d69 6c6c 6973 6563 6f6e  luded millisecon
+0000fed0: 6473 2069 6e20 7468 6520 7469 6d65 2065  ds in the time e
+0000fee0: 6c61 7073 6564 2063 616c 6375 6c61 7469  lapsed calculati
+0000fef0: 6f6e 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  on.....* Version
+0000ff00: 2034 2e30 2e33 0d0a 2020 2020 2a20 4669   4.0.3..    * Fi
+0000ff10: 7869 6e67 2069 7373 7565 2069 6e20 656c  xing issue in el
+0000ff20: 6170 7365 6420 7469 6d65 2063 616c 6375  apsed time calcu
+0000ff30: 6c61 7469 6f6e 2e0d 0a20 2020 202a 2046  lation...    * F
+0000ff40: 6978 696e 6720 6973 7375 6520 7769 7468  ixing issue with
+0000ff50: 2074 6865 2069 6d70 6f72 7420 6f66 204c   the import of L
+0000ff60: 5453 7069 6365 4c6f 6752 6561 6465 7220  TSpiceLogReader 
+0000ff70: 6672 6f6d 204c 5453 7465 7073 2e70 790d  from LTSteps.py.
+0000ff80: 0a0d 0a2a 2056 6572 7369 6f6e 2034 2e30  ...* Version 4.0
+0000ff90: 2e32 0d0a 2020 2020 2a20 4368 616e 6769  .2..    * Changi
+0000ffa0: 6e67 206c 6973 7420 6f66 204c 6962 7261  ng list of Libra
+0000ffb0: 7279 2064 6570 656e 6465 6e63 6965 732e  ry dependencies.
+0000ffc0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
+0000ffd0: 302e 310d 0a20 2020 202a 2042 7567 2066  0.1..    * Bug f
+0000ffe0: 6978 206f 6e20 434c 4920 666f 7220 7468  ix on CLI for th
+0000fff0: 6520 4869 7374 6f67 7261 6d2e 7079 2061  e Histogram.py a
+00010000: 6e64 204c 5453 7465 7073 2e70 790d 0a0d  nd LTSteps.py...
+00010010: 0a2a 2056 6572 7369 6f6e 2034 2e30 2e30  .* Version 4.0.0
+00010020: 0d0a 2020 2020 2a20 5365 7061 7261 7469  ..    * Separati
+00010030: 6e67 2074 6865 2053 696d 436f 6d6d 616e  ng the SimComman
+00010040: 6465 7220 696e 746f 2074 776f 2073 6570  der into two sep
+00010050: 6172 6174 6520 636c 6173 7365 732c 206f  arate classes, o
+00010060: 6e65 2066 6f72 2074 6865 2073 7069 6365  ne for the spice
+00010070: 206e 6574 6c69 7374 2065 6469 7469 6e67   netlist editing
+00010080: 2028 5370 6963 6545 6469 746f 7229 2061   (SpiceEditor) a
+00010090: 6e64 2061 6e6f 7468 6572 0d0a 2020 2020  nd another..    
+000100a0: 2020 666f 7220 7468 6520 7369 6d75 6c61    for the simula
+000100b0: 7469 6f6e 2065 7865 6375 7469 6f6e 2028  tion execution (
+000100c0: 5369 6d52 756e 6e65 7229 2e0d 0a20 2020  SimRunner)...   
+000100d0: 202a 2049 6d70 6c65 6d65 6e74 696e 6720   * Implementing 
+000100e0: 7369 6d75 6c61 7469 6f6e 2073 6572 7665  simulation serve
+000100f0: 7220 746f 2061 6c6c 6f77 2066 6f72 2072  r to allow for r
+00010100: 656d 6f74 6520 7369 6d75 6c61 7469 6f6e  emote simulation
+00010110: 2065 7865 6375 7469 6f6e 2061 6e64 2074   execution and t
+00010120: 6865 2072 6573 7065 6374 6976 6520 636c  he respective cl
+00010130: 6965 6e74 2e0d 0a20 2020 202a 2053 7570  ient...    * Sup
+00010140: 706f 7274 696e 6720 5769 6767 6c65 7220  porting Wiggler 
+00010150: 656c 656d 656e 7420 696e 2074 6865 206e  element in the n
+00010160: 6577 204c 5453 7069 6365 5856 4949 2e0d  ew LTSpiceXVII..
+00010170: 0a20 2020 202a 2052 656e 616d 696e 6720  .    * Renaming 
+00010180: 616c 6c20 6669 6c65 7320 696e 746f 206c  all files into l
+00010190: 6f77 6572 6361 7365 2e0d 0a20 2020 202a  owercase...    *
+000101a0: 2043 7265 6174 696e 6720 4572 726f 7220   Creating Error 
+000101b0: 636c 6173 7365 7320 666f 7220 6265 7474  classes for bett
+000101c0: 6572 2065 7272 6f72 2068 616e 646c 696e  er error handlin
+000101d0: 672e 0d0a 2020 2020 2a20 4164 6469 6e67  g...    * Adding
+000101e0: 2073 7570 706f 7274 2066 6f72 206f 7468   support for oth
+000101f0: 6572 2073 696d 756c 6174 6f72 7320 2865  er simulators (e
+00010200: 783a 206e 6773 7069 6365 2920 7768 6572  x: ngspice) wher
+00010210: 6520 7468 6520 7369 6d75 6c61 746f 7220  e the simulator 
+00010220: 6973 2064 6566 696e 6564 2062 7920 6120  is defined by a 
+00010230: 636c 6173 732e 2054 6869 730d 0a20 2020  class. This..   
+00010240: 2020 2073 7570 706f 7274 2063 6c61 7373     support class
+00010250: 206e 6565 6473 2074 6f20 6265 2061 2073   needs to be a s
+00010260: 7562 636c 6173 7320 6f66 2074 6865 2061  ubclass of the a
+00010270: 6273 7472 6163 7420 636c 6173 7320 5369  bstract class Si
+00010280: 6d75 6c61 746f 722e 0d0a 2020 2020 2a20  mulator...    * 
+00010290: 456e 6f72 6d6f 7573 2069 6d70 726f 7665  Enormous improve
+000102a0: 6d65 6e74 2069 6e20 7468 6520 646f 6375  ment in the docu
+000102b0: 6d65 6e74 6174 696f 6e20 6f66 2074 6865  mentation of the
+000102c0: 2063 6f64 652e 0d0a 0d0a 2a20 5665 7273   code.....* Vers
+000102d0: 696f 6e20 332e 300d 0a20 2020 202a 2045  ion 3.0..    * E
+000102e0: 6c69 6d69 6e61 7469 6e67 2074 6865 204c  liminating the L
+000102f0: 5453 7069 6365 2070 7265 6669 7865 7320  TSpice prefixes 
+00010300: 6672 6f6d 2066 696c 6573 2061 6e64 2063  from files and c
+00010310: 6c61 7373 6573 2e0d 0a20 2020 202a 2041  lasses...    * A
+00010320: 646f 7074 696e 6720 7468 6520 6c6f 7765  dopting the lowe
+00010330: 7263 6173 6520 636f 6e76 656e 7469 6f6e  rcase convention
+00010340: 2066 6f72 2066 696c 656e 616d 6573 2e0d   for filenames..
+00010350: 0a0d 0a2a 2056 6572 7369 6f6e 2032 2e33  ...* Version 2.3
+00010360: 2e31 0d0a 2020 2020 2a20 4275 6720 6669  .1..    * Bug fi
+00010370: 7820 6f6e 2074 6865 2070 6172 616d 6574  x on the paramet
+00010380: 6572 2072 6570 6c61 6365 6d65 6e74 2e0d  er replacement..
+00010390: 0a0d 0a2a 2056 6572 7369 6f6e 2032 2e33  ...* Version 2.3
+000103a0: 0d0a 2020 2020 2a20 5375 7070 6f72 7469  ..    * Supporti
+000103b0: 6e67 2074 6865 2063 7265 6174 696f 6e20  ng the creation 
+000103c0: 6f66 2052 4157 204e 6f69 7365 2041 6e61  of RAW Noise Ana
+000103d0: 6c79 7369 730d 0a20 2020 202a 2042 7567  lysis..    * Bug
+000103e0: 2046 6978 6573 2028 5365 6520 4769 7448   Fixes (See GitH
+000103f0: 7562 204c 6f67 290d 0a0d 0a2a 2056 6572  ub Log)....* Ver
+00010400: 7369 6f6e 2032 2e32 0d0a 2020 2020 2a20  sion 2.2..    * 
+00010410: 4d61 6b69 6e67 206e 756d 7079 2061 7320  Making numpy as 
+00010420: 6120 7265 7175 6972 656d 656e 7420 616e  a requirement an
+00010430: 6420 656c 696d 696e 6174 696e 6720 616c  d eliminating al
+00010440: 6c20 636f 6465 2074 6861 7420 6176 6f69  l code that avoi
+00010450: 6465 6420 7468 6520 7573 6520 6f66 206e  ded the use of n
+00010460: 756d 7079 0d0a 2020 2020 2a20 5573 696e  umpy..    * Usin
+00010470: 6720 6e65 7720 7061 636b 6167 696e 6720  g new packaging 
+00010480: 746f 6f6c 0d0a 2020 2020 2a20 4669 7865  tool..    * Fixe
+00010490: 7320 6f6e 2074 6865 204c 5453 7069 6365  s on the LTSpice
+000104a0: 5f52 6177 5772 6974 650d 0a20 2020 202a  _RawWrite..    *
+000104b0: 2046 6978 6573 2069 6e20 7468 6520 6861   Fixes in the ha
+000104c0: 6e64 6c69 6e67 206f 6620 7374 6570 7065  ndling of steppe
+000104d0: 6420 6f70 6572 6174 696e 6720 706f 696e  d operating poin
+000104e0: 7420 7369 6d75 6c61 7469 6f6e 730d 0a0d  t simulations...
+000104f0: 0a2a 2056 6572 7369 6f6e 2032 2e31 0d0a  .* Version 2.1..
+00010500: 2020 2020 2a20 4164 6f70 7469 6e67 206d      * Adopting m
+00010510: 696e 696d 756d 2070 7974 686f 6e20 7665  inimum python ve
+00010520: 7273 696f 6e20 332e 370d 0a20 2020 202a  rsion 3.7..    *
+00010530: 2053 7461 7274 696e 6720 746f 2075 7365   Starting to use
+00010540: 2075 6e69 7420 7465 7374 7320 746f 2076   unit tests to v
+00010550: 616c 6964 6174 6520 616c 6c20 6d6f 6475  alidate all modu
+00010560: 6c65 7320 616e 6420 696d 7072 6f76 696e  les and improvin
+00010570: 6720 7465 7374 6265 6e63 6865 730d 0a20  g testbenches.. 
+00010580: 2020 202a 2043 6f6d 7061 7469 6269 6c69     * Compatibili
+00010590: 7479 2077 6974 6820 4e47 5370 6963 650d  ty with NGSpice.
+000105a0: 0a20 2020 202a 2041 766f 6964 696e 6720  .    * Avoiding 
+000105b0: 7468 6520 7573 6520 6f66 2073 6574 7570  the use of setup
+000105c0: 2e70 7920 6173 2070 6572 2050 4550 3531  .py as per PEP51
+000105d0: 3720 616e 6420 5045 5035 3138 0d0a 2020  7 and PEP518..  
+000105e0: 2020 2a20 4275 6720 4669 7865 7320 2853    * Bug Fixes (S
+000105f0: 6565 2047 6974 4875 6220 6c6f 6720 666f  ee GitHub log fo
+00010600: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+00010610: 6f6e 290d 0a20 2020 202a 2049 6d70 726f  on)..    * Impro
+00010620: 7665 6d65 6e74 7320 6f6e 2074 6865 206d  vements on the m
+00010630: 616e 6167 656d 656e 7420 6f66 2073 7465  anagement of ste
+00010640: 7070 6564 2064 6174 6120 696e 2074 6865  pped data in the
+00010650: 204c 5453 7069 6365 5f52 6177 5265 6164   LTSpice_RawRead
+00010660: 2e70 790d 0a0d 0a2a 2056 6572 7369 6f6e  .py....* Version
+00010670: 2032 2e30 2e32 0d0a 2020 2020 2a20 496d   2.0.2..    * Im
+00010680: 7072 6f76 656d 656e 7473 206f 6e20 456e  provements on En
+00010690: 636f 6469 6e67 2064 6574 6563 7469 6f6e  coding detection
+000106a0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 322e  ....* Version 2.
+000106b0: 300d 0a20 2020 202a 2049 6e74 6572 6e61  0..    * Interna
+000106c0: 7469 6f6e 616c 2053 7570 706f 7274 2075  tional Support u
+000106d0: 7369 6e67 2074 6865 2063 6f72 7265 6374  sing the correct
+000106e0: 2065 6e63 6f64 696e 6720 7768 656e 206c   encoding when l
+000106f0: 6f61 6469 6e67 206c 6f67 2066 696c 6573  oading log files
+00010700: 2e0d 0a20 2020 202a 2043 6f64 6520 4f70  ...    * Code Op
+00010710: 7469 6d69 7a61 7469 6f6e 7320 6f6e 2074  timizations on t
+00010720: 6865 204c 5453 7069 6365 5f52 6177 5265  he LTSpice_RawRe
+00010730: 6164 6572 2074 6861 7420 616c 6c6f 7720  ader that allow 
+00010740: 6661 7374 6572 2064 6174 6120 6c6f 6164  faster data load
+00010750: 696e 672e 0d0a 2020 2020 2a20 496d 7072  ing...    * Impr
+00010760: 6f76 696e 6720 7468 6520 6675 6e63 7469  oving the functi
+00010770: 6f6e 616c 6974 7920 6f6e 2074 6865 204c  onality on the L
+00010780: 5453 7069 6365 5f52 6177 5772 6974 6572  TSpice_RawWriter
+00010790: 2e70 790d 0a20 2020 202a 2041 6464 696e  .py..    * Addin
+000107a0: 6720 7375 7070 6f72 7420 746f 2065 6469  g support to edi
+000107b0: 7469 6e67 2063 6f6d 706f 6e65 6e74 7320  ting components 
+000107c0: 696e 7369 6465 2073 7562 6369 7263 7569  inside subcircui
+000107d0: 7473 2028 2e73 7562 636b 7429 0d0a 2020  ts (.subckt)..  
+000107e0: 2020 2a20 5375 7070 6f72 7469 6e67 2072    * Supporting r
+000107f0: 6573 6973 746f 7273 2077 6974 6820 4d6f  esistors with Mo
+00010800: 6465 6c20 4465 6669 6e69 7469 6f6e 730d  del Definitions.
+00010810: 0a20 2020 202a 2046 6978 696e 6720 7072  .    * Fixing pr
+00010820: 6f62 6c65 6d20 7769 7468 204c 5453 7069  oblem with LTSpi
+00010830: 6365 4c6f 6752 6561 6465 7220 7468 6174  ceLogReader that
+00010840: 2077 6f75 6c64 2072 6574 7572 6e20 6d65   would return me
+00010850: 7373 6564 2075 7020 6461 7461 0d0a 2020  ssed up data..  
+00010860: 2020 2a20 4669 7869 6e67 2070 726f 626c    * Fixing probl
+00010870: 656d 2077 6974 6820 7265 706c 6163 696e  em with replacin
+00010880: 6720 7468 6520 6669 6c65 2065 7874 656e  g the file exten
+00010890: 7369 6f6e 2069 6e20 6365 7274 6169 6e20  sion in certain 
+000108a0: 6e61 6d65 730d 0a20 2020 202a 2043 6f72  names..    * Cor
+000108b0: 7265 6374 696e 6720 7072 6f62 6c65 6d20  recting problem 
+000108c0: 7769 7468 2064 6570 7265 6361 7469 6f6e  with deprecation
+000108d0: 7320 6f6e 2074 6865 206e 756d 7079 2066  s on the numpy f
+000108e0: 756e 6374 696f 6e73 2075 7365 6420 6279  unctions used by
+000108f0: 2074 6865 2048 6973 746f 6772 616d 2e70   the Histogram.p
+00010900: 790d 0a20 2020 202a 2041 6464 696e 6720  y..    * Adding 
+00010910: 6261 636b 2074 6865 2052 4541 444d 452e  back the README.
+00010920: 6d64 2074 6861 7420 736f 6d65 686f 7720  md that somehow 
+00010930: 7761 7320 6465 6c65 7465 640d 0a0d 0a2a  was deleted....*
+00010940: 2056 6572 7369 6f6e 2031 2e39 0d0a 2020   Version 1.9..  
+00010950: 2020 2a20 4164 6469 6e67 2073 7570 706f    * Adding suppo
+00010960: 7274 2066 6f72 20c2 b520 6368 6172 6163  rt for .. charac
+00010970: 7465 7220 696e 2074 6865 2053 7069 6365  ter in the Spice
+00010980: 4564 6974 6f72 2e0d 0a20 2020 202a 2041  Editor...    * A
+00010990: 6464 696e 6720 6765 745f 636f 6d70 6f6e  dding get_compon
+000109a0: 656e 745f 666c 6f61 7476 616c 7565 2829  ent_floatvalue()
+000109b0: 206d 6574 686f 6420 696e 2074 6865 206e   method in the n
+000109c0: 6574 6c69 7374 206d 616e 6970 756c 6174  etlist manipulat
+000109d0: 696e 6720 636c 6173 7320 7468 6174 2068  ing class that h
+000109e0: 616e 646c 6573 2074 6865 2063 6f6e 7665  andles the conve
+000109f0: 7273 696f 6e20 6f66 206e 756d 6572 6963  rsion of numeric
+00010a00: 0d0a 2020 2020 2020 6669 656c 6473 2069  ..      fields i
+00010a10: 6e74 6f20 6120 666c 6f61 742e 2054 6869  nto a float. Thi
+00010a20: 7320 6675 6e63 7469 6f6e 2074 616b 6573  s function takes
+00010a30: 2069 6e74 6f20 6163 636f 756e 7420 7468   into account th
+00010a40: 6520 656e 6769 6e65 6572 696e 6720 7175  e engineering qu
+00010a50: 616c 6966 6965 7273 2027 6b27 2066 6f72  alifiers 'k' for
+00010a60: 206b 696c 6f73 2c20 276d 2720 6f72 206d   kilos, 'm' or m
+00010a70: 696c 6973 2c0d 0a20 2020 2020 2027 7527  ilis,..      'u'
+00010a80: 206f 7220 27c2 b527 2066 6f72 206d 6963   or '..' for mic
+00010a90: 726f 6e73 2c20 276e 2720 666f 7220 6e61  rons, 'n' for na
+00010aa0: 6e6f 732c 2027 6627 2066 6f72 2066 656d  nos, 'f' for fem
+00010ab0: 746f 7320 616e 6420 274d 6567 2720 666f  tos and 'Meg' fo
+00010ac0: 7220 4d65 6761 732e 0d0a 0d0a 2a20 5665  r Megas.....* Ve
+00010ad0: 7273 696f 6e20 312e 380d 0a20 2020 202a  rsion 1.8..    *
+00010ae0: 2055 6e69 666f 726d 696e 6720 4c69 6365   Uniforming Lice
+00010af0: 6e73 6520 7265 6665 7265 6e63 6520 6163  nse reference ac
+00010b00: 726f 7373 2066 696c 6573 2061 6e64 2069  ross files and i
+00010b10: 6d70 726f 7665 6d65 6e74 7320 6f6e 2074  mprovements on t
+00010b20: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00010b30: 0d0a 2020 2020 2a20 416e 2065 6e6f 726d  ..    * An enorm
+00010b40: 6f75 7320 616e 6420 7768 6f6c 6568 6561  ous and wholehea
+00010b50: 7274 6564 2074 6861 6e6b 7320 746f 2040  rted thanks to @
+00010b60: 6c70 6865 7272 2066 6f72 2074 6865 2069  lpherr for the i
+00010b70: 6d70 726f 7665 6d65 6e74 7320 696e 2074  mprovements in t
+00010b80: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00010b90: 2e0d 0a20 2020 202a 2042 7567 6669 7820  ...    * Bugfix 
+00010ba0: 6f6e 2074 6865 2061 6464 5f4c 5473 7069  on the add_LTspi
+00010bb0: 6365 5275 6e43 6d64 4c69 6e65 5377 6974  ceRunCmdLineSwit
+00010bc0: 6368 6573 2829 203b 2053 7570 706f 7274  ches() ; Support
+00010bd0: 696e 6720 2e70 6172 616d 206e 616d 6520  ing .param name 
+00010be0: 7661 6c75 6520 666f 726d 6174 0d0a 2020  value format..  
+00010bf0: 2020 2a20 416c 6c6f 7769 6e67 2074 6865    * Allowing the
+00010c00: 204c 5453 7069 6365 5261 7752 6561 6420   LTSpiceRawRead 
+00010c10: 746f 2070 726f 6365 6564 2077 6865 6e20  to proceed when 
+00010c20: 7468 6520 6c6f 6720 6669 6c65 2063 616e  the log file can
+00010c30: 2774 2062 6520 666f 756e 6420 6f72 2077  't be found or w
+00010c40: 6865 6e20 7468 6572 6520 6172 6520 7072  hen there are pr
+00010c50: 6f62 6c65 6d73 2072 6561 6469 6e67 2069  oblems reading i
+00010c60: 742e 0d0a 2a20 5665 7273 696f 6e20 312e  t...* Version 1.
+00010c70: 370d 0a20 2020 202a 2052 756e 6e69 6e67  7..    * Running
+00010c80: 2069 6e20 4c69 6e75 7820 756e 6465 7220   in Linux under 
+00010c90: 7769 6e65 2069 7320 6e6f 7720 706f 7373  wine is now poss
+00010ca0: 6962 6c65 0d0a 0d0a 2a20 5665 7273 696f  ible....* Versio
+00010cb0: 6e20 312e 360d 0a20 2020 202a 2041 6464  n 1.6..    * Add
+00010cc0: 696e 6720 4c54 5370 6963 655f 5261 7757  ing LTSpice_RawW
+00010cd0: 7269 7465 2e20 4164 6469 6e67 2064 6f63  rite. Adding doc
+00010ce0: 756d 656e 7461 7469 6f6e 2e0d 0a0d 0a2a  umentation.....*
+00010cf0: 2056 6572 7369 6f6e 2031 2e35 0d0a 2020   Version 1.5..  
+00010d00: 2020 2a20 536d 616c 6c20 6669 7865 7320    * Small fixes 
+00010d10: 616e 6420 696d 7072 6f76 656d 656e 7473  and improvements
+00010d20: 206f 6e20 7468 6520 636c 6173 7320 7573   on the class us
+00010d30: 6167 652e 204e 6f20 6164 6465 6420 6665  age. No added fe
+00010d40: 6174 7572 6573 0d0a 0d0a 2a20 5665 7273  atures....* Vers
+00010d50: 696f 6e20 312e 340d 0a20 2020 202a 2041  ion 1.4..    * A
+00010d60: 6464 696e 6720 7468 6520 4c54 5370 6963  dding the LTSpic
+00010d70: 655f 5365 6d69 4465 764f 7052 6561 6465  e_SemiDevOpReade
+00010d80: 7220 6d6f 6475 6c65 0d0a 2020 2020 2a20  r module..    * 
+00010d90: 5265 2d65 6e61 626c 696e 6720 7468 6520  Re-enabling the 
+00010da0: 4869 7374 6f67 7261 6d20 6675 6e63 7469  Histogram functi
+00010db0: 6f6e 7320 7768 6963 6820 7768 6572 6520  ons which where 
+00010dc0: 6469 7361 626c 6564 2062 7920 6d69 7374  disabled by mist
+00010dd0: 616b 652e 0d0a 0d0a 2a20 5665 7273 696f  ake.....* Versio
+00010de0: 6e20 312e 330d 0a20 2020 202a 2042 7567  n 1.3..    * Bug
+00010df0: 2066 6978 6573 206f 6e20 7468 6520 5370   fixes on the Sp
+00010e00: 6963 6545 6469 746f 7220 436c 6173 730d  iceEditor Class.
+00010e10: 0a0d 0a2a 2056 6572 7369 6f6e 2031 2e32  ...* Version 1.2
+00010e20: 0d0a 2020 2020 2a20 5245 4144 4d45 2e6d  ..    * README.m
+00010e30: 643a 0d0a 2020 2020 2020 4164 6469 6e67  d:..      Adding
+00010e40: 206c 696e 6b20 746f 2072 6561 6474 6865   link to readthe
+00010e50: 646f 6373 2064 6f63 756d 656e 7461 7469  docs documentati
+00010e60: 6f6e 0d0a 2020 2020 2a20 416c 6c20 6669  on..    * All fi
+00010e70: 6c65 733a 0d0a 2020 2020 2020 436f 6d70  les:..      Comp
+00010e80: 7265 6865 6e73 6976 6520 646f 6375 6d65  rehensive docume
+00010e90: 6e74 6174 696f 6e20 6f6e 2068 6f77 2074  ntation on how t
+00010ea0: 6f20 7573 6520 6561 6368 206d 6f64 756c  o use each modul
+00010eb0: 650d 0a0d 0a2a 2056 6572 7369 6f6e 2031  e....* Version 1
+00010ec0: 2e31 0d0a 2020 2020 2a20 5245 4144 4d45  .1..    * README
+00010ed0: 2e6d 643a 0d0a 2020 2020 2020 5570 6461  .md:..      Upda
+00010ee0: 7465 6420 7468 6520 6465 7363 7269 7074  ted the descript
+00010ef0: 696f 6e0d 0a20 2020 202a 204c 5453 7069  ion..    * LTSpi
+00010f00: 6365 4261 7463 682e 7079 3a0d 0a20 2020  ceBatch.py:..   
+00010f10: 2020 2043 6f72 7265 6374 6564 2074 6865     Corrected the
+00010f20: 206e 616d 6520 6f66 2074 6865 2072 6574   name of the ret
+00010f30: 7572 6e65 6420 7261 7720 6669 6c65 2e0d  urned raw file..
+00010f40: 0a20 2020 202a 2041 6464 6564 2063 6f6d  .    * Added com
+00010f50: 6d65 6e74 7320 7468 726f 7567 686f 7574  ments throughout
+00010f60: 2074 6865 2063 6f64 6520 616e 6420 636c   the code and cl
+00010f70: 6561 6e75 700d 0a0d 0a2a 2056 6572 7369  eanup....* Versi
+00010f80: 6f6e 2031 2e30 0d0a 2020 2020 2a20 4c54  on 1.0..    * LT
+00010f90: 5370 6963 6542 6174 6368 2e70 793a 5c0d  SpiceBatch.py:\.
+00010fa0: 0a20 2020 2020 2049 6d70 6c65 6d65 6e74  .      Implement
+00010fb0: 6564 2061 206e 6577 2061 7070 726f 6163  ed a new approac
+00010fc0: 6820 284e 4f54 2042 4143 4b57 4152 4453  h (NOT BACKWARDS
+00010fd0: 2043 4f4d 5041 5449 424c 4529 2c20 7468   COMPATIBLE), th
+00010fe0: 6174 2061 766f 6964 7320 7468 6520 7573  at avoids the us
+00010ff0: 6167 6520 6f66 2074 6865 2073 696d 5f73  age of the sim_s
+00011000: 6574 7469 6e67 732e 696e 6320 6669 6c65  ettings.inc file
+00011010: 2e0d 0a20 2020 2020 2041 6e64 2061 6c6c  ...      And all
+00011020: 6f77 7320 746f 206d 6f64 6966 7920 6e6f  ows to modify no
+00011030: 7420 6f6e 6c79 2070 6172 616d 6574 6572  t only parameter
+00011040: 732c 2062 7574 2061 6c73 6f20 6d6f 6465  s, but also mode
+00011050: 6c73 2061 6e64 2065 7665 6e20 7468 6520  ls and even the 
+00011060: 7369 6d75 6c61 7469 6f6e 2063 6f6d 6d61  simulation comma
+00011070: 6e64 732e 0d0a 2020 2020 2a20 4c54 5370  nds...    * LTSp
+00011080: 6963 655f 5261 7752 6561 642e 7079 3a5c  ice_RawRead.py:\
+00011090: 0d0a 2020 2020 2020 4164 6465 6420 7468  ..      Added th
+000110a0: 6520 6765 745f 7469 6d65 5f61 7869 7320  e get_time_axis 
+000110b0: 6d65 7468 6f64 2074 6f20 7468 6520 5261  method to the Ra
+000110c0: 7752 6561 6420 636c 6173 7320 746f 2061  wRead class to a
+000110d0: 766f 6964 2074 6865 2070 726f 626c 656d  void the problem
+000110e0: 7320 7769 7468 206e 6567 6174 6976 6520  s with negative 
+000110f0: 7661 6c75 6573 206f 6e20 7469 6d65 2061  values on time a
+00011100: 7869 732c 0d0a 2020 2020 2020 7768 656e  xis,..      when
+00011110: 2032 6e64 206f 7264 6572 2063 6f6d 7072   2nd order compr
+00011120: 6573 7369 6f6e 2069 7320 656e 6162 6c65  ession is enable
+00011130: 6420 696e 204c 5453 7069 6365 2e0d 0a20  d in LTSpice... 
+00011140: 2020 202a 204c 5453 7465 7073 2e70 793a     * LTSteps.py:
+00011150: 5c0d 0a20 2020 2020 204d 6f64 6966 6965  \..      Modifie
+00011160: 6420 7468 6520 4c54 5374 6570 732c 2073  d the LTSteps, s
+00011170: 6f20 6974 2063 616e 2061 6c73 6f20 7265  o it can also re
+00011180: 6164 206d 6561 7375 7265 6d65 6e74 7320  ad measurements 
+00011190: 6f6e 206c 6f67 2066 696c 6573 2077 6974  on log files wit
+000111a0: 686f 7574 2061 6e79 2073 7465 7073 2064  hout any steps d
+000111b0: 6f6e 652e 0d0a 0d0a 2a20 5665 7273 696f  one.....* Versio
+000111c0: 6e20 302e 360d 0a20 202a 2048 6973 746f  n 0.6..  * Histo
+000111d0: 6772 616d 2e70 7920 6e6f 7720 6861 7320  gram.py now has 
+000111e0: 616e 206f 7074 696f 6e20 746f 206d 616b  an option to mak
+000111f0: 6520 7468 6520 6869 7374 6f67 7261 6d20  e the histogram 
+00011200: 6469 7265 6374 6c79 2066 726f 6d20 7661  directly from va
+00011210: 6c75 6573 2073 746f 7265 6420 696e 2074  lues stored in t
+00011220: 6865 2063 6c69 7062 6f61 7264 0d0a 0d0a  he clipboard....
+00011230: 2a20 5665 7273 696f 6e20 302e 350d 0a20  * Version 0.5.. 
+00011240: 202a 2054 6865 204c 5453 7069 6365 5f52   * The LTSpice_R
+00011250: 6177 5265 6164 6572 2e70 7920 6e6f 7720  awReader.py now 
+00011260: 7573 6573 2074 6865 2060 7374 7275 6374  uses the `struct
+00011270: 2e75 6e70 6163 6b60 2066 756e 6374 696f  .unpack` functio
+00011280: 6e20 666f 7220 6120 6661 7374 6572 2065  n for a faster e
+00011290: 7865 6375 7469 6f6e 0d0a 0d0a 2a20 5665  xecution....* Ve
+000112a0: 7273 696f 6e20 302e 340d 0a20 202a 2041  rsion 0.4..  * A
+000112b0: 6464 6564 204c 5453 7069 6365 4261 7463  dded LTSpiceBatc
+000112c0: 682e 7079 2074 6f20 7468 6520 636f 6c6c  h.py to the coll
+000112d0: 6563 7469 6f6e 206f 6620 746f 6f6c 730d  ection of tools.
+000112e0: 0a0d 0a2a 2056 6572 7369 6f6e 2030 2e33  ...* Version 0.3
+000112f0: 0d0a 2020 2a20 4120 7665 7273 696f 6e20  ..  * A version 
+00011300: 6f66 204c 5453 7465 7073 2074 6861 7420  of LTSteps that 
+00011310: 6361 6e20 6265 2069 6d70 6f72 7465 6420  can be imported 
+00011320: 746f 2075 7365 2069 6e20 6120 6869 6768  to use in a high
+00011330: 6572 206c 6576 656c 2073 6372 6970 740d  er level script.
+00011340: 0a0d 0a2a 2056 6572 7369 6f6e 2030 2e32  ...* Version 0.2
+00011350: 0d0a 2020 2a20 4164 6469 6e67 204c 5453  ..  * Adding LTS
+00011360: 7465 7073 2e70 7920 616e 6420 4869 7374  teps.py and Hist
+00011370: 6f67 7261 6d2e 7079 0d0a 0d0a 2a20 5665  ogram.py....* Ve
+00011380: 7273 696f 6e20 302e 3120 0d0a 2020 2a20  rsion 0.1 ..  * 
+00011390: 4669 7273 7420 636f 6d6d 6974 2074 6f20  First commit to 
+000113a0: 7468 6520 6269 7462 7563 6b65 7420 7265  the bitbucket re
+000113b0: 706f 7369 746f 7279 2e0d 0a              pository...
```

### Comparing `pyltspice-5.3.0/PyLTSpice.egg-info/SOURCES.txt` & `pyltspice-5.3.1/PyLTSpice.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 PyLTSpice/sim/sim_stepping.py
 PyLTSpice/sim/tookit/montecarlo.py
 PyLTSpice/sim/tookit/worst_case.py
 PyLTSpice/utils/detect_encoding.py
 PyLTSpice/utils/sweep_iterators.py
 examples/ltsteps_example.py
 examples/raw_plotting.py
+examples/raw_read_example.py
 examples/raw_write_example.py
 examples/run_montecarlo.py
 examples/run_worst_case.py
 examples/sim_runner_asc_example.py
 examples/sim_runner_callback_example.py
 examples/sim_runner_callback_process_example.py
 examples/sim_runner_example.py
 examples/sim_stepper_example.py
 examples/spice_editor_example.py
+examples/sub_circuit_asc_edits.py
 unittests/sweep_iterators_unittest.py
 unittests/test_asc_editor.py
 unittests/test_pyltspice.py
```

### Comparing `pyltspice-5.3.0/README.md` & `pyltspice-5.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -83,48 +83,49 @@
 "TRAN - STEP.raw" and displays all steps of the "I(R1)" trace in a matplotlib plot
 
 ```python
 from PyLTSpice import RawRead
 
 from matplotlib import pyplot as plt
 
-LTR = RawRead("TRAN - STEP.raw")
+LTR = RawRead("./testfiles/TRAN - STEP.raw")
 
 print(LTR.get_trace_names())
 print(LTR.get_raw_property())
 
 IR1 = LTR.get_trace("I(R1)")
 x = LTR.get_trace('time')  # Gets the time axis
 steps = LTR.get_steps()
 for step in range(len(steps)):
     # print(steps[step])
     plt.plot(x.get_wave(step), IR1.get_wave(step), label=steps[step])
 
 plt.legend()  # order a legend
 plt.show()
-```   
+```
+-- in examples/raw_read_example.py   
 
 ### RawWrite ###
 
 The following example writes a RAW file with a 3 milliseconds transient simulation sine with a 10kHz and a cosine with
 9.997kHz
 
 ```python
 import numpy as np
-from PyLTSpice import Trace, RawWrite
-
+from PyLTSpice import RawRead, Trace, RawWrite
 LW = RawWrite(fastacces=False)
 tx = Trace('time', np.arange(0.0, 3e-3, 997E-11))
 vy = Trace('N001', np.sin(2 * np.pi * tx.data * 10000))
 vz = Trace('N002', np.cos(2 * np.pi * tx.data * 9970))
 LW.add_trace(tx)
 LW.add_trace(vy)
 LW.add_trace(vz)
-LW.save("teste_snippet1.raw")
+LW.save("./testfiles/teste_snippet1.raw")
 ```   
+-- in examples/raw_write_example.py [RawWrite Example]
 
 ### SpiceEditor, AscEditor and SimRunner.py ###
 
 This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead or with the
 LTSteps module to read the log file which can contain .MEAS results.
 
 The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be updated
@@ -132,28 +133,32 @@
 
 Here follows an example of operation.
 
 ```python
 from PyLTSpice import SimRunner
 from PyLTSpice import SpiceEditor
 
+# Force another simulatior
+simulator = r"C:\Program Files\LTC\LTspiceXVII\XVIIx64.exe"
+
 # select spice model
 LTC = SimRunner(output_folder='./temp')
-LTC.create_netlist('Batch_Test.asc')
-netlist = SpiceEditor('Batch_Test.net')
+LTC.create_netlist('./testfiles/Batch_Test.asc')
+netlist = SpiceEditor('./testfiles/Batch_Test.net')
 # set default arguments
-netlist.set_parameters(res=0, cap=100e-6, run=-1)
+netlist.set_parameters(res=0, cap=100e-6)
 netlist.set_component_value('R2', '2k')  # Modifying the value of a resistor
 netlist.set_component_value('R1', '4k')
 netlist.set_element_model('V3', "SINE(0 1 3k 0 0 0)")  # Modifying the
 netlist.set_component_value('XU1:C2', 20e-12)  # modifying a define simulation
 netlist.add_instructions(
     "; Simulation settings",
-    ".save V(Vin) I(R1)",
+    ";.param run = 0"
 )
+netlist.set_parameter('run', 0)
 
 for opamp in ('AD712', 'AD820'):
     netlist.set_element_model('XU1', opamp)
     for supply_voltage in (5, 10, 15):
         netlist.set_component_value('V1', supply_voltage)
         netlist.set_component_value('V2', -supply_voltage)
         print("simulating OpAmp", opamp, "Voltage", supply_voltage)
@@ -177,14 +182,15 @@
 # Sim Statistics
 print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
 
 enter = input("Press enter to delete created files")
 if enter == '':
     LTC.file_cleanup()
 ```
+-- in examples/sim_runner_example.py
 
 The example above is using the SpiceEditor to create and modify a spice netlist, but it is also possible to use the
 AscEditor to directly modify the .asc file. The edited .asc file can then be opened by the LTSpice GUI and the
 simulation can be run from there.
 
 ### Simulation Analysis Toolkit ###
 
@@ -218,20 +224,34 @@
 # Tolerances can be set for parameters as well
 mc.set_parameter_deviation('Vos', 3e-4, 5e-3, 'uniform')  # The keyword 'distribution' is optional
 mc.prepare_testbench(num_runs=1000)  # Prepares the testbench for 1000 simulations
 
 # Finally the netlist is saved to a file
 mc.save_netlist('./testfiles/sallenkey_mc.net')
 
-mc.run(100)  # Runs the simulation with splits of 100 runs each
+mc.run_testbench(runs_per_sim=100)  # Runs the simulation with splits of 100 runs each
+logs = mc.read_logfiles()   # Reads the log files and stores the results in the results attribute
+logs.obtain_amplitude_and_phase_from_complex_values()  # Splits the complex values into real and imaginary parts
+logs.export_data('./temp_mc/data_testbench.csv')  # Exports the data to a csv file
+logs.plot_histogram('fcut')  # Plots the histograms for the results
+mc.cleanup_files()  # Deletes the temporary files
+
+print("=====================================")
+# Now using the second method, where the simulations are ran one by one
+mc.clear_simulation_data()  # Clears the simulation data
+mc.reset_netlist()  # Resets the netlist to the original
+mc.run_analysis(num_runs=1000)  # Runs the 1000 simulations
 logs = mc.read_logfiles()   # Reads the log files and stores the results in the results attribute
-logs.export_data('./temp_mc/data.csv')  # Exports the data to a csv file
+logs.export_data('./temp_mc/data_sims.csv')  # Exports the data to a csv file
 logs.plot_histogram('fcut')  # Plots the histograms for the results
 mc.cleanup_files()  # Deletes the temporary files
+
 ```
+-- in examples/run_montecarlo.py
+
 When opening the created sallenkey_mc.net file, we can see that the following circuit.
 
 ![Sallen-Key Amplifier with Montecarlo](./doc/modules/sallenkey_mc.png "Sallen-Key Amplifier with Montecarlo")
 
 The following updates were made to the circuit:
 - The value of each component was replaced by a function that generates a random value within the specified tolerance.
 - The .step param run command was added to the netlist. Starts at -1 which it's the nominal value simulation, and 
@@ -264,25 +284,27 @@
 
 # Tolerances can be set for parameters as well.
 wca.set_parameter_deviation('Vos', 3e-4, 5e-3)
 
 # Finally the netlist is saved to a file
 wca.save_netlist('./testfiles/sallenkey_wc.asc')
 
+wca.run_testbench()  # Runs the simulation with splits of 100 runs each
 
-wca.run()  # Runs the simulation with splits of 100 runs each
 logs = wca.read_logfiles()   # Reads the log files and stores the results in the results attribute
 logs.export_data('./temp_wca/data.csv')  # Exports the data to a csv file
 
 print("Worst case results:")
 for param in ('fcut', 'fcut_FROM'):
     print(f"{param}: min:{logs.min_measure_value(param)} max:{logs.max_measure_value(param)}")
 
 wca.cleanup_files()  # Deletes the temporary files
 ```
+-- in examples/run_worst_case.py
+
 When opening the created sallenkey_wc.net file, we can see that the following circuit.
 
 ![Sallen-Key Amplifier with WCA](./doc/modules/sallenkey_wc.png "Sallen-Key Amplifier with WCA")
 
 The following updates were made to the circuit:
 - The value of each component was replaced by a function that generates a nominal, minimum and maximum value depending
 on the run parameter and is assigned a unique index number. (R1=0, Vos=1, R2=2, ... V2=7, VIN=8)
@@ -302,17 +324,20 @@
 ### LTSteps.py ###
 
 This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is
 written. There are two possible usages of this module, either programmatically by importing the module and then
 accessing data through the class as exemplified here:
 
 ```python
+#!/usr/bin/env python
+# coding=utf-8
+
 from PyLTSpice.log.ltsteps import LTSpiceLogReader
 
-data = LTSpiceLogReader("Batch_Test_AD820_15.log")
+data = LTSpiceLogReader("./testfiles/Batch_Test_AD820_15.log")
 
 print("Number of steps  :", data.step_count)
 step_names = data.get_step_vars()
 meas_names = data.get_measure_names()
 
 # Printing Headers
 print(' '.join([f"{step:15s}" for step in step_names]), end='')  # Print steps names with no new line
@@ -320,14 +345,15 @@
 # Printing data
 for i in range(data.step_count):
     print(' '.join([f"{data[step][i]:15}" for step in step_names]), end='')  # Print steps names with no new line
     print(' '.join([f"{data[name][i]:15}" for name in meas_names]), end='\n')  # Print Header
 
 print("Total number of measures found :", data.measure_count)
 ```
+-- in examples/ltsteps_example.py
 
 The second possibility is to use the module directly on the command line
 
 # Command Line Interface #
 
 ### ltsteps.exe ###
 
@@ -428,14 +454,19 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](mailto:me@nunobrum.com)
 * Alternative contact : [nuno.brum@gmail.com](mailto:nuno.brum@gmail.com)
 
 ## History ##
+* Version 5.3.1
+  * Bugfixes 
+    * Updates on the README.md file. Issue #137
+    * Hierarchical support on AscEditor. Issue #138
+  * Rich format is only used if the user has it already installed. Issue #136
 * Version 5.3.0
   * Hierarchical Support (Aligning with the spicelib 1.1.1)
 * Version 5.2.3
   * Updating loggers to use the "spicelib" IDs.
   * Fixing autodoc errors
   * Correcting Version references
```

### Comparing `pyltspice-5.3.0/examples/ltsteps_example.py` & `pyltspice-5.3.1/examples/ltsteps_example.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/examples/raw_plotting.py` & `pyltspice-5.3.1/examples/raw_plotting.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/examples/raw_write_example.py` & `pyltspice-5.3.1/examples/raw_write_example.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-import numpy as np
-from PyLTSpice import RawRead, Trace, RawWrite
-
 
 def test_readme_snippet():
+    # -- Start of RawWrite Example --
+    import numpy as np
+    from PyLTSpice import RawRead, Trace, RawWrite
     LW = RawWrite(fastacces=False)
     tx = Trace('time', np.arange(0.0, 3e-3, 997E-11))
     vy = Trace('N001', np.sin(2 * np.pi * tx.data * 10000))
     vz = Trace('N002', np.cos(2 * np.pi * tx.data * 9970))
     LW.add_trace(tx)
     LW.add_trace(vy)
     LW.add_trace(vz)
     LW.save("./testfiles/teste_snippet1.raw")
+    # -- End of RawWrite Example --
 
 
 def test_trc2raw():  # Convert Teledyne-Lecroy trace files to raw files
+    # -- Start of Lecroy Raw File into LTspice raw file Example --
+    import numpy as np
+    from PyLTSpice import RawRead, Trace, RawWrite
     f = open(r"./testfiles/Current_Lock_Front_Right_8V.trc")
     raw_type = ''  # Initialization of parameters that need to be overridden by the file header
     wave_size = 0
     for line in f:
         tokens = line.rstrip('\r\n').split(',')
         if len(tokens) == 4:
             if tokens[0] == 'Segments' and tokens[2] == 'SegmentSize':
@@ -29,17 +33,21 @@
     if raw_type == 'transient' and wave_size > 0:
         data = np.genfromtxt(f, dtype='float,float', delimiter=',', max_rows=wave_size)
         LW = RawWrite()
         LW.add_trace(Trace('time', [x[0] for x in data]))
         LW.add_trace(Trace('Ampl', [x[1] for x in data]))
         LW.save("teste_trc.raw")
     f.close()
+    # -- End of Lecroy Raw File into LTspice raw file Example --
 
 
 def test_axis_sync():  # Test axis sync
+    # -- Start of Combining two different time axis --
+    import numpy as np
+    from PyLTSpice import RawRead, Trace, RawWrite
     LW = RawWrite()
     tx = Trace('time', np.arange(0.0, 3e-3, 997E-11))
     vy = Trace('N001', np.sin(2 * np.pi * tx.data * 10000))
     vz = Trace('N002', np.cos(2 * np.pi * tx.data * 9970))
     LW.add_trace(tx)
     LW.add_trace(vy)
     LW.add_trace(vz)
@@ -60,52 +68,62 @@
     for ii in range(len(vy)):
         err = abs(v[ii] - vy[ii])
         if err > max_error:
             max_error = err
             print(v[ii], vy[ii], v[ii] - vy[ii])
     print(max_error)
     """
+    # -- End of Combining two different Raw Files --
 
 
 def test_write_ac():
+    # -- Start of Writing .AC raw files Example --
+    from PyLTSpice import RawRead, Trace, RawWrite
     LW = RawWrite()
     LR = RawRead("./testfiles/PI_Filter.raw")
     LR1 = RawRead("./testfiles/PI_Filter_resampled.raw")
     LW.add_traces_from_raw(LR, ('V(N002)',))
     LW.add_traces_from_raw(LR1, 'V(N002)', rename_format='N002_resampled', force_axis_alignment=True)
     LW.flag_fastaccess = False
     LW.save("./testfiles/PI_filter_rewritten.raw")
     LW.flag_fastaccess = True
     LW.save("./testfiles/PI_filter_rewritten_fast.raw")
+    # -- End of Writing .AC raw files Example --
 
 
 def test_write_tran():
+    # -- Start of creating a subset of a raw file --
+    from PyLTSpice import RawRead, Trace, RawWrite
     LR = RawRead("./testfiles/TRAN - STEP.raw")
     LW = RawWrite()
     LW.add_traces_from_raw(LR, ('V(out)', 'I(C1)'))
     LW.flag_fastaccess = False
     LW.save("./testfiles/TRAN - STEP0_normal.raw")
     LW.flag_fastaccess = True
     LW.save("./testfiles/TRAN - STEP0_fast.raw")
+    # -- End of creating a subset of a raw file --
 
 
 def test_combine_tran():
+    # -- Start of Combining two different Raw Files --
+    from PyLTSpice import RawRead, RawWrite
     LW = RawWrite()
     for tag, raw in (
             ("AD820_15", "./testfiles/Batch_Test_AD820_15.raw"),
             # ("AD820_10", "./testfiles/Batch_Test_AD820_10.raw"),
             ("AD712_15", "./testfiles/Batch_Test_AD712_15.raw"),
             # ("AD712_10", "./testfiles/Batch_Test_AD712_10.raw"),
             # ("AD820_5", "./testfiles/Batch_Test_AD820_5.raw"),
             # ("AD712_5", "./testfiles/Batch_Test_AD712_5.raw"),
     ):
         LR = RawRead(raw)
         LW.add_traces_from_raw(LR, ("V(out)", "I(R1)"), rename_format="{}_{tag}", tag=tag, force_axis_alignment=True)
     LW.flag_fastaccess = False
     LW.save("./testfiles/Batch_Test_Combine.raw")
+    # -- End of Combining two different Raw Files --
 
 
 test_readme_snippet()
 test_axis_sync()
 test_write_ac()
 test_write_tran()
 test_combine_tran()
```

### Comparing `pyltspice-5.3.0/examples/run_montecarlo.py` & `pyltspice-5.3.1/examples/run_montecarlo.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/examples/run_worst_case.py` & `pyltspice-5.3.1/examples/run_worst_case.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/examples/sim_runner_asc_example.py` & `pyltspice-5.3.1/examples/sim_runner_asc_example.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/examples/sim_runner_callback_example.py` & `pyltspice-5.3.1/examples/sim_runner_callback_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # coding=utf-8
 import logging
-from rich.logging import RichHandler
+try:
+    from rich.logging import RichHandler
+except ImportError:
+    RichHandler = None
 import PyLTSpice
 
-from PyLTSpice import SimRunner, SpiceEditor
+from PyLTSpice import SimRunner, AscEditor
 PyLTSpice.set_log_level(logging.DEBUG)
-PyLTSpice.add_log_handler(RichHandler())
+if RichHandler:
+    PyLTSpice.add_log_handler(RichHandler())
 
 from time import sleep
 from random import random
 
 
 def processing_data(raw_file, log_file):
     print("Handling the simulation data of ""%s"", log file ""%s""" % (raw_file, log_file))
@@ -18,37 +22,37 @@
     sleep(time_to_sleep)
     return "This is the result passed to the iterator"
 
 
 runner = SimRunner(output_folder='./temp_batch3')  # Configures the simulator to use and output
 # folder
 
-netlist = SpiceEditor("./testfiles/Batch_Test.asc")  # Open the Spice Model, and creates the .net
+netlist = AscEditor("./testfiles/Batch_Test.asc")  # Open the Spice Model, and creates the .net
 # set default arguments
 netlist.set_parameters(res=0, cap=100e-6)
 netlist.set_component_value('R2', '2k')  # Modifying the value of a resistor
 netlist.set_component_value('R1', '4k')
 netlist.set_element_model('V3', "SINE(0 1 3k 0 0 0)")  # Modifying the
-netlist.set_component_value('XU1:C2', 20e-12)  # modifying a
+netlist.set_component_value('U1:C2', 20e-12)  # modifying a
 # define simulation
 netlist.add_instructions(
     "; Simulation settings",
     ";.param run = 0"
 )
 netlist.set_parameter('run', 0)
 
 use_run_now = False
 
 for opamp in ('AD712', 'AD820'):
-    netlist.set_element_model('XU1', opamp)
+    netlist.set_element_model('U1', opamp)
     for supply_voltage in (5, 10, 15):
         netlist.set_component_value('V1', supply_voltage)
         netlist.set_component_value('V2', -supply_voltage)
         # overriding the automatic netlist naming
-        run_netlist_file = "{}_{}_{}.net".format(netlist.netlist_file.stem, opamp, supply_voltage)
+        run_netlist_file = "{}_{}_{}.net".format(netlist.circuit_file.stem, opamp, supply_voltage)
         if use_run_now:
             runner.run_now(netlist, run_filename=run_netlist_file)
         else:
             runner.run(netlist, run_filename=run_netlist_file, callback=processing_data)
 
 for results in runner:
     print(results)
```

### Comparing `pyltspice-5.3.0/examples/sim_runner_callback_process_example.py` & `pyltspice-5.3.1/examples/sim_runner_callback_process_example.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/examples/sim_runner_example.py` & `pyltspice-5.3.1/examples/sim_runner_example.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/examples/sim_stepper_example.py` & `pyltspice-5.3.1/examples/sim_stepper_example.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/pyproject.toml` & `pyltspice-5.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "PyLTSpice"
-version = "5.3.0"
+version = "5.3.1"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to Automate LTSpice simulations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
 dependencies = [
-    "spicelib>=1.1.1",
+    "spicelib>=1.1.2",
 ]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pyltspice-5.3.0/unittests/sweep_iterators_unittest.py` & `pyltspice-5.3.1/unittests/sweep_iterators_unittest.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/unittests/test_asc_editor.py` & `pyltspice-5.3.1/unittests/test_asc_editor.py`

 * *Files identical despite different names*

### Comparing `pyltspice-5.3.0/unittests/test_pyltspice.py` & `pyltspice-5.3.1/unittests/test_pyltspice.py`

 * *Files identical despite different names*

