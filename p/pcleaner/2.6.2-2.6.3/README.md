# Comparing `tmp/pcleaner-2.6.2.tar.gz` & `tmp/pcleaner-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-2.6.2.tar", last modified: Wed May  1 23:59:31 2024, max compression
+gzip compressed data, was "pcleaner-2.6.3.tar", last modified: Sun May  5 14:13:45 2024, max compression
```

## Comparing `pcleaner-2.6.2.tar` & `pcleaner-2.6.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.517274 pcleaner-2.6.2/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-2.6.2/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16416 2024-05-01 23:59:31.517274 pcleaner-2.6.2/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14769 2024-05-01 21:30:08.000000 pcleaner-2.6.2/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.407273 pcleaner-2.6.2/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2024-05-01 23:58:10.000000 pcleaner-2.6.2/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23733 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6986 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.410607 pcleaner-2.6.2/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.410607 pcleaner-2.6.2/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.417273 pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.440607 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    59689 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10442 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/ctd_interface.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.447273 pcleaner-2.6.2/pcleaner/data/
--rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-2.6.2/pcleaner/data/LiberationSans-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-2.6.2/pcleaner/data/NotoMono-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-2.6.2/pcleaner/data/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4258 2024-04-17 23:18:42.000000 pcleaner-2.6.2/pcleaner/data/windows_explorer_integration_regedit.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6796 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.463940 pcleaner-2.6.2/pcleaner/gui/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.483940 pcleaner-2.6.2/pcleaner/gui/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5671 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CBadgeButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2642 2024-01-25 04:44:05.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CColorButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4791 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      682 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CDropFrame.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2092 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CElidedLabel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3346 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1150 2024-02-15 00:39:49.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CTextEdit.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1628 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CTooltipLabel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-2.6.2/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1381 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/about_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5547 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/ctd_interface_gui.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2293 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/error_dialog_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10963 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/file_manager_extension_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27366 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14479 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/gui_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    33067 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/image_details_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21465 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/image_file.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4315 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/image_tab.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7561 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/image_viewer.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3591 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/issue_reporter_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6685 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/launcher.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      519 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/license_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3563 2024-02-12 16:50:11.000000 pcleaner-2.6.2/pcleaner/gui/log_parser.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4873 2024-02-12 23:21:16.000000 pcleaner-2.6.2/pcleaner/gui/log_viewer.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    64509 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/mainwindow_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    19431 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/model_downloader_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4648 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/new_profile_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    41984 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/processing.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21373 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/profile_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.493940 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   105176 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   169588 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_theme_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4452 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_themes.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   348275 2024-05-01 22:25:41.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_translations.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   107395 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   175979 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4675 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_themes.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   843082 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_translations.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      956 2024-03-02 00:01:57.000000 pcleaner-2.6.2/pcleaner/gui/setup_greeter_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      559 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/structures.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      701 2024-01-30 21:06:51.000000 pcleaner-2.6.2/pcleaner/gui/supported_languages.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.513940 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2024-02-12 21:19:18.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6619 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_About.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5576 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4481 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13725 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6367 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_IssueReporter.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    41024 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_License.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    49222 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6958 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7411 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_NewProfile.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12580 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5545 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/worker_thread.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8826 2024-05-01 21:35:49.000000 pcleaner-2.6.2/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    32498 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11506 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/inpainting.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    30621 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     9496 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/masker.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7541 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     9207 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/preprocessor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8311 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    22016 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.517274 pcleaner-2.6.2/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16416 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3730 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       90 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      412 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2024-01-09 17:47:58.000000 pcleaner-2.6.2/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1497 2024-05-01 23:59:31.517274 pcleaner-2.6.2/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-2.6.2/setup.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.513940 pcleaner-2.6.2/tests/
--rw-r--r--   0 corbin    (1000) corbin    (1001)      635 2024-02-11 23:18:20.000000 pcleaner-2.6.2/tests/test_log_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.400987 pcleaner-2.6.3/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-2.6.3/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16423 2024-05-05 14:13:45.400987 pcleaner-2.6.3/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14769 2024-05-05 14:12:25.000000 pcleaner-2.6.3/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.390987 pcleaner-2.6.3/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2024-05-05 14:12:43.000000 pcleaner-2.6.3/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23733 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6986 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.394321 pcleaner-2.6.3/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.394321 pcleaner-2.6.3/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.394321 pcleaner-2.6.3/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.394321 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-2.6.3/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    59773 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10442 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.394321 pcleaner-2.6.3/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-2.6.3/pcleaner/data/LiberationSans-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-2.6.3/pcleaner/data/NotoMono-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-2.6.3/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4258 2024-04-17 23:18:42.000000 pcleaner-2.6.3/pcleaner/data/windows_explorer_integration_regedit.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6796 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.397654 pcleaner-2.6.3/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.397654 pcleaner-2.6.3/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5671 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/gui/CustomQ/CBadgeButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2642 2024-01-25 04:44:05.000000 pcleaner-2.6.3/pcleaner/gui/CustomQ/CColorButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4791 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/gui/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      682 2023-10-07 13:58:30.000000 pcleaner-2.6.3/pcleaner/gui/CustomQ/CDropFrame.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2092 2023-10-07 13:58:30.000000 pcleaner-2.6.3/pcleaner/gui/CustomQ/CElidedLabel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3346 2023-10-07 13:58:30.000000 pcleaner-2.6.3/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1150 2024-02-15 00:39:49.000000 pcleaner-2.6.3/pcleaner/gui/CustomQ/CTextEdit.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1628 2023-10-07 13:58:30.000000 pcleaner-2.6.3/pcleaner/gui/CustomQ/CTooltipLabel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-2.6.3/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-2.6.3/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1381 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/gui/about_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5547 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/ctd_interface_gui.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2293 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/gui/error_dialog_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10963 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/file_manager_extension_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27366 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14479 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/gui/gui_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    33067 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/image_details_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21465 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/image_file.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4315 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/image_tab.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7561 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/gui/image_viewer.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3591 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/gui/issue_reporter_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6685 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      519 2023-10-07 13:58:30.000000 pcleaner-2.6.3/pcleaner/gui/license_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3563 2024-02-12 16:50:11.000000 pcleaner-2.6.3/pcleaner/gui/log_parser.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4873 2024-02-12 23:21:16.000000 pcleaner-2.6.3/pcleaner/gui/log_viewer.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    64509 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/mainwindow_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19431 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/gui/model_downloader_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4648 2023-10-07 13:58:30.000000 pcleaner-2.6.3/pcleaner/gui/new_profile_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    41984 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/processing.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21373 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/profile_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.397654 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   105206 2024-05-05 14:13:43.000000 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   169588 2024-05-05 14:13:43.000000 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_theme_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4452 2024-05-05 14:13:43.000000 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_themes.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   348308 2024-05-05 14:13:03.000000 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_translations.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107395 2024-05-02 19:32:19.000000 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_windows_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   175979 2024-05-02 19:32:19.000000 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4675 2024-05-02 19:32:19.000000 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_windows_themes.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   843082 2024-05-02 19:32:19.000000 pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_windows_translations.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      956 2024-03-02 00:01:57.000000 pcleaner-2.6.3/pcleaner/gui/setup_greeter_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      559 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/gui/structures.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      701 2024-01-30 21:06:51.000000 pcleaner-2.6.3/pcleaner/gui/supported_languages.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.400987 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2024-02-12 21:19:18.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6619 2024-05-05 14:13:43.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_About.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5576 2024-05-05 14:13:43.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4481 2024-05-05 14:13:43.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13725 2024-05-05 14:13:43.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6367 2024-05-05 14:13:43.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_IssueReporter.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    41024 2024-05-05 14:13:43.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_License.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    49222 2024-05-05 14:13:44.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6958 2024-05-05 14:13:44.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7411 2024-05-05 14:13:44.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_NewProfile.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12580 2024-05-05 14:13:44.000000 pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5545 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8826 2024-05-01 21:35:49.000000 pcleaner-2.6.3/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    32498 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11506 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/inpainting.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    30621 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     9496 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7541 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     9207 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/preprocessor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8311 2024-04-14 22:05:44.000000 pcleaner-2.6.3/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    22016 2024-05-05 14:12:25.000000 pcleaner-2.6.3/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.400987 pcleaner-2.6.3/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16423 2024-05-05 14:13:45.000000 pcleaner-2.6.3/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3730 2024-05-05 14:13:45.000000 pcleaner-2.6.3/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2024-05-05 14:13:45.000000 pcleaner-2.6.3/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       90 2024-05-05 14:13:45.000000 pcleaner-2.6.3/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      419 2024-05-05 14:13:45.000000 pcleaner-2.6.3/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2024-05-05 14:13:45.000000 pcleaner-2.6.3/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2024-01-09 17:47:58.000000 pcleaner-2.6.3/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1506 2024-05-05 14:13:45.400987 pcleaner-2.6.3/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-2.6.3/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-05 14:13:45.400987 pcleaner-2.6.3/tests/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      635 2024-02-11 23:18:20.000000 pcleaner-2.6.3/tests/test_log_parser.py
```

### Comparing `pcleaner-2.6.2/LICENSE` & `pcleaner-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/PKG-INFO` & `pcleaner-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 2.6.2
+Version: 2.6.3
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -29,15 +29,15 @@
 Requires-Dist: ConfigUpdater
 Requires-Dist: loguru
 Requires-Dist: prettytable
 Requires-Dist: colorama
 Requires-Dist: requests
 Requires-Dist: xdg
 Requires-Dist: tifffile
-Requires-Dist: PySide6
+Requires-Dist: PySide6>=6.7.0
 Requires-Dist: attrs
 Requires-Dist: psutil
 Requires-Dist: dictdiffer
 Requires-Dist: humanfriendly
 Requires-Dist: simple_lama_inpainting
 Requires-Dist: python-magic; platform_system != "Windows"
 Requires-Dist: python-magic-bin; platform_system == "Windows"
```

### Comparing `pcleaner-2.6.2/README.md` & `pcleaner-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/analytics.py` & `pcleaner-2.6.3/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/cli_utils.py` & `pcleaner-2.6.3/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/inference.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-2.6.3/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/config.py` & `pcleaner-2.6.3/pcleaner/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
         # (or VRAM with CUDA) to run multiple models at the same time.
         # This, of course, will increase the speed of the process, but can also
         # crash your computer if you overestimate your hardware.
         # I recommend using 1 model per 2 GB of memory available, or 1 model per 50 images.
         # Note: This is ignored if processing less than 50 files due to the overhead
         # of starting multiple models not being worth it below that.
         # Warning: This may cause program instability, use at your own risk.
+        # DO NOT report issues about this problem, as it's very hardware-dependent!
         concurrent_models = {self.concurrent_models}
         
         """
         detector_conf = cu.ConfigUpdater()
         detector_conf.read_string(multi_left_strip(format_for_version(config_str, gui_mode)))
         general_section = detector_conf["TextDetector"]
         config_updater[add_after_section].add_after.space(2).section(general_section.detach())
```

### Comparing `pcleaner-2.6.2/pcleaner/ctd_interface.py` & `pcleaner-2.6.3/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/data/LiberationSans-Regular.ttf` & `pcleaner-2.6.3/pcleaner/data/LiberationSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/data/NotoMono-Regular.ttf` & `pcleaner-2.6.3/pcleaner/data/NotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/data/windows_explorer_integration_regedit.py` & `pcleaner-2.6.3/pcleaner/data/windows_explorer_integration_regedit.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/denoiser.py` & `pcleaner-2.6.3/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/CustomQ/CBadgeButton.py` & `pcleaner-2.6.3/pcleaner/gui/CustomQ/CBadgeButton.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/CustomQ/CColorButton.py` & `pcleaner-2.6.3/pcleaner/gui/CustomQ/CColorButton.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/CustomQ/CComboBox.py` & `pcleaner-2.6.3/pcleaner/gui/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/CustomQ/CDropFrame.py` & `pcleaner-2.6.3/pcleaner/gui/CustomQ/CDropFrame.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/CustomQ/CElidedLabel.py` & `pcleaner-2.6.3/pcleaner/gui/CustomQ/CElidedLabel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/CustomQ/CTableWidget.py` & `pcleaner-2.6.3/pcleaner/gui/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/CustomQ/CTextEdit.py` & `pcleaner-2.6.3/pcleaner/gui/CustomQ/CTextEdit.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/CustomQ/CTooltipLabel.py` & `pcleaner-2.6.3/pcleaner/gui/CustomQ/CTooltipLabel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/about_driver.py` & `pcleaner-2.6.3/pcleaner/gui/about_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ctd_interface_gui.py` & `pcleaner-2.6.3/pcleaner/gui/ctd_interface_gui.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/error_dialog_driver.py` & `pcleaner-2.6.3/pcleaner/gui/error_dialog_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/file_manager_extension_driver.py` & `pcleaner-2.6.3/pcleaner/gui/file_manager_extension_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/file_table.py` & `pcleaner-2.6.3/pcleaner/gui/file_table.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/gui_utils.py` & `pcleaner-2.6.3/pcleaner/gui/gui_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/image_details_driver.py` & `pcleaner-2.6.3/pcleaner/gui/image_details_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/image_file.py` & `pcleaner-2.6.3/pcleaner/gui/image_file.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/image_tab.py` & `pcleaner-2.6.3/pcleaner/gui/image_tab.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/image_viewer.py` & `pcleaner-2.6.3/pcleaner/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/issue_reporter_driver.py` & `pcleaner-2.6.3/pcleaner/gui/issue_reporter_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/launcher.py` & `pcleaner-2.6.3/pcleaner/gui/launcher.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/license_driver.py` & `pcleaner-2.6.3/pcleaner/gui/license_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/log_parser.py` & `pcleaner-2.6.3/pcleaner/gui/log_parser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/log_viewer.py` & `pcleaner-2.6.3/pcleaner/gui/log_viewer.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/mainwindow_driver.py` & `pcleaner-2.6.3/pcleaner/gui/mainwindow_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/model_downloader_driver.py` & `pcleaner-2.6.3/pcleaner/gui/model_downloader_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/new_profile_driver.py` & `pcleaner-2.6.3/pcleaner/gui/new_profile_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/processing.py` & `pcleaner-2.6.3/pcleaner/gui/processing.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/profile_parser.py` & `pcleaner-2.6.3/pcleaner/gui/profile_parser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_icons.py` & `pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -3067,23 +3067,23 @@
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x05\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00l\x00\x02\x00\x00\x00\x05\x00\x00\x00\x0c\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00z\x00\x02\x00\x00\x00\x05\x00\x00\x00\x07\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x01\x00\x00\x04\x00\x00\x00\x01\x00\x00\x87\xc5\
-\x00\x00\x01\x8f6C[\xe0\
+\x00\x00\x01\x8fI\x19\xcc\x0b\
 \x00\x00\x00\xb6\x00\x00\x00\x00\x00\x01\x00\x00y\x06\
-\x00\x00\x01\x8f6C[\xe0\
+\x00\x00\x01\x8fI\x19\xcc\x0b\
 \x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x80$\
-\x00\x00\x01\x8f6C[\xe0\
+\x00\x00\x01\x8fI\x19\xcc\x0b\
 \x00\x00\x01(\x00\x00\x00\x00\x00\x01\x00\x00\x8c0\
-\x00\x00\x01\x8f6C[\xe0\
+\x00\x00\x01\x8fI\x19\xcc\x0b\
 \x00\x00\x00\x8a\x00\x00\x00\x00\x00\x01\x00\x00qa\
-\x00\x00\x01\x8f6C[\xe0\
+\x00\x00\x01\x8fI\x19\xcc\x0b\
 \x00\x00\x01\x00\x00\x04\x00\x00\x00\x01\x00\x00\xab\xd5\
 \x00\x00\x01\x8b\x0an\xba\x80\
 \x00\x00\x00\xb6\x00\x00\x00\x00\x00\x01\x00\x00\x9d\x16\
 \x00\x00\x01\x8b\x0an\xba\x80\
 \x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\xa44\
 \x00\x00\x01\x8b\x0an\xba\x80\
 \x00\x00\x01(\x00\x00\x00\x00\x00\x01\x00\x00\xb0A\
```

### Comparing `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_theme_icons.py` & `pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_theme_icons.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_themes.py` & `pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_themes.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_translations.py` & `pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_translations.py`

 * *Files 0% similar despite different names*

```diff
@@ -7203,23 +7203,23 @@
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x05\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\xde\x00\x04\x00\x00\x00\x01\x00\x01g\x18\
-\x00\x00\x01\x8f6Ct,\
+\x00\x00\x01\x8fI\x19\xde\x8f\
 \x00\x00\x00\x1e\x00\x04\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x8f6CuK\
+\x00\x00\x01\x8fI\x19\xdfT\
 \x00\x00\x00\xae\x00\x04\x00\x00\x00\x01\x00\x01\x0c\xe5\
-\x00\x00\x01\x8f6Cu\x94\
+\x00\x00\x01\x8fI\x19\xdf\x93\
 \x00\x00\x00N\x00\x04\x00\x00\x00\x01\x00\x00W\xca\
-\x00\x00\x01\x8f6Ct\x83\
+\x00\x00\x01\x8fI\x19\xde\xd2\
 \x00\x00\x00~\x00\x04\x00\x00\x00\x01\x00\x00\xb5\x1e\
-\x00\x00\x01\x8f6Ct\xfb\
+\x00\x00\x01\x8fI\x19\xdf\x11\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_icons.py` & `pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_windows_icons.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py` & `pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_themes.py` & `pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_windows_themes.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_translations.py` & `pcleaner-2.6.3/pcleaner/gui/rc_generated_files/rc_windows_translations.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/setup_greeter_driver.py` & `pcleaner-2.6.3/pcleaner/gui/setup_greeter_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/structures.py` & `pcleaner-2.6.3/pcleaner/gui/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/supported_languages.py` & `pcleaner-2.6.3/pcleaner/gui/supported_languages.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_About.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_About.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_ImageDetails.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_IssueReporter.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_IssueReporter.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_License.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_License.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_Mainwindow.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_NewProfile.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_NewProfile.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py` & `pcleaner-2.6.3/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/gui/worker_thread.py` & `pcleaner-2.6.3/pcleaner/gui/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/helpers.py` & `pcleaner-2.6.3/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/image_ops.py` & `pcleaner-2.6.3/pcleaner/image_ops.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/inpainting.py` & `pcleaner-2.6.3/pcleaner/inpainting.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/main.py` & `pcleaner-2.6.3/pcleaner/main.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/masker.py` & `pcleaner-2.6.3/pcleaner/masker.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/model_downloader.py` & `pcleaner-2.6.3/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/preprocessor.py` & `pcleaner-2.6.3/pcleaner/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/profile_cli.py` & `pcleaner-2.6.3/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner/structures.py` & `pcleaner-2.6.3/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/pcleaner.egg-info/PKG-INFO` & `pcleaner-2.6.3/pcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 2.6.2
+Version: 2.6.3
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -29,15 +29,15 @@
 Requires-Dist: ConfigUpdater
 Requires-Dist: loguru
 Requires-Dist: prettytable
 Requires-Dist: colorama
 Requires-Dist: requests
 Requires-Dist: xdg
 Requires-Dist: tifffile
-Requires-Dist: PySide6
+Requires-Dist: PySide6>=6.7.0
 Requires-Dist: attrs
 Requires-Dist: psutil
 Requires-Dist: dictdiffer
 Requires-Dist: humanfriendly
 Requires-Dist: simple_lama_inpainting
 Requires-Dist: python-magic; platform_system != "Windows"
 Requires-Dist: python-magic-bin; platform_system == "Windows"
```

### Comparing `pcleaner-2.6.2/pcleaner.egg-info/SOURCES.txt` & `pcleaner-2.6.3/pcleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.2/setup.cfg` & `pcleaner-2.6.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 	ConfigUpdater
 	loguru
 	prettytable
 	colorama
 	requests
 	xdg
 	tifffile
-	PySide6
+	PySide6 >= 6.7.0
 	attrs
 	psutil
 	dictdiffer
 	humanfriendly
 	simple_lama_inpainting
 	python-magic; platform_system != "Windows"
 	python-magic-bin; platform_system == "Windows"
```

### Comparing `pcleaner-2.6.2/tests/test_log_parser.py` & `pcleaner-2.6.3/tests/test_log_parser.py`

 * *Files identical despite different names*

