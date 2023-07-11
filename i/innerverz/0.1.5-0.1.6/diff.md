# Comparing `tmp/innerverz-0.1.5.tar.gz` & `tmp/innerverz-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.1.5.tar", last modified: Tue Jul 11 12:06:37 2023, max compression
+gzip compressed data, was "innerverz-0.1.6.tar", last modified: Tue Jul 11 12:13:17 2023, max compression
```

## Comparing `innerverz-0.1.5.tar` & `innerverz-0.1.6.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.521898 innerverz-0.1.5/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.5/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 12:06:37.522015 innerverz-0.1.5/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.5/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.496664 innerverz-0.1.5/innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1730 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.497719 innerverz-0.1.5/innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.498567 innerverz-0.1.5/innerverz/deblurrer/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deblurrer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2611 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deblurrer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deblurrer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      843 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.499064 innerverz-0.1.5/innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    24631 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.500467 innerverz-0.1.5/innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12950 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1200 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.502291 innerverz-0.1.5/innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/cfg.py
--rw-r--r--   0 jjy        (501) staff       (20)    19673 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/lmks_756.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.502591 innerverz-0.1.5/innerverz/deca/utils/rasterizer/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/rasterizer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      706 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    11870 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/tracker_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)    26664 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.503550 innerverz-0.1.5/innerverz/deep3dmm/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deep3dmm/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3582 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deep3dmm/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      627 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.504634 innerverz-0.1.5/innerverz/face_alignment/
--rw-r--r--   0 jjy        (501) staff       (20)      125 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_alignment/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_alignment/graphic_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_alignment/landmark.py
--rw-r--r--   0 jjy        (501) staff       (20)     8059 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_alignment/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      640 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.505117 innerverz-0.1.5/innerverz/face_alignment/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_alignment/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.505843 innerverz-0.1.5/innerverz/face_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5595 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.506610 innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2015 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.507184 innerverz-0.1.5/innerverz/face_enhancer/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_enhancer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3881 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_enhancer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      768 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.508297 innerverz-0.1.5/innerverz/face_matting/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8110 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.509379 innerverz-0.1.5/innerverz/face_matting/nets/
--rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.509699 innerverz-0.1.5/innerverz/face_matting/nets/decoders/
--rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/decoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/decoders/resnet_decoder.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.510015 innerverz-0.1.5/innerverz/face_matting/nets/encoders/
--rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/encoders/MatteFormer.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/encoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/generators.py
--rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/ops.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.510256 innerverz-0.1.5/innerverz/face_matting/nets/raft/
--rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/raft/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/raft/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.510945 innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/nets/utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_matting/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.511605 innerverz-0.1.5/innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2894 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      689 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.512446 innerverz-0.1.5/innerverz/face_reshaper/
--rw-r--r--   0 jjy        (501) staff       (20)       31 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3928 2023-07-11 12:06:15.000000 innerverz-0.1.5/innerverz/face_reshaper/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.513060 innerverz-0.1.5/innerverz/face_reshaper/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/sub_nets/LadderEncoder.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/sub_nets/dense_motion.py
--rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/sub_nets/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4694 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/test.py
--rw-r--r--   0 jjy        (501) staff       (20)     1750 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.513782 innerverz-0.1.5/innerverz/face_reshaper/vis_utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/vis_utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      885 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/vis_utils/vis_68.py
--rw-r--r--   0 jjy        (501) staff       (20)    10261 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/face_reshaper/vis_utils/vis_756.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.515122 innerverz-0.1.5/innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5773 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.515896 innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1965 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.517158 innerverz-0.1.5/innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2443 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      693 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.517917 innerverz-0.1.5/innerverz/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2618 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/reage/net_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)      763 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/reage/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.519144 innerverz-0.1.5/innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3213 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3030 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.519770 innerverz-0.1.5/innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/upsampler/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2429 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/upsampler/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      830 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.520341 innerverz-0.1.5/innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.520882 innerverz-0.1.5/innerverz/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.521041 innerverz-0.1.5/innerverz/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.521718 innerverz-0.1.5/innerverz/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-11 11:54:41.000000 innerverz-0.1.5/innerverz/video_faceparser/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:06:37.497439 innerverz-0.1.5/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 12:06:37.000000 innerverz-0.1.5/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     4955 2023-07-11 12:06:37.000000 innerverz-0.1.5/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-11 12:06:37.000000 innerverz-0.1.5/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-11 12:06:37.000000 innerverz-0.1.5/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-11 12:06:37.000000 innerverz-0.1.5/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.5/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-11 12:06:37.522352 innerverz-0.1.5/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-11 12:06:31.000000 innerverz-0.1.5/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.314030 innerverz-0.1.6/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.6/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 12:13:17.314126 innerverz-0.1.6/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.6/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.282776 innerverz-0.1.6/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1730 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.284427 innerverz-0.1.6/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.285533 innerverz-0.1.6/innerverz/deblurrer/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deblurrer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2611 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deblurrer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deblurrer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      843 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.286484 innerverz-0.1.6/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    24607 2023-07-11 12:11:09.000000 innerverz-0.1.6/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.287814 innerverz-0.1.6/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12950 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1200 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.289892 innerverz-0.1.6/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/cfg.py
+-rw-r--r--   0 jjy        (501) staff       (20)    19673 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/lmks_756.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.290427 innerverz-0.1.6/innerverz/deca/utils/rasterizer/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/rasterizer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      706 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11870 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/tracker_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26664 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.291569 innerverz-0.1.6/innerverz/deep3dmm/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deep3dmm/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3582 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deep3dmm/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      627 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.292866 innerverz-0.1.6/innerverz/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8059 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      640 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.293424 innerverz-0.1.6/innerverz/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.294438 innerverz-0.1.6/innerverz/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5595 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.295579 innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2015 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.296531 innerverz-0.1.6/innerverz/face_enhancer/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3881 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_enhancer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      768 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.297147 innerverz-0.1.6/innerverz/face_matting/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8110 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.298066 innerverz-0.1.6/innerverz/face_matting/nets/
+-rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.298557 innerverz-0.1.6/innerverz/face_matting/nets/decoders/
+-rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/decoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/decoders/resnet_decoder.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.299064 innerverz-0.1.6/innerverz/face_matting/nets/encoders/
+-rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/encoders/MatteFormer.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/encoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/generators.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/ops.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.299374 innerverz-0.1.6/innerverz/face_matting/nets/raft/
+-rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/raft/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/raft/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.300497 innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/nets/utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_matting/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.301337 innerverz-0.1.6/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2894 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      689 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.302373 innerverz-0.1.6/innerverz/face_reshaper/
+-rw-r--r--   0 jjy        (501) staff       (20)       31 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3928 2023-07-11 12:06:15.000000 innerverz-0.1.6/innerverz/face_reshaper/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.303072 innerverz-0.1.6/innerverz/face_reshaper/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/sub_nets/LadderEncoder.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/sub_nets/dense_motion.py
+-rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/sub_nets/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4694 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/test.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1750 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.303771 innerverz-0.1.6/innerverz/face_reshaper/vis_utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/vis_utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      885 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/vis_utils/vis_68.py
+-rw-r--r--   0 jjy        (501) staff       (20)    10261 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/face_reshaper/vis_utils/vis_756.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.304872 innerverz-0.1.6/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5773 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.306681 innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1965 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.307625 innerverz-0.1.6/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2443 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      693 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.308745 innerverz-0.1.6/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2618 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/reage/net_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)      763 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/reage/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.309537 innerverz-0.1.6/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3213 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3030 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.310649 innerverz-0.1.6/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/upsampler/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2429 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/upsampler/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      830 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.311426 innerverz-0.1.6/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.312434 innerverz-0.1.6/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.312711 innerverz-0.1.6/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.313823 innerverz-0.1.6/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-11 11:54:41.000000 innerverz-0.1.6/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-11 12:13:17.283748 innerverz-0.1.6/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-11 12:13:16.000000 innerverz-0.1.6/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     4955 2023-07-11 12:13:17.000000 innerverz-0.1.6/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-11 12:13:16.000000 innerverz-0.1.6/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-11 12:13:17.000000 innerverz-0.1.6/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-11 12:13:17.000000 innerverz-0.1.6/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.6/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-11 12:13:17.314447 innerverz-0.1.6/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-11 12:12:49.000000 innerverz-0.1.6/setup.py
```

### Comparing `innerverz-0.1.5/LICENSE.txt` & `innerverz-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/__init__.py` & `innerverz-0.1.6/innerverz/__init__.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/data_process/main.py` & `innerverz-0.1.6/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deblurrer/main.py` & `innerverz-0.1.6/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deblurrer/nets.py` & `innerverz-0.1.6/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deblurrer/test.py` & `innerverz-0.1.6/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/main.py` & `innerverz-0.1.6/innerverz/deca/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,11 +533,11 @@
         trans_landmarks_756_3d = batch_orth_proj(landmarks_756_3d, cam_params); trans_landmarks_756_3d[:,:,1:] = -trans_landmarks_756_3d[:,:,1:]; # trans_landmarks3d = trans_landmarks3d*256 + 256
         
         trans_verts = transform_points(trans_verts, tform_invs, [224, 224], [512, 512])
         trans_landmarks2d = transform_points(trans_landmarks2d, tform_invs, [224, 224], [512, 512])*512/2+512/2
         trans_landmarks3d = transform_points(trans_landmarks3d, tform_invs, [224, 224], [512, 512])*512/2+512/2
         trans_landmarks_756_3d = transform_points(trans_landmarks_756_3d, tform_invs, [224, 224], [512, 512])*512/2+512/2
 
-        return verts, landmarks2d, landmarks3d, trans_verts, trans_landmarks2d, trans_landmarks3d, trans_landmarks_756_2d, trans_landmarks_756_3d
+        return verts, landmarks2d, landmarks3d, trans_verts, trans_landmarks2d, trans_landmarks3d, trans_landmarks_756_3d
 
     def get_dense_lmks(self):
         return
```

### Comparing `innerverz-0.1.5/innerverz/deca/models/FLAME.py` & `innerverz-0.1.6/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/models/decoders.py` & `innerverz-0.1.6/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/models/detectors.py` & `innerverz-0.1.6/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/models/encoders.py` & `innerverz-0.1.6/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/models/face_detectors.py` & `innerverz-0.1.6/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/models/lbs.py` & `innerverz-0.1.6/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/models/resnet.py` & `innerverz-0.1.6/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/test.py` & `innerverz-0.1.6/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/utils/cfg.py` & `innerverz-0.1.6/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/utils/lmks_756.py` & `innerverz-0.1.6/innerverz/deca/utils/lmks_756.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.1.6/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/utils/renderer.py` & `innerverz-0.1.6/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.1.6/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.1.6/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/utils/tracker_utils.py` & `innerverz-0.1.6/innerverz/deca/utils/tracker_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deca/utils/util.py` & `innerverz-0.1.6/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deep3dmm/main.py` & `innerverz-0.1.6/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deep3dmm/nets.py` & `innerverz-0.1.6/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/deep3dmm/test.py` & `innerverz-0.1.6/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.1.6/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_alignment/landmark.py` & `innerverz-0.1.6/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_alignment/main.py` & `innerverz-0.1.6/innerverz/face_alignment/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_alignment/retina_face.py` & `innerverz-0.1.6/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_alignment/test.py` & `innerverz-0.1.6/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.1.6/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_alignment/utils/transform.py` & `innerverz-0.1.6/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_color_transfer/main.py` & `innerverz-0.1.6/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_color_transfer/nets.py` & `innerverz-0.1.6/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.6/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_color_transfer/test.py` & `innerverz-0.1.6/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_enhancer/main.py` & `innerverz-0.1.6/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_enhancer/nets.py` & `innerverz-0.1.6/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_enhancer/test.py` & `innerverz-0.1.6/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/main.py` & `innerverz-0.1.6/innerverz/face_matting/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/decoders/resnet_decoder.py` & `innerverz-0.1.6/innerverz/face_matting/nets/decoders/resnet_decoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/encoders/MatteFormer.py` & `innerverz-0.1.6/innerverz/face_matting/nets/encoders/MatteFormer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/generators.py` & `innerverz-0.1.6/innerverz/face_matting/nets/generators.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/ops.py` & `innerverz-0.1.6/innerverz/face_matting/nets/ops.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/raft/main.py` & `innerverz-0.1.6/innerverz/face_matting/nets/raft/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/corr.py` & `innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/extractor.py` & `innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/update.py` & `innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/raft/utils/util.py` & `innerverz-0.1.6/innerverz/face_matting/nets/raft/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/nets/utils.py` & `innerverz-0.1.6/innerverz/face_matting/nets/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_matting/test.py` & `innerverz-0.1.6/innerverz/face_matting/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_parser/main.py` & `innerverz-0.1.6/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_parser/nets.py` & `innerverz-0.1.6/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_parser/test.py` & `innerverz-0.1.6/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_reshaper/main.py` & `innerverz-0.1.6/innerverz/face_reshaper/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_reshaper/nets.py` & `innerverz-0.1.6/innerverz/face_reshaper/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_reshaper/sub_nets/LadderEncoder.py` & `innerverz-0.1.6/innerverz/face_reshaper/sub_nets/LadderEncoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_reshaper/sub_nets/dense_motion.py` & `innerverz-0.1.6/innerverz/face_reshaper/sub_nets/dense_motion.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_reshaper/sub_nets/util.py` & `innerverz-0.1.6/innerverz/face_reshaper/sub_nets/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_reshaper/test.py` & `innerverz-0.1.6/innerverz/face_reshaper/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_reshaper/util.py` & `innerverz-0.1.6/innerverz/face_reshaper/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_reshaper/vis_utils/vis_68.py` & `innerverz-0.1.6/innerverz/face_reshaper/vis_utils/vis_68.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/face_reshaper/vis_utils/vis_756.py` & `innerverz-0.1.6/innerverz/face_reshaper/vis_utils/vis_756.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/head_color_transfer/main.py` & `innerverz-0.1.6/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/head_color_transfer/nets.py` & `innerverz-0.1.6/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.6/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/head_color_transfer/test.py` & `innerverz-0.1.6/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/id_extractor/main.py` & `innerverz-0.1.6/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/id_extractor/nets.py` & `innerverz-0.1.6/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/id_extractor/test.py` & `innerverz-0.1.6/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/reage/main.py` & `innerverz-0.1.6/innerverz/reage/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/reage/net.py` & `innerverz-0.1.6/innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/reage/net_utils.py` & `innerverz-0.1.6/innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/reage/test.py` & `innerverz-0.1.6/innerverz/reage/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/relighter/main.py` & `innerverz-0.1.6/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/relighter/nets.py` & `innerverz-0.1.6/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/relighter/test.py` & `innerverz-0.1.6/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/upsampler/main.py` & `innerverz-0.1.6/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/upsampler/nets.py` & `innerverz-0.1.6/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/upsampler/test.py` & `innerverz-0.1.6/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/utils/download.py` & `innerverz-0.1.6/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/utils/input.py` & `innerverz-0.1.6/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/utils/utils.py` & `innerverz-0.1.6/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/video_faceparser/main.py` & `innerverz-0.1.6/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/video_faceparser/nets.py` & `innerverz-0.1.6/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.1.6/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.1.6/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/video_faceparser/utils/update.py` & `innerverz-0.1.6/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz/video_faceparser/utils/util.py` & `innerverz-0.1.6/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/innerverz.egg-info/SOURCES.txt` & `innerverz-0.1.6/innerverz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.5/setup.py` & `innerverz-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.1.5",
+    version="0.1.6",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

