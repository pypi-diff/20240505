# Comparing `tmp/pyams_app_msc-1.99.2.4.tar.gz` & `tmp/pyams_app_msc-1.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_app_msc-1.99.2.4.tar", last modified: Thu May  2 21:32:26 2024, max compression
+gzip compressed data, was "dist/pyams_app_msc-1.99.3.tar", last modified: Sun May  5 21:12:40 2024, max compression
```

## Comparing `pyams_app_msc-1.99.2.4.tar` & `pyams_app_msc-1.99.3.tar`

### file list

```diff
@@ -1,386 +1,393 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3489 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1950 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/booking.puml
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/classes.puml
--rw-rw-rw-   0 root         (0) root         (0)    16507 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/es-mapping.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/assets/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/clock.png
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/email.png
--rw-rw-rw-   0 root         (0) root         (0)   207972 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-brands-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)   117372 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-brands-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)    68004 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-regular-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)    25452 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-regular-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)   419720 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-solid-900.ttf
--rw-rw-rw-   0 root         (0) root         (0)   156496 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-solid-900.woff2
--rw-rw-rw-   0 root         (0) root         (0)    10832 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-v4compatibility.ttf
--rw-rw-rw-   0 root         (0) root         (0)     4792 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-v4compatibility.woff2
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/form.png
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/layers-2x.png
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/layers.png
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/marker-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/phone.png
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/select2-spinner.gif
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/select2.png
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/select2x2.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/css/dev/
--rw-rw-rw-   0 root         (0) root         (0)   263831 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/dev/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/css/dist/
--rw-rw-rw-   0 root         (0) root         (0)   337917 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/dist/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/css/img/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/clock.png
--rw-rw-rw-   0 root         (0) root         (0)      880 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/download.svg
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/email.png
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/form.png
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/link.svg
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/phone.png
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/print.svg
--rw-rw-rw-   0 root         (0) root         (0)     4315 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/search.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/
--rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/mscapp.js.map
--rw-rw-rw-   0 root         (0) root         (0)     4652 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    10624 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)     6409 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    19333 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
--rw-rw-rw-   0 root         (0) root         (0)    29675 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   209738 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
--rw-rw-rw-   0 root         (0) root         (0)   236865 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   182041 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
--rw-rw-rw-   0 root         (0) root         (0)   230602 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
--rw-rw-rw-   0 root         (0) root         (0)   181575 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
--rw-rw-rw-   0 root         (0) root         (0)   230045 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
--rw-rw-rw-   0 root         (0) root         (0)   174144 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
--rw-rw-rw-   0 root         (0) root         (0)   220941 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
--rw-rw-rw-   0 root         (0) root         (0)    21983 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)    18395 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    18911 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
--rw-rw-rw-   0 root         (0) root         (0)    20127 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   450498 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
--rw-rw-rw-   0 root         (0) root         (0)   569896 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    46418 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
--rw-rw-rw-   0 root         (0) root         (0)    53162 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)   153997 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
--rw-rw-rw-   0 root         (0) root         (0)   189149 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   114212 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
--rw-rw-rw-   0 root         (0) root         (0)   139871 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/116.js
--rw-rw-rw-   0 root         (0) root         (0)     8340 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/137.js
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/178.js
--rw-rw-rw-   0 root         (0) root         (0)    67548 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/23.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/23.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/243.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/243.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16009 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/274.js
--rw-rw-rw-   0 root         (0) root         (0)     3221 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/284.js
--rw-rw-rw-   0 root         (0) root         (0)    69465 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/458.js
--rw-rw-rw-   0 root         (0) root         (0)     3219 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/47.js
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/481.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/481.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/528.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/528.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70026 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/612.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/612.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16008 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/623.js
--rw-rw-rw-   0 root         (0) root         (0)    61493 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/624.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/624.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   105878 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/660.js
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/660.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/671.js
--rw-rw-rw-   0 root         (0) root         (0)    69464 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/686.js
--rw-rw-rw-   0 root         (0) root         (0)    61491 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/698.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/698.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/814.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/814.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/830.js
--rw-rw-rw-   0 root         (0) root         (0)     1859 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/854.js
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/860.js
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/882.js
--rw-rw-rw-   0 root         (0) root         (0)   937336 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)     1770 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/mscapp.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3901 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1268 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/
--rw-rw-rw-   0 root         (0) root         (0)     1027 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1828 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/
--rw-rw-rw-   0 root         (0) root         (0)    12350 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/container.py
--rw-rw-rw-   0 root         (0) root         (0)     9708 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4366 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/reminder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6130 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     3861 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    36201 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15562 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/home.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/reminder.py
--rw-rw-rw-   0 root         (0) root         (0)     8133 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3121 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
--rw-rw-rw-   0 root         (0) root         (0)    38087 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/
--rw-rw-rw-   0 root         (0) root         (0)     1816 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/
--rw-rw-rw-   0 root         (0) root         (0)     2173 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3464 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/
--rw-rw-rw-   0 root         (0) root         (0)     3511 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5672 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    12100 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8006 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16194 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2395 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/
--rw-rw-rw-   0 root         (0) root         (0)     3980 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7142 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/password.py
--rw-rw-rw-   0 root         (0) root         (0)    11384 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      642 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     6337 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12105 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/
--rw-rw-rw-   0 root         (0) root         (0)    20552 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   167336 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)   167000 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
--rw-rw-rw-   0 root         (0) root         (0)   168644 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/
--rw-rw-rw-   0 root         (0) root         (0)    17688 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4826 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/generations/
--rw-rw-rw-   0 root         (0) root         (0)     3771 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8674 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/include.py
--rw-rw-rw-   0 root         (0) root         (0)     2375 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    62537 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
--rw-rw-rw-   0 root         (0) root         (0)   107792 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
--rw-rw-rw-   0 root         (0) root         (0)    76407 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/pyams_app_msc.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5752 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3216 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2257 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/api/
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1862 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/index.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2381 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4485 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3434 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     2050 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/security.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3704 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     6790 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8269 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6079 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/
--rw-rw-rw-   0 root         (0) root         (0)     8410 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/price.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4330 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/audience.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    12262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/audience.py
--rw-rw-rw-   0 root         (0) root         (0)     4080 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2938 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/price.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/room.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/page.py
--rw-rw-rw-   0 root         (0) root         (0)     4262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/price.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/room.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/session.py
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12679 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9666 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/audience.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5472 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3642 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/planning.py
--rw-rw-rw-   0 root         (0) root         (0)     3108 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/presentation.py
--rw-rw-rw-   0 root         (0) root         (0)     9318 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/price.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)     9175 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/room.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     3618 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4526 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/types.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/form.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     5255 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/
--rw-rw-rw-   0 root         (0) root         (0)    11860 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_form.js
--rw-rw-rw-   0 root         (0) root         (0)     5731 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_gis.js
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_i18n.js
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_search.js
--rw-rw-rw-   0 root         (0) root         (0)     9714 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_utils.js
--rw-rw-rw-   0 root         (0) root         (0)     4237 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/mscapp.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_content.scss
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     3047 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_list.scss
--rw-rw-rw-   0 root         (0) root         (0)     4416 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_search.scss
--rw-rw-rw-   0 root         (0) root         (0)     4329 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/msc.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/templates/select-admin-theater.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/img/
--rw-rw-rw-   0 root         (0) root         (0)     4680 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/img/pass-culture.webp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    21353 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/msc.js
--rw-rw-rw-   0 root         (0) root         (0)     8471 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/msc.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3489 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13305 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 21:32:14.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      698 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3973 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     2436 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/booking.puml
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/classes.puml
+-rw-rw-rw-   0 root         (0) root         (0)    16507 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/es-mapping.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/email.png
+-rw-rw-rw-   0 root         (0) root         (0)   207972 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-brands-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   117372 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-brands-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    68004 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-regular-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    25452 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-regular-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   419720 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-solid-900.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   156496 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-solid-900.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    10832 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-v4compatibility.ttf
+-rw-rw-rw-   0 root         (0) root         (0)     4792 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-v4compatibility.woff2
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/form.png
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/layers-2x.png
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/layers.png
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/marker-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/select2-spinner.gif
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/select2.png
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/select2x2.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/css/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/css/dev/
+-rw-rw-rw-   0 root         (0) root         (0)   263831 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/dev/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/css/dist/
+-rw-rw-rw-   0 root         (0) root         (0)   337917 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/dist/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/css/img/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/download.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/email.png
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/form.png
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/link.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/print.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/search.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/js/dev/
+-rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/mscapp.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     4652 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    10624 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)     6409 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    19333 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    29675 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   209738 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   236865 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   182041 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
+-rw-rw-rw-   0 root         (0) root         (0)   230602 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   181575 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
+-rw-rw-rw-   0 root         (0) root         (0)   230045 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   174144 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
+-rw-rw-rw-   0 root         (0) root         (0)   220941 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    21983 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    18395 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    18911 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   450498 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   569896 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    46418 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    53162 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   153997 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   189149 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   114212 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   139871 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/js/dist/
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/116.js
+-rw-rw-rw-   0 root         (0) root         (0)     8340 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/137.js
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/178.js
+-rw-rw-rw-   0 root         (0) root         (0)    67548 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/23.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/23.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/243.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/243.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16009 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/274.js
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/284.js
+-rw-rw-rw-   0 root         (0) root         (0)    69465 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/458.js
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/47.js
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/481.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/481.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/528.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/528.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70026 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/612.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/612.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16008 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/623.js
+-rw-rw-rw-   0 root         (0) root         (0)    61493 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/624.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/624.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   105878 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/660.js
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/660.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/671.js
+-rw-rw-rw-   0 root         (0) root         (0)    69464 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/686.js
+-rw-rw-rw-   0 root         (0) root         (0)    61491 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/698.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/698.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/814.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/814.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/830.js
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/854.js
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/860.js
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/882.js
+-rw-rw-rw-   0 root         (0) root         (0)   937336 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/mscapp.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3899 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5092 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt
+-rw-rw-rw-   0 root         (0) root         (0)      968 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/zmi/container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/
+-rw-rw-rw-   0 root         (0) root         (0)    12350 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     9708 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4366 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/reminder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6130 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    36247 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15562 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/home.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/reminder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8133 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3155 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
+-rw-rw-rw-   0 root         (0) root         (0)    38087 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3464 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/
+-rw-rw-rw-   0 root         (0) root         (0)     3511 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5672 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    12100 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8538 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16194 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7142 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/password.py
+-rw-rw-rw-   0 root         (0) root         (0)    11384 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      642 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     6337 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12105 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/
+-rw-rw-rw-   0 root         (0) root         (0)    20787 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   167336 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   167000 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   168644 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/
+-rw-rw-rw-   0 root         (0) root         (0)    17688 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4826 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8674 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    63416 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
+-rw-rw-rw-   0 root         (0) root         (0)   109342 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
+-rw-rw-rw-   0 root         (0) root         (0)    77437 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/pyams_app_msc.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4485 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     6790 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8974 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6079 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/
+-rw-rw-rw-   0 root         (0) root         (0)     8410 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4330 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/audience.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    12262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)     4080 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     4262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/room.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12486 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9666 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5472 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3642 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/planning.py
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/presentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9318 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9175 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5255 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)    11860 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_form.js
+-rw-rw-rw-   0 root         (0) root         (0)     5731 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_gis.js
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_i18n.js
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_search.js
+-rw-rw-rw-   0 root         (0) root         (0)     9714 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/mscapp.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_content.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_list.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4416 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_search.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/msc.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/templates/select-admin-theater.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/img/
+-rw-rw-rw-   0 root         (0) root         (0)     4680 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/img/pass-culture.webp
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    24830 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/msc.js
+-rw-rw-rw-   0 root         (0) root         (0)    10063 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/msc.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3973 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13539 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:12:29.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      698 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/top_level.txt
```

### Comparing `pyams_app_msc-1.99.2.4/LICENSE` & `pyams_app_msc-1.99.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/PKG-INFO` & `pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_app_msc
-Version: 1.99.2.4
+Name: pyams-app-msc
+Version: 1.99.3
 Summary: PyAMS application for cinema reservation management
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -44,14 +44,24 @@
 PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
 
 
 Changelog
 =========
 
+1.99.3
+------
+ - issue #21: added display of principal phone number
+ - issue #22: updated shared content header viewlet to add button to go back to dashboard
+ - issue #25: updated prompt of activity selection widget
+ - issue #26: added support for vertical synchronization of calendars
+ - issue #27: removed theater week view from calendar
+ - issue #30: added action to set content illustration from medias gallery image
+ - issue #31: updated accompagnists price handler in quotations
+
 1.99.2.4
 --------
  - removed code dependency on OAuth authentication module (bis!)
 
 1.99.2.3
 --------
  - removed code dependency on OAuth authentication module
```

### Comparing `pyams_app_msc-1.99.2.4/docs/HISTORY.rst` & `pyams_app_msc-1.99.3/docs/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+1.99.3
+------
+ - issue #21: added display of principal phone number
+ - issue #22: updated shared content header viewlet to add button to go back to dashboard
+ - issue #25: updated prompt of activity selection widget
+ - issue #26: added support for vertical synchronization of calendars
+ - issue #27: removed theater week view from calendar
+ - issue #30: added action to set content illustration from medias gallery image
+ - issue #31: updated accompagnists price handler in quotations
+
 1.99.2.4
 --------
  - removed code dependency on OAuth authentication module (bis!)
 
 1.99.2.3
 --------
  - removed code dependency on OAuth authentication module
```

### Comparing `pyams_app_msc-1.99.2.4/docs/README.rst` & `pyams_app_msc-1.99.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/docs/classes.puml` & `pyams_app_msc-1.99.3/docs/classes.puml`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/docs/es-mapping.json` & `pyams_app_msc-1.99.3/docs/es-mapping.json`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/clock.png` & `pyams_app_msc-1.99.3/pkg/assets/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/email.png` & `pyams_app_msc-1.99.3/pkg/assets/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/fa-brands-400.ttf` & `pyams_app_msc-1.99.3/pkg/assets/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/fa-brands-400.woff2` & `pyams_app_msc-1.99.3/pkg/assets/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/fa-regular-400.ttf` & `pyams_app_msc-1.99.3/pkg/assets/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/fa-regular-400.woff2` & `pyams_app_msc-1.99.3/pkg/assets/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/fa-solid-900.ttf` & `pyams_app_msc-1.99.3/pkg/assets/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/fa-solid-900.woff2` & `pyams_app_msc-1.99.3/pkg/assets/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/fa-v4compatibility.ttf` & `pyams_app_msc-1.99.3/pkg/assets/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/fa-v4compatibility.woff2` & `pyams_app_msc-1.99.3/pkg/assets/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/form.png` & `pyams_app_msc-1.99.3/pkg/assets/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/layers-2x.png` & `pyams_app_msc-1.99.3/pkg/assets/layers-2x.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/layers.png` & `pyams_app_msc-1.99.3/pkg/assets/layers.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/list-item.png` & `pyams_app_msc-1.99.3/pkg/assets/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/map.png` & `pyams_app_msc-1.99.3/pkg/assets/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/marker-icon.png` & `pyams_app_msc-1.99.3/pkg/assets/marker-icon.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/mobile-menu.png` & `pyams_app_msc-1.99.3/pkg/assets/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/phone.png` & `pyams_app_msc-1.99.3/pkg/assets/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/select2-spinner.gif` & `pyams_app_msc-1.99.3/pkg/assets/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/select2.png` & `pyams_app_msc-1.99.3/pkg/assets/select2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/select2x2.png` & `pyams_app_msc-1.99.3/pkg/assets/select2x2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/assets/social-icons.png` & `pyams_app_msc-1.99.3/pkg/assets/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/dev/msc.css` & `pyams_app_msc-1.99.3/pkg/css/dev/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/dist/msc.css` & `pyams_app_msc-1.99.3/pkg/css/dist/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/clock.png` & `pyams_app_msc-1.99.3/pkg/css/img/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/download.svg` & `pyams_app_msc-1.99.3/pkg/css/img/download.svg`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/email.png` & `pyams_app_msc-1.99.3/pkg/css/img/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/form.png` & `pyams_app_msc-1.99.3/pkg/css/img/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/list-item.png` & `pyams_app_msc-1.99.3/pkg/css/img/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/map.png` & `pyams_app_msc-1.99.3/pkg/css/img/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/mobile-menu.png` & `pyams_app_msc-1.99.3/pkg/css/img/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/phone.png` & `pyams_app_msc-1.99.3/pkg/css/img/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/search.png` & `pyams_app_msc-1.99.3/pkg/css/img/search.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/css/img/social-icons.png` & `pyams_app_msc-1.99.3/pkg/css/img/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/mscapp.js` & `pyams_app_msc-1.99.3/pkg/js/dev/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/mscapp.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/mscapp.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js` & `pyams_app_msc-1.99.3/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.3/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js` & `pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js` & `pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map` & `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/116.js` & `pyams_app_msc-1.99.3/pkg/js/dist/116.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/137.js` & `pyams_app_msc-1.99.3/pkg/js/dist/137.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/23.js` & `pyams_app_msc-1.99.3/pkg/js/dist/23.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/23.js.LICENSE.txt` & `pyams_app_msc-1.99.3/pkg/js/dist/23.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/243.js` & `pyams_app_msc-1.99.3/pkg/js/dist/243.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/274.js` & `pyams_app_msc-1.99.3/pkg/js/dist/274.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/284.js` & `pyams_app_msc-1.99.3/pkg/js/dist/284.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/458.js` & `pyams_app_msc-1.99.3/pkg/js/dist/458.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/47.js` & `pyams_app_msc-1.99.3/pkg/js/dist/47.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/481.js` & `pyams_app_msc-1.99.3/pkg/js/dist/481.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/528.js` & `pyams_app_msc-1.99.3/pkg/js/dist/528.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/528.js.LICENSE.txt` & `pyams_app_msc-1.99.3/pkg/js/dist/528.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/612.js` & `pyams_app_msc-1.99.3/pkg/js/dist/612.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/612.js.LICENSE.txt` & `pyams_app_msc-1.99.3/pkg/js/dist/612.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/623.js` & `pyams_app_msc-1.99.3/pkg/js/dist/623.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/624.js` & `pyams_app_msc-1.99.3/pkg/js/dist/624.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/660.js` & `pyams_app_msc-1.99.3/pkg/js/dist/660.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/686.js` & `pyams_app_msc-1.99.3/pkg/js/dist/686.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/698.js` & `pyams_app_msc-1.99.3/pkg/js/dist/698.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/814.js` & `pyams_app_msc-1.99.3/pkg/js/dist/814.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/814.js.LICENSE.txt` & `pyams_app_msc-1.99.3/pkg/js/dist/814.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/830.js` & `pyams_app_msc-1.99.3/pkg/js/dist/830.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/854.js` & `pyams_app_msc-1.99.3/pkg/js/dist/854.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/860.js` & `pyams_app_msc-1.99.3/pkg/js/dist/860.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/882.js` & `pyams_app_msc-1.99.3/pkg/js/dist/882.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/mscapp.js` & `pyams_app_msc-1.99.3/pkg/js/dist/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/pkg/js/dist/mscapp.js.LICENSE.txt` & `pyams_app_msc-1.99.3/pkg/js/dist/mscapp.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/setup.py` & `pyams_app_msc-1.99.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.2.4'
+version = '1.99.3'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 data_dir = 'pkg'
 data_files = [(d, [os.path.join(d, f) for f in files])
               for d, folders, files in os.walk(data_dir)]
 
 tests_require = [
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/schema.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/container.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/doctests/README.rst` & `pyams_app_msc-1.99.3/src/pyams_app_msc/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/container.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/container.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/reminder.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/task.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,16 @@
     """Booking label getter"""
     recipient = get_principal(request, context.recipient)
     result = recipient.title
     profile_info = IUserProfile(recipient, None)
     if (profile_info is None) or not profile_info.establishment:
         return result
     return (f'{result} ({profile_info.get_structure_type()} - '
-            f'{profile_info.establishment}, {profile_info.establishment_address.city})')
+            f'{profile_info.establishment}, {profile_info.establishment_address.city} - '
+            f'{profile_info.phone_number})')
 
 
 @viewlet_config(name='add-booking.action',
                 context=IBookingTarget, layer=IAdminLayer,
                 view=IBookingContainerTable,
                 manager=IToolbarViewletManager, weigth=20,
                 permission=MANAGE_BOOKING_PERMISSION)
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/dashboard.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/home.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/home.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/reminder.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/search.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/task.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 								 (has_bookings, bookings) tales:boolean_iter(items)">
 					<tal:loop repeat="booking bookings">
 						<div class="card-title"
 							 tal:define="(principal, profile) booking.get_recipient()">
 							<a class="text-dark"
 							   href="${tales:absolute_url(booking, 'properties.html')}" data-toggle="modal">
 								${profile.establishment}
-								(${profile.get_structure_type()}, ${profile.establishment_address.city}) - <strong>${principal.title}</strong>
+								(${profile.get_structure_type()}, ${profile.establishment_address.city}) - <strong>${principal.title}</strong> (${profile.phone_number or '--'})
 							</a>
 							<tal:if condition="booking.cultural_pass">
 								<img title="Cultural pass" alt="" i18n:attributes="title"
 									 class="position-absolute mx-3 mt-n2 hint"
 									 src="/--static--/msc/img/pass-culture.webp"
 									 width="32" height="32" />
 							</tal:if><br />
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/workflow.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/skin/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/session.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,30 +117,31 @@
                 'url': absolute_url(context, self.request, 'get-planning-events.json'),
                 'extraParams': {
                     'room': room.__name__
                 }
             }],
             'height': '100%',
             'initialDate': next_wednesday.date().isoformat(),
-            'views': {
-                'cinemaGridWeek': {
-                    'type': 'timeGrid',
-                    'firstDay': 4,
-                    'duration': {
-                        'days': 7
-                    },
-                    'buttonText': translate(_('Theater week'))
-                }
-            },
+            # 'views': {
+            #     'cinemaGridWeek': {
+            #         'type': 'timeGrid',
+            #         'duration': {
+            #             'days': 7
+            #         },
+            #         'firstDay': 3,
+            #         'buttonText': translate(_('Theater week'))
+            #     }
+            # },
             'dateClick': 'MyAMS.msc.calendar.addEvent',
             'initialView': 'timeGridWeek',
             'headerToolbar': {
                 'center': 'today',
-                'right': 'prev,next dayGridMonth,timeGridWeek,cinemaGridWeek,timeGridDay,listMonth'
-            },
+                'right': 'prev,next dayGridMonth,timeGridWeek,timeGridDay,listMonth'
+                # 'right': 'prev,next dayGridMonth,timeGridWeek,cinemaGridWeek,timeGridDay,listMonth'
+        },
             'allDaySlot': False,
             'slotDuration': f'00:{settings.calendar_slot_duration:#02}:00',
             'slotMinTime': room.start_time.isoformat(),
             'slotMaxTime': room.end_time.isoformat(),
             'buttonText': {
                 'today': translate(_("Today")),
                 'month': translate(_("Month")),
@@ -189,24 +190,37 @@
 @viewlet_config(name='planning.transpose',
                 layer=IAdminLayer, view=PlanningView,
                 manager=ISecondaryActionsViewletManager, weight=10)
 class PlanningTransposeAction(JsContextAction):
     """Planning transpose action"""
 
     icon_class = 'fas fa-recycle'
-    hint = _("Transpose")
+    hint = _("Transpose calendars")
     hint_placement = 'bottom'
 
     href = 'MyAMS.msc.calendar.transpose'
 
 
 @viewlet_config(name='planning.synchronize',
                 layer=IAdminLayer, view=PlanningView,
                 manager=ISecondaryActionsViewletManager, weight=20)
 class PlanningSynchronizeAction(JsContextAction):
     """Planning synchronize action"""
 
     icon_class = 'fas fa-sync-alt'
-    hint = _("Synchronize")
+    hint = _("Synchronize calendars views")
     hint_placement = 'bottom'
 
     href = 'MyAMS.msc.calendar.synchronize'
+
+
+@viewlet_config(name='planning.scroll',
+                layer=IAdminLayer, view=PlanningView,
+                manager=ISecondaryActionsViewletManager, weight=30)
+class PlanningScrollAction(JsContextAction):
+    """Planning scrolling action"""
+
+    icon_class = 'fas fa-arrows-alt-v'
+    hint = _("Synchronize calendars scrolling")
+    hint_placement = 'bottom'
+
+    href = 'MyAMS.msc.calendar.scroll'
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/session.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/password.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/password.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/register.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/register.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/task.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/widget.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,26 +263,30 @@
                     nb_participants = int(nb_participants or 0)
                 nb_accompanists = preview_args.get('nb_accompanists')
                 if nb_accompanists is None:
                     nb_accompanists = booking.nb_accompanists
                 else:
                     nb_accompanists = int(nb_accompanists or 0)
                 if price is not None:
-                    ratio = preview_args.get('ratio')
-                    if ratio is None:
-                        ratio = booking.accompanying_ratio
+                    if price.accompanying_price == 0.:
+                        free_accompanists = nb_accompanists
+                        paid_accompanists = 0
                     else:
-                        ratio = float(ratio or 0)
-                    if ratio:
-                        max_accompanists = math.ceil(nb_participants / ratio)
-                        free_accompanists = min(max_accompanists, nb_accompanists)
-                        paid_accompanists = nb_accompanists - free_accompanists
-                    else:
-                        free_accompanists = 0
-                        paid_accompanists = nb_accompanists
+                        ratio = preview_args.get('ratio')
+                        if ratio is None:
+                            ratio = booking.accompanying_ratio
+                        else:
+                            ratio = float(ratio or 0)
+                        if ratio:
+                            max_accompanists = math.ceil(nb_participants / ratio)
+                            free_accompanists = min(max_accompanists, nb_accompanists)
+                            paid_accompanists = nb_accompanists - free_accompanists
+                        else:
+                            free_accompanists = 0
+                            paid_accompanists = nb_accompanists
                     participants_amount = price.participant_price * nb_participants
                     accompanying_amount = price.accompanying_price * paid_accompanists
                 else:
                     free_accompanists = nb_accompanists
                     paid_accompanists = 0
                     participants_amount = 0.
                     accompanying_amount = 0.
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/schema.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/lookup.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/lookup.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/generations/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/include.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/include.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo` & `pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -350,14 +350,17 @@
 "Impossible d'activer ce compte avec les paramètres de connexion indiqués !"
 
 msgid "Can't change password with provided arguments!"
 msgstr ""
 "Impossible de modifier le mot de passe avec les paramètres de connexion "
 "indiqués !"
 
+msgid "Can't find illustration target!"
+msgstr "Impossible de trouver la cible de l'illustration !"
+
 msgid "Cancel"
 msgstr "Annuler"
 
 msgid "Cancel booking"
 msgstr "Annuler la réservation"
 
 msgid "Cancel max delay"
@@ -508,14 +511,17 @@
 
 msgid "Contact phone number"
 msgstr "Téléphone"
 
 msgid "Contacts"
 msgstr "Contacts"
 
+msgid "Content illustration has been updated successfully."
+msgstr "L'illustration du contenu a été modifiée avec succès."
+
 msgid "Contributors"
 msgstr "Contributeurs"
 
 msgid ""
 "Contributors can add activities to theater catalog, but can't publish them"
 msgstr ""
 "Les contributeurs peuvent ajouter des activités au catalogue, mais ne "
@@ -723,20 +729,26 @@
 
 msgid "Full name"
 msgstr "Nom complet"
 
 msgid "Full theater address"
 msgstr "Adresse complète du cinéma"
 
+msgid "Gallery medias"
+msgstr "Galerie de médias"
+
 msgid "Get confirmation message?"
 msgstr "Recevoir un message de confirmation"
 
 msgid "Get videos for selected language only"
 msgstr "Seulement pour la langue sélectionnée"
 
+msgid "Given element name doesn't exist!"
+msgstr "Le nom indiqué n'existe pas !"
+
 msgid "Go to login page"
 msgstr "Aller à l'écran de connexion"
 
 msgid "Groups count"
 msgstr "Nombre de groupes"
 
 msgid "Header"
@@ -1157,14 +1169,20 @@
 
 msgid "New theater properties"
 msgstr "Propriétés du nouveau cinéma"
 
 msgid "Next page"
 msgstr "Page suivante"
 
+msgid "No illustration on content!"
+msgstr "Ce contenu ne comporte pas d'illustration !"
+
+msgid "No provided object_name argument!"
+msgstr "L'argument manquant !"
+
 msgid "No session selected, booking was not changed."
 msgstr "Aucun événement sélectionné, la réservation n'a pas été modifiée."
 
 msgid "Not displayed"
 msgstr "Non affichées"
 
 msgid "Notepad"
@@ -1364,14 +1382,17 @@
 
 msgid "Price name"
 msgstr "Nom du tarif"
 
 msgid "Primary language used for TMDB API"
 msgstr "Langue principale utilisée pour les accès à l'API"
 
+msgid "Principal ID"
+msgstr "ID du mandataire"
+
 msgid "Producer:"
 msgstr "Producteurs :"
 
 msgid "Producers"
 msgstr "Producteurs"
 
 msgid "Properties"
@@ -1601,14 +1622,17 @@
 
 msgid "Sessions planning"
 msgstr "Agenda des événements programmés"
 
 msgid "Sessions weeks"
 msgstr "Nombre de semaines"
 
+msgid "Set as content illustration"
+msgstr "Utiliser comme illustration du contenu"
+
 msgid "Settings"
 msgstr "Paramètres"
 
 msgid "Site's header is generally displayed in page header"
 msgstr "Le chapô est généralement affiché dans les en-têtes de pages"
 
 msgid "Sites managers"
@@ -1652,16 +1676,19 @@
 
 msgid "Subject of update message sent to the recipient"
 msgstr "Sujet du message de modification adressé au bénéficiaire"
 
 msgid "Subject prefix"
 msgstr "Préfixe des sujets"
 
-msgid "Synchronize"
-msgstr "Synchronizer les agendas"
+msgid "Synchronize calendars scrolling"
+msgstr "Synchroniser le défilement des agendas"
+
+msgid "Synchronize calendars views"
+msgstr "Synchroniser les vues des agendas"
 
 msgid "Synopsis"
 msgstr "Synopsis"
 
 msgid "Synopsis:"
 msgstr "Synopsis :"
 
@@ -1724,17 +1751,14 @@
 
 msgid "Theater management"
 msgstr "Gérer le cinéma"
 
 msgid "Theater room in which session is planned"
 msgstr "Salle dans laquelle la séance est planifiée"
 
-msgid "Theater week"
-msgstr "Sem. ciné."
-
 msgid "There are only {} free seats left in this session!"
 msgstr ""
 "<strong>ATTENTION :</strong> il ne reste que {} places libres sur cet "
 "événement !"
 
 msgid "There is no confirmed booking for this session."
 msgstr "Aucune réservation validée pour cet événement."
@@ -1998,15 +2022,15 @@
 
 msgid "Total amount"
 msgstr "Total TTC"
 
 msgid "Translated version"
 msgstr "Version traduite"
 
-msgid "Transpose"
+msgid "Transpose calendars"
 msgstr "Transposer les agendas"
 
 msgid "URL of theater web site"
 msgstr "URL du site web du cinéma"
 
 msgid "Unit price"
 msgstr "Tarif"
@@ -2135,15 +2159,17 @@
 
 msgid ""
 "You can select an existing activity from your catalog, or keep this input "
 "empty if you just want to mark a period as not being available for booking"
 msgstr ""
 "Vous pouvez sélectionner une activité présente au sein de votre catalogue, "
 "ou ne rien sélectionner si vous voulez simplement indiquer qu'une période "
-"n'est pas disponible pour d'autres activités"
+"n'est pas disponible pour d'autres activités ; le fait qu'un événement soit "
+"\"hors catalogue\" ne vous empêche pas cependant d'y associer des "
+"réservations"
 
 msgid ""
 "You can set an integer number which will define the count of participants "
 "for which one accompanying person will have free access"
 msgstr ""
 "Vous pouvez indiquer ici le nombre de participants par accompagnateur qui "
 "bénéficient d'une entrée non payante, ou 0 pour que tous les accompagnateurs "
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po` & `pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # PyAMS application for cinema reservation management
 #
 # This file is distributed under the same license as the PACKAGE package.
 # Thierry Florac <tflorac@ulthar.net>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: PyAMS MSC application 1.0.0\n"
-"POT-Creation-Date: 2024-04-27 14:19+0200\n"
+"POT-Creation-Date: 2024-05-05 20:34+0200\n"
 "Last-Translator: Thierry Florac <tflorac@ulthar.net>\n"
 "Language-Team: FRENCH <FR@li.org>\n"
 "Language: French\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.10.dev0\n"
@@ -338,15 +338,15 @@
 
 #: src/pyams_app_msc/feature/tmdb/zmi/__init__.py:64
 msgid "TMDB service properties"
 msgstr "Propriétés du service"
 
 #: src/pyams_app_msc/feature/profile/interfaces.py:43
 msgid "Principal ID"
-msgstr ""
+msgstr "ID du mandataire"
 
 #: src/pyams_app_msc/feature/profile/interfaces.py:46
 msgid "Active user?"
 msgstr "Profil actif ?"
 
 #: src/pyams_app_msc/feature/profile/interfaces.py:47
 msgid "Inactive users can't login anymore to website"
@@ -387,35 +387,35 @@
 msgid "Establishment address"
 msgstr "Adresse de l'établissement ou de la structure"
 
 #: src/pyams_app_msc/feature/profile/interfaces.py:75
 msgid "Preferred local theaters"
 msgstr "Cinémas de rattachement"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:89
+#: src/pyams_app_msc/feature/profile/interfaces.py:92
 msgid "Not displayed"
 msgstr "Non affichées"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:90
+#: src/pyams_app_msc/feature/profile/interfaces.py:93
 msgid "Display confirmed/requested/capacity seats"
 msgstr "Afficher les places acceptées / demandées / en jauge"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:91
+#: src/pyams_app_msc/feature/profile/interfaces.py:94
 msgid "Display confirmed/waiting/capacity seats"
 msgstr "Afficher les places acceptées / en attente / en jauge"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:92
+#: src/pyams_app_msc/feature/profile/interfaces.py:95
 msgid "Display confirmed/capacity seats"
 msgstr "Afficher les places acceptées / en jauge"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:108
+#: src/pyams_app_msc/feature/profile/interfaces.py:111
 msgid "Session seats display mode"
 msgstr "Affichage des places dans l'agenda"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:109
+#: src/pyams_app_msc/feature/profile/interfaces.py:112
 msgid ""
 "You can choose how session seats are displayed in movie theater planning view"
 msgstr ""
 "Vous pouvez choisir la façon dont les places sont affichées dans le planning "
 "des activités"
 
 #: src/pyams_app_msc/feature/profile/task.py:56
@@ -715,14 +715,16 @@
 
 #: src/pyams_app_msc/feature/messaging/zmi/__init__.py:54
 msgid "Messaging properties"
 msgstr "Propriétés de la messagerie"
 
 #: src/pyams_app_msc/feature/planning/session.py:155
 #: src/pyams_app_msc/feature/planning/zmi/session.py:236
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:198
+#: src/pyams_app_msc/shared/theater/zmi/session.py:76
 msgid "Out of catalog activity"
 msgstr "(activité hors-catalogue)"
 
 #: src/pyams_app_msc/feature/planning/session.py:160
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:180
 #, python-format
 msgid "{room} - {date} from {start_time} to {end_time}"
@@ -882,26 +884,28 @@
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:133
 #: src/pyams_app_msc/feature/booking/interfaces.py:166
 msgid "These comments are for internal use only"
 msgstr "Ce commentaire est à usage interne uniquement"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:140
-#: src/pyams_app_msc/feature/quotation/__init__.py:293
+#: src/pyams_app_msc/feature/quotation/__init__.py:297
 msgid "Activity"
 msgstr "Activité"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:141
 msgid ""
 "You can select an existing activity from your catalog, or keep this input "
 "empty if you just want to mark a period as not being available for booking"
 msgstr ""
 "Vous pouvez sélectionner une activité présente au sein de votre catalogue, "
 "ou ne rien sélectionner si vous voulez simplement indiquer qu'une période "
-"n'est pas disponible pour d'autres activités"
+"n'est pas disponible pour d'autres activités ; le fait qu'un événement soit "
+"\"hors catalogue\" ne vous empêche pas cependant d'y associer des "
+"réservations"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:61
 msgid "New session"
 msgstr "Nouvel événement"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:62
 msgid "New session properties"
@@ -917,15 +921,15 @@
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:188
 msgid "Session planning"
 msgstr "Programmation d'un événement"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:189
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:468
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:715
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:717
 msgid "Session properties"
 msgstr "Propriétés de l'événement"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:258
 msgid "You can't define a session gauge higher than the room's capacity!"
 msgstr ""
 "Vous ne pouvez pas définir une jauge supérieure à la capacité de la salle !"
@@ -965,52 +969,53 @@
 msgid "Planning"
 msgstr "Agenda"
 
 #: src/pyams_app_msc/feature/planning/zmi/__init__.py:76
 msgid "Sessions planning"
 msgstr "Agenda des événements programmés"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:131
-msgid "Theater week"
-msgstr "Sem. ciné."
-
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:145
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:146
 msgid "Today"
 msgstr "Aujourd'hui"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:146
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:147
 msgid "Month"
 msgstr "Mois"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:147
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:148
 msgid "Week"
 msgstr "Semaine"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:148
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:149
 msgid "Day"
 msgstr "Jour"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:149
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:150
 msgid "List"
 msgstr "Liste"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:150
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:151
 msgid "All-day"
 msgstr "(jour)"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:196
-msgid "Transpose"
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:197
+msgid "Transpose calendars"
 msgstr "Transposer les agendas"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:209
-msgid "Synchronize"
-msgstr "Synchronizer les agendas"
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:210
+msgid "Synchronize calendars views"
+msgstr "Synchroniser les vues des agendas"
+
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:223
+msgid "Synchronize calendars scrolling"
+msgstr "Synchroniser le défilement des agendas"
 
 #: src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:13
 #: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:13
+#: src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt:17
 msgid "Back to previous page"
 msgstr "Revenir à la page précédente"
 
 #: src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:42
 msgid "Manage event booking..."
 msgstr "Gérer les réservations"
 
@@ -1030,118 +1035,118 @@
 msgid "Date:"
 msgstr "Date :"
 
 #: src/pyams_app_msc/feature/quotation/__init__.py:198
 msgid "Object:"
 msgstr "Objet :"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:294
+#: src/pyams_app_msc/feature/quotation/__init__.py:298
 msgid "Units"
 msgstr "Unités"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:295
+#: src/pyams_app_msc/feature/quotation/__init__.py:299
 msgid "Unit price"
 msgstr "Tarif"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:296
+#: src/pyams_app_msc/feature/quotation/__init__.py:300
 msgid "Total"
 msgstr "Total"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:301
+#: src/pyams_app_msc/feature/quotation/__init__.py:305
 #, python-format
 msgid "   - Entries ({})"
 msgstr "   - Entrées ({})"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:302
+#: src/pyams_app_msc/feature/quotation/__init__.py:306
 #: src/pyams_app_msc/feature/booking/zmi/home.py:93
 msgid "1 group"
 msgstr "1 groupe"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:303
+#: src/pyams_app_msc/feature/quotation/__init__.py:307
 #: src/pyams_app_msc/feature/booking/zmi/home.py:92
 #, python-format
 msgid "{} groups"
 msgstr "{} groupes"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:310
+#: src/pyams_app_msc/feature/quotation/__init__.py:314
 msgid "   - Free accompanists"
 msgstr "   - Accompagnateurs non payants"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:317
+#: src/pyams_app_msc/feature/quotation/__init__.py:321
 msgid "   - Paying accompanists"
 msgstr "   - Accompagnateurs payants"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:328
+#: src/pyams_app_msc/feature/quotation/__init__.py:332
 msgid "Base amount"
 msgstr "Total HT"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:332
+#: src/pyams_app_msc/feature/quotation/__init__.py:336
 msgid "VAT"
 msgstr "TVA"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:336
+#: src/pyams_app_msc/feature/quotation/__init__.py:340
 msgid "Total amount"
 msgstr "Total TTC"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:371
+#: src/pyams_app_msc/feature/quotation/__init__.py:375
 #, python-format
 msgid "Bank location: {}"
 msgstr "Établissement bancaire : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:372
+#: src/pyams_app_msc/feature/quotation/__init__.py:376
 #: src/pyams_app_msc/component/banking/interfaces.py:31
 msgid "Bank code"
 msgstr "Code banque"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:373
+#: src/pyams_app_msc/feature/quotation/__init__.py:377
 #: src/pyams_app_msc/component/banking/interfaces.py:36
 msgid "Counter code"
 msgstr "Code guichet"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:374
+#: src/pyams_app_msc/feature/quotation/__init__.py:378
 #: src/pyams_app_msc/component/banking/interfaces.py:41
 msgid "Account number"
 msgstr "N° de compte"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:375
+#: src/pyams_app_msc/feature/quotation/__init__.py:379
 msgid "Key"
 msgstr "Clé"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:380
+#: src/pyams_app_msc/feature/quotation/__init__.py:384
 #, python-format
 msgid "IBAN: {}"
 msgstr "IBAN : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:383
+#: src/pyams_app_msc/feature/quotation/__init__.py:387
 #, python-format
 msgid "BIC: {}"
 msgstr "BIC : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:414
+#: src/pyams_app_msc/feature/quotation/__init__.py:418
 #, python-format
 msgid "APE: {}"
 msgstr "APE : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:415
+#: src/pyams_app_msc/feature/quotation/__init__.py:419
 #, python-format
 msgid "SIRET: {}"
 msgstr "SIRET : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:417
+#: src/pyams_app_msc/feature/quotation/__init__.py:421
 #, python-format
 msgid "VAT: {}"
 msgstr "Code TVA : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:443
+#: src/pyams_app_msc/feature/quotation/__init__.py:447
 #, python-format
 msgid "Quotation: {}"
 msgstr "Devis : {}"
 
 #: src/pyams_app_msc/feature/booking/reminder.py:50
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:819
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:821
 #: src/pyams_app_msc/shared/theater/zmi/mail.py:142
 msgid "Booking reminder"
 msgstr "Rappel de réservation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:75
 msgid "Waiting"
 msgstr "En attente"
@@ -1159,36 +1164,36 @@
 msgstr "En attente de confirmation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:79
 msgid "Accepted"
 msgstr "Acceptée"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:109
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:232
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:242
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:126
 msgid "Creator"
 msgstr "Créateur"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:110
 msgid "Name of the principal who created the booking"
 msgstr "Nom du mandataire ayant effectué la demande de réservation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:113
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:248
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:258
 #: src/pyams_app_msc/feature/booking/zmi/search.py:71
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:140
 msgid "Recipient"
 msgstr "Bénéficiaire"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:114
 msgid "Name of the principal for which the booking is done"
 msgstr "Nom du mandataire bénéficiaire de la réservation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:120
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:292
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:302
 #: src/pyams_app_msc/feature/booking/zmi/search.py:74
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:183
 msgid "Status"
 msgstr "Statut"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:125
 msgid "Participants"
@@ -1233,17 +1238,17 @@
 "for which one accompanying person will have free access"
 msgstr ""
 "Vous pouvez indiquer ici le nombre de participants par accompagnateur qui "
 "bénéficient d'une entrée non payante, ou 0 pour que tous les accompagnateurs "
 "aient à régler leur entrée"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:156
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:262
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:272
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:169
-#: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:46
+#: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:47
 msgid "Cultural pass"
 msgstr "Pass Culture"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:157
 msgid "Check this option if payment is done using cultural pass"
 msgstr ""
 "Sélectionnez cette option lorsque le paiement est fait via un Pass Culture"
@@ -1257,15 +1262,15 @@
 msgstr "Commentaire"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:162
 msgid "These comments where added by booking recipient"
 msgstr "Ce commentaire précise la demande du bénéficiaire"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:169
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:353
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:363
 msgid "Archived"
 msgstr "Archivée"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:170
 msgid ""
 "A booking is archived automatically after session end and can't be modified "
 "anymore"
@@ -1287,15 +1292,15 @@
 msgstr "Message associé au devis"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:192
 msgid "This message is added to quotation as an information message"
 msgstr "Ce message d'information est associé au devis envoyé au client"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:195
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:310
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:320
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:214
 msgid "Quotation"
 msgstr "Devis"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:196
 msgid "This quotation was attached to booking confirmation"
 msgstr "Ceci est le document au format PDF contenant le devis"
@@ -1451,21 +1456,21 @@
 msgstr "Nouvel événement auquel doit s'appliquer la réservation"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:217
 msgid "Change session"
 msgstr "Changer d'événement"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:221
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:510
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:512
 msgid "Cancel"
 msgstr "Annuler"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:234
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:367
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:523
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:525
 #, python-format
 msgid "Booking: {}"
 msgstr "Réservation : {}"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:237
 msgid "Change booking session"
 msgstr "Changement d'événement"
@@ -1483,15 +1488,15 @@
 msgid "There are only {} free seats left in this session!"
 msgstr ""
 "<strong>ATTENTION :</strong> il ne reste que {} places libres sur cet "
 "événement !"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:370
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:489
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:527
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:529
 msgid "Booking properties"
 msgstr "Propriétés de la réservation"
 
 #. Default: Cancel booking
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:622
 msgid "cancel-booking-menu"
 msgstr "Annuler"
@@ -1514,15 +1519,15 @@
 msgstr "Refuser la réservation"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:669
 msgid "Booking refused"
 msgstr "Réservation refusée"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:682
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:497
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:499
 msgid "Quotation preview"
 msgstr "Prévisualiser le devis"
 
 #. Default: Optional booking
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:701
 msgid "option-booking-menu"
 msgstr "Accepter (sous réserve)"
@@ -1557,15 +1562,15 @@
 msgstr "Accepter la réservation"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:780
 msgid "Booking accepted"
 msgstr "Réservation acceptée"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:826
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:703
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:705
 msgid "You must set a price to accept a booking!"
 msgstr "Vous devez spécifier un tarif pour pouvoir accepter une réservation !"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:908
 msgid ""
 "**WARNING**<br />The session capacity is too low to accept this booking!"
 msgstr ""
@@ -1593,57 +1598,57 @@
 msgstr "Tableau de bord"
 
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:99
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:100
 msgid "Booking dashboard"
 msgstr "Gestion des réservations"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:183
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:186
 msgid "Session"
 msgstr "Séance"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:199
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:209
 msgid "Room"
 msgstr "Salle"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:216
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:226
 msgid "Date"
 msgstr "Date"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:276
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:286
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:199
 msgid "Seats"
 msgstr "Places"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:331
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:341
 msgid "Last update"
 msgstr "Dernière modification"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:397
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:407
 msgid "MANAGER - No booking waiting for your action"
 msgstr "RESPONSABLE - Aucune réservation en attente"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:398
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:408
 msgid "MANAGER - 1 booking waiting for your action"
 msgstr "RESPONSABLE - 1 réservation en attente"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:399
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:409
 #, python-format
 msgid "MANAGER - {} bookings waiting for your action"
 msgstr "RESPONSABLE - {} réservations en attente"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:439
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:449
 msgid "MANAGER - No booking accepted"
 msgstr "RESPONSABLE - Aucune réservation acceptée"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:440
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:450
 msgid "MANAGER - 1 booking accepted"
 msgstr "RESPONSABLE - 1 réservation acceptée"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:441
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:451
 #, python-format
 msgid "MANAGER - {} bookings accepted"
 msgstr "RESPONSABLE - {} réservations acceptées"
 
 #: src/pyams_app_msc/feature/booking/zmi/search.py:64
 #: src/pyams_app_msc/feature/booking/zmi/search.py:115
 msgid "Advanced search"
@@ -1700,81 +1705,81 @@
 msgstr " (places : {})"
 
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:314
 #, python-format
 msgid "{}: {}"
 msgstr "{}: {}"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:341
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:343
 msgid "Add booking"
 msgstr "Ajouter une réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:358
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:360
 msgid "Add and accept"
 msgstr "Ajouter et accepter"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:368
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:370
 msgid "New booking"
 msgstr "Nouvelle réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:369
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:371
 msgid "New booking properties"
 msgstr "Propriétés de la nouvelle réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:500
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:502
 msgid "Reset quotation"
 msgstr "Ré-éditer le devis"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:506
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:508
 msgid "Apply"
 msgstr "Enregistrer"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:674
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:676
 msgid "This booking is archived and can't be modified anymore!"
 msgstr "Cette réservation est archivée et ne peut plus être modifiée !"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:743
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:745
 msgid "Booking quotation"
 msgstr "Devis de la réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:761
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:763
 msgid "Booking update"
 msgstr "Réservation modifiée"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:796
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:798
 msgid ""
 "Update message can be sent to booking recipient when a booking is modified "
 "after being validated."
 msgstr ""
 "Ce nouveau message sera adressé au bénéficiaire (avec le devis actualisé) "
 "pour indiquer que cette réservation qui a déjà été acceptée a été modifiée."
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:857
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:859
 #, python-format
 msgid ""
 "Reminder message will be sent to booking recipient {} hours before session "
 "begin date..."
 msgstr ""
 "Le message de rappel sera envoyé au bénéficiaire {} heures avant le début de "
 "l'événement."
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:872
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:874
 msgid "Quotation has been reset!"
 msgstr "Le devis a été re-généré !"
 
-#: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:52
+#: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:53
 msgid "${groups}: ${participants} participants, ${accompanists} accompanists"
 msgstr ""
 "${groups} : ${participants} participants, ${accompanists} accompagnateurs"
 
-#: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:65
+#: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:66
 msgid "There is no confirmed booking for this session."
 msgstr "Aucune réservation validée pour cet événement."
 
-#: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:73
+#: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:74
 msgid "There is no session planned for today."
 msgstr "Aucun événement n'est programmé aujourd'hui."
 
 #: src/pyams_app_msc/feature/booking/skin/__init__.py:50
 msgid "Session ID"
 msgstr "ID de l'événement"
 
@@ -1890,14 +1895,42 @@
 
 #: src/pyams_app_msc/component/address/interfaces.py:42
 msgid "Optional observations which can be added to describe the location"
 msgstr ""
 "Observations complémentaires qui peuvent être ajoutées pour décrire "
 "l'emplacement"
 
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:59
+msgid "Set as content illustration"
+msgstr "Utiliser comme illustration du contenu"
+
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:86
+msgid "No provided object_name argument!"
+msgstr "L'argument manquant !"
+
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:95
+msgid "Given element name doesn't exist!"
+msgstr "Le nom indiqué n'existe pas !"
+
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:104
+msgid "Can't find illustration target!"
+msgstr "Impossible de trouver la cible de l'illustration !"
+
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:118
+msgid "No illustration on content!"
+msgstr "Ce contenu ne comporte pas d'illustration !"
+
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:132
+msgid "Content illustration has been updated successfully."
+msgstr "L'illustration du contenu a été modifiée avec succès."
+
+#: src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt:15
+msgid "Gallery medias"
+msgstr "Galerie de médias"
+
 #: src/pyams_app_msc/component/contact/interfaces.py:30
 msgid "Full name"
 msgstr "Nom complet"
 
 #: src/pyams_app_msc/component/contact/interfaces.py:31
 msgid "Contact full name"
 msgstr "Nom complet du contact"
@@ -1915,15 +1948,15 @@
 msgstr "Téléphone"
 
 #: src/pyams_app_msc/shared/theater/room.py:112
 #, python-format
 msgid "{} ({} seats)"
 msgstr "{} ({} places)"
 
-#: src/pyams_app_msc/shared/theater/__init__.py:83
+#: src/pyams_app_msc/shared/theater/__init__.py:84
 msgid "Theater"
 msgstr "Cinéma"
 
 #: src/pyams_app_msc/shared/theater/zmi/mail.py:48
 #: src/pyams_app_msc/shared/theater/zmi/mail.py:59
 msgid "Mail templates"
 msgstr "Modèles de messages"
@@ -2147,67 +2180,67 @@
 msgid "Movie theater name is required!"
 msgstr "Le nom du cinéma est obligatoire !"
 
 #: src/pyams_app_msc/shared/theater/zmi/__init__.py:111
 msgid "A movie theater is already registered with this name!"
 msgstr "Un autre cinéma est déjà inscrit avec ce nom !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:168
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:162
 msgid "Theater management"
 msgstr "Gérer le cinéma"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:179
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:173
 msgid "Properties"
 msgstr "Propriétés"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:190
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:184
 msgid "Movie theater properties"
 msgstr "Propriétés du cinéma"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:191
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:185
 msgid "Main theater properties"
 msgstr "Propriétés principales"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:204
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:198
 msgid "Contacts"
 msgstr "Contacts"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:238
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:232
 msgid "Settings"
 msgstr "Paramètres"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:248
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:242
 msgid "Movie theater settings"
 msgstr "Paramètres du cinéma"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:249
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:243
 msgid "Main theater settings"
 msgstr "Paramètres principaux"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:269
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:263
 msgid "Booking settings"
 msgstr "Gestion des réservations"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:282
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:276
 msgid "Booking cancel mode"
 msgstr "Gestion des annulations"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:296
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:290
 msgid "Cancel max delay must be set in \"max delay\" mode!"
 msgstr ""
 "Le délai maximum après la réservation doit être indiqué pour utiliser ce "
 "mode d'annulation !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:299
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:293
 msgid "Cancel notice period must be set in \"notice period\" mode!"
 msgstr ""
 "Le préavis minimum avant l'événement doit être indiqué pour utiliser ce mode "
 "d'annulation !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:308
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:302
 msgid "Quotations settings"
 msgstr "Gestion des devis"
 
 #: src/pyams_app_msc/shared/theater/zmi/price.py:60
 #: src/pyams_app_msc/shared/theater/zmi/price.py:159
 msgid "Cinema prices"
 msgstr "Gestion des tarifs"
@@ -2860,35 +2893,35 @@
 msgid "Catalog management"
 msgstr "Gérer le catalogue"
 
 #: src/pyams_app_msc/shared/catalog/zmi/dashboard.py:69
 msgid "Activities catalog"
 msgstr "Gérer le catalogue"
 
-#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:60
+#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:63
 msgid "Enter text for TMDB movie search"
 msgstr "Indiquez un titre pour rechercher dans TMDB..."
 
-#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:93
+#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:96
 msgid "Add catalog entry"
 msgstr "Ajouter une activité au catalogue"
 
-#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:102
+#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:105
 msgid "New catalog entry properties"
 msgstr "Propriétés de la nouvelle activité"
 
-#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:173
+#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:191
 msgid "Activity details"
 msgstr "Détails de l'activité"
 
-#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:183
+#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:201
 msgid "Activity information"
 msgstr "Détails spécifiques de l'activité"
 
-#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:184
+#: src/pyams_app_msc/shared/catalog/zmi/__init__.py:202
 msgid "Custom properties"
 msgstr "Propriétés spécifiques"
 
 #: src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py:29
 msgid "Display sessions"
 msgstr "Afficher les séances"
 
@@ -3013,14 +3046,20 @@
 #: src/pyams_app_msc/root/interfaces.py:32
 msgid ""
 "These principals are allowed to create and manage sites and movie theaters"
 msgstr ""
 "Ces mandataires peuvent procéder à la création d'un nouveau cinéma et nommer "
 "ses gestionnaires"
 
+#~ msgid "Theater week"
+#~ msgstr "Sem. ciné."
+
+#~ msgid "Synchronize"
+#~ msgstr "Synchronizer les agendas"
+
 #~ msgid "Apartment"
 #~ msgstr "Appartement"
 
 #~ msgid "Floor, corridor..."
 #~ msgstr "Niveau, couloir..."
 
 #~ msgid "Entry"
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/pyams_app_msc.pot` & `pyams_app_msc-1.99.3/src/pyams_app_msc/locales/pyams_app_msc.pot`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-04-27 14:19+0200\n"
+"POT-Creation-Date: 2024-05-05 20:34+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -360,35 +360,35 @@
 msgid "Establishment address"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/profile/interfaces.py:75
 msgid "Preferred local theaters"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:89
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:92
 msgid "Not displayed"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:90
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:93
 msgid "Display confirmed/requested/capacity seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:91
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:94
 msgid "Display confirmed/waiting/capacity seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:92
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:95
 msgid "Display confirmed/capacity seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:108
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:111
 msgid "Session seats display mode"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:109
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:112
 msgid ""
 "You can choose how session seats are displayed in movie theater planning view"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/profile/task.py:56
 msgid "User profile cleaner"
 msgstr ""
@@ -652,14 +652,16 @@
 
 #: ./src/pyams_app_msc/feature/messaging/zmi/__init__.py:54
 msgid "Messaging properties"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/session.py:155
 #: ./src/pyams_app_msc/feature/planning/zmi/session.py:236
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:198
+#: ./src/pyams_app_msc/shared/theater/zmi/session.py:76
 msgid "Out of catalog activity"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/session.py:160
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:180
 #, python-format
 msgid "{room} - {date} from {start_time} to {end_time}"
@@ -810,15 +812,15 @@
 
 #: ./src/pyams_app_msc/feature/planning/interfaces.py:133
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:166
 msgid "These comments are for internal use only"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/interfaces.py:140
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:293
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:297
 msgid "Activity"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/interfaces.py:141
 msgid ""
 "You can select an existing activity from your catalog, or keep this input "
 "empty if you just want to mark a period as not being available for booking"
@@ -842,15 +844,15 @@
 
 #: ./src/pyams_app_msc/feature/planning/zmi/session.py:188
 msgid "Session planning"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/session.py:189
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:468
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:715
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:717
 msgid "Session properties"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/session.py:258
 msgid "You can't define a session gauge higher than the room's capacity!"
 msgstr ""
 
@@ -883,52 +885,53 @@
 msgid "Planning"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:76
 msgid "Sessions planning"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:131
-msgid "Theater week"
-msgstr ""
-
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:145
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:146
 msgid "Today"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:146
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:147
 msgid "Month"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:147
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:148
 msgid "Week"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:148
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:149
 msgid "Day"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:149
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:150
 msgid "List"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:150
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:151
 msgid "All-day"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:196
-msgid "Transpose"
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:197
+msgid "Transpose calendars"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:209
-msgid "Synchronize"
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:210
+msgid "Synchronize calendars views"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:223
+msgid "Synchronize calendars scrolling"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:13
 #: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:13
+#: ./src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt:17
 msgid "Back to previous page"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:42
 msgid "Manage event booking..."
 msgstr ""
 
@@ -948,118 +951,118 @@
 msgid "Date:"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/quotation/__init__.py:198
 msgid "Object:"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:294
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:298
 msgid "Units"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:295
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:299
 msgid "Unit price"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:296
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:300
 msgid "Total"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:301
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:305
 #, python-format
 msgid "   - Entries ({})"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:302
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:306
 #: ./src/pyams_app_msc/feature/booking/zmi/home.py:93
 msgid "1 group"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:303
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:307
 #: ./src/pyams_app_msc/feature/booking/zmi/home.py:92
 #, python-format
 msgid "{} groups"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:310
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:314
 msgid "   - Free accompanists"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:317
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:321
 msgid "   - Paying accompanists"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:328
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:332
 msgid "Base amount"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:332
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:336
 msgid "VAT"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:336
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:340
 msgid "Total amount"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:371
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:375
 #, python-format
 msgid "Bank location: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:372
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:376
 #: ./src/pyams_app_msc/component/banking/interfaces.py:31
 msgid "Bank code"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:373
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:377
 #: ./src/pyams_app_msc/component/banking/interfaces.py:36
 msgid "Counter code"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:374
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:378
 #: ./src/pyams_app_msc/component/banking/interfaces.py:41
 msgid "Account number"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:375
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:379
 msgid "Key"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:380
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:384
 #, python-format
 msgid "IBAN: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:383
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:387
 #, python-format
 msgid "BIC: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:414
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:418
 #, python-format
 msgid "APE: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:415
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:419
 #, python-format
 msgid "SIRET: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:417
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:421
 #, python-format
 msgid "VAT: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:443
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:447
 #, python-format
 msgid "Quotation: {}"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/reminder.py:50
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:819
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:821
 #: ./src/pyams_app_msc/shared/theater/zmi/mail.py:142
 msgid "Booking reminder"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:75
 msgid "Waiting"
 msgstr ""
@@ -1077,36 +1080,36 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:79
 msgid "Accepted"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:109
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:232
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:242
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:126
 msgid "Creator"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:110
 msgid "Name of the principal who created the booking"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:113
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:248
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:258
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:71
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:140
 msgid "Recipient"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:114
 msgid "Name of the principal for which the booking is done"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:120
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:292
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:302
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:74
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:183
 msgid "Status"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:125
 msgid "Participants"
@@ -1148,17 +1151,17 @@
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:150
 msgid ""
 "You can set an integer number which will define the count of participants for"
 " which one accompanying person will have free access"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:156
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:262
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:272
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:169
-#: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:46
+#: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:47
 msgid "Cultural pass"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:157
 msgid "Check this option if payment is done using cultural pass"
 msgstr ""
 
@@ -1171,15 +1174,15 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:162
 msgid "These comments where added by booking recipient"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:169
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:353
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:363
 msgid "Archived"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:170
 msgid ""
 "A booking is archived automatically after session end and can't be modified "
 "anymore"
@@ -1199,15 +1202,15 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:192
 msgid "This message is added to quotation as an information message"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:195
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:310
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:320
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:214
 msgid "Quotation"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:196
 msgid "This quotation was attached to booking confirmation"
 msgstr ""
@@ -1343,21 +1346,21 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:217
 msgid "Change session"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:221
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:510
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:512
 msgid "Cancel"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:234
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:367
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:523
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:525
 #, python-format
 msgid "Booking: {}"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:237
 msgid "Change booking session"
 msgstr ""
@@ -1373,15 +1376,15 @@
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:303
 #, python-format
 msgid "There are only {} free seats left in this session!"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:370
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:489
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:527
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:529
 msgid "Booking properties"
 msgstr ""
 
 #. Default: Cancel booking
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:622
 msgid "cancel-booking-menu"
 msgstr ""
@@ -1404,15 +1407,15 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:669
 msgid "Booking refused"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:682
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:497
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:499
 msgid "Quotation preview"
 msgstr ""
 
 #. Default: Optional booking
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:701
 msgid "option-booking-menu"
 msgstr ""
@@ -1447,15 +1450,15 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:780
 msgid "Booking accepted"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:826
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:703
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:705
 msgid "You must set a price to accept a booking!"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:908
 msgid ""
 "**WARNING**<br />The session capacity is too low to accept this booking!"
 msgstr ""
@@ -1479,57 +1482,57 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:99
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:100
 msgid "Booking dashboard"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:183
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:186
 msgid "Session"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:199
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:209
 msgid "Room"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:216
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:226
 msgid "Date"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:276
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:286
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:199
 msgid "Seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:331
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:341
 msgid "Last update"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:397
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:407
 msgid "MANAGER - No booking waiting for your action"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:398
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:408
 msgid "MANAGER - 1 booking waiting for your action"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:399
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:409
 #, python-format
 msgid "MANAGER - {} bookings waiting for your action"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:439
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:449
 msgid "MANAGER - No booking accepted"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:440
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:450
 msgid "MANAGER - 1 booking accepted"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:441
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:451
 #, python-format
 msgid "MANAGER - {} bookings accepted"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:64
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:115
 msgid "Advanced search"
@@ -1586,76 +1589,76 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:314
 #, python-format
 msgid "{}: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:341
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:343
 msgid "Add booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:358
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:360
 msgid "Add and accept"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:368
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:370
 msgid "New booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:369
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:371
 msgid "New booking properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:500
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:502
 msgid "Reset quotation"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:506
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:508
 msgid "Apply"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:674
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:676
 msgid "This booking is archived and can't be modified anymore!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:743
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:745
 msgid "Booking quotation"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:761
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:763
 msgid "Booking update"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:796
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:798
 msgid ""
 "Update message can be sent to booking recipient when a booking is modified "
 "after being validated."
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:857
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:859
 #, python-format
 msgid ""
 "Reminder message will be sent to booking recipient {} hours before session "
 "begin date..."
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:872
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:874
 msgid "Quotation has been reset!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:52
+#: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:53
 msgid "${groups}: ${participants} participants, ${accompanists} accompanists"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:65
+#: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:66
 msgid "There is no confirmed booking for this session."
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:73
+#: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:74
 msgid "There is no session planned for today."
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/skin/__init__.py:50
 msgid "Session ID"
 msgstr ""
 
@@ -1759,14 +1762,42 @@
 msgid "City"
 msgstr ""
 
 #: ./src/pyams_app_msc/component/address/interfaces.py:42
 msgid "Optional observations which can be added to describe the location"
 msgstr ""
 
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:59
+msgid "Set as content illustration"
+msgstr ""
+
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:86
+msgid "No provided object_name argument!"
+msgstr ""
+
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:95
+msgid "Given element name doesn't exist!"
+msgstr ""
+
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:104
+msgid "Can't find illustration target!"
+msgstr ""
+
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:118
+msgid "No illustration on content!"
+msgstr ""
+
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:132
+msgid "Content illustration has been updated successfully."
+msgstr ""
+
+#: ./src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt:15
+msgid "Gallery medias"
+msgstr ""
+
 #: ./src/pyams_app_msc/component/contact/interfaces.py:30
 msgid "Full name"
 msgstr ""
 
 #: ./src/pyams_app_msc/component/contact/interfaces.py:31
 msgid "Contact full name"
 msgstr ""
@@ -1784,15 +1815,15 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/room.py:112
 #, python-format
 msgid "{} ({} seats)"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/__init__.py:83
+#: ./src/pyams_app_msc/shared/theater/__init__.py:84
 msgid "Theater"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/mail.py:48
 #: ./src/pyams_app_msc/shared/theater/zmi/mail.py:59
 msgid "Mail templates"
 msgstr ""
@@ -2003,63 +2034,63 @@
 msgid "Movie theater name is required!"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:111
 msgid "A movie theater is already registered with this name!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:168
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:162
 msgid "Theater management"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:179
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:173
 msgid "Properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:190
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:184
 msgid "Movie theater properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:191
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:185
 msgid "Main theater properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:204
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:198
 msgid "Contacts"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:238
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:232
 msgid "Settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:248
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:242
 msgid "Movie theater settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:249
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:243
 msgid "Main theater settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:269
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:263
 msgid "Booking settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:282
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:276
 msgid "Booking cancel mode"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:296
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:290
 msgid "Cancel max delay must be set in \"max delay\" mode!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:299
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:293
 msgid "Cancel notice period must be set in \"notice period\" mode!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:308
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:302
 msgid "Quotations settings"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/price.py:60
 #: ./src/pyams_app_msc/shared/theater/zmi/price.py:159
 msgid "Cinema prices"
 msgstr ""
@@ -2633,35 +2664,35 @@
 msgid "Catalog management"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/catalog/zmi/dashboard.py:69
 msgid "Activities catalog"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:60
+#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:63
 msgid "Enter text for TMDB movie search"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:93
+#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:96
 msgid "Add catalog entry"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:102
+#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:105
 msgid "New catalog entry properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:173
+#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:191
 msgid "Activity details"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:183
+#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:201
 msgid "Activity information"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:184
+#: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:202
 msgid "Custom properties"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py:29
 msgid "Display sessions"
 msgstr ""
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/table.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/viewlet.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/root/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/root/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/root/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/api/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/index.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/index.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/manager.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/page.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/search.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/security.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/security.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,31 +22,34 @@
 from pyams_app_msc.feature.tmdb.zmi.lookup import ITMDBSearchInterface
 from pyams_app_msc.interfaces import MANAGE_CATALOG_PERMISSION
 from pyams_app_msc.shared.catalog.interfaces import ICatalogEntryInfo, ICatalogManager, ICatalogManagerTarget, \
     IWfCatalogEntry, IWfCatalogEntryAddInfo
 from pyams_app_msc.shared.catalog.zmi.interfaces import ICatalogManagementMenu, ICatalogManagementView
 from pyams_app_msc.shared.theater import IMovieTheater
 from pyams_content.shared.common.zmi import SharedContentAddAction, SharedContentAddForm
+from pyams_content.shared.common.zmi.content import SharedContentHeaderViewlet
 from pyams_content.shared.common.zmi.types.content import TypedSharedContentCustomInfoEditForm, \
     TypedSharedContentPropertiesEditForm
 from pyams_form.ajax import AJAXFormRenderer, ajax_form_config
 from pyams_form.browser.select import SelectWidget
 from pyams_form.field import Fields
 from pyams_form.interfaces.form import IAJAXFormRenderer, IFormContent
 from pyams_form.widget import FieldWidget
 from pyams_i18n.interfaces import INegotiator
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces import IViewContextPermissionChecker
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
+from pyams_skin.interfaces.viewlet import IHeaderViewletManager
 from pyams_skin.interfaces.widget import IDynamicSelectWidget
 from pyams_utils.adapter import NullAdapter, adapter_config
 from pyams_utils.factory import create_object
 from pyams_utils.interfaces.data import IObjectData
 from pyams_utils.registry import get_utility
 from pyams_utils.traversing import get_parent
+from pyams_utils.url import absolute_url
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IPropertiesMenu, IToolbarViewletManager
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
 __docformat__ = 'restructuredtext'
 
@@ -148,14 +151,29 @@
     def render(self, changes):
         return {
             'status': 'redirect',
             'location': self.form.next_url()
         }
 
 
+@viewlet_config(name='pyams.content_header',
+                context=IWfCatalogEntry, layer=IAdminLayer,
+                manager=IHeaderViewletManager, weight=10)
+class CatalogEntryHeaderViewlet(SharedContentHeaderViewlet):
+    """Catalog entry header viewlet"""
+
+    @property
+    def parent_target_url(self):
+        """Parent target URL"""
+        tool = get_parent(self.context, IMovieTheater)
+        if tool is None:
+            return None
+        return absolute_url(tool, self.request, 'admin#dashboard.html')
+
+
 @ajax_form_config(name='properties.html',
                   context=IWfCatalogEntry, layer=IPyAMSLayer,
                   permission=VIEW_SYSTEM_PERMISSION)
 class CatalogEntryPropertiesEditForm(TypedSharedContentPropertiesEditForm):
     """Catalog entry properties edit form"""
 
     interface = IWfCatalogEntry
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/dashboard.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/workflow.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/viewlet.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/viewlet.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/price.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/schema.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/audience.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/audience.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/mail.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/price.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/room.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/mail.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/page.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/price.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/room.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/session.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/settings.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,21 +148,15 @@
     """Movie theater breadcrumb item"""
 
     @property
     def label(self):
         return II18n(self.context).query_attribute('short_name', request=self.request)
 
     css_class = 'breadcrumb-item persistent strong'
-
-    @property
-    def view_name(self):
-        """Movie theater breadcrumb view getter"""
-        if IWfCatalogEntry.providedBy(self.request.context):
-            return 'admin#dashboard.html'
-        return 'admin'
+    view_name = 'admin'
 
 
 @adapter_config(required=(IMovieTheater, IAdminLayer, Interface, ISiteManagementMenu),
                 provides=IMenuHeader)
 def movie_theater_management_menu_header(context, request, view, manager):
     """Movie theater management menu header adapter"""
     return _("Theater management")
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/audience.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/interfaces.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/mail.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/planning.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/planning.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/presentation.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/presentation.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/price.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/restrictions.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/room.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/search.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/session.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_*** module
 
 """
 
-__docformat__ = 'restructuredtext'
-
 from pyramid.view import view_config
 from zope.interface import alsoProvides
 
 from pyams_app_msc.feature.planning.interfaces import IMovieTheaterSession, IPlanning, ISession
 from pyams_app_msc.feature.planning.zmi.session import SessionAddForm
 from pyams_app_msc.interfaces import MANAGE_CATALOG_PERMISSION
 from pyams_app_msc.shared.catalog.interfaces import CATALOG_ENTRY_CONTENT_TYPE
@@ -32,14 +30,19 @@
 from pyams_sequence.api.rest import find_references
 from pyams_sequence.reference import get_reference_target
 from pyams_utils.fanstatic import get_resource_path
 from pyams_utils.interfaces.data import IObjectData
 from pyams_utils.interfaces.form import NO_VALUE_STRING
 from pyams_utils.url import absolute_url
 
+__docformat__ = 'restructuredtext'
+
+from pyams_app_msc import _
+
+
 IMovieTheaterSession['activity'].content_type = CATALOG_ENTRY_CONTENT_TYPE
 
 
 @view_config(name='find-references.json',
              context=IMovieTheater, request_type=IPyAMSLayer,
              permission=USE_INTERNAL_API_PERMISSION,
              renderer='json', xhr=True)
@@ -65,14 +68,16 @@
 
     planning_target = None
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         activity = self.widgets.get('activity')
         if activity is not None:
+            activity.prompt = True
+            activity.prompt_message = self.request.localizer.translate(_("Out of catalog activity"))
             activity.ajax_url = absolute_url(self.context, self.request, 'find-references.json')
             activity.object_data = {
                 'ams-modules': {
                     'msc': {
                         'src': get_resource_path(msc)
                     }
                 },
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/types.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/types.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/viewlet.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/form.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/form.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/layer.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/layer.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/login.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/login.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_form.js` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_form.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_gis.js` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_gis.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_search.js` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_search.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_utils.js` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_utils.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/app.js` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/app.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_content.scss` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_content.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_footer.scss` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_footer.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_forms.scss` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_forms.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_layout.scss` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_layout.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_misc.scss` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_misc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_variables.scss` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_variables.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/msc.scss` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/msc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/templates/select-admin-theater.pt` & `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/templates/select-admin-theater.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/test_utilsdocs.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/test_utilsdocstrings.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/__init__.py` & `pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/img/pass-culture.webp` & `pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/img/pass-culture.webp`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/msc.js` & `pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/msc.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -39,14 +39,53 @@
             const
                 source = $(evt.currentTarget),
                 select = source.siblings('select'),
                 principalId = select.val();
             MyAMS.require('modal').then(() => {
                 MyAMS.modal.open(`edit-user-profile.html?principal_id=${principalId}`);
             })
+        },
+
+        setIllustrationFromGallery: (evt, options) => {
+            const
+                source = $(evt.currentTarget),
+                sourceHtml = source.html(),
+                media = source.parents('.media-thumbnail'),
+                gallery = media.parents('.gallery'),
+                location = gallery.data('ams-location');
+            MyAMS.require('ajax', 'alert', 'i18n').then(() => {
+                MyAMS.alert.bigBox({
+                    status: 'warning',
+                    icon: 'fas fa-bell',
+                    title: MyAMS.i18n.WARNING,
+                    message: "Confirmez-vous le remplacement de l'illustration ?",
+                    successLabel: MyAMS.i18n.CONFIRM,
+                    cancelLabel: MyAMS.i18n.BTN_CANCEL
+                }).then((status) => {
+                    if (status !== 'success') {
+                        return
+                    }
+                    source.html('<i class="fas fa-fw fa-spinner fa-spin"></i>');
+                    MyAMS.ajax.post(`${location}/set-content-illustration.json`, {
+                        object_name: media.data('ams-element-name')
+                    }).then((result) => {
+                        MyAMS.require('alert').then(() => {
+                            MyAMS.alert.smallBox({
+                                status: result.status,
+                                message: result.message,
+                                icon: 'fa-info-circle',
+                                timeout: 3000
+                            });
+                            source.html(sourceHtml);
+                        });
+                    }).catch(() => {
+                        source.html(sourceHtml);
+                    });
+                });
+            });
         }
     },
 
     /**
      * Session management
      */
     session: {
@@ -79,16 +118,17 @@
      * Calendar management
      */
     calendar: {
 
         /**
          * Boolean flag to check if calendars are synchronized
          */
-        synchronized: localStorage.getItem('msc.synchronized') === 'true',
         transposed: localStorage.getItem('msc.transposed') === 'true',
+        synchronized: localStorage.getItem('msc.synchronized') === 'true',
+        scrolling: localStorage.getItem('msc.scrolling') === 'true',
 
         /**
          * Initialize calendar events handlers
          */
         init: (event, element, settings, veto) => {
             settings['eventContent'] = MyAMS.msc.calendar.setEventContent;
             settings['eventClassNames'] = MyAMS.msc.calendar.setEventClassNames;
@@ -145,14 +185,32 @@
                     button.button('toggle')
                         .toggleClass('btn-light')
                         .toggleClass('btn-link')
                         .toggleClass('btn-secondary')
                         .toggleClass('border-secondary');
                 }
             }
+            if (msc.calendar.scrolling) {
+                const button = $('a[href="MyAMS.msc.calendar.scroll"]');
+                if (button.exists()) {
+                    button.button('toggle')
+                        .toggleClass('btn-light')
+                        .toggleClass('btn-link')
+                        .toggleClass('btn-secondary')
+                        .toggleClass('border-secondary');
+                }
+                setTimeout(() => {
+                    const scrollers = $('.fc-scroller', $('.calendar tbody td'));
+                    scrollers.off('scroll')
+                        .on('scroll', (evt) => {
+                            const top = $(evt.currentTarget).scrollTop();
+                            scrollers.scrollTop(top);
+                        });
+                }, 50);
+            }
         },
 
         setEventContent: (info) => {
             const title = info.event.title.split('\n');
             return {
                 html: `<strong>${title[0]}</strong><br />${title[1] || ''}`
             }
@@ -231,14 +289,36 @@
                 .toggleClass('btn-link')
                 .toggleClass('btn-secondary')
                 .toggleClass('border-secondary');
             localStorage.setItem('msc.synchronized', source.hasClass('btn-secondary'));
         },
 
         /**
+         *
+         */
+        scroll: (source) => {
+            const scrollers = $('.fc-scroller', $('.calendar tbody td'));
+            msc.calendar.scrolling = !msc.calendar.scrolling;
+            if (msc.calendar.scrolling) {
+                scrollers.on('scroll', (evt) => {
+                    const top = $(evt.currentTarget).scrollTop();
+                    scrollers.scrollTop(top);
+                });
+            } else {
+                scrollers.off('scroll');
+            }
+            source.button('toggle')
+                .toggleClass('btn-light')
+                .toggleClass('btn-link')
+                .toggleClass('btn-secondary')
+                .toggleClass('border-secondary');
+            localStorage.setItem('msc.scrolling', source.hasClass('btn-secondary'));
+        },
+
+        /**
          * List of calendar being updated
          */
         updating: [],
 
         /**
          * Synchronize calendars dates changes
          */
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/msc.min.js` & `pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/msc.min.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,46 @@
         getPrincipalID: e => {
             const t = $(e.currentTarget),
                 a = t.siblings("select"),
                 n = a.val();
             MyAMS.require("modal").then(() => {
                 MyAMS.modal.open("edit-user-profile.html?principal_id=" + n)
             })
+        },
+        setIllustrationFromGallery: (e, t) => {
+            const a = $(e.currentTarget),
+                n = a.html(),
+                r = a.parents(".media-thumbnail"),
+                s = r.parents(".gallery"),
+                o = s.data("ams-location");
+            MyAMS.require("ajax", "alert", "i18n").then(() => {
+                MyAMS.alert.bigBox({
+                    status: "warning",
+                    icon: "fas fa-bell",
+                    title: MyAMS.i18n.WARNING,
+                    message: "Confirmez-vous le remplacement de l'illustration ?",
+                    successLabel: MyAMS.i18n.CONFIRM,
+                    cancelLabel: MyAMS.i18n.BTN_CANCEL
+                }).then(e => {
+                    "success" === e && (a.html('<i class="fas fa-fw fa-spinner fa-spin"></i>'), MyAMS.ajax.post(o + "/set-content-illustration.json", {
+                        object_name: r.data("ams-element-name")
+                    }).then(e => {
+                        MyAMS.require("alert").then(() => {
+                            MyAMS.alert.smallBox({
+                                status: e.status,
+                                message: e.message,
+                                icon: "fa-info-circle",
+                                timeout: 3e3
+                            }), a.html(n)
+                        })
+                    }).catch(() => {
+                        a.html(n)
+                    }))
+                })
+            })
         }
     },
     session: {
         changeActivity: e => {
             $("html").attr("lang");
             const n = $(e.currentTarget).parents("form"),
                 t = $('select[name$=".widgets.activity"]', n),
@@ -35,31 +67,38 @@
                     var t, a, e = e.info?.catalog_entry?.duration;
                     e && (a = $('input[name$=".widgets.start_date"]', n), a = new Date(a.val()), t = $('input[id$="-widgets-end_date-dt"]', n), a = new Date(a.getTime() + 6e4 * e), t.data("datetimepicker").date(a))
                 })
             })
         }
     },
     calendar: {
-        synchronized: "true" === localStorage.getItem("msc.synchronized"),
         transposed: "true" === localStorage.getItem("msc.transposed"),
+        synchronized: "true" === localStorage.getItem("msc.synchronized"),
+        scrolling: "true" === localStorage.getItem("msc.scrolling"),
         init: (e, t, a, n) => {
             a.eventContent = MyAMS.msc.calendar.setEventContent, a.eventClassNames = MyAMS.msc.calendar.setEventClassNames, a.eventDidMount = MyAMS.msc.calendar.renderedEvent, a.dateClick = MyAMS.msc.calendar.addEvent, a.eventClick = MyAMS.msc.calendar.showEvent, a.eventDrop = MyAMS.msc.calendar.dropEvent, a.eventResize = MyAMS.msc.calendar.resizeEvent, a.eventReceive = MyAMS.msc.calendar.receiveEvent, a.datesSet = MyAMS.msc.calendar.setDates
         },
         refresh: (e, t) => {
             "object" == typeof t && (e = t.room_id);
             t = $(`.calendar[data-msc-room="${e}"]`).data("msc-calendar");
             t && t.refetchEvents()
         },
         refreshAll: () => {
             $(".calendar").each((e, t) => {
                 $(t).data("msc-calendar").refetchEvents()
             })
         },
         afterInit: (e, t, a) => {
-            t.data("msc-calendar", a), msc.calendar.transposed && ($(".calendar-wrapper").addClass("transposed"), (t = $('a[href="MyAMS.msc.calendar.transpose"]')).exists()) && t.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), msc.calendar.synchronized && (a = $('a[href="MyAMS.msc.calendar.synchronize"]')).exists() && a.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary")
+            t.data("msc-calendar", a), msc.calendar.transposed && ($(".calendar-wrapper").addClass("transposed"), (t = $('a[href="MyAMS.msc.calendar.transpose"]')).exists()) && t.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), msc.calendar.synchronized && (a = $('a[href="MyAMS.msc.calendar.synchronize"]')).exists() && a.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), msc.calendar.scrolling && ((t = $('a[href="MyAMS.msc.calendar.scroll"]')).exists() && t.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), setTimeout(() => {
+                const t = $(".fc-scroller", $(".calendar tbody td"));
+                t.off("scroll").on("scroll", e => {
+                    e = $(e.currentTarget).scrollTop();
+                    t.scrollTop(e)
+                })
+            }, 50))
         },
         setEventContent: e => {
             e = e.event.title.split("\n");
             return {
                 html: `<strong>${e[0]}</strong><br />` + (e[1] || "")
             }
         },
@@ -94,14 +133,21 @@
                     })
                 } finally {
                     msc.calendar.synchronized = !0
                 }
             }
             e.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), localStorage.setItem("msc.synchronized", e.hasClass("btn-secondary"))
         },
+        scroll: e => {
+            const t = $(".fc-scroller", $(".calendar tbody td"));
+            msc.calendar.scrolling = !msc.calendar.scrolling, msc.calendar.scrolling ? t.on("scroll", e => {
+                e = $(e.currentTarget).scrollTop();
+                t.scrollTop(e)
+            }) : t.off("scroll"), e.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), localStorage.setItem("msc.scrolling", e.hasClass("btn-secondary"))
+        },
         updating: [],
         setDates: a => {
             if ($(".tooltip").tooltip("hide"), msc.calendar.synchronized) {
                 const n = msc.calendar.updating;
                 if (!(-1 < n.indexOf(a.view.calendar))) {
                     n.push(a.view.calendar);
                     var e = $(".calendar");
@@ -195,27 +241,27 @@
         receiveEvent: i => ($(".tooltip").tooltip("hide"), new Promise((t, e) => {
             const a = i.event,
                 n = a.extendedProps?.href;
             if (n) {
                 const r = $(i.view.calendar.el),
                     s = r.data("msc-calendar"),
                     o = r.data("msc-room"),
-                    d = a.extendedProps?.room,
-                    l = $(`.calendar[data-msc-room="${d}"]`).data("msc-calendar");
+                    l = a.extendedProps?.room,
+                    c = $(`.calendar[data-msc-room="${l}"]`).data("msc-calendar");
                 MyAMS.require("ajax").then(() => {
                     MyAMS.ajax.post(n + "/update-event.json", {
                         room: o.toString(),
                         start: a.startStr,
                         end: a.endStr
                     }).then(e => {
-                        i.revert(), l.refetchEvents(), s.refetchEvents(), e.messagebox ? MyAMS.require("alert").then(() => {
+                        i.revert(), c.refetchEvents(), s.refetchEvents(), e.messagebox ? MyAMS.require("alert").then(() => {
                             MyAMS.alert.messageBox(e.messagebox), t(e)
                         }) : t(e)
                     }, () => {
-                        i.revert(), l.refetchEvents(), s.refetchEvents(), e()
+                        i.revert(), c.refetchEvents(), s.refetchEvents(), e()
                     })
                 })
             } else i.revert(), e()
         })),
         deleteEventCallback: (e, t) => {
             t = $(`.calendar[data-msc-room="${t.room}"]`).data("msc-calendar").getEventById(t.event_id);
             $(".tooltip").tooltip("hide"), t && t.remove()
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/PKG-INFO` & `pyams_app_msc-1.99.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-app-msc
-Version: 1.99.2.4
+Name: pyams_app_msc
+Version: 1.99.3
 Summary: PyAMS application for cinema reservation management
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -44,14 +44,24 @@
 PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
 
 
 Changelog
 =========
 
+1.99.3
+------
+ - issue #21: added display of principal phone number
+ - issue #22: updated shared content header viewlet to add button to go back to dashboard
+ - issue #25: updated prompt of activity selection widget
+ - issue #26: added support for vertical synchronization of calendars
+ - issue #27: removed theater week view from calendar
+ - issue #30: added action to set content illustration from medias gallery image
+ - issue #31: updated accompagnists price handler in quotations
+
 1.99.2.4
 --------
  - removed code dependency on OAuth authentication module (bis!)
 
 1.99.2.3
 --------
  - removed code dependency on OAuth authentication module
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/SOURCES.txt` & `pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 src/pyams_app_msc/component/contact/interfaces.py
 src/pyams_app_msc/component/contact/zmi/__init__.py
 src/pyams_app_msc/component/duration/__init__.py
 src/pyams_app_msc/component/duration/interfaces.py
 src/pyams_app_msc/component/duration/schema.py
 src/pyams_app_msc/component/duration/zmi/__init__.py
 src/pyams_app_msc/component/duration/zmi/interfaces.py
+src/pyams_app_msc/component/gallery/__init__.py
+src/pyams_app_msc/component/gallery/zmi/__init__.py
+src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt
+src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt
 src/pyams_app_msc/component/paragraph/__init__.py
 src/pyams_app_msc/component/paragraph/zmi/__init__.py
 src/pyams_app_msc/component/paragraph/zmi/container.py
 src/pyams_app_msc/doctests/README.rst
 src/pyams_app_msc/feature/__init__.py
 src/pyams_app_msc/feature/booking/__init__.py
 src/pyams_app_msc/feature/booking/container.py
```

### Comparing `pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/requires.txt` & `pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/requires.txt`

 * *Files identical despite different names*

