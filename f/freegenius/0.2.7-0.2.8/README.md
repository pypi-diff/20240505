# Comparing `tmp/freegenius-0.2.7.tar.gz` & `tmp/freegenius-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.2.7.tar", last modified: Sat May  4 15:44:55 2024, max compression
+gzip compressed data, was "freegenius-0.2.8.tar", last modified: Sun May  5 16:20:09 2024, max compression
```

## Comparing `freegenius-0.2.7.tar` & `freegenius-0.2.8.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.503968 freegenius-0.2.7/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-04 15:44:55.499968 freegenius-0.2.7/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.471969 freegenius-0.2.7/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11707 2024-05-04 15:44:55.000000 freegenius-0.2.7/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.2.7/freegenius/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.471969 freegenius-0.2.7/freegenius/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.2.7/freegenius/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.2.7/freegenius/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.2.7/freegenius/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.2.7/freegenius/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7006 2024-04-28 21:17:47.000000 freegenius-0.2.7/freegenius/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.2.7/freegenius/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11081 2024-04-28 21:19:22.000000 freegenius-0.2.7/freegenius/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.2.7/freegenius/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.2.7/freegenius/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.2.7/freegenius/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.000000 freegenius-0.2.7/freegenius/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.2.7/freegenius/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.471969 freegenius-0.2.7/freegenius/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.2.7/freegenius/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.2.7/freegenius/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.2.7/freegenius/geminiprovision.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6513 2024-05-02 21:45:33.000000 freegenius-0.2.7/freegenius/groqchat.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.471969 freegenius-0.2.7/freegenius/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.2.7/freegenius/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.2.7/freegenius/gui/worker.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.471969 freegenius-0.2.7/freegenius/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.2.7/freegenius/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.483968 freegenius-0.2.7/freegenius/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.2.7/freegenius/icons/FreeGenius.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.2.7/freegenius/icons/FreeGenius.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.2.7/freegenius/icons/FreeGenius_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.2.7/freegenius/icons/ai.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.2.7/freegenius/icons/ai_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.2.7/freegenius/llamacpp.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.467969 freegenius-0.2.7/freegenius/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.467969 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.467969 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.467969 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.467969 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.467969 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.487968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.467969 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.491968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.491968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.467969 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.491968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.491968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.467969 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.491968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.491968 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.2.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.2.7/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.2.7/freegenius/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-05-04 15:44:55.000000 freegenius-0.2.7/freegenius/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.2.7/freegenius/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.495968 freegenius-0.2.7/freegenius/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.2.7/freegenius/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.2.7/freegenius/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.2.7/freegenius/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.2.7/freegenius/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.2.7/freegenius/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.2.7/freegenius/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.2.7/freegenius/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.2.7/freegenius/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.2.7/freegenius/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.2.7/freegenius/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2563 2024-05-02 19:23:00.000000 freegenius-0.2.7/freegenius/plugins/auto correct python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.2.7/freegenius/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.2.7/freegenius/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.2.7/freegenius/plugins/chat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.2.7/freegenius/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.2.7/freegenius/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.2.7/freegenius/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.2.7/freegenius/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.2.7/freegenius/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.2.7/freegenius/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.2.7/freegenius/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.2.7/freegenius/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.2.7/freegenius/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.2.7/freegenius/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.2.7/freegenius/plugins/execute computing tasks.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.2.7/freegenius/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.2.7/freegenius/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.2.7/freegenius/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.2.7/freegenius/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.2.7/freegenius/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.2.7/freegenius/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.2.7/freegenius/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.2.7/freegenius/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.2.7/freegenius/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.2.7/freegenius/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.2.7/freegenius/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.2.7/freegenius/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1165 2024-05-02 19:22:09.000000 freegenius-0.2.7/freegenius/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.2.7/freegenius/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.2.7/freegenius/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.2.7/freegenius/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.2.7/freegenius/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.2.7/freegenius/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.2.7/freegenius/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.2.7/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.2.7/freegenius/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.2.7/freegenius/rag.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-05-04 11:11:55.000000 freegenius-0.2.7/freegenius/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.2.7/freegenius/servers.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.2.7/freegenius/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.495968 freegenius-0.2.7/freegenius/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.2.7/freegenius/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.499968 freegenius-0.2.7/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   113539 2024-05-04 15:44:12.000000 freegenius-0.2.7/freegenius/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    30152 2024-05-03 15:57:52.000000 freegenius-0.2.7/freegenius/utils/call_chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17682 2024-05-03 15:59:20.000000 freegenius-0.2.7/freegenius/utils/call_gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21380 2024-05-03 15:52:00.000000 freegenius-0.2.7/freegenius/utils/call_groq.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    25047 2024-05-03 16:02:40.000000 freegenius-0.2.7/freegenius/utils/call_llamacpp.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.2.7/freegenius/utils/call_llm.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19102 2024-05-03 16:04:26.000000 freegenius-0.2.7/freegenius/utils/call_ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18528 2024-05-04 13:26:06.000000 freegenius-0.2.7/freegenius/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.2.7/freegenius/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.2.7/freegenius/utils/download.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.2.7/freegenius/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4976 2024-05-04 08:21:49.000000 freegenius-0.2.7/freegenius/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.2.7/freegenius/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.2.7/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.2.7/freegenius/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.2.7/freegenius/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.2.7/freegenius/utils/python_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    51559 2024-05-04 10:54:38.000000 freegenius-0.2.7/freegenius/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.2.7/freegenius/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.2.7/freegenius/utils/single_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.2.7/freegenius/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.2.7/freegenius/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.2.7/freegenius/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.2.7/freegenius/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.2.7/freegenius/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4353 2024-05-02 17:22:30.000000 freegenius-0.2.7/freegenius/utils/tool_plugins.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11304 2024-05-04 13:53:35.000000 freegenius-0.2.7/freegenius/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9152 2024-05-04 15:43:23.000000 freegenius-0.2.7/freegenius/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4721 2024-05-04 10:56:37.000000 freegenius-0.2.7/freegenius/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:44:55.499968 freegenius-0.2.7/freegenius.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-04 15:44:55.000000 freegenius-0.2.7/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-05-04 15:44:55.000000 freegenius-0.2.7/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-05-04 15:44:55.000000 freegenius-0.2.7/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-05-04 15:44:55.000000 freegenius-0.2.7/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-05-04 15:44:55.000000 freegenius-0.2.7/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-05-04 15:44:55.000000 freegenius-0.2.7/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-05-04 15:44:55.503968 freegenius-0.2.7/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10460 2024-05-04 15:44:42.000000 freegenius-0.2.7/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.239193 freegenius-0.2.8/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14931 2024-05-05 16:20:09.239193 freegenius-0.2.8/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.191194 freegenius-0.2.8/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11707 2024-05-05 16:20:08.000000 freegenius-0.2.8/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.2.8/freegenius/__init__.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.191194 freegenius-0.2.8/freegenius/audio/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.2.8/freegenius/audio/notification1.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.2.8/freegenius/audio/notification1_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.2.8/freegenius/audio/notification2.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.2.8/freegenius/audio/notification2_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7006 2024-04-28 21:17:47.000000 freegenius-0.2.8/freegenius/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.2.8/freegenius/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11081 2024-04-28 21:19:22.000000 freegenius-0.2.8/freegenius/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.2.8/freegenius/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.2.8/freegenius/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.2.8/freegenius/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:08.000000 freegenius-0.2.8/freegenius/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.2.8/freegenius/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.191194 freegenius-0.2.8/freegenius/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.2.8/freegenius/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.2.8/freegenius/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.2.8/freegenius/geminiprovision.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6513 2024-05-02 21:45:33.000000 freegenius-0.2.8/freegenius/groqchat.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.191194 freegenius-0.2.8/freegenius/gui/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.2.8/freegenius/gui/chatgui.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.2.8/freegenius/gui/worker.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.191194 freegenius-0.2.8/freegenius/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.2.8/freegenius/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.211193 freegenius-0.2.8/freegenius/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.2.8/freegenius/icons/FreeGenius.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.2.8/freegenius/icons/FreeGenius.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.2.8/freegenius/icons/FreeGenius_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.2.8/freegenius/icons/ai.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.2.8/freegenius/icons/ai_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.2.8/freegenius/llamacpp.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.187194 freegenius-0.2.8/freegenius/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.183194 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.215193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.219193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.183194 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.219193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.219193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.187194 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.219193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.219193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.187194 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.219193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.219193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.187194 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.219193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.219193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.187194 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.223193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.223193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.187194 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.223193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.223193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.187194 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.223193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.223193 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.2.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.2.8/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.2.8/freegenius/ollamachat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-05-05 16:20:08.000000 freegenius-0.2.8/freegenius/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.2.8/freegenius/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.231193 freegenius-0.2.8/freegenius/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.2.8/freegenius/plugins/000_check_ffmpeg.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.2.8/freegenius/plugins/000_check_pyaudio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.2.8/freegenius/plugins/000_check_vlc.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.2.8/freegenius/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.2.8/freegenius/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.2.8/freegenius/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.2.8/freegenius/plugins/analyze audio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.2.8/freegenius/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.2.8/freegenius/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.2.8/freegenius/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2563 2024-05-02 19:23:00.000000 freegenius-0.2.8/freegenius/plugins/auto correct python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.2.8/freegenius/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.2.8/freegenius/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.2.8/freegenius/plugins/chat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.2.8/freegenius/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.2.8/freegenius/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.2.8/freegenius/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.2.8/freegenius/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.2.8/freegenius/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.2.8/freegenius/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.2.8/freegenius/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.2.8/freegenius/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.2.8/freegenius/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.2.8/freegenius/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.2.8/freegenius/plugins/execute computing tasks.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.2.8/freegenius/plugins/execute termux command.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.2.8/freegenius/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.2.8/freegenius/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.2.8/freegenius/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.2.8/freegenius/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.2.8/freegenius/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.2.8/freegenius/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.2.8/freegenius/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.2.8/freegenius/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.2.8/freegenius/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.2.8/freegenius/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.2.8/freegenius/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1165 2024-05-02 19:22:09.000000 freegenius-0.2.8/freegenius/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.2.8/freegenius/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.2.8/freegenius/plugins/search sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.2.8/freegenius/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.2.8/freegenius/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.2.8/freegenius/plugins/send tweet.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.2.8/freegenius/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.2.8/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.2.8/freegenius/qt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.2.8/freegenius/rag.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      872 2024-05-05 16:16:42.000000 freegenius-0.2.8/freegenius/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.2.8/freegenius/servers.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.2.8/freegenius/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.231193 freegenius-0.2.8/freegenius/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.2.8/freegenius/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.239193 freegenius-0.2.8/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   113539 2024-05-04 15:44:12.000000 freegenius-0.2.8/freegenius/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    30152 2024-05-03 15:57:52.000000 freegenius-0.2.8/freegenius/utils/call_chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17682 2024-05-03 15:59:20.000000 freegenius-0.2.8/freegenius/utils/call_gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21380 2024-05-03 15:52:00.000000 freegenius-0.2.8/freegenius/utils/call_groq.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    25047 2024-05-03 16:02:40.000000 freegenius-0.2.8/freegenius/utils/call_llamacpp.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.2.8/freegenius/utils/call_llm.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19102 2024-05-03 16:04:26.000000 freegenius-0.2.8/freegenius/utils/call_ollama.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18528 2024-05-04 13:26:06.000000 freegenius-0.2.8/freegenius/utils/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.2.8/freegenius/utils/config_tools.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.2.8/freegenius/utils/download.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.2.8/freegenius/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4976 2024-05-04 08:21:49.000000 freegenius-0.2.8/freegenius/utils/ollama_models.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.2.8/freegenius/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.2.8/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.2.8/freegenius/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.2.8/freegenius/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.2.8/freegenius/utils/python_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    51559 2024-05-04 10:54:38.000000 freegenius-0.2.8/freegenius/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.2.8/freegenius/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.2.8/freegenius/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.2.8/freegenius/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.2.8/freegenius/utils/sttLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.2.8/freegenius/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.2.8/freegenius/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.2.8/freegenius/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4353 2024-05-02 17:22:30.000000 freegenius-0.2.8/freegenius/utils/tool_plugins.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11304 2024-05-04 13:53:35.000000 freegenius-0.2.8/freegenius/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9152 2024-05-04 15:43:23.000000 freegenius-0.2.8/freegenius/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4721 2024-05-04 10:56:37.000000 freegenius-0.2.8/freegenius/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-05 16:20:09.239193 freegenius-0.2.8/freegenius.egg-info/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14931 2024-05-05 16:20:08.000000 freegenius-0.2.8/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-05-05 16:20:09.000000 freegenius-0.2.8/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-05-05 16:20:08.000000 freegenius-0.2.8/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-05-05 16:20:08.000000 freegenius-0.2.8/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      873 2024-05-05 16:20:08.000000 freegenius-0.2.8/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-05-05 16:20:08.000000 freegenius-0.2.8/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-05-05 16:20:09.239193 freegenius-0.2.8/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10460 2024-05-05 16:10:10.000000 freegenius-0.2.8/setup.py
```

### Comparing `freegenius-0.2.7/PKG-INFO` & `freegenius-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.2.7
+Version: 0.2.8
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
@@ -18,16 +18,34 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <3.12
-Requires-Dist: openai==1.19.0
+Requires-Dist: llama-cpp-python[server]==0.2.69
+Requires-Dist: ollama==0.1.9
 Requires-Dist: groq==0.5.0
+Requires-Dist: openai==1.25.1
+Requires-Dist: google-cloud-aiplatform==1.50.0
+Requires-Dist: pyautogen[autobuild,retrievechat]==0.2.27
+Requires-Dist: transformers==4.40.1
+Requires-Dist: torch==2.3.0
+Requires-Dist: torchaudio==2.3.0
+Requires-Dist: torchvision==0.18.0
+Requires-Dist: sentence-transformers==2.7.0
+Requires-Dist: chromadb==0.5.0
+Requires-Dist: autogenstudio==0.0.56
+Requires-Dist: soundfile==0.12.1
+Requires-Dist: sounddevice==0.4.6
+Requires-Dist: elevenlabs==1.2.1
+Requires-Dist: huggingface-hub==0.23.0
+Requires-Dist: langchain==0.1.17
+Requires-Dist: langchain_openai==0.1.6
+Requires-Dist: guidance==0.1.13
 Requires-Dist: requests
 Requires-Dist: argparse
 Requires-Dist: pendulum
 Requires-Dist: folium
 Requires-Dist: seaborn[stats]
 Requires-Dist: sympy
 Requires-Dist: numpy
@@ -38,56 +56,39 @@
 Requires-Dist: geocoder
 Requires-Dist: googlesearch-python
 Requires-Dist: art
 Requires-Dist: apsw
 Requires-Dist: gTTS
 Requires-Dist: google-cloud-speech
 Requires-Dist: google-cloud-texttospeech
-Requires-Dist: google-cloud-aiplatform==1.47.0
 Requires-Dist: pywhatkit
 Requires-Dist: yt-dlp
 Requires-Dist: rembg
 Requires-Dist: qrcode
 Requires-Dist: pyperclip
 Requires-Dist: colorama
 Requires-Dist: pillow
 Requires-Dist: docker
 Requires-Dist: einops
-Requires-Dist: transformers==4.40.1
-Requires-Dist: torch==2.2.2
-Requires-Dist: torchvision==0.17.2
-Requires-Dist: sentence-transformers
-Requires-Dist: chromadb==0.4.24
 Requires-Dist: unstructured[all-docs]
-Requires-Dist: pyautogen[autobuild,retrievechat]==0.2.24
-Requires-Dist: autogenstudio==0.0.56
 Requires-Dist: tiktoken
 Requires-Dist: pygame
 Requires-Dist: PySide6
 Requires-Dist: feedparser
 Requires-Dist: html2text
 Requires-Dist: pypdf
 Requires-Dist: PyMuPDF
 Requires-Dist: yfinance
 Requires-Dist: setuptools-rust
 Requires-Dist: SpeechRecognition
 Requires-Dist: openai-whisper
-Requires-Dist: soundfile==0.12.1
-Requires-Dist: sounddevice==0.4.6
-Requires-Dist: elevenlabs==1.0.3
-Requires-Dist: ollama==0.1.8
-Requires-Dist: llama-cpp-python[server]==0.2.61
-Requires-Dist: huggingface-hub
-Requires-Dist: langchain==0.1.13
-Requires-Dist: langchain_openai==0.1.3
 Requires-Dist: pydub
 Requires-Dist: stable-diffusion-cpp-python
 Requires-Dist: pytz
 Requires-Dist: geopy
-Requires-Dist: guidance==0.1.13
 
 # FreeGenius AI
 
 FreeGenius AI is an ambitious project sparked by the pioneering work of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). It's designed with the primary objective of offering a comprehensive suite of AI solutions that mirror the capabilities of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). However, FreeGenius AI is remarkably different in that all core features are completely free, and it doesn't require the use of an OpenAI key.
 
 As with [LetMeDoIt AI](https://github.com/eliranwong/letmedoit), FreeGenius AI is designed to be capable of engaging in intuitive conversations, executing codes, providing up-to-date information, and performing a wide range of tasks. It's designed to learn, adapt, and grow with the user, offering personalized experiences and interactions.
```

### Comparing `freegenius-0.2.7/freegenius/README.md` & `freegenius-0.2.8/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/__init__.py` & `freegenius-0.2.8/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/audio/notification1.mp3` & `freegenius-0.2.8/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/audio/notification1_mild.mp3` & `freegenius-0.2.8/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/audio/notification2.mp3` & `freegenius-0.2.8/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/audio/notification2_mild.mp3` & `freegenius-0.2.8/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/autoassist.py` & `freegenius-0.2.8/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/autobuilder.py` & `freegenius-0.2.8/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/autoretriever.py` & `freegenius-0.2.8/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/chatgpt.py` & `freegenius-0.2.8/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/codey.py` & `freegenius-0.2.8/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/commandprompt.py` & `freegenius-0.2.8/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/eTextEdit.py` & `freegenius-0.2.8/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/geminipro.py` & `freegenius-0.2.8/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/geminiprovision.py` & `freegenius-0.2.8/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/groqchat.py` & `freegenius-0.2.8/freegenius/groqchat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/gui/chatgui.py` & `freegenius-0.2.8/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/gui/worker.py` & `freegenius-0.2.8/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/icons/FreeGenius.ico` & `freegenius-0.2.8/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/icons/FreeGenius.png` & `freegenius-0.2.8/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/icons/FreeGenius_original.png` & `freegenius-0.2.8/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/icons/ai.png` & `freegenius-0.2.8/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/icons/ai_original.png` & `freegenius-0.2.8/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/llamacpp.py` & `freegenius-0.2.8/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.2.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/main.py` & `freegenius-0.2.8/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/ollamachat.py` & `freegenius-0.2.8/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/palm2.py` & `freegenius-0.2.8/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.2.8/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.2.8/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/000_check_vlc.py` & `freegenius-0.2.8/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/add calendar event.py` & `freegenius-0.2.8/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/aliases.py` & `freegenius-0.2.8/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/analyze audio.py` & `freegenius-0.2.8/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/analyze files.py` & `freegenius-0.2.8/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/analyze images.py` & `freegenius-0.2.8/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/analyze web content.py` & `freegenius-0.2.8/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/auto correct python code.py` & `freegenius-0.2.8/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/awesome prompts.py` & `freegenius-0.2.8/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/character analysis.py` & `freegenius-0.2.8/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/chat.py` & `freegenius-0.2.8/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/contexts.py` & `freegenius-0.2.8/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/counselling.py` & `freegenius-0.2.8/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/create ai assistants.py` & `freegenius-0.2.8/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/create images.py` & `freegenius-0.2.8/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/create maps.py` & `freegenius-0.2.8/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/create qrcode.py` & `freegenius-0.2.8/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/create statistical graphics.py` & `freegenius-0.2.8/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/dates and times.py` & `freegenius-0.2.8/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/download youtube or web content.py` & `freegenius-0.2.8/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/edit text.py` & `freegenius-0.2.8/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/execute computing tasks.py` & `freegenius-0.2.8/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/execute termux command.py` & `freegenius-0.2.8/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/global finance.py` & `freegenius-0.2.8/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/improve British English.py` & `freegenius-0.2.8/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/input suggestions.py` & `freegenius-0.2.8/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/install python package.py` & `freegenius-0.2.8/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/integrate google searches.py` & `freegenius-0.2.8/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/memory.py` & `freegenius-0.2.8/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/modify images.py` & `freegenius-0.2.8/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/open web browser.py` & `freegenius-0.2.8/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/pronounce words.py` & `freegenius-0.2.8/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/remove image background.py` & `freegenius-0.2.8/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/search chat records.py` & `freegenius-0.2.8/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/search financial data.py` & `freegenius-0.2.8/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/search latest news.py` & `freegenius-0.2.8/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/search sqlite.py` & `freegenius-0.2.8/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/search weather info.py` & `freegenius-0.2.8/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/send email.py` & `freegenius-0.2.8/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/send tweet.py` & `freegenius-0.2.8/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.2.8/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.2.8/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/rag.py` & `freegenius-0.2.8/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/servers.py` & `freegenius-0.2.8/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/systemtray.py` & `freegenius-0.2.8/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/assistant.py` & `freegenius-0.2.8/freegenius/utils/assistant.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/call_chatgpt.py` & `freegenius-0.2.8/freegenius/utils/call_chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/call_gemini.py` & `freegenius-0.2.8/freegenius/utils/call_gemini.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/call_groq.py` & `freegenius-0.2.8/freegenius/utils/call_groq.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/call_llamacpp.py` & `freegenius-0.2.8/freegenius/utils/call_llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/call_llm.py` & `freegenius-0.2.8/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/call_ollama.py` & `freegenius-0.2.8/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/config_essential.py` & `freegenius-0.2.8/freegenius/utils/config_essential.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/config_tools.py` & `freegenius-0.2.8/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/download.py` & `freegenius-0.2.8/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/get_path_prompt.py` & `freegenius-0.2.8/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/ollama_models.py` & `freegenius-0.2.8/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/promptValidator.py` & `freegenius-0.2.8/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.2.8/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.2.8/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/prompts.py` & `freegenius-0.2.8/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/python_utils.py` & `freegenius-0.2.8/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/shared_utils.py` & `freegenius-0.2.8/freegenius/utils/shared_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/shortcuts.py` & `freegenius-0.2.8/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/single_prompt.py` & `freegenius-0.2.8/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.2.8/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/sttLanguages.py` & `freegenius-0.2.8/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.2.8/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.2.8/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/text_utils.py` & `freegenius-0.2.8/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/tool_plugins.py` & `freegenius-0.2.8/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/ttsLanguages.py` & `freegenius-0.2.8/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/tts_utils.py` & `freegenius-0.2.8/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius/utils/vlc_utils.py` & `freegenius-0.2.8/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius.egg-info/PKG-INFO` & `freegenius-0.2.8/freegenius.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.2.7
+Version: 0.2.8
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
@@ -18,16 +18,34 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <3.12
-Requires-Dist: openai==1.19.0
+Requires-Dist: llama-cpp-python[server]==0.2.69
+Requires-Dist: ollama==0.1.9
 Requires-Dist: groq==0.5.0
+Requires-Dist: openai==1.25.1
+Requires-Dist: google-cloud-aiplatform==1.50.0
+Requires-Dist: pyautogen[autobuild,retrievechat]==0.2.27
+Requires-Dist: transformers==4.40.1
+Requires-Dist: torch==2.3.0
+Requires-Dist: torchaudio==2.3.0
+Requires-Dist: torchvision==0.18.0
+Requires-Dist: sentence-transformers==2.7.0
+Requires-Dist: chromadb==0.5.0
+Requires-Dist: autogenstudio==0.0.56
+Requires-Dist: soundfile==0.12.1
+Requires-Dist: sounddevice==0.4.6
+Requires-Dist: elevenlabs==1.2.1
+Requires-Dist: huggingface-hub==0.23.0
+Requires-Dist: langchain==0.1.17
+Requires-Dist: langchain_openai==0.1.6
+Requires-Dist: guidance==0.1.13
 Requires-Dist: requests
 Requires-Dist: argparse
 Requires-Dist: pendulum
 Requires-Dist: folium
 Requires-Dist: seaborn[stats]
 Requires-Dist: sympy
 Requires-Dist: numpy
@@ -38,56 +56,39 @@
 Requires-Dist: geocoder
 Requires-Dist: googlesearch-python
 Requires-Dist: art
 Requires-Dist: apsw
 Requires-Dist: gTTS
 Requires-Dist: google-cloud-speech
 Requires-Dist: google-cloud-texttospeech
-Requires-Dist: google-cloud-aiplatform==1.47.0
 Requires-Dist: pywhatkit
 Requires-Dist: yt-dlp
 Requires-Dist: rembg
 Requires-Dist: qrcode
 Requires-Dist: pyperclip
 Requires-Dist: colorama
 Requires-Dist: pillow
 Requires-Dist: docker
 Requires-Dist: einops
-Requires-Dist: transformers==4.40.1
-Requires-Dist: torch==2.2.2
-Requires-Dist: torchvision==0.17.2
-Requires-Dist: sentence-transformers
-Requires-Dist: chromadb==0.4.24
 Requires-Dist: unstructured[all-docs]
-Requires-Dist: pyautogen[autobuild,retrievechat]==0.2.24
-Requires-Dist: autogenstudio==0.0.56
 Requires-Dist: tiktoken
 Requires-Dist: pygame
 Requires-Dist: PySide6
 Requires-Dist: feedparser
 Requires-Dist: html2text
 Requires-Dist: pypdf
 Requires-Dist: PyMuPDF
 Requires-Dist: yfinance
 Requires-Dist: setuptools-rust
 Requires-Dist: SpeechRecognition
 Requires-Dist: openai-whisper
-Requires-Dist: soundfile==0.12.1
-Requires-Dist: sounddevice==0.4.6
-Requires-Dist: elevenlabs==1.0.3
-Requires-Dist: ollama==0.1.8
-Requires-Dist: llama-cpp-python[server]==0.2.61
-Requires-Dist: huggingface-hub
-Requires-Dist: langchain==0.1.13
-Requires-Dist: langchain_openai==0.1.3
 Requires-Dist: pydub
 Requires-Dist: stable-diffusion-cpp-python
 Requires-Dist: pytz
 Requires-Dist: geopy
-Requires-Dist: guidance==0.1.13
 
 # FreeGenius AI
 
 FreeGenius AI is an ambitious project sparked by the pioneering work of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). It's designed with the primary objective of offering a comprehensive suite of AI solutions that mirror the capabilities of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). However, FreeGenius AI is remarkably different in that all core features are completely free, and it doesn't require the use of an OpenAI key.
 
 As with [LetMeDoIt AI](https://github.com/eliranwong/letmedoit), FreeGenius AI is designed to be capable of engaging in intuitive conversations, executing codes, providing up-to-date information, and performing a wide range of tasks. It's designed to learn, adapt, and grow with the user, offering personalized experiences and interactions.
```

### Comparing `freegenius-0.2.7/freegenius.egg-info/SOURCES.txt` & `freegenius-0.2.8/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius.egg-info/entry_points.txt` & `freegenius-0.2.8/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.7/freegenius.egg-info/requires.txt` & `freegenius-0.2.8/freegenius.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,27 @@
-openai==1.19.0
+llama-cpp-python[server]==0.2.69
+ollama==0.1.9
 groq==0.5.0
+openai==1.25.1
+google-cloud-aiplatform==1.50.0
+pyautogen[autobuild,retrievechat]==0.2.27
+transformers==4.40.1
+torch==2.3.0
+torchaudio==2.3.0
+torchvision==0.18.0
+sentence-transformers==2.7.0
+chromadb==0.5.0
+autogenstudio==0.0.56
+soundfile==0.12.1
+sounddevice==0.4.6
+elevenlabs==1.2.1
+huggingface-hub==0.23.0
+langchain==0.1.17
+langchain_openai==0.1.6
+guidance==0.1.13
 requests
 argparse
 pendulum
 folium
 seaborn[stats]
 sympy
 numpy
@@ -14,49 +32,32 @@
 geocoder
 googlesearch-python
 art
 apsw
 gTTS
 google-cloud-speech
 google-cloud-texttospeech
-google-cloud-aiplatform==1.47.0
 pywhatkit
 yt-dlp
 rembg
 qrcode
 pyperclip
 colorama
 pillow
 docker
 einops
-transformers==4.40.1
-torch==2.2.2
-torchvision==0.17.2
-sentence-transformers
-chromadb==0.4.24
 unstructured[all-docs]
-pyautogen[autobuild,retrievechat]==0.2.24
-autogenstudio==0.0.56
 tiktoken
 pygame
 PySide6
 feedparser
 html2text
 pypdf
 PyMuPDF
 yfinance
 setuptools-rust
 SpeechRecognition
 openai-whisper
-soundfile==0.12.1
-sounddevice==0.4.6
-elevenlabs==1.0.3
-ollama==0.1.8
-llama-cpp-python[server]==0.2.61
-huggingface-hub
-langchain==0.1.13
-langchain_openai==0.1.3
 pydub
 stable-diffusion-cpp-python
 pytz
 geopy
-guidance==0.1.13
```

### Comparing `freegenius-0.2.7/setup.py` & `freegenius-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.2.07",
+    version="0.2.08",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

