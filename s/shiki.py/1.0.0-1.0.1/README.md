# Comparing `tmp/shiki_py-1.0.0.tar.gz` & `tmp/shiki_py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiki_py-1.0.0.tar", max compression
+gzip compressed data, was "shiki_py-1.0.1.tar", max compression
```

## Comparing `shiki_py-1.0.0.tar` & `shiki_py-1.0.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1065 2024-01-06 13:37:49.930848 shiki_py-1.0.0/LICENSE
--rw-r--r--   0        0        0     4658 2024-05-05 09:49:52.378845 shiki_py-1.0.0/README.md
--rw-r--r--   0        0        0      788 2024-05-05 10:01:43.060324 shiki_py-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      204 2024-03-23 16:30:48.773881 shiki_py-1.0.0/shikimori/__init__.py
--rw-r--r--   0        0        0     3353 2024-05-04 17:46:18.444467 shiki_py-1.0.0/shikimori/auth.py
--rw-r--r--   0        0        0      872 2024-03-23 16:30:48.790860 shiki_py-1.0.0/shikimori/base.py
--rw-r--r--   0        0        0     7890 2024-05-04 17:46:18.444792 shiki_py-1.0.0/shikimori/client.py
--rw-r--r--   0        0        0       97 2024-01-06 16:48:55.193076 shiki_py-1.0.0/shikimori/constants.py
--rw-r--r--   0        0        0     2048 2024-02-11 11:27:50.574403 shiki_py-1.0.0/shikimori/endpoints/__init__.py
--rw-r--r--   0        0        0     3911 2024-05-04 17:46:18.445258 shiki_py-1.0.0/shikimori/endpoints/abuse_requests.py
--rw-r--r--   0        0        0      819 2024-05-04 17:46:18.445582 shiki_py-1.0.0/shikimori/endpoints/achievements.py
--rw-r--r--   0        0        0     8947 2024-05-04 17:46:18.445985 shiki_py-1.0.0/shikimori/endpoints/animes.py
--rw-r--r--   0        0        0      850 2024-05-04 17:46:18.446254 shiki_py-1.0.0/shikimori/endpoints/appears.py
--rw-r--r--   0        0        0      737 2024-04-29 11:07:01.788203 shiki_py-1.0.0/shikimori/endpoints/bans.py
--rw-r--r--   0        0        0      363 2024-03-23 16:30:48.798016 shiki_py-1.0.0/shikimori/endpoints/base.py
--rw-r--r--   0        0        0      992 2024-05-04 17:46:18.446570 shiki_py-1.0.0/shikimori/endpoints/calendar.py
--rw-r--r--   0        0        0     1461 2024-05-04 17:46:18.446825 shiki_py-1.0.0/shikimori/endpoints/characters.py
--rw-r--r--   0        0        0    11310 2024-05-04 17:46:18.447290 shiki_py-1.0.0/shikimori/endpoints/club.py
--rw-r--r--   0        0        0     5262 2024-05-04 17:46:18.447671 shiki_py-1.0.0/shikimori/endpoints/comments.py
--rw-r--r--   0        0        0     2777 2024-05-04 17:46:18.447942 shiki_py-1.0.0/shikimori/endpoints/constants.py
--rw-r--r--   0        0        0     2080 2024-05-04 17:46:18.448426 shiki_py-1.0.0/shikimori/endpoints/dialogs.py
--rw-r--r--   0        0        0     2125 2024-05-04 17:46:18.448738 shiki_py-1.0.0/shikimori/endpoints/episode_notifications.py
--rw-r--r--   0        0        0     2407 2024-05-04 17:46:18.449120 shiki_py-1.0.0/shikimori/endpoints/favorites.py
--rw-r--r--   0        0        0      682 2024-04-29 12:55:52.524822 shiki_py-1.0.0/shikimori/endpoints/forums.py
--rw-r--r--   0        0        0     1351 2024-05-04 17:46:18.449359 shiki_py-1.0.0/shikimori/endpoints/friends.py
--rw-r--r--   0        0        0      698 2024-04-29 12:55:52.530763 shiki_py-1.0.0/shikimori/endpoints/genres.py
--rw-r--r--   0        0        0     8297 2024-05-04 17:46:18.449630 shiki_py-1.0.0/shikimori/endpoints/manga.py
--rw-r--r--   0        0        0     5220 2024-05-04 17:48:26.584427 shiki_py-1.0.0/shikimori/endpoints/message.py
--rw-r--r--   0        0        0     1622 2024-05-04 17:46:18.450179 shiki_py-1.0.0/shikimori/endpoints/people.py
--rw-r--r--   0        0        0      753 2024-04-29 11:57:01.855597 shiki_py-1.0.0/shikimori/endpoints/publisher.py
--rw-r--r--   0        0        0     8011 2024-05-04 17:51:30.352733 shiki_py-1.0.0/shikimori/endpoints/ranobe.py
--rw-r--r--   0        0        0     2472 2024-05-04 17:46:18.450707 shiki_py-1.0.0/shikimori/endpoints/review.py
--rw-r--r--   0        0        0      744 2024-02-03 17:23:20.458677 shiki_py-1.0.0/shikimori/endpoints/stats.py
--rw-r--r--   0        0        0      740 2024-04-29 12:55:52.533106 shiki_py-1.0.0/shikimori/endpoints/studios.py
--rw-r--r--   0        0        0     3167 2024-05-04 17:46:18.450961 shiki_py-1.0.0/shikimori/endpoints/styles.py
--rw-r--r--   0        0        0     1513 2024-05-04 17:46:18.451131 shiki_py-1.0.0/shikimori/endpoints/topic_ignore.py
--rw-r--r--   0        0        0     8167 2024-05-04 17:46:18.451479 shiki_py-1.0.0/shikimori/endpoints/topics.py
--rw-r--r--   0        0        0     1475 2024-05-04 17:46:18.451701 shiki_py-1.0.0/shikimori/endpoints/user_ignore.py
--rw-r--r--   0        0        0     1052 2024-05-04 17:46:18.451855 shiki_py-1.0.0/shikimori/endpoints/user_images.py
--rw-r--r--   0        0        0     8409 2024-05-04 17:46:18.452185 shiki_py-1.0.0/shikimori/endpoints/user_rates.py
--rw-r--r--   0        0        0    11127 2024-05-04 17:46:18.452363 shiki_py-1.0.0/shikimori/endpoints/users.py
--rw-r--r--   0        0        0     2487 2024-05-04 17:46:18.452515 shiki_py-1.0.0/shikimori/endpoints/videos.py
--rw-r--r--   0        0        0      940 2024-05-04 17:46:18.452741 shiki_py-1.0.0/shikimori/exceptions.py
--rw-r--r--   0        0        0     1968 2024-05-04 17:46:18.452933 shiki_py-1.0.0/shikimori/request.py
--rw-r--r--   0        0        0     1854 2024-05-01 11:49:35.943228 shiki_py-1.0.0/shikimori/requestLimiter.py
--rw-r--r--   0        0        0        1 2024-02-15 18:41:37.196491 shiki_py-1.0.0/shikimori/types/__init__.py
--rw-r--r--   0        0        0      406 2024-04-28 12:40:35.901175 shiki_py-1.0.0/shikimori/types/abuse_requests.py
--rw-r--r--   0        0        0      631 2024-04-28 11:24:53.624883 shiki_py-1.0.0/shikimori/types/achievements.py
--rw-r--r--   0        0        0     4597 2024-05-04 17:46:18.453183 shiki_py-1.0.0/shikimori/types/animes.py
--rw-r--r--   0        0        0      322 2024-05-04 17:46:18.453274 shiki_py-1.0.0/shikimori/types/auth.py
--rw-r--r--   0        0        0      922 2024-05-04 17:46:18.453439 shiki_py-1.0.0/shikimori/types/bans.py
--rw-r--r--   0        0        0      554 2024-04-28 11:24:53.609019 shiki_py-1.0.0/shikimori/types/calendar.py
--rw-r--r--   0        0        0     3825 2024-05-04 17:46:18.453689 shiki_py-1.0.0/shikimori/types/character.py
--rw-r--r--   0        0        0     2474 2024-05-04 17:46:18.453928 shiki_py-1.0.0/shikimori/types/club.py
--rw-r--r--   0        0        0     1714 2024-05-04 17:46:18.454424 shiki_py-1.0.0/shikimori/types/comment.py
--rw-r--r--   0        0        0     1352 2024-05-04 17:46:18.454583 shiki_py-1.0.0/shikimori/types/constants.py
--rw-r--r--   0        0        0      446 2024-04-28 11:24:53.632864 shiki_py-1.0.0/shikimori/types/dialog.py
--rw-r--r--   0        0        0      723 2024-04-28 11:30:54.856496 shiki_py-1.0.0/shikimori/types/episode_notification.py
--rw-r--r--   0        0        0      742 2024-05-04 17:46:18.454677 shiki_py-1.0.0/shikimori/types/externalLink.py
--rw-r--r--   0        0        0     1618 2024-04-28 11:22:41.642911 shiki_py-1.0.0/shikimori/types/franchise.py
--rw-r--r--   0        0        0      824 2024-05-04 17:46:18.454831 shiki_py-1.0.0/shikimori/types/genres.py
--rw-r--r--   0        0        0     3247 2024-05-04 17:46:18.455093 shiki_py-1.0.0/shikimori/types/manga.py
--rw-r--r--   0        0        0     1738 2024-05-04 17:46:18.455302 shiki_py-1.0.0/shikimori/types/message.py
--rw-r--r--   0        0        0     3115 2024-04-28 11:29:21.423368 shiki_py-1.0.0/shikimori/types/people.py
--rw-r--r--   0        0        0     4132 2024-04-28 13:03:34.704505 shiki_py-1.0.0/shikimori/types/photo.py
--rw-r--r--   0        0        0      280 2024-04-28 11:30:54.864635 shiki_py-1.0.0/shikimori/types/publisher.py
--rw-r--r--   0        0        0     3431 2024-05-04 17:46:18.455603 shiki_py-1.0.0/shikimori/types/ranobe.py
--rw-r--r--   0        0        0     1113 2024-04-28 11:30:54.861555 shiki_py-1.0.0/shikimori/types/review.py
--rw-r--r--   0        0        0      787 2024-05-04 17:46:18.455759 shiki_py-1.0.0/shikimori/types/roles.py
--rw-r--r--   0        0        0      549 2024-04-28 13:06:47.040816 shiki_py-1.0.0/shikimori/types/screenshots.py
--rw-r--r--   0        0        0      490 2024-04-28 11:30:54.850044 shiki_py-1.0.0/shikimori/types/studios.py
--rw-r--r--   0        0        0      673 2024-04-28 11:30:54.859945 shiki_py-1.0.0/shikimori/types/style.py
--rw-r--r--   0        0        0      313 2024-04-28 11:30:54.865687 shiki_py-1.0.0/shikimori/types/topic_ignore.py
--rw-r--r--   0        0        0     6451 2024-05-04 17:46:18.456004 shiki_py-1.0.0/shikimori/types/topics.py
--rw-r--r--   0        0        0     9604 2024-05-04 17:46:18.456216 shiki_py-1.0.0/shikimori/types/user.py
--rw-r--r--   0        0        0      315 2024-04-28 11:30:54.842896 shiki_py-1.0.0/shikimori/types/user_ignore.py
--rw-r--r--   0        0        0     1836 2024-05-04 17:46:18.456480 shiki_py-1.0.0/shikimori/types/user_rates.py
--rw-r--r--   0        0        0      595 2024-04-28 11:30:54.836706 shiki_py-1.0.0/shikimori/types/videos.py
--rw-r--r--   0        0        0       43 2024-02-11 15:13:43.589751 shiki_py-1.0.0/shikimori/utils/__init__.py
--rw-r--r--   0        0        0      323 2024-04-28 11:32:01.921240 shiki_py-1.0.0/shikimori/utils/filter.py
--rw-r--r--   0        0        0     5203 1970-01-01 00:00:00.000000 shiki_py-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-06 13:37:49.930848 shiki_py-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4658 2024-05-05 09:49:52.378845 shiki_py-1.0.1/README.md
+-rw-r--r--   0        0        0      787 2024-05-05 18:13:50.363140 shiki_py-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      204 2024-03-23 16:30:48.773881 shiki_py-1.0.1/shikimori/__init__.py
+-rw-r--r--   0        0        0     3353 2024-05-04 17:46:18.444467 shiki_py-1.0.1/shikimori/auth.py
+-rw-r--r--   0        0        0      872 2024-03-23 16:30:48.790860 shiki_py-1.0.1/shikimori/base.py
+-rw-r--r--   0        0        0     7890 2024-05-04 17:46:18.444792 shiki_py-1.0.1/shikimori/client.py
+-rw-r--r--   0        0        0       97 2024-01-06 16:48:55.193076 shiki_py-1.0.1/shikimori/constants.py
+-rw-r--r--   0        0        0     2048 2024-02-11 11:27:50.574403 shiki_py-1.0.1/shikimori/endpoints/__init__.py
+-rw-r--r--   0        0        0     3911 2024-05-04 17:46:18.445258 shiki_py-1.0.1/shikimori/endpoints/abuse_requests.py
+-rw-r--r--   0        0        0      819 2024-05-04 17:46:18.445582 shiki_py-1.0.1/shikimori/endpoints/achievements.py
+-rw-r--r--   0        0        0     8947 2024-05-04 17:46:18.445985 shiki_py-1.0.1/shikimori/endpoints/animes.py
+-rw-r--r--   0        0        0      850 2024-05-04 17:46:18.446254 shiki_py-1.0.1/shikimori/endpoints/appears.py
+-rw-r--r--   0        0        0      737 2024-04-29 11:07:01.788203 shiki_py-1.0.1/shikimori/endpoints/bans.py
+-rw-r--r--   0        0        0      363 2024-03-23 16:30:48.798016 shiki_py-1.0.1/shikimori/endpoints/base.py
+-rw-r--r--   0        0        0      992 2024-05-04 17:46:18.446570 shiki_py-1.0.1/shikimori/endpoints/calendar.py
+-rw-r--r--   0        0        0     1461 2024-05-04 17:46:18.446825 shiki_py-1.0.1/shikimori/endpoints/characters.py
+-rw-r--r--   0        0        0    11310 2024-05-04 17:46:18.447290 shiki_py-1.0.1/shikimori/endpoints/club.py
+-rw-r--r--   0        0        0     5262 2024-05-04 17:46:18.447671 shiki_py-1.0.1/shikimori/endpoints/comments.py
+-rw-r--r--   0        0        0     2777 2024-05-04 17:46:18.447942 shiki_py-1.0.1/shikimori/endpoints/constants.py
+-rw-r--r--   0        0        0     2080 2024-05-04 17:46:18.448426 shiki_py-1.0.1/shikimori/endpoints/dialogs.py
+-rw-r--r--   0        0        0     2125 2024-05-04 17:46:18.448738 shiki_py-1.0.1/shikimori/endpoints/episode_notifications.py
+-rw-r--r--   0        0        0     2407 2024-05-04 17:46:18.449120 shiki_py-1.0.1/shikimori/endpoints/favorites.py
+-rw-r--r--   0        0        0      682 2024-04-29 12:55:52.524822 shiki_py-1.0.1/shikimori/endpoints/forums.py
+-rw-r--r--   0        0        0     1351 2024-05-04 17:46:18.449359 shiki_py-1.0.1/shikimori/endpoints/friends.py
+-rw-r--r--   0        0        0      698 2024-04-29 12:55:52.530763 shiki_py-1.0.1/shikimori/endpoints/genres.py
+-rw-r--r--   0        0        0     8297 2024-05-04 17:46:18.449630 shiki_py-1.0.1/shikimori/endpoints/manga.py
+-rw-r--r--   0        0        0     5220 2024-05-04 17:48:26.584427 shiki_py-1.0.1/shikimori/endpoints/message.py
+-rw-r--r--   0        0        0     1622 2024-05-04 17:46:18.450179 shiki_py-1.0.1/shikimori/endpoints/people.py
+-rw-r--r--   0        0        0      753 2024-04-29 11:57:01.855597 shiki_py-1.0.1/shikimori/endpoints/publisher.py
+-rw-r--r--   0        0        0     8011 2024-05-04 17:51:30.352733 shiki_py-1.0.1/shikimori/endpoints/ranobe.py
+-rw-r--r--   0        0        0     2472 2024-05-04 17:46:18.450707 shiki_py-1.0.1/shikimori/endpoints/review.py
+-rw-r--r--   0        0        0      744 2024-02-03 17:23:20.458677 shiki_py-1.0.1/shikimori/endpoints/stats.py
+-rw-r--r--   0        0        0      740 2024-04-29 12:55:52.533106 shiki_py-1.0.1/shikimori/endpoints/studios.py
+-rw-r--r--   0        0        0     3167 2024-05-04 17:46:18.450961 shiki_py-1.0.1/shikimori/endpoints/styles.py
+-rw-r--r--   0        0        0     1513 2024-05-04 17:46:18.451131 shiki_py-1.0.1/shikimori/endpoints/topic_ignore.py
+-rw-r--r--   0        0        0     8167 2024-05-04 17:46:18.451479 shiki_py-1.0.1/shikimori/endpoints/topics.py
+-rw-r--r--   0        0        0     1475 2024-05-04 17:46:18.451701 shiki_py-1.0.1/shikimori/endpoints/user_ignore.py
+-rw-r--r--   0        0        0     1052 2024-05-04 17:46:18.451855 shiki_py-1.0.1/shikimori/endpoints/user_images.py
+-rw-r--r--   0        0        0     8409 2024-05-04 17:46:18.452185 shiki_py-1.0.1/shikimori/endpoints/user_rates.py
+-rw-r--r--   0        0        0    11127 2024-05-04 17:46:18.452363 shiki_py-1.0.1/shikimori/endpoints/users.py
+-rw-r--r--   0        0        0     2487 2024-05-04 17:46:18.452515 shiki_py-1.0.1/shikimori/endpoints/videos.py
+-rw-r--r--   0        0        0      940 2024-05-04 17:46:18.452741 shiki_py-1.0.1/shikimori/exceptions.py
+-rw-r--r--   0        0        0     1968 2024-05-04 17:46:18.452933 shiki_py-1.0.1/shikimori/request.py
+-rw-r--r--   0        0        0     1854 2024-05-01 11:49:35.943228 shiki_py-1.0.1/shikimori/requestLimiter.py
+-rw-r--r--   0        0        0        1 2024-02-15 18:41:37.196491 shiki_py-1.0.1/shikimori/types/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-28 12:40:35.901175 shiki_py-1.0.1/shikimori/types/abuse_requests.py
+-rw-r--r--   0        0        0      631 2024-04-28 11:24:53.624883 shiki_py-1.0.1/shikimori/types/achievements.py
+-rw-r--r--   0        0        0     4597 2024-05-04 17:46:18.453183 shiki_py-1.0.1/shikimori/types/animes.py
+-rw-r--r--   0        0        0      322 2024-05-04 17:46:18.453274 shiki_py-1.0.1/shikimori/types/auth.py
+-rw-r--r--   0        0        0      922 2024-05-04 17:46:18.453439 shiki_py-1.0.1/shikimori/types/bans.py
+-rw-r--r--   0        0        0      554 2024-04-28 11:24:53.609019 shiki_py-1.0.1/shikimori/types/calendar.py
+-rw-r--r--   0        0        0     3825 2024-05-04 17:46:18.453689 shiki_py-1.0.1/shikimori/types/character.py
+-rw-r--r--   0        0        0     2474 2024-05-04 17:46:18.453928 shiki_py-1.0.1/shikimori/types/club.py
+-rw-r--r--   0        0        0     1714 2024-05-04 17:46:18.454424 shiki_py-1.0.1/shikimori/types/comment.py
+-rw-r--r--   0        0        0     1352 2024-05-04 17:46:18.454583 shiki_py-1.0.1/shikimori/types/constants.py
+-rw-r--r--   0        0        0      446 2024-04-28 11:24:53.632864 shiki_py-1.0.1/shikimori/types/dialog.py
+-rw-r--r--   0        0        0      723 2024-04-28 11:30:54.856496 shiki_py-1.0.1/shikimori/types/episode_notification.py
+-rw-r--r--   0        0        0      742 2024-05-04 17:46:18.454677 shiki_py-1.0.1/shikimori/types/externalLink.py
+-rw-r--r--   0        0        0     1618 2024-04-28 11:22:41.642911 shiki_py-1.0.1/shikimori/types/franchise.py
+-rw-r--r--   0        0        0      824 2024-05-04 17:46:18.454831 shiki_py-1.0.1/shikimori/types/genres.py
+-rw-r--r--   0        0        0     3247 2024-05-04 17:46:18.455093 shiki_py-1.0.1/shikimori/types/manga.py
+-rw-r--r--   0        0        0     1738 2024-05-04 17:46:18.455302 shiki_py-1.0.1/shikimori/types/message.py
+-rw-r--r--   0        0        0     3115 2024-04-28 11:29:21.423368 shiki_py-1.0.1/shikimori/types/people.py
+-rw-r--r--   0        0        0     4132 2024-04-28 13:03:34.704505 shiki_py-1.0.1/shikimori/types/photo.py
+-rw-r--r--   0        0        0      280 2024-04-28 11:30:54.864635 shiki_py-1.0.1/shikimori/types/publisher.py
+-rw-r--r--   0        0        0     3431 2024-05-04 17:46:18.455603 shiki_py-1.0.1/shikimori/types/ranobe.py
+-rw-r--r--   0        0        0     1113 2024-04-28 11:30:54.861555 shiki_py-1.0.1/shikimori/types/review.py
+-rw-r--r--   0        0        0      787 2024-05-04 17:46:18.455759 shiki_py-1.0.1/shikimori/types/roles.py
+-rw-r--r--   0        0        0      549 2024-04-28 13:06:47.040816 shiki_py-1.0.1/shikimori/types/screenshots.py
+-rw-r--r--   0        0        0      490 2024-04-28 11:30:54.850044 shiki_py-1.0.1/shikimori/types/studios.py
+-rw-r--r--   0        0        0      673 2024-04-28 11:30:54.859945 shiki_py-1.0.1/shikimori/types/style.py
+-rw-r--r--   0        0        0      313 2024-04-28 11:30:54.865687 shiki_py-1.0.1/shikimori/types/topic_ignore.py
+-rw-r--r--   0        0        0     6451 2024-05-04 17:46:18.456004 shiki_py-1.0.1/shikimori/types/topics.py
+-rw-r--r--   0        0        0     9604 2024-05-04 17:46:18.456216 shiki_py-1.0.1/shikimori/types/user.py
+-rw-r--r--   0        0        0      315 2024-04-28 11:30:54.842896 shiki_py-1.0.1/shikimori/types/user_ignore.py
+-rw-r--r--   0        0        0     1836 2024-05-04 17:46:18.456480 shiki_py-1.0.1/shikimori/types/user_rates.py
+-rw-r--r--   0        0        0      595 2024-04-28 11:30:54.836706 shiki_py-1.0.1/shikimori/types/videos.py
+-rw-r--r--   0        0        0       43 2024-02-11 15:13:43.589751 shiki_py-1.0.1/shikimori/utils/__init__.py
+-rw-r--r--   0        0        0      323 2024-04-28 11:32:01.921240 shiki_py-1.0.1/shikimori/utils/filter.py
+-rw-r--r--   0        0        0     5210 1970-01-01 00:00:00.000000 shiki_py-1.0.1/PKG-INFO
```

### Comparing `shiki_py-1.0.0/LICENSE` & `shiki_py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/README.md` & `shiki_py-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/pyproject.toml` & `shiki_py-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "shiki.py"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python Async Wrapper for Shikimori Api"
 authors = ["Snayt1k3 <snayt1k3twitch@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shikimori"}]
 
 [tool.poetry.dependencies]
 python =  ">=3.10,<3.13"
-aiohttp = ">=3.9.1"
+aiohttp = "^3.9.1"
 tomli = "^2.0.1"
 setuptools = "^69.0.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pytest-asyncio = "^0.23.5"
 black = "^24.2.0"
```

### Comparing `shiki_py-1.0.0/shikimori/auth.py` & `shiki_py-1.0.1/shikimori/auth.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/base.py` & `shiki_py-1.0.1/shikimori/base.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/client.py` & `shiki_py-1.0.1/shikimori/client.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/__init__.py` & `shiki_py-1.0.1/shikimori/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/abuse_requests.py` & `shiki_py-1.0.1/shikimori/endpoints/abuse_requests.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/achievements.py` & `shiki_py-1.0.1/shikimori/endpoints/achievements.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/animes.py` & `shiki_py-1.0.1/shikimori/endpoints/animes.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/appears.py` & `shiki_py-1.0.1/shikimori/endpoints/appears.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/bans.py` & `shiki_py-1.0.1/shikimori/endpoints/bans.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/calendar.py` & `shiki_py-1.0.1/shikimori/endpoints/calendar.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/characters.py` & `shiki_py-1.0.1/shikimori/endpoints/characters.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/club.py` & `shiki_py-1.0.1/shikimori/endpoints/club.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/comments.py` & `shiki_py-1.0.1/shikimori/endpoints/comments.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/constants.py` & `shiki_py-1.0.1/shikimori/endpoints/constants.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/dialogs.py` & `shiki_py-1.0.1/shikimori/endpoints/dialogs.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/episode_notifications.py` & `shiki_py-1.0.1/shikimori/endpoints/episode_notifications.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/favorites.py` & `shiki_py-1.0.1/shikimori/endpoints/favorites.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/forums.py` & `shiki_py-1.0.1/shikimori/endpoints/forums.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/friends.py` & `shiki_py-1.0.1/shikimori/endpoints/friends.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/genres.py` & `shiki_py-1.0.1/shikimori/endpoints/genres.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/manga.py` & `shiki_py-1.0.1/shikimori/endpoints/manga.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/message.py` & `shiki_py-1.0.1/shikimori/endpoints/message.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/people.py` & `shiki_py-1.0.1/shikimori/endpoints/people.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/publisher.py` & `shiki_py-1.0.1/shikimori/endpoints/publisher.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/ranobe.py` & `shiki_py-1.0.1/shikimori/endpoints/ranobe.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/review.py` & `shiki_py-1.0.1/shikimori/endpoints/review.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/stats.py` & `shiki_py-1.0.1/shikimori/endpoints/stats.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/studios.py` & `shiki_py-1.0.1/shikimori/endpoints/studios.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/styles.py` & `shiki_py-1.0.1/shikimori/endpoints/styles.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/topic_ignore.py` & `shiki_py-1.0.1/shikimori/endpoints/topic_ignore.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/topics.py` & `shiki_py-1.0.1/shikimori/endpoints/topics.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/user_ignore.py` & `shiki_py-1.0.1/shikimori/endpoints/user_ignore.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/user_images.py` & `shiki_py-1.0.1/shikimori/endpoints/user_images.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/user_rates.py` & `shiki_py-1.0.1/shikimori/endpoints/user_rates.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/users.py` & `shiki_py-1.0.1/shikimori/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/endpoints/videos.py` & `shiki_py-1.0.1/shikimori/endpoints/videos.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/exceptions.py` & `shiki_py-1.0.1/shikimori/exceptions.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/request.py` & `shiki_py-1.0.1/shikimori/request.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/requestLimiter.py` & `shiki_py-1.0.1/shikimori/requestLimiter.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/achievements.py` & `shiki_py-1.0.1/shikimori/types/achievements.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/animes.py` & `shiki_py-1.0.1/shikimori/types/animes.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/bans.py` & `shiki_py-1.0.1/shikimori/types/bans.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/calendar.py` & `shiki_py-1.0.1/shikimori/types/calendar.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/character.py` & `shiki_py-1.0.1/shikimori/types/character.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/club.py` & `shiki_py-1.0.1/shikimori/types/club.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/comment.py` & `shiki_py-1.0.1/shikimori/types/comment.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/constants.py` & `shiki_py-1.0.1/shikimori/types/constants.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/episode_notification.py` & `shiki_py-1.0.1/shikimori/types/episode_notification.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/externalLink.py` & `shiki_py-1.0.1/shikimori/types/externalLink.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/franchise.py` & `shiki_py-1.0.1/shikimori/types/franchise.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/genres.py` & `shiki_py-1.0.1/shikimori/types/genres.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/manga.py` & `shiki_py-1.0.1/shikimori/types/manga.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/message.py` & `shiki_py-1.0.1/shikimori/types/message.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/people.py` & `shiki_py-1.0.1/shikimori/types/people.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/photo.py` & `shiki_py-1.0.1/shikimori/types/photo.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/ranobe.py` & `shiki_py-1.0.1/shikimori/types/ranobe.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/review.py` & `shiki_py-1.0.1/shikimori/types/review.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/roles.py` & `shiki_py-1.0.1/shikimori/types/roles.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/screenshots.py` & `shiki_py-1.0.1/shikimori/types/screenshots.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/style.py` & `shiki_py-1.0.1/shikimori/types/style.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/topics.py` & `shiki_py-1.0.1/shikimori/types/topics.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/user.py` & `shiki_py-1.0.1/shikimori/types/user.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/user_rates.py` & `shiki_py-1.0.1/shikimori/types/user_rates.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/shikimori/types/videos.py` & `shiki_py-1.0.1/shikimori/types/videos.py`

 * *Files identical despite different names*

### Comparing `shiki_py-1.0.0/PKG-INFO` & `shiki_py-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: shiki.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Async Wrapper for Shikimori Api
 Author: Snayt1k3
 Author-email: snayt1k3twitch@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.9.1)
+Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Shikimori API Wrapper
```

