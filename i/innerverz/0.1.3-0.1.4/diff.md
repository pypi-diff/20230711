# Comparing `tmp/innerverz-0.1.3.tar.gz` & `tmp/innerverz-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.1.3.tar", last modified: Tue Jul 11 06:21:50 2023, max compression
+gzip compressed data, was "innerverz-0.1.4.tar", last modified: Tue Jul 11 11:55:10 2023, max compression
```

## Comparing `innerverz-0.1.3.tar` & `innerverz-0.1.4.tar`

### file list

```diff
@@ -1,169 +1,174 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.080297 innerverz-0.1.3/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.3/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 06:21:50.080399 innerverz-0.1.3/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.3/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.059457 innerverz-0.1.3/innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1733 2023-07-07 09:03:21.000000 innerverz-0.1.3/innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.060525 innerverz-0.1.3/innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-04 08:52:32.000000 innerverz-0.1.3/innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.061091 innerverz-0.1.3/innerverz/deblurrer/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deblurrer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2611 2023-07-11 05:59:21.000000 innerverz-0.1.3/innerverz/deblurrer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deblurrer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      843 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.061549 innerverz-0.1.3/innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    23911 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.062932 innerverz-0.1.3/innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1200 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.063942 innerverz-0.1.3/innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/cfg.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.064249 innerverz-0.1.3/innerverz/deca/utils/rasterizer/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/rasterizer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    11870 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deca/utils/tracker_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)    26664 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.064842 innerverz-0.1.3/innerverz/deep3dmm/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deep3dmm/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3582 2023-07-11 05:48:53.000000 innerverz-0.1.3/innerverz/deep3dmm/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      627 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.065714 innerverz-0.1.3/innerverz/face_alignment/
--rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/graphic_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/landmark.py
--rw-r--r--   0 jjy        (501) staff       (20)     8059 2023-07-11 06:18:23.000000 innerverz-0.1.3/innerverz/face_alignment/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      640 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.066475 innerverz-0.1.3/innerverz/face_alignment/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.067330 innerverz-0.1.3/innerverz/face_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5595 2023-07-11 06:04:34.000000 innerverz-0.1.3/innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.068044 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2015 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.068633 innerverz-0.1.3/innerverz/face_enhancer/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_enhancer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3881 2023-07-11 06:05:17.000000 innerverz-0.1.3/innerverz/face_enhancer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      768 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.069315 innerverz-0.1.3/innerverz/face_matting/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-04 12:12:59.000000 innerverz-0.1.3/innerverz/face_matting/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8110 2023-07-11 06:06:04.000000 innerverz-0.1.3/innerverz/face_matting/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.069917 innerverz-0.1.3/innerverz/face_matting/nets/
--rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.070209 innerverz-0.1.3/innerverz/face_matting/nets/decoders/
--rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/decoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-05 10:54:16.000000 innerverz-0.1.3/innerverz/face_matting/nets/decoders/resnet_decoder.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.070666 innerverz-0.1.3/innerverz/face_matting/nets/encoders/
--rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-05 10:54:29.000000 innerverz-0.1.3/innerverz/face_matting/nets/encoders/MatteFormer.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/encoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-05 11:01:53.000000 innerverz-0.1.3/innerverz/face_matting/nets/generators.py
--rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/ops.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.070934 innerverz-0.1.3/innerverz/face_matting/nets/raft/
--rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.071851 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 12:13:24.000000 innerverz-0.1.3/innerverz/face_matting/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.072543 innerverz-0.1.3/innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2894 2023-07-11 06:06:56.000000 innerverz-0.1.3/innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      689 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.073247 innerverz-0.1.3/innerverz/face_reshaping/
--rw-r--r--   0 jjy        (501) staff       (20)       32 2023-07-07 08:56:40.000000 innerverz-0.1.3/innerverz/face_reshaping/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3483 2023-07-11 06:09:10.000000 innerverz-0.1.3/innerverz/face_reshaping/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-05 11:02:06.000000 innerverz-0.1.3/innerverz/face_reshaping/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.073786 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-04 10:48:50.000000 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/LadderEncoder.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-05 10:42:47.000000 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-05 10:51:39.000000 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/dense_motion.py
--rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-04 10:48:50.000000 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4694 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_reshaping/test.py
--rw-r--r--   0 jjy        (501) staff       (20)     1750 2023-07-11 06:08:13.000000 innerverz-0.1.3/innerverz/face_reshaping/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.074527 innerverz-0.1.3/innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5773 2023-07-11 06:09:54.000000 innerverz-0.1.3/innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.075297 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1965 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.075885 innerverz-0.1.3/innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2443 2023-07-11 06:10:48.000000 innerverz-0.1.3/innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      693 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.076555 innerverz-0.1.3/innerverz/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.1.3/innerverz/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2618 2023-07-11 06:11:41.000000 innerverz-0.1.3/innerverz/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.1.3/innerverz/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/reage/net_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.1.3/innerverz/reage/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.077362 innerverz-0.1.3/innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3213 2023-07-11 06:12:48.000000 innerverz-0.1.3/innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3030 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.078081 innerverz-0.1.3/innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/upsampler/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2429 2023-07-11 06:14:26.000000 innerverz-0.1.3/innerverz/upsampler/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      830 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.078661 innerverz-0.1.3/innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.079247 innerverz-0.1.3/innerverz/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.079401 innerverz-0.1.3/innerverz/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-30 02:29:25.000000 innerverz-0.1.3/innerverz/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.080141 innerverz-0.1.3/innerverz/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.060235 innerverz-0.1.3/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 06:21:49.000000 innerverz-0.1.3/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-11 06:21:50.000000 innerverz-0.1.3/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-11 06:21:49.000000 innerverz-0.1.3/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-11 06:21:49.000000 innerverz-0.1.3/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-11 06:21:49.000000 innerverz-0.1.3/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.3/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-11 06:21:50.080723 innerverz-0.1.3/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-11 06:21:35.000000 innerverz-0.1.3/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.536442 innerverz-0.1.4/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.4/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 11:55:10.536564 innerverz-0.1.4/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.4/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.512292 innerverz-0.1.4/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1730 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.513320 innerverz-0.1.4/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.513859 innerverz-0.1.4/innerverz/deblurrer/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deblurrer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2611 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deblurrer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deblurrer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      843 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.514304 innerverz-0.1.4/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    24631 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.515504 innerverz-0.1.4/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12950 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1200 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.516688 innerverz-0.1.4/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/cfg.py
+-rw-r--r--   0 jjy        (501) staff       (20)    19673 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/lmks_756.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.516970 innerverz-0.1.4/innerverz/deca/utils/rasterizer/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/rasterizer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      706 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11870 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/tracker_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26664 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.517614 innerverz-0.1.4/innerverz/deep3dmm/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deep3dmm/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3582 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deep3dmm/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      627 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.518653 innerverz-0.1.4/innerverz/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8059 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      640 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.519159 innerverz-0.1.4/innerverz/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.519739 innerverz-0.1.4/innerverz/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5595 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.520462 innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2015 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.521062 innerverz-0.1.4/innerverz/face_enhancer/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3881 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_enhancer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      768 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.521551 innerverz-0.1.4/innerverz/face_matting/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8110 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.522541 innerverz-0.1.4/innerverz/face_matting/nets/
+-rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.523021 innerverz-0.1.4/innerverz/face_matting/nets/decoders/
+-rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/decoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/decoders/resnet_decoder.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.523406 innerverz-0.1.4/innerverz/face_matting/nets/encoders/
+-rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/encoders/MatteFormer.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/encoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/generators.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/ops.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.523718 innerverz-0.1.4/innerverz/face_matting/nets/raft/
+-rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/raft/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/raft/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.524536 innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/nets/utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_matting/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.525156 innerverz-0.1.4/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2894 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      689 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.527449 innerverz-0.1.4/innerverz/face_reshaper/
+-rw-r--r--   0 jjy        (501) staff       (20)       31 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3931 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.527995 innerverz-0.1.4/innerverz/face_reshaper/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/sub_nets/LadderEncoder.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/sub_nets/dense_motion.py
+-rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/sub_nets/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4694 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/test.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1750 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.528416 innerverz-0.1.4/innerverz/face_reshaper/vis_utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/vis_utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      885 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/vis_utils/vis_68.py
+-rw-r--r--   0 jjy        (501) staff       (20)    10261 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/face_reshaper/vis_utils/vis_756.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.529759 innerverz-0.1.4/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5773 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.530609 innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1965 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.531172 innerverz-0.1.4/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2443 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      693 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.531877 innerverz-0.1.4/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2618 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/reage/net_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)      763 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/reage/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.532411 innerverz-0.1.4/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3213 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3030 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.533070 innerverz-0.1.4/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/upsampler/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2429 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/upsampler/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      830 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.533643 innerverz-0.1.4/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.535456 innerverz-0.1.4/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.535611 innerverz-0.1.4/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.536295 innerverz-0.1.4/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-11 11:54:41.000000 innerverz-0.1.4/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 11:55:10.513043 innerverz-0.1.4/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 11:55:10.000000 innerverz-0.1.4/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     4955 2023-07-11 11:55:10.000000 innerverz-0.1.4/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-11 11:55:10.000000 innerverz-0.1.4/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-11 11:55:10.000000 innerverz-0.1.4/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-11 11:55:10.000000 innerverz-0.1.4/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.4/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-11 11:55:10.536910 innerverz-0.1.4/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-11 11:54:10.000000 innerverz-0.1.4/setup.py
```

### Comparing `innerverz-0.1.3/LICENSE.txt` & `innerverz-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/__init__.py` & `innerverz-0.1.4/innerverz/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,17 +96,17 @@
 from innerverz import Reage
 
 reage = Reage()
 
 # face_reshaping
 --------
 
-from innerverz import Face_Reshaping
+from innerverz import Face_Reshaper
 
-LW = Face_Reshaping()
+LW = Face_Reshaper()
 
 # face_matting
 --------
 
 from innerverz import Face_Matting
 
 FM = Face_Matting()
@@ -124,9 +124,9 @@
 from .utils import *
 from .face_color_transfer import *
 from .deca import *
 from .face_enhancer import *
 from .relighter import *
 from .video_faceparser import *
 from .reage import *
-from .face_reshaping import *
+from .face_reshaper import *
 from .face_matting import *
```

### Comparing `innerverz-0.1.3/innerverz/data_process/main.py` & `innerverz-0.1.4/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deblurrer/main.py` & `innerverz-0.1.4/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deblurrer/nets.py` & `innerverz-0.1.4/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deblurrer/test.py` & `innerverz-0.1.4/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/main.py` & `innerverz-0.1.4/innerverz/deca/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from .models.decoders import Generator
 
 from .utils.util import copy_state_dict, batch_orth_proj, tensor_vis_landmarks, vertex_normals
 from .utils.rotation_converter import batch_euler2axis
 from .utils.tensor_cropper import transform_points
 from .utils.renderer import SRenderY, set_rasterizer
 from .utils import tracker_utils
+from .utils.lmks_756 import indexes_756
 from ..utils import check_ckpt_exist, convert_image_type, get_url_id
 
 class DECA(nn.Module):
     def __init__(self, folder_name='deca', ckpt_name = 'ckpt.zip', force=False, device = 'cuda'):
         """
         Related Links
         --------
@@ -63,14 +64,16 @@
         self.image_size = 224
         self.uv_size = 256
         self.rasterizer_type = 'pytorch3d' # 'standard'
         
         self._create_model()
         self._setup_renderer()
         
+        self.indexes_756 = np.array(indexes_756, dtype=np.long)
+        
     def _setup_renderer(self,):
         set_rasterizer(self.rasterizer_type)
         self.render = SRenderY(self.image_size, obj_filename=os.path.join(self.dir_folder_path, 'head_template.obj'), uv_size=self.uv_size, rasterizer_type=self.rasterizer_type).to(self.device)
         # face mask for rendering details
         mask = imread(os.path.join(self.dir_folder_path, 'uv_face_eye_mask.png')).astype(np.float32)/255.; mask = torch.from_numpy(mask[:,:,0])[None,None,:,:].contiguous()
         self.uv_face_eye_mask = F.interpolate(mask, [self.uv_size, self.uv_size]).to(self.device)
         mask = imread(os.path.join(self.dir_folder_path, 'uv_face_mask.png')).astype(np.float32)/255.; mask = torch.from_numpy(mask[:,:,0])[None,None,:,:].contiguous()
@@ -348,15 +351,15 @@
             - shape_detail_images
                 - dtype : tensor
                 - shape : (b, 3, h, w)
                 - min max : (0, 1)
         """
         
         ## decode
-        verts, landmarks2d, landmarks3d, trans_verts, trans_landmarks2d, trans_landmarks3d = self.get_lmks_from_params(codedict, tform_invs=tform_invs)
+        verts, landmarks2d, landmarks3d, trans_verts, trans_landmarks2d, trans_landmarks3d, trans_landmarks_756_3d = self.get_lmks_from_params(codedict, tform_invs=tform_invs)
         
         # rendering
         albedo = self.flametex(codedict['tex']) if albedo else torch.zeros([codedict['images'].shape[0], 3, self.uv_size, self.uv_size], device=codedict['images'].device) 
         ops = self.render(verts, trans_verts, albedo, lights= codedict['light'],h=original_image.shape[-2], w=original_image.shape[-1], background=None)
         
         # detail
         uv_z = self.D_detail(torch.cat([codedict['pose'][:,3:], codedict['exp'], codedict['detail']], dim=1))
@@ -365,21 +368,24 @@
         # extract shape images
         shape_images, _, grid, alpha_images = self.render.render_shape(verts, trans_verts, lights= codedict['light'], h=original_image.shape[-2], w=original_image.shape[-1], images=None, return_grid=True)
         detail_normal_images = F.grid_sample(uv_detail_normals, grid, align_corners=False)*alpha_images
         shape_detail_images = self.render.render_shape(verts, trans_verts, lights= codedict['light'], detail_normal_images=detail_normal_images, h=original_image.shape[-2], w=original_image.shape[-1], images=None)
         
         vis_landmarks2d = tensor_vis_landmarks(original_image, landmarks2d)
         vis_landmarks3d = tensor_vis_landmarks(original_image, landmarks3d)
-        
+        vis_landmarks_756_3d = tensor_vis_landmarks(original_image, trans_landmarks_756_3d)
+
         visdict = {
             'inputs': original_image, 
             'landmarks2d': vis_landmarks2d,
             'landmarks3d': vis_landmarks3d,
+            'landmarks756_3d': vis_landmarks_756_3d,
             'landmarks2d_points': trans_landmarks2d,
             'landmarks3d_points': trans_landmarks3d,
+            'landmarks756_3d_points': trans_landmarks_756_3d,
             'shape_images': shape_images,
             'shape_detail_images': shape_detail_images,
         }
         return visdict
 
     def setup_tracker(self, deca_params, sparse_lmks, tform_invs, device='cuda'):
         self.device = device
@@ -510,26 +516,28 @@
         assert 'shape' in params_dict.keys()
         expression_params = params_dict['exp'] if 'exp' in params_dict.keys() else self.exp
         pose_params = params_dict['pose'] if 'pose' in params_dict.keys() else self.pose
         cam_params = params_dict['cam'] if 'cam' in params_dict.keys() else self.cam
         tform_invs = self.tform_invs if tform_invs is None else tform_invs
         
         # flame
-        verts, landmarks2d, landmarks3d = self.flame(
+        verts, landmarks2d, landmarks3d, landmarks_756_3d = self.flame(
             shape_params=params_dict['shape'], 
             expression_params=expression_params, 
             pose_params=pose_params,
             )
             
         # projection
         trans_verts = batch_orth_proj(verts, cam_params); trans_verts[:,:,1:] = -trans_verts[:,:,1:]
         trans_landmarks2d = batch_orth_proj(landmarks2d, cam_params)[:,:,:2]; trans_landmarks2d[:,:,1:] = -trans_landmarks2d[:,:,1:]; # trans_landmarks2d = trans_landmarks2d*256 + 256
         trans_landmarks3d = batch_orth_proj(landmarks3d, cam_params); trans_landmarks3d[:,:,1:] = -trans_landmarks3d[:,:,1:]; # trans_landmarks3d = trans_landmarks3d*256 + 256
+        trans_landmarks_756_3d = batch_orth_proj(landmarks_756_3d, cam_params); trans_landmarks_756_3d[:,:,1:] = -trans_landmarks_756_3d[:,:,1:]; # trans_landmarks3d = trans_landmarks3d*256 + 256
         
         trans_verts = transform_points(trans_verts, tform_invs, [224, 224], [512, 512])
         trans_landmarks2d = transform_points(trans_landmarks2d, tform_invs, [224, 224], [512, 512])*512/2+512/2
         trans_landmarks3d = transform_points(trans_landmarks3d, tform_invs, [224, 224], [512, 512])*512/2+512/2
+        trans_landmarks_756_3d = transform_points(trans_landmarks_756_3d, tform_invs, [224, 224], [512, 512])*512/2+512/2
 
-        return verts, landmarks2d, landmarks3d, trans_verts, trans_landmarks2d, trans_landmarks3d
+        return verts, landmarks2d, landmarks3d, trans_verts, trans_landmarks2d, trans_landmarks3d, trans_landmarks_756_2d, trans_landmarks_756_3d
 
     def get_dense_lmks(self):
         return
```

### Comparing `innerverz-0.1.3/innerverz/deca/models/FLAME.py` & `innerverz-0.1.4/innerverz/deca/models/FLAME.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import os
 import torch
 import torch.nn as nn
 import numpy as np
 import pickle
 import torch.nn.functional as F
 
+from ..utils.lmks_756 import indexes_756
 from .lbs import lbs, batch_rodrigues, vertices2landmarks, rot_mat_to_euler
 
 def to_tensor(array, dtype=torch.float32):
     if 'torch.tensor' not in str(type(array)):
         return torch.tensor(array, dtype=dtype)
 def to_np(array, dtype=np.float32):
     if 'scipy.sparse' in str(type(array)):
@@ -86,14 +87,17 @@
         neck_kin_chain = []; NECK_IDX=1
         curr_idx = torch.tensor(NECK_IDX, dtype=torch.long)
         while curr_idx != -1:
             neck_kin_chain.append(curr_idx)
             curr_idx = self.parents[curr_idx]
         self.register_buffer('neck_kin_chain', torch.stack(neck_kin_chain))
         
+        self.indexes_756 = torch.tensor(np.array(indexes_756, dtype=np.long), device=self.neck_kin_chain.device).unsqueeze(0)
+        
+        
     def _find_dynamic_lmk_idx_and_bcoords(self, pose, dynamic_lmk_faces_idx,
                                           dynamic_lmk_b_coords,
                                           neck_kin_chain, dtype=torch.float32):
         """
             Selects the face contour depending on the reletive position of the head
             Input:
                 vertices: N X num_of_vertices X 3
@@ -199,25 +203,30 @@
         lmk_faces_idx = self.lmk_faces_idx.unsqueeze(dim=0).expand(batch_size, -1)
         lmk_bary_coords = self.lmk_bary_coords.unsqueeze(dim=0).expand(batch_size, -1, -1)
         
         dyn_lmk_faces_idx, dyn_lmk_bary_coords = self._find_dynamic_lmk_idx_and_bcoords(
             full_pose, self.dynamic_lmk_faces_idx,
             self.dynamic_lmk_bary_coords,
             self.neck_kin_chain, dtype=self.dtype)
+        
+        
+        
         lmk_faces_idx = torch.cat([dyn_lmk_faces_idx, lmk_faces_idx], 1)
         lmk_bary_coords = torch.cat([dyn_lmk_bary_coords, lmk_bary_coords], 1)
-
         landmarks2d = vertices2landmarks(vertices, self.faces_tensor,
                                        lmk_faces_idx,
                                        lmk_bary_coords)
         bz = vertices.shape[0]
         landmarks3d = vertices2landmarks(vertices, self.faces_tensor,
                                        self.full_lmk_faces_idx.repeat(bz, 1),
                                        self.full_lmk_bary_coords.repeat(bz, 1, 1))
-        return vertices, landmarks2d, landmarks3d
+        
+        landmarks_756_3d = vertices.squeeze()[self.indexes_756.squeeze()].unsqueeze(0)
+        
+        return vertices, landmarks2d, landmarks3d, landmarks_756_3d
 
 class FLAMETex(nn.Module):
     """
     FLAME texture:
     https://github.com/TimoBolkart/TF_FLAME/blob/ade0ab152300ec5f0e8555d6765411555c5ed43d/sample_texture.py#L64
     FLAME texture converted from BFM:
     https://github.com/TimoBolkart/BFM_to_FLAME
```

### Comparing `innerverz-0.1.3/innerverz/deca/models/decoders.py` & `innerverz-0.1.4/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/models/detectors.py` & `innerverz-0.1.4/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/models/encoders.py` & `innerverz-0.1.4/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/models/face_detectors.py` & `innerverz-0.1.4/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/models/lbs.py` & `innerverz-0.1.4/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/models/resnet.py` & `innerverz-0.1.4/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/test.py` & `innerverz-0.1.4/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/utils/cfg.py` & `innerverz-0.1.4/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.1.4/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/utils/renderer.py` & `innerverz-0.1.4/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.1.4/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.1.4/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/utils/tracker_utils.py` & `innerverz-0.1.4/innerverz/deca/utils/tracker_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deca/utils/util.py` & `innerverz-0.1.4/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deep3dmm/main.py` & `innerverz-0.1.4/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deep3dmm/nets.py` & `innerverz-0.1.4/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/deep3dmm/test.py` & `innerverz-0.1.4/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.1.4/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_alignment/landmark.py` & `innerverz-0.1.4/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_alignment/main.py` & `innerverz-0.1.4/innerverz/face_alignment/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_alignment/retina_face.py` & `innerverz-0.1.4/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_alignment/test.py` & `innerverz-0.1.4/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.1.4/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_alignment/utils/transform.py` & `innerverz-0.1.4/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_color_transfer/main.py` & `innerverz-0.1.4/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_color_transfer/nets.py` & `innerverz-0.1.4/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.4/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_color_transfer/test.py` & `innerverz-0.1.4/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_enhancer/main.py` & `innerverz-0.1.4/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_enhancer/nets.py` & `innerverz-0.1.4/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_enhancer/test.py` & `innerverz-0.1.4/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/main.py` & `innerverz-0.1.4/innerverz/face_matting/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/decoders/resnet_decoder.py` & `innerverz-0.1.4/innerverz/face_matting/nets/decoders/resnet_decoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/encoders/MatteFormer.py` & `innerverz-0.1.4/innerverz/face_matting/nets/encoders/MatteFormer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/generators.py` & `innerverz-0.1.4/innerverz/face_matting/nets/generators.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/ops.py` & `innerverz-0.1.4/innerverz/face_matting/nets/ops.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/raft/main.py` & `innerverz-0.1.4/innerverz/face_matting/nets/raft/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/corr.py` & `innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/extractor.py` & `innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/update.py` & `innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/util.py` & `innerverz-0.1.4/innerverz/face_matting/nets/raft/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/nets/utils.py` & `innerverz-0.1.4/innerverz/face_matting/nets/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_matting/test.py` & `innerverz-0.1.4/innerverz/face_matting/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_parser/main.py` & `innerverz-0.1.4/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_parser/nets.py` & `innerverz-0.1.4/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_parser/test.py` & `innerverz-0.1.4/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_reshaping/main.py` & `innerverz-0.1.4/innerverz/face_reshaper/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import sys
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 from .nets import MyGenerator
-from .util import set_random_colors, plot_kpts
+from .util import set_random_colors, plot_kpts, plot_kpt
+from .vis_utils.vis_68 import contour_lines_68
+from .vis_utils.vis_756 import contour_lines_756
 from ..utils import check_ckpt_exist, get_url_id
 
 class Face_Reshaping(nn.Module):
-    def __init__(self, img_size : int = 512, folder_name='face_reshaping', ckpt_name = 'G_38k_unalign_multiaug.pt', force=False, device = 'cuda'):
+    def __init__(self, img_size : int = 512, color_num : int = 68, folder_name='face_reshaping', ckpt_name = 'G_38k_unalign_multiaug.pt', force=False, device = 'cuda'):
         """
             Related Links
             --------
             https://meta-portrait.github.io/
             
             Options
             --------
@@ -23,24 +25,24 @@
             
 
             
             get_vis_color_landmark
             --------
             - input
                 - lmks
-                    - shape : (68 2)
+                    - shape : (68 2) or (756,2)
                     
                 - size
                     - dtype : int
                     - default : 512
                     - plz check landmark size
 
                 - color_nums
                     - dtype : int
-                    - default : 68 + 3
+                    - default : 68 or 756
             
             - output
                 - dicts 'vis_color_lmk'
                     - dtype : numpy
                     - shape : (3, h, w)
                     - min max : (0 255)
             
@@ -81,21 +83,27 @@
         
         self.generator.load_state_dict(ckpt['model'])
         for param in self.generator.parameters():
             param.requires_grad = False
         self.generator.eval()
         del ckpt
         
-        self.colors = set_random_colors(color_num=68+3)
+        if color_num == 68:
+            self.contour_lines = np.array(contour_lines_68)
+            self.colors = set_random_colors(color_num=color_num)
+        elif color_num == 756:
+            self.contour_lines = np.array(contour_lines_756)
+            self.colors = set_random_colors(color_num=color_num)
         
-    def get_vis_color_landmark(self, lmks, size=512, color_num=68+3, dicts={}) -> dict:
-    # def get_vis_color_landmark(self, lmks, size=512, color_num=68+3):
+    def get_vis_color_landmark(self, lmks, size=512, dicts={}) -> dict:
         canvas = np.zeros((size, size, 3))
-        vis_lmk = plot_kpts(canvas, lmks, self.colors)
-        dicts['vis_color_lmk'] = vis_lmk
+        for (st, ed), color in zip(self.contour_lines, self.colors):
+            st_point, ed_point = lmks[int(st)], lmks[int(ed)]
+            canvas = plot_kpt(canvas, st_point, ed_point, color)
+        dicts['vis_color_lmk'] = canvas
         return dicts
 
     def forward(self, from_face, from_color_vis_lmk, to_color_vis_lmk, dicts={}) -> dict:
         inputs = torch.cat((from_color_vis_lmk, to_color_vis_lmk), dim=1)
         result = self.generator(from_face, inputs)
         dicts['from_vis_lmks'] = from_color_vis_lmk
         dicts['to_vis_lmks'] = to_color_vis_lmk
```

### Comparing `innerverz-0.1.3/innerverz/face_reshaping/nets.py` & `innerverz-0.1.4/innerverz/face_reshaper/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_reshaping/sub_nets/LadderEncoder.py` & `innerverz-0.1.4/innerverz/face_reshaper/sub_nets/LadderEncoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_reshaping/sub_nets/dense_motion.py` & `innerverz-0.1.4/innerverz/face_reshaper/sub_nets/dense_motion.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_reshaping/sub_nets/util.py` & `innerverz-0.1.4/innerverz/face_reshaper/sub_nets/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_reshaping/test.py` & `innerverz-0.1.4/innerverz/face_reshaper/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/face_reshaping/util.py` & `innerverz-0.1.4/innerverz/face_reshaper/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/head_color_transfer/main.py` & `innerverz-0.1.4/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/head_color_transfer/nets.py` & `innerverz-0.1.4/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.4/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/head_color_transfer/test.py` & `innerverz-0.1.4/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/id_extractor/main.py` & `innerverz-0.1.4/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/id_extractor/nets.py` & `innerverz-0.1.4/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/id_extractor/test.py` & `innerverz-0.1.4/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/reage/main.py` & `innerverz-0.1.4/innerverz/reage/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/reage/net.py` & `innerverz-0.1.4/innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/reage/net_utils.py` & `innerverz-0.1.4/innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/reage/test.py` & `innerverz-0.1.4/innerverz/reage/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/relighter/main.py` & `innerverz-0.1.4/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/relighter/nets.py` & `innerverz-0.1.4/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/relighter/test.py` & `innerverz-0.1.4/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/upsampler/main.py` & `innerverz-0.1.4/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/upsampler/nets.py` & `innerverz-0.1.4/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/upsampler/test.py` & `innerverz-0.1.4/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/utils/download.py` & `innerverz-0.1.4/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/utils/input.py` & `innerverz-0.1.4/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/utils/utils.py` & `innerverz-0.1.4/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/video_faceparser/main.py` & `innerverz-0.1.4/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/video_faceparser/nets.py` & `innerverz-0.1.4/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.1.4/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.1.4/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/video_faceparser/utils/update.py` & `innerverz-0.1.4/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz/video_faceparser/utils/util.py` & `innerverz-0.1.4/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.3/innerverz.egg-info/SOURCES.txt` & `innerverz-0.1.4/innerverz.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 innerverz/deca/models/detectors.py
 innerverz/deca/models/encoders.py
 innerverz/deca/models/face_detectors.py
 innerverz/deca/models/lbs.py
 innerverz/deca/models/resnet.py
 innerverz/deca/utils/__init__.py
 innerverz/deca/utils/cfg.py
+innerverz/deca/utils/lmks_756.py
 innerverz/deca/utils/renderer.py
 innerverz/deca/utils/rotation_converter.py
 innerverz/deca/utils/tensor_cropper.py
 innerverz/deca/utils/tracker_utils.py
 innerverz/deca/utils/util.py
 innerverz/deca/utils/rasterizer/__init__.py
 innerverz/deca/utils/rasterizer/setup.py
@@ -79,23 +80,26 @@
 innerverz/face_matting/nets/raft/utils/extractor.py
 innerverz/face_matting/nets/raft/utils/update.py
 innerverz/face_matting/nets/raft/utils/util.py
 innerverz/face_parser/__init__.py
 innerverz/face_parser/main.py
 innerverz/face_parser/nets.py
 innerverz/face_parser/test.py
-innerverz/face_reshaping/__init__.py
-innerverz/face_reshaping/main.py
-innerverz/face_reshaping/nets.py
-innerverz/face_reshaping/test.py
-innerverz/face_reshaping/util.py
-innerverz/face_reshaping/sub_nets/LadderEncoder.py
-innerverz/face_reshaping/sub_nets/__init__.py
-innerverz/face_reshaping/sub_nets/dense_motion.py
-innerverz/face_reshaping/sub_nets/util.py
+innerverz/face_reshaper/__init__.py
+innerverz/face_reshaper/main.py
+innerverz/face_reshaper/nets.py
+innerverz/face_reshaper/test.py
+innerverz/face_reshaper/util.py
+innerverz/face_reshaper/sub_nets/LadderEncoder.py
+innerverz/face_reshaper/sub_nets/__init__.py
+innerverz/face_reshaper/sub_nets/dense_motion.py
+innerverz/face_reshaper/sub_nets/util.py
+innerverz/face_reshaper/vis_utils/__init__.py
+innerverz/face_reshaper/vis_utils/vis_68.py
+innerverz/face_reshaper/vis_utils/vis_756.py
 innerverz/head_color_transfer/__init__.py
 innerverz/head_color_transfer/main.py
 innerverz/head_color_transfer/nets.py
 innerverz/head_color_transfer/test.py
 innerverz/head_color_transfer/sub_nets/__init__.py
 innerverz/head_color_transfer/sub_nets/blend_net.py
 innerverz/head_color_transfer/sub_nets/discriminator.py
```

### Comparing `innerverz-0.1.3/setup.py` & `innerverz-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.1.3",
+    version="0.1.4",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

