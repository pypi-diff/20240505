# Comparing `tmp/notolog-0.9.0b13.tar.gz` & `tmp/notolog-0.9.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.0b13.tar", last modified: Sat May  4 22:23:05 2024, max compression
+gzip compressed data, was "notolog-0.9.1b0.tar", last modified: Sun May  5 14:52:07 2024, max compression
```

## Comparing `notolog-0.9.0b13.tar` & `notolog-0.9.1b0.tar`

### file list

```diff
@@ -1,405 +1,430 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.164716 notolog-0.9.0b13/
--rw-r--r--   0 vadikus    (501) staff       (20)     3651 2024-05-04 21:27:31.000000 notolog-0.9.0b13/CHANGELOG.md
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.0b13/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      167 2024-05-04 21:37:15.000000 notolog-0.9.0b13/MANIFEST.in
--rw-r--r--   0 vadikus    (501) staff       (20)    17415 2024-05-04 22:23:05.162975 notolog-0.9.0b13/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    15269 2024-05-04 22:15:08.000000 notolog-0.9.0b13/README.md
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.158147 notolog-0.9.0b13/app/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3924 2024-05-04 22:22:23.000000 notolog-0.9.0b13/app/app_config.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.161616 notolog-0.9.0b13/app/assets/
--rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/notolog-example-image.png
--rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/notolog-logo.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.030271 notolog-0.9.0b13/app/assets/themes/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.181461 notolog-0.9.0b13/app/assets/themes/calligraphy/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2187 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6330 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/calligraphy/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.249354 notolog-0.9.0b13/app/assets/themes/default/
--rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/editor.css
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.405262 notolog-0.9.0b13/app/assets/themes/default/icons/
--rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/arrow-clockwise.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/arrow-repeat.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/balloon-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/balloon.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/bandaid-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/bandaid.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/box-arrow-up-right.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/box-arrow-up.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/caret-down-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/caret-up-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/code-slash.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/cursor-text.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/eyedropper.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/eyeglasses.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/file-earmark-lock2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/file-earmark-plus-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/file-earmark-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/file-earmark.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/filetype-html.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/filetype-md.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/filetype-txt.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/floppy2-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/floppy2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/folder-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/folder-symlink.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/folder.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/github.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/link-45deg.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/linkedin.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/pencil-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/power.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/quote.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/robot.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/share-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/shield-lock-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/shield-lock.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/star-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/star.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/three-dots.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/trash3-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/trash3.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/twitter-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/type-bold.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/type-italic.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/type-strikethrough.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/type-underline.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/x-circle-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/x-square-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/icons/x-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7980 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/default/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.429604 notolog-0.9.0b13/app/assets/themes/noir_dark/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6433 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/noir_dark/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.484546 notolog-0.9.0b13/app/assets/themes/strawberry/
--rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      771 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7963 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/assets/themes/strawberry/viewer.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.499079 notolog-0.9.0b13/app/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3247 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/encrypt/enc_password_reset_dialog.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.504527 notolog-0.9.0b13/app/enums/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/enums/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1855 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/enums/ai_model_names.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6229 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/enums/colors.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1388 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/enums/languages.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1365 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/enums/themes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3236 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/etree_extension.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.506568 notolog-0.9.0b13/app/exceptions/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/exceptions/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/exceptions/file_header_empty_exception.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7388 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.511992 notolog-0.9.0b13/app/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2730 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-04 21:27:31.000000 notolog-0.9.0b13/app/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.516698 notolog-0.9.0b13/app/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9027 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    48888 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/highlight/view_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9589 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/image_downloader.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.518600 notolog-0.9.0b13/app/lexemes/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/__init__.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.521001 notolog-0.9.0b13/app/lexemes/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      160 2024-05-04 21:42:24.000000 notolog-0.9.0b13/app/lexemes/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3224 2024-05-04 21:42:24.000000 notolog-0.9.0b13/app/lexemes/__pycache__/lexemes.cpython-39.pyc
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.536160 notolog-0.9.0b13/app/lexemes/de/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.544220 notolog-0.9.0b13/app/lexemes/de/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6854 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5899 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2183 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2914 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1272 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2730 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6579 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/de/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.556289 notolog-0.9.0b13/app/lexemes/en/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.563597 notolog-0.9.0b13/app/lexemes/en/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:55:13.000000 notolog-0.9.0b13/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6663 2024-05-04 21:55:13.000000 notolog-0.9.0b13/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5462 2024-05-04 21:55:13.000000 notolog-0.9.0b13/app/lexemes/en/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2086 2024-05-04 21:55:13.000000 notolog-0.9.0b13/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3470 2024-05-04 21:55:13.000000 notolog-0.9.0b13/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1243 2024-05-04 21:55:13.000000 notolog-0.9.0b13/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2495 2024-05-04 21:55:13.000000 notolog-0.9.0b13/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/en/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/en/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6044 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/en/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/en/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/en/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/en/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/en/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.612478 notolog-0.9.0b13/app/lexemes/es/
--rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/es/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/es/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6549 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/es/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/es/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/es/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/es/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/es/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.619796 notolog-0.9.0b13/app/lexemes/fr/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.632602 notolog-0.9.0b13/app/lexemes/fr/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6899 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6212 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2256 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3928 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1274 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2794 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6709 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/fr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.657765 notolog-0.9.0b13/app/lexemes/ge/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.671890 notolog-0.9.0b13/app/lexemes/ge/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1355 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)    10384 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     9053 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ge/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3389 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5710 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1642 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     4138 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ge/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ge/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9721 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ge/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ge/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ge/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ge/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ge/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.681010 notolog-0.9.0b13/app/lexemes/gr/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.688546 notolog-0.9.0b13/app/lexemes/gr/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1172 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8982 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8175 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/gr/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2804 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5014 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1528 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3735 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/lexemes/gr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/lexemes/gr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8654 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/gr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/lexemes/gr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/gr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/lexemes/gr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/gr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.739711 notolog-0.9.0b13/app/lexemes/in/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.749139 notolog-0.9.0b13/app/lexemes/in/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     9403 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     9416 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3029 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5585 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1618 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10062 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/in/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.767691 notolog-0.9.0b13/app/lexemes/it/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.789495 notolog-0.9.0b13/app/lexemes/it/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      930 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6824 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5639 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2188 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2925 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1290 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2700 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6359 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/it/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.811082 notolog-0.9.0b13/app/lexemes/ja/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.860374 notolog-0.9.0b13/app/lexemes/ja/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1020 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8452 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6837 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2411 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     4046 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1301 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3047 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7241 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ja/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.881352 notolog-0.9.0b13/app/lexemes/ko/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.911597 notolog-0.9.0b13/app/lexemes/ko/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      954 2024-05-04 21:28:24.000000 notolog-0.9.0b13/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     7562 2024-05-04 21:28:24.000000 notolog-0.9.0b13/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6404 2024-05-04 21:28:24.000000 notolog-0.9.0b13/app/lexemes/ko/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2277 2024-05-04 21:28:24.000000 notolog-0.9.0b13/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3723 2024-05-04 21:28:24.000000 notolog-0.9.0b13/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1285 2024-05-04 21:28:24.000000 notolog-0.9.0b13/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:28:24.000000 notolog-0.9.0b13/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ko/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ko/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6765 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ko/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ko/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ko/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ko/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/ko/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:04.926763 notolog-0.9.0b13/app/lexemes/la/
--rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/la/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/la/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6236 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/la/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/la/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/la/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/la/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/la/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/lexemes.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.011620 notolog-0.9.0b13/app/lexemes/pt/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/pt/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/pt/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6347 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/pt/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/pt/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/pt/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/pt/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/pt/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.023795 notolog-0.9.0b13/app/lexemes/ru/
--rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ru/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ru/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7931 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ru/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ru/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ru/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ru/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/ru/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.041009 notolog-0.9.0b13/app/lexemes/tr/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.056026 notolog-0.9.0b13/app/lexemes/tr/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      912 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     7114 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5741 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2272 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3751 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1297 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6147 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:27:29.000000 notolog-0.9.0b13/app/lexemes/tr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.065483 notolog-0.9.0b13/app/lexemes/zh/
--rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/zh/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/zh/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5770 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/zh/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/zh/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/zh/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/zh/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-04 21:27:28.000000 notolog-0.9.0b13/app/lexemes/zh/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)   175532 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.122501 notolog-0.9.0b13/app/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:26.000000 notolog-0.9.0b13/app/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8280 2024-05-04 21:27:26.000000 notolog-0.9.0b13/app/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-05-04 21:27:26.000000 notolog-0.9.0b13/app/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-05-04 21:27:26.000000 notolog-0.9.0b13/app/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3520 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-05-04 21:27:26.000000 notolog-0.9.0b13/app/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2712 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    37330 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6896 2024-05-04 21:27:26.000000 notolog-0.9.0b13/app/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)    12713 2024-05-04 21:27:27.000000 notolog-0.9.0b13/app/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:26.000000 notolog-0.9.0b13/app/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-04 21:27:30.000000 notolog-0.9.0b13/app/view_widget.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.127764 notolog-0.9.0b13/docs/
--rw-r--r--   0 vadikus    (501) staff       (20)     8625 2024-05-04 21:27:32.000000 notolog-0.9.0b13/docs/Examples.md
--rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.0b13/docs/notolog-ui-settings.png
--rw-r--r--   0 vadikus    (501) staff       (20)     2702 2024-05-04 21:27:41.000000 notolog-0.9.0b13/main.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.161456 notolog-0.9.0b13/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    17415 2024-05-04 22:23:03.000000 notolog-0.9.0b13/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    13447 2024-05-04 22:23:03.000000 notolog-0.9.0b13/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-04 22:23:03.000000 notolog-0.9.0b13/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-04 22:23:03.000000 notolog-0.9.0b13/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-05-04 22:23:03.000000 notolog-0.9.0b13/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       15 2024-05-04 22:23:03.000000 notolog-0.9.0b13/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-05-04 21:27:31.000000 notolog-0.9.0b13/requirements.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-04 22:23:05.164924 notolog-0.9.0b13/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     2167 2024-05-04 22:22:23.000000 notolog-0.9.0b13/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 22:23:05.157337 notolog-0.9.0b13/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.0b13/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5975 2024-05-04 21:27:31.000000 notolog-0.9.0b13/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2305 2024-05-04 21:27:32.000000 notolog-0.9.0b13/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9197 2024-05-04 21:27:32.000000 notolog-0.9.0b13/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3962 2024-05-04 21:27:31.000000 notolog-0.9.0b13/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5810 2024-05-04 21:27:31.000000 notolog-0.9.0b13/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5823 2024-05-04 21:27:31.000000 notolog-0.9.0b13/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1154 2024-05-04 21:27:32.000000 notolog-0.9.0b13/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4971 2024-05-04 21:27:32.000000 notolog-0.9.0b13/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4464 2024-05-04 21:27:32.000000 notolog-0.9.0b13/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6222 2024-05-04 21:27:32.000000 notolog-0.9.0b13/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.029801 notolog-0.9.1b0/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4751 2024-05-05 14:33:15.000000 notolog-0.9.1b0/CHANGELOG.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b0/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      191 2024-05-05 14:33:15.000000 notolog-0.9.1b0/MANIFEST.in
+-rw-r--r--   0 vadikus    (501) staff       (20)    18015 2024-05-05 14:52:07.027689 notolog-0.9.1b0/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    15870 2024-05-05 14:33:15.000000 notolog-0.9.1b0/README.md
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.603522 notolog-0.9.1b0/app/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4777 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/app_config.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.605430 notolog-0.9.1b0/app/assets/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/notolog-example-image.png
+-rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/notolog-logo.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.571156 notolog-0.9.1b0/app/assets/themes/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.620631 notolog-0.9.1b0/app/assets/themes/calligraphy/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2187 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6330 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.635281 notolog-0.9.1b0/app/assets/themes/default/
+-rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/editor.css
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.686332 notolog-0.9.1b0/app/assets/themes/default/icons/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/arrow-clockwise.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/arrow-repeat.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/balloon-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/balloon.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/bandaid-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/bandaid.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/box-arrow-up-right.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/box-arrow-up.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/caret-down-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/caret-up-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/code-slash.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/cursor-text.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/eyedropper.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/eyeglasses.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/file-earmark-lock2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/file-earmark-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/file-earmark.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/filetype-html.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/filetype-md.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/filetype-txt.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/floppy2-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/floppy2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/folder-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/folder-symlink.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/folder.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/github.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/link-45deg.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/linkedin.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/pencil-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/power.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/quote.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/robot.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/share-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/shield-lock-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/shield-lock.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/star-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/star.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/three-dots.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/trash3-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/trash3.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/twitter-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/type-bold.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/type-italic.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/type-strikethrough.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/type-underline.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/x-circle-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/x-square-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/x-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7980 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.697229 notolog-0.9.1b0/app/assets/themes/noir_dark/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6433 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.712332 notolog-0.9.1b0/app/assets/themes/strawberry/
+-rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      771 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7963 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/viewer.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.724840 notolog-0.9.1b0/app/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4337 2024-05-05 14:40:40.000000 notolog-0.9.1b0/app/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6076 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4172 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3211 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.732733 notolog-0.9.1b0/app/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1876 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6158 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1470 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1386 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3236 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.733723 notolog-0.9.1b0/app/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.739524 notolog-0.9.1b0/app/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4227 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.744935 notolog-0.9.1b0/app/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9027 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    48888 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/highlight/view_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9600 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/image_downloader.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.747525 notolog-0.9.1b0/app/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/__init__.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.750002 notolog-0.9.1b0/app/lexemes/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      160 2024-05-04 21:42:24.000000 notolog-0.9.1b0/app/lexemes/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3224 2024-05-05 14:44:43.000000 notolog-0.9.1b0/app/lexemes/__pycache__/lexemes.cpython-39.pyc
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.757090 notolog-0.9.1b0/app/lexemes/de/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.764205 notolog-0.9.1b0/app/lexemes/de/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6854 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5899 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2183 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2914 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1272 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2730 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6579 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.778370 notolog-0.9.1b0/app/lexemes/en/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.786332 notolog-0.9.1b0/app/lexemes/en/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6663 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5462 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2086 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3470 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1243 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2495 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6044 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.793193 notolog-0.9.1b0/app/lexemes/es/
+-rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6549 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.801668 notolog-0.9.1b0/app/lexemes/fi/
+-rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6284 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.808184 notolog-0.9.1b0/app/lexemes/fr/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.815721 notolog-0.9.1b0/app/lexemes/fr/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6899 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6212 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2256 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3928 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1274 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2794 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6709 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.829335 notolog-0.9.1b0/app/lexemes/ge/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.837231 notolog-0.9.1b0/app/lexemes/ge/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1355 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)    10384 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     9053 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3389 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5710 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1642 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     4138 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9721 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.844850 notolog-0.9.1b0/app/lexemes/gr/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.855987 notolog-0.9.1b0/app/lexemes/gr/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1172 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8982 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8175 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2804 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5014 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1528 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3735 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8654 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.861966 notolog-0.9.1b0/app/lexemes/in/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.870851 notolog-0.9.1b0/app/lexemes/in/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     9403 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     9416 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3029 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5585 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1618 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10062 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.882984 notolog-0.9.1b0/app/lexemes/it/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.889821 notolog-0.9.1b0/app/lexemes/it/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      930 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6824 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5639 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2188 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2925 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1290 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2700 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6359 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.896330 notolog-0.9.1b0/app/lexemes/ja/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.903427 notolog-0.9.1b0/app/lexemes/ja/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1020 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8452 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6837 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2411 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     4046 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1301 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3047 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7241 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.909112 notolog-0.9.1b0/app/lexemes/ko/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.915635 notolog-0.9.1b0/app/lexemes/ko/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      954 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     7562 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6404 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2277 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3723 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1285 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6765 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.927248 notolog-0.9.1b0/app/lexemes/la/
+-rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6236 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/lexemes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.935376 notolog-0.9.1b0/app/lexemes/pt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6347 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.941882 notolog-0.9.1b0/app/lexemes/ru/
+-rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7931 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.950917 notolog-0.9.1b0/app/lexemes/se/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.957197 notolog-0.9.1b0/app/lexemes/se/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      912 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6826 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5756 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2125 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3568 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1275 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2574 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6246 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.963809 notolog-0.9.1b0/app/lexemes/tr/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.974534 notolog-0.9.1b0/app/lexemes/tr/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      912 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     7114 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5741 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2272 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3751 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1297 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6147 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.983125 notolog-0.9.1b0/app/lexemes/zh/
+-rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5770 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   175569 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.002594 notolog-0.9.1b0/app/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8224 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16816 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2099 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3509 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6999 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2610 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    37283 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3197 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    12655 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:26.000000 notolog-0.9.1b0/app/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/view_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       87 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app_config.toml
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.004956 notolog-0.9.1b0/docs/
+-rw-r--r--   0 vadikus    (501) staff       (20)     8621 2024-05-05 14:47:11.000000 notolog-0.9.1b0/docs/Examples.md
+-rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b0/docs/notolog-ui-settings.png
+-rw-r--r--   0 vadikus    (501) staff       (20)     2770 2024-05-05 14:33:15.000000 notolog-0.9.1b0/main.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.025968 notolog-0.9.1b0/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    18015 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    14261 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       15 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-05-05 14:33:15.000000 notolog-0.9.1b0/requirements.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-05 14:52:07.030211 notolog-0.9.1b0/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2166 2024-05-05 14:33:15.000000 notolog-0.9.1b0/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.024292 notolog-0.9.1b0/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5975 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2305 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9880 2024-05-05 14:33:15.000000 notolog-0.9.1b0/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3962 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5810 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5823 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1154 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4971 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4464 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6222 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_themes.py
```

### Comparing `notolog-0.9.0b13/CHANGELOG.md` & `notolog-0.9.1b0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 # Changelog
 All notologable changes to this project will be documented in this file.
 
+## [0.9.1b0] - 2024-05-05
+### Added
+- New interface languages: Finnish and Swedish, expanding accessibility for users in these regions.
+- Additional entries to the `.gitignore` and `.gitattributes` files to improve version control practices.
+- A dedicated `app_config.toml` file with initial configuration parameters, simplifying initial setup and customization.
+
+### Updated
+- Updated the `Libraries and Licenses` section within the README.md file to provide comprehensive information about third-party dependencies and their licenses.
+- Updated `cryptography` to version 42.0.6 and `Pygments` to version 2.18.0 to ensure compatibility with the latest standards and to incorporate the newest features and security enhancements.
+
+### Changed
+- Modified file handling: The file header can now be the only content of the file, streamlining setups where minimal data is required.
+- Updated encryption description to clarify that Fernet uses AES-128 for encryption, derived from a 256-bit key, accurately reflecting the cryptographic standards employed.
+
 ## [0.9.0b11] - 2024-05-04
 ### Added
 - Support for embedding external images within documents, with caching.
 - Option to auto-save downloaded image resources on local disk and reuse them in subsequent document sessions.
 - New interface languages: Greek, Hindi, Turkish.
 - Expanded example content and resources.
 - Added `CHANGELOG.md` to document all notable changes to the project, enhancing transparency and trackability for developers and users alike.
 
+### Updated
+- Updated pytest to version 8.2.0 to take advantage of improved test suite performance and new features. (Previously listed under "Changed")
+
 ### Changed
 - Updated pip installer related packages and file structure.
 - Current directory now persists during file events, even if no files are actively open.
 - Minor logo adjustment.
-- Updated pytest to version 8.2.0 to take advantage of improved test suite performance and new features.
 
 ### Fixed
 - Resolved sudden crashes when switching between edit and view modes.
 - Addressed UI style issues for improved text visibility under various color schemes.
 
 ## [0.9.0b10] - 2024-04-29
-### Fixed
-- Corrected startup failures following pip installation.
-
 ### Changed
 - Updated pip installer related packages and file structure.
 
+### Fixed
+- Corrected startup failures following pip installation.
+
 ## [0.9.0b0] - 2024-04-29
 ### Added
 - Initial release features, open sourced under the MIT license for full transparency and collaboration.
 - Markdown syntax highlighting:
     - Editor mode offers smooth highlighting tailored specifically for Notolog by our development team, including line numbers and extended syntax highlighting.
     - View mode utilizes the Python Markdown library for seamless rendering of Markdown syntax.
     - Supports multi-line block open-close tokens for enhanced readability and structure.
```

### Comparing `notolog-0.9.0b13/LICENSE` & `notolog-0.9.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/PKG-INFO` & `notolog-0.9.1b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b13
+Version: 0.9.1b0
 Summary: Notolog Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Keywords: notolog,ai,markdown,editor
@@ -30,54 +30,50 @@
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi==1.16.0
 Requires-Dist: click==8.1.7
-Requires-Dist: cryptography==42.0.5
+Requires-Dist: cryptography==42.0.6
 Requires-Dist: emoji==2.11.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: Markdown==3.6
 Requires-Dist: packaging==24.0
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pycparser==2.22
-Requires-Dist: Pygments==2.17.2
+Requires-Dist: Pygments==2.18.0
 Requires-Dist: PySide6==6.7.0
 Requires-Dist: PySide6_Addons==6.7.0
 Requires-Dist: PySide6_Essentials==6.7.0
 Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: qasync==0.27.1
 Requires-Dist: qt6-applications==6.5.0.2.3
 Requires-Dist: qt6-tools==6.5.0.1.3
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-04 22:22:51.958596"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-05 15:21:52.653006"}} -->
 # Notolog
 
 ![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
 
 ## Overview
 
-Notolog is a markdown editor crafted in Python and Qt, offered as an open-source solution.
-
-In short, I was in search of a simple, lightweight, and cross-platform editor to fulfill my daily needs as a software developer. Concurrently, I aimed to deepen my understanding of Python, leading me to embark on creating my own editor. Thus, the Notolog editor was born.
-
-The editor has no aim but the path, hence its proof-of-concept nature and many tasks yet to be completed. Speaking of tasks, the editor features special highlighting for the word 'TODO'; simply type it with '@', like '@todo something', and see what happens.
+Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
 
 ---
 ![Notolog settings UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
 
 
 ## Features
 
-* Open sourced under the MIT license for full transparency and collaboration.
+* Notolog is open-sourced under the MIT license, promoting full transparency and encouraging collaboration.
 * Markdown syntax highlighting:
 	* Editor mode offers smooth highlighting tailored specifically for Notolog, with line numbers and extended syntax highlighting.
 	* View mode utilizes the Python Markdown library for seamless rendering of Markdown syntax.
 	* Supports multi-line block open-close tokens for improved readability and structure.
 * Multi-platform support: Compatible with all major platforms where Python is installed, ensuring accessibility across operating systems.
 * Accessible features, including:
 	* Clear and accessible descriptions for enhanced usability.
@@ -85,31 +81,32 @@
 * Background and cross-action save changes experience:
 	* Automatically saves changes in the background to ensure data integrity and minimize user intervention.
 	* Seamlessly handles unsaved changes when performing cross-actions, providing a smooth user experience.
 * Search functionality:
 	* Allows users to search within the opened file.
 	* Quick search by file name within the tree, enabling efficient navigation and content retrieval.
 * File meta-headers in the form of HTML comments to avoid excess visibility.
-* Password-based file symmetric encryption and decryption:
-	* Employing AES-256 in CBC mode (Cipher Block Chaining) with the power of the Fernet library.
-	* Key derivation based on a 256-bit key using PBKDF2HMAC from the cryptography library, using SHA-256 as the hash function.
-	* Fernet provides an easy-to-use and secure way of performing symmetric (also known as "secret key") encryption.
-	* File meta-headers to keep encryption params to allow a seamless decryption process.
+* Password-based File Encryption and Decryption:
+	* Utilizes Fernet for encryption, providing a secure and user-friendly method for symmetric (also known as "secret key") encryption.
+	* Fernet employs AES-128 in CBC mode. Plans to introduce AES-256 in future updates are aimed at further enhancing security.
+* File Meta-Headers:
+	* Notolog implements file meta-headers to store encryption parameters, ensuring a seamless decryption process.
 * Translations-friendly file structure:
 	* Supports several languages out of the box, with provisions for adding and supporting additional languages.
 * Color themes support:
 	* Comes with a few predefined color themes to customize the editor's appearance, for both light and dark modes.
 * Hotkeys support:
 	* It currently supports hotkeys like Ctrl+S for saving and Ctrl+F for searching, with plans for further expansion.
 * In-line context menus:
 	* Right-click context menu options in the file tree for file rename and delete actions.
 	* Customizable toolbar with right-click functionality to show/hide icons based on user preferences.
 * Includes a suite of unit tests to ensure code reliability and maintainability, providing confidence in the editor's functionality.
 * AI Assistant UI to get all things you need in one place:
 	* At the moment the OpenAI API is supported with plans to extend support with other providers.
+* Notolog includes specialized highlighting for TODOs. Simply type '@todo something' to mark tasks, enhancing the ability to track and manage future plans efficiently.
 
 There is no classical web engine integration to make overall package more lightweight and to achieve the best possible performance.
 
 
 ## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
@@ -233,57 +230,67 @@
 notolog\Scripts\activate
 ```
 _Mind the environment name (**notolog** or any other selected before)._
 
 
 ## Contributing
 
-If you encounter any issues or would like to contribute to the project, please don't hesitate to open an issue or submit a pull request on GitHub.
+If you encounter any issues or would like to contribute to the project, please don't hesitate to [open an issue](https://github.com/notolog/notolog-editor/issues) or submit a [pull request](https://github.com/notolog/notolog-editor/pulls) on the project's [GitHub page](https://github.com/notolog/notolog-editor).
 
 ## License
 
 The Notolog project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Third-Party Components
 
-### Libraries and Dependencies
+### Libraries and Licenses
+
+This project utilizes numerous third-party libraries, each with its own licensing terms. Below is a detailed list of these libraries grouped by license type to help clarify what each license permits and requires. This categorization aids in ensuring compliance with legal terms for use, modification, and distribution of these software components.
+
+#### GNU LGPLv3, GNU GPLv2, or Commercial License
+
+- **Qt (open-source)**: Framework for graphical user interfaces and more. [Project Details](https://www.qt.io), [Qt Licensing](https://www.qt.io/licensing)
+- **PySide6**: GUI creation with Qt6 in Python. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6/)
+- **PySide6_Addons**: Additional modules for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Addons/)
+- **PySide6_Essentials**: Core libraries for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Essentials/)
+- **shiboken6**: Binding generator for Qt framework. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/shiboken6/)
+
+#### MIT License
 
-This project utilizes the following third-party libraries:
+- **Bootstrap Icons**: Icons for UI elements. [Project Details](https://icons.getbootstrap.com/), [License Details](https://github.com/twbs/icons/blob/main/LICENSE)
+- **pytest**: Used for unit testing. It provides powerful features like fixtures, assertions, and test parameterization to facilitate writing and running Python tests. [Project Details](https://pytest.org/), [License Details](https://docs.pytest.org/en/8.0.x/license.html)
+- **pytest-mock**: Enhances pytest for unit tests by offering a simple interface to powerful mocking functionalities. [License Details](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/)
+- **cffi**: Used for interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
+- **iniconfig**: For parsing and working with INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
+- **tomli**: A Python library used for parsing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
+- **pluggy**: For creating and managing plugin systems in Python applications. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
 
-* Qt (open-source): Distributed under the GNU LGPLv3, GNU GPLv2, or Qt Commercial License. ([Qt Licensing](https://www.qt.io/licensing))
-* PySide6: Used for creating graphical user interfaces with Qt6 in Python. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/PySide6/))
-	* PySide6_Addons: Additional modules and utilities for PySide6 to enhance functionality. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/PySide6-Addons/))
-	* PySide6_Essentials: Essential components and tools for PySide6 development, including core libraries and resources. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/PySide6-Essentials/))
-* shiboken6: A Python binding generator used in conjunction with PySide6 to create Python bindings for the Qt framework. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/shiboken6/))
-* Python-Markdown: Used for Markdown to HTML conversion. ([The 3-Clause BSD License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md))
-* Emoji library: Used for converting emoji code to real emoji. ([New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt))
-* qasync: Used for handling async syntax highlighting. ([BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE))
-* cryptography: Used for generating cryptographic hashes and keys in this project is dual-licensed under the:
-	* ([Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
-	* ([BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD))
-* Bootstrap Icons: Used for UI toolbar icons and other visual elements. ([The MIT License (MIT)](https://github.com/twbs/icons/blob/main/LICENSE))
-* pytest: Used for testing. ([The MIT License (MIT)](https://docs.pytest.org/en/8.0.x/license.html))
-* pytest-mock: Used for testing. ([The MIT License (MIT)](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE))
-* asyncio: Used for handling async syntax highlighting is part of the Python standard library, which typically falls under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license).
-* cffi: Used for interfacing with C code. ([The MIT License (MIT)](https://github.com/python-cffi/cffi/blob/main/LICENSE))
-* click: Used for creating command-line interfaces. ([BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/))
-* iniconfig: Used for parsing and working with INI configuration files. ([The MIT License (MIT)](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE))
-* packaging: Used for working with Python package metadata and distribution utilities is dual-licensed under the:
-	* ([Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE))
-	* ([BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD))
-* tomli: A Python library used for parsing TOML configuration files effortlessly. ([The MIT License (MIT)](https://github.com/hukkin/tomli/blob/master/LICENSE))
-* pluggy: Used for creating and managing plugin systems in Python applications. ([The MIT License (MIT)](https://github.com/pytest-dev/pluggy/blob/main/LICENSE))
-* pycparser: Used for parsing C code and generating Abstract Syntax Trees (AST) in Python. ([BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE))
-* Pygments: Used for syntax highlighting source code in various programming languages. ([BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE))
+#### BSD Licenses
 
-Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Please refer to the documentation of each library for information about its license and terms of use.
+- **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
+- **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
+- **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
+- **Pygments**: Syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
+- **click**: Used for creating command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
+- **pycparser**: C code parser and for generating Abstract Syntax Trees (AST) in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
 
-This project includes code from external sources that are licensed under The Unlicense. We acknowledge and thank the original authors for their contributions.
+#### Other Dual Licensed
 
-* [Examples of codehilite CSS themes](https://github.com/richleland/pygments-css): Used to create color themes for code block highlighting. ([The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt))
+- **cryptography**: Provides cryptographic functions and primitives. [Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE) and [BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/cryptography/)
+- **packaging**: Python package metadata and distribution utilities. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
+
+#### Python Standard Library
+
+- **asyncio**: Part of the Python standard library, licensed under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license).
+
+#### The Unlicense
+
+- **Codehilite CSS Themes**: Base themes for code highlighting. [The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt)
+
+Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Always refer to the documentation of each library for detailed information about its license and terms of use.
 
 ### APIs
 
 #### OpenAI API Disclaimer
 
 **Disclaimer:** This project is independent and neither affiliated with, endorsed by, nor sponsored by OpenAI. Integration of the OpenAI API in this project is provided on an "as is" basis, without any official partnership or endorsement by OpenAI. The creators of this project disclaim all liability for any misuse, harm, or other consequences resulting from the use of the OpenAI API.
 
@@ -293,17 +300,15 @@
 
 **Security:** It is crucial for users to manage their API keys securely, ensuring they are not exposed or shared in public forums.
 
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
 ## Security Disclaimer
 
-This application, primarily designed for educational purposes, employs PBKDF2HMAC for key derivation and AES-256 in CBC mode for encryption, using a 256-bit key. Note that the encryption salt and iteration counts are stored unencrypted in the file's header. While secure for educational and non-critical uses, this setup may not meet the highest security standards. Users can opt to add a password hint in the file header, which should be used judiciously to balance convenience against security risks.
-
-As an educational tool, this software is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws. The developers disclaim liability for misuse or for ensuring legal compliance.
+This application is primarily designed for educational purposes and uses PBKDF2HMAC for key derivation. It employs Fernet, which utilizes AES-128 in CBC mode. The key is initially created at 256 bits but truncated to 128 bits for encryption. The encryption salt and iteration counts are stored unencrypted in the file's header, making this setup suitable for educational and non-critical applications only. As such, while this software provides basic security, it is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws, and the developers disclaim liability for misuse or legal non-compliance.
 
 ---
 
 `░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
 `╔═══════════════════════════════════════════════════════════════════════════════════════════╗`
 `║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
 `╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
```

### Comparing `notolog-0.9.0b13/README.md` & `notolog-0.9.1b0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-04 22:22:51.958596"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-05 15:21:52.653006"}} -->
 # Notolog
 
 ![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
 
 ## Overview
 
-Notolog is a markdown editor crafted in Python and Qt, offered as an open-source solution.
-
-In short, I was in search of a simple, lightweight, and cross-platform editor to fulfill my daily needs as a software developer. Concurrently, I aimed to deepen my understanding of Python, leading me to embark on creating my own editor. Thus, the Notolog editor was born.
-
-The editor has no aim but the path, hence its proof-of-concept nature and many tasks yet to be completed. Speaking of tasks, the editor features special highlighting for the word 'TODO'; simply type it with '@', like '@todo something', and see what happens.
+Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
 
 ---
 ![Notolog settings UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
 
 
 ## Features
 
-* Open sourced under the MIT license for full transparency and collaboration.
+* Notolog is open-sourced under the MIT license, promoting full transparency and encouraging collaboration.
 * Markdown syntax highlighting:
 	* Editor mode offers smooth highlighting tailored specifically for Notolog, with line numbers and extended syntax highlighting.
 	* View mode utilizes the Python Markdown library for seamless rendering of Markdown syntax.
 	* Supports multi-line block open-close tokens for improved readability and structure.
 * Multi-platform support: Compatible with all major platforms where Python is installed, ensuring accessibility across operating systems.
 * Accessible features, including:
 	* Clear and accessible descriptions for enhanced usability.
@@ -29,31 +25,32 @@
 * Background and cross-action save changes experience:
 	* Automatically saves changes in the background to ensure data integrity and minimize user intervention.
 	* Seamlessly handles unsaved changes when performing cross-actions, providing a smooth user experience.
 * Search functionality:
 	* Allows users to search within the opened file.
 	* Quick search by file name within the tree, enabling efficient navigation and content retrieval.
 * File meta-headers in the form of HTML comments to avoid excess visibility.
-* Password-based file symmetric encryption and decryption:
-	* Employing AES-256 in CBC mode (Cipher Block Chaining) with the power of the Fernet library.
-	* Key derivation based on a 256-bit key using PBKDF2HMAC from the cryptography library, using SHA-256 as the hash function.
-	* Fernet provides an easy-to-use and secure way of performing symmetric (also known as "secret key") encryption.
-	* File meta-headers to keep encryption params to allow a seamless decryption process.
+* Password-based File Encryption and Decryption:
+	* Utilizes Fernet for encryption, providing a secure and user-friendly method for symmetric (also known as "secret key") encryption.
+	* Fernet employs AES-128 in CBC mode. Plans to introduce AES-256 in future updates are aimed at further enhancing security.
+* File Meta-Headers:
+	* Notolog implements file meta-headers to store encryption parameters, ensuring a seamless decryption process.
 * Translations-friendly file structure:
 	* Supports several languages out of the box, with provisions for adding and supporting additional languages.
 * Color themes support:
 	* Comes with a few predefined color themes to customize the editor's appearance, for both light and dark modes.
 * Hotkeys support:
 	* It currently supports hotkeys like Ctrl+S for saving and Ctrl+F for searching, with plans for further expansion.
 * In-line context menus:
 	* Right-click context menu options in the file tree for file rename and delete actions.
 	* Customizable toolbar with right-click functionality to show/hide icons based on user preferences.
 * Includes a suite of unit tests to ensure code reliability and maintainability, providing confidence in the editor's functionality.
 * AI Assistant UI to get all things you need in one place:
 	* At the moment the OpenAI API is supported with plans to extend support with other providers.
+* Notolog includes specialized highlighting for TODOs. Simply type '@todo something' to mark tasks, enhancing the ability to track and manage future plans efficiently.
 
 There is no classical web engine integration to make overall package more lightweight and to achieve the best possible performance.
 
 
 ## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
@@ -177,57 +174,67 @@
 notolog\Scripts\activate
 ```
 _Mind the environment name (**notolog** or any other selected before)._
 
 
 ## Contributing
 
-If you encounter any issues or would like to contribute to the project, please don't hesitate to open an issue or submit a pull request on GitHub.
+If you encounter any issues or would like to contribute to the project, please don't hesitate to [open an issue](https://github.com/notolog/notolog-editor/issues) or submit a [pull request](https://github.com/notolog/notolog-editor/pulls) on the project's [GitHub page](https://github.com/notolog/notolog-editor).
 
 ## License
 
 The Notolog project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Third-Party Components
 
-### Libraries and Dependencies
+### Libraries and Licenses
+
+This project utilizes numerous third-party libraries, each with its own licensing terms. Below is a detailed list of these libraries grouped by license type to help clarify what each license permits and requires. This categorization aids in ensuring compliance with legal terms for use, modification, and distribution of these software components.
+
+#### GNU LGPLv3, GNU GPLv2, or Commercial License
+
+- **Qt (open-source)**: Framework for graphical user interfaces and more. [Project Details](https://www.qt.io), [Qt Licensing](https://www.qt.io/licensing)
+- **PySide6**: GUI creation with Qt6 in Python. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6/)
+- **PySide6_Addons**: Additional modules for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Addons/)
+- **PySide6_Essentials**: Core libraries for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Essentials/)
+- **shiboken6**: Binding generator for Qt framework. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/shiboken6/)
+
+#### MIT License
 
-This project utilizes the following third-party libraries:
+- **Bootstrap Icons**: Icons for UI elements. [Project Details](https://icons.getbootstrap.com/), [License Details](https://github.com/twbs/icons/blob/main/LICENSE)
+- **pytest**: Used for unit testing. It provides powerful features like fixtures, assertions, and test parameterization to facilitate writing and running Python tests. [Project Details](https://pytest.org/), [License Details](https://docs.pytest.org/en/8.0.x/license.html)
+- **pytest-mock**: Enhances pytest for unit tests by offering a simple interface to powerful mocking functionalities. [License Details](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/)
+- **cffi**: Used for interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
+- **iniconfig**: For parsing and working with INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
+- **tomli**: A Python library used for parsing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
+- **pluggy**: For creating and managing plugin systems in Python applications. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
 
-* Qt (open-source): Distributed under the GNU LGPLv3, GNU GPLv2, or Qt Commercial License. ([Qt Licensing](https://www.qt.io/licensing))
-* PySide6: Used for creating graphical user interfaces with Qt6 in Python. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/PySide6/))
-	* PySide6_Addons: Additional modules and utilities for PySide6 to enhance functionality. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/PySide6-Addons/))
-	* PySide6_Essentials: Essential components and tools for PySide6 development, including core libraries and resources. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/PySide6-Essentials/))
-* shiboken6: A Python binding generator used in conjunction with PySide6 to create Python bindings for the Qt framework. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/shiboken6/))
-* Python-Markdown: Used for Markdown to HTML conversion. ([The 3-Clause BSD License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md))
-* Emoji library: Used for converting emoji code to real emoji. ([New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt))
-* qasync: Used for handling async syntax highlighting. ([BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE))
-* cryptography: Used for generating cryptographic hashes and keys in this project is dual-licensed under the:
-	* ([Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
-	* ([BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD))
-* Bootstrap Icons: Used for UI toolbar icons and other visual elements. ([The MIT License (MIT)](https://github.com/twbs/icons/blob/main/LICENSE))
-* pytest: Used for testing. ([The MIT License (MIT)](https://docs.pytest.org/en/8.0.x/license.html))
-* pytest-mock: Used for testing. ([The MIT License (MIT)](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE))
-* asyncio: Used for handling async syntax highlighting is part of the Python standard library, which typically falls under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license).
-* cffi: Used for interfacing with C code. ([The MIT License (MIT)](https://github.com/python-cffi/cffi/blob/main/LICENSE))
-* click: Used for creating command-line interfaces. ([BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/))
-* iniconfig: Used for parsing and working with INI configuration files. ([The MIT License (MIT)](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE))
-* packaging: Used for working with Python package metadata and distribution utilities is dual-licensed under the:
-	* ([Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE))
-	* ([BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD))
-* tomli: A Python library used for parsing TOML configuration files effortlessly. ([The MIT License (MIT)](https://github.com/hukkin/tomli/blob/master/LICENSE))
-* pluggy: Used for creating and managing plugin systems in Python applications. ([The MIT License (MIT)](https://github.com/pytest-dev/pluggy/blob/main/LICENSE))
-* pycparser: Used for parsing C code and generating Abstract Syntax Trees (AST) in Python. ([BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE))
-* Pygments: Used for syntax highlighting source code in various programming languages. ([BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE))
+#### BSD Licenses
 
-Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Please refer to the documentation of each library for information about its license and terms of use.
+- **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
+- **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
+- **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
+- **Pygments**: Syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
+- **click**: Used for creating command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
+- **pycparser**: C code parser and for generating Abstract Syntax Trees (AST) in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
 
-This project includes code from external sources that are licensed under The Unlicense. We acknowledge and thank the original authors for their contributions.
+#### Other Dual Licensed
 
-* [Examples of codehilite CSS themes](https://github.com/richleland/pygments-css): Used to create color themes for code block highlighting. ([The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt))
+- **cryptography**: Provides cryptographic functions and primitives. [Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE) and [BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/cryptography/)
+- **packaging**: Python package metadata and distribution utilities. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
+
+#### Python Standard Library
+
+- **asyncio**: Part of the Python standard library, licensed under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license).
+
+#### The Unlicense
+
+- **Codehilite CSS Themes**: Base themes for code highlighting. [The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt)
+
+Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Always refer to the documentation of each library for detailed information about its license and terms of use.
 
 ### APIs
 
 #### OpenAI API Disclaimer
 
 **Disclaimer:** This project is independent and neither affiliated with, endorsed by, nor sponsored by OpenAI. Integration of the OpenAI API in this project is provided on an "as is" basis, without any official partnership or endorsement by OpenAI. The creators of this project disclaim all liability for any misuse, harm, or other consequences resulting from the use of the OpenAI API.
 
@@ -237,17 +244,15 @@
 
 **Security:** It is crucial for users to manage their API keys securely, ensuring they are not exposed or shared in public forums.
 
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
 ## Security Disclaimer
 
-This application, primarily designed for educational purposes, employs PBKDF2HMAC for key derivation and AES-256 in CBC mode for encryption, using a 256-bit key. Note that the encryption salt and iteration counts are stored unencrypted in the file's header. While secure for educational and non-critical uses, this setup may not meet the highest security standards. Users can opt to add a password hint in the file header, which should be used judiciously to balance convenience against security risks.
-
-As an educational tool, this software is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws. The developers disclaim liability for misuse or for ensuring legal compliance.
+This application is primarily designed for educational purposes and uses PBKDF2HMAC for key derivation. It employs Fernet, which utilizes AES-128 in CBC mode. The key is initially created at 256 bits but truncated to 128 bits for encryption. The encryption salt and iteration counts are stored unencrypted in the file's header, making this setup suitable for educational and non-critical applications only. As such, while this software provides basic security, it is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws, and the developers disclaim liability for misuse or legal non-compliance.
 
 ---
 
 `░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
 `╔═══════════════════════════════════════════════════════════════════════════════════════════╗`
 `║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
 `╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
```

### Comparing `notolog-0.9.0b13/app/assets/notolog-example-image.png` & `notolog-0.9.1b0/app/assets/notolog-example-image.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/notolog-logo.png` & `notolog-0.9.1b0/app/assets/notolog-logo.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/calligraphy/about_popup.css` & `notolog-0.9.1b0/app/assets/themes/calligraphy/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/calligraphy/default.ini` & `notolog-0.9.1b0/app/assets/themes/calligraphy/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/calligraphy/md.ini` & `notolog-0.9.1b0/app/assets/themes/calligraphy/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/calligraphy/settings_dialog.css` & `notolog-0.9.1b0/app/assets/themes/calligraphy/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/calligraphy/styles.css` & `notolog-0.9.1b0/app/assets/themes/calligraphy/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/calligraphy/tree_view.css` & `notolog-0.9.1b0/app/assets/themes/calligraphy/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/about_popup.css` & `notolog-0.9.1b0/app/assets/themes/default/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/default.ini` & `notolog-0.9.1b0/app/assets/themes/default/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/LICENSE` & `notolog-0.9.1b0/app/assets/themes/default/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/arrow-repeat.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/balloon-fill.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/balloon-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/balloon.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/bandaid-fill.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/bandaid-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/bandaid.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/bandaid.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/box-arrow-up-right.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/box-arrow-up.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/box-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/cursor-text.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/cursor-text.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/filetype-html.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/filetype-html.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/filetype-md.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/filetype-md.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/filetype-txt.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/filetype-txt.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/floppy2.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/floppy2.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/folder-symlink.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/folder-symlink.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/folder.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/github.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/github.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/link-45deg.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/link-45deg.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/linkedin.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/pencil-square.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/pencil-square.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/quote.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/robot.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/shield-lock-fill.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/shield-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/shield-lock.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/shield-lock.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/star.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/star.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/trash3-fill.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/trash3-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/trash3.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/trash3.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/icons/type-strikethrough.svg` & `notolog-0.9.1b0/app/assets/themes/default/icons/type-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/md.ini` & `notolog-0.9.1b0/app/assets/themes/default/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/settings_dialog.css` & `notolog-0.9.1b0/app/assets/themes/default/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/styles.css` & `notolog-0.9.1b0/app/assets/themes/default/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/default/tree_view.css` & `notolog-0.9.1b0/app/assets/themes/default/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/noir_dark/about_popup.css` & `notolog-0.9.1b0/app/assets/themes/noir_dark/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/noir_dark/default.ini` & `notolog-0.9.1b0/app/assets/themes/noir_dark/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/noir_dark/md.ini` & `notolog-0.9.1b0/app/assets/themes/noir_dark/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/noir_dark/settings_dialog.css` & `notolog-0.9.1b0/app/assets/themes/noir_dark/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/noir_dark/styles.css` & `notolog-0.9.1b0/app/assets/themes/noir_dark/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/noir_dark/tree_view.css` & `notolog-0.9.1b0/app/assets/themes/noir_dark/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/strawberry/about_popup.css` & `notolog-0.9.1b0/app/assets/themes/strawberry/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/strawberry/default.ini` & `notolog-0.9.1b0/app/assets/themes/strawberry/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/strawberry/md.ini` & `notolog-0.9.1b0/app/assets/themes/strawberry/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/strawberry/settings_dialog.css` & `notolog-0.9.1b0/app/assets/themes/strawberry/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/strawberry/styles.css` & `notolog-0.9.1b0/app/assets/themes/strawberry/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/assets/themes/strawberry/tree_view.css` & `notolog-0.9.1b0/app/assets/themes/strawberry/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/edit_widget.py` & `notolog-0.9.1b0/app/edit_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/editor_state.py` & `notolog-0.9.1b0/app/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/encrypt/enc_helper.py` & `notolog-0.9.1b0/app/encrypt/enc_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from cryptography.fernet import Fernet
 
-from ..app_config import AppConfig
-from ..settings import Settings
 from .enc_password import EncPassword
 
+from . import AppConfig
+from . import Settings
+
 import logging
 import secrets
 import base64
 
 from typing import Union
 
 
@@ -59,14 +60,15 @@
             if self.logging:
                 self.logger.warning('No iterations provided! Default value fallback')
             self.iterations = self.__class__.get_default_iterations()
 
         # Derive key from password
         key = self.generate_key_from_password()
         encoded_key = base64.urlsafe_b64encode(key)
+        # Fernet uses only the first 128 bits (16 bytes) of the key for AES encryption.
         self.cipher_suite = Fernet(encoded_key)
 
         self.key = None
 
     def generate_key_from_password(self) -> bytes:
         """
         Generate a key from the password
@@ -74,15 +76,15 @@
         Password-Based Key Derivation Function 2 (PBKDF2) implementation.
         The param length=32 is the length of the derived key.
         """
         kdf = PBKDF2HMAC(
             algorithm=hashes.SHA256(),
             iterations=self.iterations,
             salt=self.salt,
-            length=32  # Key length for AES-256
+            length=32  # 32 bytes = 256 bits key
         )
 
         self.key = kdf.derive(self.password)
 
         return self.key
 
     @staticmethod
```

### Comparing `notolog-0.9.0b13/app/encrypt/enc_new_password_dialog.py` & `notolog-0.9.1b0/app/encrypt/enc_new_password_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QLabel, QLineEdit, QPushButton, QHBoxLayout, QVBoxLayout, QStyle, QMessageBox
 from PySide6.QtGui import QFontMetrics, QFont
 
-from ..settings import Settings
-from ..app_config import AppConfig
-from ..lexemes.lexemes import Lexemes
-from ..helpers.theme_helper import ThemeHelper
+from . import Settings
+from . import AppConfig
+from . import Lexemes
+from . import ThemeHelper
 
 import logging
 
 
 class EncNewPasswordDialog(QDialog):
 
     HINT_MAX_LENGTH = 32
```

### Comparing `notolog-0.9.0b13/app/encrypt/enc_password.py` & `notolog-0.9.1b0/app/encrypt/enc_password.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 class EncPassword:
+    """
+    Password object class to store password related data.
+    """
+
     def __init__(self):
         self._password = None
         self._hint = None
 
     @property
     def password(self):
         return self._password
```

### Comparing `notolog-0.9.0b13/app/encrypt/enc_password_dialog.py` & `notolog-0.9.1b0/app/encrypt/enc_password_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QLabel, QLineEdit, QPushButton, QHBoxLayout, QVBoxLayout, QStyle, QMessageBox
 from PySide6.QtGui import QFontMetrics, QFont
 
-from ..settings import Settings
-from ..app_config import AppConfig
-from ..lexemes.lexemes import Lexemes
-from ..helpers.theme_helper import ThemeHelper
+from . import Settings
+from . import AppConfig
+from . import Lexemes
+from . import ThemeHelper
 
 import logging
 
 
 class EncPasswordDialog(QDialog):
 
     def __init__(self, hint: str = None, parent=None):
```

### Comparing `notolog-0.9.0b13/app/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.1b0/app/encrypt/enc_password_reset_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QLabel, QVBoxLayout, QDialogButtonBox, QSizePolicy
 from PySide6.QtGui import QFontMetrics
 
 from typing import Optional, Callable, Any
 
-from ..settings import Settings
-from ..app_config import AppConfig
-from ..lexemes.lexemes import Lexemes
+from . import Settings
+from . import AppConfig
+from . import Lexemes
 
 import logging
 
 
 class EncPasswordResetDialog(QDialog):
 
     def __init__(self, callback: Optional[Callable[..., Any]] = None, parent=None):
```

### Comparing `notolog-0.9.0b13/app/enums/ai_model_names.py` & `notolog-0.9.1b0/app/enums/ai_model_names.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from enum import Enum
 
 
 class AiModelNames(Enum):
 
-    # Override _generate_next_value_ to allow for custom attributes on enum members (mostly for default).
+    @staticmethod
     def _generate_next_value_(name, start, count, last_values):
         """
+        Override _generate_next_value_ to allow for custom attributes on enum members (mostly for default).
+
         'name' is the name of the Enum's member, which will be 'A', 'B', 'C', etc.
         This method returns the name itself, a 'default' marker (False), and a 'legacy' marker (False)
         """
         return name, False, False
 
     GPT_3_5 = ("gpt-3.5-turbo", True)  # The second item in the tuple marks this as the default
     GPT_3_5_LEGACY = ("gpt-3.5-turbo-instruct", False, True)  # Third param is a legacy flag (e.g. legacy completions)
```

### Comparing `notolog-0.9.0b13/app/enums/colors.py` & `notolog-0.9.1b0/app/enums/colors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from enum import Enum
 
-from PySide6.QtCore import QSize
-from PySide6.QtGui import QPixmap, QPainter, QColor, QIcon
 
 class Colors(Enum):
 
-    # Override _generate_next_value_ to allow for custom attributes on enum members (mostly for default).
+    @staticmethod
     def _generate_next_value_(name, start, count, last_values):
         """
+        Override _generate_next_value_ to allow for custom attributes on enum members (mostly for default).
+
         'name' is the name of the Enum's member, which will be 'A', 'B', 'C', etc.
         This method returns the name itself, an 'extended' marker (False), and a 'default' marker (False).
         Extended means extended color palette.
         """
         return name, False, False
 
     # Red Spectrum
```

### Comparing `notolog-0.9.0b13/app/enums/languages.py` & `notolog-0.9.1b0/app/enums/themes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 from enum import Enum
 
 
-class Languages(Enum):
+class Themes(Enum):
 
-    # Override _generate_next_value_ to allow for custom attributes on enum members (mostly for default).
+    @staticmethod
     def _generate_next_value_(name, start, count, last_values):
-        return name, False  # The second value in the tuple is the custom attribute indicating whether it's the default
+        """
+        Override _generate_next_value_ to allow for custom attributes on enum members (mostly for default).
 
-    DE = "German"
-    EN = ("English", True)
-    ES = "Spanish"
-    FR = "French"
-    GE = "Georgian"
-    GR = "Greek"
-    IN = "Hindi"
-    IT = "Italian"
-    JA = "Japanese"
-    KO = "Korean"
-    LA = "Latin"
-    PT = "Portuguese"
-    RU = "Russian"
-    TR = "Turkish"
-    ZH = "Chinese"
+        'name' is the name of the Enum's member, which will be 'A', 'B', 'C', etc.
+        This method returns the name itself and a 'default' marker (False)
+        """
+        return name, False
+
+    DEFAULT = ("Default", True)  # The second item in the tuple marks this as the default
+    CALLIGRAPHY = "Calligraphy"
+    NOIR_DARK = "Noir Dark"
+    STRAWBERRY = "Strawberry"
 
     def __init__(self, value, is_default=False):
         self._value_ = value
         self.is_default = is_default
 
     def __str__(self):
         return self.name.lower()
```

### Comparing `notolog-0.9.0b13/app/etree_extension.py` & `notolog-0.9.1b0/app/etree_extension.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/file_header.py` & `notolog-0.9.1b0/app/file_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             # Return header without content
             return header_line
 
     def load_file(self, file_path: str) -> tuple[Any, str]:
         file_data = read_file(file_path)
         return self.load(file_data)
 
-    def load(self, file_data: str) -> tuple[Any, str]:
+    def load(self, file_data: str) -> tuple[Any, Union[str, None]]:
         try:
             file_header_line = file_data.splitlines()[0]
         except (IndexError, AttributeError):
             if self.debug:
                 self.logger.debug('File header is not found')
             return self, file_data
 
@@ -181,15 +181,20 @@
             self.validate_enc()
         except (TypeError, JSONDecodeError):
             if self.debug:
                 self.logger.debug('File header is empty')
             return self, file_data
 
         if self.is_valid():
-            file_body = "\n".join(file_data.splitlines()[1:])
+            # Splitting file_data into lines
+            lines = file_data.splitlines()
+            if len(lines) >= 2:
+                file_body = "\n".join(lines[1:])
+            else:
+                file_body = None
             return self, file_body
 
         if self.debug:
             self.logger.debug('File header is empty')  # Suppose to be a valid situation if not set yet or not created
 
         return self, file_data
```

### Comparing `notolog-0.9.0b13/app/file_system_watcher.py` & `notolog-0.9.1b0/app/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/helpers/theme_helper.py` & `notolog-0.9.1b0/app/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/helpers/tooltip_helper.py` & `notolog-0.9.1b0/app/helpers/tooltip_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,20 +3,30 @@
 
 
 class TooltipHelper(QWidget):
 
     @staticmethod
     def show_tooltip(widget: QWidget, text: str, offset=QPoint(20, -20)) -> None:
         """
+        Displays a tooltip for a specified widget.
+
+        This static method is used to show a tooltip near a widget with custom text and a positional offset.
+
+        Args:
+            widget (QWidget): The widget for which the tooltip is displayed.
+            text (str): The text displayed inside the tooltip.
+            offset (QPoint): The offset from the widget's position where the tooltip should be shown.
+
+        Returns:
+            None
+        """
+
+        """
         # Using the static method to show the tooltip
         TooltipManager.show_tooltip(self.button, "Copied!", QPoint(20, -20)
-        @param widget: tooltip's target
-        @param text: tooltip's text
-        @param offset: tooltip's offset
-        @return: None
         """
 
         # Adjust where the tooltip should appear
         global_pos = widget.mapToGlobal(QPoint(0, 0)) + offset
 
         # Show tooltip
         QToolTip.showText(global_pos, text, widget)
```

### Comparing `notolog-0.9.0b13/app/helpers/update_helper.py` & `notolog-0.9.1b0/app/helpers/update_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/highlight/main_highlighter.py` & `notolog-0.9.1b0/app/highlight/main_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/highlight/md_highlighter.py` & `notolog-0.9.1b0/app/highlight/md_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/highlight/view_highlighter.py` & `notolog-0.9.1b0/app/highlight/view_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/image_downloader.py` & `notolog-0.9.1b0/app/image_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def save_image(self, url: str, data: QByteArray) -> None:
         # file_name = os.path.basename(url)
         file_name = self.url_to_filename(url)
         # File path to save
         file_path = os.path.join(self.folder.path(), file_name)
         # Save received data
-        if save_file(file_path, data, b=True):
+        if save_file(file_path, data, as_bytearray=True):
             if self.debug:
                 self.logger.debug(f"Resource saved {url} to {file_path} [{size_f(len(data))}]")
         else:
             if self.debug:
                 self.logger.debug(f"Resource not saved {url} to {file_path} [{size_f(len(data))}]")
 
     def handle_network_reply(self, reply, error_code=None):
```

### Comparing `notolog-0.9.0b13/app/lexemes/__pycache__/lexemes.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/__pycache__/lexemes.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat May  4 21:27:28 2024 UTC, .py size: 3739 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-00000000: 610d 0d0a 0000 0000 40a8 3666 9b0e 0000  a.......@.6f....
+00000000: 610d 0d0a 0000 0000 ab98 3766 9b0e 0000  a.........7f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c03 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 6d06 5a06 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000060: 8302 5a07 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2902 da05 556e 696f 6eda 0444 6963 7463  )...Union..Dictc
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0500 0000 4000 0000 7386 0000 0065 005a  ....@...s....e.Z
 000000a0: 0164 005a 0264 1965 0365 0364 039c 0264  .d.Z.d.e.e.d...d
 000000b0: 0464 0584 055a 0464 0664 0784 005a 0565  .d...Z.d.d...Z.e
@@ -189,14 +189,14 @@
 00000bc0: 655f 5fda 0373 7472 7213 0000 0072 1b00  e__..strr....r..
 00000bd0: 0000 7203 0000 0072 0f00 0000 722e 0000  ..r....r....r...
 00000be0: 0072 0200 0000 7232 0000 0072 3c00 0000  .r....r2...r<...
 00000bf0: 7231 0000 0072 3e00 0000 7211 0000 0072  r1...r>...r....r
 00000c00: 1100 0000 7211 0000 0072 1200 0000 7204  ....r....r....r.
 00000c10: 0000 0008 0000 0073 1000 0000 0801 120e  .......s........
 00000c20: 0803 1619 1009 1a18 0804 080b 7204 0000  ............r...
-00000c30: 0029 0872 1500 0000 da0e 696d 706f 7274  .).r......import
-00000c40: 6c69 622e 7574 696c 7223 0000 0072 0c00  lib.utilr#...r..
+00000c30: 0029 0872 1500 0000 720c 0000 00da 0e69  .).r....r......i
+00000c40: 6d70 6f72 746c 6962 2e75 7469 6c72 2300  mportlib.utilr#.
 00000c50: 0000 da06 7479 7069 6e67 7202 0000 0072  ....typingr....r
 00000c60: 0300 0000 7204 0000 0072 1100 0000 7211  ....r....r....r.
 00000c70: 0000 0072 1100 0000 7212 0000 00da 083c  ...r....r......<
 00000c80: 6d6f 6475 6c65 3e01 0000 0073 0800 0000  module>....s....
-00000c90: 0801 0802 0801 1003                      ........
+00000c90: 0801 0801 0802 1003                      ........
```

### Comparing `notolog-0.9.0b13/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/de/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/de/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/de/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/common.py` & `notolog-0.9.1b0/app/lexemes/de/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/main_menu.py` & `notolog-0.9.1b0/app/lexemes/de/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/de/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/statusbar.py` & `notolog-0.9.1b0/app/lexemes/de/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/de/toolbar.py` & `notolog-0.9.1b0/app/lexemes/de/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/en/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/en/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/en/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/common.py` & `notolog-0.9.1b0/app/lexemes/en/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/main_menu.py` & `notolog-0.9.1b0/app/lexemes/en/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/en/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/statusbar.py` & `notolog-0.9.1b0/app/lexemes/en/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/en/toolbar.py` & `notolog-0.9.1b0/app/lexemes/en/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/es/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/es/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/es/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/es/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/es/common.py` & `notolog-0.9.1b0/app/lexemes/es/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/es/main_menu.py` & `notolog-0.9.1b0/app/lexemes/es/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/es/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/es/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/es/statusbar.py` & `notolog-0.9.1b0/app/lexemes/es/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/es/toolbar.py` & `notolog-0.9.1b0/app/lexemes/es/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/fr/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/fr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/fr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/common.py` & `notolog-0.9.1b0/app/lexemes/fr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/main_menu.py` & `notolog-0.9.1b0/app/lexemes/fr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/fr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/statusbar.py` & `notolog-0.9.1b0/app/lexemes/fr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/fr/toolbar.py` & `notolog-0.9.1b0/app/lexemes/fr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ge/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/ge/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/ge/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/common.py` & `notolog-0.9.1b0/app/lexemes/ge/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/main_menu.py` & `notolog-0.9.1b0/app/lexemes/ge/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/ge/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/statusbar.py` & `notolog-0.9.1b0/app/lexemes/ge/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ge/toolbar.py` & `notolog-0.9.1b0/app/lexemes/ge/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/gr/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/gr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/gr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/common.py` & `notolog-0.9.1b0/app/lexemes/gr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/main_menu.py` & `notolog-0.9.1b0/app/lexemes/gr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/gr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/statusbar.py` & `notolog-0.9.1b0/app/lexemes/gr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/gr/toolbar.py` & `notolog-0.9.1b0/app/lexemes/gr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/in/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/in/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/in/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/common.py` & `notolog-0.9.1b0/app/lexemes/in/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/main_menu.py` & `notolog-0.9.1b0/app/lexemes/in/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/in/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/statusbar.py` & `notolog-0.9.1b0/app/lexemes/in/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/in/toolbar.py` & `notolog-0.9.1b0/app/lexemes/in/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/it/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/it/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/it/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/common.py` & `notolog-0.9.1b0/app/lexemes/it/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/main_menu.py` & `notolog-0.9.1b0/app/lexemes/it/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/it/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/statusbar.py` & `notolog-0.9.1b0/app/lexemes/it/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/it/toolbar.py` & `notolog-0.9.1b0/app/lexemes/it/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ja/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/ja/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/ja/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/common.py` & `notolog-0.9.1b0/app/lexemes/ja/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/main_menu.py` & `notolog-0.9.1b0/app/lexemes/ja/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/ja/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/statusbar.py` & `notolog-0.9.1b0/app/lexemes/ja/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ja/toolbar.py` & `notolog-0.9.1b0/app/lexemes/ja/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ko/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/ko/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/ko/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/common.py` & `notolog-0.9.1b0/app/lexemes/ko/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/main_menu.py` & `notolog-0.9.1b0/app/lexemes/ko/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/ko/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/statusbar.py` & `notolog-0.9.1b0/app/lexemes/ko/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ko/toolbar.py` & `notolog-0.9.1b0/app/lexemes/ko/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/la/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/la/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/la/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/la/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/la/common.py` & `notolog-0.9.1b0/app/lexemes/la/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/la/main_menu.py` & `notolog-0.9.1b0/app/lexemes/la/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/la/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/la/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/la/statusbar.py` & `notolog-0.9.1b0/app/lexemes/la/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/la/toolbar.py` & `notolog-0.9.1b0/app/lexemes/la/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/lexemes.py` & `notolog-0.9.1b0/app/lexemes/lexemes.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
+import logging
 import importlib.util
 
-import logging
 from typing import Union, Dict
 
 
 class Lexemes:
     def __init__(self, language: str = 'en', default_scope: str = 'common'):
         if not language or language in ('.', '..'):
             language = 'en'
```

### Comparing `notolog-0.9.0b13/app/lexemes/pt/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/pt/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/pt/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/pt/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/pt/common.py` & `notolog-0.9.1b0/app/lexemes/pt/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/pt/main_menu.py` & `notolog-0.9.1b0/app/lexemes/pt/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/pt/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/pt/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/pt/statusbar.py` & `notolog-0.9.1b0/app/lexemes/pt/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/pt/toolbar.py` & `notolog-0.9.1b0/app/lexemes/pt/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ru/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/ru/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ru/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/ru/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ru/common.py` & `notolog-0.9.1b0/app/lexemes/ru/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ru/main_menu.py` & `notolog-0.9.1b0/app/lexemes/ru/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ru/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/ru/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ru/statusbar.py` & `notolog-0.9.1b0/app/lexemes/ru/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/ru/toolbar.py` & `notolog-0.9.1b0/app/lexemes/ru/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/tr/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/tr/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/tr/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/tr/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/tr/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b0/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/tr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/tr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/common.py` & `notolog-0.9.1b0/app/lexemes/tr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/main_menu.py` & `notolog-0.9.1b0/app/lexemes/tr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/tr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/statusbar.py` & `notolog-0.9.1b0/app/lexemes/tr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/tr/toolbar.py` & `notolog-0.9.1b0/app/lexemes/tr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/zh/ai_assistant.py` & `notolog-0.9.1b0/app/lexemes/zh/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/zh/color_picker_dialog.py` & `notolog-0.9.1b0/app/lexemes/zh/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/zh/common.py` & `notolog-0.9.1b0/app/lexemes/zh/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/zh/main_menu.py` & `notolog-0.9.1b0/app/lexemes/zh/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/zh/settings_dialog.py` & `notolog-0.9.1b0/app/lexemes/zh/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/zh/statusbar.py` & `notolog-0.9.1b0/app/lexemes/zh/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/lexemes/zh/toolbar.py` & `notolog-0.9.1b0/app/lexemes/zh/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/notolog_editor.py` & `notolog-0.9.1b0/app/notolog_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3146,16 +3146,16 @@
                 return False
         # File is not encrypted
         else:
             # Load the file as usual
             file_header, file_body = FileHeader().load_file(file_path)
 
         # Load fields content
-        if file_body is not None:  # There should be no valid situation with file_body equal to None
-            self.load_content(file_header, file_body)
+        if file_header or file_body:  # File body equal to None when file is just created but the header was removed
+            self.load_content(file_header, file_body if file_body else '')
         else:
             self.message_box(self.lexemes.get('load_file_none_content_error'), icon_type=2)
             return False
 
         # Confirm current file path is set
         self.confirm_current_path()
```

### Comparing `notolog-0.9.0b13/app/settings.py` & `notolog-0.9.1b0/app/settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/text_block_data.py` & `notolog-0.9.1b0/app/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/theme.py` & `notolog-0.9.1b0/app/theme.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/ui/about_popup.py` & `notolog-0.9.1b0/app/ui/about_popup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 """
 
 from PySide6.QtCore import Qt, QEvent, QUrl
 from PySide6.QtGui import QPixmap, QCursor, QDesktopServices
 from PySide6.QtWidgets import QHBoxLayout, QVBoxLayout, QGridLayout, QDialog, QLabel, QFrame, QPushButton, QWidget
 from PySide6.QtWidgets import QSizePolicy
 
-from ..settings import Settings
-from ..app_config import AppConfig
-from ..lexemes.lexemes import Lexemes
-from ..helpers.theme_helper import ThemeHelper
+from . import Settings
+from . import AppConfig
+from . import Lexemes
+from . import ThemeHelper
+
 from functools import partial
 
 import logging
 
 
 class AboutPopup(QDialog):
     def __init__(self, parent=None):
```

### Comparing `notolog-0.9.0b13/app/ui/ai_assistant.py` & `notolog-0.9.1b0/app/ui/ai_assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 from PySide6.QtWidgets import QDialog, QVBoxLayout, QWidget, QLineEdit, QTextEdit, QPushButton
 from PySide6.QtWidgets import QLabel, QSizePolicy, QHBoxLayout
 from PySide6.QtGui import QPixmap
 
 import json
 import logging
 
-from ..settings import Settings
-from ..app_config import AppConfig
-from ..lexemes.lexemes import Lexemes
-from ..helpers.theme_helper import ThemeHelper
+from . import Settings
+from . import AppConfig
+from . import Lexemes
+from . import ThemeHelper
+
+from .vertical_line_spacer import VerticalLineSpacer
+
 from ..ui.rotating_label import RotatingLabel
 from ..enums.ai_model_names import AiModelNames
-from .vertical_line_spacer import VerticalLineSpacer
 
 
 class AIAssistant(QDialog):
 
     def __init__(self, parent):
         super().__init__(parent, Qt.WindowType.Dialog)
```

### Comparing `notolog-0.9.0b13/app/ui/color_picker_dialog.py` & `notolog-0.9.1b0/app/ui/color_picker_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from PySide6.QtCore import Qt, Signal
 from PySide6.QtWidgets import QGridLayout, QDialog, QPushButton
 
-from ..settings import Settings
+from . import Settings
+from . import AppConfig
+from . import Lexemes
+
 from ..enums.colors import Colors
-from ..app_config import AppConfig
-from ..lexemes.lexemes import Lexemes
 
 from functools import partial
 
 import logging
 
 
 class ColorPickerDialog(QDialog):
```

### Comparing `notolog-0.9.0b13/app/ui/common_dialog.py` & `notolog-0.9.1b0/app/ui/common_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QLabel, QVBoxLayout, QDialogButtonBox, QSizePolicy
 from PySide6.QtGui import QFontMetrics
 
-from ..app_config import AppConfig
+from . import AppConfig
 
 import logging
 
 
 class CommonDialog(QDialog):
 
     debug = AppConfig.get_debug()
```

### Comparing `notolog-0.9.0b13/app/ui/enum_combo_box.py` & `notolog-0.9.1b0/app/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/ui/file_system_model.py` & `notolog-0.9.1b0/app/ui/file_system_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from PySide6.QtGui import QColor
 from PySide6.QtWidgets import QFileSystemModel
 
 import os
 
 from typing import Any
 
-from ..helpers.theme_helper import ThemeHelper
+from . import ThemeHelper
+
 from ..helpers.file_helper import remove_trailing_numbers
 
 
 class FileSystemModel(QFileSystemModel):
     def __init__(self, *args, **kwargs):
         super(FileSystemModel, self).__init__(*args, **kwargs)
```

### Comparing `notolog-0.9.0b13/app/ui/line_numbers.py` & `notolog-0.9.1b0/app/ui/line_numbers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 from PySide6.QtCore import Qt, QObject, QRect, QSize, Slot
 from PySide6.QtWidgets import QWidget, QTextEdit, QPlainTextEdit
 from PySide6.QtGui import QPainter, QColor, QTextFormat, QTextCharFormat, QFont
 
 from typing import Union
 
-from ..app_config import AppConfig
+from . import Settings
+from . import ThemeHelper
+
 from ..edit_widget import EditWidget
-from ..helpers.theme_helper import ThemeHelper
-from ..settings import Settings
 
 
 class LineNumbers(QWidget):
     def __init__(self, editor: Union[EditWidget, QPlainTextEdit] = None):
         QWidget.__init__(self, editor)
 
         self.editor = editor
```

### Comparing `notolog-0.9.0b13/app/ui/rename_file_dialog.py` & `notolog-0.9.1b0/app/ui/rename_file_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from PySide6.QtCore import Signal, QSize
 from PySide6.QtWidgets import QInputDialog, QLineEdit, QDialogButtonBox, QSizePolicy
 
-from ..settings import Settings
-from ..enums.colors import Colors
-from ..app_config import AppConfig
-from ..lexemes.lexemes import Lexemes
+from . import Settings
+from . import AppConfig
+from . import Lexemes
 
 import logging
 
 
 class RenameFileDialog(QInputDialog):
-    colorSelected = Signal(str)
 
     def __init__(self, file_name: str, parent=None):
         super().__init__(parent)
 
         self.file_name = file_name
         self.parent = parent
```

### Comparing `notolog-0.9.0b13/app/ui/rotating_label.py` & `notolog-0.9.1b0/app/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/ui/settings_dialog.py` & `notolog-0.9.1b0/app/ui/settings_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from PySide6.QtCore import Qt, QObject, QRegularExpression
 from PySide6.QtWidgets import QDialog, QVBoxLayout, QTabWidget, QWidget, QFrame, QSizePolicy, QPlainTextEdit
 from PySide6.QtWidgets import QLabel, QCheckBox, QLineEdit, QPushButton, QComboBox, QSpinBox, QSlider, QSpacerItem
 
 import logging
 from typing import Union
 
-from ..app_config import AppConfig
-from ..lexemes.lexemes import Lexemes
-from ..helpers.theme_helper import ThemeHelper
+from . import AppConfig
+from . import Lexemes
+from . import ThemeHelper
+
 from ..enums.languages import Languages
 from ..enums.ai_model_names import AiModelNames
 from ..enums.themes import Themes
 from ..ui.enum_combo_box import EnumComboBox
 
 
 class SettingsDialog(QDialog):
```

### Comparing `notolog-0.9.0b13/app/ui/sort_filter_proxy_model.py` & `notolog-0.9.1b0/app/ui/sort_filter_proxy_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from PySide6.QtCore import QModelIndex, QSortFilterProxyModel, QRegularExpression
 
 import os
 import logging
 
-from ..app_config import AppConfig
+from . import AppConfig
+
 from ..helpers.file_helper import remove_trailing_numbers
 
 
 class SortFilterProxyModel(QSortFilterProxyModel):
 
     def __init__(self, extensions: list = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `notolog-0.9.0b13/app/ui/statusbar.py` & `notolog-0.9.1b0/app/ui/statusbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QColor
 from PySide6.QtWidgets import QStatusBar, QWidget, QLabel, QPushButton, QSizePolicy
 
 import logging
 from typing import Union
 
-from ..settings import Settings
-from ..app_config import AppConfig
-from ..lexemes.lexemes import Lexemes
-from ..helpers.theme_helper import ThemeHelper
+from . import Settings
+from . import AppConfig
+from . import Lexemes
+from . import ThemeHelper
+
 from .sort_filter_proxy_model import SortFilterProxyModel
 from .vertical_line_spacer import VerticalLineSpacer
 
 
 class StatusBar(QStatusBar):
     def __init__(self, parent=None):
         super().__init__(parent)
```

### Comparing `notolog-0.9.0b13/app/ui/toolbar.py` & `notolog-0.9.1b0/app/ui/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from PySide6.QtCore import Qt, QSize
 from PySide6.QtGui import QAction, QColor
 from PySide6.QtWidgets import QToolBar, QWidget, QMenu, QLabel, QLineEdit, QCheckBox, QToolButton, QPushButton
 from PySide6.QtWidgets import QSizePolicy
 
-from ..lexemes.lexemes import Lexemes
-from ..app_config import AppConfig
-from ..settings import Settings
-
-from ..helpers.theme_helper import ThemeHelper
+from . import Settings
+from . import AppConfig
+from . import Lexemes
+from . import ThemeHelper
 
 from typing import Union
 
 import logging
 
 
 class ToolBar(QToolBar):
```

### Comparing `notolog-0.9.0b13/app/view_decorator.py` & `notolog-0.9.1b0/app/view_decorator.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/view_processor.py` & `notolog-0.9.1b0/app/view_processor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/app/view_widget.py` & `notolog-0.9.1b0/app/view_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/docs/Examples.md` & `notolog-0.9.1b0/docs/Examples.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ## Images
 
 ### Image with path
 
 ![Notolog](app/assets/notolog-example-image.png)
 
-Code looks like: `![Alt text](notolog/assets/notolog-example-image.png)`
+Code looks like: `![Alt text](app/assets/notolog-example-image.png)`
 
 ### Image with base64 data
 
 ![Notolog inline logo](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAQAAADZc7J/AAABImlDQ1BJQ0MgcHJvZmlsZQAAKJGdkLFKw1AUhr/UokV0UhTEIYNrRwOCg1UhCBVirGB1SpMUi0kMSUrxDXwTfZgOguAzOCs4+9/o4GAWbzj8H4dz/v/eQMtOwrRsH0CaVYXr94aXwyt76Y02m/r26ARhmfc8r0/j+XzFMvrSNV7Nc3+exSguQ+lclYV5UYG1L3ZmVW5YxfrtwD8SP4jtKM0i8ZN4J0ojw2bXT5Np+ONpbrMSZxfnpq/axuWEUzxsRkyZkFDRlWbqHOOwK3UpCLinJJQmxOrNNFNxIyrl5HIoGoh0m4a8rTrPU8pIHhN5mYQ7UnmaPMz//V77OKs3rY15HhRB3VpQtcZjeH+E1SGsPcPydUNW5/fbGmaceuafb/wCNn9Qi6s+bdsAAAACYktHRADENoQlmwAABZlJREFUSMdtlWtsXMUVx38z9+57vY4fG+zFjhM7tkOc1ElKCXWbSrQQVBAIqrQqNEhAyBeKYrVFjdpIobRWPkSRSGhUakiLgqBVU7lIhJhSIZqKGEofOCWY2ImJ467ttZP1Y73Pu/femX7w2rHbzpHm05zfnPOfc+aIaQY44cnsCD3ka7PcbQNVp4LvbbBr+X/raVRj8rvyDq/h71v1/LqhxzSI07xdduFw9tEf+G/hJLXUF3yv8vTNqdv+x/0AFz439we7MSj8eAgkbtodfrcLw/YMPOfu3e7tU3GFrMVnZre4dcm32p3/BnR7rr10fbsSAgMTWeZ2BH9zV96ov2f0UEbn/ywHP3Y+DQ/gSq9UbXn3vXMdeiWgv7z/uaxPYOLHj5eZSOrcty+biUcdp+3XhUYrXn2xECmrPl//Uftm76r9U/966o3jKxDpYMbj4lBkliI+5qSKgml1tJ2MTsevZ3c3NHzdrCOvLxhvYARDx/PDTw78YhnAEg5gk8emiIc8NiAJbTySMe0DG1vqfTNG3mgxvy+6aWS4buiX0xV/WgZw0Gg0FgUKpMiRBczAxKQe2Sd9l6kgzRwXuYnbuZswf+kYPPT8vp32DQC4uEgkFgqFRmP64qtr3/FaCPxEaKKZecZoZR1Snt2T+vib3afUIsLFQSEQaECw3gTpfymzfoFWJM8wffRxjT6SFGj3THVN3X5fyV2hAI2Lu4ASlR6QFT2xflC4OGSYJckoPUyS4AOmWVeZ6LZiXQAUcbFxUSgUDpKIRyN7lN/VGGgciuSYYZoIm0nSygAu5W3jx6+GFkVciNVYiEZICXI/42Elokg0Di42RWZp4imSRPgbRTF//8CB3eaCBhqNnyCVGCjtapDj3rMHlS8G6CWhXA5jsYt2Khhk3hj+XvwbDwtRCr4Ol9WYgEQjCxsTXzMII5BQeul5ApwgSz3f4j7KSfmHj05thnJChKnCIYaBIYQ4iSxsap0wXYNmPl8CBHRjup8cf+cic6zlQXZCbfxluyYPbCHNLXgpUoMse/FhaeO5bqs8ecbQKMBbaP+hmfsrI8AME6SoYgvBrddeqPRsJI2gmX8SI6qzruoymjIVsc++IAwPcSLk0Yjil/a4Vu4rSTmGQDFNlixKzMUMaVLHKj5kjC1k1ezrvntl6Mqtv0JdZh7NDBpw9Oli+ZHK36HTnOd9LvEhCVzKqcHPRd5khPX4mHRq7XzBPEVntqg91DDJYs1O80DhTKfTcPXLmgIFYKSkuQYMmqhjjPAH/97me1tqXrOaMbibJ/Audd7jRKfX7qm+4kHgI0IQA4GBjxjt1DKJNRq9lNvZcFhYtMRahycDNj/hKt1cwZPx1sxk4R6srxZ72lf9kQQRgvgI4EVhk6I5V/gssX7D7prXJewJT4gGxvgxsI9deEsl1UvLWe/+aPEYe6kiwVUGucAnDDHOPwIjm9u9FeVJaWoMI06IJgb5EXUUsPGUEnlBPfByb+tY5+PGXoYYIU2Aenr5PYZoYVbKrTMBqbFxOM8cqwkzwTU0oNAoNL321mfef+sRfZQUrWynkcsUuJcYKQbR17lTagwEFqNMkENB6cNY6P08VZn6J92BV+jmI5IYbGIH46S5RBbTLEZMjXI1oFk5CHRpf5Zn4vYT1unz0U+pwUueOSwcNCEtNskkOTpiMlfqIo1Ge9MNoRzL7TGx45GywvIzaLRXbZv9Yqd02ZCrzi6/e421UyhumMvPdeVv1x4z3ZWDpijmc209EqYyVb1iaYQIIu9kC3ophYX0XnWaf9pwRq4YNP5i9KAal5o7nLpnqz9ZQEhiVxp+dqtzw3lxhbM1e9ee8TiL11Tmbuu6+ZWjWowC3yG0Jt6p7hL4z605VjZ0aElEEEuSHuFSYH7X3ENTjWE72l99oq7voAv/AaLcmaVSeOLtAAAAAElFTkSuQmCC)
 
 To get base64 image code from the real image use this example in Python (*Learn more about code blocks below*):
```

### Comparing `notolog-0.9.0b13/docs/notolog-ui-settings.png` & `notolog-0.9.1b0/docs/notolog-ui-settings.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/main.py` & `notolog-0.9.1b0/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,18 +41,18 @@
     """
     Possible params:
     filename='notolog.log'
     format='%(asctime)s:%(levelname)s:%(name)s:%(message)s'
     """
     logging.basicConfig(level=logging.DEBUG, format='[%(name)s] %(funcName)s: %(levelname)s: %(message)s')
 
-    # Enable logging
-    AppConfig.set_logging(True)
-    # Enable debug mode (a lot of logs)
-    AppConfig.set_debug(False)
+    # Enable logging, uncomment or change app config
+    # AppConfig.set_logging(True)
+    # Enable debug mode (a lot of logs), uncomment or change app config
+    # AppConfig.set_debug(False)
 
     # Main application
     app = QApplication(sys.argv)
 
     # Detect the operating system to choose the style
     current_os = platform.system()
     if current_os == "Windows":
```

### Comparing `notolog-0.9.0b13/notolog.egg-info/PKG-INFO` & `notolog-0.9.1b0/notolog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b13
+Version: 0.9.1b0
 Summary: Notolog Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Keywords: notolog,ai,markdown,editor
@@ -30,54 +30,50 @@
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi==1.16.0
 Requires-Dist: click==8.1.7
-Requires-Dist: cryptography==42.0.5
+Requires-Dist: cryptography==42.0.6
 Requires-Dist: emoji==2.11.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: Markdown==3.6
 Requires-Dist: packaging==24.0
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pycparser==2.22
-Requires-Dist: Pygments==2.17.2
+Requires-Dist: Pygments==2.18.0
 Requires-Dist: PySide6==6.7.0
 Requires-Dist: PySide6_Addons==6.7.0
 Requires-Dist: PySide6_Essentials==6.7.0
 Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: qasync==0.27.1
 Requires-Dist: qt6-applications==6.5.0.2.3
 Requires-Dist: qt6-tools==6.5.0.1.3
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-04 22:22:51.958596"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-05 15:21:52.653006"}} -->
 # Notolog
 
 ![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
 
 ## Overview
 
-Notolog is a markdown editor crafted in Python and Qt, offered as an open-source solution.
-
-In short, I was in search of a simple, lightweight, and cross-platform editor to fulfill my daily needs as a software developer. Concurrently, I aimed to deepen my understanding of Python, leading me to embark on creating my own editor. Thus, the Notolog editor was born.
-
-The editor has no aim but the path, hence its proof-of-concept nature and many tasks yet to be completed. Speaking of tasks, the editor features special highlighting for the word 'TODO'; simply type it with '@', like '@todo something', and see what happens.
+Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
 
 ---
 ![Notolog settings UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
 
 
 ## Features
 
-* Open sourced under the MIT license for full transparency and collaboration.
+* Notolog is open-sourced under the MIT license, promoting full transparency and encouraging collaboration.
 * Markdown syntax highlighting:
 	* Editor mode offers smooth highlighting tailored specifically for Notolog, with line numbers and extended syntax highlighting.
 	* View mode utilizes the Python Markdown library for seamless rendering of Markdown syntax.
 	* Supports multi-line block open-close tokens for improved readability and structure.
 * Multi-platform support: Compatible with all major platforms where Python is installed, ensuring accessibility across operating systems.
 * Accessible features, including:
 	* Clear and accessible descriptions for enhanced usability.
@@ -85,31 +81,32 @@
 * Background and cross-action save changes experience:
 	* Automatically saves changes in the background to ensure data integrity and minimize user intervention.
 	* Seamlessly handles unsaved changes when performing cross-actions, providing a smooth user experience.
 * Search functionality:
 	* Allows users to search within the opened file.
 	* Quick search by file name within the tree, enabling efficient navigation and content retrieval.
 * File meta-headers in the form of HTML comments to avoid excess visibility.
-* Password-based file symmetric encryption and decryption:
-	* Employing AES-256 in CBC mode (Cipher Block Chaining) with the power of the Fernet library.
-	* Key derivation based on a 256-bit key using PBKDF2HMAC from the cryptography library, using SHA-256 as the hash function.
-	* Fernet provides an easy-to-use and secure way of performing symmetric (also known as "secret key") encryption.
-	* File meta-headers to keep encryption params to allow a seamless decryption process.
+* Password-based File Encryption and Decryption:
+	* Utilizes Fernet for encryption, providing a secure and user-friendly method for symmetric (also known as "secret key") encryption.
+	* Fernet employs AES-128 in CBC mode. Plans to introduce AES-256 in future updates are aimed at further enhancing security.
+* File Meta-Headers:
+	* Notolog implements file meta-headers to store encryption parameters, ensuring a seamless decryption process.
 * Translations-friendly file structure:
 	* Supports several languages out of the box, with provisions for adding and supporting additional languages.
 * Color themes support:
 	* Comes with a few predefined color themes to customize the editor's appearance, for both light and dark modes.
 * Hotkeys support:
 	* It currently supports hotkeys like Ctrl+S for saving and Ctrl+F for searching, with plans for further expansion.
 * In-line context menus:
 	* Right-click context menu options in the file tree for file rename and delete actions.
 	* Customizable toolbar with right-click functionality to show/hide icons based on user preferences.
 * Includes a suite of unit tests to ensure code reliability and maintainability, providing confidence in the editor's functionality.
 * AI Assistant UI to get all things you need in one place:
 	* At the moment the OpenAI API is supported with plans to extend support with other providers.
+* Notolog includes specialized highlighting for TODOs. Simply type '@todo something' to mark tasks, enhancing the ability to track and manage future plans efficiently.
 
 There is no classical web engine integration to make overall package more lightweight and to achieve the best possible performance.
 
 
 ## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
@@ -233,57 +230,67 @@
 notolog\Scripts\activate
 ```
 _Mind the environment name (**notolog** or any other selected before)._
 
 
 ## Contributing
 
-If you encounter any issues or would like to contribute to the project, please don't hesitate to open an issue or submit a pull request on GitHub.
+If you encounter any issues or would like to contribute to the project, please don't hesitate to [open an issue](https://github.com/notolog/notolog-editor/issues) or submit a [pull request](https://github.com/notolog/notolog-editor/pulls) on the project's [GitHub page](https://github.com/notolog/notolog-editor).
 
 ## License
 
 The Notolog project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Third-Party Components
 
-### Libraries and Dependencies
+### Libraries and Licenses
+
+This project utilizes numerous third-party libraries, each with its own licensing terms. Below is a detailed list of these libraries grouped by license type to help clarify what each license permits and requires. This categorization aids in ensuring compliance with legal terms for use, modification, and distribution of these software components.
+
+#### GNU LGPLv3, GNU GPLv2, or Commercial License
+
+- **Qt (open-source)**: Framework for graphical user interfaces and more. [Project Details](https://www.qt.io), [Qt Licensing](https://www.qt.io/licensing)
+- **PySide6**: GUI creation with Qt6 in Python. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6/)
+- **PySide6_Addons**: Additional modules for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Addons/)
+- **PySide6_Essentials**: Core libraries for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Essentials/)
+- **shiboken6**: Binding generator for Qt framework. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/shiboken6/)
+
+#### MIT License
 
-This project utilizes the following third-party libraries:
+- **Bootstrap Icons**: Icons for UI elements. [Project Details](https://icons.getbootstrap.com/), [License Details](https://github.com/twbs/icons/blob/main/LICENSE)
+- **pytest**: Used for unit testing. It provides powerful features like fixtures, assertions, and test parameterization to facilitate writing and running Python tests. [Project Details](https://pytest.org/), [License Details](https://docs.pytest.org/en/8.0.x/license.html)
+- **pytest-mock**: Enhances pytest for unit tests by offering a simple interface to powerful mocking functionalities. [License Details](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/)
+- **cffi**: Used for interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
+- **iniconfig**: For parsing and working with INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
+- **tomli**: A Python library used for parsing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
+- **pluggy**: For creating and managing plugin systems in Python applications. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
 
-* Qt (open-source): Distributed under the GNU LGPLv3, GNU GPLv2, or Qt Commercial License. ([Qt Licensing](https://www.qt.io/licensing))
-* PySide6: Used for creating graphical user interfaces with Qt6 in Python. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/PySide6/))
-	* PySide6_Addons: Additional modules and utilities for PySide6 to enhance functionality. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/PySide6-Addons/))
-	* PySide6_Essentials: Essential components and tools for PySide6 development, including core libraries and resources. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/PySide6-Essentials/))
-* shiboken6: A Python binding generator used in conjunction with PySide6 to create Python bindings for the Qt framework. ([PySide6 is available under both Open Source (LGPLv3/GPLv2) and commercial license.](https://pypi.org/project/shiboken6/))
-* Python-Markdown: Used for Markdown to HTML conversion. ([The 3-Clause BSD License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md))
-* Emoji library: Used for converting emoji code to real emoji. ([New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt))
-* qasync: Used for handling async syntax highlighting. ([BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE))
-* cryptography: Used for generating cryptographic hashes and keys in this project is dual-licensed under the:
-	* ([Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
-	* ([BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD))
-* Bootstrap Icons: Used for UI toolbar icons and other visual elements. ([The MIT License (MIT)](https://github.com/twbs/icons/blob/main/LICENSE))
-* pytest: Used for testing. ([The MIT License (MIT)](https://docs.pytest.org/en/8.0.x/license.html))
-* pytest-mock: Used for testing. ([The MIT License (MIT)](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE))
-* asyncio: Used for handling async syntax highlighting is part of the Python standard library, which typically falls under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license).
-* cffi: Used for interfacing with C code. ([The MIT License (MIT)](https://github.com/python-cffi/cffi/blob/main/LICENSE))
-* click: Used for creating command-line interfaces. ([BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/))
-* iniconfig: Used for parsing and working with INI configuration files. ([The MIT License (MIT)](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE))
-* packaging: Used for working with Python package metadata and distribution utilities is dual-licensed under the:
-	* ([Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE))
-	* ([BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD))
-* tomli: A Python library used for parsing TOML configuration files effortlessly. ([The MIT License (MIT)](https://github.com/hukkin/tomli/blob/master/LICENSE))
-* pluggy: Used for creating and managing plugin systems in Python applications. ([The MIT License (MIT)](https://github.com/pytest-dev/pluggy/blob/main/LICENSE))
-* pycparser: Used for parsing C code and generating Abstract Syntax Trees (AST) in Python. ([BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE))
-* Pygments: Used for syntax highlighting source code in various programming languages. ([BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE))
+#### BSD Licenses
 
-Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Please refer to the documentation of each library for information about its license and terms of use.
+- **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
+- **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
+- **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
+- **Pygments**: Syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
+- **click**: Used for creating command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
+- **pycparser**: C code parser and for generating Abstract Syntax Trees (AST) in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
 
-This project includes code from external sources that are licensed under The Unlicense. We acknowledge and thank the original authors for their contributions.
+#### Other Dual Licensed
 
-* [Examples of codehilite CSS themes](https://github.com/richleland/pygments-css): Used to create color themes for code block highlighting. ([The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt))
+- **cryptography**: Provides cryptographic functions and primitives. [Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE) and [BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/cryptography/)
+- **packaging**: Python package metadata and distribution utilities. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
+
+#### Python Standard Library
+
+- **asyncio**: Part of the Python standard library, licensed under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license).
+
+#### The Unlicense
+
+- **Codehilite CSS Themes**: Base themes for code highlighting. [The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt)
+
+Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Always refer to the documentation of each library for detailed information about its license and terms of use.
 
 ### APIs
 
 #### OpenAI API Disclaimer
 
 **Disclaimer:** This project is independent and neither affiliated with, endorsed by, nor sponsored by OpenAI. Integration of the OpenAI API in this project is provided on an "as is" basis, without any official partnership or endorsement by OpenAI. The creators of this project disclaim all liability for any misuse, harm, or other consequences resulting from the use of the OpenAI API.
 
@@ -293,17 +300,15 @@
 
 **Security:** It is crucial for users to manage their API keys securely, ensuring they are not exposed or shared in public forums.
 
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
 ## Security Disclaimer
 
-This application, primarily designed for educational purposes, employs PBKDF2HMAC for key derivation and AES-256 in CBC mode for encryption, using a 256-bit key. Note that the encryption salt and iteration counts are stored unencrypted in the file's header. While secure for educational and non-critical uses, this setup may not meet the highest security standards. Users can opt to add a password hint in the file header, which should be used judiciously to balance convenience against security risks.
-
-As an educational tool, this software is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws. The developers disclaim liability for misuse or for ensuring legal compliance.
+This application is primarily designed for educational purposes and uses PBKDF2HMAC for key derivation. It employs Fernet, which utilizes AES-128 in CBC mode. The key is initially created at 256 bits but truncated to 128 bits for encryption. The encryption salt and iteration counts are stored unencrypted in the file's header, making this setup suitable for educational and non-critical applications only. As such, while this software provides basic security, it is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws, and the developers disclaim liability for misuse or legal non-compliance.
 
 ---
 
 `░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
 `╔═══════════════════════════════════════════════════════════════════════════════════════════╗`
 `║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
 `╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
```

### Comparing `notolog-0.9.0b13/notolog.egg-info/SOURCES.txt` & `notolog-0.9.1b0/notolog.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+app_config.toml
 main.py
 requirements.txt
 setup.py
 app/__init__.py
 app/app_config.py
 app/edit_widget.py
 app/editor_state.py
@@ -178,14 +179,21 @@
 app/lexemes/es/ai_assistant.py
 app/lexemes/es/color_picker_dialog.py
 app/lexemes/es/common.py
 app/lexemes/es/main_menu.py
 app/lexemes/es/settings_dialog.py
 app/lexemes/es/statusbar.py
 app/lexemes/es/toolbar.py
+app/lexemes/fi/ai_assistant.py
+app/lexemes/fi/color_picker_dialog.py
+app/lexemes/fi/common.py
+app/lexemes/fi/main_menu.py
+app/lexemes/fi/settings_dialog.py
+app/lexemes/fi/statusbar.py
+app/lexemes/fi/toolbar.py
 app/lexemes/fr/ai_assistant.py
 app/lexemes/fr/color_picker_dialog.py
 app/lexemes/fr/common.py
 app/lexemes/fr/main_menu.py
 app/lexemes/fr/settings_dialog.py
 app/lexemes/fr/statusbar.py
 app/lexemes/fr/toolbar.py
@@ -297,14 +305,28 @@
 app/lexemes/ru/ai_assistant.py
 app/lexemes/ru/color_picker_dialog.py
 app/lexemes/ru/common.py
 app/lexemes/ru/main_menu.py
 app/lexemes/ru/settings_dialog.py
 app/lexemes/ru/statusbar.py
 app/lexemes/ru/toolbar.py
+app/lexemes/se/ai_assistant.py
+app/lexemes/se/color_picker_dialog.py
+app/lexemes/se/common.py
+app/lexemes/se/main_menu.py
+app/lexemes/se/settings_dialog.py
+app/lexemes/se/statusbar.py
+app/lexemes/se/toolbar.py
+app/lexemes/se/__pycache__/ai_assistant.cpython-39.pyc
+app/lexemes/se/__pycache__/color_picker_dialog.cpython-39.pyc
+app/lexemes/se/__pycache__/common.cpython-39.pyc
+app/lexemes/se/__pycache__/main_menu.cpython-39.pyc
+app/lexemes/se/__pycache__/settings_dialog.cpython-39.pyc
+app/lexemes/se/__pycache__/statusbar.cpython-39.pyc
+app/lexemes/se/__pycache__/toolbar.cpython-39.pyc
 app/lexemes/tr/ai_assistant.py
 app/lexemes/tr/color_picker_dialog.py
 app/lexemes/tr/common.py
 app/lexemes/tr/main_menu.py
 app/lexemes/tr/settings_dialog.py
 app/lexemes/tr/statusbar.py
 app/lexemes/tr/toolbar.py
```

### Comparing `notolog-0.9.0b13/setup.py` & `notolog-0.9.1b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='notolog',
-    version='0.9.0b13',
+    version='0.9.1b0',
     description='Notolog Markdown Editor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/notolog/notolog-editor',
     author='Vadim Bakhrenkov',
     license='MIT',
     py_modules=['main'],
```

### Comparing `notolog-0.9.0b13/tests/test_enc_helper.py` & `notolog-0.9.1b0/tests/test_enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/tests/test_enc_password.py` & `notolog-0.9.1b0/tests/test_enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/tests/test_file_header.py` & `notolog-0.9.1b0/tests/test_file_header.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,24 @@
         "test_obj_file_header_load, test_exp_fixture",
         [
             (
                 '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->',
                 '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->'
             ),
             (
+                    # New line but nothing else
+                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\n',
+                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->'
+            ),
+            (
+                    # New line with return
+                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\n\r',
+                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\n'
+            ),
+            (
                 '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\ntest content',
                 '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\ntest content'
             ),
             (
                 '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837", "slt": "qwerty789ABC"}} -->',
                 '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837", "slt": "qwerty789ABC"}} -->'
             ),
```

### Comparing `notolog-0.9.0b13/tests/test_html_view.py` & `notolog-0.9.1b0/tests/test_html_view.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/tests/test_lexemes.py` & `notolog-0.9.1b0/tests/test_lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/tests/test_notolog_editor.py` & `notolog-0.9.1b0/tests/test_notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/tests/test_settings.py` & `notolog-0.9.1b0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/tests/test_text_block_data.py` & `notolog-0.9.1b0/tests/test_text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/tests/test_theme_helper.py` & `notolog-0.9.1b0/tests/test_theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b13/tests/test_themes.py` & `notolog-0.9.1b0/tests/test_themes.py`

 * *Files identical despite different names*

