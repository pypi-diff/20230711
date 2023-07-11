# Comparing `tmp/bmtrain-0.2.2.tar.gz` & `tmp/bmtrain-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bmtrain-0.2.2.tar", last modified: Fri May  5 02:09:17 2023, max compression
+gzip compressed data, was "./sdist/bmtrain-0.2.3.tar", last modified: Tue Jul 11 07:02:19 2023, max compression
```

## Comparing `bmtrain-0.2.2.tar` & `bmtrain-0.2.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 02:08:46.000000 bmtrain-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 02:09:17.000000 bmtrain-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-05 02:08:46.000000 bmtrain-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/all_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/send_recv.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/block_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/distributed/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/global_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/inspect/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/inspect/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/inspect/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/inspect/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/loss/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/loss/cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/no_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/noam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/nccl/
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/nccl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/nccl/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/optim/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/optim/adam_offload.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/optim/optim_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/param_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27322 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/pipe_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/synchronize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/adam_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/adam_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cross_entropy_loss.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/csrc/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cuda/adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cuda/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cuda/has_inf_nan.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cuda/reduce.cuh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/csrc/include/
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/include/nccl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/include/nccl_net.h
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/nccl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:09:17.000000 bmtrain-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-05 02:08:46.000000 bmtrain-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-11 06:56:12.000000 bmtrain-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-11 07:02:19.000000 bmtrain-0.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13480 2023-07-11 06:56:12.000000 bmtrain-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/benchmark/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/all_gather.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/reduce_scatter.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/send_recv.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/shape.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/utils.py
+-rw-r--r--   0 root         (0) root         (0)    42476 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/block_layer.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/checkpointing.py
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/distributed/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/distributed/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5283 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/distributed/ops.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/global_var.py
+-rw-r--r--   0 root         (0) root         (0)     6821 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/inspect/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/inspect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/inspect/format.py
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/inspect/model.py
+-rw-r--r--   0 root         (0) root         (0)    13766 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/inspect/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     6825 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/loss/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4659 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/loss/_function.py
+-rw-r--r--   0 root         (0) root         (0)     9644 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/loss/cross_entropy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/cosine.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/exponential.py
+-rw-r--r--   0 root         (0) root         (0)      605 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/linear.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/no_decay.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/noam.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/nccl/
+-rw-r--r--   0 root         (0) root         (0)    10248 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/nccl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      437 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/nccl/enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/optim/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/_function.py
+-rw-r--r--   0 root         (0) root         (0)     8169 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/adam.py
+-rw-r--r--   0 root         (0) root         (0)    11534 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/adam_offload.py
+-rw-r--r--   0 root         (0) root         (0)     8175 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/optim_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/param_init.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/parameter.py
+-rw-r--r--   0 root         (0) root         (0)    27322 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/pipe_layer.py
+-rw-r--r--   0 root         (0) root         (0)     7916 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/store.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/synchronize.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/csrc/
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/bind.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/csrc/cuda/
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/cuda/adam_cuda.cu
+-rw-r--r--   0 root         (0) root         (0)     7067 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/cuda/cross_entropy.cu
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/cuda/has_inf_nan.cu
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/cuda/reduce.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/csrc/include/
+-rw-r--r--   0 root         (0) root         (0)    10281 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/include/adam_cpu.hpp
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/include/bind.hpp
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/include/nccl.hpp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 07:02:19.000000 bmtrain-0.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3973 2023-07-11 06:56:12.000000 bmtrain-0.2.3/setup.py
```

### Comparing `bmtrain-0.2.2/README.md` & `bmtrain-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/__init__.py` & `bmtrain-0.2.3/bmtrain/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/benchmark/all_gather.py` & `bmtrain-0.2.3/bmtrain/benchmark/all_gather.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/benchmark/reduce_scatter.py` & `bmtrain-0.2.3/bmtrain/benchmark/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/benchmark/send_recv.py` & `bmtrain-0.2.3/bmtrain/benchmark/send_recv.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/block_layer.py` & `bmtrain-0.2.3/bmtrain/block_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import torch
 from . import nccl
 from .synchronize import wait_loader
 from .parameter import DistributedParameter, OpAllGather
 from .checkpointing import ScopedTensorInspectorContext
 from . import debug
 import copy
+import inspect
 
 
 # the flag is used to control the zero level , 0 means normal zero3 , 1 means forward without release parameter ,2 means backward without gather parameter
 class OpCheckpointBlock(torch.autograd.Function):
     @staticmethod
     def forward(ctx, placeholder, block : 'CheckpointBlock', preserve_rng_state, len_args, *args):
         ctx.block = block
@@ -613,18 +614,22 @@
                 # PyTorch 1.11 changed the API of storage.__getitem__
                 d_dtype = self._storage_params[kw_name].dtype
                 d_device = self._storage_params[kw_name].device
                 param.data[:] = \
                     torch.tensor([], dtype=d_dtype, device=d_device).set_(tmp_tensor.storage(), offset_st, (offset_end - offset_st,))[:]
                 del tmp_tensor
         
-    def _named_members(self, get_members_fn, prefix='', recurse=True):
+    def _named_members(self, get_members_fn, prefix='', recurse=True, **kwargs):
         r"""Helper method for yielding various names + members of modules."""
-        return self._module._named_members(get_members_fn, prefix, recurse)
         
+        #compitibity with torch 2.0
+        if "remove_duplicate" in inspect.signature(torch.nn.Module._named_members).parameters and "remove_duplicate" not in kwargs:
+            kwargs['remove_duplicate'] = True
+        return self._module._named_members(get_members_fn, prefix, recurse, **kwargs)
+    
     def named_modules(self, memo = None, prefix: str = '', remove_duplicate: bool = True):
         r"""Returns an iterator over all modules in the network, yielding
         both the name of the module as well as the module itself.
 
         Args:
             memo: a memo to store the set of modules already added to the result
             prefix: a prefix that will be added to the name of the module
```

### Comparing `bmtrain-0.2.2/bmtrain/checkpointing.py` & `bmtrain-0.2.3/bmtrain/checkpointing.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/debug.py` & `bmtrain-0.2.3/bmtrain/debug.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/distributed/ops.py` & `bmtrain-0.2.3/bmtrain/distributed/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,30 +16,37 @@
     torch.int8,
     torch.bfloat16,
     torch.bool
 ]
 def send_activations(hidden_state, next_rank, comm):
     send_meta(hidden_state, next_rank, comm)
     ncclSend(hidden_state.storage(), next_rank, comm)
+
 def recv_activations(prev_rank, comm):
     dtype, shape = recv_meta(prev_rank, comm)
     hidden_state = torch.empty(shape, dtype=dtype, device="cuda")
     ncclRecv(hidden_state.storage(), prev_rank, comm)
     return hidden_state
+
 def send_meta(x, next_rank, comm):
-    meta = [len(x.size()), DTYPE_LIST.index(x.dtype)] + list(x.size())
-    meta_data = torch.tensor(data=meta, device=x.device, dtype=torch.long)
+    meta_data = torch.tensor(data=[0]*50, device="cuda", dtype=torch.int)
+    meta_data[0] = len(x.size())
+    meta_data[1] = DTYPE_LIST.index(x.dtype)
+    meta_data[2:len(x.size())+2] = torch.tensor(x.size(), device="cuda", dtype=torch.int)
+    meta_data = meta_data.contiguous()
     ncclSend(meta_data.storage(), next_rank, comm)
+
 def recv_meta(prev_rank, comm):
-    meta_data = torch.tensor(data=[0]*50, device="cuda", dtype=torch.long)
+    meta_data = torch.tensor(data=[0]*50, device="cuda", dtype=torch.int)
     ncclRecv(meta_data.storage(), prev_rank, comm)
     n_dims = meta_data[0].item()
     dtype = DTYPE_LIST[meta_data[1].item()]
     shape = meta_data[2:n_dims+2].tolist()
     return dtype,shape
+
 class OpBroadcast(torch.autograd.Function):
     @staticmethod
     def forward(ctx, src, root, comm = None):
         if comm is None:
             comm = config["comm"]
         ctx.comm = comm
         outputs = torch.empty_like(src, dtype = src.dtype, device = src.device)
```

### Comparing `bmtrain-0.2.2/bmtrain/global_var.py` & `bmtrain-0.2.3/bmtrain/global_var.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/init.py` & `bmtrain-0.2.3/bmtrain/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,19 +145,21 @@
         self.pipe_idx = (self.pp_group == self.rank).nonzero()[0, 0].item() # x axes
         self.zero_id = self.pipe_idx
         self.zero_idx = self.stage_id
         self.next_rank = self.stage_id+1 if self.stage_id < config['pipe_size'] - 1 else -1
         self.prev_rank = self.stage_id-1 if self.stage_id > 0 else -1
         self.tails = self.pp_group[self.pipe_idx, self.stage_id:].tolist()
         self.heads = self.pp_group[self.pipe_idx, :self.stage_id + 1].tolist()
+
     def get_group_id(self,group_name):
         if group_name == "pipe":
             return self.pipe_idx
         elif group_name == "zero":
             return self.zero_idx
+        
     def get_group_rank(self,group_name):
         if group_name == "pipe":
             return self.stage_id
         elif group_name == "zero":
             return self.zero_id
 
 def is_initialized() -> bool:
```

### Comparing `bmtrain-0.2.2/bmtrain/inspect/format.py` & `bmtrain-0.2.3/bmtrain/inspect/format.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/inspect/model.py` & `bmtrain-0.2.3/bmtrain/inspect/model.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/inspect/tensor.py` & `bmtrain-0.2.3/bmtrain/inspect/tensor.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/layer.py` & `bmtrain-0.2.3/bmtrain/layer.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/loss/cross_entropy.py` & `bmtrain-0.2.3/bmtrain/loss/cross_entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from typing import Optional
 import torch
-from . import _cuda as C
-
+from . import _function as F
 class OpFusedCrossEntropy(torch.autograd.Function):
     """
     CrossEntropy dim = 1
     """
     @staticmethod
     def forward(ctx, x : torch.Tensor, target : torch.Tensor, ignore_index: int):
         assert x.ndim == 2
         softmax = torch.empty(x.size(), device=x.device, dtype=x.dtype)
         out = torch.empty(x.size(0), device=x.device, dtype=torch.float)
-        C.f_cross_entropy_forward(
+        F.cross_entropy_forward(
             x.size(0), x.size(1),
             x, target,
             softmax, out,
             ignore_index,
         )
         ctx.ignore_index = ignore_index
         ctx.save_for_backward(softmax, target)
         return out # float tensor
         
     @staticmethod
     def backward(ctx, grad_output : torch.Tensor):
         grad_output = grad_output.contiguous()
         softmax, target = ctx.saved_tensors
-        C.f_cross_entropy_backward_inplace(
+        F.cross_entropy_backward_inplace(
             softmax.size(0), softmax.size(1),
             grad_output, target,
             softmax,
             ctx.ignore_index,
         )
         return (softmax, None, None)
 
@@ -37,29 +36,29 @@
     """
     CrossEntropy dim = 1
     """
     @staticmethod
     def forward(ctx, x : torch.Tensor, target : torch.Tensor, ignore_index: int):
         assert x.ndim == 2
         out = torch.empty(x.size(0), device=x.device, dtype=torch.float)
-        C.f_cross_entropy_forward_inplace(
+        F.cross_entropy_forward_inplace(
             x.size(0), x.size(1),
             x, target,
             out,
             ignore_index,
         ) # x is inplace modify to softmax result
         ctx.ignore_index = ignore_index
         ctx.save_for_backward(x, target)
         return out # float tensor
         
     @staticmethod
     def backward(ctx, grad_output : torch.Tensor):
         grad_output = grad_output.contiguous()
         softmax, target = ctx.saved_tensors
-        C.f_cross_entropy_backward_inplace(
+        F.cross_entropy_backward_inplace(
             softmax.size(0), softmax.size(1),
             grad_output, target,
             softmax,
             ctx.ignore_index,
         ) # softmax is inplace modify to grad_input
         return (softmax, None, None)
```

### Comparing `bmtrain-0.2.2/bmtrain/lr_scheduler/cosine.py` & `bmtrain-0.2.3/bmtrain/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/lr_scheduler/exponential.py` & `bmtrain-0.2.3/bmtrain/lr_scheduler/exponential.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/lr_scheduler/linear.py` & `bmtrain-0.2.3/bmtrain/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/lr_scheduler/noam.py` & `bmtrain-0.2.3/bmtrain/lr_scheduler/noam.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/lr_scheduler/warmup.py` & `bmtrain-0.2.3/bmtrain/lr_scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/nccl/__init__.py` & `bmtrain-0.2.3/bmtrain/nccl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from typing_extensions import Literal
 import torch
-from . import _C as C
+from .. import C
 from .enums import *
 
 class NCCLCommunicator:
     """
     NCCL communicator stores the communicator handle.
     """
```

### Comparing `bmtrain-0.2.2/bmtrain/optim/adam.py` & `bmtrain-0.2.3/bmtrain/optim/adam.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import torch
 from ..global_var import config
-import torch.optim._functional as F
-from . import _cuda as C
+from . import _function as F
+import torch.optim._functional
+from .. import  C
 from .. import nccl
 import inspect
-
+from ..utils import check_torch_version
 from copy import deepcopy
 from itertools import chain
 from collections import defaultdict
 
 class AdamOptimizer(torch.optim.Optimizer):
     """
     Adam optimizer
@@ -83,38 +84,38 @@
 
                     if ('maximize' in group) and (group['maximize'] is True):
                         grad = -p.grad
                     else:
                         grad = p.grad
                         
                     if p.dtype == torch.half:
-                        C.f_adam(
+                        F.adam(
                             state["_param_fp32"],    # fp32
                             p,                      # fp16
                             grad,                 # fp16
                             state['exp_avg'],       # fp16: m
                             state["exp_avg_sq"],    # fp32: v
                             group['betas'][0], group['betas'][1],
                             group['eps'],
                             0.0 if state["step"] <= self._hold_steps else group['lr'],
                             scale,
                             group['weight_decay'],
                             state['step']
                         )
                     else:
                         other_kwargs = {}
-                        if 'maximize' in inspect.signature(F.adam).parameters:
+                        if 'maximize' in inspect.signature(torch.optim._functional.adam).parameters:
                             other_kwargs['maximize'] = False
-                        F.adam(
+                        torch.optim._functional.adam(
                             [p],
                             [grad / scale],
                             [state['exp_avg']],
                             [state["exp_avg_sq"]],
                             [],
-                            [state["step"]] if int(torch.__version__.split('.')[1]) < 12
+                            [state["step"]] if check_torch_version("1.12.0") < 0 
                                 else [torch.tensor(state["step"])],
                             amsgrad=False,
                             beta1=group['betas'][0],
                             beta2=group['betas'][1],
                             lr=0.0 if state["step"] <= self._hold_steps else group['lr'],
                             weight_decay=group['weight_decay'],
                             eps=group['eps'],
@@ -172,8 +173,12 @@
 
         # Update parameter groups, setting their 'params' value
         def update_group(group, new_group):
             new_group['params'] = group['params']
             return new_group
         param_groups = [
             update_group(g, ng) for g, ng in zip(groups, saved_groups)]
-        self.__setstate__({'state': state, 'param_groups': param_groups})
+        self.__setstate__({'state': state, 'param_groups': param_groups})
+
+    #TODO zero_grad(set_to_none=True) makes optimizer crashed, maybe the reason of grad accu
+    def zero_grad(self, set_to_none: bool = False):
+        super().zero_grad(set_to_none=set_to_none)
```

### Comparing `bmtrain-0.2.2/bmtrain/optim/adam_offload.py` & `bmtrain-0.2.3/bmtrain/optim/adam_offload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import torch
 from ..global_var import config
-from . import _cpu as C
-from . import _cuda as G
+from . import _function as F
 from .. import nccl
-import torch.optim._functional as F
 import inspect
-
+from ..utils import check_torch_version
 from copy import deepcopy
 from itertools import chain
 from collections import defaultdict
 
 class AdamOffloadOptimizer(torch.optim.Optimizer):
     """
     Adam optimizer
@@ -103,15 +101,15 @@
 
             # update parameters
             if param.dtype == torch.half:
                 if ('maximize' in group) and (group['maximize'] is True):
                     grad = -state["_grad_fp16"]
                 else:
                     grad = state["_grad_fp16"]
-                C.f_adam_cpu(
+                F.adam_cpu(
                     state["_param_fp32"].view(-1),
                     state["_param_fp16"].view(-1),
                     grad.view(-1),
                     state["exp_avg"].view(-1),
                     state["exp_avg_sq"].view(-1),
                     beta1, beta2,
                     eps,  0.0 if state["step"] <= self._hold_steps else lr,
@@ -124,23 +122,23 @@
             else:
                 state["_grad_fp32"].mul_(1.0 / scale)
                 if ('maximize' in group) and (group['maximize'] is True):
                     grad = -state["_grad_fp32"]
                 else:
                     grad = state["_grad_fp32"]
                 other_kwargs = {}
-                if 'maximize' in inspect.signature(F.adam).parameters:
+                if 'maximize' in inspect.signature(torch.optim._functional.adam).parameters:
                     other_kwargs['maximize'] = False
-                F.adam(
+                torch.optim._functional.adam(
                     [state["_param_fp32"]],
                     [grad],
                     [state["exp_avg"]],
                     [state["exp_avg_sq"]],
                     [],
-                    [state["step"]] if int(torch.__version__.split('.')[1]) < 12
+                    [state["step"]] if check_torch_version("1.12.0") < 0
                         else [torch.tensor(state["step"])],
                     amsgrad=False,
                     beta1=beta1,
                     beta2=beta2,
                     lr=0.0 if state["step"] <= self._hold_steps else lr,
                     weight_decay=weight_decay,
                     eps=eps,
@@ -248,8 +246,13 @@
         param_groups = [pack_group(g) for g in self.param_groups]
         # Remap state to use order indices as keys
         packed_state = {(param_mappings[id(k)] if isinstance(k, torch.Tensor) else k): cut_states(v)
                         for k, v in self.state.items()}
         return {
             'state': packed_state,
             'param_groups': param_groups,
-        }
+        }
+            
+    #TODO zero_grad(set_to_none=True) makes optimizer crashed, maybe the reason of grad accu
+    def zero_grad(self, set_to_none: bool = False):
+        super().zero_grad(set_to_none=set_to_none)
+
```

### Comparing `bmtrain-0.2.2/bmtrain/optim/optim_manager.py` & `bmtrain-0.2.3/bmtrain/optim/optim_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import Optional, Union, List, Dict, Tuple
 import torch
-
-from . import _cuda as G
+from ..loss._function import has_inf_nan
 from ..utils import print_rank
 from ..lr_scheduler.warmup import WarmupLRScheduler
 from .. import nccl
 from ..global_var import config
 
 def check_overflow(param_groups):
     # check overflow
     has_inf_or_nan = torch.zeros(1, dtype=torch.uint8, device="cuda")[0]
     for group in param_groups:
         for p in group['params']:
             if p.grad is not None and p.dtype == torch.half: # TODO support other types
-                G.f_has_inf_nan(p.grad, has_inf_or_nan)
+                has_inf_nan(p.grad, has_inf_or_nan)
 
     if "comm" in config:
         nccl.allReduce(has_inf_or_nan.storage(), has_inf_or_nan.storage(), "max", config["comm"])
 
     if has_inf_or_nan > 0:
         raise OverflowError("Gradient overflow")
 
@@ -77,14 +76,15 @@
             optim (torch.optim.Optimizer): A pytorch optimizer, e.g. torch.optim.Adam, torch.optim.SGD or bmtrain.optim.AdamOffloadOptimizer
             lr_scheduler (Optional[WarmupLRScheduler]): A warmup lr scheduler, e.g. bmt.lr_scheduler.Noam
         """
         self.optimizers.append(optimizer)
         self.lr_schedulers.append(lr_scheduler)
 
     def scale_loss(self, loss : torch.Tensor) -> torch.Tensor:
+
         return loss * (self.loss_scale / config['world_size']) # loss scale
 
     def backward(self, loss : torch.Tensor):
         """
         Backward with loss scale.
 
         Args:
@@ -97,15 +97,15 @@
         current_stream.wait_stream(config['load_stream'])
 
     def zero_grad(self):
         """
         This is a helper function to call optimizer.zero_grad()
         """
         for optimizer in self.optimizers:
-            optimizer.zero_grad()
+            optimizer.zero_grad(set_to_none=False)
 
     def step(self):
         """
         Backward with loss scale.
         Synchronize streams before optimizer steps.
 
         This is a helper function to call optimizer.step() and lr_scheduler.step() and synchronize streams.
@@ -118,18 +118,18 @@
                 try:
                     check_overflow(optimizer.param_groups)
                 except OverflowError:
                     has_overflow = True
                     break
             if has_overflow:
                 print_rank("Gradient overflow, change scale from %lf to %lf" % (self.loss_scale, self.loss_scale / self.loss_scale_factor))
-                self._justify_scale(self.loss_scale / self.loss_scale_factor)
-                self.zero_grad()
+                with torch.no_grad():
+                    self._justify_scale(self.loss_scale / self.loss_scale_factor)
+                    self.zero_grad()
                 return
-                
         for optimizer, lr_scheduler in zip(self.optimizers, self.lr_schedulers):
             if hasattr(optimizer, "_bmtrain_optimizer") and optimizer._bmtrain_optimizer:
                 optimizer.step(scale=self.loss_scale)
             else:
                 if self.loss_scale_enabled:
                     grad_rescale(optimizer.param_groups, self.loss_scale)
                 optimizer.step()
```

### Comparing `bmtrain-0.2.2/bmtrain/param_init.py` & `bmtrain-0.2.3/bmtrain/param_init.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/parameter.py` & `bmtrain-0.2.3/bmtrain/parameter.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/pipe_layer.py` & `bmtrain-0.2.3/bmtrain/pipe_layer.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/store.py` & `bmtrain-0.2.3/bmtrain/store.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/synchronize.py` & `bmtrain-0.2.3/bmtrain/synchronize.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain/utils.py` & `bmtrain-0.2.3/bmtrain/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 import torch
 import sys
 from typing import Any, Dict, Iterable, Optional
 from .global_var import config
 
 ALIGN = 4
 ROW_WIDTH = 60
+def check_torch_version(version_str):
+    """
+    Checks if the current torch version is greater than or equal to the given version.
+    version_str (str): The version to compare with, in the format of "x.y.z" ,and the func will convert it into a int value of x*100+y*10+z.
+    """
+    version_int_arr = [int(v) for v in version_str.split(".")]
+
+    version_int = version_int_arr[0] * 10000 + version_int_arr[1] * 100 + version_int_arr[2]
+    torch_version = torch.__version__.split("+")[0]
+    current_version_int_arr = [int(v) for v in torch_version.split(".")]
+    current_version_int = current_version_int_arr[0] * 10000 + current_version_int_arr[1] * 100 + current_version_int_arr[2]
+    return current_version_int - version_int
 
 def round_up(x, d):
     return (x + d - 1) // d * d
 
 def print_dict(title : str, content : Dict[str, Any], file=sys.stdout):
     max_kw_len = max([ len(kw) for kw in content.keys() ])
     max_kw_len = round_up(max_kw_len + 3, 4)
```

### Comparing `bmtrain-0.2.2/bmtrain/wrapper.py` & `bmtrain-0.2.3/bmtrain/wrapper.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.2/bmtrain.egg-info/SOURCES.txt` & `bmtrain-0.2.3/bmtrain.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -29,31 +29,31 @@
 bmtrain/distributed/__init__.py
 bmtrain/distributed/ops.py
 bmtrain/inspect/__init__.py
 bmtrain/inspect/format.py
 bmtrain/inspect/model.py
 bmtrain/inspect/tensor.py
 bmtrain/loss/__init__.py
+bmtrain/loss/_function.py
 bmtrain/loss/cross_entropy.py
 bmtrain/lr_scheduler/__init__.py
 bmtrain/lr_scheduler/cosine.py
 bmtrain/lr_scheduler/exponential.py
 bmtrain/lr_scheduler/linear.py
 bmtrain/lr_scheduler/no_decay.py
 bmtrain/lr_scheduler/noam.py
 bmtrain/lr_scheduler/warmup.py
 bmtrain/nccl/__init__.py
 bmtrain/nccl/enums.py
 bmtrain/optim/__init__.py
+bmtrain/optim/_function.py
 bmtrain/optim/adam.py
 bmtrain/optim/adam_offload.py
 bmtrain/optim/optim_manager.py
-csrc/adam_cpu.cpp
-csrc/adam_cuda.cpp
-csrc/cross_entropy_loss.cpp
-csrc/nccl.cpp
-csrc/cuda/adam.cu
+csrc/bind.cpp
+csrc/cuda/adam_cuda.cu
 csrc/cuda/cross_entropy.cu
 csrc/cuda/has_inf_nan.cu
 csrc/cuda/reduce.cuh
-csrc/include/nccl.h
-csrc/include/nccl_net.h
+csrc/include/adam_cpu.hpp
+csrc/include/bind.hpp
+csrc/include/nccl.hpp
```

### Comparing `bmtrain-0.2.2/csrc/cuda/adam.cu` & `bmtrain-0.2.3/csrc/cuda/adam_cuda.cu`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #include <cuda_fp16.h>
-#include <torch/extension.h>
-#include <ATen/cuda/CUDAContext.h>
+#include <cstdint>
 
 namespace {
 // blocks <n // 1024>,      threads<min(n, 1024)>
 __global__ void adam_fp32_accum(
     int32_t n,
     const half *g,        // (n)
     half *m,        // (n)
@@ -33,32 +32,32 @@
         v[col] = local_v;
         m[col] = __float2half(local_m);
     }
 }
 }
 
 void adam_launcher(
-    const torch::Tensor &param_fp32,
-    const torch::Tensor &param_fp16,
-    const torch::Tensor &g_fp16,
-    const torch::Tensor &m_fp16,
-    const torch::Tensor &v_fp32,
+    int n,
+    std::uintptr_t param_fp32,
+    std::uintptr_t param_fp16,
+    std::uintptr_t g_fp16,
+    std::uintptr_t m_fp16,
+    std::uintptr_t v_fp32,
     float beta1, float beta2,
     float eps, float lr,
     float scale,
     float weight_decay,
     float bias_correction1,
-    float bias_correction2
+    float bias_correction2,
+    uintptr_t stream
 ) {
-    int32_t n = param_fp32.numel();
     if (n <= 0) return;
-    auto g_ptr = reinterpret_cast<half*>(g_fp16.data_ptr<at::Half>());
-    auto m_ptr = reinterpret_cast<half*>(m_fp16.data_ptr<at::Half>());
-    auto v_ptr = v_fp32.data_ptr<float>();
-    auto param_ptr = param_fp32.data_ptr<float>();
-    auto param_h_ptr = reinterpret_cast<half*>(param_fp16.data_ptr<at::Half>());
+    auto g_ptr = reinterpret_cast<half*>(g_fp16);
+    auto m_ptr = reinterpret_cast<half*>(m_fp16);
+    auto param_h_ptr = reinterpret_cast<half*>(param_fp16);
+    auto param_fp32_ptr = reinterpret_cast<float*>(param_fp32);
+    auto v_fp32_ptr = reinterpret_cast<float*>(v_fp32);
     int32_t threads = 1024;
     dim3 block_size = dim3(threads, 1, 1);
     dim3 grid_size = dim3((n + threads - 1) / threads, 1, 1);
-    auto stream = at::cuda::getCurrentCUDAStream();
-    adam_fp32_accum<<<grid_size, block_size, 0, stream.stream()>>>(n, g_ptr, m_ptr, v_ptr, param_ptr, param_h_ptr, beta1, beta2, eps, lr, scale, weight_decay, bias_correction1, bias_correction2);
+    adam_fp32_accum<<<grid_size, block_size, 0, reinterpret_cast<cudaStream_t>(stream)>>>(n, g_ptr, m_ptr, v_fp32_ptr, param_fp32_ptr, param_h_ptr, beta1, beta2, eps, lr, scale, weight_decay, bias_correction1, bias_correction2);
 }
```

### Comparing `bmtrain-0.2.2/csrc/cuda/cross_entropy.cu` & `bmtrain-0.2.3/csrc/cuda/cross_entropy.cu`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #include <cuda_fp16.h>
-#include <torch/extension.h>
-#include <ATen/cuda/CUDAContext.h>
 #include "reduce.cuh"
+#include <cstdint>
+#include<cuda_runtime_api.h>
 
 namespace {
 // blocks <m>,      threads<1024>
 __global__ void cross_entropy_forward(
     int64_t n,
     const half *input,      // (m, n)
     const int32_t *target,  // (m)
@@ -130,68 +130,78 @@
     }
 }
 
 }
 
 void cross_entropy_forward_launcher(
     int32_t m, int32_t n,
-    const torch::Tensor &input,
-    const torch::Tensor &target,
-    torch::Tensor &softmax,
-    torch::Tensor &output,
-    int32_t ignore_index
-) {
-    auto input_ptr = reinterpret_cast<half*>(input.data_ptr<at::Half>());
-    auto target_ptr = target.data_ptr<int32_t>();
-    auto softmax_ptr = reinterpret_cast<half*>(softmax.data_ptr<at::Half>());
-    auto output_ptr = output.data_ptr<float>();
+    std::uintptr_t input,
+    std::uintptr_t target,
+    std::uintptr_t softmax,
+    std::uintptr_t output,
+    int32_t ignore_index,
+    std::uintptr_t stream
+) {
+    auto input_ptr = reinterpret_cast<half*>(input);
+    auto target_ptr = reinterpret_cast<int32_t*>(target);
+    auto softmax_ptr = reinterpret_cast<half*>(softmax);
+    auto output_ptr = reinterpret_cast<float*>(output);
     int32_t threads = 1024;
-    auto stream = at::cuda::getCurrentCUDAStream();
-    cross_entropy_forward<<<m, threads, 0, stream.stream()>>>(n, input_ptr, target_ptr, softmax_ptr, output_ptr, ignore_index);
+    cross_entropy_forward<<<m, threads, 0, reinterpret_cast<cudaStream_t>(stream)>>>(n, input_ptr, target_ptr, softmax_ptr, output_ptr, ignore_index);
 }
 
 void cross_entropy_backward_launcher(
     int32_t m, int32_t n,
-    const torch::Tensor &grad_output,
-    const torch::Tensor &target,
-    const torch::Tensor &softmax,
-    torch::Tensor &grad_input,
-    int32_t ignore_index
-) {
-    auto output_ptr = grad_output.data_ptr<float>();
-    auto target_ptr = target.data_ptr<int32_t>();
-    auto softmax_ptr = reinterpret_cast<half*>(softmax.data_ptr<at::Half>());
-    auto input_ptr = reinterpret_cast<half*>(grad_input.data_ptr<at::Half>());
+    std::uintptr_t grad_output,
+    std::uintptr_t target,
+    std::uintptr_t softmax,
+    std::uintptr_t grad_input,
+    int32_t ignore_index,
+    std::uintptr_t stream
+) {
+    // auto output_ptr = grad_output.data_ptr<float>();
+    auto output_ptr = reinterpret_cast<float*>(grad_output);
+    // auto target_ptr = target.data_ptr<int32_t>();
+    auto target_ptr = reinterpret_cast<int32_t*>(target);
+    auto softmax_ptr = reinterpret_cast<half*>(softmax);
+    auto input_ptr = reinterpret_cast<half*>(grad_input);
     int32_t threads = 1024;
-    auto stream = at::cuda::getCurrentCUDAStream();
-    cross_entropy_backward<<<m, threads, 0, stream.stream()>>>(n, output_ptr, target_ptr, softmax_ptr, input_ptr, ignore_index);
+    cross_entropy_backward<<<m, threads, 0, reinterpret_cast<cudaStream_t>(stream)>>>(n, output_ptr, target_ptr, softmax_ptr, input_ptr, ignore_index);
 }
 
 void cross_entropy_forward_inplace_launcher(
     int32_t m, int32_t n,
-    torch::Tensor &x,
-    const torch::Tensor &target,
-    torch::Tensor &output,
-    int32_t ignore_index
-) {
-    auto x_ptr = reinterpret_cast<half*>(x.data_ptr<at::Half>());
-    auto target_ptr = target.data_ptr<int32_t>();
-    auto output_ptr = output.data_ptr<float>();
+    std::uintptr_t x,
+    std::uintptr_t target,
+    std::uintptr_t output,
+    int32_t ignore_index,
+    std::uintptr_t stream
+) {
+    // auto x_ptr = reinterpret_cast<half*>(x.data_ptr<at::Half>());
+    auto x_ptr = reinterpret_cast<half*>(x);
+    // auto target_ptr = target.data_ptr<int32_t>();
+    auto target_ptr = reinterpret_cast<int32_t*>(target);
+    // auto output_ptr = output.data_ptr<float>();
+    auto output_ptr = reinterpret_cast<float*>(output);
     int32_t threads = 1024;
-    auto stream = at::cuda::getCurrentCUDAStream();
-    cross_entropy_forward_inplace<<<m, threads, 0, stream.stream()>>>(n, x_ptr, target_ptr, output_ptr, ignore_index);
+    // auto stream = at::cuda::getCurrentCUDAStream();
+    cross_entropy_forward_inplace<<<m, threads, 0, reinterpret_cast<cudaStream_t>(stream)>>>(n, x_ptr, target_ptr, output_ptr, ignore_index);
 }
 
 void cross_entropy_backward_inplace_launcher(
     int32_t m, int32_t n,
-    const torch::Tensor &grad_output,
-    const torch::Tensor &target,
-    torch::Tensor &x,
-    int32_t ignore_index
-) {
-    auto output_ptr = grad_output.data_ptr<float>();
-    auto target_ptr = target.data_ptr<int32_t>();
-    auto x_ptr = reinterpret_cast<half*>(x.data_ptr<at::Half>());
+    std::uintptr_t grad_output,
+    std::uintptr_t target,
+    std::uintptr_t x,
+    int32_t ignore_index,
+    std::uintptr_t stream
+) {
+    // auto output_ptr = grad_output.data_ptr<float>();
+    auto output_ptr = reinterpret_cast<float*>(grad_output);
+    // auto target_ptr = target.data_ptr<int32_t>();
+    auto target_ptr = reinterpret_cast<int32_t*>(target);
+    // auto x_ptr = reinterpret_cast<half*>(x.data_ptr<at::Half>());
+    auto x_ptr = reinterpret_cast<half*>(x);
     int32_t threads = 1024;
-    auto stream = at::cuda::getCurrentCUDAStream();
-    cross_entropy_backward_inplace<<<m, threads, 0, stream.stream()>>>(n, output_ptr, target_ptr, x_ptr, ignore_index);
+    // auto stream = at::cuda::getCurrentCUDAStream();
+    cross_entropy_backward_inplace<<<m, threads, 0, reinterpret_cast<cudaStream_t>(stream)>>>(n, output_ptr, target_ptr, x_ptr, ignore_index);
 }
```

### Comparing `bmtrain-0.2.2/csrc/cuda/has_inf_nan.cu` & `bmtrain-0.2.3/csrc/cuda/has_inf_nan.cu`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #include <cuda_fp16.h>
-#include <torch/extension.h>
-#include <ATen/cuda/CUDAContext.h>
+#include <cstdint>
 
 namespace{
 __inline__ __device__ bool isnan_(half v) {
 #if __CUDA_ARCH__ >= 700 || __CUDA_ARCH__ == 600
     return __hisnan(v);
 #else
     
@@ -64,25 +63,25 @@
         out[0] = 1;
     }
 }
 
 }
 
 void has_nan_inf_launcher(
-    const torch::Tensor &g_fp16,
-    torch::Tensor mid,
-    torch::Tensor out
+    int32_t n,
+    std::uintptr_t g_fp16,
+    std::uintptr_t mid,
+    std::uintptr_t out,
+    std::uintptr_t stream
 ) {
-    int n = g_fp16.numel();
     if (n <= 0) return;
-    auto g_ptr = reinterpret_cast<half*>(g_fp16.data_ptr<at::Half>());
-    auto mid_ptr = mid.data_ptr<uint8_t>();
-    auto stream = at::cuda::getCurrentCUDAStream();
-
+    auto g_ptr = reinterpret_cast<half*>(g_fp16);
+    auto mid_ptr = reinterpret_cast<uint8_t*>(mid);
+    auto out_ptr = reinterpret_cast<uint8_t*>(out);
     int32_t threads = 1024;
     dim3 block_size = dim3(threads, 1, 1);
     dim3 grid_size = dim3((n + threads - 1) / threads, 1, 1);
     dim3 clamp_grid_size = dim3(min((n + threads - 1) / threads, 1024), 1, 1);
     
-    bmt_has_nan_inf_1<<<clamp_grid_size, block_size, 0, stream.stream()>>>(n, g_ptr, mid_ptr);
-    bmt_has_nan_inf_2<<<1, block_size, 0, stream.stream()>>>(mid_ptr, out.data_ptr<uint8_t>());
+    bmt_has_nan_inf_1<<<clamp_grid_size, block_size, 0, reinterpret_cast<cudaStream_t>(stream)>>>(n, g_ptr, mid_ptr);
+    bmt_has_nan_inf_2<<<1, block_size, 0, reinterpret_cast<cudaStream_t>(stream)>>>(mid_ptr, out_ptr);
 }
```

### Comparing `bmtrain-0.2.2/csrc/cuda/reduce.cuh` & `bmtrain-0.2.3/csrc/cuda/reduce.cuh`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #include <cuda_fp16.h>
-#include <torch/extension.h>
-#include <ATen/cuda/CUDAContext.h>
 
 namespace {
 const int WARP_SZ = 32;
 
 // blocks <block_size>,      threads<1024>
 __device__ float block_reduce_sum(float val) {
     static __shared__ float s_x[WARP_SZ];
```

### Comparing `bmtrain-0.2.2/csrc/nccl.cpp` & `bmtrain-0.2.3/csrc/include/nccl.hpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+#include <cstdint>
+#include <string>
+#include <pybind11/pybind11.h>
 
-#include <torch/extension.h>
-#include "include/nccl.h"
-#include <ATen/cuda/CUDAContext.h>
+namespace py = pybind11;
+#include <nccl.h>
 
 void checkNCCLStatus(ncclResult_t result) {
     if (result == ncclSuccess) return;
     throw std::logic_error(
         std::string("NCCL Error: ") +
         ncclGetErrorString(result)
     );
@@ -180,23 +182,7 @@
 int pyNCCLCommUserRank(
     std::uintptr_t comm
 ){
     int rank;
     checkNCCLStatus(ncclCommUserRank(reinterpret_cast<ncclComm_t>(comm),&rank));
     return rank;
 }
-PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
-    m.def("ncclGetUniqueId", &pyNCCLGetUniqueID, "nccl get unique ID");
-    m.def("ncclCommInitRank", &pyNCCLCommInitRank, "nccl init rank");
-    m.def("ncclCommDestroy", &pyNCCLCommDestroy, "nccl delete rank");
-    m.def("ncclAllGather", &pyNCCLAllGather, "nccl all gather");
-    m.def("ncclAllReduce", &pyNCCLAllReduce, "nccl all reduce");
-    m.def("ncclBroadcast", &pyNCCLBroadcast, "nccl broadcast");
-    m.def("ncclReduce", &pyNCCLReduce, "nccl reduce");
-    m.def("ncclReduceScatter", &pyNCCLReduceScatter, "nccl reduce scatter");
-    m.def("ncclGroupStart", &pyNCCLGroupStart, "nccl group start");
-    m.def("ncclGroupEnd", &pyNCCLGroupEnd, "nccl group end");
-    m.def("ncclSend",&pyNCCLSend,"nccl send");
-    m.def("ncclRecv",&pyNCCLRecv,"nccl recv");
-    m.def("ncclCommCount",&pyNCCLCommCount,"nccl comm count");
-    m.def("ncclCommUserRank",&pyNCCLCommUserRank,"nccl comm user rank");
-}
```

