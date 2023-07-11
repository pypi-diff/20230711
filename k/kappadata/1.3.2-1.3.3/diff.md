# Comparing `tmp/kappadata-1.3.2.tar.gz` & `tmp/kappadata-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappadata-1.3.2.tar", last modified: Mon Jul 10 20:38:58 2023, max compression
+gzip compressed data, was "kappadata-1.3.3.tar", last modified: Tue Jul 11 12:53:16 2023, max compression
```

## Comparing `kappadata-1.3.2.tar` & `kappadata-1.3.3.tar`

### file list

```diff
@@ -1,197 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.196143 kappadata-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 20:36:28.000000 kappadata-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-10 20:38:58.196143 kappadata-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-10 20:36:28.000000 kappadata-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.156143 kappadata-1.3.2/kappadata/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 20:38:41.000000 kappadata-1.3.2/kappadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.156143 kappadata-1.3.2/kappadata/caching/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/caching/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/caching/shared_dict_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.160143 kappadata-1.3.2/kappadata/collators/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/collators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.160143 kappadata-1.3.2/kappadata/collators/base/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/collators/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/collators/base/kd_collator_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/collators/base/kd_compose_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/collators/base/kd_single_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/collators/kd_mix_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/collators/pad_sequences_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.160143 kappadata-1.3.2/kappadata/common/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.160143 kappadata-1.3.2/kappadata/common/collators/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/collators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/collators/mae_finetune_mix_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.160143 kappadata-1.3.2/kappadata/common/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/datasets/kd_image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.164143 kappadata-1.3.2/kappadata/common/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/byol_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/imagenet_minaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/imagenet_noaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/mae_finetune_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.164143 kappadata-1.3.2/kappadata/common/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/norm/kd_ade20k_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/norm/kd_cifar100_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/norm/kd_cifar10_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/transforms/norm/kd_image_net_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.164143 kappadata-1.3.2/kappadata/common/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.168143 kappadata-1.3.2/kappadata/common/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/wrappers/sample_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.168143 kappadata-1.3.2/kappadata/copying/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/copying/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/copying/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/copying/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.172143 kappadata-1.3.2/kappadata/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/datasets/kd_concat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/datasets/kd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/datasets/kd_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/datasets/kd_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/error_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.172143 kappadata-1.3.2/kappadata/loading/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/loading/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.172143 kappadata-1.3.2/kappadata/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/samplers/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/samplers/infinite_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/samplers/interleaved_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/samplers/semi_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/samplers/sequential_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.184143 kappadata-1.3.2/kappadata/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.184143 kappadata-1.3.2/kappadata/transforms/base/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/base/kd_compose_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/base/kd_identity_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/base/kd_random_apply_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/base/kd_scheduled_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/base/kd_stochastic_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/base/kd_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/image_pos_embed_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/image_pos_embed_sincos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_additive_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_bucketize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_columnwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_minsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_rand_augment_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_additive_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_erasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_resized_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_random_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_rearrange.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_simple_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_three_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/kd_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.184143 kappadata-1.3.2/kappadata/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/norm/kd_image_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/norm/kd_image_range_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/norm/kd_norm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/patchify_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/patchwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/patchwise_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/patchwise_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/save_state_to_context_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.184143 kappadata-1.3.2/kappadata/transforms/semseg/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/semseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/semseg/kd_semseg_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/semseg/kd_semseg_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/semseg/kd_semseg_random_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/semseg/kd_semseg_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/transforms/unpatchify_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.188144 kappadata-1.3.2/kappadata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/bounding_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/class_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/color_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/getall_class_as_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/magnitude_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/multi_crop_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/param_checking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/pos_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/utils/transform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.188144 kappadata-1.3.2/kappadata/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/visualization/visualize_dataset_imgsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/visualization/visualize_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/visualization/visualize_jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/visualization/visualize_mae_schematic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/visualization/visualize_masked_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/visualization/visualize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/visualization/visualize_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.192144 kappadata-1.3.2/kappadata/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.192144 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/mode_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.192144 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.192144 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-10 20:36:28.000000 kappadata-1.3.2/kappadata/wrappers/torch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.156143 kappadata-1.3.2/kappadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-10 20:38:58.000000 kappadata-1.3.2/kappadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-10 20:38:58.000000 kappadata-1.3.2/kappadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:38:58.000000 kappadata-1.3.2/kappadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 20:38:58.000000 kappadata-1.3.2/kappadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 20:38:58.000000 kappadata-1.3.2/kappadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 20:36:28.000000 kappadata-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-10 20:38:58.196143 kappadata-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:38:58.192144 kappadata-1.3.2/test_unit_long/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:28.000000 kappadata-1.3.2/test_unit_long/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-10 20:36:28.000000 kappadata-1.3.2/test_unit_long/test_stochastic_transform_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.538794 kappadata-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 12:50:47.000000 kappadata-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-11 12:53:16.538794 kappadata-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-11 12:50:47.000000 kappadata-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.510794 kappadata-1.3.3/kappadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 12:52:59.000000 kappadata-1.3.3/kappadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.514794 kappadata-1.3.3/kappadata/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/caching/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/caching/shared_dict_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.514794 kappadata-1.3.3/kappadata/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/collators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.514794 kappadata-1.3.3/kappadata/collators/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/collators/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/collators/base/kd_collator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/collators/base/kd_compose_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/collators/base/kd_single_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/collators/kd_dino_mask_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/collators/kd_mix_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/collators/pad_sequences_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.514794 kappadata-1.3.3/kappadata/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.514794 kappadata-1.3.3/kappadata/common/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/collators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/collators/mae_finetune_mix_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.514794 kappadata-1.3.3/kappadata/common/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/datasets/kd_image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.514794 kappadata-1.3.3/kappadata/common/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/byol_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/imagenet_minaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/imagenet_noaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/mae_finetune_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.518794 kappadata-1.3.3/kappadata/common/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/norm/kd_ade20k_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/norm/kd_cifar100_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/norm/kd_cifar10_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/transforms/norm/kd_image_net_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.518794 kappadata-1.3.3/kappadata/common/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.518794 kappadata-1.3.3/kappadata/common/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/wrappers/sample_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.518794 kappadata-1.3.3/kappadata/copying/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/copying/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/copying/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/copying/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.518794 kappadata-1.3.3/kappadata/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/datasets/kd_concat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/datasets/kd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/datasets/kd_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/datasets/kd_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.518794 kappadata-1.3.3/kappadata/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/loading/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.518794 kappadata-1.3.3/kappadata/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/samplers/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/samplers/infinite_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/samplers/interleaved_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/samplers/semi_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/samplers/sequential_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.526794 kappadata-1.3.3/kappadata/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.526794 kappadata-1.3.3/kappadata/transforms/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/base/kd_compose_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/base/kd_identity_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/base/kd_random_apply_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/base/kd_scheduled_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/base/kd_stochastic_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/base/kd_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/image_pos_embed_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/image_pos_embed_sincos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_columnwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_minsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_rand_augment_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_erasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_resized_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_random_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_rearrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_simple_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_three_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/kd_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.526794 kappadata-1.3.3/kappadata/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/norm/kd_image_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/norm/kd_image_range_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/norm/kd_norm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/patchify_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/patchwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/patchwise_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/patchwise_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/save_state_to_context_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.530794 kappadata-1.3.3/kappadata/transforms/semseg/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/semseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/semseg/kd_semseg_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/semseg/kd_semseg_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/semseg/kd_semseg_random_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/semseg/kd_semseg_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/transforms/unpatchify_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.530794 kappadata-1.3.3/kappadata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/bounding_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/class_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/color_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/getall_class_as_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/magnitude_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/multi_crop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/param_checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/pos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/utils/transform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.534794 kappadata-1.3.3/kappadata/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/visualization/visualize_dataset_imgsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/visualization/visualize_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/visualization/visualize_jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/visualization/visualize_mae_schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/visualization/visualize_masked_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/visualization/visualize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/visualization/visualize_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.534794 kappadata-1.3.3/kappadata/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.534794 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/mode_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.538794 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.538794 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 12:50:47.000000 kappadata-1.3.3/kappadata/wrappers/torch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.514794 kappadata-1.3.3/kappadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-11 12:53:16.000000 kappadata-1.3.3/kappadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-07-11 12:53:16.000000 kappadata-1.3.3/kappadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:53:16.000000 kappadata-1.3.3/kappadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 12:53:16.000000 kappadata-1.3.3/kappadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 12:53:16.000000 kappadata-1.3.3/kappadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 12:50:47.000000 kappadata-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-11 12:53:16.538794 kappadata-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.538794 kappadata-1.3.3/test_unit_long/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:50:47.000000 kappadata-1.3.3/test_unit_long/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-11 12:50:47.000000 kappadata-1.3.3/test_unit_long/test_stochastic_transform_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:53:16.538794 kappadata-1.3.3/tests_external_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:50:47.000000 kappadata-1.3.3/tests_external_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-11 12:50:47.000000 kappadata-1.3.3/tests_external_sources/dinov2.py
```

### Comparing `kappadata-1.3.2/LICENSE` & `kappadata-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/PKG-INFO` & `kappadata-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.3.2
+Version: 1.3.3
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.3.2/README.md` & `kappadata-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/__init__.py` & `kappadata-1.3.3/kappadata/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 import kappadata.caching
 import kappadata.collators
 import kappadata.common
 import kappadata.copying
 import kappadata.datasets
 import kappadata.loading
```

### Comparing `kappadata-1.3.2/kappadata/caching/cached_dataset.py` & `kappadata-1.3.3/kappadata/caching/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/caching/shared_dict_dataset.py` & `kappadata-1.3.3/kappadata/caching/shared_dict_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/collators/base/kd_collator_base.py` & `kappadata-1.3.3/kappadata/collators/base/kd_collator_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from torch.utils.data import default_collate
-
+import numpy as np
+from kappadata.utils.random import get_rng_from_global
 
 class KDCollatorBase:
     def __init__(self, dataset_mode: str, return_ctx: bool):
         self.dataset_mode = dataset_mode
         self.return_ctx = return_ctx
 
+    def set_rng(self, rng):
+        raise NotImplementedError
+
+    def worker_init_fn(self, *_, **__):
+        self.set_rng(get_rng_from_global())
+
     def __call__(self, batch):
         raise NotImplementedError
 
     @staticmethod
     def _call_impl(batch, collators, dataset_mode, return_ctx):
         called_default_collate = False
         removed_ctx_from_batch = False
```

### Comparing `kappadata-1.3.2/kappadata/collators/base/kd_compose_collator.py` & `kappadata-1.3.3/kappadata/collators/base/kd_compose_collator.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,19 @@
         assert self.return_ctx is not None, "KDComposeCollator requires return_ctx"
 
         assert isinstance(collators, list) and len(collators) > 0
         assert all(isinstance(c, KDSingleCollator) for c in collators)
         self.collators = collators
         assert all(c.default_collate_mode in [None, "before", "after"] for c in collators)
 
+    def set_rng(self, rng):
+        for collator in self.collators:
+            collator.set_rng(rng)
+        return self
+
     def __call__(self, batch):
         return self._call_impl(
             batch=batch,
             collators=self.collators,
             dataset_mode=self.dataset_mode,
             return_ctx=self.return_ctx,
         )
```

### Comparing `kappadata-1.3.2/kappadata/collators/base/kd_single_collator.py` & `kappadata-1.3.3/kappadata/collators/base/kd_single_collator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from .kd_collator_base import KDCollatorBase
+import numpy as np
+from kappadata.utils.random import get_rng_from_global
 
 
 class KDSingleCollator(KDCollatorBase):
     def __init__(self, dataset_mode: str = None, return_ctx: bool = None):
         # dataset_mode/return_ctx is only needed when KDCollator is called directly (i.e. not via KDComposeCollator)
         super().__init__(dataset_mode=dataset_mode, return_ctx=return_ctx)
+        self.rng = get_rng_from_global()
+
+    def set_rng(self, rng):
+        self.rng = rng
+        return self
 
     def __call__(self, batch):
         assert self.dataset_mode is not None and self.return_ctx is not None, \
             "use KDCollator as part of KDComposeCollator or specify dataset_mode and return_ctx"
         return self._call_impl(
             batch=batch,
             collators=[self],
```

### Comparing `kappadata-1.3.2/kappadata/collators/kd_mix_collator.py` & `kappadata-1.3.3/kappadata/collators/kd_mix_collator.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,14 @@
             mixup_alpha: float = None,
             cutmix_alpha: float = None,
             mixup_p: float = None,
             cutmix_p: float = None,
             apply_mode: str = "batch",
             lamb_mode: str = "batch",
             shuffle_mode: str = "flip",
-            seed: int = None,
             **kwargs,
     ):
         super().__init__(**kwargs)
         # check probabilities
         assert (mixup_p is not None) or (cutmix_p is not None), REQUIRES_MIXUP_P_OR_CUTMIX_P
         if mixup_p is None and cutmix_p is None:
             # no percentages specified -> equal split by default
@@ -69,16 +68,14 @@
         self.mixup_alpha = mixup_alpha
         self.cutmix_alpha = cutmix_alpha
         self.mixup_p = mixup_p
         self.cutmix_p = cutmix_p
         self.apply_mode = apply_mode
         self.lamb_mode = lamb_mode
         self.shuffle_mode = shuffle_mode
-        self.seed = seed
-        self.rng = np.random.default_rng(seed=seed)
 
     @property
     def default_collate_mode(self) -> str:
         return "before"
 
     @property
     def total_p(self) -> float:
```

### Comparing `kappadata-1.3.2/kappadata/collators/pad_sequences_collator.py` & `kappadata-1.3.3/kappadata/collators/pad_sequences_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/common/datasets/kd_image_folder.py` & `kappadata-1.3.3/kappadata/common/datasets/kd_image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/common/transforms/byol_transforms.py` & `kappadata-1.3.3/kappadata/common/transforms/byol_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/common/transforms/imagenet_minaug_transforms.py` & `kappadata-1.3.3/kappadata/common/transforms/imagenet_minaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/common/transforms/imagenet_noaug_transforms.py` & `kappadata-1.3.3/kappadata/common/transforms/imagenet_noaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/common/transforms/mae_finetune_transform.py` & `kappadata-1.3.3/kappadata/common/transforms/mae_finetune_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py` & `kappadata-1.3.3/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py` & `kappadata-1.3.3/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py` & `kappadata-1.3.3/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/copying/folder.py` & `kappadata-1.3.3/kappadata/copying/folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/copying/image_folder.py` & `kappadata-1.3.3/kappadata/copying/image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/datasets/kd_concat_dataset.py` & `kappadata-1.3.3/kappadata/datasets/kd_concat_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,18 @@
         self.dispose()
 
     def dispose(self):
         for dataset in self.datasets:
             dataset.dispose()
 
     @property
+    def collators(self):
+        return []
+
+    @property
     def root_dataset(self):
         if len(self.datasets) == 1:
             return self.datasets[0].root_dataset
         # warning/exception here might make sense
         return self.datasets[0].root_dataset
 
     @property
```

### Comparing `kappadata-1.3.2/kappadata/datasets/kd_dataset.py` & `kappadata-1.3.3/kappadata/datasets/kd_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import logging
 from functools import partial
 
 from torch.utils.data import Dataset
 
 from kappadata.error_messages import getshape_instead_of_getdim
 from kappadata.errors import UseModeWrapperException
+from kappadata.utils.random import get_rng_from_global
 
 
 class KDDataset(Dataset):
-    def __init__(self):
+    def __init__(self, collators=None):
         super().__init__()
         self.logger = logging.getLogger(type(self).__name__)
+        self._collators = collators
 
         # getdim_... is an alias -> should be defined via getshape_...
         getdim_names = [name for name in dir(self) if name.startswith("getdim_")]
         assert len(getdim_names) == 0, getshape_instead_of_getdim(getdim_names)
 
     def __getattr__(self, item):
         # make getdim_... an alias to getshape_...[0]
@@ -32,14 +34,18 @@
         self.dispose()
 
     def dispose(self):
         """ release resources occupied by dataset (e.g. filehandles) """
         pass
 
     @property
+    def collators(self):
+        return self._collators or []
+
+    @property
     def root_dataset(self):
         return self
 
     @property
     def fused_operations(self):
         return []
 
@@ -70,15 +76,18 @@
         assert len(wrappers) == 1
         return wrappers[0]
 
     def get_wrappers_of_type(self, wrapper_type):
         return []
 
     def worker_init_fn(self, rank, **kwargs):
-        pass
+        if self.collators is not None:
+            rng = get_rng_from_global()
+            for collator in self.collators:
+                collator.set_rng(rng)
 
     def __getitem__(self, idx):
         raise UseModeWrapperException
 
     def getshape(self, kind):
         attr = f"getshape_{kind}"
         assert hasattr(self, attr)
```

### Comparing `kappadata-1.3.2/kappadata/datasets/kd_subset.py` & `kappadata-1.3.3/kappadata/datasets/kd_subset.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     def __enter__(self):
         return self
 
     def __exit__(self, *_):
         self.dispose()
 
     @property
+    def collators(self):
+        return self.dataset.collators
+
+    @property
     def root_dataset(self):
         return self.dataset.root_dataset
 
     @property
     def fused_operations(self):
         return self.dataset.fused_operations
```

### Comparing `kappadata-1.3.2/kappadata/datasets/kd_wrapper.py` & `kappadata-1.3.3/kappadata/datasets/kd_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,19 @@
     def __getitem__(self, idx):
         raise UseModeWrapperException
 
     def dispose(self):
         self.dataset.dispose()
 
     @property
+    def collators(self):
+        assert self._collators is None, "register collators on root datset"
+        return self.dataset.collators
+
+    @property
     def root_dataset(self):
         # KDDataset implements root_dataset -> __getitem__ doesn't trigger
         return self.dataset.root_dataset
 
     @property
     def fused_operations(self):
         return self.dataset.fused_operations
```

### Comparing `kappadata-1.3.2/kappadata/factory.py` & `kappadata-1.3.3/kappadata/factory.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/samplers/distributed_sampler.py` & `kappadata-1.3.3/kappadata/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/samplers/infinite_batch_sampler.py` & `kappadata-1.3.3/kappadata/samplers/infinite_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/samplers/interleaved_sampler.py` & `kappadata-1.3.3/kappadata/samplers/interleaved_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/samplers/random_sampler.py` & `kappadata-1.3.3/kappadata/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/samplers/semi_sampler.py` & `kappadata-1.3.3/kappadata/samplers/semi_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/__init__.py` & `kappadata-1.3.3/kappadata/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/base/kd_compose_transform.py` & `kappadata-1.3.3/kappadata/transforms/base/kd_compose_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def _apply(t, x, ctx):
         if isinstance(t, KDTransform):
             return t(x, ctx)
         return t(x)
 
     def set_rng(self, rng):
         for t in self.transforms:
-            if isinstance(t, KDStochasticTransform):
+            if isinstance(t, KDTransform):
                 t.set_rng(rng)
         return self
 
     def _scale_strength(self, factor):
         for t in self.transforms:
             if isinstance(t, KDTransform):
                 t.scale_strength(factor)
```

### Comparing `kappadata-1.3.2/kappadata/transforms/base/kd_random_apply_base.py` & `kappadata-1.3.3/kappadata/transforms/base/kd_random_apply_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/base/kd_scheduled_transform.py` & `kappadata-1.3.3/kappadata/transforms/base/kd_scheduled_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/image_pos_embed_grid.py` & `kappadata-1.3.3/kappadata/transforms/image_pos_embed_grid.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/image_pos_embed_sincos.py` & `kappadata-1.3.3/kappadata/transforms/image_pos_embed_sincos.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_additive_gaussian_noise.py` & `kappadata-1.3.3/kappadata/transforms/kd_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_bucketize.py` & `kappadata-1.3.3/kappadata/transforms/kd_bucketize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_color_jitter.py` & `kappadata-1.3.3/kappadata/transforms/kd_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_columnwise_norm.py` & `kappadata-1.3.3/kappadata/transforms/kd_columnwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_gaussian_blur_pil.py` & `kappadata-1.3.3/kappadata/transforms/kd_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_gaussian_blur_tv.py` & `kappadata-1.3.3/kappadata/transforms/kd_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_minsize.py` & `kappadata-1.3.3/kappadata/transforms/kd_minsize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_rand_augment.py` & `kappadata-1.3.3/kappadata/transforms/kd_rand_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_additive_gaussian_noise.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_apply.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_apply.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_color_jitter.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_crop.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_erasing.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_erasing.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_gaussian_blur_pil.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_gaussian_blur_tv.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_grayscale.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_grayscale.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_resized_crop.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_rotation.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_solarize.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_random_threshold.py` & `kappadata-1.3.3/kappadata/transforms/kd_random_threshold.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_resize.py` & `kappadata-1.3.3/kappadata/transforms/kd_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_simple_random_crop.py` & `kappadata-1.3.3/kappadata/transforms/kd_simple_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_solarize.py` & `kappadata-1.3.3/kappadata/transforms/kd_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_three_augment.py` & `kappadata-1.3.3/kappadata/transforms/kd_three_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_threshold.py` & `kappadata-1.3.3/kappadata/transforms/kd_threshold.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/kd_two_random_crop.py` & `kappadata-1.3.3/kappadata/transforms/kd_two_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/norm/kd_image_norm.py` & `kappadata-1.3.3/kappadata/transforms/norm/kd_image_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/norm/kd_image_range_norm.py` & `kappadata-1.3.3/kappadata/transforms/norm/kd_image_range_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/norm/kd_norm_base.py` & `kappadata-1.3.3/kappadata/transforms/norm/kd_norm_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/patchify_image.py` & `kappadata-1.3.3/kappadata/transforms/patchify_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/patchwise_norm.py` & `kappadata-1.3.3/kappadata/transforms/patchwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/patchwise_random_rotation.py` & `kappadata-1.3.3/kappadata/transforms/patchwise_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/semseg/kd_semseg_pad.py` & `kappadata-1.3.3/kappadata/transforms/semseg/kd_semseg_pad.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/semseg/kd_semseg_random_crop.py` & `kappadata-1.3.3/kappadata/transforms/semseg/kd_semseg_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/semseg/kd_semseg_random_resize.py` & `kappadata-1.3.3/kappadata/transforms/semseg/kd_semseg_random_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/transforms/semseg/kd_semseg_resize.py` & `kappadata-1.3.3/kappadata/transforms/semseg/kd_semseg_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/utils/bounding_box_utils.py` & `kappadata-1.3.3/kappadata/utils/bounding_box_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/utils/class_counts.py` & `kappadata-1.3.3/kappadata/utils/class_counts.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/utils/color_histogram.py` & `kappadata-1.3.3/kappadata/utils/color_histogram.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/utils/hash_utils.py` & `kappadata-1.3.3/kappadata/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/utils/magnitude_sampler.py` & `kappadata-1.3.3/kappadata/utils/magnitude_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/utils/multi_crop_utils.py` & `kappadata-1.3.3/kappadata/utils/multi_crop_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/utils/pos_embed.py` & `kappadata-1.3.3/kappadata/utils/pos_embed.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/utils/save_image.py` & `kappadata-1.3.3/kappadata/utils/save_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/utils/transform_utils.py` & `kappadata-1.3.3/kappadata/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/visualization/visualize_dataset_imgsize.py` & `kappadata-1.3.3/kappadata/visualization/visualize_dataset_imgsize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/visualization/visualize_interpolation.py` & `kappadata-1.3.3/kappadata/visualization/visualize_interpolation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/visualization/visualize_jigsaw.py` & `kappadata-1.3.3/kappadata/visualization/visualize_jigsaw.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/visualization/visualize_mae_schematic.py` & `kappadata-1.3.3/kappadata/visualization/visualize_mae_schematic.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/visualization/visualize_masked_image.py` & `kappadata-1.3.3/kappadata/visualization/visualize_masked_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/visualization/visualize_transform.py` & `kappadata-1.3.3/kappadata/visualization/visualize_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/visualization/visualize_two_random_crop.py` & `kappadata-1.3.3/kappadata/visualization/visualize_two_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/dataset_wrappers/subset_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/dataset_wrappers/subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/mode_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/mode_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,19 @@
             return items, ctx
         return items
 
     def __len__(self):
         return len(self.dataset)
 
     @property
+    def collators(self):
+        assert self._collators is None, "register collators on root datset"
+        return self.dataset.collators
+
+    @property
     def root_dataset(self):
         # root_dataset is implemented in base class -> not handled in __getattr__
         return self.dataset.root_dataset
 
     @property
     def fused_operations(self):
         raise RuntimeError("fused_operations should not be called from ModeWrapper")
```

### Comparing `kappadata-1.3.2/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py` & `kappadata-1.3.3/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata/wrappers/torch_wrapper.py` & `kappadata-1.3.3/kappadata/wrappers/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.2/kappadata.egg-info/PKG-INFO` & `kappadata-1.3.3/kappadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.3.2
+Version: 1.3.3
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.3.2/kappadata.egg-info/SOURCES.txt` & `kappadata-1.3.3/kappadata.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 kappadata.egg-info/dependency_links.txt
 kappadata.egg-info/requires.txt
 kappadata.egg-info/top_level.txt
 kappadata/caching/__init__.py
 kappadata/caching/cached_dataset.py
 kappadata/caching/shared_dict_dataset.py
 kappadata/collators/__init__.py
+kappadata/collators/kd_dino_mask_collator.py
 kappadata/collators/kd_mix_collator.py
 kappadata/collators/pad_sequences_collator.py
 kappadata/collators/base/__init__.py
 kappadata/collators/base/kd_collator_base.py
 kappadata/collators/base/kd_compose_collator.py
 kappadata/collators/base/kd_single_collator.py
 kappadata/common/__init__.py
@@ -126,14 +127,15 @@
 kappadata/utils/image_utils.py
 kappadata/utils/logging.py
 kappadata/utils/magnitude_sampler.py
 kappadata/utils/multi_crop_utils.py
 kappadata/utils/one_hot.py
 kappadata/utils/param_checking.py
 kappadata/utils/pos_embed.py
+kappadata/utils/random.py
 kappadata/utils/save_image.py
 kappadata/utils/transform_utils.py
 kappadata/visualization/__init__.py
 kappadata/visualization/visualize_dataset_imgsize.py
 kappadata/visualization/visualize_interpolation.py
 kappadata/visualization/visualize_jigsaw.py
 kappadata/visualization/visualize_mae_schematic.py
@@ -161,8 +163,10 @@
 kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
 kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/base/__init__.py
 kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
 test_unit_long/__init__.py
-test_unit_long/test_stochastic_transform_seed.py
+test_unit_long/test_stochastic_transform_seed.py
+tests_external_sources/__init__.py
+tests_external_sources/dinov2.py
```

### Comparing `kappadata-1.3.2/setup.cfg` & `kappadata-1.3.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.3.2
+version = 1.3.3
 name = kappadata
 description = pytorch dataset wrappers for in-memory caching
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaData
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaData
```

### Comparing `kappadata-1.3.2/test_unit_long/test_stochastic_transform_seed.py` & `kappadata-1.3.3/test_unit_long/test_stochastic_transform_seed.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import numpy as np
 import unittest
-from kappadata.transforms import KDStochasticTransform
 from tests_util.datasets.x_dataset import XDataset
+from tests_util.collators import AddRandomSequenceCollator
+from tests_util.transforms import ReplaceWithRandomTransform, AddRandomTransform
 from torch.utils.data import DataLoader
 from kappadata.wrappers import ModeWrapper, XTransformWrapper
+from kappadata.collators import KDComposeCollator
 import torch
 
 class TestStochasticTransformSeed(unittest.TestCase):
-    class _TestTransform(KDStochasticTransform):
-        def __call__(self, x, ctx=None):
-            return self.rng.random()
-
     def test_single_worker_noseed(self):
-        dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=self._TestTransform())
+        dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=ReplaceWithRandomTransform())
         dataset = ModeWrapper(dataset, mode="x")
         values = torch.concat([x for x in DataLoader(dataset, batch_size=2)])
         self.assertEqual(values.unique().numel(), values.numel())
 
     def test_single_worker_globalseed(self):
         for _ in range(2):
             np.random.seed(0)
-            dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=self._TestTransform())
+            dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=ReplaceWithRandomTransform())
             dataset = ModeWrapper(dataset, mode="x")
             values = torch.concat([x for x in DataLoader(dataset, batch_size=2)])
             expected = [
                 0.38255389159742137,
                 0.34776831374136297,
                 0.7534087540864453,
                 0.5815352814832978,
@@ -34,43 +32,87 @@
                 0.6524144695739501,
                 0.4358178202087156,
                 0.3025380253474623,
             ]
             self.assertEqual(expected, values.tolist())
 
     def test_two_worker_noseed(self):
-        dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=self._TestTransform())
+        dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=ReplaceWithRandomTransform())
         dataset = ModeWrapper(dataset, mode="x")
         dataloader = DataLoader(dataset, batch_size=2, num_workers=2, worker_init_fn=dataset.worker_init_fn)
         values = torch.concat([x for x in dataloader])
         self.assertEqual(values.unique().numel(), values.numel())
 
 
     def test_two_worker_globalseed(self):
         for _ in range(2):
             torch.manual_seed(0)
-            dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=self._TestTransform())
+            dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=ReplaceWithRandomTransform())
             dataset = ModeWrapper(dataset, mode="x")
             dataloader = DataLoader(dataset, batch_size=2, num_workers=2, worker_init_fn=dataset.worker_init_fn)
             values = torch.concat([x for x in dataloader])
             expected = [
-                0.7769574528852247,
-                0.6413399201175735,
-                0.6528946343441658,
-                0.2668958984056612,
-                0.3520944933037099,
-                0.46693979902613325,
-                0.9319926092440057,
-                0.8229667001843889,
-                0.31564052947560894,
-                0.20301340820491776,
+                0.05265565657170268,
+                0.5856545413116812,
+                0.5245641455144165,
+                0.9032732387757539,
+                0.7345538141574777,
+                0.9076975596537473,
+                0.2264209460224459,
+                0.9893990449288441,
+                0.7417763462601573,
+                0.7998301927398731,
             ]
             self.assertEqual(expected, values.tolist())
 
     def test_is_num_worker_independent_with_seed(self):
-        dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=self._TestTransform(), seed=0)
+        dataset = XTransformWrapper(dataset=XDataset(torch.arange(10)), transform=ReplaceWithRandomTransform(), seed=0)
         dataset = ModeWrapper(dataset, mode="x")
         dataloader0 = DataLoader(dataset, batch_size=2)
         dataloader1 = DataLoader(dataset, batch_size=2, num_workers=2, worker_init_fn=dataset.worker_init_fn)
         values0 = torch.concat([x for x in dataloader0])
         values1 = torch.concat([x for x in dataloader1])
         self.assertEqual(values0.tolist(), values1.tolist())
+
+    def test_nested_xtransformwrapper(self):
+        dataset = XDataset(torch.arange(10))
+        dataset = XTransformWrapper(dataset=dataset, transform=ReplaceWithRandomTransform())
+        dataset = XTransformWrapper(dataset=dataset, transform=AddRandomTransform())
+        dataset = ModeWrapper(dataset, mode="x")
+        values = torch.concat([
+            torch.concat(x)
+            for x in DataLoader(dataset, batch_size=2, worker_init_fn=dataset.worker_init_fn)
+        ])
+        self.assertEqual(values.unique().numel(), values.numel())
+
+    def test_xtransformwrapper_collated(self):
+        dataset = XDataset(torch.arange(10), collators=[AddRandomSequenceCollator(dataset_mode="x", return_ctx=False)])
+        dataset = XTransformWrapper(dataset=dataset, transform=ReplaceWithRandomTransform())
+        dataset = ModeWrapper(dataset, mode="x")
+        values = torch.concat([
+            x
+            for x in DataLoader(
+                dataset=dataset,
+                batch_size=2,
+                worker_init_fn=dataset.worker_init_fn,
+                collate_fn=dataset.collators[0],
+            )
+        ])
+        self.assertEqual(values.unique().numel(), values.numel())
+
+    def test_xtransformwrapper_composecollated(self):
+        for num_collators in [1, 2]:
+            collators = [AddRandomSequenceCollator() for _ in range(num_collators)]
+            dataset = XDataset(torch.arange(10), collators=collators)
+            dataset = XTransformWrapper(dataset=dataset, transform=ReplaceWithRandomTransform())
+            dataset = ModeWrapper(dataset, mode="x")
+            values = torch.concat([
+                x
+                for x in DataLoader(
+                    dataset=dataset,
+                    batch_size=2,
+                    worker_init_fn=dataset.worker_init_fn,
+                    collate_fn=KDComposeCollator(dataset.collators, dataset_mode="x", return_ctx=False),
+                )
+            ])
+            self.assertEqual(values.unique().numel(), values.numel())
+
```

