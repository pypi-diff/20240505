# Comparing `tmp/clear_skies_aws-1.9.0.tar.gz` & `tmp/clear_skies_aws-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_aws-1.9.0.tar", max compression
+gzip compressed data, was "clear_skies_aws-1.9.1.tar", max compression
```

## Comparing `clear_skies_aws-1.9.0.tar` & `clear_skies_aws-1.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1053 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.0/LICENSE
--rw-r--r--   0        0        0     7780 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.0/README.md
--rw-r--r--   0        0        0      789 2024-03-29 18:05:02.738023 clear_skies_aws-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      134 2023-12-30 16:33:38.123814 clear_skies_aws-1.9.0/src/clearskies_aws/__init__.py
--rw-r--r--   0        0        0     2865 2024-02-28 23:50:28.351377 clear_skies_aws-1.9.0/src/clearskies_aws/actions/__init__.py
--rw-r--r--   0        0        0     3877 2024-03-20 10:13:37.291200 clear_skies_aws-1.9.0/src/clearskies_aws/actions/action_aws.py
--rw-r--r--   0        0        0     4085 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.0/src/clearskies_aws/actions/assume_role.py
--rw-r--r--   0        0        0     2450 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.0/src/clearskies_aws/actions/assume_role_test.py
--rw-r--r--   0        0        0     6933 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.0/src/clearskies_aws/actions/ses.py
--rw-r--r--   0        0        0     1739 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.0/src/clearskies_aws/actions/ses_test.py
--rw-r--r--   0        0        0     2197 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.0/src/clearskies_aws/actions/sns.py
--rw-r--r--   0        0        0     2306 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.0/src/clearskies_aws/actions/sns_test.py
--rw-r--r--   0        0        0     2340 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/actions/sqs.py
--rw-r--r--   0        0        0     2346 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/actions/sqs_test.py
--rw-r--r--   0        0        0     2363 2024-03-08 14:32:55.873530 clear_skies_aws-1.9.0/src/clearskies_aws/actions/step_function.py
--rw-r--r--   0        0        0     2742 2024-03-08 14:32:45.065230 clear_skies_aws-1.9.0/src/clearskies_aws/actions/step_function_test.py
--rw-r--r--   0        0        0       83 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/backends/__init__.py
--rw-r--r--   0        0        0    29126 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/backends/dynamo_db_backend.py
--rw-r--r--   0        0        0    13150 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/backends/dynamo_db_backend_test.py
--rw-r--r--   0        0        0     2726 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/backends/sqs_backend.py
--rw-r--r--   0        0        0     1138 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/backends/sqs_backend_test.py
--rw-r--r--   0        0        0      472 2024-01-06 13:06:05.318595 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/__init__.py
--rw-r--r--   0        0        0     1305 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1276 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1251 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0      506 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/cli.py
--rw-r--r--   0        0        0     1085 2024-01-06 13:10:52.693804 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/cli_websocket_mock.py
--rw-r--r--   0        0        0     1002 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_api_gateway.py
--rw-r--r--   0        0        0     1067 2023-12-18 00:15:49.555696 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_api_gateway_web_socket.py
--rw-r--r--   0        0        0      952 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_elb.py
--rw-r--r--   0        0        0     1009 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_http_gateway.py
--rw-r--r--   0        0        0     1336 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_invocation.py
--rw-r--r--   0        0        0     1317 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_sns.py
--rw-r--r--   0        0        0     1685 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
--rw-r--r--   0        0        0     1999 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
--rw-r--r--   0        0        0      510 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/contexts/wsgi.py
--rw-r--r--   0        0        0       56 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/di/__init__.py
--rw-r--r--   0        0        0      775 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/di/standard_dependencies.py
--rw-r--r--   0        0        0      112 2024-03-29 18:03:20.842321 clear_skies_aws-1.9.0/src/clearskies_aws/handlers/__init__.py
--rw-r--r--   0        0        0     7471 2024-03-29 18:02:23.674537 clear_skies_aws-1.9.0/src/clearskies_aws/handlers/secrets_manager_rotation.py
--rw-r--r--   0        0        0     1449 2024-01-06 12:49:14.731820 clear_skies_aws-1.9.0/src/clearskies_aws/handlers/simple_body_routing.py
--rw-r--r--   0        0        0      385 2024-01-06 13:10:44.713712 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/__init__.py
--rw-r--r--   0        0        0      943 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     3710 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     2761 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
--rw-r--r--   0        0        0      901 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0      434 2024-01-06 13:10:39.925657 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/cli_websocket_mock.py
--rw-r--r--   0        0        0     3401 2024-03-02 21:11:37.111733 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_api_gateway.py
--rw-r--r--   0        0        0     2845 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
--rw-r--r--   0        0        0      308 2023-12-18 00:15:15.884654 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_api_gateway_web_socket.py
--rw-r--r--   0        0        0      750 2024-03-02 21:10:37.703292 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_elb.py
--rw-r--r--   0        0        0      692 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_http_gateway.py
--rw-r--r--   0        0        0      928 2023-10-20 10:10:52.408121 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_invocation.py
--rw-r--r--   0        0        0     2163 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_sns.py
--rw-r--r--   0        0        0     2082 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
--rw-r--r--   0        0        0       22 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/mocks/__init__.py
--rw-r--r--   0        0        0       21 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/mocks/actions/__init__.py
--rw-r--r--   0        0        0      937 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/mocks/actions/ses.py
--rw-r--r--   0        0        0      326 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/__init__.py
--rw-r--r--   0        0        0     1919 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/__init__.py
--rw-r--r--   0        0        0     1082 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
--rw-r--r--   0        0        0     3467 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
--rw-r--r--   0        0        0     3776 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
--rw-r--r--   0        0        0     6444 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
--rw-r--r--   0        0        0     1443 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py
--rw-r--r--   0        0        0     1810 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/parameter_store.py
--rw-r--r--   0        0        0      761 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/parameter_store_test.py
--rw-r--r--   0        0        0     3056 2024-03-01 17:17:16.849026 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/secrets_manager.py
--rw-r--r--   0        0        0      786 2023-10-19 20:17:08.669304 clear_skies_aws-1.9.0/src/clearskies_aws/secrets/secrets_manager_test.py
--rw-r--r--   0        0        0     1776 2023-12-30 17:11:03.525609 clear_skies_aws-1.9.0/src/clearskies_aws/web_socket_connection_model.py
--rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/LICENSE
+-rw-r--r--   0        0        0     7780 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/README.md
+-rw-r--r--   0        0        0      789 2024-05-04 23:48:02.059008 clear_skies_aws-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-12-30 16:33:38.123814 clear_skies_aws-1.9.1/src/clearskies_aws/__init__.py
+-rw-r--r--   0        0        0     2865 2024-02-28 23:50:28.351377 clear_skies_aws-1.9.1/src/clearskies_aws/actions/__init__.py
+-rw-r--r--   0        0        0     3877 2024-03-20 10:13:37.291200 clear_skies_aws-1.9.1/src/clearskies_aws/actions/action_aws.py
+-rw-r--r--   0        0        0     4085 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/assume_role.py
+-rw-r--r--   0        0        0     2450 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/assume_role_test.py
+-rw-r--r--   0        0        0     7886 2024-05-04 23:47:53.230973 clear_skies_aws-1.9.1/src/clearskies_aws/actions/ses.py
+-rw-r--r--   0        0        0     3076 2024-05-04 23:45:51.234501 clear_skies_aws-1.9.1/src/clearskies_aws/actions/ses_test.py
+-rw-r--r--   0        0        0     2197 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/sns.py
+-rw-r--r--   0        0        0     2306 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/sns_test.py
+-rw-r--r--   0        0        0     2340 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/sqs.py
+-rw-r--r--   0        0        0     2346 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/sqs_test.py
+-rw-r--r--   0        0        0     2363 2024-03-08 14:32:55.873530 clear_skies_aws-1.9.1/src/clearskies_aws/actions/step_function.py
+-rw-r--r--   0        0        0     2742 2024-03-08 14:32:45.065230 clear_skies_aws-1.9.1/src/clearskies_aws/actions/step_function_test.py
+-rw-r--r--   0        0        0       83 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/backends/__init__.py
+-rw-r--r--   0        0        0    29126 2024-04-19 11:51:58.524701 clear_skies_aws-1.9.1/src/clearskies_aws/backends/dynamo_db_backend.py
+-rw-r--r--   0        0        0    13150 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/backends/dynamo_db_backend_test.py
+-rw-r--r--   0        0        0     2726 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/backends/sqs_backend.py
+-rw-r--r--   0        0        0     1138 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/backends/sqs_backend_test.py
+-rw-r--r--   0        0        0      472 2024-01-06 13:06:05.318595 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__init__.py
+-rw-r--r--   0        0        0     1305 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1276 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1251 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0      506 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/cli.py
+-rw-r--r--   0        0        0     1085 2024-01-06 13:10:52.693804 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/cli_websocket_mock.py
+-rw-r--r--   0        0        0     1002 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_api_gateway.py
+-rw-r--r--   0        0        0     1067 2023-12-18 00:15:49.555696 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_api_gateway_web_socket.py
+-rw-r--r--   0        0        0      952 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_elb.py
+-rw-r--r--   0        0        0     1009 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_http_gateway.py
+-rw-r--r--   0        0        0     1336 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_invocation.py
+-rw-r--r--   0        0        0     1317 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sns.py
+-rw-r--r--   0        0        0     1685 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
+-rw-r--r--   0        0        0     1999 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
+-rw-r--r--   0        0        0      510 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/wsgi.py
+-rw-r--r--   0        0        0       56 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/di/__init__.py
+-rw-r--r--   0        0        0      775 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/di/standard_dependencies.py
+-rw-r--r--   0        0        0      112 2024-03-29 18:03:20.842321 clear_skies_aws-1.9.1/src/clearskies_aws/handlers/__init__.py
+-rw-r--r--   0        0        0     7471 2024-03-29 18:02:23.674537 clear_skies_aws-1.9.1/src/clearskies_aws/handlers/secrets_manager_rotation.py
+-rw-r--r--   0        0        0     1449 2024-01-06 12:49:14.731820 clear_skies_aws-1.9.1/src/clearskies_aws/handlers/simple_body_routing.py
+-rw-r--r--   0        0        0      385 2024-01-06 13:10:44.713712 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__init__.py
+-rw-r--r--   0        0        0      943 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     3710 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     2761 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
+-rw-r--r--   0        0        0      901 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0      434 2024-01-06 13:10:39.925657 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/cli_websocket_mock.py
+-rw-r--r--   0        0        0     3401 2024-03-02 21:11:37.111733 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway.py
+-rw-r--r--   0        0        0     2845 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
+-rw-r--r--   0        0        0      308 2023-12-18 00:15:15.884654 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway_web_socket.py
+-rw-r--r--   0        0        0      750 2024-03-02 21:10:37.703292 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_elb.py
+-rw-r--r--   0        0        0      692 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_http_gateway.py
+-rw-r--r--   0        0        0      928 2023-10-20 10:10:52.408121 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_invocation.py
+-rw-r--r--   0        0        0     2163 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_sns.py
+-rw-r--r--   0        0        0     2082 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
+-rw-r--r--   0        0        0       22 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/mocks/__init__.py
+-rw-r--r--   0        0        0       21 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/mocks/actions/__init__.py
+-rw-r--r--   0        0        0      937 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/mocks/actions/ses.py
+-rw-r--r--   0        0        0      326 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/__init__.py
+-rw-r--r--   0        0        0     1919 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/__init__.py
+-rw-r--r--   0        0        0     1082 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
+-rw-r--r--   0        0        0     3467 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
+-rw-r--r--   0        0        0     3776 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
+-rw-r--r--   0        0        0     6444 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
+-rw-r--r--   0        0        0     1443 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py
+-rw-r--r--   0        0        0     1810 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/parameter_store.py
+-rw-r--r--   0        0        0      761 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/parameter_store_test.py
+-rw-r--r--   0        0        0     3056 2024-03-01 17:17:16.849026 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/secrets_manager.py
+-rw-r--r--   0        0        0      786 2023-10-19 20:17:08.669304 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/secrets_manager_test.py
+-rw-r--r--   0        0        0     1776 2023-12-30 17:11:03.525609 clear_skies_aws-1.9.1/src/clearskies_aws/web_socket_connection_model.py
+-rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.9.1/PKG-INFO
```

### Comparing `clear_skies_aws-1.9.0/LICENSE` & `clear_skies_aws-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/README.md` & `clear_skies_aws-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/pyproject.toml` & `clear_skies_aws-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-aws"
-version = "1.9.0"
+version = "1.9.1"
 description = "clearskies bindings for working in AWS"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
     "tnijboer"
 ]
 repository = "https://github.com/cmancone/clearskies-aws"
 license = "MIT"
```

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/__init__.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/action_aws.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/action_aws.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/assume_role.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/assume_role.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/assume_role_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/assume_role_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/ses.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/ses.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     def __init__(self, environment: Environment, boto3: boto3, di: StandardDependencies) -> None:
         """Setup action."""
         super().__init__(environment, boto3, di)
 
     def configure(
         self,
         sender,
-        to: Optional[Union[list, str]] = None,
-        cc: Optional[Union[list, str]] = None,
-        bcc: Optional[Union[list, str]] = None,
+        to: Optional[Union[list, str,  Callable]] = None,
+        cc: Optional[Union[list, str,  Callable]] = None,
+        bcc: Optional[Union[list, str,  Callable]] = None,
         subject: Optional[str] = None,
         message: Optional[str] = None,
         subject_template: Optional[str] = None,
         message_template: Optional[str] = None,
         subject_template_file: Optional[str] = None,
         message_template_file: Optional[str] = None,
         assume_role: Optional[AssumeRole] = None,
@@ -44,15 +44,15 @@
         }
         # this just moves the data from the various "to" inputs (to, cc, bcc) into the self.destinations
         # dictionary, after normalizing it so that it is always a list.
         for key in self.destinations.keys():
             destination_values = locals()[key]
             if not destination_values:
                 continue
-            if type(destination_values) == str:
+            if type(destination_values) == str or callable(destination_values):
                 self.destinations[key] = [destination_values]
             else:
                 self.destinations[key] = destination_values
         self.subject = subject
         self.message = message
         self.sender = sender
         self.subject_template = None
@@ -132,14 +132,25 @@
 
          1. An email address
          2. The name of a column in the model that contains an email address
         """
         resolved = []
         destinations = self.destinations[name]
         for destination in destinations:
+            if callable(destination):
+                more = self.di.call_function(destination, model=model)
+                if not isinstance(more, list):
+                    more = [more]
+                for entry in more:
+                    if not isinstance(entry, str):
+                        raise ValueError(f"I invoked a callable to fetch the '{name}' addresses for model '{model.__class__.__name__}' but it returned something other than a string.  Callables must return a valid email address or a list of email addresses.")
+                    if "@" not in entry:
+                        raise ValueError(f"I invoked a callable to fetch the '{name}' addresses for model '{model.__class__.__name__}' but it returned a non-email address.  Callables must return a valid email address or a list of email addresses.")
+                resolved.extend(more)
+                continue
             if "@" in destination:
                 resolved.append(destination)
                 continue
             resolved.append(model.get(destination))
         return resolved
 
     def _resolve_message_as_html(self, model: clearskies.Model, now: datetime.datetime) -> str:
```

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/ses_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/sns_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,77 @@
 import unittest
+import boto3
+
 from unittest.mock import MagicMock, call
-from .ses import SES
+from .sns import SNS
 import clearskies
 from ..di import StandardDependencies
-class SESTest(unittest.TestCase):
+import json
+from collections import OrderedDict
+class User(clearskies.Model):
+    def __init__(self, memory_backend, columns):
+        super().__init__(memory_backend, columns)
+
+    def columns_configuration(self):
+        return OrderedDict([
+            clearskies.column_types.string('name'),
+            clearskies.column_types.email('email'),
+        ])
+class SNSTest(unittest.TestCase):
     def setUp(self):
         self.di = StandardDependencies()
         self.di.bind('environment', {'AWS_REGION': 'us-east-2'})
-        self.ses = MagicMock()
-        self.ses.send_email = MagicMock()
+        self.users = self.di.build(User)
+        self.sns = MagicMock()
+        self.sns.publish = MagicMock()
         self.boto3 = MagicMock()
-        self.boto3.client = MagicMock(return_value=self.ses)
+        self.boto3.client = MagicMock(return_value=self.sns)
+        self.when = None
         self.environment = MagicMock()
         self.environment.get = MagicMock(return_value='us-east-1')
 
+    def always(self, model):
+        self.when = model
+        return True
+
+    def never(self, model):
+        self.when = model
+        return False
+
     def test_send(self):
-        ses = SES(self.environment, self.boto3, self.di)
-        ses.configure(
-            'test@example.com', to='jane@example.com', subject='welcome!', message_template='hi {{ model.id }}!'
+        sns = SNS(self.environment, self.boto3, self.di)
+        sns.configure(
+            topic='arn:aws:my-topic',
+            when=self.always,
         )
-        model = MagicMock()
-        model.id = 'asdf'
-        ses(model)
-        self.ses.send_email.assert_has_calls([
+        user = self.users.model({
+            "id": "1-2-3-4",
+            "name": "Jane",
+            "email": "jane@example.com",
+        })
+        sns(user)
+        self.sns.publish.assert_has_calls([
             call(
-                Destination={
-                    'ToAddresses': ['jane@example.com'],
-                    'CcAddresses': [],
-                    'BccAddresses': []
-                },
-                Message={
-                    'Body': {
-                        'Html': {
-                            'Charset': 'utf-8',
-                            'Data': 'hi asdf!'
-                        },
-                        'Text': {
-                            'Charset': 'utf-8',
-                            'Data': 'hi asdf!'
-                        }
-                    },
-                    'Subject': {
-                        'Charset': 'utf-8',
-                        'Data': 'welcome!'
-                    }
-                },
-                Source='test@example.com'
+                TopicArn='arn:aws:my-topic',
+                Message=json.dumps({
+                    "id": "1-2-3-4",
+                    "name": "Jane",
+                    "email": "jane@example.com",
+                }),
             ),
         ])
+        self.assertEqual(id(user), id(self.when))
+
+    def test_not_now(self):
+        sns = SNS(self.environment, self.boto3, self.di)
+        sns.configure(
+            topic='arn:aws:my-topic',
+            when=self.never,
+        )
+        user = self.users.model({
+            "id": "1-2-3-4",
+            "name": "Jane",
+            "email": "jane@example.com",
+        })
+        sns(user)
+        self.sns.publish.assert_not_called()
+        self.assertEqual(id(user), id(self.when))
```

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/sns.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/sns_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/sqs_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,75 @@
 import unittest
-import boto3
-
 from unittest.mock import MagicMock, call
-from .sns import SNS
+from .sqs import SQS
 import clearskies
 from ..di import StandardDependencies
 import json
 from collections import OrderedDict
 class User(clearskies.Model):
     def __init__(self, memory_backend, columns):
         super().__init__(memory_backend, columns)
 
     def columns_configuration(self):
         return OrderedDict([
             clearskies.column_types.string('name'),
             clearskies.column_types.email('email'),
         ])
-class SNSTest(unittest.TestCase):
+class SQSTest(unittest.TestCase):
     def setUp(self):
         self.di = StandardDependencies()
         self.di.bind('environment', {'AWS_REGION': 'us-east-2'})
         self.users = self.di.build(User)
-        self.sns = MagicMock()
-        self.sns.publish = MagicMock()
+        self.sqs = MagicMock()
+        self.sqs.send_message = MagicMock()
         self.boto3 = MagicMock()
-        self.boto3.client = MagicMock(return_value=self.sns)
+        self.boto3.client = MagicMock(return_value=self.sqs)
         self.when = None
         self.environment = MagicMock()
         self.environment.get = MagicMock(return_value='us-east-1')
 
     def always(self, model):
         self.when = model
         return True
 
     def never(self, model):
         self.when = model
         return False
 
     def test_send(self):
-        sns = SNS(self.environment, self.boto3, self.di)
-        sns.configure(
-            topic='arn:aws:my-topic',
+        sqs = SQS(self.environment, self.boto3, self.di)
+        sqs.configure(
+            queue_url='https://queue.example.com',
             when=self.always,
         )
         user = self.users.model({
             "id": "1-2-3-4",
             "name": "Jane",
             "email": "jane@example.com",
         })
-        sns(user)
-        self.sns.publish.assert_has_calls([
+        sqs(user)
+        self.sqs.send_message.assert_has_calls([
             call(
-                TopicArn='arn:aws:my-topic',
-                Message=json.dumps({
+                QueueUrl='https://queue.example.com',
+                MessageBody=json.dumps({
                     "id": "1-2-3-4",
                     "name": "Jane",
                     "email": "jane@example.com",
                 }),
             ),
         ])
         self.assertEqual(id(user), id(self.when))
 
     def test_not_now(self):
-        sns = SNS(self.environment, self.boto3, self.di)
-        sns.configure(
-            topic='arn:aws:my-topic',
+        sqs = SQS(self.environment, self.boto3, self.di)
+        sqs.configure(
+            queue_url='https://queue.example.com',
             when=self.never,
         )
         user = self.users.model({
             "id": "1-2-3-4",
             "name": "Jane",
             "email": "jane@example.com",
         })
-        sns(user)
-        self.sns.publish.assert_not_called()
+        sqs(user)
+        self.sqs.send_message.assert_not_called()
         self.assertEqual(id(user), id(self.when))
```

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/sqs.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/sqs.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/step_function.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/step_function.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/actions/step_function_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/actions/step_function_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/backends/dynamo_db_backend.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/backends/dynamo_db_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/backends/dynamo_db_backend_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/backends/dynamo_db_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/backends/sqs_backend.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/backends/sqs_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/backends/sqs_backend_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/backends/sqs_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/cli_websocket_mock.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/cli_websocket_mock.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_api_gateway.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_api_gateway_web_socket.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_api_gateway_web_socket.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_elb.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_http_gateway.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_invocation.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_sns.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/di/standard_dependencies.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/di/standard_dependencies.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/handlers/secrets_manager_rotation.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/handlers/secrets_manager_rotation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/handlers/simple_body_routing.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/handlers/simple_body_routing.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_api_gateway.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_elb.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_http_gateway.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_invocation.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_sns.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/input_outputs/lambda_sqs_standard.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_sqs_standard.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/mocks/actions/ses.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/mocks/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/__init__.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/parameter_store.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/parameter_store.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/parameter_store_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/parameter_store_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/secrets_manager.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/secrets/secrets_manager_test.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/secrets_manager_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/src/clearskies_aws/web_socket_connection_model.py` & `clear_skies_aws-1.9.1/src/clearskies_aws/web_socket_connection_model.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.0/PKG-INFO` & `clear_skies_aws-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-aws
-Version: 1.9.0
+Version: 1.9.1
 Summary: clearskies bindings for working in AWS
 Home-page: https://github.com/cmancone/clearskies-aws
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

