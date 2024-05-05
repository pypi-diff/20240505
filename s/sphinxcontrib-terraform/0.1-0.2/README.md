# Comparing `tmp/sphinxcontrib_terraform-0.1.tar.gz` & `tmp/sphinxcontrib_terraform-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_terraform-0.1.tar", last modified: Sun May  5 13:18:44 2024, max compression
+gzip compressed data, was "sphinxcontrib_terraform-0.2.tar", last modified: Sun May  5 13:25:20 2024, max compression
```

## Comparing `sphinxcontrib_terraform-0.1.tar` & `sphinxcontrib_terraform-0.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.521301 sphinxcontrib_terraform-0.1/
--rw-r--r--   0 jonathf    (501) staff       (20)     1224 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/.flake8
--rw-r--r--   0 jonathf    (501) staff       (20)      160 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/.gitignore
--rw-r--r--   0 jonathf    (501) staff       (20)     8221 2024-04-20 13:30:09.000000 sphinxcontrib_terraform-0.1/.gitlab-ci.yml
--rw-r--r--   0 jonathf    (501) staff       (20)      230 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/CHANGELOG.rst
--rw-r--r--   0 jonathf    (501) staff       (20)      245 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/CONTRIBUTING.rst
--rw-r--r--   0 jonathf    (501) staff       (20)     4223 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/LICENSE
--rw-r--r--   0 jonathf    (501) staff       (20)     5535 2024-05-05 13:18:44.520942 sphinxcontrib_terraform-0.1/PKG-INFO
--rw-r--r--   0 jonathf    (501) staff       (20)     2844 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/README.rst
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.508632 sphinxcontrib_terraform-0.1/docs/
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.509138 sphinxcontrib_terraform-0.1/docs/_ext/
--rw-r--r--   0 jonathf    (501) staff       (20)     5321 2024-04-20 14:09:31.000000 sphinxcontrib_terraform-0.1/docs/_ext/extlinks.py
--rw-r--r--   0 jonathf    (501) staff       (20)     1320 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/_ext/sphinxcompat.py
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.509309 sphinxcontrib_terraform-0.1/docs/_static/
--rw-r--r--   0 jonathf    (501) staff       (20)      586 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/_static/style.css
--rw-r--r--   0 jonathf    (501) staff       (20)      173 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/about.rst
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.509483 sphinxcontrib_terraform-0.1/docs/apidoc/
--rw-r--r--   0 jonathf    (501) staff       (20)      263 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/apidoc/index.rst
--rw-r--r--   0 jonathf    (501) staff       (20)     2221 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/changelog.rst
--rw-r--r--   0 jonathf    (501) staff       (20)    18818 2024-04-20 13:39:26.000000 sphinxcontrib_terraform-0.1/docs/conf.py
--rw-r--r--   0 jonathf    (501) staff       (20)      168 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/contributing.rst
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.509642 sphinxcontrib_terraform-0.1/docs/demo/
--rw-r--r--   0 jonathf    (501) staff       (20)      382 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/demo/index.rst
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.510106 sphinxcontrib_terraform-0.1/docs/demo/terraform/
--rw-r--r--   0 jonathf    (501) staff       (20)     1803 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/demo/terraform/main.tf
--rw-r--r--   0 jonathf    (501) staff       (20)       26 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/demo/terraform/outputs.tf
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.510401 sphinxcontrib_terraform-0.1/docs/demo/terraform/sub/
--rw-r--r--   0 jonathf    (501) staff       (20)       49 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/demo/terraform/sub/output.tf
--rw-r--r--   0 jonathf    (501) staff       (20)       73 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/demo/terraform/sub/variables.tf
--rw-r--r--   0 jonathf    (501) staff       (20)       58 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/demo/terraform/variables.tf
--rw-r--r--   0 jonathf    (501) staff       (20)     4258 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/glossary.rst
--rw-r--r--   0 jonathf    (501) staff       (20)     2734 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/index.rst
--rw-r--r--   0 jonathf    (501) staff       (20)    14253 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/docs/usage.rst
--rw-r--r--   0 jonathf    (501) staff       (20)     3735 2024-04-20 13:42:33.000000 sphinxcontrib_terraform-0.1/noxfile.py
--rw-r--r--   0 jonathf    (501) staff       (20)     7841 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/pyproject.toml
--rw-r--r--   0 jonathf    (501) staff       (20)      117 2024-04-20 13:43:25.000000 sphinxcontrib_terraform-0.1/requirements.in
--rw-r--r--   0 jonathf    (501) staff       (20)       38 2024-05-05 13:18:44.521348 sphinxcontrib_terraform-0.1/setup.cfg
--rw-r--r--   0 jonathf    (501) staff       (20)     2865 2024-05-05 13:18:32.000000 sphinxcontrib_terraform-0.1/setup.py
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.504042 sphinxcontrib_terraform-0.1/src/
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.512178 sphinxcontrib_terraform-0.1/src/sphinx_terraform/
--rw-r--r--   0 jonathf    (501) staff       (20)     3364 2024-04-20 13:39:19.000000 sphinxcontrib_terraform-0.1/src/sphinx_terraform/__init__.py
--rw-r--r--   0 jonathf    (501) staff       (20)      400 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/src/sphinx_terraform/code.py
--rw-r--r--   0 jonathf    (501) staff       (20)      158 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/src/sphinx_terraform/i18n.py
--rw-r--r--   0 jonathf    (501) staff       (20)    26040 2024-04-20 14:14:32.000000 sphinxcontrib_terraform-0.1/src/sphinx_terraform/markup.py
--rw-r--r--   0 jonathf    (501) staff       (20)        0 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/src/sphinx_terraform/py.typed
--rw-r--r--   0 jonathf    (501) staff       (20)     4609 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/src/sphinx_terraform/sphinxapi.py
--rw-r--r--   0 jonathf    (501) staff       (20)    29679 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/src/sphinx_terraform/terraform.py
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.513177 sphinxcontrib_terraform-0.1/src/sphinx_terraform/viewcode/
--rw-r--r--   0 jonathf    (501) staff       (20)     5169 2024-04-20 13:39:30.000000 sphinxcontrib_terraform-0.1/src/sphinx_terraform/viewcode/__init__.py
--rw-r--r--   0 jonathf    (501) staff       (20)     8900 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/src/sphinx_terraform/viewcode/html.py
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.519034 sphinxcontrib_terraform-0.1/src/sphinxcontrib_terraform.egg-info/
--rw-r--r--   0 jonathf    (501) staff       (20)     5535 2024-05-05 13:18:44.000000 sphinxcontrib_terraform-0.1/src/sphinxcontrib_terraform.egg-info/PKG-INFO
--rw-r--r--   0 jonathf    (501) staff       (20)     2523 2024-05-05 13:18:44.000000 sphinxcontrib_terraform-0.1/src/sphinxcontrib_terraform.egg-info/SOURCES.txt
--rw-r--r--   0 jonathf    (501) staff       (20)        1 2024-05-05 13:18:44.000000 sphinxcontrib_terraform-0.1/src/sphinxcontrib_terraform.egg-info/dependency_links.txt
--rw-r--r--   0 jonathf    (501) staff       (20)      504 2024-05-05 13:18:44.000000 sphinxcontrib_terraform-0.1/src/sphinxcontrib_terraform.egg-info/requires.txt
--rw-r--r--   0 jonathf    (501) staff       (20)       17 2024-05-05 13:18:44.000000 sphinxcontrib_terraform-0.1/src/sphinxcontrib_terraform.egg-info/top_level.txt
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.514135 sphinxcontrib_terraform-0.1/test/
--rw-r--r--   0 jonathf    (501) staff       (20)       81 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/conftest.py
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.514609 sphinxcontrib_terraform-0.1/test/integrated/
--rw-r--r--   0 jonathf    (501) staff       (20)     1003 2024-04-20 13:56:45.000000 sphinxcontrib_terraform-0.1/test/integrated/conftest.py
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.504752 sphinxcontrib_terraform-0.1/test/integrated/samples/
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.515001 sphinxcontrib_terraform-0.1/test/integrated/samples/test-basic/
--rw-r--r--   0 jonathf    (501) staff       (20)        0 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-basic/conf.py
--rw-r--r--   0 jonathf    (501) staff       (20)       43 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-basic/index.rst
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.515511 sphinxcontrib_terraform-0.1/test/integrated/samples/test-config-terraform_comment_markup-md/
--rw-r--r--   0 jonathf    (501) staff       (20)      118 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-config-terraform_comment_markup-md/conf.py
--rw-r--r--   0 jonathf    (501) staff       (20)      414 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-config-terraform_comment_markup-md/index.rst
--rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-config-terraform_comment_markup-md/main.tf
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.516269 sphinxcontrib_terraform-0.1/test/integrated/samples/test-config-terraform_comment_markup-rst/
--rw-r--r--   0 jonathf    (501) staff       (20)      119 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-config-terraform_comment_markup-rst/conf.py
--rw-r--r--   0 jonathf    (501) staff       (20)      435 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-config-terraform_comment_markup-rst/index.md
--rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-config-terraform_comment_markup-rst/main.tf
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.516803 sphinxcontrib_terraform-0.1/test/integrated/samples/test-md-comment-from-md-document/
--rw-r--r--   0 jonathf    (501) staff       (20)       85 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-md-comment-from-md-document/conf.py
--rw-r--r--   0 jonathf    (501) staff       (20)      444 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-md-comment-from-md-document/index.md
--rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-md-comment-from-md-document/main.tf
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.517297 sphinxcontrib_terraform-0.1/test/integrated/samples/test-md-directive-in-rst-document/
--rw-r--r--   0 jonathf    (501) staff       (20)       85 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-md-directive-in-rst-document/conf.py
--rw-r--r--   0 jonathf    (501) staff       (20)      493 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-md-directive-in-rst-document/index.rst
--rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-md-directive-in-rst-document/main.tf
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.517923 sphinxcontrib_terraform-0.1/test/integrated/samples/test-rst-comment-from-rst-document/
--rw-r--r--   0 jonathf    (501) staff       (20)       85 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-rst-comment-from-rst-document/conf.py
--rw-r--r--   0 jonathf    (501) staff       (20)      477 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-rst-comment-from-rst-document/index.rst
--rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-rst-comment-from-rst-document/main.tf
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.518609 sphinxcontrib_terraform-0.1/test/integrated/samples/test-rst-directive-in-md-document/
--rw-r--r--   0 jonathf    (501) staff       (20)       85 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-rst-directive-in-md-document/conf.py
--rw-r--r--   0 jonathf    (501) staff       (20)      472 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-rst-directive-in-md-document/index.md
--rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/integrated/samples/test-rst-directive-in-md-document/main.tf
--rw-r--r--   0 jonathf    (501) staff       (20)     3214 2024-04-20 14:07:06.000000 sphinxcontrib_terraform-0.1/test/integrated/test_tf.py
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.504870 sphinxcontrib_terraform-0.1/test/unit/
-drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:18:44.518787 sphinxcontrib_terraform-0.1/test/unit/terraform/
--rw-r--r--   0 jonathf    (501) staff       (20)      479 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.1/test/unit/terraform/test_resourcesignature.py
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.762048 sphinxcontrib_terraform-0.2/
+-rw-r--r--   0 jonathf    (501) staff       (20)     1224 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/.flake8
+-rw-r--r--   0 jonathf    (501) staff       (20)      160 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/.gitignore
+-rw-r--r--   0 jonathf    (501) staff       (20)     8176 2024-05-05 13:24:58.000000 sphinxcontrib_terraform-0.2/.gitlab-ci.yml
+-rw-r--r--   0 jonathf    (501) staff       (20)      230 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/CHANGELOG.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)      245 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/CONTRIBUTING.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)     4223 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/LICENSE
+-rw-r--r--   0 jonathf    (501) staff       (20)     5507 2024-05-05 13:25:20.761723 sphinxcontrib_terraform-0.2/PKG-INFO
+-rw-r--r--   0 jonathf    (501) staff       (20)     2844 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/README.rst
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.751098 sphinxcontrib_terraform-0.2/docs/
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.751589 sphinxcontrib_terraform-0.2/docs/_ext/
+-rw-r--r--   0 jonathf    (501) staff       (20)     5321 2024-04-20 14:09:31.000000 sphinxcontrib_terraform-0.2/docs/_ext/extlinks.py
+-rw-r--r--   0 jonathf    (501) staff       (20)     1320 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/_ext/sphinxcompat.py
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.751747 sphinxcontrib_terraform-0.2/docs/_static/
+-rw-r--r--   0 jonathf    (501) staff       (20)      586 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/_static/style.css
+-rw-r--r--   0 jonathf    (501) staff       (20)      173 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/about.rst
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.751897 sphinxcontrib_terraform-0.2/docs/apidoc/
+-rw-r--r--   0 jonathf    (501) staff       (20)      263 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/apidoc/index.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)     2221 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/changelog.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)    18819 2024-05-05 13:24:58.000000 sphinxcontrib_terraform-0.2/docs/conf.py
+-rw-r--r--   0 jonathf    (501) staff       (20)      168 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/contributing.rst
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.752045 sphinxcontrib_terraform-0.2/docs/demo/
+-rw-r--r--   0 jonathf    (501) staff       (20)      382 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/demo/index.rst
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.752524 sphinxcontrib_terraform-0.2/docs/demo/terraform/
+-rw-r--r--   0 jonathf    (501) staff       (20)     1803 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/demo/terraform/main.tf
+-rw-r--r--   0 jonathf    (501) staff       (20)       26 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/demo/terraform/outputs.tf
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.752830 sphinxcontrib_terraform-0.2/docs/demo/terraform/sub/
+-rw-r--r--   0 jonathf    (501) staff       (20)       49 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/demo/terraform/sub/output.tf
+-rw-r--r--   0 jonathf    (501) staff       (20)       73 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/demo/terraform/sub/variables.tf
+-rw-r--r--   0 jonathf    (501) staff       (20)       58 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/demo/terraform/variables.tf
+-rw-r--r--   0 jonathf    (501) staff       (20)     4258 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/glossary.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)     2734 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/index.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)    14253 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/docs/usage.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)     3726 2024-05-05 13:24:58.000000 sphinxcontrib_terraform-0.2/noxfile.py
+-rw-r--r--   0 jonathf    (501) staff       (20)     7841 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/pyproject.toml
+-rw-r--r--   0 jonathf    (501) staff       (20)      104 2024-05-05 13:24:58.000000 sphinxcontrib_terraform-0.2/requirements.in
+-rw-r--r--   0 jonathf    (501) staff       (20)       38 2024-05-05 13:25:20.762100 sphinxcontrib_terraform-0.2/setup.cfg
+-rw-r--r--   0 jonathf    (501) staff       (20)     2865 2024-05-05 13:25:08.000000 sphinxcontrib_terraform-0.2/setup.py
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.746803 sphinxcontrib_terraform-0.2/src/
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.754077 sphinxcontrib_terraform-0.2/src/sphinx_terraform/
+-rw-r--r--   0 jonathf    (501) staff       (20)     3363 2024-05-05 13:24:58.000000 sphinxcontrib_terraform-0.2/src/sphinx_terraform/__init__.py
+-rw-r--r--   0 jonathf    (501) staff       (20)      400 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/src/sphinx_terraform/code.py
+-rw-r--r--   0 jonathf    (501) staff       (20)      158 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/src/sphinx_terraform/i18n.py
+-rw-r--r--   0 jonathf    (501) staff       (20)    26048 2024-05-05 13:24:58.000000 sphinxcontrib_terraform-0.2/src/sphinx_terraform/markup.py
+-rw-r--r--   0 jonathf    (501) staff       (20)        0 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/src/sphinx_terraform/py.typed
+-rw-r--r--   0 jonathf    (501) staff       (20)     4609 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/src/sphinx_terraform/sphinxapi.py
+-rw-r--r--   0 jonathf    (501) staff       (20)    29679 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/src/sphinx_terraform/terraform.py
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.754890 sphinxcontrib_terraform-0.2/src/sphinx_terraform/viewcode/
+-rw-r--r--   0 jonathf    (501) staff       (20)     5166 2024-05-05 13:24:58.000000 sphinxcontrib_terraform-0.2/src/sphinx_terraform/viewcode/__init__.py
+-rw-r--r--   0 jonathf    (501) staff       (20)     8900 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/src/sphinx_terraform/viewcode/html.py
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.759873 sphinxcontrib_terraform-0.2/src/sphinxcontrib_terraform.egg-info/
+-rw-r--r--   0 jonathf    (501) staff       (20)     5507 2024-05-05 13:25:20.000000 sphinxcontrib_terraform-0.2/src/sphinxcontrib_terraform.egg-info/PKG-INFO
+-rw-r--r--   0 jonathf    (501) staff       (20)     2523 2024-05-05 13:25:20.000000 sphinxcontrib_terraform-0.2/src/sphinxcontrib_terraform.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathf    (501) staff       (20)        1 2024-05-05 13:25:20.000000 sphinxcontrib_terraform-0.2/src/sphinxcontrib_terraform.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathf    (501) staff       (20)      491 2024-05-05 13:25:20.000000 sphinxcontrib_terraform-0.2/src/sphinxcontrib_terraform.egg-info/requires.txt
+-rw-r--r--   0 jonathf    (501) staff       (20)       17 2024-05-05 13:25:20.000000 sphinxcontrib_terraform-0.2/src/sphinxcontrib_terraform.egg-info/top_level.txt
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.755688 sphinxcontrib_terraform-0.2/test/
+-rw-r--r--   0 jonathf    (501) staff       (20)       81 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/conftest.py
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.755963 sphinxcontrib_terraform-0.2/test/integrated/
+-rw-r--r--   0 jonathf    (501) staff       (20)     1157 2024-05-05 13:24:58.000000 sphinxcontrib_terraform-0.2/test/integrated/conftest.py
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.747536 sphinxcontrib_terraform-0.2/test/integrated/samples/
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.756411 sphinxcontrib_terraform-0.2/test/integrated/samples/test-basic/
+-rw-r--r--   0 jonathf    (501) staff       (20)        0 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-basic/conf.py
+-rw-r--r--   0 jonathf    (501) staff       (20)       43 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-basic/index.rst
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.756875 sphinxcontrib_terraform-0.2/test/integrated/samples/test-config-terraform_comment_markup-md/
+-rw-r--r--   0 jonathf    (501) staff       (20)      118 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-config-terraform_comment_markup-md/conf.py
+-rw-r--r--   0 jonathf    (501) staff       (20)      414 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-config-terraform_comment_markup-md/index.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-config-terraform_comment_markup-md/main.tf
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.757353 sphinxcontrib_terraform-0.2/test/integrated/samples/test-config-terraform_comment_markup-rst/
+-rw-r--r--   0 jonathf    (501) staff       (20)      119 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-config-terraform_comment_markup-rst/conf.py
+-rw-r--r--   0 jonathf    (501) staff       (20)      435 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-config-terraform_comment_markup-rst/index.md
+-rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-config-terraform_comment_markup-rst/main.tf
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.757820 sphinxcontrib_terraform-0.2/test/integrated/samples/test-md-comment-from-md-document/
+-rw-r--r--   0 jonathf    (501) staff       (20)       85 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-md-comment-from-md-document/conf.py
+-rw-r--r--   0 jonathf    (501) staff       (20)      444 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-md-comment-from-md-document/index.md
+-rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-md-comment-from-md-document/main.tf
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.758276 sphinxcontrib_terraform-0.2/test/integrated/samples/test-md-directive-in-rst-document/
+-rw-r--r--   0 jonathf    (501) staff       (20)       85 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-md-directive-in-rst-document/conf.py
+-rw-r--r--   0 jonathf    (501) staff       (20)      493 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-md-directive-in-rst-document/index.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-md-directive-in-rst-document/main.tf
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.758825 sphinxcontrib_terraform-0.2/test/integrated/samples/test-rst-comment-from-rst-document/
+-rw-r--r--   0 jonathf    (501) staff       (20)       85 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-rst-comment-from-rst-document/conf.py
+-rw-r--r--   0 jonathf    (501) staff       (20)      477 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-rst-comment-from-rst-document/index.rst
+-rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-rst-comment-from-rst-document/main.tf
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.759481 sphinxcontrib_terraform-0.2/test/integrated/samples/test-rst-directive-in-md-document/
+-rw-r--r--   0 jonathf    (501) staff       (20)       85 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-rst-directive-in-md-document/conf.py
+-rw-r--r--   0 jonathf    (501) staff       (20)      472 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-rst-directive-in-md-document/index.md
+-rw-r--r--   0 jonathf    (501) staff       (20)      330 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/integrated/samples/test-rst-directive-in-md-document/main.tf
+-rw-r--r--   0 jonathf    (501) staff       (20)     3214 2024-04-20 14:07:06.000000 sphinxcontrib_terraform-0.2/test/integrated/test_tf.py
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.747666 sphinxcontrib_terraform-0.2/test/unit/
+drwxr-xr-x   0 jonathf    (501) staff       (20)        0 2024-05-05 13:25:20.759641 sphinxcontrib_terraform-0.2/test/unit/terraform/
+-rw-r--r--   0 jonathf    (501) staff       (20)      479 2024-04-17 18:01:09.000000 sphinxcontrib_terraform-0.2/test/unit/terraform/test_resourcesignature.py
```

### Comparing `sphinxcontrib_terraform-0.1/.flake8` & `sphinxcontrib_terraform-0.2/.flake8`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/.gitlab-ci.yml` & `sphinxcontrib_terraform-0.2/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -217,19 +217,18 @@
   image: python:$PYVERSION
   artifacts:
     when: always
     paths:
       - build/report/coverage*
   parallel:
     matrix:
-      - PYVERSION: "3.12"
-      - PYVERSION: "3.11"
       - PYVERSION: "3.10"
       - PYVERSION: "3.9"
       - PYVERSION: "3.8"
+      - PYVERSION: "3.7"
   needs: []
   allow_failure: true
 
 #
 ###
 
 ###
@@ -259,19 +258,18 @@
 coverage:
   stage: report
   script:
     - pip install -U nox
     - nox -rs coverage
   artifacts:
     when: always
+    paths:
+      - build/report/coverage
     reports:
-      coverage_report:
-        coverage_format: cobertura
-        path: build/report/coverage
-
+      cobertura: build/report/*.xml
   needs:
     - test
   coverage: '/TOTAL +\d+ +\d+ +\d+ +\d+ +(\d+)%/'
   allow_failure: false
   rules:
     # Always run except on schedules
     - if: $CI_PIPELINE_SOURCE == "schedule"
```

### Comparing `sphinxcontrib_terraform-0.1/LICENSE` & `sphinxcontrib_terraform-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/PKG-INFO` & `sphinxcontrib_terraform-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-terraform
-Version: 0.1
+Version: 0.2
 Summary: A Sphinx extension for documenting Terraform modules.
 Home-page: https://cblegare.gitlab.io/sphinx-terraform
 Author: Charles Bouchard-Légaré
 Author-email: charlesbouchardlegare@gmail.com
 License: BSD-2-Clause-Patent
 Project-URL: Documentation, https://cblegare.gitlab.io/sphinx-terraform
 Project-URL: Source, https://gitlab.com/cblegare/sphinx-terraform
@@ -24,19 +24,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: sphinx>=3.0
+Requires-Dist: sphinx>=3
 Requires-Dist: docutils
 Requires-Dist: typing_extensions; python_version < "3.8"
 Requires-Dist: importlib_metadata; python_version < "3.8"
-Requires-Dist: defusedxml
 Provides-Extra: test
 Requires-Dist: nox; extra == "test"
 Provides-Extra: markdown
 Requires-Dist: myst_parser; extra == "markdown"
 Requires-Dist: docutils>=0.16; extra == "markdown"
 Provides-Extra: docs
 Requires-Dist: myst_parser; extra == "docs"
@@ -45,24 +44,24 @@
 Requires-Dist: sphinx_paramlinks; extra == "docs"
 Requires-Dist: sphinx_copybutton; extra == "docs"
 Requires-Dist: sphinxcontrib_bibtex; extra == "docs"
 Requires-Dist: sphinxcontrib_programoutput; extra == "docs"
 Requires-Dist: sphinx_tabs; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Provides-Extra: all
+Requires-Dist: nox; extra == "all"
+Requires-Dist: sphinx_paramlinks; extra == "all"
 Requires-Dist: sphinxcontrib_programoutput; extra == "all"
-Requires-Dist: sphinx_tabs; extra == "all"
 Requires-Dist: myst_parser; extra == "all"
-Requires-Dist: docutils>=0.16; extra == "all"
-Requires-Dist: sphinxcontrib_bibtex; extra == "all"
-Requires-Dist: pydata-sphinx-theme; extra == "all"
-Requires-Dist: sphinx_paramlinks; extra == "all"
+Requires-Dist: sphinx_tabs; extra == "all"
 Requires-Dist: sphinx_copybutton; extra == "all"
+Requires-Dist: sphinxcontrib_bibtex; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints; extra == "all"
-Requires-Dist: nox; extra == "all"
+Requires-Dist: pydata-sphinx-theme; extra == "all"
+Requires-Dist: docutils>=0.16; extra == "all"
 
 ################
 Sphinx-Terraform
 ################
 
 .. container:: tagline
```

### Comparing `sphinxcontrib_terraform-0.1/README.rst` & `sphinxcontrib_terraform-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/docs/_ext/extlinks.py` & `sphinxcontrib_terraform-0.2/docs/_ext/extlinks.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/docs/_ext/sphinxcompat.py` & `sphinxcontrib_terraform-0.2/docs/_ext/sphinxcompat.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/docs/_static/style.css` & `sphinxcontrib_terraform-0.2/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/docs/changelog.rst` & `sphinxcontrib_terraform-0.2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/docs/conf.py` & `sphinxcontrib_terraform-0.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ##############################################################################
 
 
 ##############################################################################
 # -- General configuration ---------------------------------------------------
 
 # If your project needs a minimal Sphinx version, state it here.
-needs_sphinx = "3.0"
+needs_sphinx = "3"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named "sphinx.ext.*") or your custom
 # ones.
 extensions = [
     "sphinx.ext.napoleon",  # Google-style docstrings
     "sphinx.ext.intersphinx",  # Link to other Sphinx docs
@@ -530,19 +530,19 @@
 #
 terraform_sources = {"terraform": str(DOC_ROOT.joinpath("demo/terraform"))}
 ###
 
 #####
 ##############################################################################
 
-
 ##############################################################################
 # -- Local extension ---------------------------------------------------------
 #####
 #
 # The conf.py file can act directly as a Sphinx extension by defining a
 # setup function that takes a Sphinx object as an argument.
-def setup(app: Sphinx): ...
+def setup(app: Sphinx):
+    ...
 
 
 #####
 ##############################################################################
```

### Comparing `sphinxcontrib_terraform-0.1/docs/demo/terraform/main.tf` & `sphinxcontrib_terraform-0.2/docs/demo/terraform/main.tf`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/docs/glossary.rst` & `sphinxcontrib_terraform-0.2/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/docs/index.rst` & `sphinxcontrib_terraform-0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/docs/usage.rst` & `sphinxcontrib_terraform-0.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/noxfile.py` & `sphinxcontrib_terraform-0.2/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 import shutil
 from typing import List
 
 import nox
 
-supported_python_versions = ["3.8", "3.9", "3.10", "3.11", "3.12"]
+supported_python_versions = ["3.7", "3.8", "3.9", "3.10"]
 
 default_python = sorted(supported_python_versions)[-1]
 
 repo_root = Path(__file__).parent
 
 
 @nox.session(reuse_venv=True)
```

### Comparing `sphinxcontrib_terraform-0.1/pyproject.toml` & `sphinxcontrib_terraform-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/setup.py` & `sphinxcontrib_terraform-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 this_directory = Path(__file__).parent
 requirements_in = this_directory.joinpath("requirements.in")
 
 
 if __name__ == "__main__":
     setup(
         name="sphinxcontrib-terraform",
-        version="0.1",
+        version="0.2",
         description="A Sphinx extension for documenting Terraform modules.",
         long_description=(this_directory / "README.rst").read_text(),
         long_description_content_type="text/x-rst",
         url="https://cblegare.gitlab.io/sphinx-terraform",
         author="Charles Bouchard-Légaré",
         author_email="charlesbouchardlegare@gmail.com",
         license="BSD-2-Clause-Patent",
```

### Comparing `sphinxcontrib_terraform-0.1/src/sphinx_terraform/__init__.py` & `sphinxcontrib_terraform-0.2/src/sphinx_terraform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 This is **not** an API.
 """
-
 from __future__ import annotations
 
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, Union
 
 from sphinx.application import Sphinx
```

### Comparing `sphinxcontrib_terraform-0.1/src/sphinx_terraform/markup.py` & `sphinxcontrib_terraform-0.2/src/sphinx_terraform/markup.py`

 * *Files 0% similar despite different names*

```diff
@@ -738,30 +738,30 @@
             for sphinx_reference in candidates
         ]
 
     def _resolve_target(
         self, target: str, typename: Optional[str] = None
     ) -> List[SphinxData]:
         match = re.match(
-            r"^(?P<module>(\w+\/)*)?((?P<type>[a-z]+)-)?(?P<name>(([\w-]+)(\.([\w-]+))*)?)$",
+            r"^(?P<module>([\w-]+\/)*)?((?P<type>[a-z]+)-)?(?P<name>(([\w-]+)(\.([\w-]+))*)?)$",
             target,
         )
 
         if not match:
             return []
 
         matcher = self._make_matcher(target, typename)
 
         return list(filter(matcher, self.sphinx_references.values()))
 
     def _make_matcher(
         self, target: str, typename: Optional[str]
     ) -> Callable[[SphinxData], bool]:
         match = re.match(
-            r"^(?P<module>(\w+\/)*)?((?P<type>[a-z]+)-)?(?P<name>(([\w-]+)(\.([\w-]+))*)?)$",
+            r"^(?P<module>([\w-]+\/)*)?((?P<type>[a-z]+)-)?(?P<name>(([\w-]+)(\.([\w-]+))*)?)$",
             target,
         )
 
         if not match:
             return lambda x: False
 
         def matcher(sphinx_reference: SphinxData) -> bool:
@@ -771,14 +771,14 @@
             typename_ok = (
                 not typename or typename == sphinx_reference.sphinx_obj.type
             )
             module_ok = (
                 not matched_module
                 or matched_module.strip("/") == sphinx_reference.module.fullname
             )
-            name_ok = not matched_name or matched_name in str(
+            name_ok = not matched_name or (matched_name == str(
                 sphinx_reference.signature
-            )
+            ))
 
             return all([typename_ok, module_ok, name_ok])
 
         return matcher
```

### Comparing `sphinxcontrib_terraform-0.1/src/sphinx_terraform/sphinxapi.py` & `sphinxcontrib_terraform-0.2/src/sphinx_terraform/sphinxapi.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/src/sphinx_terraform/terraform.py` & `sphinxcontrib_terraform-0.2/src/sphinx_terraform/terraform.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/src/sphinx_terraform/viewcode/__init__.py` & `sphinxcontrib_terraform-0.2/src/sphinx_terraform/viewcode/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Similar to :mod:`sphinx.ext.viewcode`.
 """
-
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any, Iterator
 
 from docutils import nodes
 from docutils.nodes import Element, Node
@@ -27,15 +26,15 @@
 
 OUTPUT_DIRNAME = "_terraform_files"
 
 log = getLogger(__name__)
 
 
 def setup(app: Sphinx) -> ExtensionMetadata:
-    app.require_sphinx("3.0")
+    app.require_sphinx("3")
 
     app.connect("env-purge-doc", env_purge_doc)
     app.connect("doctree-read", doctree_read)
     app.connect("html-collect-pages", collect_pages)
     app.add_post_transform(ViewcodeAnchorToggler)
 
     return {
```

### Comparing `sphinxcontrib_terraform-0.1/src/sphinx_terraform/viewcode/html.py` & `sphinxcontrib_terraform-0.2/src/sphinx_terraform/viewcode/html.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/src/sphinxcontrib_terraform.egg-info/PKG-INFO` & `sphinxcontrib_terraform-0.2/src/sphinxcontrib_terraform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-terraform
-Version: 0.1
+Version: 0.2
 Summary: A Sphinx extension for documenting Terraform modules.
 Home-page: https://cblegare.gitlab.io/sphinx-terraform
 Author: Charles Bouchard-Légaré
 Author-email: charlesbouchardlegare@gmail.com
 License: BSD-2-Clause-Patent
 Project-URL: Documentation, https://cblegare.gitlab.io/sphinx-terraform
 Project-URL: Source, https://gitlab.com/cblegare/sphinx-terraform
@@ -24,19 +24,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: sphinx>=3.0
+Requires-Dist: sphinx>=3
 Requires-Dist: docutils
 Requires-Dist: typing_extensions; python_version < "3.8"
 Requires-Dist: importlib_metadata; python_version < "3.8"
-Requires-Dist: defusedxml
 Provides-Extra: test
 Requires-Dist: nox; extra == "test"
 Provides-Extra: markdown
 Requires-Dist: myst_parser; extra == "markdown"
 Requires-Dist: docutils>=0.16; extra == "markdown"
 Provides-Extra: docs
 Requires-Dist: myst_parser; extra == "docs"
@@ -45,24 +44,24 @@
 Requires-Dist: sphinx_paramlinks; extra == "docs"
 Requires-Dist: sphinx_copybutton; extra == "docs"
 Requires-Dist: sphinxcontrib_bibtex; extra == "docs"
 Requires-Dist: sphinxcontrib_programoutput; extra == "docs"
 Requires-Dist: sphinx_tabs; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Provides-Extra: all
+Requires-Dist: nox; extra == "all"
+Requires-Dist: sphinx_paramlinks; extra == "all"
 Requires-Dist: sphinxcontrib_programoutput; extra == "all"
-Requires-Dist: sphinx_tabs; extra == "all"
 Requires-Dist: myst_parser; extra == "all"
-Requires-Dist: docutils>=0.16; extra == "all"
-Requires-Dist: sphinxcontrib_bibtex; extra == "all"
-Requires-Dist: pydata-sphinx-theme; extra == "all"
-Requires-Dist: sphinx_paramlinks; extra == "all"
+Requires-Dist: sphinx_tabs; extra == "all"
 Requires-Dist: sphinx_copybutton; extra == "all"
+Requires-Dist: sphinxcontrib_bibtex; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints; extra == "all"
-Requires-Dist: nox; extra == "all"
+Requires-Dist: pydata-sphinx-theme; extra == "all"
+Requires-Dist: docutils>=0.16; extra == "all"
 
 ################
 Sphinx-Terraform
 ################
 
 .. container:: tagline
```

### Comparing `sphinxcontrib_terraform-0.1/src/sphinxcontrib_terraform.egg-info/SOURCES.txt` & `sphinxcontrib_terraform-0.2/src/sphinxcontrib_terraform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_terraform-0.1/test/integrated/test_tf.py` & `sphinxcontrib_terraform-0.2/test/integrated/test_tf.py`

 * *Files identical despite different names*

