# Comparing `tmp/qwak_core-0.3.99.tar.gz` & `tmp/qwak_core-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.3.99.tar", max compression
+gzip compressed data, was "qwak_core-0.4.0.tar", max compression
```

## Comparing `qwak_core-0.3.99.tar` & `qwak_core-0.4.0.tar`

### file list

```diff
@@ -1,810 +1,818 @@
--rw-r--r--   0        0        0      264 2024-02-26 14:58:48.575938 qwak_core-0.3.99/README.md
--rw-r--r--   0        0        0        0 2024-02-26 15:00:33.921999 qwak_core-0.3.99/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5877 2024-02-26 15:00:33.942000 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     7824 2024-02-26 15:00:13.689602 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.942000 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0    12703 2024-02-26 15:00:33.942000 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py
--rw-r--r--   0        0        0    10914 2024-02-26 15:00:13.829605 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi
--rw-r--r--   0        0        0    14681 2024-02-26 15:00:33.942000 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2024-02-26 15:00:33.938000 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2024-02-26 15:00:13.409597 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.938000 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2024-02-26 15:00:33.938000 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2024-02-26 15:00:13.549600 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.938000 qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2024-02-26 15:00:33.934000 qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2024-02-26 15:00:12.989589 qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2024-02-26 15:00:33.934000 qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2024-02-26 15:00:33.934000 qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2024-02-26 15:00:13.125591 qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.934000 qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2024-02-26 15:00:33.934000 qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2024-02-26 15:00:13.269594 qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.938000 qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2024-02-26 15:00:33.921999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2024-02-26 15:00:12.845586 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2024-02-26 15:00:33.921999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     7360 2024-02-26 15:00:33.921999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0    11651 2024-02-26 15:00:13.973608 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.921999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2024-02-26 15:00:33.925999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2024-02-26 15:00:14.257614 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.925999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2024-02-26 15:00:33.929999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2024-02-26 15:00:14.401616 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2024-02-26 15:00:33.929999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2024-02-26 15:00:33.925999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2024-02-26 15:00:14.117611 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.925999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6541 2024-02-26 15:00:33.929999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10595 2024-02-26 15:00:14.541619 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.929999 qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0    15382 2024-02-26 15:00:33.970000 qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    20668 2024-02-26 15:00:16.537658 qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.970000 qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2024-02-26 15:00:33.970000 qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2024-02-26 15:00:16.681661 qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2024-02-26 15:00:33.970000 qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7405 2024-02-26 15:00:34.090003 qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11995 2024-02-26 15:00:23.497795 qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.094003 qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0    13411 2024-02-26 15:00:34.094003 qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0    11116 2024-02-26 15:00:23.641798 qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    17346 2024-02-26 15:00:34.094003 qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2024-02-26 15:00:34.098003 qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2024-02-26 15:00:24.505815 qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2024-02-26 15:00:34.098003 qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8864 2024-02-26 15:00:34.094003 qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13789 2024-02-26 15:00:24.361812 qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.098003 qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2024-02-26 15:00:34.098003 qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2024-02-26 15:00:24.645817 qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.098003 qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2024-02-26 15:00:34.102003 qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2024-02-26 15:00:24.785820 qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2024-02-26 15:00:34.102003 qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    14053 2024-02-26 15:00:34.178004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    20860 2024-02-26 15:00:31.349949 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.182005 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2024-02-26 15:00:34.178004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2024-02-26 15:00:31.061943 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.178004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3954 2024-02-26 15:00:34.178004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     5309 2024-02-26 15:00:31.201946 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.178004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    21176 2024-02-26 15:00:34.174004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    15049 2024-02-26 15:00:30.773938 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    25475 2024-02-26 15:00:34.174004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2024-02-26 15:00:34.174004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2024-02-26 15:00:30.921940 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.174004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2024-02-26 15:00:34.186004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2024-02-26 15:00:31.773957 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.186004 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2024-02-26 15:00:34.182005 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2024-02-26 15:00:31.633955 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.182005 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2024-02-26 15:00:34.182005 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2024-02-26 15:00:31.489952 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.182005 qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2024-02-26 15:00:34.170004 qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    15333 2024-02-26 15:00:30.621935 qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.170004 qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2083 2024-02-26 15:00:34.166004 qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1977 2024-02-26 15:00:30.325929 qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.170004 qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    45969 2024-02-26 15:00:34.170004 qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    59718 2024-02-26 15:00:30.477932 qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    32008 2024-02-26 15:00:34.170004 qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    29124 2024-02-26 15:00:34.126003 qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    24434 2024-02-26 15:00:26.249849 qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    27837 2024-02-26 15:00:34.126003 qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    33162 2024-02-26 15:00:34.122003 qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    51725 2024-02-26 15:00:25.957843 qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.122003 qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0     5757 2024-02-26 15:00:34.126003 qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py
--rw-r--r--   0        0        0     4013 2024-02-26 15:00:26.677857 qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi
--rw-r--r--   0        0        0     6783 2024-02-26 15:00:34.130004 qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py
--rw-r--r--   0        0        0     6016 2024-02-26 15:00:34.126003 qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_pb2.py
--rw-r--r--   0        0        0     7049 2024-02-26 15:00:26.533854 qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.126003 qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_pb2_grpc.py
--rw-r--r--   0        0        0    14412 2024-02-26 15:00:34.114003 qwak_core-0.3.99/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    22691 2024-02-26 15:00:25.809840 qwak_core-0.3.99/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.114003 qwak_core-0.3.99/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     5552 2024-02-26 15:00:34.114003 qwak_core-0.3.99/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     7299 2024-02-26 15:00:26.101846 qwak_core-0.3.99/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.118003 qwak_core-0.3.99/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    15672 2024-02-26 15:00:34.118003 qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0    12741 2024-02-26 15:00:26.393852 qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    16925 2024-02-26 15:00:34.118003 qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38431 2024-02-26 15:00:34.122003 qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    53202 2024-02-26 15:00:27.133866 qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2024-02-26 15:00:34.122003 qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     3508 2024-02-26 15:00:34.118003 qwak_core-0.3.99/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     2300 2024-02-26 15:00:26.821860 qwak_core-0.3.99/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0     3101 2024-02-26 15:00:34.118003 qwak_core-0.3.99/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0     2270 2024-02-26 15:00:34.134003 qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     2697 2024-02-26 15:00:27.433872 qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.134003 qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4458 2024-02-26 15:00:34.134003 qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     3113 2024-02-26 15:00:27.577875 qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2024-02-26 15:00:34.138004 qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2024-02-26 15:00:34.110003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2024-02-26 15:00:25.377832 qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.110003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11871 2024-02-26 15:00:34.110003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     8790 2024-02-26 15:00:25.521834 qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2024-02-26 15:00:34.110003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2024-02-26 15:00:34.106003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2024-02-26 15:00:25.081826 qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.106003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    49923 2024-02-26 15:00:34.102003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    73782 2024-02-26 15:00:24.937823 qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.102003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    46309 2024-02-26 15:00:34.106003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    40356 2024-02-26 15:00:25.237829 qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    27756 2024-02-26 15:00:34.106003 qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     3345 2024-02-26 15:00:33.958000 qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     4098 2024-02-26 15:00:15.825644 qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.958000 qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12707 2024-02-26 15:00:33.962000 qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    13800 2024-02-26 15:00:15.969647 qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.962000 qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    17949 2024-02-26 15:00:33.962000 qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    18562 2024-02-26 15:00:16.113650 qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    12833 2024-02-26 15:00:33.962000 qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     6463 2024-02-26 15:00:34.062002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/backfill_pb2.py
--rw-r--r--   0        0        0     7945 2024-02-26 15:00:20.309732 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.062002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/backfill_pb2_grpc.py
--rw-r--r--   0        0        0     2971 2024-02-26 15:00:34.062002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/batch_pb2.py
--rw-r--r--   0        0        0     3266 2024-02-26 15:00:20.453735 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.062002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5530 2024-02-26 15:00:34.066002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/execution_pb2.py
--rw-r--r--   0        0        0     6938 2024-02-26 15:00:20.597738 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.066002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/execution_pb2_grpc.py
--rw-r--r--   0        0        0     9463 2024-02-26 15:00:34.066002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/execution_service_pb2.py
--rw-r--r--   0        0        0     6365 2024-02-26 15:00:20.741741 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi
--rw-r--r--   0        0        0    11016 2024-02-26 15:00:34.066002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py
--rw-r--r--   0        0        0     7695 2024-02-26 15:00:34.070002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py
--rw-r--r--   0        0        0    14959 2024-02-26 15:00:21.037747 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.070002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0    13820 2024-02-26 15:00:34.070002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py
--rw-r--r--   0        0        0    11303 2024-02-26 15:00:21.181749 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    15043 2024-02-26 15:00:34.074002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     8440 2024-02-26 15:00:34.070002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py
--rw-r--r--   0        0        0    13312 2024-02-26 15:00:20.885744 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.070002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     2051 2024-02-26 15:00:34.074002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py
--rw-r--r--   0        0        0     1952 2024-02-26 15:00:21.337752 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.074002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_pb2_grpc.py
--rw-r--r--   0        0        0    12222 2024-02-26 15:00:34.074002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py
--rw-r--r--   0        0        0     7930 2024-02-26 15:00:21.485755 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi
--rw-r--r--   0        0        0    14212 2024-02-26 15:00:34.078003 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py
--rw-r--r--   0        0        0     1685 2024-02-26 15:00:34.078003 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py
--rw-r--r--   0        0        0     1272 2024-02-26 15:00:21.625758 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.078003 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2_grpc.py
--rw-r--r--   0        0        0     6198 2024-02-26 15:00:34.078003 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py
--rw-r--r--   0        0        0     7677 2024-02-26 15:00:21.765761 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.082002 qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2024-02-26 15:00:34.042002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2024-02-26 15:00:20.161729 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.042002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2024-02-26 15:00:34.042002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2024-02-26 15:00:20.021727 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2024-02-26 15:00:34.042002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2024-02-26 15:00:34.022001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2024-02-26 15:00:18.429695 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.022001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0    13825 2024-02-26 15:00:34.030001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_pb2.py
--rw-r--r--   0        0        0    19227 2024-02-26 15:00:19.137709 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.030001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3307 2024-02-26 15:00:34.030001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py
--rw-r--r--   0        0        0     1637 2024-02-26 15:00:19.281712 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3293 2024-02-26 15:00:34.034002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2024-02-26 15:00:34.018001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2024-02-26 15:00:18.285693 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.022001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2024-02-26 15:00:34.014001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2024-02-26 15:00:17.841684 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.014001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2024-02-26 15:00:34.018001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2024-02-26 15:00:18.145690 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2024-02-26 15:00:34.018001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2024-02-26 15:00:34.022001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2024-02-26 15:00:18.569698 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.022001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2024-02-26 15:00:34.026002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2024-02-26 15:00:18.713701 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2024-02-26 15:00:34.026002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    26853 2024-02-26 15:00:34.014001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    39247 2024-02-26 15:00:17.993687 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.018001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2024-02-26 15:00:34.026002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2024-02-26 15:00:18.853704 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.026002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    13240 2024-02-26 15:00:34.030001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    18420 2024-02-26 15:00:18.993707 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.030001 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2024-02-26 15:00:34.046002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2024-02-26 15:00:33.193985 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.046002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2024-02-26 15:00:34.046002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2024-02-26 15:00:33.337988 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2024-02-26 15:00:34.046002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     4308 2024-02-26 15:00:34.050002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     7410 2024-02-26 15:00:23.069786 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.050002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    15316 2024-02-26 15:00:34.050002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    14087 2024-02-26 15:00:23.217789 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    18465 2024-02-26 15:00:34.050002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2024-02-26 15:00:34.054002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2024-02-26 15:00:23.357792 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.054002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     5111 2024-02-26 15:00:34.058002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/management_pb2.py
--rw-r--r--   0        0        0     2739 2024-02-26 15:00:24.217809 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi
--rw-r--r--   0        0        0     5436 2024-02-26 15:00:34.062002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py
--rw-r--r--   0        0        0     5385 2024-02-26 15:00:34.054002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     7551 2024-02-26 15:00:23.929803 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.058002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    17474 2024-02-26 15:00:34.054002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2024-02-26 15:00:23.785801 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2024-02-26 15:00:34.054002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2024-02-26 15:00:34.058002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2024-02-26 15:00:24.069806 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.058002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    26604 2024-02-26 15:00:34.034002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    42530 2024-02-26 15:00:19.425715 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.034002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5147 2024-02-26 15:00:34.034002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6208 2024-02-26 15:00:19.581718 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.038002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2024-02-26 15:00:34.038002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2024-02-26 15:00:19.729721 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2024-02-26 15:00:34.038002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11049 2024-02-26 15:00:34.038002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15942 2024-02-26 15:00:19.873724 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.038002 qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2024-02-26 15:00:34.190005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2024-02-26 15:00:32.337968 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.194005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2024-02-26 15:00:34.194005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2024-02-26 15:00:32.477971 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2024-02-26 15:00:34.194005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2024-02-26 15:00:34.194005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2024-02-26 15:00:32.621974 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.198005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2024-02-26 15:00:34.198005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2024-02-26 15:00:32.769977 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2024-02-26 15:00:34.198005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0    10469 2024-02-26 15:00:34.198005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0    11719 2024-02-26 15:00:32.913980 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     9458 2024-02-26 15:00:34.198005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     5302 2024-02-26 15:00:34.202005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     5484 2024-02-26 15:00:33.053982 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.202005 qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2975 2024-02-26 15:00:34.138004 qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     4026 2024-02-26 15:00:27.721878 qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.138004 qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4455 2024-02-26 15:00:34.138004 qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     3113 2024-02-26 15:00:27.861880 qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2024-02-26 15:00:34.138004 qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6489 2024-02-26 15:00:33.970000 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10455 2024-02-26 15:00:17.257672 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.982001 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     3383 2024-02-26 15:00:33.986001 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     5457 2024-02-26 15:00:17.397675 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.986001 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2024-02-26 15:00:33.998001 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2024-02-26 15:00:17.541678 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2024-02-26 15:00:33.998001 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8504 2024-02-26 15:00:33.998001 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12440 2024-02-26 15:00:17.685681 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.014001 qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2024-02-26 15:00:34.114003 qwak_core-0.3.99/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2024-02-26 15:00:25.661837 qwak_core-0.3.99/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2024-02-26 15:00:34.114003 qwak_core-0.3.99/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3792 2024-02-26 15:00:34.142004 qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4344 2024-02-26 15:00:28.005883 qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.142004 qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2024-02-26 15:00:34.142004 qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2024-02-26 15:00:28.145886 qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2024-02-26 15:00:34.142004 qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2024-02-26 15:00:34.150004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2024-02-26 15:00:29.017903 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.154004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2024-02-26 15:00:34.154004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2024-02-26 15:00:29.161906 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.154004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    24765 2024-02-26 15:00:34.154004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    30174 2024-02-26 15:00:29.305909 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.158004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13184 2024-02-26 15:00:34.158004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21824 2024-02-26 15:00:29.449912 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.158004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12784 2024-02-26 15:00:34.158004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16585 2024-02-26 15:00:29.597915 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.158004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    51171 2024-02-26 15:00:34.162004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    40800 2024-02-26 15:00:29.757918 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    73869 2024-02-26 15:00:34.162004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-02-26 15:00:34.162004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2024-02-26 15:00:29.901920 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.162004 qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2024-02-26 15:00:34.146004 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2024-02-26 15:00:28.433892 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.146004 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2024-02-26 15:00:34.150004 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2024-02-26 15:00:28.877900 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.150004 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2024-02-26 15:00:34.146004 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2024-02-26 15:00:28.593895 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2024-02-26 15:00:34.146004 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2024-02-26 15:00:34.150004 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2024-02-26 15:00:28.737898 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.150004 qwak_core-0.3.99/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    27866 2024-02-26 15:00:34.130004 qwak_core-0.3.99/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    32184 2024-02-26 15:00:27.289869 qwak_core-0.3.99/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    19830 2024-02-26 15:00:34.134003 qwak_core-0.3.99/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2024-02-26 15:00:33.954000 qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2024-02-26 15:00:16.969667 qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2024-02-26 15:00:33.954000 qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2024-02-26 15:00:33.954000 qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2024-02-26 15:00:16.825664 qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.954000 qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2024-02-26 15:00:33.958000 qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2024-02-26 15:00:17.113669 qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2024-02-26 15:00:33.958000 qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     1598 2024-02-26 15:00:34.186004 qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py
--rw-r--r--   0        0        0     1221 2024-02-26 15:00:31.913960 qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.186004 qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2_grpc.py
--rw-r--r--   0        0        0    11437 2024-02-26 15:00:34.190005 qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py
--rw-r--r--   0        0        0    12170 2024-02-26 15:00:32.193966 qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi
--rw-r--r--   0        0        0     9793 2024-02-26 15:00:34.190005 qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4060 2024-02-26 15:00:34.190005 qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/population_pb2.py
--rw-r--r--   0        0        0     3906 2024-02-26 15:00:32.053963 qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.190005 qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/population_pb2_grpc.py
--rw-r--r--   0        0        0    10804 2024-02-26 15:00:34.130004 qwak_core-0.3.99/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0    12120 2024-02-26 15:00:26.973863 qwak_core-0.3.99/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     9642 2024-02-26 15:00:34.130004 qwak_core-0.3.99/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2024-02-26 15:00:34.142004 qwak_core-0.3.99/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2024-02-26 15:00:28.289889 qwak_core-0.3.99/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2024-02-26 15:00:34.146004 qwak_core-0.3.99/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     9413 2024-02-26 15:00:33.950000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0    11436 2024-02-26 15:00:15.253633 qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.954000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    19751 2024-02-26 15:00:33.950000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    13467 2024-02-26 15:00:15.113630 qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    24352 2024-02-26 15:00:33.950000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2024-02-26 15:00:33.946000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2024-02-26 15:00:14.681622 qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.946000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2477 2024-02-26 15:00:33.946000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2679 2024-02-26 15:00:14.825625 qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.946000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2024-02-26 15:00:33.946000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2024-02-26 15:00:14.969627 qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2024-02-26 15:00:33.950000 qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6909 2024-02-26 15:00:34.166004 qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     5186 2024-02-26 15:00:30.185926 qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2024-02-26 15:00:34.166004 qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7868 2024-02-26 15:00:34.162004 qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    12177 2024-02-26 15:00:30.041923 qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.166004 qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11009 2024-02-26 15:00:33.966000 qwak_core-0.3.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    14329 2024-02-26 15:00:16.257653 qwak_core-0.3.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.966000 qwak_core-0.3.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3521 2024-02-26 15:00:33.966000 qwak_core-0.3.99/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2815 2024-02-26 15:00:16.397656 qwak_core-0.3.99/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:33.966000 qwak_core-0.3.99/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     8406 2024-02-26 15:00:34.082002 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py
--rw-r--r--   0        0        0    12199 2024-02-26 15:00:22.061767 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.082002 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_pb2_grpc.py
--rw-r--r--   0        0        0    13830 2024-02-26 15:00:34.086003 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py
--rw-r--r--   0        0        0    10297 2024-02-26 15:00:22.205769 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi
--rw-r--r--   0        0        0    17183 2024-02-26 15:00:34.086003 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py
--rw-r--r--   0        0        0     1873 2024-02-26 15:00:34.082002 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py
--rw-r--r--   0        0        0     1550 2024-02-26 15:00:21.913764 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.082002 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2_grpc.py
--rw-r--r--   0        0        0     8996 2024-02-26 15:00:34.086003 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/filters_pb2.py
--rw-r--r--   0        0        0    11380 2024-02-26 15:00:22.357772 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.086003 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/filters_pb2_grpc.py
--rw-r--r--   0        0        0     4533 2024-02-26 15:00:34.090003 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_pb2.py
--rw-r--r--   0        0        0     6103 2024-02-26 15:00:22.501775 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.090003 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_pb2_grpc.py
--rw-r--r--   0        0        0     9738 2024-02-26 15:00:34.090003 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py
--rw-r--r--   0        0        0    10977 2024-02-26 15:00:22.645778 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi
--rw-r--r--   0        0        0    10157 2024-02-26 15:00:34.090003 qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py
--rw-r--r--   0        0        0    10852 2024-02-26 15:00:34.202005 qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_pb2.py
--rw-r--r--   0        0        0    17043 2024-02-26 15:00:33.481991 qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-26 15:00:34.202005 qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_pb2_grpc.py
--rw-r--r--   0        0        0    21429 2024-02-26 15:00:34.206005 qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_service_pb2.py
--rw-r--r--   0        0        0    13726 2024-02-26 15:00:33.625994 qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi
--rw-r--r--   0        0        0    27193 2024-02-26 15:00:34.206005 qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py
--rw-r--r--   0        0        0     3697 2024-02-26 15:00:44.866214 qwak_core-0.3.99/pyproject.toml
--rw-r--r--   0        0        0      586 2024-02-26 15:00:44.870214 qwak_core-0.3.99/qwak/__init__.py
--rw-r--r--   0        0        0     1522 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3228 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12456 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/automations/automations.py
--rw-r--r--   0        0        0    12907 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    26800 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     2404 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/_inner/__init__.py
--rw-r--r--   0        0        0      849 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/_inner/edge_communications.py
--rw-r--r--   0        0        0      224 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       43 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/alerts_registry/__init__.py
--rw-r--r--   0        0        0     4040 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/alerts_registry/channel.py
--rw-r--r--   0        0        0     5355 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/alerts_registry/client.py
--rw-r--r--   0        0        0       42 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     9034 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    20927 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6815 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4209 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0      105 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0     4936 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/build_orchestrator/build_model_request_getter.py
--rw-r--r--   0        0        0    16148 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0     3981 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/build_orchestrator/internal_client.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     2401 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0      885 2024-02-26 14:58:48.575938 qwak_core-0.3.99/qwak/clients/data_versioning/data_tag_filter.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6806 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     4051 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/feature_store/execution_management_client.py
--rw-r--r--   0        0        0     2635 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    16056 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     8022 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/feature_store/offline_serving_client.py
--rw-r--r--   0        0        0     5811 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     2505 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0      885 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/file_versioning/file_tag_filter.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9308 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     4431 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3559 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      102 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/vector_store/__init__.py
--rw-r--r--   0        0        0     4247 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/vector_store/management_client.py
--rw-r--r--   0        0        0     5293 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/vector_store/serving_client.py
--rw-r--r--   0        0        0       43 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/workspace_manager/__init__.py
--rw-r--r--   0        0        0     8136 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/clients/workspace_manager/client.py
--rw-r--r--   0        0        0      790 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      135 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      424 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_general_build_exception.py
--rw-r--r--   0        0        0      579 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0       54 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_load_configuration_exception.py
--rw-r--r--   0        0        0      274 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      137 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_remote_build_failed.py
--rw-r--r--   0        0        0      746 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/exceptions/qwak_suggestion_exception.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     1977 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/_common/artifact_utils.py
--rw-r--r--   0        0        0     5141 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/_common/feature_set_utils.py
--rw-r--r--   0        0        0     4707 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     6680 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/_common/packaging.py
--rw-r--r--   0        0        0     2114 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0     2694 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/base.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/__init__.py
--rw-r--r--   0        0        0      197 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/_batch.py
--rw-r--r--   0        0        0      658 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/_jdbc.py
--rw-r--r--   0        0        0    10805 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/athena.py
--rw-r--r--   0        0        0     3022 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/big_query.py
--rw-r--r--   0        0        0     2063 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/clickhouse.py
--rw-r--r--   0        0        0     1905 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/csv.py
--rw-r--r--   0        0        0     2130 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/elastic_search.py
--rw-r--r--   0        0        0     3695 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/filesystem_config.py
--rw-r--r--   0        0        0     1921 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/mongodb.py
--rw-r--r--   0        0        0     1595 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/mysql.py
--rw-r--r--   0        0        0     1752 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/parquet.py
--rw-r--r--   0        0        0     1648 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/postgres.py
--rw-r--r--   0        0        0     3114 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/redshift.py
--rw-r--r--   0        0        0     2579 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/snowflake.py
--rw-r--r--   0        0        0     1830 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/batch/vertica.py
--rw-r--r--   0        0        0      895 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/source_authentication.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/__init__.py
--rw-r--r--   0        0        0      181 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/_streaming.py
--rw-r--r--   0        0        0      649 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/kafka/__init__.py
--rw-r--r--   0        0        0     3959 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/kafka/authentication.py
--rw-r--r--   0        0        0     3510 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/kafka/deserialization.py
--rw-r--r--   0        0        0     4398 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/kafka/kafka.py
--rw-r--r--   0        0        0     5984 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/data_sources/time_partition_columns.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     2313 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/execution/__init__.py
--rw-r--r--   0        0        0     6470 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/execution/backfill.py
--rw-r--r--   0        0        0    21243 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/execution/execution.py
--rw-r--r--   0        0        0     3564 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/execution/execution_query.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1636 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/_utils/_featureset_utils.py
--rw-r--r--   0        0        0     1979 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0     5285 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/base_feature_set.py
--rw-r--r--   0        0        0    16910 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1670 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0     1155 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0    23233 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/streaming.py
--rw-r--r--   0        0        0     9584 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/streaming_backfill.py
--rw-r--r--   0        0        0      733 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/aggregations/__init__.py
--rw-r--r--   0        0        0    14117 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py
--rw-r--r--   0        0        0     2253 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/aggregations/windows.py
--rw-r--r--   0        0        0      281 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/functions/__init__.py
--rw-r--r--   0        0        0     2425 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py
--rw-r--r--   0        0        0     1156 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/functions/schema.py
--rw-r--r--   0        0        0     9659 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/transformations.py
--rw-r--r--   0        0        0      173 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0     1216 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/offline/_offline_serving_validations.py
--rw-r--r--   0        0        0      738 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28651 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0    12572 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/offline/client_v2.py
--rw-r--r--   0        0        0      739 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/offline/feature_set_features.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9982 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0     2210 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/online/endpoint_utils.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/validations/__init__.py
--rw-r--r--   0        0        0     2656 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/validations/validation_options.py
--rw-r--r--   0        0        0     3783 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/validations/validation_response.py
--rw-r--r--   0        0        0     3864 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/feature_store/validations/validator.py
--rw-r--r--   0        0        0      226 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_config/__init__.py
--rw-r--r--   0        0        0    10469 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_config/build_config_v1.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/build_loggers/__init__.py
--rw-r--r--   0        0        0     1426 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/build_loggers/trigger_build_logger.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/constants/__init__.py
--rw-r--r--   0        0        0      209 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/constants/dependencies.py
--rw-r--r--   0        0        0      131 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/constants/host_resource.py
--rw-r--r--   0        0        0       94 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/constants/messages.py
--rw-r--r--   0        0        0       36 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/constants/temp_dir.py
--rw-r--r--   0        0        0      279 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/constants/upload_tag.py
--rw-r--r--   0        0        0      116 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/dependency_manager_type.py
--rw-r--r--   0        0        0     2299 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/execute_build_pipeline.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/interface/__init__.py
--rw-r--r--   0        0        0      528 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/interface/build_logger_interface.py
--rw-r--r--   0        0        0      675 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/interface/build_phase.py
--rw-r--r--   0        0        0     2094 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/interface/context_interface.py
--rw-r--r--   0        0        0     1723 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/interface/phase_run_handler.py
--rw-r--r--   0        0        0      718 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/interface/step_inteface.py
--rw-r--r--   0        0        0      585 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/interface/time_source.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/phases/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/__init__.py
--rw-r--r--   0        0        0     1895 2024-02-26 14:58:48.579938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/__init__.py
--rw-r--r--   0        0        0      953 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py
--rw-r--r--   0        0        0     2067 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/__init__.py
--rw-r--r--   0        0        0     5057 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/__init__.py
--rw-r--r--   0        0        0     5944 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py
--rw-r--r--   0        0        0     1424 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/__init__.py
--rw-r--r--   0        0        0     2258 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py
--rw-r--r--   0        0        0     5399 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py
--rw-r--r--   0        0        0     8796 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py
--rw-r--r--   0        0        0     1186 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/__init__.py
--rw-r--r--   0        0        0      618 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py
--rw-r--r--   0        0        0     1599 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py
--rw-r--r--   0        0        0     9553 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py
--rw-r--r--   0        0        0     1244 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/phases/phases_pipeline.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/run_handlers/__init__.py
--rw-r--r--   0        0        0     3484 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/tools/__init__.py
--rw-r--r--   0        0        0     2498 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/tools/dependencies_tools.py
--rw-r--r--   0        0        0     8228 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/tools/files.py
--rw-r--r--   0        0        0      750 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/tools/ignore_files.py
--rw-r--r--   0        0        0      188 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/tools/text.py
--rw-r--r--   0        0        0      200 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/build_logic/trigger_build_context.py
--rw-r--r--   0        0        0     1084 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/const.py
--rw-r--r--   0        0        0     1595 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0      242 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0     1018 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      414 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/instance_template/__init__.py
--rw-r--r--   0        0        0     1497 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/instance_template/verify_template_id.py
--rw-r--r--   0        0        0     2933 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      281 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      545 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     6897 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      422 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0     1686 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/protobuf_factory.py
--rw-r--r--   0        0        0      435 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     4200 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6976 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/__init__.py
--rw-r--r--   0        0        0     4762 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/_entity_extraction.py
--rw-r--r--   0        0        0     1739 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      322 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      321 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/base.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1857 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/decorators/api.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/decorators/impl/__init__.py
--rw-r--r--   0        0        0      956 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/decorators/impl/api_implementation.py
--rw-r--r--   0        0        0      215 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/decorators/impl/timer_implementation.py
--rw-r--r--   0        0        0      739 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/decorators/timer.py
--rw-r--r--   0        0        0     1503 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0     1981 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/schema.py
--rw-r--r--   0        0        0     2411 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      786 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     2176 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0     1560 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2712 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      798 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0     2289 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2938 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5472 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0     1757 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/batch_jobs/execution.py
--rw-r--r--   0        0        0     1531 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/batch_jobs/task.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/build_api_helpers/__init__.py
--rw-r--r--   0        0        0     1886 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/build_api_helpers/build_api_steps.py
--rw-r--r--   0        0        0      184 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/build_api_helpers/messages.py
--rw-r--r--   0        0        0     2355 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/build_api_helpers/trigger_build_api.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    26680 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/data_versioning/__init__.py
--rw-r--r--   0        0        0      806 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/data_versioning/data_tag.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13287 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/file_versioning/__init__.py
--rw-r--r--   0        0        0      806 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/file_versioning/file_tag.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0     1191 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2390 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/utils/__init__.py
--rw-r--r--   0        0        0      581 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/utils/datetime_utils.py
--rw-r--r--   0        0        0      120 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/vector_store/__init__.py
--rw-r--r--   0        0        0     5835 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/vector_store/client.py
--rw-r--r--   0        0        0    16916 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/vector_store/collection.py
--rw-r--r--   0        0        0     8209 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/vector_store/filters.py
--rw-r--r--   0        0        0     3619 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/vector_store/inference_client.py
--rw-r--r--   0        0        0     2658 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/vector_store/rest_helpers.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/vector_store/utils/__init__.py
--rw-r--r--   0        0        0      837 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/vector_store/utils/filter_utils.py
--rw-r--r--   0        0        0     7459 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak/vector_store/utils/upsert_utils.py
--rw-r--r--   0        0        0       46 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2263 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/mocks/alert_registry_service_api.py
--rw-r--r--   0        0        0     2129 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1189 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    13129 2024-02-26 14:58:48.583938 qwak_core-0.3.99/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3686 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     4984 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     1264 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py
--rw-r--r--   0        0        0     5226 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     2453 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    20753 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1608 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0      886 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/execution_management_service.py
--rw-r--r--   0        0        0     3207 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     3400 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3712 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     6155 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     2592 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     1635 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/fs_offline_serving_service.py
--rw-r--r--   0        0        0     3905 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     1046 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/internal_build_orchestrator_service.py
--rw-r--r--   0        0        0     2696 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     4153 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     5500 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0     5722 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/vector_serving_api.py
--rw-r--r--   0        0        0     3594 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/vectors_management_api.py
--rw-r--r--   0        0        0     7591 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/mocks/workspace_manager_service_mock.py
--rw-r--r--   0        0        0    17551 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2024-02-26 14:58:48.587938 qwak_core-0.3.99/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     7247 1970-01-01 00:00:00.000000 qwak_core-0.3.99/setup.py
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 qwak_core-0.3.99/PKG-INFO
+-rw-r--r--   0        0        0      264 2024-05-05 10:41:18.274960 qwak_core-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 10:43:53.597721 qwak_core-0.4.0/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5877 2024-05-05 10:43:53.625721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     7824 2024-05-05 10:43:24.025959 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.625721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0    12703 2024-05-05 10:43:53.625721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py
+-rw-r--r--   0        0        0    10914 2024-05-05 10:43:24.221957 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi
+-rw-r--r--   0        0        0    14681 2024-05-05 10:43:53.629721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2024-05-05 10:43:53.617721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2024-05-05 10:43:23.637962 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.621721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2024-05-05 10:43:53.621721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2024-05-05 10:43:23.829960 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.621721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2024-05-05 10:43:53.613721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2024-05-05 10:43:23.053967 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2024-05-05 10:43:53.613721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2024-05-05 10:43:53.613721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2024-05-05 10:43:23.249965 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.613721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2024-05-05 10:43:53.617721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2024-05-05 10:43:23.445963 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.617721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2024-05-05 10:43:53.597721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2024-05-05 10:43:22.857968 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2024-05-05 10:43:53.597721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7360 2024-05-05 10:43:53.597721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0    11651 2024-05-05 10:43:24.417956 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.601721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     5029 2024-05-05 10:43:53.605721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     6943 2024-05-05 10:43:24.805953 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.605721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2024-05-05 10:43:53.605721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2024-05-05 10:43:25.001951 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2024-05-05 10:43:53.609721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2024-05-05 10:43:53.601721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2024-05-05 10:43:24.609954 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.601721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6541 2024-05-05 10:43:53.609721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10595 2024-05-05 10:43:25.197950 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.609721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0    15382 2024-05-05 10:43:53.661720 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    20668 2024-05-05 10:43:28.013927 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.661720 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2024-05-05 10:43:53.665720 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2024-05-05 10:43:28.209925 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2024-05-05 10:43:53.665720 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7616 2024-05-05 10:43:53.813719 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11995 2024-05-05 10:43:37.865847 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.813719 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0    14893 2024-05-05 10:43:53.817719 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0    11812 2024-05-05 10:43:38.065846 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    19155 2024-05-05 10:43:53.817719 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2024-05-05 10:43:53.821719 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2024-05-05 10:43:39.273836 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2024-05-05 10:43:53.821719 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8864 2024-05-05 10:43:53.817719 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13789 2024-05-05 10:43:39.069838 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.817719 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2024-05-05 10:43:53.821719 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2024-05-05 10:43:39.473835 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.825719 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2024-05-05 10:43:53.825719 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2024-05-05 10:43:39.669833 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2024-05-05 10:43:53.825719 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    14053 2024-05-05 10:43:53.941718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    20860 2024-05-05 10:43:49.473754 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.941718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2024-05-05 10:43:53.933718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2024-05-05 10:43:49.049757 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.937718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3954 2024-05-05 10:43:53.937718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     5309 2024-05-05 10:43:49.249756 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.937718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    21176 2024-05-05 10:43:53.929718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    15049 2024-05-05 10:43:48.633761 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    25475 2024-05-05 10:43:53.929718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2024-05-05 10:43:53.933718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2024-05-05 10:43:48.845759 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.933718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2024-05-05 10:43:53.945718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2024-05-05 10:43:50.069749 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.949718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2024-05-05 10:43:53.945718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2024-05-05 10:43:49.873751 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.945718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2024-05-05 10:43:53.941718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2024-05-05 10:43:49.673752 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.941718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    11218 2024-05-05 10:43:53.925718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    15584 2024-05-05 10:43:48.385763 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.929718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2083 2024-05-05 10:43:53.921718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1977 2024-05-05 10:43:47.949766 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.921718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    46028 2024-05-05 10:43:53.925718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    60013 2024-05-05 10:43:48.181764 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    32008 2024-05-05 10:43:53.925718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    29124 2024-05-05 10:43:53.857719 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    24434 2024-05-05 10:43:41.861815 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    27837 2024-05-05 10:43:53.861719 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    33279 2024-05-05 10:43:53.857719 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    52325 2024-05-05 10:43:41.437819 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.857719 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0     5757 2024-05-05 10:43:53.865719 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py
+-rw-r--r--   0        0        0     4013 2024-05-05 10:43:42.493810 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi
+-rw-r--r--   0        0        0     6783 2024-05-05 10:43:53.865719 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py
+-rw-r--r--   0        0        0     6016 2024-05-05 10:43:53.861719 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2.py
+-rw-r--r--   0        0        0     7049 2024-05-05 10:43:42.285812 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.861719 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2_grpc.py
+-rw-r--r--   0        0        0    14932 2024-05-05 10:43:53.841719 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    24192 2024-05-05 10:43:41.193821 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.845719 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     5552 2024-05-05 10:43:53.845719 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     7299 2024-05-05 10:43:41.645817 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.845719 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    15672 2024-05-05 10:43:53.849719 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0    12741 2024-05-05 10:43:42.077813 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    16925 2024-05-05 10:43:53.849719 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38491 2024-05-05 10:43:53.853719 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    53557 2024-05-05 10:43:43.193805 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2024-05-05 10:43:53.853719 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     3508 2024-05-05 10:43:53.849719 qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     2300 2024-05-05 10:43:42.709808 qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0     3101 2024-05-05 10:43:53.853719 qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2270 2024-05-05 10:43:53.869719 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     2697 2024-05-05 10:43:43.641801 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.873719 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4458 2024-05-05 10:43:53.873719 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     3113 2024-05-05 10:43:43.853799 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2024-05-05 10:43:53.873719 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2024-05-05 10:43:53.837719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2024-05-05 10:43:40.549826 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.837719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11871 2024-05-05 10:43:53.837719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     8790 2024-05-05 10:43:40.761824 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2024-05-05 10:43:53.841719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2024-05-05 10:43:53.829719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2024-05-05 10:43:40.101829 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.833719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    50041 2024-05-05 10:43:53.829719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    74372 2024-05-05 10:43:39.897831 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.829719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    46309 2024-05-05 10:43:53.833719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    40356 2024-05-05 10:43:40.337828 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    27756 2024-05-05 10:43:53.833719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3345 2024-05-05 10:43:53.649720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     4098 2024-05-05 10:43:27.001935 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.649720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12707 2024-05-05 10:43:53.649720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    13800 2024-05-05 10:43:27.201933 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.653720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    17949 2024-05-05 10:43:53.653720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    18562 2024-05-05 10:43:27.401932 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    12833 2024-05-05 10:43:53.653720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6463 2024-05-05 10:43:53.769719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2.py
+-rw-r--r--   0        0        0     7945 2024-05-05 10:43:33.209885 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.769719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2_grpc.py
+-rw-r--r--   0        0        0     2971 2024-05-05 10:43:53.769719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2.py
+-rw-r--r--   0        0        0     3266 2024-05-05 10:43:33.417883 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.773719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     2210 2024-05-05 10:43:53.773719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/deletion_pb2.py
+-rw-r--r--   0        0        0     1540 2024-05-05 10:43:33.637882 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.773719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/deletion_pb2_grpc.py
+-rw-r--r--   0        0        0     5793 2024-05-05 10:43:53.777719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2.py
+-rw-r--r--   0        0        0     7373 2024-05-05 10:43:33.849880 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.777719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    14900 2024-05-05 10:43:53.777719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2.py
+-rw-r--r--   0        0        0    11103 2024-05-05 10:43:34.061878 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi
+-rw-r--r--   0        0        0    17220 2024-05-05 10:43:53.781719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7695 2024-05-05 10:43:53.785719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py
+-rw-r--r--   0        0        0    14959 2024-05-05 10:43:34.489875 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.785719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0    19304 2024-05-05 10:43:53.785719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0    16916 2024-05-05 10:43:34.689873 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    21145 2024-05-05 10:43:53.785719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8440 2024-05-05 10:43:53.781719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py
+-rw-r--r--   0        0        0    13312 2024-05-05 10:43:34.281876 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.781719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     2051 2024-05-05 10:43:53.789719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py
+-rw-r--r--   0        0        0     1952 2024-05-05 10:43:34.885872 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.789719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2_grpc.py
+-rw-r--r--   0        0        0    12222 2024-05-05 10:43:53.789719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py
+-rw-r--r--   0        0        0     7930 2024-05-05 10:43:35.081870 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi
+-rw-r--r--   0        0        0    14212 2024-05-05 10:43:53.793719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1685 2024-05-05 10:43:53.793719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py
+-rw-r--r--   0        0        0     1272 2024-05-05 10:43:35.277868 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.793719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2_grpc.py
+-rw-r--r--   0        0        0     6198 2024-05-05 10:43:53.797719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py
+-rw-r--r--   0        0        0     7677 2024-05-05 10:43:35.473867 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.797719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2024-05-05 10:43:53.745720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2024-05-05 10:43:33.005887 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.745720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2024-05-05 10:43:53.741720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2024-05-05 10:43:32.805888 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2024-05-05 10:43:53.741720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2024-05-05 10:43:53.713720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2024-05-05 10:43:30.637906 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.713720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0    13825 2024-05-05 10:43:53.725720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2.py
+-rw-r--r--   0        0        0    19227 2024-05-05 10:43:31.617898 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.725720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3307 2024-05-05 10:43:53.729720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py
+-rw-r--r--   0        0        0     1637 2024-05-05 10:43:31.817896 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3293 2024-05-05 10:43:53.729720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2024-05-05 10:43:53.709720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2024-05-05 10:43:30.441907 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.713720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2024-05-05 10:43:53.701720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2024-05-05 10:43:29.829912 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.705720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2024-05-05 10:43:53.709720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2024-05-05 10:43:30.245909 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2024-05-05 10:43:53.709720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2024-05-05 10:43:53.717720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2024-05-05 10:43:30.833904 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.717720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2024-05-05 10:43:53.717720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2024-05-05 10:43:31.029903 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2024-05-05 10:43:53.721720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    26853 2024-05-05 10:43:53.705720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    39247 2024-05-05 10:43:30.037911 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.705720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2024-05-05 10:43:53.721720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2024-05-05 10:43:31.221901 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.721720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    13240 2024-05-05 10:43:53.721720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    18420 2024-05-05 10:43:31.417899 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.725720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2024-05-05 10:43:53.745720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2024-05-05 10:43:52.317731 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.745720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2024-05-05 10:43:53.749719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2024-05-05 10:43:52.533729 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2024-05-05 10:43:53.749719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4308 2024-05-05 10:43:53.749719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     7410 2024-05-05 10:43:37.277852 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.753719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    15316 2024-05-05 10:43:53.753719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    14087 2024-05-05 10:43:37.477851 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    18465 2024-05-05 10:43:53.753719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2024-05-05 10:43:53.757719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2024-05-05 10:43:37.673849 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.757719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     5111 2024-05-05 10:43:53.765720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2.py
+-rw-r--r--   0        0        0     2739 2024-05-05 10:43:38.869840 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi
+-rw-r--r--   0        0        0     5436 2024-05-05 10:43:53.765720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py
+-rw-r--r--   0        0        0     5385 2024-05-05 10:43:53.761720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     7551 2024-05-05 10:43:38.469843 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.761720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    17474 2024-05-05 10:43:53.757719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2024-05-05 10:43:38.265844 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2024-05-05 10:43:53.761720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2024-05-05 10:43:53.765720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2024-05-05 10:43:38.665841 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.765720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    27355 2024-05-05 10:43:53.729720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    43393 2024-05-05 10:43:32.017895 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.733720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5147 2024-05-05 10:43:53.733720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6208 2024-05-05 10:43:32.213893 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.733720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2024-05-05 10:43:53.737720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2024-05-05 10:43:32.413891 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2024-05-05 10:43:53.737720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11049 2024-05-05 10:43:53.737720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15942 2024-05-05 10:43:32.609890 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.741720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2024-05-05 10:43:53.957718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2024-05-05 10:43:50.973742 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.957718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2024-05-05 10:43:53.961718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2024-05-05 10:43:51.193740 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2024-05-05 10:43:53.961718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2024-05-05 10:43:53.961718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2024-05-05 10:43:51.425738 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.965718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2024-05-05 10:43:53.965718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2024-05-05 10:43:51.653736 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2024-05-05 10:43:53.965718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10469 2024-05-05 10:43:53.969718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0    11719 2024-05-05 10:43:51.893735 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     9458 2024-05-05 10:43:53.969718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5302 2024-05-05 10:43:53.969718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     5484 2024-05-05 10:43:52.109733 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.969718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2975 2024-05-05 10:43:53.877719 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     4026 2024-05-05 10:43:44.069797 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.877719 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4455 2024-05-05 10:43:53.877719 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     3113 2024-05-05 10:43:44.281796 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2024-05-05 10:43:53.881718 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6950 2024-05-05 10:43:53.665720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    11560 2024-05-05 10:43:29.005919 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.669720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     3383 2024-05-05 10:43:53.669720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     5457 2024-05-05 10:43:29.201917 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.669720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2024-05-05 10:43:53.697720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2024-05-05 10:43:29.397916 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2024-05-05 10:43:53.697720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8504 2024-05-05 10:43:53.701720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12440 2024-05-05 10:43:29.597914 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.701720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2024-05-05 10:43:53.841719 qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2024-05-05 10:43:40.977822 qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2024-05-05 10:43:53.841719 qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3876 2024-05-05 10:43:53.881718 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4658 2024-05-05 10:43:44.497794 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.881718 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2024-05-05 10:43:53.885718 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2024-05-05 10:43:44.705792 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2024-05-05 10:43:53.885718 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2024-05-05 10:43:53.897718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2024-05-05 10:43:45.985782 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.901718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2024-05-05 10:43:53.901718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2024-05-05 10:43:46.197780 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.901718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    25218 2024-05-05 10:43:53.905718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    31280 2024-05-05 10:43:46.421779 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.905718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13432 2024-05-05 10:43:53.905718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    22974 2024-05-05 10:43:46.633777 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.905718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12784 2024-05-05 10:43:53.909718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16585 2024-05-05 10:43:46.861775 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.909718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    51171 2024-05-05 10:43:53.913718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    40800 2024-05-05 10:43:47.105773 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    73869 2024-05-05 10:43:53.913718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-05-05 10:43:53.913718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2024-05-05 10:43:47.313771 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.917718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2024-05-05 10:43:53.889718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2024-05-05 10:43:45.133789 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.889718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2024-05-05 10:43:53.897718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2024-05-05 10:43:45.765784 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.897718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2024-05-05 10:43:53.889718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2024-05-05 10:43:45.357787 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2024-05-05 10:43:53.893718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2024-05-05 10:43:53.893718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2024-05-05 10:43:45.561786 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.893718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    27866 2024-05-05 10:43:53.869719 qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    32184 2024-05-05 10:43:43.417803 qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    19830 2024-05-05 10:43:53.869719 qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2024-05-05 10:43:53.645720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2024-05-05 10:43:28.609922 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2024-05-05 10:43:53.645720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2024-05-05 10:43:53.641720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2024-05-05 10:43:28.409924 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.641720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2024-05-05 10:43:53.645720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2024-05-05 10:43:28.805920 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2024-05-05 10:43:53.649720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1598 2024-05-05 10:43:53.949718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py
+-rw-r--r--   0        0        0     1221 2024-05-05 10:43:50.305747 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.949718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2_grpc.py
+-rw-r--r--   0        0        0    11437 2024-05-05 10:43:53.953718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py
+-rw-r--r--   0        0        0    12170 2024-05-05 10:43:50.741744 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi
+-rw-r--r--   0        0        0     9793 2024-05-05 10:43:53.957718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4060 2024-05-05 10:43:53.953718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2.py
+-rw-r--r--   0        0        0     3906 2024-05-05 10:43:50.521746 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.953718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2_grpc.py
+-rw-r--r--   0        0        0    10804 2024-05-05 10:43:53.865719 qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0    12120 2024-05-05 10:43:42.965806 qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     9642 2024-05-05 10:43:53.865719 qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2024-05-05 10:43:53.885718 qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2024-05-05 10:43:44.917791 qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2024-05-05 10:43:53.885718 qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10718 2024-05-05 10:43:53.637720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0    12627 2024-05-05 10:43:26.213941 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.641720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    19751 2024-05-05 10:43:53.637720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    13467 2024-05-05 10:43:26.013943 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    24352 2024-05-05 10:43:53.637720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2024-05-05 10:43:53.629721 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2024-05-05 10:43:25.397948 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.629721 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2477 2024-05-05 10:43:53.629721 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2679 2024-05-05 10:43:25.605946 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.633720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2024-05-05 10:43:53.633720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2024-05-05 10:43:25.809944 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2024-05-05 10:43:53.633720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6909 2024-05-05 10:43:53.917718 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     5186 2024-05-05 10:43:47.733768 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2024-05-05 10:43:53.921718 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7868 2024-05-05 10:43:53.917718 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    12177 2024-05-05 10:43:47.525770 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.917718 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11396 2024-05-05 10:43:53.657720 qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15139 2024-05-05 10:43:27.601930 qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.657720 qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3645 2024-05-05 10:43:53.657720 qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2983 2024-05-05 10:43:27.805929 qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.661720 qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     8648 2024-05-05 10:43:53.801719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py
+-rw-r--r--   0        0        0    12852 2024-05-05 10:43:35.869864 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.801719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2_grpc.py
+-rw-r--r--   0        0        0    13830 2024-05-05 10:43:53.801719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py
+-rw-r--r--   0        0        0    10297 2024-05-05 10:43:36.081862 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi
+-rw-r--r--   0        0        0    17183 2024-05-05 10:43:53.805719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1873 2024-05-05 10:43:53.797719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py
+-rw-r--r--   0        0        0     1550 2024-05-05 10:43:35.665865 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.801719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2_grpc.py
+-rw-r--r--   0        0        0     8996 2024-05-05 10:43:53.805719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2.py
+-rw-r--r--   0        0        0    11380 2024-05-05 10:43:36.277860 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.805719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2_grpc.py
+-rw-r--r--   0        0        0     4533 2024-05-05 10:43:53.809719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2.py
+-rw-r--r--   0        0        0     6103 2024-05-05 10:43:36.477859 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.809719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2_grpc.py
+-rw-r--r--   0        0        0     9738 2024-05-05 10:43:53.809719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py
+-rw-r--r--   0        0        0    10977 2024-05-05 10:43:36.681857 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi
+-rw-r--r--   0        0        0    10157 2024-05-05 10:43:53.813719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10852 2024-05-05 10:43:53.973718 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2.py
+-rw-r--r--   0        0        0    17043 2024-05-05 10:43:52.781727 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 10:43:53.973718 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0    21429 2024-05-05 10:43:53.973718 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2.py
+-rw-r--r--   0        0        0    13726 2024-05-05 10:43:52.989726 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi
+-rw-r--r--   0        0        0    27193 2024-05-05 10:43:53.977718 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3696 2024-05-05 10:43:58.997677 qwak_core-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      585 2024-05-05 10:43:58.997677 qwak_core-0.4.0/qwak/__init__.py
+-rw-r--r--   0        0        0     1522 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12456 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/automations.py
+-rw-r--r--   0        0        0    12907 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    26800 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     2404 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/_inner/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/_inner/edge_communications.py
+-rw-r--r--   0        0        0      224 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5340 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       43 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alerts_registry/__init__.py
+-rw-r--r--   0        0        0     4040 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alerts_registry/channel.py
+-rw-r--r--   0        0        0     5355 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alerts_registry/client.py
+-rw-r--r--   0        0        0       42 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     9034 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    21054 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6882 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4209 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0      105 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0     5045 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_orchestrator/build_model_request_getter.py
+-rw-r--r--   0        0        0    16148 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0     3981 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_orchestrator/internal_client.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     2401 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0      885 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/data_versioning/data_tag_filter.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6806 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     4051 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/execution_management_client.py
+-rw-r--r--   0        0        0     2635 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    16056 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     8022 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/offline_serving_client.py
+-rw-r--r--   0        0        0     5811 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     2505 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0      885 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/file_versioning/file_tag_filter.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2509 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9308 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     4431 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3581 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      102 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/vector_store/__init__.py
+-rw-r--r--   0        0        0     4247 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/vector_store/management_client.py
+-rw-r--r--   0        0        0     5293 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/vector_store/serving_client.py
+-rw-r--r--   0        0        0       43 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/workspace_manager/__init__.py
+-rw-r--r--   0        0        0     8136 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/workspace_manager/client.py
+-rw-r--r--   0        0        0      790 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      192 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      424 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_general_build_exception.py
+-rw-r--r--   0        0        0      579 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0       54 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_load_configuration_exception.py
+-rw-r--r--   0        0        0      274 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      137 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_remote_build_failed.py
+-rw-r--r--   0        0        0      746 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_suggestion_exception.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     1977 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/artifact_utils.py
+-rw-r--r--   0        0        0     7046 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/feature_set_utils.py
+-rw-r--r--   0        0        0     4707 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     6680 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/packaging.py
+-rw-r--r--   0        0        0     2316 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0     2694 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/base.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/_batch.py
+-rw-r--r--   0        0        0      658 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/_jdbc.py
+-rw-r--r--   0        0        0    10805 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/athena.py
+-rw-r--r--   0        0        0     3022 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/big_query.py
+-rw-r--r--   0        0        0     2063 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/clickhouse.py
+-rw-r--r--   0        0        0     1981 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/csv.py
+-rw-r--r--   0        0        0     2130 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/elastic_search.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/aws.py
+-rw-r--r--   0        0        0      245 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/base_config.py
+-rw-r--r--   0        0        0     1572 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/gcp.py
+-rw-r--r--   0        0        0     1874 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/utils.py
+-rw-r--r--   0        0        0     1921 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/mongodb.py
+-rw-r--r--   0        0        0     1595 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/mysql.py
+-rw-r--r--   0        0        0     1867 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/parquet.py
+-rw-r--r--   0        0        0     1648 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/postgres.py
+-rw-r--r--   0        0        0     3114 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/redshift.py
+-rw-r--r--   0        0        0     2579 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/snowflake.py
+-rw-r--r--   0        0        0     1830 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/vertica.py
+-rw-r--r--   0        0        0      895 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/source_authentication.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/__init__.py
+-rw-r--r--   0        0        0      181 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/_streaming.py
+-rw-r--r--   0        0        0      649 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/__init__.py
+-rw-r--r--   0        0        0     3959 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/authentication.py
+-rw-r--r--   0        0        0     3510 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/deserialization.py
+-rw-r--r--   0        0        0     4398 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/kafka.py
+-rw-r--r--   0        0        0     5984 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/time_partition_columns.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     2313 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/execution/__init__.py
+-rw-r--r--   0        0        0     6470 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/execution/backfill.py
+-rw-r--r--   0        0        0    21243 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/execution/execution.py
+-rw-r--r--   0        0        0     3564 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/execution/execution_query.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1636 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/_utils/_featureset_utils.py
+-rw-r--r--   0        0        0     1979 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0     5285 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/base_feature_set.py
+-rw-r--r--   0        0        0    16910 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1670 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0     1155 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0    23233 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/streaming.py
+-rw-r--r--   0        0        0     9584 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/streaming_backfill.py
+-rw-r--r--   0        0        0      733 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/__init__.py
+-rw-r--r--   0        0        0    14117 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py
+-rw-r--r--   0        0        0     2253 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/windows.py
+-rw-r--r--   0        0        0      281 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/__init__.py
+-rw-r--r--   0        0        0     2425 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py
+-rw-r--r--   0        0        0     1156 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/schema.py
+-rw-r--r--   0        0        0     9659 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/transformations.py
+-rw-r--r--   0        0        0      173 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0     1216 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/_offline_serving_validations.py
+-rw-r--r--   0        0        0      738 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28651 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0    12597 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/client_v2.py
+-rw-r--r--   0        0        0      739 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/feature_set_features.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0    11144 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0     2210 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/online/endpoint_utils.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/validations/__init__.py
+-rw-r--r--   0        0        0     2656 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/validations/validation_options.py
+-rw-r--r--   0        0        0     3783 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/validations/validation_response.py
+-rw-r--r--   0        0        0     3864 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/validations/validator.py
+-rw-r--r--   0        0        0      226 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_config/__init__.py
+-rw-r--r--   0        0        0    10978 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_config/build_config_v1.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/build_loggers/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/build_loggers/trigger_build_logger.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/dependencies.py
+-rw-r--r--   0        0        0      131 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/host_resource.py
+-rw-r--r--   0        0        0       94 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/messages.py
+-rw-r--r--   0        0        0       36 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/temp_dir.py
+-rw-r--r--   0        0        0      279 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/upload_tag.py
+-rw-r--r--   0        0        0      116 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/dependency_manager_type.py
+-rw-r--r--   0        0        0     2299 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/execute_build_pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/__init__.py
+-rw-r--r--   0        0        0      528 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/build_logger_interface.py
+-rw-r--r--   0        0        0      675 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/build_phase.py
+-rw-r--r--   0        0        0     2247 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/context_interface.py
+-rw-r--r--   0        0        0     1723 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/phase_run_handler.py
+-rw-r--r--   0        0        0      718 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/step_inteface.py
+-rw-r--r--   0        0        0      585 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/time_source.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/__init__.py
+-rw-r--r--   0        0        0     1895 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py
+-rw-r--r--   0        0        0     2067 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/__init__.py
+-rw-r--r--   0        0        0     5057 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/__init__.py
+-rw-r--r--   0        0        0     5944 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py
+-rw-r--r--   0        0        0     1424 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/__init__.py
+-rw-r--r--   0        0        0     2258 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py
+-rw-r--r--   0        0        0     5399 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py
+-rw-r--r--   0        0        0    10894 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py
+-rw-r--r--   0        0        0     1186 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/__init__.py
+-rw-r--r--   0        0        0      618 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py
+-rw-r--r--   0        0        0     1599 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py
+-rw-r--r--   0        0        0     9553 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py
+-rw-r--r--   0        0        0     1244 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phases_pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/run_handlers/__init__.py
+-rw-r--r--   0        0        0     3484 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/__init__.py
+-rw-r--r--   0        0        0     2498 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/dependencies_tools.py
+-rw-r--r--   0        0        0     8228 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/files.py
+-rw-r--r--   0        0        0      750 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/ignore_files.py
+-rw-r--r--   0        0        0      188 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/text.py
+-rw-r--r--   0        0        0      200 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/trigger_build_context.py
+-rw-r--r--   0        0        0     1084 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/const.py
+-rw-r--r--   0        0        0     1595 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0      242 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0     1018 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      414 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/instance_template/__init__.py
+-rw-r--r--   0        0        0     1916 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/instance_template/verify_template_id.py
+-rw-r--r--   0        0        0     2933 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0       70 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/provider.py
+-rw-r--r--   0        0        0      281 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      545 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3830 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     6897 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      422 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0     1686 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/protobuf_factory.py
+-rw-r--r--   0        0        0      435 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     4200 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6976 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/__init__.py
+-rw-r--r--   0        0        0     4762 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/_entity_extraction.py
+-rw-r--r--   0        0        0     1739 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      322 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      321 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1938 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/impl/__init__.py
+-rw-r--r--   0        0        0      993 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/impl/api_implementation.py
+-rw-r--r--   0        0        0      215 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/impl/timer_implementation.py
+-rw-r--r--   0        0        0      739 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/timer.py
+-rw-r--r--   0        0        0     1503 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0     1981 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/schema.py
+-rw-r--r--   0        0        0     2411 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      786 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     2176 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0     1560 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2712 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      798 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0     2289 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2938 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5472 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0     1757 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/batch_jobs/execution.py
+-rw-r--r--   0        0        0     1531 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/batch_jobs/task.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/__init__.py
+-rw-r--r--   0        0        0     1886 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/build_api_steps.py
+-rw-r--r--   0        0        0      184 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/messages.py
+-rw-r--r--   0        0        0     2355 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/trigger_build_api.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    26693 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/data_versioning/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/data_versioning/data_tag.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13288 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/file_versioning/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/file_versioning/file_tag.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0     1191 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/utils/__init__.py
+-rw-r--r--   0        0        0      581 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/utils/datetime_utils.py
+-rw-r--r--   0        0        0      120 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/__init__.py
+-rw-r--r--   0        0        0     6040 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/client.py
+-rw-r--r--   0        0        0    16916 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/collection.py
+-rw-r--r--   0        0        0     8209 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/filters.py
+-rw-r--r--   0        0        0     3711 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/inference_client.py
+-rw-r--r--   0        0        0     2658 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/rest_helpers.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/utils/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/utils/filter_utils.py
+-rw-r--r--   0        0        0     7459 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/utils/upsert_utils.py
+-rw-r--r--   0        0        0       46 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2263 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/alert_registry_service_api.py
+-rw-r--r--   0        0        0     2129 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1189 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    13129 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3686 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     4984 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     1264 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py
+-rw-r--r--   0        0        0     5226 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     2453 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    20753 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1608 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0      886 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/execution_management_service.py
+-rw-r--r--   0        0        0     3207 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     3400 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3712 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     6800 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     2592 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     1635 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/fs_offline_serving_service.py
+-rw-r--r--   0        0        0     4567 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     1046 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/internal_build_orchestrator_service.py
+-rw-r--r--   0        0        0     2696 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     4153 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     5500 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0     5722 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/vector_serving_api.py
+-rw-r--r--   0        0        0     3594 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/vectors_management_api.py
+-rw-r--r--   0        0        0     7591 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/workspace_manager_service_mock.py
+-rw-r--r--   0        0        0    17551 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 qwak_core-0.4.0/setup.py
+-rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 qwak_core-0.4.0/PKG-INFO
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,21 +14,27 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.administration.v0.environments import configuration_pb2 as qwak_dot_administration_dot_v0_dot_environments_dot_configuration__pb2
 from _qwak_proto.qwak.administration.v0.environments import personalization_pb2 as qwak_dot_administration_dot_v0_dot_environments_dot_personalization__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5qwak/administration/v0/environments/environment.proto\x12\x1fqwak.administration.environment\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x37qwak/administration/v0/environments/configuration.proto\x1a\x39qwak/administration/v0/environments/personalization.proto\"\xc4\x03\n\x0fQwakEnvironment\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\ttenant_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x12\n\naccount_id\x18\x08 \x01(\t\x12\x12\n\ncluster_id\x18\n \x01(\t\x12\x46\n\x06status\x18\x04 \x01(\x0e\x32\x36.qwak.administration.environment.QwakEnvironmentStatus\x12T\n\rconfiguration\x18\x05 \x01(\x0b\x32=.qwak.administration.environment.QwakEnvironmentConfiguration\x12T\n\x0fpersonalization\x18\t \x01(\x0b\x32;.qwak.administration.environment.EnvironmentPersonalization\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"8\n%EnvironmentApplicationUserCredentials\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t*w\n\x15QwakEnvironmentStatus\x12\x1e\n\x1a\x45NVIRONMENT_STATUS_INVALID\x10\x00\x12\x1d\n\x19\x45NVIRONMENT_STATUS_ACTIVE\x10\x01\x12\x1f\n\x1b\x45NVIRONMENT_STATUS_DISABLED\x10\x02\x42\xb2\x01\n\x1e\x63om.qwak.ai.administration.apiP\x01Z\x8d\x01github.com/qwak-ai/qwak-platform/services/core/java/user-management/user-management-api/pb/qwak/administration/v0/environments;environment_v0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5qwak/administration/v0/environments/environment.proto\x12\x1fqwak.administration.environment\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x37qwak/administration/v0/environments/configuration.proto\x1a\x39qwak/administration/v0/environments/personalization.proto\"\x88\x04\n\x0fQwakEnvironment\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\ttenant_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x12\n\naccount_id\x18\x08 \x01(\t\x12\x12\n\ncluster_id\x18\n \x01(\t\x12\x42\n\x0c\x61\x63\x63ount_tier\x18\x0b \x01(\x0e\x32,.qwak.administration.environment.AccountTier\x12\x46\n\x06status\x18\x04 \x01(\x0e\x32\x36.qwak.administration.environment.QwakEnvironmentStatus\x12T\n\rconfiguration\x18\x05 \x01(\x0b\x32=.qwak.administration.environment.QwakEnvironmentConfiguration\x12T\n\x0fpersonalization\x18\t \x01(\x0b\x32;.qwak.administration.environment.EnvironmentPersonalization\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"8\n%EnvironmentApplicationUserCredentials\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t*w\n\x15QwakEnvironmentStatus\x12\x1e\n\x1a\x45NVIRONMENT_STATUS_INVALID\x10\x00\x12\x1d\n\x19\x45NVIRONMENT_STATUS_ACTIVE\x10\x01\x12\x1f\n\x1b\x45NVIRONMENT_STATUS_DISABLED\x10\x02*L\n\x0b\x41\x63\x63ountTier\x12\x18\n\x14\x41\x43\x43OUNT_TIER_INVALID\x10\x00\x12\x08\n\x04\x46REE\x10\x01\x12\r\n\tVALIDATED\x10\x02\x12\n\n\x06PAYING\x10\x03\x42\xb2\x01\n\x1e\x63om.qwak.ai.administration.apiP\x01Z\x8d\x01github.com/qwak-ai/qwak-platform/services/core/java/user-management/user-management-api/pb/qwak/administration/v0/environments;environment_v0b\x06proto3')
 
 _QWAKENVIRONMENTSTATUS = DESCRIPTOR.enum_types_by_name['QwakEnvironmentStatus']
 QwakEnvironmentStatus = enum_type_wrapper.EnumTypeWrapper(_QWAKENVIRONMENTSTATUS)
+_ACCOUNTTIER = DESCRIPTOR.enum_types_by_name['AccountTier']
+AccountTier = enum_type_wrapper.EnumTypeWrapper(_ACCOUNTTIER)
 ENVIRONMENT_STATUS_INVALID = 0
 ENVIRONMENT_STATUS_ACTIVE = 1
 ENVIRONMENT_STATUS_DISABLED = 2
+ACCOUNT_TIER_INVALID = 0
+FREE = 1
+VALIDATED = 2
+PAYING = 3
 
 
 _QWAKENVIRONMENT = DESCRIPTOR.message_types_by_name['QwakEnvironment']
 _ENVIRONMENTAPPLICATIONUSERCREDENTIALS = DESCRIPTOR.message_types_by_name['EnvironmentApplicationUserCredentials']
 QwakEnvironment = _reflection.GeneratedProtocolMessageType('QwakEnvironment', (_message.Message,), {
   'DESCRIPTOR' : _QWAKENVIRONMENT,
   '__module__' : 'qwak.administration.v0.environments.environment_pb2'
@@ -45,14 +51,16 @@
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.qwak.ai.administration.apiP\001Z\215\001github.com/qwak-ai/qwak-platform/services/core/java/user-management/user-management-api/pb/qwak/administration/v0/environments;environment_v0'
   _QWAKENVIRONMENT.fields_by_name['tenant_id']._options = None
   _QWAKENVIRONMENT.fields_by_name['tenant_id']._serialized_options = b'\030\001'
-  _QWAKENVIRONMENTSTATUS._serialized_start=752
-  _QWAKENVIRONMENTSTATUS._serialized_end=871
+  _QWAKENVIRONMENTSTATUS._serialized_start=820
+  _QWAKENVIRONMENTSTATUS._serialized_end=939
+  _ACCOUNTTIER._serialized_start=941
+  _ACCOUNTTIER._serialized_end=1017
   _QWAKENVIRONMENT._serialized_start=240
-  _QWAKENVIRONMENT._serialized_end=692
-  _ENVIRONMENTAPPLICATIONUSERCREDENTIALS._serialized_start=694
-  _ENVIRONMENTAPPLICATIONUSERCREDENTIALS._serialized_end=750
+  _QWAKENVIRONMENT._serialized_end=760
+  _ENVIRONMENTAPPLICATIONUSERCREDENTIALS._serialized_start=762
+  _ENVIRONMENTAPPLICATIONUSERCREDENTIALS._serialized_end=818
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -38,28 +38,56 @@
 """Default invalid State"""
 ENVIRONMENT_STATUS_ACTIVE: QwakEnvironmentStatus.ValueType  # 1
 """Marks the environment is currently active for the linked tenant"""
 ENVIRONMENT_STATUS_DISABLED: QwakEnvironmentStatus.ValueType  # 2
 """Marks that the environment is no longer valid"""
 global___QwakEnvironmentStatus = QwakEnvironmentStatus
 
+class _AccountTier:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _AccountTierEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_AccountTier.ValueType], builtins.type):  # noqa: F821
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    ACCOUNT_TIER_INVALID: _AccountTier.ValueType  # 0
+    """Default invalid account tier"""
+    FREE: _AccountTier.ValueType  # 1
+    """Free account tier"""
+    VALIDATED: _AccountTier.ValueType  # 2
+    """Validated account tier"""
+    PAYING: _AccountTier.ValueType  # 3
+    """Paying account tier"""
+
+class AccountTier(_AccountTier, metaclass=_AccountTierEnumTypeWrapper): ...
+
+ACCOUNT_TIER_INVALID: AccountTier.ValueType  # 0
+"""Default invalid account tier"""
+FREE: AccountTier.ValueType  # 1
+"""Free account tier"""
+VALIDATED: AccountTier.ValueType  # 2
+"""Validated account tier"""
+PAYING: AccountTier.ValueType  # 3
+"""Paying account tier"""
+global___AccountTier = AccountTier
+
 class QwakEnvironment(google.protobuf.message.Message):
     """An environment configuration for a Qwak Tenant.
     Provides a layer of isolation / access control to for a single tenant. Can be used for modeling different lifecycle
     stages, such as - Prod, Dev, and Staging. But can also be used for separating projects and models between teams or
     organizational unit, in a way that every team / OU has its own environment.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     TENANT_ID_FIELD_NUMBER: builtins.int
     ACCOUNT_ID_FIELD_NUMBER: builtins.int
     CLUSTER_ID_FIELD_NUMBER: builtins.int
+    ACCOUNT_TIER_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     CONFIGURATION_FIELD_NUMBER: builtins.int
     PERSONALIZATION_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     LAST_MODIFIED_AT_FIELD_NUMBER: builtins.int
     id: builtins.str
     """Assigned environment ID"""
@@ -67,14 +95,16 @@
     """Given environment name"""
     tenant_id: builtins.str
     """Tenant ID which the environment is set up for (migrated to account id)"""
     account_id: builtins.str
     """Account ID which the environment is set up for (migrated to account id)"""
     cluster_id: builtins.str
     """Cluster ID which the environment is located in"""
+    account_tier: global___AccountTier.ValueType
+    """The account tier of the environment"""
     status: global___QwakEnvironmentStatus.ValueType
     """Current environment status"""
     @property
     def configuration(self) -> qwak.administration.v0.environments.configuration_pb2.QwakEnvironmentConfiguration:
         """Environment configuration"""
     @property
     def personalization(self) -> qwak.administration.v0.environments.personalization_pb2.EnvironmentPersonalization:
@@ -89,22 +119,23 @@
         self,
         *,
         id: builtins.str = ...,
         name: builtins.str = ...,
         tenant_id: builtins.str = ...,
         account_id: builtins.str = ...,
         cluster_id: builtins.str = ...,
+        account_tier: global___AccountTier.ValueType = ...,
         status: global___QwakEnvironmentStatus.ValueType = ...,
         configuration: qwak.administration.v0.environments.configuration_pb2.QwakEnvironmentConfiguration | None = ...,
         personalization: qwak.administration.v0.environments.personalization_pb2.EnvironmentPersonalization | None = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["configuration", b"configuration", "created_at", b"created_at", "last_modified_at", b"last_modified_at", "personalization", b"personalization"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["account_id", b"account_id", "cluster_id", b"cluster_id", "configuration", b"configuration", "created_at", b"created_at", "id", b"id", "last_modified_at", b"last_modified_at", "name", b"name", "personalization", b"personalization", "status", b"status", "tenant_id", b"tenant_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["account_id", b"account_id", "account_tier", b"account_tier", "cluster_id", b"cluster_id", "configuration", b"configuration", "created_at", b"created_at", "id", b"id", "last_modified_at", b"last_modified_at", "name", b"name", "personalization", b"personalization", "status", b"status", "tenant_id", b"tenant_id"]) -> None: ...
 
 global___QwakEnvironment = QwakEnvironment
 
 class EnvironmentApplicationUserCredentials(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     API_KEY_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eqwak/analytics/analytics.proto\x12\x0eqwak.analytics\"w\n\nResultData\x12\x0f\n\x07headers\x18\x01 \x03(\t\x12/\n\x0bheadersDesc\x18\x03 \x03(\x0b\x32\x1a.qwak.analytics.HeaderDesc\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.qwak.analytics.ResultRow\"(\n\nHeaderDesc\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x1b\n\tResultRow\x12\x0e\n\x06values\x18\x01 \x03(\t\":\n\x0bTableColumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07\x63omment\x18\x03 \x01(\t\"O\n\x15TableColumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12(\n\x04type\x18\x02 \x01(\x0e\x32\x1a.qwak.analytics.ColumnType\"\xe8\x01\n\x0fTableDefinition\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t\x12\x12\n\ntable_name\x18\x02 \x01(\t\x12\x36\n\x07\x63olumns\x18\x03 \x03(\x0b\x32%.qwak.analytics.TableColumnDefinition\x12\x11\n\tdata_path\x18\x04 \x01(\t\x12*\n\x06\x66ormat\x18\x05 \x01(\x0b\x32\x1a.qwak.analytics.DataFormat\x12\x39\n\npartitions\x18\x06 \x03(\x0b\x32%.qwak.analytics.TableColumnDefinition\"?\n\nDataFormat\x12\'\n\x03\x63sv\x18\x01 \x01(\x0b\x32\x18.qwak.analytics.CsvInputH\x00\x42\x08\n\x06\x66ormat\"F\n\x08\x43svInput\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\x12\n\nquote_char\x18\x02 \x01(\t\x12\x13\n\x0b\x65scape_char\x18\x03 \x01(\t\"0\n\x1cQueryResultDownloadURLParams\x12\x10\n\x08query_id\x18\x01 \x01(\t*N\n\x0bQueryStatus\x12\x0b\n\x07INVALID\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\x0c\n\x08\x43\x41NCELED\x10\x03\x12\n\n\x06\x46\x41ILED\x10\x04*\xad\x01\n\nColumnType\x12\x10\n\x0cINVALID_TYPE\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\x0b\n\x07TINYINT\x10\x02\x12\x0c\n\x08SMALLINT\x10\x03\x12\x07\n\x03INT\x10\x04\x12\n\n\x06\x42IGINT\x10\x05\x12\n\n\x06\x44OUBLE\x10\x06\x12\t\n\x05\x46LOAT\x10\x07\x12\x08\n\x04\x43HAR\x10\x08\x12\n\n\x06STRING\x10\t\x12\n\n\x06\x42INARY\x10\n\x12\x08\n\x04\x44\x41TE\x10\x0b\x12\r\n\tTIMESTAMP\x10\x0c\x42\x1d\n\x19\x63om.qwak.ai.analytics.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eqwak/analytics/analytics.proto\x12\x0eqwak.analytics\"w\n\nResultData\x12\x0f\n\x07headers\x18\x01 \x03(\t\x12/\n\x0bheadersDesc\x18\x03 \x03(\x0b\x32\x1a.qwak.analytics.HeaderDesc\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.qwak.analytics.ResultRow\"(\n\nHeaderDesc\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x1b\n\tResultRow\x12\x0e\n\x06values\x18\x01 \x03(\t\":\n\x0bTableColumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07\x63omment\x18\x03 \x01(\t\"O\n\x15TableColumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12(\n\x04type\x18\x02 \x01(\x0e\x32\x1a.qwak.analytics.ColumnType\"\xe8\x01\n\x0fTableDefinition\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t\x12\x12\n\ntable_name\x18\x02 \x01(\t\x12\x36\n\x07\x63olumns\x18\x03 \x03(\x0b\x32%.qwak.analytics.TableColumnDefinition\x12\x11\n\tdata_path\x18\x04 \x01(\t\x12*\n\x06\x66ormat\x18\x05 \x01(\x0b\x32\x1a.qwak.analytics.DataFormat\x12\x39\n\npartitions\x18\x06 \x03(\x0b\x32%.qwak.analytics.TableColumnDefinition\"?\n\nDataFormat\x12\'\n\x03\x63sv\x18\x01 \x01(\x0b\x32\x18.qwak.analytics.CsvInputH\x00\x42\x08\n\x06\x66ormat\"F\n\x08\x43svInput\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\x12\n\nquote_char\x18\x02 \x01(\t\x12\x13\n\x0b\x65scape_char\x18\x03 \x01(\t\"0\n\x1cQueryResultDownloadURLParams\x12\x10\n\x08query_id\x18\x01 \x01(\t*N\n\x0bQueryStatus\x12\x0b\n\x07INVALID\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\x0c\n\x08\x43\x41NCELED\x10\x03\x12\n\n\x06\x46\x41ILED\x10\x04*\xad\x01\n\nColumnType\x12\x10\n\x0cINVALID_TYPE\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\x0b\n\x07TINYINT\x10\x02\x12\x0c\n\x08SMALLINT\x10\x03\x12\x07\n\x03INT\x10\x04\x12\n\n\x06\x42IGINT\x10\x05\x12\n\n\x06\x44OUBLE\x10\x06\x12\t\n\x05\x46LOAT\x10\x07\x12\x08\n\x04\x43HAR\x10\x08\x12\n\n\x06STRING\x10\t\x12\n\n\x06\x42INARY\x10\n\x12\x08\n\x04\x44\x41TE\x10\x0b\x12\r\n\tTIMESTAMP\x10\x0c\x42\x86\x01\n\x19\x63om.qwak.ai.analytics.apiP\x01Zggithub.com/qwak-ai/qwak-platform/services/core/java/analytics/analytics-api/pb/qwak/analytics;analyticsb\x06proto3')
 
 _QUERYSTATUS = DESCRIPTOR.enum_types_by_name['QueryStatus']
 QueryStatus = enum_type_wrapper.EnumTypeWrapper(_QUERYSTATUS)
 _COLUMNTYPE = DESCRIPTOR.enum_types_by_name['ColumnType']
 ColumnType = enum_type_wrapper.EnumTypeWrapper(_COLUMNTYPE)
 INVALID = 0
 SUCCESS = 1
@@ -112,15 +112,15 @@
   # @@protoc_insertion_point(class_scope:qwak.analytics.QueryResultDownloadURLParams)
   })
 _sym_db.RegisterMessage(QueryResultDownloadURLParams)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\031com.qwak.ai.analytics.apiP\001'
+  DESCRIPTOR._serialized_options = b'\n\031com.qwak.ai.analytics.apiP\001Zggithub.com/qwak-ai/qwak-platform/services/core/java/analytics/analytics-api/pb/qwak/analytics;analytics'
   _QUERYSTATUS._serialized_start=805
   _QUERYSTATUS._serialized_end=883
   _COLUMNTYPE._serialized_start=886
   _COLUMNTYPE._serialized_end=1059
   _RESULTDATA._serialized_start=50
   _RESULTDATA._serialized_end=169
   _HEADERDESC._serialized_start=171
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.analytics import analytics_pb2 as qwak_dot_analytics_dot_analytics__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&qwak/analytics/analytics_service.proto\x12\x0eqwak.analytics\x1a\x1eqwak/analytics/analytics.proto\"\x1d\n\x0cQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"!\n\rQueryResponse\x12\x10\n\x08query_id\x18\x01 \x01(\t\"\'\n\x16\x45xecuteDdlQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"+\n\x17\x45xecuteDdlQueryResponse\x12\x10\n\x08query_id\x18\x01 \x01(\t\"T\n\x1aGetQueryResultsPageRequest\x12\x10\n\x08query_id\x18\x01 \x01(\t\x12\x0f\n\x07page_id\x18\x02 \x01(\t\x12\x13\n\x0bmax_results\x18\x03 \x01(\x05\"\xa2\x01\n\x1bGetQueryResultsPageResponse\x12+\n\x06status\x18\x01 \x01(\x0e\x32\x1b.qwak.analytics.QueryStatus\x12\x16\n\x0e\x66\x61ilure_reason\x18\x04 \x01(\t\x12\x14\n\x0cnext_page_id\x18\x02 \x01(\t\x12(\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1a.qwak.analytics.ResultData\")\n\x15GetQueryStatusRequest\x12\x10\n\x08query_id\x18\x01 \x01(\t\"]\n\x16GetQueryStatusResponse\x12+\n\x06status\x18\x01 \x01(\x0e\x32\x1b.qwak.analytics.QueryStatus\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"A\n\x14\x44\x65scribeTableRequest\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x15\n\rdatabase_name\x18\x02 \x01(\t\"Y\n\x15\x44\x65scribeTableResponse\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12,\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\x1b.qwak.analytics.TableColumn\"\x12\n\x10ListTableRequest\"(\n\x11ListTableResponse\x12\x13\n\x0btable_names\x18\x01 \x03(\t\"D\n\x12\x43reateTableRequest\x12.\n\x05table\x18\x01 \x01(\x0b\x32\x1f.qwak.analytics.TableDefinition\"\x15\n\x13\x43reateTableResponse\"`\n GetQueryResultDownloadURLRequest\x12<\n\x06params\x18\x01 \x01(\x0b\x32,.qwak.analytics.QueryResultDownloadURLParams\"9\n!GetQueryResultDownloadURLResponse\x12\x14\n\x0c\x64ownload_url\x18\x01 \x01(\t\"B\n\x14OptimizeTableRequest\x12\x16\n\x0e\x65nvironment_id\x18\x01 \x01(\t\x12\x12\n\ntable_name\x18\x02 \x01(\t\")\n\x15OptimizeTableResponse\x12\x10\n\x08query_id\x18\x01 \x01(\t2\xfc\x06\n\x15\x41nalyticsQueryService\x12\x44\n\x05Query\x12\x1c.qwak.analytics.QueryRequest\x1a\x1d.qwak.analytics.QueryResponse\x12\x62\n\x0f\x45xecuteDdlQuery\x12&.qwak.analytics.ExecuteDdlQueryRequest\x1a\'.qwak.analytics.ExecuteDdlQueryResponse\x12n\n\x13GetQueryResultsPage\x12*.qwak.analytics.GetQueryResultsPageRequest\x1a+.qwak.analytics.GetQueryResultsPageResponse\x12_\n\x0eGetQueryStatus\x12%.qwak.analytics.GetQueryStatusRequest\x1a&.qwak.analytics.GetQueryStatusResponse\x12\\\n\rDescribeTable\x12$.qwak.analytics.DescribeTableRequest\x1a%.qwak.analytics.DescribeTableResponse\x12Q\n\nListTables\x12 .qwak.analytics.ListTableRequest\x1a!.qwak.analytics.ListTableResponse\x12V\n\x0b\x43reateTable\x12\".qwak.analytics.CreateTableRequest\x1a#.qwak.analytics.CreateTableResponse\x12\x80\x01\n\x19GetQueryResultDownloadURL\x12\x30.qwak.analytics.GetQueryResultDownloadURLRequest\x1a\x31.qwak.analytics.GetQueryResultDownloadURLResponse\x12\\\n\rOptimizeTable\x12$.qwak.analytics.OptimizeTableRequest\x1a%.qwak.analytics.OptimizeTableResponseB\x1d\n\x19\x63om.qwak.ai.analytics.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&qwak/analytics/analytics_service.proto\x12\x0eqwak.analytics\x1a\x1eqwak/analytics/analytics.proto\"\x1d\n\x0cQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"!\n\rQueryResponse\x12\x10\n\x08query_id\x18\x01 \x01(\t\"\'\n\x16\x45xecuteDdlQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"+\n\x17\x45xecuteDdlQueryResponse\x12\x10\n\x08query_id\x18\x01 \x01(\t\"T\n\x1aGetQueryResultsPageRequest\x12\x10\n\x08query_id\x18\x01 \x01(\t\x12\x0f\n\x07page_id\x18\x02 \x01(\t\x12\x13\n\x0bmax_results\x18\x03 \x01(\x05\"\xa2\x01\n\x1bGetQueryResultsPageResponse\x12+\n\x06status\x18\x01 \x01(\x0e\x32\x1b.qwak.analytics.QueryStatus\x12\x16\n\x0e\x66\x61ilure_reason\x18\x04 \x01(\t\x12\x14\n\x0cnext_page_id\x18\x02 \x01(\t\x12(\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1a.qwak.analytics.ResultData\")\n\x15GetQueryStatusRequest\x12\x10\n\x08query_id\x18\x01 \x01(\t\"]\n\x16GetQueryStatusResponse\x12+\n\x06status\x18\x01 \x01(\x0e\x32\x1b.qwak.analytics.QueryStatus\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"A\n\x14\x44\x65scribeTableRequest\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x15\n\rdatabase_name\x18\x02 \x01(\t\"Y\n\x15\x44\x65scribeTableResponse\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12,\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\x1b.qwak.analytics.TableColumn\"\x12\n\x10ListTableRequest\"(\n\x11ListTableResponse\x12\x13\n\x0btable_names\x18\x01 \x03(\t\"D\n\x12\x43reateTableRequest\x12.\n\x05table\x18\x01 \x01(\x0b\x32\x1f.qwak.analytics.TableDefinition\"\x15\n\x13\x43reateTableResponse\"`\n GetQueryResultDownloadURLRequest\x12<\n\x06params\x18\x01 \x01(\x0b\x32,.qwak.analytics.QueryResultDownloadURLParams\"9\n!GetQueryResultDownloadURLResponse\x12\x14\n\x0c\x64ownload_url\x18\x01 \x01(\t\"B\n\x14OptimizeTableRequest\x12\x16\n\x0e\x65nvironment_id\x18\x01 \x01(\t\x12\x12\n\ntable_name\x18\x02 \x01(\t\")\n\x15OptimizeTableResponse\x12\x10\n\x08query_id\x18\x01 \x01(\t\".\n\x15\x43reateDatabaseRequest\x12\x15\n\rdatabase_name\x18\x01 \x01(\t\"\x18\n\x16\x43reateDatabaseResponse2\xdd\x07\n\x15\x41nalyticsQueryService\x12\x44\n\x05Query\x12\x1c.qwak.analytics.QueryRequest\x1a\x1d.qwak.analytics.QueryResponse\x12\x62\n\x0f\x45xecuteDdlQuery\x12&.qwak.analytics.ExecuteDdlQueryRequest\x1a\'.qwak.analytics.ExecuteDdlQueryResponse\x12n\n\x13GetQueryResultsPage\x12*.qwak.analytics.GetQueryResultsPageRequest\x1a+.qwak.analytics.GetQueryResultsPageResponse\x12_\n\x0eGetQueryStatus\x12%.qwak.analytics.GetQueryStatusRequest\x1a&.qwak.analytics.GetQueryStatusResponse\x12\\\n\rDescribeTable\x12$.qwak.analytics.DescribeTableRequest\x1a%.qwak.analytics.DescribeTableResponse\x12Q\n\nListTables\x12 .qwak.analytics.ListTableRequest\x1a!.qwak.analytics.ListTableResponse\x12V\n\x0b\x43reateTable\x12\".qwak.analytics.CreateTableRequest\x1a#.qwak.analytics.CreateTableResponse\x12\x80\x01\n\x19GetQueryResultDownloadURL\x12\x30.qwak.analytics.GetQueryResultDownloadURLRequest\x1a\x31.qwak.analytics.GetQueryResultDownloadURLResponse\x12\\\n\rOptimizeTable\x12$.qwak.analytics.OptimizeTableRequest\x1a%.qwak.analytics.OptimizeTableResponse\x12_\n\x0e\x43reateDatabase\x12%.qwak.analytics.CreateDatabaseRequest\x1a&.qwak.analytics.CreateDatabaseResponseB\x86\x01\n\x19\x63om.qwak.ai.analytics.apiP\x01Zggithub.com/qwak-ai/qwak-platform/services/core/java/analytics/analytics-api/pb/qwak/analytics;analyticsb\x06proto3')
 
 
 
 _QUERYREQUEST = DESCRIPTOR.message_types_by_name['QueryRequest']
 _QUERYRESPONSE = DESCRIPTOR.message_types_by_name['QueryResponse']
 _EXECUTEDDLQUERYREQUEST = DESCRIPTOR.message_types_by_name['ExecuteDdlQueryRequest']
 _EXECUTEDDLQUERYRESPONSE = DESCRIPTOR.message_types_by_name['ExecuteDdlQueryResponse']
@@ -33,14 +33,16 @@
 _LISTTABLERESPONSE = DESCRIPTOR.message_types_by_name['ListTableResponse']
 _CREATETABLEREQUEST = DESCRIPTOR.message_types_by_name['CreateTableRequest']
 _CREATETABLERESPONSE = DESCRIPTOR.message_types_by_name['CreateTableResponse']
 _GETQUERYRESULTDOWNLOADURLREQUEST = DESCRIPTOR.message_types_by_name['GetQueryResultDownloadURLRequest']
 _GETQUERYRESULTDOWNLOADURLRESPONSE = DESCRIPTOR.message_types_by_name['GetQueryResultDownloadURLResponse']
 _OPTIMIZETABLEREQUEST = DESCRIPTOR.message_types_by_name['OptimizeTableRequest']
 _OPTIMIZETABLERESPONSE = DESCRIPTOR.message_types_by_name['OptimizeTableResponse']
+_CREATEDATABASEREQUEST = DESCRIPTOR.message_types_by_name['CreateDatabaseRequest']
+_CREATEDATABASERESPONSE = DESCRIPTOR.message_types_by_name['CreateDatabaseResponse']
 QueryRequest = _reflection.GeneratedProtocolMessageType('QueryRequest', (_message.Message,), {
   'DESCRIPTOR' : _QUERYREQUEST,
   '__module__' : 'qwak.analytics.analytics_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.analytics.QueryRequest)
   })
 _sym_db.RegisterMessage(QueryRequest)
 
@@ -159,19 +161,33 @@
 OptimizeTableResponse = _reflection.GeneratedProtocolMessageType('OptimizeTableResponse', (_message.Message,), {
   'DESCRIPTOR' : _OPTIMIZETABLERESPONSE,
   '__module__' : 'qwak.analytics.analytics_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.analytics.OptimizeTableResponse)
   })
 _sym_db.RegisterMessage(OptimizeTableResponse)
 
+CreateDatabaseRequest = _reflection.GeneratedProtocolMessageType('CreateDatabaseRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEDATABASEREQUEST,
+  '__module__' : 'qwak.analytics.analytics_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.analytics.CreateDatabaseRequest)
+  })
+_sym_db.RegisterMessage(CreateDatabaseRequest)
+
+CreateDatabaseResponse = _reflection.GeneratedProtocolMessageType('CreateDatabaseResponse', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEDATABASERESPONSE,
+  '__module__' : 'qwak.analytics.analytics_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.analytics.CreateDatabaseResponse)
+  })
+_sym_db.RegisterMessage(CreateDatabaseResponse)
+
 _ANALYTICSQUERYSERVICE = DESCRIPTOR.services_by_name['AnalyticsQueryService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\031com.qwak.ai.analytics.apiP\001'
+  DESCRIPTOR._serialized_options = b'\n\031com.qwak.ai.analytics.apiP\001Zggithub.com/qwak-ai/qwak-platform/services/core/java/analytics/analytics-api/pb/qwak/analytics;analytics'
   _QUERYREQUEST._serialized_start=90
   _QUERYREQUEST._serialized_end=119
   _QUERYRESPONSE._serialized_start=121
   _QUERYRESPONSE._serialized_end=154
   _EXECUTEDDLQUERYREQUEST._serialized_start=156
   _EXECUTEDDLQUERYREQUEST._serialized_end=195
   _EXECUTEDDLQUERYRESPONSE._serialized_start=197
@@ -200,10 +216,14 @@
   _GETQUERYRESULTDOWNLOADURLREQUEST._serialized_end=1040
   _GETQUERYRESULTDOWNLOADURLRESPONSE._serialized_start=1042
   _GETQUERYRESULTDOWNLOADURLRESPONSE._serialized_end=1099
   _OPTIMIZETABLEREQUEST._serialized_start=1101
   _OPTIMIZETABLEREQUEST._serialized_end=1167
   _OPTIMIZETABLERESPONSE._serialized_start=1169
   _OPTIMIZETABLERESPONSE._serialized_end=1210
-  _ANALYTICSQUERYSERVICE._serialized_start=1213
-  _ANALYTICSQUERYSERVICE._serialized_end=2105
+  _CREATEDATABASEREQUEST._serialized_start=1212
+  _CREATEDATABASEREQUEST._serialized_end=1258
+  _CREATEDATABASERESPONSE._serialized_start=1260
+  _CREATEDATABASERESPONSE._serialized_end=1284
+  _ANALYTICSQUERYSERVICE._serialized_start=1287
+  _ANALYTICSQUERYSERVICE._serialized_end=2276
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -310,7 +310,30 @@
         self,
         *,
         query_id: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["query_id", b"query_id"]) -> None: ...
 
 global___OptimizeTableResponse = OptimizeTableResponse
+
+class CreateDatabaseRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DATABASE_NAME_FIELD_NUMBER: builtins.int
+    database_name: builtins.str
+    def __init__(
+        self,
+        *,
+        database_name: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["database_name", b"database_name"]) -> None: ...
+
+global___CreateDatabaseRequest = CreateDatabaseRequest
+
+class CreateDatabaseResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___CreateDatabaseResponse = CreateDatabaseResponse
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,19 @@
                 response_deserializer=qwak_dot_analytics_dot_analytics__service__pb2.GetQueryResultDownloadURLResponse.FromString,
                 )
         self.OptimizeTable = channel.unary_unary(
                 '/qwak.analytics.AnalyticsQueryService/OptimizeTable',
                 request_serializer=qwak_dot_analytics_dot_analytics__service__pb2.OptimizeTableRequest.SerializeToString,
                 response_deserializer=qwak_dot_analytics_dot_analytics__service__pb2.OptimizeTableResponse.FromString,
                 )
+        self.CreateDatabase = channel.unary_unary(
+                '/qwak.analytics.AnalyticsQueryService/CreateDatabase',
+                request_serializer=qwak_dot_analytics_dot_analytics__service__pb2.CreateDatabaseRequest.SerializeToString,
+                response_deserializer=qwak_dot_analytics_dot_analytics__service__pb2.CreateDatabaseResponse.FromString,
+                )
 
 
 class AnalyticsQueryServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Query(self, request, context):
         """Initiates a query request from the user. Returns a query ID which the client should start subscribing on
@@ -121,14 +126,20 @@
 
     def OptimizeTable(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def CreateDatabase(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_AnalyticsQueryServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Query': grpc.unary_unary_rpc_method_handler(
                     servicer.Query,
                     request_deserializer=qwak_dot_analytics_dot_analytics__service__pb2.QueryRequest.FromString,
                     response_serializer=qwak_dot_analytics_dot_analytics__service__pb2.QueryResponse.SerializeToString,
@@ -169,14 +180,19 @@
                     response_serializer=qwak_dot_analytics_dot_analytics__service__pb2.GetQueryResultDownloadURLResponse.SerializeToString,
             ),
             'OptimizeTable': grpc.unary_unary_rpc_method_handler(
                     servicer.OptimizeTable,
                     request_deserializer=qwak_dot_analytics_dot_analytics__service__pb2.OptimizeTableRequest.FromString,
                     response_serializer=qwak_dot_analytics_dot_analytics__service__pb2.OptimizeTableResponse.SerializeToString,
             ),
+            'CreateDatabase': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateDatabase,
+                    request_deserializer=qwak_dot_analytics_dot_analytics__service__pb2.CreateDatabaseRequest.FromString,
+                    response_serializer=qwak_dot_analytics_dot_analytics__service__pb2.CreateDatabaseResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'qwak.analytics.AnalyticsQueryService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -331,7 +347,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/qwak.analytics.AnalyticsQueryService/OptimizeTable',
             qwak_dot_analytics_dot_analytics__service__pb2.OptimizeTableRequest.SerializeToString,
             qwak_dot_analytics_dot_analytics__service__pb2.OptimizeTableResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateDatabase(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qwak.analytics.AnalyticsQueryService/CreateDatabase',
+            qwak_dot_analytics_dot_analytics__service__pb2.CreateDatabaseRequest.SerializeToString,
+            qwak_dot_analytics_dot_analytics__service__pb2.CreateDatabaseResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(qwak/batch_job/v1/batch_job_events.proto\x12\rqwak.batchjob\x1a/qwak/user_application/common/v0/resources.proto\"\xa5\x01\n\x14\x42\x61tchJobEventMessage\x12\x45\n\x14\x62\x61tch_job_event_type\x18\x01 \x01(\x0e\x32\'.qwak.batchjob.BatchJobEventTypeMessage\x12\x14\n\x0c\x62\x61tch_job_id\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\r\n\x05\x64\x65lay\x18\x04 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x05 \x01(\x05\"\x84\x02\n\x15\x42\x61tchTaskEventMessage\x12G\n\x15\x62\x61tch_task_event_type\x18\x01 \x01(\x0e\x32(.qwak.batchjob.BatchTaskEventTypeMessage\x12\x14\n\x0c\x62\x61tch_job_id\x18\x02 \x01(\t\x12\x15\n\rbatch_task_id\x18\x03 \x01(\t\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\r\n\x05\x64\x65lay\x18\x05 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x06 \x01(\x05\x12\x43\n\x19\x62\x61tch_task_failure_reason\x18\x07 \x01(\x0b\x32 .qwak.batchjob.TaskFailureReason\"\xec\x01\n\x12WarmupEventMessage\x12\x44\n\x15warmup_job_event_type\x18\x01 \x01(\x0e\x32%.qwak.batchjob.WarmupEventTypeMessage\x12\r\n\x05\x64\x65lay\x18\x02 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x03 \x01(\x05\x12.\n\x0bwarmup_size\x18\x04 \x01(\x0b\x32\x19.qwak.batchjob.WarmupSize\x12?\n\x10model_identifier\x18\x05 \x01(\x0b\x32%.qwak.batchjob.ModelIdentifierMessage\"\xb9\x02\n\nWarmupSize\x12\x0f\n\x03\x63pu\x18\x01 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x32\n\x0bmemory_unit\x18\x03 \x01(\x0e\x32\x19.qwak.batchjob.MemoryUnitB\x02\x18\x01\x12\x13\n\x0bnum_of_pods\x18\x04 \x01(\x05\x12\x17\n\x0ftimeout_seconds\x18\x05 \x01(\x05\x12H\n\rgpu_resources\x18\x06 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesB\x02\x18\x01\x12S\n\x15pod_compute_resources\x18\x07 \x01(\x0b\x32\x34.qwak.user_application.common.v0.PodComputeResources\"\x90\x01\n\x16ModelIdentifierMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x05 \x01(\t\x12\x12\n\naccount_id\x18\x06 \x01(\t\"\x80\x01\n\x11TaskFailureReason\x12\x46\n\x18task_failure_reason_code\x18\x01 \x01(\x0e\x32$.qwak.batchjob.TaskFailureReasonCode\x12#\n\x1btask_failure_reason_details\x18\x02 \x01(\t*\xf2\x01\n\x18\x42\x61tchJobEventTypeMessage\x12\x1d\n\x19UNDEFINED_BATCH_JOB_EVENT\x10\x00\x12\x17\n\x13\x42\x41TCH_JOB_COMMITTED\x10\x01\x12\x16\n\x12\x42\x41TCH_JOB_PREPARED\x10\x07\x12\x1b\n\x17\x42\x41TCH_JOB_TASKS_CREATED\x10\x02\x12\x17\n\x13\x42\x41TCH_JOB_CANCELLED\x10\x03\x12\x15\n\x11\x42\x41TCH_JOB_CLEANUP\x10\x04\x12\x1c\n\x18\x42\x41TCH_JOB_CHECK_FINISHED\x10\x05\x12\x1b\n\x17\x42\x41TCH_JOB_CHECK_TIMEOUT\x10\x06*\xce\x01\n\x19\x42\x61tchTaskEventTypeMessage\x12\x1e\n\x1aUNDEFINED_BATCH_TASK_EVENT\x10\x00\x12\x16\n\x12\x42\x41TCH_TASK_RUNNING\x10\x01\x12\x17\n\x13\x42\x41TCH_TASK_FINISHED\x10\x02\x12\x15\n\x11\x42\x41TCH_TASK_FAILED\x10\x03\x12\x1b\n\x17\x42\x41TCH_TASK_CHECK_STATUS\x10\x04\x12\x14\n\x10\x42\x41TCH_TASK_START\x10\x05\x12\x16\n\x12\x42\x41TCH_TASK_CLEANUP\x10\x06*e\n\x16WarmupEventTypeMessage\x12\x1e\n\x1aUNDEFINED_WARMUP_JOB_EVENT\x10\x00\x12\x18\n\x14WARMUP_JOB_COMMITTED\x10\x01\x12\x11\n\rWARMUP_CANCEL\x10\x02*+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\xc0\x04\n\x15TaskFailureReasonCode\x12\x35\n1TASK_FAILURE_REASON_CODE_FAILURE_CODE_UNSPECIFIED\x10\x00\x12\x44\n@TASK_FAILURE_REASON_CODE_NO_REPLICA_SETS_PODS_FOUND_FAILURE_CODE\x10\x01\x12\x43\n?TASK_FAILURE_REASON_CODE_MODEL_CONTAINER_NOT_FOUND_FAILURE_CODE\x10\x02\x12\x37\n3TASK_FAILURE_REASON_CODE_UNSCHEDULABLE_FAILURE_CODE\x10\x03\x12@\n<TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_NOT_FOUND_FAILURE_CODE\x10\x04\x12?\n;TASK_FAILURE_REASON_CODE_MEMORY_LIMIT_EXCEEDED_FAILURE_CODE\x10\x05\x12\x34\n0TASK_FAILURE_REASON_CODE_CRASH_LOOP_FAILURE_CODE\x10\x06\x12\x46\nBTASK_FAILURE_REASON_CODE_CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON\x10\x07\x12+\n\'TASK_FAILURE_REASON_CODE_UNKNOWN_REASON\x10\x08\x42.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(qwak/batch_job/v1/batch_job_events.proto\x12\rqwak.batchjob\x1a/qwak/user_application/common/v0/resources.proto\"\xa5\x01\n\x14\x42\x61tchJobEventMessage\x12\x45\n\x14\x62\x61tch_job_event_type\x18\x01 \x01(\x0e\x32\'.qwak.batchjob.BatchJobEventTypeMessage\x12\x14\n\x0c\x62\x61tch_job_id\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\r\n\x05\x64\x65lay\x18\x04 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x05 \x01(\x05\"\x84\x02\n\x15\x42\x61tchTaskEventMessage\x12G\n\x15\x62\x61tch_task_event_type\x18\x01 \x01(\x0e\x32(.qwak.batchjob.BatchTaskEventTypeMessage\x12\x14\n\x0c\x62\x61tch_job_id\x18\x02 \x01(\t\x12\x15\n\rbatch_task_id\x18\x03 \x01(\t\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\r\n\x05\x64\x65lay\x18\x05 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x06 \x01(\x05\x12\x43\n\x19\x62\x61tch_task_failure_reason\x18\x07 \x01(\x0b\x32 .qwak.batchjob.TaskFailureReason\"\xec\x01\n\x12WarmupEventMessage\x12\x44\n\x15warmup_job_event_type\x18\x01 \x01(\x0e\x32%.qwak.batchjob.WarmupEventTypeMessage\x12\r\n\x05\x64\x65lay\x18\x02 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x03 \x01(\x05\x12.\n\x0bwarmup_size\x18\x04 \x01(\x0b\x32\x19.qwak.batchjob.WarmupSize\x12?\n\x10model_identifier\x18\x05 \x01(\x0b\x32%.qwak.batchjob.ModelIdentifierMessage\"\xb9\x02\n\nWarmupSize\x12\x0f\n\x03\x63pu\x18\x01 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x32\n\x0bmemory_unit\x18\x03 \x01(\x0e\x32\x19.qwak.batchjob.MemoryUnitB\x02\x18\x01\x12\x13\n\x0bnum_of_pods\x18\x04 \x01(\x05\x12\x17\n\x0ftimeout_seconds\x18\x05 \x01(\x05\x12H\n\rgpu_resources\x18\x06 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesB\x02\x18\x01\x12S\n\x15pod_compute_resources\x18\x07 \x01(\x0b\x32\x34.qwak.user_application.common.v0.PodComputeResources\"\x90\x01\n\x16ModelIdentifierMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x05 \x01(\t\x12\x12\n\naccount_id\x18\x06 \x01(\t\"\x80\x01\n\x11TaskFailureReason\x12\x46\n\x18task_failure_reason_code\x18\x01 \x01(\x0e\x32$.qwak.batchjob.TaskFailureReasonCode\x12#\n\x1btask_failure_reason_details\x18\x02 \x01(\t*\xf2\x01\n\x18\x42\x61tchJobEventTypeMessage\x12\x1d\n\x19UNDEFINED_BATCH_JOB_EVENT\x10\x00\x12\x17\n\x13\x42\x41TCH_JOB_COMMITTED\x10\x01\x12\x16\n\x12\x42\x41TCH_JOB_PREPARED\x10\x07\x12\x1b\n\x17\x42\x41TCH_JOB_TASKS_CREATED\x10\x02\x12\x17\n\x13\x42\x41TCH_JOB_CANCELLED\x10\x03\x12\x15\n\x11\x42\x41TCH_JOB_CLEANUP\x10\x04\x12\x1c\n\x18\x42\x41TCH_JOB_CHECK_FINISHED\x10\x05\x12\x1b\n\x17\x42\x41TCH_JOB_CHECK_TIMEOUT\x10\x06*\xce\x01\n\x19\x42\x61tchTaskEventTypeMessage\x12\x1e\n\x1aUNDEFINED_BATCH_TASK_EVENT\x10\x00\x12\x16\n\x12\x42\x41TCH_TASK_RUNNING\x10\x01\x12\x17\n\x13\x42\x41TCH_TASK_FINISHED\x10\x02\x12\x15\n\x11\x42\x41TCH_TASK_FAILED\x10\x03\x12\x1b\n\x17\x42\x41TCH_TASK_CHECK_STATUS\x10\x04\x12\x14\n\x10\x42\x41TCH_TASK_START\x10\x05\x12\x16\n\x12\x42\x41TCH_TASK_CLEANUP\x10\x06*e\n\x16WarmupEventTypeMessage\x12\x1e\n\x1aUNDEFINED_WARMUP_JOB_EVENT\x10\x00\x12\x18\n\x14WARMUP_JOB_COMMITTED\x10\x01\x12\x11\n\rWARMUP_CANCEL\x10\x02*+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x9a\x05\n\x15TaskFailureReasonCode\x12\x35\n1TASK_FAILURE_REASON_CODE_FAILURE_CODE_UNSPECIFIED\x10\x00\x12\x44\n@TASK_FAILURE_REASON_CODE_NO_REPLICA_SETS_PODS_FOUND_FAILURE_CODE\x10\x01\x12\x43\n?TASK_FAILURE_REASON_CODE_MODEL_CONTAINER_NOT_FOUND_FAILURE_CODE\x10\x02\x12\x37\n3TASK_FAILURE_REASON_CODE_UNSCHEDULABLE_FAILURE_CODE\x10\x03\x12@\n<TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_NOT_FOUND_FAILURE_CODE\x10\x04\x12?\n;TASK_FAILURE_REASON_CODE_MEMORY_LIMIT_EXCEEDED_FAILURE_CODE\x10\x05\x12\x34\n0TASK_FAILURE_REASON_CODE_CRASH_LOOP_FAILURE_CODE\x10\x06\x12\x46\nBTASK_FAILURE_REASON_CODE_CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON\x10\x07\x12+\n\'TASK_FAILURE_REASON_CODE_UNKNOWN_REASON\x10\x08\x12X\nTTASK_FAILURE_REASON_CODE_DOCKER_IMAGE_GETS_THROTTLING_BY_CLOUD_PROVIDER_FAILURE_CODE\x10\tB.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
 
 _BATCHJOBEVENTTYPEMESSAGE = DESCRIPTOR.enum_types_by_name['BatchJobEventTypeMessage']
 BatchJobEventTypeMessage = enum_type_wrapper.EnumTypeWrapper(_BATCHJOBEVENTTYPEMESSAGE)
 _BATCHTASKEVENTTYPEMESSAGE = DESCRIPTOR.enum_types_by_name['BatchTaskEventTypeMessage']
 BatchTaskEventTypeMessage = enum_type_wrapper.EnumTypeWrapper(_BATCHTASKEVENTTYPEMESSAGE)
 _WARMUPEVENTTYPEMESSAGE = DESCRIPTOR.enum_types_by_name['WarmupEventTypeMessage']
 WarmupEventTypeMessage = enum_type_wrapper.EnumTypeWrapper(_WARMUPEVENTTYPEMESSAGE)
@@ -54,14 +54,15 @@
 TASK_FAILURE_REASON_CODE_MODEL_CONTAINER_NOT_FOUND_FAILURE_CODE = 2
 TASK_FAILURE_REASON_CODE_UNSCHEDULABLE_FAILURE_CODE = 3
 TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_NOT_FOUND_FAILURE_CODE = 4
 TASK_FAILURE_REASON_CODE_MEMORY_LIMIT_EXCEEDED_FAILURE_CODE = 5
 TASK_FAILURE_REASON_CODE_CRASH_LOOP_FAILURE_CODE = 6
 TASK_FAILURE_REASON_CODE_CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON = 7
 TASK_FAILURE_REASON_CODE_UNKNOWN_REASON = 8
+TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_GETS_THROTTLING_BY_CLOUD_PROVIDER_FAILURE_CODE = 9
 
 
 _BATCHJOBEVENTMESSAGE = DESCRIPTOR.message_types_by_name['BatchJobEventMessage']
 _BATCHTASKEVENTMESSAGE = DESCRIPTOR.message_types_by_name['BatchTaskEventMessage']
 _WARMUPEVENTMESSAGE = DESCRIPTOR.message_types_by_name['WarmupEventMessage']
 _WARMUPSIZE = DESCRIPTOR.message_types_by_name['WarmupSize']
 _MODELIDENTIFIERMESSAGE = DESCRIPTOR.message_types_by_name['ModelIdentifierMessage']
@@ -127,15 +128,15 @@
   _BATCHTASKEVENTTYPEMESSAGE._serialized_start=1618
   _BATCHTASKEVENTTYPEMESSAGE._serialized_end=1824
   _WARMUPEVENTTYPEMESSAGE._serialized_start=1826
   _WARMUPEVENTTYPEMESSAGE._serialized_end=1927
   _MEMORYUNIT._serialized_start=1929
   _MEMORYUNIT._serialized_end=1972
   _TASKFAILUREREASONCODE._serialized_start=1975
-  _TASKFAILUREREASONCODE._serialized_end=2551
+  _TASKFAILUREREASONCODE._serialized_end=2641
   _BATCHJOBEVENTMESSAGE._serialized_start=109
   _BATCHJOBEVENTMESSAGE._serialized_end=274
   _BATCHTASKEVENTMESSAGE._serialized_start=277
   _BATCHTASKEVENTMESSAGE._serialized_end=537
   _WARMUPEVENTMESSAGE._serialized_start=540
   _WARMUPEVENTMESSAGE._serialized_end=776
   _WARMUPSIZE._serialized_start=779
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -114,26 +114,28 @@
     TASK_FAILURE_REASON_CODE_MODEL_CONTAINER_NOT_FOUND_FAILURE_CODE: _TaskFailureReasonCode.ValueType  # 2
     TASK_FAILURE_REASON_CODE_UNSCHEDULABLE_FAILURE_CODE: _TaskFailureReasonCode.ValueType  # 3
     TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_NOT_FOUND_FAILURE_CODE: _TaskFailureReasonCode.ValueType  # 4
     TASK_FAILURE_REASON_CODE_MEMORY_LIMIT_EXCEEDED_FAILURE_CODE: _TaskFailureReasonCode.ValueType  # 5
     TASK_FAILURE_REASON_CODE_CRASH_LOOP_FAILURE_CODE: _TaskFailureReasonCode.ValueType  # 6
     TASK_FAILURE_REASON_CODE_CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON: _TaskFailureReasonCode.ValueType  # 7
     TASK_FAILURE_REASON_CODE_UNKNOWN_REASON: _TaskFailureReasonCode.ValueType  # 8
+    TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_GETS_THROTTLING_BY_CLOUD_PROVIDER_FAILURE_CODE: _TaskFailureReasonCode.ValueType  # 9
 
 class TaskFailureReasonCode(_TaskFailureReasonCode, metaclass=_TaskFailureReasonCodeEnumTypeWrapper): ...
 
 TASK_FAILURE_REASON_CODE_FAILURE_CODE_UNSPECIFIED: TaskFailureReasonCode.ValueType  # 0
 TASK_FAILURE_REASON_CODE_NO_REPLICA_SETS_PODS_FOUND_FAILURE_CODE: TaskFailureReasonCode.ValueType  # 1
 TASK_FAILURE_REASON_CODE_MODEL_CONTAINER_NOT_FOUND_FAILURE_CODE: TaskFailureReasonCode.ValueType  # 2
 TASK_FAILURE_REASON_CODE_UNSCHEDULABLE_FAILURE_CODE: TaskFailureReasonCode.ValueType  # 3
 TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_NOT_FOUND_FAILURE_CODE: TaskFailureReasonCode.ValueType  # 4
 TASK_FAILURE_REASON_CODE_MEMORY_LIMIT_EXCEEDED_FAILURE_CODE: TaskFailureReasonCode.ValueType  # 5
 TASK_FAILURE_REASON_CODE_CRASH_LOOP_FAILURE_CODE: TaskFailureReasonCode.ValueType  # 6
 TASK_FAILURE_REASON_CODE_CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON: TaskFailureReasonCode.ValueType  # 7
 TASK_FAILURE_REASON_CODE_UNKNOWN_REASON: TaskFailureReasonCode.ValueType  # 8
+TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_GETS_THROTTLING_BY_CLOUD_PROVIDER_FAILURE_CODE: TaskFailureReasonCode.ValueType  # 9
 global___TaskFailureReasonCode = TaskFailureReasonCode
 
 class BatchJobEventMessage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BATCH_JOB_EVENT_TYPE_FIELD_NUMBER: builtins.int
     BATCH_JOB_ID_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 from _qwak_proto.qwak.batch_job.v1 import batch_job_events_pb2 as qwak_dot_batch__job_dot_v1_dot_batch__job__events__pb2
 from _qwak_proto.qwak.administration.authenticated_user.v1 import credentials_pb2 as qwak_dot_administration_dot_authenticated__user_dot_v1_dot_credentials__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)qwak/batch_job/v1/batch_job_service.proto\x12\rqwak.batchjob\x1a\x1fgoogle/protobuf/timestamp.proto\x1a/qwak/user_application/common/v0/resources.proto\x1a(qwak/batch_job/v1/batch_job_events.proto\x1a;qwak/administration/authenticated_user/v1/credentials.proto\"\xb4\x01\n\x15StartWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x05 \x01(\t\x12\x16\n\x0ewarmup_timeout\x18\x03 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x04 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\"B\n\x16StartWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"S\n\x16\x43\x61ncelWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\"C\n\x17\x43\x61ncelWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"\x89\x05\n\x14StartBatchJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\x12\x15\n\rsource_bucket\x18\x03 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x04 \x01(\t\x12\x15\n\rsource_folder\x18\x05 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x06 \x01(\t\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12\x13\n\x0bjob_timeout\x18\x08 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\t \x01(\x05\x12\x35\n\x0finput_file_type\x18\n \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x0b \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x0e \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x10 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\x12\x39\n\x11\x62\x61tch_job_request\x18\x11 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobRequest\"\xcb\x01\n\x0f\x42\x61tchJobRequest\x12:\n\rmodel_details\x18\x01 \x01(\x0b\x32#.qwak.batchjob.BatchJobModelDetails\x12\x38\n\x0c\x64\x61ta_details\x18\x02 \x01(\x0b\x32\".qwak.batchjob.BatchJobDataDetails\x12\x42\n\x11\x65xecution_details\x18\x04 \x01(\x0b\x32\'.qwak.batchjob.BatchJobExecutionDetails\":\n\x14\x42\x61tchJobModelDetails\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\"\xe5\x01\n\x13\x42\x61tchJobDataDetails\x12\x36\n\x0bsource_path\x18\x01 \x01(\x0b\x32!.qwak.batchjob.BatchJobSourcePath\x12@\n\x10\x64\x65stination_path\x18\x02 \x01(\x0b\x32&.qwak.batchjob.BatchJobDestinationPath\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\x12\'\n\x1fservice_account_json_key_secret\x18\x05 \x01(\t\"y\n\x12\x42\x61tchJobSourcePath\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x15\n\rsource_folder\x18\x02 \x01(\t\x12\x35\n\x0finput_file_type\x18\x03 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\"\x8a\x01\n\x17\x42\x61tchJobDestinationPath\x12\x1a\n\x12\x64\x65stination_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x02 \x01(\t\x12\x37\n\x10output_file_type\x18\x03 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\"\x94\x02\n\x18\x42\x61tchJobExecutionDetails\x12\x13\n\x0bjob_timeout\x18\x01 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\x02 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x05 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\"/\n\x11\x42\x61tchJobParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"S\n\x15StartBatchJobResponse\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\")\n\x15\x43\x61ncelBatchJobRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"B\n\x16\x43\x61ncelBatchJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\",\n\x18GetBatchJobStatusRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"\xac\x01\n\x19GetBatchJobStatusResponse\x12\x38\n\njob_status\x18\x01 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\x12\x16\n\x0e\x66inished_files\x18\x04 \x01(\x05\x12\x13\n\x0btotal_files\x18\x05 \x01(\x05\",\n\x18GetBatchJobReportRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"a\n\x19GetBatchJobReportResponse\x12\x12\n\nsuccessful\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\x12\x17\n\x0freport_messages\x18\x03 \x03(\t\"`\n\x1dUpdateBatchTasksStatusRequest\x12?\n\x11\x62\x61tch_task_events\x18\x01 \x03(\x0b\x32$.qwak.batchjob.BatchTaskEventMessage\"I\n\x1dUpdateBatchTaskStatusResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"Q\n\x19\x41\x64vancedDeploymentOptions\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x01 \x01(\t\x12\x17\n\x0fpurchase_option\x18\x02 \x01(\t\"\x85\x03\n\x16\x42\x61tchJobDeploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0f\n\x03\x63pu\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x03 \x01(\x05\x42\x02\x18\x01\x12J\n\x0cmemory_units\x18\x04 \x01(\x0e\x32\x30.qwak.batchjob.BatchJobDeploymentSize.MemoryUnitB\x02\x18\x01\x12H\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesB\x02\x18\x01\x12`\n\x1c\x63lient_pod_compute_resources\x18\x06 \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResources\"/\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02\x1a\x02\x18\x01\"\x99\x01\n\x15\x42\x61tchJobExecutionSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12S\n\x15pod_compute_resources\x18\x02 \x01(\x0b\x32\x34.qwak.user_application.common.v0.PodComputeResources\x12\x13\n\x0btemplate_id\x18\x03 \x01(\t\"Q\n\x14ListBatchJobsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\"K\n\x15ListBatchJobsResponse\x12\x32\n\nbatch_jobs\x18\x01 \x03(\x0b\x32\x1e.qwak.batchjob.BatchJobDetails\"\x81\x03\n\x0f\x42\x61tchJobDetails\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x38\n\njob_status\x18\x03 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\x12;\n\x08job_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSizeB\x02\x18\x01\x12\x46\n\x18\x62\x61tch_job_execution_size\x18\x08 \x01(\x0b\x32$.qwak.batchjob.BatchJobExecutionSize\x12\x16\n\x0e\x65nvironment_id\x18\t \x01(\t\"+\n\x19GetBatchJobDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"y\n\x1aGetBatchJobDetailsResponse\x12\x31\n\tbatch_job\x18\x01 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"\x84\x04\n\x0f\x42\x61tchJobMessage\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\tbranch_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\njob_status\x18\x07 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x15\n\rtotal_records\x18\x08 \x01(\x05\x12\x37\n\x08job_size\x18\t \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12;\n\x0freport_messages\x18\n \x03(\x0b\x32\".qwak.batchjob.ExecutionReportLine\x12\x43\n\x16\x65xecution_file_details\x18\x0b \x01(\x0b\x32#.qwak.batchjob.ExecutionFileDetails\x12<\n\x0ftask_executions\x18\x0c \x03(\x0b\x32#.qwak.batchjob.TaskExecutionDetails\"M\n\x13\x45xecutionReportLine\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04line\x18\x02 \x01(\t\"\x95\x02\n\x14\x45xecutionFileDetails\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x02 \x01(\t\x12\x13\n\x0bsource_path\x18\x03 \x01(\t\x12\x18\n\x10\x64\x65stination_path\x18\x04 \x01(\t\x12\x35\n\x0finput_file_type\x18\x05 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x06 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x16\n\x0e\x66inished_files\x18\x07 \x01(\x05\x12\x13\n\x0btotal_files\x18\x08 \x01(\x05\"\xe6\x01\n\x14TaskExecutionDetails\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.qwak.batchjob.BatchTaskStatusMessage\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0enum_of_records\x18\x05 \x01(\x05\x12\x10\n\x08\x66ilename\x18\x06 \x01(\t\"d\n$GetBatchJobPreSignedUploadUrlRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x17\n\x0fnumber_of_files\x18\x02 \x01(\x05\x12\x11\n\tfile_type\x18\x03 \x01(\t\"\x98\x01\n%GetBatchJobPreSignedUploadUrlResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12\x0c\n\x04urls\x18\x04 \x03(\t\x12\x0f\n\x07success\x18\x05 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\"8\n&GetBatchJobPreSignedDownloadUrlRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"a\n\'GetBatchJobPreSignedDownloadUrlResponse\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"3\n\x1fGetBatchJobUploadDetailsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\xb4\x01\n GetBatchJobUploadDetailsResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12W\n\x0b\x63redentials\x18\x04 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"3\n!GetBatchJobDownloadDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"\x9b\x01\n\"GetBatchJobDownloadDetailsResponse\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12W\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"\xd7\x01\n\x1aUpdateDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x46\n\x17\x64\x65\x66\x61ult_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\"\x1d\n\x1bUpdateDefaultParamsResponse\".\n\x1a\x44\x65leteDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\x1d\n\x1b\x44\x65leteDefaultParamsResponse\"S\n&UpdateTaskIngestedRecordsAmountRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x18\n\x10ingested_records\x18\x02 \x01(\x03\")\n\'UpdateTaskIngestedRecordsAmountResponse*\x81\x01\n\rInputFileType\x12\x1d\n\x19UNDEFINED_INPUT_FILE_TYPE\x10\x00\x12\x17\n\x13\x43SV_INPUT_FILE_TYPE\x10\x01\x12\x1b\n\x17\x46\x45\x41THER_INPUT_FILE_TYPE\x10\x02\x12\x1b\n\x17PARQUET_INPUT_FILE_TYPE\x10\x03*\x86\x01\n\x0eOutputFileType\x12\x1e\n\x1aUNDEFINED_OUTPUT_FILE_TYPE\x10\x00\x12\x18\n\x14\x43SV_OUTPUT_FILE_TYPE\x10\x01\x12\x1c\n\x18\x46\x45\x41THER_OUTPUT_FILE_TYPE\x10\x02\x12\x1c\n\x18PARQUET_OUTPUT_FILE_TYPE\x10\x03*\x8d\x02\n\x15\x42\x61tchJobStatusMessage\x12\x1e\n\x1aUNDEFINED_BATCH_JOB_STATUS\x10\x00\x12\x1e\n\x1a\x42\x41TCH_JOB_COMMITTED_STATUS\x10\x01\x12\x1c\n\x18\x42\x41TCH_JOB_PENDING_STATUS\x10\x02\x12\x1c\n\x18\x42\x41TCH_JOB_RUNNING_STATUS\x10\x03\x12\x1d\n\x19\x42\x41TCH_JOB_FINISHED_STATUS\x10\x04\x12\x1b\n\x17\x42\x41TCH_JOB_FAILED_STATUS\x10\x05\x12\x1e\n\x1a\x42\x41TCH_JOB_CANCELLED_STATUS\x10\x06\x12\x1c\n\x18\x42\x41TCH_JOB_TIMEOUT_STATUS\x10\x07*\x9c\x02\n\x16\x42\x61tchTaskStatusMessage\x12\x1f\n\x1bUNDEFINED_BATCH_TASK_STATUS\x10\x00\x12\x1f\n\x1b\x42\x41TCH_TASK_COMMITTED_STATUS\x10\x01\x12#\n\x1f\x42\x41TCH_TASK_PENDING_START_STATUS\x10\x02\x12\x1d\n\x19\x42\x41TCH_TASK_RUNNING_STATUS\x10\x03\x12\x1e\n\x1a\x42\x41TCH_TASK_FINISHED_STATUS\x10\x04\x12\x1c\n\x18\x42\x41TCH_TASK_FAILED_STATUS\x10\x05\x12\x1f\n\x1b\x42\x41TCH_TASK_CANCELLED_STATUS\x10\x06\x12\x1d\n\x19\x42\x41TCH_TASK_TIMEOUT_STATUS\x10\x07\x32\xb4\x0e\n\x19\x42\x61tchJobManagementService\x12Z\n\rStartBatchJob\x12#.qwak.batchjob.StartBatchJobRequest\x1a$.qwak.batchjob.StartBatchJobResponse\x12]\n\x0e\x43\x61ncelBatchJob\x12$.qwak.batchjob.CancelBatchJobRequest\x1a%.qwak.batchjob.CancelBatchJobResponse\x12]\n\x0eStartWarmupJob\x12$.qwak.batchjob.StartWarmupJobRequest\x1a%.qwak.batchjob.StartWarmupJobResponse\x12`\n\x0f\x43\x61ncelWarmupJob\x12%.qwak.batchjob.CancelWarmupJobRequest\x1a&.qwak.batchjob.CancelWarmupJobResponse\x12\x66\n\x11GetBatchJobStatus\x12\'.qwak.batchjob.GetBatchJobStatusRequest\x1a(.qwak.batchjob.GetBatchJobStatusResponse\x12\x66\n\x11GetBatchJobReport\x12\'.qwak.batchjob.GetBatchJobReportRequest\x1a(.qwak.batchjob.GetBatchJobReportResponse\x12t\n\x16UpdateBatchTasksStatus\x12,.qwak.batchjob.UpdateBatchTasksStatusRequest\x1a,.qwak.batchjob.UpdateBatchTaskStatusResponse\x12Z\n\rListBatchJobs\x12#.qwak.batchjob.ListBatchJobsRequest\x1a$.qwak.batchjob.ListBatchJobsResponse\x12i\n\x12GetBatchJobDetails\x12(.qwak.batchjob.GetBatchJobDetailsRequest\x1a).qwak.batchjob.GetBatchJobDetailsResponse\x12\x8a\x01\n\x1dGetBatchJobPreSignedUploadUrl\x12\x33.qwak.batchjob.GetBatchJobPreSignedUploadUrlRequest\x1a\x34.qwak.batchjob.GetBatchJobPreSignedUploadUrlResponse\x12\x90\x01\n\x1fGetBatchJobPreSignedDownloadUrl\x12\x35.qwak.batchjob.GetBatchJobPreSignedDownloadUrlRequest\x1a\x36.qwak.batchjob.GetBatchJobPreSignedDownloadUrlResponse\x12{\n\x18GetBatchJobUploadDetails\x12..qwak.batchjob.GetBatchJobUploadDetailsRequest\x1a/.qwak.batchjob.GetBatchJobUploadDetailsResponse\x12\x81\x01\n\x1aGetBatchJobDownloadDetails\x12\x30.qwak.batchjob.GetBatchJobDownloadDetailsRequest\x1a\x31.qwak.batchjob.GetBatchJobDownloadDetailsResponse\x12l\n\x13UpdateDefaultParams\x12).qwak.batchjob.UpdateDefaultParamsRequest\x1a*.qwak.batchjob.UpdateDefaultParamsResponse\x12l\n\x13\x44\x65leteDefaultParams\x12).qwak.batchjob.DeleteDefaultParamsRequest\x1a*.qwak.batchjob.DeleteDefaultParamsResponse\x12\x90\x01\n\x1fUpdateTaskIngestedRecordsAmount\x12\x35.qwak.batchjob.UpdateTaskIngestedRecordsAmountRequest\x1a\x36.qwak.batchjob.UpdateTaskIngestedRecordsAmountResponseB.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)qwak/batch_job/v1/batch_job_service.proto\x12\rqwak.batchjob\x1a\x1fgoogle/protobuf/timestamp.proto\x1a/qwak/user_application/common/v0/resources.proto\x1a(qwak/batch_job/v1/batch_job_events.proto\x1a;qwak/administration/authenticated_user/v1/credentials.proto\"\xb4\x01\n\x15StartWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x05 \x01(\t\x12\x16\n\x0ewarmup_timeout\x18\x03 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x04 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\"B\n\x16StartWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"S\n\x16\x43\x61ncelWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\"C\n\x17\x43\x61ncelWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"\x89\x05\n\x14StartBatchJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\x12\x15\n\rsource_bucket\x18\x03 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x04 \x01(\t\x12\x15\n\rsource_folder\x18\x05 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x06 \x01(\t\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12\x13\n\x0bjob_timeout\x18\x08 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\t \x01(\x05\x12\x35\n\x0finput_file_type\x18\n \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x0b \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x0e \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x10 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\x12\x39\n\x11\x62\x61tch_job_request\x18\x11 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobRequest\"\xcb\x01\n\x0f\x42\x61tchJobRequest\x12:\n\rmodel_details\x18\x01 \x01(\x0b\x32#.qwak.batchjob.BatchJobModelDetails\x12\x38\n\x0c\x64\x61ta_details\x18\x02 \x01(\x0b\x32\".qwak.batchjob.BatchJobDataDetails\x12\x42\n\x11\x65xecution_details\x18\x04 \x01(\x0b\x32\'.qwak.batchjob.BatchJobExecutionDetails\":\n\x14\x42\x61tchJobModelDetails\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\"\xe5\x01\n\x13\x42\x61tchJobDataDetails\x12\x36\n\x0bsource_path\x18\x01 \x01(\x0b\x32!.qwak.batchjob.BatchJobSourcePath\x12@\n\x10\x64\x65stination_path\x18\x02 \x01(\x0b\x32&.qwak.batchjob.BatchJobDestinationPath\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\x12\'\n\x1fservice_account_json_key_secret\x18\x05 \x01(\t\"y\n\x12\x42\x61tchJobSourcePath\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x15\n\rsource_folder\x18\x02 \x01(\t\x12\x35\n\x0finput_file_type\x18\x03 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\"\x8a\x01\n\x17\x42\x61tchJobDestinationPath\x12\x1a\n\x12\x64\x65stination_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x02 \x01(\t\x12\x37\n\x10output_file_type\x18\x03 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\"\x94\x02\n\x18\x42\x61tchJobExecutionDetails\x12\x13\n\x0bjob_timeout\x18\x01 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\x02 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x05 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\"/\n\x11\x42\x61tchJobParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"S\n\x15StartBatchJobResponse\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\")\n\x15\x43\x61ncelBatchJobRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"B\n\x16\x43\x61ncelBatchJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\",\n\x18GetBatchJobStatusRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"\xac\x01\n\x19GetBatchJobStatusResponse\x12\x38\n\njob_status\x18\x01 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\x12\x16\n\x0e\x66inished_files\x18\x04 \x01(\x05\x12\x13\n\x0btotal_files\x18\x05 \x01(\x05\",\n\x18GetBatchJobReportRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"a\n\x19GetBatchJobReportResponse\x12\x12\n\nsuccessful\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\x12\x17\n\x0freport_messages\x18\x03 \x03(\t\"`\n\x1dUpdateBatchTasksStatusRequest\x12?\n\x11\x62\x61tch_task_events\x18\x01 \x03(\x0b\x32$.qwak.batchjob.BatchTaskEventMessage\"I\n\x1dUpdateBatchTaskStatusResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"z\n\x19\x41\x64vancedDeploymentOptions\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x01 \x01(\t\x12\x17\n\x0fpurchase_option\x18\x02 \x01(\t\x12\'\n\x1fservice_account_key_secret_name\x18\x03 \x01(\t\"\x85\x03\n\x16\x42\x61tchJobDeploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0f\n\x03\x63pu\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x03 \x01(\x05\x42\x02\x18\x01\x12J\n\x0cmemory_units\x18\x04 \x01(\x0e\x32\x30.qwak.batchjob.BatchJobDeploymentSize.MemoryUnitB\x02\x18\x01\x12H\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesB\x02\x18\x01\x12`\n\x1c\x63lient_pod_compute_resources\x18\x06 \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResources\"/\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02\x1a\x02\x18\x01\"\x99\x01\n\x15\x42\x61tchJobExecutionSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12S\n\x15pod_compute_resources\x18\x02 \x01(\x0b\x32\x34.qwak.user_application.common.v0.PodComputeResources\x12\x13\n\x0btemplate_id\x18\x03 \x01(\t\"Q\n\x14ListBatchJobsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\"K\n\x15ListBatchJobsResponse\x12\x32\n\nbatch_jobs\x18\x01 \x03(\x0b\x32\x1e.qwak.batchjob.BatchJobDetails\"\x81\x03\n\x0f\x42\x61tchJobDetails\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x38\n\njob_status\x18\x03 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\x12;\n\x08job_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSizeB\x02\x18\x01\x12\x46\n\x18\x62\x61tch_job_execution_size\x18\x08 \x01(\x0b\x32$.qwak.batchjob.BatchJobExecutionSize\x12\x16\n\x0e\x65nvironment_id\x18\t \x01(\t\"+\n\x19GetBatchJobDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"y\n\x1aGetBatchJobDetailsResponse\x12\x31\n\tbatch_job\x18\x01 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"\x84\x04\n\x0f\x42\x61tchJobMessage\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\tbranch_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\njob_status\x18\x07 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x15\n\rtotal_records\x18\x08 \x01(\x05\x12\x37\n\x08job_size\x18\t \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12;\n\x0freport_messages\x18\n \x03(\x0b\x32\".qwak.batchjob.ExecutionReportLine\x12\x43\n\x16\x65xecution_file_details\x18\x0b \x01(\x0b\x32#.qwak.batchjob.ExecutionFileDetails\x12<\n\x0ftask_executions\x18\x0c \x03(\x0b\x32#.qwak.batchjob.TaskExecutionDetails\"M\n\x13\x45xecutionReportLine\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04line\x18\x02 \x01(\t\"\x95\x02\n\x14\x45xecutionFileDetails\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x02 \x01(\t\x12\x13\n\x0bsource_path\x18\x03 \x01(\t\x12\x18\n\x10\x64\x65stination_path\x18\x04 \x01(\t\x12\x35\n\x0finput_file_type\x18\x05 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x06 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x16\n\x0e\x66inished_files\x18\x07 \x01(\x05\x12\x13\n\x0btotal_files\x18\x08 \x01(\x05\"\xe6\x01\n\x14TaskExecutionDetails\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.qwak.batchjob.BatchTaskStatusMessage\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0enum_of_records\x18\x05 \x01(\x05\x12\x10\n\x08\x66ilename\x18\x06 \x01(\t\"d\n$GetBatchJobPreSignedUploadUrlRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x17\n\x0fnumber_of_files\x18\x02 \x01(\x05\x12\x11\n\tfile_type\x18\x03 \x01(\t\"\x98\x01\n%GetBatchJobPreSignedUploadUrlResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12\x0c\n\x04urls\x18\x04 \x03(\t\x12\x0f\n\x07success\x18\x05 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\"8\n&GetBatchJobPreSignedDownloadUrlRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"a\n\'GetBatchJobPreSignedDownloadUrlResponse\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"3\n\x1fGetBatchJobUploadDetailsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\xb4\x01\n GetBatchJobUploadDetailsResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12W\n\x0b\x63redentials\x18\x04 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"3\n!GetBatchJobDownloadDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"\x9b\x01\n\"GetBatchJobDownloadDetailsResponse\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12W\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"\xd7\x01\n\x1aUpdateDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x46\n\x17\x64\x65\x66\x61ult_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\"\x1d\n\x1bUpdateDefaultParamsResponse\".\n\x1a\x44\x65leteDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\x1d\n\x1b\x44\x65leteDefaultParamsResponse\"S\n&UpdateTaskIngestedRecordsAmountRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x18\n\x10ingested_records\x18\x02 \x01(\x03\")\n\'UpdateTaskIngestedRecordsAmountResponse*\x81\x01\n\rInputFileType\x12\x1d\n\x19UNDEFINED_INPUT_FILE_TYPE\x10\x00\x12\x17\n\x13\x43SV_INPUT_FILE_TYPE\x10\x01\x12\x1b\n\x17\x46\x45\x41THER_INPUT_FILE_TYPE\x10\x02\x12\x1b\n\x17PARQUET_INPUT_FILE_TYPE\x10\x03*\x86\x01\n\x0eOutputFileType\x12\x1e\n\x1aUNDEFINED_OUTPUT_FILE_TYPE\x10\x00\x12\x18\n\x14\x43SV_OUTPUT_FILE_TYPE\x10\x01\x12\x1c\n\x18\x46\x45\x41THER_OUTPUT_FILE_TYPE\x10\x02\x12\x1c\n\x18PARQUET_OUTPUT_FILE_TYPE\x10\x03*\x8d\x02\n\x15\x42\x61tchJobStatusMessage\x12\x1e\n\x1aUNDEFINED_BATCH_JOB_STATUS\x10\x00\x12\x1e\n\x1a\x42\x41TCH_JOB_COMMITTED_STATUS\x10\x01\x12\x1c\n\x18\x42\x41TCH_JOB_PENDING_STATUS\x10\x02\x12\x1c\n\x18\x42\x41TCH_JOB_RUNNING_STATUS\x10\x03\x12\x1d\n\x19\x42\x41TCH_JOB_FINISHED_STATUS\x10\x04\x12\x1b\n\x17\x42\x41TCH_JOB_FAILED_STATUS\x10\x05\x12\x1e\n\x1a\x42\x41TCH_JOB_CANCELLED_STATUS\x10\x06\x12\x1c\n\x18\x42\x41TCH_JOB_TIMEOUT_STATUS\x10\x07*\x9c\x02\n\x16\x42\x61tchTaskStatusMessage\x12\x1f\n\x1bUNDEFINED_BATCH_TASK_STATUS\x10\x00\x12\x1f\n\x1b\x42\x41TCH_TASK_COMMITTED_STATUS\x10\x01\x12#\n\x1f\x42\x41TCH_TASK_PENDING_START_STATUS\x10\x02\x12\x1d\n\x19\x42\x41TCH_TASK_RUNNING_STATUS\x10\x03\x12\x1e\n\x1a\x42\x41TCH_TASK_FINISHED_STATUS\x10\x04\x12\x1c\n\x18\x42\x41TCH_TASK_FAILED_STATUS\x10\x05\x12\x1f\n\x1b\x42\x41TCH_TASK_CANCELLED_STATUS\x10\x06\x12\x1d\n\x19\x42\x41TCH_TASK_TIMEOUT_STATUS\x10\x07\x32\xb4\x0e\n\x19\x42\x61tchJobManagementService\x12Z\n\rStartBatchJob\x12#.qwak.batchjob.StartBatchJobRequest\x1a$.qwak.batchjob.StartBatchJobResponse\x12]\n\x0e\x43\x61ncelBatchJob\x12$.qwak.batchjob.CancelBatchJobRequest\x1a%.qwak.batchjob.CancelBatchJobResponse\x12]\n\x0eStartWarmupJob\x12$.qwak.batchjob.StartWarmupJobRequest\x1a%.qwak.batchjob.StartWarmupJobResponse\x12`\n\x0f\x43\x61ncelWarmupJob\x12%.qwak.batchjob.CancelWarmupJobRequest\x1a&.qwak.batchjob.CancelWarmupJobResponse\x12\x66\n\x11GetBatchJobStatus\x12\'.qwak.batchjob.GetBatchJobStatusRequest\x1a(.qwak.batchjob.GetBatchJobStatusResponse\x12\x66\n\x11GetBatchJobReport\x12\'.qwak.batchjob.GetBatchJobReportRequest\x1a(.qwak.batchjob.GetBatchJobReportResponse\x12t\n\x16UpdateBatchTasksStatus\x12,.qwak.batchjob.UpdateBatchTasksStatusRequest\x1a,.qwak.batchjob.UpdateBatchTaskStatusResponse\x12Z\n\rListBatchJobs\x12#.qwak.batchjob.ListBatchJobsRequest\x1a$.qwak.batchjob.ListBatchJobsResponse\x12i\n\x12GetBatchJobDetails\x12(.qwak.batchjob.GetBatchJobDetailsRequest\x1a).qwak.batchjob.GetBatchJobDetailsResponse\x12\x8a\x01\n\x1dGetBatchJobPreSignedUploadUrl\x12\x33.qwak.batchjob.GetBatchJobPreSignedUploadUrlRequest\x1a\x34.qwak.batchjob.GetBatchJobPreSignedUploadUrlResponse\x12\x90\x01\n\x1fGetBatchJobPreSignedDownloadUrl\x12\x35.qwak.batchjob.GetBatchJobPreSignedDownloadUrlRequest\x1a\x36.qwak.batchjob.GetBatchJobPreSignedDownloadUrlResponse\x12{\n\x18GetBatchJobUploadDetails\x12..qwak.batchjob.GetBatchJobUploadDetailsRequest\x1a/.qwak.batchjob.GetBatchJobUploadDetailsResponse\x12\x81\x01\n\x1aGetBatchJobDownloadDetails\x12\x30.qwak.batchjob.GetBatchJobDownloadDetailsRequest\x1a\x31.qwak.batchjob.GetBatchJobDownloadDetailsResponse\x12l\n\x13UpdateDefaultParams\x12).qwak.batchjob.UpdateDefaultParamsRequest\x1a*.qwak.batchjob.UpdateDefaultParamsResponse\x12l\n\x13\x44\x65leteDefaultParams\x12).qwak.batchjob.DeleteDefaultParamsRequest\x1a*.qwak.batchjob.DeleteDefaultParamsResponse\x12\x90\x01\n\x1fUpdateTaskIngestedRecordsAmount\x12\x35.qwak.batchjob.UpdateTaskIngestedRecordsAmountRequest\x1a\x36.qwak.batchjob.UpdateTaskIngestedRecordsAmountResponseB.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
 
 _INPUTFILETYPE = DESCRIPTOR.enum_types_by_name['InputFileType']
 InputFileType = enum_type_wrapper.EnumTypeWrapper(_INPUTFILETYPE)
 _OUTPUTFILETYPE = DESCRIPTOR.enum_types_by_name['OutputFileType']
 OutputFileType = enum_type_wrapper.EnumTypeWrapper(_OUTPUTFILETYPE)
 _BATCHJOBSTATUSMESSAGE = DESCRIPTOR.enum_types_by_name['BatchJobStatusMessage']
 BatchJobStatusMessage = enum_type_wrapper.EnumTypeWrapper(_BATCHJOBSTATUSMESSAGE)
@@ -455,22 +455,22 @@
   _BATCHJOBDEPLOYMENTSIZE.fields_by_name['gpu_resources']._serialized_options = b'\030\001'
   _LISTBATCHJOBSREQUEST.fields_by_name['branch_id']._options = None
   _LISTBATCHJOBSREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _BATCHJOBDETAILS.fields_by_name['job_size']._options = None
   _BATCHJOBDETAILS.fields_by_name['job_size']._serialized_options = b'\030\001'
   _BATCHJOBMESSAGE.fields_by_name['branch_id']._options = None
   _BATCHJOBMESSAGE.fields_by_name['branch_id']._serialized_options = b'\030\001'
-  _INPUTFILETYPE._serialized_start=6903
-  _INPUTFILETYPE._serialized_end=7032
-  _OUTPUTFILETYPE._serialized_start=7035
-  _OUTPUTFILETYPE._serialized_end=7169
-  _BATCHJOBSTATUSMESSAGE._serialized_start=7172
-  _BATCHJOBSTATUSMESSAGE._serialized_end=7441
-  _BATCHTASKSTATUSMESSAGE._serialized_start=7444
-  _BATCHTASKSTATUSMESSAGE._serialized_end=7728
+  _INPUTFILETYPE._serialized_start=6944
+  _INPUTFILETYPE._serialized_end=7073
+  _OUTPUTFILETYPE._serialized_start=7076
+  _OUTPUTFILETYPE._serialized_end=7210
+  _BATCHJOBSTATUSMESSAGE._serialized_start=7213
+  _BATCHJOBSTATUSMESSAGE._serialized_end=7482
+  _BATCHTASKSTATUSMESSAGE._serialized_start=7485
+  _BATCHTASKSTATUSMESSAGE._serialized_end=7769
   _STARTWARMUPJOBREQUEST._serialized_start=246
   _STARTWARMUPJOBREQUEST._serialized_end=426
   _STARTWARMUPJOBRESPONSE._serialized_start=428
   _STARTWARMUPJOBRESPONSE._serialized_end=494
   _CANCELWARMUPJOBREQUEST._serialized_start=496
   _CANCELWARMUPJOBREQUEST._serialized_end=579
   _CANCELWARMUPJOBRESPONSE._serialized_start=581
@@ -506,63 +506,63 @@
   _GETBATCHJOBREPORTRESPONSE._serialized_start=2855
   _GETBATCHJOBREPORTRESPONSE._serialized_end=2952
   _UPDATEBATCHTASKSSTATUSREQUEST._serialized_start=2954
   _UPDATEBATCHTASKSSTATUSREQUEST._serialized_end=3050
   _UPDATEBATCHTASKSTATUSRESPONSE._serialized_start=3052
   _UPDATEBATCHTASKSTATUSRESPONSE._serialized_end=3125
   _ADVANCEDDEPLOYMENTOPTIONS._serialized_start=3127
-  _ADVANCEDDEPLOYMENTOPTIONS._serialized_end=3208
-  _BATCHJOBDEPLOYMENTSIZE._serialized_start=3211
-  _BATCHJOBDEPLOYMENTSIZE._serialized_end=3600
-  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_start=3553
-  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_end=3600
-  _BATCHJOBEXECUTIONSIZE._serialized_start=3603
-  _BATCHJOBEXECUTIONSIZE._serialized_end=3756
-  _LISTBATCHJOBSREQUEST._serialized_start=3758
-  _LISTBATCHJOBSREQUEST._serialized_end=3839
-  _LISTBATCHJOBSRESPONSE._serialized_start=3841
-  _LISTBATCHJOBSRESPONSE._serialized_end=3916
-  _BATCHJOBDETAILS._serialized_start=3919
-  _BATCHJOBDETAILS._serialized_end=4304
-  _GETBATCHJOBDETAILSREQUEST._serialized_start=4306
-  _GETBATCHJOBDETAILSREQUEST._serialized_end=4349
-  _GETBATCHJOBDETAILSRESPONSE._serialized_start=4351
-  _GETBATCHJOBDETAILSRESPONSE._serialized_end=4472
-  _BATCHJOBMESSAGE._serialized_start=4475
-  _BATCHJOBMESSAGE._serialized_end=4991
-  _EXECUTIONREPORTLINE._serialized_start=4993
-  _EXECUTIONREPORTLINE._serialized_end=5070
-  _EXECUTIONFILEDETAILS._serialized_start=5073
-  _EXECUTIONFILEDETAILS._serialized_end=5350
-  _TASKEXECUTIONDETAILS._serialized_start=5353
-  _TASKEXECUTIONDETAILS._serialized_end=5583
-  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_start=5585
-  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_end=5685
-  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_start=5688
-  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_end=5840
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_start=5842
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_end=5898
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_start=5900
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_end=5997
-  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_start=5999
-  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_end=6050
-  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_start=6053
-  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_end=6233
-  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_start=6235
-  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_end=6286
-  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_start=6289
-  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_end=6444
-  _UPDATEDEFAULTPARAMSREQUEST._serialized_start=6447
-  _UPDATEDEFAULTPARAMSREQUEST._serialized_end=6662
-  _UPDATEDEFAULTPARAMSRESPONSE._serialized_start=6664
-  _UPDATEDEFAULTPARAMSRESPONSE._serialized_end=6693
-  _DELETEDEFAULTPARAMSREQUEST._serialized_start=6695
-  _DELETEDEFAULTPARAMSREQUEST._serialized_end=6741
-  _DELETEDEFAULTPARAMSRESPONSE._serialized_start=6743
-  _DELETEDEFAULTPARAMSRESPONSE._serialized_end=6772
-  _UPDATETASKINGESTEDRECORDSAMOUNTREQUEST._serialized_start=6774
-  _UPDATETASKINGESTEDRECORDSAMOUNTREQUEST._serialized_end=6857
-  _UPDATETASKINGESTEDRECORDSAMOUNTRESPONSE._serialized_start=6859
-  _UPDATETASKINGESTEDRECORDSAMOUNTRESPONSE._serialized_end=6900
-  _BATCHJOBMANAGEMENTSERVICE._serialized_start=7731
-  _BATCHJOBMANAGEMENTSERVICE._serialized_end=9575
+  _ADVANCEDDEPLOYMENTOPTIONS._serialized_end=3249
+  _BATCHJOBDEPLOYMENTSIZE._serialized_start=3252
+  _BATCHJOBDEPLOYMENTSIZE._serialized_end=3641
+  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_start=3594
+  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_end=3641
+  _BATCHJOBEXECUTIONSIZE._serialized_start=3644
+  _BATCHJOBEXECUTIONSIZE._serialized_end=3797
+  _LISTBATCHJOBSREQUEST._serialized_start=3799
+  _LISTBATCHJOBSREQUEST._serialized_end=3880
+  _LISTBATCHJOBSRESPONSE._serialized_start=3882
+  _LISTBATCHJOBSRESPONSE._serialized_end=3957
+  _BATCHJOBDETAILS._serialized_start=3960
+  _BATCHJOBDETAILS._serialized_end=4345
+  _GETBATCHJOBDETAILSREQUEST._serialized_start=4347
+  _GETBATCHJOBDETAILSREQUEST._serialized_end=4390
+  _GETBATCHJOBDETAILSRESPONSE._serialized_start=4392
+  _GETBATCHJOBDETAILSRESPONSE._serialized_end=4513
+  _BATCHJOBMESSAGE._serialized_start=4516
+  _BATCHJOBMESSAGE._serialized_end=5032
+  _EXECUTIONREPORTLINE._serialized_start=5034
+  _EXECUTIONREPORTLINE._serialized_end=5111
+  _EXECUTIONFILEDETAILS._serialized_start=5114
+  _EXECUTIONFILEDETAILS._serialized_end=5391
+  _TASKEXECUTIONDETAILS._serialized_start=5394
+  _TASKEXECUTIONDETAILS._serialized_end=5624
+  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_start=5626
+  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_end=5726
+  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_start=5729
+  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_end=5881
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_start=5883
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_end=5939
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_start=5941
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_end=6038
+  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_start=6040
+  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_end=6091
+  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_start=6094
+  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_end=6274
+  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_start=6276
+  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_end=6327
+  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_start=6330
+  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_end=6485
+  _UPDATEDEFAULTPARAMSREQUEST._serialized_start=6488
+  _UPDATEDEFAULTPARAMSREQUEST._serialized_end=6703
+  _UPDATEDEFAULTPARAMSRESPONSE._serialized_start=6705
+  _UPDATEDEFAULTPARAMSRESPONSE._serialized_end=6734
+  _DELETEDEFAULTPARAMSREQUEST._serialized_start=6736
+  _DELETEDEFAULTPARAMSREQUEST._serialized_end=6782
+  _DELETEDEFAULTPARAMSRESPONSE._serialized_start=6784
+  _DELETEDEFAULTPARAMSRESPONSE._serialized_end=6813
+  _UPDATETASKINGESTEDRECORDSAMOUNTREQUEST._serialized_start=6815
+  _UPDATETASKINGESTEDRECORDSAMOUNTREQUEST._serialized_end=6898
+  _UPDATETASKINGESTEDRECORDSAMOUNTRESPONSE._serialized_start=6900
+  _UPDATETASKINGESTEDRECORDSAMOUNTRESPONSE._serialized_end=6941
+  _BATCHJOBMANAGEMENTSERVICE._serialized_start=7772
+  _BATCHJOBMANAGEMENTSERVICE._serialized_end=9616
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -655,25 +655,29 @@
 global___UpdateBatchTaskStatusResponse = UpdateBatchTaskStatusResponse
 
 class AdvancedDeploymentOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CUSTOM_IAM_ROLE_ARN_FIELD_NUMBER: builtins.int
     PURCHASE_OPTION_FIELD_NUMBER: builtins.int
+    SERVICE_ACCOUNT_KEY_SECRET_NAME_FIELD_NUMBER: builtins.int
     custom_iam_role_arn: builtins.str
     """Custom IAM Role ARN"""
     purchase_option: builtins.str
     """Whether it is spot/ondemand (default - spot)"""
+    service_account_key_secret_name: builtins.str
+    """Service account key secret name for gcp"""
     def __init__(
         self,
         *,
         custom_iam_role_arn: builtins.str = ...,
         purchase_option: builtins.str = ...,
+        service_account_key_secret_name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["custom_iam_role_arn", b"custom_iam_role_arn", "purchase_option", b"purchase_option"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["custom_iam_role_arn", b"custom_iam_role_arn", "purchase_option", b"purchase_option", "service_account_key_secret_name", b"service_account_key_secret_name"]) -> None: ...
 
 global___AdvancedDeploymentOptions = AdvancedDeploymentOptions
 
 class BatchJobDeploymentSize(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _MemoryUnit:
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.builds import build_pb2 as qwak_dot_builds_dot_build__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19qwak/build/v1/build.proto\x12\x11\x63om.qwak.build.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17qwak/builds/build.proto\"\xda\x01\n\x0bModelSchema\x12+\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x19.com.qwak.build.v1.Entity\x12,\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32\x1a.com.qwak.build.v1.Feature\x12\x32\n\x0bpredictions\x18\x03 \x03(\x0b\x32\x1d.com.qwak.build.v1.Prediction\x12<\n\x10inference_output\x18\x04 \x03(\x0b\x32\".com.qwak.build.v1.InferenceOutput\"B\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"\xa8\x04\n\x07\x46\x65\x61ture\x12\x38\n\rbatch_feature\x18\x01 \x01(\x0b\x32\x1f.com.qwak.build.v1.BatchFeatureH\x00\x12>\n\x10\x65xplicit_feature\x18\x02 \x01(\x0b\x32\".com.qwak.build.v1.ExplicitFeatureH\x00\x12@\n\x12on_the_fly_feature\x18\x03 \x01(\x0b\x32\".com.qwak.build.v1.OnTheFlyFeatureH\x00\x12@\n\x11streaming_feature\x18\x04 \x01(\x0b\x32#.com.qwak.build.v1.StreamingFeatureH\x00\x12\x38\n\rrequest_input\x18\x05 \x01(\x0b\x32\x1f.com.qwak.build.v1.RequestInputH\x00\x12W\n\x1dstreaming_aggregation_feature\x18\x06 \x01(\x0b\x32..com.qwak.build.v1.StreamingAggregationFeatureH\x00\x12=\n\x10\x62\x61tch_feature_v1\x18\x07 \x01(\x0b\x32!.com.qwak.build.v1.BatchFeatureV1H\x00\x12\x45\n\x14streaming_feature_v1\x18\x08 \x01(\x0b\x32%.com.qwak.build.v1.StreamingFeatureV1H\x00\x42\x06\n\x04type\"\x85\x01\n\x0fOnTheFlyFeature\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x39\n\x0fsource_features\x18\x03 \x03(\x0b\x32 .com.qwak.build.v1.SourceFeature\"I\n\x0e\x42\x61tchFeatureV1\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"M\n\x12StreamingFeatureV1\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"G\n\x0c\x42\x61tchFeature\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"K\n\x10StreamingFeature\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"V\n\x1bStreamingAggregationFeature\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"K\n\x0f\x45xplicitFeature\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"H\n\x0cRequestInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"\x91\x01\n\rSourceFeature\x12>\n\x10\x65xplicit_feature\x18\x01 \x01(\x0b\x32\".com.qwak.build.v1.ExplicitFeatureH\x00\x12\x38\n\rrequest_input\x18\x02 \x01(\x0b\x32\x1f.com.qwak.build.v1.RequestInputH\x00\x42\x06\n\x04type\"F\n\nPrediction\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"K\n\x0fInferenceOutput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"\xa1\x01\n\tValueType\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".com.qwak.build.v1.ValueType.Types\"b\n\x05Types\x12\x0b\n\x07INVALID\x10\x00\x12\t\n\x05\x42YTES\x10\x01\x12\n\n\x06STRING\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\n\n\x06\x44OUBLE\x10\x05\x12\t\n\x05\x46LOAT\x10\x06\x12\x08\n\x04\x42OOL\x10\x07\"j\n\x11ParameterCategory\"U\n\x08\x43\x61tegory\x12\x0b\n\x07INVALID\x10\x00\x12\n\n\x06\x45NTITY\x10\x01\x12\x0b\n\x07\x46\x45\x41TURE\x10\x02\x12\x0e\n\nPREDICTION\x10\x03\x12\x13\n\x0fINFERENCEOUTPUT\x10\x04\"\xc5\x06\n\x05\x42uild\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x10\n\x08\x63ommitId\x18\x02 \x01(\t\x12\x10\n\x08\x62ranchId\x18\x03 \x01(\t\x12\x13\n\x0b\x62uildConfig\x18\x04 \x01(\t\x12\x34\n\x0c\x62uild_status\x18\x05 \x01(\x0e\x32\x1e.com.qwak.build.v1.BuildStatus\x12\x0c\n\x04tags\x18\x06 \x03(\t\x12\r\n\x05steps\x18\x07 \x03(\t\x12\x34\n\x06params\x18\x08 \x03(\x0b\x32$.com.qwak.build.v1.Build.ParamsEntry\x12\x36\n\x07metrics\x18\t \x03(\x0b\x32%.com.qwak.build.v1.Build.MetricsEntry\x12\x34\n\x0cmodel_schema\x18\n \x01(\x0b\x32\x1e.com.qwak.build.v1.ModelSchema\x12\'\n\x05\x61udit\x18\x0b \x01(\x0b\x32\x18.com.qwak.build.v1.Audit\x12\x12\n\nmodel_uuid\x18\x0c \x01(\t\x12\x13\n\x0bsdk_version\x18\r \x01(\t\x12\x16\n\x0eimage_name_tag\x18\x0e \x01(\t\x12J\n\x1b\x62uild_configuration_message\x18\x0f \x01(\x0b\x32%.com.qwak.build.v1.BuildConfiguration\x12,\n\x08\x65nd_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x65nvironment_id\x18\x11 \x01(\t\x12\x1c\n\x14\x62uild_destined_image\x18\x12 \x01(\t\x12;\n\x10\x66ramework_models\x18\x13 \x03(\x0b\x32!.com.qwak.build.v1.FrameworkModel\x12(\n build_destined_image_pull_secret\x18\x14 \x01(\t\x12\x1b\n\x13\x66\x61ilure_reason_code\x18\x15 \x01(\t\x1a-\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\x9b\x01\n\x05\x41udit\x12\x12\n\ncreated_by\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x03 \x01(\t\x12\x34\n\x10last_modified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb3\x02\n\x12\x42uildConfiguration\x12<\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32\".com.qwak.build.v1.BuildProperties\x12\x36\n\tbuild_env\x18\x02 \x01(\x0b\x32#.com.qwak.build.v1.BuildEnvironment\x12\x36\n\tpre_build\x18\x03 \x01(\x0b\x32#.com.qwak.build.v1.BuildEnvironment\x12\x37\n\npost_build\x18\x04 \x01(\x0b\x32#.com.qwak.build.v1.BuildEnvironment\x12%\n\x04step\x18\x05 \x01(\x0b\x32\x17.com.qwak.build.v1.Step\x12\x0f\n\x07verbose\x18\x06 \x01(\x05\"\xba\x01\n\x0f\x42uildProperties\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x33\n\tmodel_uri\x18\x02 \x01(\x0b\x32 .com.qwak.build.v1.BuildModelUri\x12\x0c\n\x04tags\x18\x03 \x03(\t\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x05 \x01(\t\x12\x18\n\x10\x65nvironment_name\x18\x06 \x01(\t\x12\x16\n\x0egpu_compatible\x18\x07 \x01(\x08\"B\n\rBuildModelUri\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x10\n\x08main_dir\x18\x03 \x01(\t\"\xd4\x01\n\x10\x42uildEnvironment\x12.\n\x06\x64ocker\x18\x01 \x01(\x0b\x32\x1e.com.qwak.build.v1.DockerBuild\x12,\n\x05local\x18\x02 \x01(\x0b\x32\x1d.com.qwak.build.v1.LocalBuild\x12\x32\n\npython_env\x18\x03 \x01(\x0b\x32\x1e.com.qwak.build.v1.PythonBuild\x12.\n\x06remote\x18\x04 \x01(\x0b\x32\x1e.com.qwak.build.v1.RemoteBuild\"\x85\x02\n\x0b\x44ockerBuild\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x41\n\nbuild_args\x18\x02 \x03(\x0b\x32-.com.qwak.build.v1.DockerBuild.BuildArgsEntry\x12\x10\n\x08\x65nv_vars\x18\x03 \x03(\t\x12\x10\n\x08no_cache\x18\x04 \x01(\x08\x12\x0e\n\x06params\x18\x05 \x03(\t\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x06 \x01(\t\x12\r\n\x05\x63\x61\x63he\x18\x07 \x01(\x08\x12\x0c\n\x04push\x18\x08 \x01(\x08\x1a\x30\n\x0e\x42uildArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"2\n\nLocalBuild\x12\x13\n\x0b\x61ws_profile\x18\x01 \x01(\t\x12\x0f\n\x07no_push\x18\x02 \x01(\x08\"\x8c\x02\n\x0bPythonBuild\x12 \n\x18qwak_sdk_extra_index_url\x18\x01 \x01(\t\x12>\n\nvirtualenv\x18\x02 \x01(\x0b\x32*.com.qwak.build.v1.VirtualEnvironmentBuild\x12,\n\x05\x63onda\x18\x03 \x01(\x0b\x32\x1d.com.qwak.build.v1.CondaBuild\x12.\n\x06poetry\x18\x04 \x01(\x0b\x32\x1e.com.qwak.build.v1.PoetryBuild\x12\x1c\n\x14\x64\x65pendency_file_path\x18\x05 \x01(\t\x12\x1f\n\x17use_deprecated_resolver\x18\x06 \x01(\x08\" \n\nCondaBuild\x12\x12\n\nconda_file\x18\x01 \x01(\t\"8\n\x0bPoetryBuild\x12\x16\n\x0epython_version\x18\x01 \x01(\t\x12\x11\n\tlock_file\x18\x02 \x01(\t\"K\n\x17VirtualEnvironmentBuild\x12\x16\n\x0epython_version\x18\x01 \x01(\t\x12\x18\n\x10requirements_txt\x18\x02 \x01(\t\"\\\n\x0bRemoteBuild\x12\x11\n\tis_remote\x18\x01 \x01(\x08\x12:\n\tresources\x18\x02 \x01(\x0b\x32\'.com.qwak.build.v1.RemoteBuildResources\"\x8f\x01\n\x14RemoteBuildResources\x12\x0c\n\x04\x63pus\x18\x01 \x01(\x02\x12\x0e\n\x06memory\x18\x02 \x01(\t\x12\x33\n\x08gpu_type\x18\x03 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x04 \x01(\x05\x12\x10\n\x08instance\x18\x05 \x01(\t\"_\n\x04Step\x12\r\n\x05tests\x18\x01 \x01(\x08\x12\x1f\n\x17validate_build_artifact\x18\x02 \x01(\x08\x12\'\n\x1fvalidate_build_artifact_timeout\x18\x03 \x01(\x05\"\xdc\x01\n\x0b\x42uildFilter\x12\x0c\n\x04tags\x18\x01 \x03(\t\x12\x37\n\x0emetric_filters\x18\x02 \x03(\x0b\x32\x1f.com.qwak.build.v1.MetricFilter\x12=\n\x11parameter_filters\x18\x03 \x03(\x0b\x32\".com.qwak.build.v1.ParameterFilter\x12\x18\n\x10require_all_tags\x18\x04 \x01(\x08\x12\x1a\n\x12include_extra_tags\x18\x05 \x01(\x08\x12\x11\n\tbuild_ids\x18\x06 \x03(\t\"r\n\x0cMetricFilter\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\x12\x14\n\x0cmetric_value\x18\x02 \x01(\x02\x12\x37\n\x08operator\x18\x03 \x01(\x0e\x32%.com.qwak.build.v1.MetricOperatorType\"~\n\x0fParameterFilter\x12\x16\n\x0eparameter_name\x18\x01 \x01(\t\x12\x17\n\x0fparameter_value\x18\x02 \x01(\t\x12:\n\x08operator\x18\x03 \x01(\x0e\x32(.com.qwak.build.v1.ParameterOperatorType\"d\n\x13\x46rameworkModelsSpec\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12;\n\x10\x66ramework_models\x18\x02 \x03(\x0b\x32!.com.qwak.build.v1.FrameworkModel\"c\n\x0e\x46rameworkModel\x12I\n\x16huggingface_model_spec\x18\x02 \x01(\x0b\x32\'.com.qwak.build.v1.HuggingFaceModelSpecH\x00\x42\x06\n\x04type\"]\n\x14HuggingFaceModelSpec\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x12\n\nmodel_name\x18\x03 \x01(\t\x12\x0c\n\x04sha1\x18\x04 \x01(\t\"r\n\x11ScanResultSummary\x12(\n\x06issues\x18\x01 \x03(\x0b\x32\x18.com.qwak.build.v1.Issue\x12\x16\n\x0eui_direct_link\x18\x02 \x01(\t\x12\x1b\n\x13ui_scan_direct_link\x18\x03 \x01(\t\"a\n\x05Issue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08severity\x18\x02 \x01(\t\x12\x12\n\nissue_type\x18\x03 \x01(\t\x12\x0f\n\x07summary\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"L\n\x11\x42uildImageDetails\x12\x17\n\x0fimage_full_path\x18\x01 \x01(\t\x12\x1e\n\x16image_pull_secret_name\x18\x02 \x01(\t*\xe8\x01\n\x0b\x42uildStatus\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bIN_PROGRESS\x10\x01\x12\x0e\n\nSUCCESSFUL\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x1d\n\x19REMOTE_BUILD_INITIALIZING\x10\x04\x12\x1a\n\x16REMOTE_BUILD_CANCELLED\x10\x05\x12\x1a\n\x16REMOTE_BUILD_TIMED_OUT\x10\x06\x12\x18\n\x14REMOTE_BUILD_UNKNOWN\x10\x07\x12\x18\n\x14SYNCING_ENVIRONMENTS\x10\x08\x12\x14\n\x10\x46INISHED_SYNCING\x10\t*\xa0\x02\n\x12MetricOperatorType\x12 \n\x1cMETRIC_OPERATOR_TYPE_INVALID\x10\x00\x12\x1f\n\x1bMETRIC_OPERATOR_TYPE_EQUALS\x10\x01\x12#\n\x1fMETRIC_OPERATOR_TYPE_NOT_EQUALS\x10\x02\x12\"\n\x1eMETRIC_OPERATOR_TYPE_LESS_THAN\x10\x03\x12)\n%METRIC_OPERATOR_TYPE_LESS_THAN_EQUALS\x10\x04\x12%\n!METRIC_OPERATOR_TYPE_GREATER_THAN\x10\x05\x12,\n(METRIC_OPERATOR_TYPE_GREATER_THAN_EQUALS\x10\x06*\x88\x01\n\x15ParameterOperatorType\x12#\n\x1fPARAMETER_OPERATOR_TYPE_INVALID\x10\x00\x12\"\n\x1ePARAMETER_OPERATOR_TYPE_EQUALS\x10\x01\x12&\n\"PARAMETER_OPERATOR_TYPE_NOT_EQUALS\x10\x02\x42!\n\x11\x63om.qwak.build.v1B\nBuildProtoP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19qwak/build/v1/build.proto\x12\x11\x63om.qwak.build.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17qwak/builds/build.proto\"\xda\x01\n\x0bModelSchema\x12+\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x19.com.qwak.build.v1.Entity\x12,\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32\x1a.com.qwak.build.v1.Feature\x12\x32\n\x0bpredictions\x18\x03 \x03(\x0b\x32\x1d.com.qwak.build.v1.Prediction\x12<\n\x10inference_output\x18\x04 \x03(\x0b\x32\".com.qwak.build.v1.InferenceOutput\"B\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"\xa8\x04\n\x07\x46\x65\x61ture\x12\x38\n\rbatch_feature\x18\x01 \x01(\x0b\x32\x1f.com.qwak.build.v1.BatchFeatureH\x00\x12>\n\x10\x65xplicit_feature\x18\x02 \x01(\x0b\x32\".com.qwak.build.v1.ExplicitFeatureH\x00\x12@\n\x12on_the_fly_feature\x18\x03 \x01(\x0b\x32\".com.qwak.build.v1.OnTheFlyFeatureH\x00\x12@\n\x11streaming_feature\x18\x04 \x01(\x0b\x32#.com.qwak.build.v1.StreamingFeatureH\x00\x12\x38\n\rrequest_input\x18\x05 \x01(\x0b\x32\x1f.com.qwak.build.v1.RequestInputH\x00\x12W\n\x1dstreaming_aggregation_feature\x18\x06 \x01(\x0b\x32..com.qwak.build.v1.StreamingAggregationFeatureH\x00\x12=\n\x10\x62\x61tch_feature_v1\x18\x07 \x01(\x0b\x32!.com.qwak.build.v1.BatchFeatureV1H\x00\x12\x45\n\x14streaming_feature_v1\x18\x08 \x01(\x0b\x32%.com.qwak.build.v1.StreamingFeatureV1H\x00\x42\x06\n\x04type\"\x85\x01\n\x0fOnTheFlyFeature\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x39\n\x0fsource_features\x18\x03 \x03(\x0b\x32 .com.qwak.build.v1.SourceFeature\"I\n\x0e\x42\x61tchFeatureV1\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"M\n\x12StreamingFeatureV1\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"G\n\x0c\x42\x61tchFeature\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"K\n\x10StreamingFeature\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"V\n\x1bStreamingAggregationFeature\x12)\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x19.com.qwak.build.v1.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"K\n\x0f\x45xplicitFeature\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"H\n\x0cRequestInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"\x91\x01\n\rSourceFeature\x12>\n\x10\x65xplicit_feature\x18\x01 \x01(\x0b\x32\".com.qwak.build.v1.ExplicitFeatureH\x00\x12\x38\n\rrequest_input\x18\x02 \x01(\x0b\x32\x1f.com.qwak.build.v1.RequestInputH\x00\x42\x06\n\x04type\"F\n\nPrediction\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"K\n\x0fInferenceOutput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0b\x32\x1c.com.qwak.build.v1.ValueType\"\xa1\x01\n\tValueType\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".com.qwak.build.v1.ValueType.Types\"b\n\x05Types\x12\x0b\n\x07INVALID\x10\x00\x12\t\n\x05\x42YTES\x10\x01\x12\n\n\x06STRING\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\n\n\x06\x44OUBLE\x10\x05\x12\t\n\x05\x46LOAT\x10\x06\x12\x08\n\x04\x42OOL\x10\x07\"j\n\x11ParameterCategory\"U\n\x08\x43\x61tegory\x12\x0b\n\x07INVALID\x10\x00\x12\n\n\x06\x45NTITY\x10\x01\x12\x0b\n\x07\x46\x45\x41TURE\x10\x02\x12\x0e\n\nPREDICTION\x10\x03\x12\x13\n\x0fINFERENCEOUTPUT\x10\x04\"\xc5\x06\n\x05\x42uild\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x10\n\x08\x63ommitId\x18\x02 \x01(\t\x12\x10\n\x08\x62ranchId\x18\x03 \x01(\t\x12\x13\n\x0b\x62uildConfig\x18\x04 \x01(\t\x12\x34\n\x0c\x62uild_status\x18\x05 \x01(\x0e\x32\x1e.com.qwak.build.v1.BuildStatus\x12\x0c\n\x04tags\x18\x06 \x03(\t\x12\r\n\x05steps\x18\x07 \x03(\t\x12\x34\n\x06params\x18\x08 \x03(\x0b\x32$.com.qwak.build.v1.Build.ParamsEntry\x12\x36\n\x07metrics\x18\t \x03(\x0b\x32%.com.qwak.build.v1.Build.MetricsEntry\x12\x34\n\x0cmodel_schema\x18\n \x01(\x0b\x32\x1e.com.qwak.build.v1.ModelSchema\x12\'\n\x05\x61udit\x18\x0b \x01(\x0b\x32\x18.com.qwak.build.v1.Audit\x12\x12\n\nmodel_uuid\x18\x0c \x01(\t\x12\x13\n\x0bsdk_version\x18\r \x01(\t\x12\x16\n\x0eimage_name_tag\x18\x0e \x01(\t\x12J\n\x1b\x62uild_configuration_message\x18\x0f \x01(\x0b\x32%.com.qwak.build.v1.BuildConfiguration\x12,\n\x08\x65nd_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x65nvironment_id\x18\x11 \x01(\t\x12\x1c\n\x14\x62uild_destined_image\x18\x12 \x01(\t\x12;\n\x10\x66ramework_models\x18\x13 \x03(\x0b\x32!.com.qwak.build.v1.FrameworkModel\x12(\n build_destined_image_pull_secret\x18\x14 \x01(\t\x12\x1b\n\x13\x66\x61ilure_reason_code\x18\x15 \x01(\t\x1a-\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\x9b\x01\n\x05\x41udit\x12\x12\n\ncreated_by\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x03 \x01(\t\x12\x34\n\x10last_modified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb3\x02\n\x12\x42uildConfiguration\x12<\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32\".com.qwak.build.v1.BuildProperties\x12\x36\n\tbuild_env\x18\x02 \x01(\x0b\x32#.com.qwak.build.v1.BuildEnvironment\x12\x36\n\tpre_build\x18\x03 \x01(\x0b\x32#.com.qwak.build.v1.BuildEnvironment\x12\x37\n\npost_build\x18\x04 \x01(\x0b\x32#.com.qwak.build.v1.BuildEnvironment\x12%\n\x04step\x18\x05 \x01(\x0b\x32\x17.com.qwak.build.v1.Step\x12\x0f\n\x07verbose\x18\x06 \x01(\x05\"\xba\x01\n\x0f\x42uildProperties\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x33\n\tmodel_uri\x18\x02 \x01(\x0b\x32 .com.qwak.build.v1.BuildModelUri\x12\x0c\n\x04tags\x18\x03 \x03(\t\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x05 \x01(\t\x12\x18\n\x10\x65nvironment_name\x18\x06 \x01(\t\x12\x16\n\x0egpu_compatible\x18\x07 \x01(\x08\"g\n\rBuildModelUri\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x10\n\x08main_dir\x18\x03 \x01(\t\x12#\n\x1b\x64\x65pendency_required_folders\x18\x04 \x03(\t\"\xd4\x01\n\x10\x42uildEnvironment\x12.\n\x06\x64ocker\x18\x01 \x01(\x0b\x32\x1e.com.qwak.build.v1.DockerBuild\x12,\n\x05local\x18\x02 \x01(\x0b\x32\x1d.com.qwak.build.v1.LocalBuild\x12\x32\n\npython_env\x18\x03 \x01(\x0b\x32\x1e.com.qwak.build.v1.PythonBuild\x12.\n\x06remote\x18\x04 \x01(\x0b\x32\x1e.com.qwak.build.v1.RemoteBuild\"\xae\x02\n\x0b\x44ockerBuild\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x41\n\nbuild_args\x18\x02 \x03(\x0b\x32-.com.qwak.build.v1.DockerBuild.BuildArgsEntry\x12\x10\n\x08\x65nv_vars\x18\x03 \x03(\t\x12\x10\n\x08no_cache\x18\x04 \x01(\x08\x12\x0e\n\x06params\x18\x05 \x03(\t\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x06 \x01(\t\x12\r\n\x05\x63\x61\x63he\x18\x07 \x01(\x08\x12\x0c\n\x04push\x18\x08 \x01(\x08\x12\'\n\x1fservice_account_key_secret_name\x18\t \x01(\t\x1a\x30\n\x0e\x42uildArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"2\n\nLocalBuild\x12\x13\n\x0b\x61ws_profile\x18\x01 \x01(\t\x12\x0f\n\x07no_push\x18\x02 \x01(\x08\"\x8c\x02\n\x0bPythonBuild\x12 \n\x18qwak_sdk_extra_index_url\x18\x01 \x01(\t\x12>\n\nvirtualenv\x18\x02 \x01(\x0b\x32*.com.qwak.build.v1.VirtualEnvironmentBuild\x12,\n\x05\x63onda\x18\x03 \x01(\x0b\x32\x1d.com.qwak.build.v1.CondaBuild\x12.\n\x06poetry\x18\x04 \x01(\x0b\x32\x1e.com.qwak.build.v1.PoetryBuild\x12\x1c\n\x14\x64\x65pendency_file_path\x18\x05 \x01(\t\x12\x1f\n\x17use_deprecated_resolver\x18\x06 \x01(\x08\" \n\nCondaBuild\x12\x12\n\nconda_file\x18\x01 \x01(\t\"8\n\x0bPoetryBuild\x12\x16\n\x0epython_version\x18\x01 \x01(\t\x12\x11\n\tlock_file\x18\x02 \x01(\t\"K\n\x17VirtualEnvironmentBuild\x12\x16\n\x0epython_version\x18\x01 \x01(\t\x12\x18\n\x10requirements_txt\x18\x02 \x01(\t\"\\\n\x0bRemoteBuild\x12\x11\n\tis_remote\x18\x01 \x01(\x08\x12:\n\tresources\x18\x02 \x01(\x0b\x32\'.com.qwak.build.v1.RemoteBuildResources\"\x8f\x01\n\x14RemoteBuildResources\x12\x0c\n\x04\x63pus\x18\x01 \x01(\x02\x12\x0e\n\x06memory\x18\x02 \x01(\t\x12\x33\n\x08gpu_type\x18\x03 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x04 \x01(\x05\x12\x10\n\x08instance\x18\x05 \x01(\t\"_\n\x04Step\x12\r\n\x05tests\x18\x01 \x01(\x08\x12\x1f\n\x17validate_build_artifact\x18\x02 \x01(\x08\x12\'\n\x1fvalidate_build_artifact_timeout\x18\x03 \x01(\x05\"\xdc\x01\n\x0b\x42uildFilter\x12\x0c\n\x04tags\x18\x01 \x03(\t\x12\x37\n\x0emetric_filters\x18\x02 \x03(\x0b\x32\x1f.com.qwak.build.v1.MetricFilter\x12=\n\x11parameter_filters\x18\x03 \x03(\x0b\x32\".com.qwak.build.v1.ParameterFilter\x12\x18\n\x10require_all_tags\x18\x04 \x01(\x08\x12\x1a\n\x12include_extra_tags\x18\x05 \x01(\x08\x12\x11\n\tbuild_ids\x18\x06 \x03(\t\"r\n\x0cMetricFilter\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\x12\x14\n\x0cmetric_value\x18\x02 \x01(\x02\x12\x37\n\x08operator\x18\x03 \x01(\x0e\x32%.com.qwak.build.v1.MetricOperatorType\"~\n\x0fParameterFilter\x12\x16\n\x0eparameter_name\x18\x01 \x01(\t\x12\x17\n\x0fparameter_value\x18\x02 \x01(\t\x12:\n\x08operator\x18\x03 \x01(\x0e\x32(.com.qwak.build.v1.ParameterOperatorType\"d\n\x13\x46rameworkModelsSpec\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12;\n\x10\x66ramework_models\x18\x02 \x03(\x0b\x32!.com.qwak.build.v1.FrameworkModel\"c\n\x0e\x46rameworkModel\x12I\n\x16huggingface_model_spec\x18\x02 \x01(\x0b\x32\'.com.qwak.build.v1.HuggingFaceModelSpecH\x00\x42\x06\n\x04type\"]\n\x14HuggingFaceModelSpec\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x12\n\nmodel_name\x18\x03 \x01(\t\x12\x0c\n\x04sha1\x18\x04 \x01(\t\"r\n\x11ScanResultSummary\x12(\n\x06issues\x18\x01 \x03(\x0b\x32\x18.com.qwak.build.v1.Issue\x12\x16\n\x0eui_direct_link\x18\x02 \x01(\t\x12\x1b\n\x13ui_scan_direct_link\x18\x03 \x01(\t\"a\n\x05Issue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08severity\x18\x02 \x01(\t\x12\x12\n\nissue_type\x18\x03 \x01(\t\x12\x0f\n\x07summary\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"L\n\x11\x42uildImageDetails\x12\x17\n\x0fimage_full_path\x18\x01 \x01(\t\x12\x1e\n\x16image_pull_secret_name\x18\x02 \x01(\t*\xe8\x01\n\x0b\x42uildStatus\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bIN_PROGRESS\x10\x01\x12\x0e\n\nSUCCESSFUL\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x1d\n\x19REMOTE_BUILD_INITIALIZING\x10\x04\x12\x1a\n\x16REMOTE_BUILD_CANCELLED\x10\x05\x12\x1a\n\x16REMOTE_BUILD_TIMED_OUT\x10\x06\x12\x18\n\x14REMOTE_BUILD_UNKNOWN\x10\x07\x12\x18\n\x14SYNCING_ENVIRONMENTS\x10\x08\x12\x14\n\x10\x46INISHED_SYNCING\x10\t*\xa0\x02\n\x12MetricOperatorType\x12 \n\x1cMETRIC_OPERATOR_TYPE_INVALID\x10\x00\x12\x1f\n\x1bMETRIC_OPERATOR_TYPE_EQUALS\x10\x01\x12#\n\x1fMETRIC_OPERATOR_TYPE_NOT_EQUALS\x10\x02\x12\"\n\x1eMETRIC_OPERATOR_TYPE_LESS_THAN\x10\x03\x12)\n%METRIC_OPERATOR_TYPE_LESS_THAN_EQUALS\x10\x04\x12%\n!METRIC_OPERATOR_TYPE_GREATER_THAN\x10\x05\x12,\n(METRIC_OPERATOR_TYPE_GREATER_THAN_EQUALS\x10\x06*\x88\x01\n\x15ParameterOperatorType\x12#\n\x1fPARAMETER_OPERATOR_TYPE_INVALID\x10\x00\x12\"\n\x1ePARAMETER_OPERATOR_TYPE_EQUALS\x10\x01\x12&\n\"PARAMETER_OPERATOR_TYPE_NOT_EQUALS\x10\x02\x42!\n\x11\x63om.qwak.build.v1B\nBuildProtoP\x01\x62\x06proto3')
 
 _BUILDSTATUS = DESCRIPTOR.enum_types_by_name['BuildStatus']
 BuildStatus = enum_type_wrapper.EnumTypeWrapper(_BUILDSTATUS)
 _METRICOPERATORTYPE = DESCRIPTOR.enum_types_by_name['MetricOperatorType']
 MetricOperatorType = enum_type_wrapper.EnumTypeWrapper(_METRICOPERATORTYPE)
 _PARAMETEROPERATORTYPE = DESCRIPTOR.enum_types_by_name['ParameterOperatorType']
 ParameterOperatorType = enum_type_wrapper.EnumTypeWrapper(_PARAMETEROPERATORTYPE)
@@ -402,20 +402,20 @@
   DESCRIPTOR._serialized_options = b'\n\021com.qwak.build.v1B\nBuildProtoP\001'
   _BUILD_PARAMSENTRY._options = None
   _BUILD_PARAMSENTRY._serialized_options = b'8\001'
   _BUILD_METRICSENTRY._options = None
   _BUILD_METRICSENTRY._serialized_options = b'8\001'
   _DOCKERBUILD_BUILDARGSENTRY._options = None
   _DOCKERBUILD_BUILDARGSENTRY._serialized_options = b'8\001'
-  _BUILDSTATUS._serialized_start=6130
-  _BUILDSTATUS._serialized_end=6362
-  _METRICOPERATORTYPE._serialized_start=6365
-  _METRICOPERATORTYPE._serialized_end=6653
-  _PARAMETEROPERATORTYPE._serialized_start=6656
-  _PARAMETEROPERATORTYPE._serialized_end=6792
+  _BUILDSTATUS._serialized_start=6208
+  _BUILDSTATUS._serialized_end=6440
+  _METRICOPERATORTYPE._serialized_start=6443
+  _METRICOPERATORTYPE._serialized_end=6731
+  _PARAMETEROPERATORTYPE._serialized_start=6734
+  _PARAMETEROPERATORTYPE._serialized_end=6870
   _MODELSCHEMA._serialized_start=107
   _MODELSCHEMA._serialized_end=325
   _ENTITY._serialized_start=327
   _ENTITY._serialized_end=393
   _FEATURE._serialized_start=396
   _FEATURE._serialized_end=948
   _ONTHEFLYFEATURE._serialized_start=951
@@ -457,49 +457,49 @@
   _AUDIT._serialized_start=3039
   _AUDIT._serialized_end=3194
   _BUILDCONFIGURATION._serialized_start=3197
   _BUILDCONFIGURATION._serialized_end=3504
   _BUILDPROPERTIES._serialized_start=3507
   _BUILDPROPERTIES._serialized_end=3693
   _BUILDMODELURI._serialized_start=3695
-  _BUILDMODELURI._serialized_end=3761
-  _BUILDENVIRONMENT._serialized_start=3764
-  _BUILDENVIRONMENT._serialized_end=3976
-  _DOCKERBUILD._serialized_start=3979
-  _DOCKERBUILD._serialized_end=4240
-  _DOCKERBUILD_BUILDARGSENTRY._serialized_start=4192
-  _DOCKERBUILD_BUILDARGSENTRY._serialized_end=4240
-  _LOCALBUILD._serialized_start=4242
-  _LOCALBUILD._serialized_end=4292
-  _PYTHONBUILD._serialized_start=4295
-  _PYTHONBUILD._serialized_end=4563
-  _CONDABUILD._serialized_start=4565
-  _CONDABUILD._serialized_end=4597
-  _POETRYBUILD._serialized_start=4599
-  _POETRYBUILD._serialized_end=4655
-  _VIRTUALENVIRONMENTBUILD._serialized_start=4657
-  _VIRTUALENVIRONMENTBUILD._serialized_end=4732
-  _REMOTEBUILD._serialized_start=4734
-  _REMOTEBUILD._serialized_end=4826
-  _REMOTEBUILDRESOURCES._serialized_start=4829
-  _REMOTEBUILDRESOURCES._serialized_end=4972
-  _STEP._serialized_start=4974
-  _STEP._serialized_end=5069
-  _BUILDFILTER._serialized_start=5072
-  _BUILDFILTER._serialized_end=5292
-  _METRICFILTER._serialized_start=5294
-  _METRICFILTER._serialized_end=5408
-  _PARAMETERFILTER._serialized_start=5410
-  _PARAMETERFILTER._serialized_end=5536
-  _FRAMEWORKMODELSSPEC._serialized_start=5538
-  _FRAMEWORKMODELSSPEC._serialized_end=5638
-  _FRAMEWORKMODEL._serialized_start=5640
-  _FRAMEWORKMODEL._serialized_end=5739
-  _HUGGINGFACEMODELSPEC._serialized_start=5741
-  _HUGGINGFACEMODELSPEC._serialized_end=5834
-  _SCANRESULTSUMMARY._serialized_start=5836
-  _SCANRESULTSUMMARY._serialized_end=5950
-  _ISSUE._serialized_start=5952
-  _ISSUE._serialized_end=6049
-  _BUILDIMAGEDETAILS._serialized_start=6051
-  _BUILDIMAGEDETAILS._serialized_end=6127
+  _BUILDMODELURI._serialized_end=3798
+  _BUILDENVIRONMENT._serialized_start=3801
+  _BUILDENVIRONMENT._serialized_end=4013
+  _DOCKERBUILD._serialized_start=4016
+  _DOCKERBUILD._serialized_end=4318
+  _DOCKERBUILD_BUILDARGSENTRY._serialized_start=4270
+  _DOCKERBUILD_BUILDARGSENTRY._serialized_end=4318
+  _LOCALBUILD._serialized_start=4320
+  _LOCALBUILD._serialized_end=4370
+  _PYTHONBUILD._serialized_start=4373
+  _PYTHONBUILD._serialized_end=4641
+  _CONDABUILD._serialized_start=4643
+  _CONDABUILD._serialized_end=4675
+  _POETRYBUILD._serialized_start=4677
+  _POETRYBUILD._serialized_end=4733
+  _VIRTUALENVIRONMENTBUILD._serialized_start=4735
+  _VIRTUALENVIRONMENTBUILD._serialized_end=4810
+  _REMOTEBUILD._serialized_start=4812
+  _REMOTEBUILD._serialized_end=4904
+  _REMOTEBUILDRESOURCES._serialized_start=4907
+  _REMOTEBUILDRESOURCES._serialized_end=5050
+  _STEP._serialized_start=5052
+  _STEP._serialized_end=5147
+  _BUILDFILTER._serialized_start=5150
+  _BUILDFILTER._serialized_end=5370
+  _METRICFILTER._serialized_start=5372
+  _METRICFILTER._serialized_end=5486
+  _PARAMETERFILTER._serialized_start=5488
+  _PARAMETERFILTER._serialized_end=5614
+  _FRAMEWORKMODELSSPEC._serialized_start=5616
+  _FRAMEWORKMODELSSPEC._serialized_end=5716
+  _FRAMEWORKMODEL._serialized_start=5718
+  _FRAMEWORKMODEL._serialized_end=5817
+  _HUGGINGFACEMODELSPEC._serialized_start=5819
+  _HUGGINGFACEMODELSPEC._serialized_end=5912
+  _SCANRESULTSUMMARY._serialized_start=5914
+  _SCANRESULTSUMMARY._serialized_end=6028
+  _ISSUE._serialized_start=6030
+  _ISSUE._serialized_end=6127
+  _BUILDIMAGEDETAILS._serialized_start=6129
+  _BUILDIMAGEDETAILS._serialized_end=6205
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -738,25 +738,29 @@
 
 class BuildModelUri(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     URI_FIELD_NUMBER: builtins.int
     GIT_BRANCH_FIELD_NUMBER: builtins.int
     MAIN_DIR_FIELD_NUMBER: builtins.int
+    DEPENDENCY_REQUIRED_FOLDERS_FIELD_NUMBER: builtins.int
     uri: builtins.str
     git_branch: builtins.str
     main_dir: builtins.str
+    @property
+    def dependency_required_folders(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
         uri: builtins.str = ...,
         git_branch: builtins.str = ...,
         main_dir: builtins.str = ...,
+        dependency_required_folders: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["git_branch", b"git_branch", "main_dir", b"main_dir", "uri", b"uri"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dependency_required_folders", b"dependency_required_folders", "git_branch", b"git_branch", "main_dir", b"main_dir", "uri", b"uri"]) -> None: ...
 
 global___BuildModelUri = BuildModelUri
 
 class BuildEnvironment(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DOCKER_FIELD_NUMBER: builtins.int
@@ -806,38 +810,41 @@
     BUILD_ARGS_FIELD_NUMBER: builtins.int
     ENV_VARS_FIELD_NUMBER: builtins.int
     NO_CACHE_FIELD_NUMBER: builtins.int
     PARAMS_FIELD_NUMBER: builtins.int
     ASSUMED_IAM_ROLE_ARN_FIELD_NUMBER: builtins.int
     CACHE_FIELD_NUMBER: builtins.int
     PUSH_FIELD_NUMBER: builtins.int
+    SERVICE_ACCOUNT_KEY_SECRET_NAME_FIELD_NUMBER: builtins.int
     base_image: builtins.str
     @property
     def build_args(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     @property
     def env_vars(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     no_cache: builtins.bool
     @property
     def params(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     assumed_iam_role_arn: builtins.str
     cache: builtins.bool
     push: builtins.bool
+    service_account_key_secret_name: builtins.str
     def __init__(
         self,
         *,
         base_image: builtins.str = ...,
         build_args: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         env_vars: collections.abc.Iterable[builtins.str] | None = ...,
         no_cache: builtins.bool = ...,
         params: collections.abc.Iterable[builtins.str] | None = ...,
         assumed_iam_role_arn: builtins.str = ...,
         cache: builtins.bool = ...,
         push: builtins.bool = ...,
+        service_account_key_secret_name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["assumed_iam_role_arn", b"assumed_iam_role_arn", "base_image", b"base_image", "build_args", b"build_args", "cache", b"cache", "env_vars", b"env_vars", "no_cache", b"no_cache", "params", b"params", "push", b"push"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["assumed_iam_role_arn", b"assumed_iam_role_arn", "base_image", b"base_image", "build_args", b"build_args", "cache", b"cache", "env_vars", b"env_vars", "no_cache", b"no_cache", "params", b"params", "push", b"push", "service_account_key_secret_name", b"service_account_key_secret_name"]) -> None: ...
 
 global___DockerBuild = DockerBuild
 
 class LocalBuild(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AWS_PROFILE_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 from _qwak_proto.qwak.fitness_service import fitness_pb2 as qwak_dot_fitness__service_dot_fitness__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17qwak/builds/build.proto\x12\x18qwak.builds.orchestrator\x1a/qwak/user_application/common/v0/resources.proto\x1a\"qwak/fitness_service/fitness.proto\"\xc8\x05\n\x0fRemoteBuildSpec\x12\x43\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32).qwak.builds.orchestrator.BuildProperties\x12\x35\n\tbuild_env\x18\x02 \x01(\x0b\x32\".qwak.builds.orchestrator.BuildEnv\x12\x43\n\rcpu_resources\x18\x03 \x01(\x0b\x32&.qwak.builds.orchestrator.CpuResourcesB\x02\x18\x01H\x00\x12\x43\n\rgpu_resources\x18\x07 \x01(\x0b\x32&.qwak.builds.orchestrator.GpuResourcesB\x02\x18\x01H\x00\x12\x62\n\x1c\x63lient_pod_compute_resources\x18\r \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResourcesH\x00\x12\x0f\n\x07verbose\x18\x04 \x01(\x05\x12\x17\n\x0f\x62uild_code_path\x18\x05 \x01(\t\x12\x14\n\x0c\x62uild_config\x18\x06 \x01(\t\x12\x15\n\rbuild_v1_flag\x18\x08 \x01(\x08\x12H\n\x13\x62uild_properties_v1\x18\t \x01(\x0b\x32+.qwak.builds.orchestrator.BuildPropertiesV1\x12\x13\n\x0b\x62uild_steps\x18\n \x03(\t\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x13\n\x0bsdk_version\x18\x0c \x01(\t\x12=\n\x0fpurchase_option\x18\x0e \x01(\x0e\x32$.qwak.fitness.service.PurchaseOption\x12\x1c\n\x14\x62uild_destined_image\x18\x0f \x01(\tB\x0b\n\tResources\"g\n\x11\x42uildPropertiesV1\x12\x18\n\x10\x62uild_config_url\x18\x01 \x01(\t\x12\x1a\n\x12qwak_sdk_wheel_url\x18\x02 \x01(\t\x12\x1c\n\x14qwak_sdk_version_url\x18\x03 \x01(\t\"\xa6\x01\n\x0f\x42uildProperties\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x39\n\tmodel_uri\x18\x05 \x01(\x0b\x32&.qwak.builds.orchestrator.ModelUriSpec\x12\x16\n\x0egpu_compatible\x18\x06 \x01(\x08\"\x8d\x01\n\x0cModelUriSpec\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x17\n\x0fgit_credentials\x18\x03 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x04 \x01(\t\x12\x11\n\tcommit_id\x18\x05 \x01(\t\x12\x10\n\x08main_dir\x18\x06 \x01(\t\"|\n\x08\x42uildEnv\x12\x37\n\ndocker_env\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.DockerEnv\x12\x37\n\npython_env\x18\x02 \x01(\x0b\x32#.qwak.builds.orchestrator.PythonEnv\"a\n\tDockerEnv\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x10\n\x08\x65nv_vars\x18\x02 \x03(\t\x12\x10\n\x08no_cache\x18\x03 \x01(\x08\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x04 \x01(\t\"|\n\tPythonEnv\x12\x17\n\x0fgit_credentials\x18\x01 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x02 \x01(\t\x12\x18\n\x10qwak_sdk_version\x18\x03 \x01(\t\x12\x1c\n\x14qwak_sdk_extra_index\x18\x04 \x01(\t\"n\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12:\n\x0cmemory_units\x18\x03 \x01(\x0e\x32$.qwak.builds.orchestrator.MemoryUnit\"W\n\x0cGpuResources\x12\x33\n\x08gpu_type\x18\x01 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x91\x01\n\x13\x44\x61taTableDefinition\x12?\n\x07\x63olumns\x18\x01 \x03(\x0b\x32..qwak.builds.orchestrator.DataColumnDefinition\x12\x39\n\x0b\x64\x61ta_format\x18\x02 \x01(\x0b\x32$.qwak.builds.orchestrator.DataFormat\"\\\n\x14\x44\x61taColumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x04type\x18\x02 \x01(\x0e\x32(.qwak.builds.orchestrator.DataColumnType\"J\n\nDataFormat\x12\x32\n\x03\x63sv\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.CsvFormatH\x00\x42\x08\n\x06\x66ormat\"G\n\tCsvFormat\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\x12\n\nquote_char\x18\x02 \x01(\t\x12\x13\n\x0b\x65scape_char\x18\x03 \x01(\t\"\xa5\x01\n\x0e\x42uildInitiator\x12<\n\x04user\x18\x01 \x01(\x0b\x32,.qwak.builds.orchestrator.UserBuildInitiatorH\x00\x12H\n\nautomation\x18\x02 \x01(\x0b\x32\x32.qwak.builds.orchestrator.AutomationBuildInitiatorH\x00\x42\x0b\n\tInitiator\"\x14\n\x12UserBuildInitiator\"`\n\x18\x41utomationBuildInitiator\x12\x15\n\rautomation_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x17\n\x0f\x61utomation_name\x18\x03 \x01(\t*7\n\nMemoryUnit\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*w\n\x07GpuType\x12\x0b\n\x07INVALID\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06*d\n\x0e\x44\x61taColumnType\x12\x17\n\x13INVALID_COLUMN_TYPE\x10\x00\x12\n\n\x06OBJECT\x10\x01\x12\x07\n\x03INT\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07\x42OOLEAN\x10\x04\x12\x0c\n\x08\x44\x41TETIME\x10\x05*K\n\x13\x42\x61seDockerImageType\x12\"\n\x1eUNKNOWN_BASE_DOCKER_IMAGE_TYPE\x10\x00\x12\x07\n\x03\x43PU\x10\x01\x12\x07\n\x03GPU\x10\x02\x42\'\n#com.qwak.ai.builds.orchestrator.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17qwak/builds/build.proto\x12\x18qwak.builds.orchestrator\x1a/qwak/user_application/common/v0/resources.proto\x1a\"qwak/fitness_service/fitness.proto\"\xc8\x05\n\x0fRemoteBuildSpec\x12\x43\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32).qwak.builds.orchestrator.BuildProperties\x12\x35\n\tbuild_env\x18\x02 \x01(\x0b\x32\".qwak.builds.orchestrator.BuildEnv\x12\x43\n\rcpu_resources\x18\x03 \x01(\x0b\x32&.qwak.builds.orchestrator.CpuResourcesB\x02\x18\x01H\x00\x12\x43\n\rgpu_resources\x18\x07 \x01(\x0b\x32&.qwak.builds.orchestrator.GpuResourcesB\x02\x18\x01H\x00\x12\x62\n\x1c\x63lient_pod_compute_resources\x18\r \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResourcesH\x00\x12\x0f\n\x07verbose\x18\x04 \x01(\x05\x12\x17\n\x0f\x62uild_code_path\x18\x05 \x01(\t\x12\x14\n\x0c\x62uild_config\x18\x06 \x01(\t\x12\x15\n\rbuild_v1_flag\x18\x08 \x01(\x08\x12H\n\x13\x62uild_properties_v1\x18\t \x01(\x0b\x32+.qwak.builds.orchestrator.BuildPropertiesV1\x12\x13\n\x0b\x62uild_steps\x18\n \x03(\t\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x13\n\x0bsdk_version\x18\x0c \x01(\t\x12=\n\x0fpurchase_option\x18\x0e \x01(\x0e\x32$.qwak.fitness.service.PurchaseOption\x12\x1c\n\x14\x62uild_destined_image\x18\x0f \x01(\tB\x0b\n\tResources\"g\n\x11\x42uildPropertiesV1\x12\x18\n\x10\x62uild_config_url\x18\x01 \x01(\t\x12\x1a\n\x12qwak_sdk_wheel_url\x18\x02 \x01(\t\x12\x1c\n\x14qwak_sdk_version_url\x18\x03 \x01(\t\"\xa6\x01\n\x0f\x42uildProperties\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x39\n\tmodel_uri\x18\x05 \x01(\x0b\x32&.qwak.builds.orchestrator.ModelUriSpec\x12\x16\n\x0egpu_compatible\x18\x06 \x01(\x08\"\xb2\x01\n\x0cModelUriSpec\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x17\n\x0fgit_credentials\x18\x03 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x04 \x01(\t\x12\x11\n\tcommit_id\x18\x05 \x01(\t\x12\x10\n\x08main_dir\x18\x06 \x01(\t\x12#\n\x1b\x64\x65pendency_required_folders\x18\x07 \x03(\t\"|\n\x08\x42uildEnv\x12\x37\n\ndocker_env\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.DockerEnv\x12\x37\n\npython_env\x18\x02 \x01(\x0b\x32#.qwak.builds.orchestrator.PythonEnv\"\x8a\x01\n\tDockerEnv\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x10\n\x08\x65nv_vars\x18\x02 \x03(\t\x12\x10\n\x08no_cache\x18\x03 \x01(\x08\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x04 \x01(\t\x12\'\n\x1fservice_account_key_secret_name\x18\x05 \x01(\t\"|\n\tPythonEnv\x12\x17\n\x0fgit_credentials\x18\x01 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x02 \x01(\t\x12\x18\n\x10qwak_sdk_version\x18\x03 \x01(\t\x12\x1c\n\x14qwak_sdk_extra_index\x18\x04 \x01(\t\"n\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12:\n\x0cmemory_units\x18\x03 \x01(\x0e\x32$.qwak.builds.orchestrator.MemoryUnit\"W\n\x0cGpuResources\x12\x33\n\x08gpu_type\x18\x01 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x91\x01\n\x13\x44\x61taTableDefinition\x12?\n\x07\x63olumns\x18\x01 \x03(\x0b\x32..qwak.builds.orchestrator.DataColumnDefinition\x12\x39\n\x0b\x64\x61ta_format\x18\x02 \x01(\x0b\x32$.qwak.builds.orchestrator.DataFormat\"\\\n\x14\x44\x61taColumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x04type\x18\x02 \x01(\x0e\x32(.qwak.builds.orchestrator.DataColumnType\"J\n\nDataFormat\x12\x32\n\x03\x63sv\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.CsvFormatH\x00\x42\x08\n\x06\x66ormat\"G\n\tCsvFormat\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\x12\n\nquote_char\x18\x02 \x01(\t\x12\x13\n\x0b\x65scape_char\x18\x03 \x01(\t\"\xa5\x01\n\x0e\x42uildInitiator\x12<\n\x04user\x18\x01 \x01(\x0b\x32,.qwak.builds.orchestrator.UserBuildInitiatorH\x00\x12H\n\nautomation\x18\x02 \x01(\x0b\x32\x32.qwak.builds.orchestrator.AutomationBuildInitiatorH\x00\x42\x0b\n\tInitiator\"\x14\n\x12UserBuildInitiator\"`\n\x18\x41utomationBuildInitiator\x12\x15\n\rautomation_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x17\n\x0f\x61utomation_name\x18\x03 \x01(\t*7\n\nMemoryUnit\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x8c\x02\n\x07GpuType\x12\x0b\n\x07INVALID\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06\x12\x14\n\x10NVIDIA_T4_1_4_15\x10\x07\x12\x14\n\x10NVIDIA_T4_1_8_30\x10\x08\x12\x15\n\x11NVIDIA_T4_1_16_60\x10\t\x12\x1e\n\x1aNVIDIA_A100_80GB_8_96_1360\x10\n\x12\x16\n\x12NVIDIA_V100_1_8_52\x10\x0b\x12\x18\n\x14NVIDIA_V100_4_32_208\x10\x0c*d\n\x0e\x44\x61taColumnType\x12\x17\n\x13INVALID_COLUMN_TYPE\x10\x00\x12\n\n\x06OBJECT\x10\x01\x12\x07\n\x03INT\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07\x42OOLEAN\x10\x04\x12\x0c\n\x08\x44\x41TETIME\x10\x05*K\n\x13\x42\x61seDockerImageType\x12\"\n\x1eUNKNOWN_BASE_DOCKER_IMAGE_TYPE\x10\x00\x12\x07\n\x03\x43PU\x10\x01\x12\x07\n\x03GPU\x10\x02\x42\'\n#com.qwak.ai.builds.orchestrator.apiP\x01\x62\x06proto3')
 
 _MEMORYUNIT = DESCRIPTOR.enum_types_by_name['MemoryUnit']
 MemoryUnit = enum_type_wrapper.EnumTypeWrapper(_MEMORYUNIT)
 _GPUTYPE = DESCRIPTOR.enum_types_by_name['GpuType']
 GpuType = enum_type_wrapper.EnumTypeWrapper(_GPUTYPE)
 _DATACOLUMNTYPE = DESCRIPTOR.enum_types_by_name['DataColumnType']
 DataColumnType = enum_type_wrapper.EnumTypeWrapper(_DATACOLUMNTYPE)
@@ -33,14 +33,20 @@
 INVALID = 0
 NVIDIA_K80 = 1
 NVIDIA_V100 = 2
 NVIDIA_A100 = 3
 NVIDIA_T4 = 4
 NVIDIA_A10G = 5
 NVIDIA_L4 = 6
+NVIDIA_T4_1_4_15 = 7
+NVIDIA_T4_1_8_30 = 8
+NVIDIA_T4_1_16_60 = 9
+NVIDIA_A100_80GB_8_96_1360 = 10
+NVIDIA_V100_1_8_52 = 11
+NVIDIA_V100_4_32_208 = 12
 INVALID_COLUMN_TYPE = 0
 OBJECT = 1
 INT = 2
 FLOAT = 3
 BOOLEAN = 4
 DATETIME = 5
 UNKNOWN_BASE_DOCKER_IMAGE_TYPE = 0
@@ -180,48 +186,48 @@
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n#com.qwak.ai.builds.orchestrator.apiP\001'
   _REMOTEBUILDSPEC.fields_by_name['cpu_resources']._options = None
   _REMOTEBUILDSPEC.fields_by_name['cpu_resources']._serialized_options = b'\030\001'
   _REMOTEBUILDSPEC.fields_by_name['gpu_resources']._options = None
   _REMOTEBUILDSPEC.fields_by_name['gpu_resources']._serialized_options = b'\030\001'
-  _MEMORYUNIT._serialized_start=2502
-  _MEMORYUNIT._serialized_end=2557
-  _GPUTYPE._serialized_start=2559
-  _GPUTYPE._serialized_end=2678
-  _DATACOLUMNTYPE._serialized_start=2680
-  _DATACOLUMNTYPE._serialized_end=2780
-  _BASEDOCKERIMAGETYPE._serialized_start=2782
-  _BASEDOCKERIMAGETYPE._serialized_end=2857
+  _MEMORYUNIT._serialized_start=2581
+  _MEMORYUNIT._serialized_end=2636
+  _GPUTYPE._serialized_start=2639
+  _GPUTYPE._serialized_end=2907
+  _DATACOLUMNTYPE._serialized_start=2909
+  _DATACOLUMNTYPE._serialized_end=3009
+  _BASEDOCKERIMAGETYPE._serialized_start=3011
+  _BASEDOCKERIMAGETYPE._serialized_end=3086
   _REMOTEBUILDSPEC._serialized_start=139
   _REMOTEBUILDSPEC._serialized_end=851
   _BUILDPROPERTIESV1._serialized_start=853
   _BUILDPROPERTIESV1._serialized_end=956
   _BUILDPROPERTIES._serialized_start=959
   _BUILDPROPERTIES._serialized_end=1125
   _MODELURISPEC._serialized_start=1128
-  _MODELURISPEC._serialized_end=1269
-  _BUILDENV._serialized_start=1271
-  _BUILDENV._serialized_end=1395
-  _DOCKERENV._serialized_start=1397
-  _DOCKERENV._serialized_end=1494
-  _PYTHONENV._serialized_start=1496
-  _PYTHONENV._serialized_end=1620
-  _CPURESOURCES._serialized_start=1622
-  _CPURESOURCES._serialized_end=1732
-  _GPURESOURCES._serialized_start=1734
-  _GPURESOURCES._serialized_end=1821
-  _DATATABLEDEFINITION._serialized_start=1824
-  _DATATABLEDEFINITION._serialized_end=1969
-  _DATACOLUMNDEFINITION._serialized_start=1971
-  _DATACOLUMNDEFINITION._serialized_end=2063
-  _DATAFORMAT._serialized_start=2065
-  _DATAFORMAT._serialized_end=2139
-  _CSVFORMAT._serialized_start=2141
-  _CSVFORMAT._serialized_end=2212
-  _BUILDINITIATOR._serialized_start=2215
-  _BUILDINITIATOR._serialized_end=2380
-  _USERBUILDINITIATOR._serialized_start=2382
-  _USERBUILDINITIATOR._serialized_end=2402
-  _AUTOMATIONBUILDINITIATOR._serialized_start=2404
-  _AUTOMATIONBUILDINITIATOR._serialized_end=2500
+  _MODELURISPEC._serialized_end=1306
+  _BUILDENV._serialized_start=1308
+  _BUILDENV._serialized_end=1432
+  _DOCKERENV._serialized_start=1435
+  _DOCKERENV._serialized_end=1573
+  _PYTHONENV._serialized_start=1575
+  _PYTHONENV._serialized_end=1699
+  _CPURESOURCES._serialized_start=1701
+  _CPURESOURCES._serialized_end=1811
+  _GPURESOURCES._serialized_start=1813
+  _GPURESOURCES._serialized_end=1900
+  _DATATABLEDEFINITION._serialized_start=1903
+  _DATATABLEDEFINITION._serialized_end=2048
+  _DATACOLUMNDEFINITION._serialized_start=2050
+  _DATACOLUMNDEFINITION._serialized_end=2142
+  _DATAFORMAT._serialized_start=2144
+  _DATAFORMAT._serialized_end=2218
+  _CSVFORMAT._serialized_start=2220
+  _CSVFORMAT._serialized_end=2291
+  _BUILDINITIATOR._serialized_start=2294
+  _BUILDINITIATOR._serialized_end=2459
+  _USERBUILDINITIATOR._serialized_start=2461
+  _USERBUILDINITIATOR._serialized_end=2481
+  _AUTOMATIONBUILDINITIATOR._serialized_start=2483
+  _AUTOMATIONBUILDINITIATOR._serialized_end=2579
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -46,24 +46,52 @@
     INVALID: _GpuType.ValueType  # 0
     NVIDIA_K80: _GpuType.ValueType  # 1
     NVIDIA_V100: _GpuType.ValueType  # 2
     NVIDIA_A100: _GpuType.ValueType  # 3
     NVIDIA_T4: _GpuType.ValueType  # 4
     NVIDIA_A10G: _GpuType.ValueType  # 5
     NVIDIA_L4: _GpuType.ValueType  # 6
+    NVIDIA_T4_1_4_15: _GpuType.ValueType  # 7
+    """More specific node types
+    t4.xl
+    """
+    NVIDIA_T4_1_8_30: _GpuType.ValueType  # 8
+    """t4.2xl"""
+    NVIDIA_T4_1_16_60: _GpuType.ValueType  # 9
+    """t4.4xl"""
+    NVIDIA_A100_80GB_8_96_1360: _GpuType.ValueType  # 10
+    """a100.8xl"""
+    NVIDIA_V100_1_8_52: _GpuType.ValueType  # 11
+    """a100.xl"""
+    NVIDIA_V100_4_32_208: _GpuType.ValueType  # 12
+    """v100.4xl"""
 
 class GpuType(_GpuType, metaclass=_GpuTypeEnumTypeWrapper): ...
 
 INVALID: GpuType.ValueType  # 0
 NVIDIA_K80: GpuType.ValueType  # 1
 NVIDIA_V100: GpuType.ValueType  # 2
 NVIDIA_A100: GpuType.ValueType  # 3
 NVIDIA_T4: GpuType.ValueType  # 4
 NVIDIA_A10G: GpuType.ValueType  # 5
 NVIDIA_L4: GpuType.ValueType  # 6
+NVIDIA_T4_1_4_15: GpuType.ValueType  # 7
+"""More specific node types
+t4.xl
+"""
+NVIDIA_T4_1_8_30: GpuType.ValueType  # 8
+"""t4.2xl"""
+NVIDIA_T4_1_16_60: GpuType.ValueType  # 9
+"""t4.4xl"""
+NVIDIA_A100_80GB_8_96_1360: GpuType.ValueType  # 10
+"""a100.8xl"""
+NVIDIA_V100_1_8_52: GpuType.ValueType  # 11
+"""a100.xl"""
+NVIDIA_V100_4_32_208: GpuType.ValueType  # 12
+"""v100.4xl"""
 global___GpuType = GpuType
 
 class _DataColumnType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _DataColumnTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_DataColumnType.ValueType], builtins.type):  # noqa: F821
@@ -246,37 +274,42 @@
 
     URI_FIELD_NUMBER: builtins.int
     GIT_BRANCH_FIELD_NUMBER: builtins.int
     GIT_CREDENTIALS_FIELD_NUMBER: builtins.int
     GIT_CREDENTIALS_SECRET_FIELD_NUMBER: builtins.int
     COMMIT_ID_FIELD_NUMBER: builtins.int
     MAIN_DIR_FIELD_NUMBER: builtins.int
+    DEPENDENCY_REQUIRED_FOLDERS_FIELD_NUMBER: builtins.int
     uri: builtins.str
     """Model code to build upon, can be a download link or a git repo"""
     git_branch: builtins.str
     """Model code branch to clone"""
     git_credentials: builtins.str
     """Git credentials"""
     git_credentials_secret: builtins.str
     """Secret to fetch git credentials, overrides git_credentials if set"""
     commit_id: builtins.str
     """Commit id - filled when using local model code which is part of a git repo"""
     main_dir: builtins.str
     """Override for main dir of model"""
+    @property
+    def dependency_required_folders(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Required folders for the model"""
     def __init__(
         self,
         *,
         uri: builtins.str = ...,
         git_branch: builtins.str = ...,
         git_credentials: builtins.str = ...,
         git_credentials_secret: builtins.str = ...,
         commit_id: builtins.str = ...,
         main_dir: builtins.str = ...,
+        dependency_required_folders: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["commit_id", b"commit_id", "git_branch", b"git_branch", "git_credentials", b"git_credentials", "git_credentials_secret", b"git_credentials_secret", "main_dir", b"main_dir", "uri", b"uri"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["commit_id", b"commit_id", "dependency_required_folders", b"dependency_required_folders", "git_branch", b"git_branch", "git_credentials", b"git_credentials", "git_credentials_secret", b"git_credentials_secret", "main_dir", b"main_dir", "uri", b"uri"]) -> None: ...
 
 global___ModelUriSpec = ModelUriSpec
 
 class BuildEnv(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DOCKER_ENV_FIELD_NUMBER: builtins.int
@@ -299,34 +332,38 @@
 class DockerEnv(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BASE_IMAGE_FIELD_NUMBER: builtins.int
     ENV_VARS_FIELD_NUMBER: builtins.int
     NO_CACHE_FIELD_NUMBER: builtins.int
     ASSUMED_IAM_ROLE_ARN_FIELD_NUMBER: builtins.int
+    SERVICE_ACCOUNT_KEY_SECRET_NAME_FIELD_NUMBER: builtins.int
     base_image: builtins.str
     """Base image to use for serving"""
     @property
     def env_vars(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Environment variables for the model code"""
     no_cache: builtins.bool
     """Don't use remote cache to build the images, defaults to use cache,
     if the model dependencies changed significantly it could be faster and better to run with no cache
     """
     assumed_iam_role_arn: builtins.str
     """Custom IAM role to be assumed by model"""
+    service_account_key_secret_name: builtins.str
+    """Service account key secret name for gcp"""
     def __init__(
         self,
         *,
         base_image: builtins.str = ...,
         env_vars: collections.abc.Iterable[builtins.str] | None = ...,
         no_cache: builtins.bool = ...,
         assumed_iam_role_arn: builtins.str = ...,
+        service_account_key_secret_name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["assumed_iam_role_arn", b"assumed_iam_role_arn", "base_image", b"base_image", "env_vars", b"env_vars", "no_cache", b"no_cache"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["assumed_iam_role_arn", b"assumed_iam_role_arn", "base_image", b"base_image", "env_vars", b"env_vars", "no_cache", b"no_cache", "service_account_key_secret_name", b"service_account_key_secret_name"]) -> None: ...
 
 global___DockerEnv = DockerEnv
 
 class PythonEnv(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GIT_CREDENTIALS_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.deployment import deployment_pb2 as qwak_dot_deployment_dot_deployment__pb2
 from _qwak_proto.qwak.builds import build_pb2 as qwak_dot_builds_dot_build__pb2
 from _qwak_proto.qwak.fitness_service import status_pb2 as qwak_dot_fitness__service_dot_status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18qwak/builds/builds.proto\x12\x16qwak.builds.management\x1a\x1fgoogle/protobuf/timestamp.proto\x1a qwak/deployment/deployment.proto\x1a\x17qwak/builds/build.proto\x1a!qwak/fitness_service/status.proto\"\xf4\x05\n\x05\x42uild\x12\x35\n\nbuild_spec\x18\x01 \x01(\x0b\x32!.qwak.builds.management.BuildSpec\x12\x39\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32#.qwak.builds.management.BuildStatus\x12\x39\n\x0cmodel_schema\x18\x03 \x01(\x0b\x32#.qwak.builds.management.ModelSchema\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x05 \x01(\t\x12\x34\n\x10last_modified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x07 \x01(\t\x12V\n\x17\x64\x65ployment_build_status\x18\x08 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatusB\x02\x18\x01\x12V\n\x14hosting_service_type\x18\t \x01(\x0e\x32\x38.qwak.deployment.management.DeploymentHostingServiceType\x12,\n\x08\x65nd_date\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16\x61vailable_environments\x18\x0b \x03(\t\x12\x1d\n\x15\x64\x65ployed_environments\x18\x0c \x03(\t\x12\x32\n\tpodStatus\x18\r \x01(\x0b\x32\x1f.qwak.fitness.service.PodStatus\x12\x16\n\x0eimage_name_tag\x18\x0e \x01(\t\x12\x41\n\x0f\x62uild_initiator\x18\x0f \x01(\x0b\x32(.qwak.builds.orchestrator.BuildInitiator\"\x86\x03\n\tBuildSpec\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x11\n\tcommit_id\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\t\x12\x11\n\tbranch_id\x18\x08 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x03(\t\x12T\n\x1a\x65xperiment_tracking_values\x18\x06 \x01(\x0b\x32\x30.qwak.builds.management.ExperimentTrackingValues\x12G\n\x13\x62uild_configuration\x18\x07 \x01(\x0b\x32*.qwak.builds.management.BuildConfiguration\x12\x17\n\x0f\x62uild_code_path\x18\t \x01(\t\x12\x13\n\x0b\x62uild_steps\x18\n \x03(\t\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x12\n\nmodel_uuid\x18\x0c \x01(\t\x12\x13\n\x0bsdk_version\x18\r \x01(\t\"\xee\x01\n\x0bModelSchema\x12\x30\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x31\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32\x1f.qwak.builds.management.Feature\x12\x37\n\x0bpredictions\x18\x03 \x03(\x0b\x32\".qwak.builds.management.Prediction\x12\x41\n\x10inference_output\x18\x04 \x03(\x0b\x32\'.qwak.builds.management.InferenceOutput\"G\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"\xd0\x04\n\x07\x46\x65\x61ture\x12=\n\rbatch_feature\x18\x01 \x01(\x0b\x32$.qwak.builds.management.BatchFeatureH\x00\x12\x43\n\x10\x65xplicit_feature\x18\x02 \x01(\x0b\x32\'.qwak.builds.management.ExplicitFeatureH\x00\x12\x45\n\x12on_the_fly_feature\x18\x03 \x01(\x0b\x32\'.qwak.builds.management.OnTheFlyFeatureH\x00\x12\x45\n\x11streaming_feature\x18\x04 \x01(\x0b\x32(.qwak.builds.management.StreamingFeatureH\x00\x12=\n\rrequest_input\x18\x05 \x01(\x0b\x32$.qwak.builds.management.RequestInputH\x00\x12\\\n\x1dstreaming_aggregation_feature\x18\x06 \x01(\x0b\x32\x33.qwak.builds.management.StreamingAggregationFeatureH\x00\x12\x42\n\x10\x62\x61tch_feature_v1\x18\x07 \x01(\x0b\x32&.qwak.builds.management.BatchFeatureV1H\x00\x12J\n\x14streaming_feature_v1\x18\x08 \x01(\x0b\x32*.qwak.builds.management.StreamingFeatureV1H\x00\x42\x06\n\x04type\"\x8f\x01\n\x0fOnTheFlyFeature\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\x12>\n\x0fsource_features\x18\x03 \x03(\x0b\x32%.qwak.builds.management.SourceFeature\"N\n\x0e\x42\x61tchFeatureV1\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"R\n\x12StreamingFeatureV1\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"L\n\x0c\x42\x61tchFeature\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"P\n\x10StreamingFeature\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"[\n\x1bStreamingAggregationFeature\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"P\n\x0f\x45xplicitFeature\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"M\n\x0cRequestInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"\x9b\x01\n\rSourceFeature\x12\x43\n\x10\x65xplicit_feature\x18\x01 \x01(\x0b\x32\'.qwak.builds.management.ExplicitFeatureH\x00\x12=\n\rrequest_input\x18\x02 \x01(\x0b\x32$.qwak.builds.management.RequestInputH\x00\x42\x06\n\x04type\"K\n\nPrediction\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"P\n\x0fInferenceOutput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"\xa6\x01\n\tValueType\x12\x35\n\x04type\x18\x01 \x01(\x0e\x32\'.qwak.builds.management.ValueType.Types\"b\n\x05Types\x12\x0b\n\x07INVALID\x10\x00\x12\t\n\x05\x42YTES\x10\x01\x12\n\n\x06STRING\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\n\n\x06\x44OUBLE\x10\x05\x12\t\n\x05\x46LOAT\x10\x06\x12\x08\n\x04\x42OOL\x10\x07\"j\n\x11ParameterCategory\"U\n\x08\x43\x61tegory\x12\x0b\n\x07INVALID\x10\x00\x12\n\n\x06\x45NTITY\x10\x01\x12\x0b\n\x07\x46\x45\x41TURE\x10\x02\x12\x0e\n\nPREDICTION\x10\x03\x12\x13\n\x0fINFERENCEOUTPUT\x10\x04\"\xae\x01\n\x14RegisterBuildRequest\x12\x35\n\nbuild_spec\x18\x01 \x01(\x0b\x32!.qwak.builds.management.BuildSpec\x12=\n\x0cmodel_schema\x18\x02 \x01(\x0b\x32#.qwak.builds.management.ModelSchemaB\x02\x18\x01\x12 \n\x14qwak_calling_user_id\x18\x03 \x01(\tB\x02\x18\x01\"i\n\x1aRegisterModelSchemaRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x39\n\x0cmodel_schema\x18\x02 \x01(\x0b\x32#.qwak.builds.management.ModelSchema\"\x91\x01\n\'RegisterExperimentTrackingValuesRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12T\n\x1a\x65xperiment_tracking_values\x18\x02 \x01(\x0b\x32\x30.qwak.builds.management.ExperimentTrackingValues\"*\n(RegisterExperimentTrackingValuesResponse\"z\n\x18\x45xperimentTrackingValues\x12/\n\x07metrics\x18\x01 \x03(\x0b\x32\x1e.qwak.builds.management.Metric\x12-\n\x06params\x18\x02 \x03(\x0b\x32\x1d.qwak.builds.management.Param\"\xd1\x02\n\x12\x42uildConfiguration\x12\x46\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32,.qwak.builds.management.BuildPropertiesProto\x12;\n\tbuild_env\x18\x02 \x01(\x0b\x32(.qwak.builds.management.BuildEnvironment\x12;\n\tpre_build\x18\x03 \x01(\x0b\x32(.qwak.builds.management.BuildEnvironment\x12<\n\npost_build\x18\x04 \x01(\x0b\x32(.qwak.builds.management.BuildEnvironment\x12*\n\x04step\x18\x05 \x01(\x0b\x32\x1c.qwak.builds.management.Step\x12\x0f\n\x07verbose\x18\x06 \x01(\x05\"_\n\x04Step\x12\r\n\x05tests\x18\x01 \x01(\x08\x12\x1f\n\x17validate_build_artifact\x18\x02 \x01(\x08\x12\'\n\x1fvalidate_build_artifact_timeout\x18\x03 \x01(\x05\"\xc4\x01\n\x14\x42uildPropertiesProto\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x38\n\tmodel_uri\x18\x02 \x01(\x0b\x32%.qwak.builds.management.BuildModelUri\x12\x0c\n\x04tags\x18\x03 \x03(\t\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x05 \x01(\t\x12\x18\n\x10\x65nvironment_name\x18\x06 \x01(\t\x12\x16\n\x0egpu_compatible\x18\x07 \x01(\x08\"B\n\rBuildModelUri\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x10\n\x08main_dir\x18\x03 \x01(\t\"\xe8\x01\n\x10\x42uildEnvironment\x12\x33\n\x06\x64ocker\x18\x01 \x01(\x0b\x32#.qwak.builds.management.DockerBuild\x12\x31\n\x05local\x18\x02 \x01(\x0b\x32\".qwak.builds.management.LocalBuild\x12\x37\n\npython_env\x18\x03 \x01(\x0b\x32#.qwak.builds.management.PythonBuild\x12\x33\n\x06remote\x18\x04 \x01(\x0b\x32#.qwak.builds.management.RemoteBuild\"\x8a\x02\n\x0b\x44ockerBuild\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x46\n\nbuild_args\x18\x02 \x03(\x0b\x32\x32.qwak.builds.management.DockerBuild.BuildArgsEntry\x12\x10\n\x08\x65nv_vars\x18\x03 \x03(\t\x12\x10\n\x08no_cache\x18\x04 \x01(\x08\x12\x0e\n\x06params\x18\x05 \x03(\t\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x06 \x01(\t\x12\r\n\x05\x63\x61\x63he\x18\x07 \x01(\x08\x12\x0c\n\x04push\x18\x08 \x01(\x08\x1a\x30\n\x0e\x42uildArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"2\n\nLocalBuild\x12\x13\n\x0b\x61ws_profile\x18\x01 \x01(\t\x12\x0f\n\x07no_push\x18\x02 \x01(\x08\"\x9b\x02\n\x0bPythonBuild\x12 \n\x18qwak_sdk_extra_index_url\x18\x01 \x01(\t\x12\x43\n\nvirtualenv\x18\x02 \x01(\x0b\x32/.qwak.builds.management.VirtualEnvironmentBuild\x12\x31\n\x05\x63onda\x18\x03 \x01(\x0b\x32\".qwak.builds.management.CondaBuild\x12\x33\n\x06poetry\x18\x04 \x01(\x0b\x32#.qwak.builds.management.PoetryBuild\x12\x1c\n\x14\x64\x65pendency_file_path\x18\x05 \x01(\t\x12\x1f\n\x17use_deprecated_resolver\x18\x06 \x01(\x08\" \n\nCondaBuild\x12\x12\n\nconda_file\x18\x01 \x01(\t\"8\n\x0bPoetryBuild\x12\x16\n\x0epython_version\x18\x01 \x01(\t\x12\x11\n\tlock_file\x18\x02 \x01(\t\"K\n\x17VirtualEnvironmentBuild\x12\x16\n\x0epython_version\x18\x01 \x01(\t\x12\x18\n\x10requirements_txt\x18\x02 \x01(\t\"a\n\x0bRemoteBuild\x12\x11\n\tis_remote\x18\x01 \x01(\x08\x12?\n\tresources\x18\x02 \x01(\x0b\x32,.qwak.builds.management.RemoteBuildResources\"\x8f\x01\n\x14RemoteBuildResources\x12\x0c\n\x04\x63pus\x18\x01 \x01(\x02\x12\x0e\n\x06memory\x18\x02 \x01(\t\x12\x33\n\x08gpu_type\x18\x03 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x04 \x01(\x05\x12\x10\n\x08instance\x18\x05 \x01(\t\"$\n\x06Metric\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02\"#\n\x05Param\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x1d\n\x1bRegisterModelSchemaResponse\"d\n\x15RegisterBuildResponse\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x39\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32#.qwak.builds.management.BuildStatus\"\xa9\x01\n\x18UpdateBuildStatusRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x39\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32#.qwak.builds.management.BuildStatus\x12 \n\x14qwak_calling_user_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x1e\n\x16\x61vailable_environments\x18\x04 \x03(\t\"\x1b\n\x19UpdateBuildStatusResponse\"A\n\x18UpdateBuildBranchRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\t\"\x1b\n\x19UpdateBuildBranchResponse\"#\n\x0fGetBuildRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\"@\n\x10GetBuildResponse\x12,\n\x05\x62uild\x18\x01 \x01(\x0b\x32\x1d.qwak.builds.management.Build\"Q\n\x11ListBuildsRequest\x12\x15\n\tbranch_id\x18\x01 \x01(\tB\x02\x18\x01\x12\x12\n\nmodel_uuid\x18\x02 \x01(\t\x12\x11\n\tbuild_ids\x18\x03 \x03(\t\"C\n\x12ListBuildsResponse\x12-\n\x06\x62uilds\x18\x01 \x03(\x0b\x32\x1d.qwak.builds.management.Build*\xe8\x01\n\x0b\x42uildStatus\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bIN_PROGRESS\x10\x01\x12\x0e\n\nSUCCESSFUL\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x1d\n\x19REMOTE_BUILD_INITIALIZING\x10\x04\x12\x1a\n\x16REMOTE_BUILD_CANCELLED\x10\x05\x12\x1a\n\x16REMOTE_BUILD_TIMED_OUT\x10\x06\x12\x18\n\x14REMOTE_BUILD_UNKNOWN\x10\x07\x12\x18\n\x14SYNCING_ENVIRONMENTS\x10\x08\x12\x14\n\x10\x46INISHED_SYNCING\x10\t2\xed\x05\n\x17\x42uildsManagementService\x12l\n\rRegisterBuild\x12,.qwak.builds.management.RegisterBuildRequest\x1a-.qwak.builds.management.RegisterBuildResponse\x12x\n\x11UpdateBuildStatus\x12\x30.qwak.builds.management.UpdateBuildStatusRequest\x1a\x31.qwak.builds.management.UpdateBuildStatusResponse\x12~\n\x13RegisterModelSchema\x12\x32.qwak.builds.management.RegisterModelSchemaRequest\x1a\x33.qwak.builds.management.RegisterModelSchemaResponse\x12\xa5\x01\n RegisterExperimentTrackingValues\x12?.qwak.builds.management.RegisterExperimentTrackingValuesRequest\x1a@.qwak.builds.management.RegisterExperimentTrackingValuesResponse\x12]\n\x08GetBuild\x12\'.qwak.builds.management.GetBuildRequest\x1a(.qwak.builds.management.GetBuildResponse\x12\x63\n\nListBuilds\x12).qwak.builds.management.ListBuildsRequest\x1a*.qwak.builds.management.ListBuildsResponseB%\n!com.qwak.ai.management.builds.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18qwak/builds/builds.proto\x12\x16qwak.builds.management\x1a\x1fgoogle/protobuf/timestamp.proto\x1a qwak/deployment/deployment.proto\x1a\x17qwak/builds/build.proto\x1a!qwak/fitness_service/status.proto\"\xf4\x05\n\x05\x42uild\x12\x35\n\nbuild_spec\x18\x01 \x01(\x0b\x32!.qwak.builds.management.BuildSpec\x12\x39\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32#.qwak.builds.management.BuildStatus\x12\x39\n\x0cmodel_schema\x18\x03 \x01(\x0b\x32#.qwak.builds.management.ModelSchema\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x05 \x01(\t\x12\x34\n\x10last_modified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x07 \x01(\t\x12V\n\x17\x64\x65ployment_build_status\x18\x08 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatusB\x02\x18\x01\x12V\n\x14hosting_service_type\x18\t \x01(\x0e\x32\x38.qwak.deployment.management.DeploymentHostingServiceType\x12,\n\x08\x65nd_date\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16\x61vailable_environments\x18\x0b \x03(\t\x12\x1d\n\x15\x64\x65ployed_environments\x18\x0c \x03(\t\x12\x32\n\tpodStatus\x18\r \x01(\x0b\x32\x1f.qwak.fitness.service.PodStatus\x12\x16\n\x0eimage_name_tag\x18\x0e \x01(\t\x12\x41\n\x0f\x62uild_initiator\x18\x0f \x01(\x0b\x32(.qwak.builds.orchestrator.BuildInitiator\"\x86\x03\n\tBuildSpec\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x11\n\tcommit_id\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\t\x12\x11\n\tbranch_id\x18\x08 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x03(\t\x12T\n\x1a\x65xperiment_tracking_values\x18\x06 \x01(\x0b\x32\x30.qwak.builds.management.ExperimentTrackingValues\x12G\n\x13\x62uild_configuration\x18\x07 \x01(\x0b\x32*.qwak.builds.management.BuildConfiguration\x12\x17\n\x0f\x62uild_code_path\x18\t \x01(\t\x12\x13\n\x0b\x62uild_steps\x18\n \x03(\t\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x12\n\nmodel_uuid\x18\x0c \x01(\t\x12\x13\n\x0bsdk_version\x18\r \x01(\t\"\xee\x01\n\x0bModelSchema\x12\x30\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x31\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32\x1f.qwak.builds.management.Feature\x12\x37\n\x0bpredictions\x18\x03 \x03(\x0b\x32\".qwak.builds.management.Prediction\x12\x41\n\x10inference_output\x18\x04 \x03(\x0b\x32\'.qwak.builds.management.InferenceOutput\"G\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"\xd0\x04\n\x07\x46\x65\x61ture\x12=\n\rbatch_feature\x18\x01 \x01(\x0b\x32$.qwak.builds.management.BatchFeatureH\x00\x12\x43\n\x10\x65xplicit_feature\x18\x02 \x01(\x0b\x32\'.qwak.builds.management.ExplicitFeatureH\x00\x12\x45\n\x12on_the_fly_feature\x18\x03 \x01(\x0b\x32\'.qwak.builds.management.OnTheFlyFeatureH\x00\x12\x45\n\x11streaming_feature\x18\x04 \x01(\x0b\x32(.qwak.builds.management.StreamingFeatureH\x00\x12=\n\rrequest_input\x18\x05 \x01(\x0b\x32$.qwak.builds.management.RequestInputH\x00\x12\\\n\x1dstreaming_aggregation_feature\x18\x06 \x01(\x0b\x32\x33.qwak.builds.management.StreamingAggregationFeatureH\x00\x12\x42\n\x10\x62\x61tch_feature_v1\x18\x07 \x01(\x0b\x32&.qwak.builds.management.BatchFeatureV1H\x00\x12J\n\x14streaming_feature_v1\x18\x08 \x01(\x0b\x32*.qwak.builds.management.StreamingFeatureV1H\x00\x42\x06\n\x04type\"\x8f\x01\n\x0fOnTheFlyFeature\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\x12>\n\x0fsource_features\x18\x03 \x03(\x0b\x32%.qwak.builds.management.SourceFeature\"N\n\x0e\x42\x61tchFeatureV1\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"R\n\x12StreamingFeatureV1\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"L\n\x0c\x42\x61tchFeature\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"P\n\x10StreamingFeature\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"[\n\x1bStreamingAggregationFeature\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1e.qwak.builds.management.Entity\x12\x0c\n\x04name\x18\x02 \x01(\t\"P\n\x0f\x45xplicitFeature\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"M\n\x0cRequestInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"\x9b\x01\n\rSourceFeature\x12\x43\n\x10\x65xplicit_feature\x18\x01 \x01(\x0b\x32\'.qwak.builds.management.ExplicitFeatureH\x00\x12=\n\rrequest_input\x18\x02 \x01(\x0b\x32$.qwak.builds.management.RequestInputH\x00\x42\x06\n\x04type\"K\n\nPrediction\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"P\n\x0fInferenceOutput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0b\x32!.qwak.builds.management.ValueType\"\xa6\x01\n\tValueType\x12\x35\n\x04type\x18\x01 \x01(\x0e\x32\'.qwak.builds.management.ValueType.Types\"b\n\x05Types\x12\x0b\n\x07INVALID\x10\x00\x12\t\n\x05\x42YTES\x10\x01\x12\n\n\x06STRING\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\n\n\x06\x44OUBLE\x10\x05\x12\t\n\x05\x46LOAT\x10\x06\x12\x08\n\x04\x42OOL\x10\x07\"j\n\x11ParameterCategory\"U\n\x08\x43\x61tegory\x12\x0b\n\x07INVALID\x10\x00\x12\n\n\x06\x45NTITY\x10\x01\x12\x0b\n\x07\x46\x45\x41TURE\x10\x02\x12\x0e\n\nPREDICTION\x10\x03\x12\x13\n\x0fINFERENCEOUTPUT\x10\x04\"\xae\x01\n\x14RegisterBuildRequest\x12\x35\n\nbuild_spec\x18\x01 \x01(\x0b\x32!.qwak.builds.management.BuildSpec\x12=\n\x0cmodel_schema\x18\x02 \x01(\x0b\x32#.qwak.builds.management.ModelSchemaB\x02\x18\x01\x12 \n\x14qwak_calling_user_id\x18\x03 \x01(\tB\x02\x18\x01\"i\n\x1aRegisterModelSchemaRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x39\n\x0cmodel_schema\x18\x02 \x01(\x0b\x32#.qwak.builds.management.ModelSchema\"\x91\x01\n\'RegisterExperimentTrackingValuesRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12T\n\x1a\x65xperiment_tracking_values\x18\x02 \x01(\x0b\x32\x30.qwak.builds.management.ExperimentTrackingValues\"*\n(RegisterExperimentTrackingValuesResponse\"z\n\x18\x45xperimentTrackingValues\x12/\n\x07metrics\x18\x01 \x03(\x0b\x32\x1e.qwak.builds.management.Metric\x12-\n\x06params\x18\x02 \x03(\x0b\x32\x1d.qwak.builds.management.Param\"\xd1\x02\n\x12\x42uildConfiguration\x12\x46\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32,.qwak.builds.management.BuildPropertiesProto\x12;\n\tbuild_env\x18\x02 \x01(\x0b\x32(.qwak.builds.management.BuildEnvironment\x12;\n\tpre_build\x18\x03 \x01(\x0b\x32(.qwak.builds.management.BuildEnvironment\x12<\n\npost_build\x18\x04 \x01(\x0b\x32(.qwak.builds.management.BuildEnvironment\x12*\n\x04step\x18\x05 \x01(\x0b\x32\x1c.qwak.builds.management.Step\x12\x0f\n\x07verbose\x18\x06 \x01(\x05\"_\n\x04Step\x12\r\n\x05tests\x18\x01 \x01(\x08\x12\x1f\n\x17validate_build_artifact\x18\x02 \x01(\x08\x12\'\n\x1fvalidate_build_artifact_timeout\x18\x03 \x01(\x05\"\xc4\x01\n\x14\x42uildPropertiesProto\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x38\n\tmodel_uri\x18\x02 \x01(\x0b\x32%.qwak.builds.management.BuildModelUri\x12\x0c\n\x04tags\x18\x03 \x03(\t\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x05 \x01(\t\x12\x18\n\x10\x65nvironment_name\x18\x06 \x01(\t\x12\x16\n\x0egpu_compatible\x18\x07 \x01(\x08\"g\n\rBuildModelUri\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x10\n\x08main_dir\x18\x03 \x01(\t\x12#\n\x1b\x64\x65pendency_required_folders\x18\x04 \x03(\t\"\xe8\x01\n\x10\x42uildEnvironment\x12\x33\n\x06\x64ocker\x18\x01 \x01(\x0b\x32#.qwak.builds.management.DockerBuild\x12\x31\n\x05local\x18\x02 \x01(\x0b\x32\".qwak.builds.management.LocalBuild\x12\x37\n\npython_env\x18\x03 \x01(\x0b\x32#.qwak.builds.management.PythonBuild\x12\x33\n\x06remote\x18\x04 \x01(\x0b\x32#.qwak.builds.management.RemoteBuild\"\x8a\x02\n\x0b\x44ockerBuild\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x46\n\nbuild_args\x18\x02 \x03(\x0b\x32\x32.qwak.builds.management.DockerBuild.BuildArgsEntry\x12\x10\n\x08\x65nv_vars\x18\x03 \x03(\t\x12\x10\n\x08no_cache\x18\x04 \x01(\x08\x12\x0e\n\x06params\x18\x05 \x03(\t\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x06 \x01(\t\x12\r\n\x05\x63\x61\x63he\x18\x07 \x01(\x08\x12\x0c\n\x04push\x18\x08 \x01(\x08\x1a\x30\n\x0e\x42uildArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"2\n\nLocalBuild\x12\x13\n\x0b\x61ws_profile\x18\x01 \x01(\t\x12\x0f\n\x07no_push\x18\x02 \x01(\x08\"\x9b\x02\n\x0bPythonBuild\x12 \n\x18qwak_sdk_extra_index_url\x18\x01 \x01(\t\x12\x43\n\nvirtualenv\x18\x02 \x01(\x0b\x32/.qwak.builds.management.VirtualEnvironmentBuild\x12\x31\n\x05\x63onda\x18\x03 \x01(\x0b\x32\".qwak.builds.management.CondaBuild\x12\x33\n\x06poetry\x18\x04 \x01(\x0b\x32#.qwak.builds.management.PoetryBuild\x12\x1c\n\x14\x64\x65pendency_file_path\x18\x05 \x01(\t\x12\x1f\n\x17use_deprecated_resolver\x18\x06 \x01(\x08\" \n\nCondaBuild\x12\x12\n\nconda_file\x18\x01 \x01(\t\"8\n\x0bPoetryBuild\x12\x16\n\x0epython_version\x18\x01 \x01(\t\x12\x11\n\tlock_file\x18\x02 \x01(\t\"K\n\x17VirtualEnvironmentBuild\x12\x16\n\x0epython_version\x18\x01 \x01(\t\x12\x18\n\x10requirements_txt\x18\x02 \x01(\t\"a\n\x0bRemoteBuild\x12\x11\n\tis_remote\x18\x01 \x01(\x08\x12?\n\tresources\x18\x02 \x01(\x0b\x32,.qwak.builds.management.RemoteBuildResources\"\x8f\x01\n\x14RemoteBuildResources\x12\x0c\n\x04\x63pus\x18\x01 \x01(\x02\x12\x0e\n\x06memory\x18\x02 \x01(\t\x12\x33\n\x08gpu_type\x18\x03 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x04 \x01(\x05\x12\x10\n\x08instance\x18\x05 \x01(\t\"$\n\x06Metric\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02\"#\n\x05Param\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x1d\n\x1bRegisterModelSchemaResponse\"d\n\x15RegisterBuildResponse\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x39\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32#.qwak.builds.management.BuildStatus\"\xa9\x01\n\x18UpdateBuildStatusRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x39\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32#.qwak.builds.management.BuildStatus\x12 \n\x14qwak_calling_user_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x1e\n\x16\x61vailable_environments\x18\x04 \x03(\t\"\x1b\n\x19UpdateBuildStatusResponse\"A\n\x18UpdateBuildBranchRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\t\"\x1b\n\x19UpdateBuildBranchResponse\"#\n\x0fGetBuildRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\"@\n\x10GetBuildResponse\x12,\n\x05\x62uild\x18\x01 \x01(\x0b\x32\x1d.qwak.builds.management.Build\"Q\n\x11ListBuildsRequest\x12\x15\n\tbranch_id\x18\x01 \x01(\tB\x02\x18\x01\x12\x12\n\nmodel_uuid\x18\x02 \x01(\t\x12\x11\n\tbuild_ids\x18\x03 \x03(\t\"C\n\x12ListBuildsResponse\x12-\n\x06\x62uilds\x18\x01 \x03(\x0b\x32\x1d.qwak.builds.management.Build*\xe8\x01\n\x0b\x42uildStatus\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bIN_PROGRESS\x10\x01\x12\x0e\n\nSUCCESSFUL\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x1d\n\x19REMOTE_BUILD_INITIALIZING\x10\x04\x12\x1a\n\x16REMOTE_BUILD_CANCELLED\x10\x05\x12\x1a\n\x16REMOTE_BUILD_TIMED_OUT\x10\x06\x12\x18\n\x14REMOTE_BUILD_UNKNOWN\x10\x07\x12\x18\n\x14SYNCING_ENVIRONMENTS\x10\x08\x12\x14\n\x10\x46INISHED_SYNCING\x10\t2\xed\x05\n\x17\x42uildsManagementService\x12l\n\rRegisterBuild\x12,.qwak.builds.management.RegisterBuildRequest\x1a-.qwak.builds.management.RegisterBuildResponse\x12x\n\x11UpdateBuildStatus\x12\x30.qwak.builds.management.UpdateBuildStatusRequest\x1a\x31.qwak.builds.management.UpdateBuildStatusResponse\x12~\n\x13RegisterModelSchema\x12\x32.qwak.builds.management.RegisterModelSchemaRequest\x1a\x33.qwak.builds.management.RegisterModelSchemaResponse\x12\xa5\x01\n RegisterExperimentTrackingValues\x12?.qwak.builds.management.RegisterExperimentTrackingValuesRequest\x1a@.qwak.builds.management.RegisterExperimentTrackingValuesResponse\x12]\n\x08GetBuild\x12\'.qwak.builds.management.GetBuildRequest\x1a(.qwak.builds.management.GetBuildResponse\x12\x63\n\nListBuilds\x12).qwak.builds.management.ListBuildsRequest\x1a*.qwak.builds.management.ListBuildsResponseB%\n!com.qwak.ai.management.builds.apiP\x01\x62\x06proto3')
 
 _BUILDSTATUS = DESCRIPTOR.enum_types_by_name['BuildStatus']
 BuildStatus = enum_type_wrapper.EnumTypeWrapper(_BUILDSTATUS)
 INVALID = 0
 IN_PROGRESS = 1
 SUCCESSFUL = 2
 FAILED = 3
@@ -443,16 +443,16 @@
   _REGISTERBUILDREQUEST.fields_by_name['qwak_calling_user_id']._serialized_options = b'\030\001'
   _DOCKERBUILD_BUILDARGSENTRY._options = None
   _DOCKERBUILD_BUILDARGSENTRY._serialized_options = b'8\001'
   _UPDATEBUILDSTATUSREQUEST.fields_by_name['qwak_calling_user_id']._options = None
   _UPDATEBUILDSTATUSREQUEST.fields_by_name['qwak_calling_user_id']._serialized_options = b'\030\001'
   _LISTBUILDSREQUEST.fields_by_name['branch_id']._options = None
   _LISTBUILDSREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
-  _BUILDSTATUS._serialized_start=6879
-  _BUILDSTATUS._serialized_end=7111
+  _BUILDSTATUS._serialized_start=6916
+  _BUILDSTATUS._serialized_end=7148
   _BUILD._serialized_start=180
   _BUILD._serialized_end=936
   _BUILDSPEC._serialized_start=939
   _BUILDSPEC._serialized_end=1329
   _MODELSCHEMA._serialized_start=1332
   _MODELSCHEMA._serialized_end=1570
   _ENTITY._serialized_start=1572
@@ -502,55 +502,55 @@
   _BUILDCONFIGURATION._serialized_start=4159
   _BUILDCONFIGURATION._serialized_end=4496
   _STEP._serialized_start=4498
   _STEP._serialized_end=4593
   _BUILDPROPERTIESPROTO._serialized_start=4596
   _BUILDPROPERTIESPROTO._serialized_end=4792
   _BUILDMODELURI._serialized_start=4794
-  _BUILDMODELURI._serialized_end=4860
-  _BUILDENVIRONMENT._serialized_start=4863
-  _BUILDENVIRONMENT._serialized_end=5095
-  _DOCKERBUILD._serialized_start=5098
-  _DOCKERBUILD._serialized_end=5364
-  _DOCKERBUILD_BUILDARGSENTRY._serialized_start=5316
-  _DOCKERBUILD_BUILDARGSENTRY._serialized_end=5364
-  _LOCALBUILD._serialized_start=5366
-  _LOCALBUILD._serialized_end=5416
-  _PYTHONBUILD._serialized_start=5419
-  _PYTHONBUILD._serialized_end=5702
-  _CONDABUILD._serialized_start=5704
-  _CONDABUILD._serialized_end=5736
-  _POETRYBUILD._serialized_start=5738
-  _POETRYBUILD._serialized_end=5794
-  _VIRTUALENVIRONMENTBUILD._serialized_start=5796
-  _VIRTUALENVIRONMENTBUILD._serialized_end=5871
-  _REMOTEBUILD._serialized_start=5873
-  _REMOTEBUILD._serialized_end=5970
-  _REMOTEBUILDRESOURCES._serialized_start=5973
-  _REMOTEBUILDRESOURCES._serialized_end=6116
-  _METRIC._serialized_start=6118
-  _METRIC._serialized_end=6154
-  _PARAM._serialized_start=6156
-  _PARAM._serialized_end=6191
-  _REGISTERMODELSCHEMARESPONSE._serialized_start=6193
-  _REGISTERMODELSCHEMARESPONSE._serialized_end=6222
-  _REGISTERBUILDRESPONSE._serialized_start=6224
-  _REGISTERBUILDRESPONSE._serialized_end=6324
-  _UPDATEBUILDSTATUSREQUEST._serialized_start=6327
-  _UPDATEBUILDSTATUSREQUEST._serialized_end=6496
-  _UPDATEBUILDSTATUSRESPONSE._serialized_start=6498
-  _UPDATEBUILDSTATUSRESPONSE._serialized_end=6525
-  _UPDATEBUILDBRANCHREQUEST._serialized_start=6527
-  _UPDATEBUILDBRANCHREQUEST._serialized_end=6592
-  _UPDATEBUILDBRANCHRESPONSE._serialized_start=6594
-  _UPDATEBUILDBRANCHRESPONSE._serialized_end=6621
-  _GETBUILDREQUEST._serialized_start=6623
-  _GETBUILDREQUEST._serialized_end=6658
-  _GETBUILDRESPONSE._serialized_start=6660
-  _GETBUILDRESPONSE._serialized_end=6724
-  _LISTBUILDSREQUEST._serialized_start=6726
-  _LISTBUILDSREQUEST._serialized_end=6807
-  _LISTBUILDSRESPONSE._serialized_start=6809
-  _LISTBUILDSRESPONSE._serialized_end=6876
-  _BUILDSMANAGEMENTSERVICE._serialized_start=7114
-  _BUILDSMANAGEMENTSERVICE._serialized_end=7863
+  _BUILDMODELURI._serialized_end=4897
+  _BUILDENVIRONMENT._serialized_start=4900
+  _BUILDENVIRONMENT._serialized_end=5132
+  _DOCKERBUILD._serialized_start=5135
+  _DOCKERBUILD._serialized_end=5401
+  _DOCKERBUILD_BUILDARGSENTRY._serialized_start=5353
+  _DOCKERBUILD_BUILDARGSENTRY._serialized_end=5401
+  _LOCALBUILD._serialized_start=5403
+  _LOCALBUILD._serialized_end=5453
+  _PYTHONBUILD._serialized_start=5456
+  _PYTHONBUILD._serialized_end=5739
+  _CONDABUILD._serialized_start=5741
+  _CONDABUILD._serialized_end=5773
+  _POETRYBUILD._serialized_start=5775
+  _POETRYBUILD._serialized_end=5831
+  _VIRTUALENVIRONMENTBUILD._serialized_start=5833
+  _VIRTUALENVIRONMENTBUILD._serialized_end=5908
+  _REMOTEBUILD._serialized_start=5910
+  _REMOTEBUILD._serialized_end=6007
+  _REMOTEBUILDRESOURCES._serialized_start=6010
+  _REMOTEBUILDRESOURCES._serialized_end=6153
+  _METRIC._serialized_start=6155
+  _METRIC._serialized_end=6191
+  _PARAM._serialized_start=6193
+  _PARAM._serialized_end=6228
+  _REGISTERMODELSCHEMARESPONSE._serialized_start=6230
+  _REGISTERMODELSCHEMARESPONSE._serialized_end=6259
+  _REGISTERBUILDRESPONSE._serialized_start=6261
+  _REGISTERBUILDRESPONSE._serialized_end=6361
+  _UPDATEBUILDSTATUSREQUEST._serialized_start=6364
+  _UPDATEBUILDSTATUSREQUEST._serialized_end=6533
+  _UPDATEBUILDSTATUSRESPONSE._serialized_start=6535
+  _UPDATEBUILDSTATUSRESPONSE._serialized_end=6562
+  _UPDATEBUILDBRANCHREQUEST._serialized_start=6564
+  _UPDATEBUILDBRANCHREQUEST._serialized_end=6629
+  _UPDATEBUILDBRANCHRESPONSE._serialized_start=6631
+  _UPDATEBUILDBRANCHRESPONSE._serialized_end=6658
+  _GETBUILDREQUEST._serialized_start=6660
+  _GETBUILDREQUEST._serialized_end=6695
+  _GETBUILDRESPONSE._serialized_start=6697
+  _GETBUILDRESPONSE._serialized_end=6761
+  _LISTBUILDSREQUEST._serialized_start=6763
+  _LISTBUILDSREQUEST._serialized_end=6844
+  _LISTBUILDSRESPONSE._serialized_start=6846
+  _LISTBUILDSRESPONSE._serialized_end=6913
+  _BUILDSMANAGEMENTSERVICE._serialized_start=7151
+  _BUILDSMANAGEMENTSERVICE._serialized_end=7900
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -821,25 +821,29 @@
 
 class BuildModelUri(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     URI_FIELD_NUMBER: builtins.int
     GIT_BRANCH_FIELD_NUMBER: builtins.int
     MAIN_DIR_FIELD_NUMBER: builtins.int
+    DEPENDENCY_REQUIRED_FOLDERS_FIELD_NUMBER: builtins.int
     uri: builtins.str
     git_branch: builtins.str
     main_dir: builtins.str
+    @property
+    def dependency_required_folders(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
         uri: builtins.str = ...,
         git_branch: builtins.str = ...,
         main_dir: builtins.str = ...,
+        dependency_required_folders: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["git_branch", b"git_branch", "main_dir", b"main_dir", "uri", b"uri"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dependency_required_folders", b"dependency_required_folders", "git_branch", b"git_branch", "main_dir", b"main_dir", "uri", b"uri"]) -> None: ...
 
 global___BuildModelUri = BuildModelUri
 
 class BuildEnvironment(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DOCKER_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from _qwak_proto.qwak.audience.v1 import audience_pb2 as qwak_dot_audience_dot_v1_dot_audience__pb2
 from _qwak_proto.qwak.auto_scaling.v1 import auto_scaling_pb2 as qwak_dot_auto__scaling_dot_v1_dot_auto__scaling__pb2
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n qwak/deployment/deployment.proto\x12\x1aqwak.deployment.management\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fqwak/audience/v1/audience.proto\x1a\'qwak/auto_scaling/v1/auto_scaling.proto\x1a/qwak/user_application/common/v0/resources.proto\"\x9e\x01\n\x0eHostingService\x12>\n\tsagemaker\x18\x01 \x01(\x0b\x32%.qwak.deployment.management.SageMakerB\x02\x18\x01H\x00\x12\x45\n\x0fkube_deployment\x18\x02 \x01(\x0b\x32*.qwak.deployment.management.KubeDeploymentH\x00\x42\x05\n\x03val\"\xff\x03\n\x0eKubeDeployment\x12\x15\n\tpod_count\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x43\n\x0f\x64\x65ployment_size\x18\x05 \x01(\x0b\x32*.qwak.deployment.management.DeploymentSize\x12Z\n\x1b\x61\x64vanced_deployment_options\x18\x06 \x01(\x0b\x32\x35.qwak.deployment.management.AdvancedDeploymentOptions\x12L\n\x14kube_deployment_type\x18\x07 \x01(\x0e\x32..qwak.deployment.management.KubeDeploymentType\x12\x45\n\x10serving_strategy\x18\t \x01(\x0b\x32+.qwak.deployment.management.ServingStrategy\x12\x63\n\x15\x65nvironment_variables\x18\n \x03(\x0b\x32\x44.qwak.deployment.management.KubeDeployment.EnvironmentVariablesEntry\x1a;\n\x19\x45nvironmentVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe8\x01\n\x0fServingStrategy\x12\x45\n\x0frealtime_config\x18\x01 \x01(\x0b\x32*.qwak.deployment.management.RealTimeConfigH\x00\x12\x41\n\rstream_config\x18\x02 \x01(\x0b\x32(.qwak.deployment.management.StreamConfigH\x00\x12?\n\x0c\x62\x61tch_config\x18\x03 \x01(\x0b\x32\'.qwak.deployment.management.BatchConfigH\x00\x42\n\n\x08Strategy\"\x99\x01\n\x0eRealTimeConfig\x12\x41\n\x0etraffic_config\x18\x01 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\x12\x44\n\x13\x61uto_scaling_config\x18\x02 \x01(\x0b\x32\'.qwak.auto_scaling.v1.AutoScalingConfig\"\xfd\x01\n\rTrafficConfig\x12\x1f\n\x17selected_variation_name\x18\x01 \x01(\t\x12=\n\nvariations\x18\x02 \x03(\x0b\x32%.qwak.deployment.management.VariationB\x02\x18\x01\x12\x46\n\x17\x61udience_routes_entries\x18\x03 \x03(\x0b\x32%.qwak.audience.v1.AudienceRoutesEntry\x12\x1a\n\x12\x66\x61llback_variation\x18\x04 \x01(\t\x12(\n selected_variation_protect_state\x18\x05 \x01(\x08\"F\n\x0cStreamConfig\x12\x36\n\x05kafka\x18\x01 \x01(\x0b\x32\'.qwak.deployment.management.KafkaConfig\"\r\n\x0b\x42\x61tchConfig\"\xaf\x05\n\x0bKafkaConfig\x12\x42\n\x08\x63onsumer\x18\x01 \x01(\x0b\x32\x30.qwak.deployment.management.KafkaConfig.Consumer\x12\x42\n\x08producer\x18\x02 \x01(\x0b\x32\x30.qwak.deployment.management.KafkaConfig.Producer\x12\x0f\n\x07workers\x18\x03 \x01(\x05\x1a\x99\x02\n\x08\x43onsumer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x05\x12Y\n\x10\x61uto_offset_type\x18\x05 \x01(\x0e\x32?.qwak.deployment.management.KafkaConfig.Consumer.AutoOffSetType\x12\x16\n\x0emax_batch_size\x18\x06 \x01(\x05\x12\x18\n\x10max_poll_latency\x18\x07 \x01(\x01\"7\n\x0e\x41utoOffSetType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x45\x41RLIEST\x10\x01\x12\n\n\x06LATEST\x10\x02\x1a\xea\x01\n\x08Producer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12Z\n\x10\x63ompression_type\x18\x03 \x01(\x0e\x32@.qwak.deployment.management.KafkaConfig.Producer.CompressionType\"Y\n\x0f\x43ompressionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0cUNCOMPRESSED\x10\x01\x12\x08\n\x04GZIP\x10\x02\x12\n\n\x06SNAPPY\x10\x03\x12\x07\n\x03LZ4\x10\x04\x12\x08\n\x04ZSTD\x10\x05\":\n\tSageMaker\x12\x16\n\x0einstance_count\x18\x04 \x01(\x05\x12\x15\n\rinstance_type\x18\x05 \x01(\t\"\xc2\x02\n\x0e\x44\x65ploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0f\n\x03\x63pu\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x03 \x01(\x05\x42\x02\x18\x01\x12@\n\x0cmemory_units\x18\x04 \x01(\x0e\x32&.qwak.deployment.management.MemoryUnitB\x02\x18\x01\x12H\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesB\x02\x18\x01\x12`\n\x1c\x63lient_pod_compute_resources\x18\x06 \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResources\"Y\n\x0cGpuResources\x12\x35\n\x08gpu_type\x18\x01 \x01(\x0e\x32#.qwak.deployment.management.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x8c\x02\n\x19\x41\x64vancedDeploymentOptions\x12%\n\x1dnumber_of_http_server_workers\x18\x01 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x02 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x04 \x01(\t\x12\x16\n\x0emax_batch_size\x18\x05 \x01(\x05\x12(\n deployment_process_timeout_limit\x18\x06 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x07 \x01(\t\"\x98\t\n\x11\x44\x65ploymentDetails\x12\x31\n\rlast_deployed\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x16\n\x0enumber_of_pods\x18\x03 \x01(\x05\x12\x14\n\x0c\x63pu_fraction\x18\x04 \x01(\x02\x12\x15\n\rmemory_amount\x18\x05 \x01(\x05\x12<\n\x0cmemory_units\x18\x06 \x01(\x0e\x32&.qwak.deployment.management.MemoryUnit\x12\x19\n\x11number_of_workers\x18\x07 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x08 \x01(\x05\x12L\n\x14kube_deployment_type\x18\t \x01(\x0e\x32..qwak.deployment.management.KubeDeploymentType\x12\x45\n\x10serving_strategy\x18\n \x01(\x0b\x32+.qwak.deployment.management.ServingStrategy\x12\x38\n\tvariation\x18\x0b \x01(\x0b\x32%.qwak.deployment.management.Variation\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x0c \x01(\t\x12\x16\n\x0emax_batch_size\x18\r \x01(\x05\x12:\n\x08gpu_type\x18\x0e \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x0f \x01(\x05\x12\x16\n\x0e\x65nvironment_id\x18\x10 \x01(\t\x12\x1a\n\x12\x61vailable_replicas\x18\x11 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12(\n deployment_process_timeout_limit\x18\x13 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x14 \x01(\t\x12\x66\n\x15\x65nvironment_variables\x18\x15 \x03(\x0b\x32G.qwak.deployment.management.DeploymentDetails.EnvironmentVariablesEntry\x12\x35\n\x11undeployment_time\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x06status\x18\x17 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x15\n\rdeployment_id\x18\x18 \x01(\t\x12M\n\x0f\x66\x61ilure_details\x18\x19 \x01(\x0b\x32\x34.qwak.deployment.management.DeploymentFailureDetails\x1a;\n\x19\x45nvironmentVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"3\n\x18\x44\x65ploymentFailureDetails\x12\x17\n\x0f\x66\x61ilure_message\x18\x01 \x01(\t\"\xb9\x01\n\x19RuntimeDeploymentSettings\x12Y\n\x11root_logger_level\x18\x01 \x01(\x0e\x32>.qwak.deployment.management.RuntimeDeploymentSettings.LogLevel\"A\n\x08LogLevel\x12\x0b\n\x07NOT_SET\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x08\n\x04WARN\x10\x02\x12\x08\n\x04INFO\x10\x03\x12\t\n\x05\x44\x45\x42UG\x10\x04\"\xee\x02\n\x0f\x44\x65ploymentBrief\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x13\n\x0b\x64\x65ployed_by\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x61ilure_reason_code\x18\x04 \x01(\t\x12\x17\n\x0f\x66\x61ilure_message\x18\x05 \x01(\t\x12\x19\n\x11technical_details\x18\x06 \x01(\t\x12\x38\n\x14\x64\x65ployment_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x65nvironment_id\x18\x08 \x01(\t\x12\x16\n\x0evariation_name\x18\t \x01(\t\x12\x1f\n\x17variation_protect_state\x18\n \x01(\x08\x12\x15\n\rdeployment_id\x18\x0b \x01(\t\"\xd7\x02\n\x1eKubernetesModelDeploymentState\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x41\n\x06status\x18\x03 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x41\n\x0estatus_details\x18\x04 \x01(\x0b\x32).qwak.deployment.management.StatusDetails\x12\x16\n\x0evariation_name\x18\x05 \x01(\t\x12\x15\n\rdeployment_id\x18\x06 \x01(\t\x12\x12\n\nmodel_uuid\x18\x07 \x01(\t\x12\x43\n\nmanaged_by\x18\x08 \x01(\x0e\x32/.qwak.deployment.management.DeploymentManagedBy\"\x9e\x02\n\rStatusDetails\x12R\n\x16pending_status_details\x18\x01 \x01(\x0b\x32\x30.qwak.deployment.management.PendingStatusDetailsH\x00\x12U\n\x16success_status_details\x18\x02 \x01(\x0b\x32\x33.qwak.deployment.management.SuccessfulStatusDetailsH\x00\x12P\n\x15\x66\x61iled_status_details\x18\x03 \x01(\x0b\x32/.qwak.deployment.management.FailedStatusDetailsH\x00\x42\x10\n\x0estatus_details\"\x9c\x01\n\x14PendingStatusDetails\x12\x41\n\x0cold_instance\x18\x01 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\x12\x41\n\x0cnew_instance\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"`\n\x17SuccessfulStatusDetails\x12\x45\n\x10running_instance\x18\x01 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"\xe3\x01\n\x13\x46\x61iledStatusDetails\x12\x43\n\x0f\x66\x61ilure_details\x18\x01 \x01(\x0b\x32*.qwak.deployment.management.FailureDetails\x12\x41\n\x0cold_instance\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\x12\x44\n\x0f\x66\x61iled_instance\x18\x03 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"\x91\x01\n\x0e\x46\x61ilureDetails\x12_\n\x1e\x64\x65ployment_failure_reason_code\x18\x01 \x01(\x0e\x32\x37.qwak.deployment.management.DeploymentFailureReasonCode\x12\x1e\n\x16\x66\x61ilure_reason_details\x18\x02 \x01(\t\"\x8f\x01\n\x0fInstanceDetails\x12\x15\n\rdeployment_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x1a\n\x12\x61vailable_replicas\x18\x03 \x01(\x05\x12\x37\n\x04pods\x18\x04 \x03(\x0e\x32).qwak.deployment.management.ModelPodPhase\"a\n\x17\x44\x65ploymentPhasesDetails\x12\x46\n\x11\x64\x65ployment_phases\x18\x01 \x03(\x0b\x32+.qwak.deployment.management.DeploymentPhase\"\xd7\x02\n\x0f\x44\x65ploymentPhase\x12N\n\x15\x64\x65ployment_phase_type\x18\x01 \x01(\x0e\x32/.qwak.deployment.management.DeploymentPhaseType\x12R\n\x17\x64\x65ployment_phase_status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.DeploymentPhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x03 \x01(\x05\x12.\n\nstarted_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x64isplay_message\x18\x06 \x01(\t\"\x88\x01\n\tVariation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x03 \x01(\t\x12:\n\x07traffic\x18\x02 \x01(\x0b\x32\'.qwak.deployment.management.TrafficSpecH\x00\x12\x11\n\tprotected\x18\x04 \x01(\x08\x42\x06\n\x04spec\"4\n\x0bTrafficSpec\x12\x12\n\npercentage\x18\x01 \x01(\x05\x12\x11\n\tis_shadow\x18\x02 \x01(\x08\"]\n\x18\x46utureDeploymentSettings\x12\x41\n\x0etraffic_config\x18\x01 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\"\xb6\x01\n\x1c\x45nvironmentDeploymentMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x43\n\x0fhosting_service\x18\x04 \x01(\x0b\x32*.qwak.deployment.management.HostingService\x12\x16\n\nmodel_uuid\x18\x05 \x01(\tB\x02\x18\x01\"\x92\x01\n\"EnvironmentDeploymentResultMessage\x12\x1b\n\x13\x64\x65ployment_named_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x0c\n\x04info\x18\x03 \x01(\t\"\x90\x02\n\x1e\x45nvironmentUndeploymentMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12V\n\x14hosting_service_type\x18\x03 \x01(\x0e\x32\x38.qwak.deployment.management.DeploymentHostingServiceType\x12\x41\n\x0etraffic_config\x18\x04 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\x12\x16\n\x0evariation_name\x18\x05 \x01(\t\x12\x12\n\nmodel_uuid\x18\x06 \x01(\t\"w\n$EnvironmentUndeploymentResultMessage\x12\x41\n\x06status\x18\x01 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x0c\n\x04info\x18\x02 \x01(\t\"\xd6\x01\n+EnvironmentRuntimeDeploymentSettingsMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12R\n\x13\x64\x65ployment_settings\x18\x03 \x01(\x0b\x32\x35.qwak.deployment.management.RuntimeDeploymentSettings\x12\x16\n\x0evariation_name\x18\x04 \x01(\t\x12\x12\n\nmodel_uuid\x18\x05 \x01(\t\"G\n1EnvironmentRuntimeDeploymentSettingsResultMessage\x12\x12\n\nerror_info\x18\x01 \x01(\t\"4\n$EnvironmentApplyModelTrafficResponse\x12\x0c\n\x04info\x18\x01 \x01(\t\"\xce\x01\n#EnvironmentDeploymentDetailsMessage\x12J\n\x13\x64\x65ployments_details\x18\x01 \x03(\x0b\x32-.qwak.deployment.management.DeploymentDetails\x12?\n\x10\x61udiences_routes\x18\x02 \x03(\x0b\x32%.qwak.audience.v1.AudienceRoutesEntry\x12\x1a\n\x12\x66\x61llback_variation\x18\x03 \x01(\t\"g\n#EnvironmentDeploymentHistoryMessage\x12@\n\x0b\x64\x65ployments\x18\x01 \x03(\x0b\x32+.qwak.deployment.management.DeploymentBrief\"V\n\x19\x45nvironmentTrafficMessage\x12\x39\n\nvariations\x18\x01 \x03(\x0b\x32%.qwak.deployment.management.Variation\"\x9e\x02\n BuildDeploymentEnvironmentStatus\x12\x87\x01\n\x1f\x65nvironment_to_deployment_brief\x18\x01 \x03(\x0b\x32^.qwak.deployment.management.BuildDeploymentEnvironmentStatus.EnvironmentToDeploymentBriefEntry\x1ap\n!EnvironmentToDeploymentBriefEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.DeploymentBrief:\x02\x38\x01\"S\n\x15\x42uildDeploymentStatus\x12\x12\n\nbuild_uuid\x18\x01 \x01(\t\x12\x13\n\x0bis_deployed\x18\x02 \x01(\x08\x12\x11\n\tis_in_use\x18\x03 \x01(\x08\"]\n\x1d\x43\x61ncelDeploymentRequestStatus\x12%\n\x1d\x63\x61ncel_requested_successfully\x18\x01 \x01(\x08\x12\x15\n\rerror_message\x18\x02 \x01(\t*\x85\x03\n\x15ModelDeploymentStatus\x12\x16\n\x12INVALID_DEPLOYMENT\x10\x00\x12\x19\n\x15INITIATING_DEPLOYMENT\x10\x01\x12 \n\x1c\x46\x41ILED_INITIATING_DEPLOYMENT\x10\x08\x12\x16\n\x12PENDING_DEPLOYMENT\x10\x02\x12\x19\n\x15SUCCESSFUL_DEPLOYMENT\x10\x03\x12\x15\n\x11\x46\x41ILED_DEPLOYMENT\x10\x04\x12\x1b\n\x17INITIATING_UNDEPLOYMENT\x10\t\x12\x18\n\x14PENDING_UNDEPLOYMENT\x10\n\x12\x1b\n\x17SUCCESSFUL_UNDEPLOYMENT\x10\x05\x12\x17\n\x13\x46\x41ILED_UNDEPLOYMENT\x10\x06\x12\t\n\x05UNSET\x10\x07\x12\x19\n\x15\x41LL_BUILDS_UNDEPLOYED\x10\x0b\x12\x18\n\x14\x43\x41NCELLED_DEPLOYMENT\x10\x0c\x12 \n\x1cINITIATING_CANCEL_DEPLOYMENT\x10\r*O\n\x1c\x44\x65ploymentHostingServiceType\x12\x0b\n\x07INVALID\x10\x00\x12\r\n\tSAGEMAKER\x10\x01\x12\x13\n\x0fKUBE_DEPLOYMENT\x10\x02*F\n\x12KubeDeploymentType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06ONLINE\x10\x01\x12\n\n\x06STREAM\x10\x02\x12\t\n\x05\x42\x41TCH\x10\x03*{\n\x07GpuType\x12\x0f\n\x0bINVALID_GPU\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06*+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x83\x01\n\x13\x44\x65ploymentManagedBy\x12!\n\x1d\x44\x45PLOYMENT_MANAGED_BY_INVALID\x10\x00\x12&\n\"DEPLOYMENT_MANAGED_BY_KUBE_CAPTAIN\x10\x01\x12!\n\x1d\x44\x45PLOYMENT_MANAGED_BY_ADMIRAL\x10\x02*\x93\x02\n\x1b\x44\x65ploymentFailureReasonCode\x12\x18\n\x14INVALID_FAILURE_CODE\x10\x00\x12\x12\n\x0eUNKNOWN_REASON\x10\x01\x12\x1e\n\x1aNO_REPLICA_SETS_PODS_FOUND\x10\x02\x12\x1d\n\x19MODEL_CONTAINER_NOT_FOUND\x10\x03\x12\x11\n\rUNSCHEDULABLE\x10\x04\x12\x1a\n\x16\x44OCKER_IMAGE_NOT_FOUND\x10\x05\x12\x19\n\x15MEMORY_LIMIT_EXCEEDED\x10\x06\x12\x0e\n\nCRASH_LOOP\x10\x07\x12-\n)CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON\x10\x08*\xb7\x01\n\rModelPodPhase\x12\x15\n\x11INVALID_POD_PHASE\x10\x00\x12)\n%MODEL_POD_PHASE_PROVISIONING_INSTANCE\x10\x01\x12!\n\x1dMODEL_POD_PHASE_PULLING_IMAGE\x10\x02\x12&\n\"MODEL_POD_PHASE_INITIALIZING_MODEL\x10\x03\x12\x19\n\x15MODEL_POD_PHASE_READY\x10\x04*\xac\x01\n\x13\x44\x65ploymentPhaseType\x12\x1c\n\x18INVALID_DEPLOYMENT_PHASE\x10\x00\x12*\n&DEPLOYMENT_PHASE_PROVISIONING_INSTANCE\x10\x01\x12\"\n\x1e\x44\x45PLOYMENT_PHASE_PULLING_IMAGE\x10\x02\x12\'\n#DEPLOYMENT_PHASE_INITIALIZING_MODEL\x10\x03*\xf5\x01\n\x15\x44\x65ploymentPhaseStatus\x12#\n\x1fINVALID_DEPLOYMENT_PHASE_STATUS\x10\x00\x12 \n\x1c\x44\x45PLOYMENT_PHASE_NOT_STARTED\x10\x01\x12\x1c\n\x18\x44\x45PLOYMENT_PHASE_STARTED\x10\x02\x12\x1d\n\x19\x44\x45PLOYMENT_PHASE_FINISHED\x10\x03\x12\x1d\n\x19\x44\x45PLOYMENT_PHASE_CANCELED\x10\x04\x12\x1b\n\x17\x44\x45PLOYMENT_PHASE_FAILED\x10\x05\x12\x1c\n\x18\x44\x45PLOYMENT_PHASE_ABORTED\x10\x06\x42\x45\n%com.qwak.ai.management.deployment.apiP\x01Z\x1aqwak/deployment;deploymentb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n qwak/deployment/deployment.proto\x12\x1aqwak.deployment.management\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fqwak/audience/v1/audience.proto\x1a\'qwak/auto_scaling/v1/auto_scaling.proto\x1a/qwak/user_application/common/v0/resources.proto\"\x9e\x01\n\x0eHostingService\x12>\n\tsagemaker\x18\x01 \x01(\x0b\x32%.qwak.deployment.management.SageMakerB\x02\x18\x01H\x00\x12\x45\n\x0fkube_deployment\x18\x02 \x01(\x0b\x32*.qwak.deployment.management.KubeDeploymentH\x00\x42\x05\n\x03val\"\xff\x03\n\x0eKubeDeployment\x12\x15\n\tpod_count\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x43\n\x0f\x64\x65ployment_size\x18\x05 \x01(\x0b\x32*.qwak.deployment.management.DeploymentSize\x12Z\n\x1b\x61\x64vanced_deployment_options\x18\x06 \x01(\x0b\x32\x35.qwak.deployment.management.AdvancedDeploymentOptions\x12L\n\x14kube_deployment_type\x18\x07 \x01(\x0e\x32..qwak.deployment.management.KubeDeploymentType\x12\x45\n\x10serving_strategy\x18\t \x01(\x0b\x32+.qwak.deployment.management.ServingStrategy\x12\x63\n\x15\x65nvironment_variables\x18\n \x03(\x0b\x32\x44.qwak.deployment.management.KubeDeployment.EnvironmentVariablesEntry\x1a;\n\x19\x45nvironmentVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe8\x01\n\x0fServingStrategy\x12\x45\n\x0frealtime_config\x18\x01 \x01(\x0b\x32*.qwak.deployment.management.RealTimeConfigH\x00\x12\x41\n\rstream_config\x18\x02 \x01(\x0b\x32(.qwak.deployment.management.StreamConfigH\x00\x12?\n\x0c\x62\x61tch_config\x18\x03 \x01(\x0b\x32\'.qwak.deployment.management.BatchConfigH\x00\x42\n\n\x08Strategy\"\x99\x01\n\x0eRealTimeConfig\x12\x41\n\x0etraffic_config\x18\x01 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\x12\x44\n\x13\x61uto_scaling_config\x18\x02 \x01(\x0b\x32\'.qwak.auto_scaling.v1.AutoScalingConfig\"\xfd\x01\n\rTrafficConfig\x12\x1f\n\x17selected_variation_name\x18\x01 \x01(\t\x12=\n\nvariations\x18\x02 \x03(\x0b\x32%.qwak.deployment.management.VariationB\x02\x18\x01\x12\x46\n\x17\x61udience_routes_entries\x18\x03 \x03(\x0b\x32%.qwak.audience.v1.AudienceRoutesEntry\x12\x1a\n\x12\x66\x61llback_variation\x18\x04 \x01(\t\x12(\n selected_variation_protect_state\x18\x05 \x01(\x08\"F\n\x0cStreamConfig\x12\x36\n\x05kafka\x18\x01 \x01(\x0b\x32\'.qwak.deployment.management.KafkaConfig\"\r\n\x0b\x42\x61tchConfig\"\xaf\x05\n\x0bKafkaConfig\x12\x42\n\x08\x63onsumer\x18\x01 \x01(\x0b\x32\x30.qwak.deployment.management.KafkaConfig.Consumer\x12\x42\n\x08producer\x18\x02 \x01(\x0b\x32\x30.qwak.deployment.management.KafkaConfig.Producer\x12\x0f\n\x07workers\x18\x03 \x01(\x05\x1a\x99\x02\n\x08\x43onsumer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x05\x12Y\n\x10\x61uto_offset_type\x18\x05 \x01(\x0e\x32?.qwak.deployment.management.KafkaConfig.Consumer.AutoOffSetType\x12\x16\n\x0emax_batch_size\x18\x06 \x01(\x05\x12\x18\n\x10max_poll_latency\x18\x07 \x01(\x01\"7\n\x0e\x41utoOffSetType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x45\x41RLIEST\x10\x01\x12\n\n\x06LATEST\x10\x02\x1a\xea\x01\n\x08Producer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12Z\n\x10\x63ompression_type\x18\x03 \x01(\x0e\x32@.qwak.deployment.management.KafkaConfig.Producer.CompressionType\"Y\n\x0f\x43ompressionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0cUNCOMPRESSED\x10\x01\x12\x08\n\x04GZIP\x10\x02\x12\n\n\x06SNAPPY\x10\x03\x12\x07\n\x03LZ4\x10\x04\x12\x08\n\x04ZSTD\x10\x05\":\n\tSageMaker\x12\x16\n\x0einstance_count\x18\x04 \x01(\x05\x12\x15\n\rinstance_type\x18\x05 \x01(\t\"\xc2\x02\n\x0e\x44\x65ploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0f\n\x03\x63pu\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x03 \x01(\x05\x42\x02\x18\x01\x12@\n\x0cmemory_units\x18\x04 \x01(\x0e\x32&.qwak.deployment.management.MemoryUnitB\x02\x18\x01\x12H\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesB\x02\x18\x01\x12`\n\x1c\x63lient_pod_compute_resources\x18\x06 \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResources\"Y\n\x0cGpuResources\x12\x35\n\x08gpu_type\x18\x01 \x01(\x0e\x32#.qwak.deployment.management.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\xb5\x02\n\x19\x41\x64vancedDeploymentOptions\x12%\n\x1dnumber_of_http_server_workers\x18\x01 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x02 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x04 \x01(\t\x12\x16\n\x0emax_batch_size\x18\x05 \x01(\x05\x12(\n deployment_process_timeout_limit\x18\x06 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x07 \x01(\t\x12\'\n\x1fservice_account_key_secret_name\x18\x08 \x01(\t\"\xc1\t\n\x11\x44\x65ploymentDetails\x12\x31\n\rlast_deployed\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x16\n\x0enumber_of_pods\x18\x03 \x01(\x05\x12\x14\n\x0c\x63pu_fraction\x18\x04 \x01(\x02\x12\x15\n\rmemory_amount\x18\x05 \x01(\x05\x12<\n\x0cmemory_units\x18\x06 \x01(\x0e\x32&.qwak.deployment.management.MemoryUnit\x12\x19\n\x11number_of_workers\x18\x07 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x08 \x01(\x05\x12L\n\x14kube_deployment_type\x18\t \x01(\x0e\x32..qwak.deployment.management.KubeDeploymentType\x12\x45\n\x10serving_strategy\x18\n \x01(\x0b\x32+.qwak.deployment.management.ServingStrategy\x12\x38\n\tvariation\x18\x0b \x01(\x0b\x32%.qwak.deployment.management.Variation\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x0c \x01(\t\x12\x16\n\x0emax_batch_size\x18\r \x01(\x05\x12:\n\x08gpu_type\x18\x0e \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x0f \x01(\x05\x12\x16\n\x0e\x65nvironment_id\x18\x10 \x01(\t\x12\x1a\n\x12\x61vailable_replicas\x18\x11 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12(\n deployment_process_timeout_limit\x18\x13 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x14 \x01(\t\x12\x66\n\x15\x65nvironment_variables\x18\x15 \x03(\x0b\x32G.qwak.deployment.management.DeploymentDetails.EnvironmentVariablesEntry\x12\x35\n\x11undeployment_time\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x06status\x18\x17 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x15\n\rdeployment_id\x18\x18 \x01(\t\x12M\n\x0f\x66\x61ilure_details\x18\x19 \x01(\x0b\x32\x34.qwak.deployment.management.DeploymentFailureDetails\x12\'\n\x1fservice_account_key_secret_name\x18\x1a \x01(\t\x1a;\n\x19\x45nvironmentVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"3\n\x18\x44\x65ploymentFailureDetails\x12\x17\n\x0f\x66\x61ilure_message\x18\x01 \x01(\t\"\xb9\x01\n\x19RuntimeDeploymentSettings\x12Y\n\x11root_logger_level\x18\x01 \x01(\x0e\x32>.qwak.deployment.management.RuntimeDeploymentSettings.LogLevel\"A\n\x08LogLevel\x12\x0b\n\x07NOT_SET\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x08\n\x04WARN\x10\x02\x12\x08\n\x04INFO\x10\x03\x12\t\n\x05\x44\x45\x42UG\x10\x04\"\xee\x02\n\x0f\x44\x65ploymentBrief\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x13\n\x0b\x64\x65ployed_by\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x61ilure_reason_code\x18\x04 \x01(\t\x12\x17\n\x0f\x66\x61ilure_message\x18\x05 \x01(\t\x12\x19\n\x11technical_details\x18\x06 \x01(\t\x12\x38\n\x14\x64\x65ployment_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x65nvironment_id\x18\x08 \x01(\t\x12\x16\n\x0evariation_name\x18\t \x01(\t\x12\x1f\n\x17variation_protect_state\x18\n \x01(\x08\x12\x15\n\rdeployment_id\x18\x0b \x01(\t\"\xd7\x02\n\x1eKubernetesModelDeploymentState\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x41\n\x06status\x18\x03 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x41\n\x0estatus_details\x18\x04 \x01(\x0b\x32).qwak.deployment.management.StatusDetails\x12\x16\n\x0evariation_name\x18\x05 \x01(\t\x12\x15\n\rdeployment_id\x18\x06 \x01(\t\x12\x12\n\nmodel_uuid\x18\x07 \x01(\t\x12\x43\n\nmanaged_by\x18\x08 \x01(\x0e\x32/.qwak.deployment.management.DeploymentManagedBy\"\x9e\x02\n\rStatusDetails\x12R\n\x16pending_status_details\x18\x01 \x01(\x0b\x32\x30.qwak.deployment.management.PendingStatusDetailsH\x00\x12U\n\x16success_status_details\x18\x02 \x01(\x0b\x32\x33.qwak.deployment.management.SuccessfulStatusDetailsH\x00\x12P\n\x15\x66\x61iled_status_details\x18\x03 \x01(\x0b\x32/.qwak.deployment.management.FailedStatusDetailsH\x00\x42\x10\n\x0estatus_details\"\x9c\x01\n\x14PendingStatusDetails\x12\x41\n\x0cold_instance\x18\x01 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\x12\x41\n\x0cnew_instance\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"`\n\x17SuccessfulStatusDetails\x12\x45\n\x10running_instance\x18\x01 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"\xe3\x01\n\x13\x46\x61iledStatusDetails\x12\x43\n\x0f\x66\x61ilure_details\x18\x01 \x01(\x0b\x32*.qwak.deployment.management.FailureDetails\x12\x41\n\x0cold_instance\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\x12\x44\n\x0f\x66\x61iled_instance\x18\x03 \x01(\x0b\x32+.qwak.deployment.management.InstanceDetails\"\x91\x01\n\x0e\x46\x61ilureDetails\x12_\n\x1e\x64\x65ployment_failure_reason_code\x18\x01 \x01(\x0e\x32\x37.qwak.deployment.management.DeploymentFailureReasonCode\x12\x1e\n\x16\x66\x61ilure_reason_details\x18\x02 \x01(\t\"\x8f\x01\n\x0fInstanceDetails\x12\x15\n\rdeployment_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x1a\n\x12\x61vailable_replicas\x18\x03 \x01(\x05\x12\x37\n\x04pods\x18\x04 \x03(\x0e\x32).qwak.deployment.management.ModelPodPhase\"a\n\x17\x44\x65ploymentPhasesDetails\x12\x46\n\x11\x64\x65ployment_phases\x18\x01 \x03(\x0b\x32+.qwak.deployment.management.DeploymentPhase\"\xd7\x02\n\x0f\x44\x65ploymentPhase\x12N\n\x15\x64\x65ployment_phase_type\x18\x01 \x01(\x0e\x32/.qwak.deployment.management.DeploymentPhaseType\x12R\n\x17\x64\x65ployment_phase_status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.DeploymentPhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x03 \x01(\x05\x12.\n\nstarted_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x64isplay_message\x18\x06 \x01(\t\"\x88\x01\n\tVariation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x03 \x01(\t\x12:\n\x07traffic\x18\x02 \x01(\x0b\x32\'.qwak.deployment.management.TrafficSpecH\x00\x12\x11\n\tprotected\x18\x04 \x01(\x08\x42\x06\n\x04spec\"4\n\x0bTrafficSpec\x12\x12\n\npercentage\x18\x01 \x01(\x05\x12\x11\n\tis_shadow\x18\x02 \x01(\x08\"]\n\x18\x46utureDeploymentSettings\x12\x41\n\x0etraffic_config\x18\x01 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\"\xb6\x01\n\x1c\x45nvironmentDeploymentMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x43\n\x0fhosting_service\x18\x04 \x01(\x0b\x32*.qwak.deployment.management.HostingService\x12\x16\n\nmodel_uuid\x18\x05 \x01(\tB\x02\x18\x01\"\x92\x01\n\"EnvironmentDeploymentResultMessage\x12\x1b\n\x13\x64\x65ployment_named_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x0c\n\x04info\x18\x03 \x01(\t\"\x90\x02\n\x1e\x45nvironmentUndeploymentMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12V\n\x14hosting_service_type\x18\x03 \x01(\x0e\x32\x38.qwak.deployment.management.DeploymentHostingServiceType\x12\x41\n\x0etraffic_config\x18\x04 \x01(\x0b\x32).qwak.deployment.management.TrafficConfig\x12\x16\n\x0evariation_name\x18\x05 \x01(\t\x12\x12\n\nmodel_uuid\x18\x06 \x01(\t\"w\n$EnvironmentUndeploymentResultMessage\x12\x41\n\x06status\x18\x01 \x01(\x0e\x32\x31.qwak.deployment.management.ModelDeploymentStatus\x12\x0c\n\x04info\x18\x02 \x01(\t\"\xd6\x01\n+EnvironmentRuntimeDeploymentSettingsMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12R\n\x13\x64\x65ployment_settings\x18\x03 \x01(\x0b\x32\x35.qwak.deployment.management.RuntimeDeploymentSettings\x12\x16\n\x0evariation_name\x18\x04 \x01(\t\x12\x12\n\nmodel_uuid\x18\x05 \x01(\t\"G\n1EnvironmentRuntimeDeploymentSettingsResultMessage\x12\x12\n\nerror_info\x18\x01 \x01(\t\"4\n$EnvironmentApplyModelTrafficResponse\x12\x0c\n\x04info\x18\x01 \x01(\t\"\xce\x01\n#EnvironmentDeploymentDetailsMessage\x12J\n\x13\x64\x65ployments_details\x18\x01 \x03(\x0b\x32-.qwak.deployment.management.DeploymentDetails\x12?\n\x10\x61udiences_routes\x18\x02 \x03(\x0b\x32%.qwak.audience.v1.AudienceRoutesEntry\x12\x1a\n\x12\x66\x61llback_variation\x18\x03 \x01(\t\"g\n#EnvironmentDeploymentHistoryMessage\x12@\n\x0b\x64\x65ployments\x18\x01 \x03(\x0b\x32+.qwak.deployment.management.DeploymentBrief\"V\n\x19\x45nvironmentTrafficMessage\x12\x39\n\nvariations\x18\x01 \x03(\x0b\x32%.qwak.deployment.management.Variation\"\x9e\x02\n BuildDeploymentEnvironmentStatus\x12\x87\x01\n\x1f\x65nvironment_to_deployment_brief\x18\x01 \x03(\x0b\x32^.qwak.deployment.management.BuildDeploymentEnvironmentStatus.EnvironmentToDeploymentBriefEntry\x1ap\n!EnvironmentToDeploymentBriefEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.qwak.deployment.management.DeploymentBrief:\x02\x38\x01\"S\n\x15\x42uildDeploymentStatus\x12\x12\n\nbuild_uuid\x18\x01 \x01(\t\x12\x13\n\x0bis_deployed\x18\x02 \x01(\x08\x12\x11\n\tis_in_use\x18\x03 \x01(\x08\"]\n\x1d\x43\x61ncelDeploymentRequestStatus\x12%\n\x1d\x63\x61ncel_requested_successfully\x18\x01 \x01(\x08\x12\x15\n\rerror_message\x18\x02 \x01(\t*\x85\x03\n\x15ModelDeploymentStatus\x12\x16\n\x12INVALID_DEPLOYMENT\x10\x00\x12\x19\n\x15INITIATING_DEPLOYMENT\x10\x01\x12 \n\x1c\x46\x41ILED_INITIATING_DEPLOYMENT\x10\x08\x12\x16\n\x12PENDING_DEPLOYMENT\x10\x02\x12\x19\n\x15SUCCESSFUL_DEPLOYMENT\x10\x03\x12\x15\n\x11\x46\x41ILED_DEPLOYMENT\x10\x04\x12\x1b\n\x17INITIATING_UNDEPLOYMENT\x10\t\x12\x18\n\x14PENDING_UNDEPLOYMENT\x10\n\x12\x1b\n\x17SUCCESSFUL_UNDEPLOYMENT\x10\x05\x12\x17\n\x13\x46\x41ILED_UNDEPLOYMENT\x10\x06\x12\t\n\x05UNSET\x10\x07\x12\x19\n\x15\x41LL_BUILDS_UNDEPLOYED\x10\x0b\x12\x18\n\x14\x43\x41NCELLED_DEPLOYMENT\x10\x0c\x12 \n\x1cINITIATING_CANCEL_DEPLOYMENT\x10\r*O\n\x1c\x44\x65ploymentHostingServiceType\x12\x0b\n\x07INVALID\x10\x00\x12\r\n\tSAGEMAKER\x10\x01\x12\x13\n\x0fKUBE_DEPLOYMENT\x10\x02*F\n\x12KubeDeploymentType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06ONLINE\x10\x01\x12\n\n\x06STREAM\x10\x02\x12\t\n\x05\x42\x41TCH\x10\x03*{\n\x07GpuType\x12\x0f\n\x0bINVALID_GPU\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06*+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x83\x01\n\x13\x44\x65ploymentManagedBy\x12!\n\x1d\x44\x45PLOYMENT_MANAGED_BY_INVALID\x10\x00\x12&\n\"DEPLOYMENT_MANAGED_BY_KUBE_CAPTAIN\x10\x01\x12!\n\x1d\x44\x45PLOYMENT_MANAGED_BY_ADMIRAL\x10\x02*\x93\x02\n\x1b\x44\x65ploymentFailureReasonCode\x12\x18\n\x14INVALID_FAILURE_CODE\x10\x00\x12\x12\n\x0eUNKNOWN_REASON\x10\x01\x12\x1e\n\x1aNO_REPLICA_SETS_PODS_FOUND\x10\x02\x12\x1d\n\x19MODEL_CONTAINER_NOT_FOUND\x10\x03\x12\x11\n\rUNSCHEDULABLE\x10\x04\x12\x1a\n\x16\x44OCKER_IMAGE_NOT_FOUND\x10\x05\x12\x19\n\x15MEMORY_LIMIT_EXCEEDED\x10\x06\x12\x0e\n\nCRASH_LOOP\x10\x07\x12-\n)CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON\x10\x08*\xb7\x01\n\rModelPodPhase\x12\x15\n\x11INVALID_POD_PHASE\x10\x00\x12)\n%MODEL_POD_PHASE_PROVISIONING_INSTANCE\x10\x01\x12!\n\x1dMODEL_POD_PHASE_PULLING_IMAGE\x10\x02\x12&\n\"MODEL_POD_PHASE_INITIALIZING_MODEL\x10\x03\x12\x19\n\x15MODEL_POD_PHASE_READY\x10\x04*\xac\x01\n\x13\x44\x65ploymentPhaseType\x12\x1c\n\x18INVALID_DEPLOYMENT_PHASE\x10\x00\x12*\n&DEPLOYMENT_PHASE_PROVISIONING_INSTANCE\x10\x01\x12\"\n\x1e\x44\x45PLOYMENT_PHASE_PULLING_IMAGE\x10\x02\x12\'\n#DEPLOYMENT_PHASE_INITIALIZING_MODEL\x10\x03*\xf5\x01\n\x15\x44\x65ploymentPhaseStatus\x12#\n\x1fINVALID_DEPLOYMENT_PHASE_STATUS\x10\x00\x12 \n\x1c\x44\x45PLOYMENT_PHASE_NOT_STARTED\x10\x01\x12\x1c\n\x18\x44\x45PLOYMENT_PHASE_STARTED\x10\x02\x12\x1d\n\x19\x44\x45PLOYMENT_PHASE_FINISHED\x10\x03\x12\x1d\n\x19\x44\x45PLOYMENT_PHASE_CANCELED\x10\x04\x12\x1b\n\x17\x44\x45PLOYMENT_PHASE_FAILED\x10\x05\x12\x1c\n\x18\x44\x45PLOYMENT_PHASE_ABORTED\x10\x06\x42\x45\n%com.qwak.ai.management.deployment.apiP\x01Z\x1aqwak/deployment;deploymentb\x06proto3')
 
 _MODELDEPLOYMENTSTATUS = DESCRIPTOR.enum_types_by_name['ModelDeploymentStatus']
 ModelDeploymentStatus = enum_type_wrapper.EnumTypeWrapper(_MODELDEPLOYMENTSTATUS)
 _DEPLOYMENTHOSTINGSERVICETYPE = DESCRIPTOR.enum_types_by_name['DeploymentHostingServiceType']
 DeploymentHostingServiceType = enum_type_wrapper.EnumTypeWrapper(_DEPLOYMENTHOSTINGSERVICETYPE)
 _KUBEDEPLOYMENTTYPE = DESCRIPTOR.enum_types_by_name['KubeDeploymentType']
 KubeDeploymentType = enum_type_wrapper.EnumTypeWrapper(_KUBEDEPLOYMENTTYPE)
@@ -509,34 +509,34 @@
   _ENVIRONMENTDEPLOYMENTMESSAGE.fields_by_name['model_uuid']._serialized_options = b'\030\001'
   _ENVIRONMENTUNDEPLOYMENTMESSAGE.fields_by_name['branch_id']._options = None
   _ENVIRONMENTUNDEPLOYMENTMESSAGE.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE.fields_by_name['branch_id']._options = None
   _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._options = None
   _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_options = b'8\001'
-  _MODELDEPLOYMENTSTATUS._serialized_start=8982
-  _MODELDEPLOYMENTSTATUS._serialized_end=9371
-  _DEPLOYMENTHOSTINGSERVICETYPE._serialized_start=9373
-  _DEPLOYMENTHOSTINGSERVICETYPE._serialized_end=9452
-  _KUBEDEPLOYMENTTYPE._serialized_start=9454
-  _KUBEDEPLOYMENTTYPE._serialized_end=9524
-  _GPUTYPE._serialized_start=9526
-  _GPUTYPE._serialized_end=9649
-  _MEMORYUNIT._serialized_start=9651
-  _MEMORYUNIT._serialized_end=9694
-  _DEPLOYMENTMANAGEDBY._serialized_start=9697
-  _DEPLOYMENTMANAGEDBY._serialized_end=9828
-  _DEPLOYMENTFAILUREREASONCODE._serialized_start=9831
-  _DEPLOYMENTFAILUREREASONCODE._serialized_end=10106
-  _MODELPODPHASE._serialized_start=10109
-  _MODELPODPHASE._serialized_end=10292
-  _DEPLOYMENTPHASETYPE._serialized_start=10295
-  _DEPLOYMENTPHASETYPE._serialized_end=10467
-  _DEPLOYMENTPHASESTATUS._serialized_start=10470
-  _DEPLOYMENTPHASESTATUS._serialized_end=10715
+  _MODELDEPLOYMENTSTATUS._serialized_start=9064
+  _MODELDEPLOYMENTSTATUS._serialized_end=9453
+  _DEPLOYMENTHOSTINGSERVICETYPE._serialized_start=9455
+  _DEPLOYMENTHOSTINGSERVICETYPE._serialized_end=9534
+  _KUBEDEPLOYMENTTYPE._serialized_start=9536
+  _KUBEDEPLOYMENTTYPE._serialized_end=9606
+  _GPUTYPE._serialized_start=9608
+  _GPUTYPE._serialized_end=9731
+  _MEMORYUNIT._serialized_start=9733
+  _MEMORYUNIT._serialized_end=9776
+  _DEPLOYMENTMANAGEDBY._serialized_start=9779
+  _DEPLOYMENTMANAGEDBY._serialized_end=9910
+  _DEPLOYMENTFAILUREREASONCODE._serialized_start=9913
+  _DEPLOYMENTFAILUREREASONCODE._serialized_end=10188
+  _MODELPODPHASE._serialized_start=10191
+  _MODELPODPHASE._serialized_end=10374
+  _DEPLOYMENTPHASETYPE._serialized_start=10377
+  _DEPLOYMENTPHASETYPE._serialized_end=10549
+  _DEPLOYMENTPHASESTATUS._serialized_start=10552
+  _DEPLOYMENTPHASESTATUS._serialized_end=10797
   _HOSTINGSERVICE._serialized_start=253
   _HOSTINGSERVICE._serialized_end=411
   _KUBEDEPLOYMENT._serialized_start=414
   _KUBEDEPLOYMENT._serialized_end=925
   _KUBEDEPLOYMENT_ENVIRONMENTVARIABLESENTRY._serialized_start=866
   _KUBEDEPLOYMENT_ENVIRONMENTVARIABLESENTRY._serialized_end=925
   _SERVINGSTRATEGY._serialized_start=928
@@ -562,73 +562,73 @@
   _SAGEMAKER._serialized_start=2351
   _SAGEMAKER._serialized_end=2409
   _DEPLOYMENTSIZE._serialized_start=2412
   _DEPLOYMENTSIZE._serialized_end=2734
   _GPURESOURCES._serialized_start=2736
   _GPURESOURCES._serialized_end=2825
   _ADVANCEDDEPLOYMENTOPTIONS._serialized_start=2828
-  _ADVANCEDDEPLOYMENTOPTIONS._serialized_end=3096
-  _DEPLOYMENTDETAILS._serialized_start=3099
-  _DEPLOYMENTDETAILS._serialized_end=4275
+  _ADVANCEDDEPLOYMENTOPTIONS._serialized_end=3137
+  _DEPLOYMENTDETAILS._serialized_start=3140
+  _DEPLOYMENTDETAILS._serialized_end=4357
   _DEPLOYMENTDETAILS_ENVIRONMENTVARIABLESENTRY._serialized_start=866
   _DEPLOYMENTDETAILS_ENVIRONMENTVARIABLESENTRY._serialized_end=925
-  _DEPLOYMENTFAILUREDETAILS._serialized_start=4277
-  _DEPLOYMENTFAILUREDETAILS._serialized_end=4328
-  _RUNTIMEDEPLOYMENTSETTINGS._serialized_start=4331
-  _RUNTIMEDEPLOYMENTSETTINGS._serialized_end=4516
-  _RUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_start=4451
-  _RUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_end=4516
-  _DEPLOYMENTBRIEF._serialized_start=4519
-  _DEPLOYMENTBRIEF._serialized_end=4885
-  _KUBERNETESMODELDEPLOYMENTSTATE._serialized_start=4888
-  _KUBERNETESMODELDEPLOYMENTSTATE._serialized_end=5231
-  _STATUSDETAILS._serialized_start=5234
-  _STATUSDETAILS._serialized_end=5520
-  _PENDINGSTATUSDETAILS._serialized_start=5523
-  _PENDINGSTATUSDETAILS._serialized_end=5679
-  _SUCCESSFULSTATUSDETAILS._serialized_start=5681
-  _SUCCESSFULSTATUSDETAILS._serialized_end=5777
-  _FAILEDSTATUSDETAILS._serialized_start=5780
-  _FAILEDSTATUSDETAILS._serialized_end=6007
-  _FAILUREDETAILS._serialized_start=6010
-  _FAILUREDETAILS._serialized_end=6155
-  _INSTANCEDETAILS._serialized_start=6158
-  _INSTANCEDETAILS._serialized_end=6301
-  _DEPLOYMENTPHASESDETAILS._serialized_start=6303
-  _DEPLOYMENTPHASESDETAILS._serialized_end=6400
-  _DEPLOYMENTPHASE._serialized_start=6403
-  _DEPLOYMENTPHASE._serialized_end=6746
-  _VARIATION._serialized_start=6749
-  _VARIATION._serialized_end=6885
-  _TRAFFICSPEC._serialized_start=6887
-  _TRAFFICSPEC._serialized_end=6939
-  _FUTUREDEPLOYMENTSETTINGS._serialized_start=6941
-  _FUTUREDEPLOYMENTSETTINGS._serialized_end=7034
-  _ENVIRONMENTDEPLOYMENTMESSAGE._serialized_start=7037
-  _ENVIRONMENTDEPLOYMENTMESSAGE._serialized_end=7219
-  _ENVIRONMENTDEPLOYMENTRESULTMESSAGE._serialized_start=7222
-  _ENVIRONMENTDEPLOYMENTRESULTMESSAGE._serialized_end=7368
-  _ENVIRONMENTUNDEPLOYMENTMESSAGE._serialized_start=7371
-  _ENVIRONMENTUNDEPLOYMENTMESSAGE._serialized_end=7643
-  _ENVIRONMENTUNDEPLOYMENTRESULTMESSAGE._serialized_start=7645
-  _ENVIRONMENTUNDEPLOYMENTRESULTMESSAGE._serialized_end=7764
-  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE._serialized_start=7767
-  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE._serialized_end=7981
-  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSRESULTMESSAGE._serialized_start=7983
-  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSRESULTMESSAGE._serialized_end=8054
-  _ENVIRONMENTAPPLYMODELTRAFFICRESPONSE._serialized_start=8056
-  _ENVIRONMENTAPPLYMODELTRAFFICRESPONSE._serialized_end=8108
-  _ENVIRONMENTDEPLOYMENTDETAILSMESSAGE._serialized_start=8111
-  _ENVIRONMENTDEPLOYMENTDETAILSMESSAGE._serialized_end=8317
-  _ENVIRONMENTDEPLOYMENTHISTORYMESSAGE._serialized_start=8319
-  _ENVIRONMENTDEPLOYMENTHISTORYMESSAGE._serialized_end=8422
-  _ENVIRONMENTTRAFFICMESSAGE._serialized_start=8424
-  _ENVIRONMENTTRAFFICMESSAGE._serialized_end=8510
-  _BUILDDEPLOYMENTENVIRONMENTSTATUS._serialized_start=8513
-  _BUILDDEPLOYMENTENVIRONMENTSTATUS._serialized_end=8799
-  _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_start=8687
-  _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_end=8799
-  _BUILDDEPLOYMENTSTATUS._serialized_start=8801
-  _BUILDDEPLOYMENTSTATUS._serialized_end=8884
-  _CANCELDEPLOYMENTREQUESTSTATUS._serialized_start=8886
-  _CANCELDEPLOYMENTREQUESTSTATUS._serialized_end=8979
+  _DEPLOYMENTFAILUREDETAILS._serialized_start=4359
+  _DEPLOYMENTFAILUREDETAILS._serialized_end=4410
+  _RUNTIMEDEPLOYMENTSETTINGS._serialized_start=4413
+  _RUNTIMEDEPLOYMENTSETTINGS._serialized_end=4598
+  _RUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_start=4533
+  _RUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_end=4598
+  _DEPLOYMENTBRIEF._serialized_start=4601
+  _DEPLOYMENTBRIEF._serialized_end=4967
+  _KUBERNETESMODELDEPLOYMENTSTATE._serialized_start=4970
+  _KUBERNETESMODELDEPLOYMENTSTATE._serialized_end=5313
+  _STATUSDETAILS._serialized_start=5316
+  _STATUSDETAILS._serialized_end=5602
+  _PENDINGSTATUSDETAILS._serialized_start=5605
+  _PENDINGSTATUSDETAILS._serialized_end=5761
+  _SUCCESSFULSTATUSDETAILS._serialized_start=5763
+  _SUCCESSFULSTATUSDETAILS._serialized_end=5859
+  _FAILEDSTATUSDETAILS._serialized_start=5862
+  _FAILEDSTATUSDETAILS._serialized_end=6089
+  _FAILUREDETAILS._serialized_start=6092
+  _FAILUREDETAILS._serialized_end=6237
+  _INSTANCEDETAILS._serialized_start=6240
+  _INSTANCEDETAILS._serialized_end=6383
+  _DEPLOYMENTPHASESDETAILS._serialized_start=6385
+  _DEPLOYMENTPHASESDETAILS._serialized_end=6482
+  _DEPLOYMENTPHASE._serialized_start=6485
+  _DEPLOYMENTPHASE._serialized_end=6828
+  _VARIATION._serialized_start=6831
+  _VARIATION._serialized_end=6967
+  _TRAFFICSPEC._serialized_start=6969
+  _TRAFFICSPEC._serialized_end=7021
+  _FUTUREDEPLOYMENTSETTINGS._serialized_start=7023
+  _FUTUREDEPLOYMENTSETTINGS._serialized_end=7116
+  _ENVIRONMENTDEPLOYMENTMESSAGE._serialized_start=7119
+  _ENVIRONMENTDEPLOYMENTMESSAGE._serialized_end=7301
+  _ENVIRONMENTDEPLOYMENTRESULTMESSAGE._serialized_start=7304
+  _ENVIRONMENTDEPLOYMENTRESULTMESSAGE._serialized_end=7450
+  _ENVIRONMENTUNDEPLOYMENTMESSAGE._serialized_start=7453
+  _ENVIRONMENTUNDEPLOYMENTMESSAGE._serialized_end=7725
+  _ENVIRONMENTUNDEPLOYMENTRESULTMESSAGE._serialized_start=7727
+  _ENVIRONMENTUNDEPLOYMENTRESULTMESSAGE._serialized_end=7846
+  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE._serialized_start=7849
+  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSMESSAGE._serialized_end=8063
+  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSRESULTMESSAGE._serialized_start=8065
+  _ENVIRONMENTRUNTIMEDEPLOYMENTSETTINGSRESULTMESSAGE._serialized_end=8136
+  _ENVIRONMENTAPPLYMODELTRAFFICRESPONSE._serialized_start=8138
+  _ENVIRONMENTAPPLYMODELTRAFFICRESPONSE._serialized_end=8190
+  _ENVIRONMENTDEPLOYMENTDETAILSMESSAGE._serialized_start=8193
+  _ENVIRONMENTDEPLOYMENTDETAILSMESSAGE._serialized_end=8399
+  _ENVIRONMENTDEPLOYMENTHISTORYMESSAGE._serialized_start=8401
+  _ENVIRONMENTDEPLOYMENTHISTORYMESSAGE._serialized_end=8504
+  _ENVIRONMENTTRAFFICMESSAGE._serialized_start=8506
+  _ENVIRONMENTTRAFFICMESSAGE._serialized_end=8592
+  _BUILDDEPLOYMENTENVIRONMENTSTATUS._serialized_start=8595
+  _BUILDDEPLOYMENTENVIRONMENTSTATUS._serialized_end=8881
+  _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_start=8769
+  _BUILDDEPLOYMENTENVIRONMENTSTATUS_ENVIRONMENTTODEPLOYMENTBRIEFENTRY._serialized_end=8881
+  _BUILDDEPLOYMENTSTATUS._serialized_start=8883
+  _BUILDDEPLOYMENTSTATUS._serialized_end=8966
+  _CANCELDEPLOYMENTREQUESTSTATUS._serialized_start=8968
+  _CANCELDEPLOYMENTREQUESTSTATUS._serialized_end=9061
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -669,14 +669,15 @@
     NUMBER_OF_HTTP_SERVER_WORKERS_FIELD_NUMBER: builtins.int
     HTTP_REQUEST_TIMEOUT_MS_FIELD_NUMBER: builtins.int
     DAEMON_MODE_FIELD_NUMBER: builtins.int
     CUSTOM_IAM_ROLE_ARN_FIELD_NUMBER: builtins.int
     MAX_BATCH_SIZE_FIELD_NUMBER: builtins.int
     DEPLOYMENT_PROCESS_TIMEOUT_LIMIT_FIELD_NUMBER: builtins.int
     PURCHASE_OPTION_FIELD_NUMBER: builtins.int
+    SERVICE_ACCOUNT_KEY_SECRET_NAME_FIELD_NUMBER: builtins.int
     number_of_http_server_workers: builtins.int
     """Amount of http server workers"""
     http_request_timeout_ms: builtins.int
     """Http request timeout in ms"""
     @property
     def daemon_mode(self) -> google.protobuf.wrappers_pb2.BoolValue:
         """Serve model container in daemon mode"""
@@ -684,27 +685,30 @@
     """Custom IAM Role ARN"""
     max_batch_size: builtins.int
     """Max batch size of records"""
     deployment_process_timeout_limit: builtins.int
     """The timeout for the deployment (in seconds)"""
     purchase_option: builtins.str
     """Whether it is spot/ondemand (default - spot)"""
+    service_account_key_secret_name: builtins.str
+    """Service account key secret name for gcp"""
     def __init__(
         self,
         *,
         number_of_http_server_workers: builtins.int = ...,
         http_request_timeout_ms: builtins.int = ...,
         daemon_mode: google.protobuf.wrappers_pb2.BoolValue | None = ...,
         custom_iam_role_arn: builtins.str = ...,
         max_batch_size: builtins.int = ...,
         deployment_process_timeout_limit: builtins.int = ...,
         purchase_option: builtins.str = ...,
+        service_account_key_secret_name: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["daemon_mode", b"daemon_mode"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["custom_iam_role_arn", b"custom_iam_role_arn", "daemon_mode", b"daemon_mode", "deployment_process_timeout_limit", b"deployment_process_timeout_limit", "http_request_timeout_ms", b"http_request_timeout_ms", "max_batch_size", b"max_batch_size", "number_of_http_server_workers", b"number_of_http_server_workers", "purchase_option", b"purchase_option"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["custom_iam_role_arn", b"custom_iam_role_arn", "daemon_mode", b"daemon_mode", "deployment_process_timeout_limit", b"deployment_process_timeout_limit", "http_request_timeout_ms", b"http_request_timeout_ms", "max_batch_size", b"max_batch_size", "number_of_http_server_workers", b"number_of_http_server_workers", "purchase_option", b"purchase_option", "service_account_key_secret_name", b"service_account_key_secret_name"]) -> None: ...
 
 global___AdvancedDeploymentOptions = AdvancedDeploymentOptions
 
 class DeploymentDetails(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class EnvironmentVariablesEntry(google.protobuf.message.Message):
@@ -743,14 +747,15 @@
     DEPLOYMENT_PROCESS_TIMEOUT_LIMIT_FIELD_NUMBER: builtins.int
     PURCHASE_OPTION_FIELD_NUMBER: builtins.int
     ENVIRONMENT_VARIABLES_FIELD_NUMBER: builtins.int
     UNDEPLOYMENT_TIME_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     DEPLOYMENT_ID_FIELD_NUMBER: builtins.int
     FAILURE_DETAILS_FIELD_NUMBER: builtins.int
+    SERVICE_ACCOUNT_KEY_SECRET_NAME_FIELD_NUMBER: builtins.int
     @property
     def last_deployed(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Deployed date"""
     build_id: builtins.str
     """The build id that deployed"""
     number_of_pods: builtins.int
     """Number of pods to deploy"""
@@ -799,14 +804,16 @@
         """Time that the deployment was changed."""
     status: global___ModelDeploymentStatus.ValueType
     """The status of the deployment"""
     deployment_id: builtins.str
     """Deployment id"""
     @property
     def failure_details(self) -> global___DeploymentFailureDetails: ...
+    service_account_key_secret_name: builtins.str
+    """Service account key secret name for gcp"""
     def __init__(
         self,
         *,
         last_deployed: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         build_id: builtins.str = ...,
         number_of_pods: builtins.int = ...,
         cpu_fraction: builtins.float = ...,
@@ -827,17 +834,18 @@
         deployment_process_timeout_limit: builtins.int = ...,
         purchase_option: builtins.str = ...,
         environment_variables: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         undeployment_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         status: global___ModelDeploymentStatus.ValueType = ...,
         deployment_id: builtins.str = ...,
         failure_details: global___DeploymentFailureDetails | None = ...,
+        service_account_key_secret_name: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["daemon_mode", b"daemon_mode", "failure_details", b"failure_details", "last_deployed", b"last_deployed", "serving_strategy", b"serving_strategy", "undeployment_time", b"undeployment_time", "variation", b"variation"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["available_replicas", b"available_replicas", "build_id", b"build_id", "cpu_fraction", b"cpu_fraction", "custom_iam_role_arn", b"custom_iam_role_arn", "daemon_mode", b"daemon_mode", "deployment_id", b"deployment_id", "deployment_process_timeout_limit", b"deployment_process_timeout_limit", "environment_id", b"environment_id", "environment_variables", b"environment_variables", "failure_details", b"failure_details", "gpu_amount", b"gpu_amount", "gpu_type", b"gpu_type", "http_request_timeout_ms", b"http_request_timeout_ms", "kube_deployment_type", b"kube_deployment_type", "last_deployed", b"last_deployed", "max_batch_size", b"max_batch_size", "memory_amount", b"memory_amount", "memory_units", b"memory_units", "number_of_pods", b"number_of_pods", "number_of_workers", b"number_of_workers", "purchase_option", b"purchase_option", "serving_strategy", b"serving_strategy", "status", b"status", "undeployment_time", b"undeployment_time", "variation", b"variation"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["available_replicas", b"available_replicas", "build_id", b"build_id", "cpu_fraction", b"cpu_fraction", "custom_iam_role_arn", b"custom_iam_role_arn", "daemon_mode", b"daemon_mode", "deployment_id", b"deployment_id", "deployment_process_timeout_limit", b"deployment_process_timeout_limit", "environment_id", b"environment_id", "environment_variables", b"environment_variables", "failure_details", b"failure_details", "gpu_amount", b"gpu_amount", "gpu_type", b"gpu_type", "http_request_timeout_ms", b"http_request_timeout_ms", "kube_deployment_type", b"kube_deployment_type", "last_deployed", b"last_deployed", "max_batch_size", b"max_batch_size", "memory_amount", b"memory_amount", "memory_units", b"memory_units", "number_of_pods", b"number_of_pods", "number_of_workers", b"number_of_workers", "purchase_option", b"purchase_option", "service_account_key_secret_name", b"service_account_key_secret_name", "serving_strategy", b"serving_strategy", "status", b"status", "undeployment_time", b"undeployment_time", "variation", b"variation"]) -> None: ...
 
 global___DeploymentDetails = DeploymentDetails
 
 class DeploymentFailureDetails(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FAILURE_MESSAGE_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/backfill_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/batch_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/batch_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/execution_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.execution.v1 import backfill_pb2 as qwak_dot_execution_dot_v1_dot_backfill__pb2
 from _qwak_proto.qwak.execution.v1 import batch_pb2 as qwak_dot_execution_dot_v1_dot_batch__pb2
+from _qwak_proto.qwak.execution.v1 import deletion_pb2 as qwak_dot_execution_dot_v1_dot_deletion__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!qwak/execution/v1/execution.proto\x12\x1fqwak.feature.store.execution.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a qwak/execution/v1/backfill.proto\x1a\x1dqwak/execution/v1/batch.proto\"\x88\x04\n\x0e\x45xecutionEntry\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12J\n\x10\x65xecution_status\x18\x03 \x01(\x0e\x32\x30.qwak.feature.store.execution.v1.ExecutionStatus\x12\x30\n\x0csubmitted_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x45\n\x0csubmitted_by\x18\x05 \x01(\x0b\x32/.qwak.feature.store.execution.v1.InvokerDetails\x12\x30\n\x0ctriggered_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x46\n\rbackfill_spec\x18\x08 \x01(\x0b\x32-.qwak.feature.store.execution.v1.BackfillSpecH\x00\x12J\n\x0f\x62\x61tch_ingestion\x18\t \x01(\x0b\x32/.qwak.feature.store.execution.v1.BatchIngestionH\x00\x42\x10\n\x0e\x65xecution_type\"\xbc\x01\n\x0eInvokerDetails\x12L\n\x10\x65xternal_invoker\x18\x01 \x01(\x0b\x32\x30.qwak.feature.store.execution.v1.ExternalInvokerH\x00\x12L\n\x10internal_invoker\x18\x02 \x01(\x0b\x32\x30.qwak.feature.store.execution.v1.InternalInvokerH\x00\x42\x0e\n\x0cinvoker_type\"(\n\x0f\x45xternalInvoker\x12\x15\n\rinvoker_email\x18\x01 \x01(\t\"\x11\n\x0fInternalInvoker*\xcb\x02\n\x0f\x45xecutionStatus\x12\x1c\n\x18\x45XECUTION_STATUS_INVALID\x10\x00\x12\x1b\n\x17\x45XECUTION_STATUS_QUEUED\x10\x01\x12\x1c\n\x18\x45XECUTION_STATUS_PENDING\x10\x02\x12\x1c\n\x18\x45XECUTION_STATUS_RUNNING\x10\x03\x12\x1e\n\x1a\x45XECUTION_STATUS_COMPLETED\x10\x04\x12\x1b\n\x17\x45XECUTION_STATUS_FAILED\x10\x05\x12\x1e\n\x1a\x45XECUTION_STATUS_CANCELLED\x10\x06\x12\x1e\n\x1a\x45XECUTION_STATUS_SUBMITTED\x10\x07\x12&\n\"EXECUTION_STATUS_FAILED_SUBMISSION\x10\x08\x12\x1c\n\x18\x45XECUTION_STATUS_SKIPPED\x10\tBN\n%com.qwak.ai.features.execution.api.v1P\x01Z#qwak/execution_management;executionb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!qwak/execution/v1/execution.proto\x12\x1fqwak.feature.store.execution.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a qwak/execution/v1/backfill.proto\x1a\x1dqwak/execution/v1/batch.proto\x1a qwak/execution/v1/deletion.proto\"\xdc\x04\n\x0e\x45xecutionEntry\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12J\n\x10\x65xecution_status\x18\x03 \x01(\x0e\x32\x30.qwak.feature.store.execution.v1.ExecutionStatus\x12\x30\n\x0csubmitted_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x45\n\x0csubmitted_by\x18\x05 \x01(\x0b\x32/.qwak.feature.store.execution.v1.InvokerDetails\x12\x30\n\x0ctriggered_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x46\n\rbackfill_spec\x18\x08 \x01(\x0b\x32-.qwak.feature.store.execution.v1.BackfillSpecH\x00\x12J\n\x0f\x62\x61tch_ingestion\x18\t \x01(\x0b\x32/.qwak.feature.store.execution.v1.BatchIngestionH\x00\x12R\n\x13\x66\x65\x61tureset_deletion\x18\n \x01(\x0b\x32\x33.qwak.feature.store.execution.v1.FeaturesetDeletionH\x00\x42\x10\n\x0e\x65xecution_type\"\xbc\x01\n\x0eInvokerDetails\x12L\n\x10\x65xternal_invoker\x18\x01 \x01(\x0b\x32\x30.qwak.feature.store.execution.v1.ExternalInvokerH\x00\x12L\n\x10internal_invoker\x18\x02 \x01(\x0b\x32\x30.qwak.feature.store.execution.v1.InternalInvokerH\x00\x42\x0e\n\x0cinvoker_type\"(\n\x0f\x45xternalInvoker\x12\x15\n\rinvoker_email\x18\x01 \x01(\t\"\x11\n\x0fInternalInvoker*\xcb\x02\n\x0f\x45xecutionStatus\x12\x1c\n\x18\x45XECUTION_STATUS_INVALID\x10\x00\x12\x1b\n\x17\x45XECUTION_STATUS_QUEUED\x10\x01\x12\x1c\n\x18\x45XECUTION_STATUS_PENDING\x10\x02\x12\x1c\n\x18\x45XECUTION_STATUS_RUNNING\x10\x03\x12\x1e\n\x1a\x45XECUTION_STATUS_COMPLETED\x10\x04\x12\x1b\n\x17\x45XECUTION_STATUS_FAILED\x10\x05\x12\x1e\n\x1a\x45XECUTION_STATUS_CANCELLED\x10\x06\x12\x1e\n\x1a\x45XECUTION_STATUS_SUBMITTED\x10\x07\x12&\n\"EXECUTION_STATUS_FAILED_SUBMISSION\x10\x08\x12\x1c\n\x18\x45XECUTION_STATUS_SKIPPED\x10\tBN\n%com.qwak.ai.features.execution.api.v1P\x01Z#qwak/execution_management;executionb\x06proto3')
 
 _EXECUTIONSTATUS = DESCRIPTOR.enum_types_by_name['ExecutionStatus']
 ExecutionStatus = enum_type_wrapper.EnumTypeWrapper(_EXECUTIONSTATUS)
 EXECUTION_STATUS_INVALID = 0
 EXECUTION_STATUS_QUEUED = 1
 EXECUTION_STATUS_PENDING = 2
 EXECUTION_STATUS_RUNNING = 3
@@ -66,18 +67,18 @@
   })
 _sym_db.RegisterMessage(InternalInvoker)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n%com.qwak.ai.features.execution.api.v1P\001Z#qwak/execution_management;execution'
-  _EXECUTIONSTATUS._serialized_start=944
-  _EXECUTIONSTATUS._serialized_end=1275
-  _EXECUTIONENTRY._serialized_start=169
-  _EXECUTIONENTRY._serialized_end=689
-  _INVOKERDETAILS._serialized_start=692
-  _INVOKERDETAILS._serialized_end=880
-  _EXTERNALINVOKER._serialized_start=882
-  _EXTERNALINVOKER._serialized_end=922
-  _INTERNALINVOKER._serialized_start=924
-  _INTERNALINVOKER._serialized_end=941
+  _EXECUTIONSTATUS._serialized_start=1062
+  _EXECUTIONSTATUS._serialized_end=1393
+  _EXECUTIONENTRY._serialized_start=203
+  _EXECUTIONENTRY._serialized_end=807
+  _INVOKERDETAILS._serialized_start=810
+  _INVOKERDETAILS._serialized_end=998
+  _EXTERNALINVOKER._serialized_start=1000
+  _EXTERNALINVOKER._serialized_end=1040
+  _INTERNALINVOKER._serialized_start=1042
+  _INTERNALINVOKER._serialized_end=1059
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/execution_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
 import qwak.execution.v1.backfill_pb2
 import qwak.execution.v1.batch_pb2
+import qwak.execution.v1.deletion_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
@@ -58,14 +59,15 @@
     EXECUTION_STATUS_FIELD_NUMBER: builtins.int
     SUBMITTED_AT_FIELD_NUMBER: builtins.int
     SUBMITTED_BY_FIELD_NUMBER: builtins.int
     TRIGGERED_AT_FIELD_NUMBER: builtins.int
     ENDED_AT_FIELD_NUMBER: builtins.int
     BACKFILL_SPEC_FIELD_NUMBER: builtins.int
     BATCH_INGESTION_FIELD_NUMBER: builtins.int
+    FEATURESET_DELETION_FIELD_NUMBER: builtins.int
     featureset_id: builtins.str
     execution_id: builtins.str
     execution_status: global___ExecutionStatus.ValueType
     @property
     def submitted_at(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
     def submitted_by(self) -> global___InvokerDetails: ...
@@ -74,30 +76,34 @@
     @property
     def ended_at(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
     def backfill_spec(self) -> qwak.execution.v1.backfill_pb2.BackfillSpec: ...
     @property
     def batch_ingestion(self) -> qwak.execution.v1.batch_pb2.BatchIngestion:
         """"Regular" batch ingestion"""
+    @property
+    def featureset_deletion(self) -> qwak.execution.v1.deletion_pb2.FeaturesetDeletion:
+        """Featureset deletion"""
     def __init__(
         self,
         *,
         featureset_id: builtins.str = ...,
         execution_id: builtins.str = ...,
         execution_status: global___ExecutionStatus.ValueType = ...,
         submitted_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         submitted_by: global___InvokerDetails | None = ...,
         triggered_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         ended_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         backfill_spec: qwak.execution.v1.backfill_pb2.BackfillSpec | None = ...,
         batch_ingestion: qwak.execution.v1.batch_pb2.BatchIngestion | None = ...,
+        featureset_deletion: qwak.execution.v1.deletion_pb2.FeaturesetDeletion | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["backfill_spec", b"backfill_spec", "batch_ingestion", b"batch_ingestion", "ended_at", b"ended_at", "execution_type", b"execution_type", "submitted_at", b"submitted_at", "submitted_by", b"submitted_by", "triggered_at", b"triggered_at"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["backfill_spec", b"backfill_spec", "batch_ingestion", b"batch_ingestion", "ended_at", b"ended_at", "execution_id", b"execution_id", "execution_status", b"execution_status", "execution_type", b"execution_type", "featureset_id", b"featureset_id", "submitted_at", b"submitted_at", "submitted_by", b"submitted_by", "triggered_at", b"triggered_at"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["execution_type", b"execution_type"]) -> typing_extensions.Literal["backfill_spec", "batch_ingestion"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["backfill_spec", b"backfill_spec", "batch_ingestion", b"batch_ingestion", "ended_at", b"ended_at", "execution_type", b"execution_type", "featureset_deletion", b"featureset_deletion", "submitted_at", b"submitted_at", "submitted_by", b"submitted_by", "triggered_at", b"triggered_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["backfill_spec", b"backfill_spec", "batch_ingestion", b"batch_ingestion", "ended_at", b"ended_at", "execution_id", b"execution_id", "execution_status", b"execution_status", "execution_type", b"execution_type", "featureset_deletion", b"featureset_deletion", "featureset_id", b"featureset_id", "submitted_at", b"submitted_at", "submitted_by", b"submitted_by", "triggered_at", b"triggered_at"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["execution_type", b"execution_type"]) -> typing_extensions.Literal["backfill_spec", "batch_ingestion", "featureset_deletion"] | None: ...
 
 global___ExecutionEntry = ExecutionEntry
 
 class InvokerDetails(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EXTERNAL_INVOKER_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,14 +20,19 @@
                 response_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerBackfillResponse.FromString,
                 )
         self.TriggerBatchFeatureset = channel.unary_unary(
                 '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/TriggerBatchFeatureset',
                 request_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerBatchFeaturesetRequest.SerializeToString,
                 response_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerBatchFeaturesetResponse.FromString,
                 )
+        self.TriggerFeaturesetDeletion = channel.unary_unary(
+                '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/TriggerFeaturesetDeletion',
+                request_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerFeaturesetDeletionRequest.SerializeToString,
+                response_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerFeaturesetDeletionResponse.FromString,
+                )
         self.GetExecutionStatus = channel.unary_unary(
                 '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/GetExecutionStatus',
                 request_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetExecutionStatusRequest.SerializeToString,
                 response_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetExecutionStatusResponse.FromString,
                 )
         self.GetExecutionEntry = channel.unary_unary(
                 '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/GetExecutionEntry',
@@ -35,14 +40,24 @@
                 response_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetExecutionEntryResponse.FromString,
                 )
         self.GetRunningExecutionEntries = channel.unary_unary(
                 '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/GetRunningExecutionEntries',
                 request_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetRunningExecutionEntriesRequest.SerializeToString,
                 response_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetRunningExecutionEntriesResponse.FromString,
                 )
+        self.InitPaginationByFeaturesetId = channel.unary_unary(
+                '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/InitPaginationByFeaturesetId',
+                request_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.InitPaginationByFeaturesetIdRequest.SerializeToString,
+                response_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.InitPaginationByFeaturesetIdResponse.FromString,
+                )
+        self.ListExecutionsByFeaturesetId = channel.unary_unary(
+                '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/ListExecutionsByFeaturesetId',
+                request_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.ListExecutionsByFeaturesetIdRequest.SerializeToString,
+                response_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.ListExecutionsByFeaturesetIdResponse.FromString,
+                )
 
 
 class FeatureStoreExecutionServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def TriggerBatchBackfill(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -52,14 +67,20 @@
 
     def TriggerBatchFeatureset(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def TriggerFeaturesetDeletion(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetExecutionStatus(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetExecutionEntry(self, request, context):
@@ -70,27 +91,44 @@
 
     def GetRunningExecutionEntries(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def InitPaginationByFeaturesetId(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ListExecutionsByFeaturesetId(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_FeatureStoreExecutionServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'TriggerBatchBackfill': grpc.unary_unary_rpc_method_handler(
                     servicer.TriggerBatchBackfill,
                     request_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerBackfillRequest.FromString,
                     response_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerBackfillResponse.SerializeToString,
             ),
             'TriggerBatchFeatureset': grpc.unary_unary_rpc_method_handler(
                     servicer.TriggerBatchFeatureset,
                     request_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerBatchFeaturesetRequest.FromString,
                     response_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerBatchFeaturesetResponse.SerializeToString,
             ),
+            'TriggerFeaturesetDeletion': grpc.unary_unary_rpc_method_handler(
+                    servicer.TriggerFeaturesetDeletion,
+                    request_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerFeaturesetDeletionRequest.FromString,
+                    response_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerFeaturesetDeletionResponse.SerializeToString,
+            ),
             'GetExecutionStatus': grpc.unary_unary_rpc_method_handler(
                     servicer.GetExecutionStatus,
                     request_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetExecutionStatusRequest.FromString,
                     response_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetExecutionStatusResponse.SerializeToString,
             ),
             'GetExecutionEntry': grpc.unary_unary_rpc_method_handler(
                     servicer.GetExecutionEntry,
@@ -98,14 +136,24 @@
                     response_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetExecutionEntryResponse.SerializeToString,
             ),
             'GetRunningExecutionEntries': grpc.unary_unary_rpc_method_handler(
                     servicer.GetRunningExecutionEntries,
                     request_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetRunningExecutionEntriesRequest.FromString,
                     response_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetRunningExecutionEntriesResponse.SerializeToString,
             ),
+            'InitPaginationByFeaturesetId': grpc.unary_unary_rpc_method_handler(
+                    servicer.InitPaginationByFeaturesetId,
+                    request_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.InitPaginationByFeaturesetIdRequest.FromString,
+                    response_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.InitPaginationByFeaturesetIdResponse.SerializeToString,
+            ),
+            'ListExecutionsByFeaturesetId': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListExecutionsByFeaturesetId,
+                    request_deserializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.ListExecutionsByFeaturesetIdRequest.FromString,
+                    response_serializer=qwak_dot_execution_dot_v1_dot_execution__service__pb2.ListExecutionsByFeaturesetIdResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'qwak.feature.store.execution.v1.FeatureStoreExecutionService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -143,14 +191,31 @@
         return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/TriggerBatchFeatureset',
             qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerBatchFeaturesetRequest.SerializeToString,
             qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerBatchFeaturesetResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def TriggerFeaturesetDeletion(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/TriggerFeaturesetDeletion',
+            qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerFeaturesetDeletionRequest.SerializeToString,
+            qwak_dot_execution_dot_v1_dot_execution__service__pb2.TriggerFeaturesetDeletionResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetExecutionStatus(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -192,7 +257,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/GetRunningExecutionEntries',
             qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetRunningExecutionEntriesRequest.SerializeToString,
             qwak_dot_execution_dot_v1_dot_execution__service__pb2.GetRunningExecutionEntriesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def InitPaginationByFeaturesetId(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/InitPaginationByFeaturesetId',
+            qwak_dot_execution_dot_v1_dot_execution__service__pb2.InitPaginationByFeaturesetIdRequest.SerializeToString,
+            qwak_dot_execution_dot_v1_dot_execution__service__pb2.InitPaginationByFeaturesetIdResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListExecutionsByFeaturesetId(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.FeatureStoreExecutionService/ListExecutionsByFeaturesetId',
+            qwak_dot_execution_dot_v1_dot_execution__service__pb2.ListExecutionsByFeaturesetIdRequest.SerializeToString,
+            qwak_dot_execution_dot_v1_dot_execution__service__pb2.ListExecutionsByFeaturesetIdResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,33 +12,39 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.execution.v1.jobs import job_pb2 as qwak_dot_execution_dot_v1_dot_jobs_dot_job__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(qwak/execution/v1/jobs/job_service.proto\x12$qwak.feature.store.execution.v1.jobs\x1a\x1fgoogle/protobuf/timestamp.proto\x1a qwak/execution/v1/jobs/job.proto\"\\\n\x15\x41pplyJobRecordRequest\x12\x43\n\njob_record\x18\x01 \x01(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecord\"\x18\n\x16\x41pplyJobRecordResponse\".\n\x15InitPaginationRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\"E\n\x16InitPaginationResponse\x12\x14\n\x0crecord_count\x18\x01 \x01(\x03\x12\x15\n\rmax_record_id\x18\x02 \x01(\x03\"g\n\x0fListJobsRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x13\n\x0bpage_number\x18\x03 \x01(\x05\x12\x15\n\rmax_record_id\x18\x04 \x01(\x03\"X\n\x10ListJobsResponse\x12\x44\n\x0bjob_records\x18\x01 \x03(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecord\"4\n\x1b\x44\x65leteFeaturesetJobsRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\"@\n\x1c\x44\x65leteFeaturesetJobsResponse\x12 \n\x18\x64\x65leted_job_record_count\x18\x01 \x01(\x03\"D\n+GetLatestSuccessfulJobByFeaturesetIdRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\"\x88\x01\n,GetLatestSuccessfulJobByFeaturesetIdResponse\x12\x45\n\njob_record\x18\x01 \x01(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecordH\x00\x42\x11\n\x0fjob_record_resp\"-\n+GetAllFeaturesetLatestSuccessfulJobsRequest\"t\n,GetAllFeaturesetLatestSuccessfulJobsResponse\x12\x44\n\x0bjob_records\x18\x01 \x03(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecord\"\xa3\x01\n$GetAllFeaturesetJobsSummariesRequest\x12\x34\n\x10lower_time_bound\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x10upper_time_bound\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x42\r\n\x0bupper_bound\"|\n%GetAllFeaturesetJobsSummariesResponse\x12S\n\x0ejobs_summaries\x18\x01 \x03(\x0b\x32;.qwak.feature.store.execution.v1.jobs.FeaturesetJobsSummary\"K\n\x15\x46\x65\x61turesetJobsSummary\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x1b\n\x13total_affected_rows\x18\x02 \x01(\x03\x32\x9e\t\n\nJobService\x12\x8b\x01\n\x0e\x41pplyJobRecord\x12;.qwak.feature.store.execution.v1.jobs.ApplyJobRecordRequest\x1a<.qwak.feature.store.execution.v1.jobs.ApplyJobRecordResponse\x12\x8b\x01\n\x0eInitPagination\x12;.qwak.feature.store.execution.v1.jobs.InitPaginationRequest\x1a<.qwak.feature.store.execution.v1.jobs.InitPaginationResponse\x12y\n\x08ListJobs\x12\x35.qwak.feature.store.execution.v1.jobs.ListJobsRequest\x1a\x36.qwak.feature.store.execution.v1.jobs.ListJobsResponse\x12\x9d\x01\n\x14\x44\x65leteFeaturesetJobs\x12\x41.qwak.feature.store.execution.v1.jobs.DeleteFeaturesetJobsRequest\x1a\x42.qwak.feature.store.execution.v1.jobs.DeleteFeaturesetJobsResponse\x12\xcd\x01\n$GetLatestSuccessfulJobByFeaturesetId\x12Q.qwak.feature.store.execution.v1.jobs.GetLatestSuccessfulJobByFeaturesetIdRequest\x1aR.qwak.feature.store.execution.v1.jobs.GetLatestSuccessfulJobByFeaturesetIdResponse\x12\xcd\x01\n$GetAllFeaturesetLatestSuccessfulJobs\x12Q.qwak.feature.store.execution.v1.jobs.GetAllFeaturesetLatestSuccessfulJobsRequest\x1aR.qwak.feature.store.execution.v1.jobs.GetAllFeaturesetLatestSuccessfulJobsResponse\x12\xb8\x01\n\x1dGetAllFeaturesetJobsSummaries\x12J.qwak.feature.store.execution.v1.jobs.GetAllFeaturesetJobsSummariesRequest\x1aK.qwak.feature.store.execution.v1.jobs.GetAllFeaturesetJobsSummariesResponseBG\n*com.qwak.ai.features.execution.api.v1.jobsP\x01Z\x17qwak/fsexecution;fsjobsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(qwak/execution/v1/jobs/job_service.proto\x12$qwak.feature.store.execution.v1.jobs\x1a\x1fgoogle/protobuf/timestamp.proto\x1a qwak/execution/v1/jobs/job.proto\"\\\n\x15\x41pplyJobRecordRequest\x12\x43\n\njob_record\x18\x01 \x01(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecord\"\x18\n\x16\x41pplyJobRecordResponse\".\n\x15InitPaginationRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\"E\n\x16InitPaginationResponse\x12\x14\n\x0crecord_count\x18\x01 \x01(\x03\x12\x15\n\rmax_record_id\x18\x02 \x01(\x03\"g\n\x0fListJobsRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x13\n\x0bpage_number\x18\x03 \x01(\x05\x12\x15\n\rmax_record_id\x18\x04 \x01(\x03\"X\n\x10ListJobsResponse\x12\x44\n\x0bjob_records\x18\x01 \x03(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecord\":\n\"InitPaginationByExecutionIdRequest\x12\x14\n\x0c\x65xecution_id\x18\x01 \x01(\t\"R\n#InitPaginationByExecutionIdResponse\x12\x14\n\x0crecord_count\x18\x01 \x01(\x03\x12\x15\n\rmax_record_id\x18\x02 \x01(\x03\"s\n\x1cListJobsByExecutionIdRequest\x12\x14\n\x0c\x65xecution_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x13\n\x0bpage_number\x18\x03 \x01(\x05\x12\x15\n\rmax_record_id\x18\x04 \x01(\x03\"e\n\x1dListJobsByExecutionIdResponse\x12\x44\n\x0bjob_records\x18\x01 \x03(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecord\"4\n\x1b\x44\x65leteFeaturesetJobsRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\"@\n\x1c\x44\x65leteFeaturesetJobsResponse\x12 \n\x18\x64\x65leted_job_record_count\x18\x01 \x01(\x03\"D\n+GetLatestSuccessfulJobByFeaturesetIdRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\"\x88\x01\n,GetLatestSuccessfulJobByFeaturesetIdResponse\x12\x45\n\njob_record\x18\x01 \x01(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecordH\x00\x42\x11\n\x0fjob_record_resp\"-\n+GetAllFeaturesetLatestSuccessfulJobsRequest\"t\n,GetAllFeaturesetLatestSuccessfulJobsResponse\x12\x44\n\x0bjob_records\x18\x01 \x03(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecord\"\xa3\x01\n$GetAllFeaturesetJobsSummariesRequest\x12\x34\n\x10lower_time_bound\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x10upper_time_bound\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x42\r\n\x0bupper_bound\"|\n%GetAllFeaturesetJobsSummariesResponse\x12S\n\x0ejobs_summaries\x18\x01 \x03(\x0b\x32;.qwak.feature.store.execution.v1.jobs.FeaturesetJobsSummary\"K\n\x15\x46\x65\x61turesetJobsSummary\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x1b\n\x13total_affected_rows\x18\x02 \x01(\x03\":\n\"GetJobsSummaryByExecutionIdRequest\x12\x14\n\x0c\x65xecution_id\x18\x01 \x01(\t\"\x80\x02\n#GetJobsSummaryByExecutionIdResponse\x12\x14\n\x0c\x65xecution_id\x18\x01 \x01(\t\x12\x11\n\tjob_count\x18\x02 \x01(\x03\x12\x1b\n\x13total_affected_rows\x18\x03 \x01(\x03\x12I\n\x10\x66irst_job_record\x18\x04 \x01(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecord\x12H\n\x0flast_job_record\x18\x05 \x01(\x0b\x32/.qwak.feature.store.execution.v1.jobs.JobRecord2\xab\r\n\nJobService\x12\x8b\x01\n\x0e\x41pplyJobRecord\x12;.qwak.feature.store.execution.v1.jobs.ApplyJobRecordRequest\x1a<.qwak.feature.store.execution.v1.jobs.ApplyJobRecordResponse\x12\x8b\x01\n\x0eInitPagination\x12;.qwak.feature.store.execution.v1.jobs.InitPaginationRequest\x1a<.qwak.feature.store.execution.v1.jobs.InitPaginationResponse\x12y\n\x08ListJobs\x12\x35.qwak.feature.store.execution.v1.jobs.ListJobsRequest\x1a\x36.qwak.feature.store.execution.v1.jobs.ListJobsResponse\x12\xb2\x01\n\x1bInitPaginationByExecutionId\x12H.qwak.feature.store.execution.v1.jobs.InitPaginationByExecutionIdRequest\x1aI.qwak.feature.store.execution.v1.jobs.InitPaginationByExecutionIdResponse\x12\xa0\x01\n\x15ListJobsByExecutionId\x12\x42.qwak.feature.store.execution.v1.jobs.ListJobsByExecutionIdRequest\x1a\x43.qwak.feature.store.execution.v1.jobs.ListJobsByExecutionIdResponse\x12\x9d\x01\n\x14\x44\x65leteFeaturesetJobs\x12\x41.qwak.feature.store.execution.v1.jobs.DeleteFeaturesetJobsRequest\x1a\x42.qwak.feature.store.execution.v1.jobs.DeleteFeaturesetJobsResponse\x12\xcd\x01\n$GetLatestSuccessfulJobByFeaturesetId\x12Q.qwak.feature.store.execution.v1.jobs.GetLatestSuccessfulJobByFeaturesetIdRequest\x1aR.qwak.feature.store.execution.v1.jobs.GetLatestSuccessfulJobByFeaturesetIdResponse\x12\xcd\x01\n$GetAllFeaturesetLatestSuccessfulJobs\x12Q.qwak.feature.store.execution.v1.jobs.GetAllFeaturesetLatestSuccessfulJobsRequest\x1aR.qwak.feature.store.execution.v1.jobs.GetAllFeaturesetLatestSuccessfulJobsResponse\x12\xb8\x01\n\x1dGetAllFeaturesetJobsSummaries\x12J.qwak.feature.store.execution.v1.jobs.GetAllFeaturesetJobsSummariesRequest\x1aK.qwak.feature.store.execution.v1.jobs.GetAllFeaturesetJobsSummariesResponse\x12\xb2\x01\n\x1bGetJobsSummaryByExecutionId\x12H.qwak.feature.store.execution.v1.jobs.GetJobsSummaryByExecutionIdRequest\x1aI.qwak.feature.store.execution.v1.jobs.GetJobsSummaryByExecutionIdResponseBG\n*com.qwak.ai.features.execution.api.v1.jobsP\x01Z\x17qwak/fsexecution;fsjobsb\x06proto3')
 
 
 
 _APPLYJOBRECORDREQUEST = DESCRIPTOR.message_types_by_name['ApplyJobRecordRequest']
 _APPLYJOBRECORDRESPONSE = DESCRIPTOR.message_types_by_name['ApplyJobRecordResponse']
 _INITPAGINATIONREQUEST = DESCRIPTOR.message_types_by_name['InitPaginationRequest']
 _INITPAGINATIONRESPONSE = DESCRIPTOR.message_types_by_name['InitPaginationResponse']
 _LISTJOBSREQUEST = DESCRIPTOR.message_types_by_name['ListJobsRequest']
 _LISTJOBSRESPONSE = DESCRIPTOR.message_types_by_name['ListJobsResponse']
+_INITPAGINATIONBYEXECUTIONIDREQUEST = DESCRIPTOR.message_types_by_name['InitPaginationByExecutionIdRequest']
+_INITPAGINATIONBYEXECUTIONIDRESPONSE = DESCRIPTOR.message_types_by_name['InitPaginationByExecutionIdResponse']
+_LISTJOBSBYEXECUTIONIDREQUEST = DESCRIPTOR.message_types_by_name['ListJobsByExecutionIdRequest']
+_LISTJOBSBYEXECUTIONIDRESPONSE = DESCRIPTOR.message_types_by_name['ListJobsByExecutionIdResponse']
 _DELETEFEATURESETJOBSREQUEST = DESCRIPTOR.message_types_by_name['DeleteFeaturesetJobsRequest']
 _DELETEFEATURESETJOBSRESPONSE = DESCRIPTOR.message_types_by_name['DeleteFeaturesetJobsResponse']
 _GETLATESTSUCCESSFULJOBBYFEATURESETIDREQUEST = DESCRIPTOR.message_types_by_name['GetLatestSuccessfulJobByFeaturesetIdRequest']
 _GETLATESTSUCCESSFULJOBBYFEATURESETIDRESPONSE = DESCRIPTOR.message_types_by_name['GetLatestSuccessfulJobByFeaturesetIdResponse']
 _GETALLFEATURESETLATESTSUCCESSFULJOBSREQUEST = DESCRIPTOR.message_types_by_name['GetAllFeaturesetLatestSuccessfulJobsRequest']
 _GETALLFEATURESETLATESTSUCCESSFULJOBSRESPONSE = DESCRIPTOR.message_types_by_name['GetAllFeaturesetLatestSuccessfulJobsResponse']
 _GETALLFEATURESETJOBSSUMMARIESREQUEST = DESCRIPTOR.message_types_by_name['GetAllFeaturesetJobsSummariesRequest']
 _GETALLFEATURESETJOBSSUMMARIESRESPONSE = DESCRIPTOR.message_types_by_name['GetAllFeaturesetJobsSummariesResponse']
 _FEATURESETJOBSSUMMARY = DESCRIPTOR.message_types_by_name['FeaturesetJobsSummary']
+_GETJOBSSUMMARYBYEXECUTIONIDREQUEST = DESCRIPTOR.message_types_by_name['GetJobsSummaryByExecutionIdRequest']
+_GETJOBSSUMMARYBYEXECUTIONIDRESPONSE = DESCRIPTOR.message_types_by_name['GetJobsSummaryByExecutionIdResponse']
 ApplyJobRecordRequest = _reflection.GeneratedProtocolMessageType('ApplyJobRecordRequest', (_message.Message,), {
   'DESCRIPTOR' : _APPLYJOBRECORDREQUEST,
   '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.ApplyJobRecordRequest)
   })
 _sym_db.RegisterMessage(ApplyJobRecordRequest)
 
@@ -73,14 +79,42 @@
 ListJobsResponse = _reflection.GeneratedProtocolMessageType('ListJobsResponse', (_message.Message,), {
   'DESCRIPTOR' : _LISTJOBSRESPONSE,
   '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.ListJobsResponse)
   })
 _sym_db.RegisterMessage(ListJobsResponse)
 
+InitPaginationByExecutionIdRequest = _reflection.GeneratedProtocolMessageType('InitPaginationByExecutionIdRequest', (_message.Message,), {
+  'DESCRIPTOR' : _INITPAGINATIONBYEXECUTIONIDREQUEST,
+  '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.InitPaginationByExecutionIdRequest)
+  })
+_sym_db.RegisterMessage(InitPaginationByExecutionIdRequest)
+
+InitPaginationByExecutionIdResponse = _reflection.GeneratedProtocolMessageType('InitPaginationByExecutionIdResponse', (_message.Message,), {
+  'DESCRIPTOR' : _INITPAGINATIONBYEXECUTIONIDRESPONSE,
+  '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.InitPaginationByExecutionIdResponse)
+  })
+_sym_db.RegisterMessage(InitPaginationByExecutionIdResponse)
+
+ListJobsByExecutionIdRequest = _reflection.GeneratedProtocolMessageType('ListJobsByExecutionIdRequest', (_message.Message,), {
+  'DESCRIPTOR' : _LISTJOBSBYEXECUTIONIDREQUEST,
+  '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.ListJobsByExecutionIdRequest)
+  })
+_sym_db.RegisterMessage(ListJobsByExecutionIdRequest)
+
+ListJobsByExecutionIdResponse = _reflection.GeneratedProtocolMessageType('ListJobsByExecutionIdResponse', (_message.Message,), {
+  'DESCRIPTOR' : _LISTJOBSBYEXECUTIONIDRESPONSE,
+  '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.ListJobsByExecutionIdResponse)
+  })
+_sym_db.RegisterMessage(ListJobsByExecutionIdResponse)
+
 DeleteFeaturesetJobsRequest = _reflection.GeneratedProtocolMessageType('DeleteFeaturesetJobsRequest', (_message.Message,), {
   'DESCRIPTOR' : _DELETEFEATURESETJOBSREQUEST,
   '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.DeleteFeaturesetJobsRequest)
   })
 _sym_db.RegisterMessage(DeleteFeaturesetJobsRequest)
 
@@ -136,14 +170,28 @@
 FeaturesetJobsSummary = _reflection.GeneratedProtocolMessageType('FeaturesetJobsSummary', (_message.Message,), {
   'DESCRIPTOR' : _FEATURESETJOBSSUMMARY,
   '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.FeaturesetJobsSummary)
   })
 _sym_db.RegisterMessage(FeaturesetJobsSummary)
 
+GetJobsSummaryByExecutionIdRequest = _reflection.GeneratedProtocolMessageType('GetJobsSummaryByExecutionIdRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETJOBSSUMMARYBYEXECUTIONIDREQUEST,
+  '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.GetJobsSummaryByExecutionIdRequest)
+  })
+_sym_db.RegisterMessage(GetJobsSummaryByExecutionIdRequest)
+
+GetJobsSummaryByExecutionIdResponse = _reflection.GeneratedProtocolMessageType('GetJobsSummaryByExecutionIdResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETJOBSSUMMARYBYEXECUTIONIDRESPONSE,
+  '__module__' : 'qwak.execution.v1.jobs.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.execution.v1.jobs.GetJobsSummaryByExecutionIdResponse)
+  })
+_sym_db.RegisterMessage(GetJobsSummaryByExecutionIdResponse)
+
 _JOBSERVICE = DESCRIPTOR.services_by_name['JobService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n*com.qwak.ai.features.execution.api.v1.jobsP\001Z\027qwak/fsexecution;fsjobs'
   _APPLYJOBRECORDREQUEST._serialized_start=149
   _APPLYJOBRECORDREQUEST._serialized_end=241
@@ -153,28 +201,40 @@
   _INITPAGINATIONREQUEST._serialized_end=315
   _INITPAGINATIONRESPONSE._serialized_start=317
   _INITPAGINATIONRESPONSE._serialized_end=386
   _LISTJOBSREQUEST._serialized_start=388
   _LISTJOBSREQUEST._serialized_end=491
   _LISTJOBSRESPONSE._serialized_start=493
   _LISTJOBSRESPONSE._serialized_end=581
-  _DELETEFEATURESETJOBSREQUEST._serialized_start=583
-  _DELETEFEATURESETJOBSREQUEST._serialized_end=635
-  _DELETEFEATURESETJOBSRESPONSE._serialized_start=637
-  _DELETEFEATURESETJOBSRESPONSE._serialized_end=701
-  _GETLATESTSUCCESSFULJOBBYFEATURESETIDREQUEST._serialized_start=703
-  _GETLATESTSUCCESSFULJOBBYFEATURESETIDREQUEST._serialized_end=771
-  _GETLATESTSUCCESSFULJOBBYFEATURESETIDRESPONSE._serialized_start=774
-  _GETLATESTSUCCESSFULJOBBYFEATURESETIDRESPONSE._serialized_end=910
-  _GETALLFEATURESETLATESTSUCCESSFULJOBSREQUEST._serialized_start=912
-  _GETALLFEATURESETLATESTSUCCESSFULJOBSREQUEST._serialized_end=957
-  _GETALLFEATURESETLATESTSUCCESSFULJOBSRESPONSE._serialized_start=959
-  _GETALLFEATURESETLATESTSUCCESSFULJOBSRESPONSE._serialized_end=1075
-  _GETALLFEATURESETJOBSSUMMARIESREQUEST._serialized_start=1078
-  _GETALLFEATURESETJOBSSUMMARIESREQUEST._serialized_end=1241
-  _GETALLFEATURESETJOBSSUMMARIESRESPONSE._serialized_start=1243
-  _GETALLFEATURESETJOBSSUMMARIESRESPONSE._serialized_end=1367
-  _FEATURESETJOBSSUMMARY._serialized_start=1369
-  _FEATURESETJOBSSUMMARY._serialized_end=1444
-  _JOBSERVICE._serialized_start=1447
-  _JOBSERVICE._serialized_end=2629
+  _INITPAGINATIONBYEXECUTIONIDREQUEST._serialized_start=583
+  _INITPAGINATIONBYEXECUTIONIDREQUEST._serialized_end=641
+  _INITPAGINATIONBYEXECUTIONIDRESPONSE._serialized_start=643
+  _INITPAGINATIONBYEXECUTIONIDRESPONSE._serialized_end=725
+  _LISTJOBSBYEXECUTIONIDREQUEST._serialized_start=727
+  _LISTJOBSBYEXECUTIONIDREQUEST._serialized_end=842
+  _LISTJOBSBYEXECUTIONIDRESPONSE._serialized_start=844
+  _LISTJOBSBYEXECUTIONIDRESPONSE._serialized_end=945
+  _DELETEFEATURESETJOBSREQUEST._serialized_start=947
+  _DELETEFEATURESETJOBSREQUEST._serialized_end=999
+  _DELETEFEATURESETJOBSRESPONSE._serialized_start=1001
+  _DELETEFEATURESETJOBSRESPONSE._serialized_end=1065
+  _GETLATESTSUCCESSFULJOBBYFEATURESETIDREQUEST._serialized_start=1067
+  _GETLATESTSUCCESSFULJOBBYFEATURESETIDREQUEST._serialized_end=1135
+  _GETLATESTSUCCESSFULJOBBYFEATURESETIDRESPONSE._serialized_start=1138
+  _GETLATESTSUCCESSFULJOBBYFEATURESETIDRESPONSE._serialized_end=1274
+  _GETALLFEATURESETLATESTSUCCESSFULJOBSREQUEST._serialized_start=1276
+  _GETALLFEATURESETLATESTSUCCESSFULJOBSREQUEST._serialized_end=1321
+  _GETALLFEATURESETLATESTSUCCESSFULJOBSRESPONSE._serialized_start=1323
+  _GETALLFEATURESETLATESTSUCCESSFULJOBSRESPONSE._serialized_end=1439
+  _GETALLFEATURESETJOBSSUMMARIESREQUEST._serialized_start=1442
+  _GETALLFEATURESETJOBSSUMMARIESREQUEST._serialized_end=1605
+  _GETALLFEATURESETJOBSSUMMARIESRESPONSE._serialized_start=1607
+  _GETALLFEATURESETJOBSSUMMARIESRESPONSE._serialized_end=1731
+  _FEATURESETJOBSSUMMARY._serialized_start=1733
+  _FEATURESETJOBSSUMMARY._serialized_end=1808
+  _GETJOBSSUMMARYBYEXECUTIONIDREQUEST._serialized_start=1810
+  _GETJOBSSUMMARYBYEXECUTIONIDREQUEST._serialized_end=1868
+  _GETJOBSSUMMARYBYEXECUTIONIDRESPONSE._serialized_start=1871
+  _GETJOBSSUMMARYBYEXECUTIONIDRESPONSE._serialized_end=2127
+  _JOBSERVICE._serialized_start=2130
+  _JOBSERVICE._serialized_end=3837
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -4,271 +4,346 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
-import qwak.execution.v1.jobs.job_pb2
+import qwak.feature_store.jobs.v1.job_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class ApplyJobRecordRequest(google.protobuf.message.Message):
+class DeleteFeaturesetJobByJobIdRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    FEATURESET_ID_FIELD_NUMBER: builtins.int
+    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
+    JOB_ID_FIELD_NUMBER: builtins.int
+    featureset_id: builtins.str
+    """Featureset id"""
+    environment_id: builtins.str
+    """Environment id"""
+    job_id: builtins.str
+    """Job id"""
+    def __init__(
+        self,
+        *,
+        featureset_id: builtins.str = ...,
+        environment_id: builtins.str = ...,
+        job_id: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id", "job_id", b"job_id"]) -> None: ...
+
+global___DeleteFeaturesetJobByJobIdRequest = DeleteFeaturesetJobByJobIdRequest
+
+class DeleteFeaturesetJobByJobIdResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DELETED_JOB_RECORD_COUNT_FIELD_NUMBER: builtins.int
+    deleted_job_record_count: builtins.int
+    def __init__(
+        self,
+        *,
+        deleted_job_record_count: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["deleted_job_record_count", b"deleted_job_record_count"]) -> None: ...
+
+global___DeleteFeaturesetJobByJobIdResponse = DeleteFeaturesetJobByJobIdResponse
+
+class ApplyJobRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_RECORD_FIELD_NUMBER: builtins.int
     @property
-    def job_record(self) -> qwak.execution.v1.jobs.job_pb2.JobRecord:
-        """a Job Record to create or replace"""
+    def job_record(self) -> qwak.feature_store.jobs.v1.job_pb2.JobRecord:
+        """The job record to register"""
     def __init__(
         self,
         *,
-        job_record: qwak.execution.v1.jobs.job_pb2.JobRecord | None = ...,
+        job_record: qwak.feature_store.jobs.v1.job_pb2.JobRecord | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["job_record", b"job_record"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_record", b"job_record"]) -> None: ...
 
-global___ApplyJobRecordRequest = ApplyJobRecordRequest
+global___ApplyJobRequest = ApplyJobRequest
 
-class ApplyJobRecordResponse(google.protobuf.message.Message):
+class ApplyJobResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    JOB_RUNNING_ID_FIELD_NUMBER: builtins.int
+    JOB_ID_FIELD_NUMBER: builtins.int
+    job_running_id: builtins.int
+    """Job running id"""
+    job_id: builtins.str
+    """Job Id"""
     def __init__(
         self,
+        *,
+        job_running_id: builtins.int = ...,
+        job_id: builtins.str = ...,
     ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["job_id", b"job_id", "job_running_id", b"job_running_id"]) -> None: ...
 
-global___ApplyJobRecordResponse = ApplyJobRecordResponse
+global___ApplyJobResponse = ApplyJobResponse
 
 class InitPaginationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FEATURESET_ID_FIELD_NUMBER: builtins.int
+    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
     featureset_id: builtins.str
-    """the featureset id for which to start a pagination"""
+    """The featureset id of the requested job records"""
+    environment_id: builtins.str
+    """Environment id"""
     def __init__(
         self,
         *,
         featureset_id: builtins.str = ...,
+        environment_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id"]) -> None: ...
 
 global___InitPaginationRequest = InitPaginationRequest
 
 class InitPaginationResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RECORD_COUNT_FIELD_NUMBER: builtins.int
-    MAX_RECORD_ID_FIELD_NUMBER: builtins.int
+    PAGINATION_SESSION_MAX_ID_FIELD_NUMBER: builtins.int
     record_count: builtins.int
-    """Number of records found for this Featureset at the time of querying
-    this is used mainly by the client to plan things like number of pages etc.
-    """
-    max_record_id: builtins.int
-    """the current highest record id for this FS. this is the anchor
-    to use on subsequent requests if the caller wants to achieve
-    a view of a static list
-    """
+    """The amount of records that exist for this pagination session (current total amount of records for the featureset)"""
+    pagination_session_max_id: builtins.int
+    """The record to use for the max pagination sessions id in the ListJobs request"""
     def __init__(
         self,
         *,
         record_count: builtins.int = ...,
-        max_record_id: builtins.int = ...,
+        pagination_session_max_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_record_id", b"max_record_id", "record_count", b"record_count"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pagination_session_max_id", b"pagination_session_max_id", "record_count", b"record_count"]) -> None: ...
 
 global___InitPaginationResponse = InitPaginationResponse
 
 class ListJobsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FEATURESET_ID_FIELD_NUMBER: builtins.int
+    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     PAGE_NUMBER_FIELD_NUMBER: builtins.int
-    MAX_RECORD_ID_FIELD_NUMBER: builtins.int
+    PAGINATION_SESSION_MAX_ID_FIELD_NUMBER: builtins.int
     featureset_id: builtins.str
-    """featureset id"""
+    """The featureset id of the requested job records"""
+    environment_id: builtins.str
+    """Environment id"""
     page_size: builtins.int
-    """The page size to use for the response - the number of results in the response
-    is the minimum of the page_size and number of matching rows.
-    - a negative value means all results will be returned (in that case page_number is ignored)
-    """
+    """The amount of records to send in the result set"""
     page_number: builtins.int
-    """The page number to use"""
-    max_record_id: builtins.int
-    """The max record id to use as anchor - this is the value returned from InitPagination"""
+    """The page number to get"""
+    pagination_session_max_id: builtins.int
+    """The max session record id from which we retrieve the data, if unset (defaults to 0) we return the first records"""
     def __init__(
         self,
         *,
         featureset_id: builtins.str = ...,
+        environment_id: builtins.str = ...,
         page_size: builtins.int = ...,
         page_number: builtins.int = ...,
-        max_record_id: builtins.int = ...,
+        pagination_session_max_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id", "max_record_id", b"max_record_id", "page_number", b"page_number", "page_size", b"page_size"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id", "page_number", b"page_number", "page_size", b"page_size", "pagination_session_max_id", b"pagination_session_max_id"]) -> None: ...
 
 global___ListJobsRequest = ListJobsRequest
 
 class ListJobsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOB_RECORDS_FIELD_NUMBER: builtins.int
+    JOBS_FIELD_NUMBER: builtins.int
     @property
-    def job_records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.execution.v1.jobs.job_pb2.JobRecord]:
-        """All rows, sorted by the job record start time (event time)"""
+    def jobs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.feature_store.jobs.v1.job_pb2.JobRecord]:
+        """Result set of the requested jobs"""
     def __init__(
         self,
         *,
-        job_records: collections.abc.Iterable[qwak.execution.v1.jobs.job_pb2.JobRecord] | None = ...,
+        jobs: collections.abc.Iterable[qwak.feature_store.jobs.v1.job_pb2.JobRecord] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["job_records", b"job_records"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["jobs", b"jobs"]) -> None: ...
 
 global___ListJobsResponse = ListJobsResponse
 
-class DeleteFeaturesetJobsRequest(google.protobuf.message.Message):
+class GetLatestSuccessfulJobRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FEATURESET_ID_FIELD_NUMBER: builtins.int
+    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
     featureset_id: builtins.str
-    """The featureset id"""
+    """The featureset id of the requested latest successful job record"""
+    environment_id: builtins.str
+    """The jobs' environment id"""
     def __init__(
         self,
         *,
         featureset_id: builtins.str = ...,
+        environment_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id"]) -> None: ...
 
-global___DeleteFeaturesetJobsRequest = DeleteFeaturesetJobsRequest
+global___GetLatestSuccessfulJobRequest = GetLatestSuccessfulJobRequest
 
-class DeleteFeaturesetJobsResponse(google.protobuf.message.Message):
+class GetLatestJobRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DELETED_JOB_RECORD_COUNT_FIELD_NUMBER: builtins.int
-    deleted_job_record_count: builtins.int
+    FEATURESET_ID_FIELD_NUMBER: builtins.int
+    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
+    featureset_id: builtins.str
+    """The featureset id of the requested latest job record running"""
+    environment_id: builtins.str
+    """The jobs' environment id"""
     def __init__(
         self,
         *,
-        deleted_job_record_count: builtins.int = ...,
+        featureset_id: builtins.str = ...,
+        environment_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["deleted_job_record_count", b"deleted_job_record_count"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id"]) -> None: ...
 
-global___DeleteFeaturesetJobsResponse = DeleteFeaturesetJobsResponse
+global___GetLatestJobRequest = GetLatestJobRequest
 
-class GetLatestSuccessfulJobByFeaturesetIdRequest(google.protobuf.message.Message):
+class GetLatestJobResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    FEATURESET_ID_FIELD_NUMBER: builtins.int
-    featureset_id: builtins.str
+    JOB_FIELD_NUMBER: builtins.int
+    @property
+    def job(self) -> qwak.feature_store.jobs.v1.job_pb2.JobRecord:
+        """the requested job"""
     def __init__(
         self,
         *,
-        featureset_id: builtins.str = ...,
+        job: qwak.feature_store.jobs.v1.job_pb2.JobRecord | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["job", b"job"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["job", b"job"]) -> None: ...
 
-global___GetLatestSuccessfulJobByFeaturesetIdRequest = GetLatestSuccessfulJobByFeaturesetIdRequest
+global___GetLatestJobResponse = GetLatestJobResponse
 
-class GetLatestSuccessfulJobByFeaturesetIdResponse(google.protobuf.message.Message):
+class GetLatestSuccessfulJobResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOB_RECORD_FIELD_NUMBER: builtins.int
+    JOB_FIELD_NUMBER: builtins.int
+    FOUND_FIELD_NUMBER: builtins.int
     @property
-    def job_record(self) -> qwak.execution.v1.jobs.job_pb2.JobRecord: ...
+    def job(self) -> qwak.feature_store.jobs.v1.job_pb2.JobRecord:
+        """the requested job"""
+    found: builtins.bool
+    """is the job empty or not"""
     def __init__(
         self,
         *,
-        job_record: qwak.execution.v1.jobs.job_pb2.JobRecord | None = ...,
+        job: qwak.feature_store.jobs.v1.job_pb2.JobRecord | None = ...,
+        found: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["job_record", b"job_record", "job_record_resp", b"job_record_resp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["job_record", b"job_record", "job_record_resp", b"job_record_resp"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["job_record_resp", b"job_record_resp"]) -> typing_extensions.Literal["job_record"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["job", b"job"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["found", b"found", "job", b"job"]) -> None: ...
 
-global___GetLatestSuccessfulJobByFeaturesetIdResponse = GetLatestSuccessfulJobByFeaturesetIdResponse
+global___GetLatestSuccessfulJobResponse = GetLatestSuccessfulJobResponse
 
-class GetAllFeaturesetLatestSuccessfulJobsRequest(google.protobuf.message.Message):
+class GetAllLatestSuccessfulJobsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
-global___GetAllFeaturesetLatestSuccessfulJobsRequest = GetAllFeaturesetLatestSuccessfulJobsRequest
+global___GetAllLatestSuccessfulJobsRequest = GetAllLatestSuccessfulJobsRequest
 
-class GetAllFeaturesetLatestSuccessfulJobsResponse(google.protobuf.message.Message):
+class GetAllLatestSuccessfulJobsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOB_RECORDS_FIELD_NUMBER: builtins.int
+    JOBS_FIELD_NUMBER: builtins.int
     @property
-    def job_records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.execution.v1.jobs.job_pb2.JobRecord]:
+    def jobs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.feature_store.jobs.v1.job_pb2.JobRecord]:
         """all latest requested jobs"""
     def __init__(
         self,
         *,
-        job_records: collections.abc.Iterable[qwak.execution.v1.jobs.job_pb2.JobRecord] | None = ...,
+        jobs: collections.abc.Iterable[qwak.feature_store.jobs.v1.job_pb2.JobRecord] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["job_records", b"job_records"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["jobs", b"jobs"]) -> None: ...
 
-global___GetAllFeaturesetLatestSuccessfulJobsResponse = GetAllFeaturesetLatestSuccessfulJobsResponse
+global___GetAllLatestSuccessfulJobsResponse = GetAllLatestSuccessfulJobsResponse
 
-class GetAllFeaturesetJobsSummariesRequest(google.protobuf.message.Message):
+class DeleteFeaturesetJobsRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    FEATURESET_ID_FIELD_NUMBER: builtins.int
+    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
+    featureset_id: builtins.str
+    """The featureset id of the requested delete featureset jobs"""
+    environment_id: builtins.str
+    """Environment id"""
+    def __init__(
+        self,
+        *,
+        featureset_id: builtins.str = ...,
+        environment_id: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id"]) -> None: ...
+
+global___DeleteFeaturesetJobsRequest = DeleteFeaturesetJobsRequest
+
+class DeleteFeaturesetJobsResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DELETED_JOB_RECORDS_COUNT_FIELD_NUMBER: builtins.int
+    deleted_job_records_count: builtins.int
+    def __init__(
+        self,
+        *,
+        deleted_job_records_count: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["deleted_job_records_count", b"deleted_job_records_count"]) -> None: ...
+
+global___DeleteFeaturesetJobsResponse = DeleteFeaturesetJobsResponse
+
+class GetJobsSummariesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOWER_TIME_BOUND_FIELD_NUMBER: builtins.int
     UPPER_TIME_BOUND_FIELD_NUMBER: builtins.int
     @property
     def lower_time_bound(self) -> google.protobuf.timestamp_pb2.Timestamp:
-        """Summary lower time bound.
-        applied on processing start_time column.
-        """
+        """Summary lower time bound"""
     @property
     def upper_time_bound(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     def __init__(
         self,
         *,
         lower_time_bound: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         upper_time_bound: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["lower_time_bound", b"lower_time_bound", "upper_bound", b"upper_bound", "upper_time_bound", b"upper_time_bound"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["lower_time_bound", b"lower_time_bound", "upper_bound", b"upper_bound", "upper_time_bound", b"upper_time_bound"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["upper_bound", b"upper_bound"]) -> typing_extensions.Literal["upper_time_bound"] | None: ...
 
-global___GetAllFeaturesetJobsSummariesRequest = GetAllFeaturesetJobsSummariesRequest
+global___GetJobsSummariesRequest = GetJobsSummariesRequest
 
-class GetAllFeaturesetJobsSummariesResponse(google.protobuf.message.Message):
+class GetJobsSummariesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOBS_SUMMARIES_FIELD_NUMBER: builtins.int
     @property
-    def jobs_summaries(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___FeaturesetJobsSummary]:
+    def jobs_summaries(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.feature_store.jobs.v1.job_pb2.FeaturesetLevelJobsSummary]:
         """Job summaries per featureset for the entire environment"""
     def __init__(
         self,
         *,
-        jobs_summaries: collections.abc.Iterable[global___FeaturesetJobsSummary] | None = ...,
+        jobs_summaries: collections.abc.Iterable[qwak.feature_store.jobs.v1.job_pb2.FeaturesetLevelJobsSummary] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["jobs_summaries", b"jobs_summaries"]) -> None: ...
 
-global___GetAllFeaturesetJobsSummariesResponse = GetAllFeaturesetJobsSummariesResponse
-
-class FeaturesetJobsSummary(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    FEATURESET_ID_FIELD_NUMBER: builtins.int
-    TOTAL_AFFECTED_ROWS_FIELD_NUMBER: builtins.int
-    featureset_id: builtins.str
-    """Featureset Id"""
-    total_affected_rows: builtins.int
-    """Number of affected rows"""
-    def __init__(
-        self,
-        *,
-        featureset_id: builtins.str = ...,
-        total_affected_rows: builtins.int = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id", "total_affected_rows", b"total_affected_rows"]) -> None: ...
-
-global___FeaturesetJobsSummary = FeaturesetJobsSummary
+global___GetJobsSummariesResponse = GetJobsSummariesResponse
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,14 +25,24 @@
                 response_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.InitPaginationResponse.FromString,
                 )
         self.ListJobs = channel.unary_unary(
                 '/qwak.feature.store.execution.v1.jobs.JobService/ListJobs',
                 request_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsRequest.SerializeToString,
                 response_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsResponse.FromString,
                 )
+        self.InitPaginationByExecutionId = channel.unary_unary(
+                '/qwak.feature.store.execution.v1.jobs.JobService/InitPaginationByExecutionId',
+                request_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.InitPaginationByExecutionIdRequest.SerializeToString,
+                response_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.InitPaginationByExecutionIdResponse.FromString,
+                )
+        self.ListJobsByExecutionId = channel.unary_unary(
+                '/qwak.feature.store.execution.v1.jobs.JobService/ListJobsByExecutionId',
+                request_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsByExecutionIdRequest.SerializeToString,
+                response_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsByExecutionIdResponse.FromString,
+                )
         self.DeleteFeaturesetJobs = channel.unary_unary(
                 '/qwak.feature.store.execution.v1.jobs.JobService/DeleteFeaturesetJobs',
                 request_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.DeleteFeaturesetJobsRequest.SerializeToString,
                 response_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.DeleteFeaturesetJobsResponse.FromString,
                 )
         self.GetLatestSuccessfulJobByFeaturesetId = channel.unary_unary(
                 '/qwak.feature.store.execution.v1.jobs.JobService/GetLatestSuccessfulJobByFeaturesetId',
@@ -45,14 +55,19 @@
                 response_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetAllFeaturesetLatestSuccessfulJobsResponse.FromString,
                 )
         self.GetAllFeaturesetJobsSummaries = channel.unary_unary(
                 '/qwak.feature.store.execution.v1.jobs.JobService/GetAllFeaturesetJobsSummaries',
                 request_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetAllFeaturesetJobsSummariesRequest.SerializeToString,
                 response_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetAllFeaturesetJobsSummariesResponse.FromString,
                 )
+        self.GetJobsSummaryByExecutionId = channel.unary_unary(
+                '/qwak.feature.store.execution.v1.jobs.JobService/GetJobsSummaryByExecutionId',
+                request_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetJobsSummaryByExecutionIdRequest.SerializeToString,
+                response_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetJobsSummaryByExecutionIdResponse.FromString,
+                )
 
 
 class JobServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ApplyJobRecord(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -68,14 +83,26 @@
 
     def ListJobs(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def InitPaginationByExecutionId(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ListJobsByExecutionId(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def DeleteFeaturesetJobs(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetLatestSuccessfulJobByFeaturesetId(self, request, context):
@@ -92,14 +119,20 @@
 
     def GetAllFeaturesetJobsSummaries(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetJobsSummaryByExecutionId(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_JobServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ApplyJobRecord': grpc.unary_unary_rpc_method_handler(
                     servicer.ApplyJobRecord,
                     request_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ApplyJobRecordRequest.FromString,
                     response_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ApplyJobRecordResponse.SerializeToString,
@@ -110,14 +143,24 @@
                     response_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.InitPaginationResponse.SerializeToString,
             ),
             'ListJobs': grpc.unary_unary_rpc_method_handler(
                     servicer.ListJobs,
                     request_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsRequest.FromString,
                     response_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsResponse.SerializeToString,
             ),
+            'InitPaginationByExecutionId': grpc.unary_unary_rpc_method_handler(
+                    servicer.InitPaginationByExecutionId,
+                    request_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.InitPaginationByExecutionIdRequest.FromString,
+                    response_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.InitPaginationByExecutionIdResponse.SerializeToString,
+            ),
+            'ListJobsByExecutionId': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListJobsByExecutionId,
+                    request_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsByExecutionIdRequest.FromString,
+                    response_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsByExecutionIdResponse.SerializeToString,
+            ),
             'DeleteFeaturesetJobs': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteFeaturesetJobs,
                     request_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.DeleteFeaturesetJobsRequest.FromString,
                     response_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.DeleteFeaturesetJobsResponse.SerializeToString,
             ),
             'GetLatestSuccessfulJobByFeaturesetId': grpc.unary_unary_rpc_method_handler(
                     servicer.GetLatestSuccessfulJobByFeaturesetId,
@@ -130,14 +173,19 @@
                     response_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetAllFeaturesetLatestSuccessfulJobsResponse.SerializeToString,
             ),
             'GetAllFeaturesetJobsSummaries': grpc.unary_unary_rpc_method_handler(
                     servicer.GetAllFeaturesetJobsSummaries,
                     request_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetAllFeaturesetJobsSummariesRequest.FromString,
                     response_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetAllFeaturesetJobsSummariesResponse.SerializeToString,
             ),
+            'GetJobsSummaryByExecutionId': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetJobsSummaryByExecutionId,
+                    request_deserializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetJobsSummaryByExecutionIdRequest.FromString,
+                    response_serializer=qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetJobsSummaryByExecutionIdResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'qwak.feature.store.execution.v1.jobs.JobService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -192,14 +240,48 @@
         return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.jobs.JobService/ListJobs',
             qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsRequest.SerializeToString,
             qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def InitPaginationByExecutionId(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.jobs.JobService/InitPaginationByExecutionId',
+            qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.InitPaginationByExecutionIdRequest.SerializeToString,
+            qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.InitPaginationByExecutionIdResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListJobsByExecutionId(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.jobs.JobService/ListJobsByExecutionId',
+            qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsByExecutionIdRequest.SerializeToString,
+            qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.ListJobsByExecutionIdResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def DeleteFeaturesetJobs(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -258,7 +340,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.jobs.JobService/GetAllFeaturesetJobsSummaries',
             qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetAllFeaturesetJobsSummariesRequest.SerializeToString,
             qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetAllFeaturesetJobsSummariesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetJobsSummaryByExecutionId(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qwak.feature.store.execution.v1.jobs.JobService/GetJobsSummaryByExecutionId',
+            qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetJobsSummaryByExecutionIdRequest.SerializeToString,
+            qwak_dot_execution_dot_v1_dot_jobs_dot_job__service__pb2.GetJobsSummaryByExecutionIdResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -4,346 +4,399 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
-import qwak.feature_store.jobs.v1.job_pb2
+import qwak.execution.v1.jobs.job_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class DeleteFeaturesetJobByJobIdRequest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    FEATURESET_ID_FIELD_NUMBER: builtins.int
-    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
-    JOB_ID_FIELD_NUMBER: builtins.int
-    featureset_id: builtins.str
-    """Featureset id"""
-    environment_id: builtins.str
-    """Environment id"""
-    job_id: builtins.str
-    """Job id"""
-    def __init__(
-        self,
-        *,
-        featureset_id: builtins.str = ...,
-        environment_id: builtins.str = ...,
-        job_id: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id", "job_id", b"job_id"]) -> None: ...
-
-global___DeleteFeaturesetJobByJobIdRequest = DeleteFeaturesetJobByJobIdRequest
-
-class DeleteFeaturesetJobByJobIdResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    DELETED_JOB_RECORD_COUNT_FIELD_NUMBER: builtins.int
-    deleted_job_record_count: builtins.int
-    def __init__(
-        self,
-        *,
-        deleted_job_record_count: builtins.int = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["deleted_job_record_count", b"deleted_job_record_count"]) -> None: ...
-
-global___DeleteFeaturesetJobByJobIdResponse = DeleteFeaturesetJobByJobIdResponse
-
-class ApplyJobRequest(google.protobuf.message.Message):
+class ApplyJobRecordRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_RECORD_FIELD_NUMBER: builtins.int
     @property
-    def job_record(self) -> qwak.feature_store.jobs.v1.job_pb2.JobRecord:
-        """The job record to register"""
+    def job_record(self) -> qwak.execution.v1.jobs.job_pb2.JobRecord:
+        """a Job Record to create or replace"""
     def __init__(
         self,
         *,
-        job_record: qwak.feature_store.jobs.v1.job_pb2.JobRecord | None = ...,
+        job_record: qwak.execution.v1.jobs.job_pb2.JobRecord | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["job_record", b"job_record"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_record", b"job_record"]) -> None: ...
 
-global___ApplyJobRequest = ApplyJobRequest
+global___ApplyJobRecordRequest = ApplyJobRecordRequest
 
-class ApplyJobResponse(google.protobuf.message.Message):
+class ApplyJobRecordResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOB_RUNNING_ID_FIELD_NUMBER: builtins.int
-    JOB_ID_FIELD_NUMBER: builtins.int
-    job_running_id: builtins.int
-    """Job running id"""
-    job_id: builtins.str
-    """Job Id"""
     def __init__(
         self,
-        *,
-        job_running_id: builtins.int = ...,
-        job_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["job_id", b"job_id", "job_running_id", b"job_running_id"]) -> None: ...
 
-global___ApplyJobResponse = ApplyJobResponse
+global___ApplyJobRecordResponse = ApplyJobRecordResponse
 
 class InitPaginationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FEATURESET_ID_FIELD_NUMBER: builtins.int
-    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
     featureset_id: builtins.str
-    """The featureset id of the requested job records"""
-    environment_id: builtins.str
-    """Environment id"""
+    """the featureset id for which to start a pagination"""
     def __init__(
         self,
         *,
         featureset_id: builtins.str = ...,
-        environment_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id"]) -> None: ...
 
 global___InitPaginationRequest = InitPaginationRequest
 
 class InitPaginationResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RECORD_COUNT_FIELD_NUMBER: builtins.int
-    PAGINATION_SESSION_MAX_ID_FIELD_NUMBER: builtins.int
+    MAX_RECORD_ID_FIELD_NUMBER: builtins.int
     record_count: builtins.int
-    """The amount of records that exist for this pagination session (current total amount of records for the featureset)"""
-    pagination_session_max_id: builtins.int
-    """The record to use for the max pagination sessions id in the ListJobs request"""
+    """Number of records found for this Featureset at the time of querying
+    this is used mainly by the client to plan things like number of pages etc.
+    """
+    max_record_id: builtins.int
+    """the current highest record id for this FS. this is the anchor
+    to use on subsequent requests if the caller wants to achieve
+    a view of a static list
+    """
     def __init__(
         self,
         *,
         record_count: builtins.int = ...,
-        pagination_session_max_id: builtins.int = ...,
+        max_record_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pagination_session_max_id", b"pagination_session_max_id", "record_count", b"record_count"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["max_record_id", b"max_record_id", "record_count", b"record_count"]) -> None: ...
 
 global___InitPaginationResponse = InitPaginationResponse
 
 class ListJobsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FEATURESET_ID_FIELD_NUMBER: builtins.int
-    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     PAGE_NUMBER_FIELD_NUMBER: builtins.int
-    PAGINATION_SESSION_MAX_ID_FIELD_NUMBER: builtins.int
+    MAX_RECORD_ID_FIELD_NUMBER: builtins.int
     featureset_id: builtins.str
-    """The featureset id of the requested job records"""
-    environment_id: builtins.str
-    """Environment id"""
+    """featureset id"""
     page_size: builtins.int
-    """The amount of records to send in the result set"""
+    """The page size to use for the response - the number of results in the response
+    is the minimum of the page_size and number of matching rows.
+    - a negative value means all results will be returned (in that case page_number is ignored)
+    """
     page_number: builtins.int
-    """The page number to get"""
-    pagination_session_max_id: builtins.int
-    """The max session record id from which we retrieve the data, if unset (defaults to 0) we return the first records"""
+    """The page number to use"""
+    max_record_id: builtins.int
+    """The max record id to use as anchor - this is the value returned from InitPagination"""
     def __init__(
         self,
         *,
         featureset_id: builtins.str = ...,
-        environment_id: builtins.str = ...,
         page_size: builtins.int = ...,
         page_number: builtins.int = ...,
-        pagination_session_max_id: builtins.int = ...,
+        max_record_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id", "page_number", b"page_number", "page_size", b"page_size", "pagination_session_max_id", b"pagination_session_max_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id", "max_record_id", b"max_record_id", "page_number", b"page_number", "page_size", b"page_size"]) -> None: ...
 
 global___ListJobsRequest = ListJobsRequest
 
 class ListJobsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOBS_FIELD_NUMBER: builtins.int
+    JOB_RECORDS_FIELD_NUMBER: builtins.int
     @property
-    def jobs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.feature_store.jobs.v1.job_pb2.JobRecord]:
-        """Result set of the requested jobs"""
+    def job_records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.execution.v1.jobs.job_pb2.JobRecord]:
+        """All rows, sorted by the job record start time (event time)"""
     def __init__(
         self,
         *,
-        jobs: collections.abc.Iterable[qwak.feature_store.jobs.v1.job_pb2.JobRecord] | None = ...,
+        job_records: collections.abc.Iterable[qwak.execution.v1.jobs.job_pb2.JobRecord] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["jobs", b"jobs"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["job_records", b"job_records"]) -> None: ...
 
 global___ListJobsResponse = ListJobsResponse
 
-class GetLatestSuccessfulJobRequest(google.protobuf.message.Message):
+class InitPaginationByExecutionIdRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    FEATURESET_ID_FIELD_NUMBER: builtins.int
-    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
-    featureset_id: builtins.str
-    """The featureset id of the requested latest successful job record"""
-    environment_id: builtins.str
-    """The jobs' environment id"""
+    EXECUTION_ID_FIELD_NUMBER: builtins.int
+    execution_id: builtins.str
+    """the execution id"""
     def __init__(
         self,
         *,
-        featureset_id: builtins.str = ...,
-        environment_id: builtins.str = ...,
+        execution_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["execution_id", b"execution_id"]) -> None: ...
 
-global___GetLatestSuccessfulJobRequest = GetLatestSuccessfulJobRequest
+global___InitPaginationByExecutionIdRequest = InitPaginationByExecutionIdRequest
 
-class GetLatestJobRequest(google.protobuf.message.Message):
+class InitPaginationByExecutionIdResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    FEATURESET_ID_FIELD_NUMBER: builtins.int
-    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
-    featureset_id: builtins.str
-    """The featureset id of the requested latest job record running"""
-    environment_id: builtins.str
-    """The jobs' environment id"""
+    RECORD_COUNT_FIELD_NUMBER: builtins.int
+    MAX_RECORD_ID_FIELD_NUMBER: builtins.int
+    record_count: builtins.int
+    """Number of records found for this Featureset and execution at the time of querying.
+    this is used mainly by the client to plan things like number of pages etc.
+    """
+    max_record_id: builtins.int
+    """the current highest record id for this FS. this is the anchor
+    to use on subsequent requests if the caller wants to achieve
+    a view of a static list
+    """
     def __init__(
         self,
         *,
-        featureset_id: builtins.str = ...,
-        environment_id: builtins.str = ...,
+        record_count: builtins.int = ...,
+        max_record_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["max_record_id", b"max_record_id", "record_count", b"record_count"]) -> None: ...
 
-global___GetLatestJobRequest = GetLatestJobRequest
+global___InitPaginationByExecutionIdResponse = InitPaginationByExecutionIdResponse
 
-class GetLatestJobResponse(google.protobuf.message.Message):
+class ListJobsByExecutionIdRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOB_FIELD_NUMBER: builtins.int
-    @property
-    def job(self) -> qwak.feature_store.jobs.v1.job_pb2.JobRecord:
-        """the requested job"""
+    EXECUTION_ID_FIELD_NUMBER: builtins.int
+    PAGE_SIZE_FIELD_NUMBER: builtins.int
+    PAGE_NUMBER_FIELD_NUMBER: builtins.int
+    MAX_RECORD_ID_FIELD_NUMBER: builtins.int
+    execution_id: builtins.str
+    """execution id"""
+    page_size: builtins.int
+    """The page size to use for the response - the number of results in the response
+    is the minimum of the page_size and number of matching rows.
+    - a negative value means all results will be returned (in that case page_number is ignored)
+    """
+    page_number: builtins.int
+    """The page number to use"""
+    max_record_id: builtins.int
+    """The max record id to use as anchor - this is the value returned from InitPagination"""
     def __init__(
         self,
         *,
-        job: qwak.feature_store.jobs.v1.job_pb2.JobRecord | None = ...,
+        execution_id: builtins.str = ...,
+        page_size: builtins.int = ...,
+        page_number: builtins.int = ...,
+        max_record_id: builtins.int = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["job", b"job"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["job", b"job"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["execution_id", b"execution_id", "max_record_id", b"max_record_id", "page_number", b"page_number", "page_size", b"page_size"]) -> None: ...
 
-global___GetLatestJobResponse = GetLatestJobResponse
+global___ListJobsByExecutionIdRequest = ListJobsByExecutionIdRequest
 
-class GetLatestSuccessfulJobResponse(google.protobuf.message.Message):
+class ListJobsByExecutionIdResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOB_FIELD_NUMBER: builtins.int
-    FOUND_FIELD_NUMBER: builtins.int
+    JOB_RECORDS_FIELD_NUMBER: builtins.int
     @property
-    def job(self) -> qwak.feature_store.jobs.v1.job_pb2.JobRecord:
-        """the requested job"""
-    found: builtins.bool
-    """is the job empty or not"""
+    def job_records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.execution.v1.jobs.job_pb2.JobRecord]:
+        """All rows, sorted by the job record start time (event time)"""
     def __init__(
         self,
         *,
-        job: qwak.feature_store.jobs.v1.job_pb2.JobRecord | None = ...,
-        found: builtins.bool = ...,
+        job_records: collections.abc.Iterable[qwak.execution.v1.jobs.job_pb2.JobRecord] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["job", b"job"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["found", b"found", "job", b"job"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["job_records", b"job_records"]) -> None: ...
 
-global___GetLatestSuccessfulJobResponse = GetLatestSuccessfulJobResponse
+global___ListJobsByExecutionIdResponse = ListJobsByExecutionIdResponse
 
-class GetAllLatestSuccessfulJobsRequest(google.protobuf.message.Message):
+class DeleteFeaturesetJobsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    FEATURESET_ID_FIELD_NUMBER: builtins.int
+    featureset_id: builtins.str
+    """The featureset id"""
     def __init__(
         self,
+        *,
+        featureset_id: builtins.str = ...,
     ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id"]) -> None: ...
 
-global___GetAllLatestSuccessfulJobsRequest = GetAllLatestSuccessfulJobsRequest
+global___DeleteFeaturesetJobsRequest = DeleteFeaturesetJobsRequest
 
-class GetAllLatestSuccessfulJobsResponse(google.protobuf.message.Message):
+class DeleteFeaturesetJobsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOBS_FIELD_NUMBER: builtins.int
-    @property
-    def jobs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.feature_store.jobs.v1.job_pb2.JobRecord]:
-        """all latest requested jobs"""
+    DELETED_JOB_RECORD_COUNT_FIELD_NUMBER: builtins.int
+    deleted_job_record_count: builtins.int
     def __init__(
         self,
         *,
-        jobs: collections.abc.Iterable[qwak.feature_store.jobs.v1.job_pb2.JobRecord] | None = ...,
+        deleted_job_record_count: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["jobs", b"jobs"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["deleted_job_record_count", b"deleted_job_record_count"]) -> None: ...
 
-global___GetAllLatestSuccessfulJobsResponse = GetAllLatestSuccessfulJobsResponse
+global___DeleteFeaturesetJobsResponse = DeleteFeaturesetJobsResponse
 
-class DeleteFeaturesetJobsRequest(google.protobuf.message.Message):
+class GetLatestSuccessfulJobByFeaturesetIdRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FEATURESET_ID_FIELD_NUMBER: builtins.int
-    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
     featureset_id: builtins.str
-    """The featureset id of the requested delete featureset jobs"""
-    environment_id: builtins.str
-    """Environment id"""
     def __init__(
         self,
         *,
         featureset_id: builtins.str = ...,
-        environment_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["environment_id", b"environment_id", "featureset_id", b"featureset_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id"]) -> None: ...
 
-global___DeleteFeaturesetJobsRequest = DeleteFeaturesetJobsRequest
+global___GetLatestSuccessfulJobByFeaturesetIdRequest = GetLatestSuccessfulJobByFeaturesetIdRequest
 
-class DeleteFeaturesetJobsResponse(google.protobuf.message.Message):
+class GetLatestSuccessfulJobByFeaturesetIdResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DELETED_JOB_RECORDS_COUNT_FIELD_NUMBER: builtins.int
-    deleted_job_records_count: builtins.int
+    JOB_RECORD_FIELD_NUMBER: builtins.int
+    @property
+    def job_record(self) -> qwak.execution.v1.jobs.job_pb2.JobRecord: ...
     def __init__(
         self,
         *,
-        deleted_job_records_count: builtins.int = ...,
+        job_record: qwak.execution.v1.jobs.job_pb2.JobRecord | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["deleted_job_records_count", b"deleted_job_records_count"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["job_record", b"job_record", "job_record_resp", b"job_record_resp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["job_record", b"job_record", "job_record_resp", b"job_record_resp"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["job_record_resp", b"job_record_resp"]) -> typing_extensions.Literal["job_record"] | None: ...
 
-global___DeleteFeaturesetJobsResponse = DeleteFeaturesetJobsResponse
+global___GetLatestSuccessfulJobByFeaturesetIdResponse = GetLatestSuccessfulJobByFeaturesetIdResponse
+
+class GetAllFeaturesetLatestSuccessfulJobsRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___GetAllFeaturesetLatestSuccessfulJobsRequest = GetAllFeaturesetLatestSuccessfulJobsRequest
 
-class GetJobsSummariesRequest(google.protobuf.message.Message):
+class GetAllFeaturesetLatestSuccessfulJobsResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    JOB_RECORDS_FIELD_NUMBER: builtins.int
+    @property
+    def job_records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.execution.v1.jobs.job_pb2.JobRecord]:
+        """all latest requested jobs"""
+    def __init__(
+        self,
+        *,
+        job_records: collections.abc.Iterable[qwak.execution.v1.jobs.job_pb2.JobRecord] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["job_records", b"job_records"]) -> None: ...
+
+global___GetAllFeaturesetLatestSuccessfulJobsResponse = GetAllFeaturesetLatestSuccessfulJobsResponse
+
+class GetAllFeaturesetJobsSummariesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOWER_TIME_BOUND_FIELD_NUMBER: builtins.int
     UPPER_TIME_BOUND_FIELD_NUMBER: builtins.int
     @property
     def lower_time_bound(self) -> google.protobuf.timestamp_pb2.Timestamp:
-        """Summary lower time bound"""
+        """Summary lower time bound.
+        applied on processing start_time column.
+        """
     @property
     def upper_time_bound(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     def __init__(
         self,
         *,
         lower_time_bound: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         upper_time_bound: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["lower_time_bound", b"lower_time_bound", "upper_bound", b"upper_bound", "upper_time_bound", b"upper_time_bound"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["lower_time_bound", b"lower_time_bound", "upper_bound", b"upper_bound", "upper_time_bound", b"upper_time_bound"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["upper_bound", b"upper_bound"]) -> typing_extensions.Literal["upper_time_bound"] | None: ...
 
-global___GetJobsSummariesRequest = GetJobsSummariesRequest
+global___GetAllFeaturesetJobsSummariesRequest = GetAllFeaturesetJobsSummariesRequest
 
-class GetJobsSummariesResponse(google.protobuf.message.Message):
+class GetAllFeaturesetJobsSummariesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOBS_SUMMARIES_FIELD_NUMBER: builtins.int
     @property
-    def jobs_summaries(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.feature_store.jobs.v1.job_pb2.FeaturesetLevelJobsSummary]:
+    def jobs_summaries(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___FeaturesetJobsSummary]:
         """Job summaries per featureset for the entire environment"""
     def __init__(
         self,
         *,
-        jobs_summaries: collections.abc.Iterable[qwak.feature_store.jobs.v1.job_pb2.FeaturesetLevelJobsSummary] | None = ...,
+        jobs_summaries: collections.abc.Iterable[global___FeaturesetJobsSummary] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["jobs_summaries", b"jobs_summaries"]) -> None: ...
 
-global___GetJobsSummariesResponse = GetJobsSummariesResponse
+global___GetAllFeaturesetJobsSummariesResponse = GetAllFeaturesetJobsSummariesResponse
+
+class FeaturesetJobsSummary(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    FEATURESET_ID_FIELD_NUMBER: builtins.int
+    TOTAL_AFFECTED_ROWS_FIELD_NUMBER: builtins.int
+    featureset_id: builtins.str
+    """Featureset Id"""
+    total_affected_rows: builtins.int
+    """Number of affected rows"""
+    def __init__(
+        self,
+        *,
+        featureset_id: builtins.str = ...,
+        total_affected_rows: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["featureset_id", b"featureset_id", "total_affected_rows", b"total_affected_rows"]) -> None: ...
+
+global___FeaturesetJobsSummary = FeaturesetJobsSummary
+
+class GetJobsSummaryByExecutionIdRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    EXECUTION_ID_FIELD_NUMBER: builtins.int
+    execution_id: builtins.str
+    def __init__(
+        self,
+        *,
+        execution_id: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["execution_id", b"execution_id"]) -> None: ...
+
+global___GetJobsSummaryByExecutionIdRequest = GetJobsSummaryByExecutionIdRequest
+
+class GetJobsSummaryByExecutionIdResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    EXECUTION_ID_FIELD_NUMBER: builtins.int
+    JOB_COUNT_FIELD_NUMBER: builtins.int
+    TOTAL_AFFECTED_ROWS_FIELD_NUMBER: builtins.int
+    FIRST_JOB_RECORD_FIELD_NUMBER: builtins.int
+    LAST_JOB_RECORD_FIELD_NUMBER: builtins.int
+    execution_id: builtins.str
+    job_count: builtins.int
+    total_affected_rows: builtins.int
+    @property
+    def first_job_record(self) -> qwak.execution.v1.jobs.job_pb2.JobRecord: ...
+    @property
+    def last_job_record(self) -> qwak.execution.v1.jobs.job_pb2.JobRecord: ...
+    def __init__(
+        self,
+        *,
+        execution_id: builtins.str = ...,
+        job_count: builtins.int = ...,
+        total_affected_rows: builtins.int = ...,
+        first_job_record: qwak.execution.v1.jobs.job_pb2.JobRecord | None = ...,
+        last_job_record: qwak.execution.v1.jobs.job_pb2.JobRecord | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["first_job_record", b"first_job_record", "last_job_record", b"last_job_record"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["execution_id", b"execution_id", "first_job_record", b"first_job_record", "job_count", b"job_count", "last_job_record", b"last_job_record", "total_affected_rows", b"total_affected_rows"]) -> None: ...
+
+global___GetJobsSummaryByExecutionIdResponse = GetJobsSummaryByExecutionIdResponse
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/management_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&qwak/feature_store/sources/batch.proto\x12\x1aqwak.feature.store.sources\x1a\x1fgoogle/protobuf/timestamp.proto\"\x81\x06\n\x0b\x42\x61tchSource\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61te_created_column\x18\x03 \x01(\t\x12@\n\x0c\x61thenaSource\x18\x04 \x01(\x0b\x32(.qwak.feature.store.sources.AthenaSourceH\x00\x12>\n\x0bmongoSource\x18\x05 \x01(\x0b\x32\'.qwak.feature.store.sources.MongoSourceH\x00\x12:\n\tcsvSource\x18\x06 \x01(\x0b\x32%.qwak.feature.store.sources.CsvSourceH\x00\x12\x46\n\x0fsnowflakeSource\x18\x07 \x01(\x0b\x32+.qwak.feature.store.sources.SnowflakeSourceH\x00\x12\x42\n\rparquetSource\x18\x08 \x01(\x0b\x32).qwak.feature.store.sources.ParquetSourceH\x00\x12<\n\njdbcSource\x18\t \x01(\x0b\x32&.qwak.feature.store.sources.JdbcSourceH\x00\x12\x42\n\rverticaSource\x18\n \x01(\x0b\x32).qwak.feature.store.sources.VerticaSourceH\x00\x12\x44\n\x0e\x62igquerySource\x18\x0b \x01(\x0b\x32*.qwak.feature.store.sources.BigquerySourceH\x00\x12N\n\x13\x65lasticsearchSource\x18\x0c \x01(\x0b\x32/.qwak.feature.store.sources.ElasticsearchSourceH\x00\x12H\n\x10\x63lickhouseSource\x18\r \x01(\x0b\x32,.qwak.feature.store.sources.ClickhouseSourceH\x00\x42\x06\n\x04type\"\xae\x04\n\x17\x46ileSystemConfiguration\x12X\n\x14\x61ws_s3_configuration\x18\x01 \x01(\x0b\x32\x38.qwak.feature.store.sources.AwsS3FileSystemConfigurationH\x00\x12P\n\x10\x61ws_s3_anonymous\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.sources.AnonymousS3ConfigurationH\x00\x12W\n aws_s3_assume_role_configuration\x18\x03 \x01(\x0b\x32+.qwak.feature.store.sources.AwsS3AssumeRoleH\x00\x12M\n\x13gcs_unauthenticated\x18\x04 \x01(\x0b\x32..qwak.feature.store.sources.GcsUnauthenticatedH\x00\x12N\n\x14gcs_user_credentials\x18\x05 \x01(\x0b\x32..qwak.feature.store.sources.GcsUserCredentialsH\x00\x12g\n!gcs_service_account_impersonation\x18\x06 \x01(\x0b\x32:.qwak.feature.store.sources.GcsServiceAccountImpersonationH\x00\x42\x06\n\x04type\"#\n\x0f\x41wsS3AssumeRole\x12\x10\n\x08role_arn\x18\x01 \x01(\t\"\x91\x01\n\x1c\x41wsS3FileSystemConfiguration\x12\x1e\n\x16\x61\x63\x63\x65ss_key_secret_name\x18\x01 \x01(\t\x12\x1e\n\x16secret_key_secret_name\x18\x02 \x01(\t\x12!\n\x19session_token_secret_name\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"\x1a\n\x18\x41nonymousS3Configuration\"\x92\x03\n\nJdbcSource\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x01 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x02 \x01(\t\x12\x10\n\x08\x64\x62_table\x18\x04 \x01(\t\x12\r\n\x05query\x18\x05 \x01(\t\x12>\n\x0bmysqlSource\x18\x06 \x01(\x0b\x32\'.qwak.feature.store.sources.MysqlSourceH\x00\x12H\n\x10postgresqlSource\x18\x07 \x01(\x0b\x32,.qwak.feature.store.sources.PostgresqlSourceH\x00\x12\x44\n\x0eredshiftSource\x18\x08 \x01(\x0b\x32*.qwak.feature.store.sources.RedshiftSourceH\x00\x12\x42\n\x0c\x61thenaSource\x18\t \x01(\x0b\x32*.qwak.feature.store.sources.AthenaSourceV1H\x00\x42\x06\n\x04type\"\r\n\x0bMysqlSource\"\x12\n\x10PostgresqlSource\"\x89\x01\n\x10\x43lickhouseSource\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x0f\n\x05table\x18\x04 \x01(\tH\x00\x12\r\n\x03sql\x18\x05 \x01(\tH\x00\x42\x0c\n\nquery_type\"i\n\x0eRedshiftSource\x12\x0f\n\x07\x64\x62_user\x18\x01 \x01(\t\x12\x14\n\x0ciam_role_arn\x18\x02 \x01(\t\x12\x15\n\raccess_key_id\x18\x03 \x01(\t\x12\x19\n\x11secret_access_key\x18\x04 \x01(\t\"\x8d\x03\n\x0e\x41thenaSourceV1\x12\x12\n\naws_region\x18\x01 \x01(\t\x12I\n\x12\x61ws_authentication\x18\x02 \x01(\x0b\x32-.qwak.feature.store.sources.AwsAuthentication\x12\x1a\n\x12s3_output_location\x18\x03 \x01(\t\x12R\n\x16\x64\x61te_partition_columns\x18\x04 \x01(\x0b\x32\x30.qwak.feature.store.sources.DatePartitionColumnsH\x00\x12g\n!time_fragmented_partition_columns\x18\x05 \x01(\x0b\x32:.qwak.feature.store.sources.TimeFragmentedPartitionColumnsH\x00\x12\x13\n\tworkgroup\x18\x06 \x01(\tH\x01\x42\x18\n\x16time_partition_columnsB\x14\n\x12optional_workgroup\"E\n\x14\x44\x61tePartitionColumns\x12\x18\n\x10\x64\x61te_column_name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61te_format\x18\x02 \x01(\t\"\xb5\x02\n\x1eTimeFragmentedPartitionColumns\x12M\n\x15year_partition_column\x18\x01 \x01(\x0b\x32..qwak.feature.store.sources.YearFragmentColumn\x12Q\n\x16month_partition_column\x18\x02 \x01(\x0b\x32/.qwak.feature.store.sources.MonthFragmentColumnH\x00\x12M\n\x14\x64\x61y_partition_column\x18\x03 \x01(\x0b\x32-.qwak.feature.store.sources.DayFragmentColumnH\x01\x42\x11\n\x0fmonth_partitionB\x0f\n\rday_partition\"\xa4\x01\n\x12YearFragmentColumn\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12`\n\x1dnumeric_column_representation\x18\x02 \x01(\x0b\x32\x37.qwak.feature.store.sources.NumericColumnRepresentationH\x00\x42\x17\n\x15\x63olumn_representation\"\x87\x02\n\x13MonthFragmentColumn\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12`\n\x1dnumeric_column_representation\x18\x02 \x01(\x0b\x32\x37.qwak.feature.store.sources.NumericColumnRepresentationH\x00\x12`\n\x1dtextual_column_representation\x18\x03 \x01(\x0b\x32\x37.qwak.feature.store.sources.TextualColumnRepresentationH\x00\x42\x17\n\x15\x63olumn_representation\"\xa3\x01\n\x11\x44\x61yFragmentColumn\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12`\n\x1dnumeric_column_representation\x18\x02 \x01(\x0b\x32\x37.qwak.feature.store.sources.NumericColumnRepresentationH\x00\x42\x17\n\x15\x63olumn_representation\"\x1d\n\x1bNumericColumnRepresentation\"\x1d\n\x1bTextualColumnRepresentation\"/\n\x0c\x41thenaSource\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\xa0\x02\n\x0e\x42igquerySource\x12\x1f\n\x17\x63redentials_secret_name\x18\x01 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x02 \x01(\t\x12\r\n\x05table\x18\x03 \x01(\t\x12\x0f\n\x07project\x18\x04 \x01(\t\x12\x16\n\x0eparent_project\x18\x05 \x01(\t\x12\x0b\n\x03sql\x18\x06 \x01(\t\x12\x15\n\rviews_enabled\x18\x07 \x01(\x08\x12#\n\x17materialization_dataset\x18\x08 \x01(\tB\x02\x18\x01\x12#\n\x17materialization_project\x18\t \x01(\tB\x02\x18\x01\x12\x36\n*materialization_expiration_time_in_minutes\x18\n \x01(\tB\x02\x18\x01\"\xa3\x01\n\tCsvSource\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x17\n\x0fquote_character\x18\x02 \x01(\t\x12\x18\n\x10\x65scape_character\x18\x03 \x01(\t\x12U\n\x18\x66ilesystem_configuration\x18\x04 \x01(\x0b\x32\x33.qwak.feature.store.sources.FileSystemConfiguration\"\xab\x01\n\x0bMongoSource\x12\r\n\x05hosts\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\x12\n\ncollection\x18\x05 \x01(\t\x12\x19\n\x11\x63onnection_params\x18\x06 \x01(\t\x12\x10\n\x08protocol\x18\x07 \x01(\t\"\xae\x01\n\x0fSnowflakeSource\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\x0e\n\x06schema\x18\x05 \x01(\t\x12\x11\n\twarehouse\x18\x06 \x01(\t\x12\r\n\x05table\x18\x07 \x01(\t\x12\r\n\x05query\x18\x08 \x01(\t\"t\n\rParquetSource\x12\x0c\n\x04path\x18\x01 \x01(\t\x12U\n\x18\x66ilesystem_configuration\x18\x02 \x01(\x0b\x32\x33.qwak.feature.store.sources.FileSystemConfiguration\"\x98\x01\n\rVerticaSource\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x10\n\x08\x64\x61tabase\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x06 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x07 \x01(\t\"\xbc\x01\n\x13\x45lasticsearchSource\x12\r\n\x05nodes\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x10\n\x08resource\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x16\n\x0e\x65xclude_fields\x18\x05 \x01(\t\x12\x13\n\x0bparse_dates\x18\x06 \x01(\x08\x12\x1c\n\x14username_secret_name\x18\x07 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x08 \x01(\t\"\xe9\x01\n\x11\x41wsAuthentication\x12\x61\n\x1e\x61ws_assume_role_authentication\x18\x01 \x01(\x0b\x32\x37.qwak.feature.store.sources.AwsAssumeRoleAuthenticationH\x00\x12i\n%aws_static_credentials_authentication\x18\x02 \x01(\x0b\x32\x38.qwak.feature.store.sources.AwsCredentialsAuthenticationH\x00\x42\x06\n\x04type\"/\n\x1b\x41wsAssumeRoleAuthentication\x12\x10\n\x08role_arn\x18\x01 \x01(\t\"^\n\x1c\x41wsCredentialsAuthentication\x12\x1e\n\x16\x61\x63\x63\x65ss_key_secret_name\x18\x01 \x01(\t\x12\x1e\n\x16secret_key_secret_name\x18\x02 \x01(\t\"\x14\n\x12GcsUnauthenticated\"y\n\x12GcsUserCredentials\x12\x1d\n\x15\x63lient_id_secret_name\x18\x01 \x01(\t\x12!\n\x19\x63lient_secret_secret_name\x18\x02 \x01(\t\x12!\n\x19refresh_token_secret_name\x18\x03 \x01(\t\">\n\x1eGcsServiceAccountImpersonation\x12\x1c\n\x14service_account_user\x18\x01 \x01(\tBX\n%com.qwak.ai.feature.store.sources.apiP\x01Z-qwak/featurestore/sources;featurestoresourcesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&qwak/feature_store/sources/batch.proto\x12\x1aqwak.feature.store.sources\x1a\x1fgoogle/protobuf/timestamp.proto\"\xd9\x06\n\x0b\x42\x61tchSource\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61te_created_column\x18\x03 \x01(\t\x12@\n\x0c\x61thenaSource\x18\x04 \x01(\x0b\x32(.qwak.feature.store.sources.AthenaSourceH\x00\x12>\n\x0bmongoSource\x18\x05 \x01(\x0b\x32\'.qwak.feature.store.sources.MongoSourceH\x00\x12:\n\tcsvSource\x18\x06 \x01(\x0b\x32%.qwak.feature.store.sources.CsvSourceH\x00\x12\x46\n\x0fsnowflakeSource\x18\x07 \x01(\x0b\x32+.qwak.feature.store.sources.SnowflakeSourceH\x00\x12\x42\n\rparquetSource\x18\x08 \x01(\x0b\x32).qwak.feature.store.sources.ParquetSourceH\x00\x12<\n\njdbcSource\x18\t \x01(\x0b\x32&.qwak.feature.store.sources.JdbcSourceH\x00\x12\x42\n\rverticaSource\x18\n \x01(\x0b\x32).qwak.feature.store.sources.VerticaSourceH\x00\x12\x44\n\x0e\x62igquerySource\x18\x0b \x01(\x0b\x32*.qwak.feature.store.sources.BigquerySourceH\x00\x12N\n\x13\x65lasticsearchSource\x18\x0c \x01(\x0b\x32/.qwak.feature.store.sources.ElasticsearchSourceH\x00\x12H\n\x10\x63lickhouseSource\x18\r \x01(\x0b\x32,.qwak.feature.store.sources.ClickhouseSourceH\x00\x12V\n\x17\x66\x65\x61turesetOfflineSource\x18\x0e \x01(\x0b\x32\x33.qwak.feature.store.sources.FeaturesetOfflineSourceH\x00\x42\x06\n\x04type\"\xae\x04\n\x17\x46ileSystemConfiguration\x12X\n\x14\x61ws_s3_configuration\x18\x01 \x01(\x0b\x32\x38.qwak.feature.store.sources.AwsS3FileSystemConfigurationH\x00\x12P\n\x10\x61ws_s3_anonymous\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.sources.AnonymousS3ConfigurationH\x00\x12W\n aws_s3_assume_role_configuration\x18\x03 \x01(\x0b\x32+.qwak.feature.store.sources.AwsS3AssumeRoleH\x00\x12M\n\x13gcs_unauthenticated\x18\x04 \x01(\x0b\x32..qwak.feature.store.sources.GcsUnauthenticatedH\x00\x12N\n\x14gcs_user_credentials\x18\x05 \x01(\x0b\x32..qwak.feature.store.sources.GcsUserCredentialsH\x00\x12g\n!gcs_service_account_impersonation\x18\x06 \x01(\x0b\x32:.qwak.feature.store.sources.GcsServiceAccountImpersonationH\x00\x42\x06\n\x04type\"#\n\x0f\x41wsS3AssumeRole\x12\x10\n\x08role_arn\x18\x01 \x01(\t\"\x91\x01\n\x1c\x41wsS3FileSystemConfiguration\x12\x1e\n\x16\x61\x63\x63\x65ss_key_secret_name\x18\x01 \x01(\t\x12\x1e\n\x16secret_key_secret_name\x18\x02 \x01(\t\x12!\n\x19session_token_secret_name\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"\x1a\n\x18\x41nonymousS3Configuration\"\x92\x03\n\nJdbcSource\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x01 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x02 \x01(\t\x12\x10\n\x08\x64\x62_table\x18\x04 \x01(\t\x12\r\n\x05query\x18\x05 \x01(\t\x12>\n\x0bmysqlSource\x18\x06 \x01(\x0b\x32\'.qwak.feature.store.sources.MysqlSourceH\x00\x12H\n\x10postgresqlSource\x18\x07 \x01(\x0b\x32,.qwak.feature.store.sources.PostgresqlSourceH\x00\x12\x44\n\x0eredshiftSource\x18\x08 \x01(\x0b\x32*.qwak.feature.store.sources.RedshiftSourceH\x00\x12\x42\n\x0c\x61thenaSource\x18\t \x01(\x0b\x32*.qwak.feature.store.sources.AthenaSourceV1H\x00\x42\x06\n\x04type\"\r\n\x0bMysqlSource\"\x12\n\x10PostgresqlSource\"\x89\x01\n\x10\x43lickhouseSource\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x0f\n\x05table\x18\x04 \x01(\tH\x00\x12\r\n\x03sql\x18\x05 \x01(\tH\x00\x42\x0c\n\nquery_type\"i\n\x0eRedshiftSource\x12\x0f\n\x07\x64\x62_user\x18\x01 \x01(\t\x12\x14\n\x0ciam_role_arn\x18\x02 \x01(\t\x12\x15\n\raccess_key_id\x18\x03 \x01(\t\x12\x19\n\x11secret_access_key\x18\x04 \x01(\t\"\x8d\x03\n\x0e\x41thenaSourceV1\x12\x12\n\naws_region\x18\x01 \x01(\t\x12I\n\x12\x61ws_authentication\x18\x02 \x01(\x0b\x32-.qwak.feature.store.sources.AwsAuthentication\x12\x1a\n\x12s3_output_location\x18\x03 \x01(\t\x12R\n\x16\x64\x61te_partition_columns\x18\x04 \x01(\x0b\x32\x30.qwak.feature.store.sources.DatePartitionColumnsH\x00\x12g\n!time_fragmented_partition_columns\x18\x05 \x01(\x0b\x32:.qwak.feature.store.sources.TimeFragmentedPartitionColumnsH\x00\x12\x13\n\tworkgroup\x18\x06 \x01(\tH\x01\x42\x18\n\x16time_partition_columnsB\x14\n\x12optional_workgroup\"E\n\x14\x44\x61tePartitionColumns\x12\x18\n\x10\x64\x61te_column_name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61te_format\x18\x02 \x01(\t\"\xb5\x02\n\x1eTimeFragmentedPartitionColumns\x12M\n\x15year_partition_column\x18\x01 \x01(\x0b\x32..qwak.feature.store.sources.YearFragmentColumn\x12Q\n\x16month_partition_column\x18\x02 \x01(\x0b\x32/.qwak.feature.store.sources.MonthFragmentColumnH\x00\x12M\n\x14\x64\x61y_partition_column\x18\x03 \x01(\x0b\x32-.qwak.feature.store.sources.DayFragmentColumnH\x01\x42\x11\n\x0fmonth_partitionB\x0f\n\rday_partition\"\xa4\x01\n\x12YearFragmentColumn\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12`\n\x1dnumeric_column_representation\x18\x02 \x01(\x0b\x32\x37.qwak.feature.store.sources.NumericColumnRepresentationH\x00\x42\x17\n\x15\x63olumn_representation\"\x87\x02\n\x13MonthFragmentColumn\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12`\n\x1dnumeric_column_representation\x18\x02 \x01(\x0b\x32\x37.qwak.feature.store.sources.NumericColumnRepresentationH\x00\x12`\n\x1dtextual_column_representation\x18\x03 \x01(\x0b\x32\x37.qwak.feature.store.sources.TextualColumnRepresentationH\x00\x42\x17\n\x15\x63olumn_representation\"\xa3\x01\n\x11\x44\x61yFragmentColumn\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12`\n\x1dnumeric_column_representation\x18\x02 \x01(\x0b\x32\x37.qwak.feature.store.sources.NumericColumnRepresentationH\x00\x42\x17\n\x15\x63olumn_representation\"\x1d\n\x1bNumericColumnRepresentation\"\x1d\n\x1bTextualColumnRepresentation\"/\n\x0c\x41thenaSource\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\xa0\x02\n\x0e\x42igquerySource\x12\x1f\n\x17\x63redentials_secret_name\x18\x01 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x02 \x01(\t\x12\r\n\x05table\x18\x03 \x01(\t\x12\x0f\n\x07project\x18\x04 \x01(\t\x12\x16\n\x0eparent_project\x18\x05 \x01(\t\x12\x0b\n\x03sql\x18\x06 \x01(\t\x12\x15\n\rviews_enabled\x18\x07 \x01(\x08\x12#\n\x17materialization_dataset\x18\x08 \x01(\tB\x02\x18\x01\x12#\n\x17materialization_project\x18\t \x01(\tB\x02\x18\x01\x12\x36\n*materialization_expiration_time_in_minutes\x18\n \x01(\tB\x02\x18\x01\"\xa3\x01\n\tCsvSource\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x17\n\x0fquote_character\x18\x02 \x01(\t\x12\x18\n\x10\x65scape_character\x18\x03 \x01(\t\x12U\n\x18\x66ilesystem_configuration\x18\x04 \x01(\x0b\x32\x33.qwak.feature.store.sources.FileSystemConfiguration\"\xab\x01\n\x0bMongoSource\x12\r\n\x05hosts\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\x12\n\ncollection\x18\x05 \x01(\t\x12\x19\n\x11\x63onnection_params\x18\x06 \x01(\t\x12\x10\n\x08protocol\x18\x07 \x01(\t\"\xae\x01\n\x0fSnowflakeSource\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\x0e\n\x06schema\x18\x05 \x01(\t\x12\x11\n\twarehouse\x18\x06 \x01(\t\x12\r\n\x05table\x18\x07 \x01(\t\x12\r\n\x05query\x18\x08 \x01(\t\"t\n\rParquetSource\x12\x0c\n\x04path\x18\x01 \x01(\t\x12U\n\x18\x66ilesystem_configuration\x18\x02 \x01(\x0b\x32\x33.qwak.feature.store.sources.FileSystemConfiguration\"\x98\x01\n\rVerticaSource\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x10\n\x08\x64\x61tabase\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x06 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x07 \x01(\t\"\xbc\x01\n\x13\x45lasticsearchSource\x12\r\n\x05nodes\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x10\n\x08resource\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x16\n\x0e\x65xclude_fields\x18\x05 \x01(\t\x12\x13\n\x0bparse_dates\x18\x06 \x01(\x08\x12\x1c\n\x14username_secret_name\x18\x07 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x08 \x01(\t\"(\n\x17\x46\x65\x61turesetOfflineSource\x12\r\n\x05\x61lias\x18\x01 \x01(\t\"\xe9\x01\n\x11\x41wsAuthentication\x12\x61\n\x1e\x61ws_assume_role_authentication\x18\x01 \x01(\x0b\x32\x37.qwak.feature.store.sources.AwsAssumeRoleAuthenticationH\x00\x12i\n%aws_static_credentials_authentication\x18\x02 \x01(\x0b\x32\x38.qwak.feature.store.sources.AwsCredentialsAuthenticationH\x00\x42\x06\n\x04type\"/\n\x1b\x41wsAssumeRoleAuthentication\x12\x10\n\x08role_arn\x18\x01 \x01(\t\"^\n\x1c\x41wsCredentialsAuthentication\x12\x1e\n\x16\x61\x63\x63\x65ss_key_secret_name\x18\x01 \x01(\t\x12\x1e\n\x16secret_key_secret_name\x18\x02 \x01(\t\"\x14\n\x12GcsUnauthenticated\"y\n\x12GcsUserCredentials\x12\x1d\n\x15\x63lient_id_secret_name\x18\x01 \x01(\t\x12!\n\x19\x63lient_secret_secret_name\x18\x02 \x01(\t\x12!\n\x19refresh_token_secret_name\x18\x03 \x01(\t\">\n\x1eGcsServiceAccountImpersonation\x12\x1c\n\x14service_account_user\x18\x01 \x01(\tBX\n%com.qwak.ai.feature.store.sources.apiP\x01Z-qwak/featurestore/sources;featurestoresourcesb\x06proto3')
 
 
 
 _BATCHSOURCE = DESCRIPTOR.message_types_by_name['BatchSource']
 _FILESYSTEMCONFIGURATION = DESCRIPTOR.message_types_by_name['FileSystemConfiguration']
 _AWSS3ASSUMEROLE = DESCRIPTOR.message_types_by_name['AwsS3AssumeRole']
 _AWSS3FILESYSTEMCONFIGURATION = DESCRIPTOR.message_types_by_name['AwsS3FileSystemConfiguration']
@@ -41,14 +41,15 @@
 _BIGQUERYSOURCE = DESCRIPTOR.message_types_by_name['BigquerySource']
 _CSVSOURCE = DESCRIPTOR.message_types_by_name['CsvSource']
 _MONGOSOURCE = DESCRIPTOR.message_types_by_name['MongoSource']
 _SNOWFLAKESOURCE = DESCRIPTOR.message_types_by_name['SnowflakeSource']
 _PARQUETSOURCE = DESCRIPTOR.message_types_by_name['ParquetSource']
 _VERTICASOURCE = DESCRIPTOR.message_types_by_name['VerticaSource']
 _ELASTICSEARCHSOURCE = DESCRIPTOR.message_types_by_name['ElasticsearchSource']
+_FEATURESETOFFLINESOURCE = DESCRIPTOR.message_types_by_name['FeaturesetOfflineSource']
 _AWSAUTHENTICATION = DESCRIPTOR.message_types_by_name['AwsAuthentication']
 _AWSASSUMEROLEAUTHENTICATION = DESCRIPTOR.message_types_by_name['AwsAssumeRoleAuthentication']
 _AWSCREDENTIALSAUTHENTICATION = DESCRIPTOR.message_types_by_name['AwsCredentialsAuthentication']
 _GCSUNAUTHENTICATED = DESCRIPTOR.message_types_by_name['GcsUnauthenticated']
 _GCSUSERCREDENTIALS = DESCRIPTOR.message_types_by_name['GcsUserCredentials']
 _GCSSERVICEACCOUNTIMPERSONATION = DESCRIPTOR.message_types_by_name['GcsServiceAccountImpersonation']
 BatchSource = _reflection.GeneratedProtocolMessageType('BatchSource', (_message.Message,), {
@@ -229,14 +230,21 @@
 ElasticsearchSource = _reflection.GeneratedProtocolMessageType('ElasticsearchSource', (_message.Message,), {
   'DESCRIPTOR' : _ELASTICSEARCHSOURCE,
   '__module__' : 'qwak.feature_store.sources.batch_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.sources.ElasticsearchSource)
   })
 _sym_db.RegisterMessage(ElasticsearchSource)
 
+FeaturesetOfflineSource = _reflection.GeneratedProtocolMessageType('FeaturesetOfflineSource', (_message.Message,), {
+  'DESCRIPTOR' : _FEATURESETOFFLINESOURCE,
+  '__module__' : 'qwak.feature_store.sources.batch_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.sources.FeaturesetOfflineSource)
+  })
+_sym_db.RegisterMessage(FeaturesetOfflineSource)
+
 AwsAuthentication = _reflection.GeneratedProtocolMessageType('AwsAuthentication', (_message.Message,), {
   'DESCRIPTOR' : _AWSAUTHENTICATION,
   '__module__' : 'qwak.feature_store.sources.batch_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.sources.AwsAuthentication)
   })
 _sym_db.RegisterMessage(AwsAuthentication)
 
@@ -282,71 +290,73 @@
   _BIGQUERYSOURCE.fields_by_name['materialization_dataset']._options = None
   _BIGQUERYSOURCE.fields_by_name['materialization_dataset']._serialized_options = b'\030\001'
   _BIGQUERYSOURCE.fields_by_name['materialization_project']._options = None
   _BIGQUERYSOURCE.fields_by_name['materialization_project']._serialized_options = b'\030\001'
   _BIGQUERYSOURCE.fields_by_name['materialization_expiration_time_in_minutes']._options = None
   _BIGQUERYSOURCE.fields_by_name['materialization_expiration_time_in_minutes']._serialized_options = b'\030\001'
   _BATCHSOURCE._serialized_start=104
-  _BATCHSOURCE._serialized_end=873
-  _FILESYSTEMCONFIGURATION._serialized_start=876
-  _FILESYSTEMCONFIGURATION._serialized_end=1434
-  _AWSS3ASSUMEROLE._serialized_start=1436
-  _AWSS3ASSUMEROLE._serialized_end=1471
-  _AWSS3FILESYSTEMCONFIGURATION._serialized_start=1474
-  _AWSS3FILESYSTEMCONFIGURATION._serialized_end=1619
-  _ANONYMOUSS3CONFIGURATION._serialized_start=1621
-  _ANONYMOUSS3CONFIGURATION._serialized_end=1647
-  _JDBCSOURCE._serialized_start=1650
-  _JDBCSOURCE._serialized_end=2052
-  _MYSQLSOURCE._serialized_start=2054
-  _MYSQLSOURCE._serialized_end=2067
-  _POSTGRESQLSOURCE._serialized_start=2069
-  _POSTGRESQLSOURCE._serialized_end=2087
-  _CLICKHOUSESOURCE._serialized_start=2090
-  _CLICKHOUSESOURCE._serialized_end=2227
-  _REDSHIFTSOURCE._serialized_start=2229
-  _REDSHIFTSOURCE._serialized_end=2334
-  _ATHENASOURCEV1._serialized_start=2337
-  _ATHENASOURCEV1._serialized_end=2734
-  _DATEPARTITIONCOLUMNS._serialized_start=2736
-  _DATEPARTITIONCOLUMNS._serialized_end=2805
-  _TIMEFRAGMENTEDPARTITIONCOLUMNS._serialized_start=2808
-  _TIMEFRAGMENTEDPARTITIONCOLUMNS._serialized_end=3117
-  _YEARFRAGMENTCOLUMN._serialized_start=3120
-  _YEARFRAGMENTCOLUMN._serialized_end=3284
-  _MONTHFRAGMENTCOLUMN._serialized_start=3287
-  _MONTHFRAGMENTCOLUMN._serialized_end=3550
-  _DAYFRAGMENTCOLUMN._serialized_start=3553
-  _DAYFRAGMENTCOLUMN._serialized_end=3716
-  _NUMERICCOLUMNREPRESENTATION._serialized_start=3718
-  _NUMERICCOLUMNREPRESENTATION._serialized_end=3747
-  _TEXTUALCOLUMNREPRESENTATION._serialized_start=3749
-  _TEXTUALCOLUMNREPRESENTATION._serialized_end=3778
-  _ATHENASOURCE._serialized_start=3780
-  _ATHENASOURCE._serialized_end=3827
-  _BIGQUERYSOURCE._serialized_start=3830
-  _BIGQUERYSOURCE._serialized_end=4118
-  _CSVSOURCE._serialized_start=4121
-  _CSVSOURCE._serialized_end=4284
-  _MONGOSOURCE._serialized_start=4287
-  _MONGOSOURCE._serialized_end=4458
-  _SNOWFLAKESOURCE._serialized_start=4461
-  _SNOWFLAKESOURCE._serialized_end=4635
-  _PARQUETSOURCE._serialized_start=4637
-  _PARQUETSOURCE._serialized_end=4753
-  _VERTICASOURCE._serialized_start=4756
-  _VERTICASOURCE._serialized_end=4908
-  _ELASTICSEARCHSOURCE._serialized_start=4911
-  _ELASTICSEARCHSOURCE._serialized_end=5099
-  _AWSAUTHENTICATION._serialized_start=5102
-  _AWSAUTHENTICATION._serialized_end=5335
-  _AWSASSUMEROLEAUTHENTICATION._serialized_start=5337
-  _AWSASSUMEROLEAUTHENTICATION._serialized_end=5384
-  _AWSCREDENTIALSAUTHENTICATION._serialized_start=5386
-  _AWSCREDENTIALSAUTHENTICATION._serialized_end=5480
-  _GCSUNAUTHENTICATED._serialized_start=5482
-  _GCSUNAUTHENTICATED._serialized_end=5502
-  _GCSUSERCREDENTIALS._serialized_start=5504
-  _GCSUSERCREDENTIALS._serialized_end=5625
-  _GCSSERVICEACCOUNTIMPERSONATION._serialized_start=5627
-  _GCSSERVICEACCOUNTIMPERSONATION._serialized_end=5689
+  _BATCHSOURCE._serialized_end=961
+  _FILESYSTEMCONFIGURATION._serialized_start=964
+  _FILESYSTEMCONFIGURATION._serialized_end=1522
+  _AWSS3ASSUMEROLE._serialized_start=1524
+  _AWSS3ASSUMEROLE._serialized_end=1559
+  _AWSS3FILESYSTEMCONFIGURATION._serialized_start=1562
+  _AWSS3FILESYSTEMCONFIGURATION._serialized_end=1707
+  _ANONYMOUSS3CONFIGURATION._serialized_start=1709
+  _ANONYMOUSS3CONFIGURATION._serialized_end=1735
+  _JDBCSOURCE._serialized_start=1738
+  _JDBCSOURCE._serialized_end=2140
+  _MYSQLSOURCE._serialized_start=2142
+  _MYSQLSOURCE._serialized_end=2155
+  _POSTGRESQLSOURCE._serialized_start=2157
+  _POSTGRESQLSOURCE._serialized_end=2175
+  _CLICKHOUSESOURCE._serialized_start=2178
+  _CLICKHOUSESOURCE._serialized_end=2315
+  _REDSHIFTSOURCE._serialized_start=2317
+  _REDSHIFTSOURCE._serialized_end=2422
+  _ATHENASOURCEV1._serialized_start=2425
+  _ATHENASOURCEV1._serialized_end=2822
+  _DATEPARTITIONCOLUMNS._serialized_start=2824
+  _DATEPARTITIONCOLUMNS._serialized_end=2893
+  _TIMEFRAGMENTEDPARTITIONCOLUMNS._serialized_start=2896
+  _TIMEFRAGMENTEDPARTITIONCOLUMNS._serialized_end=3205
+  _YEARFRAGMENTCOLUMN._serialized_start=3208
+  _YEARFRAGMENTCOLUMN._serialized_end=3372
+  _MONTHFRAGMENTCOLUMN._serialized_start=3375
+  _MONTHFRAGMENTCOLUMN._serialized_end=3638
+  _DAYFRAGMENTCOLUMN._serialized_start=3641
+  _DAYFRAGMENTCOLUMN._serialized_end=3804
+  _NUMERICCOLUMNREPRESENTATION._serialized_start=3806
+  _NUMERICCOLUMNREPRESENTATION._serialized_end=3835
+  _TEXTUALCOLUMNREPRESENTATION._serialized_start=3837
+  _TEXTUALCOLUMNREPRESENTATION._serialized_end=3866
+  _ATHENASOURCE._serialized_start=3868
+  _ATHENASOURCE._serialized_end=3915
+  _BIGQUERYSOURCE._serialized_start=3918
+  _BIGQUERYSOURCE._serialized_end=4206
+  _CSVSOURCE._serialized_start=4209
+  _CSVSOURCE._serialized_end=4372
+  _MONGOSOURCE._serialized_start=4375
+  _MONGOSOURCE._serialized_end=4546
+  _SNOWFLAKESOURCE._serialized_start=4549
+  _SNOWFLAKESOURCE._serialized_end=4723
+  _PARQUETSOURCE._serialized_start=4725
+  _PARQUETSOURCE._serialized_end=4841
+  _VERTICASOURCE._serialized_start=4844
+  _VERTICASOURCE._serialized_end=4996
+  _ELASTICSEARCHSOURCE._serialized_start=4999
+  _ELASTICSEARCHSOURCE._serialized_end=5187
+  _FEATURESETOFFLINESOURCE._serialized_start=5189
+  _FEATURESETOFFLINESOURCE._serialized_end=5229
+  _AWSAUTHENTICATION._serialized_start=5232
+  _AWSAUTHENTICATION._serialized_end=5465
+  _AWSASSUMEROLEAUTHENTICATION._serialized_start=5467
+  _AWSASSUMEROLEAUTHENTICATION._serialized_end=5514
+  _AWSCREDENTIALSAUTHENTICATION._serialized_start=5516
+  _AWSCREDENTIALSAUTHENTICATION._serialized_end=5610
+  _GCSUNAUTHENTICATED._serialized_start=5612
+  _GCSUNAUTHENTICATED._serialized_end=5632
+  _GCSUSERCREDENTIALS._serialized_start=5634
+  _GCSUSERCREDENTIALS._serialized_end=5755
+  _GCSSERVICEACCOUNTIMPERSONATION._serialized_start=5757
+  _GCSSERVICEACCOUNTIMPERSONATION._serialized_end=5819
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     SNOWFLAKESOURCE_FIELD_NUMBER: builtins.int
     PARQUETSOURCE_FIELD_NUMBER: builtins.int
     JDBCSOURCE_FIELD_NUMBER: builtins.int
     VERTICASOURCE_FIELD_NUMBER: builtins.int
     BIGQUERYSOURCE_FIELD_NUMBER: builtins.int
     ELASTICSEARCHSOURCE_FIELD_NUMBER: builtins.int
     CLICKHOUSESOURCE_FIELD_NUMBER: builtins.int
+    FEATURESETOFFLINESOURCE_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Source given name (by the user)"""
     description: builtins.str
     """Source description"""
     date_created_column: builtins.str
     """Date column of the database, used slicing the data already processed by the feature store engine"""
     @property
@@ -53,14 +54,16 @@
     def verticaSource(self) -> global___VerticaSource: ...
     @property
     def bigquerySource(self) -> global___BigquerySource: ...
     @property
     def elasticsearchSource(self) -> global___ElasticsearchSource: ...
     @property
     def clickhouseSource(self) -> global___ClickhouseSource: ...
+    @property
+    def featuresetOfflineSource(self) -> global___FeaturesetOfflineSource: ...
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         description: builtins.str = ...,
         date_created_column: builtins.str = ...,
         athenaSource: global___AthenaSource | None = ...,
@@ -69,18 +72,19 @@
         snowflakeSource: global___SnowflakeSource | None = ...,
         parquetSource: global___ParquetSource | None = ...,
         jdbcSource: global___JdbcSource | None = ...,
         verticaSource: global___VerticaSource | None = ...,
         bigquerySource: global___BigquerySource | None = ...,
         elasticsearchSource: global___ElasticsearchSource | None = ...,
         clickhouseSource: global___ClickhouseSource | None = ...,
+        featuresetOfflineSource: global___FeaturesetOfflineSource | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["athenaSource", b"athenaSource", "bigquerySource", b"bigquerySource", "clickhouseSource", b"clickhouseSource", "csvSource", b"csvSource", "elasticsearchSource", b"elasticsearchSource", "jdbcSource", b"jdbcSource", "mongoSource", b"mongoSource", "parquetSource", b"parquetSource", "snowflakeSource", b"snowflakeSource", "type", b"type", "verticaSource", b"verticaSource"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["athenaSource", b"athenaSource", "bigquerySource", b"bigquerySource", "clickhouseSource", b"clickhouseSource", "csvSource", b"csvSource", "date_created_column", b"date_created_column", "description", b"description", "elasticsearchSource", b"elasticsearchSource", "jdbcSource", b"jdbcSource", "mongoSource", b"mongoSource", "name", b"name", "parquetSource", b"parquetSource", "snowflakeSource", b"snowflakeSource", "type", b"type", "verticaSource", b"verticaSource"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["athenaSource", "mongoSource", "csvSource", "snowflakeSource", "parquetSource", "jdbcSource", "verticaSource", "bigquerySource", "elasticsearchSource", "clickhouseSource"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["athenaSource", b"athenaSource", "bigquerySource", b"bigquerySource", "clickhouseSource", b"clickhouseSource", "csvSource", b"csvSource", "elasticsearchSource", b"elasticsearchSource", "featuresetOfflineSource", b"featuresetOfflineSource", "jdbcSource", b"jdbcSource", "mongoSource", b"mongoSource", "parquetSource", b"parquetSource", "snowflakeSource", b"snowflakeSource", "type", b"type", "verticaSource", b"verticaSource"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["athenaSource", b"athenaSource", "bigquerySource", b"bigquerySource", "clickhouseSource", b"clickhouseSource", "csvSource", b"csvSource", "date_created_column", b"date_created_column", "description", b"description", "elasticsearchSource", b"elasticsearchSource", "featuresetOfflineSource", b"featuresetOfflineSource", "jdbcSource", b"jdbcSource", "mongoSource", b"mongoSource", "name", b"name", "parquetSource", b"parquetSource", "snowflakeSource", b"snowflakeSource", "type", b"type", "verticaSource", b"verticaSource"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["athenaSource", "mongoSource", "csvSource", "snowflakeSource", "parquetSource", "jdbcSource", "verticaSource", "bigquerySource", "elasticsearchSource", "clickhouseSource", "featuresetOfflineSource"] | None: ...
 
 global___BatchSource = BatchSource
 
 class FileSystemConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AWS_S3_CONFIGURATION_FIELD_NUMBER: builtins.int
@@ -785,14 +789,29 @@
         username_secret_name: builtins.str = ...,
         password_secret_name: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["exclude_fields", b"exclude_fields", "nodes", b"nodes", "parse_dates", b"parse_dates", "password_secret_name", b"password_secret_name", "port", b"port", "query", b"query", "resource", b"resource", "username_secret_name", b"username_secret_name"]) -> None: ...
 
 global___ElasticsearchSource = ElasticsearchSource
 
+class FeaturesetOfflineSource(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ALIAS_FIELD_NUMBER: builtins.int
+    alias: builtins.str
+    """Featureset alias as referred to in the transformation"""
+    def __init__(
+        self,
+        *,
+        alias: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["alias", b"alias"]) -> None: ...
+
+global___FeaturesetOfflineSource = FeaturesetOfflineSource
+
 class AwsAuthentication(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AWS_ASSUME_ROLE_AUTHENTICATION_FIELD_NUMBER: builtins.int
     AWS_STATIC_CREDENTIALS_AUTHENTICATION_FIELD_NUMBER: builtins.int
     @property
     def aws_assume_role_authentication(self) -> global___AwsAssumeRoleAuthentication: ...
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%qwak/fitness_service/constructs.proto\x12\x14qwak.fitness.service\"\xa2\x01\n\x0f\x42uildProperties\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x35\n\tmodel_uri\x18\x05 \x01(\x0b\x32\".qwak.fitness.service.ModelUriSpec\x12\x16\n\x0egpu_compatible\x18\x06 \x01(\x08\"\x8d\x01\n\x0cModelUriSpec\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x17\n\x0fgit_credentials\x18\x03 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x04 \x01(\t\x12\x11\n\tcommit_id\x18\x05 \x01(\t\x12\x10\n\x08main_dir\x18\x06 \x01(\t\"t\n\x08\x42uildEnv\x12\x33\n\ndocker_env\x18\x01 \x01(\x0b\x32\x1f.qwak.fitness.service.DockerEnv\x12\x33\n\npython_env\x18\x02 \x01(\x0b\x32\x1f.qwak.fitness.service.PythonEnv\"a\n\tDockerEnv\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x10\n\x08\x65nv_vars\x18\x02 \x03(\t\x12\x10\n\x08no_cache\x18\x03 \x01(\x08\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x04 \x01(\t\"|\n\tPythonEnv\x12\x17\n\x0fgit_credentials\x18\x01 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x02 \x01(\t\x12\x18\n\x10qwak_sdk_version\x18\x03 \x01(\t\x12\x1c\n\x14qwak_sdk_extra_index\x18\x04 \x01(\t\"j\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12\x36\n\x0cmemory_units\x18\x03 \x01(\x0e\x32 .qwak.fitness.service.MemoryUnit\"\xaf\x01\n\x0cGpuResources\x12/\n\x08gpu_type\x18\x01 \x01(\x0e\x32\x1d.qwak.fitness.service.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x03 \x01(\x02\x12\x15\n\rmemory_amount\x18\x04 \x01(\x05\x12\x36\n\x0cmemory_units\x18\x05 \x01(\x0e\x32 .qwak.fitness.service.MemoryUnit*7\n\nMemoryUnit\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*w\n\x07GpuType\x12\x0b\n\x07INVALID\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06\x42#\n\x1f\x63om.qwak.ai.fitness.service.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%qwak/fitness_service/constructs.proto\x12\x14qwak.fitness.service\"\xa2\x01\n\x0f\x42uildProperties\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x35\n\tmodel_uri\x18\x05 \x01(\x0b\x32\".qwak.fitness.service.ModelUriSpec\x12\x16\n\x0egpu_compatible\x18\x06 \x01(\x08\"\x8d\x01\n\x0cModelUriSpec\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x17\n\x0fgit_credentials\x18\x03 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x04 \x01(\t\x12\x11\n\tcommit_id\x18\x05 \x01(\t\x12\x10\n\x08main_dir\x18\x06 \x01(\t\"t\n\x08\x42uildEnv\x12\x33\n\ndocker_env\x18\x01 \x01(\x0b\x32\x1f.qwak.fitness.service.DockerEnv\x12\x33\n\npython_env\x18\x02 \x01(\x0b\x32\x1f.qwak.fitness.service.PythonEnv\"\x8a\x01\n\tDockerEnv\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x10\n\x08\x65nv_vars\x18\x02 \x03(\t\x12\x10\n\x08no_cache\x18\x03 \x01(\x08\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x04 \x01(\t\x12\'\n\x1fservice_account_key_secret_name\x18\x05 \x01(\t\"|\n\tPythonEnv\x12\x17\n\x0fgit_credentials\x18\x01 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x02 \x01(\t\x12\x18\n\x10qwak_sdk_version\x18\x03 \x01(\t\x12\x1c\n\x14qwak_sdk_extra_index\x18\x04 \x01(\t\"j\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12\x36\n\x0cmemory_units\x18\x03 \x01(\x0e\x32 .qwak.fitness.service.MemoryUnit\"\xaf\x01\n\x0cGpuResources\x12/\n\x08gpu_type\x18\x01 \x01(\x0e\x32\x1d.qwak.fitness.service.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x03 \x01(\x02\x12\x15\n\rmemory_amount\x18\x04 \x01(\x05\x12\x36\n\x0cmemory_units\x18\x05 \x01(\x0e\x32 .qwak.fitness.service.MemoryUnit*7\n\nMemoryUnit\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x8c\x02\n\x07GpuType\x12\x0b\n\x07INVALID\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06\x12\x14\n\x10NVIDIA_T4_1_4_15\x10\x07\x12\x14\n\x10NVIDIA_T4_1_8_30\x10\x08\x12\x15\n\x11NVIDIA_T4_1_16_60\x10\t\x12\x1e\n\x1aNVIDIA_A100_80GB_8_96_1360\x10\n\x12\x16\n\x12NVIDIA_V100_1_8_52\x10\x0b\x12\x18\n\x14NVIDIA_V100_4_32_208\x10\x0c\x42#\n\x1f\x63om.qwak.ai.fitness.service.apiP\x01\x62\x06proto3')
 
 _MEMORYUNIT = DESCRIPTOR.enum_types_by_name['MemoryUnit']
 MemoryUnit = enum_type_wrapper.EnumTypeWrapper(_MEMORYUNIT)
 _GPUTYPE = DESCRIPTOR.enum_types_by_name['GpuType']
 GpuType = enum_type_wrapper.EnumTypeWrapper(_GPUTYPE)
 UNKNOWN_MEMORY_UNIT = 0
 MIB = 1
@@ -27,14 +27,20 @@
 INVALID = 0
 NVIDIA_K80 = 1
 NVIDIA_V100 = 2
 NVIDIA_A100 = 3
 NVIDIA_T4 = 4
 NVIDIA_A10G = 5
 NVIDIA_L4 = 6
+NVIDIA_T4_1_4_15 = 7
+NVIDIA_T4_1_8_30 = 8
+NVIDIA_T4_1_16_60 = 9
+NVIDIA_A100_80GB_8_96_1360 = 10
+NVIDIA_V100_1_8_52 = 11
+NVIDIA_V100_4_32_208 = 12
 
 
 _BUILDPROPERTIES = DESCRIPTOR.message_types_by_name['BuildProperties']
 _MODELURISPEC = DESCRIPTOR.message_types_by_name['ModelUriSpec']
 _BUILDENV = DESCRIPTOR.message_types_by_name['BuildEnv']
 _DOCKERENV = DESCRIPTOR.message_types_by_name['DockerEnv']
 _PYTHONENV = DESCRIPTOR.message_types_by_name['PythonEnv']
@@ -89,26 +95,26 @@
   })
 _sym_db.RegisterMessage(GpuResources)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\037com.qwak.ai.fitness.service.apiP\001'
-  _MEMORYUNIT._serialized_start=1001
-  _MEMORYUNIT._serialized_end=1056
-  _GPUTYPE._serialized_start=1058
-  _GPUTYPE._serialized_end=1177
+  _MEMORYUNIT._serialized_start=1043
+  _MEMORYUNIT._serialized_end=1098
+  _GPUTYPE._serialized_start=1101
+  _GPUTYPE._serialized_end=1369
   _BUILDPROPERTIES._serialized_start=64
   _BUILDPROPERTIES._serialized_end=226
   _MODELURISPEC._serialized_start=229
   _MODELURISPEC._serialized_end=370
   _BUILDENV._serialized_start=372
   _BUILDENV._serialized_end=488
-  _DOCKERENV._serialized_start=490
-  _DOCKERENV._serialized_end=587
-  _PYTHONENV._serialized_start=589
-  _PYTHONENV._serialized_end=713
-  _CPURESOURCES._serialized_start=715
-  _CPURESOURCES._serialized_end=821
-  _GPURESOURCES._serialized_start=824
-  _GPURESOURCES._serialized_end=999
+  _DOCKERENV._serialized_start=491
+  _DOCKERENV._serialized_end=629
+  _PYTHONENV._serialized_start=631
+  _PYTHONENV._serialized_end=755
+  _CPURESOURCES._serialized_start=757
+  _CPURESOURCES._serialized_end=863
+  _GPURESOURCES._serialized_start=866
+  _GPURESOURCES._serialized_end=1041
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -44,24 +44,52 @@
     INVALID: _GpuType.ValueType  # 0
     NVIDIA_K80: _GpuType.ValueType  # 1
     NVIDIA_V100: _GpuType.ValueType  # 2
     NVIDIA_A100: _GpuType.ValueType  # 3
     NVIDIA_T4: _GpuType.ValueType  # 4
     NVIDIA_A10G: _GpuType.ValueType  # 5
     NVIDIA_L4: _GpuType.ValueType  # 6
+    NVIDIA_T4_1_4_15: _GpuType.ValueType  # 7
+    """More specific node types
+    t4.xl
+    """
+    NVIDIA_T4_1_8_30: _GpuType.ValueType  # 8
+    """t4.2xl"""
+    NVIDIA_T4_1_16_60: _GpuType.ValueType  # 9
+    """t4.4xl"""
+    NVIDIA_A100_80GB_8_96_1360: _GpuType.ValueType  # 10
+    """a100.8xl"""
+    NVIDIA_V100_1_8_52: _GpuType.ValueType  # 11
+    """a100.xl"""
+    NVIDIA_V100_4_32_208: _GpuType.ValueType  # 12
+    """v100.4xl"""
 
 class GpuType(_GpuType, metaclass=_GpuTypeEnumTypeWrapper): ...
 
 INVALID: GpuType.ValueType  # 0
 NVIDIA_K80: GpuType.ValueType  # 1
 NVIDIA_V100: GpuType.ValueType  # 2
 NVIDIA_A100: GpuType.ValueType  # 3
 NVIDIA_T4: GpuType.ValueType  # 4
 NVIDIA_A10G: GpuType.ValueType  # 5
 NVIDIA_L4: GpuType.ValueType  # 6
+NVIDIA_T4_1_4_15: GpuType.ValueType  # 7
+"""More specific node types
+t4.xl
+"""
+NVIDIA_T4_1_8_30: GpuType.ValueType  # 8
+"""t4.2xl"""
+NVIDIA_T4_1_16_60: GpuType.ValueType  # 9
+"""t4.4xl"""
+NVIDIA_A100_80GB_8_96_1360: GpuType.ValueType  # 10
+"""a100.8xl"""
+NVIDIA_V100_1_8_52: GpuType.ValueType  # 11
+"""a100.xl"""
+NVIDIA_V100_4_32_208: GpuType.ValueType  # 12
+"""v100.4xl"""
 global___GpuType = GpuType
 
 class BuildProperties(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BUILD_ID_FIELD_NUMBER: builtins.int
     BRANCH_FIELD_NUMBER: builtins.int
@@ -156,34 +184,38 @@
 class DockerEnv(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BASE_IMAGE_FIELD_NUMBER: builtins.int
     ENV_VARS_FIELD_NUMBER: builtins.int
     NO_CACHE_FIELD_NUMBER: builtins.int
     ASSUMED_IAM_ROLE_ARN_FIELD_NUMBER: builtins.int
+    SERVICE_ACCOUNT_KEY_SECRET_NAME_FIELD_NUMBER: builtins.int
     base_image: builtins.str
     """Base image to use for serving"""
     @property
     def env_vars(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Environment variables for the model code"""
     no_cache: builtins.bool
     """Don't use remote cache to build the images, defaults to use cache,
     if the model dependencies changed significantly it could be faster and better to run with no cache
     """
     assumed_iam_role_arn: builtins.str
     """Custom IAM role to be assumed by model"""
+    service_account_key_secret_name: builtins.str
+    """Service account key secret name for gcp"""
     def __init__(
         self,
         *,
         base_image: builtins.str = ...,
         env_vars: collections.abc.Iterable[builtins.str] | None = ...,
         no_cache: builtins.bool = ...,
         assumed_iam_role_arn: builtins.str = ...,
+        service_account_key_secret_name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["assumed_iam_role_arn", b"assumed_iam_role_arn", "base_image", b"base_image", "env_vars", b"env_vars", "no_cache", b"no_cache"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["assumed_iam_role_arn", b"assumed_iam_role_arn", "base_image", b"base_image", "env_vars", b"env_vars", "no_cache", b"no_cache", "service_account_key_secret_name", b"service_account_key_secret_name"]) -> None: ...
 
 global___DockerEnv = DockerEnv
 
 class PythonEnv(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GIT_CREDENTIALS_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.qwak/instance_template/instance_template.proto\x12!qwak.management.instance_template\x1a/qwak/user_application/common/v0/resources.proto\"\x82\x02\n\x14InstanceTemplateSpec\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\r\n\x05order\x18\x03 \x01(\x05\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12S\n\x15pod_compute_resources\x18\x05 \x01(\x0b\x32\x34.qwak.user_application.common.v0.PodComputeResources\x12\x46\n\rinstance_type\x18\x06 \x01(\x0e\x32/.qwak.management.instance_template.InstanceType\x12\x0b\n\x03qpu\x18\x07 \x01(\x02\"e\n\x0eInstanceFilter\x12S\n\x14instance_type_filter\x18\x01 \x01(\x0e\x32\x35.qwak.management.instance_template.InstanceTypeFilter*\x94\x01\n\x12InstanceTypeFilter\x12$\n INSTANCE_TYPE_FILTER_UNSPECIFIED\x10\x00\x12\x1c\n\x18INSTANCE_TYPE_FILTER_ALL\x10\x01\x12\x1c\n\x18INSTANCE_TYPE_FILTER_CPU\x10\x02\x12\x1c\n\x18INSTANCE_TYPE_FILTER_GPU\x10\x03*[\n\x0cInstanceType\x12\x1d\n\x19INSTANCE_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11INSTANCE_TYPE_CPU\x10\x01\x12\x15\n\x11INSTANCE_TYPE_GPU\x10\x02\x42\x30\n,com.qwak.ai.management.instance_template.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.qwak/instance_template/instance_template.proto\x12!qwak.management.instance_template\x1a/qwak/user_application/common/v0/resources.proto\"\xb0\x02\n\x14InstanceTemplateSpec\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\r\n\x05order\x18\x03 \x01(\x05\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12S\n\x15pod_compute_resources\x18\x05 \x01(\x0b\x32\x34.qwak.user_application.common.v0.PodComputeResources\x12\x46\n\rinstance_type\x18\x06 \x01(\x0e\x32/.qwak.management.instance_template.InstanceType\x12\x0b\n\x03qpu\x18\x07 \x01(\x02\x12\x15\n\raws_supported\x18\x08 \x01(\x08\x12\x15\n\rgcp_supported\x18\t \x01(\x08\"e\n\x0eInstanceFilter\x12S\n\x14instance_type_filter\x18\x01 \x01(\x0e\x32\x35.qwak.management.instance_template.InstanceTypeFilter*\x94\x01\n\x12InstanceTypeFilter\x12$\n INSTANCE_TYPE_FILTER_UNSPECIFIED\x10\x00\x12\x1c\n\x18INSTANCE_TYPE_FILTER_ALL\x10\x01\x12\x1c\n\x18INSTANCE_TYPE_FILTER_CPU\x10\x02\x12\x1c\n\x18INSTANCE_TYPE_FILTER_GPU\x10\x03*[\n\x0cInstanceType\x12\x1d\n\x19INSTANCE_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11INSTANCE_TYPE_CPU\x10\x01\x12\x15\n\x11INSTANCE_TYPE_GPU\x10\x02\x42\x30\n,com.qwak.ai.management.instance_template.apiP\x01\x62\x06proto3')
 
 _INSTANCETYPEFILTER = DESCRIPTOR.enum_types_by_name['InstanceTypeFilter']
 InstanceTypeFilter = enum_type_wrapper.EnumTypeWrapper(_INSTANCETYPEFILTER)
 _INSTANCETYPE = DESCRIPTOR.enum_types_by_name['InstanceType']
 InstanceType = enum_type_wrapper.EnumTypeWrapper(_INSTANCETYPE)
 INSTANCE_TYPE_FILTER_UNSPECIFIED = 0
 INSTANCE_TYPE_FILTER_ALL = 1
@@ -47,16 +47,16 @@
   })
 _sym_db.RegisterMessage(InstanceFilter)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n,com.qwak.ai.management.instance_template.apiP\001'
-  _INSTANCETYPEFILTER._serialized_start=499
-  _INSTANCETYPEFILTER._serialized_end=647
-  _INSTANCETYPE._serialized_start=649
-  _INSTANCETYPE._serialized_end=740
+  _INSTANCETYPEFILTER._serialized_start=545
+  _INSTANCETYPEFILTER._serialized_end=693
+  _INSTANCETYPE._serialized_start=695
+  _INSTANCETYPE._serialized_end=786
   _INSTANCETEMPLATESPEC._serialized_start=135
-  _INSTANCETEMPLATESPEC._serialized_end=393
-  _INSTANCEFILTER._serialized_start=395
-  _INSTANCEFILTER._serialized_end=496
+  _INSTANCETEMPLATESPEC._serialized_end=439
+  _INSTANCEFILTER._serialized_start=441
+  _INSTANCEFILTER._serialized_end=542
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -59,35 +59,41 @@
     ID_FIELD_NUMBER: builtins.int
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     ORDER_FIELD_NUMBER: builtins.int
     ENABLED_FIELD_NUMBER: builtins.int
     POD_COMPUTE_RESOURCES_FIELD_NUMBER: builtins.int
     INSTANCE_TYPE_FIELD_NUMBER: builtins.int
     QPU_FIELD_NUMBER: builtins.int
+    AWS_SUPPORTED_FIELD_NUMBER: builtins.int
+    GCP_SUPPORTED_FIELD_NUMBER: builtins.int
     id: builtins.str
     display_name: builtins.str
     order: builtins.int
     enabled: builtins.bool
     @property
     def pod_compute_resources(self) -> qwak.user_application.common.v0.resources_pb2.PodComputeResources: ...
     instance_type: global___InstanceType.ValueType
     qpu: builtins.float
+    aws_supported: builtins.bool
+    gcp_supported: builtins.bool
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         display_name: builtins.str = ...,
         order: builtins.int = ...,
         enabled: builtins.bool = ...,
         pod_compute_resources: qwak.user_application.common.v0.resources_pb2.PodComputeResources | None = ...,
         instance_type: global___InstanceType.ValueType = ...,
         qpu: builtins.float = ...,
+        aws_supported: builtins.bool = ...,
+        gcp_supported: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pod_compute_resources", b"pod_compute_resources"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "enabled", b"enabled", "id", b"id", "instance_type", b"instance_type", "order", b"order", "pod_compute_resources", b"pod_compute_resources", "qpu", b"qpu"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["aws_supported", b"aws_supported", "display_name", b"display_name", "enabled", b"enabled", "gcp_supported", b"gcp_supported", "id", b"id", "instance_type", b"instance_type", "order", b"order", "pod_compute_resources", b"pod_compute_resources", "qpu", b"qpu"]) -> None: ...
 
 global___InstanceTemplateSpec = InstanceTemplateSpec
 
 class InstanceFilter(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INSTANCE_TYPE_FILTER_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,qwak/kube_deployment_captain/batch_job.proto\x12\x1cqwak.kube.deployment.captain\"\xdb\x02\n\x1cListInferenceJobFilesRequest\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x16\n\x0e\x64irectory_path\x18\x02 \x01(\t\x12\x18\n\x0ctoken_secret\x18\x03 \x01(\tB\x02\x18\x01\x12\x19\n\rsecret_secret\x18\x04 \x01(\tB\x02\x18\x01\x12\x1a\n\x12secret_service_url\x18\x05 \x01(\t\x12\x14\n\x08role_arn\x18\x06 \x01(\tB\x02\x18\x01\x12G\n\x0f\x61ws_credentials\x18\x07 \x01(\x0b\x32,.qwak.kube.deployment.captain.AwsCredentialsH\x00\x12G\n\x0fgcp_credentials\x18\x08 \x01(\x0b\x32,.qwak.kube.deployment.captain.GcpCredentialsH\x00\x42\x1a\n\x18\x63loud_client_credentials\"O\n\x0e\x41wsCredentials\x12\x10\n\x08role_arn\x18\x01 \x01(\t\x12\x14\n\x0ctoken_secret\x18\x02 \x01(\t\x12\x15\n\rsecret_secret\x18\x04 \x01(\t\"9\n\x0eGcpCredentials\x12\'\n\x1fservice_account_json_key_secret\x18\x01 \x01(\t\"\\\n\x1dListInferenceJobFilesResponse\x12\x12\n\nfile_names\x18\x01 \x03(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x03 \x01(\t\"\xf0\x01\n\"CreateInferenceTaskExecutorRequest\x12\x63\n\x1btask_executor_configuration\x18\x01 \x01(\x0b\x32>.qwak.kube.deployment.captain.TaskExecutorConfigurationMessage\x12\x65\n\x1cinference_task_configuration\x18\x02 \x01(\x0b\x32?.qwak.kube.deployment.captain.InferenceTaskConfigurationMessage\"\x89\x01\n\x1aPrepareInferenceJobRequest\x12k\n#inference_job_configuration_message\x18\x01 \x01(\x0b\x32>.qwak.kube.deployment.captain.InferenceJobConfigurationMessage\"F\n\x1bPrepareInferenceJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"\xe9\x03\n TaskExecutorConfigurationMessage\x12\x18\n\x10inference_job_id\x18\x01 \x01(\t\x12\x19\n\x11inference_task_id\x18\x02 \x01(\t\x12G\n\x10model_identifier\x18\x05 \x01(\x0b\x32-.qwak.kube.deployment.captain.ModelIdentifier\x12\x11\n\timage_url\x18\x06 \x01(\t\x12\x15\n\rbackoff_limit\x18\x07 \x01(\x05\x12\x0f\n\x03\x63pu\x18\x08 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\t \x01(\x05\x42\x02\x18\x01\x12\x45\n\x0cmemory_units\x18\n \x01(\x0e\x32+.qwak.kube.deployment.captain.MemoryUnitApiB\x02\x18\x01\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x0c \x01(\t\x12\x41\n\x08job_size\x18\r \x01(\x0b\x32/.qwak.kube.deployment.captain.BatchJobResources\x12\x17\n\x0fpurchase_option\x18\x0e \x01(\t\x12\x19\n\x11image_pull_secret\x18\x0f \x01(\t\"q\n InferenceJobConfigurationMessage\x12\x18\n\x10inference_job_id\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x02 \x01(\t\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x03 \x01(\t\"`\n\x0fModelIdentifier\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x15\n\tbranch_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x12\n\nmodel_uuid\x18\x04 \x01(\t\"\xf0\x03\n!InferenceTaskConfigurationMessage\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x02 \x01(\t\x12\x10\n\x08\x66ilepath\x18\x03 \x01(\t\x12\x18\n\x10\x64\x65stination_path\x18\x04 \x01(\t\x12\x44\n\x0finput_file_type\x18\x05 \x01(\x0e\x32+.qwak.kube.deployment.captain.InputFileType\x12\x46\n\x10output_file_type\x18\x06 \x01(\x0e\x32,.qwak.kube.deployment.captain.OutputFileType\x12\x14\n\x0ctoken_secret\x18\x07 \x01(\t\x12\x15\n\rsecret_secret\x18\x08 \x01(\t\x12\x43\n\nparameters\x18\t \x03(\x0b\x32/.qwak.kube.deployment.captain.BatchJobParameter\x12\x43\n\x0e\x63loud_provider\x18\n \x01(\x0e\x32+.qwak.kube.deployment.captain.CloudProvider\x12\'\n\x1fservice_account_json_key_secret\x18\x0b \x01(\t\"/\n\x11\x42\x61tchJobParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"?\n#CleanInferenceTasksExecutorsRequest\x12\x18\n\x10inference_job_id\x18\x01 \x01(\t\"O\n$CleanInferenceTasksExecutorsResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"X\n!CleanInferenceTaskExecutorRequest\x12\x18\n\x10inference_job_id\x18\x01 \x01(\t\x12\x19\n\x11inference_task_id\x18\x02 \x01(\t\"M\n\"CleanInferenceTaskExecutorResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"N\n#CreateInferenceTaskExecutorResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"\xf7\x02\n\x1eStartInferenceJobWarmupRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x11\n\timage_url\x18\x04 \x01(\t\x12\x0f\n\x03\x63pu\x18\x05 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x06 \x01(\x05\x42\x02\x18\x01\x12\x45\n\x0cmemory_units\x18\x07 \x01(\x0e\x32+.qwak.kube.deployment.captain.MemoryUnitApiB\x02\x18\x01\x12\x11\n\texecutors\x18\x08 \x01(\x05\x12\x0f\n\x07timeout\x18\t \x01(\x05\x12\x41\n\x08job_size\x18\n \x01(\x0b\x32/.qwak.kube.deployment.captain.BatchJobResources\x12\x12\n\nmodel_uuid\x18\x0b \x01(\t\x12\x19\n\x11image_pull_secret\x18\x0c \x01(\t\"!\n\x1fStartInferenceJobWarmupResponse\"p\n\x1f\x43\x61ncelInferenceJobWarmupRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x12\n\nmodel_uuid\x18\x04 \x01(\t\"\"\n CancelInferenceJobWarmupResponse\"\xd5\x01\n\x11\x42\x61tchJobResources\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x15\n\rmemory_amount\x18\x03 \x01(\x05\x12\x41\n\x0cmemory_units\x18\x04 \x01(\x0e\x32+.qwak.kube.deployment.captain.MemoryUnitApi\x12\x41\n\rgpu_resources\x18\x05 \x01(\x0b\x32*.qwak.kube.deployment.captain.GpuResources\"[\n\x0cGpuResources\x12\x37\n\x08gpu_type\x18\x01 \x01(\x0e\x32%.qwak.kube.deployment.captain.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05*:\n\rMemoryUnitApi\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x81\x01\n\rInputFileType\x12\x1d\n\x19UNDEFINED_INPUT_FILE_TYPE\x10\x00\x12\x17\n\x13\x43SV_INPUT_FILE_TYPE\x10\x01\x12\x1b\n\x17\x46\x45\x41THER_INPUT_FILE_TYPE\x10\x02\x12\x1b\n\x17PARQUET_INPUT_FILE_TYPE\x10\x03*\x86\x01\n\x0eOutputFileType\x12\x1e\n\x1aUNDEFINED_OUTPUT_FILE_TYPE\x10\x00\x12\x18\n\x14\x43SV_OUTPUT_FILE_TYPE\x10\x01\x12\x1c\n\x18\x46\x45\x41THER_OUTPUT_FILE_TYPE\x10\x02\x12\x1c\n\x18PARQUET_OUTPUT_FILE_TYPE\x10\x03*{\n\x07GpuType\x12\x0f\n\x0bINVALID_GPU\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06*=\n\rCloudProvider\x12\x1a\n\x16UNKNOWN_CLOUD_PROVIDER\x10\x00\x12\x07\n\x03\x41WS\x10\x01\x12\x07\n\x03GCP\x10\x02\x42+\n\'com.qwak.ai.kube.deployment.captain.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,qwak/kube_deployment_captain/batch_job.proto\x12\x1cqwak.kube.deployment.captain\"\xdb\x02\n\x1cListInferenceJobFilesRequest\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x16\n\x0e\x64irectory_path\x18\x02 \x01(\t\x12\x18\n\x0ctoken_secret\x18\x03 \x01(\tB\x02\x18\x01\x12\x19\n\rsecret_secret\x18\x04 \x01(\tB\x02\x18\x01\x12\x1a\n\x12secret_service_url\x18\x05 \x01(\t\x12\x14\n\x08role_arn\x18\x06 \x01(\tB\x02\x18\x01\x12G\n\x0f\x61ws_credentials\x18\x07 \x01(\x0b\x32,.qwak.kube.deployment.captain.AwsCredentialsH\x00\x12G\n\x0fgcp_credentials\x18\x08 \x01(\x0b\x32,.qwak.kube.deployment.captain.GcpCredentialsH\x00\x42\x1a\n\x18\x63loud_client_credentials\"O\n\x0e\x41wsCredentials\x12\x10\n\x08role_arn\x18\x01 \x01(\t\x12\x14\n\x0ctoken_secret\x18\x02 \x01(\t\x12\x15\n\rsecret_secret\x18\x04 \x01(\t\"9\n\x0eGcpCredentials\x12\'\n\x1fservice_account_json_key_secret\x18\x01 \x01(\t\"\\\n\x1dListInferenceJobFilesResponse\x12\x12\n\nfile_names\x18\x01 \x03(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x03 \x01(\t\"\xf0\x01\n\"CreateInferenceTaskExecutorRequest\x12\x63\n\x1btask_executor_configuration\x18\x01 \x01(\x0b\x32>.qwak.kube.deployment.captain.TaskExecutorConfigurationMessage\x12\x65\n\x1cinference_task_configuration\x18\x02 \x01(\x0b\x32?.qwak.kube.deployment.captain.InferenceTaskConfigurationMessage\"\x89\x01\n\x1aPrepareInferenceJobRequest\x12k\n#inference_job_configuration_message\x18\x01 \x01(\x0b\x32>.qwak.kube.deployment.captain.InferenceJobConfigurationMessage\"F\n\x1bPrepareInferenceJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"\x90\x04\n TaskExecutorConfigurationMessage\x12\x18\n\x10inference_job_id\x18\x01 \x01(\t\x12\x19\n\x11inference_task_id\x18\x02 \x01(\t\x12G\n\x10model_identifier\x18\x05 \x01(\x0b\x32-.qwak.kube.deployment.captain.ModelIdentifier\x12\x11\n\timage_url\x18\x06 \x01(\t\x12\x15\n\rbackoff_limit\x18\x07 \x01(\x05\x12\x0f\n\x03\x63pu\x18\x08 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\t \x01(\x05\x42\x02\x18\x01\x12\x45\n\x0cmemory_units\x18\n \x01(\x0e\x32+.qwak.kube.deployment.captain.MemoryUnitApiB\x02\x18\x01\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x0c \x01(\t\x12\x41\n\x08job_size\x18\r \x01(\x0b\x32/.qwak.kube.deployment.captain.BatchJobResources\x12\x17\n\x0fpurchase_option\x18\x0e \x01(\t\x12\x19\n\x11image_pull_secret\x18\x0f \x01(\t\x12%\n\x1d\x63ustom_service_account_secret\x18\x10 \x01(\t\"q\n InferenceJobConfigurationMessage\x12\x18\n\x10inference_job_id\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x02 \x01(\t\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x03 \x01(\t\"`\n\x0fModelIdentifier\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x15\n\tbranch_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x12\n\nmodel_uuid\x18\x04 \x01(\t\"\xf0\x03\n!InferenceTaskConfigurationMessage\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x02 \x01(\t\x12\x10\n\x08\x66ilepath\x18\x03 \x01(\t\x12\x18\n\x10\x64\x65stination_path\x18\x04 \x01(\t\x12\x44\n\x0finput_file_type\x18\x05 \x01(\x0e\x32+.qwak.kube.deployment.captain.InputFileType\x12\x46\n\x10output_file_type\x18\x06 \x01(\x0e\x32,.qwak.kube.deployment.captain.OutputFileType\x12\x14\n\x0ctoken_secret\x18\x07 \x01(\t\x12\x15\n\rsecret_secret\x18\x08 \x01(\t\x12\x43\n\nparameters\x18\t \x03(\x0b\x32/.qwak.kube.deployment.captain.BatchJobParameter\x12\x43\n\x0e\x63loud_provider\x18\n \x01(\x0e\x32+.qwak.kube.deployment.captain.CloudProvider\x12\'\n\x1fservice_account_json_key_secret\x18\x0b \x01(\t\"/\n\x11\x42\x61tchJobParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"?\n#CleanInferenceTasksExecutorsRequest\x12\x18\n\x10inference_job_id\x18\x01 \x01(\t\"O\n$CleanInferenceTasksExecutorsResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"X\n!CleanInferenceTaskExecutorRequest\x12\x18\n\x10inference_job_id\x18\x01 \x01(\t\x12\x19\n\x11inference_task_id\x18\x02 \x01(\t\"M\n\"CleanInferenceTaskExecutorResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"N\n#CreateInferenceTaskExecutorResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x16\n\x0e\x66\x61ilure_reason\x18\x02 \x01(\t\"\xf7\x02\n\x1eStartInferenceJobWarmupRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x11\n\timage_url\x18\x04 \x01(\t\x12\x0f\n\x03\x63pu\x18\x05 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x06 \x01(\x05\x42\x02\x18\x01\x12\x45\n\x0cmemory_units\x18\x07 \x01(\x0e\x32+.qwak.kube.deployment.captain.MemoryUnitApiB\x02\x18\x01\x12\x11\n\texecutors\x18\x08 \x01(\x05\x12\x0f\n\x07timeout\x18\t \x01(\x05\x12\x41\n\x08job_size\x18\n \x01(\x0b\x32/.qwak.kube.deployment.captain.BatchJobResources\x12\x12\n\nmodel_uuid\x18\x0b \x01(\t\x12\x19\n\x11image_pull_secret\x18\x0c \x01(\t\"!\n\x1fStartInferenceJobWarmupResponse\"p\n\x1f\x43\x61ncelInferenceJobWarmupRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x12\n\nmodel_uuid\x18\x04 \x01(\t\"\"\n CancelInferenceJobWarmupResponse\"\xd5\x01\n\x11\x42\x61tchJobResources\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x15\n\rmemory_amount\x18\x03 \x01(\x05\x12\x41\n\x0cmemory_units\x18\x04 \x01(\x0e\x32+.qwak.kube.deployment.captain.MemoryUnitApi\x12\x41\n\rgpu_resources\x18\x05 \x01(\x0b\x32*.qwak.kube.deployment.captain.GpuResources\"[\n\x0cGpuResources\x12\x37\n\x08gpu_type\x18\x01 \x01(\x0e\x32%.qwak.kube.deployment.captain.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05*:\n\rMemoryUnitApi\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x81\x01\n\rInputFileType\x12\x1d\n\x19UNDEFINED_INPUT_FILE_TYPE\x10\x00\x12\x17\n\x13\x43SV_INPUT_FILE_TYPE\x10\x01\x12\x1b\n\x17\x46\x45\x41THER_INPUT_FILE_TYPE\x10\x02\x12\x1b\n\x17PARQUET_INPUT_FILE_TYPE\x10\x03*\x86\x01\n\x0eOutputFileType\x12\x1e\n\x1aUNDEFINED_OUTPUT_FILE_TYPE\x10\x00\x12\x18\n\x14\x43SV_OUTPUT_FILE_TYPE\x10\x01\x12\x1c\n\x18\x46\x45\x41THER_OUTPUT_FILE_TYPE\x10\x02\x12\x1c\n\x18PARQUET_OUTPUT_FILE_TYPE\x10\x03*\x90\x02\n\x07GpuType\x12\x0f\n\x0bINVALID_GPU\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06\x12\x14\n\x10NVIDIA_T4_1_4_15\x10\x07\x12\x14\n\x10NVIDIA_T4_1_8_30\x10\x08\x12\x15\n\x11NVIDIA_T4_1_16_60\x10\t\x12\x1e\n\x1aNVIDIA_A100_80GB_8_96_1360\x10\n\x12\x16\n\x12NVIDIA_V100_1_8_52\x10\x0b\x12\x18\n\x14NVIDIA_V100_4_32_208\x10\x0c*=\n\rCloudProvider\x12\x1a\n\x16UNKNOWN_CLOUD_PROVIDER\x10\x00\x12\x07\n\x03\x41WS\x10\x01\x12\x07\n\x03GCP\x10\x02\x42+\n\'com.qwak.ai.kube.deployment.captain.apiP\x01\x62\x06proto3')
 
 _MEMORYUNITAPI = DESCRIPTOR.enum_types_by_name['MemoryUnitApi']
 MemoryUnitApi = enum_type_wrapper.EnumTypeWrapper(_MEMORYUNITAPI)
 _INPUTFILETYPE = DESCRIPTOR.enum_types_by_name['InputFileType']
 InputFileType = enum_type_wrapper.EnumTypeWrapper(_INPUTFILETYPE)
 _OUTPUTFILETYPE = DESCRIPTOR.enum_types_by_name['OutputFileType']
 OutputFileType = enum_type_wrapper.EnumTypeWrapper(_OUTPUTFILETYPE)
@@ -41,14 +41,20 @@
 INVALID_GPU = 0
 NVIDIA_K80 = 1
 NVIDIA_V100 = 2
 NVIDIA_A100 = 3
 NVIDIA_T4 = 4
 NVIDIA_A10G = 5
 NVIDIA_L4 = 6
+NVIDIA_T4_1_4_15 = 7
+NVIDIA_T4_1_8_30 = 8
+NVIDIA_T4_1_16_60 = 9
+NVIDIA_A100_80GB_8_96_1360 = 10
+NVIDIA_V100_1_8_52 = 11
+NVIDIA_V100_4_32_208 = 12
 UNKNOWN_CLOUD_PROVIDER = 0
 AWS = 1
 GCP = 2
 
 
 _LISTINFERENCEJOBFILESREQUEST = DESCRIPTOR.message_types_by_name['ListInferenceJobFilesRequest']
 _AWSCREDENTIALS = DESCRIPTOR.message_types_by_name['AwsCredentials']
@@ -258,24 +264,24 @@
   _STARTINFERENCEJOBWARMUPREQUEST.fields_by_name['cpu']._serialized_options = b'\030\001'
   _STARTINFERENCEJOBWARMUPREQUEST.fields_by_name['memory_amount']._options = None
   _STARTINFERENCEJOBWARMUPREQUEST.fields_by_name['memory_amount']._serialized_options = b'\030\001'
   _STARTINFERENCEJOBWARMUPREQUEST.fields_by_name['memory_units']._options = None
   _STARTINFERENCEJOBWARMUPREQUEST.fields_by_name['memory_units']._serialized_options = b'\030\001'
   _CANCELINFERENCEJOBWARMUPREQUEST.fields_by_name['branch_id']._options = None
   _CANCELINFERENCEJOBWARMUPREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
-  _MEMORYUNITAPI._serialized_start=3637
-  _MEMORYUNITAPI._serialized_end=3695
-  _INPUTFILETYPE._serialized_start=3698
-  _INPUTFILETYPE._serialized_end=3827
-  _OUTPUTFILETYPE._serialized_start=3830
-  _OUTPUTFILETYPE._serialized_end=3964
-  _GPUTYPE._serialized_start=3966
-  _GPUTYPE._serialized_end=4089
-  _CLOUDPROVIDER._serialized_start=4091
-  _CLOUDPROVIDER._serialized_end=4152
+  _MEMORYUNITAPI._serialized_start=3676
+  _MEMORYUNITAPI._serialized_end=3734
+  _INPUTFILETYPE._serialized_start=3737
+  _INPUTFILETYPE._serialized_end=3866
+  _OUTPUTFILETYPE._serialized_start=3869
+  _OUTPUTFILETYPE._serialized_end=4003
+  _GPUTYPE._serialized_start=4006
+  _GPUTYPE._serialized_end=4278
+  _CLOUDPROVIDER._serialized_start=4280
+  _CLOUDPROVIDER._serialized_end=4341
   _LISTINFERENCEJOBFILESREQUEST._serialized_start=79
   _LISTINFERENCEJOBFILESREQUEST._serialized_end=426
   _AWSCREDENTIALS._serialized_start=428
   _AWSCREDENTIALS._serialized_end=507
   _GCPCREDENTIALS._serialized_start=509
   _GCPCREDENTIALS._serialized_end=566
   _LISTINFERENCEJOBFILESRESPONSE._serialized_start=568
@@ -283,39 +289,39 @@
   _CREATEINFERENCETASKEXECUTORREQUEST._serialized_start=663
   _CREATEINFERENCETASKEXECUTORREQUEST._serialized_end=903
   _PREPAREINFERENCEJOBREQUEST._serialized_start=906
   _PREPAREINFERENCEJOBREQUEST._serialized_end=1043
   _PREPAREINFERENCEJOBRESPONSE._serialized_start=1045
   _PREPAREINFERENCEJOBRESPONSE._serialized_end=1115
   _TASKEXECUTORCONFIGURATIONMESSAGE._serialized_start=1118
-  _TASKEXECUTORCONFIGURATIONMESSAGE._serialized_end=1607
-  _INFERENCEJOBCONFIGURATIONMESSAGE._serialized_start=1609
-  _INFERENCEJOBCONFIGURATIONMESSAGE._serialized_end=1722
-  _MODELIDENTIFIER._serialized_start=1724
-  _MODELIDENTIFIER._serialized_end=1820
-  _INFERENCETASKCONFIGURATIONMESSAGE._serialized_start=1823
-  _INFERENCETASKCONFIGURATIONMESSAGE._serialized_end=2319
-  _BATCHJOBPARAMETER._serialized_start=2321
-  _BATCHJOBPARAMETER._serialized_end=2368
-  _CLEANINFERENCETASKSEXECUTORSREQUEST._serialized_start=2370
-  _CLEANINFERENCETASKSEXECUTORSREQUEST._serialized_end=2433
-  _CLEANINFERENCETASKSEXECUTORSRESPONSE._serialized_start=2435
-  _CLEANINFERENCETASKSEXECUTORSRESPONSE._serialized_end=2514
-  _CLEANINFERENCETASKEXECUTORREQUEST._serialized_start=2516
-  _CLEANINFERENCETASKEXECUTORREQUEST._serialized_end=2604
-  _CLEANINFERENCETASKEXECUTORRESPONSE._serialized_start=2606
-  _CLEANINFERENCETASKEXECUTORRESPONSE._serialized_end=2683
-  _CREATEINFERENCETASKEXECUTORRESPONSE._serialized_start=2685
-  _CREATEINFERENCETASKEXECUTORRESPONSE._serialized_end=2763
-  _STARTINFERENCEJOBWARMUPREQUEST._serialized_start=2766
-  _STARTINFERENCEJOBWARMUPREQUEST._serialized_end=3141
-  _STARTINFERENCEJOBWARMUPRESPONSE._serialized_start=3143
-  _STARTINFERENCEJOBWARMUPRESPONSE._serialized_end=3176
-  _CANCELINFERENCEJOBWARMUPREQUEST._serialized_start=3178
-  _CANCELINFERENCEJOBWARMUPREQUEST._serialized_end=3290
-  _CANCELINFERENCEJOBWARMUPRESPONSE._serialized_start=3292
-  _CANCELINFERENCEJOBWARMUPRESPONSE._serialized_end=3326
-  _BATCHJOBRESOURCES._serialized_start=3329
-  _BATCHJOBRESOURCES._serialized_end=3542
-  _GPURESOURCES._serialized_start=3544
-  _GPURESOURCES._serialized_end=3635
+  _TASKEXECUTORCONFIGURATIONMESSAGE._serialized_end=1646
+  _INFERENCEJOBCONFIGURATIONMESSAGE._serialized_start=1648
+  _INFERENCEJOBCONFIGURATIONMESSAGE._serialized_end=1761
+  _MODELIDENTIFIER._serialized_start=1763
+  _MODELIDENTIFIER._serialized_end=1859
+  _INFERENCETASKCONFIGURATIONMESSAGE._serialized_start=1862
+  _INFERENCETASKCONFIGURATIONMESSAGE._serialized_end=2358
+  _BATCHJOBPARAMETER._serialized_start=2360
+  _BATCHJOBPARAMETER._serialized_end=2407
+  _CLEANINFERENCETASKSEXECUTORSREQUEST._serialized_start=2409
+  _CLEANINFERENCETASKSEXECUTORSREQUEST._serialized_end=2472
+  _CLEANINFERENCETASKSEXECUTORSRESPONSE._serialized_start=2474
+  _CLEANINFERENCETASKSEXECUTORSRESPONSE._serialized_end=2553
+  _CLEANINFERENCETASKEXECUTORREQUEST._serialized_start=2555
+  _CLEANINFERENCETASKEXECUTORREQUEST._serialized_end=2643
+  _CLEANINFERENCETASKEXECUTORRESPONSE._serialized_start=2645
+  _CLEANINFERENCETASKEXECUTORRESPONSE._serialized_end=2722
+  _CREATEINFERENCETASKEXECUTORRESPONSE._serialized_start=2724
+  _CREATEINFERENCETASKEXECUTORRESPONSE._serialized_end=2802
+  _STARTINFERENCEJOBWARMUPREQUEST._serialized_start=2805
+  _STARTINFERENCEJOBWARMUPREQUEST._serialized_end=3180
+  _STARTINFERENCEJOBWARMUPRESPONSE._serialized_start=3182
+  _STARTINFERENCEJOBWARMUPRESPONSE._serialized_end=3215
+  _CANCELINFERENCEJOBWARMUPREQUEST._serialized_start=3217
+  _CANCELINFERENCEJOBWARMUPREQUEST._serialized_end=3329
+  _CANCELINFERENCEJOBWARMUPRESPONSE._serialized_start=3331
+  _CANCELINFERENCEJOBWARMUPRESPONSE._serialized_end=3365
+  _BATCHJOBRESOURCES._serialized_start=3368
+  _BATCHJOBRESOURCES._serialized_end=3581
+  _GPURESOURCES._serialized_start=3583
+  _GPURESOURCES._serialized_end=3674
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -82,24 +82,52 @@
     INVALID_GPU: _GpuType.ValueType  # 0
     NVIDIA_K80: _GpuType.ValueType  # 1
     NVIDIA_V100: _GpuType.ValueType  # 2
     NVIDIA_A100: _GpuType.ValueType  # 3
     NVIDIA_T4: _GpuType.ValueType  # 4
     NVIDIA_A10G: _GpuType.ValueType  # 5
     NVIDIA_L4: _GpuType.ValueType  # 6
+    NVIDIA_T4_1_4_15: _GpuType.ValueType  # 7
+    """More specific node types
+    t4.xl
+    """
+    NVIDIA_T4_1_8_30: _GpuType.ValueType  # 8
+    """t4.2xl"""
+    NVIDIA_T4_1_16_60: _GpuType.ValueType  # 9
+    """t4.4xl"""
+    NVIDIA_A100_80GB_8_96_1360: _GpuType.ValueType  # 10
+    """a100.8xl"""
+    NVIDIA_V100_1_8_52: _GpuType.ValueType  # 11
+    """a100.xl"""
+    NVIDIA_V100_4_32_208: _GpuType.ValueType  # 12
+    """v100.4xl"""
 
 class GpuType(_GpuType, metaclass=_GpuTypeEnumTypeWrapper): ...
 
 INVALID_GPU: GpuType.ValueType  # 0
 NVIDIA_K80: GpuType.ValueType  # 1
 NVIDIA_V100: GpuType.ValueType  # 2
 NVIDIA_A100: GpuType.ValueType  # 3
 NVIDIA_T4: GpuType.ValueType  # 4
 NVIDIA_A10G: GpuType.ValueType  # 5
 NVIDIA_L4: GpuType.ValueType  # 6
+NVIDIA_T4_1_4_15: GpuType.ValueType  # 7
+"""More specific node types
+t4.xl
+"""
+NVIDIA_T4_1_8_30: GpuType.ValueType  # 8
+"""t4.2xl"""
+NVIDIA_T4_1_16_60: GpuType.ValueType  # 9
+"""t4.4xl"""
+NVIDIA_A100_80GB_8_96_1360: GpuType.ValueType  # 10
+"""a100.8xl"""
+NVIDIA_V100_1_8_52: GpuType.ValueType  # 11
+"""a100.xl"""
+NVIDIA_V100_4_32_208: GpuType.ValueType  # 12
+"""v100.4xl"""
 global___GpuType = GpuType
 
 class _CloudProvider:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _CloudProviderEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_CloudProvider.ValueType], builtins.type):  # noqa: F821
@@ -288,14 +316,15 @@
     MEMORY_AMOUNT_FIELD_NUMBER: builtins.int
     MEMORY_UNITS_FIELD_NUMBER: builtins.int
     ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
     CUSTOM_IAM_ROLE_ARN_FIELD_NUMBER: builtins.int
     JOB_SIZE_FIELD_NUMBER: builtins.int
     PURCHASE_OPTION_FIELD_NUMBER: builtins.int
     IMAGE_PULL_SECRET_FIELD_NUMBER: builtins.int
+    CUSTOM_SERVICE_ACCOUNT_SECRET_FIELD_NUMBER: builtins.int
     inference_job_id: builtins.str
     """The id of the inference job"""
     inference_task_id: builtins.str
     """The id of the current inference task"""
     @property
     def model_identifier(self) -> global___ModelIdentifier:
         """Model details"""
@@ -313,14 +342,16 @@
     custom_iam_role_arn: builtins.str
     @property
     def job_size(self) -> global___BatchJobResources: ...
     purchase_option: builtins.str
     """Whether it is spot/ondemand (default - spot)"""
     image_pull_secret: builtins.str
     """If the image saved in out source repository (jfrog e.g.)  and image pull secret is needed"""
+    custom_service_account_secret: builtins.str
+    """The custom service account json key secret for gcp"""
     def __init__(
         self,
         *,
         inference_job_id: builtins.str = ...,
         inference_task_id: builtins.str = ...,
         model_identifier: global___ModelIdentifier | None = ...,
         image_url: builtins.str = ...,
@@ -329,17 +360,18 @@
         memory_amount: builtins.int = ...,
         memory_units: global___MemoryUnitApi.ValueType = ...,
         environment_id: builtins.str = ...,
         custom_iam_role_arn: builtins.str = ...,
         job_size: global___BatchJobResources | None = ...,
         purchase_option: builtins.str = ...,
         image_pull_secret: builtins.str = ...,
+        custom_service_account_secret: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["job_size", b"job_size", "model_identifier", b"model_identifier"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["backoff_limit", b"backoff_limit", "cpu", b"cpu", "custom_iam_role_arn", b"custom_iam_role_arn", "environment_id", b"environment_id", "image_pull_secret", b"image_pull_secret", "image_url", b"image_url", "inference_job_id", b"inference_job_id", "inference_task_id", b"inference_task_id", "job_size", b"job_size", "memory_amount", b"memory_amount", "memory_units", b"memory_units", "model_identifier", b"model_identifier", "purchase_option", b"purchase_option"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["backoff_limit", b"backoff_limit", "cpu", b"cpu", "custom_iam_role_arn", b"custom_iam_role_arn", "custom_service_account_secret", b"custom_service_account_secret", "environment_id", b"environment_id", "image_pull_secret", b"image_pull_secret", "image_url", b"image_url", "inference_job_id", b"inference_job_id", "inference_task_id", b"inference_task_id", "job_size", b"job_size", "memory_amount", b"memory_amount", "memory_units", b"memory_units", "model_identifier", b"model_identifier", "purchase_option", b"purchase_option"]) -> None: ...
 
 global___TaskExecutorConfigurationMessage = TaskExecutorConfigurationMessage
 
 class InferenceJobConfigurationMessage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INFERENCE_JOB_ID_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-qwak/kube_deployment_captain/deployment.proto\x12\x1cqwak.kube.deployment.captain\x1a\x1egoogle/protobuf/wrappers.proto\"\x84\x02\n\x1dKubeAdvancedDeploymentOptions\x12\x19\n\x11number_of_workers\x18\x01 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x02 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x04 \x01(\t\x12\x16\n\x0emax_batch_size\x18\x05 \x01(\x05\x12(\n deployment_process_timeout_limit\x18\x06 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x07 \x01(\t\"\xaf\x01\n\x13KubeServingStrategy\x12G\n\x0frealtime_config\x18\x01 \x01(\x0b\x32,.qwak.kube.deployment.captain.RealTimeConfigH\x00\x12\x43\n\rstream_config\x18\x02 \x01(\x0b\x32*.qwak.kube.deployment.captain.StreamConfigH\x00\x42\n\n\x08Strategy\"\xb5\x01\n\x0f\x41utoScalingSpec\x12\x19\n\x11min_replica_count\x18\x01 \x01(\x05\x12\x19\n\x11max_replica_count\x18\x02 \x01(\x05\x12\x18\n\x10polling_interval\x18\x03 \x01(\x05\x12\x18\n\x10\x63ool_down_period\x18\x04 \x01(\x05\x12\x38\n\x08triggers\x18\x05 \x03(\x0b\x32&.qwak.kube.deployment.captain.Triggers\"i\n\x08Triggers\x12M\n\x12prometheus_trigger\x18\x01 \x01(\x0b\x32/.qwak.kube.deployment.captain.PrometheusTriggerH\x00\x42\x0e\n\x0ctrigger_type\"J\n\x11PrometheusTrigger\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\x12\x11\n\tthreshold\x18\x02 \x01(\x05\x12\r\n\x05query\x18\x03 \x01(\t\"W\n\x0eRealTimeConfig\x12\'\n\x1fselected_variation_mapping_name\x18\x01 \x01(\t\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x02 \x01(\t\"[\n\x0cStreamConfig\x12:\n\x05kafka\x18\x01 \x01(\x0b\x32).qwak.kube.deployment.captain.KafkaConfigH\x00\x42\x0f\n\rconfiguration\"\xb7\x05\n\x0bKafkaConfig\x12\x44\n\x08\x63onsumer\x18\x01 \x01(\x0b\x32\x32.qwak.kube.deployment.captain.KafkaConfig.Consumer\x12\x44\n\x08producer\x18\x02 \x01(\x0b\x32\x32.qwak.kube.deployment.captain.KafkaConfig.Producer\x12\x0f\n\x07workers\x18\x03 \x01(\x05\x1a\x9b\x02\n\x08\x43onsumer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x05\x12[\n\x10\x61uto_offset_type\x18\x05 \x01(\x0e\x32\x41.qwak.kube.deployment.captain.KafkaConfig.Consumer.AutoOffSetType\x12\x16\n\x0emax_batch_size\x18\x06 \x01(\x05\x12\x18\n\x10max_poll_latency\x18\x07 \x01(\x01\"7\n\x0e\x41utoOffSetType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x45\x41RLIEST\x10\x01\x12\n\n\x06LATEST\x10\x02\x1a\xec\x01\n\x08Producer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\\\n\x10\x63ompression_type\x18\x03 \x01(\x0e\x32\x42.qwak.kube.deployment.captain.KafkaConfig.Producer.CompressionType\"Y\n\x0f\x43ompressionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0cUNCOMPRESSED\x10\x01\x12\x08\n\x04GZIP\x10\x02\x12\n\n\x06SNAPPY\x10\x03\x12\x07\n\x03LZ4\x10\x04\x12\x08\n\x04ZSTD\x10\x05\"\x93\x04\n\x12KubeDeploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x15\n\rmemory_amount\x18\x03 \x01(\x05\x12Q\n\x0cmemory_units\x18\x04 \x01(\x0e\x32;.qwak.kube.deployment.captain.KubeDeploymentSize.MemoryUnit\x12T\n\rgpu_resources\x18\x05 \x01(\x0b\x32=.qwak.kube.deployment.captain.KubeDeploymentSize.GpuResources\x1an\n\x0cGpuResources\x12J\n\x08gpu_type\x18\x01 \x01(\x0e\x32\x38.qwak.kube.deployment.captain.KubeDeploymentSize.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"{\n\x07GpuType\x12\x0f\n\x0bINVALID_GPU\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06\"+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02\"\xc3\x01\n\x1dKubeRuntimeDeploymentSettings\x12_\n\x11root_logger_level\x18\x01 \x01(\x0e\x32\x44.qwak.kube.deployment.captain.KubeRuntimeDeploymentSettings.LogLevel\"A\n\x08LogLevel\x12\x0b\n\x07NOT_SET\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x08\n\x04WARN\x10\x02\x12\x08\n\x04INFO\x10\x03\x12\t\n\x05\x44\x45\x42UG\x10\x04*;\n\x12KubeDeploymentType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08REALTIME\x10\x01\x12\n\n\x06STREAM\x10\x02\x42+\n\'com.qwak.ai.kube.deployment.captain.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-qwak/kube_deployment_captain/deployment.proto\x12\x1cqwak.kube.deployment.captain\x1a\x1egoogle/protobuf/wrappers.proto\"\x84\x02\n\x1dKubeAdvancedDeploymentOptions\x12\x19\n\x11number_of_workers\x18\x01 \x01(\x05\x12\x1f\n\x17http_request_timeout_ms\x18\x02 \x01(\x05\x12/\n\x0b\x64\x61\x65mon_mode\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x04 \x01(\t\x12\x16\n\x0emax_batch_size\x18\x05 \x01(\x05\x12(\n deployment_process_timeout_limit\x18\x06 \x01(\x05\x12\x17\n\x0fpurchase_option\x18\x07 \x01(\t\"\xaf\x01\n\x13KubeServingStrategy\x12G\n\x0frealtime_config\x18\x01 \x01(\x0b\x32,.qwak.kube.deployment.captain.RealTimeConfigH\x00\x12\x43\n\rstream_config\x18\x02 \x01(\x0b\x32*.qwak.kube.deployment.captain.StreamConfigH\x00\x42\n\n\x08Strategy\"\xb5\x01\n\x0f\x41utoScalingSpec\x12\x19\n\x11min_replica_count\x18\x01 \x01(\x05\x12\x19\n\x11max_replica_count\x18\x02 \x01(\x05\x12\x18\n\x10polling_interval\x18\x03 \x01(\x05\x12\x18\n\x10\x63ool_down_period\x18\x04 \x01(\x05\x12\x38\n\x08triggers\x18\x05 \x03(\x0b\x32&.qwak.kube.deployment.captain.Triggers\"i\n\x08Triggers\x12M\n\x12prometheus_trigger\x18\x01 \x01(\x0b\x32/.qwak.kube.deployment.captain.PrometheusTriggerH\x00\x42\x0e\n\x0ctrigger_type\"J\n\x11PrometheusTrigger\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\x12\x11\n\tthreshold\x18\x02 \x01(\x05\x12\r\n\x05query\x18\x03 \x01(\t\"W\n\x0eRealTimeConfig\x12\'\n\x1fselected_variation_mapping_name\x18\x01 \x01(\t\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x02 \x01(\t\"[\n\x0cStreamConfig\x12:\n\x05kafka\x18\x01 \x01(\x0b\x32).qwak.kube.deployment.captain.KafkaConfigH\x00\x42\x0f\n\rconfiguration\"\xb7\x05\n\x0bKafkaConfig\x12\x44\n\x08\x63onsumer\x18\x01 \x01(\x0b\x32\x32.qwak.kube.deployment.captain.KafkaConfig.Consumer\x12\x44\n\x08producer\x18\x02 \x01(\x0b\x32\x32.qwak.kube.deployment.captain.KafkaConfig.Producer\x12\x0f\n\x07workers\x18\x03 \x01(\x05\x1a\x9b\x02\n\x08\x43onsumer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x05\x12[\n\x10\x61uto_offset_type\x18\x05 \x01(\x0e\x32\x41.qwak.kube.deployment.captain.KafkaConfig.Consumer.AutoOffSetType\x12\x16\n\x0emax_batch_size\x18\x06 \x01(\x05\x12\x18\n\x10max_poll_latency\x18\x07 \x01(\x01\"7\n\x0e\x41utoOffSetType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x45\x41RLIEST\x10\x01\x12\n\n\x06LATEST\x10\x02\x1a\xec\x01\n\x08Producer\x12\x18\n\x10\x62ootstrap_server\x18\x01 \x03(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\\\n\x10\x63ompression_type\x18\x03 \x01(\x0e\x32\x42.qwak.kube.deployment.captain.KafkaConfig.Producer.CompressionType\"Y\n\x0f\x43ompressionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0cUNCOMPRESSED\x10\x01\x12\x08\n\x04GZIP\x10\x02\x12\n\n\x06SNAPPY\x10\x03\x12\x07\n\x03LZ4\x10\x04\x12\x08\n\x04ZSTD\x10\x05\"\xa9\x05\n\x12KubeDeploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x15\n\rmemory_amount\x18\x03 \x01(\x05\x12Q\n\x0cmemory_units\x18\x04 \x01(\x0e\x32;.qwak.kube.deployment.captain.KubeDeploymentSize.MemoryUnit\x12T\n\rgpu_resources\x18\x05 \x01(\x0b\x32=.qwak.kube.deployment.captain.KubeDeploymentSize.GpuResources\x1an\n\x0cGpuResources\x12J\n\x08gpu_type\x18\x01 \x01(\x0e\x32\x38.qwak.kube.deployment.captain.KubeDeploymentSize.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x90\x02\n\x07GpuType\x12\x0f\n\x0bINVALID_GPU\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06\x12\x14\n\x10NVIDIA_T4_1_4_15\x10\x07\x12\x14\n\x10NVIDIA_T4_1_8_30\x10\x08\x12\x15\n\x11NVIDIA_T4_1_16_60\x10\t\x12\x1e\n\x1aNVIDIA_A100_80GB_8_96_1360\x10\n\x12\x16\n\x12NVIDIA_V100_1_8_52\x10\x0b\x12\x18\n\x14NVIDIA_V100_4_32_208\x10\x0c\"+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02\"\xc3\x01\n\x1dKubeRuntimeDeploymentSettings\x12_\n\x11root_logger_level\x18\x01 \x01(\x0e\x32\x44.qwak.kube.deployment.captain.KubeRuntimeDeploymentSettings.LogLevel\"A\n\x08LogLevel\x12\x0b\n\x07NOT_SET\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x08\n\x04WARN\x10\x02\x12\x08\n\x04INFO\x10\x03\x12\t\n\x05\x44\x45\x42UG\x10\x04*;\n\x12KubeDeploymentType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08REALTIME\x10\x01\x12\n\n\x06STREAM\x10\x02\x42+\n\'com.qwak.ai.kube.deployment.captain.apiP\x01\x62\x06proto3')
 
 _KUBEDEPLOYMENTTYPE = DESCRIPTOR.enum_types_by_name['KubeDeploymentType']
 KubeDeploymentType = enum_type_wrapper.EnumTypeWrapper(_KUBEDEPLOYMENTTYPE)
 UNKNOWN = 0
 REALTIME = 1
 STREAM = 2
 
@@ -137,16 +137,16 @@
   })
 _sym_db.RegisterMessage(KubeRuntimeDeploymentSettings)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\'com.qwak.ai.kube.deployment.captain.apiP\001'
-  _KUBEDEPLOYMENTTYPE._serialized_start=2531
-  _KUBEDEPLOYMENTTYPE._serialized_end=2590
+  _KUBEDEPLOYMENTTYPE._serialized_start=2681
+  _KUBEDEPLOYMENTTYPE._serialized_end=2740
   _KUBEADVANCEDDEPLOYMENTOPTIONS._serialized_start=112
   _KUBEADVANCEDDEPLOYMENTOPTIONS._serialized_end=372
   _KUBESERVINGSTRATEGY._serialized_start=375
   _KUBESERVINGSTRATEGY._serialized_end=550
   _AUTOSCALINGSPEC._serialized_start=553
   _AUTOSCALINGSPEC._serialized_end=734
   _TRIGGERS._serialized_start=736
@@ -164,19 +164,19 @@
   _KAFKACONFIG_CONSUMER_AUTOOFFSETTYPE._serialized_start=1503
   _KAFKACONFIG_CONSUMER_AUTOOFFSETTYPE._serialized_end=1558
   _KAFKACONFIG_PRODUCER._serialized_start=1561
   _KAFKACONFIG_PRODUCER._serialized_end=1797
   _KAFKACONFIG_PRODUCER_COMPRESSIONTYPE._serialized_start=1708
   _KAFKACONFIG_PRODUCER_COMPRESSIONTYPE._serialized_end=1797
   _KUBEDEPLOYMENTSIZE._serialized_start=1800
-  _KUBEDEPLOYMENTSIZE._serialized_end=2331
+  _KUBEDEPLOYMENTSIZE._serialized_end=2481
   _KUBEDEPLOYMENTSIZE_GPURESOURCES._serialized_start=2051
   _KUBEDEPLOYMENTSIZE_GPURESOURCES._serialized_end=2161
-  _KUBEDEPLOYMENTSIZE_GPUTYPE._serialized_start=2163
-  _KUBEDEPLOYMENTSIZE_GPUTYPE._serialized_end=2286
-  _KUBEDEPLOYMENTSIZE_MEMORYUNIT._serialized_start=2288
-  _KUBEDEPLOYMENTSIZE_MEMORYUNIT._serialized_end=2331
-  _KUBERUNTIMEDEPLOYMENTSETTINGS._serialized_start=2334
-  _KUBERUNTIMEDEPLOYMENTSETTINGS._serialized_end=2529
-  _KUBERUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_start=2464
-  _KUBERUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_end=2529
+  _KUBEDEPLOYMENTSIZE_GPUTYPE._serialized_start=2164
+  _KUBEDEPLOYMENTSIZE_GPUTYPE._serialized_end=2436
+  _KUBEDEPLOYMENTSIZE_MEMORYUNIT._serialized_start=2438
+  _KUBEDEPLOYMENTSIZE_MEMORYUNIT._serialized_end=2481
+  _KUBERUNTIMEDEPLOYMENTSETTINGS._serialized_start=2484
+  _KUBERUNTIMEDEPLOYMENTSETTINGS._serialized_end=2679
+  _KUBERUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_start=2614
+  _KUBERUNTIMEDEPLOYMENTSETTINGS_LOGLEVEL._serialized_end=2679
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -344,23 +344,51 @@
         INVALID_GPU: KubeDeploymentSize._GpuType.ValueType  # 0
         NVIDIA_K80: KubeDeploymentSize._GpuType.ValueType  # 1
         NVIDIA_V100: KubeDeploymentSize._GpuType.ValueType  # 2
         NVIDIA_A100: KubeDeploymentSize._GpuType.ValueType  # 3
         NVIDIA_T4: KubeDeploymentSize._GpuType.ValueType  # 4
         NVIDIA_A10G: KubeDeploymentSize._GpuType.ValueType  # 5
         NVIDIA_L4: KubeDeploymentSize._GpuType.ValueType  # 6
+        NVIDIA_T4_1_4_15: KubeDeploymentSize._GpuType.ValueType  # 7
+        """More specific node types
+        t4.xl
+        """
+        NVIDIA_T4_1_8_30: KubeDeploymentSize._GpuType.ValueType  # 8
+        """t4.2xl"""
+        NVIDIA_T4_1_16_60: KubeDeploymentSize._GpuType.ValueType  # 9
+        """t4.4xl"""
+        NVIDIA_A100_80GB_8_96_1360: KubeDeploymentSize._GpuType.ValueType  # 10
+        """a100.8xl"""
+        NVIDIA_V100_1_8_52: KubeDeploymentSize._GpuType.ValueType  # 11
+        """a100.xl"""
+        NVIDIA_V100_4_32_208: KubeDeploymentSize._GpuType.ValueType  # 12
+        """v100.4xl"""
 
     class GpuType(_GpuType, metaclass=_GpuTypeEnumTypeWrapper): ...
     INVALID_GPU: KubeDeploymentSize.GpuType.ValueType  # 0
     NVIDIA_K80: KubeDeploymentSize.GpuType.ValueType  # 1
     NVIDIA_V100: KubeDeploymentSize.GpuType.ValueType  # 2
     NVIDIA_A100: KubeDeploymentSize.GpuType.ValueType  # 3
     NVIDIA_T4: KubeDeploymentSize.GpuType.ValueType  # 4
     NVIDIA_A10G: KubeDeploymentSize.GpuType.ValueType  # 5
     NVIDIA_L4: KubeDeploymentSize.GpuType.ValueType  # 6
+    NVIDIA_T4_1_4_15: KubeDeploymentSize.GpuType.ValueType  # 7
+    """More specific node types
+    t4.xl
+    """
+    NVIDIA_T4_1_8_30: KubeDeploymentSize.GpuType.ValueType  # 8
+    """t4.2xl"""
+    NVIDIA_T4_1_16_60: KubeDeploymentSize.GpuType.ValueType  # 9
+    """t4.4xl"""
+    NVIDIA_A100_80GB_8_96_1360: KubeDeploymentSize.GpuType.ValueType  # 10
+    """a100.8xl"""
+    NVIDIA_V100_1_8_52: KubeDeploymentSize.GpuType.ValueType  # 11
+    """a100.xl"""
+    NVIDIA_V100_4_32_208: KubeDeploymentSize.GpuType.ValueType  # 12
+    """v100.4xl"""
 
     class _MemoryUnit:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
     class _MemoryUnitEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[KubeDeploymentSize._MemoryUnit.ValueType], builtins.type):  # noqa: F821
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/population_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 from _qwak_proto.qwak.administration.v0.users import user_pb2 as qwak_dot_administration_dot_v0_dot_users_dot_user__pb2
 from _qwak_proto.qwak.self_service.account.v0 import managing_account_pb2 as qwak_dot_self__service_dot_account_dot_v0_dot_managing__account__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5qwak/self_service/account/v0/account_membership.proto\x12\x1cqwak.self_service.account.v0\x1a\'qwak/administration/v0/users/user.proto\x1a\x33qwak/self_service/account/v0/managing_account.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"]\n\rInviteOptions\x12L\n\x0finvitation_spec\x18\x01 \x01(\x0b\x32\x33.qwak.self_service.account.v0.JoiningInvitationSpec\"\xa9\x02\n\x1cJoiningInvitationDescription\x12I\n\x08metadata\x18\x01 \x01(\x0b\x32\x37.qwak.self_service.account.v0.JoiningInvitationMetadata\x12\x41\n\x04spec\x18\x02 \x01(\x0b\x32\x33.qwak.self_service.account.v0.JoiningInvitationSpec\x12\x45\n\x06status\x18\x03 \x01(\x0b\x32\x35.qwak.self_service.account.v0.JoiningInvitationStatus\x12\x1e\n\x16num_of_account_members\x18\x04 \x01(\x05\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x05 \x01(\t\"\xa6\x01\n\x19JoiningInvitationMetadata\x12\x15\n\rinvitation_id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpired_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ninvited_by\x18\x04 \x01(\t\"\x98\x03\n\x15JoiningInvitationSpec\x12\x15\n\rinvitee_email\x18\x01 \x01(\t\x12?\n\x0c\x61\x63\x63ount_role\x18\x02 \x01(\x0e\x32).qwak.administration.user.QwakAccountRole\x12\x17\n\x0f\x65nvironment_ids\x18\x03 \x03(\t\x12\x19\n\x11\x65nvironment_names\x18\x04 \x03(\t\x12z\n\x1d\x65nvironment_id_to_description\x18\x05 \x03(\x0b\x32S.qwak.self_service.account.v0.JoiningInvitationSpec.EnvironmentIdToDescriptionEntry\x1aw\n\x1f\x45nvironmentIdToDescriptionEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x43\n\x05value\x18\x02 \x01(\x0b\x32\x34.qwak.self_service.account.v0.EnvironmentDescription:\x02\x38\x01\"\x97\x01\n\x17JoiningInvitationStatus\x12G\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x39.qwak.self_service.account.v0.JoiningInvitationStatusCode\x12\x33\n\x0flast_changed_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa6\x01\n\x16UserAccountDescription\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x1a\n\x12is_default_account\x18\x08 \x01(\x08\x12?\n\x0c\x61\x63\x63ount_role\x18\x02 \x01(\x0e\x32).qwak.administration.user.QwakAccountRole\x12\x19\n\x11\x65nvironment_names\x18\x03 \x03(\t\"w\n\x16\x45nvironmentDescription\x12\x18\n\x10\x65nvironment_name\x18\x01 \x01(\t\x12\x43\n\x0e\x63loud_provider\x18\x02 \x01(\x0e\x32+.qwak.self_service.account.v0.CloudProvider*\x81\x01\n\x1bJoiningInvitationStatusCode\x12*\n&JOINING_INVITATION_STATUS_CODE_INVALID\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\r\n\tCANCELLED\x10\x02\x12\x0c\n\x08\x44\x45\x43LINED\x10\x03\x12\x0c\n\x08\x41\x43\x43\x45PTED\x10\x04\x42\xb9\x01\n#com.qwak.ai.self_service.account.v0P\x01Z\x8f\x01github.com/qwak-ai/qwak-platform/services/core/java/user-management/user-management-api/pb/qwak/self_service/account/v0;self_service_account_v0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5qwak/self_service/account/v0/account_membership.proto\x12\x1cqwak.self_service.account.v0\x1a\'qwak/administration/v0/users/user.proto\x1a\x33qwak/self_service/account/v0/managing_account.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"]\n\rInviteOptions\x12L\n\x0finvitation_spec\x18\x01 \x01(\x0b\x32\x33.qwak.self_service.account.v0.JoiningInvitationSpec\"\xa9\x02\n\x1cJoiningInvitationDescription\x12I\n\x08metadata\x18\x01 \x01(\x0b\x32\x37.qwak.self_service.account.v0.JoiningInvitationMetadata\x12\x41\n\x04spec\x18\x02 \x01(\x0b\x32\x33.qwak.self_service.account.v0.JoiningInvitationSpec\x12\x45\n\x06status\x18\x03 \x01(\x0b\x32\x35.qwak.self_service.account.v0.JoiningInvitationStatus\x12\x1e\n\x16num_of_account_members\x18\x04 \x01(\x05\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x05 \x01(\t\"\xa6\x01\n\x19JoiningInvitationMetadata\x12\x15\n\rinvitation_id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpired_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ninvited_by\x18\x04 \x01(\t\"\x98\x03\n\x15JoiningInvitationSpec\x12\x15\n\rinvitee_email\x18\x01 \x01(\t\x12?\n\x0c\x61\x63\x63ount_role\x18\x02 \x01(\x0e\x32).qwak.administration.user.QwakAccountRole\x12\x17\n\x0f\x65nvironment_ids\x18\x03 \x03(\t\x12\x19\n\x11\x65nvironment_names\x18\x04 \x03(\t\x12z\n\x1d\x65nvironment_id_to_description\x18\x05 \x03(\x0b\x32S.qwak.self_service.account.v0.JoiningInvitationSpec.EnvironmentIdToDescriptionEntry\x1aw\n\x1f\x45nvironmentIdToDescriptionEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x43\n\x05value\x18\x02 \x01(\x0b\x32\x34.qwak.self_service.account.v0.EnvironmentDescription:\x02\x38\x01\"\x97\x01\n\x17JoiningInvitationStatus\x12G\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x39.qwak.self_service.account.v0.JoiningInvitationStatusCode\x12\x33\n\x0flast_changed_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x9c\x03\n\x16UserAccountDescription\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x1a\n\x12is_default_account\x18\x08 \x01(\x08\x12?\n\x0c\x61\x63\x63ount_role\x18\x02 \x01(\x0e\x32).qwak.administration.user.QwakAccountRole\x12\x19\n\x11\x65nvironment_names\x18\x03 \x03(\t\x12{\n\x1d\x65nvironment_id_to_description\x18\x04 \x03(\x0b\x32T.qwak.self_service.account.v0.UserAccountDescription.EnvironmentIdToDescriptionEntry\x1aw\n\x1f\x45nvironmentIdToDescriptionEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x43\n\x05value\x18\x02 \x01(\x0b\x32\x34.qwak.self_service.account.v0.EnvironmentDescription:\x02\x38\x01\"w\n\x16\x45nvironmentDescription\x12\x18\n\x10\x65nvironment_name\x18\x01 \x01(\t\x12\x43\n\x0e\x63loud_provider\x18\x02 \x01(\x0e\x32+.qwak.self_service.account.v0.CloudProvider*\x81\x01\n\x1bJoiningInvitationStatusCode\x12*\n&JOINING_INVITATION_STATUS_CODE_INVALID\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\r\n\tCANCELLED\x10\x02\x12\x0c\n\x08\x44\x45\x43LINED\x10\x03\x12\x0c\n\x08\x41\x43\x43\x45PTED\x10\x04\x42\xb9\x01\n#com.qwak.ai.self_service.account.v0P\x01Z\x8f\x01github.com/qwak-ai/qwak-platform/services/core/java/user-management/user-management-api/pb/qwak/self_service/account/v0;self_service_account_v0b\x06proto3')
 
 _JOININGINVITATIONSTATUSCODE = DESCRIPTOR.enum_types_by_name['JoiningInvitationStatusCode']
 JoiningInvitationStatusCode = enum_type_wrapper.EnumTypeWrapper(_JOININGINVITATIONSTATUSCODE)
 JOINING_INVITATION_STATUS_CODE_INVALID = 0
 PENDING = 1
 CANCELLED = 2
 DECLINED = 3
@@ -32,14 +32,15 @@
 _INVITEOPTIONS = DESCRIPTOR.message_types_by_name['InviteOptions']
 _JOININGINVITATIONDESCRIPTION = DESCRIPTOR.message_types_by_name['JoiningInvitationDescription']
 _JOININGINVITATIONMETADATA = DESCRIPTOR.message_types_by_name['JoiningInvitationMetadata']
 _JOININGINVITATIONSPEC = DESCRIPTOR.message_types_by_name['JoiningInvitationSpec']
 _JOININGINVITATIONSPEC_ENVIRONMENTIDTODESCRIPTIONENTRY = _JOININGINVITATIONSPEC.nested_types_by_name['EnvironmentIdToDescriptionEntry']
 _JOININGINVITATIONSTATUS = DESCRIPTOR.message_types_by_name['JoiningInvitationStatus']
 _USERACCOUNTDESCRIPTION = DESCRIPTOR.message_types_by_name['UserAccountDescription']
+_USERACCOUNTDESCRIPTION_ENVIRONMENTIDTODESCRIPTIONENTRY = _USERACCOUNTDESCRIPTION.nested_types_by_name['EnvironmentIdToDescriptionEntry']
 _ENVIRONMENTDESCRIPTION = DESCRIPTOR.message_types_by_name['EnvironmentDescription']
 InviteOptions = _reflection.GeneratedProtocolMessageType('InviteOptions', (_message.Message,), {
   'DESCRIPTOR' : _INVITEOPTIONS,
   '__module__' : 'qwak.self_service.account.v0.account_membership_pb2'
   # @@protoc_insertion_point(class_scope:qwak.self_service.account.v0.InviteOptions)
   })
 _sym_db.RegisterMessage(InviteOptions)
@@ -77,45 +78,57 @@
   'DESCRIPTOR' : _JOININGINVITATIONSTATUS,
   '__module__' : 'qwak.self_service.account.v0.account_membership_pb2'
   # @@protoc_insertion_point(class_scope:qwak.self_service.account.v0.JoiningInvitationStatus)
   })
 _sym_db.RegisterMessage(JoiningInvitationStatus)
 
 UserAccountDescription = _reflection.GeneratedProtocolMessageType('UserAccountDescription', (_message.Message,), {
+
+  'EnvironmentIdToDescriptionEntry' : _reflection.GeneratedProtocolMessageType('EnvironmentIdToDescriptionEntry', (_message.Message,), {
+    'DESCRIPTOR' : _USERACCOUNTDESCRIPTION_ENVIRONMENTIDTODESCRIPTIONENTRY,
+    '__module__' : 'qwak.self_service.account.v0.account_membership_pb2'
+    # @@protoc_insertion_point(class_scope:qwak.self_service.account.v0.UserAccountDescription.EnvironmentIdToDescriptionEntry)
+    })
+  ,
   'DESCRIPTOR' : _USERACCOUNTDESCRIPTION,
   '__module__' : 'qwak.self_service.account.v0.account_membership_pb2'
   # @@protoc_insertion_point(class_scope:qwak.self_service.account.v0.UserAccountDescription)
   })
 _sym_db.RegisterMessage(UserAccountDescription)
+_sym_db.RegisterMessage(UserAccountDescription.EnvironmentIdToDescriptionEntry)
 
 EnvironmentDescription = _reflection.GeneratedProtocolMessageType('EnvironmentDescription', (_message.Message,), {
   'DESCRIPTOR' : _ENVIRONMENTDESCRIPTION,
   '__module__' : 'qwak.self_service.account.v0.account_membership_pb2'
   # @@protoc_insertion_point(class_scope:qwak.self_service.account.v0.EnvironmentDescription)
   })
 _sym_db.RegisterMessage(EnvironmentDescription)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n#com.qwak.ai.self_service.account.v0P\001Z\217\001github.com/qwak-ai/qwak-platform/services/core/java/user-management/user-management-api/pb/qwak/self_service/account/v0;self_service_account_v0'
   _JOININGINVITATIONSPEC_ENVIRONMENTIDTODESCRIPTIONENTRY._options = None
   _JOININGINVITATIONSPEC_ENVIRONMENTIDTODESCRIPTIONENTRY._serialized_options = b'8\001'
-  _JOININGINVITATIONSTATUSCODE._serialized_start=1634
-  _JOININGINVITATIONSTATUSCODE._serialized_end=1763
+  _USERACCOUNTDESCRIPTION_ENVIRONMENTIDTODESCRIPTIONENTRY._options = None
+  _USERACCOUNTDESCRIPTION_ENVIRONMENTIDTODESCRIPTIONENTRY._serialized_options = b'8\001'
+  _JOININGINVITATIONSTATUSCODE._serialized_start=1880
+  _JOININGINVITATIONSTATUSCODE._serialized_end=2009
   _INVITEOPTIONS._serialized_start=214
   _INVITEOPTIONS._serialized_end=307
   _JOININGINVITATIONDESCRIPTION._serialized_start=310
   _JOININGINVITATIONDESCRIPTION._serialized_end=607
   _JOININGINVITATIONMETADATA._serialized_start=610
   _JOININGINVITATIONMETADATA._serialized_end=776
   _JOININGINVITATIONSPEC._serialized_start=779
   _JOININGINVITATIONSPEC._serialized_end=1187
   _JOININGINVITATIONSPEC_ENVIRONMENTIDTODESCRIPTIONENTRY._serialized_start=1068
   _JOININGINVITATIONSPEC_ENVIRONMENTIDTODESCRIPTIONENTRY._serialized_end=1187
   _JOININGINVITATIONSTATUS._serialized_start=1190
   _JOININGINVITATIONSTATUS._serialized_end=1341
   _USERACCOUNTDESCRIPTION._serialized_start=1344
-  _USERACCOUNTDESCRIPTION._serialized_end=1510
-  _ENVIRONMENTDESCRIPTION._serialized_start=1512
-  _ENVIRONMENTDESCRIPTION._serialized_end=1631
+  _USERACCOUNTDESCRIPTION._serialized_end=1756
+  _USERACCOUNTDESCRIPTION_ENVIRONMENTIDTODESCRIPTIONENTRY._serialized_start=1068
+  _USERACCOUNTDESCRIPTION_ENVIRONMENTIDTODESCRIPTIONENTRY._serialized_end=1187
+  _ENVIRONMENTDESCRIPTION._serialized_start=1758
+  _ENVIRONMENTDESCRIPTION._serialized_end=1877
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -203,36 +203,58 @@
     def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "last_changed_at", b"last_changed_at"]) -> None: ...
 
 global___JoiningInvitationStatus = JoiningInvitationStatus
 
 class UserAccountDescription(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    class EnvironmentIdToDescriptionEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> global___EnvironmentDescription: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: global___EnvironmentDescription | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     ACCOUNT_NAME_FIELD_NUMBER: builtins.int
     IS_DEFAULT_ACCOUNT_FIELD_NUMBER: builtins.int
     ACCOUNT_ROLE_FIELD_NUMBER: builtins.int
     ENVIRONMENT_NAMES_FIELD_NUMBER: builtins.int
+    ENVIRONMENT_ID_TO_DESCRIPTION_FIELD_NUMBER: builtins.int
     account_name: builtins.str
     """The account name"""
     is_default_account: builtins.bool
     """Indicate whether is default account"""
     account_role: qwak.administration.v0.users.user_pb2.QwakAccountRole.ValueType
     """User account role"""
     @property
     def environment_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Bind user environment names"""
+    @property
+    def environment_id_to_description(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___EnvironmentDescription]:
+        """User environments ids to their description"""
     def __init__(
         self,
         *,
         account_name: builtins.str = ...,
         is_default_account: builtins.bool = ...,
         account_role: qwak.administration.v0.users.user_pb2.QwakAccountRole.ValueType = ...,
         environment_names: collections.abc.Iterable[builtins.str] | None = ...,
+        environment_id_to_description: collections.abc.Mapping[builtins.str, global___EnvironmentDescription] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["account_name", b"account_name", "account_role", b"account_role", "environment_names", b"environment_names", "is_default_account", b"is_default_account"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["account_name", b"account_name", "account_role", b"account_role", "environment_id_to_description", b"environment_id_to_description", "environment_names", b"environment_names", "is_default_account", b"is_default_account"]) -> None: ...
 
 global___UserAccountDescription = UserAccountDescription
 
 class EnvironmentDescription(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENVIRONMENT_NAME_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/common/v0/resources.proto\x12\x1fqwak.user_application.common.v0\"u\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12\x41\n\x0cmemory_units\x18\x03 \x01(\x0e\x32+.qwak.user_application.common.v0.MemoryUnit\"^\n\x0cGpuResources\x12:\n\x08gpu_type\x18\x01 \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"s\n SparkClusterResourceTemplateSpec\x12O\n\x08template\x18\x01 \x01(\x0e\x32=.qwak.user_application.common.v0.SparkClusterResourceTemplate\"\xc3\x01\n\x1aSparkResourceConfiguration\x12\x15\n\rdriver_memory\x18\x01 \x01(\t\x12\x14\n\x0c\x64river_cores\x18\x02 \x01(\x05\x12\x19\n\x11initial_executors\x18\x03 \x01(\x05\x12\x15\n\rmin_executors\x18\x04 \x01(\x05\x12\x15\n\rmax_executors\x18\x05 \x01(\x05\x12\x17\n\x0f\x65xecutor_memory\x18\x06 \x01(\t\x12\x16\n\x0e\x65xecutor_cores\x18\x07 \x01(\x05\"5\n\x1ePodComputeResourceTemplateSpec\x12\x13\n\x0btemplate_id\x18\x01 \x01(\t\"\xcb\x02\n\x13PodComputeResources\x12P\n\x11optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12\x44\n\rcpu_resources\x18\x02 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResources\x12\x44\n\rgpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\x12V\n\rtemplate_spec\x18\x04 \x01(\x0b\x32?.qwak.user_application.common.v0.PodComputeResourceTemplateSpec\"t\n\x15SparkComputeResources\x12[\n\x16resource_configuration\x18\x01 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfiguration\"\xe5\x01\n\x1b\x43lientSparkComputeResources\x12Z\n\rtemplate_spec\x18\x01 \x01(\x0b\x32\x41.qwak.user_application.common.v0.SparkClusterResourceTemplateSpecH\x00\x12]\n\x16resource_configuration\x18\x02 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfigurationH\x00\x42\x0b\n\tresources\"\xe9\x02\n\x19\x43lientPodComputeResources\x12U\n\x16node_optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12X\n\rtemplate_spec\x18\x02 \x01(\x0b\x32?.qwak.user_application.common.v0.PodComputeResourceTemplateSpecH\x00\x12\x46\n\rcpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResourcesH\x00\x12\x46\n\rgpu_resources\x18\x04 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesH\x00\x42\x0b\n\tresources*7\n\nMemoryUnit\x12\x17\n\x13INVALID_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x80\x01\n\x07GpuType\x12\x14\n\x10INVALID_GPU_TYPE\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06*\x88\x02\n\x1cSparkClusterResourceTemplate\x12\"\n\x1eSPARK_CLUSTER_RESOURCE_INVALID\x10\x00\x12 \n\x1cSPARK_CLUSTER_RESOURCE_SMALL\x10\x01\x12!\n\x1dSPARK_CLUSTER_RESOURCE_MEDIUM\x10\x02\x12 \n\x1cSPARK_CLUSTER_RESOURCE_LARGE\x10\x03\x12\x1d\n\x19SPARK_CLUSTER_RESOURCE_XL\x10\x04\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_2XL\x10\x05\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_3XL\x10\x06*\x8a\x01\n\x14NodeOptimizationType\x12\x1d\n\x19NODE_OPTIMIZATION_INVALID\x10\x00\x12\x1a\n\x16NODE_OPTIMIZATION_NONE\x10\x01\x12\x19\n\x15NODE_OPTIMIZATION_CPU\x10\x02\x12\x1c\n\x18NODE_OPTIMIZATION_MEMORY\x10\x03\x42\xc5\x01\n&com.qwak.ai.user_application.common.v0P\x01Z\x98\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application_value/common/v0;user_application_common_v0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/common/v0/resources.proto\x12\x1fqwak.user_application.common.v0\"u\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12\x41\n\x0cmemory_units\x18\x03 \x01(\x0e\x32+.qwak.user_application.common.v0.MemoryUnit\"^\n\x0cGpuResources\x12:\n\x08gpu_type\x18\x01 \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"s\n SparkClusterResourceTemplateSpec\x12O\n\x08template\x18\x01 \x01(\x0e\x32=.qwak.user_application.common.v0.SparkClusterResourceTemplate\"\xc3\x01\n\x1aSparkResourceConfiguration\x12\x15\n\rdriver_memory\x18\x01 \x01(\t\x12\x14\n\x0c\x64river_cores\x18\x02 \x01(\x05\x12\x19\n\x11initial_executors\x18\x03 \x01(\x05\x12\x15\n\rmin_executors\x18\x04 \x01(\x05\x12\x15\n\rmax_executors\x18\x05 \x01(\x05\x12\x17\n\x0f\x65xecutor_memory\x18\x06 \x01(\t\x12\x16\n\x0e\x65xecutor_cores\x18\x07 \x01(\x05\"5\n\x1ePodComputeResourceTemplateSpec\x12\x13\n\x0btemplate_id\x18\x01 \x01(\t\"\xcb\x02\n\x13PodComputeResources\x12P\n\x11optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12\x44\n\rcpu_resources\x18\x02 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResources\x12\x44\n\rgpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\x12V\n\rtemplate_spec\x18\x04 \x01(\x0b\x32?.qwak.user_application.common.v0.PodComputeResourceTemplateSpec\"t\n\x15SparkComputeResources\x12[\n\x16resource_configuration\x18\x01 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfiguration\"\xe5\x01\n\x1b\x43lientSparkComputeResources\x12Z\n\rtemplate_spec\x18\x01 \x01(\x0b\x32\x41.qwak.user_application.common.v0.SparkClusterResourceTemplateSpecH\x00\x12]\n\x16resource_configuration\x18\x02 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfigurationH\x00\x42\x0b\n\tresources\"\xe9\x02\n\x19\x43lientPodComputeResources\x12U\n\x16node_optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12X\n\rtemplate_spec\x18\x02 \x01(\x0b\x32?.qwak.user_application.common.v0.PodComputeResourceTemplateSpecH\x00\x12\x46\n\rcpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResourcesH\x00\x12\x46\n\rgpu_resources\x18\x04 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesH\x00\x42\x0b\n\tresources*7\n\nMemoryUnit\x12\x17\n\x13INVALID_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x95\x02\n\x07GpuType\x12\x14\n\x10INVALID_GPU_TYPE\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06\x12\x14\n\x10NVIDIA_T4_1_4_15\x10\x07\x12\x14\n\x10NVIDIA_T4_1_8_30\x10\x08\x12\x15\n\x11NVIDIA_T4_1_16_60\x10\t\x12\x1e\n\x1aNVIDIA_A100_80GB_8_96_1360\x10\n\x12\x16\n\x12NVIDIA_V100_1_8_52\x10\x0b\x12\x18\n\x14NVIDIA_V100_4_32_208\x10\x0c*\x88\x02\n\x1cSparkClusterResourceTemplate\x12\"\n\x1eSPARK_CLUSTER_RESOURCE_INVALID\x10\x00\x12 \n\x1cSPARK_CLUSTER_RESOURCE_SMALL\x10\x01\x12!\n\x1dSPARK_CLUSTER_RESOURCE_MEDIUM\x10\x02\x12 \n\x1cSPARK_CLUSTER_RESOURCE_LARGE\x10\x03\x12\x1d\n\x19SPARK_CLUSTER_RESOURCE_XL\x10\x04\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_2XL\x10\x05\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_3XL\x10\x06*\x8a\x01\n\x14NodeOptimizationType\x12\x1d\n\x19NODE_OPTIMIZATION_INVALID\x10\x00\x12\x1a\n\x16NODE_OPTIMIZATION_NONE\x10\x01\x12\x19\n\x15NODE_OPTIMIZATION_CPU\x10\x02\x12\x1c\n\x18NODE_OPTIMIZATION_MEMORY\x10\x03\x42\xc5\x01\n&com.qwak.ai.user_application.common.v0P\x01Z\x98\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application_value/common/v0;user_application_common_v0b\x06proto3')
 
 _MEMORYUNIT = DESCRIPTOR.enum_types_by_name['MemoryUnit']
 MemoryUnit = enum_type_wrapper.EnumTypeWrapper(_MEMORYUNIT)
 _GPUTYPE = DESCRIPTOR.enum_types_by_name['GpuType']
 GpuType = enum_type_wrapper.EnumTypeWrapper(_GPUTYPE)
 _SPARKCLUSTERRESOURCETEMPLATE = DESCRIPTOR.enum_types_by_name['SparkClusterResourceTemplate']
 SparkClusterResourceTemplate = enum_type_wrapper.EnumTypeWrapper(_SPARKCLUSTERRESOURCETEMPLATE)
@@ -31,14 +31,20 @@
 INVALID_GPU_TYPE = 0
 NVIDIA_K80 = 1
 NVIDIA_V100 = 2
 NVIDIA_A100 = 3
 NVIDIA_T4 = 4
 NVIDIA_A10G = 5
 NVIDIA_L4 = 6
+NVIDIA_T4_1_4_15 = 7
+NVIDIA_T4_1_8_30 = 8
+NVIDIA_T4_1_16_60 = 9
+NVIDIA_A100_80GB_8_96_1360 = 10
+NVIDIA_V100_1_8_52 = 11
+NVIDIA_V100_4_32_208 = 12
 SPARK_CLUSTER_RESOURCE_INVALID = 0
 SPARK_CLUSTER_RESOURCE_SMALL = 1
 SPARK_CLUSTER_RESOURCE_MEDIUM = 2
 SPARK_CLUSTER_RESOURCE_LARGE = 3
 SPARK_CLUSTER_RESOURCE_XL = 4
 SPARK_CLUSTER_RESOURCE_2XL = 5
 SPARK_CLUSTER_RESOURCE_3XL = 6
@@ -123,19 +129,19 @@
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n&com.qwak.ai.user_application.common.v0P\001Z\230\001github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application_value/common/v0;user_application_common_v0'
   _MEMORYUNIT._serialized_start=1717
   _MEMORYUNIT._serialized_end=1772
   _GPUTYPE._serialized_start=1775
-  _GPUTYPE._serialized_end=1903
-  _SPARKCLUSTERRESOURCETEMPLATE._serialized_start=1906
-  _SPARKCLUSTERRESOURCETEMPLATE._serialized_end=2170
-  _NODEOPTIMIZATIONTYPE._serialized_start=2173
-  _NODEOPTIMIZATIONTYPE._serialized_end=2311
+  _GPUTYPE._serialized_end=2052
+  _SPARKCLUSTERRESOURCETEMPLATE._serialized_start=2055
+  _SPARKCLUSTERRESOURCETEMPLATE._serialized_end=2319
+  _NODEOPTIMIZATIONTYPE._serialized_start=2322
+  _NODEOPTIMIZATIONTYPE._serialized_end=2460
   _CPURESOURCES._serialized_start=84
   _CPURESOURCES._serialized_end=201
   _GPURESOURCES._serialized_start=203
   _GPURESOURCES._serialized_end=297
   _SPARKCLUSTERRESOURCETEMPLATESPEC._serialized_start=299
   _SPARKCLUSTERRESOURCETEMPLATESPEC._serialized_end=414
   _SPARKRESOURCECONFIGURATION._serialized_start=417
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -42,24 +42,52 @@
     INVALID_GPU_TYPE: _GpuType.ValueType  # 0
     NVIDIA_K80: _GpuType.ValueType  # 1
     NVIDIA_V100: _GpuType.ValueType  # 2
     NVIDIA_A100: _GpuType.ValueType  # 3
     NVIDIA_T4: _GpuType.ValueType  # 4
     NVIDIA_A10G: _GpuType.ValueType  # 5
     NVIDIA_L4: _GpuType.ValueType  # 6
+    NVIDIA_T4_1_4_15: _GpuType.ValueType  # 7
+    """More specific node types
+    t4.xl
+    """
+    NVIDIA_T4_1_8_30: _GpuType.ValueType  # 8
+    """t4.2xl"""
+    NVIDIA_T4_1_16_60: _GpuType.ValueType  # 9
+    """t4.4xl"""
+    NVIDIA_A100_80GB_8_96_1360: _GpuType.ValueType  # 10
+    """a100.8xl"""
+    NVIDIA_V100_1_8_52: _GpuType.ValueType  # 11
+    """a100.xl"""
+    NVIDIA_V100_4_32_208: _GpuType.ValueType  # 12
+    """v100.4xl"""
 
 class GpuType(_GpuType, metaclass=_GpuTypeEnumTypeWrapper): ...
 
 INVALID_GPU_TYPE: GpuType.ValueType  # 0
 NVIDIA_K80: GpuType.ValueType  # 1
 NVIDIA_V100: GpuType.ValueType  # 2
 NVIDIA_A100: GpuType.ValueType  # 3
 NVIDIA_T4: GpuType.ValueType  # 4
 NVIDIA_A10G: GpuType.ValueType  # 5
 NVIDIA_L4: GpuType.ValueType  # 6
+NVIDIA_T4_1_4_15: GpuType.ValueType  # 7
+"""More specific node types
+t4.xl
+"""
+NVIDIA_T4_1_8_30: GpuType.ValueType  # 8
+"""t4.2xl"""
+NVIDIA_T4_1_16_60: GpuType.ValueType  # 9
+"""t4.4xl"""
+NVIDIA_A100_80GB_8_96_1360: GpuType.ValueType  # 10
+"""a100.8xl"""
+NVIDIA_V100_1_8_52: GpuType.ValueType  # 11
+"""a100.xl"""
+NVIDIA_V100_4_32_208: GpuType.ValueType  # 12
+"""v100.4xl"""
 global___GpuType = GpuType
 
 class _SparkClusterResourceTemplate:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _SparkClusterResourceTemplateEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SparkClusterResourceTemplate.ValueType], builtins.type):  # noqa: F821
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/v0/user_application.proto\x12\x18qwak.user_application.v0\x1a\x1cgoogle/protobuf/struct.proto\".\n\x04Spec\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"0\n\x06Status\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct*\x88\x02\n\x04Type\x12!\n\x1dINVALID_USER_APPLICATION_TYPE\x10\x00\x12\x10\n\x0cREMOTE_BUILD\x10\x01\x12\x1f\n\x17\x42\x41TCH_FEATURE_PROCESSOR\x10\x02\x1a\x02\x08\x01\x12#\n\x1bSTREAMING_FEATURE_PROCESSOR\x10\x03\x1a\x02\x08\x01\x12\x18\n\x14\x42\x41TCH_INFERENCE_TASK\x10\x04\x12\x14\n\x10MODEL_DEPLOYMENT\x10\x05\x12\x11\n\rMODEL_MONITOR\x10\x06\x12\x1b\n\x17\x44\x45PLOYMENT_MICROSERVICE\x10\x07\x12\x0f\n\x0b\x41PPLICATION\x10\x08\x12\x14\n\x10\x42\x41TCH_FEATURESET\x10\tB\xaa\x01\n\x1f\x63om.qwak.ai.user_application.v0P\x01Z\x84\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application/v0;user_application_v0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/v0/user_application.proto\x12\x18qwak.user_application.v0\x1a\x1cgoogle/protobuf/struct.proto\".\n\x04Spec\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"0\n\x06Status\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct*\xb5\x02\n\x04Type\x12!\n\x1dINVALID_USER_APPLICATION_TYPE\x10\x00\x12\x10\n\x0cREMOTE_BUILD\x10\x01\x12\x1f\n\x17\x42\x41TCH_FEATURE_PROCESSOR\x10\x02\x1a\x02\x08\x01\x12#\n\x1bSTREAMING_FEATURE_PROCESSOR\x10\x03\x1a\x02\x08\x01\x12\x18\n\x14\x42\x41TCH_INFERENCE_TASK\x10\x04\x12\x14\n\x10MODEL_DEPLOYMENT\x10\x05\x12\x11\n\rMODEL_MONITOR\x10\x06\x12\x1b\n\x17\x44\x45PLOYMENT_MICROSERVICE\x10\x07\x12\x0f\n\x0b\x41PPLICATION\x10\x08\x12\x14\n\x10\x42\x41TCH_FEATURESET\x10\t\x12\x18\n\x14\x43USTOMER_ALERT_STACK\x10\n\x12\x11\n\rMODEL_TRAFFIC\x10\x0b\x42\xaa\x01\n\x1f\x63om.qwak.ai.user_application.v0P\x01Z\x84\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application/v0;user_application_v0b\x06proto3')
 
 _TYPE = DESCRIPTOR.enum_types_by_name['Type']
 Type = enum_type_wrapper.EnumTypeWrapper(_TYPE)
 INVALID_USER_APPLICATION_TYPE = 0
 REMOTE_BUILD = 1
 BATCH_FEATURE_PROCESSOR = 2
 STREAMING_FEATURE_PROCESSOR = 3
 BATCH_INFERENCE_TASK = 4
 MODEL_DEPLOYMENT = 5
 MODEL_MONITOR = 6
 DEPLOYMENT_MICROSERVICE = 7
 APPLICATION = 8
 BATCH_FEATURESET = 9
+CUSTOMER_ALERT_STACK = 10
+MODEL_TRAFFIC = 11
 
 
 _SPEC = DESCRIPTOR.message_types_by_name['Spec']
 _STATUS = DESCRIPTOR.message_types_by_name['Status']
 Spec = _reflection.GeneratedProtocolMessageType('Spec', (_message.Message,), {
   'DESCRIPTOR' : _SPEC,
   '__module__' : 'qwak.user_application.v0.user_application_pb2'
@@ -53,13 +55,13 @@
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\037com.qwak.ai.user_application.v0P\001Z\204\001github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application/v0;user_application_v0'
   _TYPE.values_by_name["BATCH_FEATURE_PROCESSOR"]._options = None
   _TYPE.values_by_name["BATCH_FEATURE_PROCESSOR"]._serialized_options = b'\010\001'
   _TYPE.values_by_name["STREAMING_FEATURE_PROCESSOR"]._options = None
   _TYPE.values_by_name["STREAMING_FEATURE_PROCESSOR"]._serialized_options = b'\010\001'
   _TYPE._serialized_start=206
-  _TYPE._serialized_end=470
+  _TYPE._serialized_end=515
   _SPEC._serialized_start=107
   _SPEC._serialized_end=153
   _STATUS._serialized_start=155
   _STATUS._serialized_end=203
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -29,27 +29,31 @@
     STREAMING_FEATURE_PROCESSOR: _Type.ValueType  # 3
     BATCH_INFERENCE_TASK: _Type.ValueType  # 4
     MODEL_DEPLOYMENT: _Type.ValueType  # 5
     MODEL_MONITOR: _Type.ValueType  # 6
     DEPLOYMENT_MICROSERVICE: _Type.ValueType  # 7
     APPLICATION: _Type.ValueType  # 8
     BATCH_FEATURESET: _Type.ValueType  # 9
+    CUSTOMER_ALERT_STACK: _Type.ValueType  # 10
+    MODEL_TRAFFIC: _Type.ValueType  # 11
 
 class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
 
 INVALID_USER_APPLICATION_TYPE: Type.ValueType  # 0
 REMOTE_BUILD: Type.ValueType  # 1
 BATCH_FEATURE_PROCESSOR: Type.ValueType  # 2
 STREAMING_FEATURE_PROCESSOR: Type.ValueType  # 3
 BATCH_INFERENCE_TASK: Type.ValueType  # 4
 MODEL_DEPLOYMENT: Type.ValueType  # 5
 MODEL_MONITOR: Type.ValueType  # 6
 DEPLOYMENT_MICROSERVICE: Type.ValueType  # 7
 APPLICATION: Type.ValueType  # 8
 BATCH_FEATURESET: Type.ValueType  # 9
+CUSTOMER_ALERT_STACK: Type.ValueType  # 10
+MODEL_TRAFFIC: Type.ValueType  # 11
 global___Type = Type
 
 class Spec(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUE_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+qwak/vectors/v1/collection/collection.proto\x12\x1fqwak.vector.store.v1.collection\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa2\x01\n\x0cQwakMetadata\x12.\n\ncreated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x02 \x01(\t\x12\x34\n\x10last_modified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x04 \x01(\t\"?\n\x1aVectorCollectionVectorizer\x12\x19\n\x0fqwak_model_name\x18\x01 \x01(\tH\x00\x42\x06\n\x04type\"\x85\x02\n\x14VectorCollectionSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12O\n\nvectorizer\x18\x03 \x01(\x0b\x32;.qwak.vector.store.v1.collection.VectorCollectionVectorizer\x12G\n\x06metric\x18\x04 \x01(\x0e\x32\x37.qwak.vector.store.v1.collection.VectorCollectionMetric\x12\x11\n\tdimension\x18\x05 \x01(\x05\x12\x1d\n\x15multi_tenancy_enabled\x18\x06 \x01(\x08\"x\n\x1aVectorCollectionDefinition\x12\n\n\x02id\x18\x01 \x01(\t\x12N\n\x0f\x63ollection_spec\x18\x02 \x01(\x0b\x32\x35.qwak.vector.store.v1.collection.VectorCollectionSpec\"\xed\x01\n\x10VectorCollection\x12?\n\x08metadata\x18\x01 \x01(\x0b\x32-.qwak.vector.store.v1.collection.QwakMetadata\x12O\n\ndefinition\x18\x02 \x01(\x0b\x32;.qwak.vector.store.v1.collection.VectorCollectionDefinition\x12G\n\x06status\x18\x03 \x01(\x0e\x32\x37.qwak.vector.store.v1.collection.VectorCollectionStatus\"Z\n\x08Property\x12\x0c\n\x04name\x18\x01 \x01(\t\x12@\n\tdata_type\x18\x02 \x01(\x0e\x32-.qwak.vector.store.v1.collection.PropertyType\"h\n\x12\x43ollectionMetadata\x12\x13\n\x0bnum_vectors\x18\x01 \x01(\x03\x12=\n\nproperties\x18\x02 \x03(\x0b\x32).qwak.vector.store.v1.collection.Property*\x8f\x02\n\x16VectorCollectionStatus\x12\x1d\n\x19\x43OLLECTION_STATUS_INVALID\x10\x00\x12&\n\"COLLECTION_STATUS_CREATE_REQUESTED\x10\x01\x12\x1d\n\x19\x43OLLECTION_STATUS_CREATED\x10\x02\x12#\n\x1f\x43OLLECTION_STATUS_CREATE_FAILED\x10\x03\x12&\n\"COLLECTION_STATUS_DELETE_REQUESTED\x10\x04\x12#\n\x1f\x43OLLECTION_STATUS_DELETE_FAILED\x10\x05\x12\x1d\n\x19\x43OLLECTION_STATUS_DELETED\x10\x06*w\n\x16VectorCollectionMetric\x12\x1d\n\x19\x43OLLECTION_METRIC_INVALID\x10\x00\x12 \n\x1c\x43OLLECTION_METRIC_L2_SQUARED\x10\x01\x12\x1c\n\x18\x43OLLECTION_METRIC_COSINE\x10\x02*\xac\x01\n\x0cPropertyType\x12\x19\n\x15PROPERTY_TYPE_INVALID\x10\x00\x12\x18\n\x14PROPERTY_TYPE_STRING\x10\x01\x12\x15\n\x11PROPERTY_TYPE_INT\x10\x02\x12\x18\n\x14PROPERTY_TYPE_DOUBLE\x10\x03\x12\x19\n\x15PROPERTY_TYPE_BOOLEAN\x10\x04\x12\x1b\n\x17PROPERTY_TYPE_TIMESTAMP\x10\x05\x42K\n!com.qwak.ai.vectors.v1.collectionP\x01Z$qwak/vector_management/v1;collectionb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+qwak/vectors/v1/collection/collection.proto\x12\x1fqwak.vector.store.v1.collection\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa2\x01\n\x0cQwakMetadata\x12.\n\ncreated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x02 \x01(\t\x12\x34\n\x10last_modified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x04 \x01(\t\"?\n\x1aVectorCollectionVectorizer\x12\x19\n\x0fqwak_model_name\x18\x01 \x01(\tH\x00\x42\x06\n\x04type\"\x85\x02\n\x14VectorCollectionSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12O\n\nvectorizer\x18\x03 \x01(\x0b\x32;.qwak.vector.store.v1.collection.VectorCollectionVectorizer\x12G\n\x06metric\x18\x04 \x01(\x0e\x32\x37.qwak.vector.store.v1.collection.VectorCollectionMetric\x12\x11\n\tdimension\x18\x05 \x01(\x05\x12\x1d\n\x15multi_tenancy_enabled\x18\x06 \x01(\x08\"x\n\x1aVectorCollectionDefinition\x12\n\n\x02id\x18\x01 \x01(\t\x12N\n\x0f\x63ollection_spec\x18\x02 \x01(\x0b\x32\x35.qwak.vector.store.v1.collection.VectorCollectionSpec\"\xed\x01\n\x10VectorCollection\x12?\n\x08metadata\x18\x01 \x01(\x0b\x32-.qwak.vector.store.v1.collection.QwakMetadata\x12O\n\ndefinition\x18\x02 \x01(\x0b\x32;.qwak.vector.store.v1.collection.VectorCollectionDefinition\x12G\n\x06status\x18\x03 \x01(\x0e\x32\x37.qwak.vector.store.v1.collection.VectorCollectionStatus\"Z\n\x08Property\x12\x0c\n\x04name\x18\x01 \x01(\t\x12@\n\tdata_type\x18\x02 \x01(\x0e\x32-.qwak.vector.store.v1.collection.PropertyType\"h\n\x12\x43ollectionMetadata\x12\x13\n\x0bnum_vectors\x18\x01 \x01(\x03\x12=\n\nproperties\x18\x02 \x03(\x0b\x32).qwak.vector.store.v1.collection.Property*\x8f\x02\n\x16VectorCollectionStatus\x12\x1d\n\x19\x43OLLECTION_STATUS_INVALID\x10\x00\x12&\n\"COLLECTION_STATUS_CREATE_REQUESTED\x10\x01\x12\x1d\n\x19\x43OLLECTION_STATUS_CREATED\x10\x02\x12#\n\x1f\x43OLLECTION_STATUS_CREATE_FAILED\x10\x03\x12&\n\"COLLECTION_STATUS_DELETE_REQUESTED\x10\x04\x12#\n\x1f\x43OLLECTION_STATUS_DELETE_FAILED\x10\x05\x12\x1d\n\x19\x43OLLECTION_STATUS_DELETED\x10\x06*\xd3\x01\n\x16VectorCollectionMetric\x12\x1d\n\x19\x43OLLECTION_METRIC_INVALID\x10\x00\x12 \n\x1c\x43OLLECTION_METRIC_L2_SQUARED\x10\x01\x12\x1c\n\x18\x43OLLECTION_METRIC_COSINE\x10\x02\x12!\n\x1d\x43OLLECTION_METRIC_DOT_PRODUCT\x10\x03\x12\x18\n\x14\x43OLLECTION_METRIC_L1\x10\x04\x12\x1d\n\x19\x43OLLECTION_METRIC_HAMMING\x10\x05*\xac\x01\n\x0cPropertyType\x12\x19\n\x15PROPERTY_TYPE_INVALID\x10\x00\x12\x18\n\x14PROPERTY_TYPE_STRING\x10\x01\x12\x15\n\x11PROPERTY_TYPE_INT\x10\x02\x12\x18\n\x14PROPERTY_TYPE_DOUBLE\x10\x03\x12\x19\n\x15PROPERTY_TYPE_BOOLEAN\x10\x04\x12\x1b\n\x17PROPERTY_TYPE_TIMESTAMP\x10\x05\x42K\n!com.qwak.ai.vectors.v1.collectionP\x01Z$qwak/vector_management/v1;collectionb\x06proto3')
 
 _VECTORCOLLECTIONSTATUS = DESCRIPTOR.enum_types_by_name['VectorCollectionStatus']
 VectorCollectionStatus = enum_type_wrapper.EnumTypeWrapper(_VECTORCOLLECTIONSTATUS)
 _VECTORCOLLECTIONMETRIC = DESCRIPTOR.enum_types_by_name['VectorCollectionMetric']
 VectorCollectionMetric = enum_type_wrapper.EnumTypeWrapper(_VECTORCOLLECTIONMETRIC)
 _PROPERTYTYPE = DESCRIPTOR.enum_types_by_name['PropertyType']
 PropertyType = enum_type_wrapper.EnumTypeWrapper(_PROPERTYTYPE)
@@ -30,14 +30,17 @@
 COLLECTION_STATUS_CREATE_FAILED = 3
 COLLECTION_STATUS_DELETE_REQUESTED = 4
 COLLECTION_STATUS_DELETE_FAILED = 5
 COLLECTION_STATUS_DELETED = 6
 COLLECTION_METRIC_INVALID = 0
 COLLECTION_METRIC_L2_SQUARED = 1
 COLLECTION_METRIC_COSINE = 2
+COLLECTION_METRIC_DOT_PRODUCT = 3
+COLLECTION_METRIC_L1 = 4
+COLLECTION_METRIC_HAMMING = 5
 PROPERTY_TYPE_INVALID = 0
 PROPERTY_TYPE_STRING = 1
 PROPERTY_TYPE_INT = 2
 PROPERTY_TYPE_DOUBLE = 3
 PROPERTY_TYPE_BOOLEAN = 4
 PROPERTY_TYPE_TIMESTAMP = 5
 
@@ -100,18 +103,18 @@
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n!com.qwak.ai.vectors.v1.collectionP\001Z$qwak/vector_management/v1;collection'
   _VECTORCOLLECTIONSTATUS._serialized_start=1168
   _VECTORCOLLECTIONSTATUS._serialized_end=1439
-  _VECTORCOLLECTIONMETRIC._serialized_start=1441
-  _VECTORCOLLECTIONMETRIC._serialized_end=1560
-  _PROPERTYTYPE._serialized_start=1563
-  _PROPERTYTYPE._serialized_end=1735
+  _VECTORCOLLECTIONMETRIC._serialized_start=1442
+  _VECTORCOLLECTIONMETRIC._serialized_end=1653
+  _PROPERTYTYPE._serialized_start=1656
+  _PROPERTYTYPE._serialized_end=1828
   _QWAKMETADATA._serialized_start=114
   _QWAKMETADATA._serialized_end=276
   _VECTORCOLLECTIONVECTORIZER._serialized_start=278
   _VECTORCOLLECTIONVECTORIZER._serialized_end=341
   _VECTORCOLLECTIONSPEC._serialized_start=344
   _VECTORCOLLECTIONSPEC._serialized_end=605
   _VECTORCOLLECTIONDEFINITION._serialized_start=607
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -66,23 +66,35 @@
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     COLLECTION_METRIC_INVALID: _VectorCollectionMetric.ValueType  # 0
     """Collection metric is invalid"""
     COLLECTION_METRIC_L2_SQUARED: _VectorCollectionMetric.ValueType  # 1
     """Collection metric defined L2"""
     COLLECTION_METRIC_COSINE: _VectorCollectionMetric.ValueType  # 2
     """Collection metric defined COSINE"""
+    COLLECTION_METRIC_DOT_PRODUCT: _VectorCollectionMetric.ValueType  # 3
+    """Collection metric defined DOT PRODUCT"""
+    COLLECTION_METRIC_L1: _VectorCollectionMetric.ValueType  # 4
+    """Collection metric defined L1"""
+    COLLECTION_METRIC_HAMMING: _VectorCollectionMetric.ValueType  # 5
+    """Collection metric defined HAMMING"""
 
 class VectorCollectionMetric(_VectorCollectionMetric, metaclass=_VectorCollectionMetricEnumTypeWrapper): ...
 
 COLLECTION_METRIC_INVALID: VectorCollectionMetric.ValueType  # 0
 """Collection metric is invalid"""
 COLLECTION_METRIC_L2_SQUARED: VectorCollectionMetric.ValueType  # 1
 """Collection metric defined L2"""
 COLLECTION_METRIC_COSINE: VectorCollectionMetric.ValueType  # 2
 """Collection metric defined COSINE"""
+COLLECTION_METRIC_DOT_PRODUCT: VectorCollectionMetric.ValueType  # 3
+"""Collection metric defined DOT PRODUCT"""
+COLLECTION_METRIC_L1: VectorCollectionMetric.ValueType  # 4
+"""Collection metric defined L1"""
+COLLECTION_METRIC_HAMMING: VectorCollectionMetric.ValueType  # 5
+"""Collection metric defined HAMMING"""
 global___VectorCollectionMetric = VectorCollectionMetric
 
 class _PropertyType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _PropertyTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_PropertyType.ValueType], builtins.type):  # noqa: F821
```

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/filters_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_service_pb2.py` & `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi` & `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py` & `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/pyproject.toml` & `qwak_core-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.3.99"
+version = "0.4.0"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
@@ -25,15 +25,15 @@
 
 [tool.poetry.urls]
 "Home page" = "https://www.qwak.com/"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.12"
 python-json-logger = ">=2.0.2"
-grpcio = ">=1.32.0"
+grpcio = ">=1.57.0"
 protobuf = [
     { version = ">=3.10,<4", python = ">=3.7.1,<3.10" },
     { version = ">=4.21.6", python = ">=3.10" }
 ]
 dependency-injector = ">=4.0"
 requests = "*"
 python-jose = "*"
```

### Comparing `qwak_core-0.3.99/qwak/__init__.py` & `qwak_core-0.4.0/qwak/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for qwak-core."""
 
 __author__ = "Qwak.ai"
-__version__ = "0.3.99"
+__version__ = "0.4.0"
 
 from qwak.inner.di_configuration import wire_dependencies
 from qwak.model.experiment_tracking import log_metric, log_param
 from qwak.model_loggers.artifact_logger import load_file, log_file
 from qwak.model_loggers.data_logger import load_data, log_data
 from qwak.model_loggers.model_logger import load_model, log_model
```

### Comparing `qwak_core-0.3.99/qwak/automations/__init__.py` & `qwak_core-0.4.0/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/automations/automation_executions.py` & `qwak_core-0.4.0/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/automations/automations.py` & `qwak_core-0.4.0/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/automations/batch_execution_action.py` & `qwak_core-0.4.0/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.4.0/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/automations/common.py` & `qwak_core-0.4.0/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/_inner/edge_communications.py` & `qwak_core-0.4.0/qwak/clients/_inner/edge_communications.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.4.0/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/administration/authentication/client.py` & `qwak_core-0.4.0/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.4.0/qwak/clients/administration/eco_system/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Dict, List, Optional, Set
 
 import grpc
 from _qwak_proto.qwak.ecosystem.v0.ecosystem_pb2 import (
     EnvironmentDetails,
     UserContextAccountDetails,
     UserContextEnvironmentDetails,
+    AuthenticatedUserContext,
 )
 from _qwak_proto.qwak.ecosystem.v0.ecosystem_runtime_service_pb2 import (
     GetAuthenticatedUserContextRequest,
-    GetAuthenticatedUserContextResponse,
     GetCloudCredentialsRequest,
     GetCloudCredentialsResponse,
 )
 from _qwak_proto.qwak.ecosystem.v0.ecosystem_runtime_service_pb2_grpc import (
     QwakEcosystemRuntimeStub,
 )
 from dependency_injector.wiring import Provide
@@ -38,15 +38,15 @@
         try:
             return self._ecosystem_service.GetCloudCredentials(request)
         except grpc.RpcError as e:
             raise QwakException(
                 f"Failed to get cloud credentials, error is {e.details()}"
             )
 
-    def get_authenticated_user_context(self) -> GetAuthenticatedUserContextResponse:
+    def get_authenticated_user_context(self) -> AuthenticatedUserContext:
         try:
             return self._ecosystem_service.GetAuthenticatedUserContext(
                 GetAuthenticatedUserContextRequest()
             ).authenticated_user_context
 
         except grpc.RpcError as e:
             raise QwakException(f"Failed to get user context, error is {e.details()}")
```

### Comparing `qwak_core-0.3.99/qwak/clients/administration/environment/client.py` & `qwak_core-0.4.0/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/administration/self_service/client.py` & `qwak_core-0.4.0/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/alert_management/client.py` & `qwak_core-0.4.0/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/alerts_registry/channel.py` & `qwak_core-0.4.0/qwak/clients/alerts_registry/channel.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/alerts_registry/client.py` & `qwak_core-0.4.0/qwak/clients/alerts_registry/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/analytics/client.py` & `qwak_core-0.4.0/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/audience/client.py` & `qwak_core-0.4.0/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/automation_management/client.py` & `qwak_core-0.4.0/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/autoscaling/client.py` & `qwak_core-0.4.0/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/batch_job_management/client.py` & `qwak_core-0.4.0/qwak/clients/batch_job_management/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,15 @@
                     execution_details=BatchJobExecutionDetails(
                         job_timeout=execution_config.execution.job_timeout,
                         task_timeout=execution_config.execution.file_timeout,
                         batch_job_deployment_size=job_size,
                         advanced_deployment_options=AdvancedDeploymentOptions(
                             custom_iam_role_arn=execution_config.advanced_options.custom_iam_role_arn,
                             purchase_option=user_purchase_option,
+                            service_account_key_secret_name=execution_config.advanced_options.service_account_key_secret_name,
                         ),
                         parameters=BatchJobManagerClient._batch_job_parameters_as_list(
                             execution_config.execution.parameters
                         ),
                     ),
                 )
             )
```

### Comparing `qwak_core-0.3.99/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.4.0/qwak/clients/batch_job_management/executions_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,15 @@
         gpu_type: str = field(default="")
         instance_size: str = field(default="")
 
     @dataclass
     class AdvancedOptions:
         custom_iam_role_arn: str = field(default=None)
         purchase_option: str = field(default=None)
+        service_account_key_secret_name: str = field(default=None)
 
     warmup: Warmup = field(default_factory=Warmup)
     execution: Execution = field(default_factory=Execution)
     resources: Resources = field(default_factory=Resources)
     advanced_options: AdvancedOptions = field(default_factory=AdvancedOptions)
```

### Comparing `qwak_core-0.3.99/qwak/clients/batch_job_management/results.py` & `qwak_core-0.4.0/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/build_management/client.py` & `qwak_core-0.4.0/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/build_orchestrator/build_model_request_getter.py` & `qwak_core-0.4.0/qwak/clients/build_orchestrator/build_model_request_getter.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                 main_dir=build_conf.build_properties.model_uri.main_dir,
             ),
         ),
         build_env=BuildEnv(
             docker_env=DockerEnv(
                 base_image=build_conf.build_env.docker.base_image,
                 assumed_iam_role_arn=build_conf.build_env.docker.assumed_iam_role_arn,
+                service_account_key_secret_name=build_conf.build_env.docker.service_account_key_secret_name,
                 no_cache=not build_conf.build_env.docker.cache,
                 env_vars=build_conf.build_env.docker.env_vars,
             ),
             python_env=PythonEnv(
                 git_credentials=build_conf.build_properties.model_uri.git_credentials,
                 git_credentials_secret=build_conf.build_properties.model_uri.git_credentials_secret,
                 qwak_sdk_version=sdk_version,
```

### Comparing `qwak_core-0.3.99/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.4.0/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/build_orchestrator/internal_client.py` & `qwak_core-0.4.0/qwak/clients/build_orchestrator/internal_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/data_versioning/client.py` & `qwak_core-0.4.0/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/data_versioning/data_tag_filter.py` & `qwak_core-0.4.0/qwak/clients/data_versioning/data_tag_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/deployment/client.py` & `qwak_core-0.4.0/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/feature_store/execution_management_client.py` & `qwak_core-0.4.0/qwak/clients/feature_store/execution_management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.4.0/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/feature_store/management_client.py` & `qwak_core-0.4.0/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/feature_store/offline_serving_client.py` & `qwak_core-0.4.0/qwak/clients/feature_store/offline_serving_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.4.0/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/file_versioning/client.py` & `qwak_core-0.4.0/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/file_versioning/file_tag_filter.py` & `qwak_core-0.4.0/qwak/clients/file_versioning/file_tag_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/instance_template/client.py` & `qwak_core-0.4.0/qwak/clients/instance_template/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,33 +35,32 @@
             result: GetInstanceTemplateResponse = (
                 self._instance_template_service.GetInstanceTemplate(
                     GetInstanceTemplateRequest(id=instance_template_id)
                 )
             )
             return result.instance_template
         except grpc.RpcError as e:
-            print(e)
             raise QwakException(
-                GET_INSTANCE_TEMPLATE_ERROR_FORMAT.format(e=e.details())
+                GET_INSTANCE_TEMPLATE_ERROR_FORMAT.format(
+                    e=e.details(), error_code=e.code()
+                )
             )
         except Exception as e:
-            print(e)
             raise QwakException(GET_INSTANCE_TEMPLATE_ERROR_FORMAT.format(e=e))
 
     def list_instance_templates(self) -> List[InstanceTemplateSpec]:
         try:
             result: ListInstanceTemplatesResponse = self._instance_template_service.ListInstanceTemplates(
                 ListInstanceTemplatesRequest(
                     optional_instance_filter=InstanceFilter(
                         instance_type_filter=InstanceTypeFilter.INSTANCE_TYPE_FILTER_ALL
                     )
                 )
             )
             return list(result.instance_template_list)
         except grpc.RpcError as e:
-            print(e)
             raise QwakException(
-                GET_INSTANCE_TEMPLATE_ERROR_FORMAT.format(e=e.details())
+                GET_INSTANCE_TEMPLATE_ERROR_FORMAT.format(e=e.details()),
+                status_code=e.code(),
             )
         except Exception as e:
-            print(e)
             raise QwakException(GET_INSTANCE_TEMPLATE_ERROR_FORMAT.format(e=e))
```

### Comparing `qwak_core-0.3.99/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.4.0/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/logging_client/client.py` & `qwak_core-0.4.0/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/model_management/client.py` & `qwak_core-0.4.0/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/project/client.py` & `qwak_core-0.4.0/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/secret_service/client.py` & `qwak_core-0.4.0/qwak/clients/secret_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def get_secret(self, name) -> str:
         try:
             request = GetSecretRequest(name=name)
             return self._secret_service.GetSecret(request).value
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.NOT_FOUND:
-                raise QwakException(f"Secret [{name}] not found")
+                raise QwakException(f"Secret [{name}] not found", status_code=e.code())
             else:
                 raise QwakException(
                     f"Failed to get secret, name: [{name}], error code is [{e.code()}], error message is [{e.details()}]"
                 )
 
     def set_secret(self, name, value) -> None:
         try:
```

### Comparing `qwak_core-0.3.99/qwak/clients/user_application_instance/client.py` & `qwak_core-0.4.0/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/vector_store/management_client.py` & `qwak_core-0.4.0/qwak/clients/vector_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/vector_store/serving_client.py` & `qwak_core-0.4.0/qwak/clients/vector_store/serving_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/clients/workspace_manager/client.py` & `qwak_core-0.4.0/qwak/clients/workspace_manager/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/exceptions/__init__.py` & `qwak_core-0.4.0/qwak/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/exceptions/quiet_error.py` & `qwak_core-0.4.0/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.4.0/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/exceptions/qwak_suggestion_exception.py` & `qwak_core-0.4.0/qwak/exceptions/qwak_suggestion_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/_common/artifact_utils.py` & `qwak_core-0.4.0/qwak/feature_store/_common/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/_common/feature_set_utils.py` & `qwak_core-0.4.0/qwak/feature_store/_common/feature_set_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,27 @@
 from dataclasses import dataclass
 from typing import Optional
 
 from _qwak_proto.qwak.build.v1.build_pb2 import (
     BatchFeature as ProtoBatchFeature,
     BatchFeatureV1 as ProtoBatchFeatureV1,
     Feature as ProtoFeature,
+    StreamingAggregationFeature as ProtoStreamingAggregationFeature,
+    StreamingFeature as ProtoStreamingFeature,
+    StreamingFeatureV1 as ProtoStreamingFeatureV1,
+)
+from _qwak_proto.qwak.feature_store.entities.entity_pb2 import (
+    EntitySpec as ProtoEntitySpec,
 )
-from _qwak_proto.qwak.feature_store.entities.entity_pb2 import EntitySpec
 from _qwak_proto.qwak.feature_store.features.feature_set_types_pb2 import (
-    BatchFeatureSet,
-    BatchFeatureSetV1,
-    FeatureSetType,
+    BatchFeatureSet as ProtoBatchFeatureSet,
+    BatchFeatureSetV1 as ProtoBatchFeatureSetV1,
+    FeatureSetType as ProtoFeatureSetType,
+    StreamingAggregationFeatureSet as ProtoStreamingAggregationFeatureSet,
+    StreamingFeatureSetV1 as ProtoStreamingFeatureSetV1,
 )
 from qwak.clients.feature_store import FeatureRegistryClient
 from qwak.exceptions import QwakException
 from qwak.model.schema_entities import BaseFeature, Entity, FeatureStoreInput
 
 _INTERNAL_KEY_PREFIX: str = "_qwak_key_"
 
@@ -40,18 +47,54 @@
         return ProtoFeature(
             batch_feature_v1=ProtoBatchFeatureV1(
                 name=self.name, entity=self.entity.to_proto()
             )
         )
 
 
+@dataclass(unsafe_hash=True)
+class StreamingFeature(BaseFeature):
+    entity: Entity
+
+    def to_proto(self):
+        return ProtoFeature(
+            streaming_feature=ProtoStreamingFeature(
+                name=self.name, entity=self.entity.to_proto()
+            )
+        )
+
+
+@dataclass(unsafe_hash=True)
+class StreamingFeatureV1(BaseFeature):
+    entity: Optional[Entity] = None
+
+    def to_proto(self):
+        return ProtoFeature(
+            streaming_feature_v1=ProtoStreamingFeatureV1(
+                name=self.name, entity=self.entity.to_proto()
+            )
+        )
+
+
+@dataclass(unsafe_hash=True)
+class StreamingAggregationFeature(BaseFeature):
+    entity: Optional[Entity] = None
+
+    def to_proto(self):
+        return ProtoFeature(
+            streaming_aggregation_feature=ProtoStreamingAggregationFeature(
+                name=self.name, entity=self.entity.to_proto()
+            )
+        )
+
+
 @dataclass()
 class FeatureSetInfo:
-    entity_spec: EntitySpec
-    feature_set_type: FeatureSetType
+    entity_spec: ProtoEntitySpec
+    feature_set_type: ProtoFeatureSetType
     feature_version: int
 
 
 def get_feature_set_info(
     feature_manager_client: FeatureRegistryClient, feature_set_name: str
 ) -> FeatureSetInfo:
     """
@@ -64,72 +107,84 @@
     """
     feature_set_response = feature_manager_client.get_feature_set_by_name(
         feature_set_name
     )
     if not feature_set_response:
         raise QwakException(f"Feature set: {feature_set_name} does not exist")
 
-    featureset_type: FeatureSetType = get_feature_type(
+    featureset_type: ProtoFeatureSetType = get_feature_type(
         feature_set_response.feature_set.feature_set_definition.feature_set_spec.feature_set_type
     )
     featureset_version = _get_featureset_version(featureset_type)
 
     return FeatureSetInfo(
         entity_spec=feature_set_response.feature_set.feature_set_definition.feature_set_spec.entity.entity_spec,
         feature_set_type=featureset_type,
         feature_version=featureset_version,
     )
 
 
-def get_feature_type(feature_set_type: FeatureSetType):
+def get_feature_type(feature_set_type: ProtoFeatureSetType):
     return getattr(feature_set_type, feature_set_type.WhichOneof("set_type"))
 
 
-def _get_featureset_version(feature_set_type: FeatureSetType) -> int:
+def _get_featureset_version(feature_set_type: ProtoFeatureSetType) -> int:
     """
     Get Featureset version. Return 0 if none version is set
     """
     if hasattr(feature_set_type, "qwak_internal_protocol_version"):
         return feature_set_type.qwak_internal_protocol_version
     return 0
 
 
 def get_typed_feature(
-    feature: FeatureStoreInput, feature_type: FeatureSetType, featureset_version: int
+    feature: FeatureStoreInput,
+    feature_type: ProtoFeatureSetType,
+    featureset_version: int,
 ) -> BaseFeature:
     """
     convert InputFeature to the relevant type
     Args:
         feature: Input feature to cast to the correct type
         feature_type: the feature type as it registered
         featureset_version: the version of the featureset
 
     Return:
         BaseFeature with the correct type
     """
-    if isinstance(feature_type, BatchFeatureSet):
+    if isinstance(feature_type, ProtoBatchFeatureSet):
         return BatchFeature(name=feature.name, entity=feature.entity)
-    elif isinstance(feature_type, BatchFeatureSetV1) and featureset_version == 0:
+    elif isinstance(feature_type, ProtoBatchFeatureSetV1) and featureset_version == 0:
         return BatchFeature(name=feature.name, entity=feature.entity)
-    elif isinstance(feature_type, BatchFeatureSetV1) and featureset_version != 0:
+    elif isinstance(feature_type, ProtoBatchFeatureSetV1) and featureset_version != 0:
         return BatchFeatureV1(name=feature.name, entity=feature.entity)
+    elif (
+        isinstance(feature_type, ProtoStreamingFeatureSetV1) and featureset_version == 0
+    ):
+        return StreamingFeature(name=feature.name, entity=feature.entity)
+    elif (
+        isinstance(feature_type, ProtoStreamingFeatureSetV1) and featureset_version != 0
+    ):
+        return StreamingFeatureV1(name=feature.name, entity=feature.entity)
+    elif isinstance(feature_type, ProtoStreamingAggregationFeatureSet):
+        return StreamingAggregationFeature(name=feature.name, entity=feature.entity)
     else:
         raise ValueError(
             f"Feature set type {feature_type} with protocol version {featureset_version} is not supported for extraction"
         )
 
 
-def get_entity_type(value_type: EntitySpec.ValueType):
+def get_entity_type(value_type: ProtoEntitySpec.ValueType):
     """
     Normalize entity by the enum
     """
 
-    if value_type == EntitySpec.ValueType.STRING:
+    if value_type == ProtoEntitySpec.ValueType.STRING:
         return str
-    elif value_type == EntitySpec.ValueType.INT:
+    elif value_type == ProtoEntitySpec.ValueType.INT:
         return int
 
 
 def generate_key_unique_name(featureset_name: str):
     """
     Generate a name for the feature set key to be registered or treated as a Qwak entity based on its' featuresets'
     name
```

### Comparing `qwak_core-0.3.99/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.4.0/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/_common/functions.py` & `qwak_core-0.4.0/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/_common/packaging.py` & `qwak_core-0.4.0/qwak/feature_store/_common/packaging.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from qwak.feature_store.data_sources.batch.athena import AthenaSource
 from qwak.feature_store.data_sources.batch.big_query import BigQuerySource
 from qwak.feature_store.data_sources.batch.clickhouse import ClickhouseSource
 from qwak.feature_store.data_sources.batch.csv import CsvSource
 from qwak.feature_store.data_sources.batch.elastic_search import ElasticSearchSource
-from qwak.feature_store.data_sources.batch.filesystem_config import (
+from qwak.feature_store.data_sources.batch.filesystem.aws import (
     AnonymousS3Configuration,
     AwsS3AssumeRoleFileSystemConfiguration,
     AwsS3FileSystemConfiguration,
 )
+from qwak.feature_store.data_sources.batch.filesystem.gcp import (
+    GcpGcsServiceAccountImpersonation,
+    GcpGcsUnauthenticated,
+)
 from qwak.feature_store.data_sources.batch.mongodb import MongoDbSource
 from qwak.feature_store.data_sources.batch.mysql import MysqlSource
 from qwak.feature_store.data_sources.batch.parquet import ParquetSource
 from qwak.feature_store.data_sources.batch.postgres import PostgresSource
 from qwak.feature_store.data_sources.batch.redshift import RedshiftSource
 from qwak.feature_store.data_sources.batch.snowflake import SnowflakeSource
 from qwak.feature_store.data_sources.batch.vertica import VerticaSource
@@ -35,14 +39,16 @@
     "BigQuerySource",
     "ClickhouseSource",
     "CsvSource",
     "ElasticSearchSource",
     "AwsS3FileSystemConfiguration",
     "AnonymousS3Configuration",
     "AwsS3AssumeRoleFileSystemConfiguration",
+    "GcpGcsServiceAccountImpersonation",
+    "GcpGcsUnauthenticated",
     "MongoDbSource",
     "MysqlSource",
     "ParquetSource",
     "PostgresSource",
     "RedshiftSource",
     "SnowflakeSource",
     "VerticaSource",
```

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/base.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/_jdbc.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/athena.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/athena.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/big_query.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/clickhouse.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/clickhouse.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/csv.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/csv.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,18 @@
     BatchSource as ProtoBatchSource,
     CsvSource as ProtoCsvSource,
 )
 from _qwak_proto.qwak.feature_store.sources.data_source_pb2 import (
     DataSourceSpec as ProtoDataSourceSpec,
 )
 from qwak.feature_store.data_sources.batch._batch import BaseBatchSource
-from qwak.feature_store.data_sources.batch.filesystem_config import (
+from qwak.feature_store.data_sources.batch.filesystem.base_config import (
     FileSystemConfiguration,
+)
+from qwak.feature_store.data_sources.batch.filesystem.utils import (
     get_fs_config_from_proto,
 )
 
 
 @dataclass
 class CsvSource(BaseBatchSource):
     path: str
```

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/elastic_search.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/filesystem_config.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/aws.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,20 @@
-from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Optional
 
 from _qwak_proto.qwak.feature_store.sources.batch_pb2 import (
     AnonymousS3Configuration as ProtoAnonymousS3Configuration,
     AwsS3AssumeRole as ProtoAwsS3AssumeRole,
     AwsS3FileSystemConfiguration as ProtoAwsS3FileSystemConfiguration,
     FileSystemConfiguration as ProtoFileSystemConfiguration,
 )
 from qwak.exceptions import QwakException
-
-
-@dataclass
-class FileSystemConfiguration(ABC):
-    @abstractmethod
-    def _to_proto(self):
-        pass
-
-    @abstractmethod
-    def _from_proto(self, proto):
-        pass
+from qwak.feature_store.data_sources.batch.filesystem.base_config import (
+    FileSystemConfiguration,
+)
 
 
 @dataclass
 class AnonymousS3Configuration(FileSystemConfiguration):
     def _to_proto(self):
         return ProtoFileSystemConfiguration(
             aws_s3_anonymous=ProtoAnonymousS3Configuration()
@@ -90,29 +81,7 @@
     def _from_proto(cls, proto):
         return AwsS3FileSystemConfiguration(
             access_key_secret_name=proto.access_key_secret_name,
             secret_key_secret_name=proto.secret_key_secret_name,
             bucket=proto.bucket,
             session_token_secret_name=proto.session_token_secret_name,
         )
-
-
-def get_fs_config_from_proto(filesystem_conf) -> Optional[FileSystemConfiguration]:
-    if not filesystem_conf:
-        return None
-
-    fs_conf_type = filesystem_conf.WhichOneof("type")
-
-    if not fs_conf_type:
-        return None
-
-    fs_conf = getattr(filesystem_conf, fs_conf_type)
-    if isinstance(fs_conf, ProtoAwsS3FileSystemConfiguration):
-        return AwsS3FileSystemConfiguration._from_proto(fs_conf)
-
-    elif isinstance(fs_conf, ProtoAnonymousS3Configuration):
-        return AnonymousS3Configuration._from_proto(fs_conf)
-
-    elif isinstance(fs_conf, ProtoAwsS3AssumeRole):
-        return AwsS3AssumeRoleFileSystemConfiguration._from_proto(fs_conf)
-    else:
-        raise QwakException(f"Unsupported FileSystemConfiguration: {fs_conf_type}")
```

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/mongodb.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/mysql.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/parquet.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/parquet.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from _qwak_proto.qwak.feature_store.sources.batch_pb2 import (
     BatchSource as ProtoBatchSource,
     ParquetSource as ProtoParquetSource,
 )
 from _qwak_proto.qwak.feature_store.sources.data_source_pb2 import (
     DataSourceSpec as ProtoDataSourceSpec,
 )
+from qwak.feature_store.data_sources import AnonymousS3Configuration
 from qwak.feature_store.data_sources.batch._batch import BaseBatchSource
-from qwak.feature_store.data_sources.batch.filesystem_config import (
-    AnonymousS3Configuration,
+from qwak.feature_store.data_sources.batch.filesystem.base_config import (
     FileSystemConfiguration,
+)
+from qwak.feature_store.data_sources.batch.filesystem.utils import (
     get_fs_config_from_proto,
 )
 
 
 @dataclass
 class ParquetSource(BaseBatchSource):
     path: str
```

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/postgres.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/redshift.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/snowflake.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/batch/vertica.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/source_authentication.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/source_authentication.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/kafka/__init__.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/kafka/authentication.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/kafka/deserialization.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/deserialization.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/streaming/kafka/kafka.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/data_sources/time_partition_columns.py` & `qwak_core-0.4.0/qwak/feature_store/data_sources/time_partition_columns.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/entities/entity.py` & `qwak_core-0.4.0/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/execution/backfill.py` & `qwak_core-0.4.0/qwak/feature_store/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/execution/execution.py` & `qwak_core-0.4.0/qwak/feature_store/execution/execution.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/execution/execution_query.py` & `qwak_core-0.4.0/qwak/feature_store/execution/execution_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/_utils/_featureset_utils.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/_utils/_featureset_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/base_feature_set.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/base_feature_set.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/streaming.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/streaming.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/streaming_backfill.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/streaming_backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/__init__.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/aggregations/windows.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/windows.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/functions/schema.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/feature_sets/transformations/transformations.py` & `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/offline/_offline_serving_validations.py` & `qwak_core-0.4.0/qwak/feature_store/offline/_offline_serving_validations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.4.0/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.4.0/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/offline/client.py` & `qwak_core-0.4.0/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/offline/client_v2.py` & `qwak_core-0.4.0/qwak/feature_store/offline/client_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,16 @@
     ) -> ProtoPopulation:
         population_arrow_schema_json = OfflineClientV2._pandas_to_json_arrow_schema(
             popuation_df
         )
         population_upload_file_url = (
             self._fs_offline_serving_client.get_population_file_upload_url()
         )
-        population_stream = popuation_df.to_parquet(index=False)
+        population_stream = popuation_df.to_parquet(index=False, coerce_timestamps="ms")
+
         upload_to_s3(
             population_upload_file_url, population_stream, self.POPULATION_CONTENT_TYPE
         )
 
         return ProtoPopulation(
             population_file=ProtoPopulationFile(
                 file_url=population_upload_file_url,
```

### Comparing `qwak_core-0.3.99/qwak/feature_store/offline/feature_set_features.py` & `qwak_core-0.4.0/qwak/feature_store/offline/feature_set_features.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/online/client.py` & `qwak_core-0.4.0/qwak/feature_store/online/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,28 @@
     EntitiesHeader,
     EntityToFeatures,
     EntityValueRow,
     Feature as ServingProtoFeature,
     RequestedEntitiesMatrix,
     RequestedEntitiesMatrixRequest,
     RequestMetaData,
+    StreamingAggregationFeature as ServingProtoStreamingAggregationFeature,
+    StreamingFeature as ServingProtoStreamingFeature,
+    StreamingV1Feature as ServingProtoStreamingV1Feature,
 )
 from _qwak_proto.qwak.feature_store.serving.serving_pb2_grpc import ServingServiceStub
 from qwak.clients.administration.eco_system.client import EcosystemClient
 from qwak.exceptions import QwakException
-from qwak.feature_store._common.feature_set_utils import BatchFeature, BatchFeatureV1
+from qwak.feature_store._common.feature_set_utils import (
+    BatchFeature,
+    BatchFeatureV1,
+    StreamingAggregationFeature,
+    StreamingFeature,
+    StreamingFeatureV1,
+)
 from qwak.feature_store.online import endpoint_utils
 from qwak.feature_store.online.endpoint_utils import EndpointConfig
 from qwak.inner.tool.grpc.grpc_tools import create_grpc_channel
 from qwak.model.schema import ModelSchema
 from qwak.model.schema_entities import BaseFeature, RequestInput
 
 logger = logging.getLogger(__name__)
@@ -232,14 +241,32 @@
                     feature_proto = ServingProtoFeature(
                         batch_v1_feature=ServingProtoBatchV1Feature(name=feature.name)
                     )
                 elif isinstance(feature, BatchFeature):
                     feature_proto = ServingProtoFeature(
                         batch_feature=ServingProtoBatchFeature(name=feature.name)
                     )
+                elif isinstance(feature, StreamingFeature):
+                    feature_proto = ServingProtoFeature(
+                        streaming_feature=ServingProtoStreamingFeature(
+                            name=feature.name
+                        )
+                    )
+                elif isinstance(feature, StreamingFeatureV1):
+                    feature_proto = ServingProtoFeature(
+                        streaming_v1_feature=ServingProtoStreamingV1Feature(
+                            name=feature.name
+                        )
+                    )
+                elif isinstance(feature, StreamingAggregationFeature):
+                    feature_proto = ServingProtoFeature(
+                        streaming_aggregation=ServingProtoStreamingAggregationFeature(
+                            name=feature.name
+                        )
+                    )
                 else:
                     raise ValueError(
                         f"Not support type for feature extraction - {type(feature)}"
                     )
 
                 entity_features_compounds[feature.entity.name].add_feature(
                     feature_proto
```

### Comparing `qwak_core-0.3.99/qwak/feature_store/online/endpoint_utils.py` & `qwak_core-0.4.0/qwak/feature_store/online/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/validations/validation_options.py` & `qwak_core-0.4.0/qwak/feature_store/validations/validation_options.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/validations/validation_response.py` & `qwak_core-0.4.0/qwak/feature_store/validations/validation_response.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/feature_store/validations/validator.py` & `qwak_core-0.4.0/qwak/feature_store/validations/validator.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_config/build_config_v1.py` & `qwak_core-0.4.0/qwak/inner/build_config/build_config_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from dataclasses import dataclass, field
 from os.path import expandvars
 from typing import Dict, List, Optional, Tuple, Union
 
+import grpc
+
 from _qwak_proto.qwak.builds.build_pb2 import BaseDockerImageType
 from _qwak_proto.qwak.builds.builds_pb2 import (
     BuildConfiguration,
     BuildEnvironment,
     BuildModelUri,
     BuildPropertiesProto,
     CondaBuild,
@@ -15,15 +17,18 @@
     RemoteBuild,
     RemoteBuildResources as RemoteBuildResourcesProto,
     Step,
     VirtualEnvironmentBuild,
 )
 from _qwak_proto.qwak.instance_template.instance_template_pb2 import InstanceType
 from qwak.clients.build_orchestrator import BuildOrchestratorClient
-from qwak.clients.instance_template.client import InstanceTemplateManagementClient
+from qwak.clients.instance_template.client import (
+    InstanceTemplateManagementClient,
+)
+from qwak.exceptions import QwakException
 from qwak.inner.tool.protobuf_factory import protobuf_factory
 from qwak.inner.tool.run_config import (
     ConfigCliMap,
     QwakConfigBase,
     YamlConfigMixin,
     validate_bool,
     validate_float,
@@ -88,14 +93,19 @@
     ConfigCliMap("param_list", "build_env.docker.params", validate_list_of_strings),
     ConfigCliMap("env_vars", "build_env.docker.env_vars", validate_list_of_strings),
     ConfigCliMap("cache", "build_env.docker.cache", validate_bool),
     ConfigCliMap("push", "build_env.docker.push", validate_bool),
     ConfigCliMap(
         "iam_role_arn", "build_env.docker.assumed_iam_role_arn", validate_string
     ),
+    ConfigCliMap(
+        "service_account_key_secret_name",
+        "build_env.docker.service_account_key_secret_name",
+        validate_string,
+    ),
     # RemoteConf
     ConfigCliMap("cpus", "build_env.remote.resources.cpus", validate_float),
     ConfigCliMap("memory", "build_env.remote.resources.memory", validate_string),
     ConfigCliMap("gpu_type", "build_env.remote.resources.gpu_type", validate_string),
     ConfigCliMap("gpu_amount", "build_env.remote.resources.gpu_amount", validate_int),
     ConfigCliMap("instance", "build_env.remote.resources.instance", validate_string),
     # Verbosity level
@@ -148,14 +158,15 @@
 @dataclass
 class DockerConf:
     base_image: Optional[str] = field(default=None)
     env_vars: Optional[Union[List[str], Dict[str, str], Tuple]] = field(
         default_factory=list
     )
     assumed_iam_role_arn: str = field(default=None)
+    service_account_key_secret_name: str = field(default=None)
     params: Optional[List[str]] = field(default_factory=list)
     no_cache: bool = field(default=False)
     cache: bool = field(default=True)
     push: bool = field(default=True)
 
     def __post_init__(self):
         if isinstance(self.env_vars, (list, tuple)):
@@ -261,24 +272,30 @@
             is_gpu_used = (
                 self.build_env.remote.resources.gpu_type
                 and self.build_env.remote.resources.gpu_amount
                 and self.build_env.remote.resources.gpu_amount > 0
             )
 
             if self.build_env.remote.resources.instance and not is_gpu_used:
-                instance_spec = instance_template.get_instance_template(
-                    self.build_env.remote.resources.instance
-                )
-                is_gpu_used = (
-                    instance_spec.instance_type == InstanceType.INSTANCE_TYPE_GPU
-                )
+                is_gpu_used = self.deduce_gpu_from_template(instance_template)
 
             if is_gpu_used or self.build_properties.gpu_compatible:
                 result = build_orchestrator.fetch_base_docker_image_name(
                     BaseDockerImageType.GPU
                 )
                 self.build_env.docker.base_image = result.base_docker_image_name
             else:
                 result = build_orchestrator.fetch_base_docker_image_name(
                     BaseDockerImageType.CPU
                 )
                 self.build_env.docker.base_image = result.base_docker_image_name
+
+    def deduce_gpu_from_template(self, instance_template):
+        try:
+            instance_spec = instance_template.get_instance_template(
+                self.build_env.remote.resources.instance
+            )
+            return instance_spec.instance_type == InstanceType.INSTANCE_TYPE_GPU
+
+        except QwakException as e:
+            if not e.status_code or e.status_code != grpc.StatusCode.NOT_FOUND:
+                raise e
```

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/build_loggers/trigger_build_logger.py` & `qwak_core-0.4.0/qwak/inner/build_logic/build_loggers/trigger_build_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/execute_build_pipeline.py` & `qwak_core-0.4.0/qwak/inner/build_logic/execute_build_pipeline.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/interface/build_logger_interface.py` & `qwak_core-0.4.0/qwak/inner/build_logic/interface/build_logger_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/interface/build_phase.py` & `qwak_core-0.4.0/qwak/inner/build_logic/interface/build_phase.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/interface/context_interface.py` & `qwak_core-0.4.0/qwak/inner/build_logic/interface/context_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABCMeta
 from dataclasses import field, dataclass
 from pathlib import Path
 from typing import Optional
 
+from qwak.clients.administration.eco_system.client import EcosystemClient
 from qwak.clients.build_orchestrator import BuildOrchestratorClient
 from qwak.clients.instance_template.client import InstanceTemplateManagementClient
 from qwak.clients.model_management import ModelsManagementClient
 from qwak.inner.build_logic.dependency_manager_type import DependencyManagerType
 from qwak.inner.di_configuration.account import UserAccount, UserAccountConfiguration
 
 
@@ -18,14 +19,15 @@
     )
     client_models_management: ModelsManagementClient = field(
         default_factory=ModelsManagementClient
     )
     client_instance_template: InstanceTemplateManagementClient = field(
         default_factory=InstanceTemplateManagementClient
     )
+    client_ecosystem: EcosystemClient = field(default_factory=EcosystemClient)
 
     # General
     user_account: UserAccount = field(
         default_factory=UserAccountConfiguration().get_user_config
     )
 
     # Pre fetch validation
```

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/interface/phase_run_handler.py` & `qwak_core-0.4.0/qwak/inner/build_logic/interface/phase_run_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/interface/step_inteface.py` & `qwak_core-0.4.0/qwak/inner/build_logic/interface/step_inteface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/interface/time_source.py` & `qwak_core-0.4.0/qwak/inner/build_logic/interface/time_source.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import uuid
 from pathlib import Path
 
+import grpc
+
 from qwak.clients.secret_service import SecretServiceClient
 from qwak.exceptions import (
     QwakSuggestionException,
     QwakException,
 )
 from qwak.inner.build_logic.constants.host_resource import HOST_TEMP_BUILD_DIR
 from qwak.inner.build_logic.interface.step_inteface import Step
 from qwak.inner.build_logic.tools.dependencies_tools import find_dependency_files
 from qwak.inner.build_logic.tools.text import snake_case
 from qwak.inner.instance_template.verify_template_id import verify_template_id
+from qwak.inner.provider import Provider
 from qwak.model.base import QwakModel
 
 
 class PreFetchValidationStep(Step):
     STEP_DESCRIPTION = "Pre model fetch validation"
     DEFAULT_CPUS = 2
     DEFAULT_MEMORY = "4Gi"
@@ -34,28 +37,33 @@
     VALIDATION_FAILURE_GPU_AND_INSTANCE_SUGGESTION = (
         "Please configure only GPU or instance"
     )
     EXISTING_MODEL_PASSED_MSG = "Build process was provided with pre built model"
     INVALID_QWAK_MODEL_MSG_FORMAT = (
         "The provided qwak model is not of {expected_class} but of {passed_class}"
     )
+    SERVICE_ACCOUNT_NOT_FOUND = (
+        "GCP service account key secret '{secret_name}' wasn't found"
+    )
+    SERVICE_ACCOUNT_NOT_FOUND_SUGGESTION = "Make sure your GCP service account key secret is configured correctly in the environment"
 
     def description(self) -> str:
         return self.STEP_DESCRIPTION
 
     def execute(self) -> None:
         self.validate_build_properties()
         self.create_build_id()
         self.collect_model_id()
         self.create_build_dir()
         self.collect_git_credentials()
         self.validate_dependencies()
         self.validate_resources()
         self.validate_deployment_resources()
         self.validate_qwak_model()
+        self.validate_gcp_service_account_secret()
 
     def validate_build_properties(self):
         if not self.config.build_properties.model_uri.uri:
             error_message = "Model uri wasn't set"
             self.build_logger.error(f"{error_message}, failing...")
 
             raise QwakSuggestionException(
@@ -176,32 +184,75 @@
         if gpu_configured and instance_configured:
             raise QwakSuggestionException(
                 message=self.VALIDATION_FAILURE_GPU_AND_INSTANCE_MESSAGE,
                 suggestion=self.VALIDATION_FAILURE_GPU_AND_INSTANCE_SUGGESTION,
             )
 
         if instance_configured:
+            provider = self.__get_provider()
             verify_template_id(
                 self.config.build_env.remote.resources.instance,
                 self.context.client_instance_template,
+                provider=provider,
             )
 
         if not (cpu_configured or gpu_configured or instance_configured):
             self.config.build_env.remote.resources.cpus = self.DEFAULT_CPUS
             self.config.build_env.remote.resources.memory = self.DEFAULT_MEMORY
 
+    def __get_provider(self):
+        user_context = self.context.client_ecosystem.get_authenticated_user_context()
+        provider = None
+        if (
+            user_context.user.environment_details.configuration.cloud_configuration.WhichOneof(
+                "configuration"
+            )
+            == "aws_cloud_configuration"
+        ):
+            provider = Provider.AWS
+        elif (
+            user_context.user.environment_details.configuration.cloud_configuration.WhichOneof(
+                "configuration"
+            )
+            == "gcp_cloud_configuration"
+        ):
+            provider = Provider.GCP
+        return provider
+
     def validate_deployment_resources(self):
         if self.config.deploy and self.config.deployment_instance:
+            provider = self.__get_provider()
             verify_template_id(
-                self.config.deployment_instance, self.context.client_instance_template
+                self.config.deployment_instance,
+                self.context.client_instance_template,
+                provider=provider,
             )
 
     def validate_qwak_model(self):
         if self.config.pre_built_model:
             self.build_logger.debug(self.EXISTING_MODEL_PASSED_MSG)
             if not isinstance(self.config.pre_built_model, QwakModel):
                 raise QwakException(
                     self.INVALID_QWAK_MODEL_MSG_FORMAT.format(
                         expected_class=QwakModel.__name__,
                         passed_class=self.config.pre_built_model.__class__,
                     )
                 )
+
+    def validate_gcp_service_account_secret(self):
+        if self.config.build_env.docker.service_account_key_secret_name:
+            self.build_logger.debug("Checking GCP service account key secret")
+            try:
+                SecretServiceClient().get_secret(
+                    self.config.build_env.docker.service_account_key_secret_name
+                )
+            except QwakException as e:
+                if e.status_code == grpc.StatusCode.NOT_FOUND:
+                    raise QwakSuggestionException(
+                        message=self.SERVICE_ACCOUNT_NOT_FOUND.format(
+                            secret_name=self.config.build_env.docker.service_account_key_secret_name
+                        ),
+                        suggestion=self.SERVICE_ACCOUNT_NOT_FOUND_SUGGESTION,
+                    )
+                raise e
+
+            self.build_logger.debug("service account key secret found")
```

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/phases/phases_pipeline.py` & `qwak_core-0.4.0/qwak/inner/build_logic/phases/phases_pipeline.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py` & `qwak_core-0.4.0/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/tools/dependencies_tools.py` & `qwak_core-0.4.0/qwak/inner/build_logic/tools/dependencies_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/tools/files.py` & `qwak_core-0.4.0/qwak/inner/build_logic/tools/files.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/build_logic/tools/ignore_files.py` & `qwak_core-0.4.0/qwak/inner/build_logic/tools/ignore_files.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/const.py` & `qwak_core-0.4.0/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.4.0/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/di_configuration/account.py` & `qwak_core-0.4.0/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/di_configuration/containers.py` & `qwak_core-0.4.0/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/instance_template/verify_template_id.py` & `qwak_core-0.4.0/qwak/inner/instance_template/verify_template_id.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,36 @@
+from typing import Optional
+
 from _qwak_proto.qwak.instance_template.instance_template_pb2 import InstanceType
 from qwak.clients.instance_template.client import InstanceTemplateManagementClient
 from qwak.exceptions import QwakException
+from qwak.inner.provider import Provider
 
 INVALID_TEMPLATE_ID_ERROR_FORMAT = (
     "Invalid instance: {template_id}. Valid instances are: {cpu_templates}. "
     "For GPU instances you can use {gpu_templates}."
 )
 
 
 def verify_template_id(
-    template_id: str, instance_template_client: InstanceTemplateManagementClient
+    template_id: str,
+    instance_template_client: InstanceTemplateManagementClient,
+    provider: Optional[Provider] = None,
 ) -> None:
     all_templates = instance_template_client.list_instance_templates()
     valid_templates = [template for template in all_templates if template.enabled]
+    if provider == Provider.AWS:
+        valid_templates = [
+            template for template in valid_templates if template.aws_supported
+        ]
+    elif provider == Provider.GCP:
+        valid_templates = [
+            template for template in valid_templates if template.gcp_supported
+        ]
+
     existing_templates = {template.id: template for template in valid_templates}
     if template_id not in existing_templates.keys():
         cpu_template_ids = [
             template.id
             for template in sorted(valid_templates, key=lambda template: template.order)
             if template.instance_type == InstanceType.INSTANCE_TYPE_CPU
         ]
```

### Comparing `qwak_core-0.3.99/qwak/inner/model_loggers_utils.py` & `qwak_core-0.4.0/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/runtime_di/containers.py` & `qwak_core-0.4.0/qwak/inner/runtime_di/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/singleton_meta.py` & `qwak_core-0.4.0/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/tool/auth.py` & `qwak_core-0.4.0/qwak/inner/tool/auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,28 +14,32 @@
 
 
 class Auth0ClientBase:
     _TOKENS_FIELD = "TOKENS"
 
     def __init__(
         self,
-        api_key,
+        api_key=None,
         auth_file=QwakConstants.QWAK_AUTHORIZATION_FILE,
         audience=QwakConstants.TOKEN_AUDIENCE,
     ):
         self._auth_file = auth_file
         self._config = configparser.ConfigParser()
         self._environment = Session().get_environment()
         self.jwks = requests.get(QwakConstants.AUTH0_JWKS_URI, timeout=60).json()
         self.token = None
         self.audience = audience
         self.api_key = api_key
 
     # Returns Non if token is expired
     def get_token(self):
+        if self._environment != Session().get_environment():
+            self.token = None
+            self.api_key = None
+            self._environment = Session().get_environment()
         try:
             if not self.token:
                 self._config.read(self._auth_file)
                 self.token = json.loads(
                     self._config.get(
                         section=self._environment, option=self._TOKENS_FIELD
                     )
@@ -50,14 +54,20 @@
         except jwt.ExpiredSignatureError:
             self.login()
             return self.token
 
     def login(self):
         from qwak.clients.administration import AuthenticationClient
 
+        if not self.api_key:
+            from qwak.inner.di_configuration import UserAccountConfiguration
+
+            user_account = UserAccountConfiguration().get_user_config()
+            self.api_key = user_account.api_key
+
         self.token = AuthenticationClient().authenticate(self.api_key).access_token
 
         from pathlib import Path
 
         Path(self._auth_file).parent.mkdir(parents=True, exist_ok=True)
         self._config.read(self._auth_file)
```

### Comparing `qwak_core-0.3.99/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.4.0/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/tool/protobuf_factory.py` & `qwak_core-0.4.0/qwak/inner/tool/protobuf_factory.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/tool/run_config/base.py` & `qwak_core-0.4.0/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.4.0/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/_entity_extraction.py` & `qwak_core-0.4.0/qwak/model/_entity_extraction.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/adapters/__init__.py` & `qwak_core-0.4.0/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.4.0/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.4.0/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.4.0/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.4.0/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.4.0/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/base.py` & `qwak_core-0.4.0/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/decorators/api.py` & `qwak_core-0.4.0/qwak/model/decorators/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 )
 
 
 @inject
 def api_decorator(
     analytics: bool = True,
     analytics_sample_ratio: float = 1.0,
+    analytics_exclude_columns: list = [],
     feature_extraction: bool = False,
     input_adapter: BaseInputAdapter = DataFrameInputAdapter(),
     output_adapter: BaseOutputAdapter = DataFrameOutputAdapter(),
     api_decorator_function_creator=Provide[
         QwakRuntimeContainer.api_decorator_function_creator
     ],
 ) -> Callable:
@@ -50,11 +51,12 @@
     try:
         return api_decorator_function_creator(
             analytics,
             feature_extraction,
             input_adapter,
             output_adapter,
             analytics_sample_ratio,
+            analytics_exclude_columns,
         )
     except TypeError as e:
         if "__call__() takes 1" in str(e):
             raise QwakException(API_NOT_CONFIGURED_ERROR_MESSAGE)
```

### Comparing `qwak_core-0.3.99/qwak/model/decorators/impl/api_implementation.py` & `qwak_core-0.4.0/qwak/model/decorators/impl/api_implementation.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 def create_decorator_function(
     analytics: bool,
     feature_extraction: bool,
     input_adapter: BaseInputAdapter,
     output_adapter: BaseOutputAdapter,
     analytics_sample_ratio: float,
+    analytics_exclude_columns: list,
 ) -> Callable:
     def api_decorator_function_load_logic(func: Callable[..., Any]):
         func = extract_wrapped(func)
         setattr(func, "_input_adapter", input_adapter)
         setattr(func, "_output_adapter", output_adapter)
         setattr(func, "_fs_extraction", feature_extraction)
```

### Comparing `qwak_core-0.3.99/qwak/model/decorators/timer.py` & `qwak_core-0.4.0/qwak/model/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/experiment_tracking.py` & `qwak_core-0.4.0/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/schema.py` & `qwak_core-0.4.0/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/schema_entities.py` & `qwak_core-0.4.0/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/__init__.py` & `qwak_core-0.4.0/qwak/model/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/input.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/output.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model/tools/run_model_locally.py` & `qwak_core-0.4.0/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.4.0/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model_loggers/data_logger.py` & `qwak_core-0.4.0/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/model_loggers/model_logger.py` & `qwak_core-0.4.0/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/batch_jobs/execution.py` & `qwak_core-0.4.0/qwak/qwak_client/batch_jobs/execution.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/batch_jobs/task.py` & `qwak_core-0.4.0/qwak/qwak_client/batch_jobs/task.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/build_api_helpers/build_api_steps.py` & `qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/build_api_steps.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/build_api_helpers/trigger_build_api.py` & `qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/trigger_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/builds/build.py` & `qwak_core-0.4.0/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.4.0/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.4.0/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/client.py` & `qwak_core-0.4.0/qwak/qwak_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
             project_id (str): The model ID
 
         Returns:
              Optional[Project]: Project by ID.
 
         """
         return Project.from_proto(
-            self._get_project_management().get_project(project_id)
+            self._get_project_management().get_project(project_id).project.spec
         )
 
     def list_projects(self) -> List[Project]:
         """
         List projects
 
         Returns:
```

### Comparing `qwak_core-0.3.99/qwak/qwak_client/data_versioning/data_tag.py` & `qwak_core-0.4.0/qwak/qwak_client/data_versioning/data_tag.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.4.0/qwak/qwak_client/deployments/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
                     metric=Metric(
                         proto_trigger.prometheus_trigger.query_spec.metric_type
                     ),
                     aggregation=Aggregation(
                         proto_trigger.prometheus_trigger.query_spec.aggregation_type
                     ),
                     time_period=proto_trigger.prometheus_trigger.query_spec.time_period,
-                    error_code=proto_trigger.prometheus_trigger.query_spec.error_code,
+                    error_code=proto_trigger.prometheus_trigger.query_spec.status_code,
                 ),
                 threshold=proto_trigger.prometheus_trigger.threshold,
             )
             triggers.append(trigger)
         return AutoScalingConfig(
             min_replica_count=proto.min_replica_count,
             max_replica_count=proto.max_replica_count,
```

### Comparing `qwak_core-0.3.99/qwak/qwak_client/file_versioning/file_tag.py` & `qwak_core-0.4.0/qwak/qwak_client/file_versioning/file_tag.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/models/model.py` & `qwak_core-0.4.0/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.4.0/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/qwak_client/projects/project.py` & `qwak_core-0.4.0/qwak/qwak_client/projects/project.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,23 +35,23 @@
                 last_modified_at=timestamp.FromDatetime(self.last_modified_at),
             )
         )
 
     @staticmethod
     def from_proto(project_spec_proto: ProjectSpecProto):
         return Project(
-            project_id=project_spec_proto.project.spec.project_id,
-            project_name=project_spec_proto.project.spec.project_name,
-            project_description=project_spec_proto.project.spec.project_description,
-            models_count=project_spec_proto.project.spec.models_count,
-            models_active=project_spec_proto.project.spec.models_active,
-            created_by=project_spec_proto.project.spec.created_by,
+            project_id=project_spec_proto.project_id,
+            project_name=project_spec_proto.project_name,
+            project_description=project_spec_proto.project_description,
+            models_count=project_spec_proto.models_count,
+            models_active=project_spec_proto.models_active,
+            created_by=project_spec_proto.created_by,
             created_at=datetime.fromtimestamp(
-                project_spec_proto.project.spec.created_at.seconds
-                + project_spec_proto.project.spec.created_at.nanos / 1e9
+                project_spec_proto.created_at.seconds
+                + project_spec_proto.created_at.nanos / 1e9
             ),
-            last_modified_by=project_spec_proto.project.spec.last_modified_by,
+            last_modified_by=project_spec_proto.last_modified_by,
             last_modified_at=datetime.fromtimestamp(
-                project_spec_proto.project.spec.last_modified_at.seconds
-                + project_spec_proto.project.spec.last_modified_at.nanos / 1e9
+                project_spec_proto.last_modified_at.seconds
+                + project_spec_proto.last_modified_at.nanos / 1e9
             ),
         )
```

### Comparing `qwak_core-0.3.99/qwak/tools/logger/logger.py` & `qwak_core-0.4.0/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/tools/logger/logging.yml` & `qwak_core-0.4.0/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/utils/datetime_utils.py` & `qwak_core-0.4.0/qwak/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/vector_store/client.py` & `qwak_core-0.4.0/qwak/vector_store/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     """
 
     _vector_management_client: VectorManagementClient
 
     _metric_dict: Dict[str, VectorCollectionMetric] = {
         "l2_squared": VectorCollectionMetric.COLLECTION_METRIC_L2_SQUARED,
         "cosine": VectorCollectionMetric.COLLECTION_METRIC_COSINE,
+        "dot_product": VectorCollectionMetric.COLLECTION_METRIC_DOT_PRODUCT,
+        "l1": VectorCollectionMetric.COLLECTION_METRIC_L1,
+        "hamming": VectorCollectionMetric.COLLECTION_METRIC_HAMMING,
     }
 
     def __init__(self, edge_services_url: Optional[str] = None):
         """
         Initializes a `VectorStoreClient` client object to interact with Qwak's vector store service
         """
         self._vector_management_client = VectorManagementClient()
```

### Comparing `qwak_core-0.3.99/qwak/vector_store/collection.py` & `qwak_core-0.4.0/qwak/vector_store/collection.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/vector_store/filters.py` & `qwak_core-0.4.0/qwak/vector_store/filters.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/vector_store/inference_client.py` & `qwak_core-0.4.0/qwak/vector_store/inference_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,19 +82,22 @@
             raise QwakException(
                 f"Vectorizer {self.model_id} failed to transform input {feature_vector} to vectors. Error is: {str(e)}"
             )
         try:
             vector = result_list[0]["embeddings"]
         except Exception:
             raise QwakException(
-                f"Vectorizer {self.model_id} must return a dataframe containing an `embeddings` column"
+                f"Vectorizer {self.model_id} must return a dataframe containing an 'embeddings' column"
             )
         if not vector:
             raise QwakException(
                 f"Vectorizer {self.model_id} did not return embeddings for the given natural input. Unable to continue with the query."
             )
         return vector
 
 
 def _get_model_url(model_id: str, model_url_prefix: str) -> str:
     scheme = "http" if model_url_prefix.startswith("localhost") else "https"
-    return f"{scheme}://{model_url_prefix}/v1/{model_id}/predict"
+    effective_model_id = model_id.replace("-", "_")
+    return (
+        f"{scheme}://{model_url_prefix}/v1/{effective_model_id}/predict"  # noqa: E231
+    )
```

### Comparing `qwak_core-0.3.99/qwak/vector_store/rest_helpers.py` & `qwak_core-0.4.0/qwak/vector_store/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/vector_store/utils/filter_utils.py` & `qwak_core-0.4.0/qwak/vector_store/utils/filter_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak/vector_store/utils/upsert_utils.py` & `qwak_core-0.4.0/qwak/vector_store/utils/upsert_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/alert_registry_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/alert_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/execution_management_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/execution_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -127,22 +127,31 @@
             if entity_to_features.entity_name == entity_name:
                 for feature in entity_to_features.features:
                     one_of = feature.WhichOneof("type")
                     if one_of == "batch_feature":
                         requested_features.add(feature.batch_feature.name)
                     elif one_of == "batch_v1_feature":
                         requested_features.add(feature.batch_v1_feature.name)
+                    elif one_of == "streaming_v1_feature":
+                        requested_features.add(feature.streaming_v1_feature.name)
+                    elif one_of == "streaming_feature":
+                        requested_features.add(feature.streaming_feature.name)
+                    elif one_of == "streaming_aggregation":
+                        requested_features.add(feature.streaming_aggregation.name)
 
     @staticmethod
     def _validate_supported_features(request):
         return all(
             [
                 (
                     feature.WhichOneof("type") == "batch_v1_feature"
                     or feature.WhichOneof("type") == "batch_feature"
+                    or feature.WhichOneof("type") == "streaming_feature"
+                    or feature.WhichOneof("type") == "streaming_feature_v1"
+                    or feature.WhichOneof("type") == "streaming_aggregation"
                 )
                 for entities in request.entities_to_features
                 for feature in entities.features
             ]
         )
 
     @staticmethod
```

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/fs_offline_serving_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/fs_offline_serving_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,21 +20,23 @@
     PodComputeResources,
 )
 from qwak.exceptions import QwakException
 from qwak_services_mock.mocks.utils.exception_handlers import raise_internal_grpc_error
 
 
 def _create_instance_template_cpu(
-    instance_id: str, name: str, order: int, cpu: float, memory_amount: int
+    instance_id: str, name: str, order: int, cpu: float, memory_amount: int, aws_supported: bool = True, gcp_supported: bool = True
 ) -> InstanceTemplateSpec:
     return InstanceTemplateSpec(
         id=instance_id,
         display_name=name,
         order=order,
         enabled=True,
+        aws_supported=aws_supported,
+        gcp_supported=gcp_supported,
         pod_compute_resources=PodComputeResources(
             optimization_type=NodeOptimizationType.NODE_OPTIMIZATION_NONE,
             cpu_resources=CpuResources(
                 cpu=cpu,
                 memory_amount=memory_amount,
                 memory_units=MemoryUnit.GIB,
             ),
@@ -47,20 +49,24 @@
     instance_id: str,
     name: str,
     order: int,
     gpu: int,
     gpu_type: GpuType,
     cpu: float,
     memory_amount: int,
+    aws_supported: bool = True,
+    gcp_supported: bool = True,
 ) -> InstanceTemplateSpec:
     return InstanceTemplateSpec(
         id=instance_id,
         display_name=name,
         order=order,
         enabled=True,
+        aws_supported=aws_supported,
+        gcp_supported=gcp_supported,
         pod_compute_resources=PodComputeResources(
             optimization_type=NodeOptimizationType.NODE_OPTIMIZATION_NONE,
             gpu_resources=GpuResources(
                 gpu_amount=gpu,
                 gpu_type=gpu_type,
             ),
             cpu_resources=CpuResources(
@@ -84,14 +90,24 @@
         ),
         "g5_2xlarge": _create_instance_template_gpu(
             "g5_2xlarge", "G5 2XLarge", 2, 2, GpuType.NVIDIA_A10G, 2, 16
         ),
         "g5_4xlarge": _create_instance_template_gpu(
             "g5_4xlarge", "G5 4XLarge", 2, 4, GpuType.NVIDIA_A10G, 4, 32
         ),
+        "aws_only": _create_instance_template_gpu(
+            "aws_only", "Aws Only", 2, 4, GpuType.NVIDIA_A10G, 4, 32,
+            aws_supported=True,
+            gcp_supported=False,
+        ),
+        "gcp_only": _create_instance_template_gpu(
+            "gcp_only", "GCP Only", 2, 4, GpuType.NVIDIA_A10G, 4, 32,
+            aws_supported=False,
+            gcp_supported=True,
+        ),
     }
 
     def ListInstanceTemplates(
         self, request: ListInstanceTemplatesRequest, context
     ) -> ListInstanceTemplatesResponse:
         try:
             return ListInstanceTemplatesResponse(
```

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/internal_build_orchestrator_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/internal_build_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/vector_serving_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/vector_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/vectors_management_api.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/vectors_management_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/mocks/workspace_manager_service_mock.py` & `qwak_core-0.4.0/qwak_services_mock/mocks/workspace_manager_service_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/qwak_services_mock/services_mock.py` & `qwak_core-0.4.0/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.3.99/setup.py` & `qwak_core-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
  'qwak.clients.vector_store',
  'qwak.clients.workspace_manager',
  'qwak.exceptions',
  'qwak.feature_store',
  'qwak.feature_store._common',
  'qwak.feature_store.data_sources',
  'qwak.feature_store.data_sources.batch',
+ 'qwak.feature_store.data_sources.batch.filesystem',
  'qwak.feature_store.data_sources.streaming',
  'qwak.feature_store.data_sources.streaming.kafka',
  'qwak.feature_store.entities',
  'qwak.feature_store.execution',
  'qwak.feature_store.feature_sets',
  'qwak.feature_store.feature_sets._utils',
  'qwak.feature_store.feature_sets.transformations',
@@ -162,15 +163,15 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML',
  'dependency-injector>=4.0',
- 'grpcio>=1.32.0',
+ 'grpcio>=1.57.0',
  'joblib>=1.3.2,<2.0.0',
  'marshmallow-dataclass>=8.5.8,<9.0.0',
  'python-jose',
  'python-json-logger>=2.0.2',
  'requests',
  'retrying==1.3.4',
  'typeguard>=2,<3']
@@ -179,15 +180,15 @@
 {':extra == "feature-store"': ['cloudpickle==2.2.1'],
  ':python_full_version >= "3.7.1" and python_version < "3.10"': ['protobuf>=3.10,<4'],
  ':python_version >= "3.10"': ['protobuf>=4.21.6'],
  'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.3.99',
+    'version': '0.4.0',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.3.99/PKG-INFO` & `qwak_core-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.3.99
+Version: 0.4.0
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: feature-store
 Requires-Dist: PyYAML
 Requires-Dist: cloudpickle (==2.2.1) ; extra == "feature-store"
 Requires-Dist: dependency-injector (>=4.0)
-Requires-Dist: grpcio (>=1.32.0)
+Requires-Dist: grpcio (>=1.57.0)
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: marshmallow-dataclass (>=8.5.8,<9.0.0)
 Requires-Dist: protobuf (>=3.10,<4) ; python_full_version >= "3.7.1" and python_version < "3.10"
 Requires-Dist: protobuf (>=4.21.6) ; python_version >= "3.10"
 Requires-Dist: pyarrow (>=6.0.0) ; extra == "feature-store"
 Requires-Dist: pyathena (>=2.2.0,!=2.18.0) ; extra == "feature-store"
 Requires-Dist: python-jose
```

