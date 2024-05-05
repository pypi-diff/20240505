# Comparing `tmp/hepai-1.1.7.tar.gz` & `tmp/hepai-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hepai-1.1.7.tar", last modified: Thu Apr 25 14:44:30 2024, max compression
+gzip compressed data, was "hepai-1.1.8.tar", last modified: Sun May  5 08:52:45 2024, max compression
```

## Comparing `hepai-1.1.7.tar` & `hepai-1.1.8.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.330472 hepai-1.1.7/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      118 2022-10-28 08:51:38.000000 hepai-1.1.7/MANIFEST.in
--rw-r--r--   0 zzd       (1000) zzd       (1000)     5660 2024-04-25 14:44:30.330472 hepai-1.1.7/PKG-INFO
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4619 2024-03-26 09:59:20.000000 hepai-1.1.7/README.md
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1613 2024-04-17 15:09:40.000000 hepai-1.1.7/hai/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2201 2024-03-25 11:14:31.000000 hepai-1.1.7/hai/apis/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/basic/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       83 2023-10-24 09:29:42.000000 hepai-1.1.7/hai/apis/basic/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       55 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/basic/argparse.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      458 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/basic/base.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       54 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/basic/grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      122 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/basic/registry.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      141 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/basic/utils.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/hub/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-04 00:48:55.000000 hepai-1.1.7/hai/apis/hub/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      803 2022-10-08 09:52:47.000000 hepai-1.1.7/hai/apis/hub/hubs.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/modules/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/modules/ResNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1057 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/modules/ResNet/ResNet.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      415 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/modules/ResNet/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/modules/UNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      637 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/modules/UNet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2478 2022-09-22 09:20:00.000000 hepai-1.1.7/hai/apis/modules/UNet/argparse_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-09-02 00:21:08.000000 hepai-1.1.7/hai/apis/modules/UNet/evaluate_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4730 2022-09-03 22:56:22.000000 hepai-1.1.7/hai/apis/modules/UNet/predict_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     9139 2022-09-22 08:22:39.000000 hepai-1.1.7/hai/apis/modules/UNet/train_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3099 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/modules/UNet/unet_api.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/modules/YOLOv5/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      434 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/apis/modules/YOLOv5/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:54:43.000000 hepai-1.1.7/hai/apis/modules/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      103 2024-03-25 11:33:22.000000 hepai-1.1.7/hai/apis/openai_api.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/workers_api/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:36:18.000000 hepai-1.1.7/hai/apis/workers_api/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/workers_api/llm/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:22:46.000000 hepai-1.1.7/hai/apis/workers_api/llm/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2953 2023-11-09 05:34:58.000000 hepai-1.1.7/hai/apis/workers_api/llm/llm.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        3 2023-04-21 09:02:06.000000 hepai-1.1.7/hai/apis/workers_api/llm/tokenizer.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8679 2024-04-10 14:20:32.000000 hepai-1.1.7/hai/apis/workers_api/model.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/workers_api/nougat/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2024-03-08 06:44:02.000000 hepai-1.1.7/hai/apis/workers_api/nougat/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      470 2024-03-08 06:44:02.000000 hepai-1.1.7/hai/apis/workers_api/nougat/pdf_process.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/apis/workers_api/sam/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-08-07 05:23:27.000000 hepai-1.1.7/hai/apis/workers_api/sam/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2164 2023-10-12 04:36:05.000000 hepai-1.1.7/hai/apis/workers_api/sam/pre_process.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5139 2023-08-04 16:18:52.000000 hepai-1.1.7/hai/apis/workers_api/sam/seg_via_sam.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/configs/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/configs/Base/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:19:48.000000 hepai-1.1.7/hai/configs/Base/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      407 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/configs/Base/hai_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      112 2024-04-17 12:28:00.000000 hepai-1.1.7/hai/configs/CONST.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/configs/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      285 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/configs/uaii_deepsort_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2706 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/configs/uaii_seyolov5_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1476 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/configs/uaii_stream_config.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/configs/urls/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1752 2022-10-19 18:44:14.000000 hepai-1.1.7/hai/configs/urls/datasets.json
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      960 2022-10-19 20:40:27.000000 hepai-1.1.7/hai/configs/urls/hub_models.json
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      534 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/configs/visible_loader_config.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:42:32.000000 hepai-1.1.7/hai/modules/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/detection/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:41:52.000000 hepai-1.1.7/hai/modules/detection/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/exporter/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:29.000000 hepai-1.1.7/hai/modules/exporter/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/exporter/images_exporter/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5282 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/modules/exporter/images_exporter/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/loader/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:28.000000 hepai-1.1.7/hai/modules/loader/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/loader/images_loader/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1618 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/modules/loader/images_loader/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3346 2023-04-21 12:08:18.000000 hepai-1.1.7/hai/modules/loader/images_loader/dataloader.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    14091 2022-10-18 10:33:57.000000 hepai-1.1.7/hai/modules/loader/images_loader/dataset_torch.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    26952 2022-10-18 11:10:17.000000 hepai-1.1.7/hai/modules/loader/images_loader/datasets.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1446 2022-10-18 17:35:03.000000 hepai-1.1.7/hai/modules/model_hub.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/segmentation/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:56:25.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1573 2022-08-31 21:12:48.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/evaluate.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      842 2022-08-30 18:18:45.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/hubconf.py
--rwxrwxr-x   0 zzd       (1000) zzd       (1000)     3997 2022-08-30 18:18:45.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/predict.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8621 2022-08-31 21:12:32.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/train.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/unet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       29 2022-08-30 18:18:45.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1130 2022-08-30 18:18:45.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2602 2022-08-30 18:18:45.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-30 18:18:45.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2991 2022-10-08 08:56:24.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-30 18:18:45.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      533 2022-09-30 09:30:48.000000 hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:55:50.000000 hepai-1.1.7/hai/modules/segmentation/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/testor/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      166 2023-04-21 07:26:13.000000 hepai-1.1.7/hai/testor/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      189 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/testor/test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      495 2023-10-23 01:04:23.000000 hepai-1.1.7/hai/testor/test_ip_connectable.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      281 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/testor/test_module.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      965 2023-10-23 01:10:57.000000 hepai-1.1.7/hai/testor/test_request_model.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      406 2023-04-21 07:26:41.000000 hepai-1.1.7/hai/testor/testor.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       46 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/actuator/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2022-12-07 09:16:51.000000 hepai-1.1.7/hai/uaii/actuator/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      430 2022-12-07 09:20:22.000000 hepai-1.1.7/hai/uaii/actuator/trainer.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/cli/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:00:08.000000 hepai-1.1.7/hai/uaii/cli/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4118 2023-05-11 12:36:29.000000 hepai-1.1.7/hai/uaii/cli/cli_functions.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     9276 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/uaii/cli/cli_main.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/datasets/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       28 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/datasets/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3240 2023-04-21 12:05:26.000000 hepai-1.1.7/hai/uaii/datasets/dataloader.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8478 2024-03-08 06:41:21.000000 hepai-1.1.7/hai/uaii/datasets/dataset_utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    40434 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/datasets/datasets.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4673 2022-10-19 18:52:31.000000 hepai-1.1.7/hai/uaii/datasets/datasets_hub.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 12:05:05.000000 hepai-1.1.7/hai/uaii/datasets/uaii_loaders.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    13228 2024-04-25 14:36:27.000000 hepai-1.1.7/hai/uaii/hepai_object.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/registry/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      374 2022-09-22 05:57:37.000000 hepai-1.1.7/hai/uaii/registry/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5669 2023-04-04 04:04:35.000000 hepai-1.1.7/hai/uaii/registry/init_register.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    11103 2022-09-22 03:26:47.000000 hepai-1.1.7/hai/uaii/registry/registy.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       81 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/registry/testor.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/registry/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/registry/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/registry/utils/general.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/server/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1893 2022-12-02 17:03:40.000000 hepai-1.1.7/hai/uaii/server/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/server/grpc/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/grpc/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/server/grpc/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/grpc/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      517 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/grpc/example/grpc-client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1353 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/grpc/example/grpc-test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3163 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/grpc/example/hello_pb2.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2242 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/grpc/example/hello_pb2_grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     6022 2022-09-02 03:06:02.000000 hepai-1.1.7/hai/uaii/server/grpc/grpc_pb2.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3707 2022-10-18 10:41:24.000000 hepai-1.1.7/hai/uaii/server/grpc/grpc_pb2_grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5517 2022-09-02 04:56:59.000000 hepai-1.1.7/hai/uaii/server/grpc/grpc_secure_client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    10437 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/uaii/server/grpc/grpc_secure_server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     6172 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/grpc/grpc_xai_client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5648 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/grpc/grpc_xai_server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/server/nacos/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/server/nacos/nacos/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      184 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/nacos/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    47889 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/nacos/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      752 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/nacos/commons.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/nacos/exception.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1645 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/nacos/files.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2403 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/nacos/listener.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      624 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/nacos/params.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4363 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/nacos/timer.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1555 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/nacos-test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2388 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/nacos/request_test.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/server/socket/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/socket/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/server/socket/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/socket/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/socket/example/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      674 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/socket/example/server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2131 2022-09-02 03:01:13.000000 hepai-1.1.7/hai/uaii/server/socket/server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/socket/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/socket/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/socket/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/socket/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/socket/example/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      672 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/socket/example/server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2153 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/socket/server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.326472 hepai-1.1.7/hai/uaii/stream/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/stream/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1411 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/stream/base_input.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     7745 2023-04-21 07:34:39.000000 hepai-1.1.7/hai/uaii/stream/base_module.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2575 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/stream/base_output.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      354 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/stream/base_queue.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/stream/rabbit_qm.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    15802 2022-09-27 10:17:02.000000 hepai-1.1.7/hai/uaii/stream/stream.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4094 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/stream/streams.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    12294 2022-08-24 17:25:48.000000 hepai-1.1.7/hai/uaii/uaii_main.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.330472 hepai-1.1.7/hai/uaii/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.7/hai/uaii/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      921 2022-09-22 07:46:07.000000 hepai-1.1.7/hai/uaii/utils/arbitrary_import.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    17055 2023-04-21 12:06:51.000000 hepai-1.1.7/hai/uaii/utils/base_uaii.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    15290 2023-05-10 16:19:50.000000 hepai-1.1.7/hai/uaii/utils/config_loader.py
--rw-r--r--   0 zzd       (1000) zzd       (1000)     4472 2022-09-30 05:15:38.000000 hepai-1.1.7/hai/uaii/utils/fake_argparse.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1339 2024-04-17 17:05:41.000000 hepai-1.1.7/hai/uaii/utils/file_object.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4033 2024-04-17 14:56:21.000000 hepai-1.1.7/hai/uaii/utils/general.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5268 2023-10-24 09:29:02.000000 hepai-1.1.7/hai/uaii/utils/hai_hf_parser.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    18952 2023-06-29 12:25:38.000000 hepai-1.1.7/hai/uaii/utils/hf_argparser.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.330472 hepai-1.1.7/hai/uaii/worker/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-05-18 13:37:30.000000 hepai-1.1.7/hai/uaii/worker/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3414 2024-04-17 17:37:35.000000 hepai-1.1.7/hai/uaii/worker/base_worker_model.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3070 2024-03-27 12:20:34.000000 hepai-1.1.7/hai/uaii/worker/run_worker.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       65 2023-05-18 13:37:30.000000 hepai-1.1.7/hai/uaii/worker/usage.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1561 2023-07-03 15:23:11.000000 hepai-1.1.7/hai/uaii/worker/utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    19483 2024-04-23 11:24:55.000000 hepai-1.1.7/hai/uaii/worker/worker.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      339 2024-04-25 14:36:41.000000 hepai-1.1.7/hai/version.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.330472 hepai-1.1.7/hepai/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      174 2024-04-17 15:09:16.000000 hepai-1.1.7/hepai/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-25 14:44:30.330472 hepai-1.1.7/hepai.egg-info/
--rw-r--r--   0 zzd       (1000) zzd       (1000)     5660 2024-04-25 14:44:30.000000 hepai-1.1.7/hepai.egg-info/PKG-INFO
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5303 2024-04-25 14:44:30.000000 hepai-1.1.7/hepai.egg-info/SOURCES.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2024-04-25 14:44:30.000000 hepai-1.1.7/hepai.egg-info/dependency_links.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       50 2024-04-25 14:44:30.000000 hepai-1.1.7/hepai.egg-info/entry_points.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       89 2024-04-25 14:44:30.000000 hepai-1.1.7/hepai.egg-info/requires.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       10 2024-04-25 14:44:30.000000 hepai-1.1.7/hepai.egg-info/top_level.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       38 2024-04-25 14:44:30.330472 hepai-1.1.7/setup.cfg
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4832 2024-04-17 12:22:34.000000 hepai-1.1.7/setup.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.174486 hepai-1.1.8/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      118 2022-10-28 08:51:38.000000 hepai-1.1.8/MANIFEST.in
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5406 2024-05-05 08:52:45.170486 hepai-1.1.8/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4619 2024-03-26 09:59:20.000000 hepai-1.1.8/README.md
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1613 2024-04-17 15:09:40.000000 hepai-1.1.8/hai/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2201 2024-03-25 11:14:31.000000 hepai-1.1.8/hai/apis/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/basic/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       83 2023-10-24 09:29:42.000000 hepai-1.1.8/hai/apis/basic/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       55 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/basic/argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      458 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/basic/base.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       54 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/basic/grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      122 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/basic/registry.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      141 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/basic/utils.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/hub/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-04 00:48:55.000000 hepai-1.1.8/hai/apis/hub/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      803 2022-10-08 09:52:47.000000 hepai-1.1.8/hai/apis/hub/hubs.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/modules/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/modules/ResNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1057 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/modules/ResNet/ResNet.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      415 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/modules/ResNet/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/modules/UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      637 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/modules/UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2478 2022-09-22 09:20:00.000000 hepai-1.1.8/hai/apis/modules/UNet/argparse_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-09-02 00:21:08.000000 hepai-1.1.8/hai/apis/modules/UNet/evaluate_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4730 2022-09-03 22:56:22.000000 hepai-1.1.8/hai/apis/modules/UNet/predict_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9139 2022-09-22 08:22:39.000000 hepai-1.1.8/hai/apis/modules/UNet/train_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3099 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/modules/UNet/unet_api.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/modules/YOLOv5/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      434 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/apis/modules/YOLOv5/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:54:43.000000 hepai-1.1.8/hai/apis/modules/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      103 2024-03-25 11:33:22.000000 hepai-1.1.8/hai/apis/openai_api.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/workers_api/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:36:18.000000 hepai-1.1.8/hai/apis/workers_api/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/workers_api/llm/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:22:46.000000 hepai-1.1.8/hai/apis/workers_api/llm/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2953 2023-11-09 05:34:58.000000 hepai-1.1.8/hai/apis/workers_api/llm/llm.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        3 2023-04-21 09:02:06.000000 hepai-1.1.8/hai/apis/workers_api/llm/tokenizer.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8679 2024-04-10 14:20:32.000000 hepai-1.1.8/hai/apis/workers_api/model.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/workers_api/nougat/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2024-03-08 06:44:02.000000 hepai-1.1.8/hai/apis/workers_api/nougat/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      470 2024-03-08 06:44:02.000000 hepai-1.1.8/hai/apis/workers_api/nougat/pdf_process.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/apis/workers_api/sam/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-08-07 05:23:27.000000 hepai-1.1.8/hai/apis/workers_api/sam/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2164 2023-10-12 04:36:05.000000 hepai-1.1.8/hai/apis/workers_api/sam/pre_process.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5139 2023-08-04 16:18:52.000000 hepai-1.1.8/hai/apis/workers_api/sam/seg_via_sam.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/configs/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.166486 hepai-1.1.8/hai/configs/Base/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:19:48.000000 hepai-1.1.8/hai/configs/Base/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      407 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/configs/Base/hai_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      112 2024-04-17 12:28:00.000000 hepai-1.1.8/hai/configs/CONST.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/configs/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      285 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/configs/uaii_deepsort_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2706 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/configs/uaii_seyolov5_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1476 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/configs/uaii_stream_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/configs/urls/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1752 2022-10-19 18:44:14.000000 hepai-1.1.8/hai/configs/urls/datasets.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      960 2022-10-19 20:40:27.000000 hepai-1.1.8/hai/configs/urls/hub_models.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      534 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/configs/visible_loader_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:42:32.000000 hepai-1.1.8/hai/modules/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/detection/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:41:52.000000 hepai-1.1.8/hai/modules/detection/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:29.000000 hepai-1.1.8/hai/modules/exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/exporter/images_exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5282 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/modules/exporter/images_exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:28.000000 hepai-1.1.8/hai/modules/loader/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/loader/images_loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1618 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/modules/loader/images_loader/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3346 2023-04-21 12:08:18.000000 hepai-1.1.8/hai/modules/loader/images_loader/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    14091 2022-10-18 10:33:57.000000 hepai-1.1.8/hai/modules/loader/images_loader/dataset_torch.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    26952 2022-10-18 11:10:17.000000 hepai-1.1.8/hai/modules/loader/images_loader/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1446 2022-10-18 17:35:03.000000 hepai-1.1.8/hai/modules/model_hub.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/segmentation/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:56:25.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1573 2022-08-31 21:12:48.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/evaluate.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      842 2022-08-30 18:18:45.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/hubconf.py
+-rwxrwxr-x   0 zzd       (1000) zzd       (1000)     3997 2022-08-30 18:18:45.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/predict.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8621 2022-08-31 21:12:32.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/train.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/unet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       29 2022-08-30 18:18:45.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1130 2022-08-30 18:18:45.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2602 2022-08-30 18:18:45.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-30 18:18:45.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2991 2022-10-08 08:56:24.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-30 18:18:45.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      533 2022-09-30 09:30:48.000000 hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:55:50.000000 hepai-1.1.8/hai/modules/segmentation/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/testor/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      166 2023-04-21 07:26:13.000000 hepai-1.1.8/hai/testor/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      189 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/testor/test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      495 2023-10-23 01:04:23.000000 hepai-1.1.8/hai/testor/test_ip_connectable.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      281 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/testor/test_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      965 2023-10-23 01:10:57.000000 hepai-1.1.8/hai/testor/test_request_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      406 2023-04-21 07:26:41.000000 hepai-1.1.8/hai/testor/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       46 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/actuator/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2022-12-07 09:16:51.000000 hepai-1.1.8/hai/uaii/actuator/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      430 2022-12-07 09:20:22.000000 hepai-1.1.8/hai/uaii/actuator/trainer.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/cli/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:00:08.000000 hepai-1.1.8/hai/uaii/cli/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4118 2023-05-11 12:36:29.000000 hepai-1.1.8/hai/uaii/cli/cli_functions.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9276 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/uaii/cli/cli_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/datasets/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       28 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/datasets/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3240 2023-04-21 12:05:26.000000 hepai-1.1.8/hai/uaii/datasets/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8478 2024-03-08 06:41:21.000000 hepai-1.1.8/hai/uaii/datasets/dataset_utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    40434 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/datasets/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4673 2022-10-19 18:52:31.000000 hepai-1.1.8/hai/uaii/datasets/datasets_hub.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 12:05:05.000000 hepai-1.1.8/hai/uaii/datasets/uaii_loaders.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    13228 2024-04-30 04:48:24.000000 hepai-1.1.8/hai/uaii/hepai_object.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/registry/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      374 2022-09-22 05:57:37.000000 hepai-1.1.8/hai/uaii/registry/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5669 2023-04-04 04:04:35.000000 hepai-1.1.8/hai/uaii/registry/init_register.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    11103 2022-09-22 03:26:47.000000 hepai-1.1.8/hai/uaii/registry/registy.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       81 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/registry/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/registry/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/registry/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/registry/utils/general.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/server/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1893 2022-12-02 17:03:40.000000 hepai-1.1.8/hai/uaii/server/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/server/grpc/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/grpc/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/server/grpc/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/grpc/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      517 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/grpc/example/grpc-client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1353 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/grpc/example/grpc-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3163 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/grpc/example/hello_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2242 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/grpc/example/hello_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6022 2022-09-02 03:06:02.000000 hepai-1.1.8/hai/uaii/server/grpc/grpc_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3707 2022-10-18 10:41:24.000000 hepai-1.1.8/hai/uaii/server/grpc/grpc_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5517 2022-09-02 04:56:59.000000 hepai-1.1.8/hai/uaii/server/grpc/grpc_secure_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    10437 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/uaii/server/grpc/grpc_secure_server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6172 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/grpc/grpc_xai_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5648 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/grpc/grpc_xai_server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/server/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/server/nacos/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      184 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/nacos/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    47889 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/nacos/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      752 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/nacos/commons.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/nacos/exception.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1645 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/nacos/files.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2403 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/nacos/listener.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      624 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/nacos/params.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4363 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/nacos/timer.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1555 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/nacos-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2388 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/nacos/request_test.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/server/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/server/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      674 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2131 2022-09-02 03:01:13.000000 hepai-1.1.8/hai/uaii/server/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      672 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2153 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/stream/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/stream/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1411 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/stream/base_input.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     7745 2023-04-21 07:34:39.000000 hepai-1.1.8/hai/uaii/stream/base_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2575 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/stream/base_output.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      354 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/stream/base_queue.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/stream/rabbit_qm.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15802 2022-09-27 10:17:02.000000 hepai-1.1.8/hai/uaii/stream/stream.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4094 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/stream/streams.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    12294 2022-08-24 17:25:48.000000 hepai-1.1.8/hai/uaii/uaii_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.8/hai/uaii/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      921 2022-09-22 07:46:07.000000 hepai-1.1.8/hai/uaii/utils/arbitrary_import.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    17055 2023-04-21 12:06:51.000000 hepai-1.1.8/hai/uaii/utils/base_uaii.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15290 2023-05-10 16:19:50.000000 hepai-1.1.8/hai/uaii/utils/config_loader.py
+-rw-r--r--   0 zzd       (1000) zzd       (1000)     4472 2022-09-30 05:15:38.000000 hepai-1.1.8/hai/uaii/utils/fake_argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1339 2024-04-17 17:05:41.000000 hepai-1.1.8/hai/uaii/utils/file_object.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4033 2024-04-17 14:56:21.000000 hepai-1.1.8/hai/uaii/utils/general.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5268 2023-10-24 09:29:02.000000 hepai-1.1.8/hai/uaii/utils/hai_hf_parser.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    18952 2023-06-29 12:25:38.000000 hepai-1.1.8/hai/uaii/utils/hf_argparser.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hai/uaii/worker/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-05-18 13:37:30.000000 hepai-1.1.8/hai/uaii/worker/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3414 2024-04-17 17:37:35.000000 hepai-1.1.8/hai/uaii/worker/base_worker_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3070 2024-03-27 12:20:34.000000 hepai-1.1.8/hai/uaii/worker/run_worker.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       65 2023-05-18 13:37:30.000000 hepai-1.1.8/hai/uaii/worker/usage.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1561 2023-07-03 15:23:11.000000 hepai-1.1.8/hai/uaii/worker/utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    19884 2024-04-30 04:03:44.000000 hepai-1.1.8/hai/uaii/worker/worker.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      339 2024-05-05 08:51:56.000000 hepai-1.1.8/hai/version.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hepai/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      174 2024-04-17 15:09:16.000000 hepai-1.1.8/hepai/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-05-05 08:52:45.170486 hepai-1.1.8/hepai.egg-info/
+-rw-r--r--   0 zzd       (1000) zzd       (1000)     5406 2024-05-05 08:52:45.000000 hepai-1.1.8/hepai.egg-info/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5303 2024-05-05 08:52:45.000000 hepai-1.1.8/hepai.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2024-05-05 08:52:45.000000 hepai-1.1.8/hepai.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       50 2024-05-05 08:52:45.000000 hepai-1.1.8/hepai.egg-info/entry_points.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       97 2024-05-05 08:52:45.000000 hepai-1.1.8/hepai.egg-info/requires.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       10 2024-05-05 08:52:45.000000 hepai-1.1.8/hepai.egg-info/top_level.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       38 2024-05-05 08:52:45.174486 hepai-1.1.8/setup.cfg
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4832 2024-04-17 12:22:34.000000 hepai-1.1.8/setup.py
```

### Comparing `hepai-1.1.7/PKG-INFO` & `hepai-1.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hepai
-Version: 1.1.7
+Version: 1.1.8
 Summary: High energy phscis Artificial Intelligence plateform, HAI.
 Home-page: https://github.com/zhangzhengde0225/hai
 Author: Zhengde Zhang
 Author-email: zdzhang@ihep.ac.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,25 +13,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
-Requires-Dist: damei
-Requires-Dist: easydict
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: pillow
-Requires-Dist: tqdm
-Requires-Dist: wandb
-Requires-Dist: grpcio-tools
-Requires-Dist: fastapi
-Requires-Dist: uvicorn
-Requires-Dist: openai
 
 
 [![Stars](https://img.shields.io/github/stars/zhangzhengde0225/CDNet)](
 https://github.com/zhangzhengde0225/hai)
 [![Open issue](https://img.shields.io/github/issues/zhangzhengde0225/CDNet)](
 https://github.com/zhangzhengde0225/hai/issues)
 <!-- [![Datasets](https://img.shields.io/static/v1?label=Download&message=datasets&color=green)](
```

#### html2text {}

```diff
@@ -1,40 +1,37 @@
-Metadata-Version: 2.1 Name: hepai Version: 1.1.7 Summary: High energy phscis
+Metadata-Version: 2.1 Name: hepai Version: 1.1.8 Summary: High energy phscis
 Artificial Intelligence plateform, HAI. Home-page: https://github.com/
 zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@ihep.ac.cn
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown Requires-Dist: damei Requires-Dist:
-easydict Requires-Dist: numpy Requires-Dist: opencv-python Requires-Dist:
-pillow Requires-Dist: tqdm Requires-Dist: wandb Requires-Dist: grpcio-tools
-Requires-Dist: fastapi Requires-Dist: uvicorn Requires-Dist: openai [![Stars]
-(https://img.shields.io/github/stars/zhangzhengde0225/CDNet)]( https://
-github.com/zhangzhengde0225/hai) [![Open issue](https://img.shields.io/github/
-issues/zhangzhengde0225/CDNet)]( https://github.com/zhangzhengde0225/hai/
-issues) #### English | [ç®ä½ä¸­æ](https://github.com/zhangzhengde0225/hai/
-blob/main/docs/readme_zh_cn.md) # HepAI Library This is [HepAI](https://
-ai.ihep.ac.cn) python library, the AI platform can accelerate scientific
-research in multidisciplinary scenarios, simplify model iteration and flow, and
-is a common infrastructure for the development of AI algorithms and
-applications. The HepAI platform itself is a software system that carries AI
-algorithm models, provides AI computing power, connects data channels, and
-conducts AI training. The HepAI framework integrates classic and state-of-the-
-art (SOTA) artificial intelligence algorithms in the field of high-energy
-physics. One can access related algorithm models, datasets, and computational
-resources through a unified interface, making the application of AI simple and
-efficient. NNeewwss + [2024.03.26] v1.0.21 Make LLM request like OpenAI via HepAI
-object. + [2023.10.24] v1.0.18
-æ¥å¥dalleæçå¾æ¨¡åï¼è°ç¨æ¹æ³æç¨è§[æ­¤å¤](https://
-note.ihep.ac.cn/s/EG60U1Rtf)ã + [2023.04.21] v1.0.7éè¿hepaiä½¿ç¨GPT-
-3.5ï¼[hepai_api.md](docs/hepai_api.md). + [2023.02.09]
+Description-Content-Type: text/markdown [![Stars](https://img.shields.io/
+github/stars/zhangzhengde0225/CDNet)]( https://github.com/zhangzhengde0225/hai)
+[![Open issue](https://img.shields.io/github/issues/zhangzhengde0225/CDNet)]
+( https://github.com/zhangzhengde0225/hai/issues) #### English | [ç®ä½ä¸­æ]
+(https://github.com/zhangzhengde0225/hai/blob/main/docs/readme_zh_cn.md) #
+HepAI Library This is [HepAI](https://ai.ihep.ac.cn) python library, the AI
+platform can accelerate scientific research in multidisciplinary scenarios,
+simplify model iteration and flow, and is a common infrastructure for the
+development of AI algorithms and applications. The HepAI platform itself is a
+software system that carries AI algorithm models, provides AI computing power,
+connects data channels, and conducts AI training. The HepAI framework
+integrates classic and state-of-the-art (SOTA) artificial intelligence
+algorithms in the field of high-energy physics. One can access related
+algorithm models, datasets, and computational resources through a unified
+interface, making the application of AI simple and efficient. NNeewwss +
+[2024.03.26] v1.0.21 Make LLM request like OpenAI via HepAI object. +
+[2023.10.24] v1.0.18 æ¥å¥dalleæçå¾æ¨¡åï¼è°ç¨æ¹æ³æç¨è§[æ­¤å¤]
+(https://note.ihep.ac.cn/s/EG60U1Rtf)ã + [2023.04.21]
+v1.0.7éè¿hepaiä½¿ç¨GPT-3.5ï¼[hepai_api.md](docs/hepai_api.md). +
+[2023.02.09]
 åºäºChatGPTç**HaiChatGPT**å·²ä¸çº¿ï¼ä½¿ç¨ç®åï¼æ éæ¢¯å­ï¼è¯¦ææ¥çï¼
 [HaiChatGPT](https://code.ihep.ac.cn/zdzhang/haichatgpt). + [2023.01.16]
 åä¸ºNPUæå¡å¨ä¸æ¶ï¼å¦æç®æ³å½äº§åéæ±ï¼è¯·æ¥é[NPUææ¡£]
 (docs/computing_power/npu_power_doc.md)ã + [2022.10.20] HAI v1.0.6-Beta
 ç¬¬ä¸ä¸ªæµè¯çæ¬åå¸ï¼4ä¸ªç®æ³å3ä¸ªæ°æ®é + [2022.08.23] HAI
 v1.0.0 TTuuttoorriiaallss [Quick Start to Using HepAI on Computing Clusters](docs/
 quickstart_hpc.md) [Reconstruction and identification of atmospheric neutrinos
```

### Comparing `hepai-1.1.7/README.md` & `hepai-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/__init__.py` & `hepai-1.1.8/hai/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/__init__.py` & `hepai-1.1.8/hai/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/hub/hubs.py` & `hepai-1.1.8/hai/apis/hub/hubs.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/modules/ResNet/ResNet.py` & `hepai-1.1.8/hai/apis/modules/ResNet/ResNet.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/modules/UNet/__init__.py` & `hepai-1.1.8/hai/apis/modules/UNet/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/modules/UNet/argparse_config.py` & `hepai-1.1.8/hai/apis/modules/UNet/argparse_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/modules/UNet/evaluate_api.py` & `hepai-1.1.8/hai/apis/modules/UNet/evaluate_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/modules/UNet/predict_api.py` & `hepai-1.1.8/hai/apis/modules/UNet/predict_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/modules/UNet/train_api.py` & `hepai-1.1.8/hai/apis/modules/UNet/train_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/modules/UNet/unet_api.py` & `hepai-1.1.8/hai/apis/modules/UNet/unet_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/workers_api/llm/llm.py` & `hepai-1.1.8/hai/apis/workers_api/llm/llm.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/workers_api/model.py` & `hepai-1.1.8/hai/apis/workers_api/model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/workers_api/sam/pre_process.py` & `hepai-1.1.8/hai/apis/workers_api/sam/pre_process.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/apis/workers_api/sam/seg_via_sam.py` & `hepai-1.1.8/hai/apis/workers_api/sam/seg_via_sam.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/configs/uaii_seyolov5_config.py` & `hepai-1.1.8/hai/configs/uaii_seyolov5_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/configs/uaii_stream_config.py` & `hepai-1.1.8/hai/configs/uaii_stream_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/configs/urls/datasets.json` & `hepai-1.1.8/hai/configs/urls/datasets.json`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/configs/urls/hub_models.json` & `hepai-1.1.8/hai/configs/urls/hub_models.json`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/configs/visible_loader_config.py` & `hepai-1.1.8/hai/configs/visible_loader_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/exporter/images_exporter/__init__.py` & `hepai-1.1.8/hai/modules/exporter/images_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/loader/images_loader/__init__.py` & `hepai-1.1.8/hai/modules/loader/images_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/loader/images_loader/dataloader.py` & `hepai-1.1.8/hai/modules/loader/images_loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/loader/images_loader/dataset_torch.py` & `hepai-1.1.8/hai/modules/loader/images_loader/dataset_torch.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/loader/images_loader/datasets.py` & `hepai-1.1.8/hai/modules/loader/images_loader/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/model_hub.py` & `hepai-1.1.8/hai/modules/model_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/evaluate.py` & `hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/evaluate.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/hubconf.py` & `hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/hubconf.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/predict.py` & `hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/predict.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/train.py` & `hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/train.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py` & `hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py` & `hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py` & `hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py` & `hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/modules/segmentation/Pytorch_UNet/utils/utils.py` & `hepai-1.1.8/hai/modules/segmentation/Pytorch_UNet/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/testor/test_request_model.py` & `hepai-1.1.8/hai/testor/test_request_model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/cli/cli_functions.py` & `hepai-1.1.8/hai/uaii/cli/cli_functions.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/cli/cli_main.py` & `hepai-1.1.8/hai/uaii/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/datasets/dataloader.py` & `hepai-1.1.8/hai/uaii/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/datasets/dataset_utils.py` & `hepai-1.1.8/hai/uaii/datasets/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/datasets/datasets.py` & `hepai-1.1.8/hai/uaii/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/datasets/datasets_hub.py` & `hepai-1.1.8/hai/uaii/datasets/datasets_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/datasets/uaii_loaders.py` & `hepai-1.1.8/hai/uaii/datasets/uaii_loaders.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/hepai_object.py` & `hepai-1.1.8/hai/uaii/hepai_object.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/registry/init_register.py` & `hepai-1.1.8/hai/uaii/registry/init_register.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/registry/registy.py` & `hepai-1.1.8/hai/uaii/registry/registy.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/registry/utils/general.py` & `hepai-1.1.8/hai/uaii/registry/utils/general.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/__init__.py` & `hepai-1.1.8/hai/uaii/server/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/example/grpc-client.py` & `hepai-1.1.8/hai/uaii/server/grpc/example/grpc-client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/example/grpc-test.py` & `hepai-1.1.8/hai/uaii/server/grpc/example/grpc-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/example/hello_pb2.py` & `hepai-1.1.8/hai/uaii/server/grpc/example/hello_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/example/hello_pb2_grpc.py` & `hepai-1.1.8/hai/uaii/server/grpc/example/hello_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/grpc_pb2.py` & `hepai-1.1.8/hai/uaii/server/grpc/grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/grpc_pb2_grpc.py` & `hepai-1.1.8/hai/uaii/server/grpc/grpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/grpc_secure_client.py` & `hepai-1.1.8/hai/uaii/server/grpc/grpc_secure_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/grpc_secure_server.py` & `hepai-1.1.8/hai/uaii/server/grpc/grpc_secure_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/grpc_xai_client.py` & `hepai-1.1.8/hai/uaii/server/grpc/grpc_xai_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/grpc/grpc_xai_server.py` & `hepai-1.1.8/hai/uaii/server/grpc/grpc_xai_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/nacos/nacos/client.py` & `hepai-1.1.8/hai/uaii/server/nacos/nacos/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/nacos/nacos/commons.py` & `hepai-1.1.8/hai/uaii/server/nacos/nacos/commons.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/nacos/nacos/files.py` & `hepai-1.1.8/hai/uaii/server/nacos/nacos/files.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/nacos/nacos/listener.py` & `hepai-1.1.8/hai/uaii/server/nacos/nacos/listener.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/nacos/nacos/params.py` & `hepai-1.1.8/hai/uaii/server/nacos/nacos/params.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/nacos/nacos/timer.py` & `hepai-1.1.8/hai/uaii/server/nacos/nacos/timer.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/nacos/nacos-test.py` & `hepai-1.1.8/hai/uaii/server/nacos/nacos-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/nacos/request_test.py` & `hepai-1.1.8/hai/uaii/server/nacos/request_test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/socket/example/client.py` & `hepai-1.1.8/hai/uaii/server/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/socket/example/server.py` & `hepai-1.1.8/hai/uaii/server/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/server/socket/server.py` & `hepai-1.1.8/hai/uaii/server/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/socket/example/client.py` & `hepai-1.1.8/hai/uaii/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/socket/example/server.py` & `hepai-1.1.8/hai/uaii/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/socket/server.py` & `hepai-1.1.8/hai/uaii/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/stream/base_input.py` & `hepai-1.1.8/hai/uaii/stream/base_input.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/stream/base_module.py` & `hepai-1.1.8/hai/uaii/stream/base_module.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/stream/base_output.py` & `hepai-1.1.8/hai/uaii/stream/base_output.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/stream/stream.py` & `hepai-1.1.8/hai/uaii/stream/stream.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/stream/streams.py` & `hepai-1.1.8/hai/uaii/stream/streams.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/uaii_main.py` & `hepai-1.1.8/hai/uaii/uaii_main.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/utils/arbitrary_import.py` & `hepai-1.1.8/hai/uaii/utils/arbitrary_import.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/utils/base_uaii.py` & `hepai-1.1.8/hai/uaii/utils/base_uaii.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/utils/config_loader.py` & `hepai-1.1.8/hai/uaii/utils/config_loader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/utils/fake_argparse.py` & `hepai-1.1.8/hai/uaii/utils/fake_argparse.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/utils/file_object.py` & `hepai-1.1.8/hai/uaii/utils/file_object.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/utils/general.py` & `hepai-1.1.8/hai/uaii/utils/general.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/utils/hai_hf_parser.py` & `hepai-1.1.8/hai/uaii/utils/hai_hf_parser.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/utils/hf_argparser.py` & `hepai-1.1.8/hai/uaii/utils/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/worker/base_worker_model.py` & `hepai-1.1.8/hai/uaii/worker/base_worker_model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/worker/run_worker.py` & `hepai-1.1.8/hai/uaii/worker/run_worker.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/worker/utils.py` & `hepai-1.1.8/hai/uaii/worker/utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/hai/uaii/worker/worker.py` & `hepai-1.1.8/hai/uaii/worker/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import traceback
 import argparse
 # import dataclasses
 from dataclasses import dataclass, field
 import os, sys
 from pathlib import Path
 
-from fastapi import FastAPI, Request, BackgroundTasks, HTTPException
+from fastapi import FastAPI, Request, BackgroundTasks, HTTPException, APIRouter
 from fastapi.responses import StreamingResponse, JSONResponse, Response, FileResponse
 from starlette.requests import Request as StarletteRequest
 import requests
 import uvicorn
 
 import damei as dm 
 import atexit
@@ -393,15 +393,15 @@
     await model_semaphore.acquire()
     stream = params.get("stream", False)
     ok, data = app.worker.unified_gate(**params)
     if not ok:
         data = data if isinstance(data, str) else json.dumps(data)
         # print(model_semaphore)
         release_model_semaphore()
-        raise HTTPException(status_code=404, detail=data, background=background_tasks)
+        raise HTTPException(status_code=404, detail=data)
     background_tasks = BackgroundTasks()  # 背景任务
     background_tasks.add_task(release_model_semaphore)  # 释放锁
     if isinstance(data, Generator) and (stream is None or stream is False):
         logger.info(f"Get a generator from function: {params.get('function')}, auto set stream=True")
         stream = True
     if not stream:
         # 判断是不是文件路径
@@ -446,15 +446,15 @@
 
 
 @app.post("/worker_get_status")
 async def get_status(request: Request):
     return app.worker.get_status()
 
 
-def run_worker(model=None, worker_args=None, daemon=False, test=False, **kwargs):
+def run_worker(model=None, worker_args=None, extra_routers=None, daemon=False, test=False, **kwargs):
     args = worker_args or WorkerArgs()
     # print(f'worker args: {args}')
     if args.port == "auto":
         start_port = args.__dict__.get("start_port", 42902)
         args.port = auto_port(args.port, start=start_port)
     args.worker_address = auto_worker_address(args.worker_address, args.host, args.port)
     logger.info(f"Worker address: {args.worker_address}")
@@ -475,14 +475,20 @@
         no_register=args.no_register,
         permissions=args.permissions,
         description=args.description,
         author=args.author,
         )
     
     app.worker = worker
+    if extra_routers:
+        if isinstance(extra_routers, APIRouter):
+            extra_routers = [extra_routers]
+        for extra_router in extra_routers:
+            assert isinstance(extra_router, APIRouter), f"extra_router should be an instance of APIRouter: {extra_router}"
+            app.include_router(extra_router)
 
     logger.info(f"Controller address: {args.controller_address}")
 
     if daemon:
         logger.info(f"Daemon Worker address: {args.worker_address}")
         import threading
         t = threading.Thread(target=uvicorn.run, args=(app,), kwargs={
@@ -515,14 +521,15 @@
     def start(**kwargs):
         """
         运行一个hepai的worker
         :param model: BaseWorkerModel = None, 模型
         :param worker_args: WorkerArgs = None, worker的参数，可以由WorkerArgs类生成，会被下面的参数覆盖
         :param host: str = "0.0.0.0"  # worker的地址，0.0.0.0表示外部可访问，127.0.0.1表示只有本机可访问
         :param port: str = "auto"  # 默认从42902开始
+        :param extra_routers: List[APIRouter] = None,  # 额外的路由
         :param controller_address: str = "http://chat.ihep.ac.cn:42901"  # 控制器的地址
         :param worker_address: str = "auto"  # 默认是http://<ip>:<port>
         :param limit_model_concurrency: int = 5  # 限制模型的并发请求
         :param stream_interval: float = 0.  # 额外的流式响应间隔
         :param no_register: bool = False  # 不注册到控制器
         :param permissions: str = 'group: all'  # 模型的权限授予，分为用户和组，用;分隔
         """
```

### Comparing `hepai-1.1.7/hepai.egg-info/PKG-INFO` & `hepai-1.1.8/hepai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hepai
-Version: 1.1.7
+Version: 1.1.8
 Summary: High energy phscis Artificial Intelligence plateform, HAI.
 Home-page: https://github.com/zhangzhengde0225/hai
 Author: Zhengde Zhang
 Author-email: zdzhang@ihep.ac.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,25 +13,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
-Requires-Dist: damei
-Requires-Dist: easydict
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: pillow
-Requires-Dist: tqdm
-Requires-Dist: wandb
-Requires-Dist: grpcio-tools
-Requires-Dist: fastapi
-Requires-Dist: uvicorn
-Requires-Dist: openai
 
 
 [![Stars](https://img.shields.io/github/stars/zhangzhengde0225/CDNet)](
 https://github.com/zhangzhengde0225/hai)
 [![Open issue](https://img.shields.io/github/issues/zhangzhengde0225/CDNet)](
 https://github.com/zhangzhengde0225/hai/issues)
 <!-- [![Datasets](https://img.shields.io/static/v1?label=Download&message=datasets&color=green)](
```

#### html2text {}

```diff
@@ -1,40 +1,37 @@
-Metadata-Version: 2.1 Name: hepai Version: 1.1.7 Summary: High energy phscis
+Metadata-Version: 2.1 Name: hepai Version: 1.1.8 Summary: High energy phscis
 Artificial Intelligence plateform, HAI. Home-page: https://github.com/
 zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@ihep.ac.cn
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown Requires-Dist: damei Requires-Dist:
-easydict Requires-Dist: numpy Requires-Dist: opencv-python Requires-Dist:
-pillow Requires-Dist: tqdm Requires-Dist: wandb Requires-Dist: grpcio-tools
-Requires-Dist: fastapi Requires-Dist: uvicorn Requires-Dist: openai [![Stars]
-(https://img.shields.io/github/stars/zhangzhengde0225/CDNet)]( https://
-github.com/zhangzhengde0225/hai) [![Open issue](https://img.shields.io/github/
-issues/zhangzhengde0225/CDNet)]( https://github.com/zhangzhengde0225/hai/
-issues) #### English | [ç®ä½ä¸­æ](https://github.com/zhangzhengde0225/hai/
-blob/main/docs/readme_zh_cn.md) # HepAI Library This is [HepAI](https://
-ai.ihep.ac.cn) python library, the AI platform can accelerate scientific
-research in multidisciplinary scenarios, simplify model iteration and flow, and
-is a common infrastructure for the development of AI algorithms and
-applications. The HepAI platform itself is a software system that carries AI
-algorithm models, provides AI computing power, connects data channels, and
-conducts AI training. The HepAI framework integrates classic and state-of-the-
-art (SOTA) artificial intelligence algorithms in the field of high-energy
-physics. One can access related algorithm models, datasets, and computational
-resources through a unified interface, making the application of AI simple and
-efficient. NNeewwss + [2024.03.26] v1.0.21 Make LLM request like OpenAI via HepAI
-object. + [2023.10.24] v1.0.18
-æ¥å¥dalleæçå¾æ¨¡åï¼è°ç¨æ¹æ³æç¨è§[æ­¤å¤](https://
-note.ihep.ac.cn/s/EG60U1Rtf)ã + [2023.04.21] v1.0.7éè¿hepaiä½¿ç¨GPT-
-3.5ï¼[hepai_api.md](docs/hepai_api.md). + [2023.02.09]
+Description-Content-Type: text/markdown [![Stars](https://img.shields.io/
+github/stars/zhangzhengde0225/CDNet)]( https://github.com/zhangzhengde0225/hai)
+[![Open issue](https://img.shields.io/github/issues/zhangzhengde0225/CDNet)]
+( https://github.com/zhangzhengde0225/hai/issues) #### English | [ç®ä½ä¸­æ]
+(https://github.com/zhangzhengde0225/hai/blob/main/docs/readme_zh_cn.md) #
+HepAI Library This is [HepAI](https://ai.ihep.ac.cn) python library, the AI
+platform can accelerate scientific research in multidisciplinary scenarios,
+simplify model iteration and flow, and is a common infrastructure for the
+development of AI algorithms and applications. The HepAI platform itself is a
+software system that carries AI algorithm models, provides AI computing power,
+connects data channels, and conducts AI training. The HepAI framework
+integrates classic and state-of-the-art (SOTA) artificial intelligence
+algorithms in the field of high-energy physics. One can access related
+algorithm models, datasets, and computational resources through a unified
+interface, making the application of AI simple and efficient. NNeewwss +
+[2024.03.26] v1.0.21 Make LLM request like OpenAI via HepAI object. +
+[2023.10.24] v1.0.18 æ¥å¥dalleæçå¾æ¨¡åï¼è°ç¨æ¹æ³æç¨è§[æ­¤å¤]
+(https://note.ihep.ac.cn/s/EG60U1Rtf)ã + [2023.04.21]
+v1.0.7éè¿hepaiä½¿ç¨GPT-3.5ï¼[hepai_api.md](docs/hepai_api.md). +
+[2023.02.09]
 åºäºChatGPTç**HaiChatGPT**å·²ä¸çº¿ï¼ä½¿ç¨ç®åï¼æ éæ¢¯å­ï¼è¯¦ææ¥çï¼
 [HaiChatGPT](https://code.ihep.ac.cn/zdzhang/haichatgpt). + [2023.01.16]
 åä¸ºNPUæå¡å¨ä¸æ¶ï¼å¦æç®æ³å½äº§åéæ±ï¼è¯·æ¥é[NPUææ¡£]
 (docs/computing_power/npu_power_doc.md)ã + [2022.10.20] HAI v1.0.6-Beta
 ç¬¬ä¸ä¸ªæµè¯çæ¬åå¸ï¼4ä¸ªç®æ³å3ä¸ªæ°æ®é + [2022.08.23] HAI
 v1.0.0 TTuuttoorriiaallss [Quick Start to Using HepAI on Computing Clusters](docs/
 quickstart_hpc.md) [Reconstruction and identification of atmospheric neutrinos
```

### Comparing `hepai-1.1.7/hepai.egg-info/SOURCES.txt` & `hepai-1.1.8/hepai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hepai-1.1.7/setup.py` & `hepai-1.1.8/setup.py`

 * *Files identical despite different names*

