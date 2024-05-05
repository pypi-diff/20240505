# Comparing `tmp/collective.volto.formsupport-3.0.1.tar.gz` & `tmp/collective.volto.formsupport-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.volto.formsupport-3.0.1.tar", last modified: Thu Apr 18 08:04:53 2024, max compression
+gzip compressed data, was "collective.volto.formsupport-3.0.2.tar", last modified: Sun May  5 06:38:59 2024, max compression
```

## Comparing `collective.volto.formsupport-3.0.1.tar` & `collective.volto.formsupport-3.0.2.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.666070 collective.volto.formsupport-3.0.1/
--rw-r--r--   0 cekk       (501) staff       (20)     3927 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)      109 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      679 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      117 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)    18224 2024-04-18 08:04:53.666143 collective.volto.formsupport-3.0.1/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)    12962 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/constraints_plone52.txt
--rw-r--r--   0 cekk       (501) staff       (20)       62 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/constraints_plone60.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.656347 collective.volto.formsupport-3.0.1/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7947 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)      107 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)       29 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      334 2024-04-18 08:04:53.666377 collective.volto.formsupport-3.0.1/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     3118 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.652823 collective.volto.formsupport-3.0.1/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.656467 collective.volto.formsupport-3.0.1/src/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.657472 collective.volto.formsupport-3.0.1/src/collective/volto/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.658457 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/
--rw-r--r--   0 cekk       (501) staff       (20)      197 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.658970 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1233 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      452 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/email_confirm_view.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.659078 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/overrides/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/overrides/.gitkeep
--rw-r--r--   0 cekk       (501) staff       (20)      655 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/send_mail_template.pt
--rw-r--r--   0 cekk       (501) staff       (20)     1061 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/send_mail_template_table.pt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.659171 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/static/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/static/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.659264 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/templates/
--rw-r--r--   0 cekk       (501) staff       (20)     9564 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/templates/email_confirm_view.pt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.659999 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/
--rw-r--r--   0 cekk       (501) staff       (20)      288 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1626 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     2224 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/hcaptcha.py
--rw-r--r--   0 cekk       (501) staff       (20)     1469 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/honeypot.py
--rw-r--r--   0 cekk       (501) staff       (20)     2271 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/norobots.py
--rw-r--r--   0 cekk       (501) staff       (20)     2089 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/recaptcha.py
--rw-r--r--   0 cekk       (501) staff       (20)      564 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/vocabularies.py
--rw-r--r--   0 cekk       (501) staff       (20)     1548 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.660334 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3832 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/catalog.py
--rw-r--r--   0 cekk       (501) staff       (20)      595 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1030 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.660887 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     5016 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/collective.volto.formsupport.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.653514 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.661122 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1654 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.mo
--rw-r--r--   0 cekk       (501) staff       (20)     5637 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.653635 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.661348 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     2375 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.mo
--rw-r--r--   0 cekk       (501) staff       (20)     6167 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.653745 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.661580 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     3102 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.mo
--rw-r--r--   0 cekk       (501) staff       (20)     6160 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.653852 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.661810 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1499 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.mo
--rw-r--r--   0 cekk       (501) staff       (20)     5495 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.po
--rw-r--r--   0 cekk       (501) staff       (20)     1778 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      521 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      273 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.654095 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662245 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      209 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      195 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662357 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/registry/
--rw-r--r--   0 cekk       (501) staff       (20)      186 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/registry/main.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662469 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      138 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662670 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      272 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662969 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/deserializer/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/deserializer/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1301 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/deserializer/blocks.py
--rw-r--r--   0 cekk       (501) staff       (20)      426 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/deserializer/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.663277 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1900 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/blocks.py
--rw-r--r--   0 cekk       (501) staff       (20)      449 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.663476 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      233 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.663994 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      942 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/clear.py
--rw-r--r--   0 cekk       (501) staff       (20)     1118 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     3451 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/csv.py
--rw-r--r--   0 cekk       (501) staff       (20)     3930 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/form_data.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.664318 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/submit_form/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/submit_form/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      443 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/submit_form/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)    18588 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/submit_form/post.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.664646 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      689 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     2801 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/email.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.664845 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/scripts/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/scripts/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2538 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/scripts/cleansing.py
--rw-r--r--   0 cekk       (501) staff       (20)      628 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     2827 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.665948 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)    74429 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/file.pdf
--rw-r--r--   0 cekk       (501) staff       (20)    16091 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_captcha.py
--rw-r--r--   0 cekk       (501) staff       (20)     2439 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_deserialize_block.py
--rw-r--r--   0 cekk       (501) staff       (20)     4504 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_event.py
--rw-r--r--   0 cekk       (501) staff       (20)    11327 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_honeypot.py
--rw-r--r--   0 cekk       (501) staff       (20)    46978 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_send_action_form.py
--rw-r--r--   0 cekk       (501) staff       (20)     8854 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_serialize_block.py
--rw-r--r--   0 cekk       (501) staff       (20)     3207 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)    11064 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_store_action_form.py
--rw-r--r--   0 cekk       (501) staff       (20)     8193 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)      940 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/upgrades.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1695 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/utils.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.657369 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)    18224 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     5683 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      214 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       28 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      493 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.888987 collective.volto.formsupport-3.0.2/
+-rw-r--r--   0 cekk       (501) staff       (20)     4058 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      109 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      679 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      117 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)    18355 2024-05-05 06:38:59.889046 collective.volto.formsupport-3.0.2/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)    12962 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/constraints_plone52.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       62 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/constraints_plone60.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.878339 collective.volto.formsupport-3.0.2/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7947 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)      107 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       29 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      334 2024-05-05 06:38:59.889296 collective.volto.formsupport-3.0.2/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     3118 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.874679 collective.volto.formsupport-3.0.2/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.878443 collective.volto.formsupport-3.0.2/src/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.879453 collective.volto.formsupport-3.0.2/src/collective/volto/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.880408 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/
+-rw-r--r--   0 cekk       (501) staff       (20)      197 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.880934 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1233 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      452 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/email_confirm_view.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.881042 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/overrides/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)      655 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/send_mail_template.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1061 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/send_mail_template_table.pt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.881136 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/static/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.881230 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)     9564 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/templates/email_confirm_view.pt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.881984 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/
+-rw-r--r--   0 cekk       (501) staff       (20)      288 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1626 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2224 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/hcaptcha.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1469 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/honeypot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2271 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/norobots.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2089 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/recaptcha.py
+-rw-r--r--   0 cekk       (501) staff       (20)      564 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/vocabularies.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1548 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.882314 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/datamanager/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/datamanager/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3832 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/datamanager/catalog.py
+-rw-r--r--   0 cekk       (501) staff       (20)      595 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/datamanager/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1030 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.882842 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5016 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/collective.volto.formsupport.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.875420 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/de/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.883067 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/de/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1654 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     5637 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.875541 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/es/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.883294 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/es/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     2375 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     6167 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.875653 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.883518 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     3102 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     6160 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.875768 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/pt_BR/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.883745 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1499 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     5495 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1778 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      521 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      273 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.876034 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.884177 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      209 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      195 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.884288 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)      186 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/default/registry/main.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.884394 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      138 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.884631 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      272 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.885026 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/deserializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/deserializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1301 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/deserializer/blocks.py
+-rw-r--r--   0 cekk       (501) staff       (20)      426 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/deserializer/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.885422 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/serializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/serializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1900 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/serializer/blocks.py
+-rw-r--r--   0 cekk       (501) staff       (20)      449 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/serializer/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.885668 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      233 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.886341 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      942 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/clear.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1118 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3451 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/csv.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3930 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/form_data.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.886745 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/submit_form/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/submit_form/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      443 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/submit_form/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)    18618 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/submit_form/post.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.887166 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/validation/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/validation/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      689 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/validation/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2801 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/validation/email.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.887418 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/scripts/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/scripts/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2538 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/scripts/cleansing.py
+-rw-r--r--   0 cekk       (501) staff       (20)      628 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2827 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.888862 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)    74429 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/file.pdf
+-rw-r--r--   0 cekk       (501) staff       (20)    16091 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_captcha.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2439 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_deserialize_block.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4504 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_event.py
+-rw-r--r--   0 cekk       (501) staff       (20)    11327 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_honeypot.py
+-rw-r--r--   0 cekk       (501) staff       (20)    46927 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_send_action_form.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8854 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_serialize_block.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3207 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)    11064 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_store_action_form.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8193 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)      940 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/upgrades.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1695 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/utils.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:38:59.879350 collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)    18355 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     5683 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      214 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       28 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      493 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2024-05-05 06:38:59.000000 collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/top_level.txt
```

### Comparing `collective.volto.formsupport-3.0.1/CHANGES.rst` & `collective.volto.formsupport-3.0.2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+3.0.2 (2024-05-05)
+------------------
+
+- Cleanup all possible HTML in user formitted data and convert it to plain text.
+  [cekk]
+
+
 3.0.1 (2024-04-18)
 ------------------
 
 - Fix README.
   [cekk]
```

### Comparing `collective.volto.formsupport-3.0.1/DEVELOP.rst` & `collective.volto.formsupport-3.0.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/LICENSE.GPL` & `collective.volto.formsupport-3.0.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/LICENSE.rst` & `collective.volto.formsupport-3.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/PKG-INFO` & `collective.volto.formsupport-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.volto.formsupport
-Version: 3.0.1
+Version: 3.0.2
 Summary: Add support for customizable forms in Volto
 Home-page: https://github.com/collective/collective.volto.formsupport
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.volto.formsupport
 Project-URL: Source, https://github.com/collective/collective.volto.formsupport
@@ -396,14 +396,21 @@
 
 - RedTurtle Technology, sviluppo@redturtle.it
 - Mauro Amico, mauro.amico@gmail.com
 
 Changelog
 =========
 
+3.0.2 (2024-05-05)
+------------------
+
+- Cleanup all possible HTML in user formitted data and convert it to plain text.
+  [cekk]
+
+
 3.0.1 (2024-04-18)
 ------------------
 
 - Fix README.
   [cekk]
```

### Comparing `collective.volto.formsupport-3.0.1/README.rst` & `collective.volto.formsupport-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/docs/conf.py` & `collective.volto.formsupport-3.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/setup.py` & `collective.volto.formsupport-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.volto.formsupport",
-    version="3.0.1",
+    version="3.0.2",
     description="Add support for customizable forms in Volto",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/configure.zcml` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/send_mail_template.pt` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/send_mail_template.pt`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/send_mail_template_table.pt` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/send_mail_template_table.pt`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/templates/email_confirm_view.pt` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/browser/templates/email_confirm_view.pt`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/configure.zcml` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/hcaptcha.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/honeypot.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/honeypot.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/norobots.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/norobots.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/recaptcha.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/recaptcha.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/vocabularies.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/captcha/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/configure.zcml` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/catalog.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/datamanager/catalog.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/configure.zcml` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/datamanager/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/interfaces.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/README.rst` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/collective.volto.formsupport.pot` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/collective.volto.formsupport.pot`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.mo` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.mo`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.po` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.po`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.mo` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.mo`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.po` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.po`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.mo` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.mo`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.po` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.po`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.mo` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.mo`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.po` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.po`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/update.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/update.sh` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/deserializer/blocks.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/deserializer/blocks.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/blocks.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/serializer/blocks.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/clear.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/clear.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/configure.zcml` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/csv.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/csv.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/form_data.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/form_data/form_data.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/submit_form/post.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/submit_form/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from plone import api
 from plone.protect.interfaces import IDisableCSRFProtection
 from plone.registry.interfaces import IRegistry
 from plone.restapi.deserializer import json_body
 from plone.restapi.services import Service
 from plone.schema.email import _isemail
 from Products.CMFPlone.interfaces.controlpanel import IMailSchema
-from Products.PortalTransforms.transforms.safe_html import SafeHTML
 from zExceptions import BadRequest
 from zope.component import getMultiAdapter, getUtility
 from zope.event import notify
 from zope.i18n import translate
 from zope.interface import alsoProvides, implementer
 
 from collective.volto.formsupport import _
@@ -90,27 +89,28 @@
         Avoid XSS injections and other attacks.
 
         - cleanup HTML with plone transform
         - remove from data, fields not defined in form schema
         """
         form_data = json_body(self.request)
         fixed_fields = []
-        transform = SafeHTML()
+        transforms = api.portal.get_tool(name="portal_transforms")
+
         block = self.get_block_data(block_id=form_data.get("block_id", ""))
         block_fields = [x.get("field_id", "") for x in block.get("subblocks", [])]
 
         for form_field in form_data.get("data", []):
             if form_field.get("field_id", "") not in block_fields:
                 # unknown field, skip it
                 continue
             new_field = deepcopy(form_field)
             value = new_field.get("value", "")
-            if not isinstance(value, str):
-                continue
-            new_field["value"] = transform.scrub_html(value)
+            if isinstance(value, str):
+                stream = transforms.convertTo("text/plain", value, mimetype="text/html")
+                new_field["value"] = stream.getData().strip()
             fixed_fields.append(new_field)
         form_data["data"] = fixed_fields
         return form_data
 
     def validate_form(self):
         """
         check all required fields and parameters
```

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/configure.zcml` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/validation/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/email.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/restapi/services/validation/email.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/scripts/cleansing.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/scripts/cleansing.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/setuphandlers.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/testing.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/testing.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/file.pdf` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_captcha.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_captcha.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_deserialize_block.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_deserialize_block.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_event.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_honeypot.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_honeypot.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_send_action_form.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_send_action_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -1298,15 +1298,15 @@
         self.assertIn("Subject: test subject", msg)
         self.assertIn("From: john@doe.com", msg)
         self.assertIn("To: site_addr@plone.com", msg)
         self.assertIn("Reply-To: john@doe.com", msg)
         self.assertIn("<strong>Message:</strong> just want to say hi", msg)
         self.assertIn("<strong>Name:</strong> John", msg)
 
-    def test_cleanup_nasy_html_tags_with_portal_transforms(self):
+    def test_cleanup_html_in_submitted_data(self):
         """
         This is needed for confirm message
         """
         self.document.blocks = {
             "form-id": {
                 "@type": "form",
                 "send": ["recipient"],
@@ -1342,34 +1342,33 @@
                 "subject": "test subject",
                 "block_id": "form-id",
             },
         )
         transaction.commit()
         self.assertEqual(response.status_code, 200)
         res = response.json()
-
         self.assertEqual(
             res,
             {
                 "data": [
                     {
                         "field_id": "message",
                         "label": "Message",
-                        "value": "<b>click here</b><p><i>keep tags</i></p>",
+                        "value": "click here keep tags",
                     },
                     {
                         "field_id": "name",
                         "label": "Name",
-                        "value": " foo",
+                        "value": "alert(‘XSS’)  foo",
                     },
                 ]
             },
         )
         msg = self.mailhost.messages[0]
         if isinstance(msg, bytes) and bytes is not str:
             # Python 3 with Products.MailHost 4.10+
             msg = msg.decode("utf-8")
         self.assertIn(
-            "<strong>Message:</strong> &lt;b&gt;click here&lt;/b&gt;&lt;p&gt;&lt=\r\n;i&gt;keep tags&lt;/i&gt;&lt;/p&gt;",
+            "<strong>Message:</strong> click here keep tags",
             msg,
         )
-        self.assertIn("<strong>Name:</strong>  foo", msg)
+        self.assertIn("<strong>Name:</strong> alert(=E2=80=98XSS=E2=80=99)  foo", msg)
```

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_serialize_block.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_serialize_block.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_setup.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_store_action_form.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/tests/test_store_action_form.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/upgrades.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/upgrades.zcml` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/utils.py` & `collective.volto.formsupport-3.0.2/src/collective/volto/formsupport/utils.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/PKG-INFO` & `collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.volto.formsupport
-Version: 3.0.1
+Version: 3.0.2
 Summary: Add support for customizable forms in Volto
 Home-page: https://github.com/collective/collective.volto.formsupport
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.volto.formsupport
 Project-URL: Source, https://github.com/collective/collective.volto.formsupport
@@ -396,14 +396,21 @@
 
 - RedTurtle Technology, sviluppo@redturtle.it
 - Mauro Amico, mauro.amico@gmail.com
 
 Changelog
 =========
 
+3.0.2 (2024-05-05)
+------------------
+
+- Cleanup all possible HTML in user formitted data and convert it to plain text.
+  [cekk]
+
+
 3.0.1 (2024-04-18)
 ------------------
 
 - Fix README.
   [cekk]
```

### Comparing `collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/SOURCES.txt` & `collective.volto.formsupport-3.0.2/src/collective.volto.formsupport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

