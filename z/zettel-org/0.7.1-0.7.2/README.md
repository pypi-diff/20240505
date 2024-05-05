# Comparing `tmp/zettel_org-0.7.1.tar.gz` & `tmp/zettel_org-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zettel_org-0.7.1.tar", last modified: Fri May  3 01:37:12 2024, max compression
+gzip compressed data, was "zettel_org-0.7.2.tar", last modified: Sun May  5 20:46:54 2024, max compression
```

## Comparing `zettel_org-0.7.1.tar` & `zettel_org-0.7.2.tar`

### file list

```diff
@@ -1,192 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.122495 zettel_org-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.102494 zettel_org-0.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.102494 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.102494 zettel_org-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-03 01:37:00.000000 zettel_org-0.7.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-03 01:37:00.000000 zettel_org-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 01:37:00.000000 zettel_org-0.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-03 01:37:00.000000 zettel_org-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 01:37:00.000000 zettel_org-0.7.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-03 01:37:00.000000 zettel_org-0.7.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-05-03 01:37:12.122495 zettel_org-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-05-03 01:37:00.000000 zettel_org-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.102494 zettel_org-0.7.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2663 2024-05-03 01:37:00.000000 zettel_org-0.7.1/bin/build_zorg_grammars
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-05-03 01:37:00.000000 zettel_org-0.7.1/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-03 01:37:00.000000 zettel_org-0.7.1/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-05-03 01:37:00.000000 zettel_org-0.7.1/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-05-03 01:37:00.000000 zettel_org-0.7.1/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.102494 zettel_org-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.102494 zettel_org-0.7.1/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.106494 zettel_org-0.7.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.106494 zettel_org-0.7.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.106494 zettel_org-0.7.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 01:37:00.000000 zettel_org-0.7.1/docs/source/zorg.rst
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 01:37:00.000000 zettel_org-0.7.1/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.094494 zettel_org-0.7.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.106494 zettel_org-0.7.1/examples/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_file/20240323.zo
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_file/basic.zo
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_file/multiblocks.zo
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_file/priority.zo
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_file/property.zo
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_file/scrambled_prj_notes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_file/subnotes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_file/subsections.zo
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_file/tags_and_ids.zo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.106494 zettel_org-0.7.1/examples/zorg_query/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_query/all_contexts.zoq
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 01:37:00.000000 zettel_org-0.7.1/examples/zorg_query/open_projects.zoq
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.106494 zettel_org-0.7.1/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-03 01:37:00.000000 zettel_org-0.7.1/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-03 01:37:00.000000 zettel_org-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-03 01:37:00.000000 zettel_org-0.7.1/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-03 01:37:00.000000 zettel_org-0.7.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 01:37:00.000000 zettel_org-0.7.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-03 01:37:00.000000 zettel_org-0.7.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.106494 zettel_org-0.7.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 01:37:00.000000 zettel_org-0.7.1/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-03 01:37:12.122495 zettel_org-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-03 01:37:00.000000 zettel_org-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.094494 zettel_org-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.122495 zettel_org-0.7.1/src/zettel_org.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-05-03 01:37:12.000000 zettel_org-0.7.1/src/zettel_org.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-03 01:37:12.000000 zettel_org-0.7.1/src/zettel_org.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:37:12.000000 zettel_org-0.7.1/src/zettel_org.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 01:37:12.000000 zettel_org-0.7.1/src/zettel_org.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:37:08.000000 zettel_org-0.7.1/src/zettel_org.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 01:37:12.000000 zettel_org-0.7.1/src/zettel_org.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 01:37:12.000000 zettel_org-0.7.1/src/zettel_org.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.110494 zettel_org-0.7.1/src/zorg/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.110494 zettel_org-0.7.1/src/zorg/app/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.110494 zettel_org-0.7.1/src/zorg/app/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/runners/_run_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/runners/_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/runners/_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/runners/_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/runners/_run_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/runners/_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/app/runners/_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.110494 zettel_org-0.7.1/src/zorg/domain/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.110494 zettel_org-0.7.1/src/zorg/domain/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/domain/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/domain/messages/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/domain/messages/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.110494 zettel_org-0.7.1/src/zorg/domain/models/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/domain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/domain/models/_zorg_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/domain/models/_zorg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/domain/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.110494 zettel_org-0.7.1/src/zorg/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.114494 zettel_org-0.7.1/src/zorg/grammar/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFile.g4
--rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFile.interp
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFile.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   119519 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.114494 zettel_org-0.7.1/src/zorg/grammar/zorg_query/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_query/ZorgQuery.g4
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_query/ZorgQuery.interp
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_query/ZorgQuery.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_query/ZorgQueryLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_query/ZorgQueryListener.py
--rw-r--r--   0 runner    (1001) docker     (127)    23293 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_query/ZorgQueryParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/grammar/zorg_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.114494 zettel_org-0.7.1/src/zorg/service/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.114494 zettel_org-0.7.1/src/zorg/service/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/compiler/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/compiler/_file_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/compiler/_query_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/messagebus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/service/zid_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.114494 zettel_org-0.7.1/src/zorg/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.118495 zettel_org-0.7.1/src/zorg/storage/file/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/file/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/file/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.118495 zettel_org-0.7.1/src/zorg/storage/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/sql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/sql/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/sql/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-03 01:37:00.000000 zettel_org-0.7.1/src/zorg/storage/sql/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-03 01:37:00.000000 zettel_org-0.7.1/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.118495 zettel_org-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.118495 zettel_org-0.7.1/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    71232 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/__snapshots__/test_run_compile.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/__snapshots__/test_run_db.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/__snapshots__/test_run_edit.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/__snapshots__/test_run_template.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:37:12.122495 zettel_org-0.7.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/data/day_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/data/done_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/data/habit_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/data/hello.zot
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/data/links.zo
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/test_file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/test_run_action_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/test_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/test_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/test_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tests/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-03 01:37:00.000000 zettel_org-0.7.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.732855 zettel_org-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.708855 zettel_org-0.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-05 20:46:46.000000 zettel_org-0.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-05 20:46:46.000000 zettel_org-0.7.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-05 20:46:46.000000 zettel_org-0.7.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-05 20:46:46.000000 zettel_org-0.7.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-05 20:46:46.000000 zettel_org-0.7.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-05-05 20:46:54.732855 zettel_org-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-05-05 20:46:46.000000 zettel_org-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3093 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/build_zorg_grammars
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/zorg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 20:46:46.000000 zettel_org-0.7.2/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.704855 zettel_org-0.7.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/examples/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/20240323.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/basic.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/multiblocks.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/priority.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/property.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/scrambled_prj_notes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/subnotes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/subsections.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/tags_and_ids.zo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/examples/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_query/all_contexts.zoq
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_query/open_projects.zoq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-05 20:46:46.000000 zettel_org-0.7.2/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-05 20:46:46.000000 zettel_org-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 20:46:46.000000 zettel_org-0.7.2/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-05 20:46:46.000000 zettel_org-0.7.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-05 20:46:46.000000 zettel_org-0.7.2/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-05 20:46:46.000000 zettel_org-0.7.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-05 20:46:46.000000 zettel_org-0.7.2/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-05 20:46:54.732855 zettel_org-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-05 20:46:46.000000 zettel_org-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.704855 zettel_org-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.732855 zettel_org-0.7.2/src/zettel_org.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:46:50.000000 zettel_org-0.7.2/src/zettel_org.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/src/zorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/src/zorg/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/domain/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/messages/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/messages/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/domain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/models/_zorg_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/models/_zorg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/CommonLexerRules.g4
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/ZorgFile.g4
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/ZorgQuery.g4
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/grammar/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)    16154 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFile.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFile.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120709 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/grammar/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQuery.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQuery.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65908 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/service/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/compiler/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/compiler/_file_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/compiler/_query_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/messagebus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/service/swog/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/swog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/swog/_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/zid_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.728855 zettel_org-0.7.2/src/zorg/storage/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-05 20:46:46.000000 zettel_org-0.7.2/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.728855 zettel_org-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.728855 zettel_org-0.7.2/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    71784 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_compile.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_db.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_edit.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    23947 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_query.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_template.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.732855 zettel_org-0.7.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/day_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/done_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/habit_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/hello.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/links.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_action_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tox.ini
```

### Comparing `zettel_org-0.7.1/.cruft.json` & `zettel_org-0.7.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/.github/labels.yml` & `zettel_org-0.7.2/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/.github/workflows/ci.yml` & `zettel_org-0.7.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/.gitignore` & `zettel_org-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/.pylintrc` & `zettel_org-0.7.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/.readthedocs.yml` & `zettel_org-0.7.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/CHANGELOG.md` & `zettel_org-0.7.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.7.1...HEAD)
+## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.7.2...HEAD)
+
+
+## [0.7.2](https://github.com/bbugyi200/zorg/compare/0.7.1...0.7.2) - 2024-05-05
+
+### Added
+
+* Implement basic functionality for `zorg query`. We can now SELECT notes with
+  a (very limited ATM) WHERE filter and GROUP BY various dimensions (e.g. file,
+  note type, projects).
 
 
 ## [0.7.1](https://github.com/bbugyi200/zorg/compare/0.7.0...0.7.1) - 2024-05-02
 
 ### Fixed
 
 * Stop removing 'edit' vim commands with no args.
```

### Comparing `zettel_org-0.7.1/CONTRIBUTING.md` & `zettel_org-0.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/Dockerfile` & `zettel_org-0.7.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/Makefile` & `zettel_org-0.7.2/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/PKG-INFO` & `zettel_org-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.7.1
+Version: 0.7.2
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: antlr4-python3-runtime~=4.13
 Requires-Dist: bolton-clack~=0.3.12
 Requires-Dist: bolton-eris~=0.2.3
 Requires-Dist: bolton-logrus~=0.1.1
 Requires-Dist: bolton-typist~=0.2.0
 Requires-Dist: jinja2
-Requires-Dist: potoroo~=0.6.0
+Requires-Dist: rich~=13.7
 Requires-Dist: sqlmodel~=0.0.16
 Requires-Dist: tqdm~=4.66
 Requires-Dist: vimala~=0.2.0
 
 # zorg
 
 **The zettel note manager of the future.**
```

### Comparing `zettel_org-0.7.1/README.md` & `zettel_org-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/bin/build_zorg_grammars` & `zettel_org-0.7.2/bin/build_zorg_grammars`

 * *Files 9% similar despite different names*

```diff
@@ -53,22 +53,34 @@
   for dir in $(find src/zorg/grammar -maxdepth 1 -mindepth 1 -type d | xargs -I_ basename _); do
     if [[ "${dir}" == "_"* ]]; then
       log::debug "Skipping the %s directory." "${dir}"
       continue
     fi
 
     log::info "Generating %s parser using antlr4." $dir
-    antlr4 -Dlanguage=Python3 src/zorg/grammar/$dir/*.g4
+
+		# Convert from snake_case to UpperCammelCase
+		local g4_stem=$(echo "$dir" | sed -r 's/(_[a-z])/\U\1/g ; s/^[a-z]/\U&/ ; s/_//')
+    local grammar_dir=src/zorg/grammar
+    local g4_path=$grammar_dir/$g4_stem.g4
+
+    # HACK: This was the only way I could get antlr to stop putting the
+    #   generated files in double-nested dirs like
+    #   src/zorg/grammar/zorg_file/src/zorg/grammar/zorg_file
+    pushd $grammar_dir >/dev/null
+    antlr4 -Dlanguage=Python3 $g4_stem.g4 -o $dir
+    popd >/dev/null
+
     for f in examples/$dir/*.zo*; do
       if [[ "${f}" != *"${ZO_NAME}"* ]]; then
         continue
       fi
       log::info "Contructing syntax tree from %s example file." $f
       echo "##### $f" >> $TMP_ERROR_FILE
-      antlr4-parse src/zorg/grammar/$dir/*.g4 prog "${parse_cmds[@]}" $f 3>&1 1>&2 2>&3 | tee /dev/stderr >> $TMP_ERROR_FILE
+      antlr4-parse $g4_path prog "${parse_cmds[@]}" $f 3>&1 1>&2 2>&3 | tee /dev/stderr >> $TMP_ERROR_FILE
       echo >> $TMP_ERROR_FILE
     done
 
     remove_header $TMP_ERROR_FILE > $TMP_ERROR_FILE_NO_HEADERS
     if [ -s $TMP_ERROR_FILE_NO_HEADERS ]; then
       log::error "Errors were logged while parsing some of the example files:"
       echo
```

### Comparing `zettel_org-0.7.1/bin/check_cc` & `zettel_org-0.7.2/bin/check_cc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/bin/publish_docs` & `zettel_org-0.7.2/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/bin/quick-lints` & `zettel_org-0.7.2/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/bin/render_all_cogs` & `zettel_org-0.7.2/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/docs/Makefile` & `zettel_org-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/docs/make.bat` & `zettel_org-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/docs/source/conf.py` & `zettel_org-0.7.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/examples/zorg_file/20240323.zo` & `zettel_org-0.7.2/examples/zorg_file/20240323.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/examples/zorg_file/scrambled_prj_notes.zo` & `zettel_org-0.7.2/examples/zorg_file/scrambled_prj_notes.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/lib/bugyi.sh` & `zettel_org-0.7.2/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/requirements-dev.in` & `zettel_org-0.7.2/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/requirements-dev.txt` & `zettel_org-0.7.2/requirements-dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,29 @@
     #   zettel-org
 antlr4-tools==0.2.1
     # via -r requirements-dev.in
 arrow==1.3.0
     # via cookiecutter
 astroid==3.1.0
     # via pylint
-babel==2.14.0
+babel==2.15.0
     # via sphinx
 binaryornot==0.4.4
     # via cookiecutter
 black==24.4.2
     # via -r requirements-dev.in
 bolton-clack==0.3.12
     # via
     #   -r requirements.in
     #   zettel-org
 bolton-eris==0.2.3
     # via
     #   -r requirements.in
     #   bolton-clack
     #   bolton-proctor
-    #   potoroo
     #   zettel-org
 bolton-ion==0.1.0
     # via bolton-eris
 bolton-logrus==0.1.3
     # via
     #   -r requirements.in
     #   bolton-clack
@@ -74,15 +73,15 @@
     #   cruft
     #   pip-tools
     #   typer
 cogapp==3.4.1
     # via -r requirements-dev.in
 cookiecutter==2.6.0
     # via cruft
-coverage[toml]==7.5.0
+coverage[toml]==7.5.1
     # via pytest-cov
 cruft[pyproject]==2.15.0
     # via -r requirements-dev.in
 dill==0.3.8
     # via pylint
 distlib==0.3.8
     # via virtualenv
@@ -162,18 +161,14 @@
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.5.0
     # via
     #   pytest
     #   tox
-potoroo==0.6.0
-    # via
-    #   -r requirements.in
-    #   zettel-org
 py==1.11.0
     # via tox
 pycodestyle==2.11.1
     # via flake8
 pydantic==2.7.1
     # via
     #   bolton-clack
@@ -183,15 +178,15 @@
     # via pydantic
 pydantic-settings==2.2.1
     # via bolton-clack
 pydocstyle[toml]==6.3.0
     # via -r requirements-dev.in
 pyflakes==3.2.0
     # via flake8
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   rich
     #   sphinx
 pylint==3.1.0
     # via -r requirements-dev.in
 pyproject-hooks==1.1.0
     # via
@@ -221,16 +216,18 @@
     #   cookiecutter
 requests==2.31.0
     # via
     #   cookiecutter
     #   sphinx
 rich==13.7.1
     # via
+    #   -r requirements.in
     #   cookiecutter
     #   typer
+    #   zettel-org
 setuptools-scm==8.0.4
     # via -r requirements-dev.in
 shellingham==1.5.4
     # via typer
 six==1.16.0
     # via
     #   python-dateutil
@@ -296,15 +293,15 @@
     # via pylint
 tox==3.28.0
     # via
     #   -r requirements-dev.in
     #   tox-pyenv
 tox-pyenv==1.1.0
     # via -r requirements-dev.in
-tqdm==4.66.2
+tqdm==4.66.4
     # via
     #   -r requirements.in
     #   zettel-org
 typer==0.12.3
     # via cruft
 types-python-dateutil==2.9.0.20240316
     # via arrow
```

### Comparing `zettel_org-0.7.1/requirements.txt` & `zettel_org-0.7.2/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 bolton-clack==0.3.12
     # via -r requirements.in
 bolton-eris==0.2.3
     # via
     #   -r requirements.in
     #   bolton-clack
     #   bolton-proctor
-    #   potoroo
 bolton-ion==0.1.0
     # via bolton-eris
 bolton-logrus==0.1.3
     # via
     #   -r requirements.in
     #   bolton-clack
 bolton-metaman==0.1.2
@@ -34,38 +33,44 @@
     #   bolton-clack
     #   bolton-eris
     #   vimala
 greenlet==3.0.3
     # via sqlalchemy
 jinja2==3.1.3
     # via -r requirements.in
+markdown-it-py==3.0.0
+    # via rich
 markupsafe==2.1.5
     # via jinja2
-potoroo==0.6.0
-    # via -r requirements.in
+mdurl==0.1.2
+    # via markdown-it-py
 pydantic==2.7.1
     # via
     #   bolton-clack
     #   pydantic-settings
     #   sqlmodel
 pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via bolton-clack
+pygments==2.18.0
+    # via rich
 python-dotenv==1.0.1
     # via pydantic-settings
 pyyaml==6.0.1
     # via bolton-clack
+rich==13.7.1
+    # via -r requirements.in
 sqlalchemy==2.0.29
     # via sqlmodel
 sqlmodel==0.0.18
     # via -r requirements.in
 structlog==24.1.0
     # via bolton-logrus
-tqdm==4.66.2
+tqdm==4.66.4
     # via -r requirements.in
 typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
     #   sqlalchemy
 vimala==0.2.0
```

### Comparing `zettel_org-0.7.1/setup.cfg` & `zettel_org-0.7.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 	raise AssertionError
 	raise NotImplementedError
 	
 	if 0:
 	if __name__ == .__main__.:
 	[ ]*pass[ ]*\#?.*
 	[ ]*\.\.\.[ ]*\#?.*
+	
+	if TYPE_CHECKING:
 
 [coverage:run]
 omit = .venv/*,tests/*,docs/*,setup.py,.tox/*,src/zorg/grammar/*
 
 [tool:pytest]
 doctest_optionflags = NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL ELLIPSIS NUMBER
 testpaths = src tests
```

### Comparing `zettel_org-0.7.1/setup.py` & `zettel_org-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DESCRIPTION = "The zettel note manager of the future."
 SUPPORTED_PYTHON_VERSIONS = [
     (3, 9),
     (3, 10),
     (3, 11),
     (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.7.1"}
+USE_SCM_VERSION = {"fallback_version": "0.7.2"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `zettel_org-0.7.1/src/zettel_org.egg-info/PKG-INFO` & `zettel_org-0.7.2/src/zettel_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.7.1
+Version: 0.7.2
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: antlr4-python3-runtime~=4.13
 Requires-Dist: bolton-clack~=0.3.12
 Requires-Dist: bolton-eris~=0.2.3
 Requires-Dist: bolton-logrus~=0.1.1
 Requires-Dist: bolton-typist~=0.2.0
 Requires-Dist: jinja2
-Requires-Dist: potoroo~=0.6.0
+Requires-Dist: rich~=13.7
 Requires-Dist: sqlmodel~=0.0.16
 Requires-Dist: tqdm~=4.66
 Requires-Dist: vimala~=0.2.0
 
 # zorg
 
 **The zettel note manager of the future.**
```

### Comparing `zettel_org-0.7.1/src/zettel_org.egg-info/SOURCES.txt` & `zettel_org-0.7.2/src/zettel_org.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -92,25 +92,26 @@
 src/zorg/domain/types.py
 src/zorg/domain/messages/__init__.py
 src/zorg/domain/messages/commands.py
 src/zorg/domain/messages/events.py
 src/zorg/domain/models/__init__.py
 src/zorg/domain/models/_zorg_file.py
 src/zorg/domain/models/_zorg_query.py
+src/zorg/grammar/CommonLexerRules.g4
+src/zorg/grammar/ZorgFile.g4
+src/zorg/grammar/ZorgQuery.g4
 src/zorg/grammar/__init__.py
-src/zorg/grammar/zorg_file/ZorgFile.g4
 src/zorg/grammar/zorg_file/ZorgFile.interp
 src/zorg/grammar/zorg_file/ZorgFile.tokens
 src/zorg/grammar/zorg_file/ZorgFileLexer.interp
 src/zorg/grammar/zorg_file/ZorgFileLexer.py
 src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
 src/zorg/grammar/zorg_file/ZorgFileListener.py
 src/zorg/grammar/zorg_file/ZorgFileParser.py
 src/zorg/grammar/zorg_file/__init__.py
-src/zorg/grammar/zorg_query/ZorgQuery.g4
 src/zorg/grammar/zorg_query/ZorgQuery.interp
 src/zorg/grammar/zorg_query/ZorgQuery.tokens
 src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
 src/zorg/grammar/zorg_query/ZorgQueryLexer.py
 src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
 src/zorg/grammar/zorg_query/ZorgQueryListener.py
 src/zorg/grammar/zorg_query/ZorgQueryParser.py
@@ -122,18 +123,17 @@
 src/zorg/service/messagebus.py
 src/zorg/service/templates.py
 src/zorg/service/zid_manager.py
 src/zorg/service/compiler/__init__.py
 src/zorg/service/compiler/_api.py
 src/zorg/service/compiler/_file_compiler.py
 src/zorg/service/compiler/_query_compiler.py
+src/zorg/service/swog/__init__.py
+src/zorg/service/swog/_executor.py
 src/zorg/storage/__init__.py
-src/zorg/storage/file/__init__.py
-src/zorg/storage/file/repo.py
-src/zorg/storage/file/session.py
 src/zorg/storage/sql/__init__.py
 src/zorg/storage/sql/converters.py
 src/zorg/storage/sql/engine.py
 src/zorg/storage/sql/models.py
 src/zorg/storage/sql/repo.py
 src/zorg/storage/sql/session.py
 tests/__init__.py
@@ -141,17 +141,19 @@
 tests/conftest.py
 tests/test_config.py
 tests/test_file_groups.py
 tests/test_run_action_open.py
 tests/test_run_compile.py
 tests/test_run_db.py
 tests/test_run_edit.py
+tests/test_run_query.py
 tests/test_run_template.py
 tests/__snapshots__/test_run_compile.ambr
 tests/__snapshots__/test_run_db.ambr
 tests/__snapshots__/test_run_edit.ambr
+tests/__snapshots__/test_run_query.ambr
 tests/__snapshots__/test_run_template.ambr
 tests/data/day_log.zot
 tests/data/done_log.zot
 tests/data/habit_log.zot
 tests/data/hello.zot
 tests/data/links.zo
```

### Comparing `zettel_org-0.7.1/src/zorg/app/config.py` & `zettel_org-0.7.2/src/zorg/app/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,31 +14,33 @@
 from ..service import common
 
 
 Command = Literal[
     "compile", "create", "edit", "init", "open", "query", "reindex", "render"
 ]
 
-_logger = Logger(__name__)
+_LOGGER = Logger(__name__)
 
 _DEFAULT_ZETTEL_DIR: Final[Path] = Path.home() / "org"
 
 
+def _get_default_database_url(zdir: Path) -> str:
+    return f"sqlite:///{zdir}/.{APP_NAME}/{APP_NAME}.db"
+
+
 class Config(clack.Config):
     """Shared clack configuration class."""
 
     command: Command
 
     # ----- ARGUMENTS
     zettel_dir: Path = _DEFAULT_ZETTEL_DIR
 
     # ----- CONFIG
-    database_url: str = "sqlite:///" + str(
-        _DEFAULT_ZETTEL_DIR / f".zorg/{APP_NAME}.db"
-    )
+    database_url: str = _get_default_database_url(_DEFAULT_ZETTEL_DIR)
     template_pattern_map: TemplatePatternMapType = {}
 
 
 class OpenActionConfig(Config):
     """Clack config for the 'action' command."""
 
     command: Literal["open"]
@@ -117,22 +119,22 @@
 
 
 def clack_parser(argv: Sequence[str]) -> dict[str, Any]:
     """Parser we pass to the `main_factory()` `parser` kwarg."""
     # HACK: Make 'edit' the default sub-command.
     argv_after_opts = list(it.dropwhile(lambda x: x.startswith("-"), argv[1:]))
     if not argv_after_opts:
-        _logger.debug(
+        _LOGGER.debug(
             "Inferring 'edit' command since no subcommand was specified."
         )
         argv = list(argv) + ["edit"]
     elif argv_after_opts[0].startswith("@"):
         argv_opts = list(it.takewhile(lambda x: x.startswith("-"), argv[1:]))
         argv = [argv[0]] + argv_opts + ["edit"] + argv_after_opts
-        _logger.debug(
+        _LOGGER.debug(
             "Inferring 'edit' command since we found a file group name.",
             file_group_name=argv_after_opts[0],
             new_args=argv[1:],
         )
 
     parser = clack.Parser(description="The zettel note manager of the future.")
     # --- Global Options
@@ -270,21 +272,36 @@
     )
 
     args = parser.parse_args(argv[1:])
     kwargs = clack.filter_cli_args(args)
 
     _convert_variables_to_var_map(kwargs)
     _process_zo_paths(kwargs)
+    _process_query(kwargs)
+    _fix_database_url(kwargs)
 
     return kwargs
 
 
+def _fix_database_url(kwargs: dict[str, Any]) -> None:
+    if "database_url" not in kwargs and (zdir := kwargs.get("zettel_dir")):
+        kwargs["database_url"] = _get_default_database_url(zdir)
+
+
+def _process_query(kwargs: dict[str, Any]) -> None:
+    if kwargs["command"] == "query" and not kwargs["query"].startswith(
+        ("S ", "W ")
+    ):
+        query = kwargs["query"]
+        kwargs["query"] = f"W {query}"
+
+
 def _process_zo_paths(kwargs: dict[str, Any]) -> None:
     if kwargs["command"] == "edit" and "zo_paths" not in kwargs:
-        _logger.debug(
+        _LOGGER.debug(
             "The 'edit' command was invoked, but no file paths were specified."
             " Auto-adding the @default file group paths.",
             kwargs=kwargs,
         )
         kwargs["zo_paths"] = [Path("@default")]
```

### Comparing `zettel_org-0.7.1/src/zorg/app/runners/__init__.py` & `zettel_org-0.7.2/src/zorg/app/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/src/zorg/app/runners/_run_action.py` & `zettel_org-0.7.2/src/zorg/app/runners/_run_action.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/src/zorg/app/runners/_run_compile.py` & `zettel_org-0.7.2/src/zorg/app/runners/_run_compile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Contains runners for the 'zorg compile' command."""
 
 from dataclasses import asdict
 from pprint import pprint
 from typing import Any
 
-from ...domain.models import ZorgFile
+from ...domain.models import File
 from ...service.compiler import walk_zorg_file
 from ..config import CompileConfig
 from ._runners import runner
 
 
 @runner
 def run_compile(cfg: CompileConfig) -> int:
     """Runner for the 'compile' command."""
     zorg_file = walk_zorg_file(cfg.zettel_dir, cfg.zo_path, verbose=True)
     zorg_file_dict = _convert_zorg_file_to_dict(zorg_file)
     pprint(zorg_file_dict)
     return 0
 
 
-def _convert_zorg_file_to_dict(zorg_file: ZorgFile) -> dict[str, Any]:
+def _convert_zorg_file_to_dict(zorg_file: File) -> dict[str, Any]:
     zorg_file_dict = asdict(zorg_file)
     for key in ["events", "has_errors", "path"]:
         del zorg_file_dict[key]
 
     for note_dict in zorg_file_dict["notes"]:
-        del note_dict["line_no"]
+        for key in ["file_path", "line_no"]:
+            del note_dict[key]
     return zorg_file_dict
```

### Comparing `zettel_org-0.7.1/src/zorg/app/runners/_run_db.py` & `zettel_org-0.7.2/src/zorg/app/runners/_run_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """Contains runners for the 'zorg db' command."""
 
-from logrus import Logger
-
 from ...domain.messages import commands
 from ...service import messagebus
 from ...storage.sql.session import SQLSession
 from ..config import DbCreateConfig, DbReindexConfig
 from ._runners import runner
 
 
-logger = Logger(__name__)
-
-
 @runner
 def run_db_create(cfg: DbCreateConfig) -> int:
     """Runner for the 'db create' command."""
     session = SQLSession(
         cfg.zettel_dir, cfg.database_url, should_delete_existing_db=True
     )
     messagebus.handle([commands.CreateDBCommand(cfg.zettel_dir)], session)
```

### Comparing `zettel_org-0.7.1/src/zorg/app/runners/_run_edit.py` & `zettel_org-0.7.2/src/zorg/app/runners/_run_edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """Contains runners for the 'zorg edit' command."""
 
-from logrus import Logger
-
 from ...domain.messages import commands
 from ...service import messagebus
 from ...service.common import prepend_zdir
 from ...service.file_groups import expand_file_group_paths
 from ...service.templates import init_from_template
 from ...storage.sql.session import SQLSession
 from ..config import EditConfig
 from ._runners import runner
 
 
-logger = Logger(__name__)
-
-
 @runner
 def run_edit(cfg: EditConfig) -> int:
     """Runner for the 'edit' command."""
     zo_paths = expand_file_group_paths(
         cfg.zo_paths, file_group_map=cfg.file_group_map
     )
     zo_paths = prepend_zdir(cfg.zettel_dir, zo_paths)
```

### Comparing `zettel_org-0.7.1/src/zorg/app/runners/_run_template.py` & `zettel_org-0.7.2/src/zorg/app/runners/_run_template.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/src/zorg/domain/messages/commands.py` & `zettel_org-0.7.2/src/zorg/domain/messages/commands.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/src/zorg/domain/messages/events.py` & `zettel_org-0.7.2/src/zorg/domain/messages/events.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Zorg events."""
 
 from dataclasses import dataclass
 from pathlib import Path
 
 from . import commands
-from ..models import ZorgNote
+from ..models import Note
 
 
 @dataclass(frozen=True)
 class Event:
     """A zorg event."""
 
 
@@ -20,16 +20,17 @@
     edit_cmd: commands.EditCommand
 
 
 @dataclass(frozen=True)
 class NewZorgNotesEvent(Event):
     """Broadcast when new zorg notes are indexed."""
 
+    zettel_dir: Path
     zorg_file_path: Path
-    new_notes: list[ZorgNote]
+    new_notes: list[Note]
 
 
 @dataclass(frozen=True)
 class DBModifiedEvent(Event):
     """Broadcast when the zorg database is done being initialized."""
 
     zettel_dir: Path
```

### Comparing `zettel_org-0.7.1/src/zorg/domain/models/_zorg_file.py` & `zettel_org-0.7.2/src/zorg/domain/models/_zorg_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 """This file contains Zorg's domain model classes."""
 
 from dataclasses import dataclass, field
 import datetime as dt
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional
 
-from ..types import NoteStatus, TodoPriorityType
+from ..types import NoteType, TodoPriorityType
 
 
 if TYPE_CHECKING:
     from ..messages.events import Event
 
 
 @dataclass(frozen=True)
 class TodoPayload:
     """Extra fields that are added to ZorgNotes that are todos."""
 
     priority: TodoPriorityType = "C"
-    status: NoteStatus = NoteStatus.OPEN_TODO
+    status: NoteType = NoteType.OPEN_TODO
 
 
 @dataclass
-class ZorgNote:
+class Note:
     """A Zorg note."""
 
     body: str
 
     areas: list[str] = field(default_factory=lambda: [])
     child_note_ids: list[int] = field(default_factory=lambda: [])
     contexts: list[str] = field(default_factory=lambda: [])
     create_date: dt.date = field(default_factory=dt.date.today)
+    file_path: Optional[Path] = None
     line_no: Optional[int] = None
     links: list[str] = field(default_factory=lambda: [])
     next_note_id: Optional[int] = None
     parent_note_id: Optional[int] = None
     people: list[str] = field(default_factory=lambda: [])
     prev_note_id: Optional[int] = None
     projects: list[str] = field(default_factory=lambda: [])
     properties: dict[str, str] = field(default_factory=lambda: {})
     todo_payload: Optional[TodoPayload] = None
     zid: Optional[str] = None
 
 
 @dataclass
-class ZorgFile:
+class File:
     """A Zorg (i.e. *.zo) file."""
 
     path: Path
     has_errors: bool = False
-    notes: list[ZorgNote] = field(default_factory=list)
+    notes: list[Note] = field(default_factory=list)
     events: list["Event"] = field(default_factory=list)
```

### Comparing `zettel_org-0.7.1/src/zorg/domain/models/_zorg_query.py` & `zettel_org-0.7.2/src/zorg/domain/models/_zorg_query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-"""Contains the ZorgQuery Domain entity."""
+"""Contains the Query domain entity."""
 
 from dataclasses import dataclass, field
 import datetime as dt
 from typing import Iterable, Optional
 
 from ..types import (
     DescOperator,
-    NoteStatus,
+    GroupByType,
+    NoteType,
+    OrderByType,
     PropertyOperator,
     PropertyValueType,
-    Select,
+    SelectType,
     TodoPriorityType,
 )
 
 
 @dataclass(frozen=True)
 class DescFilter:
     """Represents a description query filter (e.g. '"foo"' or '!"bar"')."""
@@ -41,25 +43,25 @@
     end: Optional[dt.date] = None
 
 
 @dataclass
 class WhereAndFilter:
     """Tag used to filter ZorgNotes."""
 
-    allowed_note_statuses: set[NoteStatus] = field(default_factory=set)
-    areas: list[str] = field(default_factory=list)
-    contexts: list[str] = field(default_factory=list)
-    create_date_ranges: list[DateRange] = field(default_factory=list)
-    desc_filters: list[DescFilter] = field(default_factory=list)
-    modify_date_ranges: list[DateRange] = field(default_factory=list)
+    allowed_note_types: set[NoteType] = field(default_factory=set)
+    areas: set[str] = field(default_factory=set)
+    contexts: set[str] = field(default_factory=set)
+    create_date_ranges: set[DateRange] = field(default_factory=set)
+    desc_filters: set[DescFilter] = field(default_factory=set)
+    modify_date_ranges: set[DateRange] = field(default_factory=set)
     or_filters: list["WhereOrFilter"] = field(default_factory=list)
-    people: list[str] = field(default_factory=list)
-    property_filters: list[PropertyFilter] = field(default_factory=list)
-    priorities: list[TodoPriorityType] = field(default_factory=list)
-    projects: list[str] = field(default_factory=list)
+    people: set[str] = field(default_factory=set)
+    property_filters: set[PropertyFilter] = field(default_factory=set)
+    priorities: set[TodoPriorityType] = field(default_factory=set)
+    projects: set[str] = field(default_factory=set)
 
     def __repr__(self) -> str:
         """String representation that only shows fields if they are set."""
         dict_repr = ", ".join(
             f"{k}={v!r}"
             for k, v in filter(
                 lambda item: bool(item[1]), self.__dict__.items()
@@ -73,18 +75,24 @@
 class WhereOrFilter:
     """A collection of `WhereAndFilter`s that have been ORed together."""
 
     and_filters: Iterable[WhereAndFilter]
 
 
 @dataclass
-class ZorgQuery:
+class Query:
     """A zorg query that uses SWOG syntax.
 
     (S)ELECT
     (W)HERE
     (O)RDER BY
     (G)ROUP BY
     """
 
-    select: Select = field(default=Select.NOTES)
+    select: SelectType = field(default=SelectType.NOTE)
     where: Optional[WhereOrFilter] = None
+    order_by: tuple[OrderByType, ...] = (
+        OrderByType.NOTE_TYPE,
+        OrderByType.PRIORITY,
+        OrderByType.DATE,
+    )
+    group_by: tuple[GroupByType, ...] = tuple()
```

### Comparing `zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFile.interp` & `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFile.interp`

 * *Files 14% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 null
 null
 null
 null
 NL
 LOWER_O
 LOWER_X
-ID
 DATE
 TIME
+ID
 ZID
 NUM_ID
 TWO_SPACE_DASH
 FOUR_SPACE_DASH
 SYMBOL
 DASH
 DOT
@@ -74,14 +74,15 @@
 LANGLE
 RANGLE
 
 rule names:
 prog
 head
 comment
+body
 block
 item
 footnote
 note
 base_note
 id_note_body
 note_body
@@ -121,8 +122,8 @@
 h2_header
 h3_header
 h4_header
 eol
 
 
 atn:
-[4, 1, 35, 470, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 1, 0, 1, 0, 4, 0, 97, 8, 0, 11, 0, 12, 0, 98, 1, 0, 5, 0, 102, 8, 0, 10, 0, 12, 0, 105, 9, 0, 1, 0, 5, 0, 108, 8, 0, 10, 0, 12, 0, 111, 9, 0, 1, 0, 5, 0, 114, 8, 0, 10, 0, 12, 0, 117, 9, 0, 3, 0, 119, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 124, 8, 1, 11, 1, 12, 1, 125, 1, 2, 1, 2, 3, 2, 130, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 135, 8, 3, 11, 3, 12, 3, 136, 1, 3, 5, 3, 140, 8, 3, 10, 3, 12, 3, 143, 9, 3, 1, 4, 1, 4, 1, 4, 1, 4, 3, 4, 149, 8, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 1, 6, 1, 6, 5, 6, 159, 8, 6, 10, 6, 12, 6, 162, 9, 6, 1, 7, 1, 7, 1, 7, 1, 8, 1, 8, 3, 8, 169, 8, 8, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 4, 9, 176, 8, 9, 11, 9, 12, 9, 177, 1, 9, 5, 9, 181, 8, 9, 10, 9, 12, 9, 184, 9, 9, 1, 10, 1, 10, 1, 10, 5, 10, 189, 8, 10, 10, 10, 12, 10, 192, 9, 10, 1, 11, 1, 11, 1, 11, 1, 12, 1, 12, 5, 12, 199, 8, 12, 10, 12, 12, 12, 202, 9, 12, 1, 13, 1, 13, 1, 13, 3, 13, 207, 8, 13, 1, 13, 1, 13, 1, 13, 1, 14, 1, 14, 1, 14, 1, 14, 3, 14, 216, 8, 14, 1, 15, 1, 15, 1, 15, 3, 15, 221, 8, 15, 1, 16, 1, 16, 1, 16, 1, 16, 1, 16, 1, 17, 1, 17, 1, 18, 4, 18, 231, 8, 18, 11, 18, 12, 18, 232, 1, 19, 1, 19, 1, 19, 3, 19, 238, 8, 19, 1, 19, 1, 19, 5, 19, 242, 8, 19, 10, 19, 12, 19, 245, 9, 19, 1, 19, 1, 19, 3, 19, 249, 8, 19, 1, 19, 1, 19, 1, 19, 5, 19, 254, 8, 19, 10, 19, 12, 19, 257, 9, 19, 3, 19, 259, 8, 19, 1, 19, 3, 19, 262, 8, 19, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 3, 20, 272, 8, 20, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 22, 1, 22, 4, 22, 281, 8, 22, 11, 22, 12, 22, 282, 1, 22, 1, 22, 5, 22, 287, 8, 22, 10, 22, 12, 22, 290, 9, 22, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 3, 23, 298, 8, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 26, 1, 26, 1, 26, 3, 26, 309, 8, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 30, 1, 30, 3, 30, 321, 8, 30, 1, 31, 1, 31, 1, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 1, 35, 1, 35, 4, 35, 340, 8, 35, 11, 35, 12, 35, 341, 1, 35, 1, 35, 1, 35, 4, 35, 347, 8, 35, 11, 35, 12, 35, 348, 1, 35, 1, 35, 3, 35, 353, 8, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 5, 38, 365, 8, 38, 10, 38, 12, 38, 368, 9, 38, 1, 38, 5, 38, 371, 8, 38, 10, 38, 12, 38, 374, 9, 38, 1, 38, 3, 38, 377, 8, 38, 1, 38, 5, 38, 380, 8, 38, 10, 38, 12, 38, 383, 9, 38, 1, 39, 1, 39, 5, 39, 387, 8, 39, 10, 39, 12, 39, 390, 9, 39, 1, 39, 5, 39, 393, 8, 39, 10, 39, 12, 39, 396, 9, 39, 1, 39, 3, 39, 399, 8, 39, 1, 39, 5, 39, 402, 8, 39, 10, 39, 12, 39, 405, 9, 39, 1, 40, 1, 40, 5, 40, 409, 8, 40, 10, 40, 12, 40, 412, 9, 40, 1, 40, 5, 40, 415, 8, 40, 10, 40, 12, 40, 418, 9, 40, 1, 40, 3, 40, 421, 8, 40, 1, 40, 5, 40, 424, 8, 40, 10, 40, 12, 40, 427, 9, 40, 1, 41, 1, 41, 5, 41, 431, 8, 41, 10, 41, 12, 41, 434, 9, 41, 1, 41, 5, 41, 437, 8, 41, 10, 41, 12, 41, 440, 9, 41, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 43, 1, 43, 1, 43, 1, 43, 1, 44, 1, 44, 1, 44, 1, 44, 1, 45, 1, 45, 1, 45, 1, 45, 1, 45, 1, 45, 1, 46, 1, 46, 1, 46, 0, 0, 47, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 0, 5, 2, 0, 9, 9, 32, 32, 4, 0, 17, 17, 21, 21, 24, 25, 32, 35, 2, 0, 18, 20, 22, 22, 1, 0, 26, 29, 1, 1, 7, 7, 496, 0, 94, 1, 0, 0, 0, 2, 123, 1, 0, 0, 0, 4, 127, 1, 0, 0, 0, 6, 134, 1, 0, 0, 0, 8, 148, 1, 0, 0, 0, 10, 150, 1, 0, 0, 0, 12, 155, 1, 0, 0, 0, 14, 163, 1, 0, 0, 0, 16, 168, 1, 0, 0, 0, 18, 172, 1, 0, 0, 0, 20, 185, 1, 0, 0, 0, 22, 193, 1, 0, 0, 0, 24, 196, 1, 0, 0, 0, 26, 203, 1, 0, 0, 0, 28, 215, 1, 0, 0, 0, 30, 217, 1, 0, 0, 0, 32, 222, 1, 0, 0, 0, 34, 227, 1, 0, 0, 0, 36, 230, 1, 0, 0, 0, 38, 234, 1, 0, 0, 0, 40, 271, 1, 0, 0, 0, 42, 273, 1, 0, 0, 0, 44, 278, 1, 0, 0, 0, 46, 297, 1, 0, 0, 0, 48, 299, 1, 0, 0, 0, 50, 301, 1, 0, 0, 0, 52, 308, 1, 0, 0, 0, 54, 310, 1, 0, 0, 0, 56, 312, 1, 0, 0, 0, 58, 314, 1, 0, 0, 0, 60, 320, 1, 0, 0, 0, 62, 322, 1, 0, 0, 0, 64, 325, 1, 0, 0, 0, 66, 328, 1, 0, 0, 0, 68, 331, 1, 0, 0, 0, 70, 352, 1, 0, 0, 0, 72, 354, 1, 0, 0, 0, 74, 358, 1, 0, 0, 0, 76, 362, 1, 0, 0, 0, 78, 384, 1, 0, 0, 0, 80, 406, 1, 0, 0, 0, 82, 428, 1, 0, 0, 0, 84, 441, 1, 0, 0, 0, 86, 453, 1, 0, 0, 0, 88, 457, 1, 0, 0, 0, 90, 461, 1, 0, 0, 0, 92, 467, 1, 0, 0, 0, 94, 118, 3, 2, 1, 0, 95, 97, 5, 7, 0, 0, 96, 95, 1, 0, 0, 0, 97, 98, 1, 0, 0, 0, 98, 96, 1, 0, 0, 0, 98, 99, 1, 0, 0, 0, 99, 103, 1, 0, 0, 0, 100, 102, 3, 6, 3, 0, 101, 100, 1, 0, 0, 0, 102, 105, 1, 0, 0, 0, 103, 101, 1, 0, 0, 0, 103, 104, 1, 0, 0, 0, 104, 109, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 106, 108, 3, 78, 39, 0, 107, 106, 1, 0, 0, 0, 108, 111, 1, 0, 0, 0, 109, 107, 1, 0, 0, 0, 109, 110, 1, 0, 0, 0, 110, 115, 1, 0, 0, 0, 111, 109, 1, 0, 0, 0, 112, 114, 3, 76, 38, 0, 113, 112, 1, 0, 0, 0, 114, 117, 1, 0, 0, 0, 115, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 119, 1, 0, 0, 0, 117, 115, 1, 0, 0, 0, 118, 96, 1, 0, 0, 0, 118, 119, 1, 0, 0, 0, 119, 120, 1, 0, 0, 0, 120, 121, 5, 0, 0, 1, 121, 1, 1, 0, 0, 0, 122, 124, 3, 4, 2, 0, 123, 122, 1, 0, 0, 0, 124, 125, 1, 0, 0, 0, 125, 123, 1, 0, 0, 0, 125, 126, 1, 0, 0, 0, 126, 3, 1, 0, 0, 0, 127, 129, 5, 26, 0, 0, 128, 130, 3, 36, 18, 0, 129, 128, 1, 0, 0, 0, 129, 130, 1, 0, 0, 0, 130, 131, 1, 0, 0, 0, 131, 132, 5, 7, 0, 0, 132, 5, 1, 0, 0, 0, 133, 135, 3, 8, 4, 0, 134, 133, 1, 0, 0, 0, 135, 136, 1, 0, 0, 0, 136, 134, 1, 0, 0, 0, 136, 137, 1, 0, 0, 0, 137, 141, 1, 0, 0, 0, 138, 140, 5, 7, 0, 0, 139, 138, 1, 0, 0, 0, 140, 143, 1, 0, 0, 0, 141, 139, 1, 0, 0, 0, 141, 142, 1, 0, 0, 0, 142, 7, 1, 0, 0, 0, 143, 141, 1, 0, 0, 0, 144, 149, 3, 24, 12, 0, 145, 149, 3, 12, 6, 0, 146, 149, 3, 10, 5, 0, 147, 149, 3, 4, 2, 0, 148, 144, 1, 0, 0, 0, 148, 145, 1, 0, 0, 0, 148, 146, 1, 0, 0, 0, 148, 147, 1, 0, 0, 0, 149, 9, 1, 0, 0, 0, 150, 151, 3, 74, 37, 0, 151, 152, 5, 22, 0, 0, 152, 153, 3, 36, 18, 0, 153, 154, 5, 7, 0, 0, 154, 11, 1, 0, 0, 0, 155, 156, 5, 18, 0, 0, 156, 160, 3, 14, 7, 0, 157, 159, 3, 20, 10, 0, 158, 157, 1, 0, 0, 0, 159, 162, 1, 0, 0, 0, 160, 158, 1, 0, 0, 0, 160, 161, 1, 0, 0, 0, 161, 13, 1, 0, 0, 0, 162, 160, 1, 0, 0, 0, 163, 164, 3, 16, 8, 0, 164, 165, 5, 7, 0, 0, 165, 15, 1, 0, 0, 0, 166, 167, 5, 23, 0, 0, 167, 169, 3, 34, 17, 0, 168, 166, 1, 0, 0, 0, 168, 169, 1, 0, 0, 0, 169, 170, 1, 0, 0, 0, 170, 171, 3, 18, 9, 0, 171, 17, 1, 0, 0, 0, 172, 182, 3, 36, 18, 0, 173, 175, 5, 7, 0, 0, 174, 176, 5, 23, 0, 0, 175, 174, 1, 0, 0, 0, 176, 177, 1, 0, 0, 0, 177, 175, 1, 0, 0, 0, 177, 178, 1, 0, 0, 0, 178, 179, 1, 0, 0, 0, 179, 181, 3, 36, 18, 0, 180, 173, 1, 0, 0, 0, 181, 184, 1, 0, 0, 0, 182, 180, 1, 0, 0, 0, 182, 183, 1, 0, 0, 0, 183, 19, 1, 0, 0, 0, 184, 182, 1, 0, 0, 0, 185, 186, 5, 15, 0, 0, 186, 190, 3, 14, 7, 0, 187, 189, 3, 22, 11, 0, 188, 187, 1, 0, 0, 0, 189, 192, 1, 0, 0, 0, 190, 188, 1, 0, 0, 0, 190, 191, 1, 0, 0, 0, 191, 21, 1, 0, 0, 0, 192, 190, 1, 0, 0, 0, 193, 194, 5, 16, 0, 0, 194, 195, 3, 14, 7, 0, 195, 23, 1, 0, 0, 0, 196, 200, 3, 26, 13, 0, 197, 199, 3, 20, 10, 0, 198, 197, 1, 0, 0, 0, 199, 202, 1, 0, 0, 0, 200, 198, 1, 0, 0, 0, 200, 201, 1, 0, 0, 0, 201, 25, 1, 0, 0, 0, 202, 200, 1, 0, 0, 0, 203, 206, 3, 28, 14, 0, 204, 205, 5, 23, 0, 0, 205, 207, 3, 32, 16, 0, 206, 204, 1, 0, 0, 0, 206, 207, 1, 0, 0, 0, 207, 208, 1, 0, 0, 0, 208, 209, 3, 16, 8, 0, 209, 210, 5, 7, 0, 0, 210, 27, 1, 0, 0, 0, 211, 216, 5, 8, 0, 0, 212, 216, 3, 30, 15, 0, 213, 216, 5, 34, 0, 0, 214, 216, 5, 35, 0, 0, 215, 211, 1, 0, 0, 0, 215, 212, 1, 0, 0, 0, 215, 213, 1, 0, 0, 0, 215, 214, 1, 0, 0, 0, 216, 29, 1, 0, 0, 0, 217, 220, 7, 0, 0, 0, 218, 219, 5, 22, 0, 0, 219, 221, 3, 50, 25, 0, 220, 218, 1, 0, 0, 0, 220, 221, 1, 0, 0, 0, 221, 31, 1, 0, 0, 0, 222, 223, 5, 1, 0, 0, 223, 224, 5, 26, 0, 0, 224, 225, 5, 10, 0, 0, 225, 226, 5, 2, 0, 0, 226, 33, 1, 0, 0, 0, 227, 228, 5, 13, 0, 0, 228, 35, 1, 0, 0, 0, 229, 231, 3, 38, 19, 0, 230, 229, 1, 0, 0, 0, 231, 232, 1, 0, 0, 0, 232, 230, 1, 0, 0, 0, 232, 233, 1, 0, 0, 0, 233, 37, 1, 0, 0, 0, 234, 237, 5, 23, 0, 0, 235, 236, 5, 30, 0, 0, 236, 238, 3, 54, 27, 0, 237, 235, 1, 0, 0, 0, 237, 238, 1, 0, 0, 0, 238, 243, 1, 0, 0, 0, 239, 242, 3, 54, 27, 0, 240, 242, 5, 31, 0, 0, 241, 239, 1, 0, 0, 0, 241, 240, 1, 0, 0, 0, 242, 245, 1, 0, 0, 0, 243, 241, 1, 0, 0, 0, 243, 244, 1, 0, 0, 0, 244, 248, 1, 0, 0, 0, 245, 243, 1, 0, 0, 0, 246, 249, 3, 40, 20, 0, 247, 249, 3, 70, 35, 0, 248, 246, 1, 0, 0, 0, 248, 247, 1, 0, 0, 0, 248, 249, 1, 0, 0, 0, 249, 258, 1, 0, 0, 0, 250, 255, 3, 52, 26, 0, 251, 254, 3, 52, 26, 0, 252, 254, 3, 46, 23, 0, 253, 251, 1, 0, 0, 0, 253, 252, 1, 0, 0, 0, 254, 257, 1, 0, 0, 0, 255, 253, 1, 0, 0, 0, 255, 256, 1, 0, 0, 0, 256, 259, 1, 0, 0, 0, 257, 255, 1, 0, 0, 0, 258, 250, 1, 0, 0, 0, 258, 259, 1, 0, 0, 0, 259, 261, 1, 0, 0, 0, 260, 262, 3, 74, 37, 0, 261, 260, 1, 0, 0, 0, 261, 262, 1, 0, 0, 0, 262, 39, 1, 0, 0, 0, 263, 272, 3, 58, 29, 0, 264, 272, 3, 60, 30, 0, 265, 272, 3, 72, 36, 0, 266, 272, 3, 42, 21, 0, 267, 272, 3, 44, 22, 0, 268, 272, 3, 74, 37, 0, 269, 272, 3, 34, 17, 0, 270, 272, 3, 32, 16, 0, 271, 263, 1, 0, 0, 0, 271, 264, 1, 0, 0, 0, 271, 265, 1, 0, 0, 0, 271, 266, 1, 0, 0, 0, 271, 267, 1, 0, 0, 0, 271, 268, 1, 0, 0, 0, 271, 269, 1, 0, 0, 0, 271, 270, 1, 0, 0, 0, 272, 41, 1, 0, 0, 0, 273, 274, 5, 10, 0, 0, 274, 275, 5, 22, 0, 0, 275, 276, 5, 22, 0, 0, 276, 277, 3, 44, 22, 0, 277, 43, 1, 0, 0, 0, 278, 288, 3, 46, 23, 0, 279, 281, 3, 56, 28, 0, 280, 279, 1, 0, 0, 0, 281, 282, 1, 0, 0, 0, 282, 280, 1, 0, 0, 0, 282, 283, 1, 0, 0, 0, 283, 284, 1, 0, 0, 0, 284, 285, 3, 46, 23, 0, 285, 287, 1, 0, 0, 0, 286, 280, 1, 0, 0, 0, 287, 290, 1, 0, 0, 0, 288, 286, 1, 0, 0, 0, 288, 289, 1, 0, 0, 0, 289, 45, 1, 0, 0, 0, 290, 288, 1, 0, 0, 0, 291, 298, 5, 10, 0, 0, 292, 298, 5, 14, 0, 0, 293, 298, 3, 48, 24, 0, 294, 298, 3, 50, 25, 0, 295, 298, 5, 8, 0, 0, 296, 298, 5, 9, 0, 0, 297, 291, 1, 0, 0, 0, 297, 292, 1, 0, 0, 0, 297, 293, 1, 0, 0, 0, 297, 294, 1, 0, 0, 0, 297, 295, 1, 0, 0, 0, 297, 296, 1, 0, 0, 0, 298, 47, 1, 0, 0, 0, 299, 300, 5, 11, 0, 0, 300, 49, 1, 0, 0, 0, 301, 302, 5, 12, 0, 0, 302, 51, 1, 0, 0, 0, 303, 309, 5, 30, 0, 0, 304, 309, 5, 31, 0, 0, 305, 309, 3, 54, 27, 0, 306, 309, 3, 58, 29, 0, 307, 309, 3, 56, 28, 0, 308, 303, 1, 0, 0, 0, 308, 304, 1, 0, 0, 0, 308, 305, 1, 0, 0, 0, 308, 306, 1, 0, 0, 0, 308, 307, 1, 0, 0, 0, 309, 53, 1, 0, 0, 0, 310, 311, 7, 1, 0, 0, 311, 55, 1, 0, 0, 0, 312, 313, 7, 2, 0, 0, 313, 57, 1, 0, 0, 0, 314, 315, 7, 3, 0, 0, 315, 59, 1, 0, 0, 0, 316, 321, 3, 62, 31, 0, 317, 321, 3, 64, 32, 0, 318, 321, 3, 66, 33, 0, 319, 321, 3, 68, 34, 0, 320, 316, 1, 0, 0, 0, 320, 317, 1, 0, 0, 0, 320, 318, 1, 0, 0, 0, 320, 319, 1, 0, 0, 0, 321, 61, 1, 0, 0, 0, 322, 323, 5, 26, 0, 0, 323, 324, 5, 10, 0, 0, 324, 63, 1, 0, 0, 0, 325, 326, 5, 27, 0, 0, 326, 327, 5, 10, 0, 0, 327, 65, 1, 0, 0, 0, 328, 329, 5, 29, 0, 0, 329, 330, 5, 10, 0, 0, 330, 67, 1, 0, 0, 0, 331, 332, 5, 28, 0, 0, 332, 333, 5, 10, 0, 0, 333, 69, 1, 0, 0, 0, 334, 339, 5, 30, 0, 0, 335, 340, 3, 40, 20, 0, 336, 340, 3, 32, 16, 0, 337, 340, 5, 3, 0, 0, 338, 340, 5, 4, 0, 0, 339, 335, 1, 0, 0, 0, 339, 336, 1, 0, 0, 0, 339, 337, 1, 0, 0, 0, 339, 338, 1, 0, 0, 0, 340, 341, 1, 0, 0, 0, 341, 339, 1, 0, 0, 0, 341, 342, 1, 0, 0, 0, 342, 343, 1, 0, 0, 0, 343, 353, 5, 30, 0, 0, 344, 346, 5, 31, 0, 0, 345, 347, 3, 40, 20, 0, 346, 345, 1, 0, 0, 0, 347, 348, 1, 0, 0, 0, 348, 346, 1, 0, 0, 0, 348, 349, 1, 0, 0, 0, 349, 350, 1, 0, 0, 0, 350, 351, 5, 31, 0, 0, 351, 353, 1, 0, 0, 0, 352, 334, 1, 0, 0, 0, 352, 344, 1, 0, 0, 0, 353, 71, 1, 0, 0, 0, 354, 355, 5, 3, 0, 0, 355, 356, 3, 44, 22, 0, 356, 357, 5, 4, 0, 0, 357, 73, 1, 0, 0, 0, 358, 359, 5, 1, 0, 0, 359, 360, 3, 44, 22, 0, 360, 361, 5, 2, 0, 0, 361, 75, 1, 0, 0, 0, 362, 366, 3, 84, 42, 0, 363, 365, 5, 7, 0, 0, 364, 363, 1, 0, 0, 0, 365, 368, 1, 0, 0, 0, 366, 364, 1, 0, 0, 0, 366, 367, 1, 0, 0, 0, 367, 372, 1, 0, 0, 0, 368, 366, 1, 0, 0, 0, 369, 371, 3, 6, 3, 0, 370, 369, 1, 0, 0, 0, 371, 374, 1, 0, 0, 0, 372, 370, 1, 0, 0, 0, 372, 373, 1, 0, 0, 0, 373, 381, 1, 0, 0, 0, 374, 372, 1, 0, 0, 0, 375, 377, 5, 7, 0, 0, 376, 375, 1, 0, 0, 0, 376, 377, 1, 0, 0, 0, 377, 378, 1, 0, 0, 0, 378, 380, 3, 78, 39, 0, 379, 376, 1, 0, 0, 0, 380, 383, 1, 0, 0, 0, 381, 379, 1, 0, 0, 0, 381, 382, 1, 0, 0, 0, 382, 77, 1, 0, 0, 0, 383, 381, 1, 0, 0, 0, 384, 388, 3, 86, 43, 0, 385, 387, 5, 7, 0, 0, 386, 385, 1, 0, 0, 0, 387, 390, 1, 0, 0, 0, 388, 386, 1, 0, 0, 0, 388, 389, 1, 0, 0, 0, 389, 394, 1, 0, 0, 0, 390, 388, 1, 0, 0, 0, 391, 393, 3, 6, 3, 0, 392, 391, 1, 0, 0, 0, 393, 396, 1, 0, 0, 0, 394, 392, 1, 0, 0, 0, 394, 395, 1, 0, 0, 0, 395, 403, 1, 0, 0, 0, 396, 394, 1, 0, 0, 0, 397, 399, 5, 7, 0, 0, 398, 397, 1, 0, 0, 0, 398, 399, 1, 0, 0, 0, 399, 400, 1, 0, 0, 0, 400, 402, 3, 80, 40, 0, 401, 398, 1, 0, 0, 0, 402, 405, 1, 0, 0, 0, 403, 401, 1, 0, 0, 0, 403, 404, 1, 0, 0, 0, 404, 79, 1, 0, 0, 0, 405, 403, 1, 0, 0, 0, 406, 410, 3, 88, 44, 0, 407, 409, 5, 7, 0, 0, 408, 407, 1, 0, 0, 0, 409, 412, 1, 0, 0, 0, 410, 408, 1, 0, 0, 0, 410, 411, 1, 0, 0, 0, 411, 416, 1, 0, 0, 0, 412, 410, 1, 0, 0, 0, 413, 415, 3, 6, 3, 0, 414, 413, 1, 0, 0, 0, 415, 418, 1, 0, 0, 0, 416, 414, 1, 0, 0, 0, 416, 417, 1, 0, 0, 0, 417, 425, 1, 0, 0, 0, 418, 416, 1, 0, 0, 0, 419, 421, 5, 7, 0, 0, 420, 419, 1, 0, 0, 0, 420, 421, 1, 0, 0, 0, 421, 422, 1, 0, 0, 0, 422, 424, 3, 82, 41, 0, 423, 420, 1, 0, 0, 0, 424, 427, 1, 0, 0, 0, 425, 423, 1, 0, 0, 0, 425, 426, 1, 0, 0, 0, 426, 81, 1, 0, 0, 0, 427, 425, 1, 0, 0, 0, 428, 432, 3, 90, 45, 0, 429, 431, 5, 7, 0, 0, 430, 429, 1, 0, 0, 0, 431, 434, 1, 0, 0, 0, 432, 430, 1, 0, 0, 0, 432, 433, 1, 0, 0, 0, 433, 438, 1, 0, 0, 0, 434, 432, 1, 0, 0, 0, 435, 437, 3, 6, 3, 0, 436, 435, 1, 0, 0, 0, 437, 440, 1, 0, 0, 0, 438, 436, 1, 0, 0, 0, 438, 439, 1, 0, 0, 0, 439, 83, 1, 0, 0, 0, 440, 438, 1, 0, 0, 0, 441, 442, 5, 26, 0, 0, 442, 443, 5, 26, 0, 0, 443, 444, 5, 26, 0, 0, 444, 445, 5, 26, 0, 0, 445, 446, 5, 26, 0, 0, 446, 447, 5, 26, 0, 0, 447, 448, 5, 26, 0, 0, 448, 449, 5, 26, 0, 0, 449, 450, 5, 26, 0, 0, 450, 451, 3, 36, 18, 0, 451, 452, 3, 92, 46, 0, 452, 85, 1, 0, 0, 0, 453, 454, 5, 5, 0, 0, 454, 455, 3, 36, 18, 0, 455, 456, 3, 92, 46, 0, 456, 87, 1, 0, 0, 0, 457, 458, 5, 6, 0, 0, 458, 459, 3, 36, 18, 0, 459, 460, 3, 92, 46, 0, 460, 89, 1, 0, 0, 0, 461, 462, 5, 18, 0, 0, 462, 463, 5, 18, 0, 0, 463, 464, 5, 18, 0, 0, 464, 465, 3, 36, 18, 0, 465, 466, 3, 92, 46, 0, 466, 91, 1, 0, 0, 0, 467, 468, 7, 4, 0, 0, 468, 93, 1, 0, 0, 0, 52, 98, 103, 109, 115, 118, 125, 129, 136, 141, 148, 160, 168, 177, 182, 190, 200, 206, 215, 220, 232, 237, 241, 243, 248, 253, 255, 258, 261, 271, 282, 288, 297, 308, 320, 339, 341, 348, 352, 366, 372, 376, 381, 388, 394, 398, 403, 410, 416, 420, 425, 432, 438]
+[4, 1, 35, 473, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 2, 47, 7, 47, 1, 0, 1, 0, 3, 0, 99, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 104, 8, 1, 11, 1, 12, 1, 105, 1, 2, 1, 2, 3, 2, 110, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 115, 8, 3, 11, 3, 12, 3, 116, 1, 3, 5, 3, 120, 8, 3, 10, 3, 12, 3, 123, 9, 3, 1, 3, 5, 3, 126, 8, 3, 10, 3, 12, 3, 129, 9, 3, 1, 3, 5, 3, 132, 8, 3, 10, 3, 12, 3, 135, 9, 3, 1, 4, 4, 4, 138, 8, 4, 11, 4, 12, 4, 139, 1, 4, 5, 4, 143, 8, 4, 10, 4, 12, 4, 146, 9, 4, 1, 5, 1, 5, 1, 5, 1, 5, 3, 5, 152, 8, 5, 1, 6, 1, 6, 1, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 7, 5, 7, 162, 8, 7, 10, 7, 12, 7, 165, 9, 7, 1, 8, 1, 8, 1, 8, 1, 9, 1, 9, 3, 9, 172, 8, 9, 1, 9, 1, 9, 1, 10, 1, 10, 1, 10, 4, 10, 179, 8, 10, 11, 10, 12, 10, 180, 1, 10, 5, 10, 184, 8, 10, 10, 10, 12, 10, 187, 9, 10, 1, 11, 1, 11, 1, 11, 5, 11, 192, 8, 11, 10, 11, 12, 11, 195, 9, 11, 1, 12, 1, 12, 1, 12, 1, 13, 1, 13, 5, 13, 202, 8, 13, 10, 13, 12, 13, 205, 9, 13, 1, 14, 1, 14, 1, 14, 3, 14, 210, 8, 14, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 1, 15, 3, 15, 219, 8, 15, 1, 16, 1, 16, 1, 16, 3, 16, 224, 8, 16, 1, 17, 1, 17, 1, 17, 1, 17, 1, 17, 1, 18, 1, 18, 1, 19, 4, 19, 234, 8, 19, 11, 19, 12, 19, 235, 1, 20, 1, 20, 1, 20, 3, 20, 241, 8, 20, 1, 20, 1, 20, 5, 20, 245, 8, 20, 10, 20, 12, 20, 248, 9, 20, 1, 20, 1, 20, 3, 20, 252, 8, 20, 1, 20, 1, 20, 1, 20, 5, 20, 257, 8, 20, 10, 20, 12, 20, 260, 9, 20, 3, 20, 262, 8, 20, 1, 20, 3, 20, 265, 8, 20, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 3, 21, 275, 8, 21, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 23, 1, 23, 4, 23, 284, 8, 23, 11, 23, 12, 23, 285, 1, 23, 1, 23, 5, 23, 290, 8, 23, 10, 23, 12, 23, 293, 9, 23, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 3, 24, 301, 8, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 3, 27, 312, 8, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 31, 1, 31, 3, 31, 324, 8, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 36, 4, 36, 343, 8, 36, 11, 36, 12, 36, 344, 1, 36, 1, 36, 1, 36, 4, 36, 350, 8, 36, 11, 36, 12, 36, 351, 1, 36, 1, 36, 3, 36, 356, 8, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 1, 38, 1, 38, 1, 39, 1, 39, 5, 39, 368, 8, 39, 10, 39, 12, 39, 371, 9, 39, 1, 39, 5, 39, 374, 8, 39, 10, 39, 12, 39, 377, 9, 39, 1, 39, 3, 39, 380, 8, 39, 1, 39, 5, 39, 383, 8, 39, 10, 39, 12, 39, 386, 9, 39, 1, 40, 1, 40, 5, 40, 390, 8, 40, 10, 40, 12, 40, 393, 9, 40, 1, 40, 5, 40, 396, 8, 40, 10, 40, 12, 40, 399, 9, 40, 1, 40, 3, 40, 402, 8, 40, 1, 40, 5, 40, 405, 8, 40, 10, 40, 12, 40, 408, 9, 40, 1, 41, 1, 41, 5, 41, 412, 8, 41, 10, 41, 12, 41, 415, 9, 41, 1, 41, 5, 41, 418, 8, 41, 10, 41, 12, 41, 421, 9, 41, 1, 41, 3, 41, 424, 8, 41, 1, 41, 5, 41, 427, 8, 41, 10, 41, 12, 41, 430, 9, 41, 1, 42, 1, 42, 5, 42, 434, 8, 42, 10, 42, 12, 42, 437, 9, 42, 1, 42, 5, 42, 440, 8, 42, 10, 42, 12, 42, 443, 9, 42, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 44, 1, 44, 1, 44, 1, 44, 1, 45, 1, 45, 1, 45, 1, 45, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 47, 1, 47, 1, 47, 0, 0, 48, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 94, 0, 5, 2, 0, 9, 9, 32, 32, 4, 0, 17, 17, 21, 21, 24, 25, 32, 35, 2, 0, 18, 20, 22, 22, 1, 0, 26, 29, 1, 1, 7, 7, 498, 0, 96, 1, 0, 0, 0, 2, 103, 1, 0, 0, 0, 4, 107, 1, 0, 0, 0, 6, 114, 1, 0, 0, 0, 8, 137, 1, 0, 0, 0, 10, 151, 1, 0, 0, 0, 12, 153, 1, 0, 0, 0, 14, 158, 1, 0, 0, 0, 16, 166, 1, 0, 0, 0, 18, 171, 1, 0, 0, 0, 20, 175, 1, 0, 0, 0, 22, 188, 1, 0, 0, 0, 24, 196, 1, 0, 0, 0, 26, 199, 1, 0, 0, 0, 28, 206, 1, 0, 0, 0, 30, 218, 1, 0, 0, 0, 32, 220, 1, 0, 0, 0, 34, 225, 1, 0, 0, 0, 36, 230, 1, 0, 0, 0, 38, 233, 1, 0, 0, 0, 40, 237, 1, 0, 0, 0, 42, 274, 1, 0, 0, 0, 44, 276, 1, 0, 0, 0, 46, 281, 1, 0, 0, 0, 48, 300, 1, 0, 0, 0, 50, 302, 1, 0, 0, 0, 52, 304, 1, 0, 0, 0, 54, 311, 1, 0, 0, 0, 56, 313, 1, 0, 0, 0, 58, 315, 1, 0, 0, 0, 60, 317, 1, 0, 0, 0, 62, 323, 1, 0, 0, 0, 64, 325, 1, 0, 0, 0, 66, 328, 1, 0, 0, 0, 68, 331, 1, 0, 0, 0, 70, 334, 1, 0, 0, 0, 72, 355, 1, 0, 0, 0, 74, 357, 1, 0, 0, 0, 76, 361, 1, 0, 0, 0, 78, 365, 1, 0, 0, 0, 80, 387, 1, 0, 0, 0, 82, 409, 1, 0, 0, 0, 84, 431, 1, 0, 0, 0, 86, 444, 1, 0, 0, 0, 88, 456, 1, 0, 0, 0, 90, 460, 1, 0, 0, 0, 92, 464, 1, 0, 0, 0, 94, 470, 1, 0, 0, 0, 96, 98, 3, 2, 1, 0, 97, 99, 3, 6, 3, 0, 98, 97, 1, 0, 0, 0, 98, 99, 1, 0, 0, 0, 99, 100, 1, 0, 0, 0, 100, 101, 5, 0, 0, 1, 101, 1, 1, 0, 0, 0, 102, 104, 3, 4, 2, 0, 103, 102, 1, 0, 0, 0, 104, 105, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 105, 106, 1, 0, 0, 0, 106, 3, 1, 0, 0, 0, 107, 109, 5, 26, 0, 0, 108, 110, 3, 38, 19, 0, 109, 108, 1, 0, 0, 0, 109, 110, 1, 0, 0, 0, 110, 111, 1, 0, 0, 0, 111, 112, 5, 7, 0, 0, 112, 5, 1, 0, 0, 0, 113, 115, 5, 7, 0, 0, 114, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 114, 1, 0, 0, 0, 116, 117, 1, 0, 0, 0, 117, 121, 1, 0, 0, 0, 118, 120, 3, 8, 4, 0, 119, 118, 1, 0, 0, 0, 120, 123, 1, 0, 0, 0, 121, 119, 1, 0, 0, 0, 121, 122, 1, 0, 0, 0, 122, 127, 1, 0, 0, 0, 123, 121, 1, 0, 0, 0, 124, 126, 3, 80, 40, 0, 125, 124, 1, 0, 0, 0, 126, 129, 1, 0, 0, 0, 127, 125, 1, 0, 0, 0, 127, 128, 1, 0, 0, 0, 128, 133, 1, 0, 0, 0, 129, 127, 1, 0, 0, 0, 130, 132, 3, 78, 39, 0, 131, 130, 1, 0, 0, 0, 132, 135, 1, 0, 0, 0, 133, 131, 1, 0, 0, 0, 133, 134, 1, 0, 0, 0, 134, 7, 1, 0, 0, 0, 135, 133, 1, 0, 0, 0, 136, 138, 3, 10, 5, 0, 137, 136, 1, 0, 0, 0, 138, 139, 1, 0, 0, 0, 139, 137, 1, 0, 0, 0, 139, 140, 1, 0, 0, 0, 140, 144, 1, 0, 0, 0, 141, 143, 5, 7, 0, 0, 142, 141, 1, 0, 0, 0, 143, 146, 1, 0, 0, 0, 144, 142, 1, 0, 0, 0, 144, 145, 1, 0, 0, 0, 145, 9, 1, 0, 0, 0, 146, 144, 1, 0, 0, 0, 147, 152, 3, 26, 13, 0, 148, 152, 3, 14, 7, 0, 149, 152, 3, 12, 6, 0, 150, 152, 3, 4, 2, 0, 151, 147, 1, 0, 0, 0, 151, 148, 1, 0, 0, 0, 151, 149, 1, 0, 0, 0, 151, 150, 1, 0, 0, 0, 152, 11, 1, 0, 0, 0, 153, 154, 3, 76, 38, 0, 154, 155, 5, 22, 0, 0, 155, 156, 3, 38, 19, 0, 156, 157, 5, 7, 0, 0, 157, 13, 1, 0, 0, 0, 158, 159, 5, 18, 0, 0, 159, 163, 3, 16, 8, 0, 160, 162, 3, 22, 11, 0, 161, 160, 1, 0, 0, 0, 162, 165, 1, 0, 0, 0, 163, 161, 1, 0, 0, 0, 163, 164, 1, 0, 0, 0, 164, 15, 1, 0, 0, 0, 165, 163, 1, 0, 0, 0, 166, 167, 3, 18, 9, 0, 167, 168, 5, 7, 0, 0, 168, 17, 1, 0, 0, 0, 169, 170, 5, 23, 0, 0, 170, 172, 3, 36, 18, 0, 171, 169, 1, 0, 0, 0, 171, 172, 1, 0, 0, 0, 172, 173, 1, 0, 0, 0, 173, 174, 3, 20, 10, 0, 174, 19, 1, 0, 0, 0, 175, 185, 3, 38, 19, 0, 176, 178, 5, 7, 0, 0, 177, 179, 5, 23, 0, 0, 178, 177, 1, 0, 0, 0, 179, 180, 1, 0, 0, 0, 180, 178, 1, 0, 0, 0, 180, 181, 1, 0, 0, 0, 181, 182, 1, 0, 0, 0, 182, 184, 3, 38, 19, 0, 183, 176, 1, 0, 0, 0, 184, 187, 1, 0, 0, 0, 185, 183, 1, 0, 0, 0, 185, 186, 1, 0, 0, 0, 186, 21, 1, 0, 0, 0, 187, 185, 1, 0, 0, 0, 188, 189, 5, 15, 0, 0, 189, 193, 3, 16, 8, 0, 190, 192, 3, 24, 12, 0, 191, 190, 1, 0, 0, 0, 192, 195, 1, 0, 0, 0, 193, 191, 1, 0, 0, 0, 193, 194, 1, 0, 0, 0, 194, 23, 1, 0, 0, 0, 195, 193, 1, 0, 0, 0, 196, 197, 5, 16, 0, 0, 197, 198, 3, 16, 8, 0, 198, 25, 1, 0, 0, 0, 199, 203, 3, 28, 14, 0, 200, 202, 3, 22, 11, 0, 201, 200, 1, 0, 0, 0, 202, 205, 1, 0, 0, 0, 203, 201, 1, 0, 0, 0, 203, 204, 1, 0, 0, 0, 204, 27, 1, 0, 0, 0, 205, 203, 1, 0, 0, 0, 206, 209, 3, 30, 15, 0, 207, 208, 5, 23, 0, 0, 208, 210, 3, 34, 17, 0, 209, 207, 1, 0, 0, 0, 209, 210, 1, 0, 0, 0, 210, 211, 1, 0, 0, 0, 211, 212, 3, 18, 9, 0, 212, 213, 5, 7, 0, 0, 213, 29, 1, 0, 0, 0, 214, 219, 5, 8, 0, 0, 215, 219, 3, 32, 16, 0, 216, 219, 5, 34, 0, 0, 217, 219, 5, 35, 0, 0, 218, 214, 1, 0, 0, 0, 218, 215, 1, 0, 0, 0, 218, 216, 1, 0, 0, 0, 218, 217, 1, 0, 0, 0, 219, 31, 1, 0, 0, 0, 220, 223, 7, 0, 0, 0, 221, 222, 5, 22, 0, 0, 222, 224, 3, 52, 26, 0, 223, 221, 1, 0, 0, 0, 223, 224, 1, 0, 0, 0, 224, 33, 1, 0, 0, 0, 225, 226, 5, 1, 0, 0, 226, 227, 5, 26, 0, 0, 227, 228, 5, 12, 0, 0, 228, 229, 5, 2, 0, 0, 229, 35, 1, 0, 0, 0, 230, 231, 5, 13, 0, 0, 231, 37, 1, 0, 0, 0, 232, 234, 3, 40, 20, 0, 233, 232, 1, 0, 0, 0, 234, 235, 1, 0, 0, 0, 235, 233, 1, 0, 0, 0, 235, 236, 1, 0, 0, 0, 236, 39, 1, 0, 0, 0, 237, 240, 5, 23, 0, 0, 238, 239, 5, 30, 0, 0, 239, 241, 3, 56, 28, 0, 240, 238, 1, 0, 0, 0, 240, 241, 1, 0, 0, 0, 241, 246, 1, 0, 0, 0, 242, 245, 3, 56, 28, 0, 243, 245, 5, 31, 0, 0, 244, 242, 1, 0, 0, 0, 244, 243, 1, 0, 0, 0, 245, 248, 1, 0, 0, 0, 246, 244, 1, 0, 0, 0, 246, 247, 1, 0, 0, 0, 247, 251, 1, 0, 0, 0, 248, 246, 1, 0, 0, 0, 249, 252, 3, 42, 21, 0, 250, 252, 3, 72, 36, 0, 251, 249, 1, 0, 0, 0, 251, 250, 1, 0, 0, 0, 251, 252, 1, 0, 0, 0, 252, 261, 1, 0, 0, 0, 253, 258, 3, 54, 27, 0, 254, 257, 3, 54, 27, 0, 255, 257, 3, 48, 24, 0, 256, 254, 1, 0, 0, 0, 256, 255, 1, 0, 0, 0, 257, 260, 1, 0, 0, 0, 258, 256, 1, 0, 0, 0, 258, 259, 1, 0, 0, 0, 259, 262, 1, 0, 0, 0, 260, 258, 1, 0, 0, 0, 261, 253, 1, 0, 0, 0, 261, 262, 1, 0, 0, 0, 262, 264, 1, 0, 0, 0, 263, 265, 3, 76, 38, 0, 264, 263, 1, 0, 0, 0, 264, 265, 1, 0, 0, 0, 265, 41, 1, 0, 0, 0, 266, 275, 3, 60, 30, 0, 267, 275, 3, 62, 31, 0, 268, 275, 3, 74, 37, 0, 269, 275, 3, 44, 22, 0, 270, 275, 3, 46, 23, 0, 271, 275, 3, 76, 38, 0, 272, 275, 3, 36, 18, 0, 273, 275, 3, 34, 17, 0, 274, 266, 1, 0, 0, 0, 274, 267, 1, 0, 0, 0, 274, 268, 1, 0, 0, 0, 274, 269, 1, 0, 0, 0, 274, 270, 1, 0, 0, 0, 274, 271, 1, 0, 0, 0, 274, 272, 1, 0, 0, 0, 274, 273, 1, 0, 0, 0, 275, 43, 1, 0, 0, 0, 276, 277, 5, 12, 0, 0, 277, 278, 5, 22, 0, 0, 278, 279, 5, 22, 0, 0, 279, 280, 3, 46, 23, 0, 280, 45, 1, 0, 0, 0, 281, 291, 3, 48, 24, 0, 282, 284, 3, 58, 29, 0, 283, 282, 1, 0, 0, 0, 284, 285, 1, 0, 0, 0, 285, 283, 1, 0, 0, 0, 285, 286, 1, 0, 0, 0, 286, 287, 1, 0, 0, 0, 287, 288, 3, 48, 24, 0, 288, 290, 1, 0, 0, 0, 289, 283, 1, 0, 0, 0, 290, 293, 1, 0, 0, 0, 291, 289, 1, 0, 0, 0, 291, 292, 1, 0, 0, 0, 292, 47, 1, 0, 0, 0, 293, 291, 1, 0, 0, 0, 294, 301, 5, 12, 0, 0, 295, 301, 5, 14, 0, 0, 296, 301, 3, 50, 25, 0, 297, 301, 3, 52, 26, 0, 298, 301, 5, 8, 0, 0, 299, 301, 5, 9, 0, 0, 300, 294, 1, 0, 0, 0, 300, 295, 1, 0, 0, 0, 300, 296, 1, 0, 0, 0, 300, 297, 1, 0, 0, 0, 300, 298, 1, 0, 0, 0, 300, 299, 1, 0, 0, 0, 301, 49, 1, 0, 0, 0, 302, 303, 5, 10, 0, 0, 303, 51, 1, 0, 0, 0, 304, 305, 5, 11, 0, 0, 305, 53, 1, 0, 0, 0, 306, 312, 5, 30, 0, 0, 307, 312, 5, 31, 0, 0, 308, 312, 3, 56, 28, 0, 309, 312, 3, 60, 30, 0, 310, 312, 3, 58, 29, 0, 311, 306, 1, 0, 0, 0, 311, 307, 1, 0, 0, 0, 311, 308, 1, 0, 0, 0, 311, 309, 1, 0, 0, 0, 311, 310, 1, 0, 0, 0, 312, 55, 1, 0, 0, 0, 313, 314, 7, 1, 0, 0, 314, 57, 1, 0, 0, 0, 315, 316, 7, 2, 0, 0, 316, 59, 1, 0, 0, 0, 317, 318, 7, 3, 0, 0, 318, 61, 1, 0, 0, 0, 319, 324, 3, 64, 32, 0, 320, 324, 3, 66, 33, 0, 321, 324, 3, 68, 34, 0, 322, 324, 3, 70, 35, 0, 323, 319, 1, 0, 0, 0, 323, 320, 1, 0, 0, 0, 323, 321, 1, 0, 0, 0, 323, 322, 1, 0, 0, 0, 324, 63, 1, 0, 0, 0, 325, 326, 5, 26, 0, 0, 326, 327, 5, 12, 0, 0, 327, 65, 1, 0, 0, 0, 328, 329, 5, 27, 0, 0, 329, 330, 5, 12, 0, 0, 330, 67, 1, 0, 0, 0, 331, 332, 5, 29, 0, 0, 332, 333, 5, 12, 0, 0, 333, 69, 1, 0, 0, 0, 334, 335, 5, 28, 0, 0, 335, 336, 5, 12, 0, 0, 336, 71, 1, 0, 0, 0, 337, 342, 5, 30, 0, 0, 338, 343, 3, 42, 21, 0, 339, 343, 3, 34, 17, 0, 340, 343, 5, 3, 0, 0, 341, 343, 5, 4, 0, 0, 342, 338, 1, 0, 0, 0, 342, 339, 1, 0, 0, 0, 342, 340, 1, 0, 0, 0, 342, 341, 1, 0, 0, 0, 343, 344, 1, 0, 0, 0, 344, 342, 1, 0, 0, 0, 344, 345, 1, 0, 0, 0, 345, 346, 1, 0, 0, 0, 346, 356, 5, 30, 0, 0, 347, 349, 5, 31, 0, 0, 348, 350, 3, 42, 21, 0, 349, 348, 1, 0, 0, 0, 350, 351, 1, 0, 0, 0, 351, 349, 1, 0, 0, 0, 351, 352, 1, 0, 0, 0, 352, 353, 1, 0, 0, 0, 353, 354, 5, 31, 0, 0, 354, 356, 1, 0, 0, 0, 355, 337, 1, 0, 0, 0, 355, 347, 1, 0, 0, 0, 356, 73, 1, 0, 0, 0, 357, 358, 5, 3, 0, 0, 358, 359, 3, 46, 23, 0, 359, 360, 5, 4, 0, 0, 360, 75, 1, 0, 0, 0, 361, 362, 5, 1, 0, 0, 362, 363, 3, 46, 23, 0, 363, 364, 5, 2, 0, 0, 364, 77, 1, 0, 0, 0, 365, 369, 3, 86, 43, 0, 366, 368, 5, 7, 0, 0, 367, 366, 1, 0, 0, 0, 368, 371, 1, 0, 0, 0, 369, 367, 1, 0, 0, 0, 369, 370, 1, 0, 0, 0, 370, 375, 1, 0, 0, 0, 371, 369, 1, 0, 0, 0, 372, 374, 3, 8, 4, 0, 373, 372, 1, 0, 0, 0, 374, 377, 1, 0, 0, 0, 375, 373, 1, 0, 0, 0, 375, 376, 1, 0, 0, 0, 376, 384, 1, 0, 0, 0, 377, 375, 1, 0, 0, 0, 378, 380, 5, 7, 0, 0, 379, 378, 1, 0, 0, 0, 379, 380, 1, 0, 0, 0, 380, 381, 1, 0, 0, 0, 381, 383, 3, 80, 40, 0, 382, 379, 1, 0, 0, 0, 383, 386, 1, 0, 0, 0, 384, 382, 1, 0, 0, 0, 384, 385, 1, 0, 0, 0, 385, 79, 1, 0, 0, 0, 386, 384, 1, 0, 0, 0, 387, 391, 3, 88, 44, 0, 388, 390, 5, 7, 0, 0, 389, 388, 1, 0, 0, 0, 390, 393, 1, 0, 0, 0, 391, 389, 1, 0, 0, 0, 391, 392, 1, 0, 0, 0, 392, 397, 1, 0, 0, 0, 393, 391, 1, 0, 0, 0, 394, 396, 3, 8, 4, 0, 395, 394, 1, 0, 0, 0, 396, 399, 1, 0, 0, 0, 397, 395, 1, 0, 0, 0, 397, 398, 1, 0, 0, 0, 398, 406, 1, 0, 0, 0, 399, 397, 1, 0, 0, 0, 400, 402, 5, 7, 0, 0, 401, 400, 1, 0, 0, 0, 401, 402, 1, 0, 0, 0, 402, 403, 1, 0, 0, 0, 403, 405, 3, 82, 41, 0, 404, 401, 1, 0, 0, 0, 405, 408, 1, 0, 0, 0, 406, 404, 1, 0, 0, 0, 406, 407, 1, 0, 0, 0, 407, 81, 1, 0, 0, 0, 408, 406, 1, 0, 0, 0, 409, 413, 3, 90, 45, 0, 410, 412, 5, 7, 0, 0, 411, 410, 1, 0, 0, 0, 412, 415, 1, 0, 0, 0, 413, 411, 1, 0, 0, 0, 413, 414, 1, 0, 0, 0, 414, 419, 1, 0, 0, 0, 415, 413, 1, 0, 0, 0, 416, 418, 3, 8, 4, 0, 417, 416, 1, 0, 0, 0, 418, 421, 1, 0, 0, 0, 419, 417, 1, 0, 0, 0, 419, 420, 1, 0, 0, 0, 420, 428, 1, 0, 0, 0, 421, 419, 1, 0, 0, 0, 422, 424, 5, 7, 0, 0, 423, 422, 1, 0, 0, 0, 423, 424, 1, 0, 0, 0, 424, 425, 1, 0, 0, 0, 425, 427, 3, 84, 42, 0, 426, 423, 1, 0, 0, 0, 427, 430, 1, 0, 0, 0, 428, 426, 1, 0, 0, 0, 428, 429, 1, 0, 0, 0, 429, 83, 1, 0, 0, 0, 430, 428, 1, 0, 0, 0, 431, 435, 3, 92, 46, 0, 432, 434, 5, 7, 0, 0, 433, 432, 1, 0, 0, 0, 434, 437, 1, 0, 0, 0, 435, 433, 1, 0, 0, 0, 435, 436, 1, 0, 0, 0, 436, 441, 1, 0, 0, 0, 437, 435, 1, 0, 0, 0, 438, 440, 3, 8, 4, 0, 439, 438, 1, 0, 0, 0, 440, 443, 1, 0, 0, 0, 441, 439, 1, 0, 0, 0, 441, 442, 1, 0, 0, 0, 442, 85, 1, 0, 0, 0, 443, 441, 1, 0, 0, 0, 444, 445, 5, 26, 0, 0, 445, 446, 5, 26, 0, 0, 446, 447, 5, 26, 0, 0, 447, 448, 5, 26, 0, 0, 448, 449, 5, 26, 0, 0, 449, 450, 5, 26, 0, 0, 450, 451, 5, 26, 0, 0, 451, 452, 5, 26, 0, 0, 452, 453, 5, 26, 0, 0, 453, 454, 3, 38, 19, 0, 454, 455, 3, 94, 47, 0, 455, 87, 1, 0, 0, 0, 456, 457, 5, 5, 0, 0, 457, 458, 3, 38, 19, 0, 458, 459, 3, 94, 47, 0, 459, 89, 1, 0, 0, 0, 460, 461, 5, 6, 0, 0, 461, 462, 3, 38, 19, 0, 462, 463, 3, 94, 47, 0, 463, 91, 1, 0, 0, 0, 464, 465, 5, 18, 0, 0, 465, 466, 5, 18, 0, 0, 466, 467, 5, 18, 0, 0, 467, 468, 3, 38, 19, 0, 468, 469, 3, 94, 47, 0, 469, 93, 1, 0, 0, 0, 470, 471, 7, 4, 0, 0, 471, 95, 1, 0, 0, 0, 52, 98, 105, 109, 116, 121, 127, 133, 139, 144, 151, 163, 171, 180, 185, 193, 203, 209, 218, 223, 235, 240, 244, 246, 251, 256, 258, 261, 264, 274, 285, 291, 300, 311, 323, 342, 344, 351, 355, 369, 375, 379, 384, 391, 397, 401, 406, 413, 419, 423, 428, 435, 441]
```

### Comparing `zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFile.tokens` & `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFile.tokens`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 T__2=3
 T__3=4
 T__4=5
 T__5=6
 NL=7
 LOWER_O=8
 LOWER_X=9
-ID=10
-DATE=11
-TIME=12
+DATE=10
+TIME=11
+ID=12
 ZID=13
 NUM_ID=14
 TWO_SPACE_DASH=15
 FOUR_SPACE_DASH=16
 SYMBOL=17
 DASH=18
 DOT=19
```

### Comparing `zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileLexer.interp` & `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.interp`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 null
 null
 null
 null
 NL
 LOWER_O
 LOWER_X
-ID
 DATE
 TIME
+ID
 ZID
 NUM_ID
 TWO_SPACE_DASH
 FOUR_SPACE_DASH
 SYMBOL
 DASH
 DOT
@@ -80,17 +80,17 @@
 T__2
 T__3
 T__4
 T__5
 NL
 LOWER_O
 LOWER_X
-ID
 DATE
 TIME
+ID
 ZID
 NUM_ID
 TWO_SPACE_DASH
 FOUR_SPACE_DASH
 SYMBOL
 DASH
 DOT
@@ -123,8 +123,8 @@
 DEFAULT_TOKEN_CHANNEL
 HIDDEN
 
 mode names:
 DEFAULT_MODE
 
 atn:
-[4, 0, 35, 234, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 1, 0, 1, 0, 1, 1, 1, 1, 1, 2, 1, 2, 1, 2, 1, 3, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 3, 6, 113, 8, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 5, 9, 124, 8, 9, 10, 9, 12, 9, 127, 9, 9, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 11, 1, 11, 1, 11, 1, 11, 1, 11, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 3, 12, 155, 8, 12, 1, 13, 1, 13, 1, 13, 5, 13, 160, 8, 13, 10, 13, 12, 13, 163, 9, 13, 1, 14, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 1, 15, 1, 15, 1, 15, 1, 16, 1, 16, 1, 17, 1, 17, 1, 18, 1, 18, 1, 19, 1, 19, 1, 20, 1, 20, 1, 21, 1, 21, 1, 22, 1, 22, 1, 23, 1, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 32, 1, 32, 1, 33, 1, 33, 1, 34, 1, 34, 1, 35, 1, 35, 1, 36, 1, 36, 1, 37, 1, 37, 3, 37, 219, 8, 37, 1, 38, 1, 38, 1, 39, 1, 39, 1, 40, 1, 40, 1, 41, 1, 41, 3, 41, 229, 8, 41, 1, 42, 1, 42, 3, 42, 233, 8, 42, 0, 0, 43, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 27, 14, 29, 15, 31, 16, 33, 17, 35, 18, 37, 19, 39, 20, 41, 21, 43, 22, 45, 23, 47, 24, 49, 25, 51, 26, 53, 27, 55, 28, 57, 29, 59, 30, 61, 31, 63, 32, 65, 33, 67, 34, 69, 35, 71, 0, 73, 0, 75, 0, 77, 0, 79, 0, 81, 0, 83, 0, 85, 0, 1, 0, 2, 10, 0, 33, 33, 36, 36, 38, 38, 44, 44, 59, 59, 61, 61, 63, 63, 91, 94, 96, 96, 123, 125, 6, 0, 65, 72, 74, 78, 80, 90, 97, 105, 107, 107, 109, 122, 234, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 0, 27, 1, 0, 0, 0, 0, 29, 1, 0, 0, 0, 0, 31, 1, 0, 0, 0, 0, 33, 1, 0, 0, 0, 0, 35, 1, 0, 0, 0, 0, 37, 1, 0, 0, 0, 0, 39, 1, 0, 0, 0, 0, 41, 1, 0, 0, 0, 0, 43, 1, 0, 0, 0, 0, 45, 1, 0, 0, 0, 0, 47, 1, 0, 0, 0, 0, 49, 1, 0, 0, 0, 0, 51, 1, 0, 0, 0, 0, 53, 1, 0, 0, 0, 0, 55, 1, 0, 0, 0, 0, 57, 1, 0, 0, 0, 0, 59, 1, 0, 0, 0, 0, 61, 1, 0, 0, 0, 0, 63, 1, 0, 0, 0, 0, 65, 1, 0, 0, 0, 0, 67, 1, 0, 0, 0, 0, 69, 1, 0, 0, 0, 1, 87, 1, 0, 0, 0, 3, 89, 1, 0, 0, 0, 5, 91, 1, 0, 0, 0, 7, 94, 1, 0, 0, 0, 9, 97, 1, 0, 0, 0, 11, 105, 1, 0, 0, 0, 13, 112, 1, 0, 0, 0, 15, 116, 1, 0, 0, 0, 17, 118, 1, 0, 0, 0, 19, 120, 1, 0, 0, 0, 21, 128, 1, 0, 0, 0, 23, 139, 1, 0, 0, 0, 25, 144, 1, 0, 0, 0, 27, 156, 1, 0, 0, 0, 29, 164, 1, 0, 0, 0, 31, 168, 1, 0, 0, 0, 33, 174, 1, 0, 0, 0, 35, 176, 1, 0, 0, 0, 37, 178, 1, 0, 0, 0, 39, 180, 1, 0, 0, 0, 41, 182, 1, 0, 0, 0, 43, 184, 1, 0, 0, 0, 45, 186, 1, 0, 0, 0, 47, 188, 1, 0, 0, 0, 49, 190, 1, 0, 0, 0, 51, 192, 1, 0, 0, 0, 53, 194, 1, 0, 0, 0, 55, 196, 1, 0, 0, 0, 57, 198, 1, 0, 0, 0, 59, 200, 1, 0, 0, 0, 61, 202, 1, 0, 0, 0, 63, 204, 1, 0, 0, 0, 65, 206, 1, 0, 0, 0, 67, 208, 1, 0, 0, 0, 69, 210, 1, 0, 0, 0, 71, 212, 1, 0, 0, 0, 73, 214, 1, 0, 0, 0, 75, 218, 1, 0, 0, 0, 77, 220, 1, 0, 0, 0, 79, 222, 1, 0, 0, 0, 81, 224, 1, 0, 0, 0, 83, 228, 1, 0, 0, 0, 85, 232, 1, 0, 0, 0, 87, 88, 5, 91, 0, 0, 88, 2, 1, 0, 0, 0, 89, 90, 5, 93, 0, 0, 90, 4, 1, 0, 0, 0, 91, 92, 5, 91, 0, 0, 92, 93, 5, 91, 0, 0, 93, 6, 1, 0, 0, 0, 94, 95, 5, 93, 0, 0, 95, 96, 5, 93, 0, 0, 96, 8, 1, 0, 0, 0, 97, 98, 5, 61, 0, 0, 98, 99, 5, 61, 0, 0, 99, 100, 5, 61, 0, 0, 100, 101, 5, 61, 0, 0, 101, 102, 5, 61, 0, 0, 102, 103, 5, 61, 0, 0, 103, 104, 5, 61, 0, 0, 104, 10, 1, 0, 0, 0, 105, 106, 5, 42, 0, 0, 106, 107, 5, 42, 0, 0, 107, 108, 5, 42, 0, 0, 108, 109, 5, 42, 0, 0, 109, 110, 5, 42, 0, 0, 110, 12, 1, 0, 0, 0, 111, 113, 5, 13, 0, 0, 112, 111, 1, 0, 0, 0, 112, 113, 1, 0, 0, 0, 113, 114, 1, 0, 0, 0, 114, 115, 5, 10, 0, 0, 115, 14, 1, 0, 0, 0, 116, 117, 5, 111, 0, 0, 117, 16, 1, 0, 0, 0, 118, 119, 5, 120, 0, 0, 119, 18, 1, 0, 0, 0, 120, 125, 3, 83, 41, 0, 121, 124, 3, 85, 42, 0, 122, 124, 3, 41, 20, 0, 123, 121, 1, 0, 0, 0, 123, 122, 1, 0, 0, 0, 124, 127, 1, 0, 0, 0, 125, 123, 1, 0, 0, 0, 125, 126, 1, 0, 0, 0, 126, 20, 1, 0, 0, 0, 127, 125, 1, 0, 0, 0, 128, 129, 5, 50, 0, 0, 129, 130, 3, 77, 38, 0, 130, 131, 3, 77, 38, 0, 131, 132, 3, 77, 38, 0, 132, 133, 3, 35, 17, 0, 133, 134, 3, 81, 40, 0, 134, 135, 3, 77, 38, 0, 135, 136, 3, 35, 17, 0, 136, 137, 3, 79, 39, 0, 137, 138, 3, 77, 38, 0, 138, 22, 1, 0, 0, 0, 139, 140, 2, 48, 50, 0, 140, 141, 3, 77, 38, 0, 141, 142, 2, 48, 53, 0, 142, 143, 3, 77, 38, 0, 143, 24, 1, 0, 0, 0, 144, 145, 3, 77, 38, 0, 145, 146, 3, 77, 38, 0, 146, 147, 3, 81, 40, 0, 147, 148, 3, 77, 38, 0, 148, 149, 3, 79, 39, 0, 149, 150, 3, 77, 38, 0, 150, 151, 3, 51, 25, 0, 151, 152, 3, 75, 37, 0, 152, 154, 3, 75, 37, 0, 153, 155, 3, 75, 37, 0, 154, 153, 1, 0, 0, 0, 154, 155, 1, 0, 0, 0, 155, 26, 1, 0, 0, 0, 156, 161, 3, 77, 38, 0, 157, 160, 3, 85, 42, 0, 158, 160, 3, 41, 20, 0, 159, 157, 1, 0, 0, 0, 159, 158, 1, 0, 0, 0, 160, 163, 1, 0, 0, 0, 161, 159, 1, 0, 0, 0, 161, 162, 1, 0, 0, 0, 162, 28, 1, 0, 0, 0, 163, 161, 1, 0, 0, 0, 164, 165, 5, 32, 0, 0, 165, 166, 5, 32, 0, 0, 166, 167, 5, 45, 0, 0, 167, 30, 1, 0, 0, 0, 168, 169, 5, 32, 0, 0, 169, 170, 5, 32, 0, 0, 170, 171, 5, 32, 0, 0, 171, 172, 5, 32, 0, 0, 172, 173, 5, 45, 0, 0, 173, 32, 1, 0, 0, 0, 174, 175, 7, 0, 0, 0, 175, 34, 1, 0, 0, 0, 176, 177, 5, 45, 0, 0, 177, 36, 1, 0, 0, 0, 178, 179, 5, 46, 0, 0, 179, 38, 1, 0, 0, 0, 180, 181, 5, 47, 0, 0, 181, 40, 1, 0, 0, 0, 182, 183, 5, 95, 0, 0, 183, 42, 1, 0, 0, 0, 184, 185, 5, 58, 0, 0, 185, 44, 1, 0, 0, 0, 186, 187, 5, 32, 0, 0, 187, 46, 1, 0, 0, 0, 188, 189, 5, 40, 0, 0, 189, 48, 1, 0, 0, 0, 190, 191, 5, 41, 0, 0, 191, 50, 1, 0, 0, 0, 192, 193, 5, 35, 0, 0, 193, 52, 1, 0, 0, 0, 194, 195, 5, 64, 0, 0, 195, 54, 1, 0, 0, 0, 196, 197, 5, 43, 0, 0, 197, 56, 1, 0, 0, 0, 198, 199, 5, 37, 0, 0, 199, 58, 1, 0, 0, 0, 200, 201, 5, 39, 0, 0, 201, 60, 1, 0, 0, 0, 202, 203, 5, 34, 0, 0, 203, 62, 1, 0, 0, 0, 204, 205, 5, 126, 0, 0, 205, 64, 1, 0, 0, 0, 206, 207, 5, 42, 0, 0, 207, 66, 1, 0, 0, 0, 208, 209, 5, 60, 0, 0, 209, 68, 1, 0, 0, 0, 210, 211, 5, 62, 0, 0, 211, 70, 1, 0, 0, 0, 212, 213, 2, 65, 90, 0, 213, 72, 1, 0, 0, 0, 214, 215, 2, 97, 122, 0, 215, 74, 1, 0, 0, 0, 216, 219, 3, 77, 38, 0, 217, 219, 7, 1, 0, 0, 218, 216, 1, 0, 0, 0, 218, 217, 1, 0, 0, 0, 219, 76, 1, 0, 0, 0, 220, 221, 2, 48, 57, 0, 221, 78, 1, 0, 0, 0, 222, 223, 2, 48, 51, 0, 223, 80, 1, 0, 0, 0, 224, 225, 2, 48, 49, 0, 225, 82, 1, 0, 0, 0, 226, 229, 3, 71, 35, 0, 227, 229, 3, 73, 36, 0, 228, 226, 1, 0, 0, 0, 228, 227, 1, 0, 0, 0, 229, 84, 1, 0, 0, 0, 230, 233, 3, 83, 41, 0, 231, 233, 3, 77, 38, 0, 232, 230, 1, 0, 0, 0, 232, 231, 1, 0, 0, 0, 233, 86, 1, 0, 0, 0, 10, 0, 112, 123, 125, 154, 159, 161, 218, 228, 232, 0]
+[4, 0, 35, 234, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 1, 0, 1, 0, 1, 1, 1, 1, 1, 2, 1, 2, 1, 2, 1, 3, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 3, 6, 113, 8, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 11, 1, 11, 1, 11, 5, 11, 140, 8, 11, 10, 11, 12, 11, 143, 9, 11, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 3, 12, 155, 8, 12, 1, 13, 1, 13, 1, 13, 5, 13, 160, 8, 13, 10, 13, 12, 13, 163, 9, 13, 1, 14, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 1, 15, 1, 15, 1, 15, 1, 16, 1, 16, 1, 17, 1, 17, 1, 18, 1, 18, 1, 19, 1, 19, 1, 20, 1, 20, 1, 21, 1, 21, 1, 22, 1, 22, 1, 23, 1, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 32, 1, 32, 1, 33, 1, 33, 1, 34, 1, 34, 1, 35, 1, 35, 1, 36, 1, 36, 1, 37, 1, 37, 3, 37, 219, 8, 37, 1, 38, 1, 38, 1, 39, 1, 39, 1, 40, 1, 40, 1, 41, 1, 41, 3, 41, 229, 8, 41, 1, 42, 1, 42, 3, 42, 233, 8, 42, 0, 0, 43, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 27, 14, 29, 15, 31, 16, 33, 17, 35, 18, 37, 19, 39, 20, 41, 21, 43, 22, 45, 23, 47, 24, 49, 25, 51, 26, 53, 27, 55, 28, 57, 29, 59, 30, 61, 31, 63, 32, 65, 33, 67, 34, 69, 35, 71, 0, 73, 0, 75, 0, 77, 0, 79, 0, 81, 0, 83, 0, 85, 0, 1, 0, 2, 10, 0, 33, 33, 36, 36, 38, 38, 44, 44, 59, 59, 61, 61, 63, 63, 91, 94, 96, 96, 123, 125, 6, 0, 65, 72, 74, 78, 80, 90, 97, 105, 107, 107, 109, 122, 234, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 0, 27, 1, 0, 0, 0, 0, 29, 1, 0, 0, 0, 0, 31, 1, 0, 0, 0, 0, 33, 1, 0, 0, 0, 0, 35, 1, 0, 0, 0, 0, 37, 1, 0, 0, 0, 0, 39, 1, 0, 0, 0, 0, 41, 1, 0, 0, 0, 0, 43, 1, 0, 0, 0, 0, 45, 1, 0, 0, 0, 0, 47, 1, 0, 0, 0, 0, 49, 1, 0, 0, 0, 0, 51, 1, 0, 0, 0, 0, 53, 1, 0, 0, 0, 0, 55, 1, 0, 0, 0, 0, 57, 1, 0, 0, 0, 0, 59, 1, 0, 0, 0, 0, 61, 1, 0, 0, 0, 0, 63, 1, 0, 0, 0, 0, 65, 1, 0, 0, 0, 0, 67, 1, 0, 0, 0, 0, 69, 1, 0, 0, 0, 1, 87, 1, 0, 0, 0, 3, 89, 1, 0, 0, 0, 5, 91, 1, 0, 0, 0, 7, 94, 1, 0, 0, 0, 9, 97, 1, 0, 0, 0, 11, 105, 1, 0, 0, 0, 13, 112, 1, 0, 0, 0, 15, 116, 1, 0, 0, 0, 17, 118, 1, 0, 0, 0, 19, 120, 1, 0, 0, 0, 21, 131, 1, 0, 0, 0, 23, 136, 1, 0, 0, 0, 25, 144, 1, 0, 0, 0, 27, 156, 1, 0, 0, 0, 29, 164, 1, 0, 0, 0, 31, 168, 1, 0, 0, 0, 33, 174, 1, 0, 0, 0, 35, 176, 1, 0, 0, 0, 37, 178, 1, 0, 0, 0, 39, 180, 1, 0, 0, 0, 41, 182, 1, 0, 0, 0, 43, 184, 1, 0, 0, 0, 45, 186, 1, 0, 0, 0, 47, 188, 1, 0, 0, 0, 49, 190, 1, 0, 0, 0, 51, 192, 1, 0, 0, 0, 53, 194, 1, 0, 0, 0, 55, 196, 1, 0, 0, 0, 57, 198, 1, 0, 0, 0, 59, 200, 1, 0, 0, 0, 61, 202, 1, 0, 0, 0, 63, 204, 1, 0, 0, 0, 65, 206, 1, 0, 0, 0, 67, 208, 1, 0, 0, 0, 69, 210, 1, 0, 0, 0, 71, 212, 1, 0, 0, 0, 73, 214, 1, 0, 0, 0, 75, 218, 1, 0, 0, 0, 77, 220, 1, 0, 0, 0, 79, 222, 1, 0, 0, 0, 81, 224, 1, 0, 0, 0, 83, 228, 1, 0, 0, 0, 85, 232, 1, 0, 0, 0, 87, 88, 5, 91, 0, 0, 88, 2, 1, 0, 0, 0, 89, 90, 5, 93, 0, 0, 90, 4, 1, 0, 0, 0, 91, 92, 5, 91, 0, 0, 92, 93, 5, 91, 0, 0, 93, 6, 1, 0, 0, 0, 94, 95, 5, 93, 0, 0, 95, 96, 5, 93, 0, 0, 96, 8, 1, 0, 0, 0, 97, 98, 5, 61, 0, 0, 98, 99, 5, 61, 0, 0, 99, 100, 5, 61, 0, 0, 100, 101, 5, 61, 0, 0, 101, 102, 5, 61, 0, 0, 102, 103, 5, 61, 0, 0, 103, 104, 5, 61, 0, 0, 104, 10, 1, 0, 0, 0, 105, 106, 5, 42, 0, 0, 106, 107, 5, 42, 0, 0, 107, 108, 5, 42, 0, 0, 108, 109, 5, 42, 0, 0, 109, 110, 5, 42, 0, 0, 110, 12, 1, 0, 0, 0, 111, 113, 5, 13, 0, 0, 112, 111, 1, 0, 0, 0, 112, 113, 1, 0, 0, 0, 113, 114, 1, 0, 0, 0, 114, 115, 5, 10, 0, 0, 115, 14, 1, 0, 0, 0, 116, 117, 5, 111, 0, 0, 117, 16, 1, 0, 0, 0, 118, 119, 5, 120, 0, 0, 119, 18, 1, 0, 0, 0, 120, 121, 5, 50, 0, 0, 121, 122, 3, 77, 38, 0, 122, 123, 3, 77, 38, 0, 123, 124, 3, 77, 38, 0, 124, 125, 3, 35, 17, 0, 125, 126, 3, 81, 40, 0, 126, 127, 3, 77, 38, 0, 127, 128, 3, 35, 17, 0, 128, 129, 3, 79, 39, 0, 129, 130, 3, 77, 38, 0, 130, 20, 1, 0, 0, 0, 131, 132, 2, 48, 50, 0, 132, 133, 3, 77, 38, 0, 133, 134, 2, 48, 53, 0, 134, 135, 3, 77, 38, 0, 135, 22, 1, 0, 0, 0, 136, 141, 3, 85, 42, 0, 137, 140, 3, 85, 42, 0, 138, 140, 3, 41, 20, 0, 139, 137, 1, 0, 0, 0, 139, 138, 1, 0, 0, 0, 140, 143, 1, 0, 0, 0, 141, 139, 1, 0, 0, 0, 141, 142, 1, 0, 0, 0, 142, 24, 1, 0, 0, 0, 143, 141, 1, 0, 0, 0, 144, 145, 3, 77, 38, 0, 145, 146, 3, 77, 38, 0, 146, 147, 3, 81, 40, 0, 147, 148, 3, 77, 38, 0, 148, 149, 3, 79, 39, 0, 149, 150, 3, 77, 38, 0, 150, 151, 3, 51, 25, 0, 151, 152, 3, 75, 37, 0, 152, 154, 3, 75, 37, 0, 153, 155, 3, 75, 37, 0, 154, 153, 1, 0, 0, 0, 154, 155, 1, 0, 0, 0, 155, 26, 1, 0, 0, 0, 156, 161, 3, 77, 38, 0, 157, 160, 3, 85, 42, 0, 158, 160, 3, 41, 20, 0, 159, 157, 1, 0, 0, 0, 159, 158, 1, 0, 0, 0, 160, 163, 1, 0, 0, 0, 161, 159, 1, 0, 0, 0, 161, 162, 1, 0, 0, 0, 162, 28, 1, 0, 0, 0, 163, 161, 1, 0, 0, 0, 164, 165, 5, 32, 0, 0, 165, 166, 5, 32, 0, 0, 166, 167, 5, 45, 0, 0, 167, 30, 1, 0, 0, 0, 168, 169, 5, 32, 0, 0, 169, 170, 5, 32, 0, 0, 170, 171, 5, 32, 0, 0, 171, 172, 5, 32, 0, 0, 172, 173, 5, 45, 0, 0, 173, 32, 1, 0, 0, 0, 174, 175, 7, 0, 0, 0, 175, 34, 1, 0, 0, 0, 176, 177, 5, 45, 0, 0, 177, 36, 1, 0, 0, 0, 178, 179, 5, 46, 0, 0, 179, 38, 1, 0, 0, 0, 180, 181, 5, 47, 0, 0, 181, 40, 1, 0, 0, 0, 182, 183, 5, 95, 0, 0, 183, 42, 1, 0, 0, 0, 184, 185, 5, 58, 0, 0, 185, 44, 1, 0, 0, 0, 186, 187, 5, 32, 0, 0, 187, 46, 1, 0, 0, 0, 188, 189, 5, 40, 0, 0, 189, 48, 1, 0, 0, 0, 190, 191, 5, 41, 0, 0, 191, 50, 1, 0, 0, 0, 192, 193, 5, 35, 0, 0, 193, 52, 1, 0, 0, 0, 194, 195, 5, 64, 0, 0, 195, 54, 1, 0, 0, 0, 196, 197, 5, 43, 0, 0, 197, 56, 1, 0, 0, 0, 198, 199, 5, 37, 0, 0, 199, 58, 1, 0, 0, 0, 200, 201, 5, 39, 0, 0, 201, 60, 1, 0, 0, 0, 202, 203, 5, 34, 0, 0, 203, 62, 1, 0, 0, 0, 204, 205, 5, 126, 0, 0, 205, 64, 1, 0, 0, 0, 206, 207, 5, 42, 0, 0, 207, 66, 1, 0, 0, 0, 208, 209, 5, 60, 0, 0, 209, 68, 1, 0, 0, 0, 210, 211, 5, 62, 0, 0, 211, 70, 1, 0, 0, 0, 212, 213, 2, 65, 90, 0, 213, 72, 1, 0, 0, 0, 214, 215, 2, 97, 122, 0, 215, 74, 1, 0, 0, 0, 216, 219, 3, 77, 38, 0, 217, 219, 7, 1, 0, 0, 218, 216, 1, 0, 0, 0, 218, 217, 1, 0, 0, 0, 219, 76, 1, 0, 0, 0, 220, 221, 2, 48, 57, 0, 221, 78, 1, 0, 0, 0, 222, 223, 2, 48, 51, 0, 223, 80, 1, 0, 0, 0, 224, 225, 2, 48, 49, 0, 225, 82, 1, 0, 0, 0, 226, 229, 3, 71, 35, 0, 227, 229, 3, 73, 36, 0, 228, 226, 1, 0, 0, 0, 228, 227, 1, 0, 0, 0, 229, 84, 1, 0, 0, 0, 230, 233, 3, 83, 41, 0, 231, 233, 3, 77, 38, 0, 232, 230, 1, 0, 0, 0, 232, 231, 1, 0, 0, 0, 233, 86, 1, 0, 0, 0, 10, 0, 112, 139, 141, 154, 159, 161, 218, 228, 232, 0]
```

### Comparing `zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileLexer.py` & `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from src/zorg/grammar/zorg_file/ZorgFile.g4 by ANTLR 4.13.1
+# Generated from ZorgFile.g4 by ANTLR 4.13.1
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -14,86 +14,86 @@
         2,6,7,6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,
         13,7,13,2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,
         19,2,20,7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,
         26,7,26,2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,
         32,2,33,7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,
         39,7,39,2,40,7,40,2,41,7,41,2,42,7,42,1,0,1,0,1,1,1,1,1,2,1,2,1,
         2,1,3,1,3,1,3,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,
-        5,1,5,1,6,3,6,113,8,6,1,6,1,6,1,7,1,7,1,8,1,8,1,9,1,9,1,9,5,9,124,
-        8,9,10,9,12,9,127,9,9,1,10,1,10,1,10,1,10,1,10,1,10,1,10,1,10,1,
-        10,1,10,1,10,1,11,1,11,1,11,1,11,1,11,1,12,1,12,1,12,1,12,1,12,1,
-        12,1,12,1,12,1,12,1,12,3,12,155,8,12,1,13,1,13,1,13,5,13,160,8,13,
-        10,13,12,13,163,9,13,1,14,1,14,1,14,1,14,1,15,1,15,1,15,1,15,1,15,
-        1,15,1,16,1,16,1,17,1,17,1,18,1,18,1,19,1,19,1,20,1,20,1,21,1,21,
-        1,22,1,22,1,23,1,23,1,24,1,24,1,25,1,25,1,26,1,26,1,27,1,27,1,28,
-        1,28,1,29,1,29,1,30,1,30,1,31,1,31,1,32,1,32,1,33,1,33,1,34,1,34,
-        1,35,1,35,1,36,1,36,1,37,1,37,3,37,219,8,37,1,38,1,38,1,39,1,39,
-        1,40,1,40,1,41,1,41,3,41,229,8,41,1,42,1,42,3,42,233,8,42,0,0,43,
-        1,1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,10,21,11,23,12,25,13,
-        27,14,29,15,31,16,33,17,35,18,37,19,39,20,41,21,43,22,45,23,47,24,
-        49,25,51,26,53,27,55,28,57,29,59,30,61,31,63,32,65,33,67,34,69,35,
-        71,0,73,0,75,0,77,0,79,0,81,0,83,0,85,0,1,0,2,10,0,33,33,36,36,38,
-        38,44,44,59,59,61,61,63,63,91,94,96,96,123,125,6,0,65,72,74,78,80,
-        90,97,105,107,107,109,122,234,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,
-        0,0,7,1,0,0,0,0,9,1,0,0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,
-        0,17,1,0,0,0,0,19,1,0,0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,
-        0,27,1,0,0,0,0,29,1,0,0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,
-        0,37,1,0,0,0,0,39,1,0,0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,
-        0,47,1,0,0,0,0,49,1,0,0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,
-        0,57,1,0,0,0,0,59,1,0,0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,
-        0,67,1,0,0,0,0,69,1,0,0,0,1,87,1,0,0,0,3,89,1,0,0,0,5,91,1,0,0,0,
-        7,94,1,0,0,0,9,97,1,0,0,0,11,105,1,0,0,0,13,112,1,0,0,0,15,116,1,
-        0,0,0,17,118,1,0,0,0,19,120,1,0,0,0,21,128,1,0,0,0,23,139,1,0,0,
-        0,25,144,1,0,0,0,27,156,1,0,0,0,29,164,1,0,0,0,31,168,1,0,0,0,33,
-        174,1,0,0,0,35,176,1,0,0,0,37,178,1,0,0,0,39,180,1,0,0,0,41,182,
-        1,0,0,0,43,184,1,0,0,0,45,186,1,0,0,0,47,188,1,0,0,0,49,190,1,0,
-        0,0,51,192,1,0,0,0,53,194,1,0,0,0,55,196,1,0,0,0,57,198,1,0,0,0,
-        59,200,1,0,0,0,61,202,1,0,0,0,63,204,1,0,0,0,65,206,1,0,0,0,67,208,
-        1,0,0,0,69,210,1,0,0,0,71,212,1,0,0,0,73,214,1,0,0,0,75,218,1,0,
-        0,0,77,220,1,0,0,0,79,222,1,0,0,0,81,224,1,0,0,0,83,228,1,0,0,0,
-        85,232,1,0,0,0,87,88,5,91,0,0,88,2,1,0,0,0,89,90,5,93,0,0,90,4,1,
-        0,0,0,91,92,5,91,0,0,92,93,5,91,0,0,93,6,1,0,0,0,94,95,5,93,0,0,
-        95,96,5,93,0,0,96,8,1,0,0,0,97,98,5,61,0,0,98,99,5,61,0,0,99,100,
-        5,61,0,0,100,101,5,61,0,0,101,102,5,61,0,0,102,103,5,61,0,0,103,
-        104,5,61,0,0,104,10,1,0,0,0,105,106,5,42,0,0,106,107,5,42,0,0,107,
-        108,5,42,0,0,108,109,5,42,0,0,109,110,5,42,0,0,110,12,1,0,0,0,111,
-        113,5,13,0,0,112,111,1,0,0,0,112,113,1,0,0,0,113,114,1,0,0,0,114,
-        115,5,10,0,0,115,14,1,0,0,0,116,117,5,111,0,0,117,16,1,0,0,0,118,
-        119,5,120,0,0,119,18,1,0,0,0,120,125,3,83,41,0,121,124,3,85,42,0,
-        122,124,3,41,20,0,123,121,1,0,0,0,123,122,1,0,0,0,124,127,1,0,0,
-        0,125,123,1,0,0,0,125,126,1,0,0,0,126,20,1,0,0,0,127,125,1,0,0,0,
-        128,129,5,50,0,0,129,130,3,77,38,0,130,131,3,77,38,0,131,132,3,77,
-        38,0,132,133,3,35,17,0,133,134,3,81,40,0,134,135,3,77,38,0,135,136,
-        3,35,17,0,136,137,3,79,39,0,137,138,3,77,38,0,138,22,1,0,0,0,139,
-        140,2,48,50,0,140,141,3,77,38,0,141,142,2,48,53,0,142,143,3,77,38,
-        0,143,24,1,0,0,0,144,145,3,77,38,0,145,146,3,77,38,0,146,147,3,81,
-        40,0,147,148,3,77,38,0,148,149,3,79,39,0,149,150,3,77,38,0,150,151,
-        3,51,25,0,151,152,3,75,37,0,152,154,3,75,37,0,153,155,3,75,37,0,
-        154,153,1,0,0,0,154,155,1,0,0,0,155,26,1,0,0,0,156,161,3,77,38,0,
-        157,160,3,85,42,0,158,160,3,41,20,0,159,157,1,0,0,0,159,158,1,0,
-        0,0,160,163,1,0,0,0,161,159,1,0,0,0,161,162,1,0,0,0,162,28,1,0,0,
-        0,163,161,1,0,0,0,164,165,5,32,0,0,165,166,5,32,0,0,166,167,5,45,
-        0,0,167,30,1,0,0,0,168,169,5,32,0,0,169,170,5,32,0,0,170,171,5,32,
-        0,0,171,172,5,32,0,0,172,173,5,45,0,0,173,32,1,0,0,0,174,175,7,0,
-        0,0,175,34,1,0,0,0,176,177,5,45,0,0,177,36,1,0,0,0,178,179,5,46,
-        0,0,179,38,1,0,0,0,180,181,5,47,0,0,181,40,1,0,0,0,182,183,5,95,
-        0,0,183,42,1,0,0,0,184,185,5,58,0,0,185,44,1,0,0,0,186,187,5,32,
-        0,0,187,46,1,0,0,0,188,189,5,40,0,0,189,48,1,0,0,0,190,191,5,41,
-        0,0,191,50,1,0,0,0,192,193,5,35,0,0,193,52,1,0,0,0,194,195,5,64,
-        0,0,195,54,1,0,0,0,196,197,5,43,0,0,197,56,1,0,0,0,198,199,5,37,
-        0,0,199,58,1,0,0,0,200,201,5,39,0,0,201,60,1,0,0,0,202,203,5,34,
-        0,0,203,62,1,0,0,0,204,205,5,126,0,0,205,64,1,0,0,0,206,207,5,42,
-        0,0,207,66,1,0,0,0,208,209,5,60,0,0,209,68,1,0,0,0,210,211,5,62,
-        0,0,211,70,1,0,0,0,212,213,2,65,90,0,213,72,1,0,0,0,214,215,2,97,
-        122,0,215,74,1,0,0,0,216,219,3,77,38,0,217,219,7,1,0,0,218,216,1,
-        0,0,0,218,217,1,0,0,0,219,76,1,0,0,0,220,221,2,48,57,0,221,78,1,
-        0,0,0,222,223,2,48,51,0,223,80,1,0,0,0,224,225,2,48,49,0,225,82,
+        5,1,5,1,6,3,6,113,8,6,1,6,1,6,1,7,1,7,1,8,1,8,1,9,1,9,1,9,1,9,1,
+        9,1,9,1,9,1,9,1,9,1,9,1,9,1,10,1,10,1,10,1,10,1,10,1,11,1,11,1,11,
+        5,11,140,8,11,10,11,12,11,143,9,11,1,12,1,12,1,12,1,12,1,12,1,12,
+        1,12,1,12,1,12,1,12,3,12,155,8,12,1,13,1,13,1,13,5,13,160,8,13,10,
+        13,12,13,163,9,13,1,14,1,14,1,14,1,14,1,15,1,15,1,15,1,15,1,15,1,
+        15,1,16,1,16,1,17,1,17,1,18,1,18,1,19,1,19,1,20,1,20,1,21,1,21,1,
+        22,1,22,1,23,1,23,1,24,1,24,1,25,1,25,1,26,1,26,1,27,1,27,1,28,1,
+        28,1,29,1,29,1,30,1,30,1,31,1,31,1,32,1,32,1,33,1,33,1,34,1,34,1,
+        35,1,35,1,36,1,36,1,37,1,37,3,37,219,8,37,1,38,1,38,1,39,1,39,1,
+        40,1,40,1,41,1,41,3,41,229,8,41,1,42,1,42,3,42,233,8,42,0,0,43,1,
+        1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,10,21,11,23,12,25,13,27,
+        14,29,15,31,16,33,17,35,18,37,19,39,20,41,21,43,22,45,23,47,24,49,
+        25,51,26,53,27,55,28,57,29,59,30,61,31,63,32,65,33,67,34,69,35,71,
+        0,73,0,75,0,77,0,79,0,81,0,83,0,85,0,1,0,2,10,0,33,33,36,36,38,38,
+        44,44,59,59,61,61,63,63,91,94,96,96,123,125,6,0,65,72,74,78,80,90,
+        97,105,107,107,109,122,234,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,
+        7,1,0,0,0,0,9,1,0,0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,
+        1,0,0,0,0,19,1,0,0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,
+        1,0,0,0,0,29,1,0,0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,
+        1,0,0,0,0,39,1,0,0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,
+        1,0,0,0,0,49,1,0,0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,
+        1,0,0,0,0,59,1,0,0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,
+        1,0,0,0,0,69,1,0,0,0,1,87,1,0,0,0,3,89,1,0,0,0,5,91,1,0,0,0,7,94,
+        1,0,0,0,9,97,1,0,0,0,11,105,1,0,0,0,13,112,1,0,0,0,15,116,1,0,0,
+        0,17,118,1,0,0,0,19,120,1,0,0,0,21,131,1,0,0,0,23,136,1,0,0,0,25,
+        144,1,0,0,0,27,156,1,0,0,0,29,164,1,0,0,0,31,168,1,0,0,0,33,174,
+        1,0,0,0,35,176,1,0,0,0,37,178,1,0,0,0,39,180,1,0,0,0,41,182,1,0,
+        0,0,43,184,1,0,0,0,45,186,1,0,0,0,47,188,1,0,0,0,49,190,1,0,0,0,
+        51,192,1,0,0,0,53,194,1,0,0,0,55,196,1,0,0,0,57,198,1,0,0,0,59,200,
+        1,0,0,0,61,202,1,0,0,0,63,204,1,0,0,0,65,206,1,0,0,0,67,208,1,0,
+        0,0,69,210,1,0,0,0,71,212,1,0,0,0,73,214,1,0,0,0,75,218,1,0,0,0,
+        77,220,1,0,0,0,79,222,1,0,0,0,81,224,1,0,0,0,83,228,1,0,0,0,85,232,
+        1,0,0,0,87,88,5,91,0,0,88,2,1,0,0,0,89,90,5,93,0,0,90,4,1,0,0,0,
+        91,92,5,91,0,0,92,93,5,91,0,0,93,6,1,0,0,0,94,95,5,93,0,0,95,96,
+        5,93,0,0,96,8,1,0,0,0,97,98,5,61,0,0,98,99,5,61,0,0,99,100,5,61,
+        0,0,100,101,5,61,0,0,101,102,5,61,0,0,102,103,5,61,0,0,103,104,5,
+        61,0,0,104,10,1,0,0,0,105,106,5,42,0,0,106,107,5,42,0,0,107,108,
+        5,42,0,0,108,109,5,42,0,0,109,110,5,42,0,0,110,12,1,0,0,0,111,113,
+        5,13,0,0,112,111,1,0,0,0,112,113,1,0,0,0,113,114,1,0,0,0,114,115,
+        5,10,0,0,115,14,1,0,0,0,116,117,5,111,0,0,117,16,1,0,0,0,118,119,
+        5,120,0,0,119,18,1,0,0,0,120,121,5,50,0,0,121,122,3,77,38,0,122,
+        123,3,77,38,0,123,124,3,77,38,0,124,125,3,35,17,0,125,126,3,81,40,
+        0,126,127,3,77,38,0,127,128,3,35,17,0,128,129,3,79,39,0,129,130,
+        3,77,38,0,130,20,1,0,0,0,131,132,2,48,50,0,132,133,3,77,38,0,133,
+        134,2,48,53,0,134,135,3,77,38,0,135,22,1,0,0,0,136,141,3,85,42,0,
+        137,140,3,85,42,0,138,140,3,41,20,0,139,137,1,0,0,0,139,138,1,0,
+        0,0,140,143,1,0,0,0,141,139,1,0,0,0,141,142,1,0,0,0,142,24,1,0,0,
+        0,143,141,1,0,0,0,144,145,3,77,38,0,145,146,3,77,38,0,146,147,3,
+        81,40,0,147,148,3,77,38,0,148,149,3,79,39,0,149,150,3,77,38,0,150,
+        151,3,51,25,0,151,152,3,75,37,0,152,154,3,75,37,0,153,155,3,75,37,
+        0,154,153,1,0,0,0,154,155,1,0,0,0,155,26,1,0,0,0,156,161,3,77,38,
+        0,157,160,3,85,42,0,158,160,3,41,20,0,159,157,1,0,0,0,159,158,1,
+        0,0,0,160,163,1,0,0,0,161,159,1,0,0,0,161,162,1,0,0,0,162,28,1,0,
+        0,0,163,161,1,0,0,0,164,165,5,32,0,0,165,166,5,32,0,0,166,167,5,
+        45,0,0,167,30,1,0,0,0,168,169,5,32,0,0,169,170,5,32,0,0,170,171,
+        5,32,0,0,171,172,5,32,0,0,172,173,5,45,0,0,173,32,1,0,0,0,174,175,
+        7,0,0,0,175,34,1,0,0,0,176,177,5,45,0,0,177,36,1,0,0,0,178,179,5,
+        46,0,0,179,38,1,0,0,0,180,181,5,47,0,0,181,40,1,0,0,0,182,183,5,
+        95,0,0,183,42,1,0,0,0,184,185,5,58,0,0,185,44,1,0,0,0,186,187,5,
+        32,0,0,187,46,1,0,0,0,188,189,5,40,0,0,189,48,1,0,0,0,190,191,5,
+        41,0,0,191,50,1,0,0,0,192,193,5,35,0,0,193,52,1,0,0,0,194,195,5,
+        64,0,0,195,54,1,0,0,0,196,197,5,43,0,0,197,56,1,0,0,0,198,199,5,
+        37,0,0,199,58,1,0,0,0,200,201,5,39,0,0,201,60,1,0,0,0,202,203,5,
+        34,0,0,203,62,1,0,0,0,204,205,5,126,0,0,205,64,1,0,0,0,206,207,5,
+        42,0,0,207,66,1,0,0,0,208,209,5,60,0,0,209,68,1,0,0,0,210,211,5,
+        62,0,0,211,70,1,0,0,0,212,213,2,65,90,0,213,72,1,0,0,0,214,215,2,
+        97,122,0,215,74,1,0,0,0,216,219,3,77,38,0,217,219,7,1,0,0,218,216,
+        1,0,0,0,218,217,1,0,0,0,219,76,1,0,0,0,220,221,2,48,57,0,221,78,
+        1,0,0,0,222,223,2,48,51,0,223,80,1,0,0,0,224,225,2,48,49,0,225,82,
         1,0,0,0,226,229,3,71,35,0,227,229,3,73,36,0,228,226,1,0,0,0,228,
         227,1,0,0,0,229,84,1,0,0,0,230,233,3,83,41,0,231,233,3,77,38,0,232,
-        230,1,0,0,0,232,231,1,0,0,0,233,86,1,0,0,0,10,0,112,123,125,154,
+        230,1,0,0,0,232,231,1,0,0,0,233,86,1,0,0,0,10,0,112,139,141,154,
         159,161,218,228,232,0
     ]
 
 class ZorgFileLexer(Lexer):
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
@@ -104,17 +104,17 @@
     T__2 = 3
     T__3 = 4
     T__4 = 5
     T__5 = 6
     NL = 7
     LOWER_O = 8
     LOWER_X = 9
-    ID = 10
-    DATE = 11
-    TIME = 12
+    DATE = 10
+    TIME = 11
+    ID = 12
     ZID = 13
     NUM_ID = 14
     TWO_SPACE_DASH = 15
     FOUR_SPACE_DASH = 16
     SYMBOL = 17
     DASH = 18
     DOT = 19
@@ -142,22 +142,22 @@
     literalNames = [ "<INVALID>",
             "'['", "']'", "'[['", "']]'", "'======='", "'*****'", "'o'", 
             "'x'", "'  -'", "'    -'", "'-'", "'.'", "'/'", "'_'", "':'", 
             "' '", "'('", "')'", "'#'", "'@'", "'+'", "'%'", "'''", "'\"'", 
             "'~'", "'*'", "'<'", "'>'" ]
 
     symbolicNames = [ "<INVALID>",
-            "NL", "LOWER_O", "LOWER_X", "ID", "DATE", "TIME", "ZID", "NUM_ID", 
+            "NL", "LOWER_O", "LOWER_X", "DATE", "TIME", "ID", "ZID", "NUM_ID", 
             "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", "DOT", 
             "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", "RPAREN", 
             "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", "DQUOTE", "TILDE", 
             "STAR", "LANGLE", "RANGLE" ]
 
     ruleNames = [ "T__0", "T__1", "T__2", "T__3", "T__4", "T__5", "NL", 
-                  "LOWER_O", "LOWER_X", "ID", "DATE", "TIME", "ZID", "NUM_ID", 
+                  "LOWER_O", "LOWER_X", "DATE", "TIME", "ID", "ZID", "NUM_ID", 
                   "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", 
                   "DOT", "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", 
                   "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", 
                   "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE", "UPPER_LETTER", 
                   "LOWER_LETTER", "ZID_CHAR", "NUM", "FIRST_D_NUM", "FIRST_M_NUM", 
                   "ALPHA", "ALPHANUM" ]
```

### Comparing `zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens` & `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 T__2=3
 T__3=4
 T__4=5
 T__5=6
 NL=7
 LOWER_O=8
 LOWER_X=9
-ID=10
-DATE=11
-TIME=12
+DATE=10
+TIME=11
+ID=12
 ZID=13
 NUM_ID=14
 TWO_SPACE_DASH=15
 FOUR_SPACE_DASH=16
 SYMBOL=17
 DASH=18
 DOT=19
```

### Comparing `zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileListener.py` & `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileListener.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from src/zorg/grammar/zorg_file/ZorgFile.g4 by ANTLR 4.13.1
+# Generated from ZorgFile.g4 by ANTLR 4.13.1
 from antlr4 import *
 if "." in __name__:
     from .ZorgFileParser import ZorgFileParser
 else:
     from ZorgFileParser import ZorgFileParser
 
 # This class defines a complete listener for a parse tree produced by ZorgFileParser.
@@ -31,14 +31,23 @@
         pass
 
     # Exit a parse tree produced by ZorgFileParser#comment.
     def exitComment(self, ctx:ZorgFileParser.CommentContext):
         pass
 
 
+    # Enter a parse tree produced by ZorgFileParser#body.
+    def enterBody(self, ctx:ZorgFileParser.BodyContext):
+        pass
+
+    # Exit a parse tree produced by ZorgFileParser#body.
+    def exitBody(self, ctx:ZorgFileParser.BodyContext):
+        pass
+
+
     # Enter a parse tree produced by ZorgFileParser#block.
     def enterBlock(self, ctx:ZorgFileParser.BlockContext):
         pass
 
     # Exit a parse tree produced by ZorgFileParser#block.
     def exitBlock(self, ctx:ZorgFileParser.BlockContext):
         pass
```

### Comparing `zettel_org-0.7.1/src/zorg/grammar/zorg_file/ZorgFileParser.py` & `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,191 +1,192 @@
-# Generated from src/zorg/grammar/zorg_file/ZorgFile.g4 by ANTLR 4.13.1
+# Generated from ZorgFile.g4 by ANTLR 4.13.1
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
-        4,1,35,470,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        4,1,35,473,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
         6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,13,7,13,
         2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,19,2,20,
         7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,26,7,26,
         2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,32,2,33,
         7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,39,7,39,
         2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,45,2,46,
-        7,46,1,0,1,0,4,0,97,8,0,11,0,12,0,98,1,0,5,0,102,8,0,10,0,12,0,105,
-        9,0,1,0,5,0,108,8,0,10,0,12,0,111,9,0,1,0,5,0,114,8,0,10,0,12,0,
-        117,9,0,3,0,119,8,0,1,0,1,0,1,1,4,1,124,8,1,11,1,12,1,125,1,2,1,
-        2,3,2,130,8,2,1,2,1,2,1,3,4,3,135,8,3,11,3,12,3,136,1,3,5,3,140,
-        8,3,10,3,12,3,143,9,3,1,4,1,4,1,4,1,4,3,4,149,8,4,1,5,1,5,1,5,1,
-        5,1,5,1,6,1,6,1,6,5,6,159,8,6,10,6,12,6,162,9,6,1,7,1,7,1,7,1,8,
-        1,8,3,8,169,8,8,1,8,1,8,1,9,1,9,1,9,4,9,176,8,9,11,9,12,9,177,1,
-        9,5,9,181,8,9,10,9,12,9,184,9,9,1,10,1,10,1,10,5,10,189,8,10,10,
-        10,12,10,192,9,10,1,11,1,11,1,11,1,12,1,12,5,12,199,8,12,10,12,12,
-        12,202,9,12,1,13,1,13,1,13,3,13,207,8,13,1,13,1,13,1,13,1,14,1,14,
-        1,14,1,14,3,14,216,8,14,1,15,1,15,1,15,3,15,221,8,15,1,16,1,16,1,
-        16,1,16,1,16,1,17,1,17,1,18,4,18,231,8,18,11,18,12,18,232,1,19,1,
-        19,1,19,3,19,238,8,19,1,19,1,19,5,19,242,8,19,10,19,12,19,245,9,
-        19,1,19,1,19,3,19,249,8,19,1,19,1,19,1,19,5,19,254,8,19,10,19,12,
-        19,257,9,19,3,19,259,8,19,1,19,3,19,262,8,19,1,20,1,20,1,20,1,20,
-        1,20,1,20,1,20,1,20,3,20,272,8,20,1,21,1,21,1,21,1,21,1,21,1,22,
-        1,22,4,22,281,8,22,11,22,12,22,282,1,22,1,22,5,22,287,8,22,10,22,
-        12,22,290,9,22,1,23,1,23,1,23,1,23,1,23,1,23,3,23,298,8,23,1,24,
-        1,24,1,25,1,25,1,26,1,26,1,26,1,26,1,26,3,26,309,8,26,1,27,1,27,
-        1,28,1,28,1,29,1,29,1,30,1,30,1,30,1,30,3,30,321,8,30,1,31,1,31,
-        1,31,1,32,1,32,1,32,1,33,1,33,1,33,1,34,1,34,1,34,1,35,1,35,1,35,
-        1,35,1,35,4,35,340,8,35,11,35,12,35,341,1,35,1,35,1,35,4,35,347,
-        8,35,11,35,12,35,348,1,35,1,35,3,35,353,8,35,1,36,1,36,1,36,1,36,
-        1,37,1,37,1,37,1,37,1,38,1,38,5,38,365,8,38,10,38,12,38,368,9,38,
-        1,38,5,38,371,8,38,10,38,12,38,374,9,38,1,38,3,38,377,8,38,1,38,
-        5,38,380,8,38,10,38,12,38,383,9,38,1,39,1,39,5,39,387,8,39,10,39,
-        12,39,390,9,39,1,39,5,39,393,8,39,10,39,12,39,396,9,39,1,39,3,39,
-        399,8,39,1,39,5,39,402,8,39,10,39,12,39,405,9,39,1,40,1,40,5,40,
-        409,8,40,10,40,12,40,412,9,40,1,40,5,40,415,8,40,10,40,12,40,418,
-        9,40,1,40,3,40,421,8,40,1,40,5,40,424,8,40,10,40,12,40,427,9,40,
-        1,41,1,41,5,41,431,8,41,10,41,12,41,434,9,41,1,41,5,41,437,8,41,
-        10,41,12,41,440,9,41,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,
-        1,42,1,42,1,42,1,43,1,43,1,43,1,43,1,44,1,44,1,44,1,44,1,45,1,45,
-        1,45,1,45,1,45,1,45,1,46,1,46,1,46,0,0,47,0,2,4,6,8,10,12,14,16,
-        18,20,22,24,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,58,60,
-        62,64,66,68,70,72,74,76,78,80,82,84,86,88,90,92,0,5,2,0,9,9,32,32,
-        4,0,17,17,21,21,24,25,32,35,2,0,18,20,22,22,1,0,26,29,1,1,7,7,496,
-        0,94,1,0,0,0,2,123,1,0,0,0,4,127,1,0,0,0,6,134,1,0,0,0,8,148,1,0,
-        0,0,10,150,1,0,0,0,12,155,1,0,0,0,14,163,1,0,0,0,16,168,1,0,0,0,
-        18,172,1,0,0,0,20,185,1,0,0,0,22,193,1,0,0,0,24,196,1,0,0,0,26,203,
-        1,0,0,0,28,215,1,0,0,0,30,217,1,0,0,0,32,222,1,0,0,0,34,227,1,0,
-        0,0,36,230,1,0,0,0,38,234,1,0,0,0,40,271,1,0,0,0,42,273,1,0,0,0,
-        44,278,1,0,0,0,46,297,1,0,0,0,48,299,1,0,0,0,50,301,1,0,0,0,52,308,
-        1,0,0,0,54,310,1,0,0,0,56,312,1,0,0,0,58,314,1,0,0,0,60,320,1,0,
-        0,0,62,322,1,0,0,0,64,325,1,0,0,0,66,328,1,0,0,0,68,331,1,0,0,0,
-        70,352,1,0,0,0,72,354,1,0,0,0,74,358,1,0,0,0,76,362,1,0,0,0,78,384,
-        1,0,0,0,80,406,1,0,0,0,82,428,1,0,0,0,84,441,1,0,0,0,86,453,1,0,
-        0,0,88,457,1,0,0,0,90,461,1,0,0,0,92,467,1,0,0,0,94,118,3,2,1,0,
-        95,97,5,7,0,0,96,95,1,0,0,0,97,98,1,0,0,0,98,96,1,0,0,0,98,99,1,
-        0,0,0,99,103,1,0,0,0,100,102,3,6,3,0,101,100,1,0,0,0,102,105,1,0,
-        0,0,103,101,1,0,0,0,103,104,1,0,0,0,104,109,1,0,0,0,105,103,1,0,
-        0,0,106,108,3,78,39,0,107,106,1,0,0,0,108,111,1,0,0,0,109,107,1,
-        0,0,0,109,110,1,0,0,0,110,115,1,0,0,0,111,109,1,0,0,0,112,114,3,
-        76,38,0,113,112,1,0,0,0,114,117,1,0,0,0,115,113,1,0,0,0,115,116,
-        1,0,0,0,116,119,1,0,0,0,117,115,1,0,0,0,118,96,1,0,0,0,118,119,1,
-        0,0,0,119,120,1,0,0,0,120,121,5,0,0,1,121,1,1,0,0,0,122,124,3,4,
-        2,0,123,122,1,0,0,0,124,125,1,0,0,0,125,123,1,0,0,0,125,126,1,0,
-        0,0,126,3,1,0,0,0,127,129,5,26,0,0,128,130,3,36,18,0,129,128,1,0,
-        0,0,129,130,1,0,0,0,130,131,1,0,0,0,131,132,5,7,0,0,132,5,1,0,0,
-        0,133,135,3,8,4,0,134,133,1,0,0,0,135,136,1,0,0,0,136,134,1,0,0,
-        0,136,137,1,0,0,0,137,141,1,0,0,0,138,140,5,7,0,0,139,138,1,0,0,
-        0,140,143,1,0,0,0,141,139,1,0,0,0,141,142,1,0,0,0,142,7,1,0,0,0,
-        143,141,1,0,0,0,144,149,3,24,12,0,145,149,3,12,6,0,146,149,3,10,
-        5,0,147,149,3,4,2,0,148,144,1,0,0,0,148,145,1,0,0,0,148,146,1,0,
-        0,0,148,147,1,0,0,0,149,9,1,0,0,0,150,151,3,74,37,0,151,152,5,22,
-        0,0,152,153,3,36,18,0,153,154,5,7,0,0,154,11,1,0,0,0,155,156,5,18,
-        0,0,156,160,3,14,7,0,157,159,3,20,10,0,158,157,1,0,0,0,159,162,1,
-        0,0,0,160,158,1,0,0,0,160,161,1,0,0,0,161,13,1,0,0,0,162,160,1,0,
-        0,0,163,164,3,16,8,0,164,165,5,7,0,0,165,15,1,0,0,0,166,167,5,23,
-        0,0,167,169,3,34,17,0,168,166,1,0,0,0,168,169,1,0,0,0,169,170,1,
-        0,0,0,170,171,3,18,9,0,171,17,1,0,0,0,172,182,3,36,18,0,173,175,
-        5,7,0,0,174,176,5,23,0,0,175,174,1,0,0,0,176,177,1,0,0,0,177,175,
-        1,0,0,0,177,178,1,0,0,0,178,179,1,0,0,0,179,181,3,36,18,0,180,173,
-        1,0,0,0,181,184,1,0,0,0,182,180,1,0,0,0,182,183,1,0,0,0,183,19,1,
-        0,0,0,184,182,1,0,0,0,185,186,5,15,0,0,186,190,3,14,7,0,187,189,
-        3,22,11,0,188,187,1,0,0,0,189,192,1,0,0,0,190,188,1,0,0,0,190,191,
-        1,0,0,0,191,21,1,0,0,0,192,190,1,0,0,0,193,194,5,16,0,0,194,195,
-        3,14,7,0,195,23,1,0,0,0,196,200,3,26,13,0,197,199,3,20,10,0,198,
-        197,1,0,0,0,199,202,1,0,0,0,200,198,1,0,0,0,200,201,1,0,0,0,201,
-        25,1,0,0,0,202,200,1,0,0,0,203,206,3,28,14,0,204,205,5,23,0,0,205,
-        207,3,32,16,0,206,204,1,0,0,0,206,207,1,0,0,0,207,208,1,0,0,0,208,
-        209,3,16,8,0,209,210,5,7,0,0,210,27,1,0,0,0,211,216,5,8,0,0,212,
-        216,3,30,15,0,213,216,5,34,0,0,214,216,5,35,0,0,215,211,1,0,0,0,
-        215,212,1,0,0,0,215,213,1,0,0,0,215,214,1,0,0,0,216,29,1,0,0,0,217,
-        220,7,0,0,0,218,219,5,22,0,0,219,221,3,50,25,0,220,218,1,0,0,0,220,
-        221,1,0,0,0,221,31,1,0,0,0,222,223,5,1,0,0,223,224,5,26,0,0,224,
-        225,5,10,0,0,225,226,5,2,0,0,226,33,1,0,0,0,227,228,5,13,0,0,228,
-        35,1,0,0,0,229,231,3,38,19,0,230,229,1,0,0,0,231,232,1,0,0,0,232,
-        230,1,0,0,0,232,233,1,0,0,0,233,37,1,0,0,0,234,237,5,23,0,0,235,
-        236,5,30,0,0,236,238,3,54,27,0,237,235,1,0,0,0,237,238,1,0,0,0,238,
-        243,1,0,0,0,239,242,3,54,27,0,240,242,5,31,0,0,241,239,1,0,0,0,241,
-        240,1,0,0,0,242,245,1,0,0,0,243,241,1,0,0,0,243,244,1,0,0,0,244,
-        248,1,0,0,0,245,243,1,0,0,0,246,249,3,40,20,0,247,249,3,70,35,0,
-        248,246,1,0,0,0,248,247,1,0,0,0,248,249,1,0,0,0,249,258,1,0,0,0,
-        250,255,3,52,26,0,251,254,3,52,26,0,252,254,3,46,23,0,253,251,1,
-        0,0,0,253,252,1,0,0,0,254,257,1,0,0,0,255,253,1,0,0,0,255,256,1,
-        0,0,0,256,259,1,0,0,0,257,255,1,0,0,0,258,250,1,0,0,0,258,259,1,
-        0,0,0,259,261,1,0,0,0,260,262,3,74,37,0,261,260,1,0,0,0,261,262,
-        1,0,0,0,262,39,1,0,0,0,263,272,3,58,29,0,264,272,3,60,30,0,265,272,
-        3,72,36,0,266,272,3,42,21,0,267,272,3,44,22,0,268,272,3,74,37,0,
-        269,272,3,34,17,0,270,272,3,32,16,0,271,263,1,0,0,0,271,264,1,0,
-        0,0,271,265,1,0,0,0,271,266,1,0,0,0,271,267,1,0,0,0,271,268,1,0,
-        0,0,271,269,1,0,0,0,271,270,1,0,0,0,272,41,1,0,0,0,273,274,5,10,
-        0,0,274,275,5,22,0,0,275,276,5,22,0,0,276,277,3,44,22,0,277,43,1,
-        0,0,0,278,288,3,46,23,0,279,281,3,56,28,0,280,279,1,0,0,0,281,282,
-        1,0,0,0,282,280,1,0,0,0,282,283,1,0,0,0,283,284,1,0,0,0,284,285,
-        3,46,23,0,285,287,1,0,0,0,286,280,1,0,0,0,287,290,1,0,0,0,288,286,
-        1,0,0,0,288,289,1,0,0,0,289,45,1,0,0,0,290,288,1,0,0,0,291,298,5,
-        10,0,0,292,298,5,14,0,0,293,298,3,48,24,0,294,298,3,50,25,0,295,
-        298,5,8,0,0,296,298,5,9,0,0,297,291,1,0,0,0,297,292,1,0,0,0,297,
-        293,1,0,0,0,297,294,1,0,0,0,297,295,1,0,0,0,297,296,1,0,0,0,298,
-        47,1,0,0,0,299,300,5,11,0,0,300,49,1,0,0,0,301,302,5,12,0,0,302,
-        51,1,0,0,0,303,309,5,30,0,0,304,309,5,31,0,0,305,309,3,54,27,0,306,
-        309,3,58,29,0,307,309,3,56,28,0,308,303,1,0,0,0,308,304,1,0,0,0,
-        308,305,1,0,0,0,308,306,1,0,0,0,308,307,1,0,0,0,309,53,1,0,0,0,310,
-        311,7,1,0,0,311,55,1,0,0,0,312,313,7,2,0,0,313,57,1,0,0,0,314,315,
-        7,3,0,0,315,59,1,0,0,0,316,321,3,62,31,0,317,321,3,64,32,0,318,321,
-        3,66,33,0,319,321,3,68,34,0,320,316,1,0,0,0,320,317,1,0,0,0,320,
-        318,1,0,0,0,320,319,1,0,0,0,321,61,1,0,0,0,322,323,5,26,0,0,323,
-        324,5,10,0,0,324,63,1,0,0,0,325,326,5,27,0,0,326,327,5,10,0,0,327,
-        65,1,0,0,0,328,329,5,29,0,0,329,330,5,10,0,0,330,67,1,0,0,0,331,
-        332,5,28,0,0,332,333,5,10,0,0,333,69,1,0,0,0,334,339,5,30,0,0,335,
-        340,3,40,20,0,336,340,3,32,16,0,337,340,5,3,0,0,338,340,5,4,0,0,
-        339,335,1,0,0,0,339,336,1,0,0,0,339,337,1,0,0,0,339,338,1,0,0,0,
-        340,341,1,0,0,0,341,339,1,0,0,0,341,342,1,0,0,0,342,343,1,0,0,0,
-        343,353,5,30,0,0,344,346,5,31,0,0,345,347,3,40,20,0,346,345,1,0,
-        0,0,347,348,1,0,0,0,348,346,1,0,0,0,348,349,1,0,0,0,349,350,1,0,
-        0,0,350,351,5,31,0,0,351,353,1,0,0,0,352,334,1,0,0,0,352,344,1,0,
-        0,0,353,71,1,0,0,0,354,355,5,3,0,0,355,356,3,44,22,0,356,357,5,4,
-        0,0,357,73,1,0,0,0,358,359,5,1,0,0,359,360,3,44,22,0,360,361,5,2,
-        0,0,361,75,1,0,0,0,362,366,3,84,42,0,363,365,5,7,0,0,364,363,1,0,
-        0,0,365,368,1,0,0,0,366,364,1,0,0,0,366,367,1,0,0,0,367,372,1,0,
-        0,0,368,366,1,0,0,0,369,371,3,6,3,0,370,369,1,0,0,0,371,374,1,0,
-        0,0,372,370,1,0,0,0,372,373,1,0,0,0,373,381,1,0,0,0,374,372,1,0,
-        0,0,375,377,5,7,0,0,376,375,1,0,0,0,376,377,1,0,0,0,377,378,1,0,
-        0,0,378,380,3,78,39,0,379,376,1,0,0,0,380,383,1,0,0,0,381,379,1,
-        0,0,0,381,382,1,0,0,0,382,77,1,0,0,0,383,381,1,0,0,0,384,388,3,86,
-        43,0,385,387,5,7,0,0,386,385,1,0,0,0,387,390,1,0,0,0,388,386,1,0,
-        0,0,388,389,1,0,0,0,389,394,1,0,0,0,390,388,1,0,0,0,391,393,3,6,
-        3,0,392,391,1,0,0,0,393,396,1,0,0,0,394,392,1,0,0,0,394,395,1,0,
-        0,0,395,403,1,0,0,0,396,394,1,0,0,0,397,399,5,7,0,0,398,397,1,0,
-        0,0,398,399,1,0,0,0,399,400,1,0,0,0,400,402,3,80,40,0,401,398,1,
-        0,0,0,402,405,1,0,0,0,403,401,1,0,0,0,403,404,1,0,0,0,404,79,1,0,
-        0,0,405,403,1,0,0,0,406,410,3,88,44,0,407,409,5,7,0,0,408,407,1,
-        0,0,0,409,412,1,0,0,0,410,408,1,0,0,0,410,411,1,0,0,0,411,416,1,
-        0,0,0,412,410,1,0,0,0,413,415,3,6,3,0,414,413,1,0,0,0,415,418,1,
-        0,0,0,416,414,1,0,0,0,416,417,1,0,0,0,417,425,1,0,0,0,418,416,1,
-        0,0,0,419,421,5,7,0,0,420,419,1,0,0,0,420,421,1,0,0,0,421,422,1,
-        0,0,0,422,424,3,82,41,0,423,420,1,0,0,0,424,427,1,0,0,0,425,423,
-        1,0,0,0,425,426,1,0,0,0,426,81,1,0,0,0,427,425,1,0,0,0,428,432,3,
-        90,45,0,429,431,5,7,0,0,430,429,1,0,0,0,431,434,1,0,0,0,432,430,
-        1,0,0,0,432,433,1,0,0,0,433,438,1,0,0,0,434,432,1,0,0,0,435,437,
-        3,6,3,0,436,435,1,0,0,0,437,440,1,0,0,0,438,436,1,0,0,0,438,439,
-        1,0,0,0,439,83,1,0,0,0,440,438,1,0,0,0,441,442,5,26,0,0,442,443,
-        5,26,0,0,443,444,5,26,0,0,444,445,5,26,0,0,445,446,5,26,0,0,446,
-        447,5,26,0,0,447,448,5,26,0,0,448,449,5,26,0,0,449,450,5,26,0,0,
-        450,451,3,36,18,0,451,452,3,92,46,0,452,85,1,0,0,0,453,454,5,5,0,
-        0,454,455,3,36,18,0,455,456,3,92,46,0,456,87,1,0,0,0,457,458,5,6,
-        0,0,458,459,3,36,18,0,459,460,3,92,46,0,460,89,1,0,0,0,461,462,5,
-        18,0,0,462,463,5,18,0,0,463,464,5,18,0,0,464,465,3,36,18,0,465,466,
-        3,92,46,0,466,91,1,0,0,0,467,468,7,4,0,0,468,93,1,0,0,0,52,98,103,
-        109,115,118,125,129,136,141,148,160,168,177,182,190,200,206,215,
-        220,232,237,241,243,248,253,255,258,261,271,282,288,297,308,320,
-        339,341,348,352,366,372,376,381,388,394,398,403,410,416,420,425,
-        432,438
+        7,46,2,47,7,47,1,0,1,0,3,0,99,8,0,1,0,1,0,1,1,4,1,104,8,1,11,1,12,
+        1,105,1,2,1,2,3,2,110,8,2,1,2,1,2,1,3,4,3,115,8,3,11,3,12,3,116,
+        1,3,5,3,120,8,3,10,3,12,3,123,9,3,1,3,5,3,126,8,3,10,3,12,3,129,
+        9,3,1,3,5,3,132,8,3,10,3,12,3,135,9,3,1,4,4,4,138,8,4,11,4,12,4,
+        139,1,4,5,4,143,8,4,10,4,12,4,146,9,4,1,5,1,5,1,5,1,5,3,5,152,8,
+        5,1,6,1,6,1,6,1,6,1,6,1,7,1,7,1,7,5,7,162,8,7,10,7,12,7,165,9,7,
+        1,8,1,8,1,8,1,9,1,9,3,9,172,8,9,1,9,1,9,1,10,1,10,1,10,4,10,179,
+        8,10,11,10,12,10,180,1,10,5,10,184,8,10,10,10,12,10,187,9,10,1,11,
+        1,11,1,11,5,11,192,8,11,10,11,12,11,195,9,11,1,12,1,12,1,12,1,13,
+        1,13,5,13,202,8,13,10,13,12,13,205,9,13,1,14,1,14,1,14,3,14,210,
+        8,14,1,14,1,14,1,14,1,15,1,15,1,15,1,15,3,15,219,8,15,1,16,1,16,
+        1,16,3,16,224,8,16,1,17,1,17,1,17,1,17,1,17,1,18,1,18,1,19,4,19,
+        234,8,19,11,19,12,19,235,1,20,1,20,1,20,3,20,241,8,20,1,20,1,20,
+        5,20,245,8,20,10,20,12,20,248,9,20,1,20,1,20,3,20,252,8,20,1,20,
+        1,20,1,20,5,20,257,8,20,10,20,12,20,260,9,20,3,20,262,8,20,1,20,
+        3,20,265,8,20,1,21,1,21,1,21,1,21,1,21,1,21,1,21,1,21,3,21,275,8,
+        21,1,22,1,22,1,22,1,22,1,22,1,23,1,23,4,23,284,8,23,11,23,12,23,
+        285,1,23,1,23,5,23,290,8,23,10,23,12,23,293,9,23,1,24,1,24,1,24,
+        1,24,1,24,1,24,3,24,301,8,24,1,25,1,25,1,26,1,26,1,27,1,27,1,27,
+        1,27,1,27,3,27,312,8,27,1,28,1,28,1,29,1,29,1,30,1,30,1,31,1,31,
+        1,31,1,31,3,31,324,8,31,1,32,1,32,1,32,1,33,1,33,1,33,1,34,1,34,
+        1,34,1,35,1,35,1,35,1,36,1,36,1,36,1,36,1,36,4,36,343,8,36,11,36,
+        12,36,344,1,36,1,36,1,36,4,36,350,8,36,11,36,12,36,351,1,36,1,36,
+        3,36,356,8,36,1,37,1,37,1,37,1,37,1,38,1,38,1,38,1,38,1,39,1,39,
+        5,39,368,8,39,10,39,12,39,371,9,39,1,39,5,39,374,8,39,10,39,12,39,
+        377,9,39,1,39,3,39,380,8,39,1,39,5,39,383,8,39,10,39,12,39,386,9,
+        39,1,40,1,40,5,40,390,8,40,10,40,12,40,393,9,40,1,40,5,40,396,8,
+        40,10,40,12,40,399,9,40,1,40,3,40,402,8,40,1,40,5,40,405,8,40,10,
+        40,12,40,408,9,40,1,41,1,41,5,41,412,8,41,10,41,12,41,415,9,41,1,
+        41,5,41,418,8,41,10,41,12,41,421,9,41,1,41,3,41,424,8,41,1,41,5,
+        41,427,8,41,10,41,12,41,430,9,41,1,42,1,42,5,42,434,8,42,10,42,12,
+        42,437,9,42,1,42,5,42,440,8,42,10,42,12,42,443,9,42,1,43,1,43,1,
+        43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,44,1,44,1,44,1,
+        44,1,45,1,45,1,45,1,45,1,46,1,46,1,46,1,46,1,46,1,46,1,47,1,47,1,
+        47,0,0,48,0,2,4,6,8,10,12,14,16,18,20,22,24,26,28,30,32,34,36,38,
+        40,42,44,46,48,50,52,54,56,58,60,62,64,66,68,70,72,74,76,78,80,82,
+        84,86,88,90,92,94,0,5,2,0,9,9,32,32,4,0,17,17,21,21,24,25,32,35,
+        2,0,18,20,22,22,1,0,26,29,1,1,7,7,498,0,96,1,0,0,0,2,103,1,0,0,0,
+        4,107,1,0,0,0,6,114,1,0,0,0,8,137,1,0,0,0,10,151,1,0,0,0,12,153,
+        1,0,0,0,14,158,1,0,0,0,16,166,1,0,0,0,18,171,1,0,0,0,20,175,1,0,
+        0,0,22,188,1,0,0,0,24,196,1,0,0,0,26,199,1,0,0,0,28,206,1,0,0,0,
+        30,218,1,0,0,0,32,220,1,0,0,0,34,225,1,0,0,0,36,230,1,0,0,0,38,233,
+        1,0,0,0,40,237,1,0,0,0,42,274,1,0,0,0,44,276,1,0,0,0,46,281,1,0,
+        0,0,48,300,1,0,0,0,50,302,1,0,0,0,52,304,1,0,0,0,54,311,1,0,0,0,
+        56,313,1,0,0,0,58,315,1,0,0,0,60,317,1,0,0,0,62,323,1,0,0,0,64,325,
+        1,0,0,0,66,328,1,0,0,0,68,331,1,0,0,0,70,334,1,0,0,0,72,355,1,0,
+        0,0,74,357,1,0,0,0,76,361,1,0,0,0,78,365,1,0,0,0,80,387,1,0,0,0,
+        82,409,1,0,0,0,84,431,1,0,0,0,86,444,1,0,0,0,88,456,1,0,0,0,90,460,
+        1,0,0,0,92,464,1,0,0,0,94,470,1,0,0,0,96,98,3,2,1,0,97,99,3,6,3,
+        0,98,97,1,0,0,0,98,99,1,0,0,0,99,100,1,0,0,0,100,101,5,0,0,1,101,
+        1,1,0,0,0,102,104,3,4,2,0,103,102,1,0,0,0,104,105,1,0,0,0,105,103,
+        1,0,0,0,105,106,1,0,0,0,106,3,1,0,0,0,107,109,5,26,0,0,108,110,3,
+        38,19,0,109,108,1,0,0,0,109,110,1,0,0,0,110,111,1,0,0,0,111,112,
+        5,7,0,0,112,5,1,0,0,0,113,115,5,7,0,0,114,113,1,0,0,0,115,116,1,
+        0,0,0,116,114,1,0,0,0,116,117,1,0,0,0,117,121,1,0,0,0,118,120,3,
+        8,4,0,119,118,1,0,0,0,120,123,1,0,0,0,121,119,1,0,0,0,121,122,1,
+        0,0,0,122,127,1,0,0,0,123,121,1,0,0,0,124,126,3,80,40,0,125,124,
+        1,0,0,0,126,129,1,0,0,0,127,125,1,0,0,0,127,128,1,0,0,0,128,133,
+        1,0,0,0,129,127,1,0,0,0,130,132,3,78,39,0,131,130,1,0,0,0,132,135,
+        1,0,0,0,133,131,1,0,0,0,133,134,1,0,0,0,134,7,1,0,0,0,135,133,1,
+        0,0,0,136,138,3,10,5,0,137,136,1,0,0,0,138,139,1,0,0,0,139,137,1,
+        0,0,0,139,140,1,0,0,0,140,144,1,0,0,0,141,143,5,7,0,0,142,141,1,
+        0,0,0,143,146,1,0,0,0,144,142,1,0,0,0,144,145,1,0,0,0,145,9,1,0,
+        0,0,146,144,1,0,0,0,147,152,3,26,13,0,148,152,3,14,7,0,149,152,3,
+        12,6,0,150,152,3,4,2,0,151,147,1,0,0,0,151,148,1,0,0,0,151,149,1,
+        0,0,0,151,150,1,0,0,0,152,11,1,0,0,0,153,154,3,76,38,0,154,155,5,
+        22,0,0,155,156,3,38,19,0,156,157,5,7,0,0,157,13,1,0,0,0,158,159,
+        5,18,0,0,159,163,3,16,8,0,160,162,3,22,11,0,161,160,1,0,0,0,162,
+        165,1,0,0,0,163,161,1,0,0,0,163,164,1,0,0,0,164,15,1,0,0,0,165,163,
+        1,0,0,0,166,167,3,18,9,0,167,168,5,7,0,0,168,17,1,0,0,0,169,170,
+        5,23,0,0,170,172,3,36,18,0,171,169,1,0,0,0,171,172,1,0,0,0,172,173,
+        1,0,0,0,173,174,3,20,10,0,174,19,1,0,0,0,175,185,3,38,19,0,176,178,
+        5,7,0,0,177,179,5,23,0,0,178,177,1,0,0,0,179,180,1,0,0,0,180,178,
+        1,0,0,0,180,181,1,0,0,0,181,182,1,0,0,0,182,184,3,38,19,0,183,176,
+        1,0,0,0,184,187,1,0,0,0,185,183,1,0,0,0,185,186,1,0,0,0,186,21,1,
+        0,0,0,187,185,1,0,0,0,188,189,5,15,0,0,189,193,3,16,8,0,190,192,
+        3,24,12,0,191,190,1,0,0,0,192,195,1,0,0,0,193,191,1,0,0,0,193,194,
+        1,0,0,0,194,23,1,0,0,0,195,193,1,0,0,0,196,197,5,16,0,0,197,198,
+        3,16,8,0,198,25,1,0,0,0,199,203,3,28,14,0,200,202,3,22,11,0,201,
+        200,1,0,0,0,202,205,1,0,0,0,203,201,1,0,0,0,203,204,1,0,0,0,204,
+        27,1,0,0,0,205,203,1,0,0,0,206,209,3,30,15,0,207,208,5,23,0,0,208,
+        210,3,34,17,0,209,207,1,0,0,0,209,210,1,0,0,0,210,211,1,0,0,0,211,
+        212,3,18,9,0,212,213,5,7,0,0,213,29,1,0,0,0,214,219,5,8,0,0,215,
+        219,3,32,16,0,216,219,5,34,0,0,217,219,5,35,0,0,218,214,1,0,0,0,
+        218,215,1,0,0,0,218,216,1,0,0,0,218,217,1,0,0,0,219,31,1,0,0,0,220,
+        223,7,0,0,0,221,222,5,22,0,0,222,224,3,52,26,0,223,221,1,0,0,0,223,
+        224,1,0,0,0,224,33,1,0,0,0,225,226,5,1,0,0,226,227,5,26,0,0,227,
+        228,5,12,0,0,228,229,5,2,0,0,229,35,1,0,0,0,230,231,5,13,0,0,231,
+        37,1,0,0,0,232,234,3,40,20,0,233,232,1,0,0,0,234,235,1,0,0,0,235,
+        233,1,0,0,0,235,236,1,0,0,0,236,39,1,0,0,0,237,240,5,23,0,0,238,
+        239,5,30,0,0,239,241,3,56,28,0,240,238,1,0,0,0,240,241,1,0,0,0,241,
+        246,1,0,0,0,242,245,3,56,28,0,243,245,5,31,0,0,244,242,1,0,0,0,244,
+        243,1,0,0,0,245,248,1,0,0,0,246,244,1,0,0,0,246,247,1,0,0,0,247,
+        251,1,0,0,0,248,246,1,0,0,0,249,252,3,42,21,0,250,252,3,72,36,0,
+        251,249,1,0,0,0,251,250,1,0,0,0,251,252,1,0,0,0,252,261,1,0,0,0,
+        253,258,3,54,27,0,254,257,3,54,27,0,255,257,3,48,24,0,256,254,1,
+        0,0,0,256,255,1,0,0,0,257,260,1,0,0,0,258,256,1,0,0,0,258,259,1,
+        0,0,0,259,262,1,0,0,0,260,258,1,0,0,0,261,253,1,0,0,0,261,262,1,
+        0,0,0,262,264,1,0,0,0,263,265,3,76,38,0,264,263,1,0,0,0,264,265,
+        1,0,0,0,265,41,1,0,0,0,266,275,3,60,30,0,267,275,3,62,31,0,268,275,
+        3,74,37,0,269,275,3,44,22,0,270,275,3,46,23,0,271,275,3,76,38,0,
+        272,275,3,36,18,0,273,275,3,34,17,0,274,266,1,0,0,0,274,267,1,0,
+        0,0,274,268,1,0,0,0,274,269,1,0,0,0,274,270,1,0,0,0,274,271,1,0,
+        0,0,274,272,1,0,0,0,274,273,1,0,0,0,275,43,1,0,0,0,276,277,5,12,
+        0,0,277,278,5,22,0,0,278,279,5,22,0,0,279,280,3,46,23,0,280,45,1,
+        0,0,0,281,291,3,48,24,0,282,284,3,58,29,0,283,282,1,0,0,0,284,285,
+        1,0,0,0,285,283,1,0,0,0,285,286,1,0,0,0,286,287,1,0,0,0,287,288,
+        3,48,24,0,288,290,1,0,0,0,289,283,1,0,0,0,290,293,1,0,0,0,291,289,
+        1,0,0,0,291,292,1,0,0,0,292,47,1,0,0,0,293,291,1,0,0,0,294,301,5,
+        12,0,0,295,301,5,14,0,0,296,301,3,50,25,0,297,301,3,52,26,0,298,
+        301,5,8,0,0,299,301,5,9,0,0,300,294,1,0,0,0,300,295,1,0,0,0,300,
+        296,1,0,0,0,300,297,1,0,0,0,300,298,1,0,0,0,300,299,1,0,0,0,301,
+        49,1,0,0,0,302,303,5,10,0,0,303,51,1,0,0,0,304,305,5,11,0,0,305,
+        53,1,0,0,0,306,312,5,30,0,0,307,312,5,31,0,0,308,312,3,56,28,0,309,
+        312,3,60,30,0,310,312,3,58,29,0,311,306,1,0,0,0,311,307,1,0,0,0,
+        311,308,1,0,0,0,311,309,1,0,0,0,311,310,1,0,0,0,312,55,1,0,0,0,313,
+        314,7,1,0,0,314,57,1,0,0,0,315,316,7,2,0,0,316,59,1,0,0,0,317,318,
+        7,3,0,0,318,61,1,0,0,0,319,324,3,64,32,0,320,324,3,66,33,0,321,324,
+        3,68,34,0,322,324,3,70,35,0,323,319,1,0,0,0,323,320,1,0,0,0,323,
+        321,1,0,0,0,323,322,1,0,0,0,324,63,1,0,0,0,325,326,5,26,0,0,326,
+        327,5,12,0,0,327,65,1,0,0,0,328,329,5,27,0,0,329,330,5,12,0,0,330,
+        67,1,0,0,0,331,332,5,29,0,0,332,333,5,12,0,0,333,69,1,0,0,0,334,
+        335,5,28,0,0,335,336,5,12,0,0,336,71,1,0,0,0,337,342,5,30,0,0,338,
+        343,3,42,21,0,339,343,3,34,17,0,340,343,5,3,0,0,341,343,5,4,0,0,
+        342,338,1,0,0,0,342,339,1,0,0,0,342,340,1,0,0,0,342,341,1,0,0,0,
+        343,344,1,0,0,0,344,342,1,0,0,0,344,345,1,0,0,0,345,346,1,0,0,0,
+        346,356,5,30,0,0,347,349,5,31,0,0,348,350,3,42,21,0,349,348,1,0,
+        0,0,350,351,1,0,0,0,351,349,1,0,0,0,351,352,1,0,0,0,352,353,1,0,
+        0,0,353,354,5,31,0,0,354,356,1,0,0,0,355,337,1,0,0,0,355,347,1,0,
+        0,0,356,73,1,0,0,0,357,358,5,3,0,0,358,359,3,46,23,0,359,360,5,4,
+        0,0,360,75,1,0,0,0,361,362,5,1,0,0,362,363,3,46,23,0,363,364,5,2,
+        0,0,364,77,1,0,0,0,365,369,3,86,43,0,366,368,5,7,0,0,367,366,1,0,
+        0,0,368,371,1,0,0,0,369,367,1,0,0,0,369,370,1,0,0,0,370,375,1,0,
+        0,0,371,369,1,0,0,0,372,374,3,8,4,0,373,372,1,0,0,0,374,377,1,0,
+        0,0,375,373,1,0,0,0,375,376,1,0,0,0,376,384,1,0,0,0,377,375,1,0,
+        0,0,378,380,5,7,0,0,379,378,1,0,0,0,379,380,1,0,0,0,380,381,1,0,
+        0,0,381,383,3,80,40,0,382,379,1,0,0,0,383,386,1,0,0,0,384,382,1,
+        0,0,0,384,385,1,0,0,0,385,79,1,0,0,0,386,384,1,0,0,0,387,391,3,88,
+        44,0,388,390,5,7,0,0,389,388,1,0,0,0,390,393,1,0,0,0,391,389,1,0,
+        0,0,391,392,1,0,0,0,392,397,1,0,0,0,393,391,1,0,0,0,394,396,3,8,
+        4,0,395,394,1,0,0,0,396,399,1,0,0,0,397,395,1,0,0,0,397,398,1,0,
+        0,0,398,406,1,0,0,0,399,397,1,0,0,0,400,402,5,7,0,0,401,400,1,0,
+        0,0,401,402,1,0,0,0,402,403,1,0,0,0,403,405,3,82,41,0,404,401,1,
+        0,0,0,405,408,1,0,0,0,406,404,1,0,0,0,406,407,1,0,0,0,407,81,1,0,
+        0,0,408,406,1,0,0,0,409,413,3,90,45,0,410,412,5,7,0,0,411,410,1,
+        0,0,0,412,415,1,0,0,0,413,411,1,0,0,0,413,414,1,0,0,0,414,419,1,
+        0,0,0,415,413,1,0,0,0,416,418,3,8,4,0,417,416,1,0,0,0,418,421,1,
+        0,0,0,419,417,1,0,0,0,419,420,1,0,0,0,420,428,1,0,0,0,421,419,1,
+        0,0,0,422,424,5,7,0,0,423,422,1,0,0,0,423,424,1,0,0,0,424,425,1,
+        0,0,0,425,427,3,84,42,0,426,423,1,0,0,0,427,430,1,0,0,0,428,426,
+        1,0,0,0,428,429,1,0,0,0,429,83,1,0,0,0,430,428,1,0,0,0,431,435,3,
+        92,46,0,432,434,5,7,0,0,433,432,1,0,0,0,434,437,1,0,0,0,435,433,
+        1,0,0,0,435,436,1,0,0,0,436,441,1,0,0,0,437,435,1,0,0,0,438,440,
+        3,8,4,0,439,438,1,0,0,0,440,443,1,0,0,0,441,439,1,0,0,0,441,442,
+        1,0,0,0,442,85,1,0,0,0,443,441,1,0,0,0,444,445,5,26,0,0,445,446,
+        5,26,0,0,446,447,5,26,0,0,447,448,5,26,0,0,448,449,5,26,0,0,449,
+        450,5,26,0,0,450,451,5,26,0,0,451,452,5,26,0,0,452,453,5,26,0,0,
+        453,454,3,38,19,0,454,455,3,94,47,0,455,87,1,0,0,0,456,457,5,5,0,
+        0,457,458,3,38,19,0,458,459,3,94,47,0,459,89,1,0,0,0,460,461,5,6,
+        0,0,461,462,3,38,19,0,462,463,3,94,47,0,463,91,1,0,0,0,464,465,5,
+        18,0,0,465,466,5,18,0,0,466,467,5,18,0,0,467,468,3,38,19,0,468,469,
+        3,94,47,0,469,93,1,0,0,0,470,471,7,4,0,0,471,95,1,0,0,0,52,98,105,
+        109,116,121,127,133,139,144,151,163,171,180,185,193,203,209,218,
+        223,235,240,244,246,251,256,258,261,264,274,285,291,300,311,323,
+        342,344,351,355,369,375,379,384,391,397,401,406,413,419,423,428,
+        435,441
     ]
 
 class ZorgFileParser ( Parser ):
 
     grammarFileName = "ZorgFile.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
@@ -199,69 +200,70 @@
                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                      "'  -'", "'    -'", "<INVALID>", "'-'", "'.'", "'/'", 
                      "'_'", "':'", "' '", "'('", "')'", "'#'", "'@'", "'+'", 
                      "'%'", "'''", "'\"'", "'~'", "'*'", "'<'", "'>'" ]
 
     symbolicNames = [ "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "NL", "LOWER_O", 
-                      "LOWER_X", "ID", "DATE", "TIME", "ZID", "NUM_ID", 
+                      "LOWER_X", "DATE", "TIME", "ID", "ZID", "NUM_ID", 
                       "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", 
                       "DOT", "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", 
                       "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", 
                       "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE" ]
 
     RULE_prog = 0
     RULE_head = 1
     RULE_comment = 2
-    RULE_block = 3
-    RULE_item = 4
-    RULE_footnote = 5
-    RULE_note = 6
-    RULE_base_note = 7
-    RULE_id_note_body = 8
-    RULE_note_body = 9
-    RULE_subnote = 10
-    RULE_subsubnote = 11
-    RULE_todo = 12
-    RULE_base_todo = 13
-    RULE_todo_prefix = 14
-    RULE_x_or_tilde = 15
-    RULE_priority = 16
-    RULE_zid = 17
-    RULE_space_atoms = 18
-    RULE_space_atom = 19
-    RULE_atom = 20
-    RULE_property = 21
-    RULE_id_group = 22
-    RULE_id = 23
-    RULE_date = 24
-    RULE_time = 25
-    RULE_any_symbol = 26
-    RULE_non_tag_symbol = 27
-    RULE_id_symbol = 28
-    RULE_tag_symbol = 29
-    RULE_tag = 30
-    RULE_area = 31
-    RULE_context = 32
-    RULE_person = 33
-    RULE_project = 34
-    RULE_quoted = 35
-    RULE_link = 36
-    RULE_ref = 37
-    RULE_h1_section = 38
-    RULE_h2_section = 39
-    RULE_h3_section = 40
-    RULE_h4_section = 41
-    RULE_h1_header = 42
-    RULE_h2_header = 43
-    RULE_h3_header = 44
-    RULE_h4_header = 45
-    RULE_eol = 46
+    RULE_body = 3
+    RULE_block = 4
+    RULE_item = 5
+    RULE_footnote = 6
+    RULE_note = 7
+    RULE_base_note = 8
+    RULE_id_note_body = 9
+    RULE_note_body = 10
+    RULE_subnote = 11
+    RULE_subsubnote = 12
+    RULE_todo = 13
+    RULE_base_todo = 14
+    RULE_todo_prefix = 15
+    RULE_x_or_tilde = 16
+    RULE_priority = 17
+    RULE_zid = 18
+    RULE_space_atoms = 19
+    RULE_space_atom = 20
+    RULE_atom = 21
+    RULE_property = 22
+    RULE_id_group = 23
+    RULE_id = 24
+    RULE_date = 25
+    RULE_time = 26
+    RULE_any_symbol = 27
+    RULE_non_tag_symbol = 28
+    RULE_id_symbol = 29
+    RULE_tag_symbol = 30
+    RULE_tag = 31
+    RULE_area = 32
+    RULE_context = 33
+    RULE_person = 34
+    RULE_project = 35
+    RULE_quoted = 36
+    RULE_link = 37
+    RULE_ref = 38
+    RULE_h1_section = 39
+    RULE_h2_section = 40
+    RULE_h3_section = 41
+    RULE_h4_section = 42
+    RULE_h1_header = 43
+    RULE_h2_header = 44
+    RULE_h3_header = 45
+    RULE_h4_header = 46
+    RULE_eol = 47
 
-    ruleNames =  [ "prog", "head", "comment", "block", "item", "footnote", 
+    ruleNames =  [ "prog", "head", "comment", "body", "block", "item", "footnote", 
                    "note", "base_note", "id_note_body", "note_body", "subnote", 
                    "subsubnote", "todo", "base_todo", "todo_prefix", "x_or_tilde", 
                    "priority", "zid", "space_atoms", "space_atom", "atom", 
                    "property", "id_group", "id", "date", "time", "any_symbol", 
                    "non_tag_symbol", "id_symbol", "tag_symbol", "tag", "area", 
                    "context", "person", "project", "quoted", "link", "ref", 
                    "h1_section", "h2_section", "h3_section", "h4_section", 
@@ -273,17 +275,17 @@
     T__2=3
     T__3=4
     T__4=5
     T__5=6
     NL=7
     LOWER_O=8
     LOWER_X=9
-    ID=10
-    DATE=11
-    TIME=12
+    DATE=10
+    TIME=11
+    ID=12
     ZID=13
     NUM_ID=14
     TWO_SPACE_DASH=15
     FOUR_SPACE_DASH=16
     SYMBOL=17
     DASH=18
     DOT=19
@@ -323,39 +325,16 @@
         def head(self):
             return self.getTypedRuleContext(ZorgFileParser.HeadContext,0)
 
 
         def EOF(self):
             return self.getToken(ZorgFileParser.EOF, 0)
 
-        def NL(self, i:int=None):
-            if i is None:
-                return self.getTokens(ZorgFileParser.NL)
-            else:
-                return self.getToken(ZorgFileParser.NL, i)
-
-        def block(self, i:int=None):
-            if i is None:
-                return self.getTypedRuleContexts(ZorgFileParser.BlockContext)
-            else:
-                return self.getTypedRuleContext(ZorgFileParser.BlockContext,i)
-
-
-        def h2_section(self, i:int=None):
-            if i is None:
-                return self.getTypedRuleContexts(ZorgFileParser.H2_sectionContext)
-            else:
-                return self.getTypedRuleContext(ZorgFileParser.H2_sectionContext,i)
-
-
-        def h1_section(self, i:int=None):
-            if i is None:
-                return self.getTypedRuleContexts(ZorgFileParser.H1_sectionContext)
-            else:
-                return self.getTypedRuleContext(ZorgFileParser.H1_sectionContext,i)
+        def body(self):
+            return self.getTypedRuleContext(ZorgFileParser.BodyContext,0)
 
 
         def getRuleIndex(self):
             return ZorgFileParser.RULE_prog
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterProg" ):
@@ -371,66 +350,25 @@
     def prog(self):
 
         localctx = ZorgFileParser.ProgContext(self, self._ctx, self.state)
         self.enterRule(localctx, 0, self.RULE_prog)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 94
+            self.state = 96
             self.head()
-            self.state = 118
+            self.state = 98
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==7:
-                self.state = 96 
-                self._errHandler.sync(self)
-                _la = self._input.LA(1)
-                while True:
-                    self.state = 95
-                    self.match(ZorgFileParser.NL)
-                    self.state = 98 
-                    self._errHandler.sync(self)
-                    _la = self._input.LA(1)
-                    if not (_la==7):
-                        break
+                self.state = 97
+                self.body()
 
-                self.state = 103
-                self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,1,self._ctx)
-                while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
-                    if _alt==1:
-                        self.state = 100
-                        self.block() 
-                    self.state = 105
-                    self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,1,self._ctx)
 
-                self.state = 109
-                self._errHandler.sync(self)
-                _la = self._input.LA(1)
-                while _la==5:
-                    self.state = 106
-                    self.h2_section()
-                    self.state = 111
-                    self._errHandler.sync(self)
-                    _la = self._input.LA(1)
-
-                self.state = 115
-                self._errHandler.sync(self)
-                _la = self._input.LA(1)
-                while _la==26:
-                    self.state = 112
-                    self.h1_section()
-                    self.state = 117
-                    self._errHandler.sync(self)
-                    _la = self._input.LA(1)
-
-
-
-            self.state = 120
+            self.state = 100
             self.match(ZorgFileParser.EOF)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -468,21 +406,21 @@
     def head(self):
 
         localctx = ZorgFileParser.HeadContext(self, self._ctx, self.state)
         self.enterRule(localctx, 2, self.RULE_head)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 123 
+            self.state = 103 
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while True:
-                self.state = 122
+                self.state = 102
                 self.comment()
-                self.state = 125 
+                self.state = 105 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if not (_la==26):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
@@ -527,35 +465,142 @@
     def comment(self):
 
         localctx = ZorgFileParser.CommentContext(self, self._ctx, self.state)
         self.enterRule(localctx, 4, self.RULE_comment)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 127
+            self.state = 107
             self.match(ZorgFileParser.HASH)
-            self.state = 129
+            self.state = 109
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==23:
-                self.state = 128
+                self.state = 108
                 self.space_atoms()
 
 
-            self.state = 131
+            self.state = 111
             self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
+    class BodyContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def NL(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgFileParser.NL)
+            else:
+                return self.getToken(ZorgFileParser.NL, i)
+
+        def block(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(ZorgFileParser.BlockContext)
+            else:
+                return self.getTypedRuleContext(ZorgFileParser.BlockContext,i)
+
+
+        def h2_section(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(ZorgFileParser.H2_sectionContext)
+            else:
+                return self.getTypedRuleContext(ZorgFileParser.H2_sectionContext,i)
+
+
+        def h1_section(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(ZorgFileParser.H1_sectionContext)
+            else:
+                return self.getTypedRuleContext(ZorgFileParser.H1_sectionContext,i)
+
+
+        def getRuleIndex(self):
+            return ZorgFileParser.RULE_body
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterBody" ):
+                listener.enterBody(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitBody" ):
+                listener.exitBody(self)
+
+
+
+
+    def body(self):
+
+        localctx = ZorgFileParser.BodyContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 6, self.RULE_body)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 114 
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            while True:
+                self.state = 113
+                self.match(ZorgFileParser.NL)
+                self.state = 116 
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+                if not (_la==7):
+                    break
+
+            self.state = 121
+            self._errHandler.sync(self)
+            _alt = self._interp.adaptivePredict(self._input,4,self._ctx)
+            while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
+                if _alt==1:
+                    self.state = 118
+                    self.block() 
+                self.state = 123
+                self._errHandler.sync(self)
+                _alt = self._interp.adaptivePredict(self._input,4,self._ctx)
+
+            self.state = 127
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            while _la==5:
+                self.state = 124
+                self.h2_section()
+                self.state = 129
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+
+            self.state = 133
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            while _la==26:
+                self.state = 130
+                self.h1_section()
+                self.state = 135
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
     class BlockContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
@@ -585,39 +630,39 @@
 
 
 
 
     def block(self):
 
         localctx = ZorgFileParser.BlockContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 6, self.RULE_block)
+        self.enterRule(localctx, 8, self.RULE_block)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 134 
+            self.state = 137 
             self._errHandler.sync(self)
             _alt = 1
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt == 1:
-                    self.state = 133
+                    self.state = 136
                     self.item()
 
                 else:
                     raise NoViableAltException(self)
-                self.state = 136 
+                self.state = 139 
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,7,self._ctx)
 
-            self.state = 141
+            self.state = 144
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,8,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 138
+                    self.state = 141
                     self.match(ZorgFileParser.NL) 
-                self.state = 143
+                self.state = 146
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,8,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -662,37 +707,37 @@
 
 
 
 
     def item(self):
 
         localctx = ZorgFileParser.ItemContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 8, self.RULE_item)
+        self.enterRule(localctx, 10, self.RULE_item)
         try:
-            self.state = 148
+            self.state = 151
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [8, 9, 32, 34, 35]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 144
+                self.state = 147
                 self.todo()
                 pass
             elif token in [18]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 145
+                self.state = 148
                 self.note()
                 pass
             elif token in [1]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 146
+                self.state = 149
                 self.footnote()
                 pass
             elif token in [26]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 147
+                self.state = 150
                 self.comment()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -737,24 +782,24 @@
 
 
 
 
     def footnote(self):
 
         localctx = ZorgFileParser.FootnoteContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 10, self.RULE_footnote)
+        self.enterRule(localctx, 12, self.RULE_footnote)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 150
+            self.state = 153
             self.ref()
-            self.state = 151
+            self.state = 154
             self.match(ZorgFileParser.COLON)
-            self.state = 152
+            self.state = 155
             self.space_atoms()
-            self.state = 153
+            self.state = 156
             self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -795,29 +840,29 @@
 
 
 
 
     def note(self):
 
         localctx = ZorgFileParser.NoteContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 12, self.RULE_note)
+        self.enterRule(localctx, 14, self.RULE_note)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 155
+            self.state = 158
             self.match(ZorgFileParser.DASH)
-            self.state = 156
+            self.state = 159
             self.base_note()
-            self.state = 160
+            self.state = 163
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==15:
-                self.state = 157
+                self.state = 160
                 self.subnote()
-                self.state = 162
+                self.state = 165
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -853,20 +898,20 @@
 
 
 
 
     def base_note(self):
 
         localctx = ZorgFileParser.Base_noteContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 14, self.RULE_base_note)
+        self.enterRule(localctx, 16, self.RULE_base_note)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 163
+            self.state = 166
             self.id_note_body()
-            self.state = 164
+            self.state = 167
             self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -904,28 +949,28 @@
 
 
 
 
     def id_note_body(self):
 
         localctx = ZorgFileParser.Id_note_bodyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 16, self.RULE_id_note_body)
+        self.enterRule(localctx, 18, self.RULE_id_note_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 168
+            self.state = 171
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,11,self._ctx)
             if la_ == 1:
-                self.state = 166
+                self.state = 169
                 self.match(ZorgFileParser.SPACE)
-                self.state = 167
+                self.state = 170
                 self.zid()
 
 
-            self.state = 170
+            self.state = 173
             self.note_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -971,43 +1016,43 @@
 
 
 
 
     def note_body(self):
 
         localctx = ZorgFileParser.Note_bodyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 18, self.RULE_note_body)
+        self.enterRule(localctx, 20, self.RULE_note_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 172
+            self.state = 175
             self.space_atoms()
-            self.state = 182
+            self.state = 185
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,13,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 173
+                    self.state = 176
                     self.match(ZorgFileParser.NL)
-                    self.state = 175 
+                    self.state = 178 
                     self._errHandler.sync(self)
                     _alt = 1
                     while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                         if _alt == 1:
-                            self.state = 174
+                            self.state = 177
                             self.match(ZorgFileParser.SPACE)
 
                         else:
                             raise NoViableAltException(self)
-                        self.state = 177 
+                        self.state = 180 
                         self._errHandler.sync(self)
                         _alt = self._interp.adaptivePredict(self._input,12,self._ctx)
 
-                    self.state = 179
+                    self.state = 182
                     self.space_atoms() 
-                self.state = 184
+                self.state = 187
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,13,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1050,29 +1095,29 @@
 
 
 
 
     def subnote(self):
 
         localctx = ZorgFileParser.SubnoteContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 20, self.RULE_subnote)
+        self.enterRule(localctx, 22, self.RULE_subnote)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 185
+            self.state = 188
             self.match(ZorgFileParser.TWO_SPACE_DASH)
-            self.state = 186
+            self.state = 189
             self.base_note()
-            self.state = 190
+            self.state = 193
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==16:
-                self.state = 187
+                self.state = 190
                 self.subsubnote()
-                self.state = 192
+                self.state = 195
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1108,20 +1153,20 @@
 
 
 
 
     def subsubnote(self):
 
         localctx = ZorgFileParser.SubsubnoteContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 22, self.RULE_subsubnote)
+        self.enterRule(localctx, 24, self.RULE_subsubnote)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 193
+            self.state = 196
             self.match(ZorgFileParser.FOUR_SPACE_DASH)
-            self.state = 194
+            self.state = 197
             self.base_note()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1159,27 +1204,27 @@
 
 
 
 
     def todo(self):
 
         localctx = ZorgFileParser.TodoContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 24, self.RULE_todo)
+        self.enterRule(localctx, 26, self.RULE_todo)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 196
+            self.state = 199
             self.base_todo()
-            self.state = 200
+            self.state = 203
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==15:
-                self.state = 197
+                self.state = 200
                 self.subnote()
-                self.state = 202
+                self.state = 205
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1226,32 +1271,32 @@
 
 
 
 
     def base_todo(self):
 
         localctx = ZorgFileParser.Base_todoContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 26, self.RULE_base_todo)
+        self.enterRule(localctx, 28, self.RULE_base_todo)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 203
-            self.todo_prefix()
             self.state = 206
+            self.todo_prefix()
+            self.state = 209
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,16,self._ctx)
             if la_ == 1:
-                self.state = 204
+                self.state = 207
                 self.match(ZorgFileParser.SPACE)
-                self.state = 205
+                self.state = 208
                 self.priority()
 
 
-            self.state = 208
+            self.state = 211
             self.id_note_body()
-            self.state = 209
+            self.state = 212
             self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1291,34 +1336,34 @@
 
 
 
 
     def todo_prefix(self):
 
         localctx = ZorgFileParser.Todo_prefixContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 28, self.RULE_todo_prefix)
+        self.enterRule(localctx, 30, self.RULE_todo_prefix)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 215
+            self.state = 218
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [8]:
-                self.state = 211
+                self.state = 214
                 self.match(ZorgFileParser.LOWER_O)
                 pass
             elif token in [9, 32]:
-                self.state = 212
+                self.state = 215
                 self.x_or_tilde()
                 pass
             elif token in [34]:
-                self.state = 213
+                self.state = 216
                 self.match(ZorgFileParser.LANGLE)
                 pass
             elif token in [35]:
-                self.state = 214
+                self.state = 217
                 self.match(ZorgFileParser.RANGLE)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -1362,32 +1407,32 @@
 
 
 
 
     def x_or_tilde(self):
 
         localctx = ZorgFileParser.X_or_tildeContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 30, self.RULE_x_or_tilde)
+        self.enterRule(localctx, 32, self.RULE_x_or_tilde)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 217
+            self.state = 220
             _la = self._input.LA(1)
             if not(_la==9 or _la==32):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
-            self.state = 220
+            self.state = 223
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==22:
-                self.state = 218
+                self.state = 221
                 self.match(ZorgFileParser.COLON)
-                self.state = 219
+                self.state = 222
                 self.time()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1422,24 +1467,24 @@
 
 
 
 
     def priority(self):
 
         localctx = ZorgFileParser.PriorityContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 32, self.RULE_priority)
+        self.enterRule(localctx, 34, self.RULE_priority)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 222
+            self.state = 225
             self.match(ZorgFileParser.T__0)
-            self.state = 223
+            self.state = 226
             self.match(ZorgFileParser.HASH)
-            self.state = 224
+            self.state = 227
             self.match(ZorgFileParser.ID)
-            self.state = 225
+            self.state = 228
             self.match(ZorgFileParser.T__1)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1469,18 +1514,18 @@
 
 
 
 
     def zid(self):
 
         localctx = ZorgFileParser.ZidContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 34, self.RULE_zid)
+        self.enterRule(localctx, 36, self.RULE_zid)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 227
+            self.state = 230
             self.match(ZorgFileParser.ZID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1514,25 +1559,25 @@
 
 
 
 
     def space_atoms(self):
 
         localctx = ZorgFileParser.Space_atomsContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 36, self.RULE_space_atoms)
+        self.enterRule(localctx, 38, self.RULE_space_atoms)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 230 
+            self.state = 233 
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while True:
-                self.state = 229
+                self.state = 232
                 self.space_atom()
-                self.state = 232 
+                self.state = 235 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if not (_la==23):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
@@ -1608,100 +1653,100 @@
 
 
 
 
     def space_atom(self):
 
         localctx = ZorgFileParser.Space_atomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 38, self.RULE_space_atom)
+        self.enterRule(localctx, 40, self.RULE_space_atom)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 234
-            self.match(ZorgFileParser.SPACE)
             self.state = 237
+            self.match(ZorgFileParser.SPACE)
+            self.state = 240
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,20,self._ctx)
             if la_ == 1:
-                self.state = 235
+                self.state = 238
                 self.match(ZorgFileParser.SQUOTE)
-                self.state = 236
+                self.state = 239
                 self.non_tag_symbol()
 
 
-            self.state = 243
+            self.state = 246
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,22,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 241
+                    self.state = 244
                     self._errHandler.sync(self)
                     token = self._input.LA(1)
                     if token in [17, 21, 24, 25, 32, 33, 34, 35]:
-                        self.state = 239
+                        self.state = 242
                         self.non_tag_symbol()
                         pass
                     elif token in [31]:
-                        self.state = 240
+                        self.state = 243
                         self.match(ZorgFileParser.DQUOTE)
                         pass
                     else:
                         raise NoViableAltException(self)
              
-                self.state = 245
+                self.state = 248
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,22,self._ctx)
 
-            self.state = 248
+            self.state = 251
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,23,self._ctx)
             if la_ == 1:
-                self.state = 246
+                self.state = 249
                 self.atom()
 
             elif la_ == 2:
-                self.state = 247
+                self.state = 250
                 self.quoted()
 
 
-            self.state = 258
+            self.state = 261
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (((_la) & ~0x3f) == 0 and ((1 << _la) & 68710957056) != 0):
-                self.state = 250
+                self.state = 253
                 self.any_symbol()
-                self.state = 255
+                self.state = 258
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while (((_la) & ~0x3f) == 0 and ((1 << _la) & 68710981376) != 0):
-                    self.state = 253
+                    self.state = 256
                     self._errHandler.sync(self)
                     token = self._input.LA(1)
                     if token in [17, 18, 19, 20, 21, 22, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35]:
-                        self.state = 251
+                        self.state = 254
                         self.any_symbol()
                         pass
                     elif token in [8, 9, 10, 11, 12, 14]:
-                        self.state = 252
+                        self.state = 255
                         self.id_()
                         pass
                     else:
                         raise NoViableAltException(self)
 
-                    self.state = 257
+                    self.state = 260
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
 
 
-            self.state = 261
+            self.state = 264
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==1:
-                self.state = 260
+                self.state = 263
                 self.ref()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1762,64 +1807,64 @@
 
 
 
 
     def atom(self):
 
         localctx = ZorgFileParser.AtomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 40, self.RULE_atom)
+        self.enterRule(localctx, 42, self.RULE_atom)
         try:
-            self.state = 271
+            self.state = 274
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,28,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 263
+                self.state = 266
                 self.tag_symbol()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 264
+                self.state = 267
                 self.tag()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 265
+                self.state = 268
                 self.link()
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 266
+                self.state = 269
                 self.property_()
                 pass
 
             elif la_ == 5:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 267
+                self.state = 270
                 self.id_group()
                 pass
 
             elif la_ == 6:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 268
+                self.state = 271
                 self.ref()
                 pass
 
             elif la_ == 7:
                 self.enterOuterAlt(localctx, 7)
-                self.state = 269
+                self.state = 272
                 self.zid()
                 pass
 
             elif la_ == 8:
                 self.enterOuterAlt(localctx, 8)
-                self.state = 270
+                self.state = 273
                 self.priority()
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -1862,24 +1907,24 @@
 
 
 
 
     def property_(self):
 
         localctx = ZorgFileParser.PropertyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 42, self.RULE_property)
+        self.enterRule(localctx, 44, self.RULE_property)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 273
+            self.state = 276
             self.match(ZorgFileParser.ID)
-            self.state = 274
+            self.state = 277
             self.match(ZorgFileParser.COLON)
-            self.state = 275
+            self.state = 278
             self.match(ZorgFileParser.COLON)
-            self.state = 276
+            self.state = 279
             self.id_group()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1920,40 +1965,40 @@
 
 
 
 
     def id_group(self):
 
         localctx = ZorgFileParser.Id_groupContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 44, self.RULE_id_group)
+        self.enterRule(localctx, 46, self.RULE_id_group)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 278
+            self.state = 281
             self.id_()
-            self.state = 288
+            self.state = 291
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,30,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 280 
+                    self.state = 283 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     while True:
-                        self.state = 279
+                        self.state = 282
                         self.id_symbol()
-                        self.state = 282 
+                        self.state = 285 
                         self._errHandler.sync(self)
                         _la = self._input.LA(1)
                         if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 6029312) != 0)):
                             break
 
-                    self.state = 284
+                    self.state = 287
                     self.id_() 
-                self.state = 290
+                self.state = 293
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,30,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -2002,47 +2047,47 @@
 
 
 
 
     def id_(self):
 
         localctx = ZorgFileParser.IdContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 46, self.RULE_id)
+        self.enterRule(localctx, 48, self.RULE_id)
         try:
-            self.state = 297
+            self.state = 300
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [10]:
+            if token in [12]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 291
+                self.state = 294
                 self.match(ZorgFileParser.ID)
                 pass
             elif token in [14]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 292
+                self.state = 295
                 self.match(ZorgFileParser.NUM_ID)
                 pass
-            elif token in [11]:
+            elif token in [10]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 293
+                self.state = 296
                 self.date()
                 pass
-            elif token in [12]:
+            elif token in [11]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 294
+                self.state = 297
                 self.time()
                 pass
             elif token in [8]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 295
+                self.state = 298
                 self.match(ZorgFileParser.LOWER_O)
                 pass
             elif token in [9]:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 296
+                self.state = 299
                 self.match(ZorgFileParser.LOWER_X)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2076,18 +2121,18 @@
 
 
 
 
     def date(self):
 
         localctx = ZorgFileParser.DateContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 48, self.RULE_date)
+        self.enterRule(localctx, 50, self.RULE_date)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 299
+            self.state = 302
             self.match(ZorgFileParser.DATE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2117,18 +2162,18 @@
 
 
 
 
     def time(self):
 
         localctx = ZorgFileParser.TimeContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 50, self.RULE_time)
+        self.enterRule(localctx, 52, self.RULE_time)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 301
+            self.state = 304
             self.match(ZorgFileParser.TIME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2173,42 +2218,42 @@
 
 
 
 
     def any_symbol(self):
 
         localctx = ZorgFileParser.Any_symbolContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 52, self.RULE_any_symbol)
+        self.enterRule(localctx, 54, self.RULE_any_symbol)
         try:
-            self.state = 308
+            self.state = 311
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [30]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 303
+                self.state = 306
                 self.match(ZorgFileParser.SQUOTE)
                 pass
             elif token in [31]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 304
+                self.state = 307
                 self.match(ZorgFileParser.DQUOTE)
                 pass
             elif token in [17, 21, 24, 25, 32, 33, 34, 35]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 305
+                self.state = 308
                 self.non_tag_symbol()
                 pass
             elif token in [26, 27, 28, 29]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 306
+                self.state = 309
                 self.tag_symbol()
                 pass
             elif token in [18, 19, 20, 22]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 307
+                self.state = 310
                 self.id_symbol()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2263,19 +2308,19 @@
 
 
 
 
     def non_tag_symbol(self):
 
         localctx = ZorgFileParser.Non_tag_symbolContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 54, self.RULE_non_tag_symbol)
+        self.enterRule(localctx, 56, self.RULE_non_tag_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 310
+            self.state = 313
             _la = self._input.LA(1)
             if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 64477069312) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
@@ -2319,19 +2364,19 @@
 
 
 
 
     def id_symbol(self):
 
         localctx = ZorgFileParser.Id_symbolContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 56, self.RULE_id_symbol)
+        self.enterRule(localctx, 58, self.RULE_id_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 312
+            self.state = 315
             _la = self._input.LA(1)
             if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 6029312) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
@@ -2375,19 +2420,19 @@
 
 
 
 
     def tag_symbol(self):
 
         localctx = ZorgFileParser.Tag_symbolContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 58, self.RULE_tag_symbol)
+        self.enterRule(localctx, 60, self.RULE_tag_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 314
+            self.state = 317
             _la = self._input.LA(1)
             if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006632960) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
@@ -2435,37 +2480,37 @@
 
 
 
 
     def tag(self):
 
         localctx = ZorgFileParser.TagContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 60, self.RULE_tag)
+        self.enterRule(localctx, 62, self.RULE_tag)
         try:
-            self.state = 320
+            self.state = 323
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [26]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 316
+                self.state = 319
                 self.area()
                 pass
             elif token in [27]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 317
+                self.state = 320
                 self.context()
                 pass
             elif token in [29]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 318
+                self.state = 321
                 self.person()
                 pass
             elif token in [28]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 319
+                self.state = 322
                 self.project()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2502,20 +2547,20 @@
 
 
 
 
     def area(self):
 
         localctx = ZorgFileParser.AreaContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 62, self.RULE_area)
+        self.enterRule(localctx, 64, self.RULE_area)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 322
+            self.state = 325
             self.match(ZorgFileParser.HASH)
-            self.state = 323
+            self.state = 326
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2548,20 +2593,20 @@
 
 
 
 
     def context(self):
 
         localctx = ZorgFileParser.ContextContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 64, self.RULE_context)
+        self.enterRule(localctx, 66, self.RULE_context)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 325
+            self.state = 328
             self.match(ZorgFileParser.AT_SIGN)
-            self.state = 326
+            self.state = 329
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2594,20 +2639,20 @@
 
 
 
 
     def person(self):
 
         localctx = ZorgFileParser.PersonContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 66, self.RULE_person)
+        self.enterRule(localctx, 68, self.RULE_person)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 328
+            self.state = 331
             self.match(ZorgFileParser.PERCENT)
-            self.state = 329
+            self.state = 332
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2640,20 +2685,20 @@
 
 
 
 
     def project(self):
 
         localctx = ZorgFileParser.ProjectContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 68, self.RULE_project)
+        self.enterRule(localctx, 70, self.RULE_project)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 331
+            self.state = 334
             self.match(ZorgFileParser.PLUS)
-            self.state = 332
+            self.state = 335
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2706,77 +2751,77 @@
 
 
 
 
     def quoted(self):
 
         localctx = ZorgFileParser.QuotedContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 70, self.RULE_quoted)
+        self.enterRule(localctx, 72, self.RULE_quoted)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 352
+            self.state = 355
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [30]:
-                self.state = 334
+                self.state = 337
                 self.match(ZorgFileParser.SQUOTE)
-                self.state = 339 
+                self.state = 342 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 339
+                    self.state = 342
                     self._errHandler.sync(self)
                     la_ = self._interp.adaptivePredict(self._input,34,self._ctx)
                     if la_ == 1:
-                        self.state = 335
+                        self.state = 338
                         self.atom()
                         pass
 
                     elif la_ == 2:
-                        self.state = 336
+                        self.state = 339
                         self.priority()
                         pass
 
                     elif la_ == 3:
-                        self.state = 337
+                        self.state = 340
                         self.match(ZorgFileParser.T__2)
                         pass
 
                     elif la_ == 4:
-                        self.state = 338
+                        self.state = 341
                         self.match(ZorgFileParser.T__3)
                         pass
 
 
-                    self.state = 341 
+                    self.state = 344 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006665498) != 0)):
                         break
 
-                self.state = 343
+                self.state = 346
                 self.match(ZorgFileParser.SQUOTE)
                 pass
             elif token in [31]:
-                self.state = 344
+                self.state = 347
                 self.match(ZorgFileParser.DQUOTE)
-                self.state = 346 
+                self.state = 349 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 345
+                    self.state = 348
                     self.atom()
-                    self.state = 348 
+                    self.state = 351 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006665482) != 0)):
                         break
 
-                self.state = 350
+                self.state = 353
                 self.match(ZorgFileParser.DQUOTE)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2811,22 +2856,22 @@
 
 
 
 
     def link(self):
 
         localctx = ZorgFileParser.LinkContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 72, self.RULE_link)
+        self.enterRule(localctx, 74, self.RULE_link)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 354
+            self.state = 357
             self.match(ZorgFileParser.T__2)
-            self.state = 355
+            self.state = 358
             self.id_group()
-            self.state = 356
+            self.state = 359
             self.match(ZorgFileParser.T__3)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2857,22 +2902,22 @@
 
 
 
 
     def ref(self):
 
         localctx = ZorgFileParser.RefContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 74, self.RULE_ref)
+        self.enterRule(localctx, 76, self.RULE_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 358
+            self.state = 361
             self.match(ZorgFileParser.T__0)
-            self.state = 359
+            self.state = 362
             self.id_group()
-            self.state = 360
+            self.state = 363
             self.match(ZorgFileParser.T__1)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2923,57 +2968,57 @@
 
 
 
 
     def h1_section(self):
 
         localctx = ZorgFileParser.H1_sectionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 76, self.RULE_h1_section)
+        self.enterRule(localctx, 78, self.RULE_h1_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 362
+            self.state = 365
             self.h1_header()
-            self.state = 366
+            self.state = 369
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 363
+                    self.state = 366
                     self.match(ZorgFileParser.NL) 
-                self.state = 368
+                self.state = 371
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
 
-            self.state = 372
+            self.state = 375
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 369
+                    self.state = 372
                     self.block() 
-                self.state = 374
+                self.state = 377
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
 
-            self.state = 381
+            self.state = 384
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==5 or _la==7:
-                self.state = 376
+                self.state = 379
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la==7:
-                    self.state = 375
+                    self.state = 378
                     self.match(ZorgFileParser.NL)
 
 
-                self.state = 378
+                self.state = 381
                 self.h2_section()
-                self.state = 383
+                self.state = 386
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3026,58 +3071,58 @@
 
 
 
 
     def h2_section(self):
 
         localctx = ZorgFileParser.H2_sectionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 78, self.RULE_h2_section)
+        self.enterRule(localctx, 80, self.RULE_h2_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 384
+            self.state = 387
             self.h2_header()
-            self.state = 388
+            self.state = 391
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 385
+                    self.state = 388
                     self.match(ZorgFileParser.NL) 
-                self.state = 390
+                self.state = 393
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
 
-            self.state = 394
+            self.state = 397
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 391
+                    self.state = 394
                     self.block() 
-                self.state = 396
+                self.state = 399
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
 
-            self.state = 403
+            self.state = 406
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 398
+                    self.state = 401
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 397
+                        self.state = 400
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 400
+                    self.state = 403
                     self.h3_section() 
-                self.state = 405
+                self.state = 408
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3130,58 +3175,58 @@
 
 
 
 
     def h3_section(self):
 
         localctx = ZorgFileParser.H3_sectionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 80, self.RULE_h3_section)
+        self.enterRule(localctx, 82, self.RULE_h3_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 406
+            self.state = 409
             self.h3_header()
-            self.state = 410
+            self.state = 413
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 407
+                    self.state = 410
                     self.match(ZorgFileParser.NL) 
-                self.state = 412
+                self.state = 415
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
 
-            self.state = 416
+            self.state = 419
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 413
+                    self.state = 416
                     self.block() 
-                self.state = 418
+                self.state = 421
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
 
-            self.state = 425
+            self.state = 428
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 420
+                    self.state = 423
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 419
+                        self.state = 422
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 422
+                    self.state = 425
                     self.h4_section() 
-                self.state = 427
+                self.state = 430
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3227,38 +3272,38 @@
 
 
 
 
     def h4_section(self):
 
         localctx = ZorgFileParser.H4_sectionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 82, self.RULE_h4_section)
+        self.enterRule(localctx, 84, self.RULE_h4_section)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 428
+            self.state = 431
             self.h4_header()
-            self.state = 432
+            self.state = 435
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 429
+                    self.state = 432
                     self.match(ZorgFileParser.NL) 
-                self.state = 434
+                self.state = 437
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
 
-            self.state = 438
+            self.state = 441
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 435
+                    self.state = 438
                     self.block() 
-                self.state = 440
+                self.state = 443
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3301,38 +3346,38 @@
 
 
 
 
     def h1_header(self):
 
         localctx = ZorgFileParser.H1_headerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 84, self.RULE_h1_header)
+        self.enterRule(localctx, 86, self.RULE_h1_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 441
-            self.match(ZorgFileParser.HASH)
-            self.state = 442
-            self.match(ZorgFileParser.HASH)
-            self.state = 443
-            self.match(ZorgFileParser.HASH)
             self.state = 444
             self.match(ZorgFileParser.HASH)
             self.state = 445
             self.match(ZorgFileParser.HASH)
             self.state = 446
             self.match(ZorgFileParser.HASH)
             self.state = 447
             self.match(ZorgFileParser.HASH)
             self.state = 448
             self.match(ZorgFileParser.HASH)
             self.state = 449
             self.match(ZorgFileParser.HASH)
             self.state = 450
-            self.space_atoms()
+            self.match(ZorgFileParser.HASH)
             self.state = 451
+            self.match(ZorgFileParser.HASH)
+            self.state = 452
+            self.match(ZorgFileParser.HASH)
+            self.state = 453
+            self.space_atoms()
+            self.state = 454
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3367,22 +3412,22 @@
 
 
 
 
     def h2_header(self):
 
         localctx = ZorgFileParser.H2_headerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 86, self.RULE_h2_header)
+        self.enterRule(localctx, 88, self.RULE_h2_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 453
+            self.state = 456
             self.match(ZorgFileParser.T__4)
-            self.state = 454
+            self.state = 457
             self.space_atoms()
-            self.state = 455
+            self.state = 458
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3417,22 +3462,22 @@
 
 
 
 
     def h3_header(self):
 
         localctx = ZorgFileParser.H3_headerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 88, self.RULE_h3_header)
+        self.enterRule(localctx, 90, self.RULE_h3_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 457
+            self.state = 460
             self.match(ZorgFileParser.T__5)
-            self.state = 458
+            self.state = 461
             self.space_atoms()
-            self.state = 459
+            self.state = 462
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3473,26 +3518,26 @@
 
 
 
 
     def h4_header(self):
 
         localctx = ZorgFileParser.H4_headerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 90, self.RULE_h4_header)
+        self.enterRule(localctx, 92, self.RULE_h4_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 461
+            self.state = 464
             self.match(ZorgFileParser.DASH)
-            self.state = 462
+            self.state = 465
             self.match(ZorgFileParser.DASH)
-            self.state = 463
+            self.state = 466
             self.match(ZorgFileParser.DASH)
-            self.state = 464
+            self.state = 467
             self.space_atoms()
-            self.state = 465
+            self.state = 468
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3525,19 +3570,19 @@
 
 
 
 
     def eol(self):
 
         localctx = ZorgFileParser.EolContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 92, self.RULE_eol)
+        self.enterRule(localctx, 94, self.RULE_eol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 467
+            self.state = 470
             _la = self._input.LA(1)
             if not(_la==-1 or _la==7):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
```

### Comparing `zettel_org-0.7.1/src/zorg/service/compiler/_api.py` & `zettel_org-0.7.2/src/zorg/service/compiler/_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """The public API for the zorg.service.compiler package."""
 
 from pathlib import Path
 
 import antlr4
 
-from ...domain.models import ZorgFile, ZorgQuery
+from ...domain.models import File, Query
 from ...grammar.zorg_file.ZorgFileLexer import ZorgFileLexer
 from ...grammar.zorg_file.ZorgFileParser import ZorgFileParser
 from ...grammar.zorg_query.ZorgQueryLexer import ZorgQueryLexer
 from ...grammar.zorg_query.ZorgQueryParser import ZorgQueryParser
 from ._file_compiler import ErrorManager, ZorgFileCompiler
 from ._query_compiler import ZorgQueryCompiler
 
 
 def walk_zorg_file(
     zdir: Path, zo_path_part: Path, verbose: bool = False
-) -> ZorgFile:
+) -> File:
     """Create a new ZorgFileCompiler and walk through notes in {zorg_file}."""
     zo_path = (
         zo_path_part if zo_path_part.is_absolute() else zdir / zo_path_part
     )
-    zorg_file = ZorgFile(zo_path)
+    zorg_file = File(zo_path)
     stream = antlr4.FileStream(zorg_file.path, errors="ignore")
     lexer = ZorgFileLexer(stream)
     tokens = antlr4.CommonTokenStream(lexer)
     parser = ZorgFileParser(tokens)
     if not verbose:
         parser.removeErrorListeners()
     error_manager = ErrorManager()
@@ -32,19 +32,19 @@
     tree = parser.prog()  # type: ignore[no-untyped-call]
     compiler = ZorgFileCompiler(zorg_file, error_manager)
     walker = antlr4.ParseTreeWalker()
     walker.walk(compiler, tree)
     return zorg_file
 
 
-def compile_zorg_query(query: str) -> ZorgQuery:
-    """Constructs a new ZorgQuery using {query}."""
+def build_zorg_query(query: str) -> Query:
+    """Constructs a new Query using {query}."""
     stream = antlr4.InputStream(query)
     lexer = ZorgQueryLexer(stream)
     tokens = antlr4.CommonTokenStream(lexer)
     parser = ZorgQueryParser(tokens)
     tree = parser.prog()  # type: ignore[no-untyped-call]
-    zorg_query = ZorgQuery()
+    zorg_query = Query()
     compiler = ZorgQueryCompiler(zorg_query)
     walker = antlr4.ParseTreeWalker()
     walker.walk(compiler, tree)
     return zorg_query
```

### Comparing `zettel_org-0.7.1/src/zorg/service/compiler/_file_compiler.py` & `zettel_org-0.7.2/src/zorg/service/compiler/_file_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from typing import Any, Literal, Optional
 
 import antlr4
 from antlr4.error.ErrorListener import ErrorListener
 from logrus import Logger
 from typist import assert_never
 
-from ...domain.models import TodoPayload, ZorgFile, ZorgNote
-from ...domain.types import NoteStatus, TodoPriorityType, TodoStatusPrefixChar
+from ...domain.models import File, Note, TodoPayload
+from ...domain.types import NoteType, TodoPriorityType, TodoStatusPrefixChar
 from ...grammar.zorg_file.ZorgFileListener import ZorgFileListener
 from ...grammar.zorg_file.ZorgFileParser import ZorgFileParser
 
 
 TagName = Literal["areas", "contexts", "people", "projects"]
 
 _LOGGER = Logger(__name__)
@@ -44,17 +44,15 @@
 class ZorgFileCompiler(ZorgFileListener):
     """Listener that compiles zorg files.
 
     This compiler takes as input a single *.zo file. When walked, it produces
     as output the {zorg_file} instance attribute.
     """
 
-    def __init__(
-        self, zorg_file: ZorgFile, error_manager: ErrorManager
-    ) -> None:
+    def __init__(self, zorg_file: File, error_manager: ErrorManager) -> None:
         self.zorg_file = zorg_file
         self.error_manager = error_manager
 
         self._s = _ZorgFileCompilerState()
 
     def enterArea(self, ctx: ZorgFileParser.AreaContext) -> None:  # noqa: D102
         self._add_tags(ctx, "areas")
@@ -191,27 +189,27 @@
         self._s.in_note = True
         self._s.parent_id = None
         del ctx
 
     def enterTodo_prefix(
         self, ctx: ZorgFileParser.Todo_prefixContext
     ) -> None:  # noqa: D102
-        status = NoteStatus.OPEN_TODO
+        status = NoteType.OPEN_TODO
         if self._s.in_note:
             ch: TodoStatusPrefixChar = ctx.getText()[0]
             if ch == "o":
-                status = NoteStatus.OPEN_TODO
+                status = NoteType.OPEN_TODO
             elif ch == "x":
-                status = NoteStatus.CLOSED_TODO
+                status = NoteType.CLOSED_TODO
             elif ch == "~":
-                status = NoteStatus.CANCELED_TODO
+                status = NoteType.CANCELED_TODO
             elif ch == "<":
-                status = NoteStatus.BLOCKED_TODO
+                status = NoteType.BLOCKED_TODO
             elif ch == ">":
-                status = NoteStatus.PARENT_TODO
+                status = NoteType.PARENT_TODO
             else:
                 assert_never(ch)
 
             self._s.todo_status = status
 
     def enterZid(self, ctx: ZorgFileParser.ZidContext) -> None:  # noqa: D102
         if self._s.in_note and self._s.ids_in_note == 0:
@@ -240,20 +238,20 @@
         elif self.error_manager.errors:
             _LOGGER.warning(
                 "Skipping note since zorg file has errors.",
                 file_path=str(self.zorg_file.path),
             )
             self.zorg_file.has_errors = True
         else:
-            todo = ZorgNote(id_note_body.getText(), **kwargs)
+            todo = Note(id_note_body.getText(), **kwargs)
             self.zorg_file.notes.append(todo)
 
         # Reset todo priority and status back to defaults.
         self._s.todo_priority = "C"
-        self._s.todo_status = NoteStatus.OPEN_TODO
+        self._s.todo_status = NoteType.OPEN_TODO
 
     def exitH1_header(
         self, ctx: ZorgFileParser.H1_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h1_header = False
 
@@ -337,15 +335,15 @@
             _LOGGER.warning(
                 "Skipping note since zorg file has errors.",
                 file_path=str(self.zorg_file.path),
             )
             self.zorg_file.has_errors = True
             return
 
-        note = ZorgNote(body, **kwargs)
+        note = Note(body, **kwargs)
         self.zorg_file.notes.append(note)
 
     def exitItem(self, ctx: ZorgFileParser.ItemContext) -> None:  # noqa: D102
         del ctx
         self._s.in_subnote = False
 
     def exitSubnote(
@@ -366,14 +364,15 @@
     ) -> dict[str, Any]:
         if extra_kwargs is None:
             extra_kwargs = {}
         kwargs: dict[str, Any] = {
             "areas": self._s.areas,
             "contexts": self._s.contexts,
             "create_date": self._s.create_date,
+            "file_path": self.zorg_file.path,
             "line_no": ctx.start.line,
             "links": self._s.note_links,
             "people": self._s.people,
             "projects": self._s.projects,
             "properties": self._s.properties,
             "zid": self._s.zid,
         }
@@ -471,15 +470,15 @@
     h1_date: Optional[dt.date] = None
     h2_date: Optional[dt.date] = None
     h3_date: Optional[dt.date] = None
     h4_date: Optional[dt.date] = None
     note_date: Optional[dt.date] = None
 
     todo_priority: TodoPriorityType = "C"
-    todo_status: NoteStatus = NoteStatus.OPEN_TODO
+    todo_status: NoteType = NoteType.OPEN_TODO
 
     @property
     def areas(self) -> list[str]:
         """Area tags that are currently in-scope."""
         return self._get_current_tags("areas")
 
     @property
```

### Comparing `zettel_org-0.7.1/src/zorg/service/file_groups.py` & `zettel_org-0.7.2/src/zorg/service/file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/src/zorg/service/handlers.py` & `zettel_org-0.7.2/src/zorg/service/handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 import sys
 from typing import Iterable, Iterator
 
 from logrus import Logger
 from tqdm import tqdm
 import vimala
 
-from . import common
+from . import common as c
 from .. import APP_NAME
 from ..domain.messages import commands, events
+from ..domain.types import Color
 from ..storage.sql.session import SQLSession
 from .compiler import walk_zorg_file
 from .zid_manager import ZIDManager
 
 
-logger = Logger(__name__)
+_LOGGER = Logger(__name__)
 
 
 def edit_files(cmd: commands.EditCommand, session: SQLSession) -> None:
     """Command handler for the EditCommand."""
     vimala.vim(
         *cmd.paths,
         commands=_process_vim_commands(cmd.zettel_dir, cmd.vim_commands),
@@ -33,53 +34,53 @@
 
 def check_keep_alive_file(
     event: events.EditorClosedEvent, session: SQLSession
 ) -> None:
     """Check if the 'keep alive' file exists and, if so, reopens the editor."""
     keep_alive_file = event.edit_cmd.keep_alive_file
     if not keep_alive_file.exists():
-        logger.debug(
+        _LOGGER.debug(
             "No keep alive file found.",
             keep_alive_file=keep_alive_file,
         )
         return
 
     zdir = event.edit_cmd.zettel_dir
-    prepend_zdir = partial(common.prepend_zdir, zdir)
+    prepend_zdir = partial(c.prepend_zdir, zdir)
     vim_commands = list(event.edit_cmd.vim_commands)
     if keep_alive_file.stat().st_size == 0:
-        logger.debug(
+        _LOGGER.debug(
             "Empty keep alive file found.",
             keep_alive_file=keep_alive_file,
         )
         paths = event.edit_cmd.paths
     else:
         keep_alive_lines = list(keep_alive_file.read_text().split())
         focused_filename = keep_alive_lines.pop()
         vim_commands = [
             cmd for cmd in vim_commands if not cmd.startswith("edit ")
         ]
         vim_commands.append(f"edit {focused_filename}")
         new_paths = prepend_zdir([Path(p.strip()) for p in keep_alive_lines])
-        logger.debug(
+        _LOGGER.debug(
             "Editing files specified in the keep alive file.",
             keep_alive_file=keep_alive_file,
             old_paths=event.edit_cmd.paths,
             new_paths=new_paths,
         )
         paths = new_paths
 
     verbose = event.edit_cmd.verbose
     if verbose <= 1:
-        logger.debug(
+        _LOGGER.debug(
             "Unlinking keep-alive file", keep_alive_file=keep_alive_file
         )
         keep_alive_file.unlink()
     else:
-        logger.debug(
+        _LOGGER.debug(
             "We are NOT deleting the keep-alive file",
             keep_alive_file=keep_alive_file,
         )
     session.add_last_message(
         commands.EditCommand(
             zettel_dir=zdir,
             paths=paths,
@@ -98,90 +99,99 @@
     total_num_notes = 0
     total_num_todos = 0
     for zo_path in tqdm(
         sorted(cmd.zettel_dir.rglob("*.zo"), key=lambda p: p.name),
         desc="Reading notes from zorg files",
         file=sys.stdout,
     ):
-        logger.info("Starting to walk zorg file", zorg_file=zo_path.name)
+        _LOGGER.info("Starting to walk zorg file", zorg_file=zo_path.name)
         zorg_file = walk_zorg_file(cmd.zettel_dir, zo_path)
         num_notes = len(zorg_file.notes)
         num_todos = len(
             [note for note in zorg_file.notes if note.todo_payload]
         )
         total_num_notes += num_notes
         total_num_todos += num_todos
-        logger.info(
+        _LOGGER.info(
             "Finished walking zorg file",
             zorg_file=zo_path.name,
             num_notes=num_notes,
             num_todos=num_todos,
             total_num_notes=total_num_notes,
             total_num_todos=total_num_todos,
         )
         session.repo.add(zorg_file)
         zorg_files.append(zorg_file)
-    logger.info(
+    _LOGGER.info(
         "Finished reading zettel org directory",
         num_files=len(zorg_files),
         num_notes=total_num_notes,
         num_todos=total_num_todos,
     )
     session.commit()
     session.add_message(events.DBModifiedEvent(cmd.zettel_dir))
 
 
 def reindex_database(
     cmd: commands.ReindexDBCommand, session: SQLSession
 ) -> None:
     """Reindex an existing zorg database."""
     paths = cmd.paths if cmd.paths else sorted(cmd.zettel_dir.rglob("*.zo"))
-    file_to_hash: dict[str, str] = {}
-    for path in paths:
-        key = common.strip_zdir(cmd.zettel_dir, path)
-        file_to_hash[key] = _hash_file(path)
-
-    zorg_data_dir = cmd.zettel_dir / f".{APP_NAME}"
-    zorg_data_dir.mkdir(parents=True, exist_ok=True)
-    file_hash_path = zorg_data_dir / "file_hash.json"
+    file_to_hash = _get_file_hash_map(cmd.zettel_dir, paths)
+    file_hash_path = _get_file_hash_path(cmd.zettel_dir)
     old_file_to_hash: dict[str, str] = (
         json.loads(file_hash_path.read_bytes())
         if file_hash_path.exists()
         else {}
     )
 
+    num_of_updates = 0
     for file, hash_ in file_to_hash.copy().items():
         if (
             file not in old_file_to_hash.keys()
             or old_file_to_hash[file] != hash_
         ):
-            logger.info("Changed file", file=file)
+            num_of_updates += 1
             old_zorg_file = session.repo.get(file).unwrap()
             if old_zorg_file is not None:
-                logger.info("Removing file from DB", file=file)
+                _LOGGER.debug("Removing file from DB", file=file)
+                c.zprint(
+                    "UPDATING EXISTING FILE",
+                    file,
+                    fg_color=Color.BLACK,
+                    bg_color=Color.YELLOW,
+                )
                 session.repo.remove_by_key(str(old_zorg_file.path))
+            else:
+                c.zprint(
+                    "ADDING NEW FILE",
+                    file,
+                    fg_color=Color.WHITE,
+                    bg_color=Color.GREEN,
+                )
 
             zorg_file = walk_zorg_file(
                 cmd.zettel_dir, Path(file), verbose=cmd.verbose
             )
-            logger.info("Adding zorg file", file=file)
+            _LOGGER.debug("Adding zorg file", file=file)
             session.repo.add(zorg_file)
+            session.commit()
 
-    logger.debug("Writing hash map to disk", file=str(file_hash_path))
-    with file_hash_path.open("w") as f:
-        json.dump(dict(sorted(file_to_hash.items())), f, indent=4)
+    if num_of_updates == 0:
+        c.zprint("NO ZORG FILES HAVE BEEN MODIFIED")
 
+    _write_file_hash_to_disk(file_hash_path, file_to_hash)
     session.commit()
     session.add_message(events.DBModifiedEvent(cmd.zettel_dir))
 
 
 def reindex_database_after_edit(
     event: events.EditorClosedEvent, session: SQLSession
 ) -> None:
-    """Reindex the zorg database after an edi."""
+    """Reindex the zorg database after an edit."""
     session.add_message(
         commands.ReindexDBCommand(event.edit_cmd.zettel_dir, paths=[])
     )
 
 
 def add_zids_to_notes_in_file(
     event: events.NewZorgNotesEvent, session: SQLSession
@@ -197,35 +207,63 @@
         start_idx = note.line_no - 1
         end_idx = note.line_no + len(note.body.split("\n")) - 1
         new_note_lines = zlines[start_idx:end_idx]
         first_note_line = new_note_lines[0]
         new_note_lines[0] = _add_zid_to_line(note.zid, first_note_line)
         zlines = zlines[:start_idx] + new_note_lines + zlines[end_idx:]
 
-    logger.info(
+    _LOGGER.info(
         "Adding ZIDs to zorg file",
         zorg_file=event.zorg_file_path,
         new_notes=len(event.new_notes),
     )
     event.zorg_file_path.write_text("\n".join(zlines))
 
+    zdir = event.zettel_dir
+    _write_file_hash_to_disk(
+        _get_file_hash_path(zdir),
+        _get_file_hash_map(zdir, Path(zdir).rglob("*.zo")),
+    )
+
 
 def increment_zid_counters(
     event: events.DBModifiedEvent, session: SQLSession
 ) -> None:
     """Increment the date-specific zorg ID counters.
 
     These are stored in a directory in your zettel dir and are used when
     generating new IDs (they are the XX in the YYMMDD#XX ID format).
     """
     del session
     zid_manager = ZIDManager(event.zettel_dir)
     zid_manager.write_to_disk()
 
 
+def _get_file_hash_map(zdir: Path, paths: Iterable[Path]) -> dict[str, str]:
+    file_to_hash: dict[str, str] = {}
+    for path in paths:
+        key = c.strip_zdir(zdir, path)
+        file_to_hash[key] = _hash_file(path)
+    return file_to_hash
+
+
+def _get_file_hash_path(zdir: Path) -> Path:
+    zorg_data_dir = zdir / f".{APP_NAME}"
+    zorg_data_dir.mkdir(parents=True, exist_ok=True)
+    return zorg_data_dir / "file_hash.json"
+
+
+def _write_file_hash_to_disk(
+    file_hash_path: Path, file_to_hash: dict[str, str]
+) -> None:
+    _LOGGER.debug("Writing hash map to disk", file=str(file_hash_path))
+    with file_hash_path.open("w") as f:
+        json.dump(dict(sorted(file_to_hash.items())), f, indent=4)
+
+
 def _add_zid_to_line(zid: str, line: str) -> str:
     all_words = line.split(" ")
 
     num_spaces = 0
     while all_words[0] == "":
         num_spaces += 1
         all_words.pop(0)
```

### Comparing `zettel_org-0.7.1/src/zorg/service/messagebus.py` & `zettel_org-0.7.2/src/zorg/service/messagebus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Zorg's message bus lives here."""
 
 from __future__ import annotations
 
-from typing import Any, Callable, MutableSequence, Sequence
+from typing import Any, Callable, Sequence
 
 from logrus import Logger
 from typist import assert_never
 
 from . import handlers
 from ..domain.messages import Message, commands, events
 from ..storage.sql.session import SQLSession
 
 
-logger = Logger(__name__)
+_LOGGER = Logger(__name__)
 
 MessageHandler = Callable[[Any, SQLSession], None]
 COMMAND_HANDLERS: dict[type[commands.Command], MessageHandler] = {
     commands.EditCommand: handlers.edit_files,
     commands.CreateDBCommand: handlers.create_database,
     commands.ReindexDBCommand: handlers.reindex_database,
 }
@@ -29,56 +29,53 @@
     events.DBModifiedEvent: [handlers.increment_zid_counters],
 }
 
 
 def handle(messages: Sequence[Message], session: SQLSession) -> None:
     """Entry point into Zorg's event messagebus loop."""
     queue = list(messages)
-    while queue:
+    while queue := sorted(
+        queue, key=lambda x: isinstance(x, commands.Command)
+    ):
         message = queue.pop(0)
-        _handle_message(message, queue, session)
+        _handle_message(message, session)
+        queue.extend(session.collect_new_messages())
 
 
-def _handle_message(
-    message: Message, queue: MutableSequence[Message], session: SQLSession
-) -> None:
+def _handle_message(message: Message, session: SQLSession) -> None:
     with session:
         if isinstance(message, events.Event):
-            _handle_event(message, queue, session)
+            _handle_event(message, session)
         elif isinstance(message, commands.Command):
-            _handle_command(message, queue, session)
+            _handle_command(message, session)
         else:
             assert_never(message)
 
 
 def _handle_event(
     event: events.Event,
-    queue: MutableSequence[Message],
     session: SQLSession,
 ) -> None:
     for handler in EVENT_HANDLERS[type(event)]:
         try:
-            logger.debug(
+            _LOGGER.debug(
                 "handling event with handler",
                 zorg_event=str(event),
                 handler=str(handler),
             )
             handler(event, session)
-            queue.extend(session.collect_new_messages())
         except Exception:
-            logger.exception("Exception handling event", zorg_event=event)
+            _LOGGER.exception("Exception handling event", zorg_event=event)
             continue
 
 
 def _handle_command(
     command: commands.Command,
-    queue: MutableSequence[Message],
     session: SQLSession,
 ) -> None:
-    logger.debug("handling command", command=command)
+    _LOGGER.debug("handling command", command=command)
     try:
         handler = COMMAND_HANDLERS[type(command)]
         handler(command, session)
-        queue.extend(session.collect_new_messages())
     except Exception:
-        logger.exception("Exception handling command", command=command)
+        _LOGGER.exception("Exception handling command", command=command)
         raise
```

### Comparing `zettel_org-0.7.1/src/zorg/service/templates.py` & `zettel_org-0.7.2/src/zorg/service/templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from logrus import Logger
 from typist import PathLike
 
 from . import common
 from ..domain.types import TemplatePatternMapType, VarMapType
 
 
-logger = Logger(__name__)
+_LOGGER = Logger(__name__)
 
 
 def init_from_template(
     zettel_dir: PathLike,
     template_pattern_map: TemplatePatternMapType,
     new_path: PathLike,
     *,
@@ -47,22 +47,22 @@
     for pattern, tmpl_path in template_pattern_map.items():
         if match := pattern.match(new_path.name):
             matched_template = tmpl_path
             var_map |= match.groupdict()
             break
 
     if matched_template is None:
-        logger.warn(
+        _LOGGER.warn(
             "Unable to match new filename with any registered templates.",
             template_pattern_map=template_pattern_map,
             new_path=new_path,
         )
         return
 
-    logger.info(
+    _LOGGER.info(
         "Creating new file using zorg template.",
         new_file=new_path,
         template=matched_template,
     )
     tmpl_manager = ZorgTemplateManager(zettel_dir)
     contents = tmpl_manager.render(
         common.prepend_zdir(zettel_dir, [matched_template])[0],
```

### Comparing `zettel_org-0.7.1/src/zorg/service/zid_manager.py` & `zettel_org-0.7.2/src/zorg/service/zid_manager.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/src/zorg/storage/sql/engine.py` & `zettel_org-0.7.2/src/zorg/storage/sql/engine.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/src/zorg/storage/sql/models.py` & `zettel_org-0.7.2/src/zorg/storage/sql/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # WARNING: Don't bother importing __future__.annotations in this module!
 import datetime as dt
 from typing import List, Optional
 
 from sqlmodel import Field, Relationship, SQLModel, String
 from sqlmodel.sql.expression import Select, SelectOfScalar
 
-from ...domain.types import NoteStatus
+from ...domain.types import NoteType
 
 
 # HACK: see https://github.com/tiangolo/sqlmodel/issues/189
 Select.inherit_cache = True
 SelectOfScalar.inherit_cache = True
 
 
@@ -118,15 +118,15 @@
 
     # TODO(bugyi): Make zid required to persist to DB.
     # TODO(bugyi): Make zid unique.
     zid: Optional[str] = Field(default=None)
 
     create_date: dt.date = Field(default_factory=dt.date.today)
     todo_priority: Optional[str] = None
-    todo_status: Optional[NoteStatus] = None
+    todo_status: Optional[NoteType] = None
 
     # relationships
     zorg_file: ZorgFile = Relationship(
         back_populates="notes", link_model=ZorgFileLink
     )
     contexts: List["Context"] = Relationship(
         back_populates="notes", link_model=ContextLink
```

### Comparing `zettel_org-0.7.1/src/zorg/storage/sql/repo.py` & `zettel_org-0.7.2/src/zorg/storage/sql/repo.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,73 +9,66 @@
 
 from eris import ErisResult, Err, Ok
 from logrus import Logger
 from sqlmodel import Session, select
 
 from . import models as sql
 from ...domain.messages.events import NewZorgNotesEvent
-from ...domain.models import WhereOrFilter, ZorgFile, ZorgNote
+from ...domain.models import File, Note, WhereOrFilter
 from ...service.zid_manager import ZIDManager
 from .converters import ZorgFileConverter, ZorgNoteConverter, to_select_of_note
 
 
-logger = Logger(__name__)
+_LOGGER = Logger(__name__)
 
 
 class SQLRepo:
     """Repo that stores zorg notes in sqlite database."""
 
     def __init__(
-        self,
-        zettel_dir: Path,
-        session: Session,
+        self, zettel_dir: Path, session: Session, *, verbose: int = 0
     ) -> None:
         self._zettel_dir = zettel_dir
         self._session = session
         self._converter = ZorgFileConverter(zettel_dir, session)
         self._note_converter = ZorgNoteConverter(session)
+        self._verbose = verbose
 
-        self.seen: list[ZorgFile] = []
+        self.seen: list[File] = []
 
-    def add(
-        self, zorg_file: ZorgFile, /, *, key: str = None
-    ) -> ErisResult[str]:
+    def add(self, zorg_file: File, /, *, key: str = None) -> ErisResult[str]:
         """Adds a new file to the DB.
 
         Returns a unique identifier that has been associated with this file.
         """
         del key
         self._seen_zorg_file(zorg_file)
         _add_zids(self._zettel_dir, zorg_file)
         sql_zorg_file = self._converter.from_entity(zorg_file)
         self._session.add(sql_zorg_file)
         return Ok(sql_zorg_file.path)
 
     def remove(
-        self, zorg_file: ZorgFile, /  # noqa: W504
-    ) -> ErisResult[ZorgFile | None]:
+        self, zorg_file: File, /  # noqa: W504
+    ) -> ErisResult[File | None]:
         """Remove a file from the DB."""
         sql_zorg_file = self._converter.from_entity(zorg_file)
         self._session.delete(sql_zorg_file)
         return Ok(zorg_file)
 
     # TODO(bugyi): Remove commits from this function!
-    def remove_by_key(self, key: str) -> ErisResult[Optional[ZorgFile]]:
+    def remove_by_key(self, key: str) -> ErisResult[Optional[File]]:
         """Remove a zorg file from the repo by path."""
         path = key
         stmt = select(sql.ZorgFile).where(sql.ZorgFile.path == path)
         results = self._session.exec(stmt)
         sql_zorg_file = results.first()
         if sql_zorg_file:
             zorg_file = self._converter.to_entity(sql_model=sql_zorg_file)
-            logger.info(
-                "Deleting Zorg File",
-                sql_zorg_file=sql_zorg_file,
-                zorg_file=zorg_file,
-            )
+            _LOGGER.debug("Deleting Zorg File", zorg_file=zorg_file)
             for sql_note in sql_zorg_file.notes:
                 for prop_link in sql_note.property_links:
                     delete_prop = len(prop_link.prop.links) == 1
                     self._session.delete(prop_link)
                     if delete_prop:
                         self._session.delete(prop_link.prop)
                     self._session.commit()
@@ -92,62 +85,65 @@
                             self._session.commit()
 
                 self._session.delete(sql_note)
             self._session.delete(sql_zorg_file)
             return Ok(zorg_file)
         else:
             emsg = "Failed to delete Zorg File"
-            logger.warning(emsg, path=path)
+            _LOGGER.warning(emsg, path=path)
             return Err(emsg)
 
-    def get(self, key: str) -> ErisResult[Optional[ZorgFile]]:
+    def get(self, key: str) -> ErisResult[Optional[File]]:
         """Retrieve a file from the DB."""
         path = key
         stmt = select(sql.ZorgFile).where(sql.ZorgFile.path == path)
         results = self._session.exec(stmt)
         sql_zorg_file = results.first()
         if sql_zorg_file:
             zorg_file = self._converter.to_entity(sql_zorg_file)
             self._seen_zorg_file(zorg_file)
             return Ok(zorg_file)
         else:
             return Ok(None)
 
-    def get_by_query(
-        self, query: Optional[WhereOrFilter]
-    ) -> ErisResult[list[ZorgNote]]:
+    def get_by_query(self, query: Optional[WhereOrFilter]) -> list[Note]:
         """Get file(s) from DB by using a query."""
         select_of_note = to_select_of_note(query)
-        result: list[ZorgNote] = []
+        # If the user asked for really verbose output...
+        if self._verbose > 1:
+            # ... then we print the SELECT statement.
+            print(select_of_note)
+
+        result: list[Note] = []
         for sql_note in self._session.exec(select_of_note):
             result.append(self._note_converter.to_entity(sql_note))
-        return Ok(result)
+        return result
 
-    def all(self) -> ErisResult[list[ZorgFile]]:
+    def all(self) -> ErisResult[list[File]]:
         """Returns all zorg notes contained in the underlying SQL database."""
         stmt = select(sql.ZorgFile)
-        result: list[ZorgFile] = []
+        result: list[File] = []
         for sql_zorg_file in self._session.exec(stmt).all():
             zorg_file = self._converter.to_entity(sql_zorg_file)
             self._seen_zorg_file(zorg_file)
         return Ok(result)
 
-    def _seen_zorg_file(self, zorg_file: ZorgFile) -> None:
+    def _seen_zorg_file(self, zorg_file: File) -> None:
         # TODO(bugyi): Do I need to deduplicate self.seen?
         self.seen.append(zorg_file)
 
 
-def _add_zids(zdir: Path, zorg_file: ZorgFile) -> None:
+def _add_zids(zdir: Path, zorg_file: File) -> None:
     new_notes = []
     zid_manager = ZIDManager(zdir)
     for note in zorg_file.notes:
         if note.zid is None:
-            logger.debug("Found new zorg note", zorg_note=note)
+            _LOGGER.debug("Found new zorg note", zorg_note=note)
             zid = zid_manager.get_next(note.create_date)
             note.zid = zid
             new_notes.append(note)
     if new_notes:
         zorg_file.events.append(
             NewZorgNotesEvent(
-                zorg_file_path=zorg_file.path, new_notes=new_notes
+                zdir, zorg_file_path=zorg_file.path, new_notes=new_notes
             )
         )
```

### Comparing `zettel_org-0.7.1/src/zorg/storage/sql/session.py` & `zettel_org-0.7.2/src/zorg/storage/sql/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from ...domain.messages import Message
 from ...domain.types import CreateEngineType
 from .engine import create_cached_engine
 from .repo import SQLRepo
 
 
-logger = Logger(__name__)
+_LOGGER = Logger(__name__)
 
 
 class SQLSession:
     """Unit-of-work pattern used to manage transactions on zorg's SQL DB.
 
     TODO: Document __init__() params here.
     """
@@ -41,22 +41,25 @@
             engine_kwargs["echo"] = True
 
         _prep_sqlite_db(db_url, should_delete=should_delete_existing_db)
         self._engine_factory = partial(engine_factory, db_url, **engine_kwargs)
         self._zettel_dir = zettel_dir
         self._messages: list[Message] = []
         self._last_messages: list[Message] = []
+        self._verbose = verbose
 
         self._session: Session
         self._repo: SQLRepo
 
     def __enter__(self) -> SQLSession:
         """Called before entering a SQLSession with-block."""
         self._session = Session(self._engine_factory())
-        self._repo = SQLRepo(self._zettel_dir, self._session)
+        self._repo = SQLRepo(
+            self._zettel_dir, self._session, verbose=self._verbose
+        )
         return self
 
     def __exit__(
         self,
         exc_type: Type[BaseException] | None,
         exc_value: BaseException | None,
         traceback: TracebackType | None,
@@ -96,27 +99,28 @@
         These messages will be processed AFTER any messages attached to domain
         entities (e.g. zorg files).
         """
         self._last_messages.append(message)
 
     def collect_new_messages(self) -> Iterator[Message]:
         """Collect new events/commands for our messagebus to process."""
-        while self._messages:
-            yield self._messages.pop(0)
-
-        for zorg_file in self.repo.seen:
-            while zorg_file.events:
-                yield zorg_file.events.pop(0)
+        while self._messages or any(file.events for file in self.repo.seen):
+            while self._messages:
+                yield self._messages.pop(0)
+
+            for zorg_file in self.repo.seen:
+                while zorg_file.events:
+                    yield zorg_file.events.pop(0)
 
         while self._last_messages:
             yield self._last_messages.pop(0)
 
 
 def _prep_sqlite_db(database_url: str, should_delete: bool = False) -> None:
     """Ensure sqlite DB file exists and delete if {should_delete} is True."""
     sqlite_prefix = "sqlite:///"
     if database_url.startswith(sqlite_prefix):
         db_path = Path(database_url[len(sqlite_prefix) :])
         db_path.parent.mkdir(exist_ok=True, parents=True)
         if db_path.exists() and should_delete:
-            logger.info("Deleting existing zorg database.", db_path=db_path)
+            _LOGGER.info("Deleting existing zorg database.", db_path=db_path)
             db_path.unlink()
```

### Comparing `zettel_org-0.7.1/targets.mk` & `zettel_org-0.7.2/targets.mk`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/__snapshots__/test_run_compile.ambr` & `zettel_org-0.7.2/tests/__snapshots__/test_run_compile.ambr`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-links]
   '''
   {'notes': [{'areas': [],
@@ -377,30 +377,30 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': ' Another related todo',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'A note about life...',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -421,15 +421,15 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'With a note',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -553,45 +553,45 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'A',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': ' 2024-03-13 Medium Priority TODO',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDatetime(2024, 3, 13, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'B',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': ' 2024-03-13 Low Priority TODO',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDatetime(2024, 3, 13, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-property]
   '''
   {'notes': [{'areas': [],
@@ -617,15 +617,15 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {'due': '2024-03-13', 'p': '1'},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-scrambled_prj_notes]
   '''
   {'notes': [{'areas': [],
@@ -1580,15 +1580,15 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {'due': '2024-03-30', 'p': '1'},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'Todo subnote A',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -1768,15 +1768,15 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'A note on the second section.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -1825,15 +1825,15 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'This is inside of h4_section!',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -1896,15 +1896,15 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': {'priority': 'C',
-                               'status': <NoteStatus.OPEN_TODO: 2>},
+                               'status': <NoteType.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'This is the final section!',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -1958,11 +1958,26 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['bad', 'to_the_bone'],
               'properties': {},
               'todo_payload': None,
+              'zid': None},
+             {'areas': ['tags'],
+              'body': 'Projects can start with a number, but CANNOT be all '
+                      'numbers',
+              'child_note_ids': [],
+              'contexts': [],
+              'create_date': FakeDate(2000, 1, 3),
+              'links': [],
+              'next_note_id': None,
+              'parent_note_id': None,
+              'people': [],
+              'prev_note_id': None,
+              'projects': ['2_be_or_not_2_be', 'bad'],
+              'properties': {},
+              'todo_payload': None,
               'zid': None}]}
   
   '''
 # ---
```

### Comparing `zettel_org-0.7.1/tests/__snapshots__/test_run_db.ambr` & `zettel_org-0.7.2/tests/__snapshots__/test_run_db.ambr`

 * *Files 0% similar despite different names*

```diff
@@ -26,24 +26,25 @@
     '2030-12-31',
   ])
 # ---
 # name: test_run_db_create__file_count[YAMLConfigFile]
   10
 # ---
 # name: test_run_db_create__note_count[YAMLConfigFile]
-  135
+  136
 # ---
 # name: test_run_db_create__people[YAMLConfigFile]
   list([
     'clyzajrm',
     'pig',
   ])
 # ---
 # name: test_run_db_create__projects[YAMLConfigFile]
   list([
+    '2_be_or_not_2_be',
     'arms',
     'bad',
     'bazbuz',
     'bmlakcr',
     'bqf',
     'cmeq',
     'cpv_mociy',
@@ -217,14 +218,15 @@
     '000103#21',
     '000103#22',
     '000103#23',
     '000103#24',
     '000103#25',
     '000103#26',
     '000103#27',
+    '000103#28',
     '240313#00',
     '240313#01',
     '240313#02',
     '240323#00',
     '240323#01',
     '240323#02',
     '240323#03',
```

### Comparing `zettel_org-0.7.1/tests/__snapshots__/test_run_edit.ambr` & `zettel_org-0.7.2/tests/__snapshots__/test_run_edit.ambr`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   # 2000-01-03.Mon
   #
   # ^ = [[2000/20000103]]
   # < = [[2000/20000102_day]]
   # > = [[2000/20000104_day]]
   # @ = [[day_log.zot]]
   
-  o 000103#28 #gtd pomodoro
+  o 000103#29 #gtd pomodoro
     * Google Calendar (bbugyi@google + bryanbugyi34@gmail)
     * Process yesterday's bujo log (e.g. close events, add missing pomodoros, rollover goals)
     * Copy any important gchat convos from yesterday into chat/*.txt
     * Check today's tickler file: [[tick_03]]
     * Fill out yesterday's habit tracker: [[2000/20000102_habit]]
     * go/g3co
     * Review Google Keep Inbox
```

### Comparing `zettel_org-0.7.1/tests/__snapshots__/test_run_template.ambr` & `zettel_org-0.7.2/tests/__snapshots__/test_run_template.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/common.py` & `zettel_org-0.7.2/tests/common.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/conftest.py` & `zettel_org-0.7.2/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,26 @@
 if TYPE_CHECKING:  # fixes pytest warning
     from clack.pytest_plugin import MakeConfigFile
 
 
 @fixture(scope="session")
 def zettel_dir(tmp_path_factory: TempPathFactory) -> Path:
     """Returns a zettel directory that contains copies of all *.zo files."""
-    tmp_path = tmp_path_factory.getbasetemp()
+    return _get_zettel_dir(tmp_path_factory.getbasetemp())
+
+
+@fixture(scope="module")
+def module_zettel_dir(tmp_path_factory: TempPathFactory) -> Path:
+    """Returns a zettel directory that contains copies of all *.zo files."""
+    tmp_path = tmp_path_factory.getbasetemp() / "module_scope"
+    tmp_path.mkdir()
+    return _get_zettel_dir(tmp_path)
+
+
+def _get_zettel_dir(tmp_path: Path) -> Path:
     zdir = tmp_path / "org"
     zdir.mkdir()
     for zo_path in _get_all_zo_and_zot_paths():
         zettel_zo_path = zdir / zo_path.name
         zettel_zo_path.write_bytes(zo_path.read_bytes())
     return zdir
```

### Comparing `zettel_org-0.7.1/tests/data/day_log.zot` & `zettel_org-0.7.2/tests/data/day_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/data/done_log.zot` & `zettel_org-0.7.2/tests/data/done_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/data/habit_log.zot` & `zettel_org-0.7.2/tests/data/habit_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/test_config.py` & `zettel_org-0.7.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/test_file_groups.py` & `zettel_org-0.7.2/tests/test_file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/test_run_action_open.py` & `zettel_org-0.7.2/tests/test_run_action_open.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/test_run_compile.py` & `zettel_org-0.7.2/tests/test_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/test_run_db.py` & `zettel_org-0.7.2/tests/test_run_db.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 """Tests the zorg project's 'db' CLI command."""
 
 from __future__ import annotations
 
 from pathlib import Path
 import sqlite3
 
-from _pytest.tmpdir import TempPathFactory
 from pytest import fixture
 from syrupy.assertion import SnapshotAssertion as Snapshot
 
 from . import common as c
 
 
 @fixture(name="sql_cursor", scope="session")
-def sql_cursor_fixture(
-    main: c.MainType, tmp_path_factory: TempPathFactory, zettel_dir: Path
-) -> sqlite3.Cursor:
+def sql_cursor_fixture(main: c.MainType, zettel_dir: Path) -> sqlite3.Cursor:
     """Connects to the zorg DB created by 'zorg db create'."""
-    tmp_path = tmp_path_factory.getbasetemp()
-    db_path_str = f"{tmp_path}/zorg.db"
-    exit_code = main(
-        "--dir",
-        str(zettel_dir),
-        "db",
-        "create",
-        database_url=f"sqlite:///{db_path_str}",
-    )
+    db_path_str = f"{zettel_dir}/.zorg/zorg.db"
+    exit_code = main("--dir", str(zettel_dir), "db", "create")
     assert exit_code == 0
     conn = sqlite3.connect(db_path_str)
     return conn.cursor()
 
 
 def test_run_db_create__table_names(
     sql_cursor: sqlite3.Cursor, snapshot: Snapshot
```

### Comparing `zettel_org-0.7.1/tests/test_run_edit.py` & `zettel_org-0.7.2/tests/test_run_edit.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.1/tests/test_run_template.py` & `zettel_org-0.7.2/tests/test_run_template.py`

 * *Files identical despite different names*

