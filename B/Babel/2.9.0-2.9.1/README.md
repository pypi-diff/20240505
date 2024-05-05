# Comparing `tmp/Babel-2.9.0.tar.gz` & `tmp/Babel-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Babel-2.9.0.tar", last modified: Thu Nov 12 09:21:38 2020, max compression
+gzip compressed data, was "Babel-2.9.1.tar", last modified: Wed Apr 28 19:28:20 2021, max compression
```

## Comparing `Babel-2.9.0.tar` & `Babel-2.9.1.tar`

### file list

```diff
@@ -1,954 +1,954 @@
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:38.004105 Babel-2.9.0/
--rw-r--r--   0 akx        (501) staff       (20)     2423 2020-11-12 09:20:39.000000 Babel-2.9.0/AUTHORS
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.521068 Babel-2.9.0/Babel.egg-info/
--rw-r--r--   0 akx        (501) staff       (20)     1202 2020-11-12 09:21:37.000000 Babel-2.9.0/Babel.egg-info/PKG-INFO
--rw-r--r--   0 akx        (501) staff       (20)    25548 2020-11-12 09:21:37.000000 Babel-2.9.0/Babel.egg-info/SOURCES.txt
--rw-r--r--   0 akx        (501) staff       (20)        1 2020-11-12 09:21:37.000000 Babel-2.9.0/Babel.egg-info/dependency_links.txt
--rw-r--r--   0 akx        (501) staff       (20)      764 2020-11-12 09:21:37.000000 Babel-2.9.0/Babel.egg-info/entry_points.txt
--rw-r--r--   0 akx        (501) staff       (20)        1 2020-11-12 09:21:37.000000 Babel-2.9.0/Babel.egg-info/not-zip-safe
--rw-r--r--   0 akx        (501) staff       (20)       13 2020-11-12 09:21:37.000000 Babel-2.9.0/Babel.egg-info/requires.txt
--rw-r--r--   0 akx        (501) staff       (20)        6 2020-11-12 09:21:37.000000 Babel-2.9.0/Babel.egg-info/top_level.txt
--rw-r--r--   0 akx        (501) staff       (20)    30738 2020-11-12 09:20:39.000000 Babel-2.9.0/CHANGES
--rw-r--r--   0 akx        (501) staff       (20)     1451 2020-11-11 12:00:33.000000 Babel-2.9.0/LICENSE
--rw-r--r--   0 akx        (501) staff       (20)      287 2016-11-19 14:05:40.000000 Babel-2.9.0/MANIFEST.in
--rw-r--r--   0 akx        (501) staff       (20)     1337 2019-05-27 11:55:14.000000 Babel-2.9.0/Makefile
--rw-r--r--   0 akx        (501) staff       (20)     1202 2020-11-12 09:21:38.005276 Babel-2.9.0/PKG-INFO
--rw-r--r--   0 akx        (501) staff       (20)      829 2018-02-02 16:29:02.000000 Babel-2.9.0/README.rst
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.530055 Babel-2.9.0/babel/
--rw-r--r--   0 akx        (501) staff       (20)      714 2020-11-12 09:20:39.000000 Babel-2.9.0/babel/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)     1685 2019-02-20 13:12:21.000000 Babel-2.9.0/babel/_compat.py
--rw-r--r--   0 akx        (501) staff       (20)    36907 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/core.py
--rw-r--r--   0 akx        (501) staff       (20)    67709 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/dates.py
--rw-r--r--   0 akx        (501) staff       (20)   254421 2020-11-12 09:21:19.000000 Babel-2.9.0/babel/global.dat
--rw-r--r--   0 akx        (501) staff       (20)     2743 2018-07-20 10:31:17.000000 Babel-2.9.0/babel/languages.py
--rw-r--r--   0 akx        (501) staff       (20)     2719 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/lists.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.927701 Babel-2.9.0/babel/locale-data/
--rw-r--r--   0 akx        (501) staff       (20)   171143 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/af.dat
--rw-r--r--   0 akx        (501) staff       (20)     1407 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/af_NA.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/af_ZA.dat
--rw-r--r--   0 akx        (501) staff       (20)    17339 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/agq.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/agq_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)    15859 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/ak.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ak_GH.dat
--rw-r--r--   0 akx        (501) staff       (20)   200581 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/am.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/am_ET.dat
--rw-r--r--   0 akx        (501) staff       (20)   345779 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/ar.dat
--rw-r--r--   0 akx        (501) staff       (20)     1680 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_001.dat
--rw-r--r--   0 akx        (501) staff       (20)     1038 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_AE.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_BH.dat
--rw-r--r--   0 akx        (501) staff       (20)      629 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_DJ.dat
--rw-r--r--   0 akx        (501) staff       (20)     1713 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_DZ.dat
--rw-r--r--   0 akx        (501) staff       (20)      688 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_EG.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_EH.dat
--rw-r--r--   0 akx        (501) staff       (20)      610 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_ER.dat
--rw-r--r--   0 akx        (501) staff       (20)     1195 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_IL.dat
--rw-r--r--   0 akx        (501) staff       (20)     2336 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_IQ.dat
--rw-r--r--   0 akx        (501) staff       (20)     2335 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_JO.dat
--rw-r--r--   0 akx        (501) staff       (20)     1161 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_KM.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_KW.dat
--rw-r--r--   0 akx        (501) staff       (20)     2336 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_LB.dat
--rw-r--r--   0 akx        (501) staff       (20)     1652 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_LY.dat
--rw-r--r--   0 akx        (501) staff       (20)     2007 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_MA.dat
--rw-r--r--   0 akx        (501) staff       (20)     2173 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_MR.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_OM.dat
--rw-r--r--   0 akx        (501) staff       (20)     2273 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_PS.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_QA.dat
--rw-r--r--   0 akx        (501) staff       (20)    30599 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_SA.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_SD.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_SO.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_SS.dat
--rw-r--r--   0 akx        (501) staff       (20)     2335 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_SY.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_TD.dat
--rw-r--r--   0 akx        (501) staff       (20)     1651 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ar_TN.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ar_YE.dat
--rw-r--r--   0 akx        (501) staff       (20)   234427 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/as.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/as_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)    16187 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/asa.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/asa_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)   209617 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ast.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ast_ES.dat
--rw-r--r--   0 akx        (501) staff       (20)   194898 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/az.dat
--rw-r--r--   0 akx        (501) staff       (20)    38880 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/az_Cyrl.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/az_Cyrl_AZ.dat
--rw-r--r--   0 akx        (501) staff       (20)     2225 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/az_Latn.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/az_Latn_AZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    17128 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/bas.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bas_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)   271438 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/be.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/be_BY.dat
--rw-r--r--   0 akx        (501) staff       (20)     6534 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/bem.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bem_ZM.dat
--rw-r--r--   0 akx        (501) staff       (20)    16977 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/bez.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bez_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)   232833 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/bg.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/bg_BG.dat
--rw-r--r--   0 akx        (501) staff       (20)    15886 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/bm.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bm_ML.dat
--rw-r--r--   0 akx        (501) staff       (20)   263365 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/bn.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bn_BD.dat
--rw-r--r--   0 akx        (501) staff       (20)      866 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/bn_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)    22525 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/bo.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bo_CN.dat
--rw-r--r--   0 akx        (501) staff       (20)      704 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bo_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   290897 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/br.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/br_FR.dat
--rw-r--r--   0 akx        (501) staff       (20)   124289 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/brx.dat
--rw-r--r--   0 akx        (501) staff       (20)      632 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/brx_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   239326 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/bs.dat
--rw-r--r--   0 akx        (501) staff       (20)   213685 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bs_Cyrl.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bs_Cyrl_BA.dat
--rw-r--r--   0 akx        (501) staff       (20)     1957 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bs_Latn.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/bs_Latn_BA.dat
--rw-r--r--   0 akx        (501) staff       (20)   208790 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/ca.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ca_AD.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ca_ES.dat
--rw-r--r--   0 akx        (501) staff       (20)     3644 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ca_ES_VALENCIA.dat
--rw-r--r--   0 akx        (501) staff       (20)      645 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ca_FR.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ca_IT.dat
--rw-r--r--   0 akx        (501) staff       (20)   275655 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ccp.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ccp_BD.dat
--rw-r--r--   0 akx        (501) staff       (20)      632 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ccp_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   138778 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/ce.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ce_RU.dat
--rw-r--r--   0 akx        (501) staff       (20)   103518 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/ceb.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ceb_PH.dat
--rw-r--r--   0 akx        (501) staff       (20)    16228 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/cgg.dat
--rw-r--r--   0 akx        (501) staff       (20)      613 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/cgg_UG.dat
--rw-r--r--   0 akx        (501) staff       (20)   200072 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/chr.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/chr_US.dat
--rw-r--r--   0 akx        (501) staff       (20)    41606 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ckb.dat
--rw-r--r--   0 akx        (501) staff       (20)      652 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ckb_IQ.dat
--rw-r--r--   0 akx        (501) staff       (20)     1204 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ckb_IR.dat
--rw-r--r--   0 akx        (501) staff       (20)   297675 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/cs.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/cs_CZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    20265 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/cu.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/cu_RU.dat
--rw-r--r--   0 akx        (501) staff       (20)   315824 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/cy.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/cy_GB.dat
--rw-r--r--   0 akx        (501) staff       (20)   199867 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/da.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/da_DK.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/da_GL.dat
--rw-r--r--   0 akx        (501) staff       (20)    16271 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/dav.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/dav_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)   206762 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/de.dat
--rw-r--r--   0 akx        (501) staff       (20)     2563 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/de_AT.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/de_BE.dat
--rw-r--r--   0 akx        (501) staff       (20)     3938 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/de_CH.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/de_DE.dat
--rw-r--r--   0 akx        (501) staff       (20)     1619 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/de_IT.dat
--rw-r--r--   0 akx        (501) staff       (20)     1321 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/de_LI.dat
--rw-r--r--   0 akx        (501) staff       (20)     1065 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/de_LU.dat
--rw-r--r--   0 akx        (501) staff       (20)    16192 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/dje.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/dje_NE.dat
--rw-r--r--   0 akx        (501) staff       (20)   179644 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/dsb.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/dsb_DE.dat
--rw-r--r--   0 akx        (501) staff       (20)     5355 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/dua.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/dua_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)    10541 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/dyo.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/dyo_SN.dat
--rw-r--r--   0 akx        (501) staff       (20)    89908 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/dz.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/dz_BT.dat
--rw-r--r--   0 akx        (501) staff       (20)    16243 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/ebu.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ebu_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)   142527 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/ee.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ee_GH.dat
--rw-r--r--   0 akx        (501) staff       (20)     1141 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ee_TG.dat
--rw-r--r--   0 akx        (501) staff       (20)   244752 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/el.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/el_CY.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/el_GR.dat
--rw-r--r--   0 akx        (501) staff       (20)   194682 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/en.dat
--rw-r--r--   0 akx        (501) staff       (20)    27063 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_001.dat
--rw-r--r--   0 akx        (501) staff       (20)     1765 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_150.dat
--rw-r--r--   0 akx        (501) staff       (20)     4111 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_AE.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_AG.dat
--rw-r--r--   0 akx        (501) staff       (20)     1179 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_AI.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_AS.dat
--rw-r--r--   0 akx        (501) staff       (20)     1200 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_AT.dat
--rw-r--r--   0 akx        (501) staff       (20)    23385 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_AU.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_BB.dat
--rw-r--r--   0 akx        (501) staff       (20)     1493 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_BE.dat
--rw-r--r--   0 akx        (501) staff       (20)     1162 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_BI.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_BM.dat
--rw-r--r--   0 akx        (501) staff       (20)      811 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_BS.dat
--rw-r--r--   0 akx        (501) staff       (20)     2771 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_BW.dat
--rw-r--r--   0 akx        (501) staff       (20)     2950 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_BZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    25449 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_CA.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_CC.dat
--rw-r--r--   0 akx        (501) staff       (20)     1100 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_CH.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_CK.dat
--rw-r--r--   0 akx        (501) staff       (20)     1410 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_CX.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_CY.dat
--rw-r--r--   0 akx        (501) staff       (20)      952 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_DE.dat
--rw-r--r--   0 akx        (501) staff       (20)     1141 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_DG.dat
--rw-r--r--   0 akx        (501) staff       (20)     2350 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_DK.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_DM.dat
--rw-r--r--   0 akx        (501) staff       (20)      860 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_ER.dat
--rw-r--r--   0 akx        (501) staff       (20)     2282 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_FI.dat
--rw-r--r--   0 akx        (501) staff       (20)      645 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_FJ.dat
--rw-r--r--   0 akx        (501) staff       (20)     1183 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_FK.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_FM.dat
--rw-r--r--   0 akx        (501) staff       (20)    25821 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_GB.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_GD.dat
--rw-r--r--   0 akx        (501) staff       (20)     1246 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_GG.dat
--rw-r--r--   0 akx        (501) staff       (20)      862 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_GH.dat
--rw-r--r--   0 akx        (501) staff       (20)     1201 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_GI.dat
--rw-r--r--   0 akx        (501) staff       (20)      858 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_GM.dat
--rw-r--r--   0 akx        (501) staff       (20)      688 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_GU.dat
--rw-r--r--   0 akx        (501) staff       (20)      667 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_GY.dat
--rw-r--r--   0 akx        (501) staff       (20)     2008 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_HK.dat
--rw-r--r--   0 akx        (501) staff       (20)     2043 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_IE.dat
--rw-r--r--   0 akx        (501) staff       (20)     1397 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_IL.dat
--rw-r--r--   0 akx        (501) staff       (20)     1246 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_IM.dat
--rw-r--r--   0 akx        (501) staff       (20)     3767 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)     1141 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_IO.dat
--rw-r--r--   0 akx        (501) staff       (20)     1246 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_JE.dat
--rw-r--r--   0 akx        (501) staff       (20)     1599 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_JM.dat
--rw-r--r--   0 akx        (501) staff       (20)     1431 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_KI.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_KN.dat
--rw-r--r--   0 akx        (501) staff       (20)      792 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_KY.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_LC.dat
--rw-r--r--   0 akx        (501) staff       (20)      858 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_LR.dat
--rw-r--r--   0 akx        (501) staff       (20)      858 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_LS.dat
--rw-r--r--   0 akx        (501) staff       (20)     1411 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_MG.dat
--rw-r--r--   0 akx        (501) staff       (20)     1341 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_MH.dat
--rw-r--r--   0 akx        (501) staff       (20)      803 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_MO.dat
--rw-r--r--   0 akx        (501) staff       (20)     1322 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_MP.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_MS.dat
--rw-r--r--   0 akx        (501) staff       (20)     1927 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_MT.dat
--rw-r--r--   0 akx        (501) staff       (20)     1411 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_MU.dat
--rw-r--r--   0 akx        (501) staff       (20)      859 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_MW.dat
--rw-r--r--   0 akx        (501) staff       (20)      689 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_MY.dat
--rw-r--r--   0 akx        (501) staff       (20)      858 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_NA.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_NF.dat
--rw-r--r--   0 akx        (501) staff       (20)     1412 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_NG.dat
--rw-r--r--   0 akx        (501) staff       (20)     1097 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_NL.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_NR.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_NU.dat
--rw-r--r--   0 akx        (501) staff       (20)     2234 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_NZ.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_PG.dat
--rw-r--r--   0 akx        (501) staff       (20)      629 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_PH.dat
--rw-r--r--   0 akx        (501) staff       (20)     1959 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_PK.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_PN.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_PR.dat
--rw-r--r--   0 akx        (501) staff       (20)      773 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_PW.dat
--rw-r--r--   0 akx        (501) staff       (20)     1411 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_RW.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_SB.dat
--rw-r--r--   0 akx        (501) staff       (20)     1161 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_SC.dat
--rw-r--r--   0 akx        (501) staff       (20)      901 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_SD.dat
--rw-r--r--   0 akx        (501) staff       (20)     1427 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_SE.dat
--rw-r--r--   0 akx        (501) staff       (20)     2017 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_SG.dat
--rw-r--r--   0 akx        (501) staff       (20)     1183 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_SH.dat
--rw-r--r--   0 akx        (501) staff       (20)      968 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_SI.dat
--rw-r--r--   0 akx        (501) staff       (20)      859 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_SL.dat
--rw-r--r--   0 akx        (501) staff       (20)      881 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_SS.dat
--rw-r--r--   0 akx        (501) staff       (20)     1163 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_SX.dat
--rw-r--r--   0 akx        (501) staff       (20)      858 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_SZ.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_TC.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_TK.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_TO.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_TT.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_TV.dat
--rw-r--r--   0 akx        (501) staff       (20)     1412 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)     1435 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_UG.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_UM.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_US.dat
--rw-r--r--   0 akx        (501) staff       (20)     1204 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_US_POSIX.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_VC.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/en_VG.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_VI.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_VU.dat
--rw-r--r--   0 akx        (501) staff       (20)      629 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_WS.dat
--rw-r--r--   0 akx        (501) staff       (20)     3269 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_ZA.dat
--rw-r--r--   0 akx        (501) staff       (20)      858 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_ZM.dat
--rw-r--r--   0 akx        (501) staff       (20)     3199 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/en_ZW.dat
--rw-r--r--   0 akx        (501) staff       (20)    40689 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/eo.dat
--rw-r--r--   0 akx        (501) staff       (20)      823 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/eo_001.dat
--rw-r--r--   0 akx        (501) staff       (20)   199638 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/es.dat
--rw-r--r--   0 akx        (501) staff       (20)    23299 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_419.dat
--rw-r--r--   0 akx        (501) staff       (20)     8828 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_AR.dat
--rw-r--r--   0 akx        (501) staff       (20)     1888 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_BO.dat
--rw-r--r--   0 akx        (501) staff       (20)      628 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_BR.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_BZ.dat
--rw-r--r--   0 akx        (501) staff       (20)     5128 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_CL.dat
--rw-r--r--   0 akx        (501) staff       (20)     8665 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_CO.dat
--rw-r--r--   0 akx        (501) staff       (20)     1719 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_CR.dat
--rw-r--r--   0 akx        (501) staff       (20)      629 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_CU.dat
--rw-r--r--   0 akx        (501) staff       (20)     4020 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_DO.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_EA.dat
--rw-r--r--   0 akx        (501) staff       (20)     3294 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_EC.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_ES.dat
--rw-r--r--   0 akx        (501) staff       (20)      872 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_GQ.dat
--rw-r--r--   0 akx        (501) staff       (20)     4896 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_GT.dat
--rw-r--r--   0 akx        (501) staff       (20)     3476 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_HN.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_IC.dat
--rw-r--r--   0 akx        (501) staff       (20)    24708 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_MX.dat
--rw-r--r--   0 akx        (501) staff       (20)     1653 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_NI.dat
--rw-r--r--   0 akx        (501) staff       (20)     3884 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_PA.dat
--rw-r--r--   0 akx        (501) staff       (20)     4848 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_PE.dat
--rw-r--r--   0 akx        (501) staff       (20)     1205 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_PH.dat
--rw-r--r--   0 akx        (501) staff       (20)     3798 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_PR.dat
--rw-r--r--   0 akx        (501) staff       (20)     5319 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_PY.dat
--rw-r--r--   0 akx        (501) staff       (20)     1402 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_SV.dat
--rw-r--r--   0 akx        (501) staff       (20)    25343 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/es_US.dat
--rw-r--r--   0 akx        (501) staff       (20)     2540 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_UY.dat
--rw-r--r--   0 akx        (501) staff       (20)     3752 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/es_VE.dat
--rw-r--r--   0 akx        (501) staff       (20)   200192 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/et.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/et_EE.dat
--rw-r--r--   0 akx        (501) staff       (20)   176850 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/eu.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/eu_ES.dat
--rw-r--r--   0 akx        (501) staff       (20)    17595 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ewo.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ewo_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)   217724 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/fa.dat
--rw-r--r--   0 akx        (501) staff       (20)    11247 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fa_AF.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fa_IR.dat
--rw-r--r--   0 akx        (501) staff       (20)    16084 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/ff.dat
--rw-r--r--   0 akx        (501) staff       (20)   174659 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm.dat
--rw-r--r--   0 akx        (501) staff       (20)      610 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_BF.dat
--rw-r--r--   0 akx        (501) staff       (20)      629 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)     1209 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_GH.dat
--rw-r--r--   0 akx        (501) staff       (20)     1205 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_GM.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_GN.dat
--rw-r--r--   0 akx        (501) staff       (20)      610 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_GW.dat
--rw-r--r--   0 akx        (501) staff       (20)     1205 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_LR.dat
--rw-r--r--   0 akx        (501) staff       (20)     1206 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_MR.dat
--rw-r--r--   0 akx        (501) staff       (20)      610 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_NE.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_NG.dat
--rw-r--r--   0 akx        (501) staff       (20)     1206 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_SL.dat
--rw-r--r--   0 akx        (501) staff       (20)      610 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Adlm_SN.dat
--rw-r--r--   0 akx        (501) staff       (20)      839 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_BF.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)     1188 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_GH.dat
--rw-r--r--   0 akx        (501) staff       (20)     1184 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_GM.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_GN.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_GW.dat
--rw-r--r--   0 akx        (501) staff       (20)     1184 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_LR.dat
--rw-r--r--   0 akx        (501) staff       (20)     1185 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_MR.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_NE.dat
--rw-r--r--   0 akx        (501) staff       (20)      610 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_NG.dat
--rw-r--r--   0 akx        (501) staff       (20)     1185 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_SL.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ff_Latn_SN.dat
--rw-r--r--   0 akx        (501) staff       (20)   227195 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/fi.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fi_FI.dat
--rw-r--r--   0 akx        (501) staff       (20)   179405 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fil.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fil_PH.dat
--rw-r--r--   0 akx        (501) staff       (20)   165657 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/fo.dat
--rw-r--r--   0 akx        (501) staff       (20)      647 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fo_DK.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fo_FO.dat
--rw-r--r--   0 akx        (501) staff       (20)   225342 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/fr.dat
--rw-r--r--   0 akx        (501) staff       (20)     1254 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_BE.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_BF.dat
--rw-r--r--   0 akx        (501) staff       (20)      610 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_BI.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_BJ.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_BL.dat
--rw-r--r--   0 akx        (501) staff       (20)    65858 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_CA.dat
--rw-r--r--   0 akx        (501) staff       (20)     1106 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_CD.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_CF.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_CG.dat
--rw-r--r--   0 akx        (501) staff       (20)     2970 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_CH.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_CI.dat
--rw-r--r--   0 akx        (501) staff       (20)     2083 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)     1205 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_DJ.dat
--rw-r--r--   0 akx        (501) staff       (20)     1247 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_DZ.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_FR.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_GA.dat
--rw-r--r--   0 akx        (501) staff       (20)      692 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_GF.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_GN.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_GP.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_GQ.dat
--rw-r--r--   0 akx        (501) staff       (20)     1873 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_HT.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_KM.dat
--rw-r--r--   0 akx        (501) staff       (20)      687 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_LU.dat
--rw-r--r--   0 akx        (501) staff       (20)     1277 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_MA.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_MC.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_MF.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_MG.dat
--rw-r--r--   0 akx        (501) staff       (20)     1126 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_ML.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_MQ.dat
--rw-r--r--   0 akx        (501) staff       (20)     1185 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_MR.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_MU.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_NC.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_NE.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_PF.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_PM.dat
--rw-r--r--   0 akx        (501) staff       (20)     1142 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_RE.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_RW.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_SC.dat
--rw-r--r--   0 akx        (501) staff       (20)     1277 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_SN.dat
--rw-r--r--   0 akx        (501) staff       (20)     1247 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_SY.dat
--rw-r--r--   0 akx        (501) staff       (20)     1165 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_TD.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_TG.dat
--rw-r--r--   0 akx        (501) staff       (20)     1185 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_TN.dat
--rw-r--r--   0 akx        (501) staff       (20)     1185 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_VU.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fr_WF.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fr_YT.dat
--rw-r--r--   0 akx        (501) staff       (20)    35027 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fur.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/fur_IT.dat
--rw-r--r--   0 akx        (501) staff       (20)   110221 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/fy.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/fy_NL.dat
--rw-r--r--   0 akx        (501) staff       (20)   316865 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/ga.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ga_GB.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ga_IE.dat
--rw-r--r--   0 akx        (501) staff       (20)   302010 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/gd.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/gd_GB.dat
--rw-r--r--   0 akx        (501) staff       (20)   176367 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/gl.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/gl_ES.dat
--rw-r--r--   0 akx        (501) staff       (20)   108049 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/gsw.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/gsw_CH.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/gsw_FR.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/gsw_LI.dat
--rw-r--r--   0 akx        (501) staff       (20)   246649 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/gu.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/gu_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)    16016 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/guz.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/guz_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)     4146 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/gv.dat
--rw-r--r--   0 akx        (501) staff       (20)      607 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/gv_IM.dat
--rw-r--r--   0 akx        (501) staff       (20)    78016 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/ha.dat
--rw-r--r--   0 akx        (501) staff       (20)     1188 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ha_GH.dat
--rw-r--r--   0 akx        (501) staff       (20)     1248 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ha_NE.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ha_NG.dat
--rw-r--r--   0 akx        (501) staff       (20)    16106 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/haw.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/haw_US.dat
--rw-r--r--   0 akx        (501) staff       (20)   271008 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/he.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/he_IL.dat
--rw-r--r--   0 akx        (501) staff       (20)   244568 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/hi.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/hi_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   247517 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/hr.dat
--rw-r--r--   0 akx        (501) staff       (20)     1161 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/hr_BA.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/hr_HR.dat
--rw-r--r--   0 akx        (501) staff       (20)   179178 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/hsb.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/hsb_DE.dat
--rw-r--r--   0 akx        (501) staff       (20)   192963 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/hu.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/hu_HU.dat
--rw-r--r--   0 akx        (501) staff       (20)   214313 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/hy.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/hy_AM.dat
--rw-r--r--   0 akx        (501) staff       (20)   112822 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/ia.dat
--rw-r--r--   0 akx        (501) staff       (20)      914 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ia_001.dat
--rw-r--r--   0 akx        (501) staff       (20)   163265 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/id.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/id_ID.dat
--rw-r--r--   0 akx        (501) staff       (20)    52036 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/ig.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ig_NG.dat
--rw-r--r--   0 akx        (501) staff       (20)    12588 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/ii.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ii_CN.dat
--rw-r--r--   0 akx        (501) staff       (20)   188046 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/is.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/is_IS.dat
--rw-r--r--   0 akx        (501) staff       (20)   188460 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/it.dat
--rw-r--r--   0 akx        (501) staff       (20)     2776 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/it_CH.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/it_IT.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/it_SM.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/it_VA.dat
--rw-r--r--   0 akx        (501) staff       (20)   200287 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/ja.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ja_JP.dat
--rw-r--r--   0 akx        (501) staff       (20)    12628 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/jgo.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/jgo_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)    16068 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/jmc.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/jmc_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)   129461 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/jv.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/jv_ID.dat
--rw-r--r--   0 akx        (501) staff       (20)   260705 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/ka.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ka_GE.dat
--rw-r--r--   0 akx        (501) staff       (20)   135263 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/kab.dat
--rw-r--r--   0 akx        (501) staff       (20)      652 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kab_DZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    16175 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/kam.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kam_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)    16475 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/kde.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kde_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    85757 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/kea.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kea_CV.dat
--rw-r--r--   0 akx        (501) staff       (20)    15939 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/khq.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/khq_ML.dat
--rw-r--r--   0 akx        (501) staff       (20)    16123 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/ki.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ki_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)   210242 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/kk.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kk_KZ.dat
--rw-r--r--   0 akx        (501) staff       (20)     4888 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/kkj.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kkj_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)    58200 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/kl.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kl_GL.dat
--rw-r--r--   0 akx        (501) staff       (20)    18003 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/kln.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kln_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)   202267 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/km.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/km_KH.dat
--rw-r--r--   0 akx        (501) staff       (20)   263580 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/kn.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/kn_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   175158 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/ko.dat
--rw-r--r--   0 akx        (501) staff       (20)      789 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ko_KP.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ko_KR.dat
--rw-r--r--   0 akx        (501) staff       (20)   182871 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/kok.dat
--rw-r--r--   0 akx        (501) staff       (20)      632 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kok_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   102570 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/ks.dat
--rw-r--r--   0 akx        (501) staff       (20)      823 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ks_Arab.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ks_Arab_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)    16043 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/ksb.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ksb_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    16515 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/ksf.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ksf_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)    88937 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ksh.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ksh_DE.dat
--rw-r--r--   0 akx        (501) staff       (20)    28771 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/ku.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ku_TR.dat
--rw-r--r--   0 akx        (501) staff       (20)     7242 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/kw.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/kw_GB.dat
--rw-r--r--   0 akx        (501) staff       (20)   202058 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/ky.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ky_KG.dat
--rw-r--r--   0 akx        (501) staff       (20)    17141 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/lag.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/lag_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)   164597 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/lb.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/lb_LU.dat
--rw-r--r--   0 akx        (501) staff       (20)    16434 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/lg.dat
--rw-r--r--   0 akx        (501) staff       (20)      612 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/lg_UG.dat
--rw-r--r--   0 akx        (501) staff       (20)    12766 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/lkt.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/lkt_US.dat
--rw-r--r--   0 akx        (501) staff       (20)    25891 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/ln.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ln_AO.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ln_CD.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ln_CF.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ln_CG.dat
--rw-r--r--   0 akx        (501) staff       (20)   220343 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/lo.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/lo_LA.dat
--rw-r--r--   0 akx        (501) staff       (20)    19021 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/lrc.dat
--rw-r--r--   0 akx        (501) staff       (20)     1228 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/lrc_IQ.dat
--rw-r--r--   0 akx        (501) staff       (20)      652 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/lrc_IR.dat
--rw-r--r--   0 akx        (501) staff       (20)   284211 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/lt.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/lt_LT.dat
--rw-r--r--   0 akx        (501) staff       (20)    15888 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/lu.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/lu_CD.dat
--rw-r--r--   0 akx        (501) staff       (20)    15885 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/luo.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/luo_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)    15859 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/luy.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/luy_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)   214988 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/lv.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/lv_LV.dat
--rw-r--r--   0 akx        (501) staff       (20)    14710 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/mai.dat
--rw-r--r--   0 akx        (501) staff       (20)      632 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mai_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)    17297 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/mas.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mas_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)      611 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mas_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    16088 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/mer.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mer_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)    15117 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/mfe.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mfe_MU.dat
--rw-r--r--   0 akx        (501) staff       (20)    23550 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/mg.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/mg_MG.dat
--rw-r--r--   0 akx        (501) staff       (20)    10479 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/mgh.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mgh_MZ.dat
--rw-r--r--   0 akx        (501) staff       (20)     8206 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/mgo.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mgo_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)    20727 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/mi.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mi_NZ.dat
--rw-r--r--   0 akx        (501) staff       (20)   234490 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/mk.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mk_MK.dat
--rw-r--r--   0 akx        (501) staff       (20)   285214 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/ml.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ml_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   202642 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/mn.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mn_MN.dat
--rw-r--r--   0 akx        (501) staff       (20)    14622 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/mni.dat
--rw-r--r--   0 akx        (501) staff       (20)      666 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mni_Beng.dat
--rw-r--r--   0 akx        (501) staff       (20)      632 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mni_Beng_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   246797 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/mr.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mr_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   152238 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/ms.dat
--rw-r--r--   0 akx        (501) staff       (20)     1257 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ms_BN.dat
--rw-r--r--   0 akx        (501) staff       (20)     3272 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ms_ID.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ms_MY.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ms_SG.dat
--rw-r--r--   0 akx        (501) staff       (20)    78243 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/mt.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mt_MT.dat
--rw-r--r--   0 akx        (501) staff       (20)    16547 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/mua.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mua_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)   210242 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/my.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/my_MM.dat
--rw-r--r--   0 akx        (501) staff       (20)    65499 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/mzn.dat
--rw-r--r--   0 akx        (501) staff       (20)      652 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/mzn_IR.dat
--rw-r--r--   0 akx        (501) staff       (20)    16617 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/naq.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/naq_NA.dat
--rw-r--r--   0 akx        (501) staff       (20)   210593 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/nb.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nb_NO.dat
--rw-r--r--   0 akx        (501) staff       (20)      607 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nb_SJ.dat
--rw-r--r--   0 akx        (501) staff       (20)    16312 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/nd.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nd_ZW.dat
--rw-r--r--   0 akx        (501) staff       (20)    50632 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/nds.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nds_DE.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nds_NL.dat
--rw-r--r--   0 akx        (501) staff       (20)   248497 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/ne.dat
--rw-r--r--   0 akx        (501) staff       (20)     1265 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ne_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ne_NP.dat
--rw-r--r--   0 akx        (501) staff       (20)   215801 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/nl.dat
--rw-r--r--   0 akx        (501) staff       (20)      611 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nl_AW.dat
--rw-r--r--   0 akx        (501) staff       (20)     1835 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/nl_BE.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/nl_BQ.dat
--rw-r--r--   0 akx        (501) staff       (20)      611 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/nl_CW.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nl_NL.dat
--rw-r--r--   0 akx        (501) staff       (20)      669 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nl_SR.dat
--rw-r--r--   0 akx        (501) staff       (20)      611 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nl_SX.dat
--rw-r--r--   0 akx        (501) staff       (20)    16189 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/nmg.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nmg_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)   179884 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/nn.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nn_NO.dat
--rw-r--r--   0 akx        (501) staff       (20)     6766 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/nnh.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nnh_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)     9153 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/nus.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nus_SS.dat
--rw-r--r--   0 akx        (501) staff       (20)    16275 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/nyn.dat
--rw-r--r--   0 akx        (501) staff       (20)      613 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/nyn_UG.dat
--rw-r--r--   0 akx        (501) staff       (20)    16588 2020-11-12 09:21:19.000000 Babel-2.9.0/babel/locale-data/om.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/om_ET.dat
--rw-r--r--   0 akx        (501) staff       (20)     1566 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/om_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)   241213 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/or.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/or_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)    17627 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/os.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/os_GE.dat
--rw-r--r--   0 akx        (501) staff       (20)      668 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/os_RU.dat
--rw-r--r--   0 akx        (501) staff       (20)   244684 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/pa.dat
--rw-r--r--   0 akx        (501) staff       (20)     3984 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pa_Arab.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pa_Arab_PK.dat
--rw-r--r--   0 akx        (501) staff       (20)     1249 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pa_Guru.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pa_Guru_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)   174311 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/pcm.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pcm_NG.dat
--rw-r--r--   0 akx        (501) staff       (20)   236139 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/pl.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pl_PL.dat
--rw-r--r--   0 akx        (501) staff       (20)    20167 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/prg.dat
--rw-r--r--   0 akx        (501) staff       (20)     1567 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/prg_001.dat
--rw-r--r--   0 akx        (501) staff       (20)   180248 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/ps.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ps_AF.dat
--rw-r--r--   0 akx        (501) staff       (20)     7954 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ps_PK.dat
--rw-r--r--   0 akx        (501) staff       (20)   195079 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/pt.dat
--rw-r--r--   0 akx        (501) staff       (20)      995 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_AO.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/pt_BR.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_CH.dat
--rw-r--r--   0 akx        (501) staff       (20)     1015 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_CV.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_GQ.dat
--rw-r--r--   0 akx        (501) staff       (20)      975 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_GW.dat
--rw-r--r--   0 akx        (501) staff       (20)      645 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_LU.dat
--rw-r--r--   0 akx        (501) staff       (20)     1592 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_MO.dat
--rw-r--r--   0 akx        (501) staff       (20)     1015 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_MZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    99144 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/pt_PT.dat
--rw-r--r--   0 akx        (501) staff       (20)      995 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_ST.dat
--rw-r--r--   0 akx        (501) staff       (20)      975 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/pt_TL.dat
--rw-r--r--   0 akx        (501) staff       (20)   107964 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/qu.dat
--rw-r--r--   0 akx        (501) staff       (20)      836 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/qu_BO.dat
--rw-r--r--   0 akx        (501) staff       (20)      810 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/qu_EC.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/qu_PE.dat
--rw-r--r--   0 akx        (501) staff       (20)    67934 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/rm.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/rm_CH.dat
--rw-r--r--   0 akx        (501) staff       (20)    16781 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/rn.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/rn_BI.dat
--rw-r--r--   0 akx        (501) staff       (20)   225782 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/ro.dat
--rw-r--r--   0 akx        (501) staff       (20)     3215 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ro_MD.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ro_RO.dat
--rw-r--r--   0 akx        (501) staff       (20)    16170 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/rof.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/rof_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    42432 2020-11-12 09:21:19.000000 Babel-2.9.0/babel/locale-data/root.dat
--rw-r--r--   0 akx        (501) staff       (20)   305212 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/ru.dat
--rw-r--r--   0 akx        (501) staff       (20)      649 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ru_BY.dat
--rw-r--r--   0 akx        (501) staff       (20)      632 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ru_KG.dat
--rw-r--r--   0 akx        (501) staff       (20)      629 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ru_KZ.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ru_MD.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ru_RU.dat
--rw-r--r--   0 akx        (501) staff       (20)     1747 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ru_UA.dat
--rw-r--r--   0 akx        (501) staff       (20)    16215 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/rw.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/rw_RW.dat
--rw-r--r--   0 akx        (501) staff       (20)    16057 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/rwk.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/rwk_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    48180 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/sah.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sah_RU.dat
--rw-r--r--   0 akx        (501) staff       (20)    16455 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/saq.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/saq_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)    12597 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/sat.dat
--rw-r--r--   0 akx        (501) staff       (20)      878 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sat_Olck.dat
--rw-r--r--   0 akx        (501) staff       (20)      632 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sat_Olck_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)    16479 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/sbp.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sbp_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)   194219 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/sd.dat
--rw-r--r--   0 akx        (501) staff       (20)      852 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sd_Arab.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sd_Arab_PK.dat
--rw-r--r--   0 akx        (501) staff       (20)    15216 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sd_Deva.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sd_Deva_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)    72353 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/se.dat
--rw-r--r--   0 akx        (501) staff       (20)    46574 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/se_FI.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/se_NO.dat
--rw-r--r--   0 akx        (501) staff       (20)      667 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/se_SE.dat
--rw-r--r--   0 akx        (501) staff       (20)    15910 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/seh.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/seh_MZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    15998 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ses.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ses_ML.dat
--rw-r--r--   0 akx        (501) staff       (20)    16635 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/sg.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sg_CF.dat
--rw-r--r--   0 akx        (501) staff       (20)    22036 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/shi.dat
--rw-r--r--   0 akx        (501) staff       (20)    15618 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/shi_Latn.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/shi_Latn_MA.dat
--rw-r--r--   0 akx        (501) staff       (20)      947 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/shi_Tfng.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/shi_Tfng_MA.dat
--rw-r--r--   0 akx        (501) staff       (20)   244850 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/si.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/si_LK.dat
--rw-r--r--   0 akx        (501) staff       (20)   256860 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/sk.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sk_SK.dat
--rw-r--r--   0 akx        (501) staff       (20)   241874 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/sl.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sl_SI.dat
--rw-r--r--   0 akx        (501) staff       (20)    42674 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/smn.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/smn_FI.dat
--rw-r--r--   0 akx        (501) staff       (20)    23252 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/sn.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/sn_ZW.dat
--rw-r--r--   0 akx        (501) staff       (20)   153105 2020-11-12 09:21:23.000000 Babel-2.9.0/babel/locale-data/so.dat
--rw-r--r--   0 akx        (501) staff       (20)      629 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/so_DJ.dat
--rw-r--r--   0 akx        (501) staff       (20)      628 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/so_ET.dat
--rw-r--r--   0 akx        (501) staff       (20)     1181 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/so_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/so_SO.dat
--rw-r--r--   0 akx        (501) staff       (20)   175659 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/sq.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sq_AL.dat
--rw-r--r--   0 akx        (501) staff       (20)     1181 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sq_MK.dat
--rw-r--r--   0 akx        (501) staff       (20)     1160 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sq_XK.dat
--rw-r--r--   0 akx        (501) staff       (20)   277763 2020-11-12 09:21:22.000000 Babel-2.9.0/babel/locale-data/sr.dat
--rw-r--r--   0 akx        (501) staff       (20)     1957 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Cyrl.dat
--rw-r--r--   0 akx        (501) staff       (20)     4710 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Cyrl_BA.dat
--rw-r--r--   0 akx        (501) staff       (20)     3873 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Cyrl_ME.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Cyrl_RS.dat
--rw-r--r--   0 akx        (501) staff       (20)     2756 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Cyrl_XK.dat
--rw-r--r--   0 akx        (501) staff       (20)   230252 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Latn.dat
--rw-r--r--   0 akx        (501) staff       (20)     3994 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Latn_BA.dat
--rw-r--r--   0 akx        (501) staff       (20)     3074 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Latn_ME.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Latn_RS.dat
--rw-r--r--   0 akx        (501) staff       (20)     2194 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sr_Latn_XK.dat
--rw-r--r--   0 akx        (501) staff       (20)    12452 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/su.dat
--rw-r--r--   0 akx        (501) staff       (20)      718 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/su_Latn.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/su_Latn_ID.dat
--rw-r--r--   0 akx        (501) staff       (20)   221078 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/sv.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/sv_AX.dat
--rw-r--r--   0 akx        (501) staff       (20)     2584 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/sv_FI.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sv_SE.dat
--rw-r--r--   0 akx        (501) staff       (20)   179207 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/sw.dat
--rw-r--r--   0 akx        (501) staff       (20)     2660 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sw_CD.dat
--rw-r--r--   0 akx        (501) staff       (20)    35934 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/sw_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sw_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)      633 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/sw_UG.dat
--rw-r--r--   0 akx        (501) staff       (20)   263466 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/ta.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ta_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)     1181 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ta_LK.dat
--rw-r--r--   0 akx        (501) staff       (20)     1238 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ta_MY.dat
--rw-r--r--   0 akx        (501) staff       (20)     1257 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ta_SG.dat
--rw-r--r--   0 akx        (501) staff       (20)   262280 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/te.dat
--rw-r--r--   0 akx        (501) staff       (20)      631 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/te_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)    16671 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/teo.dat
--rw-r--r--   0 akx        (501) staff       (20)      630 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/teo_KE.dat
--rw-r--r--   0 akx        (501) staff       (20)      613 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/teo_UG.dat
--rw-r--r--   0 akx        (501) staff       (20)    36303 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/tg.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/tg_TJ.dat
--rw-r--r--   0 akx        (501) staff       (20)   235280 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/th.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/th_TH.dat
--rw-r--r--   0 akx        (501) staff       (20)    73036 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/ti.dat
--rw-r--r--   0 akx        (501) staff       (20)      958 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ti_ER.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ti_ET.dat
--rw-r--r--   0 akx        (501) staff       (20)   167927 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/tk.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/tk_TM.dat
--rw-r--r--   0 akx        (501) staff       (20)   166458 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/to.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/to_TO.dat
--rw-r--r--   0 akx        (501) staff       (20)   209226 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/tr.dat
--rw-r--r--   0 akx        (501) staff       (20)     1184 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/tr_CY.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/tr_TR.dat
--rw-r--r--   0 akx        (501) staff       (20)    33588 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/tt.dat
--rw-r--r--   0 akx        (501) staff       (20)      626 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/tt_RU.dat
--rw-r--r--   0 akx        (501) staff       (20)    16171 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/twq.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/twq_NE.dat
--rw-r--r--   0 akx        (501) staff       (20)    16149 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/tzm.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/tzm_MA.dat
--rw-r--r--   0 akx        (501) staff       (20)   128534 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/ug.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ug_CN.dat
--rw-r--r--   0 akx        (501) staff       (20)   315834 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/uk.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/uk_UA.dat
--rw-r--r--   0 akx        (501) staff       (20)   197918 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/ur.dat
--rw-r--r--   0 akx        (501) staff       (20)    12595 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/ur_IN.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/ur_PK.dat
--rw-r--r--   0 akx        (501) staff       (20)   173590 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/uz.dat
--rw-r--r--   0 akx        (501) staff       (20)     4111 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/uz_Arab.dat
--rw-r--r--   0 akx        (501) staff       (20)      651 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/uz_Arab_AF.dat
--rw-r--r--   0 akx        (501) staff       (20)    98924 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/uz_Cyrl.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/uz_Cyrl_UZ.dat
--rw-r--r--   0 akx        (501) staff       (20)     1265 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/uz_Latn.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/uz_Latn_UZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    18988 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/vai.dat
--rw-r--r--   0 akx        (501) staff       (20)    14989 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/vai_Latn.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/vai_Latn_LR.dat
--rw-r--r--   0 akx        (501) staff       (20)      666 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/vai_Vaii.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/vai_Vaii_LR.dat
--rw-r--r--   0 akx        (501) staff       (20)   162325 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/vi.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/vi_VN.dat
--rw-r--r--   0 akx        (501) staff       (20)     5225 2020-11-12 09:21:20.000000 Babel-2.9.0/babel/locale-data/vo.dat
--rw-r--r--   0 akx        (501) staff       (20)      823 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/vo_001.dat
--rw-r--r--   0 akx        (501) staff       (20)    16067 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/vun.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/vun_TZ.dat
--rw-r--r--   0 akx        (501) staff       (20)    28660 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/wae.dat
--rw-r--r--   0 akx        (501) staff       (20)      627 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/wae_CH.dat
--rw-r--r--   0 akx        (501) staff       (20)    25698 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/wo.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/wo_SN.dat
--rw-r--r--   0 akx        (501) staff       (20)    15055 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/xh.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/xh_ZA.dat
--rw-r--r--   0 akx        (501) staff       (20)    16555 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/xog.dat
--rw-r--r--   0 akx        (501) staff       (20)      613 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/xog_UG.dat
--rw-r--r--   0 akx        (501) staff       (20)    15302 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/yav.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/yav_CM.dat
--rw-r--r--   0 akx        (501) staff       (20)    30314 2020-11-12 09:21:24.000000 Babel-2.9.0/babel/locale-data/yi.dat
--rw-r--r--   0 akx        (501) staff       (20)      885 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/yi_001.dat
--rw-r--r--   0 akx        (501) staff       (20)    68429 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/yo.dat
--rw-r--r--   0 akx        (501) staff       (20)    34481 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/yo_BJ.dat
--rw-r--r--   0 akx        (501) staff       (20)      589 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/yo_NG.dat
--rw-r--r--   0 akx        (501) staff       (20)   183333 2020-11-12 09:21:26.000000 Babel-2.9.0/babel/locale-data/yue.dat
--rw-r--r--   0 akx        (501) staff       (20)   183225 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/yue_Hans.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/yue_Hans_CN.dat
--rw-r--r--   0 akx        (501) staff       (20)     1279 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/yue_Hant.dat
--rw-r--r--   0 akx        (501) staff       (20)      609 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/yue_Hant_HK.dat
--rw-r--r--   0 akx        (501) staff       (20)    30498 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/zgh.dat
--rw-r--r--   0 akx        (501) staff       (20)      590 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zgh_MA.dat
--rw-r--r--   0 akx        (501) staff       (20)   181044 2020-11-12 09:21:21.000000 Babel-2.9.0/babel/locale-data/zh.dat
--rw-r--r--   0 akx        (501) staff       (20)     1278 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zh_Hans.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zh_Hans_CN.dat
--rw-r--r--   0 akx        (501) staff       (20)     3138 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zh_Hans_HK.dat
--rw-r--r--   0 akx        (501) staff       (20)     3270 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zh_Hans_MO.dat
--rw-r--r--   0 akx        (501) staff       (20)     3466 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zh_Hans_SG.dat
--rw-r--r--   0 akx        (501) staff       (20)   185029 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zh_Hant.dat
--rw-r--r--   0 akx        (501) staff       (20)    56895 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zh_Hant_HK.dat
--rw-r--r--   0 akx        (501) staff       (20)      630 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zh_Hant_MO.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zh_Hant_TW.dat
--rw-r--r--   0 akx        (501) staff       (20)   167684 2020-11-12 09:21:25.000000 Babel-2.9.0/babel/locale-data/zu.dat
--rw-r--r--   0 akx        (501) staff       (20)      608 2020-11-12 09:21:27.000000 Babel-2.9.0/babel/locale-data/zu_ZA.dat
--rw-r--r--   0 akx        (501) staff       (20)     7317 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/localedata.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.928465 Babel-2.9.0/babel/localtime/
--rw-r--r--   0 akx        (501) staff       (20)     1721 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/localtime/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)     4801 2018-05-28 09:13:13.000000 Babel-2.9.0/babel/localtime/_unix.py
--rw-r--r--   0 akx        (501) staff       (20)     3086 2019-02-20 13:12:21.000000 Babel-2.9.0/babel/localtime/_win32.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.954875 Babel-2.9.0/babel/messages/
--rw-r--r--   0 akx        (501) staff       (20)      254 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/messages/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)    32291 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/messages/catalog.py
--rw-r--r--   0 akx        (501) staff       (20)     6085 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/messages/checkers.py
--rw-r--r--   0 akx        (501) staff       (20)    26474 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/messages/extract.py
--rw-r--r--   0 akx        (501) staff       (20)    38729 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/messages/frontend.py
--rw-r--r--   0 akx        (501) staff       (20)     6334 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/messages/jslexer.py
--rw-r--r--   0 akx        (501) staff       (20)     7204 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/messages/mofile.py
--rw-r--r--   0 akx        (501) staff       (20)     7206 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/messages/plurals.py
--rw-r--r--   0 akx        (501) staff       (20)    22146 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/messages/pofile.py
--rw-r--r--   0 akx        (501) staff       (20)    39872 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/numbers.py
--rw-r--r--   0 akx        (501) staff       (20)    21314 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/plural.py
--rw-r--r--   0 akx        (501) staff       (20)    22622 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/support.py
--rw-r--r--   0 akx        (501) staff       (20)    11291 2020-11-11 11:58:13.000000 Babel-2.9.0/babel/units.py
--rw-r--r--   0 akx        (501) staff       (20)     7576 2020-11-11 12:00:33.000000 Babel-2.9.0/babel/util.py
--rw-r--r--   0 akx        (501) staff       (20)      533 2020-11-11 10:57:51.000000 Babel-2.9.0/conftest.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.962894 Babel-2.9.0/docs/
--rw-r--r--   0 akx        (501) staff       (20)     5560 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/Makefile
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.964588 Babel-2.9.0/docs/_static/
--rw-r--r--   0 akx        (501) staff       (20)    44986 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/_static/logo.pdf
--rw-r--r--   0 akx        (501) staff       (20)    15484 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/_static/logo.png
--rw-r--r--   0 akx        (501) staff       (20)     6118 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/_static/logo_small.png
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.965599 Babel-2.9.0/docs/_templates/
--rw-r--r--   0 akx        (501) staff       (20)      101 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/_templates/sidebar-about.html
--rw-r--r--   0 akx        (501) staff       (20)      582 2018-07-20 10:31:17.000000 Babel-2.9.0/docs/_templates/sidebar-links.html
--rw-r--r--   0 akx        (501) staff       (20)      142 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/_templates/sidebar-logo.html
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.966313 Babel-2.9.0/docs/_themes/
--rw-r--r--   0 akx        (501) staff       (20)     1789 2018-02-02 16:36:50.000000 Babel-2.9.0/docs/_themes/LICENSE
--rw-r--r--   0 akx        (501) staff       (20)     1093 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/_themes/README
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.967311 Babel-2.9.0/docs/_themes/babel/
--rw-r--r--   0 akx        (501) staff       (20)      937 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/_themes/babel/layout.html
--rw-r--r--   0 akx        (501) staff       (20)      590 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/_themes/babel/relations.html
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.968136 Babel-2.9.0/docs/_themes/babel/static/
--rw-r--r--   0 akx        (501) staff       (20)     6964 2018-02-02 16:36:50.000000 Babel-2.9.0/docs/_themes/babel/static/babel.css_t
--rw-r--r--   0 akx        (501) staff       (20)      976 2018-02-02 16:36:50.000000 Babel-2.9.0/docs/_themes/babel/static/small_babel.css
--rw-r--r--   0 akx        (501) staff       (20)      121 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/_themes/babel/theme.conf
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.971444 Babel-2.9.0/docs/api/
--rw-r--r--   0 akx        (501) staff       (20)      714 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/api/core.rst
--rw-r--r--   0 akx        (501) staff       (20)     1748 2018-02-02 16:29:02.000000 Babel-2.9.0/docs/api/dates.rst
--rw-r--r--   0 akx        (501) staff       (20)      249 2018-02-02 16:29:02.000000 Babel-2.9.0/docs/api/index.rst
--rw-r--r--   0 akx        (501) staff       (20)      290 2018-02-02 16:29:02.000000 Babel-2.9.0/docs/api/languages.rst
--rw-r--r--   0 akx        (501) staff       (20)      162 2018-02-02 16:29:02.000000 Babel-2.9.0/docs/api/lists.rst
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.973488 Babel-2.9.0/docs/api/messages/
--rw-r--r--   0 akx        (501) staff       (20)      471 2020-11-11 11:58:13.000000 Babel-2.9.0/docs/api/messages/catalog.rst
--rw-r--r--   0 akx        (501) staff       (20)      976 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/api/messages/extract.rst
--rw-r--r--   0 akx        (501) staff       (20)      233 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/api/messages/index.rst
--rw-r--r--   0 akx        (501) staff       (20)      271 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/api/messages/mofile.rst
--rw-r--r--   0 akx        (501) staff       (20)      279 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/api/messages/pofile.rst
--rw-r--r--   0 akx        (501) staff       (20)      900 2018-07-20 10:31:17.000000 Babel-2.9.0/docs/api/numbers.rst
--rw-r--r--   0 akx        (501) staff       (20)      479 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/api/plural.rst
--rw-r--r--   0 akx        (501) staff       (20)      418 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/api/support.rst
--rw-r--r--   0 akx        (501) staff       (20)      232 2018-02-02 16:29:02.000000 Babel-2.9.0/docs/api/units.rst
--rw-r--r--   0 akx        (501) staff       (20)       24 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/changelog.rst
--rw-r--r--   0 akx        (501) staff       (20)     6691 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/cmdline.rst
--rw-r--r--   0 akx        (501) staff       (20)     8368 2020-11-12 09:20:39.000000 Babel-2.9.0/docs/conf.py
--rw-r--r--   0 akx        (501) staff       (20)    17790 2018-07-20 10:31:17.000000 Babel-2.9.0/docs/dates.rst
--rw-r--r--   0 akx        (501) staff       (20)     3120 2018-02-02 16:29:02.000000 Babel-2.9.0/docs/dev.rst
--rw-r--r--   0 akx        (501) staff       (20)      736 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/index.rst
--rw-r--r--   0 akx        (501) staff       (20)     3022 2019-12-31 09:08:38.000000 Babel-2.9.0/docs/installation.rst
--rw-r--r--   0 akx        (501) staff       (20)     2172 2018-07-20 10:31:17.000000 Babel-2.9.0/docs/intro.rst
--rw-r--r--   0 akx        (501) staff       (20)      959 2020-11-11 11:58:13.000000 Babel-2.9.0/docs/license.rst
--rw-r--r--   0 akx        (501) staff       (20)     4377 2018-07-20 10:31:17.000000 Babel-2.9.0/docs/locale.rst
--rw-r--r--   0 akx        (501) staff       (20)     5094 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/make.bat
--rw-r--r--   0 akx        (501) staff       (20)    11768 2019-02-20 13:12:21.000000 Babel-2.9.0/docs/messages.rst
--rw-r--r--   0 akx        (501) staff       (20)     7444 2020-11-11 11:58:13.000000 Babel-2.9.0/docs/numbers.rst
--rw-r--r--   0 akx        (501) staff       (20)    15139 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/setup.rst
--rw-r--r--   0 akx        (501) staff       (20)     1724 2016-11-19 14:05:40.000000 Babel-2.9.0/docs/support.rst
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.975570 Babel-2.9.0/scripts/
--rwxr-xr-x   0 akx        (501) staff       (20)     2865 2020-11-11 18:22:35.000000 Babel-2.9.0/scripts/download_import_cldr.py
--rwxr-xr-x   0 akx        (501) staff       (20)     1526 2020-11-11 12:00:33.000000 Babel-2.9.0/scripts/dump_data.py
--rwxr-xr-x   0 akx        (501) staff       (20)      883 2020-11-11 12:00:33.000000 Babel-2.9.0/scripts/dump_global.py
--rw-r--r--   0 akx        (501) staff       (20)     1284 2018-05-28 09:13:13.000000 Babel-2.9.0/scripts/generate_authors.py
--rwxr-xr-x   0 akx        (501) staff       (20)    40547 2020-11-12 09:20:39.000000 Babel-2.9.0/scripts/import_cldr.py
--rwxr-xr-x   0 akx        (501) staff       (20)     4149 2018-02-02 16:36:50.000000 Babel-2.9.0/scripts/make-release.py
--rw-r--r--   0 akx        (501) staff       (20)      349 2020-11-12 09:21:38.009250 Babel-2.9.0/setup.cfg
--rwxr-xr-x   0 akx        (501) staff       (20)     3243 2020-11-11 18:22:35.000000 Babel-2.9.0/setup.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.982158 Babel-2.9.0/tests/
--rw-r--r--   0 akx        (501) staff       (20)        0 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)      526 2019-12-31 12:09:16.000000 Babel-2.9.0/tests/conftest.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.988012 Babel-2.9.0/tests/messages/
--rw-r--r--   0 akx        (501) staff       (20)        0 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/__init__.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.989970 Babel-2.9.0/tests/messages/data/
--rw-r--r--   0 akx        (501) staff       (20)      100 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/mapping.cfg
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.990999 Babel-2.9.0/tests/messages/data/project/
--rw-r--r--   0 akx        (501) staff       (20)        0 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)      199 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/file1.py
--rw-r--r--   0 akx        (501) staff       (20)      232 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/file2.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.991806 Babel-2.9.0/tests/messages/data/project/i18n/
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.513572 Babel-2.9.0/tests/messages/data/project/i18n/de/
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.992646 Babel-2.9.0/tests/messages/data/project/i18n/de/LC_MESSAGES/
--rw-r--r--   0 akx        (501) staff       (20)      547 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/i18n/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 akx        (501) staff       (20)      898 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/i18n/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.513796 Babel-2.9.0/tests/messages/data/project/i18n/de_DE/
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.994003 Babel-2.9.0/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/
--rw-r--r--   0 akx        (501) staff       (20)      898 2018-02-02 16:29:02.000000 Babel-2.9.0/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/bar.po
--rw-r--r--   0 akx        (501) staff       (20)      898 2018-02-02 16:29:02.000000 Babel-2.9.0/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/foo.po
--rw-r--r--   0 akx        (501) staff       (20)      882 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.514022 Babel-2.9.0/tests/messages/data/project/i18n/fi_BUGGY/
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.994359 Babel-2.9.0/tests/messages/data/project/i18n/fi_BUGGY/LC_MESSAGES/
--rw-r--r--   0 akx        (501) staff       (20)       67 2019-05-27 11:53:30.000000 Babel-2.9.0/tests/messages/data/project/i18n/fi_BUGGY/LC_MESSAGES/messages.po
--rw-r--r--   0 akx        (501) staff       (20)      823 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/i18n/messages.pot
--rw-r--r--   0 akx        (501) staff       (20)      814 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/i18n/messages_non_fuzzy.pot
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.514251 Babel-2.9.0/tests/messages/data/project/i18n/ru_RU/
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:37.996337 Babel-2.9.0/tests/messages/data/project/i18n/ru_RU/LC_MESSAGES/
--rw-r--r--   0 akx        (501) staff       (20)      971 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/i18n/ru_RU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2020-11-12 09:21:38.002315 Babel-2.9.0/tests/messages/data/project/ignored/
--rw-r--r--   0 akx        (501) staff       (20)       18 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/ignored/a_test_file.txt
--rw-r--r--   0 akx        (501) staff       (20)        0 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/ignored/an_example.txt
--rw-r--r--   0 akx        (501) staff       (20)      284 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/project/ignored/this_wont_normally_be_here.py
--rw-r--r--   0 akx        (501) staff       (20)      172 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/setup.cfg
--rwxr-xr-x   0 akx        (501) staff       (20)      823 2016-11-19 14:05:40.000000 Babel-2.9.0/tests/messages/data/setup.py
--rw-r--r--   0 akx        (501) staff       (20)    19449 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/messages/test_catalog.py
--rw-r--r--   0 akx        (501) staff       (20)    12564 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/messages/test_checkers.py
--rw-r--r--   0 akx        (501) staff       (20)    20966 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/messages/test_extract.py
--rw-r--r--   0 akx        (501) staff       (20)    47817 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/messages/test_frontend.py
--rw-r--r--   0 akx        (501) staff       (20)     4617 2019-05-27 11:55:14.000000 Babel-2.9.0/tests/messages/test_js_extract.py
--rw-r--r--   0 akx        (501) staff       (20)     3748 2019-05-27 11:55:14.000000 Babel-2.9.0/tests/messages/test_jslexer.py
--rw-r--r--   0 akx        (501) staff       (20)     3847 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/messages/test_mofile.py
--rw-r--r--   0 akx        (501) staff       (20)      636 2019-05-27 11:53:30.000000 Babel-2.9.0/tests/messages/test_normalized_string.py
--rw-r--r--   0 akx        (501) staff       (20)     2598 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/messages/test_plurals.py
--rw-r--r--   0 akx        (501) staff       (20)    29926 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/messages/test_pofile.py
--rw-r--r--   0 akx        (501) staff       (20)    12324 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/test_core.py
--rw-r--r--   0 akx        (501) staff       (20)     1853 2018-02-02 16:29:02.000000 Babel-2.9.0/tests/test_date_intervals.py
--rw-r--r--   0 akx        (501) staff       (20)    37089 2020-11-11 18:22:35.000000 Babel-2.9.0/tests/test_dates.py
--rw-r--r--   0 akx        (501) staff       (20)      644 2018-02-02 16:29:02.000000 Babel-2.9.0/tests/test_day_periods.py
--rw-r--r--   0 akx        (501) staff       (20)      631 2018-02-02 16:29:02.000000 Babel-2.9.0/tests/test_languages.py
--rw-r--r--   0 akx        (501) staff       (20)      728 2018-02-02 16:29:02.000000 Babel-2.9.0/tests/test_lists.py
--rw-r--r--   0 akx        (501) staff       (20)     4291 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/test_localedata.py
--rw-r--r--   0 akx        (501) staff       (20)    32079 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/test_numbers.py
--rw-r--r--   0 akx        (501) staff       (20)     9269 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/test_plural.py
--rw-r--r--   0 akx        (501) staff       (20)     1162 2018-05-28 12:52:42.000000 Babel-2.9.0/tests/test_smoke.py
--rw-r--r--   0 akx        (501) staff       (20)    14765 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/test_support.py
--rw-r--r--   0 akx        (501) staff       (20)     3312 2020-11-11 12:00:33.000000 Babel-2.9.0/tests/test_util.py
--rw-r--r--   0 akx        (501) staff       (20)      455 2020-11-11 18:22:35.000000 Babel-2.9.0/tox.ini
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.298481 Babel-2.9.1/
+-rw-r--r--   0 akx        (501) staff       (20)     2423 2021-04-28 19:13:49.000000 Babel-2.9.1/AUTHORS
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:19.723784 Babel-2.9.1/Babel.egg-info/
+-rw-r--r--   0 akx        (501) staff       (20)     1202 2021-04-28 19:28:19.000000 Babel-2.9.1/Babel.egg-info/PKG-INFO
+-rw-r--r--   0 akx        (501) staff       (20)    25548 2021-04-28 19:28:19.000000 Babel-2.9.1/Babel.egg-info/SOURCES.txt
+-rw-r--r--   0 akx        (501) staff       (20)        1 2021-04-28 19:28:19.000000 Babel-2.9.1/Babel.egg-info/dependency_links.txt
+-rw-r--r--   0 akx        (501) staff       (20)      764 2021-04-28 19:28:19.000000 Babel-2.9.1/Babel.egg-info/entry_points.txt
+-rw-r--r--   0 akx        (501) staff       (20)        1 2021-04-28 19:28:19.000000 Babel-2.9.1/Babel.egg-info/not-zip-safe
+-rw-r--r--   0 akx        (501) staff       (20)       13 2021-04-28 19:28:19.000000 Babel-2.9.1/Babel.egg-info/requires.txt
+-rw-r--r--   0 akx        (501) staff       (20)        6 2021-04-28 19:28:19.000000 Babel-2.9.1/Babel.egg-info/top_level.txt
+-rw-r--r--   0 akx        (501) staff       (20)    31009 2021-04-28 19:13:54.000000 Babel-2.9.1/CHANGES
+-rw-r--r--   0 akx        (501) staff       (20)     1451 2021-04-28 19:13:54.000000 Babel-2.9.1/LICENSE
+-rw-r--r--   0 akx        (501) staff       (20)      287 2016-11-19 14:05:40.000000 Babel-2.9.1/MANIFEST.in
+-rw-r--r--   0 akx        (501) staff       (20)     1337 2019-05-27 11:55:14.000000 Babel-2.9.1/Makefile
+-rw-r--r--   0 akx        (501) staff       (20)     1202 2021-04-28 19:28:20.298603 Babel-2.9.1/PKG-INFO
+-rw-r--r--   0 akx        (501) staff       (20)      829 2018-02-02 16:29:02.000000 Babel-2.9.1/README.rst
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:19.734943 Babel-2.9.1/babel/
+-rw-r--r--   0 akx        (501) staff       (20)      714 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)     1685 2019-02-20 13:12:21.000000 Babel-2.9.1/babel/_compat.py
+-rw-r--r--   0 akx        (501) staff       (20)    36907 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/core.py
+-rw-r--r--   0 akx        (501) staff       (20)    67709 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/dates.py
+-rw-r--r--   0 akx        (501) staff       (20)   254421 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/global.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2743 2018-07-20 10:31:17.000000 Babel-2.9.1/babel/languages.py
+-rw-r--r--   0 akx        (501) staff       (20)     2719 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/lists.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.236064 Babel-2.9.1/babel/locale-data/
+-rw-r--r--   0 akx        (501) staff       (20)   171143 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/af.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1407 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/af_NA.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/af_ZA.dat
+-rw-r--r--   0 akx        (501) staff       (20)    17339 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/agq.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/agq_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15859 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/ak.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ak_GH.dat
+-rw-r--r--   0 akx        (501) staff       (20)   200581 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/am.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/am_ET.dat
+-rw-r--r--   0 akx        (501) staff       (20)   345779 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/ar.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1680 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ar_001.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1038 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_AE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_BH.dat
+-rw-r--r--   0 akx        (501) staff       (20)      629 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_DJ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1713 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_DZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      688 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ar_EG.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_EH.dat
+-rw-r--r--   0 akx        (501) staff       (20)      610 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_ER.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1195 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_IL.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2336 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_IQ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2335 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_JO.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1161 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ar_KM.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_KW.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2336 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_LB.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1652 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ar_LY.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2007 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_MA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2173 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_MR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_OM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2273 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_PS.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ar_QA.dat
+-rw-r--r--   0 akx        (501) staff       (20)    30599 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_SA.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_SD.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_SO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_SS.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2335 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_SY.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_TD.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1651 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ar_TN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ar_YE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   234427 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/as.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/as_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16187 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/asa.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/asa_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)   209617 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ast.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ast_ES.dat
+-rw-r--r--   0 akx        (501) staff       (20)   194898 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/az.dat
+-rw-r--r--   0 akx        (501) staff       (20)    38880 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/az_Cyrl.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/az_Cyrl_AZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2225 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/az_Latn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/az_Latn_AZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    17128 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/bas.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/bas_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)   271438 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/be.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/be_BY.dat
+-rw-r--r--   0 akx        (501) staff       (20)     6534 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/bem.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/bem_ZM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16977 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/bez.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/bez_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)   232833 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/bg.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/bg_BG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15886 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/bm.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/bm_ML.dat
+-rw-r--r--   0 akx        (501) staff       (20)   263365 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/bn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/bn_BD.dat
+-rw-r--r--   0 akx        (501) staff       (20)      866 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/bn_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    22525 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/bo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/bo_CN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      704 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/bo_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   290897 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/br.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/br_FR.dat
+-rw-r--r--   0 akx        (501) staff       (20)   124289 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/brx.dat
+-rw-r--r--   0 akx        (501) staff       (20)      632 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/brx_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   239326 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/bs.dat
+-rw-r--r--   0 akx        (501) staff       (20)   213685 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/bs_Cyrl.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/bs_Cyrl_BA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1957 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/bs_Latn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/bs_Latn_BA.dat
+-rw-r--r--   0 akx        (501) staff       (20)   208790 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/ca.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ca_AD.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ca_ES.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3644 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ca_ES_VALENCIA.dat
+-rw-r--r--   0 akx        (501) staff       (20)      645 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ca_FR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ca_IT.dat
+-rw-r--r--   0 akx        (501) staff       (20)   275655 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ccp.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ccp_BD.dat
+-rw-r--r--   0 akx        (501) staff       (20)      632 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ccp_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   138778 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/ce.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ce_RU.dat
+-rw-r--r--   0 akx        (501) staff       (20)   103518 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/ceb.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ceb_PH.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16228 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/cgg.dat
+-rw-r--r--   0 akx        (501) staff       (20)      613 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/cgg_UG.dat
+-rw-r--r--   0 akx        (501) staff       (20)   200072 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/chr.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/chr_US.dat
+-rw-r--r--   0 akx        (501) staff       (20)    41606 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ckb.dat
+-rw-r--r--   0 akx        (501) staff       (20)      652 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ckb_IQ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1204 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ckb_IR.dat
+-rw-r--r--   0 akx        (501) staff       (20)   297675 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/cs.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/cs_CZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    20265 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/cu.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/cu_RU.dat
+-rw-r--r--   0 akx        (501) staff       (20)   315824 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/cy.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/cy_GB.dat
+-rw-r--r--   0 akx        (501) staff       (20)   199867 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/da.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/da_DK.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/da_GL.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16271 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/dav.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/dav_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   206762 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/de.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2563 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/de_AT.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/de_BE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3938 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/de_CH.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/de_DE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1619 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/de_IT.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1321 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/de_LI.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1065 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/de_LU.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16192 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/dje.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/dje_NE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   179644 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/dsb.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/dsb_DE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     5355 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/dua.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/dua_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    10541 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/dyo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/dyo_SN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    89908 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/dz.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/dz_BT.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16243 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ebu.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ebu_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   142527 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/ee.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ee_GH.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1141 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ee_TG.dat
+-rw-r--r--   0 akx        (501) staff       (20)   244752 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/el.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/el_CY.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/el_GR.dat
+-rw-r--r--   0 akx        (501) staff       (20)   194682 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/en.dat
+-rw-r--r--   0 akx        (501) staff       (20)    27063 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_001.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1765 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_150.dat
+-rw-r--r--   0 akx        (501) staff       (20)     4111 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_AE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_AG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1179 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_AI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_AS.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1200 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_AT.dat
+-rw-r--r--   0 akx        (501) staff       (20)    23385 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_AU.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_BB.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1493 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_BE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1162 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_BI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_BM.dat
+-rw-r--r--   0 akx        (501) staff       (20)      811 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_BS.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2771 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_BW.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2950 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_BZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    25449 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_CA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_CC.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1100 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_CH.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_CK.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1410 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_CX.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_CY.dat
+-rw-r--r--   0 akx        (501) staff       (20)      952 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_DE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1141 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_DG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2350 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_DK.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_DM.dat
+-rw-r--r--   0 akx        (501) staff       (20)      860 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_ER.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2282 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_FI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      645 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_FJ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1183 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_FK.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_FM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    25821 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_GB.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_GD.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1246 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_GG.dat
+-rw-r--r--   0 akx        (501) staff       (20)      862 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_GH.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1201 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_GI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      858 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_GM.dat
+-rw-r--r--   0 akx        (501) staff       (20)      688 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_GU.dat
+-rw-r--r--   0 akx        (501) staff       (20)      667 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_GY.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2008 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_HK.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2043 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_IE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1397 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_IL.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1246 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_IM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3767 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1141 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_IO.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1246 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_JE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1599 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_JM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1431 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_KI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_KN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      792 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_KY.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_LC.dat
+-rw-r--r--   0 akx        (501) staff       (20)      858 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_LR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      858 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_LS.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1411 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_MG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1341 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_MH.dat
+-rw-r--r--   0 akx        (501) staff       (20)      803 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_MO.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1322 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_MP.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_MS.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1927 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_MT.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1411 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_MU.dat
+-rw-r--r--   0 akx        (501) staff       (20)      859 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_MW.dat
+-rw-r--r--   0 akx        (501) staff       (20)      689 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_MY.dat
+-rw-r--r--   0 akx        (501) staff       (20)      858 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_NA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_NF.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1412 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_NG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1097 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_NL.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_NR.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_NU.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2234 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_NZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_PG.dat
+-rw-r--r--   0 akx        (501) staff       (20)      629 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_PH.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1959 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_PK.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_PN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_PR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      773 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_PW.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1411 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_RW.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_SB.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1161 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_SC.dat
+-rw-r--r--   0 akx        (501) staff       (20)      901 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_SD.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1427 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_SE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2017 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_SG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1183 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_SH.dat
+-rw-r--r--   0 akx        (501) staff       (20)      968 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_SI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      859 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_SL.dat
+-rw-r--r--   0 akx        (501) staff       (20)      881 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_SS.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1163 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_SX.dat
+-rw-r--r--   0 akx        (501) staff       (20)      858 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_SZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_TC.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_TK.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_TO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_TT.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_TV.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1412 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1435 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_UG.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_UM.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_US.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1204 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_US_POSIX.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_VC.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_VG.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/en_VI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_VU.dat
+-rw-r--r--   0 akx        (501) staff       (20)      629 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_WS.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3269 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_ZA.dat
+-rw-r--r--   0 akx        (501) staff       (20)      858 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_ZM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3199 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/en_ZW.dat
+-rw-r--r--   0 akx        (501) staff       (20)    40689 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/eo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      823 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/eo_001.dat
+-rw-r--r--   0 akx        (501) staff       (20)   199638 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/es.dat
+-rw-r--r--   0 akx        (501) staff       (20)    23299 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_419.dat
+-rw-r--r--   0 akx        (501) staff       (20)     8828 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_AR.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1888 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_BO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      628 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_BR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_BZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     5128 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_CL.dat
+-rw-r--r--   0 akx        (501) staff       (20)     8665 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_CO.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1719 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_CR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      629 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_CU.dat
+-rw-r--r--   0 akx        (501) staff       (20)     4020 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_DO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_EA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3294 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_EC.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_ES.dat
+-rw-r--r--   0 akx        (501) staff       (20)      872 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_GQ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     4896 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_GT.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3476 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_HN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_IC.dat
+-rw-r--r--   0 akx        (501) staff       (20)    24708 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_MX.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1653 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_NI.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3884 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_PA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     4848 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_PE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1205 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_PH.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3798 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_PR.dat
+-rw-r--r--   0 akx        (501) staff       (20)     5319 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_PY.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1402 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_SV.dat
+-rw-r--r--   0 akx        (501) staff       (20)    25343 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_US.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2540 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/es_UY.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3752 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/es_VE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   200192 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/et.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/et_EE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   176850 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/eu.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/eu_ES.dat
+-rw-r--r--   0 akx        (501) staff       (20)    17595 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ewo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ewo_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)   217724 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/fa.dat
+-rw-r--r--   0 akx        (501) staff       (20)    11247 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fa_AF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fa_IR.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16084 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/ff.dat
+-rw-r--r--   0 akx        (501) staff       (20)   174659 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm.dat
+-rw-r--r--   0 akx        (501) staff       (20)      610 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_BF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      629 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1209 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_GH.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1205 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_GM.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_GN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      610 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_GW.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1205 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_LR.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1206 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_MR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      610 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_NE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_NG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1206 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_SL.dat
+-rw-r--r--   0 akx        (501) staff       (20)      610 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Adlm_SN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      839 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_BF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1188 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_GH.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1184 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_GM.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_GN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_GW.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1184 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_LR.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1185 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_MR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_NE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      610 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_NG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1185 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_SL.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ff_Latn_SN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   227195 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/fi.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fi_FI.dat
+-rw-r--r--   0 akx        (501) staff       (20)   179405 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fil.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fil_PH.dat
+-rw-r--r--   0 akx        (501) staff       (20)   165657 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/fo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      647 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fo_DK.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fo_FO.dat
+-rw-r--r--   0 akx        (501) staff       (20)   225342 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/fr.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1254 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_BE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_BF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      610 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_BI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_BJ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_BL.dat
+-rw-r--r--   0 akx        (501) staff       (20)    65858 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_CA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1106 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_CD.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_CF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_CG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2970 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_CH.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_CI.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2083 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1205 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_DJ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1247 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_DZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_FR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_GA.dat
+-rw-r--r--   0 akx        (501) staff       (20)      692 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_GF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_GN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_GP.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_GQ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1873 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_HT.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_KM.dat
+-rw-r--r--   0 akx        (501) staff       (20)      687 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_LU.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1277 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_MA.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_MC.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_MF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_MG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1126 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_ML.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_MQ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1185 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_MR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_MU.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_NC.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_NE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_PF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_PM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1142 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_RE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_RW.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_SC.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1277 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_SN.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1247 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_SY.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1165 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_TD.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fr_TG.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1185 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_TN.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1185 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_VU.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_WF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fr_YT.dat
+-rw-r--r--   0 akx        (501) staff       (20)    35027 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fur.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/fur_IT.dat
+-rw-r--r--   0 akx        (501) staff       (20)   110221 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/fy.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/fy_NL.dat
+-rw-r--r--   0 akx        (501) staff       (20)   316865 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/ga.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ga_GB.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ga_IE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   302010 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/gd.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/gd_GB.dat
+-rw-r--r--   0 akx        (501) staff       (20)   176367 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/gl.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/gl_ES.dat
+-rw-r--r--   0 akx        (501) staff       (20)   108049 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/gsw.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/gsw_CH.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/gsw_FR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/gsw_LI.dat
+-rw-r--r--   0 akx        (501) staff       (20)   246649 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/gu.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/gu_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16016 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/guz.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/guz_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)     4146 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/gv.dat
+-rw-r--r--   0 akx        (501) staff       (20)      607 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/gv_IM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    78016 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/ha.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1188 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ha_GH.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1248 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ha_NE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ha_NG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16106 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/haw.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/haw_US.dat
+-rw-r--r--   0 akx        (501) staff       (20)   271008 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/he.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/he_IL.dat
+-rw-r--r--   0 akx        (501) staff       (20)   244568 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/hi.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/hi_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   247517 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/hr.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1161 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/hr_BA.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/hr_HR.dat
+-rw-r--r--   0 akx        (501) staff       (20)   179178 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/hsb.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/hsb_DE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   192963 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/hu.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/hu_HU.dat
+-rw-r--r--   0 akx        (501) staff       (20)   214313 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/hy.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/hy_AM.dat
+-rw-r--r--   0 akx        (501) staff       (20)   112822 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/ia.dat
+-rw-r--r--   0 akx        (501) staff       (20)      914 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ia_001.dat
+-rw-r--r--   0 akx        (501) staff       (20)   163265 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/id.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/id_ID.dat
+-rw-r--r--   0 akx        (501) staff       (20)    52036 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/ig.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ig_NG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    12588 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/ii.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ii_CN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   188046 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/is.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/is_IS.dat
+-rw-r--r--   0 akx        (501) staff       (20)   188460 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/it.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2776 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/it_CH.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/it_IT.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/it_SM.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/it_VA.dat
+-rw-r--r--   0 akx        (501) staff       (20)   200287 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/ja.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ja_JP.dat
+-rw-r--r--   0 akx        (501) staff       (20)    12628 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/jgo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/jgo_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16068 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/jmc.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/jmc_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)   129461 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/jv.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/jv_ID.dat
+-rw-r--r--   0 akx        (501) staff       (20)   260705 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/ka.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ka_GE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   135263 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/kab.dat
+-rw-r--r--   0 akx        (501) staff       (20)      652 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/kab_DZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16175 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/kam.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/kam_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16475 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/kde.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/kde_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    85757 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/kea.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/kea_CV.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15939 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/khq.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/khq_ML.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16123 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/ki.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ki_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   210242 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/kk.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/kk_KZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     4888 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/kkj.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/kkj_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    58200 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/kl.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/kl_GL.dat
+-rw-r--r--   0 akx        (501) staff       (20)    18003 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/kln.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/kln_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   202267 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/km.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/km_KH.dat
+-rw-r--r--   0 akx        (501) staff       (20)   263580 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/kn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/kn_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   175158 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/ko.dat
+-rw-r--r--   0 akx        (501) staff       (20)      789 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ko_KP.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ko_KR.dat
+-rw-r--r--   0 akx        (501) staff       (20)   182871 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/kok.dat
+-rw-r--r--   0 akx        (501) staff       (20)      632 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/kok_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   102570 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/ks.dat
+-rw-r--r--   0 akx        (501) staff       (20)      823 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ks_Arab.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ks_Arab_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16043 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ksb.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ksb_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16515 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/ksf.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ksf_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    88937 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ksh.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ksh_DE.dat
+-rw-r--r--   0 akx        (501) staff       (20)    28771 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/ku.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ku_TR.dat
+-rw-r--r--   0 akx        (501) staff       (20)     7242 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/kw.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/kw_GB.dat
+-rw-r--r--   0 akx        (501) staff       (20)   202058 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/ky.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ky_KG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    17141 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/lag.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/lag_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)   164597 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/lb.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/lb_LU.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16434 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/lg.dat
+-rw-r--r--   0 akx        (501) staff       (20)      612 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/lg_UG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    12766 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/lkt.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/lkt_US.dat
+-rw-r--r--   0 akx        (501) staff       (20)    25891 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/ln.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ln_AO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ln_CD.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ln_CF.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ln_CG.dat
+-rw-r--r--   0 akx        (501) staff       (20)   220343 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/lo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/lo_LA.dat
+-rw-r--r--   0 akx        (501) staff       (20)    19021 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/lrc.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1228 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/lrc_IQ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      652 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/lrc_IR.dat
+-rw-r--r--   0 akx        (501) staff       (20)   284211 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/lt.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/lt_LT.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15888 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/lu.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/lu_CD.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15885 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/luo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/luo_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15859 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/luy.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/luy_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   214988 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/lv.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/lv_LV.dat
+-rw-r--r--   0 akx        (501) staff       (20)    14710 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mai.dat
+-rw-r--r--   0 akx        (501) staff       (20)      632 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mai_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    17297 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mas.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mas_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      611 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mas_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16088 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mer.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mer_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15117 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mfe.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mfe_MU.dat
+-rw-r--r--   0 akx        (501) staff       (20)    23550 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/mg.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mg_MG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    10479 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mgh.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mgh_MZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     8206 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mgo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mgo_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    20727 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/mi.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mi_NZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)   234490 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/mk.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mk_MK.dat
+-rw-r--r--   0 akx        (501) staff       (20)   285214 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/ml.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ml_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   202642 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/mn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mn_MN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    14622 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mni.dat
+-rw-r--r--   0 akx        (501) staff       (20)      666 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mni_Beng.dat
+-rw-r--r--   0 akx        (501) staff       (20)      632 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mni_Beng_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   246797 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/mr.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mr_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   152238 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/ms.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1257 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ms_BN.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3272 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ms_ID.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ms_MY.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ms_SG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    78243 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/mt.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mt_MT.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16547 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mua.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mua_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)   210242 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/my.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/my_MM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    65499 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/mzn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      652 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/mzn_IR.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16617 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/naq.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/naq_NA.dat
+-rw-r--r--   0 akx        (501) staff       (20)   210593 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/nb.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nb_NO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      607 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nb_SJ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16312 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/nd.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nd_ZW.dat
+-rw-r--r--   0 akx        (501) staff       (20)    50632 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nds.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nds_DE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nds_NL.dat
+-rw-r--r--   0 akx        (501) staff       (20)   248497 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/ne.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1265 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ne_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ne_NP.dat
+-rw-r--r--   0 akx        (501) staff       (20)   215801 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/nl.dat
+-rw-r--r--   0 akx        (501) staff       (20)      611 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nl_AW.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1835 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nl_BE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nl_BQ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      611 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nl_CW.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nl_NL.dat
+-rw-r--r--   0 akx        (501) staff       (20)      669 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nl_SR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      611 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nl_SX.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16189 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nmg.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nmg_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)   179884 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/nn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nn_NO.dat
+-rw-r--r--   0 akx        (501) staff       (20)     6766 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/nnh.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nnh_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)     9153 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nus.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nus_SS.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16275 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/nyn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      613 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/nyn_UG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16588 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/om.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/om_ET.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1566 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/om_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   241213 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/or.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/or_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    17627 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/os.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/os_GE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      668 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/os_RU.dat
+-rw-r--r--   0 akx        (501) staff       (20)   244684 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/pa.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3984 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pa_Arab.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pa_Arab_PK.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1249 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pa_Guru.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pa_Guru_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   174311 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/pcm.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pcm_NG.dat
+-rw-r--r--   0 akx        (501) staff       (20)   236139 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/pl.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pl_PL.dat
+-rw-r--r--   0 akx        (501) staff       (20)    20167 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/prg.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1567 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/prg_001.dat
+-rw-r--r--   0 akx        (501) staff       (20)   180248 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/ps.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ps_AF.dat
+-rw-r--r--   0 akx        (501) staff       (20)     7954 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ps_PK.dat
+-rw-r--r--   0 akx        (501) staff       (20)   195079 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/pt.dat
+-rw-r--r--   0 akx        (501) staff       (20)      995 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/pt_AO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/pt_BR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/pt_CH.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1015 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/pt_CV.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pt_GQ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      975 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pt_GW.dat
+-rw-r--r--   0 akx        (501) staff       (20)      645 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pt_LU.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1592 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/pt_MO.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1015 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/pt_MZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    99144 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/pt_PT.dat
+-rw-r--r--   0 akx        (501) staff       (20)      995 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/pt_ST.dat
+-rw-r--r--   0 akx        (501) staff       (20)      975 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/pt_TL.dat
+-rw-r--r--   0 akx        (501) staff       (20)   107964 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/qu.dat
+-rw-r--r--   0 akx        (501) staff       (20)      836 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/qu_BO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      810 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/qu_EC.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/qu_PE.dat
+-rw-r--r--   0 akx        (501) staff       (20)    67934 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/rm.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/rm_CH.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16781 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/rn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/rn_BI.dat
+-rw-r--r--   0 akx        (501) staff       (20)   225782 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/ro.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3215 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ro_MD.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ro_RO.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16170 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/rof.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/rof_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    42432 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/root.dat
+-rw-r--r--   0 akx        (501) staff       (20)   305212 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/ru.dat
+-rw-r--r--   0 akx        (501) staff       (20)      649 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ru_BY.dat
+-rw-r--r--   0 akx        (501) staff       (20)      632 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ru_KG.dat
+-rw-r--r--   0 akx        (501) staff       (20)      629 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ru_KZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ru_MD.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ru_RU.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1747 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ru_UA.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16215 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/rw.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/rw_RW.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16057 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/rwk.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/rwk_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    48180 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sah.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sah_RU.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16455 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/saq.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/saq_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)    12597 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sat.dat
+-rw-r--r--   0 akx        (501) staff       (20)      878 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sat_Olck.dat
+-rw-r--r--   0 akx        (501) staff       (20)      632 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sat_Olck_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16479 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sbp.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sbp_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)   194219 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/sd.dat
+-rw-r--r--   0 akx        (501) staff       (20)      852 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sd_Arab.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sd_Arab_PK.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15216 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sd_Deva.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sd_Deva_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    72353 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/se.dat
+-rw-r--r--   0 akx        (501) staff       (20)    46574 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/se_FI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/se_NO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      667 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/se_SE.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15910 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/seh.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/seh_MZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15998 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ses.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/ses_ML.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16635 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/sg.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sg_CF.dat
+-rw-r--r--   0 akx        (501) staff       (20)    22036 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/shi.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15618 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/shi_Latn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/shi_Latn_MA.dat
+-rw-r--r--   0 akx        (501) staff       (20)      947 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/shi_Tfng.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/shi_Tfng_MA.dat
+-rw-r--r--   0 akx        (501) staff       (20)   244850 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/si.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/si_LK.dat
+-rw-r--r--   0 akx        (501) staff       (20)   256860 2021-04-28 19:26:52.000000 Babel-2.9.1/babel/locale-data/sk.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sk_SK.dat
+-rw-r--r--   0 akx        (501) staff       (20)   241874 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/sl.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sl_SI.dat
+-rw-r--r--   0 akx        (501) staff       (20)    42674 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/smn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/smn_FI.dat
+-rw-r--r--   0 akx        (501) staff       (20)    23252 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/sn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sn_ZW.dat
+-rw-r--r--   0 akx        (501) staff       (20)   153105 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/so.dat
+-rw-r--r--   0 akx        (501) staff       (20)      629 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/so_DJ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      628 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/so_ET.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1181 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/so_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/so_SO.dat
+-rw-r--r--   0 akx        (501) staff       (20)   175659 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/sq.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sq_AL.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1181 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sq_MK.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1160 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sq_XK.dat
+-rw-r--r--   0 akx        (501) staff       (20)   277763 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/sr.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1957 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Cyrl.dat
+-rw-r--r--   0 akx        (501) staff       (20)     4710 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Cyrl_BA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3873 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Cyrl_ME.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Cyrl_RS.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2756 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Cyrl_XK.dat
+-rw-r--r--   0 akx        (501) staff       (20)   230252 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Latn.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3994 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Latn_BA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3074 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Latn_ME.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Latn_RS.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2194 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sr_Latn_XK.dat
+-rw-r--r--   0 akx        (501) staff       (20)    12452 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/su.dat
+-rw-r--r--   0 akx        (501) staff       (20)      718 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/su_Latn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/su_Latn_ID.dat
+-rw-r--r--   0 akx        (501) staff       (20)   221078 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/sv.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sv_AX.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2584 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sv_FI.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/sv_SE.dat
+-rw-r--r--   0 akx        (501) staff       (20)   179207 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/sw.dat
+-rw-r--r--   0 akx        (501) staff       (20)     2660 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sw_CD.dat
+-rw-r--r--   0 akx        (501) staff       (20)    35934 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sw_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sw_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      633 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/sw_UG.dat
+-rw-r--r--   0 akx        (501) staff       (20)   263466 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/ta.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ta_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1181 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ta_LK.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1238 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ta_MY.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1257 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ta_SG.dat
+-rw-r--r--   0 akx        (501) staff       (20)   262280 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/te.dat
+-rw-r--r--   0 akx        (501) staff       (20)      631 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/te_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16671 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/teo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      630 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/teo_KE.dat
+-rw-r--r--   0 akx        (501) staff       (20)      613 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/teo_UG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    36303 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/tg.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/tg_TJ.dat
+-rw-r--r--   0 akx        (501) staff       (20)   235280 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/th.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/th_TH.dat
+-rw-r--r--   0 akx        (501) staff       (20)    73036 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/ti.dat
+-rw-r--r--   0 akx        (501) staff       (20)      958 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ti_ER.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ti_ET.dat
+-rw-r--r--   0 akx        (501) staff       (20)   167927 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/tk.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/tk_TM.dat
+-rw-r--r--   0 akx        (501) staff       (20)   166458 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/to.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/to_TO.dat
+-rw-r--r--   0 akx        (501) staff       (20)   209226 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/tr.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1184 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/tr_CY.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/tr_TR.dat
+-rw-r--r--   0 akx        (501) staff       (20)    33588 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/tt.dat
+-rw-r--r--   0 akx        (501) staff       (20)      626 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/tt_RU.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16171 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/twq.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/twq_NE.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16149 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/tzm.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/tzm_MA.dat
+-rw-r--r--   0 akx        (501) staff       (20)   128534 2021-04-28 19:26:51.000000 Babel-2.9.1/babel/locale-data/ug.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ug_CN.dat
+-rw-r--r--   0 akx        (501) staff       (20)   315834 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/uk.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/uk_UA.dat
+-rw-r--r--   0 akx        (501) staff       (20)   197918 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/ur.dat
+-rw-r--r--   0 akx        (501) staff       (20)    12595 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ur_IN.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/ur_PK.dat
+-rw-r--r--   0 akx        (501) staff       (20)   173590 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/uz.dat
+-rw-r--r--   0 akx        (501) staff       (20)     4111 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/uz_Arab.dat
+-rw-r--r--   0 akx        (501) staff       (20)      651 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/uz_Arab_AF.dat
+-rw-r--r--   0 akx        (501) staff       (20)    98924 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/uz_Cyrl.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/uz_Cyrl_UZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1265 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/uz_Latn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/uz_Latn_UZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    18988 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/vai.dat
+-rw-r--r--   0 akx        (501) staff       (20)    14989 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/vai_Latn.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/vai_Latn_LR.dat
+-rw-r--r--   0 akx        (501) staff       (20)      666 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/vai_Vaii.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/vai_Vaii_LR.dat
+-rw-r--r--   0 akx        (501) staff       (20)   162325 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/vi.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/vi_VN.dat
+-rw-r--r--   0 akx        (501) staff       (20)     5225 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/vo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      823 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/vo_001.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16067 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/vun.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/vun_TZ.dat
+-rw-r--r--   0 akx        (501) staff       (20)    28660 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/wae.dat
+-rw-r--r--   0 akx        (501) staff       (20)      627 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/wae_CH.dat
+-rw-r--r--   0 akx        (501) staff       (20)    25698 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/wo.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/wo_SN.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15055 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/xh.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/xh_ZA.dat
+-rw-r--r--   0 akx        (501) staff       (20)    16555 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/xog.dat
+-rw-r--r--   0 akx        (501) staff       (20)      613 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/xog_UG.dat
+-rw-r--r--   0 akx        (501) staff       (20)    15302 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/yav.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/yav_CM.dat
+-rw-r--r--   0 akx        (501) staff       (20)    30314 2021-04-28 19:26:53.000000 Babel-2.9.1/babel/locale-data/yi.dat
+-rw-r--r--   0 akx        (501) staff       (20)      885 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/yi_001.dat
+-rw-r--r--   0 akx        (501) staff       (20)    68429 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/yo.dat
+-rw-r--r--   0 akx        (501) staff       (20)    34481 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/yo_BJ.dat
+-rw-r--r--   0 akx        (501) staff       (20)      589 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/yo_NG.dat
+-rw-r--r--   0 akx        (501) staff       (20)   183333 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/yue.dat
+-rw-r--r--   0 akx        (501) staff       (20)   183225 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/yue_Hans.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/yue_Hans_CN.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1279 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/yue_Hant.dat
+-rw-r--r--   0 akx        (501) staff       (20)      609 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/yue_Hant_HK.dat
+-rw-r--r--   0 akx        (501) staff       (20)    30498 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/zgh.dat
+-rw-r--r--   0 akx        (501) staff       (20)      590 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zgh_MA.dat
+-rw-r--r--   0 akx        (501) staff       (20)   181044 2021-04-28 19:26:50.000000 Babel-2.9.1/babel/locale-data/zh.dat
+-rw-r--r--   0 akx        (501) staff       (20)     1278 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zh_Hans.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zh_Hans_CN.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3138 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zh_Hans_HK.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3270 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zh_Hans_MO.dat
+-rw-r--r--   0 akx        (501) staff       (20)     3466 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zh_Hans_SG.dat
+-rw-r--r--   0 akx        (501) staff       (20)   185029 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zh_Hant.dat
+-rw-r--r--   0 akx        (501) staff       (20)    56895 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zh_Hant_HK.dat
+-rw-r--r--   0 akx        (501) staff       (20)      630 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zh_Hant_MO.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:56.000000 Babel-2.9.1/babel/locale-data/zh_Hant_TW.dat
+-rw-r--r--   0 akx        (501) staff       (20)   167684 2021-04-28 19:26:54.000000 Babel-2.9.1/babel/locale-data/zu.dat
+-rw-r--r--   0 akx        (501) staff       (20)      608 2021-04-28 19:26:55.000000 Babel-2.9.1/babel/locale-data/zu_ZA.dat
+-rw-r--r--   0 akx        (501) staff       (20)     7931 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/localedata.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.236708 Babel-2.9.1/babel/localtime/
+-rw-r--r--   0 akx        (501) staff       (20)     1721 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/localtime/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)     4801 2018-05-28 09:13:13.000000 Babel-2.9.1/babel/localtime/_unix.py
+-rw-r--r--   0 akx        (501) staff       (20)     3086 2019-02-20 13:12:21.000000 Babel-2.9.1/babel/localtime/_win32.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.238688 Babel-2.9.1/babel/messages/
+-rw-r--r--   0 akx        (501) staff       (20)      254 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/messages/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)    32291 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/messages/catalog.py
+-rw-r--r--   0 akx        (501) staff       (20)     6085 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/messages/checkers.py
+-rw-r--r--   0 akx        (501) staff       (20)    26474 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/messages/extract.py
+-rw-r--r--   0 akx        (501) staff       (20)    38729 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/messages/frontend.py
+-rw-r--r--   0 akx        (501) staff       (20)     6334 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/messages/jslexer.py
+-rw-r--r--   0 akx        (501) staff       (20)     7204 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/messages/mofile.py
+-rw-r--r--   0 akx        (501) staff       (20)     7206 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/messages/plurals.py
+-rw-r--r--   0 akx        (501) staff       (20)    22146 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/messages/pofile.py
+-rw-r--r--   0 akx        (501) staff       (20)    39872 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/numbers.py
+-rw-r--r--   0 akx        (501) staff       (20)    21314 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/plural.py
+-rw-r--r--   0 akx        (501) staff       (20)    22622 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/support.py
+-rw-r--r--   0 akx        (501) staff       (20)    11291 2021-04-28 19:13:49.000000 Babel-2.9.1/babel/units.py
+-rw-r--r--   0 akx        (501) staff       (20)     7576 2021-04-28 19:13:54.000000 Babel-2.9.1/babel/util.py
+-rw-r--r--   0 akx        (501) staff       (20)      533 2020-11-11 10:57:51.000000 Babel-2.9.1/conftest.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.242313 Babel-2.9.1/docs/
+-rw-r--r--   0 akx        (501) staff       (20)     5560 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/Makefile
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.243201 Babel-2.9.1/docs/_static/
+-rw-r--r--   0 akx        (501) staff       (20)    44986 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/_static/logo.pdf
+-rw-r--r--   0 akx        (501) staff       (20)    15484 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/_static/logo.png
+-rw-r--r--   0 akx        (501) staff       (20)     6118 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/_static/logo_small.png
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.243818 Babel-2.9.1/docs/_templates/
+-rw-r--r--   0 akx        (501) staff       (20)      101 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/_templates/sidebar-about.html
+-rw-r--r--   0 akx        (501) staff       (20)      582 2018-07-20 10:31:17.000000 Babel-2.9.1/docs/_templates/sidebar-links.html
+-rw-r--r--   0 akx        (501) staff       (20)      142 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/_templates/sidebar-logo.html
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.244269 Babel-2.9.1/docs/_themes/
+-rw-r--r--   0 akx        (501) staff       (20)     1789 2018-02-02 16:36:50.000000 Babel-2.9.1/docs/_themes/LICENSE
+-rw-r--r--   0 akx        (501) staff       (20)     1093 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/_themes/README
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.244910 Babel-2.9.1/docs/_themes/babel/
+-rw-r--r--   0 akx        (501) staff       (20)      937 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/_themes/babel/layout.html
+-rw-r--r--   0 akx        (501) staff       (20)      590 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/_themes/babel/relations.html
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.245420 Babel-2.9.1/docs/_themes/babel/static/
+-rw-r--r--   0 akx        (501) staff       (20)     6964 2018-02-02 16:36:50.000000 Babel-2.9.1/docs/_themes/babel/static/babel.css_t
+-rw-r--r--   0 akx        (501) staff       (20)      976 2018-02-02 16:36:50.000000 Babel-2.9.1/docs/_themes/babel/static/small_babel.css
+-rw-r--r--   0 akx        (501) staff       (20)      121 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/_themes/babel/theme.conf
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.247939 Babel-2.9.1/docs/api/
+-rw-r--r--   0 akx        (501) staff       (20)      714 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/api/core.rst
+-rw-r--r--   0 akx        (501) staff       (20)     1748 2018-02-02 16:29:02.000000 Babel-2.9.1/docs/api/dates.rst
+-rw-r--r--   0 akx        (501) staff       (20)      249 2018-02-02 16:29:02.000000 Babel-2.9.1/docs/api/index.rst
+-rw-r--r--   0 akx        (501) staff       (20)      290 2018-02-02 16:29:02.000000 Babel-2.9.1/docs/api/languages.rst
+-rw-r--r--   0 akx        (501) staff       (20)      162 2018-02-02 16:29:02.000000 Babel-2.9.1/docs/api/lists.rst
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.249330 Babel-2.9.1/docs/api/messages/
+-rw-r--r--   0 akx        (501) staff       (20)      471 2021-04-28 19:13:49.000000 Babel-2.9.1/docs/api/messages/catalog.rst
+-rw-r--r--   0 akx        (501) staff       (20)      976 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/api/messages/extract.rst
+-rw-r--r--   0 akx        (501) staff       (20)      233 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/api/messages/index.rst
+-rw-r--r--   0 akx        (501) staff       (20)      271 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/api/messages/mofile.rst
+-rw-r--r--   0 akx        (501) staff       (20)      279 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/api/messages/pofile.rst
+-rw-r--r--   0 akx        (501) staff       (20)      900 2018-07-20 10:31:17.000000 Babel-2.9.1/docs/api/numbers.rst
+-rw-r--r--   0 akx        (501) staff       (20)      479 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/api/plural.rst
+-rw-r--r--   0 akx        (501) staff       (20)      418 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/api/support.rst
+-rw-r--r--   0 akx        (501) staff       (20)      232 2018-02-02 16:29:02.000000 Babel-2.9.1/docs/api/units.rst
+-rw-r--r--   0 akx        (501) staff       (20)       24 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/changelog.rst
+-rw-r--r--   0 akx        (501) staff       (20)     6691 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/cmdline.rst
+-rw-r--r--   0 akx        (501) staff       (20)     8368 2021-04-28 19:13:54.000000 Babel-2.9.1/docs/conf.py
+-rw-r--r--   0 akx        (501) staff       (20)    17790 2018-07-20 10:31:17.000000 Babel-2.9.1/docs/dates.rst
+-rw-r--r--   0 akx        (501) staff       (20)     3120 2018-02-02 16:29:02.000000 Babel-2.9.1/docs/dev.rst
+-rw-r--r--   0 akx        (501) staff       (20)      736 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/index.rst
+-rw-r--r--   0 akx        (501) staff       (20)     3022 2019-12-31 09:08:38.000000 Babel-2.9.1/docs/installation.rst
+-rw-r--r--   0 akx        (501) staff       (20)     2172 2018-07-20 10:31:17.000000 Babel-2.9.1/docs/intro.rst
+-rw-r--r--   0 akx        (501) staff       (20)      959 2021-04-28 19:13:49.000000 Babel-2.9.1/docs/license.rst
+-rw-r--r--   0 akx        (501) staff       (20)     4377 2018-07-20 10:31:17.000000 Babel-2.9.1/docs/locale.rst
+-rw-r--r--   0 akx        (501) staff       (20)     5094 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/make.bat
+-rw-r--r--   0 akx        (501) staff       (20)    11768 2019-02-20 13:12:21.000000 Babel-2.9.1/docs/messages.rst
+-rw-r--r--   0 akx        (501) staff       (20)     7444 2021-04-28 19:13:49.000000 Babel-2.9.1/docs/numbers.rst
+-rw-r--r--   0 akx        (501) staff       (20)    15139 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/setup.rst
+-rw-r--r--   0 akx        (501) staff       (20)     1724 2016-11-19 14:05:40.000000 Babel-2.9.1/docs/support.rst
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.251063 Babel-2.9.1/scripts/
+-rwxr-xr-x   0 akx        (501) staff       (20)     3000 2021-04-28 19:13:49.000000 Babel-2.9.1/scripts/download_import_cldr.py
+-rwxr-xr-x   0 akx        (501) staff       (20)     1526 2021-04-28 19:13:54.000000 Babel-2.9.1/scripts/dump_data.py
+-rwxr-xr-x   0 akx        (501) staff       (20)      883 2021-04-28 19:13:54.000000 Babel-2.9.1/scripts/dump_global.py
+-rw-r--r--   0 akx        (501) staff       (20)     1284 2018-05-28 09:13:13.000000 Babel-2.9.1/scripts/generate_authors.py
+-rwxr-xr-x   0 akx        (501) staff       (20)    40922 2021-04-28 19:13:54.000000 Babel-2.9.1/scripts/import_cldr.py
+-rwxr-xr-x   0 akx        (501) staff       (20)     4149 2018-02-02 16:36:50.000000 Babel-2.9.1/scripts/make-release.py
+-rw-r--r--   0 akx        (501) staff       (20)      349 2021-04-28 19:28:20.299051 Babel-2.9.1/setup.cfg
+-rwxr-xr-x   0 akx        (501) staff       (20)     3243 2021-04-28 19:25:28.000000 Babel-2.9.1/setup.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.254545 Babel-2.9.1/tests/
+-rw-r--r--   0 akx        (501) staff       (20)        0 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)      526 2019-12-31 12:09:16.000000 Babel-2.9.1/tests/conftest.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.294191 Babel-2.9.1/tests/messages/
+-rw-r--r--   0 akx        (501) staff       (20)        0 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/__init__.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.294923 Babel-2.9.1/tests/messages/data/
+-rw-r--r--   0 akx        (501) staff       (20)      100 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/mapping.cfg
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.295534 Babel-2.9.1/tests/messages/data/project/
+-rw-r--r--   0 akx        (501) staff       (20)        0 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)      199 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/file1.py
+-rw-r--r--   0 akx        (501) staff       (20)      232 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/file2.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.295988 Babel-2.9.1/tests/messages/data/project/i18n/
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:19.719148 Babel-2.9.1/tests/messages/data/project/i18n/de/
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.296462 Babel-2.9.1/tests/messages/data/project/i18n/de/LC_MESSAGES/
+-rw-r--r--   0 akx        (501) staff       (20)      547 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/i18n/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 akx        (501) staff       (20)      898 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/i18n/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:19.719378 Babel-2.9.1/tests/messages/data/project/i18n/de_DE/
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.297180 Babel-2.9.1/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/
+-rw-r--r--   0 akx        (501) staff       (20)      898 2018-02-02 16:29:02.000000 Babel-2.9.1/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/bar.po
+-rw-r--r--   0 akx        (501) staff       (20)      898 2018-02-02 16:29:02.000000 Babel-2.9.1/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/foo.po
+-rw-r--r--   0 akx        (501) staff       (20)      882 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:19.719609 Babel-2.9.1/tests/messages/data/project/i18n/fi_BUGGY/
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.297427 Babel-2.9.1/tests/messages/data/project/i18n/fi_BUGGY/LC_MESSAGES/
+-rw-r--r--   0 akx        (501) staff       (20)       67 2019-05-27 11:53:30.000000 Babel-2.9.1/tests/messages/data/project/i18n/fi_BUGGY/LC_MESSAGES/messages.po
+-rw-r--r--   0 akx        (501) staff       (20)      823 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/i18n/messages.pot
+-rw-r--r--   0 akx        (501) staff       (20)      814 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/i18n/messages_non_fuzzy.pot
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:19.719828 Babel-2.9.1/tests/messages/data/project/i18n/ru_RU/
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.297666 Babel-2.9.1/tests/messages/data/project/i18n/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 akx        (501) staff       (20)      971 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/i18n/ru_RU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2021-04-28 19:28:20.298282 Babel-2.9.1/tests/messages/data/project/ignored/
+-rw-r--r--   0 akx        (501) staff       (20)       18 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/ignored/a_test_file.txt
+-rw-r--r--   0 akx        (501) staff       (20)        0 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/ignored/an_example.txt
+-rw-r--r--   0 akx        (501) staff       (20)      284 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/project/ignored/this_wont_normally_be_here.py
+-rw-r--r--   0 akx        (501) staff       (20)      172 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/setup.cfg
+-rwxr-xr-x   0 akx        (501) staff       (20)      823 2016-11-19 14:05:40.000000 Babel-2.9.1/tests/messages/data/setup.py
+-rw-r--r--   0 akx        (501) staff       (20)    19449 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/messages/test_catalog.py
+-rw-r--r--   0 akx        (501) staff       (20)    12564 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/messages/test_checkers.py
+-rw-r--r--   0 akx        (501) staff       (20)    20966 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/messages/test_extract.py
+-rw-r--r--   0 akx        (501) staff       (20)    47817 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/messages/test_frontend.py
+-rw-r--r--   0 akx        (501) staff       (20)     4617 2019-05-27 11:55:14.000000 Babel-2.9.1/tests/messages/test_js_extract.py
+-rw-r--r--   0 akx        (501) staff       (20)     3748 2019-05-27 11:55:14.000000 Babel-2.9.1/tests/messages/test_jslexer.py
+-rw-r--r--   0 akx        (501) staff       (20)     3847 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/messages/test_mofile.py
+-rw-r--r--   0 akx        (501) staff       (20)      636 2019-05-27 11:53:30.000000 Babel-2.9.1/tests/messages/test_normalized_string.py
+-rw-r--r--   0 akx        (501) staff       (20)     2598 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/messages/test_plurals.py
+-rw-r--r--   0 akx        (501) staff       (20)    29926 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/messages/test_pofile.py
+-rw-r--r--   0 akx        (501) staff       (20)    12324 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/test_core.py
+-rw-r--r--   0 akx        (501) staff       (20)     1853 2018-02-02 16:29:02.000000 Babel-2.9.1/tests/test_date_intervals.py
+-rw-r--r--   0 akx        (501) staff       (20)    36889 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/test_dates.py
+-rw-r--r--   0 akx        (501) staff       (20)      644 2018-02-02 16:29:02.000000 Babel-2.9.1/tests/test_day_periods.py
+-rw-r--r--   0 akx        (501) staff       (20)      631 2018-02-02 16:29:02.000000 Babel-2.9.1/tests/test_languages.py
+-rw-r--r--   0 akx        (501) staff       (20)      728 2018-02-02 16:29:02.000000 Babel-2.9.1/tests/test_lists.py
+-rw-r--r--   0 akx        (501) staff       (20)     5378 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/test_localedata.py
+-rw-r--r--   0 akx        (501) staff       (20)    32079 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/test_numbers.py
+-rw-r--r--   0 akx        (501) staff       (20)     9269 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/test_plural.py
+-rw-r--r--   0 akx        (501) staff       (20)     1162 2018-05-28 12:52:42.000000 Babel-2.9.1/tests/test_smoke.py
+-rw-r--r--   0 akx        (501) staff       (20)    14765 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/test_support.py
+-rw-r--r--   0 akx        (501) staff       (20)     3312 2021-04-28 19:13:54.000000 Babel-2.9.1/tests/test_util.py
+-rw-r--r--   0 akx        (501) staff       (20)      385 2021-04-28 19:13:49.000000 Babel-2.9.1/tox.ini
```

### Comparing `Babel-2.9.0/AUTHORS` & `Babel-2.9.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/Babel.egg-info/PKG-INFO` & `Babel-2.9.1/Babel.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: Babel
-Version: 2.9.0
+Version: 2.9.1
 Summary: Internationalization utilities
 Home-page: http://babel.pocoo.org/
 Author: Armin Ronacher
 Author-email: armin.ronacher@active-4.com
 License: BSD
 Description: A collection of tools for internationalizing Python applications.
 Platform: UNKNOWN
```

### Comparing `Babel-2.9.0/Babel.egg-info/SOURCES.txt` & `Babel-2.9.1/Babel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/Babel.egg-info/entry_points.txt` & `Babel-2.9.1/Babel.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/CHANGES` & `Babel-2.9.1/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Babel Changelog
 ===============
 
+Version 2.9.1
+-------------
+
+Bugfixes
+~~~~~~~~
+
+* The internal locale-data loading functions now validate the name of the locale file to be loaded and only
+  allow files within Babel's data directory.  Thank you to Chris Lyne of Tenable, Inc. for discovering the issue!
+
 Version 2.9.0
 -------------
 
 Upcoming version support changes
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * This version, Babel 2.9, is the last version of Babel to support Python 2.7, Python 3.4, and Python 3.5.
```

### Comparing `Babel-2.9.0/LICENSE` & `Babel-2.9.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2013-2020 by the Babel Team, see AUTHORS for more information.
+Copyright (c) 2013-2021 by the Babel Team, see AUTHORS for more information.
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
```

### Comparing `Babel-2.9.0/Makefile` & `Babel-2.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/PKG-INFO` & `Babel-2.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: Babel
-Version: 2.9.0
+Version: 2.9.1
 Summary: Internationalization utilities
 Home-page: http://babel.pocoo.org/
 Author: Armin Ronacher
 Author-email: armin.ronacher@active-4.com
 License: BSD
 Description: A collection of tools for internationalizing Python applications.
 Platform: UNKNOWN
```

### Comparing `Babel-2.9.0/README.rst` & `Babel-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/__init__.py` & `Babel-2.9.1/babel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     This package is basically composed of two major parts:
 
      * tools to build and work with ``gettext`` message catalogs
      * a Python interface to the CLDR (Common Locale Data Repository), providing
        access to various locale display names, localized number and date
        formatting, etc.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 from babel.core import UnknownLocaleError, Locale, default_locale, \
     negotiate_locale, parse_locale, get_locale_identifier
 
 
-__version__ = '2.9.0'
+__version__ = '2.9.1'
```

### Comparing `Babel-2.9.0/babel/_compat.py` & `Babel-2.9.1/babel/_compat.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/core.py` & `Babel-2.9.1/babel/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
     babel.core
     ~~~~~~~~~~
 
     Core locale representation and locale data access.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 import os
 
 from babel import localedata
 from babel._compat import pickle, string_types
```

### Comparing `Babel-2.9.0/babel/dates.py` & `Babel-2.9.1/babel/dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     The default locale for the functions in this module is determined by the
     following environment variables, in that order:
 
      * ``LC_TIME``,
      * ``LC_ALL``, and
      * ``LANG``
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 from __future__ import division
 
 import re
 import warnings
```

### Comparing `Babel-2.9.0/babel/global.dat` & `Babel-2.9.1/babel/global.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/languages.py` & `Babel-2.9.1/babel/languages.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/lists.py` & `Babel-2.9.1/babel/lists.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The default locale for the functions in this module is determined by the
     following environment variables, in that order:
 
      * ``LC_ALL``, and
      * ``LANG``
 
-    :copyright: (c) 2015-2020 by the Babel Team.
+    :copyright: (c) 2015-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 from babel.core import Locale, default_locale
 
 DEFAULT_LOCALE = default_locale()
```

### Comparing `Babel-2.9.0/babel/locale-data/af.dat` & `Babel-2.9.1/babel/locale-data/af.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/af_NA.dat` & `Babel-2.9.1/babel/locale-data/af_NA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/af_ZA.dat` & `Babel-2.9.1/babel/locale-data/af_ZA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/agq.dat` & `Babel-2.9.1/babel/locale-data/agq.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/agq_CM.dat` & `Babel-2.9.1/babel/locale-data/agq_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ak.dat` & `Babel-2.9.1/babel/locale-data/ak.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ak_GH.dat` & `Babel-2.9.1/babel/locale-data/ak_GH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/am.dat` & `Babel-2.9.1/babel/locale-data/am.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/am_ET.dat` & `Babel-2.9.1/babel/locale-data/am_ET.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar.dat` & `Babel-2.9.1/babel/locale-data/ar.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_001.dat` & `Babel-2.9.1/babel/locale-data/ar_001.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_AE.dat` & `Babel-2.9.1/babel/locale-data/ar_AE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_BH.dat` & `Babel-2.9.1/babel/locale-data/ar_BH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_DJ.dat` & `Babel-2.9.1/babel/locale-data/ar_DJ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_DZ.dat` & `Babel-2.9.1/babel/locale-data/ar_DZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_EG.dat` & `Babel-2.9.1/babel/locale-data/ar_EG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_EH.dat` & `Babel-2.9.1/babel/locale-data/ar_EH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_ER.dat` & `Babel-2.9.1/babel/locale-data/ar_ER.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_IL.dat` & `Babel-2.9.1/babel/locale-data/ar_IL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_IQ.dat` & `Babel-2.9.1/babel/locale-data/ar_IQ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_JO.dat` & `Babel-2.9.1/babel/locale-data/ar_JO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_KM.dat` & `Babel-2.9.1/babel/locale-data/ar_KM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_KW.dat` & `Babel-2.9.1/babel/locale-data/ar_KW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_LB.dat` & `Babel-2.9.1/babel/locale-data/ar_LB.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_LY.dat` & `Babel-2.9.1/babel/locale-data/ar_LY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_MA.dat` & `Babel-2.9.1/babel/locale-data/ar_MA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_MR.dat` & `Babel-2.9.1/babel/locale-data/ar_MR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_OM.dat` & `Babel-2.9.1/babel/locale-data/ar_OM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_PS.dat` & `Babel-2.9.1/babel/locale-data/ar_PS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_QA.dat` & `Babel-2.9.1/babel/locale-data/ar_QA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_SA.dat` & `Babel-2.9.1/babel/locale-data/ar_SA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_SD.dat` & `Babel-2.9.1/babel/locale-data/ar_SD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_SO.dat` & `Babel-2.9.1/babel/locale-data/ar_SO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_SS.dat` & `Babel-2.9.1/babel/locale-data/ar_SS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_SY.dat` & `Babel-2.9.1/babel/locale-data/ar_SY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_TD.dat` & `Babel-2.9.1/babel/locale-data/ar_TD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_TN.dat` & `Babel-2.9.1/babel/locale-data/ar_TN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ar_YE.dat` & `Babel-2.9.1/babel/locale-data/ar_YE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/as.dat` & `Babel-2.9.1/babel/locale-data/as.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/as_IN.dat` & `Babel-2.9.1/babel/locale-data/as_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/asa.dat` & `Babel-2.9.1/babel/locale-data/asa.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/asa_TZ.dat` & `Babel-2.9.1/babel/locale-data/asa_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ast.dat` & `Babel-2.9.1/babel/locale-data/ast.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ast_ES.dat` & `Babel-2.9.1/babel/locale-data/ast_ES.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/az.dat` & `Babel-2.9.1/babel/locale-data/az.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/az_Cyrl.dat` & `Babel-2.9.1/babel/locale-data/az_Cyrl.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/az_Cyrl_AZ.dat` & `Babel-2.9.1/babel/locale-data/az_Cyrl_AZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/az_Latn.dat` & `Babel-2.9.1/babel/locale-data/az_Latn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/az_Latn_AZ.dat` & `Babel-2.9.1/babel/locale-data/az_Latn_AZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bas.dat` & `Babel-2.9.1/babel/locale-data/bas.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bas_CM.dat` & `Babel-2.9.1/babel/locale-data/bas_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/be.dat` & `Babel-2.9.1/babel/locale-data/be.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/be_BY.dat` & `Babel-2.9.1/babel/locale-data/be_BY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bem.dat` & `Babel-2.9.1/babel/locale-data/bem.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bem_ZM.dat` & `Babel-2.9.1/babel/locale-data/bem_ZM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bez.dat` & `Babel-2.9.1/babel/locale-data/bez.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bez_TZ.dat` & `Babel-2.9.1/babel/locale-data/bez_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bg.dat` & `Babel-2.9.1/babel/locale-data/bg.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bg_BG.dat` & `Babel-2.9.1/babel/locale-data/bg_BG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bm.dat` & `Babel-2.9.1/babel/locale-data/bm.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bm_ML.dat` & `Babel-2.9.1/babel/locale-data/bm_ML.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bn.dat` & `Babel-2.9.1/babel/locale-data/bn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bn_BD.dat` & `Babel-2.9.1/babel/locale-data/bn_BD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bn_IN.dat` & `Babel-2.9.1/babel/locale-data/bn_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bo.dat` & `Babel-2.9.1/babel/locale-data/bo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bo_CN.dat` & `Babel-2.9.1/babel/locale-data/bo_CN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bo_IN.dat` & `Babel-2.9.1/babel/locale-data/bo_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/br.dat` & `Babel-2.9.1/babel/locale-data/br.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/br_FR.dat` & `Babel-2.9.1/babel/locale-data/br_FR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/brx.dat` & `Babel-2.9.1/babel/locale-data/brx.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/brx_IN.dat` & `Babel-2.9.1/babel/locale-data/brx_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bs.dat` & `Babel-2.9.1/babel/locale-data/bs.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bs_Cyrl.dat` & `Babel-2.9.1/babel/locale-data/bs_Cyrl.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bs_Cyrl_BA.dat` & `Babel-2.9.1/babel/locale-data/bs_Cyrl_BA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bs_Latn.dat` & `Babel-2.9.1/babel/locale-data/bs_Latn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/bs_Latn_BA.dat` & `Babel-2.9.1/babel/locale-data/bs_Latn_BA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ca.dat` & `Babel-2.9.1/babel/locale-data/ca.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ca_AD.dat` & `Babel-2.9.1/babel/locale-data/ca_AD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ca_ES.dat` & `Babel-2.9.1/babel/locale-data/ca_ES.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ca_ES_VALENCIA.dat` & `Babel-2.9.1/babel/locale-data/ca_ES_VALENCIA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ca_FR.dat` & `Babel-2.9.1/babel/locale-data/ca_FR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ca_IT.dat` & `Babel-2.9.1/babel/locale-data/ca_IT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ccp.dat` & `Babel-2.9.1/babel/locale-data/ccp.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ccp_BD.dat` & `Babel-2.9.1/babel/locale-data/ccp_BD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ccp_IN.dat` & `Babel-2.9.1/babel/locale-data/ccp_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ce.dat` & `Babel-2.9.1/babel/locale-data/ce.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ce_RU.dat` & `Babel-2.9.1/babel/locale-data/ce_RU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ceb.dat` & `Babel-2.9.1/babel/locale-data/ceb.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ceb_PH.dat` & `Babel-2.9.1/babel/locale-data/ceb_PH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/cgg.dat` & `Babel-2.9.1/babel/locale-data/cgg.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/cgg_UG.dat` & `Babel-2.9.1/babel/locale-data/cgg_UG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/chr.dat` & `Babel-2.9.1/babel/locale-data/chr.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/chr_US.dat` & `Babel-2.9.1/babel/locale-data/chr_US.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ckb.dat` & `Babel-2.9.1/babel/locale-data/ckb.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ckb_IQ.dat` & `Babel-2.9.1/babel/locale-data/ckb_IQ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ckb_IR.dat` & `Babel-2.9.1/babel/locale-data/ckb_IR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/cs.dat` & `Babel-2.9.1/babel/locale-data/cs.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/cs_CZ.dat` & `Babel-2.9.1/babel/locale-data/cs_CZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/cu.dat` & `Babel-2.9.1/babel/locale-data/cu.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/cu_RU.dat` & `Babel-2.9.1/babel/locale-data/cu_RU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/cy.dat` & `Babel-2.9.1/babel/locale-data/cy.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/cy_GB.dat` & `Babel-2.9.1/babel/locale-data/cy_GB.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/da.dat` & `Babel-2.9.1/babel/locale-data/da.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/da_DK.dat` & `Babel-2.9.1/babel/locale-data/da_DK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/da_GL.dat` & `Babel-2.9.1/babel/locale-data/da_GL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dav.dat` & `Babel-2.9.1/babel/locale-data/dav.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dav_KE.dat` & `Babel-2.9.1/babel/locale-data/dav_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/de.dat` & `Babel-2.9.1/babel/locale-data/de.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/de_AT.dat` & `Babel-2.9.1/babel/locale-data/de_AT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/de_BE.dat` & `Babel-2.9.1/babel/locale-data/de_BE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/de_CH.dat` & `Babel-2.9.1/babel/locale-data/de_CH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/de_DE.dat` & `Babel-2.9.1/babel/locale-data/de_DE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/de_IT.dat` & `Babel-2.9.1/babel/locale-data/de_IT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/de_LI.dat` & `Babel-2.9.1/babel/locale-data/de_LI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/de_LU.dat` & `Babel-2.9.1/babel/locale-data/de_LU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dje.dat` & `Babel-2.9.1/babel/locale-data/dje.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dje_NE.dat` & `Babel-2.9.1/babel/locale-data/dje_NE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dsb.dat` & `Babel-2.9.1/babel/locale-data/dsb.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dsb_DE.dat` & `Babel-2.9.1/babel/locale-data/dsb_DE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dua.dat` & `Babel-2.9.1/babel/locale-data/dua.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dua_CM.dat` & `Babel-2.9.1/babel/locale-data/dua_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dyo.dat` & `Babel-2.9.1/babel/locale-data/dyo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dyo_SN.dat` & `Babel-2.9.1/babel/locale-data/dyo_SN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dz.dat` & `Babel-2.9.1/babel/locale-data/dz.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/dz_BT.dat` & `Babel-2.9.1/babel/locale-data/dz_BT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ebu.dat` & `Babel-2.9.1/babel/locale-data/ebu.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ebu_KE.dat` & `Babel-2.9.1/babel/locale-data/ebu_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ee.dat` & `Babel-2.9.1/babel/locale-data/ee.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ee_GH.dat` & `Babel-2.9.1/babel/locale-data/ee_GH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ee_TG.dat` & `Babel-2.9.1/babel/locale-data/ee_TG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/el.dat` & `Babel-2.9.1/babel/locale-data/el.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/el_CY.dat` & `Babel-2.9.1/babel/locale-data/el_CY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/el_GR.dat` & `Babel-2.9.1/babel/locale-data/el_GR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en.dat` & `Babel-2.9.1/babel/locale-data/en.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_001.dat` & `Babel-2.9.1/babel/locale-data/en_001.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_150.dat` & `Babel-2.9.1/babel/locale-data/en_150.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_AE.dat` & `Babel-2.9.1/babel/locale-data/en_AE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_AG.dat` & `Babel-2.9.1/babel/locale-data/en_AG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_AI.dat` & `Babel-2.9.1/babel/locale-data/en_AI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_AS.dat` & `Babel-2.9.1/babel/locale-data/en_AS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_AT.dat` & `Babel-2.9.1/babel/locale-data/en_AT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_AU.dat` & `Babel-2.9.1/babel/locale-data/en_AU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_BB.dat` & `Babel-2.9.1/babel/locale-data/en_BB.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_BE.dat` & `Babel-2.9.1/babel/locale-data/en_BE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_BI.dat` & `Babel-2.9.1/babel/locale-data/en_BI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_BM.dat` & `Babel-2.9.1/babel/locale-data/en_BM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_BS.dat` & `Babel-2.9.1/babel/locale-data/en_BS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_BW.dat` & `Babel-2.9.1/babel/locale-data/en_BW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_BZ.dat` & `Babel-2.9.1/babel/locale-data/en_BZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_CA.dat` & `Babel-2.9.1/babel/locale-data/en_CA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_CC.dat` & `Babel-2.9.1/babel/locale-data/en_CC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_CH.dat` & `Babel-2.9.1/babel/locale-data/en_CH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_CK.dat` & `Babel-2.9.1/babel/locale-data/en_CK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_CM.dat` & `Babel-2.9.1/babel/locale-data/en_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_CX.dat` & `Babel-2.9.1/babel/locale-data/en_CX.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_CY.dat` & `Babel-2.9.1/babel/locale-data/en_CY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_DE.dat` & `Babel-2.9.1/babel/locale-data/en_DE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_DG.dat` & `Babel-2.9.1/babel/locale-data/en_DG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_DK.dat` & `Babel-2.9.1/babel/locale-data/en_DK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_DM.dat` & `Babel-2.9.1/babel/locale-data/en_DM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_ER.dat` & `Babel-2.9.1/babel/locale-data/en_ER.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_FI.dat` & `Babel-2.9.1/babel/locale-data/en_FI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_FJ.dat` & `Babel-2.9.1/babel/locale-data/en_FJ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_FK.dat` & `Babel-2.9.1/babel/locale-data/en_FK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_FM.dat` & `Babel-2.9.1/babel/locale-data/en_FM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_GB.dat` & `Babel-2.9.1/babel/locale-data/en_GB.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_GD.dat` & `Babel-2.9.1/babel/locale-data/en_GD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_GG.dat` & `Babel-2.9.1/babel/locale-data/en_GG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_GH.dat` & `Babel-2.9.1/babel/locale-data/en_GH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_GI.dat` & `Babel-2.9.1/babel/locale-data/en_GI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_GM.dat` & `Babel-2.9.1/babel/locale-data/en_GM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_GU.dat` & `Babel-2.9.1/babel/locale-data/en_GU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_GY.dat` & `Babel-2.9.1/babel/locale-data/en_GY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_HK.dat` & `Babel-2.9.1/babel/locale-data/en_HK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_IE.dat` & `Babel-2.9.1/babel/locale-data/en_IE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_IL.dat` & `Babel-2.9.1/babel/locale-data/en_IL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_IM.dat` & `Babel-2.9.1/babel/locale-data/en_IM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_IN.dat` & `Babel-2.9.1/babel/locale-data/en_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_IO.dat` & `Babel-2.9.1/babel/locale-data/en_IO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_JE.dat` & `Babel-2.9.1/babel/locale-data/en_JE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_JM.dat` & `Babel-2.9.1/babel/locale-data/en_JM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_KE.dat` & `Babel-2.9.1/babel/locale-data/en_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_KI.dat` & `Babel-2.9.1/babel/locale-data/en_KI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_KN.dat` & `Babel-2.9.1/babel/locale-data/en_KN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_KY.dat` & `Babel-2.9.1/babel/locale-data/en_KY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_LC.dat` & `Babel-2.9.1/babel/locale-data/en_LC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_LR.dat` & `Babel-2.9.1/babel/locale-data/en_LR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_LS.dat` & `Babel-2.9.1/babel/locale-data/en_LS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_MG.dat` & `Babel-2.9.1/babel/locale-data/en_MG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_MH.dat` & `Babel-2.9.1/babel/locale-data/en_MH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_MO.dat` & `Babel-2.9.1/babel/locale-data/en_MO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_MP.dat` & `Babel-2.9.1/babel/locale-data/en_MP.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_MS.dat` & `Babel-2.9.1/babel/locale-data/en_MS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_MT.dat` & `Babel-2.9.1/babel/locale-data/en_MT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_MU.dat` & `Babel-2.9.1/babel/locale-data/en_MU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_MW.dat` & `Babel-2.9.1/babel/locale-data/en_MW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_MY.dat` & `Babel-2.9.1/babel/locale-data/en_MY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_NA.dat` & `Babel-2.9.1/babel/locale-data/en_NA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_NF.dat` & `Babel-2.9.1/babel/locale-data/en_NF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_NG.dat` & `Babel-2.9.1/babel/locale-data/en_NG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_NL.dat` & `Babel-2.9.1/babel/locale-data/en_NL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_NR.dat` & `Babel-2.9.1/babel/locale-data/en_NR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_NU.dat` & `Babel-2.9.1/babel/locale-data/en_NU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_NZ.dat` & `Babel-2.9.1/babel/locale-data/en_NZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_PG.dat` & `Babel-2.9.1/babel/locale-data/en_PG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_PH.dat` & `Babel-2.9.1/babel/locale-data/en_PH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_PK.dat` & `Babel-2.9.1/babel/locale-data/en_PK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_PN.dat` & `Babel-2.9.1/babel/locale-data/en_PN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_PR.dat` & `Babel-2.9.1/babel/locale-data/en_PR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_PW.dat` & `Babel-2.9.1/babel/locale-data/en_PW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_RW.dat` & `Babel-2.9.1/babel/locale-data/en_RW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SB.dat` & `Babel-2.9.1/babel/locale-data/en_SB.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SC.dat` & `Babel-2.9.1/babel/locale-data/en_SC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SD.dat` & `Babel-2.9.1/babel/locale-data/en_SD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SE.dat` & `Babel-2.9.1/babel/locale-data/en_SE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SG.dat` & `Babel-2.9.1/babel/locale-data/en_SG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SH.dat` & `Babel-2.9.1/babel/locale-data/en_SH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SI.dat` & `Babel-2.9.1/babel/locale-data/en_SI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SL.dat` & `Babel-2.9.1/babel/locale-data/en_SL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SS.dat` & `Babel-2.9.1/babel/locale-data/en_SS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SX.dat` & `Babel-2.9.1/babel/locale-data/en_SX.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_SZ.dat` & `Babel-2.9.1/babel/locale-data/en_SZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_TC.dat` & `Babel-2.9.1/babel/locale-data/en_TC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_TK.dat` & `Babel-2.9.1/babel/locale-data/en_TK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_TO.dat` & `Babel-2.9.1/babel/locale-data/en_TO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_TT.dat` & `Babel-2.9.1/babel/locale-data/en_TT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_TV.dat` & `Babel-2.9.1/babel/locale-data/en_TV.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_TZ.dat` & `Babel-2.9.1/babel/locale-data/en_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_UG.dat` & `Babel-2.9.1/babel/locale-data/en_UG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_UM.dat` & `Babel-2.9.1/babel/locale-data/en_UM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_US.dat` & `Babel-2.9.1/babel/locale-data/en_US.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_US_POSIX.dat` & `Babel-2.9.1/babel/locale-data/en_US_POSIX.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_VC.dat` & `Babel-2.9.1/babel/locale-data/en_VC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_VG.dat` & `Babel-2.9.1/babel/locale-data/en_VG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_VI.dat` & `Babel-2.9.1/babel/locale-data/en_VI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_VU.dat` & `Babel-2.9.1/babel/locale-data/en_VU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_WS.dat` & `Babel-2.9.1/babel/locale-data/en_WS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_ZA.dat` & `Babel-2.9.1/babel/locale-data/en_ZA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_ZM.dat` & `Babel-2.9.1/babel/locale-data/en_ZM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/en_ZW.dat` & `Babel-2.9.1/babel/locale-data/en_ZW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/eo.dat` & `Babel-2.9.1/babel/locale-data/eo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/eo_001.dat` & `Babel-2.9.1/babel/locale-data/eo_001.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es.dat` & `Babel-2.9.1/babel/locale-data/es.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_419.dat` & `Babel-2.9.1/babel/locale-data/es_419.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_AR.dat` & `Babel-2.9.1/babel/locale-data/es_AR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_BO.dat` & `Babel-2.9.1/babel/locale-data/es_BO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_BR.dat` & `Babel-2.9.1/babel/locale-data/es_BR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_BZ.dat` & `Babel-2.9.1/babel/locale-data/es_BZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_CL.dat` & `Babel-2.9.1/babel/locale-data/es_CL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_CO.dat` & `Babel-2.9.1/babel/locale-data/es_CO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_CR.dat` & `Babel-2.9.1/babel/locale-data/es_CR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_CU.dat` & `Babel-2.9.1/babel/locale-data/es_CU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_DO.dat` & `Babel-2.9.1/babel/locale-data/es_DO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_EA.dat` & `Babel-2.9.1/babel/locale-data/es_EA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_EC.dat` & `Babel-2.9.1/babel/locale-data/es_EC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_ES.dat` & `Babel-2.9.1/babel/locale-data/es_ES.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_GQ.dat` & `Babel-2.9.1/babel/locale-data/es_GQ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_GT.dat` & `Babel-2.9.1/babel/locale-data/es_GT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_HN.dat` & `Babel-2.9.1/babel/locale-data/es_HN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_IC.dat` & `Babel-2.9.1/babel/locale-data/es_IC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_MX.dat` & `Babel-2.9.1/babel/locale-data/es_MX.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_NI.dat` & `Babel-2.9.1/babel/locale-data/es_NI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_PA.dat` & `Babel-2.9.1/babel/locale-data/es_PA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_PE.dat` & `Babel-2.9.1/babel/locale-data/es_PE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_PH.dat` & `Babel-2.9.1/babel/locale-data/es_PH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_PR.dat` & `Babel-2.9.1/babel/locale-data/es_PR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_PY.dat` & `Babel-2.9.1/babel/locale-data/es_PY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_SV.dat` & `Babel-2.9.1/babel/locale-data/es_SV.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_US.dat` & `Babel-2.9.1/babel/locale-data/es_US.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_UY.dat` & `Babel-2.9.1/babel/locale-data/es_UY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/es_VE.dat` & `Babel-2.9.1/babel/locale-data/es_VE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/et.dat` & `Babel-2.9.1/babel/locale-data/et.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/et_EE.dat` & `Babel-2.9.1/babel/locale-data/et_EE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/eu.dat` & `Babel-2.9.1/babel/locale-data/eu.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/eu_ES.dat` & `Babel-2.9.1/babel/locale-data/eu_ES.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ewo.dat` & `Babel-2.9.1/babel/locale-data/ewo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ewo_CM.dat` & `Babel-2.9.1/babel/locale-data/ewo_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fa.dat` & `Babel-2.9.1/babel/locale-data/fa.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fa_AF.dat` & `Babel-2.9.1/babel/locale-data/fa_AF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fa_IR.dat` & `Babel-2.9.1/babel/locale-data/fa_IR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff.dat` & `Babel-2.9.1/babel/locale-data/ff.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_BF.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_BF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_CM.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_GH.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_GH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_GM.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_GM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_GN.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_GN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_GW.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_GW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_LR.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_LR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_MR.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_MR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_NE.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_NE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_NG.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_NG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_SL.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_SL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Adlm_SN.dat` & `Babel-2.9.1/babel/locale-data/ff_Adlm_SN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_BF.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_BF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_CM.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_GH.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_GH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_GM.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_GM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_GN.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_GN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_GW.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_GW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_LR.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_LR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_MR.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_MR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_NE.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_NE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_NG.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_NG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_SL.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_SL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ff_Latn_SN.dat` & `Babel-2.9.1/babel/locale-data/ff_Latn_SN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fi.dat` & `Babel-2.9.1/babel/locale-data/fi.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fi_FI.dat` & `Babel-2.9.1/babel/locale-data/fi_FI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fil.dat` & `Babel-2.9.1/babel/locale-data/fil.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fil_PH.dat` & `Babel-2.9.1/babel/locale-data/fil_PH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fo.dat` & `Babel-2.9.1/babel/locale-data/fo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fo_DK.dat` & `Babel-2.9.1/babel/locale-data/fo_DK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fo_FO.dat` & `Babel-2.9.1/babel/locale-data/fo_FO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr.dat` & `Babel-2.9.1/babel/locale-data/fr.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_BE.dat` & `Babel-2.9.1/babel/locale-data/fr_BE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_BF.dat` & `Babel-2.9.1/babel/locale-data/fr_BF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_BI.dat` & `Babel-2.9.1/babel/locale-data/fr_BI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_BJ.dat` & `Babel-2.9.1/babel/locale-data/fr_BJ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_BL.dat` & `Babel-2.9.1/babel/locale-data/fr_BL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_CA.dat` & `Babel-2.9.1/babel/locale-data/fr_CA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_CD.dat` & `Babel-2.9.1/babel/locale-data/fr_CD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_CF.dat` & `Babel-2.9.1/babel/locale-data/fr_CF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_CG.dat` & `Babel-2.9.1/babel/locale-data/fr_CG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_CH.dat` & `Babel-2.9.1/babel/locale-data/fr_CH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_CI.dat` & `Babel-2.9.1/babel/locale-data/fr_CI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_CM.dat` & `Babel-2.9.1/babel/locale-data/fr_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_DJ.dat` & `Babel-2.9.1/babel/locale-data/fr_DJ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_DZ.dat` & `Babel-2.9.1/babel/locale-data/fr_DZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_FR.dat` & `Babel-2.9.1/babel/locale-data/fr_FR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_GA.dat` & `Babel-2.9.1/babel/locale-data/fr_GA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_GF.dat` & `Babel-2.9.1/babel/locale-data/fr_GF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_GN.dat` & `Babel-2.9.1/babel/locale-data/fr_GN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_GP.dat` & `Babel-2.9.1/babel/locale-data/fr_GP.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_GQ.dat` & `Babel-2.9.1/babel/locale-data/fr_GQ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_HT.dat` & `Babel-2.9.1/babel/locale-data/fr_HT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_KM.dat` & `Babel-2.9.1/babel/locale-data/fr_KM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_LU.dat` & `Babel-2.9.1/babel/locale-data/fr_LU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_MA.dat` & `Babel-2.9.1/babel/locale-data/fr_MA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_MC.dat` & `Babel-2.9.1/babel/locale-data/fr_MC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_MF.dat` & `Babel-2.9.1/babel/locale-data/fr_MF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_MG.dat` & `Babel-2.9.1/babel/locale-data/fr_MG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_ML.dat` & `Babel-2.9.1/babel/locale-data/fr_ML.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_MQ.dat` & `Babel-2.9.1/babel/locale-data/fr_MQ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_MR.dat` & `Babel-2.9.1/babel/locale-data/fr_MR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_MU.dat` & `Babel-2.9.1/babel/locale-data/fr_MU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_NC.dat` & `Babel-2.9.1/babel/locale-data/fr_NC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_NE.dat` & `Babel-2.9.1/babel/locale-data/fr_NE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_PF.dat` & `Babel-2.9.1/babel/locale-data/fr_PF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_PM.dat` & `Babel-2.9.1/babel/locale-data/fr_PM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_RE.dat` & `Babel-2.9.1/babel/locale-data/fr_RE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_RW.dat` & `Babel-2.9.1/babel/locale-data/fr_RW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_SC.dat` & `Babel-2.9.1/babel/locale-data/fr_SC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_SN.dat` & `Babel-2.9.1/babel/locale-data/fr_SN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_SY.dat` & `Babel-2.9.1/babel/locale-data/fr_SY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_TD.dat` & `Babel-2.9.1/babel/locale-data/fr_TD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_TG.dat` & `Babel-2.9.1/babel/locale-data/fr_TG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_TN.dat` & `Babel-2.9.1/babel/locale-data/fr_TN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_VU.dat` & `Babel-2.9.1/babel/locale-data/fr_VU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_WF.dat` & `Babel-2.9.1/babel/locale-data/fr_WF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fr_YT.dat` & `Babel-2.9.1/babel/locale-data/fr_YT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fur.dat` & `Babel-2.9.1/babel/locale-data/fur.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fur_IT.dat` & `Babel-2.9.1/babel/locale-data/fur_IT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fy.dat` & `Babel-2.9.1/babel/locale-data/fy.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/fy_NL.dat` & `Babel-2.9.1/babel/locale-data/fy_NL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ga.dat` & `Babel-2.9.1/babel/locale-data/ga.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ga_GB.dat` & `Babel-2.9.1/babel/locale-data/ga_GB.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ga_IE.dat` & `Babel-2.9.1/babel/locale-data/ga_IE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gd.dat` & `Babel-2.9.1/babel/locale-data/gd.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gd_GB.dat` & `Babel-2.9.1/babel/locale-data/gd_GB.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gl.dat` & `Babel-2.9.1/babel/locale-data/gl.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gl_ES.dat` & `Babel-2.9.1/babel/locale-data/gl_ES.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gsw.dat` & `Babel-2.9.1/babel/locale-data/gsw.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gsw_CH.dat` & `Babel-2.9.1/babel/locale-data/gsw_CH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gsw_FR.dat` & `Babel-2.9.1/babel/locale-data/gsw_FR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gsw_LI.dat` & `Babel-2.9.1/babel/locale-data/gsw_LI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gu.dat` & `Babel-2.9.1/babel/locale-data/gu.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gu_IN.dat` & `Babel-2.9.1/babel/locale-data/gu_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/guz.dat` & `Babel-2.9.1/babel/locale-data/guz.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/guz_KE.dat` & `Babel-2.9.1/babel/locale-data/guz_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gv.dat` & `Babel-2.9.1/babel/locale-data/gv.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/gv_IM.dat` & `Babel-2.9.1/babel/locale-data/gv_IM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ha.dat` & `Babel-2.9.1/babel/locale-data/ha.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ha_GH.dat` & `Babel-2.9.1/babel/locale-data/ha_GH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ha_NE.dat` & `Babel-2.9.1/babel/locale-data/ha_NE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ha_NG.dat` & `Babel-2.9.1/babel/locale-data/ha_NG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/haw.dat` & `Babel-2.9.1/babel/locale-data/haw.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/haw_US.dat` & `Babel-2.9.1/babel/locale-data/haw_US.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/he.dat` & `Babel-2.9.1/babel/locale-data/he.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/he_IL.dat` & `Babel-2.9.1/babel/locale-data/he_IL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hi.dat` & `Babel-2.9.1/babel/locale-data/hi.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hi_IN.dat` & `Babel-2.9.1/babel/locale-data/hi_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hr.dat` & `Babel-2.9.1/babel/locale-data/hr.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hr_BA.dat` & `Babel-2.9.1/babel/locale-data/hr_BA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hr_HR.dat` & `Babel-2.9.1/babel/locale-data/hr_HR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hsb.dat` & `Babel-2.9.1/babel/locale-data/hsb.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hsb_DE.dat` & `Babel-2.9.1/babel/locale-data/hsb_DE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hu.dat` & `Babel-2.9.1/babel/locale-data/hu.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hu_HU.dat` & `Babel-2.9.1/babel/locale-data/hu_HU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hy.dat` & `Babel-2.9.1/babel/locale-data/hy.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/hy_AM.dat` & `Babel-2.9.1/babel/locale-data/hy_AM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ia.dat` & `Babel-2.9.1/babel/locale-data/ia.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ia_001.dat` & `Babel-2.9.1/babel/locale-data/ia_001.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/id.dat` & `Babel-2.9.1/babel/locale-data/id.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/id_ID.dat` & `Babel-2.9.1/babel/locale-data/id_ID.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ig.dat` & `Babel-2.9.1/babel/locale-data/ig.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ig_NG.dat` & `Babel-2.9.1/babel/locale-data/ig_NG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ii.dat` & `Babel-2.9.1/babel/locale-data/ii.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ii_CN.dat` & `Babel-2.9.1/babel/locale-data/ii_CN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/is.dat` & `Babel-2.9.1/babel/locale-data/is.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/is_IS.dat` & `Babel-2.9.1/babel/locale-data/is_IS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/it.dat` & `Babel-2.9.1/babel/locale-data/it.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/it_CH.dat` & `Babel-2.9.1/babel/locale-data/it_CH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/it_IT.dat` & `Babel-2.9.1/babel/locale-data/it_IT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/it_SM.dat` & `Babel-2.9.1/babel/locale-data/it_SM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/it_VA.dat` & `Babel-2.9.1/babel/locale-data/it_VA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ja.dat` & `Babel-2.9.1/babel/locale-data/ja.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ja_JP.dat` & `Babel-2.9.1/babel/locale-data/ja_JP.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/jgo.dat` & `Babel-2.9.1/babel/locale-data/jgo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/jgo_CM.dat` & `Babel-2.9.1/babel/locale-data/jgo_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/jmc.dat` & `Babel-2.9.1/babel/locale-data/jmc.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/jmc_TZ.dat` & `Babel-2.9.1/babel/locale-data/jmc_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/jv.dat` & `Babel-2.9.1/babel/locale-data/jv.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/jv_ID.dat` & `Babel-2.9.1/babel/locale-data/jv_ID.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ka.dat` & `Babel-2.9.1/babel/locale-data/ka.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ka_GE.dat` & `Babel-2.9.1/babel/locale-data/ka_GE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kab.dat` & `Babel-2.9.1/babel/locale-data/kab.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kab_DZ.dat` & `Babel-2.9.1/babel/locale-data/kab_DZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kam.dat` & `Babel-2.9.1/babel/locale-data/kam.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kam_KE.dat` & `Babel-2.9.1/babel/locale-data/kam_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kde.dat` & `Babel-2.9.1/babel/locale-data/kde.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kde_TZ.dat` & `Babel-2.9.1/babel/locale-data/kde_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kea.dat` & `Babel-2.9.1/babel/locale-data/kea.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kea_CV.dat` & `Babel-2.9.1/babel/locale-data/kea_CV.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/khq.dat` & `Babel-2.9.1/babel/locale-data/khq.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/khq_ML.dat` & `Babel-2.9.1/babel/locale-data/khq_ML.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ki.dat` & `Babel-2.9.1/babel/locale-data/ki.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ki_KE.dat` & `Babel-2.9.1/babel/locale-data/ki_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kk.dat` & `Babel-2.9.1/babel/locale-data/kk.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kk_KZ.dat` & `Babel-2.9.1/babel/locale-data/kk_KZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kkj.dat` & `Babel-2.9.1/babel/locale-data/kkj.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kkj_CM.dat` & `Babel-2.9.1/babel/locale-data/kkj_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kl.dat` & `Babel-2.9.1/babel/locale-data/kl.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kl_GL.dat` & `Babel-2.9.1/babel/locale-data/kl_GL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kln.dat` & `Babel-2.9.1/babel/locale-data/kln.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kln_KE.dat` & `Babel-2.9.1/babel/locale-data/kln_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/km.dat` & `Babel-2.9.1/babel/locale-data/km.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/km_KH.dat` & `Babel-2.9.1/babel/locale-data/km_KH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kn.dat` & `Babel-2.9.1/babel/locale-data/kn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kn_IN.dat` & `Babel-2.9.1/babel/locale-data/kn_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ko.dat` & `Babel-2.9.1/babel/locale-data/ko.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ko_KP.dat` & `Babel-2.9.1/babel/locale-data/ko_KP.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ko_KR.dat` & `Babel-2.9.1/babel/locale-data/ko_KR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kok.dat` & `Babel-2.9.1/babel/locale-data/kok.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kok_IN.dat` & `Babel-2.9.1/babel/locale-data/kok_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ks.dat` & `Babel-2.9.1/babel/locale-data/ks.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ks_Arab.dat` & `Babel-2.9.1/babel/locale-data/ks_Arab.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ks_Arab_IN.dat` & `Babel-2.9.1/babel/locale-data/ks_Arab_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ksb.dat` & `Babel-2.9.1/babel/locale-data/ksb.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ksb_TZ.dat` & `Babel-2.9.1/babel/locale-data/ksb_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ksf.dat` & `Babel-2.9.1/babel/locale-data/ksf.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ksf_CM.dat` & `Babel-2.9.1/babel/locale-data/ksf_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ksh.dat` & `Babel-2.9.1/babel/locale-data/ksh.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ksh_DE.dat` & `Babel-2.9.1/babel/locale-data/ksh_DE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ku.dat` & `Babel-2.9.1/babel/locale-data/ku.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ku_TR.dat` & `Babel-2.9.1/babel/locale-data/ku_TR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kw.dat` & `Babel-2.9.1/babel/locale-data/kw.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/kw_GB.dat` & `Babel-2.9.1/babel/locale-data/kw_GB.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ky.dat` & `Babel-2.9.1/babel/locale-data/ky.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ky_KG.dat` & `Babel-2.9.1/babel/locale-data/ky_KG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lag.dat` & `Babel-2.9.1/babel/locale-data/lag.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lag_TZ.dat` & `Babel-2.9.1/babel/locale-data/lag_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lb.dat` & `Babel-2.9.1/babel/locale-data/lb.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lb_LU.dat` & `Babel-2.9.1/babel/locale-data/lb_LU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lg.dat` & `Babel-2.9.1/babel/locale-data/lg.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lg_UG.dat` & `Babel-2.9.1/babel/locale-data/lg_UG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lkt.dat` & `Babel-2.9.1/babel/locale-data/lkt.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lkt_US.dat` & `Babel-2.9.1/babel/locale-data/lkt_US.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ln.dat` & `Babel-2.9.1/babel/locale-data/ln.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ln_AO.dat` & `Babel-2.9.1/babel/locale-data/ln_AO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ln_CD.dat` & `Babel-2.9.1/babel/locale-data/ln_CD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ln_CF.dat` & `Babel-2.9.1/babel/locale-data/ln_CF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ln_CG.dat` & `Babel-2.9.1/babel/locale-data/ln_CG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lo.dat` & `Babel-2.9.1/babel/locale-data/lo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lo_LA.dat` & `Babel-2.9.1/babel/locale-data/lo_LA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lrc.dat` & `Babel-2.9.1/babel/locale-data/lrc.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lrc_IQ.dat` & `Babel-2.9.1/babel/locale-data/lrc_IQ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lrc_IR.dat` & `Babel-2.9.1/babel/locale-data/lrc_IR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lt.dat` & `Babel-2.9.1/babel/locale-data/lt.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lt_LT.dat` & `Babel-2.9.1/babel/locale-data/lt_LT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lu.dat` & `Babel-2.9.1/babel/locale-data/lu.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lu_CD.dat` & `Babel-2.9.1/babel/locale-data/lu_CD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/luo.dat` & `Babel-2.9.1/babel/locale-data/luo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/luo_KE.dat` & `Babel-2.9.1/babel/locale-data/luo_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/luy.dat` & `Babel-2.9.1/babel/locale-data/luy.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/luy_KE.dat` & `Babel-2.9.1/babel/locale-data/luy_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lv.dat` & `Babel-2.9.1/babel/locale-data/lv.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/lv_LV.dat` & `Babel-2.9.1/babel/locale-data/lv_LV.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mai.dat` & `Babel-2.9.1/babel/locale-data/mai.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mai_IN.dat` & `Babel-2.9.1/babel/locale-data/mai_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mas.dat` & `Babel-2.9.1/babel/locale-data/mas.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mas_KE.dat` & `Babel-2.9.1/babel/locale-data/mas_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mas_TZ.dat` & `Babel-2.9.1/babel/locale-data/mas_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mer.dat` & `Babel-2.9.1/babel/locale-data/mer.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mer_KE.dat` & `Babel-2.9.1/babel/locale-data/mer_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mfe.dat` & `Babel-2.9.1/babel/locale-data/mfe.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mfe_MU.dat` & `Babel-2.9.1/babel/locale-data/mfe_MU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mg.dat` & `Babel-2.9.1/babel/locale-data/mg.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mg_MG.dat` & `Babel-2.9.1/babel/locale-data/mg_MG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mgh.dat` & `Babel-2.9.1/babel/locale-data/mgh.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mgh_MZ.dat` & `Babel-2.9.1/babel/locale-data/mgh_MZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mgo.dat` & `Babel-2.9.1/babel/locale-data/mgo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mgo_CM.dat` & `Babel-2.9.1/babel/locale-data/mgo_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mi.dat` & `Babel-2.9.1/babel/locale-data/mi.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mi_NZ.dat` & `Babel-2.9.1/babel/locale-data/mi_NZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mk.dat` & `Babel-2.9.1/babel/locale-data/mk.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mk_MK.dat` & `Babel-2.9.1/babel/locale-data/mk_MK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ml.dat` & `Babel-2.9.1/babel/locale-data/ml.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ml_IN.dat` & `Babel-2.9.1/babel/locale-data/ml_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mn.dat` & `Babel-2.9.1/babel/locale-data/mn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mn_MN.dat` & `Babel-2.9.1/babel/locale-data/mn_MN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mni.dat` & `Babel-2.9.1/babel/locale-data/mni.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mni_Beng.dat` & `Babel-2.9.1/babel/locale-data/mni_Beng.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mni_Beng_IN.dat` & `Babel-2.9.1/babel/locale-data/mni_Beng_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mr.dat` & `Babel-2.9.1/babel/locale-data/mr.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mr_IN.dat` & `Babel-2.9.1/babel/locale-data/mr_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ms.dat` & `Babel-2.9.1/babel/locale-data/ms.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ms_BN.dat` & `Babel-2.9.1/babel/locale-data/ms_BN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ms_ID.dat` & `Babel-2.9.1/babel/locale-data/ms_ID.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ms_MY.dat` & `Babel-2.9.1/babel/locale-data/ms_MY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ms_SG.dat` & `Babel-2.9.1/babel/locale-data/ms_SG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mt.dat` & `Babel-2.9.1/babel/locale-data/mt.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mt_MT.dat` & `Babel-2.9.1/babel/locale-data/mt_MT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mua.dat` & `Babel-2.9.1/babel/locale-data/mua.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mua_CM.dat` & `Babel-2.9.1/babel/locale-data/mua_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/my.dat` & `Babel-2.9.1/babel/locale-data/my.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/my_MM.dat` & `Babel-2.9.1/babel/locale-data/my_MM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mzn.dat` & `Babel-2.9.1/babel/locale-data/mzn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/mzn_IR.dat` & `Babel-2.9.1/babel/locale-data/mzn_IR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/naq.dat` & `Babel-2.9.1/babel/locale-data/naq.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/naq_NA.dat` & `Babel-2.9.1/babel/locale-data/naq_NA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nb.dat` & `Babel-2.9.1/babel/locale-data/nb.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nb_NO.dat` & `Babel-2.9.1/babel/locale-data/nb_NO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nb_SJ.dat` & `Babel-2.9.1/babel/locale-data/nb_SJ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nd.dat` & `Babel-2.9.1/babel/locale-data/nd.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nd_ZW.dat` & `Babel-2.9.1/babel/locale-data/nd_ZW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nds.dat` & `Babel-2.9.1/babel/locale-data/nds.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nds_DE.dat` & `Babel-2.9.1/babel/locale-data/nds_DE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nds_NL.dat` & `Babel-2.9.1/babel/locale-data/nds_NL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ne.dat` & `Babel-2.9.1/babel/locale-data/ne.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ne_IN.dat` & `Babel-2.9.1/babel/locale-data/ne_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ne_NP.dat` & `Babel-2.9.1/babel/locale-data/ne_NP.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nl.dat` & `Babel-2.9.1/babel/locale-data/nl.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nl_AW.dat` & `Babel-2.9.1/babel/locale-data/nl_AW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nl_BE.dat` & `Babel-2.9.1/babel/locale-data/nl_BE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nl_BQ.dat` & `Babel-2.9.1/babel/locale-data/nl_BQ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nl_CW.dat` & `Babel-2.9.1/babel/locale-data/nl_CW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nl_NL.dat` & `Babel-2.9.1/babel/locale-data/nl_NL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nl_SR.dat` & `Babel-2.9.1/babel/locale-data/nl_SR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nl_SX.dat` & `Babel-2.9.1/babel/locale-data/nl_SX.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nmg.dat` & `Babel-2.9.1/babel/locale-data/nmg.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nmg_CM.dat` & `Babel-2.9.1/babel/locale-data/nmg_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nn.dat` & `Babel-2.9.1/babel/locale-data/nn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nn_NO.dat` & `Babel-2.9.1/babel/locale-data/nn_NO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nnh.dat` & `Babel-2.9.1/babel/locale-data/nnh.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nnh_CM.dat` & `Babel-2.9.1/babel/locale-data/nnh_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nus.dat` & `Babel-2.9.1/babel/locale-data/nus.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nus_SS.dat` & `Babel-2.9.1/babel/locale-data/nus_SS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nyn.dat` & `Babel-2.9.1/babel/locale-data/nyn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/nyn_UG.dat` & `Babel-2.9.1/babel/locale-data/nyn_UG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/om.dat` & `Babel-2.9.1/babel/locale-data/om.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/om_ET.dat` & `Babel-2.9.1/babel/locale-data/om_ET.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/om_KE.dat` & `Babel-2.9.1/babel/locale-data/om_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/or.dat` & `Babel-2.9.1/babel/locale-data/or.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/or_IN.dat` & `Babel-2.9.1/babel/locale-data/or_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/os.dat` & `Babel-2.9.1/babel/locale-data/os.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/os_GE.dat` & `Babel-2.9.1/babel/locale-data/os_GE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/os_RU.dat` & `Babel-2.9.1/babel/locale-data/os_RU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pa.dat` & `Babel-2.9.1/babel/locale-data/pa.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pa_Arab.dat` & `Babel-2.9.1/babel/locale-data/pa_Arab.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pa_Arab_PK.dat` & `Babel-2.9.1/babel/locale-data/pa_Arab_PK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pa_Guru.dat` & `Babel-2.9.1/babel/locale-data/pa_Guru.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pa_Guru_IN.dat` & `Babel-2.9.1/babel/locale-data/pa_Guru_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pcm.dat` & `Babel-2.9.1/babel/locale-data/pcm.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pcm_NG.dat` & `Babel-2.9.1/babel/locale-data/pcm_NG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pl.dat` & `Babel-2.9.1/babel/locale-data/pl.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pl_PL.dat` & `Babel-2.9.1/babel/locale-data/pl_PL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/prg.dat` & `Babel-2.9.1/babel/locale-data/prg.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/prg_001.dat` & `Babel-2.9.1/babel/locale-data/prg_001.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ps.dat` & `Babel-2.9.1/babel/locale-data/ps.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ps_AF.dat` & `Babel-2.9.1/babel/locale-data/ps_AF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ps_PK.dat` & `Babel-2.9.1/babel/locale-data/ps_PK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt.dat` & `Babel-2.9.1/babel/locale-data/pt.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_AO.dat` & `Babel-2.9.1/babel/locale-data/pt_AO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_BR.dat` & `Babel-2.9.1/babel/locale-data/pt_BR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_CH.dat` & `Babel-2.9.1/babel/locale-data/pt_CH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_CV.dat` & `Babel-2.9.1/babel/locale-data/pt_CV.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_GQ.dat` & `Babel-2.9.1/babel/locale-data/pt_GQ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_GW.dat` & `Babel-2.9.1/babel/locale-data/pt_GW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_LU.dat` & `Babel-2.9.1/babel/locale-data/pt_LU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_MO.dat` & `Babel-2.9.1/babel/locale-data/pt_MO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_MZ.dat` & `Babel-2.9.1/babel/locale-data/pt_MZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_PT.dat` & `Babel-2.9.1/babel/locale-data/pt_PT.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_ST.dat` & `Babel-2.9.1/babel/locale-data/pt_ST.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/pt_TL.dat` & `Babel-2.9.1/babel/locale-data/pt_TL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/qu.dat` & `Babel-2.9.1/babel/locale-data/qu.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/qu_BO.dat` & `Babel-2.9.1/babel/locale-data/qu_BO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/qu_EC.dat` & `Babel-2.9.1/babel/locale-data/qu_EC.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/qu_PE.dat` & `Babel-2.9.1/babel/locale-data/qu_PE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rm.dat` & `Babel-2.9.1/babel/locale-data/rm.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rm_CH.dat` & `Babel-2.9.1/babel/locale-data/rm_CH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rn.dat` & `Babel-2.9.1/babel/locale-data/rn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rn_BI.dat` & `Babel-2.9.1/babel/locale-data/rn_BI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ro.dat` & `Babel-2.9.1/babel/locale-data/ro.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ro_MD.dat` & `Babel-2.9.1/babel/locale-data/ro_MD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ro_RO.dat` & `Babel-2.9.1/babel/locale-data/ro_RO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rof.dat` & `Babel-2.9.1/babel/locale-data/rof.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rof_TZ.dat` & `Babel-2.9.1/babel/locale-data/rof_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/root.dat` & `Babel-2.9.1/babel/locale-data/root.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ru.dat` & `Babel-2.9.1/babel/locale-data/ru.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ru_BY.dat` & `Babel-2.9.1/babel/locale-data/ru_BY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ru_KG.dat` & `Babel-2.9.1/babel/locale-data/ru_KG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ru_KZ.dat` & `Babel-2.9.1/babel/locale-data/ru_KZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ru_MD.dat` & `Babel-2.9.1/babel/locale-data/ru_MD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ru_RU.dat` & `Babel-2.9.1/babel/locale-data/ru_RU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ru_UA.dat` & `Babel-2.9.1/babel/locale-data/ru_UA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rw.dat` & `Babel-2.9.1/babel/locale-data/rw.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rw_RW.dat` & `Babel-2.9.1/babel/locale-data/rw_RW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rwk.dat` & `Babel-2.9.1/babel/locale-data/rwk.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/rwk_TZ.dat` & `Babel-2.9.1/babel/locale-data/rwk_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sah.dat` & `Babel-2.9.1/babel/locale-data/sah.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sah_RU.dat` & `Babel-2.9.1/babel/locale-data/sah_RU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/saq.dat` & `Babel-2.9.1/babel/locale-data/saq.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/saq_KE.dat` & `Babel-2.9.1/babel/locale-data/saq_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sat.dat` & `Babel-2.9.1/babel/locale-data/sat.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sat_Olck.dat` & `Babel-2.9.1/babel/locale-data/sat_Olck.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sat_Olck_IN.dat` & `Babel-2.9.1/babel/locale-data/sat_Olck_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sbp.dat` & `Babel-2.9.1/babel/locale-data/sbp.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sbp_TZ.dat` & `Babel-2.9.1/babel/locale-data/sbp_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sd.dat` & `Babel-2.9.1/babel/locale-data/sd.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sd_Arab.dat` & `Babel-2.9.1/babel/locale-data/sd_Arab.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sd_Arab_PK.dat` & `Babel-2.9.1/babel/locale-data/sd_Arab_PK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sd_Deva.dat` & `Babel-2.9.1/babel/locale-data/sd_Deva.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sd_Deva_IN.dat` & `Babel-2.9.1/babel/locale-data/sd_Deva_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/se.dat` & `Babel-2.9.1/babel/locale-data/se.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/se_FI.dat` & `Babel-2.9.1/babel/locale-data/se_FI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/se_NO.dat` & `Babel-2.9.1/babel/locale-data/se_NO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/se_SE.dat` & `Babel-2.9.1/babel/locale-data/se_SE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/seh.dat` & `Babel-2.9.1/babel/locale-data/seh.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/seh_MZ.dat` & `Babel-2.9.1/babel/locale-data/seh_MZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ses.dat` & `Babel-2.9.1/babel/locale-data/ses.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ses_ML.dat` & `Babel-2.9.1/babel/locale-data/ses_ML.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sg.dat` & `Babel-2.9.1/babel/locale-data/sg.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sg_CF.dat` & `Babel-2.9.1/babel/locale-data/sg_CF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/shi.dat` & `Babel-2.9.1/babel/locale-data/shi.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/shi_Latn.dat` & `Babel-2.9.1/babel/locale-data/shi_Latn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/shi_Latn_MA.dat` & `Babel-2.9.1/babel/locale-data/shi_Latn_MA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/shi_Tfng.dat` & `Babel-2.9.1/babel/locale-data/shi_Tfng.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/shi_Tfng_MA.dat` & `Babel-2.9.1/babel/locale-data/shi_Tfng_MA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/si.dat` & `Babel-2.9.1/babel/locale-data/si.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/si_LK.dat` & `Babel-2.9.1/babel/locale-data/si_LK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sk.dat` & `Babel-2.9.1/babel/locale-data/sk.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sk_SK.dat` & `Babel-2.9.1/babel/locale-data/sk_SK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sl.dat` & `Babel-2.9.1/babel/locale-data/sl.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sl_SI.dat` & `Babel-2.9.1/babel/locale-data/sl_SI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/smn.dat` & `Babel-2.9.1/babel/locale-data/smn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/smn_FI.dat` & `Babel-2.9.1/babel/locale-data/smn_FI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sn.dat` & `Babel-2.9.1/babel/locale-data/sn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sn_ZW.dat` & `Babel-2.9.1/babel/locale-data/sn_ZW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/so.dat` & `Babel-2.9.1/babel/locale-data/so.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/so_DJ.dat` & `Babel-2.9.1/babel/locale-data/so_DJ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/so_ET.dat` & `Babel-2.9.1/babel/locale-data/so_ET.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/so_KE.dat` & `Babel-2.9.1/babel/locale-data/so_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/so_SO.dat` & `Babel-2.9.1/babel/locale-data/so_SO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sq.dat` & `Babel-2.9.1/babel/locale-data/sq.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sq_AL.dat` & `Babel-2.9.1/babel/locale-data/sq_AL.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sq_MK.dat` & `Babel-2.9.1/babel/locale-data/sq_MK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sq_XK.dat` & `Babel-2.9.1/babel/locale-data/sq_XK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr.dat` & `Babel-2.9.1/babel/locale-data/sr.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Cyrl.dat` & `Babel-2.9.1/babel/locale-data/sr_Cyrl.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Cyrl_BA.dat` & `Babel-2.9.1/babel/locale-data/sr_Cyrl_BA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Cyrl_ME.dat` & `Babel-2.9.1/babel/locale-data/sr_Cyrl_ME.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Cyrl_RS.dat` & `Babel-2.9.1/babel/locale-data/sr_Cyrl_RS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Cyrl_XK.dat` & `Babel-2.9.1/babel/locale-data/sr_Cyrl_XK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Latn.dat` & `Babel-2.9.1/babel/locale-data/sr_Latn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Latn_BA.dat` & `Babel-2.9.1/babel/locale-data/sr_Latn_BA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Latn_ME.dat` & `Babel-2.9.1/babel/locale-data/sr_Latn_ME.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Latn_RS.dat` & `Babel-2.9.1/babel/locale-data/sr_Latn_RS.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sr_Latn_XK.dat` & `Babel-2.9.1/babel/locale-data/sr_Latn_XK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/su.dat` & `Babel-2.9.1/babel/locale-data/su.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/su_Latn.dat` & `Babel-2.9.1/babel/locale-data/su_Latn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/su_Latn_ID.dat` & `Babel-2.9.1/babel/locale-data/su_Latn_ID.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sv.dat` & `Babel-2.9.1/babel/locale-data/sv.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sv_AX.dat` & `Babel-2.9.1/babel/locale-data/sv_AX.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sv_FI.dat` & `Babel-2.9.1/babel/locale-data/sv_FI.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sv_SE.dat` & `Babel-2.9.1/babel/locale-data/sv_SE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sw.dat` & `Babel-2.9.1/babel/locale-data/sw.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sw_CD.dat` & `Babel-2.9.1/babel/locale-data/sw_CD.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sw_KE.dat` & `Babel-2.9.1/babel/locale-data/sw_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sw_TZ.dat` & `Babel-2.9.1/babel/locale-data/sw_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/sw_UG.dat` & `Babel-2.9.1/babel/locale-data/sw_UG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ta.dat` & `Babel-2.9.1/babel/locale-data/ta.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ta_IN.dat` & `Babel-2.9.1/babel/locale-data/ta_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ta_LK.dat` & `Babel-2.9.1/babel/locale-data/ta_LK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ta_MY.dat` & `Babel-2.9.1/babel/locale-data/ta_MY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ta_SG.dat` & `Babel-2.9.1/babel/locale-data/ta_SG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/te.dat` & `Babel-2.9.1/babel/locale-data/te.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/te_IN.dat` & `Babel-2.9.1/babel/locale-data/te_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/teo.dat` & `Babel-2.9.1/babel/locale-data/teo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/teo_KE.dat` & `Babel-2.9.1/babel/locale-data/teo_KE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/teo_UG.dat` & `Babel-2.9.1/babel/locale-data/teo_UG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tg.dat` & `Babel-2.9.1/babel/locale-data/tg.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tg_TJ.dat` & `Babel-2.9.1/babel/locale-data/tg_TJ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/th.dat` & `Babel-2.9.1/babel/locale-data/th.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/th_TH.dat` & `Babel-2.9.1/babel/locale-data/th_TH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ti.dat` & `Babel-2.9.1/babel/locale-data/ti.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ti_ER.dat` & `Babel-2.9.1/babel/locale-data/ti_ER.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ti_ET.dat` & `Babel-2.9.1/babel/locale-data/ti_ET.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tk.dat` & `Babel-2.9.1/babel/locale-data/tk.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tk_TM.dat` & `Babel-2.9.1/babel/locale-data/tk_TM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/to.dat` & `Babel-2.9.1/babel/locale-data/to.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/to_TO.dat` & `Babel-2.9.1/babel/locale-data/to_TO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tr.dat` & `Babel-2.9.1/babel/locale-data/tr.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tr_CY.dat` & `Babel-2.9.1/babel/locale-data/tr_CY.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tr_TR.dat` & `Babel-2.9.1/babel/locale-data/tr_TR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tt.dat` & `Babel-2.9.1/babel/locale-data/tt.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tt_RU.dat` & `Babel-2.9.1/babel/locale-data/tt_RU.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/twq.dat` & `Babel-2.9.1/babel/locale-data/twq.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/twq_NE.dat` & `Babel-2.9.1/babel/locale-data/twq_NE.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tzm.dat` & `Babel-2.9.1/babel/locale-data/tzm.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/tzm_MA.dat` & `Babel-2.9.1/babel/locale-data/tzm_MA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ug.dat` & `Babel-2.9.1/babel/locale-data/ug.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ug_CN.dat` & `Babel-2.9.1/babel/locale-data/ug_CN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/uk.dat` & `Babel-2.9.1/babel/locale-data/uk.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/uk_UA.dat` & `Babel-2.9.1/babel/locale-data/uk_UA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ur.dat` & `Babel-2.9.1/babel/locale-data/ur.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ur_IN.dat` & `Babel-2.9.1/babel/locale-data/ur_IN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/ur_PK.dat` & `Babel-2.9.1/babel/locale-data/ur_PK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/uz.dat` & `Babel-2.9.1/babel/locale-data/uz.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/uz_Arab.dat` & `Babel-2.9.1/babel/locale-data/uz_Arab.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/uz_Arab_AF.dat` & `Babel-2.9.1/babel/locale-data/uz_Arab_AF.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/uz_Cyrl.dat` & `Babel-2.9.1/babel/locale-data/uz_Cyrl.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/uz_Cyrl_UZ.dat` & `Babel-2.9.1/babel/locale-data/uz_Cyrl_UZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/uz_Latn.dat` & `Babel-2.9.1/babel/locale-data/uz_Latn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/uz_Latn_UZ.dat` & `Babel-2.9.1/babel/locale-data/uz_Latn_UZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vai.dat` & `Babel-2.9.1/babel/locale-data/vai.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vai_Latn.dat` & `Babel-2.9.1/babel/locale-data/vai_Latn.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vai_Latn_LR.dat` & `Babel-2.9.1/babel/locale-data/vai_Latn_LR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vai_Vaii.dat` & `Babel-2.9.1/babel/locale-data/vai_Vaii.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vai_Vaii_LR.dat` & `Babel-2.9.1/babel/locale-data/vai_Vaii_LR.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vi.dat` & `Babel-2.9.1/babel/locale-data/vi.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vi_VN.dat` & `Babel-2.9.1/babel/locale-data/vi_VN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vo.dat` & `Babel-2.9.1/babel/locale-data/vo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vo_001.dat` & `Babel-2.9.1/babel/locale-data/vo_001.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vun.dat` & `Babel-2.9.1/babel/locale-data/vun.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/vun_TZ.dat` & `Babel-2.9.1/babel/locale-data/vun_TZ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/wae.dat` & `Babel-2.9.1/babel/locale-data/wae.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/wae_CH.dat` & `Babel-2.9.1/babel/locale-data/wae_CH.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/wo.dat` & `Babel-2.9.1/babel/locale-data/wo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/wo_SN.dat` & `Babel-2.9.1/babel/locale-data/wo_SN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/xh.dat` & `Babel-2.9.1/babel/locale-data/xh.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/xh_ZA.dat` & `Babel-2.9.1/babel/locale-data/xh_ZA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/xog.dat` & `Babel-2.9.1/babel/locale-data/xog.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/xog_UG.dat` & `Babel-2.9.1/babel/locale-data/xog_UG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yav.dat` & `Babel-2.9.1/babel/locale-data/yav.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yav_CM.dat` & `Babel-2.9.1/babel/locale-data/yav_CM.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yi.dat` & `Babel-2.9.1/babel/locale-data/yi.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yi_001.dat` & `Babel-2.9.1/babel/locale-data/yi_001.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yo.dat` & `Babel-2.9.1/babel/locale-data/yo.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yo_BJ.dat` & `Babel-2.9.1/babel/locale-data/yo_BJ.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yo_NG.dat` & `Babel-2.9.1/babel/locale-data/yo_NG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yue.dat` & `Babel-2.9.1/babel/locale-data/yue.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yue_Hans.dat` & `Babel-2.9.1/babel/locale-data/yue_Hans.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yue_Hans_CN.dat` & `Babel-2.9.1/babel/locale-data/yue_Hans_CN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yue_Hant.dat` & `Babel-2.9.1/babel/locale-data/yue_Hant.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/yue_Hant_HK.dat` & `Babel-2.9.1/babel/locale-data/yue_Hant_HK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zgh.dat` & `Babel-2.9.1/babel/locale-data/zgh.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zgh_MA.dat` & `Babel-2.9.1/babel/locale-data/zgh_MA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh.dat` & `Babel-2.9.1/babel/locale-data/zh.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh_Hans.dat` & `Babel-2.9.1/babel/locale-data/zh_Hans.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh_Hans_CN.dat` & `Babel-2.9.1/babel/locale-data/zh_Hans_CN.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh_Hans_HK.dat` & `Babel-2.9.1/babel/locale-data/zh_Hans_HK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh_Hans_MO.dat` & `Babel-2.9.1/babel/locale-data/zh_Hans_MO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh_Hans_SG.dat` & `Babel-2.9.1/babel/locale-data/zh_Hans_SG.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh_Hant.dat` & `Babel-2.9.1/babel/locale-data/zh_Hant.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh_Hant_HK.dat` & `Babel-2.9.1/babel/locale-data/zh_Hant_HK.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh_Hant_MO.dat` & `Babel-2.9.1/babel/locale-data/zh_Hant_MO.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zh_Hant_TW.dat` & `Babel-2.9.1/babel/locale-data/zh_Hant_TW.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zu.dat` & `Babel-2.9.1/babel/locale-data/zu.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/locale-data/zu_ZA.dat` & `Babel-2.9.1/babel/locale-data/zu_ZA.dat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/localedata.py` & `Babel-2.9.1/babel/localedata.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,31 @@
     ~~~~~~~~~~~~~~~~
 
     Low-level locale data access.
 
     :note: The `Locale` class, which uses this module under the hood, provides a
            more convenient interface for accessing the locale data.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 import os
+import re
+import sys
 import threading
 from itertools import chain
 
 from babel._compat import pickle, string_types, abc
 
 
 _cache = {}
 _cache_lock = threading.RLock()
 _dirname = os.path.join(os.path.dirname(__file__), 'locale-data')
+_windows_reserved_name_re = re.compile("^(con|prn|aux|nul|com[0-9]|lpt[0-9])$", re.I)
 
 
 def normalize_locale(name):
     """Normalize a locale ID by stripping spaces and apply proper casing.
 
     Returns the normalized locale ID string or `None` if the ID is not
     recognized.
@@ -34,26 +37,42 @@
         return None
     name = name.strip().lower()
     for locale_id in chain.from_iterable([_cache, locale_identifiers()]):
         if name == locale_id.lower():
             return locale_id
 
 
+def resolve_locale_filename(name):
+    """
+    Resolve a locale identifier to a `.dat` path on disk.
+    """
+
+    # Clean up any possible relative paths.
+    name = os.path.basename(name)
+
+    # Ensure we're not left with one of the Windows reserved names.
+    if sys.platform == "win32" and _windows_reserved_name_re.match(os.path.splitext(name)[0]):
+        raise ValueError("Name %s is invalid on Windows" % name)
+
+    # Build the path.
+    return os.path.join(_dirname, '%s.dat' % name)
+
+
 def exists(name):
     """Check whether locale data is available for the given locale.
 
     Returns `True` if it exists, `False` otherwise.
 
     :param name: the locale identifier string
     """
     if not name or not isinstance(name, string_types):
         return False
     if name in _cache:
         return True
-    file_found = os.path.exists(os.path.join(_dirname, '%s.dat' % name))
+    file_found = os.path.exists(resolve_locale_filename(name))
     return True if file_found else bool(normalize_locale(name))
 
 
 def locale_identifiers():
     """Return a list of all locale identifiers for which locale data is
     available.
 
@@ -98,14 +117,15 @@
 
     :param name: the locale identifier string (or "root")
     :param merge_inherited: whether the inherited data should be merged into
                             the data of the requested locale
     :raise `IOError`: if no locale data file is found for the given locale
                       identifer, or one of the locales it inherits from
     """
+    name = os.path.basename(name)
     _cache_lock.acquire()
     try:
         data = _cache.get(name)
         if not data:
             # Load inherited data
             if name == 'root' or not merge_inherited:
                 data = {}
@@ -115,15 +135,15 @@
                 if not parent:
                     parts = name.split('_')
                     if len(parts) == 1:
                         parent = 'root'
                     else:
                         parent = '_'.join(parts[:-1])
                 data = load(parent).copy()
-            filename = os.path.join(_dirname, '%s.dat' % name)
+            filename = resolve_locale_filename(name)
             with open(filename, 'rb') as fileobj:
                 if name != 'root' and merge_inherited:
                     merge(data, pickle.load(fileobj))
                 else:
                     data = pickle.load(fileobj)
             _cache[name] = data
         return data
```

### Comparing `Babel-2.9.0/babel/localtime/__init__.py` & `Babel-2.9.1/babel/localtime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
     babel.localtime
     ~~~~~~~~~~~~~~~
 
     Babel specific fork of tzlocal to determine the local timezone
     of the system.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 import sys
 import pytz
 import time
 from datetime import timedelta
```

### Comparing `Babel-2.9.0/babel/localtime/_unix.py` & `Babel-2.9.1/babel/localtime/_unix.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/localtime/_win32.py` & `Babel-2.9.1/babel/localtime/_win32.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/messages/catalog.py` & `Babel-2.9.1/babel/messages/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
     babel.messages.catalog
     ~~~~~~~~~~~~~~~~~~~~~~
 
     Data structures for message catalogs.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 import re
 import time
 
 from cgi import parse_header
```

### Comparing `Babel-2.9.0/babel/messages/checkers.py` & `Babel-2.9.1/babel/messages/checkers.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     babel.messages.checkers
     ~~~~~~~~~~~~~~~~~~~~~~~
 
     Various routines that help with validation of translations.
 
     :since: version 0.9
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 from babel.messages.catalog import TranslationError, PYTHON_FORMAT
 from babel._compat import string_types, izip
```

### Comparing `Babel-2.9.0/babel/messages/extract.py` & `Babel-2.9.1/babel/messages/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     strings from a variety of sources. A native extractor for Python source
     files is builtin, extractors for other sources can be added using very
     simple plugins.
 
     The main entry points into the extraction functionality are the functions
     `extract_from_dir` and `extract_from_file`.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 import os
 from os.path import relpath
 import sys
 from tokenize import generate_tokens, COMMENT, NAME, OP, STRING
```

### Comparing `Babel-2.9.0/babel/messages/frontend.py` & `Babel-2.9.1/babel/messages/frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
     babel.messages.frontend
     ~~~~~~~~~~~~~~~~~~~~~~~
 
     Frontends for the message extraction functionality.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 from __future__ import print_function
 
 import logging
 import optparse
 import os
```

### Comparing `Babel-2.9.0/babel/messages/jslexer.py` & `Babel-2.9.1/babel/messages/jslexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
     babel.messages.jslexer
     ~~~~~~~~~~~~~~~~~~~~~~
 
     A simple JavaScript 1.5 lexer which is used for the JavaScript
     extractor.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 from collections import namedtuple
 import re
 from babel._compat import unichr
 
 operators = sorted([
```

### Comparing `Babel-2.9.0/babel/messages/mofile.py` & `Babel-2.9.1/babel/messages/mofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
     babel.messages.mofile
     ~~~~~~~~~~~~~~~~~~~~~
 
     Writing of files in the ``gettext`` MO (machine object) format.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 import array
 import struct
 
 from babel.messages.catalog import Catalog, Message
```

### Comparing `Babel-2.9.0/babel/messages/plurals.py` & `Babel-2.9.1/babel/messages/plurals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
     babel.messages.plurals
     ~~~~~~~~~~~~~~~~~~~~~~
 
     Plural form definitions.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 from babel.core import default_locale, Locale
 from operator import itemgetter
```

### Comparing `Babel-2.9.0/babel/messages/pofile.py` & `Babel-2.9.1/babel/messages/pofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
     babel.messages.pofile
     ~~~~~~~~~~~~~~~~~~~~~
 
     Reading and writing of files in the ``gettext`` PO (portable object)
     format.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 from __future__ import print_function
 import os
 import re
```

### Comparing `Babel-2.9.0/babel/numbers.py` & `Babel-2.9.1/babel/numbers.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     The default locale for the functions in this module is determined by the
     following environment variables, in that order:
 
      * ``LC_NUMERIC``,
      * ``LC_ALL``, and
      * ``LANG``
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 # TODO:
 #  Padding and rounding increments in pattern:
 #  - https://www.unicode.org/reports/tr35/ (Appendix G.6)
 import re
 from datetime import date as date_, datetime as datetime_
```

### Comparing `Babel-2.9.0/babel/plural.py` & `Babel-2.9.1/babel/plural.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
     babel.numbers
     ~~~~~~~~~~~~~
 
     CLDR Plural support.  See UTS #35.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 import re
 
 from babel._compat import decimal
```

### Comparing `Babel-2.9.0/babel/support.py` & `Babel-2.9.1/babel/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     ~~~~~~~~~~~~~
 
     Several classes and functions that help with integrating and using Babel
     in applications.
 
     .. note: the code in this module is not used by Babel itself
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 import gettext
 import locale
 
 from babel.core import Locale
```

### Comparing `Babel-2.9.0/babel/units.py` & `Babel-2.9.1/babel/units.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/babel/util.py` & `Babel-2.9.1/babel/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
     babel.util
     ~~~~~~~~~~
 
     Various utility classes and functions.
 
-    :copyright: (c) 2013-2020 by the Babel Team.
+    :copyright: (c) 2013-2021 by the Babel Team.
     :license: BSD, see LICENSE for more details.
 """
 
 import codecs
 import collections
 from datetime import timedelta, tzinfo
 import os
```

### Comparing `Babel-2.9.0/conftest.py` & `Babel-2.9.1/conftest.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/Makefile` & `Babel-2.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_static/logo.pdf` & `Babel-2.9.1/docs/_static/logo.pdf`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_static/logo.png` & `Babel-2.9.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_static/logo_small.png` & `Babel-2.9.1/docs/_static/logo_small.png`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_templates/sidebar-links.html` & `Babel-2.9.1/docs/_templates/sidebar-links.html`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_themes/LICENSE` & `Babel-2.9.1/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_themes/README` & `Babel-2.9.1/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_themes/babel/layout.html` & `Babel-2.9.1/docs/_themes/babel/layout.html`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_themes/babel/relations.html` & `Babel-2.9.1/docs/_themes/babel/relations.html`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_themes/babel/static/babel.css_t` & `Babel-2.9.1/docs/_themes/babel/static/babel.css_t`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/_themes/babel/static/small_babel.css` & `Babel-2.9.1/docs/_themes/babel/static/small_babel.css`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/api/core.rst` & `Babel-2.9.1/docs/api/core.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/api/dates.rst` & `Babel-2.9.1/docs/api/dates.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/api/messages/extract.rst` & `Babel-2.9.1/docs/api/messages/extract.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/api/numbers.rst` & `Babel-2.9.1/docs/api/numbers.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/cmdline.rst` & `Babel-2.9.1/docs/cmdline.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/conf.py` & `Babel-2.9.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,24 +40,24 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'Babel'
-copyright = u'2020, The Babel Team'
+copyright = u'2021, The Babel Team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '2.9'
 # The full version, including alpha/beta/rc tags.
-release = '2.9.0'
+release = '2.9.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `Babel-2.9.0/docs/dates.rst` & `Babel-2.9.1/docs/dates.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/dev.rst` & `Babel-2.9.1/docs/dev.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/index.rst` & `Babel-2.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/installation.rst` & `Babel-2.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/intro.rst` & `Babel-2.9.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/license.rst` & `Babel-2.9.1/docs/license.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/locale.rst` & `Babel-2.9.1/docs/locale.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/make.bat` & `Babel-2.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/messages.rst` & `Babel-2.9.1/docs/messages.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/numbers.rst` & `Babel-2.9.1/docs/numbers.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/setup.rst` & `Babel-2.9.1/docs/setup.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/docs/support.rst` & `Babel-2.9.1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/scripts/download_import_cldr.py` & `Babel-2.9.1/scripts/download_import_cldr.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,20 +71,21 @@
 def main():
     scripts_path = os.path.dirname(os.path.abspath(__file__))
     repo = os.path.dirname(scripts_path)
     cldr_dl_path = os.path.join(repo, 'cldr')
     cldr_path = os.path.join(repo, 'cldr', os.path.splitext(FILENAME)[0])
     zip_path = os.path.join(cldr_dl_path, FILENAME)
     changed = False
+    show_progress = (False if os.environ.get("BABEL_CLDR_NO_DOWNLOAD_PROGRESS") else sys.stdout.isatty())
 
     while not is_good_file(zip_path):
         log('Downloading \'%s\'', FILENAME)
         if os.path.isfile(zip_path):
             os.remove(zip_path)
-        urlretrieve(URL, zip_path, reporthook)
+        urlretrieve(URL, zip_path, (reporthook if show_progress else None))
         changed = True
         print()
     common_path = os.path.join(cldr_path, 'common')
 
     if changed or not os.path.isdir(common_path):
         if os.path.isdir(common_path):
             log('Deleting old CLDR checkout in \'%s\'', cldr_path)
```

### Comparing `Babel-2.9.0/scripts/dump_data.py` & `Babel-2.9.1/scripts/dump_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/scripts/dump_global.py` & `Babel-2.9.1/scripts/dump_global.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/scripts/generate_authors.py` & `Babel-2.9.1/scripts/generate_authors.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/scripts/import_cldr.py` & `Babel-2.9.1/scripts/import_cldr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
@@ -13,14 +13,15 @@
 # history and logs, available at http://babel.edgewall.org/log/.
 
 import collections
 from optparse import OptionParser
 import os
 import re
 import sys
+import logging
 
 try:
     from xml.etree import cElementTree as ElementTree
 except ImportError:
     from xml.etree import ElementTree
 
 # Make sure we're using Babel source, and not some previously installed version
@@ -58,24 +59,15 @@
     'dateTimeFormats': 'datetime_formats',
     'eraAbbr': 'abbreviated',
     'eraNames': 'wide',
     'eraNarrow': 'narrow',
     'timeFormats': 'time_formats'
 }
 
-
-def log(message, *args):
-    if args:
-        message = message % args
-    sys.stderr.write(message + '\r\n')
-    sys.stderr.flush()
-
-
-def error(message, *args):
-    log('ERROR: %s' % message, *args)
+log = logging.getLogger("import_cldr")
 
 
 def need_conversion(dst_filename, data_dict, source_filename):
     with open(source_filename, 'rb') as f:
         blob = f.read(4096)
         version_match = re.search(b'version number="\\$Revision: (\\d+)', blob)
         if not version_match:  # CLDR 36.0 was shipped without proper revision numbers
@@ -178,18 +170,27 @@
         '-f', '--force', dest='force', action='store_true', default=False,
         help='force import even if destination file seems up to date'
     )
     parser.add_option(
         '-j', '--json', dest='dump_json', action='store_true', default=False,
         help='also export debugging JSON dumps of locale data'
     )
+    parser.add_option(
+        '-q', '--quiet', dest='quiet', action='store_true', default=bool(os.environ.get('BABEL_CLDR_QUIET')),
+        help='quiesce info/warning messages',
+    )
 
     options, args = parser.parse_args()
     if len(args) != 1:
         parser.error('incorrect number of arguments')
+
+    logging.basicConfig(
+        level=(logging.ERROR if options.quiet else logging.INFO),
+    )
+
     return process_data(
         srcdir=args[0],
         destdir=BABEL_PACKAGE_ROOT,
         force=bool(options.force),
         dump_json=bool(options.dump_json)
     )
 
@@ -379,23 +380,26 @@
         elem = tree.find('.//identity/territory')
         if elem is not None:
             territory = elem.attrib['type']
         else:
             territory = '001'  # world
         regions = territory_containment.get(territory, [])
 
-        log('Processing %s (Language = %s; Territory = %s)',
-            filename, language, territory)
+        log.info(
+            'Processing %s (Language = %s; Territory = %s)',
+            filename, language, territory,
+        )
 
         locale_id = '_'.join(filter(None, [
             language,
             territory != '001' and territory or None
         ]))
 
         data['locale_id'] = locale_id
+        data['unsupported_number_systems'] = set()
 
         if locale_id in plural_rules:
             data['plural_form'] = plural_rules[locale_id]
         if locale_id in ordinal_rules:
             data['ordinal_form'] = ordinal_rules[locale_id]
         if locale_id in day_period_rules:
             data["day_period_rules"] = day_period_rules[locale_id]
@@ -428,37 +432,37 @@
         parse_currency_unit_patterns(data, tree)
         parse_currency_names(data, tree)
         parse_unit_patterns(data, tree)
         parse_date_fields(data, tree)
         parse_character_order(data, tree)
         parse_measurement_systems(data, tree)
 
+        unsupported_number_systems_string = ', '.join(sorted(data.pop('unsupported_number_systems')))
+        if unsupported_number_systems_string:
+            log.warning('%s: unsupported number systems were ignored: %s' % (
+                locale_id,
+                unsupported_number_systems_string,
+            ))
+
         write_datafile(data_filename, data, dump_json=dump_json)
 
 
 def _should_skip_number_elem(data, elem):
     """
     Figure out whether the numbering-containing element `elem` is in a currently
     non-supported (i.e. currently non-Latin) numbering system.
 
-    If it is, a warning is raised.
-
-    :param data: The root data element, for formatting the warning.
+    :param data: The root data element, for stashing the warning.
     :param elem: Element with `numberSystem` key
     :return: Boolean
     """
     number_system = elem.get('numberSystem', 'latn')
 
     if number_system != 'latn':
-        log('%s: Unsupported number system "%s" in <%s numberSystem="%s">' % (
-            data['locale_id'],
-            number_system,
-            elem.tag,
-            number_system,
-        ))
+        data['unsupported_number_systems'].add(number_system)
         return True
 
     return False
 
 
 def _should_skip_elem(elem, type=None, dest=None):
     """
@@ -682,15 +686,15 @@
                 if _should_skip_elem(elem, type, date_formats):
                     continue
                 try:
                     date_formats[type] = dates.parse_pattern(
                         text_type(elem.findtext('dateFormat/pattern'))
                     )
                 except ValueError as e:
-                    error(e)
+                    log.error(e)
             elif elem.tag == 'alias':
                 date_formats = Alias(_translate_alias(
                     ['date_formats'], elem.attrib['path'])
                 )
 
 
 def parse_calendar_time_formats(data, calendar):
@@ -702,15 +706,15 @@
                 if _should_skip_elem(elem, type, time_formats):
                     continue
                 try:
                     time_formats[type] = dates.parse_pattern(
                         text_type(elem.findtext('timeFormat/pattern'))
                     )
                 except ValueError as e:
-                    error(e)
+                    log.error(e)
             elif elem.tag == 'alias':
                 time_formats = Alias(_translate_alias(
                     ['time_formats'], elem.attrib['path'])
                 )
 
 
 def parse_calendar_datetime_skeletons(data, calendar):
@@ -721,15 +725,15 @@
             if elem.tag == 'dateTimeFormatLength':
                 type = elem.attrib.get('type')
                 if _should_skip_elem(elem, type, datetime_formats):
                     continue
                 try:
                     datetime_formats[type] = text_type(elem.findtext('dateTimeFormat/pattern'))
                 except ValueError as e:
-                    error(e)
+                    log.error(e)
             elif elem.tag == 'alias':
                 datetime_formats = Alias(_translate_alias(
                     ['datetime_formats'], elem.attrib['path'])
                 )
             elif elem.tag == 'availableFormats':
                 for datetime_skeleton in elem.findall('dateFormatItem'):
                     datetime_skeletons[datetime_skeleton.attrib['id']] = (
```

### Comparing `Babel-2.9.0/scripts/make-release.py` & `Babel-2.9.1/scripts/make-release.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/setup.py` & `Babel-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/conftest.py` & `Babel-2.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/data/project/i18n/de/LC_MESSAGES/messages.mo` & `Babel-2.9.1/tests/messages/data/project/i18n/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/data/project/i18n/de/LC_MESSAGES/messages.po` & `Babel-2.9.1/tests/messages/data/project/i18n/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/bar.po` & `Babel-2.9.1/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/bar.po`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/foo.po` & `Babel-2.9.1/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/foo.po`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/messages.po` & `Babel-2.9.1/tests/messages/data/project/i18n/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/data/project/i18n/messages.pot` & `Babel-2.9.1/tests/messages/data/project/i18n/messages.pot`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/data/project/i18n/messages_non_fuzzy.pot` & `Babel-2.9.1/tests/messages/data/project/i18n/messages_non_fuzzy.pot`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/data/project/i18n/ru_RU/LC_MESSAGES/messages.po` & `Babel-2.9.1/tests/messages/data/project/i18n/ru_RU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/data/setup.py` & `Babel-2.9.1/tests/messages/data/setup.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/test_catalog.py` & `Babel-2.9.1/tests/messages/test_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/messages/test_checkers.py` & `Babel-2.9.1/tests/messages/test_checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/messages/test_extract.py` & `Babel-2.9.1/tests/messages/test_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/messages/test_frontend.py` & `Babel-2.9.1/tests/messages/test_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/messages/test_js_extract.py` & `Babel-2.9.1/tests/messages/test_js_extract.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/test_jslexer.py` & `Babel-2.9.1/tests/messages/test_jslexer.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/test_mofile.py` & `Babel-2.9.1/tests/messages/test_mofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/messages/test_normalized_string.py` & `Babel-2.9.1/tests/messages/test_normalized_string.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/messages/test_plurals.py` & `Babel-2.9.1/tests/messages/test_plurals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/messages/test_pofile.py` & `Babel-2.9.1/tests/messages/test_pofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/test_core.py` & `Babel-2.9.1/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/test_date_intervals.py` & `Babel-2.9.1/tests/test_date_intervals.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/test_dates.py` & `Babel-2.9.1/tests/test_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
 # individuals. For the exact contribution history, see the revision
 # history and logs, available at http://babel.edgewall.org/log/.
 
 import calendar
 from datetime import date, datetime, time, timedelta
 import unittest
 
+import freezegun
 import pytest
 import pytz
 from pytz import timezone
 
 from babel import dates, Locale
 from babel.dates import NO_INHERITANCE_MARKER
 from babel.util import FixedOffsetTimezone
@@ -805,27 +806,18 @@
 
 
 def test_zh_TW_format():
     # Refs GitHub issue #378
     assert dates.format_time(datetime(2016, 4, 8, 12, 34, 56), locale='zh_TW') == u'\u4e0b\u534812:34:56'
 
 
-def test_format_current_moment(monkeypatch):
-    import datetime as datetime_module
+def test_format_current_moment():
     frozen_instant = datetime.utcnow()
-
-    class frozen_datetime(datetime):
-
-        @classmethod
-        def utcnow(cls):
-            return frozen_instant
-
-    # Freeze time! Well, some of it anyway.
-    monkeypatch.setattr(datetime_module, "datetime", frozen_datetime)
-    assert dates.format_datetime(locale="en_US") == dates.format_datetime(frozen_instant, locale="en_US")
+    with freezegun.freeze_time(time_to_freeze=frozen_instant):
+        assert dates.format_datetime(locale="en_US") == dates.format_datetime(frozen_instant, locale="en_US")
 
 
 @pytest.mark.all_locales
 def test_no_inherit_metazone_marker_never_in_output(locale):
     # See: https://github.com/python-babel/babel/issues/428
     tz = pytz.timezone('America/Los_Angeles')
     t = tz.localize(datetime(2016, 1, 6, 7))
```

### Comparing `Babel-2.9.0/tests/test_day_periods.py` & `Babel-2.9.1/tests/test_day_periods.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/test_languages.py` & `Babel-2.9.1/tests/test_languages.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/test_lists.py` & `Babel-2.9.1/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/test_numbers.py` & `Babel-2.9.1/tests/test_numbers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/test_plural.py` & `Babel-2.9.1/tests/test_plural.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/test_smoke.py` & `Babel-2.9.1/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `Babel-2.9.0/tests/test_support.py` & `Babel-2.9.1/tests/test_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

### Comparing `Babel-2.9.0/tests/test_util.py` & `Babel-2.9.1/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2007-2011 Edgewall Software, 2013-2020 the Babel team
+# Copyright (C) 2007-2011 Edgewall Software, 2013-2021 the Babel team
 # All rights reserved.
 #
 # This software is licensed as described in the file LICENSE, which
 # you should have received as part of this distribution. The terms
 # are also available at http://babel.edgewall.org/wiki/License.
 #
 # This software consists of voluntary contributions made by many
```

