# Comparing `tmp/django-richmin-0.1.8.tar.gz` & `tmp/django-richmin-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-richmin-0.1.8.tar", last modified: Mon Feb 12 06:51:16 2024, max compression
+gzip compressed data, was "django-richmin-0.1.9.tar", last modified: Thu Feb 15 08:26:58 2024, max compression
```

## Comparing `django-richmin-0.1.8.tar` & `django-richmin-0.1.9.tar`

### file list

```diff
@@ -1,256 +1,257 @@
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.938691 django-richmin-0.1.8/
--rw-rw-rw-   0        0        0       96 2024-02-12 06:48:14.000000 django-richmin-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2283 2024-02-12 06:51:16.937692 django-richmin-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      993 2024-01-27 18:39:52.000000 django-richmin-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.936729 django-richmin-0.1.8/django_richmin.egg-info/
--rw-rw-rw-   0        0        0     2283 2024-02-12 06:51:16.000000 django-richmin-0.1.8/django_richmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8220 2024-02-12 06:51:16.000000 django-richmin-0.1.8/django_richmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-12 06:51:16.000000 django-richmin-0.1.8/django_richmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-02-12 06:51:16.000000 django-richmin-0.1.8/django_richmin.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.631701 django-richmin-0.1.8/richmin/
--rw-rw-rw-   0        0        0       19 2024-02-12 06:51:11.000000 django-richmin-0.1.8/richmin/__init__.py
--rw-rw-rw-   0        0        0      178 2024-02-11 08:24:59.000000 django-richmin-0.1.8/richmin/apps.py
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.558701 django-richmin-0.1.8/richmin/locale/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.546702 django-richmin-0.1.8/richmin/locale/bg/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.635697 django-richmin-0.1.8/richmin/locale/bg/LC_MESSAGES/
--rw-rw-rw-   0        0        0     9852 2024-01-27 18:27:12.000000 django-richmin-0.1.8/richmin/locale/bg/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    18424 2024-01-27 18:27:12.000000 django-richmin-0.1.8/richmin/locale/bg/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.548703 django-richmin-0.1.8/richmin/locale/de/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.638703 django-richmin-0.1.8/richmin/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1569 2024-02-11 13:48:54.000000 django-richmin-0.1.8/richmin/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     2579 2024-01-27 18:27:12.000000 django-richmin-0.1.8/richmin/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.549705 django-richmin-0.1.8/richmin/locale/es/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.641698 django-richmin-0.1.8/richmin/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1608 2024-02-11 13:48:54.000000 django-richmin-0.1.8/richmin/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     2610 2024-01-27 18:27:12.000000 django-richmin-0.1.8/richmin/locale/es/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.551698 django-richmin-0.1.8/richmin/locale/fa/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.644736 django-richmin-0.1.8/richmin/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3247 2024-02-11 13:48:27.000000 django-richmin-0.1.8/richmin/locale/fa/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3545 2024-02-11 13:48:17.000000 django-richmin-0.1.8/richmin/locale/fa/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.553701 django-richmin-0.1.8/richmin/locale/fr/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.648697 django-richmin-0.1.8/richmin/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3142 2024-02-11 13:48:54.000000 django-richmin-0.1.8/richmin/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3481 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/locale/fr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.554698 django-richmin-0.1.8/richmin/locale/hu/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.651738 django-richmin-0.1.8/richmin/locale/hu/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3041 2024-01-27 18:27:12.000000 django-richmin-0.1.8/richmin/locale/hu/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     5512 2024-01-27 18:27:11.000000 django-richmin-0.1.8/richmin/locale/hu/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.555701 django-richmin-0.1.8/richmin/locale/ru/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.655736 django-richmin-0.1.8/richmin/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2922 2024-01-27 18:27:12.000000 django-richmin-0.1.8/richmin/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     4265 2024-01-27 18:27:12.000000 django-richmin-0.1.8/richmin/locale/ru/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.557699 django-richmin-0.1.8/richmin/locale/zh_Hans/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.658695 django-richmin-0.1.8/richmin/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1357 2024-02-11 13:48:54.000000 django-richmin-0.1.8/richmin/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     2163 2024-01-27 18:27:12.000000 django-richmin-0.1.8/richmin/locale/zh_Hans/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.559703 django-richmin-0.1.8/richmin/locale/zh_Hant/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.661697 django-richmin-0.1.8/richmin/locale/zh_Hant/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1359 2024-01-27 18:27:12.000000 django-richmin-0.1.8/richmin/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     2166 2024-01-27 18:27:11.000000 django-richmin-0.1.8/richmin/locale/zh_Hant/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0    14209 2024-02-12 05:05:38.000000 django-richmin-0.1.8/richmin/settings.py
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.565700 django-richmin-0.1.8/richmin/static/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.560701 django-richmin-0.1.8/richmin/static/admin/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.664734 django-richmin-0.1.8/richmin/static/admin/js/
--rw-rw-rw-   0        0        0      511 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/static/admin/js/cancel.js
--rw-rw-rw-   0        0        0     1779 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/static/admin/js/popup_response.js
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.564697 django-richmin-0.1.8/richmin/static/richmin/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.671697 django-richmin-0.1.8/richmin/static/richmin/css/
--rw-rw-rw-   0        0        0     8359 2024-02-11 18:10:41.000000 django-richmin-0.1.8/richmin/static/richmin/css/bootstrap-rtl.min.css
--rw-rw-rw-   0        0        0        0 2024-02-11 15:24:49.000000 django-richmin-0.1.8/richmin/static/richmin/css/ltr.css
--rw-rw-rw-   0        0        0    17180 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/static/richmin/css/main.css
--rw-rw-rw-   0        0        0     7993 2024-02-11 18:10:41.000000 django-richmin-0.1.8/richmin/static/richmin/css/rtl.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.674697 django-richmin-0.1.8/richmin/static/richmin/img/
--rw-rw-rw-   0        0        0     1108 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/richmin/img/calendar-icons.svg
--rw-rw-rw-   0        0        0     3325 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/richmin/img/selector-icons.svg
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.683700 django-richmin-0.1.8/richmin/static/richmin/js/
--rw-rw-rw-   0        0        0     5650 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/static/richmin/js/change_form.js
--rw-rw-rw-   0        0        0     2006 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/static/richmin/js/change_list.js
--rw-rw-rw-   0        0        0     2259 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/static/richmin/js/main.js
--rw-rw-rw-   0        0        0     5765 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/static/richmin/js/related-modal.js
--rw-rw-rw-   0        0        0    12758 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/static/richmin/js/ui-builder.js
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.564697 django-richmin-0.1.8/richmin/static/richmin/plugins/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.684696 django-richmin-0.1.8/richmin/static/richmin/plugins/bootstrap-show-modal/
--rw-rw-rw-   0        0        0     2757 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/richmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.590701 django-richmin-0.1.8/richmin/static/vendor/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.568699 django-richmin-0.1.8/richmin/static/vendor/adminlte/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.690702 django-richmin-0.1.8/richmin/static/vendor/adminlte/css/
--rw-rw-rw-   0        0        0  1382987 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/adminlte/css/adminlte.min.css
--rw-rw-rw-   0        0        0  3783135 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/adminlte/css/adminlte.min.css.map
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.701702 django-richmin-0.1.8/richmin/static/vendor/adminlte/img/
--rw-rw-rw-   0        0        0     2637 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/adminlte/img/AdminLTELogo.png
--rw-rw-rw-   0        0        0     1139 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/adminlte/img/icons.png
--rw-rw-rw-   0        0        0     5357 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/adminlte/img/user2-160x160.jpg
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.705704 django-richmin-0.1.8/richmin/static/vendor/adminlte/js/
--rw-rw-rw-   0        0        0    44250 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/adminlte/js/adminlte.min.js
--rw-rw-rw-   0        0        0   129652 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/adminlte/js/adminlte.min.js.map
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.570698 django-richmin-0.1.8/richmin/static/vendor/bootstrap/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.710696 django-richmin-0.1.8/richmin/static/vendor/bootstrap/js/
--rw-rw-rw-   0        0        0    62446 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   187647 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootstrap/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.588707 django-richmin-0.1.8/richmin/static/vendor/bootswatch/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.712696 django-richmin-0.1.8/richmin/static/vendor/bootswatch/cerulean/
--rw-rw-rw-   0        0        0   163362 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/cerulean/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.714695 django-richmin-0.1.8/richmin/static/vendor/bootswatch/cosmo/
--rw-rw-rw-   0        0        0   154468 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/cosmo/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.716699 django-richmin-0.1.8/richmin/static/vendor/bootswatch/cyborg/
--rw-rw-rw-   0        0        0   164609 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/cyborg/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.718700 django-richmin-0.1.8/richmin/static/vendor/bootswatch/darkly/
--rw-rw-rw-   0        0        0   164214 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/darkly/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.721700 django-richmin-0.1.8/richmin/static/vendor/bootswatch/default/
--rw-rw-rw-   0        0        0   161978 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/default/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.723697 django-richmin-0.1.8/richmin/static/vendor/bootswatch/flatly/
--rw-rw-rw-   0        0        0   164831 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/flatly/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.725725 django-richmin-0.1.8/richmin/static/vendor/bootswatch/journal/
--rw-rw-rw-   0        0        0   161747 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/journal/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.727695 django-richmin-0.1.8/richmin/static/vendor/bootswatch/litera/
--rw-rw-rw-   0        0        0   165160 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/litera/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.729699 django-richmin-0.1.8/richmin/static/vendor/bootswatch/lumen/
--rw-rw-rw-   0        0        0   167955 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/lumen/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.731699 django-richmin-0.1.8/richmin/static/vendor/bootswatch/lux/
--rw-rw-rw-   0        0        0   155944 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/lux/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.733712 django-richmin-0.1.8/richmin/static/vendor/bootswatch/materia/
--rw-rw-rw-   0        0        0   194485 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/materia/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.735694 django-richmin-0.1.8/richmin/static/vendor/bootswatch/minty/
--rw-rw-rw-   0        0        0   165958 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/minty/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.738694 django-richmin-0.1.8/richmin/static/vendor/bootswatch/pulse/
--rw-rw-rw-   0        0        0   155901 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/pulse/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.741695 django-richmin-0.1.8/richmin/static/vendor/bootswatch/sandstone/
--rw-rw-rw-   0        0        0   163555 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/sandstone/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.743698 django-richmin-0.1.8/richmin/static/vendor/bootswatch/simplex/
--rw-rw-rw-   0        0        0   163246 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/simplex/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.745698 django-richmin-0.1.8/richmin/static/vendor/bootswatch/sketchy/
--rw-rw-rw-   0        0        0   167055 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/sketchy/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.747695 django-richmin-0.1.8/richmin/static/vendor/bootswatch/slate/
--rw-rw-rw-   0        0        0   171644 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/slate/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.749701 django-richmin-0.1.8/richmin/static/vendor/bootswatch/solar/
--rw-rw-rw-   0        0        0   169231 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/solar/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.751697 django-richmin-0.1.8/richmin/static/vendor/bootswatch/spacelab/
--rw-rw-rw-   0        0        0   164906 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/spacelab/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.754696 django-richmin-0.1.8/richmin/static/vendor/bootswatch/superhero/
--rw-rw-rw-   0        0        0   164571 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/superhero/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.755695 django-richmin-0.1.8/richmin/static/vendor/bootswatch/united/
--rw-rw-rw-   0        0        0   161379 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/united/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.757736 django-richmin-0.1.8/richmin/static/vendor/bootswatch/yeti/
--rw-rw-rw-   0        0        0   168509 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/bootswatch/yeti/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.589712 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.759697 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/css/
--rw-rw-rw-   0        0        0    59349 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/css/all.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.794713 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/
--rw-rw-rw-   0        0        0   134346 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot
--rw-rw-rw-   0        0        0   751262 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg
--rw-rw-rw-   0        0        0   134040 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0    90060 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff
--rw-rw-rw-   0        0        0    76764 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    34034 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot
--rw-rw-rw-   0        0        0   145515 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg
--rw-rw-rw-   0        0        0    33736 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    16276 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff
--rw-rw-rw-   0        0        0    13276 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   203030 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot
--rw-rw-rw-   0        0        0   924025 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg
--rw-rw-rw-   0        0        0   202744 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0   101652 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff
--rw-rw-rw-   0        0        0    78196 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.592701 django-richmin-0.1.8/richmin/static/vendor/select2/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.796693 django-richmin-0.1.8/richmin/static/vendor/select2/css/
--rw-rw-rw-   0        0        0    16265 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/select2/css/select2.min.css
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.798726 django-richmin-0.1.8/richmin/static/vendor/select2/js/
--rw-rw-rw-   0        0        0    73171 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/static/vendor/select2/js/select2.min.js
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.605698 django-richmin-0.1.8/richmin/templates/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.837694 django-richmin-0.1.8/richmin/templates/admin/
--rw-rw-rw-   0        0        0     1489 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/actions.html
--rw-rw-rw-   0        0        0      508 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/app_index.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.594711 django-richmin-0.1.8/richmin/templates/admin/auth/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.840708 django-richmin-0.1.8/richmin/templates/admin/auth/user/
--rw-rw-rw-   0        0        0      367 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/auth/user/add_form.html
--rw-rw-rw-   0        0        0     4549 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/auth/user/change_password.html
--rw-rw-rw-   0        0        0    17937 2024-02-11 18:03:24.000000 django-richmin-0.1.8/richmin/templates/admin/base.html
--rw-rw-rw-   0        0        0       32 2024-02-11 08:25:00.000000 django-richmin-0.1.8/richmin/templates/admin/base_site.html
--rw-rw-rw-   0        0        0     5026 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/change_form.html
--rw-rw-rw-   0        0        0      557 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/change_form_object_tools.html
--rw-rw-rw-   0        0        0     4372 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/change_list.html
--rw-rw-rw-   0        0        0      520 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/change_list_object_tools.html
--rw-rw-rw-   0        0        0     1681 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/change_list_results.html
--rw-rw-rw-   0        0        0      938 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/date_hierarchy.html
--rw-rw-rw-   0        0        0     3922 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/delete_confirmation.html
--rw-rw-rw-   0        0        0     3884 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/delete_selected_confirmation.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.844693 django-richmin-0.1.8/richmin/templates/admin/edit_inline/
--rw-rw-rw-   0        0        0     3944 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/edit_inline/stacked.html
--rw-rw-rw-   0        0        0     5417 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/edit_inline/tabular.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.850693 django-richmin-0.1.8/richmin/templates/admin/filer/
--rw-rw-rw-   0        0        0     1790 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/filer/breadcrumbs.html
--rw-rw-rw-   0        0        0      922 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/filer/change_form.html
--rw-rw-rw-   0        0        0     3546 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/filer/delete_selected_files_confirmation.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.852708 django-richmin-0.1.8/richmin/templates/admin/filer/file/
--rw-rw-rw-   0        0        0     1521 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/filer/file/change_form.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.856707 django-richmin-0.1.8/richmin/templates/admin/filer/folder/
--rw-rw-rw-   0        0        0     1823 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/filer/folder/change_form.html
--rw-rw-rw-   0        0        0    12584 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/filer/folder/directory_listing.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.858696 django-richmin-0.1.8/richmin/templates/admin/filer/image/
--rw-rw-rw-   0        0        0     1506 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/filer/image/change_form.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.859696 django-richmin-0.1.8/richmin/templates/admin/filer/tools/
--rw-rw-rw-   0        0        0     2478 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/filer/tools/detail_info.html
--rw-rw-rw-   0        0        0      560 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/filter.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.875693 django-richmin-0.1.8/richmin/templates/admin/import_export/
--rw-rw-rw-   0        0        0      976 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/import_export/base.html
--rw-rw-rw-   0        0        0      404 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/templates/admin/import_export/change_list.html
--rw-rw-rw-   0        0        0      193 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/templates/admin/import_export/change_list_export.html
--rw-rw-rw-   0        0        0      305 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/import_export/change_list_export_item.html
--rw-rw-rw-   0        0        0      193 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/templates/admin/import_export/change_list_import.html
--rw-rw-rw-   0        0        0      316 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/import_export/change_list_import_export.html
--rw-rw-rw-   0        0        0      313 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/import_export/change_list_import_item.html
--rw-rw-rw-   0        0        0     2645 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/import_export/export.html
--rw-rw-rw-   0        0        0    10266 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/import_export/import.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.879692 django-richmin-0.1.8/richmin/templates/admin/includes/
--rw-rw-rw-   0        0        0     2520 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/includes/fieldset.html
--rw-rw-rw-   0        0        0      286 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/includes/object_delete_summary.html
--rw-rw-rw-   0        0        0     5515 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/index.html
--rw-rw-rw-   0        0        0     2651 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/login.html
--rw-rw-rw-   0        0        0      659 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/mptt_filter.html
--rw-rw-rw-   0        0        0     2948 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/object_history.html
--rw-rw-rw-   0        0        0      998 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/pagination.html
--rw-rw-rw-   0        0        0      563 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/popup_response.html
--rw-rw-rw-   0        0        0     1878 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/search_form.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.882765 django-richmin-0.1.8/richmin/templates/admin/solo/
--rw-rw-rw-   0        0        0      950 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin/solo/change_form.html
--rw-rw-rw-   0        0        0      570 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin/solo/object_history.html
--rw-rw-rw-   0        0        0     1978 2024-02-11 15:23:49.000000 django-richmin-0.1.8/richmin/templates/admin/submit_line.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.902692 django-richmin-0.1.8/richmin/templates/admin_doc/
--rw-rw-rw-   0        0        0      730 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin_doc/base_docs.html
--rw-rw-rw-   0        0        0     1706 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin_doc/bookmarklets.html
--rw-rw-rw-   0        0        0     1697 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin_doc/index.html
--rw-rw-rw-   0        0        0      841 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin_doc/missing_docutils.html
--rw-rw-rw-   0        0        0     2812 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin_doc/model_detail.html
--rw-rw-rw-   0        0        0     2067 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin_doc/model_index.html
--rw-rw-rw-   0        0        0     1185 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin_doc/template_detail.html
--rw-rw-rw-   0        0        0     3073 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin_doc/template_filter_index.html
--rw-rw-rw-   0        0        0     2514 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin_doc/template_tag_index.html
--rw-rw-rw-   0        0        0     1386 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/admin_doc/view_detail.html
--rw-rw-rw-   0        0        0     2602 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/admin_doc/view_index.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.916699 django-richmin-0.1.8/richmin/templates/registration/
--rw-rw-rw-   0        0        0     3193 2024-02-11 18:03:24.000000 django-richmin-0.1.8/richmin/templates/registration/base.html
--rw-rw-rw-   0        0        0      423 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/registration/logged_out.html
--rw-rw-rw-   0        0        0      882 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/registration/password_change_done.html
--rw-rw-rw-   0        0        0     4720 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/registration/password_change_form.html
--rw-rw-rw-   0        0        0      430 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/registration/password_reset_complete.html
--rw-rw-rw-   0        0        0     2306 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0        0        0      550 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/registration/password_reset_done.html
--rw-rw-rw-   0        0        0     1438 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/registration/password_reset_form.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.606708 django-richmin-0.1.8/richmin/templates/richmin/
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.928693 django-richmin-0.1.8/richmin/templates/richmin/includes/
--rw-rw-rw-   0        0        0     1743 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/richmin/includes/carousel.html
--rw-rw-rw-   0        0        0     1068 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/richmin/includes/collapsible.html
--rw-rw-rw-   0        0        0     1344 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/richmin/includes/horizontal_tabs.html
--rw-rw-rw-   0        0        0      633 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/richmin/includes/related_modal.html
--rw-rw-rw-   0        0        0      786 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/richmin/includes/single.html
--rw-rw-rw-   0        0        0    14144 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/richmin/includes/ui_builder_panel.html
--rw-rw-rw-   0        0        0     1383 2024-02-11 09:41:11.000000 django-richmin-0.1.8/richmin/templates/richmin/includes/vertical_tabs.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.930723 django-richmin-0.1.8/richmin/templates/richmin/widgets/
--rw-rw-rw-   0        0        0      484 2024-02-11 09:41:12.000000 django-richmin-0.1.8/richmin/templates/richmin/widgets/select.html
-drwxrwxrwx   0        0        0        0 2024-02-12 06:51:16.934691 django-richmin-0.1.8/richmin/templatetags/
--rw-rw-rw-   0        0        0        0 2024-01-27 17:41:49.000000 django-richmin-0.1.8/richmin/templatetags/__init__.py
--rw-rw-rw-   0        0        0    17892 2024-02-11 09:37:23.000000 django-richmin-0.1.8/richmin/templatetags/richmin.py
--rw-rw-rw-   0        0        0     7912 2024-02-11 09:22:38.000000 django-richmin-0.1.8/richmin/utils.py
--rw-rw-rw-   0        0        0      831 2024-02-11 09:17:39.000000 django-richmin-0.1.8/richmin/widgets.py
--rw-rw-rw-   0        0        0      988 2024-02-12 06:51:16.940697 django-richmin-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1563 2024-02-12 06:51:11.000000 django-richmin-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.336261 django-richmin-0.1.9/
+-rw-rw-rw-   0        0        0      197 2024-02-15 07:43:53.000000 django-richmin-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2311 2024-02-15 08:26:58.335275 django-richmin-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      993 2024-01-27 18:39:52.000000 django-richmin-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.334257 django-richmin-0.1.9/django_richmin.egg-info/
+-rw-rw-rw-   0        0        0     2311 2024-02-15 08:26:57.000000 django-richmin-0.1.9/django_richmin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8257 2024-02-15 08:26:57.000000 django-richmin-0.1.9/django_richmin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-15 08:26:57.000000 django-richmin-0.1.9/django_richmin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-02-15 08:26:57.000000 django-richmin-0.1.9/django_richmin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-02-15 08:26:57.000000 django-richmin-0.1.9/django_richmin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.029596 django-richmin-0.1.9/richmin/
+-rw-rw-rw-   0        0        0       19 2024-02-15 08:25:49.000000 django-richmin-0.1.9/richmin/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-02-11 08:24:59.000000 django-richmin-0.1.9/richmin/apps.py
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.961565 django-richmin-0.1.9/richmin/locale/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.949594 django-richmin-0.1.9/richmin/locale/bg/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.032596 django-richmin-0.1.9/richmin/locale/bg/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     9852 2024-01-27 18:27:12.000000 django-richmin-0.1.9/richmin/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    18424 2024-01-27 18:27:12.000000 django-richmin-0.1.9/richmin/locale/bg/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.951586 django-richmin-0.1.9/richmin/locale/de/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.036600 django-richmin-0.1.9/richmin/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1569 2024-02-11 13:48:54.000000 django-richmin-0.1.9/richmin/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     2579 2024-01-27 18:27:12.000000 django-richmin-0.1.9/richmin/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.952597 django-richmin-0.1.9/richmin/locale/es/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.039566 django-richmin-0.1.9/richmin/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1608 2024-02-11 13:48:54.000000 django-richmin-0.1.9/richmin/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     2610 2024-01-27 18:27:12.000000 django-richmin-0.1.9/richmin/locale/es/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.954566 django-richmin-0.1.9/richmin/locale/fa/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.043568 django-richmin-0.1.9/richmin/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3247 2024-02-11 13:48:27.000000 django-richmin-0.1.9/richmin/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3545 2024-02-11 13:48:17.000000 django-richmin-0.1.9/richmin/locale/fa/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.955608 django-richmin-0.1.9/richmin/locale/fr/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.046601 django-richmin-0.1.9/richmin/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3142 2024-02-11 13:48:54.000000 django-richmin-0.1.9/richmin/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3481 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/locale/fr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.957568 django-richmin-0.1.9/richmin/locale/hu/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.049597 django-richmin-0.1.9/richmin/locale/hu/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3041 2024-01-27 18:27:12.000000 django-richmin-0.1.9/richmin/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     5512 2024-01-27 18:27:11.000000 django-richmin-0.1.9/richmin/locale/hu/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.958566 django-richmin-0.1.9/richmin/locale/ru/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.053598 django-richmin-0.1.9/richmin/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2922 2024-01-27 18:27:12.000000 django-richmin-0.1.9/richmin/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     4265 2024-01-27 18:27:12.000000 django-richmin-0.1.9/richmin/locale/ru/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.960566 django-richmin-0.1.9/richmin/locale/zh_Hans/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.056567 django-richmin-0.1.9/richmin/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1357 2024-02-11 13:48:54.000000 django-richmin-0.1.9/richmin/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     2163 2024-01-27 18:27:12.000000 django-richmin-0.1.9/richmin/locale/zh_Hans/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.962603 django-richmin-0.1.9/richmin/locale/zh_Hant/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.059566 django-richmin-0.1.9/richmin/locale/zh_Hant/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1359 2024-01-27 18:27:12.000000 django-richmin-0.1.9/richmin/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     2166 2024-01-27 18:27:11.000000 django-richmin-0.1.9/richmin/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0    14209 2024-02-12 05:05:38.000000 django-richmin-0.1.9/richmin/settings.py
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.968567 django-richmin-0.1.9/richmin/static/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.963564 django-richmin-0.1.9/richmin/static/admin/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.063567 django-richmin-0.1.9/richmin/static/admin/js/
+-rw-rw-rw-   0        0        0      511 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/static/admin/js/cancel.js
+-rw-rw-rw-   0        0        0     1779 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/static/admin/js/popup_response.js
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.966565 django-richmin-0.1.9/richmin/static/richmin/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.070566 django-richmin-0.1.9/richmin/static/richmin/css/
+-rw-rw-rw-   0        0        0     8359 2024-02-11 18:10:41.000000 django-richmin-0.1.9/richmin/static/richmin/css/bootstrap-rtl.min.css
+-rw-rw-rw-   0        0        0        0 2024-02-11 15:24:49.000000 django-richmin-0.1.9/richmin/static/richmin/css/ltr.css
+-rw-rw-rw-   0        0        0    17180 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/static/richmin/css/main.css
+-rw-rw-rw-   0        0        0     7993 2024-02-11 18:10:41.000000 django-richmin-0.1.9/richmin/static/richmin/css/rtl.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.074568 django-richmin-0.1.9/richmin/static/richmin/img/
+-rw-rw-rw-   0        0        0     1108 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/richmin/img/calendar-icons.svg
+-rw-rw-rw-   0        0        0     3325 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/richmin/img/selector-icons.svg
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.082567 django-richmin-0.1.9/richmin/static/richmin/js/
+-rw-rw-rw-   0        0        0     5650 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/static/richmin/js/change_form.js
+-rw-rw-rw-   0        0        0     2006 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/static/richmin/js/change_list.js
+-rw-rw-rw-   0        0        0     2259 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/static/richmin/js/main.js
+-rw-rw-rw-   0        0        0     5765 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/static/richmin/js/related-modal.js
+-rw-rw-rw-   0        0        0    12758 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/static/richmin/js/ui-builder.js
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.967564 django-richmin-0.1.9/richmin/static/richmin/plugins/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.084569 django-richmin-0.1.9/richmin/static/richmin/plugins/bootstrap-show-modal/
+-rw-rw-rw-   0        0        0     2757 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/richmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.989566 django-richmin-0.1.9/richmin/static/vendor/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.970609 django-richmin-0.1.9/richmin/static/vendor/adminlte/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.090608 django-richmin-0.1.9/richmin/static/vendor/adminlte/css/
+-rw-rw-rw-   0        0        0  1382987 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/adminlte/css/adminlte.min.css
+-rw-rw-rw-   0        0        0  3783135 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/adminlte/css/adminlte.min.css.map
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.102574 django-richmin-0.1.9/richmin/static/vendor/adminlte/img/
+-rw-rw-rw-   0        0        0     2637 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/adminlte/img/AdminLTELogo.png
+-rw-rw-rw-   0        0        0     1139 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/adminlte/img/icons.png
+-rw-rw-rw-   0        0        0     5357 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/adminlte/img/user2-160x160.jpg
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.106569 django-richmin-0.1.9/richmin/static/vendor/adminlte/js/
+-rw-rw-rw-   0        0        0    44250 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/adminlte/js/adminlte.min.js
+-rw-rw-rw-   0        0        0   129652 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/adminlte/js/adminlte.min.js.map
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.971564 django-richmin-0.1.9/richmin/static/vendor/bootstrap/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.111579 django-richmin-0.1.9/richmin/static/vendor/bootstrap/js/
+-rw-rw-rw-   0        0        0    62446 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   187647 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootstrap/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.986565 django-richmin-0.1.9/richmin/static/vendor/bootswatch/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.113567 django-richmin-0.1.9/richmin/static/vendor/bootswatch/cerulean/
+-rw-rw-rw-   0        0        0   163362 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/cerulean/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.115567 django-richmin-0.1.9/richmin/static/vendor/bootswatch/cosmo/
+-rw-rw-rw-   0        0        0   154468 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/cosmo/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.118568 django-richmin-0.1.9/richmin/static/vendor/bootswatch/cyborg/
+-rw-rw-rw-   0        0        0   164609 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/cyborg/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.120640 django-richmin-0.1.9/richmin/static/vendor/bootswatch/darkly/
+-rw-rw-rw-   0        0        0   164214 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/darkly/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.122569 django-richmin-0.1.9/richmin/static/vendor/bootswatch/default/
+-rw-rw-rw-   0        0        0   161978 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/default/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.124568 django-richmin-0.1.9/richmin/static/vendor/bootswatch/flatly/
+-rw-rw-rw-   0        0        0   164831 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/flatly/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.126569 django-richmin-0.1.9/richmin/static/vendor/bootswatch/journal/
+-rw-rw-rw-   0        0        0   161747 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/journal/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.128567 django-richmin-0.1.9/richmin/static/vendor/bootswatch/litera/
+-rw-rw-rw-   0        0        0   165160 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/litera/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.131607 django-richmin-0.1.9/richmin/static/vendor/bootswatch/lumen/
+-rw-rw-rw-   0        0        0   167955 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/lumen/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.133608 django-richmin-0.1.9/richmin/static/vendor/bootswatch/lux/
+-rw-rw-rw-   0        0        0   155944 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/lux/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.135573 django-richmin-0.1.9/richmin/static/vendor/bootswatch/materia/
+-rw-rw-rw-   0        0        0   194485 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/materia/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.137608 django-richmin-0.1.9/richmin/static/vendor/bootswatch/minty/
+-rw-rw-rw-   0        0        0   165958 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/minty/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.139607 django-richmin-0.1.9/richmin/static/vendor/bootswatch/pulse/
+-rw-rw-rw-   0        0        0   155901 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/pulse/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.141607 django-richmin-0.1.9/richmin/static/vendor/bootswatch/sandstone/
+-rw-rw-rw-   0        0        0   163555 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/sandstone/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.144608 django-richmin-0.1.9/richmin/static/vendor/bootswatch/simplex/
+-rw-rw-rw-   0        0        0   163246 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/simplex/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.146609 django-richmin-0.1.9/richmin/static/vendor/bootswatch/sketchy/
+-rw-rw-rw-   0        0        0   167055 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/sketchy/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.148608 django-richmin-0.1.9/richmin/static/vendor/bootswatch/slate/
+-rw-rw-rw-   0        0        0   171644 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/slate/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.150573 django-richmin-0.1.9/richmin/static/vendor/bootswatch/solar/
+-rw-rw-rw-   0        0        0   169231 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/solar/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.153571 django-richmin-0.1.9/richmin/static/vendor/bootswatch/spacelab/
+-rw-rw-rw-   0        0        0   164906 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/spacelab/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.155610 django-richmin-0.1.9/richmin/static/vendor/bootswatch/superhero/
+-rw-rw-rw-   0        0        0   164571 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/superhero/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.157607 django-richmin-0.1.9/richmin/static/vendor/bootswatch/united/
+-rw-rw-rw-   0        0        0   161379 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/united/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.159607 django-richmin-0.1.9/richmin/static/vendor/bootswatch/yeti/
+-rw-rw-rw-   0        0        0   168509 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/bootswatch/yeti/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.989566 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.161627 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/css/
+-rw-rw-rw-   0        0        0    59349 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/css/all.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.195568 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/
+-rw-rw-rw-   0        0        0   134346 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0        0        0   751262 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0        0        0   134040 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0    90060 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0        0        0    76764 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    34034 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0        0        0   145515 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0        0        0    33736 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    16276 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0        0        0    13276 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   203030 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0        0        0   924025 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0        0        0   202744 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0   101652 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0        0        0    78196 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.991565 django-richmin-0.1.9/richmin/static/vendor/select2/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.197570 django-richmin-0.1.9/richmin/static/vendor/select2/css/
+-rw-rw-rw-   0        0        0    16265 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/select2/css/select2.min.css
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.199610 django-richmin-0.1.9/richmin/static/vendor/select2/js/
+-rw-rw-rw-   0        0        0    73171 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/static/vendor/select2/js/select2.min.js
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.002581 django-richmin-0.1.9/richmin/templates/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.238080 django-richmin-0.1.9/richmin/templates/admin/
+-rw-rw-rw-   0        0        0     1489 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/actions.html
+-rw-rw-rw-   0        0        0      508 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/app_index.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:57.993565 django-richmin-0.1.9/richmin/templates/admin/auth/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.242088 django-richmin-0.1.9/richmin/templates/admin/auth/user/
+-rw-rw-rw-   0        0        0      367 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/auth/user/add_form.html
+-rw-rw-rw-   0        0        0     4549 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/auth/user/change_password.html
+-rw-rw-rw-   0        0        0    17937 2024-02-11 18:03:24.000000 django-richmin-0.1.9/richmin/templates/admin/base.html
+-rw-rw-rw-   0        0        0       32 2024-02-11 08:25:00.000000 django-richmin-0.1.9/richmin/templates/admin/base_site.html
+-rw-rw-rw-   0        0        0     5026 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/change_form.html
+-rw-rw-rw-   0        0        0      557 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/change_form_object_tools.html
+-rw-rw-rw-   0        0        0     4372 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/change_list.html
+-rw-rw-rw-   0        0        0      520 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/change_list_object_tools.html
+-rw-rw-rw-   0        0        0     1681 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/change_list_results.html
+-rw-rw-rw-   0        0        0      938 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/date_hierarchy.html
+-rw-rw-rw-   0        0        0     3922 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/delete_confirmation.html
+-rw-rw-rw-   0        0        0     3884 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/delete_selected_confirmation.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.245064 django-richmin-0.1.9/richmin/templates/admin/edit_inline/
+-rw-rw-rw-   0        0        0     3944 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/edit_inline/stacked.html
+-rw-rw-rw-   0        0        0     5417 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/edit_inline/tabular.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.251116 django-richmin-0.1.9/richmin/templates/admin/filer/
+-rw-rw-rw-   0        0        0     1790 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/filer/breadcrumbs.html
+-rw-rw-rw-   0        0        0      922 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/filer/change_form.html
+-rw-rw-rw-   0        0        0     3546 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/filer/delete_selected_files_confirmation.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.253099 django-richmin-0.1.9/richmin/templates/admin/filer/file/
+-rw-rw-rw-   0        0        0     1521 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/filer/file/change_form.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.256065 django-richmin-0.1.9/richmin/templates/admin/filer/folder/
+-rw-rw-rw-   0        0        0     1823 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/filer/folder/change_form.html
+-rw-rw-rw-   0        0        0    12584 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/filer/folder/directory_listing.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.258060 django-richmin-0.1.9/richmin/templates/admin/filer/image/
+-rw-rw-rw-   0        0        0     1506 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/filer/image/change_form.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.260103 django-richmin-0.1.9/richmin/templates/admin/filer/tools/
+-rw-rw-rw-   0        0        0     2478 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/filer/tools/detail_info.html
+-rw-rw-rw-   0        0        0      560 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/filter.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.274069 django-richmin-0.1.9/richmin/templates/admin/import_export/
+-rw-rw-rw-   0        0        0      976 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/import_export/base.html
+-rw-rw-rw-   0        0        0      404 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/templates/admin/import_export/change_list.html
+-rw-rw-rw-   0        0        0      193 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/templates/admin/import_export/change_list_export.html
+-rw-rw-rw-   0        0        0      305 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/import_export/change_list_export_item.html
+-rw-rw-rw-   0        0        0      193 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/templates/admin/import_export/change_list_import.html
+-rw-rw-rw-   0        0        0      316 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/import_export/change_list_import_export.html
+-rw-rw-rw-   0        0        0      313 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/import_export/change_list_import_item.html
+-rw-rw-rw-   0        0        0     2645 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/import_export/export.html
+-rw-rw-rw-   0        0        0    10266 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/import_export/import.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.278070 django-richmin-0.1.9/richmin/templates/admin/includes/
+-rw-rw-rw-   0        0        0     2520 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/includes/fieldset.html
+-rw-rw-rw-   0        0        0      286 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/includes/object_delete_summary.html
+-rw-rw-rw-   0        0        0     5515 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/index.html
+-rw-rw-rw-   0        0        0     2651 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/login.html
+-rw-rw-rw-   0        0        0      659 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/mptt_filter.html
+-rw-rw-rw-   0        0        0     2948 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/object_history.html
+-rw-rw-rw-   0        0        0      998 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/pagination.html
+-rw-rw-rw-   0        0        0      563 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/popup_response.html
+-rw-rw-rw-   0        0        0     1878 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/search_form.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.281074 django-richmin-0.1.9/richmin/templates/admin/solo/
+-rw-rw-rw-   0        0        0      950 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin/solo/change_form.html
+-rw-rw-rw-   0        0        0      570 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin/solo/object_history.html
+-rw-rw-rw-   0        0        0     1978 2024-02-11 15:23:49.000000 django-richmin-0.1.9/richmin/templates/admin/submit_line.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.300059 django-richmin-0.1.9/richmin/templates/admin_doc/
+-rw-rw-rw-   0        0        0      730 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin_doc/base_docs.html
+-rw-rw-rw-   0        0        0     1706 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin_doc/bookmarklets.html
+-rw-rw-rw-   0        0        0     1697 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin_doc/index.html
+-rw-rw-rw-   0        0        0      841 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin_doc/missing_docutils.html
+-rw-rw-rw-   0        0        0     2812 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin_doc/model_detail.html
+-rw-rw-rw-   0        0        0     2067 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin_doc/model_index.html
+-rw-rw-rw-   0        0        0     1185 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin_doc/template_detail.html
+-rw-rw-rw-   0        0        0     3073 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin_doc/template_filter_index.html
+-rw-rw-rw-   0        0        0     2514 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin_doc/template_tag_index.html
+-rw-rw-rw-   0        0        0     1386 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/admin_doc/view_detail.html
+-rw-rw-rw-   0        0        0     2602 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/admin_doc/view_index.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.314062 django-richmin-0.1.9/richmin/templates/registration/
+-rw-rw-rw-   0        0        0     3193 2024-02-11 18:03:24.000000 django-richmin-0.1.9/richmin/templates/registration/base.html
+-rw-rw-rw-   0        0        0      423 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/registration/logged_out.html
+-rw-rw-rw-   0        0        0      882 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/registration/password_change_done.html
+-rw-rw-rw-   0        0        0     4720 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/registration/password_change_form.html
+-rw-rw-rw-   0        0        0      430 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0        0        0     2306 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0        0        0      550 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/registration/password_reset_done.html
+-rw-rw-rw-   0        0        0     1438 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/registration/password_reset_form.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.003567 django-richmin-0.1.9/richmin/templates/richmin/
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.327297 django-richmin-0.1.9/richmin/templates/richmin/includes/
+-rw-rw-rw-   0        0        0     1743 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/richmin/includes/carousel.html
+-rw-rw-rw-   0        0        0     1068 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/richmin/includes/collapsible.html
+-rw-rw-rw-   0        0        0     1344 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/richmin/includes/horizontal_tabs.html
+-rw-rw-rw-   0        0        0      633 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/richmin/includes/related_modal.html
+-rw-rw-rw-   0        0        0      786 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/richmin/includes/single.html
+-rw-rw-rw-   0        0        0    14144 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/richmin/includes/ui_builder_panel.html
+-rw-rw-rw-   0        0        0     1383 2024-02-11 09:41:11.000000 django-richmin-0.1.9/richmin/templates/richmin/includes/vertical_tabs.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.329297 django-richmin-0.1.9/richmin/templates/richmin/widgets/
+-rw-rw-rw-   0        0        0      484 2024-02-11 09:41:12.000000 django-richmin-0.1.9/richmin/templates/richmin/widgets/select.html
+drwxrwxrwx   0        0        0        0 2024-02-15 08:26:58.332270 django-richmin-0.1.9/richmin/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-01-27 17:41:49.000000 django-richmin-0.1.9/richmin/templatetags/__init__.py
+-rw-rw-rw-   0        0        0    17892 2024-02-11 09:37:23.000000 django-richmin-0.1.9/richmin/templatetags/richmin.py
+-rw-rw-rw-   0        0        0     7912 2024-02-11 09:22:38.000000 django-richmin-0.1.9/richmin/utils.py
+-rw-rw-rw-   0        0        0      831 2024-02-11 09:17:39.000000 django-richmin-0.1.9/richmin/widgets.py
+-rw-rw-rw-   0        0        0      988 2024-02-15 08:26:58.338295 django-richmin-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1655 2024-02-15 08:26:33.000000 django-richmin-0.1.9/setup.py
```

### Comparing `django-richmin-0.1.8/PKG-INFO` & `django-richmin-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-richmin
-Version: 0.1.8
+Version: 0.1.9
 Summary: Customized lte-bootstrap django admin theme with some useful tools
 Home-page: https://github.com/mymy47/django-richmin
 Author: my47
 Author-email: mymy47@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -24,14 +24,15 @@
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: django<5,>4
 
 
 # Django richmin (Rich Admin)
 
 Drop-in theme for django admin, that utilises AdminLTE 3 & Bootstrap 4 to make yo' admin look richy
 
 ## Installation
```

### Comparing `django-richmin-0.1.8/README.md` & `django-richmin-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/django_richmin.egg-info/PKG-INFO` & `django-richmin-0.1.9/django_richmin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-richmin
-Version: 0.1.8
+Version: 0.1.9
 Summary: Customized lte-bootstrap django admin theme with some useful tools
 Home-page: https://github.com/mymy47/django-richmin
 Author: my47
 Author-email: mymy47@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -24,14 +24,15 @@
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: django<5,>4
 
 
 # Django richmin (Rich Admin)
 
 Drop-in theme for django admin, that utilises AdminLTE 3 & Bootstrap 4 to make yo' admin look richy
 
 ## Installation
```

### Comparing `django-richmin-0.1.8/django_richmin.egg-info/SOURCES.txt` & `django-richmin-0.1.9/django_richmin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 django_richmin.egg-info/PKG-INFO
 django_richmin.egg-info/SOURCES.txt
 django_richmin.egg-info/dependency_links.txt
+django_richmin.egg-info/requires.txt
 django_richmin.egg-info/top_level.txt
 richmin/__init__.py
 richmin/apps.py
 richmin/settings.py
 richmin/utils.py
 richmin/widgets.py
 richmin/locale/bg/LC_MESSAGES/django.mo
```

### Comparing `django-richmin-0.1.8/richmin/locale/bg/LC_MESSAGES/django.mo` & `django-richmin-0.1.9/richmin/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/bg/LC_MESSAGES/django.po` & `django-richmin-0.1.9/richmin/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/de/LC_MESSAGES/django.mo` & `django-richmin-0.1.9/richmin/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/de/LC_MESSAGES/django.po` & `django-richmin-0.1.9/richmin/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/es/LC_MESSAGES/django.mo` & `django-richmin-0.1.9/richmin/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/es/LC_MESSAGES/django.po` & `django-richmin-0.1.9/richmin/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/fa/LC_MESSAGES/django.mo` & `django-richmin-0.1.9/richmin/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/fa/LC_MESSAGES/django.po` & `django-richmin-0.1.9/richmin/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/fr/LC_MESSAGES/django.mo` & `django-richmin-0.1.9/richmin/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/fr/LC_MESSAGES/django.po` & `django-richmin-0.1.9/richmin/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/hu/LC_MESSAGES/django.mo` & `django-richmin-0.1.9/richmin/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/hu/LC_MESSAGES/django.po` & `django-richmin-0.1.9/richmin/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/ru/LC_MESSAGES/django.mo` & `django-richmin-0.1.9/richmin/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/ru/LC_MESSAGES/django.po` & `django-richmin-0.1.9/richmin/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-richmin-0.1.9/richmin/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/zh_Hans/LC_MESSAGES/django.po` & `django-richmin-0.1.9/richmin/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/zh_Hant/LC_MESSAGES/django.mo` & `django-richmin-0.1.9/richmin/locale/zh_Hant/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/locale/zh_Hant/LC_MESSAGES/django.po` & `django-richmin-0.1.9/richmin/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/settings.py` & `django-richmin-0.1.9/richmin/settings.py`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/admin/js/popup_response.js` & `django-richmin-0.1.9/richmin/static/admin/js/popup_response.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/css/bootstrap-rtl.min.css` & `django-richmin-0.1.9/richmin/static/richmin/css/bootstrap-rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/css/main.css` & `django-richmin-0.1.9/richmin/static/richmin/css/main.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/css/rtl.css` & `django-richmin-0.1.9/richmin/static/richmin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/img/calendar-icons.svg` & `django-richmin-0.1.9/richmin/static/richmin/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/img/selector-icons.svg` & `django-richmin-0.1.9/richmin/static/richmin/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/js/change_form.js` & `django-richmin-0.1.9/richmin/static/richmin/js/change_form.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/js/change_list.js` & `django-richmin-0.1.9/richmin/static/richmin/js/change_list.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/js/main.js` & `django-richmin-0.1.9/richmin/static/richmin/js/main.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/js/related-modal.js` & `django-richmin-0.1.9/richmin/static/richmin/js/related-modal.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/js/ui-builder.js` & `django-richmin-0.1.9/richmin/static/richmin/js/ui-builder.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/richmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js` & `django-richmin-0.1.9/richmin/static/richmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/adminlte/css/adminlte.min.css` & `django-richmin-0.1.9/richmin/static/vendor/adminlte/css/adminlte.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/adminlte/css/adminlte.min.css.map` & `django-richmin-0.1.9/richmin/static/vendor/adminlte/css/adminlte.min.css.map`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/adminlte/img/AdminLTELogo.png` & `django-richmin-0.1.9/richmin/static/vendor/adminlte/img/AdminLTELogo.png`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/adminlte/img/icons.png` & `django-richmin-0.1.9/richmin/static/vendor/adminlte/img/icons.png`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/adminlte/img/user2-160x160.jpg` & `django-richmin-0.1.9/richmin/static/vendor/adminlte/img/user2-160x160.jpg`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/adminlte/js/adminlte.min.js` & `django-richmin-0.1.9/richmin/static/vendor/adminlte/js/adminlte.min.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/adminlte/js/adminlte.min.js.map` & `django-richmin-0.1.9/richmin/static/vendor/adminlte/js/adminlte.min.js.map`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootstrap/js/bootstrap.min.js` & `django-richmin-0.1.9/richmin/static/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootstrap/js/bootstrap.min.js.map` & `django-richmin-0.1.9/richmin/static/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/cerulean/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/cerulean/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/cosmo/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/cosmo/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/cyborg/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/cyborg/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/darkly/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/darkly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/default/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/default/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/flatly/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/flatly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/journal/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/journal/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/litera/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/litera/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/lumen/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/lumen/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/lux/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/lux/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/materia/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/materia/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/minty/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/minty/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/pulse/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/pulse/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/sandstone/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/sandstone/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/simplex/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/simplex/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/sketchy/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/sketchy/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/slate/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/slate/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/solar/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/solar/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/spacelab/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/spacelab/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/superhero/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/superhero/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/united/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/united/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/bootswatch/yeti/bootstrap.min.css` & `django-richmin-0.1.9/richmin/static/vendor/bootswatch/yeti/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/css/all.min.css` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2` & `django-richmin-0.1.9/richmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/select2/css/select2.min.css` & `django-richmin-0.1.9/richmin/static/vendor/select2/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/static/vendor/select2/js/select2.min.js` & `django-richmin-0.1.9/richmin/static/vendor/select2/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/actions.html` & `django-richmin-0.1.9/richmin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/auth/user/change_password.html` & `django-richmin-0.1.9/richmin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/base.html` & `django-richmin-0.1.9/richmin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/change_form.html` & `django-richmin-0.1.9/richmin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/change_form_object_tools.html` & `django-richmin-0.1.9/richmin/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/change_list.html` & `django-richmin-0.1.9/richmin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/change_list_object_tools.html` & `django-richmin-0.1.9/richmin/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/change_list_results.html` & `django-richmin-0.1.9/richmin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/date_hierarchy.html` & `django-richmin-0.1.9/richmin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/delete_confirmation.html` & `django-richmin-0.1.9/richmin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/delete_selected_confirmation.html` & `django-richmin-0.1.9/richmin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/edit_inline/stacked.html` & `django-richmin-0.1.9/richmin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/edit_inline/tabular.html` & `django-richmin-0.1.9/richmin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/filer/breadcrumbs.html` & `django-richmin-0.1.9/richmin/templates/admin/filer/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/filer/change_form.html` & `django-richmin-0.1.9/richmin/templates/admin/filer/change_form.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/filer/delete_selected_files_confirmation.html` & `django-richmin-0.1.9/richmin/templates/admin/filer/delete_selected_files_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/filer/file/change_form.html` & `django-richmin-0.1.9/richmin/templates/admin/filer/file/change_form.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/filer/folder/change_form.html` & `django-richmin-0.1.9/richmin/templates/admin/filer/folder/change_form.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/filer/folder/directory_listing.html` & `django-richmin-0.1.9/richmin/templates/admin/filer/folder/directory_listing.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/filer/image/change_form.html` & `django-richmin-0.1.9/richmin/templates/admin/filer/image/change_form.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/filer/tools/detail_info.html` & `django-richmin-0.1.9/richmin/templates/admin/filer/tools/detail_info.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/filter.html` & `django-richmin-0.1.9/richmin/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/import_export/base.html` & `django-richmin-0.1.9/richmin/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/import_export/export.html` & `django-richmin-0.1.9/richmin/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/import_export/import.html` & `django-richmin-0.1.9/richmin/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/includes/fieldset.html` & `django-richmin-0.1.9/richmin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/index.html` & `django-richmin-0.1.9/richmin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/login.html` & `django-richmin-0.1.9/richmin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/mptt_filter.html` & `django-richmin-0.1.9/richmin/templates/admin/mptt_filter.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/object_history.html` & `django-richmin-0.1.9/richmin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/pagination.html` & `django-richmin-0.1.9/richmin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/popup_response.html` & `django-richmin-0.1.9/richmin/templates/admin/popup_response.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/search_form.html` & `django-richmin-0.1.9/richmin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/solo/change_form.html` & `django-richmin-0.1.9/richmin/templates/admin/solo/change_form.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/solo/object_history.html` & `django-richmin-0.1.9/richmin/templates/admin/solo/object_history.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin/submit_line.html` & `django-richmin-0.1.9/richmin/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/base_docs.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/base_docs.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/bookmarklets.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/bookmarklets.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/index.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/index.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/missing_docutils.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/missing_docutils.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/model_detail.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/model_detail.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/model_index.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/model_index.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/template_detail.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/template_detail.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/template_filter_index.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/template_filter_index.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/template_tag_index.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/template_tag_index.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/view_detail.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/view_detail.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/admin_doc/view_index.html` & `django-richmin-0.1.9/richmin/templates/admin_doc/view_index.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/registration/base.html` & `django-richmin-0.1.9/richmin/templates/registration/base.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/registration/password_change_done.html` & `django-richmin-0.1.9/richmin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/registration/password_change_form.html` & `django-richmin-0.1.9/richmin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/registration/password_reset_confirm.html` & `django-richmin-0.1.9/richmin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/registration/password_reset_done.html` & `django-richmin-0.1.9/richmin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/registration/password_reset_form.html` & `django-richmin-0.1.9/richmin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/richmin/includes/carousel.html` & `django-richmin-0.1.9/richmin/templates/richmin/includes/carousel.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/richmin/includes/collapsible.html` & `django-richmin-0.1.9/richmin/templates/richmin/includes/collapsible.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/richmin/includes/horizontal_tabs.html` & `django-richmin-0.1.9/richmin/templates/richmin/includes/horizontal_tabs.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/richmin/includes/related_modal.html` & `django-richmin-0.1.9/richmin/templates/richmin/includes/related_modal.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/richmin/includes/single.html` & `django-richmin-0.1.9/richmin/templates/richmin/includes/single.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/richmin/includes/ui_builder_panel.html` & `django-richmin-0.1.9/richmin/templates/richmin/includes/ui_builder_panel.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templates/richmin/includes/vertical_tabs.html` & `django-richmin-0.1.9/richmin/templates/richmin/includes/vertical_tabs.html`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/templatetags/richmin.py` & `django-richmin-0.1.9/richmin/templatetags/richmin.py`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/utils.py` & `django-richmin-0.1.9/richmin/utils.py`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/richmin/widgets.py` & `django-richmin-0.1.9/richmin/widgets.py`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/setup.cfg` & `django-richmin-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-richmin-0.1.8/setup.py` & `django-richmin-0.1.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 setup(
     name='django-richmin',
     url='https://github.com/mymy47/django-richmin',
-    version='0.1.8',
+    version='0.1.9',
     license='MIT License',
-    packages=['richmin'],
+    packages=find_packages(),
+    include_package_data=True,
     description='Customized lte-bootstrap django admin theme with some useful tools',
     long_description=README,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
+    install_requires=[
+        'django>4,<5',
+    ],
     author='my47',
     author_email='mymy47@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
```

