# Comparing `tmp/OZI-1.4.1.tar.gz` & `tmp/OZI-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.4.1.tar", last modified: Sun May  5 00:19:58 2024, max compression
+gzip compressed data, was "OZI-1.4.2.tar", last modified: Sun May  5 04:35:02 2024, max compression
```

## Comparing `OZI-1.4.1.tar` & `OZI-1.4.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.394318 OZI-1.4.1/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.366318 OZI-1.4.1/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.366318 OZI-1.4.1/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.366318 OZI-1.4.1/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-05-05 00:16:04.000000 OZI-1.4.1/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-05 00:16:04.000000 OZI-1.4.1/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   299617 2024-05-05 00:16:04.000000 OZI-1.4.1/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-05 00:16:04.000000 OZI-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-05 00:19:58.170318 OZI-1.4.1/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-05 00:16:04.000000 OZI-1.4.1/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16724 2024-05-05 00:16:04.000000 OZI-1.4.1/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-05 00:16:04.000000 OZI-1.4.1/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.390318 OZI-1.4.1/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.378318 OZI-1.4.1/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.378318 OZI-1.4.1/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.378318 OZI-1.4.1/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.378318 OZI-1.4.1/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.382318 OZI-1.4.1/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.378318 OZI-1.4.1/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.378318 OZI-1.4.1/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.378318 OZI-1.4.1/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.382318 OZI-1.4.1/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.382318 OZI-1.4.1/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.382318 OZI-1.4.1/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.382318 OZI-1.4.1/ozi/lint/restructuredtext-lint/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/restructuredtext-lint/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/lint/restructuredtext-lint/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.382318 OZI-1.4.1/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     4854 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.386318 OZI-1.4.1/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.390318 OZI-1.4.1/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6066 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6360 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.390318 OZI-1.4.1/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.390318 OZI-1.4.1/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.390318 OZI-1.4.1/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.394318 OZI-1.4.1/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.394318 OZI-1.4.1/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-05 00:16:04.000000 OZI-1.4.1/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10899 2024-05-05 00:16:04.000000 OZI-1.4.1/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-05-05 00:16:04.000000 OZI-1.4.1/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.394318 OZI-1.4.1/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-05 00:16:04.000000 OZI-1.4.1/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:58.394318 OZI-1.4.1/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-05 00:16:04.000000 OZI-1.4.1/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11072 2024-05-05 00:16:04.000000 OZI-1.4.1/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-05-05 00:16:04.000000 OZI-1.4.1/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-05 00:16:04.000000 OZI-1.4.1/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.441914 OZI-1.4.2/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.413914 OZI-1.4.2/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.413914 OZI-1.4.2/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.413914 OZI-1.4.2/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-05 04:30:50.000000 OZI-1.4.2/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   299924 2024-05-05 04:30:50.000000 OZI-1.4.2/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-05 04:30:50.000000 OZI-1.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-05 04:35:02.213912 OZI-1.4.2/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-05 04:30:50.000000 OZI-1.4.2/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    16724 2024-05-05 04:30:50.000000 OZI-1.4.2/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-05 04:30:50.000000 OZI-1.4.2/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.421914 OZI-1.4.2/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.421914 OZI-1.4.2/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.421914 OZI-1.4.2/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.429914 OZI-1.4.2/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.429914 OZI-1.4.2/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.429914 OZI-1.4.2/ozi/lint/restructuredtext-lint/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/restructuredtext-lint/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/restructuredtext-lint/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.429914 OZI-1.4.2/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     4854 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.433914 OZI-1.4.2/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.433914 OZI-1.4.2/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6066 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6345 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.433914 OZI-1.4.2/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10899 2024-05-05 04:30:50.000000 OZI-1.4.2/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-05-05 04:30:50.000000 OZI-1.4.2/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.441914 OZI-1.4.2/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-05 04:30:50.000000 OZI-1.4.2/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.441914 OZI-1.4.2/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-05 04:30:50.000000 OZI-1.4.2/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11072 2024-05-05 04:30:50.000000 OZI-1.4.2/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-05-05 04:30:50.000000 OZI-1.4.2/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-05 04:30:50.000000 OZI-1.4.2/tests/test_tap.py
```

### Comparing `OZI-1.4.1/.github/CODEOWNERS` & `OZI-1.4.2/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/CODE_OF_CONDUCT.md` & `OZI-1.4.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/CONTRIBUTING.md` & `OZI-1.4.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/SECURITY.md` & `OZI-1.4.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/workflows/codeql.yml` & `OZI-1.4.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/workflows/dependency-review.yml` & `OZI-1.4.2/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/workflows/dev-workflow.yml` & `OZI-1.4.2/.github/workflows/dev-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/workflows/dist-workflow.yml` & `OZI-1.4.2/.github/workflows/dist-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.github/workflows/scorecard.yml` & `OZI-1.4.2/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/.gitignore` & `OZI-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/CHANGELOG.md` & `OZI-1.4.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,18 @@
 # CHANGELOG
+## 1.4.2 (2024-05-05)
+
+### :bug:
+
+* :bug: correct deprecated Python warnings.
+
+User-facing deprecation warnings should always use FutureWarning.
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`df2de03`](https://github.com/OZI-Project/OZI/commit/df2de0354a546f6a092c277a479b2e0fa6b2edb5))
+
 ## 1.4.1 (2024-05-05)
 
 ### :bug:
 
 * :bug: Update ozi.spec.python
 
 PendingDeprecationWarning 52 weeks prior to python end-of-life
```

### Comparing `OZI-1.4.1/LICENSE.txt` & `OZI-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/PKG-INFO` & `OZI-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.4.1
+Version: 1.4.2
 Summary: Packager for Python projects using Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.4.1.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.4.2.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Rose Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
```

### Comparing `OZI-1.4.1/README.rst` & `OZI-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/meson.build` & `OZI-1.4.2/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/meson.options` & `OZI-1.4.2/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/__main__.py` & `OZI-1.4.2/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/actions.py` & `OZI-1.4.2/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/comment.py` & `OZI-1.4.2/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/fix/__main__.py` & `OZI-1.4.2/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/fix/build_definition.py` & `OZI-1.4.2/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/fix/meson.build` & `OZI-1.4.2/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/fix/missing.py` & `OZI-1.4.2/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/fix/parser.py` & `OZI-1.4.2/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/fix/rewrite_command.py` & `OZI-1.4.2/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/lint/meson.build` & `OZI-1.4.2/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/lint/pyright/meson.build` & `OZI-1.4.2/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/meson.build` & `OZI-1.4.2/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/meson.py` & `OZI-1.4.2/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/new/__main__.py` & `OZI-1.4.2/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/new/meson.build` & `OZI-1.4.2/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/new/parser.py` & `OZI-1.4.2/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/new/validate.py` & `OZI-1.4.2/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/pkg_extra.py` & `OZI-1.4.2/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/render.py` & `OZI-1.4.2/ozi/render.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/scripts/core_metadata_template.py` & `OZI-1.4.2/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/scripts/meson.build` & `OZI-1.4.2/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.4.2/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.4.2/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/scripts/render_requirements.py` & `OZI-1.4.2/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.4.2/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/scripts/scm_version_snip.py` & `OZI-1.4.2/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/scripts/to_distribution_template.py` & `OZI-1.4.2/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/scripts/version_metadata_template.py` & `OZI-1.4.2/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/spdx.py` & `OZI-1.4.2/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/spec/_license.py` & `OZI-1.4.2/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/spec/_spec.py` & `OZI-1.4.2/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/spec/base.py` & `OZI-1.4.2/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/spec/ci.py` & `OZI-1.4.2/ozi/spec/ci.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/spec/meson.build` & `OZI-1.4.2/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/spec/pkg.py` & `OZI-1.4.2/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/spec/project.py` & `OZI-1.4.2/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/spec/python.py` & `OZI-1.4.2/ozi/spec/python.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,21 +74,21 @@
             .replace(tzinfo=timezone.utc)
             .date()
         )
         ozi_support_eol = python3_eol - timedelta(weeks=DEPRECATION_DELTA_WEEKS)
         if datetime.now(tz=timezone.utc).date() > python3_eol:  # pragma: no cover
             warn(
                 f'Python {pymajor}.{pyminor}.{pypatch} is not supported as of {python3_eol}.',
-                DeprecationWarning,
+                RuntimeWarning,
             )
         elif datetime.now(tz=timezone.utc).date() > ozi_support_eol:  # pragma: no cover
             warn(
                 f'Python {pymajor}.{pyminor}.{pypatch} support is pending deprecation '
                 f'as of {ozi_support_eol}.',
-                PendingDeprecationWarning,
+                RuntimeWarning,
             )
 
     @cached_property
     def _minor_versions(self: Self) -> list[int]:
         return sorted(
             [
                 k
```

### Comparing `OZI-1.4.1/ozi/spec/src.py` & `OZI-1.4.2/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/tap.py` & `OZI-1.4.2/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/trove.py` & `OZI-1.4.2/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/vendor/email_validator/__init__.py` & `OZI-1.4.2/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/vendor/email_validator/__main__.py` & `OZI-1.4.2/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/vendor/email_validator/deliverability.py` & `OZI-1.4.2/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.4.2/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/vendor/email_validator/meson.build` & `OZI-1.4.2/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.4.2/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/vendor/email_validator/syntax.py` & `OZI-1.4.2/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/vendor/email_validator/validate_email.py` & `OZI-1.4.2/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/ozi/vendor/meson.build` & `OZI-1.4.2/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/pyproject.toml` & `OZI-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/templates/CHANGELOG.md.j2` & `OZI-1.4.2/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/tests/meson.build` & `OZI-1.4.2/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/tests/test_ozi_fix.py` & `OZI-1.4.2/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/tests/test_ozi_new.py` & `OZI-1.4.2/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.1/tests/test_tap.py` & `OZI-1.4.2/tests/test_tap.py`

 * *Files identical despite different names*
