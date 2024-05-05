# Comparing `tmp/wrapyfi-0.4.43.tar.gz` & `tmp/wrapyfi-0.4.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapyfi-0.4.43.tar", last modified: Wed Feb 21 16:27:10 2024, max compression
+gzip compressed data, was "wrapyfi-0.4.44.tar", last modified: Sun May  5 15:52:31 2024, max compression
```

## Comparing `wrapyfi-0.4.43.tar` & `wrapyfi-0.4.44.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rwxr-xr-x   0        0        0     3942 2024-02-21 16:26:41.722180 wrapyfi-0.4.43/LICENSE
--rwxr-xr-x   0        0        0    16569 2024-02-21 16:27:07.878239 wrapyfi-0.4.43/README.md
--rwxr-xr-x   0        0        0      558 2024-02-21 16:26:41.790180 wrapyfi-0.4.43/examples/README.md
--rwxr-xr-x   0        0        0        0 2024-02-21 16:26:41.790180 wrapyfi-0.4.43/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.790180 wrapyfi-0.4.43/examples/applications/__init__.py
--rw-r--r--   0        0        0     7891 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/applications/affective_signaling_multirobot.py
--rw-r--r--   0        0        0     6485 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/applications/gaze_mirroring_multisensor.py
--rw-r--r--   0        0        0      420 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/applications/wrapyfi_configs/affective_signaling_multirobot/COMP_mainpc.yml
--rw-r--r--   0        0        0      418 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/applications/wrapyfi_configs/affective_signaling_multirobot/OPT_icubpc.yml
--rw-r--r--   0        0        0      418 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/applications/wrapyfi_configs/affective_signaling_multirobot/OPT_pepperpc.yml
--rw-r--r--   0        0        0      257 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/applications/wrapyfi_configs/gaze_mirroring_multisensor/COMP_mainpc.yml
--rw-r--r--   0        0        0      258 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/applications/wrapyfi_configs/gaze_mirroring_multisensor/OPT_camera.yml
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/communication_patterns/__init__.py
--rwxr-xr-x   0        0        0    10619 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/communication_patterns/request_reply_example.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/communication_schemes/__init__.py
--rw-r--r--   0        0        0     4989 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/communication_schemes/channeling_example.py
--rw-r--r--   0        0        0     4980 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/communication_schemes/forwarding_example.py
--rw-r--r--   0        0        0     3227 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/communication_schemes/mirroring_example.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/custom_msgs/__init__.py
--rw-r--r--   0        0        0     3081 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/custom_msgs/ros2_message_example.py
--rwxr-xr-x   0        0        0     3043 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/custom_msgs/ros_message_example.py
--rwxr-xr-x   0        0        0     3278 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/custom_msgs/ros_parameter_example.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/__init__.py
--rw-r--r--   0        0        0     3803 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/astropy_example.py
--rw-r--r--   0        0        0     3430 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/cupy_example.py
--rw-r--r--   0        0        0     4011 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/dask_example.py
--rwxr-xr-x   0        0        0     3087 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/jax_example.py
--rwxr-xr-x   0        0        0     3471 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/mxnet_example.py
--rwxr-xr-x   0        0        0     4064 2024-02-21 16:26:50.874194 wrapyfi-0.4.43/examples/encoders/numpy_pandas_example.py
--rwxr-xr-x   0        0        0     3680 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/paddlepaddle_example.py
--rwxr-xr-x   0        0        0     3110 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/pillow_example.py
--rw-r--r--   0        0        0     3389 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/pint_example.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/plugins/__init__.py
--rw-r--r--   0        0        0     3284 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/plugins/astropy_tables.py
--rwxr-xr-x   0        0        0     3003 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/pyarrow_example.py
--rwxr-xr-x   0        0        0     3496 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/pytorch_example.py
--rwxr-xr-x   0        0        0     3207 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/tensorflow_example.py
--rw-r--r--   0        0        0     3275 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/trax_example.py
--rw-r--r--   0        0        0     3582 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/xarray_example.py
--rw-r--r--   0        0        0     3483 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/encoders/zarr_example.py
--rwxr-xr-x   0        0        0     3577 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/hello_world.py
--rwxr-xr-x   0        0        0      522 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/requirements.txt
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/robots/__init__.py
--rwxr-xr-x   0        0        0    52000 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/robots/icub_head.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/sensors/__init__.py
--rwxr-xr-x   0        0        0    11309 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/examples/sensors/cam_mic.py
--rw-r--r--   0        0        0     1921 2024-02-21 16:27:10.558241 wrapyfi-0.4.43/pyproject.toml
--rwxr-xr-x   0        0        0     3462 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/__init__.py
--rwxr-xr-x   0        0        0      899 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/clients/__init__.py
--rwxr-xr-x   0        0        0    15437 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/clients/ros.py
--rwxr-xr-x   0        0        0    18523 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/clients/ros2.py
--rwxr-xr-x   0        0        0    11162 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/clients/yarp.py
--rw-r--r--   0        0        0    12807 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/clients/zeromq.py
--rwxr-xr-x   0        0        0        0 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/config/__init__.py
--rwxr-xr-x   0        0        0     1521 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/config/manager.py
--rwxr-xr-x   0        0        0      252 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/connect/__init__.py
--rwxr-xr-x   0        0        0     2537 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/connect/clients.py
--rwxr-xr-x   0        0        0     4972 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/connect/listeners.py
--rwxr-xr-x   0        0        0     4836 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/connect/publishers.py
--rwxr-xr-x   0        0        0     2846 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/connect/servers.py
--rwxr-xr-x   0        0        0    41481 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/connect/wrapper.py
--rw-r--r--   0        0        0     5540 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/encoders.py
--rwxr-xr-x   0        0        0      888 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/listeners/__init__.py
--rwxr-xr-x   0        0        0    21284 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/listeners/ros.py
--rwxr-xr-x   0        0        0    18117 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/listeners/ros2.py
--rwxr-xr-x   0        0        0    15686 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/listeners/yarp.py
--rwxr-xr-x   0        0        0    14969 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/listeners/zeromq.py
--rwxr-xr-x   0        0        0        0 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/middlewares/__init__.py
--rwxr-xr-x   0        0        0     2707 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/middlewares/ros.py
--rwxr-xr-x   0        0        0     1922 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/middlewares/ros2.py
--rwxr-xr-x   0        0        0     1534 2024-02-21 16:26:41.794180 wrapyfi-0.4.43/wrapyfi/middlewares/yarp.py
--rw-r--r--   0        0        0    36779 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/middlewares/zeromq.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/__init__.py
--rw-r--r--   0        0        0     4268 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/cupy_array.py
--rw-r--r--   0        0        0     5212 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/dask_data.py
--rw-r--r--   0        0        0     3077 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/jax_tensor.py
--rw-r--r--   0        0        0     5572 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/mxnet_tensor.py
--rw-r--r--   0        0        0     5645 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/paddle_tensor.py
--rw-r--r--   0        0        0     6333 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/pandas_data.py
--rw-r--r--   0        0        0     3619 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/pillow_image.py
--rw-r--r--   0        0        0     3550 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/pint_quantities.py
--rw-r--r--   0        0        0     3388 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/pyarrow_array.py
--rw-r--r--   0        0        0     3698 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/pytorch_tensor.py
--rw-r--r--   0        0        0     3047 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/tensorflow_tensor.py
--rw-r--r--   0        0        0     3588 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/trax_array.py
--rw-r--r--   0        0        0     5264 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/xarray_data.py
--rw-r--r--   0        0        0     4648 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/plugins/zarr_array.py
--rwxr-xr-x   0        0        0      882 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/publishers/__init__.py
--rwxr-xr-x   0        0        0    19655 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/publishers/ros.py
--rwxr-xr-x   0        0        0    17131 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/publishers/ros2.py
--rwxr-xr-x   0        0        0    16253 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/publishers/yarp.py
--rw-r--r--   0        0        0    15773 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/publishers/zeromq.py
--rwxr-xr-x   0        0        0      850 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/servers/__init__.py
--rwxr-xr-x   0        0        0    16225 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/servers/ros.py
--rwxr-xr-x   0        0        0    19352 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/servers/ros2.py
--rwxr-xr-x   0        0        0    11909 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/servers/yarp.py
--rw-r--r--   0        0        0    12524 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/servers/zeromq.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/standalone/__init__.py
--rw-r--r--   0        0        0     9096 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/standalone/zeromq_param_server.py
--rw-r--r--   0        0        0     3386 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/standalone/zeromq_proxy_broker.py
--rw-r--r--   0        0        0     1459 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/standalone/zeromq_pubsub_topic_monitor.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/tests/__init__.py
--rw-r--r--   0        0        0     2627 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/tests/test_middleware.py
--rw-r--r--   0        0        0     8101 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/tests/test_wrapper.py
--rw-r--r--   0        0        0        0 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/tests/tools/__init__.py
--rw-r--r--   0        0        0     8152 2024-02-21 16:26:41.798180 wrapyfi-0.4.43/wrapyfi/tests/tools/benchmarking_native_object.py
--rw-r--r--   0        0        0 14869541 2024-02-21 16:26:41.838180 wrapyfi-0.4.43/wrapyfi/tests/tools/benchmarking_plotter.ipynb
--rw-r--r--   0        0        0     1434 2024-02-21 16:26:41.838180 wrapyfi-0.4.43/wrapyfi/tests/tools/class_test.py
--rw-r--r--   0        0        0    95137 2024-02-21 16:26:41.838180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros.csv
--rw-r--r--   0        0        0    97177 2024-02-21 16:26:41.838180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros2.csv
--rw-r--r--   0        0        0    49004 2024-02-21 16:26:41.838180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros2__no-warmup.csv
--rw-r--r--   0        0        0    97019 2024-02-21 16:26:41.842180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_yarp.csv
--rw-r--r--   0        0        0   148705 2024-02-21 16:26:41.842180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_yarp_ros_zeromq__no-warmup.csv
--rw-r--r--   0        0        0    99970 2024-02-21 16:26:41.842180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_zeromq.csv
--rw-r--r--   0        0        0    96345 2024-02-21 16:26:41.842180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros.csv
--rw-r--r--   0        0        0    99297 2024-02-21 16:26:41.842180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros2.csv
--rw-r--r--   0        0        0    49897 2024-02-21 16:26:41.842180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros2__no-warmup.csv
--rw-r--r--   0        0        0    98353 2024-02-21 16:26:41.842180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_yarp.csv
--rw-r--r--   0        0        0   150027 2024-02-21 16:26:41.842180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_yarp_ros_zeromq__no-warmup.csv
--rw-r--r--   0        0        0   102419 2024-02-21 16:26:41.846180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_zeromq.csv
--rw-r--r--   0        0        0  3811764 2024-02-21 16:26:41.866180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/benchmarking_native_object_listen__ros,yarp,zeromq.csv
--rw-r--r--   0        0        0  1269943 2024-02-21 16:26:41.870180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/benchmarking_native_object_listen__ros2.csv
--rw-r--r--   0        0        0  3851767 2024-02-21 16:26:41.874180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/benchmarking_native_object_publish__ros,yarp,zeromq.csv
--rw-r--r--   0        0        0  1275779 2024-02-21 16:26:41.882180 wrapyfi-0.4.43/wrapyfi/tests/tools/results/benchmarking_native_object_publish__ros2.csv
--rwxr-xr-x   0        0        0     8953 2024-02-21 16:26:41.882180 wrapyfi-0.4.43/wrapyfi/utils.py
--rw-r--r--   0        0        0    18755 1970-01-01 00:00:00.000000 wrapyfi-0.4.43/PKG-INFO
+-rwxr-xr-x   0        0        0     3942 2024-05-05 15:52:03.495887 wrapyfi-0.4.44/LICENSE
+-rwxr-xr-x   0        0        0    16573 2024-05-05 15:52:29.379910 wrapyfi-0.4.44/README.md
+-rwxr-xr-x   0        0        0      558 2024-05-05 15:52:03.563887 wrapyfi-0.4.44/examples/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-05 15:52:03.563887 wrapyfi-0.4.44/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.563887 wrapyfi-0.4.44/examples/applications/__init__.py
+-rw-r--r--   0        0        0     7891 2024-05-05 15:52:03.563887 wrapyfi-0.4.44/examples/applications/affective_signaling_multirobot.py
+-rw-r--r--   0        0        0     6485 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/applications/gaze_mirroring_multisensor.py
+-rw-r--r--   0        0        0      420 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/applications/wrapyfi_configs/affective_signaling_multirobot/COMP_mainpc.yml
+-rw-r--r--   0        0        0      418 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/applications/wrapyfi_configs/affective_signaling_multirobot/OPT_icubpc.yml
+-rw-r--r--   0        0        0      418 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/applications/wrapyfi_configs/affective_signaling_multirobot/OPT_pepperpc.yml
+-rw-r--r--   0        0        0      257 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/applications/wrapyfi_configs/gaze_mirroring_multisensor/COMP_mainpc.yml
+-rw-r--r--   0        0        0      258 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/applications/wrapyfi_configs/gaze_mirroring_multisensor/OPT_camera.yml
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/communication_patterns/__init__.py
+-rwxr-xr-x   0        0        0    10619 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/communication_patterns/request_reply_example.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/communication_schemes/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/communication_schemes/channeling_example.py
+-rw-r--r--   0        0        0     4980 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/communication_schemes/forwarding_example.py
+-rw-r--r--   0        0        0     3227 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/communication_schemes/mirroring_example.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/custom_msgs/__init__.py
+-rw-r--r--   0        0        0     3081 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/custom_msgs/ros2_message_example.py
+-rwxr-xr-x   0        0        0     3043 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/custom_msgs/ros_message_example.py
+-rwxr-xr-x   0        0        0     3278 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/custom_msgs/ros_parameter_example.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/__init__.py
+-rw-r--r--   0        0        0     3803 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/astropy_example.py
+-rw-r--r--   0        0        0     3430 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/cupy_example.py
+-rw-r--r--   0        0        0     4011 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/dask_example.py
+-rwxr-xr-x   0        0        0     3087 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/jax_example.py
+-rwxr-xr-x   0        0        0     3471 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/mxnet_example.py
+-rwxr-xr-x   0        0        0     4064 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/numpy_pandas_example.py
+-rwxr-xr-x   0        0        0     3680 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/paddlepaddle_example.py
+-rwxr-xr-x   0        0        0     3110 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/pillow_example.py
+-rw-r--r--   0        0        0     3389 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/pint_example.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/plugins/__init__.py
+-rw-r--r--   0        0        0     3284 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/plugins/astropy_tables.py
+-rwxr-xr-x   0        0        0     3003 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/pyarrow_example.py
+-rwxr-xr-x   0        0        0     3496 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/pytorch_example.py
+-rwxr-xr-x   0        0        0     3207 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/tensorflow_example.py
+-rw-r--r--   0        0        0     3275 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/trax_example.py
+-rw-r--r--   0        0        0     3582 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/xarray_example.py
+-rw-r--r--   0        0        0     3483 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/encoders/zarr_example.py
+-rwxr-xr-x   0        0        0     3577 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/hello_world.py
+-rwxr-xr-x   0        0        0      522 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/requirements.txt
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/robots/__init__.py
+-rwxr-xr-x   0        0        0    52000 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/robots/icub_head.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/sensors/__init__.py
+-rwxr-xr-x   0        0        0    11309 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/examples/sensors/cam_mic.py
+-rw-r--r--   0        0        0     1925 2024-05-05 15:52:31.983912 wrapyfi-0.4.44/pyproject.toml
+-rwxr-xr-x   0        0        0     3462 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/__init__.py
+-rwxr-xr-x   0        0        0      899 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/clients/__init__.py
+-rwxr-xr-x   0        0        0    15437 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/clients/ros.py
+-rwxr-xr-x   0        0        0    18523 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/clients/ros2.py
+-rwxr-xr-x   0        0        0    11162 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/clients/yarp.py
+-rw-r--r--   0        0        0    12807 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/clients/zeromq.py
+-rwxr-xr-x   0        0        0        0 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/config/__init__.py
+-rwxr-xr-x   0        0        0     1521 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/config/manager.py
+-rwxr-xr-x   0        0        0      252 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/connect/__init__.py
+-rwxr-xr-x   0        0        0     2537 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/connect/clients.py
+-rwxr-xr-x   0        0        0     4972 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/connect/listeners.py
+-rwxr-xr-x   0        0        0     4836 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/connect/publishers.py
+-rwxr-xr-x   0        0        0     2846 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/connect/servers.py
+-rwxr-xr-x   0        0        0    41404 2024-05-05 15:52:14.047896 wrapyfi-0.4.44/wrapyfi/connect/wrapper.py
+-rw-r--r--   0        0        0     5540 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/encoders.py
+-rwxr-xr-x   0        0        0      888 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/listeners/__init__.py
+-rwxr-xr-x   0        0        0    21284 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/listeners/ros.py
+-rwxr-xr-x   0        0        0    18117 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/listeners/ros2.py
+-rwxr-xr-x   0        0        0    15686 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/listeners/yarp.py
+-rwxr-xr-x   0        0        0    14969 2024-05-05 15:52:03.567887 wrapyfi-0.4.44/wrapyfi/listeners/zeromq.py
+-rwxr-xr-x   0        0        0        0 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/middlewares/__init__.py
+-rwxr-xr-x   0        0        0     2707 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/middlewares/ros.py
+-rwxr-xr-x   0        0        0     1922 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/middlewares/ros2.py
+-rwxr-xr-x   0        0        0     1534 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/middlewares/yarp.py
+-rw-r--r--   0        0        0    36779 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/middlewares/zeromq.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/__init__.py
+-rw-r--r--   0        0        0     4268 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/cupy_array.py
+-rw-r--r--   0        0        0     5212 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/dask_data.py
+-rw-r--r--   0        0        0     3077 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/jax_tensor.py
+-rw-r--r--   0        0        0     5572 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/mxnet_tensor.py
+-rw-r--r--   0        0        0     5645 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/paddle_tensor.py
+-rw-r--r--   0        0        0     6333 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/pandas_data.py
+-rw-r--r--   0        0        0     3619 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/pillow_image.py
+-rw-r--r--   0        0        0     3550 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/pint_quantities.py
+-rw-r--r--   0        0        0     3388 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/pyarrow_array.py
+-rw-r--r--   0        0        0     3698 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/pytorch_tensor.py
+-rw-r--r--   0        0        0     3047 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/tensorflow_tensor.py
+-rw-r--r--   0        0        0     3588 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/trax_array.py
+-rw-r--r--   0        0        0     5264 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/xarray_data.py
+-rw-r--r--   0        0        0     4648 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/plugins/zarr_array.py
+-rwxr-xr-x   0        0        0      882 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/publishers/__init__.py
+-rwxr-xr-x   0        0        0    19655 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/publishers/ros.py
+-rwxr-xr-x   0        0        0    17131 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/publishers/ros2.py
+-rwxr-xr-x   0        0        0    16253 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/publishers/yarp.py
+-rw-r--r--   0        0        0    17699 2024-05-05 15:52:14.075896 wrapyfi-0.4.44/wrapyfi/publishers/zeromq.py
+-rwxr-xr-x   0        0        0      850 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/servers/__init__.py
+-rwxr-xr-x   0        0        0    16225 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/servers/ros.py
+-rwxr-xr-x   0        0        0    19352 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/servers/ros2.py
+-rwxr-xr-x   0        0        0    11909 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/servers/yarp.py
+-rw-r--r--   0        0        0    12524 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/servers/zeromq.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/standalone/__init__.py
+-rw-r--r--   0        0        0     9096 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/standalone/zeromq_param_server.py
+-rw-r--r--   0        0        0     3386 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/standalone/zeromq_proxy_broker.py
+-rw-r--r--   0        0        0     1459 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/standalone/zeromq_pubsub_topic_monitor.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/tests/__init__.py
+-rw-r--r--   0        0        0     2627 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/tests/test_middleware.py
+-rw-r--r--   0        0        0     8101 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/tests/test_wrapper.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/tests/tools/__init__.py
+-rw-r--r--   0        0        0     8152 2024-05-05 15:52:03.571887 wrapyfi-0.4.44/wrapyfi/tests/tools/benchmarking_native_object.py
+-rw-r--r--   0        0        0 14869541 2024-05-05 15:52:03.611888 wrapyfi-0.4.44/wrapyfi/tests/tools/benchmarking_plotter.ipynb
+-rw-r--r--   0        0        0     1434 2024-05-05 15:52:03.611888 wrapyfi-0.4.44/wrapyfi/tests/tools/class_test.py
+-rw-r--r--   0        0        0    95137 2024-05-05 15:52:03.611888 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros.csv
+-rw-r--r--   0        0        0    97177 2024-05-05 15:52:03.611888 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros2.csv
+-rw-r--r--   0        0        0    49004 2024-05-05 15:52:03.611888 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros2__no-warmup.csv
+-rw-r--r--   0        0        0    97019 2024-05-05 15:52:03.611888 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_yarp.csv
+-rw-r--r--   0        0        0   148705 2024-05-05 15:52:03.615887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_yarp_ros_zeromq__no-warmup.csv
+-rw-r--r--   0        0        0    99970 2024-05-05 15:52:03.615887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_zeromq.csv
+-rw-r--r--   0        0        0    96345 2024-05-05 15:52:03.615887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros.csv
+-rw-r--r--   0        0        0    99297 2024-05-05 15:52:03.615887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros2.csv
+-rw-r--r--   0        0        0    49897 2024-05-05 15:52:03.615887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros2__no-warmup.csv
+-rw-r--r--   0        0        0    98353 2024-05-05 15:52:03.615887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_yarp.csv
+-rw-r--r--   0        0        0   150027 2024-05-05 15:52:03.615887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_yarp_ros_zeromq__no-warmup.csv
+-rw-r--r--   0        0        0   102419 2024-05-05 15:52:03.615887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_zeromq.csv
+-rw-r--r--   0        0        0  3811764 2024-05-05 15:52:03.639887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/benchmarking_native_object_listen__ros,yarp,zeromq.csv
+-rw-r--r--   0        0        0  1269943 2024-05-05 15:52:03.643888 wrapyfi-0.4.44/wrapyfi/tests/tools/results/benchmarking_native_object_listen__ros2.csv
+-rw-r--r--   0        0        0  3851767 2024-05-05 15:52:03.647888 wrapyfi-0.4.44/wrapyfi/tests/tools/results/benchmarking_native_object_publish__ros,yarp,zeromq.csv
+-rw-r--r--   0        0        0  1275779 2024-05-05 15:52:03.655887 wrapyfi-0.4.44/wrapyfi/tests/tools/results/benchmarking_native_object_publish__ros2.csv
+-rwxr-xr-x   0        0        0     8953 2024-05-05 15:52:03.655887 wrapyfi-0.4.44/wrapyfi/utils.py
+-rw-r--r--   0        0        0    18759 1970-01-01 00:00:00.000000 wrapyfi-0.4.44/PKG-INFO
```

### Comparing `wrapyfi-0.4.43/LICENSE` & `wrapyfi-0.4.44/LICENSE`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/README.md` & `wrapyfi-0.4.44/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,39 +42,39 @@
 
 Please refer to the following [paper](https://www2.informatik.uni-hamburg.de/wtm/publications/2024/AAFW24/Abawi_HRI24.pdf) when citing Wrapyfi in academic work:
 
 ```
 @inproceedings{abawi2024wrapyfi,
   title = {Wrapyfi: A Python Wrapper for Integrating Robots, Sensors, and Applications across Multiple Middleware},
   author = {Abawi, Fares and Allgeuer, Philipp and Fu, Di and Wermter, Stefan},
-  booktitle = {Proceedings of the ACM/IEEE Conference on Human-Robot Interaction (HRI '24)},
+  booktitle = {Proceedings of the ACM/IEEE International Conference on Human-Robot Interaction (HRI '24)},
   year = {2024},
   organization = {ACM},
   isbn = {79-8-4007-0322-5},
   doi = {10.1145/3610977.3637471},
   url = {https://github.com/fabawi/wrapyfi}
 }
 ```
 
 # Getting Started
 
 Before using Wrapyfi, YARP, ROS, or ZeroMQ must be installed.
 
 * Follow the [YARP installation guide](https://github.com/fabawi/wrapyfi/tree/main/wrapyfi_extensions/yarp/README.md?rank=0).<!-- [YARP installation guide](docs/yarp_install_lnk.md). -->
-Note that the iCub package is not needed for Wrapyfi to work and does not have to be installed if you do not intend on using the iCub robot.
+Note that the iCub package is not needed for Wrapyfi to work and does not have to be installed if you do not intend to use the iCub robot.
 
 * For installing ROS, follow the ROS installation guide [\[Ubuntu\]](http://wiki.ros.org/noetic/Installation/Ubuntu)[\[Windows\]](https://wiki.ros.org/noetic/Installation/Windows). 
 We recommend installing ROS on Conda using the [RoboStack](https://github.com/RoboStack/ros-noetic) environment. Additionally, the 
 [Wrapyfi ROS interfaces](https://github.com/modular-ml/wrapyfi_ros_interfaces/blob/master/README.md?rank=0) must be
 built to support messages needed for audio transmission [![ROS Package Index](https://img.shields.io/ros/v/noetic/wrapyfi_ros_interfaces)](https://index.ros.org/r/wrapyfi_ros_interfaces/#noetic)
 
 * For installing ROS 2, follow the ROS 2 installation guide [\[Ubuntu\]](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html)[\[Windows\]](https://docs.ros.org/en/humble/Installation/Windows-Install-Binary.html). 
 We recommend installing ROS 2 on Conda using the [RoboStack](https://github.com/RoboStack/ros-humble) environment. Additionally, the 
 [Wrapyfi ROS 2 interfaces](https://github.com/modular-ml/wrapyfi_ros2_interfaces/blob/master/README.md?rank=0) 
-must be built to support messages and services needed for audio transmission and the REQ/REP pattern support [![ROS Package Index](https://img.shields.io/ros/v/humble/wrapyfi_ros2_interfaces)](https://index.ros.org/p/wrapyfi_ros2_interfaces/#humble)
+must be built to support messages and services needed for audio transmission and the REQ/REP pattern [![ROS Package Index](https://img.shields.io/ros/v/humble/wrapyfi_ros2_interfaces)](https://index.ros.org/p/wrapyfi_ros2_interfaces/#humble)
 
 * ZeroMQ can be installed using pip: `pip install pyzmq`. 
 The xpub-xsub pattern followed in our ZeroMQ implementation requires a proxy broker. A broker is spawned by default as a daemon process.
 To avoid automatic spawning, pass the argument `start_proxy_broker=False` to the method register decorator. 
 A standalone broker can be found [here](https://github.com/fabawi/wrapyfi/tree/main/wrapyfi/standalone/zeromq_proxy_broker.py)
```

### Comparing `wrapyfi-0.4.43/examples/README.md` & `wrapyfi-0.4.44/examples/README.md`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/applications/affective_signaling_multirobot.py` & `wrapyfi-0.4.44/examples/applications/affective_signaling_multirobot.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/applications/gaze_mirroring_multisensor.py` & `wrapyfi-0.4.44/examples/applications/gaze_mirroring_multisensor.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/communication_patterns/request_reply_example.py` & `wrapyfi-0.4.44/examples/communication_patterns/request_reply_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/communication_schemes/channeling_example.py` & `wrapyfi-0.4.44/examples/communication_schemes/channeling_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/communication_schemes/forwarding_example.py` & `wrapyfi-0.4.44/examples/communication_schemes/forwarding_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/communication_schemes/mirroring_example.py` & `wrapyfi-0.4.44/examples/communication_schemes/mirroring_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/custom_msgs/ros2_message_example.py` & `wrapyfi-0.4.44/examples/custom_msgs/ros2_message_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/custom_msgs/ros_message_example.py` & `wrapyfi-0.4.44/examples/custom_msgs/ros_message_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/custom_msgs/ros_parameter_example.py` & `wrapyfi-0.4.44/examples/custom_msgs/ros_parameter_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/astropy_example.py` & `wrapyfi-0.4.44/examples/encoders/astropy_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/cupy_example.py` & `wrapyfi-0.4.44/examples/encoders/cupy_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/dask_example.py` & `wrapyfi-0.4.44/examples/encoders/dask_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/jax_example.py` & `wrapyfi-0.4.44/examples/encoders/jax_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/mxnet_example.py` & `wrapyfi-0.4.44/examples/encoders/mxnet_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/numpy_pandas_example.py` & `wrapyfi-0.4.44/examples/encoders/numpy_pandas_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/paddlepaddle_example.py` & `wrapyfi-0.4.44/examples/encoders/paddlepaddle_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/pillow_example.py` & `wrapyfi-0.4.44/examples/encoders/pillow_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/pint_example.py` & `wrapyfi-0.4.44/examples/encoders/pint_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/plugins/astropy_tables.py` & `wrapyfi-0.4.44/examples/encoders/plugins/astropy_tables.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/pyarrow_example.py` & `wrapyfi-0.4.44/examples/encoders/pyarrow_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/pytorch_example.py` & `wrapyfi-0.4.44/examples/encoders/pytorch_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/tensorflow_example.py` & `wrapyfi-0.4.44/examples/encoders/tensorflow_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/trax_example.py` & `wrapyfi-0.4.44/examples/encoders/trax_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/xarray_example.py` & `wrapyfi-0.4.44/examples/encoders/xarray_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/encoders/zarr_example.py` & `wrapyfi-0.4.44/examples/encoders/zarr_example.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/hello_world.py` & `wrapyfi-0.4.44/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/requirements.txt` & `wrapyfi-0.4.44/examples/requirements.txt`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/robots/icub_head.py` & `wrapyfi-0.4.44/examples/robots/icub_head.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/examples/sensors/cam_mic.py` & `wrapyfi-0.4.44/examples/sensors/cam_mic.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/pyproject.toml` & `wrapyfi-0.4.44/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wrapyfi"
-version = "0.4.43"
+version = "0.4.44"
 description = "Wrapyfi is a wrapper for simplifying Middleware communication"
 readme = "README.md"
 authors = [
     { name = "Fares Abawi", email = "f.abawi@outlook.com" },
 ]
 maintainers = [
     { name = "Fares Abawi", email = "f.abawi@outlook.com" },
@@ -65,8 +65,8 @@
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
-[tool]
+[tool.pdm]
```

### Comparing `wrapyfi-0.4.43/wrapyfi/__init__.py` & `wrapyfi-0.4.44/wrapyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/clients/__init__.py` & `wrapyfi-0.4.44/wrapyfi/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/clients/ros.py` & `wrapyfi-0.4.44/wrapyfi/clients/ros.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/clients/ros2.py` & `wrapyfi-0.4.44/wrapyfi/clients/ros2.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/clients/yarp.py` & `wrapyfi-0.4.44/wrapyfi/clients/yarp.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/clients/zeromq.py` & `wrapyfi-0.4.44/wrapyfi/clients/zeromq.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/config/manager.py` & `wrapyfi-0.4.44/wrapyfi/config/manager.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/connect/clients.py` & `wrapyfi-0.4.44/wrapyfi/connect/clients.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/connect/listeners.py` & `wrapyfi-0.4.44/wrapyfi/connect/listeners.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/connect/publishers.py` & `wrapyfi-0.4.44/wrapyfi/connect/publishers.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/connect/servers.py` & `wrapyfi-0.4.44/wrapyfi/connect/servers.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/connect/wrapper.py` & `wrapyfi-0.4.44/wrapyfi/connect/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,24 +29,22 @@
                 self.activate_communication(getattr(self.__class__, key), mode=value)
 
     @classmethod
     def __trigger_publish(
         cls, func: Callable[..., Any], instance_id: str, kwd: dict, *wds, **kwds
     ):
         """
-        Triggers the publish mode of the middleware communicator.
+        Triggers the publish mode of the middleware communicator. If the intended publisher type and middleware are unavailable, resorts to a fallback publisher instead.
 
         :param func: Callable[..., Any]: The function to be triggered and whose return values are to be published
         :param instance_id: str: The unique identifier of the function instance, utilized to access the middleware communicator registry and manage different instances of communications
         :param kwd: dict: A dictionary containing keyword arguments to be matched and potentially utilized during the publisher instantiation and function invocation
         :param wds: tuple: Variable positional arguments to be passed to the function
         :param kwds: dict: Additional keyword arguments to be passed to the function
         :return: Any: The return values of the triggered function (`func`). The data type and structure depend on the output of `func`
-
-        :raises: KeyError: If the intended publisher type and middleware are unavailable, resorting to a fallback publisher
         """
         if (
             "wrapped_executor"
             not in cls._MiddlewareCommunicator__registry[
                 func.__qualname__ + instance_id
             ]["communicator"][0]
         ):
@@ -145,24 +143,22 @@
         return returns
 
     @classmethod
     def __trigger_listen(
         cls, func: Callable[..., Any], instance_id: str, kwd: dict, *wds, **kwds
     ):
         """
-        Triggers the listen mode of the middleware communicator.
+        Triggers the listen mode of the middleware communicator. If the intended listener type and middleware are unavailable, resorts to a fallback listener instead.
 
         :param func: Callable[..., Any]: The function associated with the listener and whose return values might be utilized
         :param instance_id: str: The unique identifier of the function instance, utilized to access the middleware communicator registry and manage different instances of communications
         :param kwd: dict: A dictionary containing keyword arguments to be matched and potentially utilized during the listener instantiation and function invocation
         :param wds: tuple: Variable positional arguments to be passed to the function
         :param kwds: dict: Additional keyword arguments to be passed to the function (not used since the listener does not accept any additional arguments, given that it does not execute any function or transmit any arguments)
         :return: Any: The return values obtained from the listeners. The data type and structure depend on the output of the listener
-
-        :raises: KeyError: If the intended listener type and middleware are unavailable, resorting to a fallback listener
         """
         if (
             "wrapped_executor"
             not in cls._MiddlewareCommunicator__registry[
                 func.__qualname__ + instance_id
             ]["communicator"][0]
         ):
@@ -270,24 +266,22 @@
         return returns
 
     @classmethod
     def __trigger_reply(
         cls, func: Callable[..., Any], instance_id: str, kwd, *wds, **kwds
     ):
         """
-        Triggers the reply mode of the middleware communicator.
+        Triggers the reply mode of the middleware communicator. If the intended server type and middleware are unavailable, resorts to a fallback server instead.
 
         :param func: Callable[..., Any]: The function to be triggered and whose return values may be used in replies
         :param instance_id: str: The unique identifier of the function instance, utilized to access the middleware communicator registry and manage different instances of communications
         :param kwd: dict: A dictionary containing keyword arguments to be matched and potentially utilized during the server instantiation and function invocation
         :param wds: tuple: Variable positional arguments to be passed to the function
         :param kwds: dict: Additional keyword arguments to be passed to the function
         :return: Any: The return values of the triggered function (`func`). The data type and structure depend on the output of `func`
-
-        :raises: KeyError: If the intended server type and middleware are unavailable, resorting to a fallback server
         """
         if (
             "wrapped_executor"
             not in cls._MiddlewareCommunicator__registry[
                 func.__qualname__ + instance_id
             ]["communicator"][0]
         ):
@@ -397,24 +391,22 @@
         return returns
 
     @classmethod
     def __trigger_request(
         cls, func: Callable[..., Any], instance_id: str, kwd, *wds, **kwds
     ):
         """
-        Triggers the request mode of the middleware communicator.
+        Triggers the request mode of the middleware communicator. If the intended client type and middleware are unavailable, resorts to a fallback client instead.
 
         :param func: Callable[..., Any]: The function associated with the client requests and might utilize the request results
         :param instance_id: str: The unique identifier of the function instance, utilized to access the middleware communicator registry and manage different instances of communications
         :param kwd: dict: A dictionary containing keyword arguments to be matched and potentially utilized during the client instantiation and function invocation
         :param wds: tuple: Variable positional arguments to be passed to the function
         :param kwds: dict: Additional keyword arguments to be passed to the function
         :return: Any: The return values obtained from the clients' requests. The data type and structure depend on the output of the client requests
-
-        :raises: KeyError: If the intended client type and middleware are unavailable, resorting to a fallback client
         """
         if (
             "wrapped_executor"
             not in cls._MiddlewareCommunicator__registry[
                 func.__qualname__ + instance_id
             ]["communicator"][0]
         ):
@@ -773,21 +765,20 @@
             close_instance_idxs.add(instance_addr) if instance_addr else None
         for close_instance_idx in close_instance_idxs:
             cls.close_instance(close_instance_idx)
 
     @classmethod
     def close_instance(cls, instance_addr: Optional[str] = None):
         """
-        Closes a specific instance of the middleware communicator.
+        Closes a specific instance of the middleware communicator. Note that the instance address is the hexadecimal
+        representation of the instance's id. If no instance address is provided, all instances will be closed.
 
         :param instance_addr: str: The unique identifier of the instance to be closed, defaults to None
 
         :raises: ValueError: If the instance address cannot be found in the registry
-
-        Note that the instance address is the hex representation of the instance's id. If no instance address is provided, all instances will be closed.
         """
         while True:
             del_entry = False
             del_entry_name = None
             del_entry_idx = None
             other_entry_keys = []
             # find self in registry and remove id from instances
```

### Comparing `wrapyfi-0.4.43/wrapyfi/encoders.py` & `wrapyfi-0.4.44/wrapyfi/encoders.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/listeners/__init__.py` & `wrapyfi-0.4.44/wrapyfi/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/listeners/ros.py` & `wrapyfi-0.4.44/wrapyfi/listeners/ros.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/listeners/ros2.py` & `wrapyfi-0.4.44/wrapyfi/listeners/ros2.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/listeners/yarp.py` & `wrapyfi-0.4.44/wrapyfi/listeners/yarp.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/listeners/zeromq.py` & `wrapyfi-0.4.44/wrapyfi/listeners/zeromq.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/middlewares/ros.py` & `wrapyfi-0.4.44/wrapyfi/middlewares/ros.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/middlewares/ros2.py` & `wrapyfi-0.4.44/wrapyfi/middlewares/ros2.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/middlewares/yarp.py` & `wrapyfi-0.4.44/wrapyfi/middlewares/yarp.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/middlewares/zeromq.py` & `wrapyfi-0.4.44/wrapyfi/middlewares/zeromq.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/cupy_array.py` & `wrapyfi-0.4.44/wrapyfi/plugins/cupy_array.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/dask_data.py` & `wrapyfi-0.4.44/wrapyfi/plugins/dask_data.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/jax_tensor.py` & `wrapyfi-0.4.44/wrapyfi/plugins/jax_tensor.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/mxnet_tensor.py` & `wrapyfi-0.4.44/wrapyfi/plugins/mxnet_tensor.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/paddle_tensor.py` & `wrapyfi-0.4.44/wrapyfi/plugins/paddle_tensor.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/pandas_data.py` & `wrapyfi-0.4.44/wrapyfi/plugins/pandas_data.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/pillow_image.py` & `wrapyfi-0.4.44/wrapyfi/plugins/pillow_image.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/pint_quantities.py` & `wrapyfi-0.4.44/wrapyfi/plugins/pint_quantities.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/pyarrow_array.py` & `wrapyfi-0.4.44/wrapyfi/plugins/pyarrow_array.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/pytorch_tensor.py` & `wrapyfi-0.4.44/wrapyfi/plugins/pytorch_tensor.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/tensorflow_tensor.py` & `wrapyfi-0.4.44/wrapyfi/plugins/tensorflow_tensor.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/trax_array.py` & `wrapyfi-0.4.44/wrapyfi/plugins/trax_array.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/xarray_data.py` & `wrapyfi-0.4.44/wrapyfi/plugins/xarray_data.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/plugins/zarr_array.py` & `wrapyfi-0.4.44/wrapyfi/plugins/zarr_array.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/publishers/__init__.py` & `wrapyfi-0.4.44/wrapyfi/publishers/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/publishers/ros.py` & `wrapyfi-0.4.44/wrapyfi/publishers/ros.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/publishers/ros2.py` & `wrapyfi-0.4.44/wrapyfi/publishers/ros2.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/publishers/yarp.py` & `wrapyfi-0.4.44/wrapyfi/publishers/yarp.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/publishers/zeromq.py` & `wrapyfi-0.4.44/wrapyfi/publishers/zeromq.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import json
 import time
 import os
+import threading
 import base64
 import io
 from typing import Optional, Tuple
 
 import numpy as np
 import cv2
 import zmq
@@ -162,32 +163,36 @@
 
     def __init__(
         self,
         name: str,
         out_topic: str,
         carrier: str = "tcp",
         should_wait: bool = True,
+        multi_threaded: bool = False,
         serializer_kwargs: Optional[dict] = None,
         **kwargs,
     ):
         """
         The NativeObjectPublisher using the ZeroMQ message construct assuming a combination of python native objects
         and numpy arrays as input. Serializes the data (including plugins) using the encoder and sends it as a string.
 
         :param name: str: Name of the publisher
         :param out_topic: str: Name of the output topic preceded by '/' (e.g. '/topic')
         :param carrier: str: Carrier protocol. ZeroMQ currently only supports TCP for PUB/SUB pattern. Default is 'tcp'
         :param should_wait: bool: Whether to wait for at least one listener before unblocking the script. Default is True
+        :param multi_threaded: bool: Whether to use a separate socket for each thread. Default is False
         :param serializer_kwargs: dict: Additional kwargs for the serializer
         :param kwargs: dict: Additional kwargs for the publisher
         """
         super().__init__(
             name, out_topic, carrier=carrier, should_wait=should_wait, **kwargs
         )
         self._socket = self._netconnect = None
+        if multi_threaded:
+            self._thread_local_storage = threading.local()
 
         self._plugin_encoder = JsonEncoder
         self._plugin_kwargs = kwargs
         self._serializer_kwargs = serializer_kwargs or {}
 
         if not self.should_wait:
             PublisherWatchDog().add_publisher(self)
@@ -210,14 +215,33 @@
                     getattr(zmq, socket_property[0]), socket_property[1]
                 )
         self._socket.connect(self.socket_sub_address)
         self._topic = self.out_topic.encode()
         established = self.await_connection(repeats=repeats)
         return self.check_establishment(established)
 
+    def _get_socket(self):
+        """
+        Retrieve or create a ZeroMQ socket specific to the current thread.
+        """
+        if not hasattr(self._thread_local_storage, "socket"):
+            # Initialize a new socket for the thread
+            self._thread_local_storage.socket = zmq.Context.instance().socket(zmq.PUB)
+            for socket_property in ZeroMQMiddlewarePubSub().zeromq_kwargs.items():
+                if isinstance(socket_property[1], str):
+                    self._thread_local_storage.socket.setsockopt_string(
+                        getattr(zmq, socket_property[0]), socket_property[1]
+                    )
+                else:
+                    self._thread_local_storage.socket.setsockopt(
+                        getattr(zmq, socket_property[0]), socket_property[1]
+                    )
+            self._thread_local_storage.socket.connect(self.socket_sub_address)
+        return self._thread_local_storage.socket
+
     def publish(self, obj):
         """
         Publish the object to the middleware.
 
         :param obj: object: Object to publish
         """
         if not self.established:
@@ -228,40 +252,46 @@
                 time.sleep(0.2)
         obj_str = json.dumps(
             obj,
             cls=self._plugin_encoder,
             **self._plugin_kwargs,
             serializer_kwrags=self._serializer_kwargs,
         )
-        self._socket.send_multipart([self._topic, obj_str.encode()])
+        if hasattr(self, "_thread_local_storage"):
+            socket = self._get_socket()
+        else:
+            socket = self._socket
+        socket.send_multipart([self._topic, obj_str.encode()])
 
 
 @Publishers.register("Image", "zeromq")
 class ZeroMQImagePublisher(ZeroMQNativeObjectPublisher):
 
     def __init__(
         self,
         name: str,
         out_topic: str,
         carrier: str = "tcp",
         should_wait: bool = True,
+        multi_threaded: bool = False,
         width: int = -1,
         height: int = -1,
         rgb: bool = True,
         fp: bool = False,
         jpg: bool = False,
         **kwargs,
     ):
         """
         The ImagePublisher using the ZeroMQ message construct assuming a numpy array as input.
 
         :param name: str: Name of the publisher
         :param out_topic: str: Name of the output topic preceded by '/' (e.g. '/topic')
         :param carrier: str: Carrier protocol. ZeroMQ currently only supports TCP for PUB/SUB pattern. Default is 'tcp'
         :param should_wait: bool: Whether to wait for at least one listener before unblocking the script. Default is True
+        :param multi_threaded: bool: Whether to use a separate socket for each thread. Default is False
         :param width: int: Width of the image. Default is -1 meaning that the width is not fixed
         :param height: int: Height of the image. Default is -1 meaning that the height is not fixed
         :param rgb: bool: True if the image is RGB, False if it is grayscale. Default is True
         :param fp: bool: True if the image is floating point, False if it is integer. Default is False
         :param jpg: bool: True if the image should be compressed as JPG. Default is False
         """
         super().__init__(
@@ -308,46 +338,53 @@
             img_str = json.dumps(
                 img,
                 cls=self._plugin_encoder,
                 **self._plugin_kwargs,
                 serializer_kwrags=self._serializer_kwargs,
             ).encode()
         img_header = "{timestamp:" + str(time.time()) + "}"
-        self._socket.send_multipart([self._topic, img_header.encode(), img_str])
+        if hasattr(self, "_thread_local_storage"):
+            socket = self._get_socket()
+        else:
+            socket = self._socket
+        socket.send_multipart([self._topic, img_header.encode(), img_str])
 
 
 @Publishers.register("AudioChunk", "zeromq")
 class ZeroMQAudioChunkPublisher(ZeroMQNativeObjectPublisher):
     def __init__(
         self,
         name: str,
         out_topic: str,
         carrier: str = "tcp",
         should_wait: bool = True,
+        multi_threaded: bool = False,
         channels: int = 1,
         rate: int = 44100,
         chunk: int = -1,
         **kwargs,
     ):
         """
         The AudioChunkPublisher using the ZeroMQ message construct assuming a numpy array as input.
 
         :param name: str: Name of the publisher
         :param out_topic: str: Name of the output topic preceded by '/' (e.g. '/topic')
         :param carrier: str: Carrier protocol. ZeroMQ currently only supports TCP for PUB/SUB pattern. Default is 'tcp'
         :param should_wait: bool: Whether to wait for at least one listener before unblocking the script. Default is True
+        :param multi_threaded: bool: Whether to use a separate socket for each thread. Default is False
         :param channels: int: Number of channels. Default is 1
         :param rate: int: Sampling rate. Default is 44100
         :param chunk: int: Chunk size. Default is -1 meaning that the chunk size is not fixed
         """
         super().__init__(
             name,
             out_topic,
             carrier=carrier,
             should_wait=should_wait,
+            multi_threaded=multi_threaded,
             width=chunk,
             height=channels,
             rgb=False,
             fp=True,
             jpg=False,
             **kwargs,
         )
@@ -383,15 +420,19 @@
         aud_str = json.dumps(
             (chunk, channels, rate, aud),
             cls=self._plugin_encoder,
             **self._plugin_kwargs,
             serializer_kwrags=self._serializer_kwargs,
         ).encode()
         aud_header = "{timestamp:" + str(time.time()) + "}"
-        self._socket.send_multipart([self._topic, aud_header.encode(), aud_str])
+        if hasattr(self, "_thread_local_storage"):
+            socket = self._get_socket()
+        else:
+            socket = self._socket
+        socket.send_multipart([self._topic, aud_header.encode(), aud_str])
 
 
 @Publishers.register("Properties", "zeromq")
 class ZeroMQPropertiesPublisher(ZeroMQPublisher):
 
     def __init__(self, name, out_topic, **kwargs):
         super().__init__(name, out_topic, **kwargs)
```

### Comparing `wrapyfi-0.4.43/wrapyfi/servers/__init__.py` & `wrapyfi-0.4.44/wrapyfi/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/servers/ros.py` & `wrapyfi-0.4.44/wrapyfi/servers/ros.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/servers/ros2.py` & `wrapyfi-0.4.44/wrapyfi/servers/ros2.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/servers/yarp.py` & `wrapyfi-0.4.44/wrapyfi/servers/yarp.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/servers/zeromq.py` & `wrapyfi-0.4.44/wrapyfi/servers/zeromq.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/standalone/zeromq_param_server.py` & `wrapyfi-0.4.44/wrapyfi/standalone/zeromq_param_server.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/standalone/zeromq_proxy_broker.py` & `wrapyfi-0.4.44/wrapyfi/standalone/zeromq_proxy_broker.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/standalone/zeromq_pubsub_topic_monitor.py` & `wrapyfi-0.4.44/wrapyfi/standalone/zeromq_pubsub_topic_monitor.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/test_middleware.py` & `wrapyfi-0.4.44/wrapyfi/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/test_wrapper.py` & `wrapyfi-0.4.44/wrapyfi/tests/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/benchmarking_native_object.py` & `wrapyfi-0.4.44/wrapyfi/tests/tools/benchmarking_native_object.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/benchmarking_plotter.ipynb` & `wrapyfi-0.4.44/wrapyfi/tests/tools/benchmarking_plotter.ipynb`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/class_test.py` & `wrapyfi-0.4.44/wrapyfi/tests/tools/class_test.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros2.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros2.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros2__no-warmup.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_ros2__no-warmup.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_yarp.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_yarp.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_yarp_ros_zeromq__no-warmup.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_yarp_ros_zeromq__no-warmup.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_zeromq.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_listen_zeromq.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros2.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros2.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros2__no-warmup.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_ros2__no-warmup.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_yarp.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_yarp.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_yarp_ros_zeromq__no-warmup.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_yarp_ros_zeromq__no-warmup.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_zeromq.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/05_10_22_SHOULD_WAIT-TRUE/benchmarking_native_object_publish_zeromq.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/benchmarking_native_object_listen__ros,yarp,zeromq.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/benchmarking_native_object_listen__ros,yarp,zeromq.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/benchmarking_native_object_listen__ros2.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/benchmarking_native_object_listen__ros2.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/benchmarking_native_object_publish__ros,yarp,zeromq.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/benchmarking_native_object_publish__ros,yarp,zeromq.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/tests/tools/results/benchmarking_native_object_publish__ros2.csv` & `wrapyfi-0.4.44/wrapyfi/tests/tools/results/benchmarking_native_object_publish__ros2.csv`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/wrapyfi/utils.py` & `wrapyfi-0.4.44/wrapyfi/utils.py`

 * *Files identical despite different names*

### Comparing `wrapyfi-0.4.43/PKG-INFO` & `wrapyfi-0.4.44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapyfi
-Version: 0.4.43
+Version: 0.4.44
 Summary: Wrapyfi is a wrapper for simplifying Middleware communication
 Author-Email: Fares Abawi <f.abawi@outlook.com>
 Maintainer-Email: Fares Abawi <f.abawi@outlook.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -90,39 +90,39 @@
 
 Please refer to the following [paper](https://www2.informatik.uni-hamburg.de/wtm/publications/2024/AAFW24/Abawi_HRI24.pdf) when citing Wrapyfi in academic work:
 
 ```
 @inproceedings{abawi2024wrapyfi,
   title = {Wrapyfi: A Python Wrapper for Integrating Robots, Sensors, and Applications across Multiple Middleware},
   author = {Abawi, Fares and Allgeuer, Philipp and Fu, Di and Wermter, Stefan},
-  booktitle = {Proceedings of the ACM/IEEE Conference on Human-Robot Interaction (HRI '24)},
+  booktitle = {Proceedings of the ACM/IEEE International Conference on Human-Robot Interaction (HRI '24)},
   year = {2024},
   organization = {ACM},
   isbn = {79-8-4007-0322-5},
   doi = {10.1145/3610977.3637471},
   url = {https://github.com/fabawi/wrapyfi}
 }
 ```
 
 # Getting Started
 
 Before using Wrapyfi, YARP, ROS, or ZeroMQ must be installed.
 
 * Follow the [YARP installation guide](https://github.com/fabawi/wrapyfi/tree/main/wrapyfi_extensions/yarp/README.md?rank=0).<!-- [YARP installation guide](docs/yarp_install_lnk.md). -->
-Note that the iCub package is not needed for Wrapyfi to work and does not have to be installed if you do not intend on using the iCub robot.
+Note that the iCub package is not needed for Wrapyfi to work and does not have to be installed if you do not intend to use the iCub robot.
 
 * For installing ROS, follow the ROS installation guide [\[Ubuntu\]](http://wiki.ros.org/noetic/Installation/Ubuntu)[\[Windows\]](https://wiki.ros.org/noetic/Installation/Windows). 
 We recommend installing ROS on Conda using the [RoboStack](https://github.com/RoboStack/ros-noetic) environment. Additionally, the 
 [Wrapyfi ROS interfaces](https://github.com/modular-ml/wrapyfi_ros_interfaces/blob/master/README.md?rank=0) must be
 built to support messages needed for audio transmission [![ROS Package Index](https://img.shields.io/ros/v/noetic/wrapyfi_ros_interfaces)](https://index.ros.org/r/wrapyfi_ros_interfaces/#noetic)
 
 * For installing ROS 2, follow the ROS 2 installation guide [\[Ubuntu\]](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html)[\[Windows\]](https://docs.ros.org/en/humble/Installation/Windows-Install-Binary.html). 
 We recommend installing ROS 2 on Conda using the [RoboStack](https://github.com/RoboStack/ros-humble) environment. Additionally, the 
 [Wrapyfi ROS 2 interfaces](https://github.com/modular-ml/wrapyfi_ros2_interfaces/blob/master/README.md?rank=0) 
-must be built to support messages and services needed for audio transmission and the REQ/REP pattern support [![ROS Package Index](https://img.shields.io/ros/v/humble/wrapyfi_ros2_interfaces)](https://index.ros.org/p/wrapyfi_ros2_interfaces/#humble)
+must be built to support messages and services needed for audio transmission and the REQ/REP pattern [![ROS Package Index](https://img.shields.io/ros/v/humble/wrapyfi_ros2_interfaces)](https://index.ros.org/p/wrapyfi_ros2_interfaces/#humble)
 
 * ZeroMQ can be installed using pip: `pip install pyzmq`. 
 The xpub-xsub pattern followed in our ZeroMQ implementation requires a proxy broker. A broker is spawned by default as a daemon process.
 To avoid automatic spawning, pass the argument `start_proxy_broker=False` to the method register decorator. 
 A standalone broker can be found [here](https://github.com/fabawi/wrapyfi/tree/main/wrapyfi/standalone/zeromq_proxy_broker.py)
```

