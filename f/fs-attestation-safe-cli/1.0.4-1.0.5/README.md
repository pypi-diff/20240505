# Comparing `tmp/fs_attestation_safe_cli-1.0.4.tar.gz` & `tmp/fs_attestation_safe_cli-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_attestation_safe_cli-1.0.4.tar", last modified: Sat May  4 04:20:36 2024, max compression
+gzip compressed data, was "fs_attestation_safe_cli-1.0.5.tar", last modified: Sat May  4 06:42:08 2024, max compression
```

## Comparing `fs_attestation_safe_cli-1.0.4.tar` & `fs_attestation_safe_cli-1.0.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 04:20:36.471690 fs_attestation_safe_cli-1.0.4/
--rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/LICENSE
--rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-04 04:20:36.471836 fs_attestation_safe_cli-1.0.4/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     3392 2024-05-03 11:53:59.000000 fs_attestation_safe_cli-1.0.4/README.md
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 04:20:36.451877 fs_attestation_safe_cli-1.0.4/fs_attestation_safe_cli.egg-info/
--rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-04 04:20:36.000000 fs_attestation_safe_cli-1.0.4/fs_attestation_safe_cli.egg-info/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     1997 2024-05-04 04:20:36.000000 fs_attestation_safe_cli-1.0.4/fs_attestation_safe_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mohan      (501) staff       (20)        1 2024-05-04 04:20:36.000000 fs_attestation_safe_cli-1.0.4/fs_attestation_safe_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mohan      (501) staff       (20)      105 2024-05-04 04:20:36.000000 fs_attestation_safe_cli-1.0.4/fs_attestation_safe_cli.egg-info/entry_points.txt
--rw-r--r--   0 mohan      (501) staff       (20)      163 2024-05-04 04:20:36.000000 fs_attestation_safe_cli-1.0.4/fs_attestation_safe_cli.egg-info/requires.txt
--rw-r--r--   0 mohan      (501) staff       (20)       15 2024-05-04 04:20:36.000000 fs_attestation_safe_cli-1.0.4/fs_attestation_safe_cli.egg-info/top_level.txt
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 04:20:36.457385 fs_attestation_safe_cli-1.0.4/safe_cli/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/argparse_validators.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 04:20:36.457912 fs_attestation_safe_cli-1.0.4/safe_cli/contracts/
--rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/contracts/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/contracts/safe_to_l2_migration.py
--rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     6519 2024-05-04 04:10:56.000000 fs_attestation_safe_cli-1.0.4/safe_cli/main.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 04:20:36.461187 fs_attestation_safe_cli-1.0.4/safe_cli/operators/
--rw-r--r--   0 mohan      (501) staff       (20)      347 2024-05-02 12:28:51.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/enums.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     2945 2024-05-02 12:26:43.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/fs_attestation_auth.py
--rw-r--r--   0 mohan      (501) staff       (20)    12479 2024-05-03 11:29:16.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/fs_attestation_service_operator.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 04:20:36.464561 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/constants.py
--rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/hw_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/ledger_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/trezor_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)    46526 2024-05-04 04:16:26.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    18731 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/operators/safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    24053 2024-05-03 11:26:34.000000 fs_attestation_safe_cli-1.0.4/safe_cli/prompt_parser.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)    10873 2024-05-03 11:30:32.000000 fs_attestation_safe_cli-1.0.4/safe_cli/safe_completer_constants.py
--rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)     1536 2024-05-03 11:27:04.000000 fs_attestation_safe_cli-1.0.4/safe_cli/safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/safe_cli/utils.py
--rw-r--r--   0 mohan      (501) staff       (20)       17 2024-05-04 04:20:02.000000 fs_attestation_safe_cli-1.0.4/safe_cli/version.py
--rw-r--r--   0 mohan      (501) staff       (20)      533 2024-05-04 04:20:36.472423 fs_attestation_safe_cli-1.0.4/setup.cfg
--rw-r--r--   0 mohan      (501) staff       (20)     1577 2024-04-25 06:49:01.000000 fs_attestation_safe_cli-1.0.4/setup.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 04:20:36.469936 fs_attestation_safe_cli-1.0.4/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 04:20:36.471354 fs_attestation_safe_cli-1.0.4/tests/mocks/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/mocks/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/mocks/balances_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/mocks/data_decoded_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/mocks/multisig_tx_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/mocks/txs_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/safe_cli_test_case_mixin.py
--rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_argparse_validators.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_entrypoint.py
--rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_safe_cli.py
--rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/test_utils.py
--rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.4/tests/utils.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 06:42:08.098445 fs_attestation_safe_cli-1.0.5/
+-rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/LICENSE
+-rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-04 06:42:08.098674 fs_attestation_safe_cli-1.0.5/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     3392 2024-05-03 11:53:59.000000 fs_attestation_safe_cli-1.0.5/README.md
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 06:42:08.072165 fs_attestation_safe_cli-1.0.5/fs_attestation_safe_cli.egg-info/
+-rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-04 06:42:07.000000 fs_attestation_safe_cli-1.0.5/fs_attestation_safe_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     1997 2024-05-04 06:42:08.000000 fs_attestation_safe_cli-1.0.5/fs_attestation_safe_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mohan      (501) staff       (20)        1 2024-05-04 06:42:07.000000 fs_attestation_safe_cli-1.0.5/fs_attestation_safe_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      105 2024-05-04 06:42:07.000000 fs_attestation_safe_cli-1.0.5/fs_attestation_safe_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      163 2024-05-04 06:42:07.000000 fs_attestation_safe_cli-1.0.5/fs_attestation_safe_cli.egg-info/requires.txt
+-rw-r--r--   0 mohan      (501) staff       (20)       15 2024-05-04 06:42:07.000000 fs_attestation_safe_cli-1.0.5/fs_attestation_safe_cli.egg-info/top_level.txt
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 06:42:08.077754 fs_attestation_safe_cli-1.0.5/safe_cli/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/argparse_validators.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 06:42:08.078691 fs_attestation_safe_cli-1.0.5/safe_cli/contracts/
+-rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/contracts/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/contracts/safe_to_l2_migration.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6461 2024-05-04 05:09:20.000000 fs_attestation_safe_cli-1.0.5/safe_cli/main.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 06:42:08.082890 fs_attestation_safe_cli-1.0.5/safe_cli/operators/
+-rw-r--r--   0 mohan      (501) staff       (20)      347 2024-05-02 12:28:51.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/enums.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2945 2024-05-02 12:26:43.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/fs_attestation_auth.py
+-rw-r--r--   0 mohan      (501) staff       (20)    12479 2024-05-04 04:55:58.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/fs_attestation_service_operator.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 06:42:08.087849 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/hw_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/ledger_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/trezor_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)    46560 2024-05-04 05:19:18.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    18731 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/operators/safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    24053 2024-05-03 11:26:34.000000 fs_attestation_safe_cli-1.0.5/safe_cli/prompt_parser.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)    10873 2024-05-03 11:30:32.000000 fs_attestation_safe_cli-1.0.5/safe_cli/safe_completer_constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1536 2024-05-03 11:27:04.000000 fs_attestation_safe_cli-1.0.5/safe_cli/safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/safe_cli/utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)       17 2024-05-04 06:41:56.000000 fs_attestation_safe_cli-1.0.5/safe_cli/version.py
+-rw-r--r--   0 mohan      (501) staff       (20)      533 2024-05-04 06:42:08.099422 fs_attestation_safe_cli-1.0.5/setup.cfg
+-rw-r--r--   0 mohan      (501) staff       (20)     1577 2024-05-04 05:16:29.000000 fs_attestation_safe_cli-1.0.5/setup.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 06:42:08.095575 fs_attestation_safe_cli-1.0.5/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 06:42:08.097846 fs_attestation_safe_cli-1.0.5/tests/mocks/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/mocks/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/mocks/balances_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/mocks/data_decoded_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/mocks/multisig_tx_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/mocks/txs_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/safe_cli_test_case_mixin.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_argparse_validators.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_entrypoint.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_safe_cli.py
+-rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/test_utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.5/tests/utils.py
```

### Comparing `fs_attestation_safe_cli-1.0.4/LICENSE` & `fs_attestation_safe_cli-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/PKG-INFO` & `fs_attestation_safe_cli-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs_attestation_safe_cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: Modified Command Line Interface for FailSafe Attestation Service to administrate Gnosis Safe Wallets and FailSafe Attestation Guard Contracts
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.4/README.md` & `fs_attestation_safe_cli-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/fs_attestation_safe_cli.egg-info/PKG-INFO` & `fs_attestation_safe_cli-1.0.5/fs_attestation_safe_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-attestation-safe-cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: Modified Command Line Interface for FailSafe Attestation Service to administrate Gnosis Safe Wallets and FailSafe Attestation Guard Contracts
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.4/fs_attestation_safe_cli.egg-info/SOURCES.txt` & `fs_attestation_safe_cli-1.0.5/fs_attestation_safe_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/argparse_validators.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/contracts/safe_to_l2_migration.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/contracts/safe_to_l2_migration.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/main.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,21 @@
         :param safe_address: Safe address
         :param node_url: Ethereum RPC url
         :param history: If `True` keep command history, otherwise history is not kept after closing the CLI
         """
         self.safe_address = safe_address
         self.node_url = node_url
         self.fs_attestation_service_base_url = fs_attestation_service_base_url
-        print("fs_attestation_service_base_url: ", fs_attestation_service_base_url)
         if history:
             self.session = PromptSession(
                 history=FileHistory(os.path.join(sys.path[0], ".history"))
             )
         else:
             self.session = PromptSession()
-        self.safe_operator = SafeOperator(safe_address, node_url)
+        self.safe_operator = SafeOperator(safe_address, node_url, safe_tx_service_base_url)
         self.fs_attestation_service_operator = FailSafeAttestationServiceOperator(safe_address, node_url, safe_tx_service_base_url, fs_attestation_service_base_url)
         self.prompt_parser = PromptParser(self.safe_operator, self.fs_attestation_service_operator)
 
     def print_startup_info(self):
         print_formatted_text(tprint("FailSafe Attestation"))  # Print fancy text
         print_formatted_text(text2art("Safe CLI"))  # Print fancy text
         print_formatted_text(HTML(f"<b><ansigreen>Version {version}</ansigreen></b>"))
```

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/exceptions.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/fs_attestation_auth.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/fs_attestation_auth.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/fs_attestation_service_operator.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/fs_attestation_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/hw_wallet.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/hw_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/ledger_exceptions.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/ledger_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/ledger_wallet.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/trezor_exceptions.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/trezor_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/hw_wallets/trezor_wallet.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/hw_wallets/trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/safe_operator.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/safe_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 
     return decorated
 
 
 class SafeOperator:
     address: ChecksumAddress
     node_url: str
+    safe_tx_service_base_url: str
     ethereum_client: EthereumClient
     ens: ENS
     network: EthereumNetwork
     etherscan: Optional[EtherscanClient]
     safe_tx_service: Optional[TransactionServiceApi]
     safe: Safe
     safe_contract: Contract
```

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/operators/safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/operators/safe_tx_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/prompt_parser.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/safe_addresses.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/safe_completer.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/safe_completer_constants.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/safe_completer_constants.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/safe_creator.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/safe_lexer.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/safe_lexer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/safe_cli/utils.py` & `fs_attestation_safe_cli-1.0.5/safe_cli/utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/setup.cfg` & `fs_attestation_safe_cli-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/setup.py` & `fs_attestation_safe_cli-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     test_suite="tests",
     install_requires=[
         "art>=6",
         "colorama>=0.4",
         "prompt_toolkit>=3",
         "pygments>=2",
         "requests>=2",
-        "fs-attestation-safe-eth-py==1.0.2",
+        "fs-attestation-safe-eth-py==1.0.3",
         "tabulate>=0.8",
     ],
     extras_require={"ledger": ["ledgereth==0.9.1"], "trezor": ["trezor==0.13.8"]},
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
             "fs-attestation-safe-cli=safe_cli.main:main",
```

### Comparing `fs_attestation_safe_cli-1.0.4/tests/mocks/balances_mock.py` & `fs_attestation_safe_cli-1.0.5/tests/mocks/balances_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/mocks/data_decoded_mock.py` & `fs_attestation_safe_cli-1.0.5/tests/mocks/data_decoded_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/mocks/multisig_tx_mock.py` & `fs_attestation_safe_cli-1.0.5/tests/mocks/multisig_tx_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/mocks/txs_mock.py` & `fs_attestation_safe_cli-1.0.5/tests/mocks/txs_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/safe_cli_test_case_mixin.py` & `fs_attestation_safe_cli-1.0.5/tests/safe_cli_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_argparse_validators.py` & `fs_attestation_safe_cli-1.0.5/tests/test_argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_entrypoint.py` & `fs_attestation_safe_cli-1.0.5/tests/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.5/tests/test_ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.5/tests/test_hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_ledger_wallet.py` & `fs_attestation_safe_cli-1.0.5/tests/test_ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_safe_addresses.py` & `fs_attestation_safe_cli-1.0.5/tests/test_safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_safe_cli.py` & `fs_attestation_safe_cli-1.0.5/tests/test_safe_cli.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_safe_completer.py` & `fs_attestation_safe_cli-1.0.5/tests/test_safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_safe_creator.py` & `fs_attestation_safe_cli-1.0.5/tests/test_safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_safe_lexer.py` & `fs_attestation_safe_cli-1.0.5/tests/test_safe_lexer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_safe_operator.py` & `fs_attestation_safe_cli-1.0.5/tests/test_safe_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.5/tests/test_safe_tx_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_trezor_wallet.py` & `fs_attestation_safe_cli-1.0.5/tests/test_trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/test_utils.py` & `fs_attestation_safe_cli-1.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.4/tests/utils.py` & `fs_attestation_safe_cli-1.0.5/tests/utils.py`

 * *Files identical despite different names*

