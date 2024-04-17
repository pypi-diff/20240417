# Comparing `tmp/acetone_nnet-0.1.dev2.tar.gz` & `tmp/acetone_nnet-0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.1.dev2.tar", last modified: Mon Apr 15 11:39:11 2024, max compression
+gzip compressed data, was "acetone_nnet-0.1.dev3.tar", last modified: Wed Apr 17 07:16:52 2024, max compression
```

## Comparing `acetone_nnet-0.1.dev2.tar` & `acetone_nnet-0.1.dev3.tar`

### file list

```diff
@@ -1,144 +1,145 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.201190 acetone_nnet-0.1.dev2/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev2/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev2/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev2/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7670 2024-04-15 11:39:11.200189 acetone_nnet-0.1.dev2/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6391 2024-04-15 08:20:07.000000 acetone_nnet-0.1.dev2/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1890 2024-04-15 11:38:49.000000 acetone_nnet-0.1.dev2/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-15 11:39:11.201190 acetone_nnet-0.1.dev2/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.175189 acetone_nnet-0.1.dev2/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.179189 acetone_nnet-0.1.dev2/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1770 2024-04-15 11:18:54.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2120 2024-04-15 08:00:26.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/__main__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-12 11:36:39.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.181189 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 07:57:10.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1852 2024-04-12 14:35:58.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4087 2024-04-12 11:42:37.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.183189 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/AddBias.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.184189 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1461 2024-04-12 11:51:36.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4324 2024-04-15 06:50:30.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1466 2024-04-12 11:51:50.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1477 2024-04-12 11:52:28.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-12 11:52:33.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.185189 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.186189 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.187189 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.188189 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-15 06:49:35.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 09:47:36.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2150 2024-04-15 09:56:16.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    23950 2024-04-15 11:32:04.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.188189 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.188189 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.188189 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17138 2024-04-15 07:13:20.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.188189 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.189189 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25232 2024-04-12 14:49:23.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4014 2024-04-12 09:54:11.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2453 2024-04-12 09:55:41.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.189189 acetone_nnet-0.1.dev2/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.191189 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.194189 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.196189 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.197189 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.198190 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.199190 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2122 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.199190 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.200189 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      689 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      741 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:39:11.200189 acetone_nnet-0.1.dev2/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7670 2024-04-15 11:39:11.000000 acetone_nnet-0.1.dev2/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6730 2024-04-15 11:39:11.000000 acetone_nnet-0.1.dev2/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-15 11:39:11.000000 acetone_nnet-0.1.dev2/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      120 2024-04-15 11:39:11.000000 acetone_nnet-0.1.dev2/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-15 11:39:11.000000 acetone_nnet-0.1.dev2/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-15 11:39:11.000000 acetone_nnet-0.1.dev2/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:52.030649 acetone_nnet-0.1.dev3/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.1.dev3/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev3/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev3/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7852 2024-04-17 07:16:52.029649 acetone_nnet-0.1.dev3/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6470 2024-04-16 12:29:53.000000 acetone_nnet-0.1.dev3/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2044 2024-04-16 12:07:57.000000 acetone_nnet-0.1.dev3/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-17 07:16:52.030649 acetone_nnet-0.1.dev3/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.724645 acetone_nnet-0.1.dev3/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.793646 acetone_nnet-0.1.dev3/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1790 2024-04-16 15:00:34.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-12 11:36:39.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.795647 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 07:57:10.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1872 2024-04-16 15:00:23.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4087 2024-04-12 11:42:37.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.797646 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3122 2024-04-16 14:50:44.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.798647 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1461 2024-04-12 11:51:36.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4324 2024-04-15 11:48:34.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1466 2024-04-12 11:51:50.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1477 2024-04-12 11:52:28.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-12 11:52:33.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.799646 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.800646 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.800646 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.801647 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-15 06:49:35.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 09:47:36.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    23950 2024-04-15 11:32:04.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.802646 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.802646 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7558 2024-04-17 07:04:46.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.802646 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17133 2024-04-17 07:14:08.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.803646 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.803646 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25232 2024-04-12 14:49:23.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4014 2024-04-12 09:54:11.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2453 2024-04-12 09:55:41.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.803646 acetone_nnet-0.1.dev3/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.875647 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.933648 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.976648 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.982648 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:51.985649 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:52.006649 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      535 2024-04-16 14:49:07.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2122 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:52.014649 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:52.024649 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      689 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      741 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 07:16:52.029649 acetone_nnet-0.1.dev3/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7852 2024-04-17 07:16:51.000000 acetone_nnet-0.1.dev3/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6830 2024-04-17 07:16:51.000000 acetone_nnet-0.1.dev3/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-17 07:16:51.000000 acetone_nnet-0.1.dev3/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      129 2024-04-17 07:16:51.000000 acetone_nnet-0.1.dev3/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-17 07:16:51.000000 acetone_nnet-0.1.dev3/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-17 07:16:51.000000 acetone_nnet-0.1.dev3/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.1.dev2/COPYING` & `acetone_nnet-0.1.dev3/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/LICENSE` & `acetone_nnet-0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/PKG-INFO` & `acetone_nnet-0.1.dev3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.1.dev2
+Version: 0.1.dev3
 Summary: Predictable programming framework for ML applications in safety-critical systems.
-Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
+Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -82,89 +82,95 @@
 * Run the *initial_setup.py* code
 ```
 python3 tests/models/lenet5/lenet5_example/initial_setup.py
 ```
 
 This script defines a neural network with a Lenet-5 architecture using the framework Keras. It then save the model in *.h5* and *.json* files. The later one is created using a specific function, developped by us, to write the keras model in ACETONE's format. The scripts also creates a random input to test the neural network. Finally, the scripts saves and prints, as a reference, the output of the inference done by the Keras framework.
 
-### Generating the C code with ACETONE
+### Generating the C code with ACETONE package
 
 Then, generate the C code with ACETONE.
 
 * Call ACETONE with the following arguments:
   * The file describing the model
   * The name of the function to generate (here 'lenet5')
   * The number of test to run (here 1)
   * The algorithm used for the convolution layer ('6loops','indirect_gemm_'+TYPE, 'std_gemm_'+TYPE, with TYPE being amongst 'nn','nt',    'tn','tt')
   * The directory in which the code will be generated
   * The input file with the test data
 
 ```
-python3 -m acetone_nnet tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
+cli-acetone tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
 ```
 
 * Compile the code
 ```
 make -C tests/models/lenet5/lenet5_example/lenet5_generated all
 ```
 
 * Execute the file with the path to the directory of the output file as argument
 ```
 ./tests/models/lenet5/lenet5_example/lenet5_generated/lenet5 ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt
 ```
 
 * Compare the output given by Keras and ACETONE
 ```
-python3 src/acetone_nnet/cli_compare.py ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
+cli_compare ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
 ```
 
 ## Tests
 
 Tests are implemented in the folder *tests*.
 
-To run all of them, use the following command:
+To run them, use the `run_tests.py` script from the `tests/` folder.
 ```
-python3 -m unittest discover tests/test_inference/test_layer tests/tests_network tests/tests_importer
+python3 run_tests.py all
 ```
 
-To only run a test, use the command
+You can replace the `all` argument by the name of a subfolder to only run the tests in it.
+```
+python3 run_tests.py FOLDER_NAME
+```
+where FOLDER_NAME is the name of your subfolder.
+
+You can run one test by using the command
 ```
 python3 -m unittest PATH_TO_TEST
 ```
-where PATH_TO_TEST is the path to your test.
+where PATH_TO_TEST is the path tot your test.
 
 ## Reproduce the paper's experiments
 
 To reproduce the result of semantic experiment with ACETONE as described in the paper, use the following commands:
 
 * For the acas_decr128 model
 ```
-pyhton3 src/cli_acteone.py tests/models/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas_decr128/output_acetone tests/models/acas_decr128/test_input_acas_decr128.txt
-make -C tests/models/acas_decr128/output_acetone all
-./tests/models/acas_decr128/output_acetone/acas_decr128 tests/models/acas_decr128/output_acetone/output_acetone.txt
-python3 src/cli_compare.py tests/models/acas_decr128/output_keras.txt tests/models/acas_decr128/output_acetone/output_acetone.txt
+cli-acetone tests/models/acas/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas/acas_decr128/output_acetone tests/models/acas/acas_decr128/test_input_acas_decr128.txt
+make -C tests/models/acas/acas_decr128/output_acetone all
+./tests/models/acas/acas_decr128/output_acetone/acas_decr128 tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
+cli_compare tests/models/acas/acas_decr128/output_keras.txt tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
 ```
 
 * For the lent5 model
 
 ```
-pyhton3 src/cli_acteone.py tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
+cli-acetone tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
 make -C tests/models/lenet5/lenet5_trained/output_acetone all
 ./tests/models/lenet5/lenet5_trained/output_acetone/lenet5_trained tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
-python3 src/cli_compare.py tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
+cli_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
 ```
 
 ## Capability
 
 As of the 26/03/2024, the framework can generate code for neural network meeting the following condition:
 
 * The neural network is Sequential and Feedforward
 
 * The neural-network is describeb in one of the following formats:
-  * JSON (specifique decription mad efor the framework. Confer to the file [JSON_from_keras_model.py](./src/format_importer/H5_importer/JSON_from_keras_model.py))
+  * JSON (specifique decription made for the framework. Confer to the file [JSON_from_keras_model.py](./src/format_importer/H5_importer/JSON_from_keras_model.py))
   * NNET 
   * ONNX
   * H5 (by transforming into a JSON file)
 
 * Its layers are amongst the following (both Keras and Onnx layers):
   * Dense
   * Convolutional (Conv2D) (3 option for the algorithm)
@@ -193,14 +199,13 @@
   * Linear
   * Tanh
   * ReLu
   * Sigmoid
   * Softmax
   * Exp
   * Log
-  
 
 ## License
 
 The project is under the GNU Lesser General Public License as published by the Free Software Foundation ; either version 3 of  the License or (at your option) any later version.
 
 See LICENSE for details.
```

### Comparing `acetone_nnet-0.1.dev2/README.md` & `acetone_nnet-0.1.dev3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,89 +55,95 @@
 * Run the *initial_setup.py* code
 ```
 python3 tests/models/lenet5/lenet5_example/initial_setup.py
 ```
 
 This script defines a neural network with a Lenet-5 architecture using the framework Keras. It then save the model in *.h5* and *.json* files. The later one is created using a specific function, developped by us, to write the keras model in ACETONE's format. The scripts also creates a random input to test the neural network. Finally, the scripts saves and prints, as a reference, the output of the inference done by the Keras framework.
 
-### Generating the C code with ACETONE
+### Generating the C code with ACETONE package
 
 Then, generate the C code with ACETONE.
 
 * Call ACETONE with the following arguments:
   * The file describing the model
   * The name of the function to generate (here 'lenet5')
   * The number of test to run (here 1)
   * The algorithm used for the convolution layer ('6loops','indirect_gemm_'+TYPE, 'std_gemm_'+TYPE, with TYPE being amongst 'nn','nt',    'tn','tt')
   * The directory in which the code will be generated
   * The input file with the test data
 
 ```
-python3 -m acetone_nnet tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
+cli-acetone tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
 ```
 
 * Compile the code
 ```
 make -C tests/models/lenet5/lenet5_example/lenet5_generated all
 ```
 
 * Execute the file with the path to the directory of the output file as argument
 ```
 ./tests/models/lenet5/lenet5_example/lenet5_generated/lenet5 ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt
 ```
 
 * Compare the output given by Keras and ACETONE
 ```
-python3 src/acetone_nnet/cli_compare.py ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
+cli_compare ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
 ```
 
 ## Tests
 
 Tests are implemented in the folder *tests*.
 
-To run all of them, use the following command:
+To run them, use the `run_tests.py` script from the `tests/` folder.
 ```
-python3 -m unittest discover tests/test_inference/test_layer tests/tests_network tests/tests_importer
+python3 run_tests.py all
 ```
 
-To only run a test, use the command
+You can replace the `all` argument by the name of a subfolder to only run the tests in it.
+```
+python3 run_tests.py FOLDER_NAME
+```
+where FOLDER_NAME is the name of your subfolder.
+
+You can run one test by using the command
 ```
 python3 -m unittest PATH_TO_TEST
 ```
-where PATH_TO_TEST is the path to your test.
+where PATH_TO_TEST is the path tot your test.
 
 ## Reproduce the paper's experiments
 
 To reproduce the result of semantic experiment with ACETONE as described in the paper, use the following commands:
 
 * For the acas_decr128 model
 ```
-pyhton3 src/cli_acteone.py tests/models/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas_decr128/output_acetone tests/models/acas_decr128/test_input_acas_decr128.txt
-make -C tests/models/acas_decr128/output_acetone all
-./tests/models/acas_decr128/output_acetone/acas_decr128 tests/models/acas_decr128/output_acetone/output_acetone.txt
-python3 src/cli_compare.py tests/models/acas_decr128/output_keras.txt tests/models/acas_decr128/output_acetone/output_acetone.txt
+cli-acetone tests/models/acas/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas/acas_decr128/output_acetone tests/models/acas/acas_decr128/test_input_acas_decr128.txt
+make -C tests/models/acas/acas_decr128/output_acetone all
+./tests/models/acas/acas_decr128/output_acetone/acas_decr128 tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
+cli_compare tests/models/acas/acas_decr128/output_keras.txt tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
 ```
 
 * For the lent5 model
 
 ```
-pyhton3 src/cli_acteone.py tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
+cli-acetone tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
 make -C tests/models/lenet5/lenet5_trained/output_acetone all
 ./tests/models/lenet5/lenet5_trained/output_acetone/lenet5_trained tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
-python3 src/cli_compare.py tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
+cli_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
 ```
 
 ## Capability
 
 As of the 26/03/2024, the framework can generate code for neural network meeting the following condition:
 
 * The neural network is Sequential and Feedforward
 
 * The neural-network is describeb in one of the following formats:
-  * JSON (specifique decription mad efor the framework. Confer to the file [JSON_from_keras_model.py](./src/format_importer/H5_importer/JSON_from_keras_model.py))
+  * JSON (specifique decription made for the framework. Confer to the file [JSON_from_keras_model.py](./src/format_importer/H5_importer/JSON_from_keras_model.py))
   * NNET 
   * ONNX
   * H5 (by transforming into a JSON file)
 
 * Its layers are amongst the following (both Keras and Onnx layers):
   * Dense
   * Convolutional (Conv2D) (3 option for the algorithm)
@@ -166,14 +172,13 @@
   * Linear
   * Tanh
   * ReLu
   * Sigmoid
   * Softmax
   * Exp
   * Log
-  
 
 ## License
 
 The project is under the GNU Lesser General Public License as published by the Free Software Foundation ; either version 3 of  the License or (at your option) any later version.
 
 See LICENSE for details.
```

### Comparing `acetone_nnet-0.1.dev2/pyproject.toml` & `acetone_nnet-0.1.dev3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.1.dev2"
+version = "0.1.dev3"
 requires-python = ">=3.10"
 
 authors = [
-    { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
+    { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
+    { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
+    { name="Benjamin LESAGE", email="benjamin.lesage@onera.fr"},
     { name="Claire PAGETTI", email="Claire.Pagetti@onera.fr" },
 ]
 
 description = "Predictable programming framework for ML applications in safety-critical systems."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 
@@ -51,13 +53,13 @@
     "templates/layers/*.tpl",
     "templates/layers/Resize/*.tpl",
     "templates/layers/Pad/*.tpl",
     "templates/layers/Gemm/*.tpl",
     "templates/layers/Conv/*.tpl"]
 
 [project.scripts]
-cli-acetone = "acetone_nnet.cli_acetone:cli_acetone"
-cli_compare = "acetone_nnet.cli_compare:cli_compare"
+acetone_generate = "acetone_nnet.cli_acetone:cli_acetone"
+acetone_compare = "acetone_nnet.cli_compare:cli_compare"
 
 [project.urls]
 Repository = "https://github.com/onera/acetone/"
 "Bug Tracker" = "https://github.com/onera/acetone/issues"
```

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/__init__.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from . import code_generator
 from .code_generator import (
     CodeGenerator, Layer,
-    Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax,
+    Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax, BatchNormalization,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest,
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip
 )
```

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from .neural_network import CodeGenerator
 
 from .Layer import Layer
 
 from . import layers
 from .layers import (
-    Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax,
+    Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax, BatchNormalization,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest
 )
```

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .Dot import Dot
 from .Flatten import Flatten
 from .Gather import Gather
 from .Gemm import Gemm
 from .Input import InputLayer
 from .MatMul import MatMul
 from .Softmax import Softmax
+from .BatchNormalization import BatchNormalization
 
 from . import Broadcast_layers
 from .Broadcast_layers import Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract 
 
 from . import Conv_layers
 from .Conv_layers import Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm
 
@@ -42,14 +43,14 @@
 from .Pooling_layers import Pooling2D, AveragePooling2D, MaxPooling2D
 
 from . import Resize_layers
 from .Resize_layers import Resize, ResizeCubic, ResizeLinear, ResizeNearest
 
 
 __all__ = (
-    "Add_Bias", "Concatenate", "Dense", "Dot", "Flatten", "Gather", "Gemm", "InputLayer", "MatMul", "Softmax",
+    "Add_Bias", "Concatenate", "Dense", "Dot", "Flatten", "Gather", "Gemm", "InputLayer", "MatMul", "Softmax", "BatchNormalization",
     Broadcast_layers.__all__,
     Conv_layers.__all__,
     Pad_layers.__all__,
     Pooling_layers.__all__,
     Resize_layers.__all__
 )
```

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/code_generator/neural_network.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     input_layer_size = 1
     for i in range(1, len(keras_model.input.shape)): #start in idx 1 cause idx 0 represents batch size, so it's None in inference phase
         input_layer_size = input_layer_size * keras_model.input.shape[i]
 
     model_dict['config']['data_format'] = 'channels_first'
     if ((hasattr(layer['config']['data_format']) ) 
         and (layer['config']['data_format'] == 'channels_last') for layer in model_dict['config']['layers']): 
+        print('--------------------------------------------------------------------')
         model_dict['config']['data_format'] = 'channels_last'
 
     if keras_model.layers[0].__class__.__name__ == 'InputLayer':
         start = 0
 
     else:
         start = 1
@@ -97,33 +98,53 @@
                         layer_json['config']['prev_layer_idx'].append(prev_layer_json['config']['idx']) 
         else:
             layer_json['config']['prev_layer_idx'] = [idx-1]
 
         if layer_json['class_name'] == 'Dense' or layer_json['class_name'] == 'Conv2D' :
             if layer_json['config']['dtype'] == 'float64':
                 weights = np.float64(layer_keras.get_weights()[0])
-
                 if(len(weights.shape) < 3):
                     for i in range(3-len(weights.shape)): 
                         weights = np.expand_dims(weights, axis=-1)
                 weights = np.moveaxis(weights, 2, 0)
                 if(len(weights.shape) < 4):
                     weights = np.expand_dims(weights, axis=0)
                     
                 layer_json['weights'] = weights
                 layer_json['biases'] = np.float64(layer_keras.get_weights()[1])
-            elif layer_json['config']['dtype'] == 'float32':
 
+            elif layer_json['config']['dtype'] == 'float32':
                 weights = np.float32(layer_keras.get_weights()[0])
+                if(len(weights.shape) < 3):
+                    for i in range(3-len(weights.shape)): 
+                        weights = np.expand_dims(weights, axis=-1)
+                weights = np.moveaxis(weights, 2, 0)
+                if(len(weights.shape) < 4):
+                    weights = np.expand_dims(weights, axis=0)
                 
                 layer_json['weights'] = weights
                 layer_json['biases'] = np.float32(layer_keras.get_weights()[1])
 
             i = i + 2
         
+        if(layer_json['class_name'] == 'BatchNormalization'):
+            if layer_json['config']['dtype'] == 'float64':
+                layer_json['beta'] = np.float64(layer_keras.get_weights()[0])
+                layer_json['gamma'] = np.float64(layer_keras.get_weights()[1])
+                layer_json['moving_mean'] = np.float64(layer_keras.get_weights()[2])
+                layer_json['moving_var'] = np.float64(layer_keras.get_weights()[3])
+
+            elif layer_json['config']['dtype'] == 'float32':
+                layer_json['beta'] = np.float32(layer_keras.get_weights()[0])
+                layer_json['gamma'] = np.float32(layer_keras.get_weights()[1])
+                layer_json['moving_mean'] = np.float32(layer_keras.get_weights()[2])
+                layer_json['moving_var'] = np.float32(layer_keras.get_weights()[3])
+
+            
+        
         idx += 1
 
     with open(output_dir_json, 'w', encoding='utf-8') as f:
         json.dump(model_dict, f, indent=4, cls = NumpyEncoder)
     f.close()
```

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 
 import json
 from itertools import islice
 import numpy as np
 
 from ...graph import graph_interpretor
 
-from ...code_generator.layers import AveragePooling2D, MaxPooling2D
-from ...code_generator.layers import Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm 
-from ...code_generator.layers import Constant_Pad
-from ...code_generator.layers import Add, Multiply, Subtract, Divide, Maximum, Minimum, Average
-from ...code_generator.layers import ResizeCubic, ResizeLinear, ResizeNearest
-from ...code_generator.layers import  Concatenate, InputLayer, Dense, Softmax,  Dot, Flatten
-from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH
+from ...code_generator import (
+    AveragePooling2D, MaxPooling2D,
+    Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
+    Constant_Pad,
+    Add, Multiply, Subtract, Maximum, Minimum, Average,
+    ResizeCubic, ResizeLinear, ResizeNearest,
+    Concatenate, InputLayer, Dense, Softmax,  Dot, Flatten, BatchNormalization,
+    Linear, ReLu, Sigmoid, TanH
+)
 
 def create_actv_function_obj(activation_str):
 
         if activation_str == 'sigmoid':
             return Sigmoid()
         elif activation_str == 'relu':
             return ReLu()
@@ -103,34 +105,22 @@
             if 'activation' in layer['config']:
                 if layer['config']['activation'] == 'softmax':
                     layer['config']['activation'] = 'linear'
                     add_softmax_layer = True
         
             if layer['class_name'] == 'Dense':
                 weights = np.array(data_type_py(layer['weights']))
-                if(len(weights.shape) < 3):
-                    for i in range(3-len(weights.shape)): 
-                        weights = np.expand_dims(weights, axis=-1)
-                weights = np.moveaxis(weights, 2, 0)
-                if(len(weights.shape) < 4):
-                    weights = np.expand_dims(weights, axis=0)
                 current_layer = Dense(idx=idx,
                                       size=layer['config']['units'],
                                       weights=np.array(data_type_py(layer['weights'])),
                                       biases=data_type_py(layer['biases']),
                                       activation_function=create_actv_function_obj(layer['config']['activation']))
             
             elif layer['class_name'] == 'Conv2D':
                 weights = np.array(data_type_py(layer['weights']))
-                if(len(weights.shape) < 3):
-                    for i in range(3-len(weights.shape)): 
-                        weights = np.expand_dims(weights, axis=-1)
-                weights = np.moveaxis(weights,2,0)
-                if(len(weights.shape) < 4):
-                    weights = np.expand_dims(weights, axis=0)
                 current_layer = create_conv2d_obj(algorithm = conv_algorithm,
                                                   conv_algorithm = conv_algorithm,
                                                   idx = idx,
                                                   size = layer['config']['size'],
                                                   padding = layer['config']['padding'],
                                                   strides = layer['config']['strides'][0],
                                                   kernel_h = layer['config']['kernel_size'][0],
@@ -286,14 +276,24 @@
                                              size = layer['config']['size'],
                                              pads = pads,
                                              constant_value = 0,
                                              axes = [],
                                              input_shape = layer['config']['input_shape'],
                                              activation_function = Linear())
             
+            elif layer['class_name'] == 'BatchNormalization':
+                current_layer = BatchNormalization(idx = layer['config']['idx'],
+                                                   input_shape = layer['config']['input_shape'],
+                                                   epsilon = layer['config']['epsilon'],
+                                                   scale = np.array(data_type_py(layer['gamma'])),
+                                                   biases = np.array(data_type_py(layer['beta'])),
+                                                   mean = np.array(data_type_py(layer['moving_mean'])),
+                                                   var = np.array(data_type_py(layer['moving_var'])),
+                                                   activation_function = Linear())
+            
             
             elif  'Normalization' in layer['class_name']:
                 continue
 
             elif  'Dropout' in layer['class_name']:
                 continue
 
@@ -320,10 +320,11 @@
                 l_temp.next_layer.append(current_layer)
                 current_layer.previous_layer.append(l_temp)
                 l_temp = current_layer
                 layers.append(current_layer)
 
         layers, listRoad, maxRoad, dict_cst = graph_interpretor.tri_topo(layers)
         layers = list(map(lambda x:x.find_output_str(dict_cst), layers))
-        print("Finished model initialization.")    
+        print("Finished model initialization.")
+        file.close()
         return layers, data_type, data_type_py, data_format, maxRoad, dict_cst
```

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.1.dev3/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.1.dev3/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.1.dev2
+Version: 0.1.dev3
 Summary: Predictable programming framework for ML applications in safety-critical systems.
-Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
+Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -82,89 +82,95 @@
 * Run the *initial_setup.py* code
 ```
 python3 tests/models/lenet5/lenet5_example/initial_setup.py
 ```
 
 This script defines a neural network with a Lenet-5 architecture using the framework Keras. It then save the model in *.h5* and *.json* files. The later one is created using a specific function, developped by us, to write the keras model in ACETONE's format. The scripts also creates a random input to test the neural network. Finally, the scripts saves and prints, as a reference, the output of the inference done by the Keras framework.
 
-### Generating the C code with ACETONE
+### Generating the C code with ACETONE package
 
 Then, generate the C code with ACETONE.
 
 * Call ACETONE with the following arguments:
   * The file describing the model
   * The name of the function to generate (here 'lenet5')
   * The number of test to run (here 1)
   * The algorithm used for the convolution layer ('6loops','indirect_gemm_'+TYPE, 'std_gemm_'+TYPE, with TYPE being amongst 'nn','nt',    'tn','tt')
   * The directory in which the code will be generated
   * The input file with the test data
 
 ```
-python3 -m acetone_nnet tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
+cli-acetone tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
 ```
 
 * Compile the code
 ```
 make -C tests/models/lenet5/lenet5_example/lenet5_generated all
 ```
 
 * Execute the file with the path to the directory of the output file as argument
 ```
 ./tests/models/lenet5/lenet5_example/lenet5_generated/lenet5 ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt
 ```
 
 * Compare the output given by Keras and ACETONE
 ```
-python3 src/acetone_nnet/cli_compare.py ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
+cli_compare ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
 ```
 
 ## Tests
 
 Tests are implemented in the folder *tests*.
 
-To run all of them, use the following command:
+To run them, use the `run_tests.py` script from the `tests/` folder.
 ```
-python3 -m unittest discover tests/test_inference/test_layer tests/tests_network tests/tests_importer
+python3 run_tests.py all
 ```
 
-To only run a test, use the command
+You can replace the `all` argument by the name of a subfolder to only run the tests in it.
+```
+python3 run_tests.py FOLDER_NAME
+```
+where FOLDER_NAME is the name of your subfolder.
+
+You can run one test by using the command
 ```
 python3 -m unittest PATH_TO_TEST
 ```
-where PATH_TO_TEST is the path to your test.
+where PATH_TO_TEST is the path tot your test.
 
 ## Reproduce the paper's experiments
 
 To reproduce the result of semantic experiment with ACETONE as described in the paper, use the following commands:
 
 * For the acas_decr128 model
 ```
-pyhton3 src/cli_acteone.py tests/models/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas_decr128/output_acetone tests/models/acas_decr128/test_input_acas_decr128.txt
-make -C tests/models/acas_decr128/output_acetone all
-./tests/models/acas_decr128/output_acetone/acas_decr128 tests/models/acas_decr128/output_acetone/output_acetone.txt
-python3 src/cli_compare.py tests/models/acas_decr128/output_keras.txt tests/models/acas_decr128/output_acetone/output_acetone.txt
+cli-acetone tests/models/acas/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas/acas_decr128/output_acetone tests/models/acas/acas_decr128/test_input_acas_decr128.txt
+make -C tests/models/acas/acas_decr128/output_acetone all
+./tests/models/acas/acas_decr128/output_acetone/acas_decr128 tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
+cli_compare tests/models/acas/acas_decr128/output_keras.txt tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
 ```
 
 * For the lent5 model
 
 ```
-pyhton3 src/cli_acteone.py tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
+cli-acetone tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
 make -C tests/models/lenet5/lenet5_trained/output_acetone all
 ./tests/models/lenet5/lenet5_trained/output_acetone/lenet5_trained tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
-python3 src/cli_compare.py tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
+cli_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
 ```
 
 ## Capability
 
 As of the 26/03/2024, the framework can generate code for neural network meeting the following condition:
 
 * The neural network is Sequential and Feedforward
 
 * The neural-network is describeb in one of the following formats:
-  * JSON (specifique decription mad efor the framework. Confer to the file [JSON_from_keras_model.py](./src/format_importer/H5_importer/JSON_from_keras_model.py))
+  * JSON (specifique decription made for the framework. Confer to the file [JSON_from_keras_model.py](./src/format_importer/H5_importer/JSON_from_keras_model.py))
   * NNET 
   * ONNX
   * H5 (by transforming into a JSON file)
 
 * Its layers are amongst the following (both Keras and Onnx layers):
   * Dense
   * Convolutional (Conv2D) (3 option for the algorithm)
@@ -193,14 +199,13 @@
   * Linear
   * Tanh
   * ReLu
   * Sigmoid
   * Softmax
   * Exp
   * Log
-  
 
 ## License
 
 The project is under the GNU Lesser General Public License as published by the Free Software Foundation ; either version 3 of  the License or (at your option) any later version.
 
 See LICENSE for details.
```

### Comparing `acetone_nnet-0.1.dev2/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.1.dev3/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 AUTHORS.md
 COPYING
 LICENSE
 README.md
 pyproject.toml
 src/acetone_nnet/__init__.py
-src/acetone_nnet/__main__.py
 src/acetone_nnet/cli_acetone.py
 src/acetone_nnet/cli_compare.py
 src/acetone_nnet.egg-info/PKG-INFO
 src/acetone_nnet.egg-info/SOURCES.txt
 src/acetone_nnet.egg-info/dependency_links.txt
 src/acetone_nnet.egg-info/entry_points.txt
 src/acetone_nnet.egg-info/requires.txt
 src/acetone_nnet.egg-info/top_level.txt
 src/acetone_nnet/code_generator/Layer.py
 src/acetone_nnet/code_generator/__init__.py
 src/acetone_nnet/code_generator/activation_functions.py
 src/acetone_nnet/code_generator/neural_network.py
 src/acetone_nnet/code_generator/layers/AddBias.py
+src/acetone_nnet/code_generator/layers/BatchNormalization.py
 src/acetone_nnet/code_generator/layers/Concatenate.py
 src/acetone_nnet/code_generator/layers/Dense.py
 src/acetone_nnet/code_generator/layers/Dot.py
 src/acetone_nnet/code_generator/layers/Flatten.py
 src/acetone_nnet/code_generator/layers/Gather.py
 src/acetone_nnet/code_generator/layers/Gemm.py
 src/acetone_nnet/code_generator/layers/Input.py
@@ -71,14 +71,15 @@
 src/acetone_nnet/templates/template_global_var_file.c.tpl
 src/acetone_nnet/templates/template_header_file.c.tpl
 src/acetone_nnet/templates/template_main_file.c.tpl
 src/acetone_nnet/templates/template_source_file.c.tpl
 src/acetone_nnet/templates/template_test_dataset_header.c.tpl
 src/acetone_nnet/templates/template_test_dataset_source.c.tpl
 src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
 src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
 src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
 src/acetone_nnet/templates/layers/template_Dense.c.tpl
 src/acetone_nnet/templates/layers/template_Dot.c.tpl
 src/acetone_nnet/templates/layers/template_Flatten.c.tpl
 src/acetone_nnet/templates/layers/template_Gather.c.tpl
 src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
```

