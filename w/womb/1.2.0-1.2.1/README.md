# Comparing `tmp/womb-1.2.0.tar.gz` & `tmp/womb-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "womb-1.2.0.tar", max compression
+gzip compressed data, was "womb-1.2.1.tar", max compression
```

## Comparing `womb-1.2.0.tar` & `womb-1.2.1.tar`

### file list

```diff
@@ -1,218 +1,218 @@
--rwxr-xr-x   0        0        0      856 2024-05-05 03:54:31.251510 womb-1.2.0/pyproject.toml
--rwxr-xr-x   0        0        0      247 2024-05-05 02:23:10.354766 womb-1.2.0/venues/stages/womb/_____topics/astronomers.S.HTML
--rwxr-xr-x   0        0        0      137 2024-05-05 02:54:27.929149 womb-1.2.0/venues/stages/womb/_____topics/silicon.S.HTML
--rwxr-xr-x   0        0        0      114 2024-04-28 16:30:06.063101 womb-1.2.0/venues/stages/womb/___objectives/HTML_Maps/OSM/OSM.S.HTML
--rwxr-xr-x   0        0        0      303 2024-05-05 03:06:56.130737 womb-1.2.0/venues/stages/womb/___objectives/dates/format.S.HTML
--rwxr-xr-x   0        0        0        0 2024-05-05 02:10:47.342574 womb-1.2.0/venues/stages/womb/___objectives/objectives -- athletics.S.HTML
--rwxr-xr-x   0        0        0      199 2024-05-05 03:02:43.548791 womb-1.2.0/venues/stages/womb/___objectives/objectives -- dates.S.HTML
--rwxr-xr-x   0        0        0      162 2024-05-05 02:00:30.943407 womb-1.2.0/venues/stages/womb/___objectives/objectives -- possibilities.S.HTML
--rwxr-xr-x   0        0        0      217 2024-05-05 02:01:01.339165 womb-1.2.0/venues/stages/womb/___objectives/objectives -- research.S.HTML
--rwxr-xr-x   0        0        0     1374 2024-05-05 03:09:36.721462 womb-1.2.0/venues/stages/womb/___objectives/objectives.S.HTML
--rwxr-xr-x   0        0        0      351 2024-05-04 23:23:46.329622 womb-1.2.0/venues/stages/womb/__dictionary/womb_1
--rwxr-xr-x   0        0        0       36 2024-04-23 18:57:06.249310 womb-1.2.0/venues/stages/womb/__init__.py
--rwxr-xr-x   0        0        0      423 2024-05-04 01:50:08.921331 womb-1.2.0/venues/stages/womb/__licenses/license.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 womb-1.2.0/venues/stages/womb/__licenses/licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      127 2024-05-04 01:46:14.367841 womb-1.2.0/venues/stages/womb/__licenses/licenses/non-business.S.HTML
--rwxr-xr-x   0        0        0     1136 2024-05-04 23:23:46.329622 womb-1.2.0/venues/stages/womb/_essence/__init__.py
--rwxr-xr-x   0        0        0      978 2024-05-04 23:26:03.186713 womb-1.2.0/venues/stages/womb/_essence/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      202 2024-04-27 16:49:31.955662 womb-1.2.0/venues/stages/womb/_essence/essence.S.HTML
--rwxr-xr-x   0        0        0     3073 2024-05-04 01:11:25.546484 womb-1.2.0/venues/stages/womb/_essence/merge/__init__.py
--rwxr-xr-x   0        0        0     1841 2024-05-04 01:12:33.537975 womb-1.2.0/venues/stages/womb/_essence/merge/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      719 2024-05-02 02:39:12.702510 womb-1.2.0/venues/stages/womb/_essence/scan/__init__.py
--rwxr-xr-x   0        0        0      842 2024-05-02 22:19:11.125002 womb-1.2.0/venues/stages/womb/_essence/scan/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      754 2024-05-02 22:19:56.188529 womb-1.2.0/venues/stages/womb/_essence/seek/__init__.py
--rwxr-xr-x   0        0        0      770 2024-05-02 22:20:00.192486 womb-1.2.0/venues/stages/womb/_essence/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      865 2024-05-03 16:03:11.139213 womb-1.2.0/venues/stages/womb/_internal_status/DB/records.json
--rwxr-xr-x   0        0        0       70 2024-05-04 02:42:32.171058 womb-1.2.0/venues/stages/womb/_internal_status/internal_status.S.HTML
--rwxr-xr-x   0        0        0      278 2024-05-04 02:39:35.640735 womb-1.2.0/venues/stages/womb/_internal_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       62 2024-03-23 19:55:58.252641 womb-1.2.0/venues/stages/womb/_internal_status/monitors/status_1.py
--rwxr-xr-x   0        0        0     1967 2024-05-04 23:23:35.065779 womb-1.2.0/venues/stages/womb/_internal_status/status.proc.py
--rwxr-xr-x   0        0        0      592 2024-05-05 03:51:02.160979 womb-1.2.0/venues/stages/womb/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0     1137 2024-05-05 03:55:09.463241 womb-1.2.0/venues/stages/womb/_ops/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 womb-1.2.0/venues/stages/womb/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 womb-1.2.0/venues/stages/womb/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      694 2024-05-02 02:55:52.940134 womb-1.2.0/venues/stages/womb/_ops/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 womb-1.2.0/venues/stages/womb/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1169 2024-05-05 03:55:09.463241 womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      987 2024-05-04 23:28:21.832280 womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0      756 2024-05-04 23:26:03.182713 womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      572 2024-05-04 23:28:21.836280 womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1108 2024-05-04 23:28:21.832280 womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      488 2024-05-05 03:50:32.629186 womb-1.2.0/venues/stages/womb/adventures/_ops/clique.py
--rwxr-xr-x   0        0        0      646 2024-05-04 23:23:45.869633 womb-1.2.0/venues/stages/womb/adventures/_ops/off.py
--rwxr-xr-x   0        0        0      532 2024-05-04 23:23:45.869633 womb-1.2.0/venues/stages/womb/adventures/_ops/on.py
--rwxr-xr-x   0        0        0      500 2024-05-04 23:23:45.869633 womb-1.2.0/venues/stages/womb/adventures/_ops/refresh.py
--rwxr-xr-x   0        0        0     1024 2024-05-04 23:23:45.869633 womb-1.2.0/venues/stages/womb/adventures/_ops/status.py
--rwxr-xr-x   0        0        0     2431 2024-05-04 23:23:45.869633 womb-1.2.0/venues/stages/womb/adventures/alerting/__init__.py
--rwxr-xr-x   0        0        0     1790 2024-05-04 23:28:28.876168 womb-1.2.0/venues/stages/womb/adventures/alerting/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      782 2024-05-02 22:26:24.276333 womb-1.2.0/venues/stages/womb/adventures/alerting/__pycache__/parse_exception.cpython-310.pyc
--rwxr-xr-x   0        0        0      503 2024-05-02 22:26:19.800382 womb-1.2.0/venues/stages/womb/adventures/alerting/parse_exception.py
--rwxr-xr-x   0        0        0       16 2024-05-05 03:16:28.546259 womb-1.2.0/venues/stages/womb/adventures/monetary/.gitignore
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 womb-1.2.0/venues/stages/womb/adventures/monetary/__init__.py
--rwxr-xr-x   0        0        0      150 2024-04-17 03:36:48.047066 womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1687 2024-04-17 03:33:22.113283 womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      680 2024-04-17 03:33:22.113283 womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/connect.cpython-310.pyc
--rwxr-xr-x   0        0        0      857 2024-04-17 03:33:22.113283 womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1904 2024-04-17 03:33:22.113283 womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1610 2024-04-23 19:31:08.342022 womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      564 2024-04-27 23:14:58.002218 womb-1.2.0/venues/stages/womb/adventures/monetary/__saves/saves.S.HTML
--rwxr-xr-x   0        0        0     1434 2024-04-23 20:09:59.888961 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      871 2024-05-04 23:28:21.836280 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1807 2024-05-04 23:26:03.186713 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1650 2024-05-04 23:26:03.186713 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0     1075 2024-05-04 23:23:46.321622 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/_clique.py
--rwxr-xr-x   0        0        0      882 2024-05-04 23:23:46.321622 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/off.py
--rwxr-xr-x   0        0        0     2151 2024-05-04 23:23:46.321622 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/on.py
--rwxr-xr-x   0        0        0     2452 2024-04-29 04:16:14.943069 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     2152 2024-04-17 03:33:22.117283 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     2815 2024-05-04 23:23:46.317623 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/_clique.py
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/dumps/dump.py
--rwxr-xr-x   0        0        0        2 2024-04-17 03:33:22.117283 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/dumps/restore.py
--rwxr-xr-x   0        0        0        2 2024-04-17 03:33:22.117283 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/exports/export.py
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/exports/import.py
--rwxr-xr-x   0        0        0      390 2024-04-23 20:10:51.728325 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/memories.S.HTML
--rwxr-xr-x   0        0        0     1788 2024-05-04 23:23:46.321622 womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/status.py
--rwxr-xr-x   0        0        0      721 2024-05-04 23:23:46.321622 womb-1.2.0/venues/stages/womb/adventures/monetary/databases/mesmerizing/connect.py
--rwxr-xr-x   0        0        0      853 2024-05-03 02:30:32.704613 womb-1.2.0/venues/stages/womb/adventures/monetary/databases/mesmerizing/places/insert.py
--rwxr-xr-x   0        0        0      453 2024-04-23 21:03:13.015179 womb-1.2.0/venues/stages/womb/adventures/monetary/monetary.S.HTML
--rwxr-xr-x   0        0        0      599 2024-05-04 23:26:03.186713 womb-1.2.0/venues/stages/womb/adventures/monetary/moves/URL/__pycache__/retrieve.cpython-310.pyc
--rwxr-xr-x   0        0        0      438 2024-05-04 23:23:46.321622 womb-1.2.0/venues/stages/womb/adventures/monetary/moves/URL/retrieve.py
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 womb-1.2.0/venues/stages/womb/adventures/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1406 2024-05-04 23:28:21.836280 womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1758 2024-05-04 23:28:11.100453 womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1353 2024-05-04 23:28:21.836280 womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1348 2024-05-04 23:28:11.100453 womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0     1461 2024-05-04 23:23:35.069779 womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/off.py
--rwxr-xr-x   0        0        0     1831 2024-05-04 23:23:35.069779 womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/on.py
--rwxr-xr-x   0        0        0     1229 2024-05-04 23:23:35.069779 womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/refresh.py
--rwxr-xr-x   0        0        0     1296 2024-05-04 23:23:35.069779 womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/status.py
--rwxr-xr-x   0        0        0      831 2024-05-04 23:23:35.081779 womb-1.2.0/venues/stages/womb/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py
--rwxr-xr-x   0        0        0      983 2024-05-02 22:27:02.007917 womb-1.2.0/venues/stages/womb/adventures/sanique/_status/__pycache__/API_status_besties__food_USDA__nature_v2__FDC_ID_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      776 2024-05-04 23:23:35.069779 womb-1.2.0/venues/stages/womb/adventures/sanique/clique.py
--rwxr-xr-x   0        0        0     4345 2024-05-04 23:23:35.077779 womb-1.2.0/venues/stages/womb/adventures/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     3706 2024-05-04 23:28:28.644171 womb-1.2.0/venues/stages/womb/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1383 2024-05-02 23:33:35.238000 womb-1.2.0/venues/stages/womb/adventures/sanique/harbor/addresses/__pycache__/besties__food_USDA__nature_v2__FDC_ID.cpython-310.pyc
--rwxr-xr-x   0        0        0     1275 2024-05-02 02:20:59.573374 womb-1.2.0/venues/stages/womb/adventures/sanique/harbor/addresses/__pycache__/besties__supp_NIH__nature_v2__DSLD_ID.cpython-310.pyc
--rwxr-xr-x   0        0        0       69 2024-05-04 15:48:20.602438 womb-1.2.0/venues/stages/womb/adventures/sanique/play/__init__.py
--rwxr-xr-x   0        0        0      270 2024-05-04 23:28:28.876168 womb-1.2.0/venues/stages/womb/adventures/sanique/play/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      524 2024-04-17 03:36:20.947516 womb-1.2.0/venues/stages/womb/adventures/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1278 2024-05-04 23:28:28.876168 womb-1.2.0/venues/stages/womb/adventures/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 womb-1.2.0/venues/stages/womb/adventures/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      525 2024-05-02 22:27:02.619910 womb-1.2.0/venues/stages/womb/adventures/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0     1533 2024-05-04 23:23:35.077779 womb-1.2.0/venues/stages/womb/adventures/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 womb-1.2.0/venues/stages/womb/adventures/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      290 2024-05-04 23:23:35.073779 womb-1.2.0/venues/stages/womb/adventures/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0      442 2024-05-03 00:36:01.688355 womb-1.2.0/venues/stages/womb/adventures/stack.S.HTML
--rwxr-xr-x   0        0        0      127 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/.eslintrc.js
--rwxr-xr-x   0        0        0       94 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/.gitignore
--rwxr-xr-x   0        0        0       26 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/.npmrc
--rwxr-xr-x   0        0        0      939 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/README.md
--rwxr-xr-x   0        0        0       86 2024-05-04 23:23:45.865633 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/VV.S.HTML
--rwxr-xr-x   0        0        0        3 2024-05-05 03:55:40.359023 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/builder/PID.UTF8
--rwxr-xr-x   0        0        0     1130 2024-05-04 23:23:45.209648 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/builder/__init__.py
--rwxr-xr-x   0        0        0     1459 2024-05-04 23:28:11.100453 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/builder/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1312 2024-05-04 23:23:45.205649 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/builder/vv_turbo_build.service
--rwxr-xr-x   0        0        0        3 2024-05-05 03:55:40.359023 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/PID.UTF8
--rwxr-xr-x   0        0        0     1046 2024-05-04 23:23:45.209648 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/__init__.py
--rwxr-xr-x   0        0        0     1414 2024-05-04 23:28:21.832280 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1312 2024-05-04 23:23:45.209648 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/vv_turbo_build.service
--rwxr-xr-x   0        0        0      127 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/.eslintrc.cjs
--rwxr-xr-x   0        0        0      356 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/index.html
--rwxr-xr-x   0        0        0      458 2024-05-02 18:08:51.927033 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/package.json
--rwxr-xr-x   0        0        0     1435 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/public/typescript.svg
--rwxr-xr-x   0        0        0     1497 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/public/vite.svg
--rwxr-xr-x   0        0        0      720 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/src/main.ts
--rwxr-xr-x   0        0        0     1545 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/src/style.css
--rwxr-xr-x   0        0        0       38 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/src/vite-env.d.ts
--rwxr-xr-x   0        0        0       75 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/tsconfig.json
--rwxr-xr-x   0        0        0      127 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/.eslintrc.cjs
--rwxr-xr-x   0        0        0      342 2024-05-04 23:23:45.853633 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/index.html
--rwxr-xr-x   0        0        0      544 2024-05-02 19:05:29.196939 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/package.json
--rwxr-xr-x   0        0        0     1497 2024-04-02 18:55:17.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/public/public/vite.svg
--rwxr-xr-x   0        0        0      493 2024-05-02 04:50:17.108256 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/App.vue
--rwxr-xr-x   0        0        0      560 2024-05-03 23:29:33.769057 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/assets/base.css
--rwxr-xr-x   0        0        0      276 2024-04-03 19:55:44.408084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/assets/logo.svg
--rwxr-xr-x   0        0        0      189 2024-05-04 00:46:31.848499 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/assets/main.css
--rwxr-xr-x   0        0        0      700 2024-04-03 19:55:44.432084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/HelloWorld.vue
--rwxr-xr-x   0        0        0     3282 2024-04-03 19:55:44.432084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/TheWelcome.vue
--rwxr-xr-x   0        0        0     1413 2024-04-03 19:55:44.432084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/WelcomeItem.vue
--rwxr-xr-x   0        0        0      330 2024-04-03 19:55:44.416084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/__tests__/HelloWorld.spec.js
--rwxr-xr-x   0        0        0     1054 2024-04-03 19:55:44.432084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconCommunity.vue
--rwxr-xr-x   0        0        0     1254 2024-04-03 19:55:44.432084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconDocumentation.vue
--rwxr-xr-x   0        0        0     1977 2024-04-03 19:55:44.432084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconEcosystem.vue
--rwxr-xr-x   0        0        0      288 2024-04-03 19:55:44.432084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconSupport.vue
--rwxr-xr-x   0        0        0      913 2024-04-03 19:55:44.432084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconTooling.vue
--rwxr-xr-x   0        0        0        2 2024-05-04 02:05:49.003949 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/coms/insert_place.js
--rwxr-xr-x   0        0        0        3 2024-05-04 02:05:42.124016 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/coms/receive_places.js
--rwxr-xr-x   0        0        0      241 2024-05-04 00:40:25.676015 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/main.js
--rwxr-xr-x   0        0        0     1159 2024-05-04 02:07:59.102688 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/mixes/lap/index.js
--rwxr-xr-x   0        0        0      551 2024-05-03 03:13:46.123009 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/router/index.js
--rwxr-xr-x   0        0        0      220 2024-04-03 19:55:44.432084 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/views/AboutView.vue
--rwxr-xr-x   0        0        0      303 2024-05-05 02:31:23.275825 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/views/HomeView.vue
--rwxr-xr-x   0        0        0      130 2024-05-02 17:54:36.535566 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/views/Roles.vue
--rwxr-xr-x   0        0        0       75 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/tsconfig.json
--rwxr-xr-x   0        0        0      364 2024-05-03 03:11:57.080209 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/vite.config.js
--rwxr-xr-x   0        0        0    92832 2024-05-05 00:06:52.847224 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/bun.lockb
--rwxr-xr-x   0        0        0      621 2024-05-05 00:06:52.847224 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/package.json
--rwxr-xr-x   0        0        0      375 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/config-eslint/index.js
--rwxr-xr-x   0        0        0      306 2024-05-02 18:08:51.927033 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/config-eslint/package.json
--rwxr-xr-x   0        0        0      548 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/config-typescript/base.json
--rwxr-xr-x   0        0        0      150 2024-05-02 18:08:51.927033 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/config-typescript/package.json
--rwxr-xr-x   0        0        0      369 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/config-typescript/vite.json
--rwxr-xr-x   0        0        0       10 2024-05-04 22:55:36.864187 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/geo/chords/parse.js
--rwxr-xr-x   0        0        0      461 2024-05-05 02:03:59.493756 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/geo/geo.S.HTML
--rwxr-xr-x   0        0        0      830 2024-05-02 00:05:13.219543 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/L/map/decor.vue
--rwxr-xr-x   0        0        0       70 2024-05-05 02:37:28.565415 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/OL.S.HTML
--rwxr-xr-x   0        0        0     1170 2024-05-04 22:50:53.678676 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/decor.js
--rwxr-xr-x   0        0        0     3788 2024-05-04 22:54:46.990893 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/decor.vue
--rwxr-xr-x   0        0        0      200 2024-05-02 04:51:24.775695 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/drawings/drawings.S.HTML
--rwxr-xr-x   0        0        0     4849 2024-05-04 22:53:12.224026 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/methods/index.js
--rwxr-xr-x   0        0        0       83 2024-05-05 02:32:49.183270 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/spacetime.S.HTML
--rwxr-xr-x   0        0        0      246 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/ui/.eslintrc.cjs
--rwxr-xr-x   0        0        0       87 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/ui/components/counter.ts
--rwxr-xr-x   0        0        0      138 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/ui/components/header.ts
--rwxr-xr-x   0        0        0      166 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/ui/index.ts
--rwxr-xr-x   0        0        0      418 2024-05-02 18:08:51.927033 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/ui/package.json
--rwxr-xr-x   0        0        0      104 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/ui/tsconfig.json
--rwxr-xr-x   0        0        0      278 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/ui/utils/counter.ts
--rwxr-xr-x   0        0        0      236 2024-05-02 13:56:13.000000 womb-1.2.0/venues/stages/womb/adventures/vv_turbo/turbo.json
--rwxr-xr-x   0        0        0      100 2024-04-28 16:43:11.892387 womb-1.2.0/venues/stages/womb/besties/OSM/OSM.S.HTML
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 womb-1.2.0/venues/stages/womb/license.S.HTML
--rwxr-xr-x   0        0        0      674 2024-05-05 03:10:36.396993 womb-1.2.0/venues/stages/womb/mixes/UTC/UTC.S.HTML
--rwxr-xr-x   0        0        0      921 2024-05-05 02:27:41.237212 womb-1.2.0/venues/stages/womb/mixes/bods/Earth/Earth.S.HTML
--rwxr-xr-x   0        0        0       80 2024-05-05 02:25:02.958143 womb-1.2.0/venues/stages/womb/mixes/bods/Earth/Muna/Muna.S.HTML
--rwxr-xr-x   0        0        0      356 2024-05-05 02:17:33.584331 womb-1.2.0/venues/stages/womb/mixes/bods/bods.S.HTML
--rwxr-xr-x   0        0        0      434 2024-05-01 17:44:05.674829 womb-1.2.0/venues/stages/womb/mixes/docks/__pycache__/address.cpython-310.pyc
--rwxr-xr-x   0        0        0      215 2024-05-01 17:42:03.275911 womb-1.2.0/venues/stages/womb/mixes/docks/address.py
--rwxr-xr-x   0        0        0      561 2024-05-04 23:23:35.069779 womb-1.2.0/venues/stages/womb/mixes/procedure/PID/__init__.py
--rwxr-xr-x   0        0        0     1059 2024-05-04 23:28:11.100453 womb-1.2.0/venues/stages/womb/mixes/procedure/PID/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      854 2024-05-04 23:23:35.069779 womb-1.2.0/venues/stages/womb/mixes/procedure/__init__.py
--rwxr-xr-x   0        0        0     1100 2024-05-04 23:28:10.592461 womb-1.2.0/venues/stages/womb/mixes/procedure/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      153 2024-05-04 15:50:41.850532 womb-1.2.0/venues/stages/womb/mixes/procedure/procedure.S.HTML
--rwxr-xr-x   0        0        0     1446 2024-05-05 01:06:20.098748 womb-1.2.0/venues/stages/womb/mixes/safes/Brainpool_P512_r1/__init__.py
--rwxr-xr-x   0        0        0      378 2024-05-05 03:45:20.087356 womb-1.2.0/venues/stages/womb/readme.md
--rwxr-xr-x   0        0        0       50 2024-05-04 23:28:27.572188 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger
--rwxr-xr-x   0        0        0       21 2024-05-04 23:28:27.572188 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.lock
--rwxr-xr-x   0        0        0     1468 2024-05-05 00:23:28.551604 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.turtle
--rwxr-xr-x   0        0        0    69632 2024-05-05 00:23:28.551604 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.wt
--rwxr-xr-x   0        0        0     4096 2024-05-04 23:28:27.640187 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTigerHS.wt
--rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/_mdb_catalog.wt
--rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-0--8045306896737404471.wt
--rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-2--8045306896737404471.wt
--rwxr-xr-x   0        0        0    24576 2024-05-05 00:03:28.217218 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-4--8045306896737404471.wt
--rwxr-xr-x   0        0        0   348428 2024-05-05 00:23:27.003614 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/diagnostic.data/metrics.2024-05-04T23-28-27Z-00000
--rwxr-xr-x   0        0        0    18933 2024-05-05 00:23:48.011470 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/diagnostic.data/metrics.interim
--rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-1--8045306896737404471.wt
--rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-3--8045306896737404471.wt
--rwxr-xr-x   0        0        0    24576 2024-05-05 00:03:28.217218 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-5--8045306896737404471.wt
--rwxr-xr-x   0        0        0    24576 2024-05-05 00:04:28.244605 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-6--8045306896737404471.wt
--rwxr-xr-x   0        0        0 104857600 2024-05-05 00:23:28.559604 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/journal/WiredTigerLog.0000000001
--rwxr-xr-x   0        0        0 104857600 2024-05-04 23:28:27.644187 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/journal/WiredTigerPreplog.0000000001
--rwxr-xr-x   0        0        0 104857600 2024-05-04 23:28:27.656187 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/journal/WiredTigerPreplog.0000000002
--rwxr-xr-x   0        0        0        4 2024-05-04 23:28:27.668187 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/mongod.lock
--rwxr-xr-x   0        0        0    36864 2024-05-05 00:03:28.217218 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/sizeStorer.wt
--rwxr-xr-x   0        0        0      114 2024-05-04 23:28:27.672187 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/storage.bson
--rwxr-xr-x   0        0        0    28444 2024-05-05 00:23:57.347406 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/logs/the.logs
--rwxr-xr-x   0        0        0        4 2024-05-04 23:28:27.716186 womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/the.process_identity_number
--rwxr-xr-x   0        0        0       48 2024-05-04 23:23:46.329622 womb-1.2.0/venues/stages/womb/womb.S.HTML
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 womb-1.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0      856 2024-05-05 03:58:02.617712 womb-1.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0      247 2024-05-05 02:23:10.354766 womb-1.2.1/venues/stages/womb/_____topics/astronomers.S.HTML
+-rwxr-xr-x   0        0        0      137 2024-05-05 02:54:27.929149 womb-1.2.1/venues/stages/womb/_____topics/silicon.S.HTML
+-rwxr-xr-x   0        0        0      114 2024-04-28 16:30:06.063101 womb-1.2.1/venues/stages/womb/___objectives/HTML_Maps/OSM/OSM.S.HTML
+-rwxr-xr-x   0        0        0      303 2024-05-05 03:06:56.130737 womb-1.2.1/venues/stages/womb/___objectives/dates/format.S.HTML
+-rwxr-xr-x   0        0        0        0 2024-05-05 02:10:47.342574 womb-1.2.1/venues/stages/womb/___objectives/objectives -- athletics.S.HTML
+-rwxr-xr-x   0        0        0      199 2024-05-05 03:02:43.548791 womb-1.2.1/venues/stages/womb/___objectives/objectives -- dates.S.HTML
+-rwxr-xr-x   0        0        0      162 2024-05-05 02:00:30.943407 womb-1.2.1/venues/stages/womb/___objectives/objectives -- possibilities.S.HTML
+-rwxr-xr-x   0        0        0      217 2024-05-05 02:01:01.339165 womb-1.2.1/venues/stages/womb/___objectives/objectives -- research.S.HTML
+-rwxr-xr-x   0        0        0     1374 2024-05-05 03:09:36.721462 womb-1.2.1/venues/stages/womb/___objectives/objectives.S.HTML
+-rwxr-xr-x   0        0        0      351 2024-05-04 23:23:46.329622 womb-1.2.1/venues/stages/womb/__dictionary/womb_1
+-rwxr-xr-x   0        0        0       36 2024-04-23 18:57:06.249310 womb-1.2.1/venues/stages/womb/__init__.py
+-rwxr-xr-x   0        0        0      423 2024-05-04 01:50:08.921331 womb-1.2.1/venues/stages/womb/__licenses/license.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 womb-1.2.1/venues/stages/womb/__licenses/licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      127 2024-05-04 01:46:14.367841 womb-1.2.1/venues/stages/womb/__licenses/licenses/non-business.S.HTML
+-rwxr-xr-x   0        0        0     1136 2024-05-04 23:23:46.329622 womb-1.2.1/venues/stages/womb/_essence/__init__.py
+-rwxr-xr-x   0        0        0      978 2024-05-04 23:26:03.186713 womb-1.2.1/venues/stages/womb/_essence/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      202 2024-04-27 16:49:31.955662 womb-1.2.1/venues/stages/womb/_essence/essence.S.HTML
+-rwxr-xr-x   0        0        0     3073 2024-05-04 01:11:25.546484 womb-1.2.1/venues/stages/womb/_essence/merge/__init__.py
+-rwxr-xr-x   0        0        0     1841 2024-05-04 01:12:33.537975 womb-1.2.1/venues/stages/womb/_essence/merge/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      719 2024-05-02 02:39:12.702510 womb-1.2.1/venues/stages/womb/_essence/scan/__init__.py
+-rwxr-xr-x   0        0        0      842 2024-05-02 22:19:11.125002 womb-1.2.1/venues/stages/womb/_essence/scan/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      754 2024-05-02 22:19:56.188529 womb-1.2.1/venues/stages/womb/_essence/seek/__init__.py
+-rwxr-xr-x   0        0        0      770 2024-05-02 22:20:00.192486 womb-1.2.1/venues/stages/womb/_essence/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      865 2024-05-03 16:03:11.139213 womb-1.2.1/venues/stages/womb/_internal_status/DB/records.json
+-rwxr-xr-x   0        0        0       70 2024-05-04 02:42:32.171058 womb-1.2.1/venues/stages/womb/_internal_status/internal_status.S.HTML
+-rwxr-xr-x   0        0        0      278 2024-05-04 02:39:35.640735 womb-1.2.1/venues/stages/womb/_internal_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       62 2024-03-23 19:55:58.252641 womb-1.2.1/venues/stages/womb/_internal_status/monitors/status_1.py
+-rwxr-xr-x   0        0        0     1967 2024-05-04 23:23:35.065779 womb-1.2.1/venues/stages/womb/_internal_status/status.proc.py
+-rwxr-xr-x   0        0        0      592 2024-05-05 03:51:02.160979 womb-1.2.1/venues/stages/womb/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0     1137 2024-05-05 03:55:09.463241 womb-1.2.1/venues/stages/womb/_ops/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 womb-1.2.1/venues/stages/womb/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 womb-1.2.1/venues/stages/womb/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      694 2024-05-02 02:55:52.940134 womb-1.2.1/venues/stages/womb/_ops/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 womb-1.2.1/venues/stages/womb/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1169 2024-05-05 03:55:09.463241 womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      987 2024-05-04 23:28:21.832280 womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      756 2024-05-04 23:26:03.182713 womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      572 2024-05-04 23:28:21.836280 womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1108 2024-05-04 23:28:21.832280 womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      488 2024-05-05 03:50:32.629186 womb-1.2.1/venues/stages/womb/adventures/_ops/clique.py
+-rwxr-xr-x   0        0        0      646 2024-05-04 23:23:45.869633 womb-1.2.1/venues/stages/womb/adventures/_ops/off.py
+-rwxr-xr-x   0        0        0      532 2024-05-04 23:23:45.869633 womb-1.2.1/venues/stages/womb/adventures/_ops/on.py
+-rwxr-xr-x   0        0        0      500 2024-05-04 23:23:45.869633 womb-1.2.1/venues/stages/womb/adventures/_ops/refresh.py
+-rwxr-xr-x   0        0        0     1024 2024-05-04 23:23:45.869633 womb-1.2.1/venues/stages/womb/adventures/_ops/status.py
+-rwxr-xr-x   0        0        0     2431 2024-05-04 23:23:45.869633 womb-1.2.1/venues/stages/womb/adventures/alerting/__init__.py
+-rwxr-xr-x   0        0        0     1790 2024-05-04 23:28:28.876168 womb-1.2.1/venues/stages/womb/adventures/alerting/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      782 2024-05-02 22:26:24.276333 womb-1.2.1/venues/stages/womb/adventures/alerting/__pycache__/parse_exception.cpython-310.pyc
+-rwxr-xr-x   0        0        0      503 2024-05-02 22:26:19.800382 womb-1.2.1/venues/stages/womb/adventures/alerting/parse_exception.py
+-rwxr-xr-x   0        0        0       16 2024-05-05 03:16:28.546259 womb-1.2.1/venues/stages/womb/adventures/monetary/.gitignore
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 womb-1.2.1/venues/stages/womb/adventures/monetary/__init__.py
+-rwxr-xr-x   0        0        0      150 2024-04-17 03:36:48.047066 womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1687 2024-04-17 03:33:22.113283 womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      680 2024-04-17 03:33:22.113283 womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0      857 2024-04-17 03:33:22.113283 womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1904 2024-04-17 03:33:22.113283 womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1610 2024-04-23 19:31:08.342022 womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      564 2024-04-27 23:14:58.002218 womb-1.2.1/venues/stages/womb/adventures/monetary/__saves/saves.S.HTML
+-rwxr-xr-x   0        0        0     1434 2024-04-23 20:09:59.888961 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      871 2024-05-04 23:28:21.836280 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1807 2024-05-04 23:26:03.186713 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1650 2024-05-04 23:26:03.186713 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1075 2024-05-04 23:23:46.321622 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/_clique.py
+-rwxr-xr-x   0        0        0      882 2024-05-04 23:23:46.321622 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/off.py
+-rwxr-xr-x   0        0        0     2151 2024-05-04 23:23:46.321622 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/on.py
+-rwxr-xr-x   0        0        0     2452 2024-04-29 04:16:14.943069 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2152 2024-04-17 03:33:22.117283 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2815 2024-05-04 23:23:46.317623 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/_clique.py
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/dumps/dump.py
+-rwxr-xr-x   0        0        0        2 2024-04-17 03:33:22.117283 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/dumps/restore.py
+-rwxr-xr-x   0        0        0        2 2024-04-17 03:33:22.117283 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/exports/export.py
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/exports/import.py
+-rwxr-xr-x   0        0        0      390 2024-04-23 20:10:51.728325 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/memories.S.HTML
+-rwxr-xr-x   0        0        0     1788 2024-05-04 23:23:46.321622 womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/status.py
+-rwxr-xr-x   0        0        0      721 2024-05-04 23:23:46.321622 womb-1.2.1/venues/stages/womb/adventures/monetary/databases/mesmerizing/connect.py
+-rwxr-xr-x   0        0        0      853 2024-05-03 02:30:32.704613 womb-1.2.1/venues/stages/womb/adventures/monetary/databases/mesmerizing/places/insert.py
+-rwxr-xr-x   0        0        0      453 2024-04-23 21:03:13.015179 womb-1.2.1/venues/stages/womb/adventures/monetary/monetary.S.HTML
+-rwxr-xr-x   0        0        0      599 2024-05-04 23:26:03.186713 womb-1.2.1/venues/stages/womb/adventures/monetary/moves/URL/__pycache__/retrieve.cpython-310.pyc
+-rwxr-xr-x   0        0        0      438 2024-05-04 23:23:46.321622 womb-1.2.1/venues/stages/womb/adventures/monetary/moves/URL/retrieve.py
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 womb-1.2.1/venues/stages/womb/adventures/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1406 2024-05-04 23:28:21.836280 womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1758 2024-05-04 23:28:11.100453 womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1353 2024-05-04 23:28:21.836280 womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1348 2024-05-04 23:28:11.100453 womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1461 2024-05-04 23:23:35.069779 womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/off.py
+-rwxr-xr-x   0        0        0     1831 2024-05-04 23:23:35.069779 womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/on.py
+-rwxr-xr-x   0        0        0     1229 2024-05-04 23:23:35.069779 womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/refresh.py
+-rwxr-xr-x   0        0        0     1296 2024-05-04 23:23:35.069779 womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/status.py
+-rwxr-xr-x   0        0        0      831 2024-05-04 23:23:35.081779 womb-1.2.1/venues/stages/womb/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py
+-rwxr-xr-x   0        0        0      983 2024-05-02 22:27:02.007917 womb-1.2.1/venues/stages/womb/adventures/sanique/_status/__pycache__/API_status_besties__food_USDA__nature_v2__FDC_ID_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      776 2024-05-04 23:23:35.069779 womb-1.2.1/venues/stages/womb/adventures/sanique/clique.py
+-rwxr-xr-x   0        0        0     4345 2024-05-04 23:23:35.077779 womb-1.2.1/venues/stages/womb/adventures/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     3706 2024-05-04 23:28:28.644171 womb-1.2.1/venues/stages/womb/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1383 2024-05-02 23:33:35.238000 womb-1.2.1/venues/stages/womb/adventures/sanique/harbor/addresses/__pycache__/besties__food_USDA__nature_v2__FDC_ID.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1275 2024-05-02 02:20:59.573374 womb-1.2.1/venues/stages/womb/adventures/sanique/harbor/addresses/__pycache__/besties__supp_NIH__nature_v2__DSLD_ID.cpython-310.pyc
+-rwxr-xr-x   0        0        0       69 2024-05-04 15:48:20.602438 womb-1.2.1/venues/stages/womb/adventures/sanique/play/__init__.py
+-rwxr-xr-x   0        0        0      270 2024-05-04 23:28:28.876168 womb-1.2.1/venues/stages/womb/adventures/sanique/play/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      524 2024-04-17 03:36:20.947516 womb-1.2.1/venues/stages/womb/adventures/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1278 2024-05-04 23:28:28.876168 womb-1.2.1/venues/stages/womb/adventures/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 womb-1.2.1/venues/stages/womb/adventures/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      525 2024-05-02 22:27:02.619910 womb-1.2.1/venues/stages/womb/adventures/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1533 2024-05-04 23:23:35.077779 womb-1.2.1/venues/stages/womb/adventures/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 womb-1.2.1/venues/stages/womb/adventures/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      290 2024-05-04 23:23:35.073779 womb-1.2.1/venues/stages/womb/adventures/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      442 2024-05-03 00:36:01.688355 womb-1.2.1/venues/stages/womb/adventures/stack.S.HTML
+-rwxr-xr-x   0        0        0      127 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/.eslintrc.js
+-rwxr-xr-x   0        0        0       94 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/.gitignore
+-rwxr-xr-x   0        0        0       26 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/.npmrc
+-rwxr-xr-x   0        0        0      939 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/README.md
+-rwxr-xr-x   0        0        0       86 2024-05-04 23:23:45.865633 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/VV.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-05-05 03:55:40.359023 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/builder/PID.UTF8
+-rwxr-xr-x   0        0        0     1130 2024-05-04 23:23:45.209648 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/builder/__init__.py
+-rwxr-xr-x   0        0        0     1459 2024-05-04 23:28:11.100453 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/builder/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1312 2024-05-04 23:23:45.205649 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/builder/vv_turbo_build.service
+-rwxr-xr-x   0        0        0        3 2024-05-05 03:55:40.359023 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/PID.UTF8
+-rwxr-xr-x   0        0        0     1046 2024-05-04 23:23:45.209648 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/__init__.py
+-rwxr-xr-x   0        0        0     1414 2024-05-04 23:28:21.832280 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1312 2024-05-04 23:23:45.209648 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/vv_turbo_build.service
+-rwxr-xr-x   0        0        0      127 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/.eslintrc.cjs
+-rwxr-xr-x   0        0        0      356 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/index.html
+-rwxr-xr-x   0        0        0      458 2024-05-02 18:08:51.927033 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/package.json
+-rwxr-xr-x   0        0        0     1435 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/public/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/public/vite.svg
+-rwxr-xr-x   0        0        0      720 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/src/main.ts
+-rwxr-xr-x   0        0        0     1545 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/src/style.css
+-rwxr-xr-x   0        0        0       38 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/src/vite-env.d.ts
+-rwxr-xr-x   0        0        0       75 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/tsconfig.json
+-rwxr-xr-x   0        0        0      127 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/.eslintrc.cjs
+-rwxr-xr-x   0        0        0      342 2024-05-04 23:23:45.853633 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/index.html
+-rwxr-xr-x   0        0        0      544 2024-05-02 19:05:29.196939 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/package.json
+-rwxr-xr-x   0        0        0     1497 2024-04-02 18:55:17.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/public/public/vite.svg
+-rwxr-xr-x   0        0        0      493 2024-05-02 04:50:17.108256 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/App.vue
+-rwxr-xr-x   0        0        0      560 2024-05-03 23:29:33.769057 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/assets/base.css
+-rwxr-xr-x   0        0        0      276 2024-04-03 19:55:44.408084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/assets/logo.svg
+-rwxr-xr-x   0        0        0      189 2024-05-04 00:46:31.848499 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/assets/main.css
+-rwxr-xr-x   0        0        0      700 2024-04-03 19:55:44.432084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/HelloWorld.vue
+-rwxr-xr-x   0        0        0     3282 2024-04-03 19:55:44.432084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/TheWelcome.vue
+-rwxr-xr-x   0        0        0     1413 2024-04-03 19:55:44.432084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/WelcomeItem.vue
+-rwxr-xr-x   0        0        0      330 2024-04-03 19:55:44.416084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/__tests__/HelloWorld.spec.js
+-rwxr-xr-x   0        0        0     1054 2024-04-03 19:55:44.432084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconCommunity.vue
+-rwxr-xr-x   0        0        0     1254 2024-04-03 19:55:44.432084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconDocumentation.vue
+-rwxr-xr-x   0        0        0     1977 2024-04-03 19:55:44.432084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconEcosystem.vue
+-rwxr-xr-x   0        0        0      288 2024-04-03 19:55:44.432084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconSupport.vue
+-rwxr-xr-x   0        0        0      913 2024-04-03 19:55:44.432084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconTooling.vue
+-rwxr-xr-x   0        0        0        2 2024-05-04 02:05:49.003949 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/coms/insert_place.js
+-rwxr-xr-x   0        0        0        3 2024-05-04 02:05:42.124016 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/coms/receive_places.js
+-rwxr-xr-x   0        0        0      241 2024-05-04 00:40:25.676015 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/main.js
+-rwxr-xr-x   0        0        0     1159 2024-05-04 02:07:59.102688 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/mixes/lap/index.js
+-rwxr-xr-x   0        0        0      551 2024-05-03 03:13:46.123009 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/router/index.js
+-rwxr-xr-x   0        0        0      220 2024-04-03 19:55:44.432084 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/views/AboutView.vue
+-rwxr-xr-x   0        0        0      303 2024-05-05 02:31:23.275825 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/views/HomeView.vue
+-rwxr-xr-x   0        0        0      130 2024-05-02 17:54:36.535566 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/views/Roles.vue
+-rwxr-xr-x   0        0        0       75 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/tsconfig.json
+-rwxr-xr-x   0        0        0      364 2024-05-03 03:11:57.080209 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/vite.config.js
+-rwxr-xr-x   0        0        0    92832 2024-05-05 00:06:52.847224 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/bun.lockb
+-rwxr-xr-x   0        0        0      621 2024-05-05 00:06:52.847224 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/package.json
+-rwxr-xr-x   0        0        0      375 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/config-eslint/index.js
+-rwxr-xr-x   0        0        0      306 2024-05-02 18:08:51.927033 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/config-eslint/package.json
+-rwxr-xr-x   0        0        0      548 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/config-typescript/base.json
+-rwxr-xr-x   0        0        0      150 2024-05-02 18:08:51.927033 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/config-typescript/package.json
+-rwxr-xr-x   0        0        0      369 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/config-typescript/vite.json
+-rwxr-xr-x   0        0        0       10 2024-05-04 22:55:36.864187 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/geo/chords/parse.js
+-rwxr-xr-x   0        0        0      461 2024-05-05 02:03:59.493756 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/geo/geo.S.HTML
+-rwxr-xr-x   0        0        0      830 2024-05-02 00:05:13.219543 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/L/map/decor.vue
+-rwxr-xr-x   0        0        0       70 2024-05-05 02:37:28.565415 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/OL.S.HTML
+-rwxr-xr-x   0        0        0     1170 2024-05-04 22:50:53.678676 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/decor.js
+-rwxr-xr-x   0        0        0     3788 2024-05-04 22:54:46.990893 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/decor.vue
+-rwxr-xr-x   0        0        0      200 2024-05-02 04:51:24.775695 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/drawings/drawings.S.HTML
+-rwxr-xr-x   0        0        0     4849 2024-05-04 22:53:12.224026 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/methods/index.js
+-rwxr-xr-x   0        0        0       83 2024-05-05 02:32:49.183270 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/spacetime.S.HTML
+-rwxr-xr-x   0        0        0      246 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/ui/.eslintrc.cjs
+-rwxr-xr-x   0        0        0       87 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/ui/components/counter.ts
+-rwxr-xr-x   0        0        0      138 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/ui/components/header.ts
+-rwxr-xr-x   0        0        0      166 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/ui/index.ts
+-rwxr-xr-x   0        0        0      418 2024-05-02 18:08:51.927033 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/ui/package.json
+-rwxr-xr-x   0        0        0      104 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/ui/tsconfig.json
+-rwxr-xr-x   0        0        0      278 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/ui/utils/counter.ts
+-rwxr-xr-x   0        0        0      236 2024-05-02 13:56:13.000000 womb-1.2.1/venues/stages/womb/adventures/vv_turbo/turbo.json
+-rwxr-xr-x   0        0        0      100 2024-04-28 16:43:11.892387 womb-1.2.1/venues/stages/womb/besties/OSM/OSM.S.HTML
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 womb-1.2.1/venues/stages/womb/license.S.HTML
+-rwxr-xr-x   0        0        0      674 2024-05-05 03:10:36.396993 womb-1.2.1/venues/stages/womb/mixes/UTC/UTC.S.HTML
+-rwxr-xr-x   0        0        0      921 2024-05-05 02:27:41.237212 womb-1.2.1/venues/stages/womb/mixes/bods/Earth/Earth.S.HTML
+-rwxr-xr-x   0        0        0       80 2024-05-05 02:25:02.958143 womb-1.2.1/venues/stages/womb/mixes/bods/Earth/Muna/Muna.S.HTML
+-rwxr-xr-x   0        0        0      356 2024-05-05 02:17:33.584331 womb-1.2.1/venues/stages/womb/mixes/bods/bods.S.HTML
+-rwxr-xr-x   0        0        0      434 2024-05-01 17:44:05.674829 womb-1.2.1/venues/stages/womb/mixes/docks/__pycache__/address.cpython-310.pyc
+-rwxr-xr-x   0        0        0      215 2024-05-01 17:42:03.275911 womb-1.2.1/venues/stages/womb/mixes/docks/address.py
+-rwxr-xr-x   0        0        0      561 2024-05-04 23:23:35.069779 womb-1.2.1/venues/stages/womb/mixes/procedure/PID/__init__.py
+-rwxr-xr-x   0        0        0     1059 2024-05-04 23:28:11.100453 womb-1.2.1/venues/stages/womb/mixes/procedure/PID/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      854 2024-05-04 23:23:35.069779 womb-1.2.1/venues/stages/womb/mixes/procedure/__init__.py
+-rwxr-xr-x   0        0        0     1100 2024-05-04 23:28:10.592461 womb-1.2.1/venues/stages/womb/mixes/procedure/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      153 2024-05-04 15:50:41.850532 womb-1.2.1/venues/stages/womb/mixes/procedure/procedure.S.HTML
+-rwxr-xr-x   0        0        0     1446 2024-05-05 01:06:20.098748 womb-1.2.1/venues/stages/womb/mixes/safes/Brainpool_P512_r1/__init__.py
+-rwxr-xr-x   0        0        0      375 2024-05-05 03:57:57.673765 womb-1.2.1/venues/stages/womb/readme.md
+-rwxr-xr-x   0        0        0       50 2024-05-04 23:28:27.572188 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger
+-rwxr-xr-x   0        0        0       21 2024-05-04 23:28:27.572188 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.lock
+-rwxr-xr-x   0        0        0     1468 2024-05-05 00:23:28.551604 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.turtle
+-rwxr-xr-x   0        0        0    69632 2024-05-05 00:23:28.551604 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.wt
+-rwxr-xr-x   0        0        0     4096 2024-05-04 23:28:27.640187 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTigerHS.wt
+-rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/_mdb_catalog.wt
+-rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-0--8045306896737404471.wt
+-rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-2--8045306896737404471.wt
+-rwxr-xr-x   0        0        0    24576 2024-05-05 00:03:28.217218 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-4--8045306896737404471.wt
+-rwxr-xr-x   0        0        0   348428 2024-05-05 00:23:27.003614 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/diagnostic.data/metrics.2024-05-04T23-28-27Z-00000
+-rwxr-xr-x   0        0        0    18933 2024-05-05 00:23:48.011470 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/diagnostic.data/metrics.interim
+-rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-1--8045306896737404471.wt
+-rwxr-xr-x   0        0        0    20480 2024-05-04 23:29:27.683269 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-3--8045306896737404471.wt
+-rwxr-xr-x   0        0        0    24576 2024-05-05 00:03:28.217218 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-5--8045306896737404471.wt
+-rwxr-xr-x   0        0        0    24576 2024-05-05 00:04:28.244605 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-6--8045306896737404471.wt
+-rwxr-xr-x   0        0        0 104857600 2024-05-05 00:23:28.559604 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/journal/WiredTigerLog.0000000001
+-rwxr-xr-x   0        0        0 104857600 2024-05-04 23:28:27.644187 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/journal/WiredTigerPreplog.0000000001
+-rwxr-xr-x   0        0        0 104857600 2024-05-04 23:28:27.656187 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/journal/WiredTigerPreplog.0000000002
+-rwxr-xr-x   0        0        0        4 2024-05-04 23:28:27.668187 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/mongod.lock
+-rwxr-xr-x   0        0        0    36864 2024-05-05 00:03:28.217218 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/sizeStorer.wt
+-rwxr-xr-x   0        0        0      114 2024-05-04 23:28:27.672187 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/storage.bson
+-rwxr-xr-x   0        0        0    28444 2024-05-05 00:23:57.347406 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/logs/the.logs
+-rwxr-xr-x   0        0        0        4 2024-05-04 23:28:27.716186 womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/the.process_identity_number
+-rwxr-xr-x   0        0        0       48 2024-05-04 23:23:46.329622 womb-1.2.1/venues/stages/womb/womb.S.HTML
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 womb-1.2.1/PKG-INFO
```

### Comparing `womb-1.2.0/pyproject.toml` & `womb-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "womb"
-version = "1.2.0"
+version = "1.2.1"
 description = "Drawings of the womb and fields."
 authors = []
 readme = "venues/stages/womb/readme.md"
 packages = [
     { include = "womb", from = "venues/stages" },
 ]
 license = "GPL 3.0 Standalone + non-business"
```

### Comparing `womb-1.2.0/venues/stages/womb/___objectives/objectives.S.HTML` & `womb-1.2.1/venues/stages/womb/___objectives/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/__licenses/licenses/gpl-3.0-standalone.html` & `womb-1.2.1/venues/stages/womb/__licenses/licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_essence/__init__.py` & `womb-1.2.1/venues/stages/womb/_essence/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_essence/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/_essence/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_essence/merge/__init__.py` & `womb-1.2.1/venues/stages/womb/_essence/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_essence/merge/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/_essence/merge/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_essence/scan/__init__.py` & `womb-1.2.1/venues/stages/womb/_essence/scan/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_essence/scan/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/_essence/scan/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_essence/seek/__init__.py` & `womb-1.2.1/venues/stages/womb/_essence/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_essence/seek/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/_essence/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_internal_status/DB/records.json` & `womb-1.2.1/venues/stages/womb/_internal_status/DB/records.json`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_internal_status/status.proc.py` & `womb-1.2.1/venues/stages/womb/_internal_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_ops/_clique/__init__.py` & `womb-1.2.1/venues/stages/womb/_ops/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_ops/_clique/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/_ops/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/_ops/_clique/group/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/_ops/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/clique.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/off.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/on.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/refresh.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/_ops/__pycache__/status.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/_ops/off.py` & `womb-1.2.1/venues/stages/womb/adventures/_ops/off.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/_ops/on.py` & `womb-1.2.1/venues/stages/womb/adventures/_ops/on.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/_ops/status.py` & `womb-1.2.1/venues/stages/womb/adventures/_ops/status.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/alerting/__init__.py` & `womb-1.2.1/venues/stages/womb/adventures/alerting/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/alerting/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/alerting/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/alerting/__pycache__/parse_exception.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/alerting/__pycache__/parse_exception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/clique.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/connect.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/connect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/off.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/on.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/__pycache__/status.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/__saves/saves.S.HTML` & `womb-1.2.1/venues/stages/womb/adventures/monetary/__saves/saves.S.HTML`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/_clique.py` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/_clique.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/off.py` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/off.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/on.py` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/on.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/saves/_clique.py` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/saves/_clique.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/_ops/status.py` & `womb-1.2.1/venues/stages/womb/adventures/monetary/_ops/status.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/databases/mesmerizing/connect.py` & `womb-1.2.1/venues/stages/womb/adventures/monetary/databases/mesmerizing/connect.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/databases/mesmerizing/places/insert.py` & `womb-1.2.1/venues/stages/womb/adventures/monetary/databases/mesmerizing/places/insert.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/monetary/moves/URL/__pycache__/retrieve.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/monetary/moves/URL/__pycache__/retrieve.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/off.py` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/off.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/on.py` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/on.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/refresh.py` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/refresh.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_ops/status.py` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_ops/status.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/_status/__pycache__/API_status_besties__food_USDA__nature_v2__FDC_ID_1.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/_status/__pycache__/API_status_besties__food_USDA__nature_v2__FDC_ID_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/clique.py` & `womb-1.2.1/venues/stages/womb/adventures/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/harbor/__init__.py` & `womb-1.2.1/venues/stages/womb/adventures/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/harbor/addresses/__pycache__/besties__food_USDA__nature_v2__FDC_ID.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/harbor/addresses/__pycache__/besties__food_USDA__nature_v2__FDC_ID.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/harbor/addresses/__pycache__/besties__supp_NIH__nature_v2__DSLD_ID.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/harbor/addresses/__pycache__/besties__supp_NIH__nature_v2__DSLD_ID.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/sanique.S.HTML` & `womb-1.2.1/venues/stages/womb/adventures/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/sanique/utilities/generate_inventory_paths.py` & `womb-1.2.1/venues/stages/womb/adventures/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/README.md` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/README.md`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/builder/__init__.py` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/builder/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/builder/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/builder/vv_turbo_build.service` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/builder/vv_turbo_build.service`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/__init__.py` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/vv_turbo_build.service` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/_ops/dev_harbor/vv_turbo_build.service`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/public/typescript.svg` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/public/typescript.svg`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/public/vite.svg` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/public/vite.svg`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/src/main.ts` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/src/main.ts`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/docs/src/style.css` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/docs/src/style.css`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/package.json` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/package.json`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/public/public/vite.svg` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/public/public/vite.svg`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/assets/base.css` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/assets/base.css`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/HelloWorld.vue` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/HelloWorld.vue`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/TheWelcome.vue` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/TheWelcome.vue`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/WelcomeItem.vue` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/WelcomeItem.vue`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconCommunity.vue` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconCommunity.vue`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconDocumentation.vue` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconDocumentation.vue`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconEcosystem.vue` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconEcosystem.vue`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconTooling.vue` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/components/icons/IconTooling.vue`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/mixes/lap/index.js` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/mixes/lap/index.js`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/apps/web/src/router/index.js` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/apps/web/src/router/index.js`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/bun.lockb` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/bun.lockb`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/package.json` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/package.json`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/config-typescript/base.json` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/config-typescript/base.json`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/L/map/decor.vue` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/L/map/decor.vue`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/decor.js` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/decor.js`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/decor.vue` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/decor.vue`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/methods/index.js` & `womb-1.2.1/venues/stages/womb/adventures/vv_turbo/packages/spacetime/OL/map/methods/index.js`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/mixes/UTC/UTC.S.HTML` & `womb-1.2.1/venues/stages/womb/mixes/UTC/UTC.S.HTML`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/mixes/bods/Earth/Earth.S.HTML` & `womb-1.2.1/venues/stages/womb/mixes/bods/Earth/Earth.S.HTML`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/mixes/procedure/PID/__init__.py` & `womb-1.2.1/venues/stages/womb/mixes/procedure/PID/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/mixes/procedure/PID/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/mixes/procedure/PID/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/mixes/procedure/__init__.py` & `womb-1.2.1/venues/stages/womb/mixes/procedure/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/mixes/procedure/__pycache__/__init__.cpython-310.pyc` & `womb-1.2.1/venues/stages/womb/mixes/procedure/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/mixes/safes/Brainpool_P512_r1/__init__.py` & `womb-1.2.1/venues/stages/womb/mixes/safes/Brainpool_P512_r1/__init__.py`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.turtle` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.turtle`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/WiredTiger.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/_mdb_catalog.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/_mdb_catalog.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-0--8045306896737404471.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-0--8045306896737404471.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-2--8045306896737404471.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-2--8045306896737404471.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-4--8045306896737404471.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/collection-4--8045306896737404471.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/diagnostic.data/metrics.2024-05-04T23-28-27Z-00000` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/diagnostic.data/metrics.2024-05-04T23-28-27Z-00000`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/diagnostic.data/metrics.interim` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/diagnostic.data/metrics.interim`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-1--8045306896737404471.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-1--8045306896737404471.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-3--8045306896737404471.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-3--8045306896737404471.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-5--8045306896737404471.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-5--8045306896737404471.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-6--8045306896737404471.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/index-6--8045306896737404471.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/journal/WiredTigerLog.0000000001` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/journal/WiredTigerLog.0000000001`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/sizeStorer.wt` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/_data/sizeStorer.wt`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/venues/stages/womb/wedding/adventures/monetary/__monetary_1/logs/the.logs` & `womb-1.2.1/venues/stages/womb/wedding/adventures/monetary/__monetary_1/logs/the.logs`

 * *Files identical despite different names*

### Comparing `womb-1.2.0/PKG-INFO` & `womb-1.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: womb
-Version: 1.2.0
+Version: 1.2.1
 Summary: Drawings of the womb and fields.
 License: GPL 3.0 Standalone + non-business
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -39,15 +39,15 @@
 
 You are now officially certified to include   
 this mixer in your practice.
 
 ******
 
 
-# womb (artificial)
+# womb (silicon)
 
 ---
 
 ## summary
 
 	
 ---
```

