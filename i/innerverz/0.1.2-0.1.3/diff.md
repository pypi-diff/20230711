# Comparing `tmp/innerverz-0.1.2.tar.gz` & `tmp/innerverz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.1.2.tar", last modified: Fri Jul  7 09:58:02 2023, max compression
+gzip compressed data, was "innerverz-0.1.3.tar", last modified: Tue Jul 11 06:21:50 2023, max compression
```

## Comparing `innerverz-0.1.2.tar` & `innerverz-0.1.3.tar`

### file list

```diff
@@ -1,168 +1,169 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.680818 innerverz-0.1.2/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.2/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-07 09:58:02.680923 innerverz-0.1.2/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.2/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.658133 innerverz-0.1.2/innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1739 2023-07-07 08:56:24.000000 innerverz-0.1.2/innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.659499 innerverz-0.1.2/innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-04 08:52:32.000000 innerverz-0.1.2/innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.660042 innerverz-0.1.2/innerverz/deblurrer/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deblurrer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2612 2023-07-05 10:22:28.000000 innerverz-0.1.2/innerverz/deblurrer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deblurrer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.660509 innerverz-0.1.2/innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    17533 2023-06-03 07:04:21.000000 innerverz-0.1.2/innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.661610 innerverz-0.1.2/innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.662424 innerverz-0.1.2/innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/cfg.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.662678 innerverz-0.1.2/innerverz/deca/utils/rasterizer/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/rasterizer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    26982 2023-06-03 07:04:12.000000 innerverz-0.1.2/innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.663214 innerverz-0.1.2/innerverz/deep3dmm/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deep3dmm/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3607 2023-07-04 11:21:58.000000 innerverz-0.1.2/innerverz/deep3dmm/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.664140 innerverz-0.1.2/innerverz/face_alignment/
--rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/graphic_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/landmark.py
--rw-r--r--   0 jjy        (501) staff       (20)    10096 2023-07-05 10:24:58.000000 innerverz-0.1.2/innerverz/face_alignment/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.664574 innerverz-0.1.2/innerverz/face_alignment/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.665120 innerverz-0.1.2/innerverz/face_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5352 2023-07-05 10:25:15.000000 innerverz-0.1.2/innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.666151 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.667820 innerverz-0.1.2/innerverz/face_enhancer/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_enhancer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3874 2023-07-04 11:15:07.000000 innerverz-0.1.2/innerverz/face_enhancer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.668237 innerverz-0.1.2/innerverz/face_matting/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-04 12:12:59.000000 innerverz-0.1.2/innerverz/face_matting/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8100 2023-07-05 10:55:26.000000 innerverz-0.1.2/innerverz/face_matting/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.668772 innerverz-0.1.2/innerverz/face_matting/nets/
--rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.669036 innerverz-0.1.2/innerverz/face_matting/nets/decoders/
--rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/decoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-05 10:54:16.000000 innerverz-0.1.2/innerverz/face_matting/nets/decoders/resnet_decoder.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.669337 innerverz-0.1.2/innerverz/face_matting/nets/encoders/
--rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-05 10:54:29.000000 innerverz-0.1.2/innerverz/face_matting/nets/encoders/MatteFormer.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/encoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-05 11:01:53.000000 innerverz-0.1.2/innerverz/face_matting/nets/generators.py
--rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/ops.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.669610 innerverz-0.1.2/innerverz/face_matting/nets/raft/
--rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.670261 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 12:13:24.000000 innerverz-0.1.2/innerverz/face_matting/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.671375 innerverz-0.1.2/innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2907 2023-07-07 08:51:48.000000 innerverz-0.1.2/innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.672108 innerverz-0.1.2/innerverz/face_reshaping/
--rw-r--r--   0 jjy        (501) staff       (20)       32 2023-07-07 08:56:40.000000 innerverz-0.1.2/innerverz/face_reshaping/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3309 2023-07-07 08:57:28.000000 innerverz-0.1.2/innerverz/face_reshaping/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-05 11:02:06.000000 innerverz-0.1.2/innerverz/face_reshaping/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.672650 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-04 10:48:50.000000 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/LadderEncoder.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-05 10:42:47.000000 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-05 10:51:39.000000 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/dense_motion.py
--rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-04 10:48:50.000000 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4687 2023-07-04 10:39:19.000000 innerverz-0.1.2/innerverz/face_reshaping/test.py
--rw-r--r--   0 jjy        (501) staff       (20)     1585 2023-07-04 10:39:19.000000 innerverz-0.1.2/innerverz/face_reshaping/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.673232 innerverz-0.1.2/innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5523 2023-07-05 10:29:48.000000 innerverz-0.1.2/innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.674845 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.675402 innerverz-0.1.2/innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2423 2023-07-04 11:16:46.000000 innerverz-0.1.2/innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.676068 innerverz-0.1.2/innerverz/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.1.2/innerverz/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2510 2023-07-04 12:34:32.000000 innerverz-0.1.2/innerverz/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.1.2/innerverz/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/reage/net_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.1.2/innerverz/reage/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.676979 innerverz-0.1.2/innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 10:45:51.000000 innerverz-0.1.2/innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.677588 innerverz-0.1.2/innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/upsampler/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2390 2023-07-05 10:28:22.000000 innerverz-0.1.2/innerverz/upsampler/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.678113 innerverz-0.1.2/innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.679428 innerverz-0.1.2/innerverz/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.679722 innerverz-0.1.2/innerverz/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-30 02:29:25.000000 innerverz-0.1.2/innerverz/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.680670 innerverz-0.1.2/innerverz/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.659219 innerverz-0.1.2/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     4758 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.2/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-07 09:58:02.681258 innerverz-0.1.2/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-07 09:57:56.000000 innerverz-0.1.2/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.080297 innerverz-0.1.3/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.3/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 06:21:50.080399 innerverz-0.1.3/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.3/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.059457 innerverz-0.1.3/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1733 2023-07-07 09:03:21.000000 innerverz-0.1.3/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.060525 innerverz-0.1.3/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-04 08:52:32.000000 innerverz-0.1.3/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.061091 innerverz-0.1.3/innerverz/deblurrer/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deblurrer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2611 2023-07-11 05:59:21.000000 innerverz-0.1.3/innerverz/deblurrer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deblurrer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      843 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.061549 innerverz-0.1.3/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    23911 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.062932 innerverz-0.1.3/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.1.3/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1200 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.063942 innerverz-0.1.3/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.064249 innerverz-0.1.3/innerverz/deca/utils/rasterizer/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/rasterizer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11870 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deca/utils/tracker_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26664 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.064842 innerverz-0.1.3/innerverz/deep3dmm/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deep3dmm/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3582 2023-07-11 05:48:53.000000 innerverz-0.1.3/innerverz/deep3dmm/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      627 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.065714 innerverz-0.1.3/innerverz/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8059 2023-07-11 06:18:23.000000 innerverz-0.1.3/innerverz/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      640 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.066475 innerverz-0.1.3/innerverz/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.067330 innerverz-0.1.3/innerverz/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5595 2023-07-11 06:04:34.000000 innerverz-0.1.3/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.068044 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2015 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.068633 innerverz-0.1.3/innerverz/face_enhancer/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3881 2023-07-11 06:05:17.000000 innerverz-0.1.3/innerverz/face_enhancer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      768 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.069315 innerverz-0.1.3/innerverz/face_matting/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-04 12:12:59.000000 innerverz-0.1.3/innerverz/face_matting/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8110 2023-07-11 06:06:04.000000 innerverz-0.1.3/innerverz/face_matting/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.069917 innerverz-0.1.3/innerverz/face_matting/nets/
+-rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.070209 innerverz-0.1.3/innerverz/face_matting/nets/decoders/
+-rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/decoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-05 10:54:16.000000 innerverz-0.1.3/innerverz/face_matting/nets/decoders/resnet_decoder.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.070666 innerverz-0.1.3/innerverz/face_matting/nets/encoders/
+-rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-05 10:54:29.000000 innerverz-0.1.3/innerverz/face_matting/nets/encoders/MatteFormer.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/encoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-05 11:01:53.000000 innerverz-0.1.3/innerverz/face_matting/nets/generators.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/ops.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.070934 innerverz-0.1.3/innerverz/face_matting/nets/raft/
+-rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.071851 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-04 12:12:37.000000 innerverz-0.1.3/innerverz/face_matting/nets/utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 12:13:24.000000 innerverz-0.1.3/innerverz/face_matting/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.072543 innerverz-0.1.3/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2894 2023-07-11 06:06:56.000000 innerverz-0.1.3/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      689 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.073247 innerverz-0.1.3/innerverz/face_reshaping/
+-rw-r--r--   0 jjy        (501) staff       (20)       32 2023-07-07 08:56:40.000000 innerverz-0.1.3/innerverz/face_reshaping/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3483 2023-07-11 06:09:10.000000 innerverz-0.1.3/innerverz/face_reshaping/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-05 11:02:06.000000 innerverz-0.1.3/innerverz/face_reshaping/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.073786 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-04 10:48:50.000000 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/LadderEncoder.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-05 10:42:47.000000 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-05 10:51:39.000000 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/dense_motion.py
+-rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-04 10:48:50.000000 innerverz-0.1.3/innerverz/face_reshaping/sub_nets/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4694 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/face_reshaping/test.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1750 2023-07-11 06:08:13.000000 innerverz-0.1.3/innerverz/face_reshaping/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.074527 innerverz-0.1.3/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5773 2023-07-11 06:09:54.000000 innerverz-0.1.3/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.075297 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1965 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.075885 innerverz-0.1.3/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2443 2023-07-11 06:10:48.000000 innerverz-0.1.3/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      693 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.076555 innerverz-0.1.3/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.1.3/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2618 2023-07-11 06:11:41.000000 innerverz-0.1.3/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.1.3/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/reage/net_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.1.3/innerverz/reage/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.077362 innerverz-0.1.3/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3213 2023-07-11 06:12:48.000000 innerverz-0.1.3/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3030 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.078081 innerverz-0.1.3/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/upsampler/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2429 2023-07-11 06:14:26.000000 innerverz-0.1.3/innerverz/upsampler/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      830 2023-07-11 05:45:46.000000 innerverz-0.1.3/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.078661 innerverz-0.1.3/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.079247 innerverz-0.1.3/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.079401 innerverz-0.1.3/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-30 02:29:25.000000 innerverz-0.1.3/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.080141 innerverz-0.1.3/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.1.3/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 06:21:50.060235 innerverz-0.1.3/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 06:21:49.000000 innerverz-0.1.3/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-11 06:21:50.000000 innerverz-0.1.3/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-11 06:21:49.000000 innerverz-0.1.3/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-11 06:21:49.000000 innerverz-0.1.3/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-11 06:21:49.000000 innerverz-0.1.3/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.3/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-11 06:21:50.080723 innerverz-0.1.3/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-11 06:21:35.000000 innerverz-0.1.3/setup.py
```

### Comparing `innerverz-0.1.2/LICENSE.txt` & `innerverz-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/__init__.py` & `innerverz-0.1.3/innerverz/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,20 +93,20 @@
 # reage
 --------
 
 from innerverz import Reage
 
 reage = Reage()
 
-# landmark_warping
+# face_reshaping
 --------
 
-from innerverz import Landmark_Warping
+from innerverz import Face_Reshaping
 
-LW = Landmark_Warping()
+LW = Face_Reshaping()
 
 # face_matting
 --------
 
 from innerverz import Face_Matting
 
 FM = Face_Matting()
```

### Comparing `innerverz-0.1.2/innerverz/data_process/main.py` & `innerverz-0.1.3/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deblurrer/main.py` & `innerverz-0.1.3/innerverz/deblurrer/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,26 +43,25 @@
         self.deblurrer = MyGenerator().to(self.device)
         self.deblurrer.load_state_dict(ckpt['model'])
         for param in self.deblurrer.parameters():
             param.requires_grad = False
         self.deblurrer.eval()
         del ckpt
         
-        self.dicts = {}
-
-    def forward(self, tensor_image, output_size=None):
+    def forward(self, tensor_image, output_size=None, dicts={}):
         _, _, origin_h, origin_w = tensor_image.shape
         tensor_image = F.interpolate(tensor_image, (self.size, self.size), mode='bilinear')
         fake, fake_res, edge = self.deblurrer(tensor_image)
         if output_size == None:
             _fake = F.interpolate(fake, (origin_h, origin_w), mode='bilinear')
             _fake_res = F.interpolate(fake_res, (origin_h, origin_w), mode='bilinear')
             _edge = F.interpolate(edge, (origin_h, origin_w), mode='bilinear')
         else:
             _fake = F.interpolate(fake, (output_size, output_size), mode='bilinear')
             _fake_res = F.interpolate(fake_res, (output_size, output_size), mode='bilinear')
             _edge = F.interpolate(edge, (output_size, output_size), mode='bilinear')
-            
-        self.dicts['fake'] = _fake
-        self.dicts['fake_res'] = _fake_res
-        self.dicts['edge'] = _edge
-        return self.dicts
+        
+        dicts['image'] = tensor_image
+        dicts['fake'] = _fake
+        dicts['fake_res'] = _fake_res
+        dicts['edge'] = _edge
+        return dicts
```

### Comparing `innerverz-0.1.2/innerverz/deblurrer/nets.py` & `innerverz-0.1.3/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deblurrer/test.py` & `innerverz-0.1.3/innerverz/deblurrer/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import cv2
 from PIL import Image
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 pil_image = Image.open(image_path)
 ts_image = DP.image_pp(pil_image, 512, normalize=True)
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 """
                 deblurrer usage
 """
-from innerverz_package import DeBlurrer
+from innerverz import DeBlurrer
 DB = DeBlurrer()
 ts_aligned_face = DP.image_pp(aligned_face, 1024, False, True, True, 'cuda')
 fake, fake_res, edge = DB(ts_aligned_face)
 _fake = DP.vis_pp(fake)
 _fake_res = DP.vis_pp(fake_res)
 _edge = DP.vis_pp(edge)
```

### Comparing `innerverz-0.1.2/innerverz/deca/models/FLAME.py` & `innerverz-0.1.3/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/models/decoders.py` & `innerverz-0.1.3/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/models/detectors.py` & `innerverz-0.1.3/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/models/encoders.py` & `innerverz-0.1.3/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/models/face_detectors.py` & `innerverz-0.1.3/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/models/lbs.py` & `innerverz-0.1.3/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/models/resnet.py` & `innerverz-0.1.3/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/test.py` & `innerverz-0.1.3/innerverz/deca/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import cv2
 import torch.nn.functional as F
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
 
-image_path = 'sample.png'
+image_path = 'sample1.png'
 DP = Data_Process()
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
-aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
+return_dict = FA.get_face(cv2_image)
+aligned_face, tfm, tfm_inv, lms_106, face_bool = return_dict['face_img'], return_dict['tfm'], return_dict['tfm_inv'], return_dict['lms_106'], return_dict['facebool']
 
-face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
-
-aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
-aligned_lmk = FA.affine_transform(lms_106, tfm)
+aligned_lmks_106 = FA.affine_transform(lms_106, tfm)['transform_lms_106']
 
 """
         DECA usage
 """
-from innerverz_package import DECA
+from innerverz import DECA
 deca = DECA()
-image_dict = deca.data_preprocess(aligned_face, aligned_lmk)
+image_dict = deca.data_preprocess(aligned_face, aligned_lmks_106)
 code_dict, vis_dict = deca(image_dict)
 
 inputs = DP.vis_pp(vis_dict['inputs'], normalize=False)
 landmarks2d = DP.vis_pp(vis_dict['landmarks2d'], normalize=False)
 landmarks3d = DP.vis_pp(vis_dict['landmarks3d'], normalize=False)
 shape_images = DP.vis_pp(vis_dict['shape_images'], normalize=False)
-shape_detail_images = DP.vis_pp(vis_dict['shape_detail_images'], normalize=False)
+shape_detail_images = DP.vis_pp(vis_dict['shape_detail_images'], normalize=False)
+
+cv2.imwrite('tmp.png', shape_detail_images/2 + aligned_face/2)
```

### Comparing `innerverz-0.1.2/innerverz/deca/utils/cfg.py` & `innerverz-0.1.3/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.1.3/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/utils/renderer.py` & `innerverz-0.1.3/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.1.3/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.1.3/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/deca/utils/util.py` & `innerverz-0.1.3/innerverz/deca/utils/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -636,32 +636,27 @@
     images = images.cpu().numpy()
     predicted_landmarks = landmarks.detach().cpu().numpy()
     if gt_landmarks is not None:
         gt_landmarks_np = gt_landmarks.detach().cpu().numpy()
     for i in range(images.shape[0]):
         image = images[i]
         image = image.transpose(1,2,0)[:,:,[2,1,0]].copy(); image = (image*255)
-        if isScale:
-            predicted_landmark = predicted_landmarks[i]
-            predicted_landmark[...,0] = predicted_landmark[...,0]*image.shape[1]/2 + image.shape[1]/2
-            predicted_landmark[...,1] = predicted_landmark[...,1]*image.shape[0]/2 + image.shape[0]/2
-        else:
-            predicted_landmark = predicted_landmarks[i]
+        predicted_landmark = predicted_landmarks[i]
         if predicted_landmark.shape[0] == 68:
             image_landmarks = plot_kpts(np.ones_like(image) * 127.5, predicted_landmark, color)
             if gt_landmarks is not None:
                 image_landmarks = plot_verts(image_landmarks, gt_landmarks_np[i]*image.shape[0]/2 + image.shape[0]/2, 'r')
         else:
             image_landmarks = plot_verts(image, predicted_landmark, color)
             if gt_landmarks is not None:
                 image_landmarks = plot_verts(image_landmarks, gt_landmarks_np[i]*image.shape[0]/2 + image.shape[0]/2, 'r')
         vis_landmarks.append(image_landmarks)
     vis_landmarks = np.stack(vis_landmarks)
     vis_landmarks = torch.from_numpy(vis_landmarks[:,:,:,[2,1,0]].transpose(0,3,1,2))/255.#, dtype=torch.float32)
-    return vis_landmarks, predicted_landmark
+    return vis_landmarks
 
 
 ############### for training
 def load_local_mask(image_size=256, mode='bbx'):
     if mode == 'bbx':
         # UV space face attributes bbx in size 2048 (l r t b)
         # face = np.array([512, 1536, 512, 1536]) #
```

### Comparing `innerverz-0.1.2/innerverz/deep3dmm/main.py` & `innerverz-0.1.3/innerverz/deep3dmm/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,14 @@
         ckpt=torch.load(ckpt_path, map_location=self.device)
         self.net_recon.load_state_dict(ckpt['net_recon'])
         for param in self.net_recon.parameters():
             param.requires_grad = False
         del ckpt
         self.facemodel = ParametricFaceModel(ckpt_name=BFM_name,is_train=False,device=self.device)
 
-        self.dicts = {}
-
     def get_coeff3d(self, img):
         """
         Input
         ---------
             - dtype : tensor
             - shape : (b, 3, 256, 256)
             - min max : (-1, 1)
```

### Comparing `innerverz-0.1.2/innerverz/deep3dmm/nets.py` & `innerverz-0.1.3/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.1.3/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_alignment/landmark.py` & `innerverz-0.1.3/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_alignment/retina_face.py` & `innerverz-0.1.3/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_alignment/test.py` & `innerverz-0.1.3/innerverz/face_alignment/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import cv2
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
```

### Comparing `innerverz-0.1.2/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.1.3/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_alignment/utils/transform.py` & `innerverz-0.1.3/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_color_transfer/main.py` & `innerverz-0.1.3/innerverz/face_color_transfer/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,17 +66,15 @@
 
         self.generator.load_state_dict(ckpt['model'])
         for param in self.generator.parameters():
             param.requires_grad = False
         self.generator.eval()
         del ckpt
         
-        self.dicts = {}
-        
-    def forward(self, source_rgb, target_rgb, source_onehot, target_onehot, target_gray, target_face_mask, output_size=None):
+    def forward(self, source_rgb, target_rgb, source_onehot, target_onehot, target_gray, target_face_mask, output_size=None, dicts={}):
         """
         Input
         ---------
             - source_rgb
                 - dtype : tensor
                 - shape : (b, 3, 512, 512)
                 - min max : (-1, 1)
@@ -124,10 +122,17 @@
         if output_size == None:
             result = F.interpolate(result, (origin_h, origin_w), mode='bilinear')
             color_reference_map = F.interpolate(color_reference_map, (origin_h, origin_w), mode='bilinear')
         else:
             result = F.interpolate(result, (output_size, output_size), mode='bilinear')
             color_reference_map = F.interpolate(color_reference_map, (output_size, output_size), mode='bilinear')
         
-        self.dicts['result'] = result
-        self.dicts['color_reference_map'] = color_reference_map
-        return self.dicts
+        dicts['source_rgb'] = source_rgb
+        dicts['target_rgb'] = target_rgb
+        dicts['source_onehot'] = source_onehot
+        dicts['target_onehot'] = target_onehot
+        dicts['target_gray'] = target_gray
+        dicts['target_face_mask'] = target_face_mask
+        dicts['result'] = result
+        dicts['color_reference_map'] = color_reference_map
+        return dicts
+
```

### Comparing `innerverz-0.1.2/innerverz/face_color_transfer/nets.py` & `innerverz-0.1.3/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.3/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_color_transfer/test.py` & `innerverz-0.1.3/innerverz/head_color_transfer/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,66 @@
+import torch
 import cv2
-import numpy as np
 from PIL import Image
-import torch
-from innerverz_package import Data_Process
+
+from innerverz import Data_Process
+from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 pil_image = Image.open(image_path)
 ts_image = DP.image_pp(pil_image, 512, normalize=True)
 
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 aligned_lmk = FA.affine_transform(lms_106, tfm)
 
-    
+
 """
         FaceParser usage
 """
-from innerverz_package import FaceParser
+from innerverz import FaceParser
 FP = FaceParser()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 label = FP.get_label(ts_aligned_face)
 pp_label = DP.vis_pp(label, normalize=False, color=False)
 
     
+
 """
-        face color transfer
+        head color transfer
 """
-from innerverz_package import IWCT
-iwct = IWCT()
+from innerverz import HWCT
+hwct = HWCT()
+
 # data pp
-pp_label = DP.vis_pp(label, normalize=False, color=False)
-convexhull_onehot = DP.label_pp(pp_label, 'convexhull', aligned_lmk/2, 512, one_hot=True)
+head_onehot = DP.label_pp(pp_label, 'head', aligned_lmk/2, 512, one_hot=True)
 gray_aligned_face = DP.image_pp(aligned_face, 512, True, True)
 color_aligned_face = DP.image_pp(aligned_face, 512, False, True)
-convexhull_mask = DP.label_pp(pp_label, 'convexhull', aligned_lmk/2, 512, one_hot=False)
-convexhull_mask = torch.where(convexhull_mask != 0, 1, 0)
-color_aligned_face = color_aligned_face * convexhull_mask
-gray_aligned_face = gray_aligned_face * convexhull_mask
+head_mask = DP.label_pp(pp_label, 'head', aligned_lmk/2, 512, one_hot=False)
+head_mask = torch.where(head_mask != 0, 1, 0)
+color_aligned_face = color_aligned_face * head_mask
+gray_aligned_face = gray_aligned_face * head_mask
 
-result, color_reference_map = iwct(color_aligned_face, gray_aligned_face.repeat(1,3,1,1), convexhull_onehot, convexhull_onehot, gray_aligned_face, convexhull_mask)
+result, color_reference_map = hwct(color_aligned_face, gray_aligned_face.repeat(1,3,1,1), head_onehot, head_onehot, gray_aligned_face, head_mask)
 _color_aligned_face = DP.vis_pp(color_aligned_face)
 _result = DP.vis_pp(result)
 _color_reference_map = DP.vis_pp(color_reference_map)
 
-cv2.imwrite('pp_label.png', pp_label*10+60)
-cv2.imwrite('color_alinged_face.png', _color_aligned_face)
-cv2.imwrite('ct_result.png', _result)
-cv2.imwrite('color_reference.png', _color_reference_map)
+cv2.imwrite('head_pp_label.png', pp_label*10+60)
+cv2.imwrite('head_color_alinged_face.png', _color_aligned_face)
+cv2.imwrite('head_ct_result.png', _result)
+cv2.imwrite('head_color_reference.png', _color_reference_map)
```

### Comparing `innerverz-0.1.2/innerverz/face_enhancer/main.py` & `innerverz-0.1.3/innerverz/face_enhancer/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,17 +50,15 @@
             for param in enhancer.parameters():
                 param.requires_grad = False
             enhancer.eval()
             del ckpt
 
         self.grad_mask = torch.from_numpy(get_grad_mask()).to(device)
         
-        self.dicts = {}
-
-    def forward(self, lmks, imgs):
+    def forward(self, lmks, imgs, dicts = {}):
         batch_num = imgs.size()[0]
 
         full_result = self.face_enhancer(imgs) # size: 1024, value range: [-1, 1]
 
         target_R_eye = torch.zeros((batch_num, 3, 256, 256), device=self.device)
         target_L_eye = torch.zeros((batch_num, 3, 256, 256), device=self.device) 
         target_Mouth = torch.zeros((batch_num, 3, 256, 256), device=self.device) 
@@ -78,10 +76,11 @@
         R_eye_result = self.eye_enhancer(target_R_eye)
         Mouth_result = self.mouth_enhancer(target_Mouth)
 
         full_result[:, :, L_yc-128:L_yc+128, L_xc-128:L_xc+128] = L_eye_result*self.grad_mask + full_result[:, :, L_yc-128:L_yc+128, L_xc-128:L_xc+128]*(1-self.grad_mask)
         full_result[:, :, R_yc-128:R_yc+128, R_xc-128:R_xc+128] = R_eye_result*self.grad_mask + full_result[:, :, R_yc-128:R_yc+128, R_xc-128:R_xc+128]*(1-self.grad_mask)
         full_result[:, :, M_yc-128:M_yc+128, M_xc-128:M_xc+128] = Mouth_result*self.grad_mask + full_result[:, :, M_yc-128:M_yc+128, M_xc-128:M_xc+128]*(1-self.grad_mask)
 
-        self.dicts['result'] = full_result
+        dicts['image'] = imgs
+        dicts['result'] = full_result
 
-        return self.dicts
+        return dicts
```

### Comparing `innerverz-0.1.2/innerverz/face_enhancer/nets.py` & `innerverz-0.1.3/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_enhancer/test.py` & `innerverz-0.1.3/innerverz/upsampler/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import cv2
+from PIL import Image
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 
-image_path = 'sample.png'
 DP = Data_Process()
 
+image_path = 'sample.png'
+pil_image = Image.open(image_path)
+ts_image = DP.image_pp(pil_image, 512, normalize=True)
+
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 aligned_lmk = FA.affine_transform(lms_106, tfm)
 
 """
-        face enhancer usage
+            Upsampler usage
 """
-from innerverz_package import FaceEnhancer
-FE = FaceEnhancer()
-ts_1024_aligned_face = DP.image_pp(aligned_face, 1024, normalize=True)
-result = FE(aligned_lmk[None,:,:], ts_1024_aligned_face)
-pp_result = DP.vis_pp(result, normalize=True, color=True)
+from innerverz import Upsampler
+US = Upsampler()
+ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=False)
+result = US(ts_aligned_face)
+_result = DP.vis_pp(result, normalize=False)
```

### Comparing `innerverz-0.1.2/innerverz/face_matting/main.py` & `innerverz-0.1.3/innerverz/face_matting/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.tf_color = transforms.Compose([
             transforms.Resize((self.img_size, self.img_size)),
             transforms.ToTensor(),
             transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))
         ])
         self.kernel = np.ones((3, 3), np.uint8)
         
-    def forward(self, image, trimap):
+    def forward(self, image, trimap, dicts={}):
         preds = self.generator(image, trimap)
             
         alpha_pred_os1, alpha_pred_os4, alpha_pred_os8 = preds['alpha_os1'], preds['alpha_os4'], preds['alpha_os8']
 
         # refinement
         alpha_pred = alpha_pred_os8.clone().detach()
         weight_os4 = get_unknown_tensor_from_pred(alpha_pred, rand_width=30, train_mode=False)
```

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/decoders/resnet_decoder.py` & `innerverz-0.1.3/innerverz/face_matting/nets/decoders/resnet_decoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/encoders/MatteFormer.py` & `innerverz-0.1.3/innerverz/face_matting/nets/encoders/MatteFormer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/generators.py` & `innerverz-0.1.3/innerverz/face_matting/nets/generators.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/ops.py` & `innerverz-0.1.3/innerverz/face_matting/nets/ops.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/raft/main.py` & `innerverz-0.1.3/innerverz/face_matting/nets/raft/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/corr.py` & `innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/extractor.py` & `innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/update.py` & `innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/util.py` & `innerverz-0.1.3/innerverz/face_matting/nets/raft/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/nets/utils.py` & `innerverz-0.1.3/innerverz/face_matting/nets/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_matting/test.py` & `innerverz-0.1.3/innerverz/face_matting/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_parser/main.py` & `innerverz-0.1.3/innerverz/face_parser/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,17 +44,15 @@
         
         self.parsing_net.load_state_dict(ckpt)
         for param in self.parsing_net.parameters():
             param.requires_grad = False
         self.parsing_net.eval()
         del ckpt
         
-        self.dicts = {}
-    
-    def get_label(self, tensor_img, output_size=512):
+    def get_label(self, tensor_img, output_size=512, dicts={}) -> dict:
         """
         Input
         ---------
             - dtype : tensor
             - shape : (b, 3, 512, 512)
             - min max : (-1, 1)
             
@@ -64,19 +62,19 @@
             - shape : (b, 512, 512)
             - min max : (0, 18)
         """
         label = self.parsing_net(tensor_img)
         _label = F.interpolate(label, (output_size,output_size), mode='bilinear').max(1)[1]
         _label = arrange_mask(_label, output_size)
         
-        self.dicts['label'] = _label
+        dicts['label'] = _label
         
-        return self.dicts
+        return dicts
     
-    def get_onehot(self, tensor_img, size=512):
+    def get_onehot(self, tensor_img, size=512, dicts={}) -> dict:
         """
         Input
         ---------
             - dtype : tensor
             - shape : (b, 3, 512, 512)
             - min max : (-1, 1)
             
@@ -84,9 +82,9 @@
         ---------
             - dtype : tensor
             - shape : (b, 19, size, size)
             - min max : (0 or 1)
         """
         label = self.get_label(tensor_img, size)
         onehot = get_one_hot(label.unsqueeze(0))
-        self.dicts['onehot'] = onehot
-        return self.dicts
+        dicts['onehot'] = onehot
+        return dicts
```

### Comparing `innerverz-0.1.2/innerverz/face_parser/nets.py` & `innerverz-0.1.3/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_parser/test.py` & `innerverz-0.1.3/innerverz/face_parser/test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import cv2
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 """
         FaceParser usage
 """
-from innerverz_package import FaceParser
+from innerverz import FaceParser
 FP = FaceParser()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 label = FP.get_label(ts_aligned_face)
 pp_label = DP.vis_pp(label, normalize=False, color=False)
```

### Comparing `innerverz-0.1.2/innerverz/face_reshaping/main.py` & `innerverz-0.1.3/innerverz/face_reshaping/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -81,22 +81,24 @@
         
         self.generator.load_state_dict(ckpt['model'])
         for param in self.generator.parameters():
             param.requires_grad = False
         self.generator.eval()
         del ckpt
         
-        self.dicts = {}
+        self.colors = set_random_colors(color_num=68+3)
         
-    def get_vis_color_landmark(self, lmks, size=512, color_num=68+3):
-        canvas = np.zeros_like((3, size, size))
-        colors = set_random_colors(color_num)
-        vis_lmk = plot_kpts(canvas, lmks, colors)
-        self.dicts['vis_color_lmk'] = vis_lmk
-        return self.dicts
+    def get_vis_color_landmark(self, lmks, size=512, color_num=68+3, dicts={}) -> dict:
+    # def get_vis_color_landmark(self, lmks, size=512, color_num=68+3):
+        canvas = np.zeros((size, size, 3))
+        vis_lmk = plot_kpts(canvas, lmks, self.colors)
+        dicts['vis_color_lmk'] = vis_lmk
+        return dicts
 
-    def forward(self, from_face, from_color_vis_lmk, to_color_vis_lmk):
+    def forward(self, from_face, from_color_vis_lmk, to_color_vis_lmk, dicts={}) -> dict:
         inputs = torch.cat((from_color_vis_lmk, to_color_vis_lmk), dim=1)
         result = self.generator(from_face, inputs)
-        self.dicts['result'] = result
-        return self.dicts
+        dicts['from_vis_lmks'] = from_color_vis_lmk
+        dicts['to_vis_lmks'] = to_color_vis_lmk
+        dicts['result'] = result
+        return dicts
```

### Comparing `innerverz-0.1.2/innerverz/face_reshaping/nets.py` & `innerverz-0.1.3/innerverz/face_reshaping/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_reshaping/sub_nets/LadderEncoder.py` & `innerverz-0.1.3/innerverz/face_reshaping/sub_nets/LadderEncoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_reshaping/sub_nets/dense_motion.py` & `innerverz-0.1.3/innerverz/face_reshaping/sub_nets/dense_motion.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_reshaping/sub_nets/util.py` & `innerverz-0.1.3/innerverz/face_reshaping/sub_nets/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/face_reshaping/test.py` & `innerverz-0.1.3/innerverz/face_reshaping/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 from innerverz import FaceAligner
 FA = FaceAligner(512, align_style='ffhq')
 
 from innerverz import DECA
 deca = DECA()
 
-from util import set_random_colors, plot_kpts
+from .util import set_random_colors, plot_kpts
 
-from main import LMK_Warping
-g = LMK_Warping()
+from main import Face_Reshaping
+g = Face_Reshaping()
 
 source_list = [
     'YEJI.png',
     'WINTER.png',
     'uc_388.png',
     'uc_648.png',
     'HYERI.jpg',
```

### Comparing `innerverz-0.1.2/innerverz/face_reshaping/util.py` & `innerverz-0.1.3/innerverz/face_reshaping/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import numpy as np
 from PIL import Image
 
 # random color
 
 def set_random_colors(num=68+3):
     colors = []
-    cube_root = num
+    cube_root = num ** (1.0 / 3)
     for r in range(0, 255, int(255 / cube_root)):
         for g in range(0, 255, int(255 / cube_root)):
             for b in range(0, 255, int(255 / cube_root)):
                 colors.append([int(r), int(g), int(b)])
     random.shuffle(colors)
     return colors
-    
 # ---------------------------------- visualization
 # end_list = np.array([17, 21], dtype = np.int32) - 1
 end_list = np.array([17, 22, 27, 42, 48, 31, 36, 68], dtype = np.int32) - 1
 def plot_kpts(image, kpts, colors):
     ''' Draw 68 key points
     Args: 
         image: the input image
@@ -37,7 +36,11 @@
         image = cv2.line(image, (int(st[0]), int(st[1])), (int(ed[0]), int(ed[1])), color, 1,  cv2.LINE_AA)
 
     image = cv2.line(image, (int(kpts[42-1][0]), int(kpts[42-1][1])), (int(kpts[37-1][0]), int(kpts[37-1][1])), colors[-3], 1,  cv2.LINE_AA)
     image = cv2.line(image, (int(kpts[48-1][0]), int(kpts[48-1][1])), (int(kpts[43-1][0]), int(kpts[43-1][1])), colors[-2], 1,  cv2.LINE_AA)
     image = cv2.line(image, (int(kpts[68-1][0]), int(kpts[68-1][1])), (int(kpts[61-1][0]), int(kpts[61-1][1])), colors[-1], 1,  cv2.LINE_AA)
 
     return image
+
+def plot_kpt(image, st, ed, color):
+    image = cv2.line(image, (int(st[0]), int(st[1])), (int(ed[0]), int(ed[1])), color, 1, cv2.LINE_AA)
+    return image
```

### Comparing `innerverz-0.1.2/innerverz/head_color_transfer/main.py` & `innerverz-0.1.3/innerverz/head_color_transfer/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,17 +74,15 @@
        
         self.generator.load_state_dict(ckpt['model'], strict=True)
         for param in self.generator.parameters():
             param.requires_grad = False
         self.generator.eval()
         del ckpt
         
-        self.dicts = {}
-
-    def forward(self, source_rgb, target_rgb, source_onehot, target_onehot, target_gray, target_face_mask, output_size=None):
+    def forward(self, source_rgb, target_rgb, source_onehot, target_onehot, target_gray, target_face_mask, output_size=None, dicts={}) -> dict:
         """
         Input
         ---------
             - source_rgb
                 - dtype : tensor
                 - shape : (b, 3, 512, 512)
                 - min max : (-1, 1)
@@ -133,11 +131,17 @@
         if output_size == None:
             result = F.interpolate(result, (origin_h, origin_w), mode='bilinear')
             color_reference_map = F.interpolate(color_reference_map, (origin_h, origin_w), mode='bilinear')
         else:
             result = F.interpolate(result, (output_size, output_size), mode='bilinear')
             color_reference_map = F.interpolate(color_reference_map, (output_size, output_size), mode='bilinear')
         
-        self.dicts['result'] = result
-        self.dicts['color_reference_map'] = color_reference_map
-        return self.dicts
+        dicts['source_rgb'] = source_rgb
+        dicts['target_rgb'] = target_rgb
+        dicts['source_onehot'] = source_onehot
+        dicts['target_onehot'] = target_onehot
+        dicts['target_gray'] = target_gray
+        dicts['target_face_mask'] = target_face_mask
+        dicts['result'] = result
+        dicts['color_reference_map'] = color_reference_map
+        return dicts
```

### Comparing `innerverz-0.1.2/innerverz/head_color_transfer/nets.py` & `innerverz-0.1.3/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.3/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/head_color_transfer/test.py` & `innerverz-0.1.3/innerverz/face_color_transfer/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,64 @@
-import torch
 import cv2
+import numpy as np
 from PIL import Image
-
-from innerverz_package import Data_Process
-from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
+import torch
+from innerverz import Data_Process
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 pil_image = Image.open(image_path)
 ts_image = DP.image_pp(pil_image, 512, normalize=True)
 
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 aligned_lmk = FA.affine_transform(lms_106, tfm)
 
-
+    
 """
         FaceParser usage
 """
-from innerverz_package import FaceParser
+from innerverz import FaceParser
 FP = FaceParser()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 label = FP.get_label(ts_aligned_face)
 pp_label = DP.vis_pp(label, normalize=False, color=False)
 
     
-
 """
-        head color transfer
+        face color transfer
 """
-from innerverz_package import HWCT
-hwct = HWCT()
-
+from innerverz import IWCT
+iwct = IWCT()
 # data pp
-head_onehot = DP.label_pp(pp_label, 'head', aligned_lmk/2, 512, one_hot=True)
+pp_label = DP.vis_pp(label, normalize=False, color=False)
+convexhull_onehot = DP.label_pp(pp_label, 'convexhull', aligned_lmk/2, 512, one_hot=True)
 gray_aligned_face = DP.image_pp(aligned_face, 512, True, True)
 color_aligned_face = DP.image_pp(aligned_face, 512, False, True)
-head_mask = DP.label_pp(pp_label, 'head', aligned_lmk/2, 512, one_hot=False)
-head_mask = torch.where(head_mask != 0, 1, 0)
-color_aligned_face = color_aligned_face * head_mask
-gray_aligned_face = gray_aligned_face * head_mask
+convexhull_mask = DP.label_pp(pp_label, 'convexhull', aligned_lmk/2, 512, one_hot=False)
+convexhull_mask = torch.where(convexhull_mask != 0, 1, 0)
+color_aligned_face = color_aligned_face * convexhull_mask
+gray_aligned_face = gray_aligned_face * convexhull_mask
 
-result, color_reference_map = hwct(color_aligned_face, gray_aligned_face.repeat(1,3,1,1), head_onehot, head_onehot, gray_aligned_face, head_mask)
+result, color_reference_map = iwct(color_aligned_face, gray_aligned_face.repeat(1,3,1,1), convexhull_onehot, convexhull_onehot, gray_aligned_face, convexhull_mask)
 _color_aligned_face = DP.vis_pp(color_aligned_face)
 _result = DP.vis_pp(result)
 _color_reference_map = DP.vis_pp(color_reference_map)
 
-cv2.imwrite('head_pp_label.png', pp_label*10+60)
-cv2.imwrite('head_color_alinged_face.png', _color_aligned_face)
-cv2.imwrite('head_ct_result.png', _result)
-cv2.imwrite('head_color_reference.png', _color_reference_map)
+cv2.imwrite('pp_label.png', pp_label*10+60)
+cv2.imwrite('color_alinged_face.png', _color_aligned_face)
+cv2.imwrite('ct_result.png', _result)
+cv2.imwrite('color_reference.png', _color_reference_map)
```

### Comparing `innerverz-0.1.2/innerverz/id_extractor/main.py` & `innerverz-0.1.3/innerverz/id_extractor/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,17 +36,16 @@
         self.id_extractor.load_state_dict(ckpt)
         for param in self.id_extractor.parameters():
             param.requires_grad = False
         del ckpt
 
         self.x, self.y, self.w, self.h = x, y, w, h
         
-        self.dicts = {}
 
-    def forward(self, tensor_img):
+    def forward(self, tensor_img, dicts={}) -> dict:
         """
         Input
         ---------
             - dtype : tensor
             - shape : (b, 3, h, w)
             - min max : (-1, 1)
             
@@ -55,16 +54,17 @@
             dict
             - type : tensor
             - shape : (b, 512)
         """
         tensor_img = F.interpolate(tensor_img, (256,256))
         tensor_img = F.interpolate(tensor_img[..., self.y:self.y+self.h, self.x:self.x+self.w], (112, 112), mode='bilinear')
         id_vector = self.id_extractor(tensor_img)
-        self.dicts['id_vector'] = id_vector
-        return self.dicts
+        dicts['image'] = tensor_img
+        dicts['id_vector'] = id_vector
+        return dicts
     
     def compare_similarity(self, id1, id2):
         """
         Input
         ---------
             - dtype : tensor
             - shape : id1 (1, 512) / id2 (1, 512)
```

### Comparing `innerverz-0.1.2/innerverz/id_extractor/nets.py` & `innerverz-0.1.3/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/reage/main.py` & `innerverz-0.1.3/innerverz/reage/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,20 +61,22 @@
 
         self.generator.load_state_dict(ckpt['model'])
         for param in self.generator.parameters():
             param.requires_grad = False
         self.generator.eval()
         del ckpt
         
-        self.dicts = {}
-        
-    def forward(self, masked_image, mask, from_age, to_age):
+    def forward(self, masked_image, mask, from_age, to_age, dicts={}) -> dict:
         
         model_input = torch.cat((masked_image, mask * from_age / 100, mask * to_age / 100), dim=1)
         
         delta = self.generator(model_input)
         result = masked_image + delta
         
-        self.dicts['result'] = result
-        self.dicts['delta'] = delta
         
-        return self.dicts
+        dicts['image'] = masked_image
+        dicts['mask'] = mask
+        dicts['from_age'] = from_age
+        dicts['to_age'] = to_age
+        dicts['result'] = result
+        dicts['delta'] = delta
+        return  dicts
```

### Comparing `innerverz-0.1.2/innerverz/reage/net.py` & `innerverz-0.1.3/innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/reage/net_utils.py` & `innerverz-0.1.3/innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/reage/test.py` & `innerverz-0.1.3/innerverz/reage/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/relighter/main.py` & `innerverz-0.1.3/innerverz/relighter/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,18 +60,16 @@
         ckpt = torch.load(os.path.join(ckpt_path), map_location=self.device)
         self.generator.load_state_dict(ckpt['model'])
         for param in self.generator.parameters():
             param.requires_grad = False
         self.generator.eval()
         del ckpt
 
-        self.dicts = {}
-
     # source light -> target light
-    def forward(self, masked_gray_face, relight_detail_shape, code_dict, id_param, output_size=None):
+    def forward(self, masked_gray_face, relight_detail_shape, code_dict, id_param, output_size=None, dicts={}):
         _, _, origin_h, origin_w = masked_gray_face.shape
         
         masked_gray_face = F.interpolate(masked_gray_face, (self.img_size, self.img_size), mode='bilinear')
         relight_detail_shape = F.interpolate(relight_detail_shape, (self.img_size, self.img_size), mode='bilinear')
         
         params = torch.cat((code_dict['light'].view(1, -1), code_dict['cam'].view(1, -1), code_dict['pose'].view(1, -1), code_dict['detail'].view(1, -1), id_param), dim=-1)
         res = self.generator(masked_gray_face, relight_detail_shape, params)
@@ -80,12 +78,13 @@
         if output_size == None:
             _result = F.interpolate(result, (origin_h, origin_w), mode='bilinear')
             _res = F.interpolate(res, (origin_h, origin_w), mode='bilinear')
         else:
             _result = F.interpolate(result, (output_size, output_size), mode='bilinear')
             _res = F.interpolate(res, (output_size, output_size), mode='bilinear')
         
-        self.dicts['result'] = _result
-        self.dicts['res'] = _res
-        
-        return self.dicts
+        dicts['image'] = masked_gray_face
+        dicts['detail_shape'] = relight_detail_shape
+        dicts['result'] = _result
+        dicts['res'] = _res
+        return dicts
```

### Comparing `innerverz-0.1.2/innerverz/relighter/nets.py` & `innerverz-0.1.3/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/relighter/test.py` & `innerverz-0.1.3/innerverz/relighter/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import cv2
 import numpy as np
 from PIL import Image
 
 import torch
 import torch.nn.functional as F
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 pil_image = Image.open(image_path)
 ts_image = DP.image_pp(pil_image, 512, normalize=True)
 
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
@@ -30,31 +30,31 @@
 
 aligned_lmk = FA.affine_transform(lms_106, tfm)
 
     
 """
         FaceParser usage
 """
-from innerverz_package import FaceParser
+from innerverz import FaceParser
 FP = FaceParser()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 label = FP.get_label(ts_aligned_face)
 pp_label = DP.vis_pp(label, normalize=False, color=False)
 
 """
             Relighting usage
 """
-from innerverz_package import ReLighter
+from innerverz import ReLighter
 RL = ReLighter()
 
-from innerverz_package import IdExtractor
+from innerverz import IdExtractor
 IE = IdExtractor()
 
-from innerverz_package import DECA
+from innerverz import DECA
 deca = DECA()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 id_vector = IE(ts_aligned_face)
 
 # pp
 color_aligned_face = DP.image_pp(aligned_face, 512, False, True, False, 'cpu')
```

### Comparing `innerverz-0.1.2/innerverz/upsampler/main.py` & `innerverz-0.1.3/innerverz/upsampler/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,22 +44,23 @@
         for param in self.sr_net.parameters():
             param.requires_grad = False
         self.sr_net.eval()
         del ckpt
         
         self.dicts = {}
         
-    def forward(self, x, output_size=None):
+    def forward(self, x, output_size=None, dicts={}) -> dict:
         W, H = x.size()[-1] ,x.size()[-2] 
         if W!=256 or H!=256:
             x = F.interpolate(x, (256,256), mode='bilinear')
         
         with torch.no_grad():
             result = self.sr_net(x)
             if output_size == None:
                 _result = F.interpolate(result, (1024, 1024), mode='bilinear')
             else:
                 _result = F.interpolate(result, (output_size, output_size), mode='bilinear')
                 
-            self.dicts['result'] = _result
-            return self.dicts
+            dicts['image'] = x
+            dicts['result'] = _result
+            return dicts
```

### Comparing `innerverz-0.1.2/innerverz/upsampler/nets.py` & `innerverz-0.1.3/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/utils/download.py` & `innerverz-0.1.3/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/utils/input.py` & `innerverz-0.1.3/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/utils/utils.py` & `innerverz-0.1.3/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/video_faceparser/main.py` & `innerverz-0.1.3/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/video_faceparser/nets.py` & `innerverz-0.1.3/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.1.3/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.1.3/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/video_faceparser/utils/update.py` & `innerverz-0.1.3/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz/video_faceparser/utils/util.py` & `innerverz-0.1.3/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.2/innerverz.egg-info/SOURCES.txt` & `innerverz-0.1.3/innerverz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 innerverz/deca/models/lbs.py
 innerverz/deca/models/resnet.py
 innerverz/deca/utils/__init__.py
 innerverz/deca/utils/cfg.py
 innerverz/deca/utils/renderer.py
 innerverz/deca/utils/rotation_converter.py
 innerverz/deca/utils/tensor_cropper.py
+innerverz/deca/utils/tracker_utils.py
 innerverz/deca/utils/util.py
 innerverz/deca/utils/rasterizer/__init__.py
 innerverz/deca/utils/rasterizer/setup.py
 innerverz/deep3dmm/__init__.py
 innerverz/deep3dmm/main.py
 innerverz/deep3dmm/nets.py
 innerverz/deep3dmm/test.py
```

### Comparing `innerverz-0.1.2/setup.py` & `innerverz-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.1.2",
+    version="0.1.3",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

