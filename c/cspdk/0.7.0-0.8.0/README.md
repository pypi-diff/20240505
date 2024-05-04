# Comparing `tmp/cspdk-0.7.0.tar.gz` & `tmp/cspdk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cspdk-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cspdk-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cspdk-0.7.0.tar` & `cspdk-0.8.0.tar`

### file list

```diff
@@ -1,59 +1,126 @@
--rw-r--r--   0        0        0     1077 2024-03-24 04:20:26.565957 cspdk-0.7.0/LICENSE
--rw-r--r--   0        0        0     1032 2024-03-24 04:20:26.565957 cspdk-0.7.0/README.md
--rw-r--r--   0        0        0     1034 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/__init__.py
--rw-r--r--   0        0        0    31324 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/cells.py
--rw-r--r--   0        0        0      467 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/config.py
--rw-r--r--   0        0        0    90112 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds
--rw-r--r--   0        0        0      192 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/Cell0_Institution_Name.gds
--rw-r--r--   0        0        0    27216 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds
--rw-r--r--   0        0        0      202 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/Cell0_SOI_Full_Institution_Name.gds
--rw-r--r--   0        0        0      202 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/Cell0_SOI_Half_Institution_Name.gds
--rw-r--r--   0        0        0     1156 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/Flip_Chip_Bonding_Example.gds
--rw-r--r--   0        0        0      688 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/Heater.gds
--rw-r--r--   0        0        0    20356 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/Layer_Designations.gds
--rw-r--r--   0        0        0      504 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_2x1_MMI.gds
--rw-r--r--   0        0        0      872 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds
--rw-r--r--   0        0        0     2240 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds
--rw-r--r--   0        0        0     5472 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds
--rw-r--r--   0        0        0      266 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_Waveguide.gds
--rw-r--r--   0        0        0     1108 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      586 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      714 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0      650 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds
--rw-r--r--   0        0        0     5394 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds
--rw-r--r--   0        0        0      204 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_Waveguide.gds
--rw-r--r--   0        0        0      726 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      744 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds
--rw-r--r--   0        0        0      872 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds
--rw-r--r--   0        0        0     2272 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds
--rw-r--r--   0        0        0     4192 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds
--rw-r--r--   0        0        0      266 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_Waveguide.gds
--rw-r--r--   0        0        0     1108 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      586 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      714 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0      650 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds
--rw-r--r--   0        0        0      204 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_STRIP_Waveguide.gds
--rw-r--r--   0        0        0      854 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      394 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1310nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      458 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1310nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0     1626 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1310nm_TE_STRIP_90_Degr.gds
--rw-r--r--   0        0        0     2570 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1310nm_TE_STRIP_Grating.gds
--rw-r--r--   0        0        0      202 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1310nm_TE_STRIP_Wavegui.gds
--rw-r--r--   0        0        0      650 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1550nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      458 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1550nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0     1626 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1550nm_TE_STRIP_90_Degr.gds
--rw-r--r--   0        0        0     1674 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1550nm_TE_STRIP_Grating.gds
--rw-r--r--   0        0        0      202 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/gds/SiN300nm_1550nm_TE_STRIP_Wavegui.gds
--rw-r--r--   0        0        0      213 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/import_pdk.py
--rw-r--r--   0        0        0      928 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/klayout/d25/Cornerstone.lyd25
--rw-r--r--   0        0        0     5133 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/klayout/layers.lyp
--rw-r--r--   0        0        0     5734 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/klayout/tech.lyt
--rw-r--r--   0        0        0     5133 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/klayout/tech/layers.lyp
--rw-r--r--   0        0        0     1309 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/layers.yaml
--rw-r--r--   0        0        0     6509 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/models.py
--rw-r--r--   0        0        0     2906 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/routing.py
--rw-r--r--   0        0        0      555 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/samples/circuit_simulations.py
--rw-r--r--   0        0        0      819 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/samples/component_from_yaml.py
--rw-r--r--   0        0        0     5130 2024-03-24 04:20:26.565957 cspdk-0.7.0/cspdk/tech.py
--rw-r--r--   0        0        0     2272 2024-03-24 04:20:26.569957 cspdk-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 cspdk-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-04 23:51:20.740936 cspdk-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1178 2024-05-04 23:51:20.740936 cspdk-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/__init__.py
+-rw-r--r--   0        0        0      971 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/__init__.py
+-rw-r--r--   0        0        0    40171 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/cells.py
+-rw-r--r--   0        0        0      474 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/config.py
+-rw-r--r--   0        0        0    90112 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds
+-rw-r--r--   0        0        0      192 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Cell0_Institution_Name.gds
+-rw-r--r--   0        0        0    27216 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds
+-rw-r--r--   0        0        0      202 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Cell0_SOI_Full_Institution_Name.gds
+-rw-r--r--   0        0        0      202 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Cell0_SOI_Half_Institution_Name.gds
+-rw-r--r--   0        0        0     1156 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Flip_Chip_Bonding_Example.gds
+-rw-r--r--   0        0        0      688 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Heater.gds
+-rw-r--r--   0        0        0    20356 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Layer_Designations.gds
+-rw-r--r--   0        0        0      504 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_2x1_MMI.gds
+-rw-r--r--   0        0        0      872 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds
+-rw-r--r--   0        0        0     2240 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     5472 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds
+-rw-r--r--   0        0        0      266 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Waveguide.gds
+-rw-r--r--   0        0        0     1108 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      586 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      714 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0      650 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     5394 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds
+-rw-r--r--   0        0        0      204 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Waveguide.gds
+-rw-r--r--   0        0        0      726 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      744 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds
+-rw-r--r--   0        0        0      872 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds
+-rw-r--r--   0        0        0     2272 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     4192 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds
+-rw-r--r--   0        0        0      266 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Waveguide.gds
+-rw-r--r--   0        0        0     1108 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      586 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      714 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0      650 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds
+-rw-r--r--   0        0        0      204 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_Waveguide.gds
+-rw-r--r--   0        0        0      854 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      217 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/import_pdk.py
+-rw-r--r--   0        0        0     1004 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/klayout/d25/Cornerstone.lyd25
+-rw-r--r--   0        0        0      809 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/klayout/d25/Cornerstone_si220.lyd25
+-rw-r--r--   0        0        0     4201 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/klayout/layers.lyp
+-rw-r--r--   0        0        0     5740 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/klayout/tech.lyt
+-rw-r--r--   0        0        0     1051 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/layers.yaml
+-rw-r--r--   0        0        0     5823 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/models.py
+-rw-r--r--   0        0        0      589 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/circuit_simulations_sc.py
+-rw-r--r--   0        0        0      929 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/circuit_simulations_sc_with_routing.py
+-rw-r--r--   0        0        0      825 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/component_from_yaml_sc.py
+-rw-r--r--   0        0        0      416 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/get_route_sc.py
+-rw-r--r--   0        0        0      736 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/mode_solver_r.py
+-rw-r--r--   0        0        0      733 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/mode_solver_s.py
+-rw-r--r--   0        0        0     6987 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/tech.py
+-rw-r--r--   0        0        0      971 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/__init__.py
+-rw-r--r--   0        0        0    19676 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/cells.py
+-rw-r--r--   0        0        0      474 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/config.py
+-rw-r--r--   0        0        0      217 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/import_pdk.py
+-rw-r--r--   0        0        0     1004 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/klayout/d25/Cornerstone.lyd25
+-rw-r--r--   0        0        0      809 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/klayout/d25/Cornerstone_si220.lyd25
+-rw-r--r--   0        0        0     4201 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/klayout/layers.lyp
+-rw-r--r--   0        0        0     5740 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/klayout/tech.lyt
+-rw-r--r--   0        0        0     1051 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/layers.yaml
+-rw-r--r--   0        0        0     5823 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/models.py
+-rw-r--r--   0        0        0      589 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/circuit_simulations_rc500.py
+-rw-r--r--   0        0        0      929 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/circuit_simulations_rc500_with_routing.py
+-rw-r--r--   0        0        0      825 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/component_from_yaml_rc500.py
+-rw-r--r--   0        0        0      416 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/get_route_rc500.py
+-rw-r--r--   0        0        0      734 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/mode_solver_r500.py
+-rw-r--r--   0        0        0     4853 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/tech.py
+-rw-r--r--   0        0        0      977 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/__init__.py
+-rw-r--r--   0        0        0    27490 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/cells.py
+-rw-r--r--   0        0        0      474 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/config.py
+-rw-r--r--   0        0        0    90112 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds
+-rw-r--r--   0        0        0      192 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Cell0_Institution_Name.gds
+-rw-r--r--   0        0        0    27216 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds
+-rw-r--r--   0        0        0      202 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Cell0_SOI_Full_Institution_Name.gds
+-rw-r--r--   0        0        0      202 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Cell0_SOI_Half_Institution_Name.gds
+-rw-r--r--   0        0        0     1156 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Flip_Chip_Bonding_Example.gds
+-rw-r--r--   0        0        0      688 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Heater.gds
+-rw-r--r--   0        0        0    20356 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Layer_Designations.gds
+-rw-r--r--   0        0        0      504 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_2x1_MMI.gds
+-rw-r--r--   0        0        0      872 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds
+-rw-r--r--   0        0        0     2240 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     5472 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds
+-rw-r--r--   0        0        0      266 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Waveguide.gds
+-rw-r--r--   0        0        0     1108 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      586 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      714 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0      650 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     5394 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds
+-rw-r--r--   0        0        0      204 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Waveguide.gds
+-rw-r--r--   0        0        0      726 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      744 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds
+-rw-r--r--   0        0        0      872 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds
+-rw-r--r--   0        0        0     2272 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     4192 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds
+-rw-r--r--   0        0        0      266 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Waveguide.gds
+-rw-r--r--   0        0        0     1108 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      586 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      714 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0      650 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds
+-rw-r--r--   0        0        0      204 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_Waveguide.gds
+-rw-r--r--   0        0        0      854 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      394 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      458 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0     1626 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_90_Degr.gds
+-rw-r--r--   0        0        0     2570 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_Grating.gds
+-rw-r--r--   0        0        0      202 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_Wavegui.gds
+-rw-r--r--   0        0        0      650 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      458 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0     1626 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_90_Degr.gds
+-rw-r--r--   0        0        0     1674 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_Grating.gds
+-rw-r--r--   0        0        0      202 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_Wavegui.gds
+-rw-r--r--   0        0        0      211 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/import_pdk.py
+-rw-r--r--   0        0        0     1004 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/klayout/d25/Cornerstone.lyd25
+-rw-r--r--   0        0        0      852 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/klayout/d25/Cornerstone_sin300.lyd25
+-rw-r--r--   0        0        0     3295 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/klayout/layers.lyp
+-rw-r--r--   0        0        0     5741 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/klayout/tech.lyt
+-rw-r--r--   0        0        0      800 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/layers.yaml
+-rw-r--r--   0        0        0     3711 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/models.py
+-rw-r--r--   0        0        0      590 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/circuit_simulations_nc.py
+-rw-r--r--   0        0        0      930 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/circuit_simulations_nc_with_routing.py
+-rw-r--r--   0        0        0      826 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/component_from_yaml_nc.py
+-rw-r--r--   0        0        0      417 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/get_route_nc.py
+-rw-r--r--   0        0        0      733 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/mode_solver_n.py
+-rw-r--r--   0        0        0     5441 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/tech.py
+-rw-r--r--   0        0        0     2270 2024-05-04 23:51:20.748936 cspdk-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 cspdk-0.8.0/PKG-INFO
```

### Comparing `cspdk-0.7.0/LICENSE` & `cspdk-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/README.md` & `cspdk-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# CornerStone PDK 0.7.0
+# CornerStone PDK 0.8.0
+
+![](https://i.imgur.com/V5Ukc6j.png)
 
 [CornerStone](https://www.cornerstone.sotonfab.co.uk/) Photonics PDK.
 
 ## Installation
 
 ### Installation for users
 
@@ -15,14 +17,16 @@
 ![anaconda prompt](https://i.imgur.com/eKk2bbs.png)
 ```
 pip install cspdk --upgrade
 ```
 
 Then you need to restart Klayout to make sure the new technology installed appears.
 
+You can download the [code](https://github.com/gdsfactory/cspdk/archive/refs/heads/main.zip) and examples.
+
 ### Installation for developers
 
 For developers you need to `git clone` the GitHub repository, fork it, git add, git commit, git push and merge request your changes.
 
 ```
 git clone https://github.com/gdsfactory/cspdk.git
 cd cspdk
```

### Comparing `cspdk-0.7.0/cspdk/__init__.py` & `cspdk-0.8.0/cspdk/si220/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 from gdsfactory.cross_section import get_cross_sections
 from gdsfactory.get_factories import get_cells
 from gdsfactory.pdk import Pdk
 
-from cspdk import cells, config, tech
-from cspdk.cells import _bend, _straight, _taper
-from cspdk.config import PATH
-from cspdk.models import get_models
-from cspdk.routing import get_routing_strategies
-from cspdk.tech import LAYER, LAYER_STACK, LAYER_VIEWS
+from cspdk.si220 import cells, config, tech
+from cspdk.si220.cells import _bend, _straight, _taper
+from cspdk.si220.config import PATH
+from cspdk.si220.models import get_models
+from cspdk.si220.tech import LAYER, LAYER_STACK, LAYER_VIEWS, routing_strategies
 
 _models = get_models()
 _cells = get_cells(cells)
 _cells.update(
     {
         "_straight": _straight,
         "_bend": _bend,
         "_taper": _taper,
     }
 )
 _cross_sections = get_cross_sections(tech)
-_routing_strategies = get_routing_strategies()
 PDK = Pdk(
-    name="cornerstone",
+    name="cornerstone_si220",
     cells=_cells,
     cross_sections=_cross_sections,
     layers=dict(LAYER),
     layer_stack=LAYER_STACK,
     layer_views=LAYER_VIEWS,
     models=_models,
-    routing_strategies=_routing_strategies,
+    routing_strategies=routing_strategies,
 )
 PDK.activate()
 
 __all__ = [
     "LAYER",
     "LAYER_STACK",
     "LAYER_VIEWS",
     "PATH",
     "cells",
     "config",
     "tech",
 ]
-__version__ = "0.7.0"
```

### Comparing `cspdk-0.7.0/cspdk/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds` & `cspdk-0.8.0/cspdk/si220/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds` & `cspdk-0.8.0/cspdk/si220/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/Flip_Chip_Bonding_Example.gds` & `cspdk-0.8.0/cspdk/si220/gds/Flip_Chip_Bonding_Example.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/Heater.gds` & `cspdk-0.8.0/cspdk/si220/gds/Heater.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/Layer_Designations.gds` & `cspdk-0.8.0/cspdk/si220/gds/Layer_Designations.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds` & `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SiN300nm_1310nm_TE_STRIP_90_Degr.gds` & `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_90_Degr.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SiN300nm_1310nm_TE_STRIP_Grating.gds` & `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_Grating.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SiN300nm_1550nm_TE_STRIP_2x1_MMI.gds` & `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SiN300nm_1550nm_TE_STRIP_90_Degr.gds` & `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_90_Degr.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/gds/SiN300nm_1550nm_TE_STRIP_Grating.gds` & `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_Grating.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.7.0/cspdk/klayout/d25/Cornerstone.lyd25` & `cspdk-0.8.0/cspdk/si220/klayout/d25/Cornerstone.lyd25`

 * *Files 18% similar despite different names*

#### Comparing `cspdk-0.7.0/cspdk/klayout/d25/Cornerstone.lyd25` & `cspdk-0.8.0/cspdk/si220/klayout/d25/Cornerstone.lyd25`

```diff
@@ -12,20 +12,22 @@
   <shortcut/>
   <show-in-menu>true</show-in-menu>
   <group-name>d25_scripts</group-name>
   <menu-path>tools_menu.d25.end</menu-path>
   <interpreter>dsl</interpreter>
   <dsl-interpreter-name>d25-dsl-xml</dsl-interpreter-name>
   <text>core = input(3, 0)
+slab = input(5, 0)
 nitride = input(203, 0)
 nitride_etch = input(204, 0)
 heater = input(39, 0)
 metal = input(41, 0)
 
 
 
 z(core, zstart: 0.0, zstop: 0.2, name: 'core: si 3/0', )
+z(slab, zstart: 0.0, zstop: 0.1, name: 'slab: si 5/0', )
 z(nitride, zstart: 0.0, zstop: 0.3, name: 'nitride: sin 203/0', )
 z(nitride_etch, zstart: 0.0, zstop: 0.3, name: 'nitride_etch: sin 204/0', )
 z(heater, zstart: 1.1, zstop: 1.8, name: 'heater: TiN 39/0', )
 z(metal, zstart: 1.8, zstop: 2.5, name: 'metal: Aluminum 41/0', )</text>
 </klayout-macro>
```

### Comparing `cspdk-0.7.0/cspdk/klayout/layers.lyp` & `cspdk-0.8.0/cspdk/si220/klayout/layers.lyp`

 * *Files 13% similar despite different names*

#### Comparing `cspdk-0.7.0/cspdk/klayout/layers.lyp` & `cspdk-0.8.0/cspdk/si220/klayout/layers.lyp`

```diff
@@ -65,48 +65,14 @@
     <marked>false</marked>
     <xfill>false</xfill>
     <animation>0</animation>
     <name>GRA 6/0</name>
     <source>6/0@1</source>
   </properties>
   <properties>
-    <frame-color>#ffa500</frame-color>
-    <fill-color>#ffa500</fill-color>
-    <frame-brightness>0</frame-brightness>
-    <fill-brightness>0</fill-brightness>
-    <dither-pattern>I3</dither-pattern>
-    <line-style/>
-    <valid>true</valid>
-    <visible>true</visible>
-    <transparent>false</transparent>
-    <width/>
-    <marked>false</marked>
-    <xfill>false</xfill>
-    <animation>0</animation>
-    <name>NITRIDE 203/0</name>
-    <source>203/0@1</source>
-  </properties>
-  <properties>
-    <frame-color>#0000ff</frame-color>
-    <fill-color>#0000ff</fill-color>
-    <frame-brightness>0</frame-brightness>
-    <fill-brightness>0</fill-brightness>
-    <dither-pattern>I3</dither-pattern>
-    <line-style/>
-    <valid>true</valid>
-    <visible>true</visible>
-    <transparent>true</transparent>
-    <width>1</width>
-    <marked>false</marked>
-    <xfill>false</xfill>
-    <animation>0</animation>
-    <name>NITRIDE_ETCH 204/0</name>
-    <source>204/0@1</source>
-  </properties>
-  <properties>
     <frame-color>#ebc634</frame-color>
     <fill-color>#ebc634</fill-color>
     <frame-brightness>0</frame-brightness>
     <fill-brightness>0</fill-brightness>
     <dither-pattern>I3</dither-pattern>
     <line-style/>
     <valid>true</valid>
```

### Comparing `cspdk-0.7.0/cspdk/klayout/tech.lyt` & `cspdk-0.8.0/cspdk/si500/klayout/tech.lyt`

 * *Files 1% similar despite different names*

#### Comparing `cspdk-0.7.0/cspdk/klayout/tech.lyt` & `cspdk-0.8.0/cspdk/si500/klayout/tech.lyt`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <technology>
-  <name>Cornerstone</name>
+  <name>Cornerstone_si500</name>
   <description/>
   <group/>
   <dbu>0.001</dbu>
   <default-grids/>
   <base-path/>
   <original-base-path/>
   <layer-properties_file>layers.lyp</layer-properties_file>
@@ -152,11 +152,11 @@
       <lambda>0</lambda>
       <tech/>
       <write-timestamp>true</write-timestamp>
     </mag>
   </writer-options>
   <connectivity>
     <connection>HEATER,HEATER,PAD</connection>
-    <symbols>PAD='41/0'</symbols>
     <symbols>HEATER='39/0'</symbols>
+    <symbols>PAD='41/0'</symbols>
   </connectivity>
 </technology>
```

### Comparing `cspdk-0.7.0/cspdk/klayout/tech/layers.lyp` & `cspdk-0.8.0/cspdk/si500/klayout/layers.lyp`

 * *Files 13% similar despite different names*

#### Comparing `cspdk-0.7.0/cspdk/klayout/tech/layers.lyp` & `cspdk-0.8.0/cspdk/si500/klayout/layers.lyp`

```diff
@@ -65,48 +65,14 @@
     <marked>false</marked>
     <xfill>false</xfill>
     <animation>0</animation>
     <name>GRA 6/0</name>
     <source>6/0@1</source>
   </properties>
   <properties>
-    <frame-color>#ffa500</frame-color>
-    <fill-color>#ffa500</fill-color>
-    <frame-brightness>0</frame-brightness>
-    <fill-brightness>0</fill-brightness>
-    <dither-pattern>I3</dither-pattern>
-    <line-style/>
-    <valid>true</valid>
-    <visible>true</visible>
-    <transparent>false</transparent>
-    <width/>
-    <marked>false</marked>
-    <xfill>false</xfill>
-    <animation>0</animation>
-    <name>NITRIDE 203/0</name>
-    <source>203/0@1</source>
-  </properties>
-  <properties>
-    <frame-color>#0000ff</frame-color>
-    <fill-color>#0000ff</fill-color>
-    <frame-brightness>0</frame-brightness>
-    <fill-brightness>0</fill-brightness>
-    <dither-pattern>I3</dither-pattern>
-    <line-style/>
-    <valid>true</valid>
-    <visible>true</visible>
-    <transparent>true</transparent>
-    <width>1</width>
-    <marked>false</marked>
-    <xfill>false</xfill>
-    <animation>0</animation>
-    <name>NITRIDE_ETCH 204/0</name>
-    <source>204/0@1</source>
-  </properties>
-  <properties>
     <frame-color>#ebc634</frame-color>
     <fill-color>#ebc634</fill-color>
     <frame-brightness>0</frame-brightness>
     <fill-brightness>0</fill-brightness>
     <dither-pattern>I3</dither-pattern>
     <line-style/>
     <valid>true</valid>
```

### Comparing `cspdk-0.7.0/cspdk/layers.yaml` & `cspdk-0.8.0/cspdk/si220/layers.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -21,26 +21,14 @@
   GRA:
     layer: [6, 0]
     layer_in_name: true
     hatch_pattern: coarsely dotted
     transparent: true
     width: 1
     color: "blue"
-  NITRIDE:
-    layer: [203, 0]
-    layer_in_name: true
-    color: "orange"
-    hatch_pattern: coarsely dotted
-  NITRIDE_ETCH:
-    layer: [204, 0]
-    layer_in_name: true
-    hatch_pattern: coarsely dotted
-    transparent: true
-    width: 1
-    color: "blue"
   HEATER:
     layer: [39, 0]
     layer_in_name: true
     color: "#ebc634"
     hatch_pattern: coarsely dotted
   PAD:
     layer: [41, 0]
```

### Comparing `cspdk-0.7.0/cspdk/models.py` & `cspdk-0.8.0/cspdk/si220/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
 import inspect
 from collections.abc import Callable
 from functools import partial
 
-import jax
+import gplugins.sax.models as sm
 import jax.numpy as jnp
 import sax
 from gdsfactory.pdk import get_cross_section_name
 from gdsfactory.typings import CrossSectionSpec
 from gplugins.sax.models import bend as __bend
-from gplugins.sax.models import grating_coupler
 from gplugins.sax.models import straight as __straight
 from numpy.typing import NDArray
 
 nm = 1e-3
 
 FloatArray = NDArray[jnp.floating]
 Float = float | FloatArray
@@ -27,45 +26,80 @@
 def _straight(
     *,
     wl: Float = 1.55,
     length: Float = 10.0,
     loss: Float = 0.0,
     cross_section: CrossSectionSpec = "xs_sc",
 ) -> sax.SDict:
-    if get_cross_section_name(cross_section).endswith("o"):
+    if get_cross_section_name(cross_section).endswith("so"):
         return __straight(
             wl=wl,  # type: ignore
             length=length,  # type: ignore
             loss=loss,  # type: ignore
             wl0=1.31,
-            neff=2.4,
-            ng=4.2,
+            neff=2.52,
+            ng=4.33,
+        )
+    elif get_cross_section_name(cross_section).endswith("nc"):
+        return __straight(
+            wl=wl,  # type: ignore
+            length=length,  # type: ignore
+            loss=loss,  # type: ignore
+            wl0=1.55,
+            neff=1.6,
+            ng=1.94,
+        )
+    elif get_cross_section_name(cross_section).endswith("no"):
+        return __straight(
+            wl=wl,  # type: ignore
+            length=length,  # type: ignore
+            loss=loss,  # type: ignore
+            wl0=1.31,
+            neff=1.63,
+            ng=2.00,
+        )
+    elif get_cross_section_name(cross_section).endswith("rc"):
+        return __straight(
+            wl=wl,  # type: ignore
+            length=length,  # type: ignore
+            loss=loss,  # type: ignore
+            wl0=1.55,
+            neff=2.38,
+            ng=4.30,
+        )
+    elif get_cross_section_name(cross_section).endswith("ro"):
+        return __straight(
+            wl=wl,  # type: ignore
+            length=length,  # type: ignore
+            loss=loss,  # type: ignore
+            wl0=1.31,
+            neff=2.72,
+            ng=3.98,
         )
     else:
         return __straight(
             wl=wl,  # type: ignore
             length=length,  # type: ignore
             loss=loss,  # type: ignore
             wl0=1.55,
-            neff=2.4,
-            ng=4.2,
+            neff=2.38,
+            ng=4.30,
         )
 
 
 straight_sc = partial(_straight, cross_section="xs_sc")
 straight_so = partial(_straight, cross_section="xs_so")
 straight_rc = partial(_straight, cross_section="xs_rc")
 straight_ro = partial(_straight, cross_section="xs_ro")
 straight_nc = partial(_straight, cross_section="xs_nc")
 straight_no = partial(_straight, cross_section="xs_no")
 
 ################
 # Bends
 ################
-
 bend_s = _straight
 
 
 def _bend(wl: Float = 1.5, length: Float = 20.0, loss: Float = 0.03) -> sax.SDict:
     return __bend(
         wl=wl,  # type: ignore
         length=length,  # type: ignore
@@ -89,63 +123,16 @@
 trans_sc_rc10 = partial(_taper_cross_section, length=10.0)
 trans_sc_rc20 = partial(_taper_cross_section, length=20.0)
 trans_sc_rc50 = partial(_taper_cross_section, length=50.0)
 
 ################
 # MMIs
 ################
-
-
-def _mmi_amp(
-    wl: Float = 1.55, wl0: Float = 1.55, fwhm: Float = 0.2, loss_dB: Float = 0.3
-):
-    max_power = 10 ** (-abs(loss_dB) / 10)
-    f = 1 / wl
-    f0 = 1 / wl0
-    f1 = 1 / (wl0 + fwhm / 2)
-    f2 = 1 / (wl0 - fwhm / 2)
-    _fwhm = f2 - f1
-
-    sigma = _fwhm / (2 * jnp.sqrt(2 * jnp.log(2)))
-    power = jnp.exp(-((f - f0) ** 2) / (2 * sigma**2))
-    power = max_power * power / power.max() / 2
-    amp = jnp.sqrt(power)
-    return amp
-
-
-def _mmi1x2(
-    wl: Float = 1.55, wl0: Float = 1.55, fwhm: Float = 0.2, loss_dB: Float = 0.3
-) -> sax.SDict:
-    thru = _mmi_amp(wl=wl, wl0=wl0, fwhm=fwhm, loss_dB=loss_dB)
-    return sax.reciprocal(
-        {
-            ("o1", "o2"): thru,
-            ("o1", "o3"): thru,
-        }
-    )
-
-
-def _mmi2x2(
-    wl: Float = 1.55,
-    wl0: Float = 1.55,
-    fwhm: Float = 0.2,
-    loss_dB: Float = 0.3,
-    shift: Float = 0.005,
-) -> sax.SDict:
-    thru = _mmi_amp(wl=wl, wl0=wl0, fwhm=fwhm, loss_dB=loss_dB)
-    cross = 1j * _mmi_amp(wl=wl, wl0=wl0 + shift, fwhm=fwhm, loss_dB=loss_dB)
-    return sax.reciprocal(
-        {
-            ("o1", "o3"): thru,
-            ("o1", "o4"): cross,
-            ("o2", "o3"): cross,
-            ("o2", "o4"): thru,
-        }
-    )
-
+_mmi1x2 = sm.mmi1x2
+_mmi2x2 = sm.mmi2x2
 
 _mmi1x2_o = partial(_mmi1x2, wl0=1.31)
 _mmi1x2_c = partial(_mmi1x2, wl0=1.55)
 _mmi2x2_o = partial(_mmi2x2, wl0=1.31)
 _mmi2x2_c = partial(_mmi2x2, wl0=1.55)
 
 mmi1x2_rc = _mmi1x2_c
@@ -175,75 +162,42 @@
 coupler_so = _coupler_o
 coupler_ro = _coupler_o
 coupler_no = _coupler_o
 
 ##############################
 # grating couplers Rectangular
 ##############################
-
-
-def _gc_rectangular(
-    *,
-    wl: Float = 1.55,
-    reflection: Float = 0.0,
-    reflection_fiber: Float = 0.0,
-    loss=0.0,
-    wavelength=1.55,
-    bandwidth: Float = 40 * nm,
-) -> sax.SDict:
-    return grating_coupler(
-        wl=wl,  # type: ignore
-        wl0=wavelength,
-        reflection=reflection,  # type: ignore
-        reflection_fiber=reflection_fiber,  # type: ignore
-        loss=loss,
-        bandwidth=bandwidth,  # type: ignore
-    )
-
-
+_gc_rectangular = sm.grating_coupler
 _gcro = partial(_gc_rectangular, loss=6, bandwidth=35 * nm, wavelength=1.31)
 _gcrc = partial(_gc_rectangular, loss=6, bandwidth=35 * nm, wavelength=1.55)
 gc_rectangular_sc = _gcrc
 gc_rectangular_so = _gcro
 gc_rectangular_rc = _gcrc
 gc_rectangular_ro = _gcro
 gc_rectangular_nc = _gcrc
 gc_rectangular_no = _gcro
 
 ##############################
 # grating couplers Elliptical
 ##############################
-
 _gc_elliptical = _gc_rectangular
 _gceo = partial(_gc_elliptical, loss=6, bandwidth=35 * nm, wavelength=1.31)
 _gcec = partial(_gc_elliptical, loss=6, bandwidth=35 * nm, wavelength=1.55)
 gc_elliptical_sc = _gcec
 gc_elliptical_so = _gceo
 gc_elliptical_rc = _gcec
 gc_elliptical_ro = _gceo
 gc_elliptical_nc = _gcec
 gc_elliptical_no = _gceo
 
 
 ################
 # Crossings
 ################
-
-
-@jax.jit
-def _crossing(wl: Float = 1.5) -> sax.SDict:
-    one = jnp.ones_like(jnp.asarray(wl))
-    return sax.reciprocal(
-        {
-            ("o1", "o3"): one,
-            ("o2", "o4"): one,
-        }
-    )
-
-
+_crossing = sm.crossing
 crossing_so = _crossing
 crossing_rc = _crossing
 crossing_sc = _crossing
 
 
 ################
 # Models Dict
```

### Comparing `cspdk-0.7.0/cspdk/samples/component_from_yaml.py` & `cspdk-0.8.0/cspdk/si220/samples/component_from_yaml_sc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 sample_pads = """
 name: pads
-pdk: cspdk
+pdk: cspdk.si220
 
 instances:
     bl:
       component: pad
     tl:
       component: pad
     br:
```

### Comparing `cspdk-0.7.0/cspdk/tech.py` & `cspdk-0.8.0/cspdk/si500/tech.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,53 +5,51 @@
 from typing import cast
 
 import gdsfactory as gf
 from gdsfactory.cross_section import get_cross_sections
 from gdsfactory.technology import LayerLevel, LayerMap, LayerStack, LayerViews
 from gdsfactory.typings import ConnectivitySpec, Layer
 
-from cspdk.config import PATH
+from cspdk.si500.config import PATH
 
 nm = 1e-3
 
 
 class LayerMapCornerstone(LayerMap):
     WG: Layer = (3, 0)
     SLAB: Layer = (5, 0)
     FLOORPLAN: Layer = (99, 0)
     HEATER: Layer = (39, 0)
     GRA: Layer = (6, 0)
     LBL: Layer = (100, 0)
     PAD: Layer = (41, 0)
-    NITRIDE: Layer = (203, 0)
-    NITRIDE_ETCH: Layer = (204, 0)
 
     # labels for gdsfactory
     LABEL_SETTINGS: Layer = (100, 0)
     LABEL_INSTANCE: Layer = (101, 0)
 
 
 LAYER = LayerMapCornerstone()
 
 
 def get_layer_stack(
-    thickness_wg: float = 220 * nm,
-    thickness_nitride: float = 300 * nm,
+    thickness_wg: float = 500 * nm,
+    thickness_slab: float = 200 * nm,
     zmin_heater: float = 1.1,
     thickness_heater: float = 700 * nm,
     zmin_metal: float = 1.1,
     thickness_metal: float = 700 * nm,
 ) -> LayerStack:
     """Returns LayerStack.
 
     based on paper https://www.degruyter.com/document/doi/10.1515/nanoph-2013-0034/html
 
     Args:
         thickness_wg: waveguide thickness in um.
-        thickness_nitride: nitride thickness in um.
+        thickness_slab: slab thickness in um.
         zmin_heater: TiN heater.
         thickness_heater: TiN thickness.
         zmin_metal: metal thickness in um.
         thickness_metal: metal2 thickness.
     """
 
     return LayerStack(
@@ -61,28 +59,19 @@
                 thickness=thickness_wg,
                 zmin=0.0,
                 material="si",
                 info={"mesh_order": 1},
                 sidewall_angle=10,
                 width_to_z=0.5,
             ),
-            nitride=LayerLevel(
-                layer=LAYER.NITRIDE,
-                thickness=thickness_nitride,
+            slab=LayerLevel(
+                layer=LAYER.SLAB,
+                thickness=thickness_slab,
                 zmin=0.0,
-                material="sin",
-                info={"mesh_order": 2},
-                sidewall_angle=10,
-                width_to_z=0.5,
-            ),
-            nitride_etch=LayerLevel(
-                layer=LAYER.NITRIDE_ETCH,
-                thickness=thickness_nitride,
-                zmin=0.0,
-                material="sin",
+                material="si",
                 info={"mesh_order": 1},
                 sidewall_angle=10,
                 width_to_z=0.5,
             ),
             heater=LayerLevel(
                 layer=LAYER.HEATER,
                 thickness=thickness_heater,
@@ -107,85 +96,89 @@
 
 ############################
 # Cross-sections functions
 ############################
 cladding_layers_rib = (LAYER.SLAB,)
 cladding_offsets_rib = (5,)
 
-xf_sc = partial(gf.cross_section.strip, layer=LAYER.WG, width=0.45)
-xf_so = partial(xf_sc, width=0.40)
-
 xf_rc = partial(
     gf.cross_section.strip,
     layer=LAYER.WG,
     width=0.45,
     sections=(gf.Section(width=10.45, layer="SLAB", name="slab", simplify=50 * nm),),
     radius=25,
     radius_min=25,
 )
 xf_ro = partial(xf_rc, width=0.40)
-
-xf_nc = partial(gf.cross_section.strip, layer=LAYER.NITRIDE, width=1.20, radius=25)
-xf_no = partial(gf.cross_section.strip, layer=LAYER.NITRIDE, width=0.95, radius=25)
-
 xf_rc_tip = partial(
     gf.cross_section.strip,
     sections=(gf.Section(width=0.2, layer="SLAB", name="slab"),),
 )
 
 
-xf_sc_heater_metal = partial(
-    gf.cross_section.strip_heater_metal,
-    layer=LAYER.WG,
-    heater_width=2.5,
-    layer_heater=LAYER.HEATER,
-    width=0.45,
-)
-
 metal_routing = partial(
     gf.cross_section.cross_section,
     layer=LAYER.PAD,
     width=10.0,
     port_names=gf.cross_section.port_names_electrical,
     port_types=gf.cross_section.port_types_electrical,
     radius=None,
 )
 heater_metal = partial(metal_routing, width=4, layer=LAYER.HEATER)
 
 ############################
 # Cross-sections
 ############################
-xs_sc = xf_sc()
 xs_rc = xf_rc()
-xs_so = xf_so()
-xs_ro = xf_ro()
-xs_nc = xf_nc()
-xs_no = xf_no()
 xs_rc_tip = xf_rc_tip()
-
-xs_sc_heater_metal = xf_sc_heater_metal()
 xs_metal_routing = metal_routing()
 xs_heater_metal = heater_metal()
-
 cross_sections = get_cross_sections(sys.modules[__name__])
 
+############################
+# Routing functions
+############################
+
+_settings_rc = dict(
+    straight="straight_rc", cross_section=xs_rc, bend="bend_rc", taper="taper_rc"
+)
+
+get_route_rc = partial(gf.routing.get_route, **_settings_rc)
+
+get_route_from_steps_rc = partial(
+    gf.routing.get_route_from_steps,
+    **_settings_rc,
+)
+get_bundle_rc = partial(gf.routing.get_bundle, **_settings_rc)
+
+get_bundle_from_steps_rc = partial(
+    gf.routing.get_bundle_from_steps,
+    **_settings_rc,
+)
+
+routing_strategies = dict(
+    get_route_rc=get_route_rc,
+    get_route_from_steps_rc=get_route_from_steps_rc,
+    get_bundle_rc=get_bundle_rc,
+    get_bundle_from_steps_rc=get_bundle_from_steps_rc,
+)
+
 
 if __name__ == "__main__":
     from gdsfactory.technology.klayout_tech import KLayoutTechnology
 
     LAYER_VIEWS = LayerViews(PATH.lyp_yaml)
-    LAYER_VIEWS.to_lyp(PATH.lyp)
+    # LAYER_VIEWS.to_lyp(PATH.lyp)
 
     connectivity = cast(list[ConnectivitySpec], [("HEATER", "HEATER", "PAD")])
 
     t = KLayoutTechnology(
-        name="Cornerstone",
+        name="Cornerstone_si500",
         layer_map=dict(LAYER),
         layer_views=LAYER_VIEWS,
         layer_stack=LAYER_STACK,
         connectivity=connectivity,
     )
     t.write_tech(tech_dir=PATH.klayout)
 
 if __name__ == "__main__":
     print(xs_rc.sections)
-    print(type(LAYER.NITRIDE), LAYER.NITRIDE)
```

### Comparing `cspdk-0.7.0/pyproject.toml` & `cspdk-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 ]
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent"
 ]
 dependencies = [
-  "gdsfactory==7.22.1",
-  "gplugins[sax]>=0.10.2,<0.11"
+  "gdsfactory==7.25.1",
+  "gplugins[sax]>=0.13,<0.14"
 ]
 description = "CornerStone PDK"
 keywords = ["python"]
 license = {file = "LICENSE"}
 name = "cspdk"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.7.0"
+version = "0.8.0"
 
 [project.optional-dependencies]
 dev = [
   "pre-commit",
   "pytest",
   "pytest-cov",
   "pytest_regressions"
@@ -97,15 +97,15 @@
 src = "cspdk/__init__.py"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.tbump.version]
-current = "0.7.0"
+current = "0.8.0"
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `cspdk-0.7.0/PKG-INFO` & `cspdk-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: cspdk
-Version: 0.7.0
+Version: 0.8.0
 Summary: CornerStone PDK
 Keywords: python
 Author-email: gdsfactory <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Dist: gdsfactory==7.22.1
-Requires-Dist: gplugins[sax]>=0.10.2,<0.11
+Requires-Dist: gdsfactory==7.25.1
+Requires-Dist: gplugins[sax]>=0.13,<0.14
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest_regressions ; extra == "dev"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "docs"
 Requires-Dist: jupyter-book==1.0.0 ; extra == "docs"
 Provides-Extra: dev
 Provides-Extra: docs
 
-# CornerStone PDK 0.7.0
+# CornerStone PDK 0.8.0
+
+![](https://i.imgur.com/V5Ukc6j.png)
 
 [CornerStone](https://www.cornerstone.sotonfab.co.uk/) Photonics PDK.
 
 ## Installation
 
 ### Installation for users
 
@@ -38,14 +40,16 @@
 ![anaconda prompt](https://i.imgur.com/eKk2bbs.png)
 ```
 pip install cspdk --upgrade
 ```
 
 Then you need to restart Klayout to make sure the new technology installed appears.
 
+You can download the [code](https://github.com/gdsfactory/cspdk/archive/refs/heads/main.zip) and examples.
+
 ### Installation for developers
 
 For developers you need to `git clone` the GitHub repository, fork it, git add, git commit, git push and merge request your changes.
 
 ```
 git clone https://github.com/gdsfactory/cspdk.git
 cd cspdk
```

