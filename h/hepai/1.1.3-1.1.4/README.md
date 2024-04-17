# Comparing `tmp/hepai-1.1.3.tar.gz` & `tmp/hepai-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hepai-1.1.3.tar", last modified: Sat Apr 13 15:08:51 2024, max compression
+gzip compressed data, was "hepai-1.1.4.tar", last modified: Wed Apr 17 17:36:59 2024, max compression
```

## Comparing `hepai-1.1.3.tar` & `hepai-1.1.4.tar`

### file list

```diff
@@ -1,205 +1,207 @@
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.308802 hepai-1.1.3/
--rw-r--r--   0 zzd      (58004) root         (0)      118 2023-05-18 07:14:07.000000 hepai-1.1.3/MANIFEST.in
--rw-r--r--   0 zzd      (58004) root         (0)     5402 2024-04-13 15:08:51.308802 hepai-1.1.3/PKG-INFO
--rw-r--r--   0 zzd      (58004) root         (0)     4619 2024-04-10 14:12:43.000000 hepai-1.1.3/README.md
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.280802 hepai-1.1.3/hai/
--rw-r--r--   0 zzd      (58004) root         (0)     1541 2024-04-12 16:18:32.000000 hepai-1.1.3/hai/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.280802 hepai-1.1.3/hai/apis/
--rw-r--r--   0 zzd      (58004) root         (0)     2201 2023-10-24 10:39:47.000000 hepai-1.1.3/hai/apis/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.282802 hepai-1.1.3/hai/apis/basic/
--rw-r--r--   0 zzd      (58004) root         (0)       83 2023-10-24 10:39:47.000000 hepai-1.1.3/hai/apis/basic/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)       55 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/basic/argparse.py
--rw-r--r--   0 zzd      (58004) root         (0)      458 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/basic/base.py
--rw-r--r--   0 zzd      (58004) root         (0)       54 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/basic/grpc.py
--rw-r--r--   0 zzd      (58004) root         (0)      122 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/basic/registry.py
--rw-r--r--   0 zzd      (58004) root         (0)      141 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/basic/utils.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.283802 hepai-1.1.3/hai/apis/hub/
--rw-r--r--   0 zzd      (58004) root         (0)       98 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/hub/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      803 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/hub/hubs.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.283802 hepai-1.1.3/hai/apis/modules/
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.284802 hepai-1.1.3/hai/apis/modules/ResNet/
--rw-r--r--   0 zzd      (58004) root         (0)     1057 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/ResNet/ResNet.py
--rw-r--r--   0 zzd      (58004) root         (0)      415 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/ResNet/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.285802 hepai-1.1.3/hai/apis/modules/UNet/
--rw-r--r--   0 zzd      (58004) root         (0)      637 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/UNet/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     2478 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/UNet/argparse_config.py
--rw-r--r--   0 zzd      (58004) root         (0)     1619 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/UNet/evaluate_api.py
--rw-r--r--   0 zzd      (58004) root         (0)     4730 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/UNet/predict_api.py
--rw-r--r--   0 zzd      (58004) root         (0)     9139 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/UNet/train_api.py
--rw-r--r--   0 zzd      (58004) root         (0)     3099 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/UNet/unet_api.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.285802 hepai-1.1.3/hai/apis/modules/YOLOv5/
--rw-r--r--   0 zzd      (58004) root         (0)      434 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/YOLOv5/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/modules/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      103 2024-04-10 14:12:43.000000 hepai-1.1.3/hai/apis/openai_api.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.286802 hepai-1.1.3/hai/apis/workers_api/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 09:11:02.000000 hepai-1.1.3/hai/apis/workers_api/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.287802 hepai-1.1.3/hai/apis/workers_api/llm/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/workers_api/llm/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     2953 2023-10-12 05:19:35.000000 hepai-1.1.3/hai/apis/workers_api/llm/llm.py
--rw-r--r--   0 zzd      (58004) root         (0)        3 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/apis/workers_api/llm/tokenizer.py
--rw-r--r--   0 zzd      (58004) root         (0)     8679 2024-04-12 10:35:23.000000 hepai-1.1.3/hai/apis/workers_api/model.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.287802 hepai-1.1.3/hai/apis/workers_api/nougat/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2024-04-10 14:12:43.000000 hepai-1.1.3/hai/apis/workers_api/nougat/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      470 2024-04-10 14:12:43.000000 hepai-1.1.3/hai/apis/workers_api/nougat/pdf_process.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.288802 hepai-1.1.3/hai/apis/workers_api/sam/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-08-11 08:12:07.000000 hepai-1.1.3/hai/apis/workers_api/sam/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     2164 2023-10-12 05:19:35.000000 hepai-1.1.3/hai/apis/workers_api/sam/pre_process.py
--rw-r--r--   0 zzd      (58004) root         (0)     5139 2023-08-11 08:12:07.000000 hepai-1.1.3/hai/apis/workers_api/sam/seg_via_sam.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.289802 hepai-1.1.3/hai/configs/
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.290802 hepai-1.1.3/hai/configs/Base/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/configs/Base/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      407 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/configs/Base/hai_config.py
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/configs/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      285 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/configs/uaii_deepsort_config.py
--rw-r--r--   0 zzd      (58004) root         (0)     2706 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/configs/uaii_seyolov5_config.py
--rw-r--r--   0 zzd      (58004) root         (0)     1476 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/configs/uaii_stream_config.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.290802 hepai-1.1.3/hai/configs/urls/
--rw-r--r--   0 zzd      (58004) root         (0)     1752 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/configs/urls/datasets.json
--rw-r--r--   0 zzd      (58004) root         (0)      960 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/configs/urls/hub_models.json
--rw-r--r--   0 zzd      (58004) root         (0)      534 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/configs/visible_loader_config.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.290802 hepai-1.1.3/hai/modules/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.291802 hepai-1.1.3/hai/modules/detection/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/detection/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.291802 hepai-1.1.3/hai/modules/exporter/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/exporter/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.291802 hepai-1.1.3/hai/modules/exporter/images_exporter/
--rw-r--r--   0 zzd      (58004) root         (0)     5282 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/exporter/images_exporter/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.291802 hepai-1.1.3/hai/modules/loader/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/loader/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.292802 hepai-1.1.3/hai/modules/loader/images_loader/
--rw-r--r--   0 zzd      (58004) root         (0)     1618 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/loader/images_loader/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     3346 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/loader/images_loader/dataloader.py
--rw-r--r--   0 zzd      (58004) root         (0)    14091 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/loader/images_loader/dataset_torch.py
--rw-r--r--   0 zzd      (58004) root         (0)    26952 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/loader/images_loader/datasets.py
--rw-r--r--   0 zzd      (58004) root         (0)     1446 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/model_hub.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.292802 hepai-1.1.3/hai/modules/segmentation/
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.293802 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     1573 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/evaluate.py
--rw-r--r--   0 zzd      (58004) root         (0)      842 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/hubconf.py
--rwxr-xr-x   0 zzd      (58004) root         (0)     3997 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/predict.py
--rw-r--r--   0 zzd      (58004) root         (0)     8621 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/train.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.294802 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/unet/
--rw-r--r--   0 zzd      (58004) root         (0)       29 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     1130 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
--rw-r--r--   0 zzd      (58004) root         (0)     2602 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.295802 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/utils/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     2991 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
--rw-r--r--   0 zzd      (58004) root         (0)     1619 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
--rw-r--r--   0 zzd      (58004) root         (0)      533 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/modules/segmentation/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.296802 hepai-1.1.3/hai/testor/
--rw-r--r--   0 zzd      (58004) root         (0)      166 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/testor/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      189 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/testor/test.py
--rw-r--r--   0 zzd      (58004) root         (0)      495 2023-10-24 10:39:47.000000 hepai-1.1.3/hai/testor/test_ip_connectable.py
--rw-r--r--   0 zzd      (58004) root         (0)      281 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/testor/test_module.py
--rw-r--r--   0 zzd      (58004) root         (0)      965 2023-10-24 10:39:47.000000 hepai-1.1.3/hai/testor/test_request_model.py
--rw-r--r--   0 zzd      (58004) root         (0)      406 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/testor/testor.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.296802 hepai-1.1.3/hai/uaii/
--rw-r--r--   0 zzd      (58004) root         (0)       46 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.297802 hepai-1.1.3/hai/uaii/actuator/
--rw-r--r--   0 zzd      (58004) root         (0)       71 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/actuator/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      430 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/actuator/trainer.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.297802 hepai-1.1.3/hai/uaii/cli/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/cli/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     4118 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/cli/cli_functions.py
--rw-r--r--   0 zzd      (58004) root         (0)     9276 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/cli/cli_main.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.298802 hepai-1.1.3/hai/uaii/datasets/
--rw-r--r--   0 zzd      (58004) root         (0)       28 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/datasets/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     3240 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/datasets/dataloader.py
--rw-r--r--   0 zzd      (58004) root         (0)     8478 2024-04-10 14:12:43.000000 hepai-1.1.3/hai/uaii/datasets/dataset_utils.py
--rw-r--r--   0 zzd      (58004) root         (0)    40434 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/datasets/datasets.py
--rw-r--r--   0 zzd      (58004) root         (0)     4673 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/datasets/datasets_hub.py
--rw-r--r--   0 zzd      (58004) root         (0)     4046 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/datasets/uaii_loaders.py
--rw-r--r--   0 zzd      (58004) root         (0)     9457 2024-04-12 16:44:49.000000 hepai-1.1.3/hai/uaii/hepai_object.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.298802 hepai-1.1.3/hai/uaii/registry/
--rw-r--r--   0 zzd      (58004) root         (0)      374 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/registry/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     5669 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/registry/init_register.py
--rw-r--r--   0 zzd      (58004) root         (0)    11103 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/registry/registy.py
--rw-r--r--   0 zzd      (58004) root         (0)       81 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/registry/testor.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.299802 hepai-1.1.3/hai/uaii/registry/utils/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/registry/utils/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     1619 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/registry/utils/general.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.299802 hepai-1.1.3/hai/uaii/server/
--rw-r--r--   0 zzd      (58004) root         (0)     1893 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.300802 hepai-1.1.3/hai/uaii/server/grpc/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.301802 hepai-1.1.3/hai/uaii/server/grpc/example/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/example/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      517 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/example/grpc-client.py
--rw-r--r--   0 zzd      (58004) root         (0)     1353 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/example/grpc-test.py
--rw-r--r--   0 zzd      (58004) root         (0)     3163 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/example/hello_pb2.py
--rw-r--r--   0 zzd      (58004) root         (0)     2242 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/example/hello_pb2_grpc.py
--rw-r--r--   0 zzd      (58004) root         (0)     6022 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/grpc_pb2.py
--rw-r--r--   0 zzd      (58004) root         (0)     3707 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/grpc_pb2_grpc.py
--rw-r--r--   0 zzd      (58004) root         (0)     5517 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/grpc_secure_client.py
--rw-r--r--   0 zzd      (58004) root         (0)    10437 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/grpc_secure_server.py
--rw-r--r--   0 zzd      (58004) root         (0)     6172 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/grpc_xai_client.py
--rw-r--r--   0 zzd      (58004) root         (0)     5648 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/grpc/grpc_xai_server.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.301802 hepai-1.1.3/hai/uaii/server/nacos/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.302802 hepai-1.1.3/hai/uaii/server/nacos/nacos/
--rw-r--r--   0 zzd      (58004) root         (0)      184 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/nacos/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)    47889 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/nacos/client.py
--rw-r--r--   0 zzd      (58004) root         (0)      752 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/nacos/commons.py
--rw-r--r--   0 zzd      (58004) root         (0)       98 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/nacos/exception.py
--rw-r--r--   0 zzd      (58004) root         (0)     1645 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/nacos/files.py
--rw-r--r--   0 zzd      (58004) root         (0)     2403 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/nacos/listener.py
--rw-r--r--   0 zzd      (58004) root         (0)      624 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/nacos/params.py
--rw-r--r--   0 zzd      (58004) root         (0)     4363 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/nacos/timer.py
--rw-r--r--   0 zzd      (58004) root         (0)     1555 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/nacos-test.py
--rw-r--r--   0 zzd      (58004) root         (0)     2388 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/nacos/request_test.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.302802 hepai-1.1.3/hai/uaii/server/socket/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/socket/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.302802 hepai-1.1.3/hai/uaii/server/socket/example/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/socket/example/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      730 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/socket/example/client.py
--rw-r--r--   0 zzd      (58004) root         (0)      674 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/socket/example/server.py
--rw-r--r--   0 zzd      (58004) root         (0)     2131 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/server/socket/server.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.303802 hepai-1.1.3/hai/uaii/socket/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/socket/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.303802 hepai-1.1.3/hai/uaii/socket/example/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/socket/example/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      730 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/socket/example/client.py
--rw-r--r--   0 zzd      (58004) root         (0)      672 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/socket/example/server.py
--rw-r--r--   0 zzd      (58004) root         (0)     2153 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/socket/server.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.304802 hepai-1.1.3/hai/uaii/stream/
--rw-r--r--   0 zzd      (58004) root         (0)        1 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/stream/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     1411 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/stream/base_input.py
--rw-r--r--   0 zzd      (58004) root         (0)     7745 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/stream/base_module.py
--rw-r--r--   0 zzd      (58004) root         (0)     2575 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/stream/base_output.py
--rw-r--r--   0 zzd      (58004) root         (0)      354 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/stream/base_queue.py
--rw-r--r--   0 zzd      (58004) root         (0)        4 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/stream/rabbit_qm.py
--rw-r--r--   0 zzd      (58004) root         (0)    15802 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/stream/stream.py
--rw-r--r--   0 zzd      (58004) root         (0)     4094 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/stream/streams.py
--rw-r--r--   0 zzd      (58004) root         (0)    12294 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/uaii_main.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.306802 hepai-1.1.3/hai/uaii/utils/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/utils/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)      921 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/utils/arbitrary_import.py
--rw-r--r--   0 zzd      (58004) root         (0)    17055 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/utils/base_uaii.py
--rw-r--r--   0 zzd      (58004) root         (0)    15290 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/utils/config_loader.py
--rw-r--r--   0 zzd      (58004) root         (0)     4472 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/utils/fake_argparse.py
--rw-r--r--   0 zzd      (58004) root         (0)     3729 2023-05-18 07:14:07.000000 hepai-1.1.3/hai/uaii/utils/general.py
--rw-r--r--   0 zzd      (58004) root         (0)     5268 2023-10-24 10:39:47.000000 hepai-1.1.3/hai/uaii/utils/hai_hf_parser.py
--rw-r--r--   0 zzd      (58004) root         (0)    18952 2024-04-12 10:36:14.000000 hepai-1.1.3/hai/uaii/utils/hf_argparser.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.307802 hepai-1.1.3/hai/uaii/worker/
--rw-r--r--   0 zzd      (58004) root         (0)        0 2023-05-18 07:32:31.000000 hepai-1.1.3/hai/uaii/worker/__init__.py
--rw-r--r--   0 zzd      (58004) root         (0)     2516 2024-04-10 19:18:34.000000 hepai-1.1.3/hai/uaii/worker/base_worker_model.py
--rw-r--r--   0 zzd      (58004) root         (0)     3070 2024-04-10 14:12:43.000000 hepai-1.1.3/hai/uaii/worker/run_worker.py
--rw-r--r--   0 zzd      (58004) root         (0)       65 2023-05-18 09:08:02.000000 hepai-1.1.3/hai/uaii/worker/usage.py
--rw-r--r--   0 zzd      (58004) root         (0)     1561 2023-07-11 02:02:20.000000 hepai-1.1.3/hai/uaii/worker/utils.py
--rw-r--r--   0 zzd      (58004) root         (0)    17690 2024-04-13 15:05:37.000000 hepai-1.1.3/hai/uaii/worker/worker.py
--rw-r--r--   0 zzd      (58004) root         (0)      339 2024-04-13 15:06:47.000000 hepai-1.1.3/hai/version.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.307802 hepai-1.1.3/hepai/
--rw-r--r--   0 zzd      (58004) root         (0)      147 2024-04-12 16:18:30.000000 hepai-1.1.3/hepai/__init__.py
-drwxr-xr-x   0 zzd      (58004) root         (0)        0 2024-04-13 15:08:51.307802 hepai-1.1.3/hepai.egg-info/
--rw-r--r--   0 zzd      (58004) root         (0)     5402 2024-04-13 15:08:51.000000 hepai-1.1.3/hepai.egg-info/PKG-INFO
--rw-r--r--   0 zzd      (58004) root         (0)     5252 2024-04-13 15:08:51.000000 hepai-1.1.3/hepai.egg-info/SOURCES.txt
--rw-r--r--   0 zzd      (58004) root         (0)        1 2024-04-13 15:08:51.000000 hepai-1.1.3/hepai.egg-info/dependency_links.txt
--rw-r--r--   0 zzd      (58004) root         (0)       50 2024-04-13 15:08:51.000000 hepai-1.1.3/hepai.egg-info/entry_points.txt
--rw-r--r--   0 zzd      (58004) root         (0)       89 2024-04-13 15:08:51.000000 hepai-1.1.3/hepai.egg-info/requires.txt
--rw-r--r--   0 zzd      (58004) root         (0)       10 2024-04-13 15:08:51.000000 hepai-1.1.3/hepai.egg-info/top_level.txt
--rw-r--r--   0 zzd      (58004) root         (0)       38 2024-04-13 15:08:51.308802 hepai-1.1.3/setup.cfg
--rw-r--r--   0 zzd      (58004) root         (0)     4828 2023-07-03 01:27:44.000000 hepai-1.1.3/setup.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      118 2022-10-28 08:51:38.000000 hepai-1.1.4/MANIFEST.in
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5406 2024-04-17 17:36:59.866130 hepai-1.1.4/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4619 2024-03-26 09:59:20.000000 hepai-1.1.4/README.md
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1613 2024-04-17 15:09:40.000000 hepai-1.1.4/hai/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2201 2024-03-25 11:14:31.000000 hepai-1.1.4/hai/apis/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/basic/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       83 2023-10-24 09:29:42.000000 hepai-1.1.4/hai/apis/basic/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       55 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/basic/argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      458 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/basic/base.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       54 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/basic/grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      122 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/basic/registry.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      141 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/basic/utils.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/hub/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-04 00:48:55.000000 hepai-1.1.4/hai/apis/hub/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      803 2022-10-08 09:52:47.000000 hepai-1.1.4/hai/apis/hub/hubs.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/modules/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/modules/ResNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1057 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/modules/ResNet/ResNet.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      415 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/modules/ResNet/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/modules/UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      637 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/modules/UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2478 2022-09-22 09:20:00.000000 hepai-1.1.4/hai/apis/modules/UNet/argparse_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-09-02 00:21:08.000000 hepai-1.1.4/hai/apis/modules/UNet/evaluate_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4730 2022-09-03 22:56:22.000000 hepai-1.1.4/hai/apis/modules/UNet/predict_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9139 2022-09-22 08:22:39.000000 hepai-1.1.4/hai/apis/modules/UNet/train_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3099 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/modules/UNet/unet_api.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/modules/YOLOv5/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      434 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/apis/modules/YOLOv5/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:54:43.000000 hepai-1.1.4/hai/apis/modules/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      103 2024-03-25 11:33:22.000000 hepai-1.1.4/hai/apis/openai_api.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/workers_api/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:36:18.000000 hepai-1.1.4/hai/apis/workers_api/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/workers_api/llm/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:22:46.000000 hepai-1.1.4/hai/apis/workers_api/llm/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2953 2023-11-09 05:34:58.000000 hepai-1.1.4/hai/apis/workers_api/llm/llm.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        3 2023-04-21 09:02:06.000000 hepai-1.1.4/hai/apis/workers_api/llm/tokenizer.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8679 2024-04-10 14:20:32.000000 hepai-1.1.4/hai/apis/workers_api/model.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/workers_api/nougat/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2024-03-08 06:44:02.000000 hepai-1.1.4/hai/apis/workers_api/nougat/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      470 2024-03-08 06:44:02.000000 hepai-1.1.4/hai/apis/workers_api/nougat/pdf_process.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/apis/workers_api/sam/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-08-07 05:23:27.000000 hepai-1.1.4/hai/apis/workers_api/sam/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2164 2023-10-12 04:36:05.000000 hepai-1.1.4/hai/apis/workers_api/sam/pre_process.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5139 2023-08-04 16:18:52.000000 hepai-1.1.4/hai/apis/workers_api/sam/seg_via_sam.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/configs/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/configs/Base/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:19:48.000000 hepai-1.1.4/hai/configs/Base/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      407 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/configs/Base/hai_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      112 2024-04-17 12:28:00.000000 hepai-1.1.4/hai/configs/CONST.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/configs/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      285 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/configs/uaii_deepsort_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2706 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/configs/uaii_seyolov5_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1476 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/configs/uaii_stream_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/configs/urls/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1752 2022-10-19 18:44:14.000000 hepai-1.1.4/hai/configs/urls/datasets.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      960 2022-10-19 20:40:27.000000 hepai-1.1.4/hai/configs/urls/hub_models.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      534 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/configs/visible_loader_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/modules/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:42:32.000000 hepai-1.1.4/hai/modules/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/modules/detection/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:41:52.000000 hepai-1.1.4/hai/modules/detection/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/modules/exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:29.000000 hepai-1.1.4/hai/modules/exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/modules/exporter/images_exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5282 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/modules/exporter/images_exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/modules/loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:28.000000 hepai-1.1.4/hai/modules/loader/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/modules/loader/images_loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1618 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/modules/loader/images_loader/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3346 2023-04-21 12:08:18.000000 hepai-1.1.4/hai/modules/loader/images_loader/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    14091 2022-10-18 10:33:57.000000 hepai-1.1.4/hai/modules/loader/images_loader/dataset_torch.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    26952 2022-10-18 11:10:17.000000 hepai-1.1.4/hai/modules/loader/images_loader/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1446 2022-10-18 17:35:03.000000 hepai-1.1.4/hai/modules/model_hub.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/modules/segmentation/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:56:25.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1573 2022-08-31 21:12:48.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/evaluate.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      842 2022-08-30 18:18:45.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/hubconf.py
+-rwxrwxr-x   0 zzd       (1000) zzd       (1000)     3997 2022-08-30 18:18:45.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/predict.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8621 2022-08-31 21:12:32.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/train.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.862130 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/unet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       29 2022-08-30 18:18:45.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1130 2022-08-30 18:18:45.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2602 2022-08-30 18:18:45.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-30 18:18:45.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2991 2022-10-08 08:56:24.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-30 18:18:45.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      533 2022-09-30 09:30:48.000000 hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:55:50.000000 hepai-1.1.4/hai/modules/segmentation/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/testor/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      166 2023-04-21 07:26:13.000000 hepai-1.1.4/hai/testor/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      189 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/testor/test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      495 2023-10-23 01:04:23.000000 hepai-1.1.4/hai/testor/test_ip_connectable.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      281 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/testor/test_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      965 2023-10-23 01:10:57.000000 hepai-1.1.4/hai/testor/test_request_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      406 2023-04-21 07:26:41.000000 hepai-1.1.4/hai/testor/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       46 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/actuator/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2022-12-07 09:16:51.000000 hepai-1.1.4/hai/uaii/actuator/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      430 2022-12-07 09:20:22.000000 hepai-1.1.4/hai/uaii/actuator/trainer.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/cli/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:00:08.000000 hepai-1.1.4/hai/uaii/cli/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4118 2023-05-11 12:36:29.000000 hepai-1.1.4/hai/uaii/cli/cli_functions.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9276 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/uaii/cli/cli_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/datasets/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       28 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/datasets/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3240 2023-04-21 12:05:26.000000 hepai-1.1.4/hai/uaii/datasets/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8478 2024-03-08 06:41:21.000000 hepai-1.1.4/hai/uaii/datasets/dataset_utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    40434 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/datasets/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4673 2022-10-19 18:52:31.000000 hepai-1.1.4/hai/uaii/datasets/datasets_hub.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 12:05:05.000000 hepai-1.1.4/hai/uaii/datasets/uaii_loaders.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    13127 2024-04-17 15:45:51.000000 hepai-1.1.4/hai/uaii/hepai_object.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/registry/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      374 2022-09-22 05:57:37.000000 hepai-1.1.4/hai/uaii/registry/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5669 2023-04-04 04:04:35.000000 hepai-1.1.4/hai/uaii/registry/init_register.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    11103 2022-09-22 03:26:47.000000 hepai-1.1.4/hai/uaii/registry/registy.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       81 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/registry/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/registry/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/registry/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/registry/utils/general.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/server/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1893 2022-12-02 17:03:40.000000 hepai-1.1.4/hai/uaii/server/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/server/grpc/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/grpc/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/server/grpc/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/grpc/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      517 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/grpc/example/grpc-client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1353 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/grpc/example/grpc-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3163 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/grpc/example/hello_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2242 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/grpc/example/hello_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6022 2022-09-02 03:06:02.000000 hepai-1.1.4/hai/uaii/server/grpc/grpc_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3707 2022-10-18 10:41:24.000000 hepai-1.1.4/hai/uaii/server/grpc/grpc_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5517 2022-09-02 04:56:59.000000 hepai-1.1.4/hai/uaii/server/grpc/grpc_secure_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    10437 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/uaii/server/grpc/grpc_secure_server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6172 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/grpc/grpc_xai_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5648 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/grpc/grpc_xai_server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/server/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/server/nacos/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      184 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/nacos/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    47889 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/nacos/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      752 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/nacos/commons.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/nacos/exception.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1645 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/nacos/files.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2403 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/nacos/listener.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      624 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/nacos/params.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4363 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/nacos/timer.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1555 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/nacos-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2388 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/nacos/request_test.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/server/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/server/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      674 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2131 2022-09-02 03:01:13.000000 hepai-1.1.4/hai/uaii/server/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      672 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2153 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/stream/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/stream/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1411 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/stream/base_input.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     7745 2023-04-21 07:34:39.000000 hepai-1.1.4/hai/uaii/stream/base_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2575 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/stream/base_output.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      354 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/stream/base_queue.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/stream/rabbit_qm.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15802 2022-09-27 10:17:02.000000 hepai-1.1.4/hai/uaii/stream/stream.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4094 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/stream/streams.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    12294 2022-08-24 17:25:48.000000 hepai-1.1.4/hai/uaii/uaii_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.4/hai/uaii/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      921 2022-09-22 07:46:07.000000 hepai-1.1.4/hai/uaii/utils/arbitrary_import.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    17055 2023-04-21 12:06:51.000000 hepai-1.1.4/hai/uaii/utils/base_uaii.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15290 2023-05-10 16:19:50.000000 hepai-1.1.4/hai/uaii/utils/config_loader.py
+-rw-r--r--   0 zzd       (1000) zzd       (1000)     4472 2022-09-30 05:15:38.000000 hepai-1.1.4/hai/uaii/utils/fake_argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1339 2024-04-17 17:05:41.000000 hepai-1.1.4/hai/uaii/utils/file_object.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4033 2024-04-17 14:56:21.000000 hepai-1.1.4/hai/uaii/utils/general.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5268 2023-10-24 09:29:02.000000 hepai-1.1.4/hai/uaii/utils/hai_hf_parser.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    18952 2023-06-29 12:25:38.000000 hepai-1.1.4/hai/uaii/utils/hf_argparser.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hai/uaii/worker/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-05-18 13:37:30.000000 hepai-1.1.4/hai/uaii/worker/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3414 2024-04-17 17:18:08.000000 hepai-1.1.4/hai/uaii/worker/base_worker_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3070 2024-03-27 12:20:34.000000 hepai-1.1.4/hai/uaii/worker/run_worker.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       65 2023-05-18 13:37:30.000000 hepai-1.1.4/hai/uaii/worker/usage.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1561 2023-07-03 15:23:11.000000 hepai-1.1.4/hai/uaii/worker/utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    18371 2024-04-17 16:16:40.000000 hepai-1.1.4/hai/uaii/worker/worker.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      339 2024-04-17 16:18:10.000000 hepai-1.1.4/hai/version.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hepai/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      174 2024-04-17 15:09:16.000000 hepai-1.1.4/hepai/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-17 17:36:59.866130 hepai-1.1.4/hepai.egg-info/
+-rw-r--r--   0 zzd       (1000) zzd       (1000)     5406 2024-04-17 17:36:59.000000 hepai-1.1.4/hepai.egg-info/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5303 2024-04-17 17:36:59.000000 hepai-1.1.4/hepai.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2024-04-17 17:36:59.000000 hepai-1.1.4/hepai.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       50 2024-04-17 17:36:59.000000 hepai-1.1.4/hepai.egg-info/entry_points.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       89 2024-04-17 17:36:59.000000 hepai-1.1.4/hepai.egg-info/requires.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       10 2024-04-17 17:36:59.000000 hepai-1.1.4/hepai.egg-info/top_level.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       38 2024-04-17 17:36:59.866130 hepai-1.1.4/setup.cfg
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4832 2024-04-17 12:22:34.000000 hepai-1.1.4/setup.py
```

### Comparing `hepai-1.1.3/PKG-INFO` & `hepai-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: hepai
-Version: 1.1.3
+Version: 1.1.4
 Summary: High energy phscis Artificial Intelligence plateform, HAI.
 Home-page: https://github.com/zhangzhengde0225/hai
 Author: Zhengde Zhang
-Author-email: zdzhang@163.com
+Author-email: zdzhang@ihep.ac.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 
 
 [![Stars](https://img.shields.io/github/stars/zhangzhengde0225/CDNet)](
 https://github.com/zhangzhengde0225/hai)
 [![Open issue](https://img.shields.io/github/issues/zhangzhengde0225/CDNet)](
 https://github.com/zhangzhengde0225/hai/issues)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: hepai Version: 1.1.3 Summary: High energy phscis
+Metadata-Version: 2.1 Name: hepai Version: 1.1.4 Summary: High energy phscis
 Artificial Intelligence plateform, HAI. Home-page: https://github.com/
-zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@163.com
+zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@ihep.ac.cn
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Requires-Python: >=3.6.0
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown [![Stars](https://img.shields.io/
 github/stars/zhangzhengde0225/CDNet)]( https://github.com/zhangzhengde0225/hai)
 [![Open issue](https://img.shields.io/github/issues/zhangzhengde0225/CDNet)]
 ( https://github.com/zhangzhengde0225/hai/issues) #### English | [ç®ä½ä¸­æ]
 (https://github.com/zhangzhengde0225/hai/blob/main/docs/readme_zh_cn.md) #
 HepAI Library This is [HepAI](https://ai.ihep.ac.cn) python library, the AI
 platform can accelerate scientific research in multidisciplinary scenarios,
```

### Comparing `hepai-1.1.3/README.md` & `hepai-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/__init__.py` & `hepai-1.1.4/hai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+from .configs import CONST
 from .apis import __version__, __author__, __appname__, __email__, __affiliation__, __version_suffix__
 from .version import __url__
 from .apis import AbstractInput, AbstractModule, AbstractOutput, AbstractQue
 from .apis import MODULES, SCRIPTS, IOS, init_register
 from .apis import Config
 from .apis import UAII, uaii, cli
 from .apis import hub
@@ -16,14 +17,16 @@
 
 # LLM
 from .apis import LLM, Model, Models, api_key
 # from .apis import HepAI
 from .uaii.hepai_object import (
     HepAI, HaiCompletions, ChatCompletion, ChatCompletionChunk, Stream
     )
+from .uaii.utils.file_object import HaiFile
+
 
 # from xsensing_ai.modules import *  # 加载项目的模块
 # from xsensing_ai.uaii.server.grpc.grpc_xai_client import XAIGrpcClient
 
 # from . import nn
 
 # """
```

### Comparing `hepai-1.1.3/hai/apis/__init__.py` & `hepai-1.1.4/hai/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/hub/hubs.py` & `hepai-1.1.4/hai/apis/hub/hubs.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/modules/ResNet/ResNet.py` & `hepai-1.1.4/hai/apis/modules/ResNet/ResNet.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/modules/UNet/__init__.py` & `hepai-1.1.4/hai/apis/modules/UNet/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/modules/UNet/argparse_config.py` & `hepai-1.1.4/hai/apis/modules/UNet/argparse_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/modules/UNet/evaluate_api.py` & `hepai-1.1.4/hai/apis/modules/UNet/evaluate_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/modules/UNet/predict_api.py` & `hepai-1.1.4/hai/apis/modules/UNet/predict_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/modules/UNet/train_api.py` & `hepai-1.1.4/hai/apis/modules/UNet/train_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/modules/UNet/unet_api.py` & `hepai-1.1.4/hai/apis/modules/UNet/unet_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/workers_api/llm/llm.py` & `hepai-1.1.4/hai/apis/workers_api/llm/llm.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/workers_api/model.py` & `hepai-1.1.4/hai/apis/workers_api/model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/workers_api/sam/pre_process.py` & `hepai-1.1.4/hai/apis/workers_api/sam/pre_process.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/apis/workers_api/sam/seg_via_sam.py` & `hepai-1.1.4/hai/apis/workers_api/sam/seg_via_sam.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/configs/uaii_seyolov5_config.py` & `hepai-1.1.4/hai/configs/uaii_seyolov5_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/configs/uaii_stream_config.py` & `hepai-1.1.4/hai/configs/uaii_stream_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/configs/urls/datasets.json` & `hepai-1.1.4/hai/configs/urls/datasets.json`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/configs/urls/hub_models.json` & `hepai-1.1.4/hai/configs/urls/hub_models.json`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/configs/visible_loader_config.py` & `hepai-1.1.4/hai/configs/visible_loader_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/exporter/images_exporter/__init__.py` & `hepai-1.1.4/hai/modules/exporter/images_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/loader/images_loader/__init__.py` & `hepai-1.1.4/hai/modules/loader/images_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/loader/images_loader/dataloader.py` & `hepai-1.1.4/hai/modules/loader/images_loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/loader/images_loader/dataset_torch.py` & `hepai-1.1.4/hai/modules/loader/images_loader/dataset_torch.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/loader/images_loader/datasets.py` & `hepai-1.1.4/hai/modules/loader/images_loader/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/model_hub.py` & `hepai-1.1.4/hai/modules/model_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/evaluate.py` & `hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/evaluate.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/hubconf.py` & `hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/hubconf.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/predict.py` & `hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/predict.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/train.py` & `hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/train.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py` & `hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py` & `hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py` & `hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py` & `hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/modules/segmentation/Pytorch_UNet/utils/utils.py` & `hepai-1.1.4/hai/modules/segmentation/Pytorch_UNet/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/testor/test_request_model.py` & `hepai-1.1.4/hai/testor/test_request_model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/cli/cli_functions.py` & `hepai-1.1.4/hai/uaii/cli/cli_functions.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/cli/cli_main.py` & `hepai-1.1.4/hai/uaii/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/datasets/dataloader.py` & `hepai-1.1.4/hai/uaii/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/datasets/dataset_utils.py` & `hepai-1.1.4/hai/uaii/datasets/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/datasets/datasets.py` & `hepai-1.1.4/hai/uaii/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/datasets/datasets_hub.py` & `hepai-1.1.4/hai/uaii/datasets/datasets_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/datasets/uaii_loaders.py` & `hepai-1.1.4/hai/uaii/datasets/uaii_loaders.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/hepai_object.py` & `hepai-1.1.4/hai/uaii/hepai_object.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,86 @@
 
-from typing import Mapping, Union, Literal, Iterable, Optional, Dict, List, cast
-
+from typing import (
+    Mapping, Union, Literal, Iterable, Optional, Dict, List, cast, Type,
+    Any,
+)
 import httpx
 import os, sys
 from pathlib import Path
 here = Path(__file__).parent
 
-try:
-    from openai import OpenAI, resources
-    from openai import NOT_GIVEN, Timeout, NotGiven
-    from openai._types import Headers, Query, Body
-    from openai.types import Completion
-    from openai.resources import Completions, Chat
-    from openai.resources.chat.completions import (
-        ChatCompletionMessageParam,
-        completion_create_params,
-        ChatCompletionToolChoiceOptionParam,
-        ChatCompletionToolParam,
-        ChatCompletion,
-        ChatCompletionChunk,
-        Stream,
-    )
-    from openai._utils import (
-        required_args, maybe_transform
-    )
-    from openai._base_client import make_request_options
-except:
-    try:
-        sys.path.append(str(here.parent.parent))
-        from repos.openai_python.src.openai import OpenAI
-        from repos.openai_python.src.openai import ( NOT_GIVEN, Timeout, NotGiven)
-        from repos.openai_python.src.openai._types import Headers, Query, Body
-        from repos.openai_python.src.openai.types import Completion
-        from repos.openai_python.src.openai import resources
-        from repos.openai_python.src.openai.resources import Completions, Chat
-        from repos.openai_python.src.openai.resources.chat.completions import (
-            ChatCompletionMessageParam,
-            completion_create_params,
-            ChatCompletionToolChoiceOptionParam,
-            ChatCompletionToolParam,
-            ChatCompletion,
-            ChatCompletionChunk,
-            Stream,
-        )
-        from repos.openai_python.src.openai._utils import (
-            required_args, maybe_transform
-        )
-        from repos.openai_python.src.openai._base_client import make_request_options
-    except:
-        raise ImportError("Can't find openai module, please install it first by `pip install openai --upgrade`.")
+import inspect
+
+## opneai
+from openai import OpenAI, resources
+from openai import NOT_GIVEN, Timeout, NotGiven
+from openai._types import Headers, Query, Body
+from openai.types import Completion
+from openai.resources import Completions, Chat
+from openai.resources.chat.completions import (
+    ChatCompletionMessageParam,
+    completion_create_params,
+    ChatCompletionToolChoiceOptionParam,
+    ChatCompletionToolParam,
+    ChatCompletion,
+    ChatCompletionChunk,
+    Stream,
+)
+from openai._utils import required_args, maybe_transform
+from openai._base_client import (
+    ResponseT, APIResponse, FinalRequestOptions, RAW_RESPONSE_HEADER, _T,
+    Stream, SSEDecoder, AsyncStream, SSEBytesDecoder,
+    make_request_options, LegacyAPIResponse, BaseAPIResponse,
+    get_origin, extract_response_type
+)
 
 from hai.apis.workers_api.model import HaiModel
+from .utils.general import load_image_from_bytes
+from .utils.file_object import HaiFile
 
 DEFAULT_MAX_RETRIES = 2
 DEFAULT_TIMEOUT = httpx.Timeout(timeout=600.0, connect=5.0)
 DEFAULT_LIMITS = httpx.Limits(max_connections=100, max_keepalive_connections=20)
 
+class HaiPostParser:
+    def __call__(self, parsed, **kwargs):
+        if isinstance(parsed, ChatCompletion):
+            """服务端仅仅返回字典时"""
+            if parsed.id is None and parsed.choices is None:
+                if parsed.model_extra:
+                    return parsed.model_extra
+
+        return parsed
+
+class HAPIResponse(APIResponse):
+
+    def get_filename(self, response: httpx.Response) -> str:
+        content_disposition = response.headers.get("content-disposition", "")
+        filename = content_disposition.split("filename=")[-1]
+        return filename.strip('"')
+     
+    def _parse(self, *, to: type[_T] | None = None) -> Any | _T:
+        response = self.http_response
+        content_type, *_ = response.headers.get("content-type", "*").split(";")
+        if "image/" in content_type:
+            filename = self.get_filename(response)
+            return HaiFile(type_="image", data=response.content, filename=filename)
+        elif "application/pdf" in content_type:
+            filename = self.get_filename(response)
+            return HaiFile(type_="pdf", data=response.content, filename=filename)
+        elif "text/" in content_type:
+            filename = self.get_filename(response)
+            return HaiFile(type_="txt", data=response.content, filename=filename)
+        # application/json时
+        return super()._parse(to=to)
+
+
+class HaiCompletion(ChatCompletion):
+    pass
+
 class HaiCompletions(Completions):
 
     @required_args(["messages", "model"], ["messages", "model", "stream"])
     def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
@@ -142,14 +163,46 @@
             cast_to=ChatCompletion,
             stream=stream or False,
             stream_cls=Stream[ChatCompletionChunk],
         )
 
         return res
 
+
+    def request_worker(
+            self,
+            *,
+            model: str,
+            function: str,
+            stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
+            extra_headers: Headers | None = None,
+            extra_query: Query | None = None,
+            extra_body: Body | None = None,
+            timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+            **kwargs,
+        ):
+        tmp = dict()
+        tmp["model"] = model
+        tmp["function"] = function
+        tmp.update(kwargs)
+        body=maybe_transform(tmp, completion_create_params.CompletionCreateParams)
+        options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            )
+        options["post_parser"] = HaiPostParser()
+        res = self._post(
+            "/worker/unified_gate", 
+            body=body, 
+            options=options,
+            cast_to=HaiCompletion,
+            stream=stream or False,
+            stream_cls=Stream[ChatCompletionChunk],
+        )
+        return res
+
 class HaiChat(Chat):
     @property
     def completions(self) -> HaiCompletions:
         return HaiCompletions(client=self._client)
 
 class HepAI(OpenAI):
     completions: HaiCompletions
@@ -227,9 +280,67 @@
         port = kwargs.pop("port", self.base_url.port)
         return HaiModel.list(
             api_key=api_key,
             host=host,
             port=port,
             **kwargs,
         )
+    
+    def request_worker(self, **kwargs):
+        return self.completions.request_worker(**kwargs)
+
+    def _process_response(
+        self,
+        *,
+        cast_to: Type[ResponseT],
+        options: FinalRequestOptions,
+        response: httpx.Response,
+        stream: bool,
+        stream_cls: type[Stream[Any]] | type[AsyncStream[Any]] | None,
+    ) -> ResponseT:
+        if response.request.headers.get(RAW_RESPONSE_HEADER) == "true":
+            return cast(
+                ResponseT,
+                LegacyAPIResponse(
+                    raw=response,
+                    client=self,
+                    cast_to=cast_to,
+                    stream=stream,
+                    stream_cls=stream_cls,
+                    options=options,
+                ),
+            )
+
+        origin = get_origin(cast_to) or cast_to
+
+        if inspect.isclass(origin) and issubclass(origin, BaseAPIResponse):
+            if not issubclass(origin, APIResponse):
+                raise TypeError(f"API Response types must subclass {APIResponse}; Received {origin}")
+
+            response_cls = cast("type[BaseAPIResponse[Any]]", cast_to)
+            return cast(
+                ResponseT,
+                response_cls(
+                    raw=response,
+                    client=self,
+                    cast_to=extract_response_type(response_cls),
+                    stream=stream,
+                    stream_cls=stream_cls,
+                    options=options,
+                ),
+            )
+
+        if cast_to == httpx.Response:
+            return cast(ResponseT, response)
+
+        api_response = HAPIResponse(
+            raw=response,
+            client=self,
+            cast_to=cast("type[ResponseT]", cast_to),  # pyright: ignore[reportUnnecessaryCast]
+            stream=stream,
+            stream_cls=stream_cls,
+            options=options,
+        )
+        if bool(response.request.headers.get(RAW_RESPONSE_HEADER)):
+            return cast(ResponseT, api_response)
 
-    
+        return api_response.parse()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hepai-1.1.3/hai/uaii/registry/init_register.py` & `hepai-1.1.4/hai/uaii/registry/init_register.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/registry/registy.py` & `hepai-1.1.4/hai/uaii/registry/registy.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/registry/utils/general.py` & `hepai-1.1.4/hai/uaii/registry/utils/general.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/__init__.py` & `hepai-1.1.4/hai/uaii/server/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/example/grpc-client.py` & `hepai-1.1.4/hai/uaii/server/grpc/example/grpc-client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/example/grpc-test.py` & `hepai-1.1.4/hai/uaii/server/grpc/example/grpc-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/example/hello_pb2.py` & `hepai-1.1.4/hai/uaii/server/grpc/example/hello_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/example/hello_pb2_grpc.py` & `hepai-1.1.4/hai/uaii/server/grpc/example/hello_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/grpc_pb2.py` & `hepai-1.1.4/hai/uaii/server/grpc/grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/grpc_pb2_grpc.py` & `hepai-1.1.4/hai/uaii/server/grpc/grpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/grpc_secure_client.py` & `hepai-1.1.4/hai/uaii/server/grpc/grpc_secure_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/grpc_secure_server.py` & `hepai-1.1.4/hai/uaii/server/grpc/grpc_secure_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/grpc_xai_client.py` & `hepai-1.1.4/hai/uaii/server/grpc/grpc_xai_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/grpc/grpc_xai_server.py` & `hepai-1.1.4/hai/uaii/server/grpc/grpc_xai_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/nacos/nacos/client.py` & `hepai-1.1.4/hai/uaii/server/nacos/nacos/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/nacos/nacos/commons.py` & `hepai-1.1.4/hai/uaii/server/nacos/nacos/commons.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/nacos/nacos/files.py` & `hepai-1.1.4/hai/uaii/server/nacos/nacos/files.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/nacos/nacos/listener.py` & `hepai-1.1.4/hai/uaii/server/nacos/nacos/listener.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/nacos/nacos/params.py` & `hepai-1.1.4/hai/uaii/server/nacos/nacos/params.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/nacos/nacos/timer.py` & `hepai-1.1.4/hai/uaii/server/nacos/nacos/timer.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/nacos/nacos-test.py` & `hepai-1.1.4/hai/uaii/server/nacos/nacos-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/nacos/request_test.py` & `hepai-1.1.4/hai/uaii/server/nacos/request_test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/socket/example/client.py` & `hepai-1.1.4/hai/uaii/server/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/socket/example/server.py` & `hepai-1.1.4/hai/uaii/server/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/server/socket/server.py` & `hepai-1.1.4/hai/uaii/server/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/socket/example/client.py` & `hepai-1.1.4/hai/uaii/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/socket/example/server.py` & `hepai-1.1.4/hai/uaii/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/socket/server.py` & `hepai-1.1.4/hai/uaii/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/stream/base_input.py` & `hepai-1.1.4/hai/uaii/stream/base_input.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/stream/base_module.py` & `hepai-1.1.4/hai/uaii/stream/base_module.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/stream/base_output.py` & `hepai-1.1.4/hai/uaii/stream/base_output.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/stream/stream.py` & `hepai-1.1.4/hai/uaii/stream/stream.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/stream/streams.py` & `hepai-1.1.4/hai/uaii/stream/streams.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/uaii_main.py` & `hepai-1.1.4/hai/uaii/uaii_main.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/utils/arbitrary_import.py` & `hepai-1.1.4/hai/uaii/utils/arbitrary_import.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/utils/base_uaii.py` & `hepai-1.1.4/hai/uaii/utils/base_uaii.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/utils/config_loader.py` & `hepai-1.1.4/hai/uaii/utils/config_loader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/utils/fake_argparse.py` & `hepai-1.1.4/hai/uaii/utils/fake_argparse.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/utils/general.py` & `hepai-1.1.4/hai/uaii/utils/general.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 uaii general
 """
 import damei as dm
 import numpy as np
+from PIL import Image
+from io import BytesIO
 
 from ..datasets.dataset_utils import get_file, extract_archive
 
 
 def single_plot(result, orig_img, target_names):
     """
     把检测结果绘制到原始图像上。
@@ -111,9 +113,18 @@
     if len(macthed) == 0:
         return None
     else:
         versions = [all_dict[x]['version'] for x in macthed]
         version = sorted(versions)[-1]
         return version
 
-
-
+def load_image_from_bytes(image_bytes):
+    """
+    从字节流中加载图像
+    :param image_bytes:
+    :return:
+    """
+    image_bytes = BytesIO(image_bytes)
+    img = Image.open(image_bytes)
+    # img.load()
+    # img_array = np.array(img)
+    return img
```

### Comparing `hepai-1.1.3/hai/uaii/utils/hai_hf_parser.py` & `hepai-1.1.4/hai/uaii/utils/hai_hf_parser.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/utils/hf_argparser.py` & `hepai-1.1.4/hai/uaii/utils/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/worker/base_worker_model.py` & `hepai-1.1.4/hai/uaii/worker/base_worker_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 
+from typing import List, Dict, Any
+from pathlib import Path
+here = Path(__file__).parent
 
 
 class BaseWorkerModel:
     """
     用于被控制工人模型的基类，提供了面向切片的自动流式输出等功能
     Usage:
         class MyWorker(WorkerBaseModel):
@@ -56,17 +59,49 @@
         """需要重写函数"""
         raise NotImplementedError(f"The `train` method of `{self.name}` is not implemented.")
     
     def evaluate(self, **kwargs):
         """需要重写函数"""
         raise NotImplementedError(f"The `evaluate` method of `{self.name}` is not implemented.")
     
-
     def get_misc(self, **kwargs):
         """需要重写函数"""
         misc = dict()
         misc['trainable'] = self.trainable
         misc['inferable'] = self.inferable
         return misc
     
     def chat_completions(self, **kwargs):
-        raise NotImplementedError(f'The `chat_completions` method of `{self.name}` is not implemented.')
+        raise NotImplementedError(f'The `chat_completions` method of `{self.name}` is not implemented.')
+    
+    def get_int(self, **kwargs):
+        return 1
+    
+    def get_float(self, **kwargs):
+        return 1.0
+    
+    def get_bool(self, **kwargs):
+        return True
+    
+    def get_str(self, **kwargs):
+        return "string"
+    
+    def get_list(self, **kwargs):
+        return [1, 2, 3]
+    
+    def get_dict(self, **kwargs):
+        return {"key": "value"}
+    
+    def get_image(self, **kwargs):
+        return Path(f"{here}/assets/demo.png")
+    
+    def get_pdf(self, **kwargs):
+        return Path(f"{here}/assets/demo.pdf")
+
+    def get_txt(self, **kwargs):
+        return Path(f"{here}/assets/demo.txt")
+
+    def get_stream(self, **kwargs):
+        range_num = kwargs.get('range_num', 10)
+        out = [i for i in range(range_num)]
+        for i in out:
+            yield f'data: {i}\n\n'
```

### Comparing `hepai-1.1.3/hai/uaii/worker/run_worker.py` & `hepai-1.1.4/hai/uaii/worker/run_worker.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/worker/utils.py` & `hepai-1.1.4/hai/uaii/worker/utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.3/hai/uaii/worker/worker.py` & `hepai-1.1.4/hai/uaii/worker/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Worker类别，具备基本和示例功能
 """
 
 import time
 import json
 import time
-from typing import List, Union
+from typing import List, Union, Generator
 import threading
 import uuid
 import traceback
 import argparse
 # import dataclasses
 from dataclasses import dataclass, field
 import os, sys
 from pathlib import Path
 
 from fastapi import FastAPI, Request, BackgroundTasks, HTTPException
-from fastapi.responses import StreamingResponse, JSONResponse, Response
+from fastapi.responses import StreamingResponse, JSONResponse, Response, FileResponse
 import requests
 import uvicorn
 
 import damei as dm 
 import atexit
 here = Path(__file__).parent
 
@@ -346,35 +346,50 @@
         
 app = WorkerAPP()  # It's a FastAPI instance
 
 
 def release_model_semaphore():
     model_semaphore.release()
 
+    
+@app.post("/v1/worker/unified_gate")
+async def v1_unified_gate(request: Request):
+    return await app_unified_gate(request)
+
 @app.post("/worker_unified_gate")
 async def app_unified_gate(request: Request):
     global model_semaphore, global_counter
     global_counter += 1
     params = await request.json()
     if model_semaphore is None:
         model_semaphore = asyncio.Semaphore(
             app.worker.limit_model_concurrency)
     await model_semaphore.acquire()
     stream = params.get("stream", False)
     ok, data = app.worker.unified_gate(**params)
-    background_tasks = BackgroundTasks()  # 背景任务
-    background_tasks.add_task(release_model_semaphore)  # 释放锁
     if not ok:
         data = data if isinstance(data, str) else json.dumps(data)
-        print(model_semaphore)
+        # print(model_semaphore)
+        release_model_semaphore()
         raise HTTPException(status_code=404, detail=data, background=background_tasks)
+    background_tasks = BackgroundTasks()  # 背景任务
+    background_tasks.add_task(release_model_semaphore)  # 释放锁
+    if isinstance(data, Generator) and (stream is None or stream is False):
+        logger.info(f"Get a generator from function: {params.get('function')}, auto set stream=True")
+        stream = True
     if not stream:
+        # 判断是不是文件路径
+        if isinstance(data, Path):
+            if not os.path.exists(data):
+                raise HTTPException(status_code=404, detail=f"File not found: {data}")
+            return FileResponse(data, filename=data.name, background=background_tasks)
         return JSONResponse(content=data, background=background_tasks)
     return StreamingResponse(data, background=background_tasks)
 
+
 @app.post("/worker_generate_stream")
 async def generate_stream(request: Request):
     global model_semaphore, global_counter
     global_counter += 1
     params = await request.json()
 
     if model_semaphore is None:
```

### Comparing `hepai-1.1.3/hepai.egg-info/PKG-INFO` & `hepai-1.1.4/hepai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: hepai
-Version: 1.1.3
+Version: 1.1.4
 Summary: High energy phscis Artificial Intelligence plateform, HAI.
 Home-page: https://github.com/zhangzhengde0225/hai
 Author: Zhengde Zhang
-Author-email: zdzhang@163.com
+Author-email: zdzhang@ihep.ac.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 
 
 [![Stars](https://img.shields.io/github/stars/zhangzhengde0225/CDNet)](
 https://github.com/zhangzhengde0225/hai)
 [![Open issue](https://img.shields.io/github/issues/zhangzhengde0225/CDNet)](
 https://github.com/zhangzhengde0225/hai/issues)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: hepai Version: 1.1.3 Summary: High energy phscis
+Metadata-Version: 2.1 Name: hepai Version: 1.1.4 Summary: High energy phscis
 Artificial Intelligence plateform, HAI. Home-page: https://github.com/
-zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@163.com
+zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@ihep.ac.cn
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Requires-Python: >=3.6.0
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown [![Stars](https://img.shields.io/
 github/stars/zhangzhengde0225/CDNet)]( https://github.com/zhangzhengde0225/hai)
 [![Open issue](https://img.shields.io/github/issues/zhangzhengde0225/CDNet)]
 ( https://github.com/zhangzhengde0225/hai/issues) #### English | [ç®ä½ä¸­æ]
 (https://github.com/zhangzhengde0225/hai/blob/main/docs/readme_zh_cn.md) #
 HepAI Library This is [HepAI](https://ai.ihep.ac.cn) python library, the AI
 platform can accelerate scientific research in multidisciplinary scenarios,
```

### Comparing `hepai-1.1.3/hepai.egg-info/SOURCES.txt` & `hepai-1.1.4/hepai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 hai/apis/workers_api/llm/llm.py
 hai/apis/workers_api/llm/tokenizer.py
 hai/apis/workers_api/nougat/__init__.py
 hai/apis/workers_api/nougat/pdf_process.py
 hai/apis/workers_api/sam/__init__.py
 hai/apis/workers_api/sam/pre_process.py
 hai/apis/workers_api/sam/seg_via_sam.py
+hai/configs/CONST.py
 hai/configs/__init__.py
 hai/configs/uaii_deepsort_config.py
 hai/configs/uaii_seyolov5_config.py
 hai/configs/uaii_stream_config.py
 hai/configs/visible_loader_config.py
 hai/configs/Base/__init__.py
 hai/configs/Base/hai_config.py
@@ -134,14 +135,15 @@
 hai/uaii/stream/stream.py
 hai/uaii/stream/streams.py
 hai/uaii/utils/__init__.py
 hai/uaii/utils/arbitrary_import.py
 hai/uaii/utils/base_uaii.py
 hai/uaii/utils/config_loader.py
 hai/uaii/utils/fake_argparse.py
+hai/uaii/utils/file_object.py
 hai/uaii/utils/general.py
 hai/uaii/utils/hai_hf_parser.py
 hai/uaii/utils/hf_argparser.py
 hai/uaii/worker/__init__.py
 hai/uaii/worker/base_worker_model.py
 hai/uaii/worker/run_worker.py
 hai/uaii/worker/usage.py
```

### Comparing `hepai-1.1.3/setup.py` & `hepai-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 from setuptools import find_packages, setup, Command
 
 
 NAME = 'hepai'
 DESCRIPTION = 'High energy phscis Artificial Intelligence plateform, HAI.'
 URL = 'https://github.com/zhangzhengde0225/hai'
-EMAIL = 'zdzhang@163.com'
+EMAIL = 'zdzhang@ihep.ac.cn'
 AUTHOR = 'Zhengde Zhang'
-REQUIRES_PYTHON = '>=3.6.0'
+REQUIRES_PYTHON = '>=3.10.0'
 
 with open(f'hai/version.py') as f:
     data = f.readlines()
     for line in data:
         if '__version__' in line:
             VERSION = line.split('=')[-1].strip().replace("'", '')
             break
```

