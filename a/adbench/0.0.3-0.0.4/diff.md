# Comparing `tmp/adbench-0.0.3.tar.gz` & `tmp/adbench-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adbench-0.0.3.tar", last modified: Tue Jul 11 10:04:11 2023, max compression
+gzip compressed data, was "dist\adbench-0.0.4.tar", last modified: Tue Jul 11 10:13:14 2023, max compression
```

## Comparing `adbench-0.0.3.tar` & `adbench-0.0.4.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/
--rw-rw-rw-   0        0        0      187 2023-07-08 02:17:37.000000 adbench-0.0.3/.gitattributes
--rw-rw-rw-   0        0        0       69 2023-07-08 02:17:37.000000 adbench-0.0.3/.gitignore
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/.idea/
--rw-rw-rw-   0        0        0      184 2023-07-08 02:17:37.000000 adbench-0.0.3/.idea/.gitignore
--rw-rw-rw-   0        0        0      334 2023-07-11 05:42:23.000000 adbench-0.0.3/.idea/ADBench.iml
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      179 2023-07-08 02:17:37.000000 adbench-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      198 2023-07-11 05:42:23.000000 adbench-0.0.3/.idea/misc.xml
--rw-rw-rw-   0        0        0      273 2023-07-08 02:17:37.000000 adbench-0.0.3/.idea/modules.xml
--rw-rw-rw-   0        0        0      185 2023-07-08 02:17:37.000000 adbench-0.0.3/.idea/vcs.xml
--rw-rw-rw-   0        0        0     1349 2023-07-08 02:17:37.000000 adbench-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       77 2023-07-08 02:17:37.000000 adbench-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      950 2023-07-11 10:04:11.000000 adbench-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    21380 2023-07-11 08:28:24.000000 adbench-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/adbench/
--rw-rw-rw-   0        0        0        0 2023-07-11 01:14:34.000000 adbench-0.0.3/adbench/__init__.py
--rw-rw-rw-   0        0        0    11421 2023-07-08 02:17:46.000000 adbench-0.0.3/adbench/myutils.py
--rw-rw-rw-   0        0        0    13264 2023-07-11 09:40:24.000000 adbench-0.0.3/adbench/run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/adbench.egg-info/
--rw-rw-rw-   0        0        0      950 2023-07-11 10:04:00.000000 adbench-0.0.3/adbench.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3683 2023-07-11 10:04:11.000000 adbench-0.0.3/adbench.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 10:04:00.000000 adbench-0.0.3/adbench.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-07-11 10:04:00.000000 adbench-0.0.3/adbench.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-11 10:04:00.000000 adbench-0.0.3/adbench.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DAGMM/
--rw-rw-rw-   0        0        0        8 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DAGMM/.gitignore
--rw-rw-rw-   0        0        0     3287 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DAGMM/forward_step.py
--rw-rw-rw-   0        0        0     1895 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DAGMM/main.py
--rw-rw-rw-   0        0        0     1775 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DAGMM/model.py
--rw-rw-rw-   0        0        0     2003 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DAGMM/preprocess.py
--rw-rw-rw-   0        0        0     4193 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/DAGMM/run.py
--rw-rw-rw-   0        0        0     5411 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DAGMM/test.py
--rw-rw-rw-   0        0        0     1983 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DAGMM/train.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DAGMM/utils/
--rw-rw-rw-   0        0        0      528 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DAGMM/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/
--rw-rw-rw-   0        0        0     1087 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/LICENSE
--rw-rw-rw-   0        0        0     6935 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/README.md
--rw-rw-rw-   0        0        0      138 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/ae_results.json
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/imgs/
--rw-rw-rw-   0        0        0   319030 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/imgs/fig1.png
--rw-rw-rw-   0        0        0   104296 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/log.txt
--rw-rw-rw-   0        0        0      298 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/requirements.txt
--rw-rw-rw-   0        0        0    16944 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/results.json
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/base/
--rw-rw-rw-   0        0        0      148 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/base/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/base/base_dataset.py
--rw-rw-rw-   0        0        0      823 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/base/base_net.py
--rw-rw-rw-   0        0        0     1166 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/base/base_trainer.py
--rw-rw-rw-   0        0        0     1682 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/base/odds_dataset.py
--rw-rw-rw-   0        0        0      846 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/base/torchvision_dataset.py
--rw-rw-rw-   0        0        0    13565 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baseline_SemiDGM.py
--rw-rw-rw-   0        0        0     9937 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baseline_isoforest.py
--rw-rw-rw-   0        0        0     9478 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baseline_kde.py
--rw-rw-rw-   0        0        0     9062 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baseline_ocsvm.py
--rw-rw-rw-   0        0        0     9157 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baseline_ssad.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/
--rw-rw-rw-   0        0        0     5610 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/SemiDGM.py
--rw-rw-rw-   0        0        0      202 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/__init__.py
--rw-rw-rw-   0        0        0     5879 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/isoforest.py
--rw-rw-rw-   0        0        0     6702 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/kde.py
--rw-rw-rw-   0        0        0     9033 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/ocsvm.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/shallow_ssad/
--rw-rw-rw-   0        0        0       37 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/shallow_ssad/__init__.py
--rw-rw-rw-   0        0        0     8022 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py
--rw-rw-rw-   0        0        0    10201 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/baselines/ssad.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/datasets/
--rw-rw-rw-   0        0        0      215 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/datasets/__init__.py
--rw-rw-rw-   0        0        0     3609 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/datasets/cifar10.py
--rw-rw-rw-   0        0        0     3663 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/datasets/fmnist.py
--rw-rw-rw-   0        0        0      325 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/datasets/main.py
--rw-rw-rw-   0        0        0     3598 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/datasets/mnist.py
--rw-rw-rw-   0        0        0     1468 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/datasets/odds.py
--rw-rw-rw-   0        0        0     3629 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/datasets/preprocessing.py
--rw-rw-rw-   0        0        0     7051 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/deepsad.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/
--rw-rw-rw-   0        0        0      706 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/__init__.py
--rw-rw-rw-   0        0        0     3085 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/cifar10_LeNet.py
--rw-rw-rw-   0        0        0     4405 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/dgm.py
--rw-rw-rw-   0        0        0     2584 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/fmnist_LeNet.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/inference/
--rw-rw-rw-   0        0        0     1256 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/inference/distributions.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/layers/
--rw-rw-rw-   0        0        0     1705 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/layers/standard.py
--rw-rw-rw-   0        0        0     1511 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/layers/stochastic.py
--rw-rw-rw-   0        0        0     1501 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/main.py
--rw-rw-rw-   0        0        0     2328 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/mlp.py
--rw-rw-rw-   0        0        0     2222 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/mnist_LeNet.py
--rw-rw-rw-   0        0        0     4826 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/networks/vae.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/optim/
--rw-rw-rw-   0        0        0     7116 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/optim/DeepSAD_trainer.py
--rw-rw-rw-   0        0        0     7554 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/optim/SemiDGM_trainer.py
--rw-rw-rw-   0        0        0      230 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/optim/__init__.py
--rw-rw-rw-   0        0        0     5379 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/optim/ae_trainer.py
--rw-rw-rw-   0        0        0     5247 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/optim/vae_trainer.py
--rw-rw-rw-   0        0        0     2816 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/optim/variational.py
--rw-rw-rw-   0        0        0     4957 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/DeepSAD/src/run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/utils/
--rw-rw-rw-   0        0        0      163 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/utils/__init__.py
--rw-rw-rw-   0        0        0      682 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/utils/config.py
--rw-rw-rw-   0        0        0     1468 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DeepSAD/src/utils/visualization/
--rw-rw-rw-   0        0        0      803 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/DevNet/
--rw-rw-rw-   0        0        0    10544 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/DevNet/run.py
--rw-rw-rw-   0        0        0     2367 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/DevNet/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/FEAWAD/
--rw-rw-rw-   0        0        0    18593 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/FEAWAD/run.py
--rw-rw-rw-   0        0        0     1533 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/FEAWAD/toolsdev.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/FTTransformer/
--rw-rw-rw-   0        0        0     6098 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/FTTransformer/run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/GANomaly/
--rw-rw-rw-   0        0        0     3001 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/GANomaly/fit.py
--rw-rw-rw-   0        0        0     1260 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/GANomaly/model.py
--rw-rw-rw-   0        0        0     3005 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/GANomaly/run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/PReNet/
--rw-rw-rw-   0        0        0     1219 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/PReNet/fit.py
--rw-rw-rw-   0        0        0      703 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/PReNet/model.py
--rw-rw-rw-   0        0        0     2936 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/PReNet/run.py
--rw-rw-rw-   0        0        0     2931 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/PReNet/utils.py
--rw-rw-rw-   0        0        0    13241 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/PyOD.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/baseline/REPEN/
--rw-rw-rw-   0        0        0    12601 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/REPEN/model.py
--rw-rw-rw-   0        0        0     1680 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/REPEN/run.py
--rw-rw-rw-   0        0        0     2011 2023-07-08 02:17:37.000000 adbench-0.0.3/baseline/REPEN/utils.py
--rw-rw-rw-   0        0        0     1491 2023-07-11 01:16:07.000000 adbench-0.0.3/baseline/Supervised.py
--rw-rw-rw-   0        0        0        0 2023-07-11 01:13:54.000000 adbench-0.0.3/baseline/__init__.py
--rw-rw-rw-   0        0        0   342901 2023-07-11 08:43:19.000000 adbench-0.0.3/demo.ipynb
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/figs/
--rw-rw-rw-   0        0        0   211827 2023-07-08 02:17:46.000000 adbench-0.0.3/figs/ADBench.png
--rw-rw-rw-   0        0        0   211827 2023-07-08 02:17:46.000000 adbench-0.0.3/figs/ADBenchV2.png
--rw-rw-rw-   0        0        0   654664 2023-07-08 02:17:46.000000 adbench-0.0.3/figs/Algorithms.png
--rw-rw-rw-   0        0        0   318580 2023-07-08 02:17:46.000000 adbench-0.0.3/figs/MNIST-C.png
--rw-rw-rw-   0        0        0   238201 2023-07-08 02:17:46.000000 adbench-0.0.3/figs/MVTec-AD(ViT).png
--rw-rw-rw-   0        0        0   238487 2023-07-08 02:17:46.000000 adbench-0.0.3/figs/MVTec-AD.png
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/other_utils/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:04:11.000000 adbench-0.0.3/other_utils/gmm/
--rw-rw-rw-   0        0        0     1090 2023-07-08 02:17:46.000000 adbench-0.0.3/other_utils/gmm/LICENSE.md
--rw-rw-rw-   0        0        0      863 2023-07-08 02:17:46.000000 adbench-0.0.3/other_utils/gmm/README.md
--rw-rw-rw-   0        0        0   131595 2023-07-08 02:17:46.000000 adbench-0.0.3/other_utils/gmm/example.png
--rw-rw-rw-   0        0        0     2111 2023-07-08 02:17:46.000000 adbench-0.0.3/other_utils/gmm/example.py
--rw-rw-rw-   0        0        0    19852 2023-07-08 02:17:46.000000 adbench-0.0.3/other_utils/gmm/gmm.py
--rw-rw-rw-   0        0        0     6856 2023-07-08 02:17:46.000000 adbench-0.0.3/other_utils/gmm/test.py
--rw-rw-rw-   0        0        0     1129 2023-07-08 02:17:46.000000 adbench-0.0.3/other_utils/gmm/utils.py
--rw-rw-rw-   0        0        0    14138 2023-07-08 02:17:46.000000 adbench-0.0.3/other_utils/utils.py
--rw-rw-rw-   0        0        0      133 2023-07-11 09:24:54.000000 adbench-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 10:04:11.000000 adbench-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1392 2023-07-11 09:56:29.000000 adbench-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/
+-rw-rw-rw-   0        0        0      187 2023-07-08 02:17:37.000000 adbench-0.0.4/.gitattributes
+-rw-rw-rw-   0        0        0       69 2023-07-08 02:17:37.000000 adbench-0.0.4/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/.idea/
+-rw-rw-rw-   0        0        0      184 2023-07-08 02:17:37.000000 adbench-0.0.4/.idea/.gitignore
+-rw-rw-rw-   0        0        0      334 2023-07-11 05:42:23.000000 adbench-0.0.4/.idea/ADBench.iml
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      179 2023-07-08 02:17:37.000000 adbench-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      198 2023-07-11 05:42:23.000000 adbench-0.0.4/.idea/misc.xml
+-rw-rw-rw-   0        0        0      273 2023-07-08 02:17:37.000000 adbench-0.0.4/.idea/modules.xml
+-rw-rw-rw-   0        0        0      185 2023-07-08 02:17:37.000000 adbench-0.0.4/.idea/vcs.xml
+-rw-rw-rw-   0        0        0     1349 2023-07-08 02:17:37.000000 adbench-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       77 2023-07-08 02:17:37.000000 adbench-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      950 2023-07-11 10:13:14.000000 adbench-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    21380 2023-07-11 08:28:24.000000 adbench-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/adbench/
+-rw-rw-rw-   0        0        0        0 2023-07-11 01:14:34.000000 adbench-0.0.4/adbench/__init__.py
+-rw-rw-rw-   0        0        0    11421 2023-07-08 02:17:46.000000 adbench-0.0.4/adbench/myutils.py
+-rw-rw-rw-   0        0        0    13264 2023-07-11 09:40:24.000000 adbench-0.0.4/adbench/run.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/adbench.egg-info/
+-rw-rw-rw-   0        0        0      950 2023-07-11 10:13:01.000000 adbench-0.0.4/adbench.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3683 2023-07-11 10:13:14.000000 adbench-0.0.4/adbench.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:13:01.000000 adbench-0.0.4/adbench.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-11 10:13:01.000000 adbench-0.0.4/adbench.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-11 10:13:01.000000 adbench-0.0.4/adbench.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DAGMM/
+-rw-rw-rw-   0        0        0        8 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/.gitignore
+-rw-rw-rw-   0        0        0     3287 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/forward_step.py
+-rw-rw-rw-   0        0        0     1895 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/main.py
+-rw-rw-rw-   0        0        0     1775 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/model.py
+-rw-rw-rw-   0        0        0     2003 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/preprocess.py
+-rw-rw-rw-   0        0        0     4193 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/DAGMM/run.py
+-rw-rw-rw-   0        0        0     5411 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/test.py
+-rw-rw-rw-   0        0        0     1983 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/train.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DAGMM/utils/
+-rw-rw-rw-   0        0        0      528 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/
+-rw-rw-rw-   0        0        0     1087 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/LICENSE
+-rw-rw-rw-   0        0        0     6935 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/README.md
+-rw-rw-rw-   0        0        0      138 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/ae_results.json
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/imgs/
+-rw-rw-rw-   0        0        0   319030 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/imgs/fig1.png
+-rw-rw-rw-   0        0        0   104296 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/log.txt
+-rw-rw-rw-   0        0        0      298 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/requirements.txt
+-rw-rw-rw-   0        0        0    16944 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/results.json
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/base/
+-rw-rw-rw-   0        0        0      148 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/base_dataset.py
+-rw-rw-rw-   0        0        0      823 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/base_net.py
+-rw-rw-rw-   0        0        0     1166 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/base_trainer.py
+-rw-rw-rw-   0        0        0     1682 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/odds_dataset.py
+-rw-rw-rw-   0        0        0      846 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/torchvision_dataset.py
+-rw-rw-rw-   0        0        0    13565 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_SemiDGM.py
+-rw-rw-rw-   0        0        0     9937 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_isoforest.py
+-rw-rw-rw-   0        0        0     9478 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_kde.py
+-rw-rw-rw-   0        0        0     9062 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_ocsvm.py
+-rw-rw-rw-   0        0        0     9157 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_ssad.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/
+-rw-rw-rw-   0        0        0     5610 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/SemiDGM.py
+-rw-rw-rw-   0        0        0      202 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/__init__.py
+-rw-rw-rw-   0        0        0     5879 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/isoforest.py
+-rw-rw-rw-   0        0        0     6702 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/kde.py
+-rw-rw-rw-   0        0        0     9033 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/ocsvm.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/shallow_ssad/
+-rw-rw-rw-   0        0        0       37 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/shallow_ssad/__init__.py
+-rw-rw-rw-   0        0        0     8022 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py
+-rw-rw-rw-   0        0        0    10201 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/ssad.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/
+-rw-rw-rw-   0        0        0      215 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3609 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/cifar10.py
+-rw-rw-rw-   0        0        0     3663 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/fmnist.py
+-rw-rw-rw-   0        0        0      325 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/main.py
+-rw-rw-rw-   0        0        0     3598 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/mnist.py
+-rw-rw-rw-   0        0        0     1468 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/odds.py
+-rw-rw-rw-   0        0        0     3629 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/preprocessing.py
+-rw-rw-rw-   0        0        0     7051 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/deepsad.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/
+-rw-rw-rw-   0        0        0      706 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/__init__.py
+-rw-rw-rw-   0        0        0     3085 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/cifar10_LeNet.py
+-rw-rw-rw-   0        0        0     4405 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/dgm.py
+-rw-rw-rw-   0        0        0     2584 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/fmnist_LeNet.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/inference/
+-rw-rw-rw-   0        0        0     1256 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/inference/distributions.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/layers/
+-rw-rw-rw-   0        0        0     1705 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/layers/standard.py
+-rw-rw-rw-   0        0        0     1511 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/layers/stochastic.py
+-rw-rw-rw-   0        0        0     1501 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/main.py
+-rw-rw-rw-   0        0        0     2328 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/mlp.py
+-rw-rw-rw-   0        0        0     2222 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/mnist_LeNet.py
+-rw-rw-rw-   0        0        0     4826 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/vae.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/
+-rw-rw-rw-   0        0        0     7116 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/DeepSAD_trainer.py
+-rw-rw-rw-   0        0        0     7554 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/SemiDGM_trainer.py
+-rw-rw-rw-   0        0        0      230 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/__init__.py
+-rw-rw-rw-   0        0        0     5379 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/ae_trainer.py
+-rw-rw-rw-   0        0        0     5247 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/vae_trainer.py
+-rw-rw-rw-   0        0        0     2816 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/variational.py
+-rw-rw-rw-   0        0        0     4957 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/DeepSAD/src/run.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/
+-rw-rw-rw-   0        0        0      163 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      682 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/config.py
+-rw-rw-rw-   0        0        0     1468 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/visualization/
+-rw-rw-rw-   0        0        0      803 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DevNet/
+-rw-rw-rw-   0        0        0    10544 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/DevNet/run.py
+-rw-rw-rw-   0        0        0     2367 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DevNet/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/FEAWAD/
+-rw-rw-rw-   0        0        0    18593 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/FEAWAD/run.py
+-rw-rw-rw-   0        0        0     1533 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/FEAWAD/toolsdev.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/FTTransformer/
+-rw-rw-rw-   0        0        0     6098 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/FTTransformer/run.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/GANomaly/
+-rw-rw-rw-   0        0        0     3001 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/GANomaly/fit.py
+-rw-rw-rw-   0        0        0     1260 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/GANomaly/model.py
+-rw-rw-rw-   0        0        0     3005 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/GANomaly/run.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/PReNet/
+-rw-rw-rw-   0        0        0     1219 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/PReNet/fit.py
+-rw-rw-rw-   0        0        0      703 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/PReNet/model.py
+-rw-rw-rw-   0        0        0     2936 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/PReNet/run.py
+-rw-rw-rw-   0        0        0     2931 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/PReNet/utils.py
+-rw-rw-rw-   0        0        0    13241 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/PyOD.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/REPEN/
+-rw-rw-rw-   0        0        0    12601 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/REPEN/model.py
+-rw-rw-rw-   0        0        0     1680 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/REPEN/run.py
+-rw-rw-rw-   0        0        0     2011 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/REPEN/utils.py
+-rw-rw-rw-   0        0        0     1491 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/Supervised.py
+-rw-rw-rw-   0        0        0        0 2023-07-11 01:13:54.000000 adbench-0.0.4/baseline/__init__.py
+-rw-rw-rw-   0        0        0   342901 2023-07-11 08:43:19.000000 adbench-0.0.4/demo.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/figs/
+-rw-rw-rw-   0        0        0   211827 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/ADBench.png
+-rw-rw-rw-   0        0        0   211827 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/ADBenchV2.png
+-rw-rw-rw-   0        0        0   654664 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/Algorithms.png
+-rw-rw-rw-   0        0        0   318580 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/MNIST-C.png
+-rw-rw-rw-   0        0        0   238201 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/MVTec-AD(ViT).png
+-rw-rw-rw-   0        0        0   238487 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/MVTec-AD.png
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/other_utils/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/other_utils/gmm/
+-rw-rw-rw-   0        0        0     1090 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/LICENSE.md
+-rw-rw-rw-   0        0        0      863 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/README.md
+-rw-rw-rw-   0        0        0   131595 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/example.png
+-rw-rw-rw-   0        0        0     2111 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/example.py
+-rw-rw-rw-   0        0        0    19852 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/gmm.py
+-rw-rw-rw-   0        0        0     6856 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/test.py
+-rw-rw-rw-   0        0        0     1129 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/utils.py
+-rw-rw-rw-   0        0        0    14138 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/utils.py
+-rw-rw-rw-   0        0        0      125 2023-07-11 10:11:50.000000 adbench-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 10:13:14.000000 adbench-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2023-07-11 10:12:56.000000 adbench-0.0.4/setup.py
```

### Comparing `adbench-0.0.3/LICENSE` & `adbench-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/PKG-INFO` & `adbench-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbench
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package of ADBench
 Home-page: https://github.com/Minqi824/ADBench
 Author: Minqi Jiang
 Author-email: <jiangmq95@163.com>
 Keywords: anomaly detection,outlier detection,tabular data,benchmark
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `adbench-0.0.3/README.md` & `adbench-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/adbench/myutils.py` & `adbench-0.0.4/adbench/myutils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/adbench/run.py` & `adbench-0.0.4/adbench/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/adbench.egg-info/PKG-INFO` & `adbench-0.0.4/adbench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbench
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package of ADBench
 Home-page: https://github.com/Minqi824/ADBench
 Author: Minqi Jiang
 Author-email: <jiangmq95@163.com>
 Keywords: anomaly detection,outlier detection,tabular data,benchmark
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `adbench-0.0.3/adbench.egg-info/SOURCES.txt` & `adbench-0.0.4/adbench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DAGMM/forward_step.py` & `adbench-0.0.4/baseline/DAGMM/forward_step.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DAGMM/main.py` & `adbench-0.0.4/baseline/DAGMM/main.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DAGMM/model.py` & `adbench-0.0.4/baseline/DAGMM/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DAGMM/preprocess.py` & `adbench-0.0.4/baseline/DAGMM/preprocess.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DAGMM/run.py` & `adbench-0.0.4/baseline/DAGMM/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DAGMM/test.py` & `adbench-0.0.4/baseline/DAGMM/test.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DAGMM/train.py` & `adbench-0.0.4/baseline/DAGMM/train.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DAGMM/utils/utils.py` & `adbench-0.0.4/baseline/DAGMM/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/LICENSE` & `adbench-0.0.4/baseline/DeepSAD/LICENSE`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/README.md` & `adbench-0.0.4/baseline/DeepSAD/README.md`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/imgs/fig1.png` & `adbench-0.0.4/baseline/DeepSAD/imgs/fig1.png`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/log.txt` & `adbench-0.0.4/baseline/DeepSAD/log.txt`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/results.json` & `adbench-0.0.4/baseline/DeepSAD/results.json`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/base/base_dataset.py` & `adbench-0.0.4/baseline/DeepSAD/src/base/base_dataset.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/base/base_net.py` & `adbench-0.0.4/baseline/DeepSAD/src/base/base_net.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/base/base_trainer.py` & `adbench-0.0.4/baseline/DeepSAD/src/base/base_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/base/odds_dataset.py` & `adbench-0.0.4/baseline/DeepSAD/src/base/odds_dataset.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/base/torchvision_dataset.py` & `adbench-0.0.4/baseline/DeepSAD/src/base/torchvision_dataset.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baseline_SemiDGM.py` & `adbench-0.0.4/baseline/DeepSAD/src/baseline_SemiDGM.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baseline_isoforest.py` & `adbench-0.0.4/baseline/DeepSAD/src/baseline_isoforest.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baseline_kde.py` & `adbench-0.0.4/baseline/DeepSAD/src/baseline_kde.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baseline_ocsvm.py` & `adbench-0.0.4/baseline/DeepSAD/src/baseline_ocsvm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baseline_ssad.py` & `adbench-0.0.4/baseline/DeepSAD/src/baseline_ssad.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baselines/SemiDGM.py` & `adbench-0.0.4/baseline/DeepSAD/src/baselines/SemiDGM.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baselines/isoforest.py` & `adbench-0.0.4/baseline/DeepSAD/src/baselines/isoforest.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baselines/kde.py` & `adbench-0.0.4/baseline/DeepSAD/src/baselines/kde.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baselines/ocsvm.py` & `adbench-0.0.4/baseline/DeepSAD/src/baselines/ocsvm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py` & `adbench-0.0.4/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/baselines/ssad.py` & `adbench-0.0.4/baseline/DeepSAD/src/baselines/ssad.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/datasets/cifar10.py` & `adbench-0.0.4/baseline/DeepSAD/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/datasets/fmnist.py` & `adbench-0.0.4/baseline/DeepSAD/src/datasets/fmnist.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/datasets/mnist.py` & `adbench-0.0.4/baseline/DeepSAD/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/datasets/odds.py` & `adbench-0.0.4/baseline/DeepSAD/src/datasets/odds.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/datasets/preprocessing.py` & `adbench-0.0.4/baseline/DeepSAD/src/datasets/preprocessing.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/deepsad.py` & `adbench-0.0.4/baseline/DeepSAD/src/deepsad.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/__init__.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/cifar10_LeNet.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/cifar10_LeNet.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/dgm.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/dgm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/fmnist_LeNet.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/fmnist_LeNet.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/inference/distributions.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/inference/distributions.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/layers/standard.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/layers/standard.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/layers/stochastic.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/layers/stochastic.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/main.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/main.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/mlp.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/mnist_LeNet.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/mnist_LeNet.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/networks/vae.py` & `adbench-0.0.4/baseline/DeepSAD/src/networks/vae.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/optim/DeepSAD_trainer.py` & `adbench-0.0.4/baseline/DeepSAD/src/optim/DeepSAD_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/optim/SemiDGM_trainer.py` & `adbench-0.0.4/baseline/DeepSAD/src/optim/SemiDGM_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/optim/ae_trainer.py` & `adbench-0.0.4/baseline/DeepSAD/src/optim/ae_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/optim/vae_trainer.py` & `adbench-0.0.4/baseline/DeepSAD/src/optim/vae_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/optim/variational.py` & `adbench-0.0.4/baseline/DeepSAD/src/optim/variational.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/run.py` & `adbench-0.0.4/baseline/DeepSAD/src/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/utils/config.py` & `adbench-0.0.4/baseline/DeepSAD/src/utils/config.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/utils/misc.py` & `adbench-0.0.4/baseline/DeepSAD/src/utils/misc.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py` & `adbench-0.0.4/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DevNet/run.py` & `adbench-0.0.4/baseline/DevNet/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/DevNet/utils.py` & `adbench-0.0.4/baseline/DevNet/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/FEAWAD/run.py` & `adbench-0.0.4/baseline/FEAWAD/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/FEAWAD/toolsdev.py` & `adbench-0.0.4/baseline/FEAWAD/toolsdev.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/FTTransformer/run.py` & `adbench-0.0.4/baseline/FTTransformer/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/GANomaly/fit.py` & `adbench-0.0.4/baseline/GANomaly/fit.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/GANomaly/model.py` & `adbench-0.0.4/baseline/GANomaly/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/GANomaly/run.py` & `adbench-0.0.4/baseline/GANomaly/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/PReNet/fit.py` & `adbench-0.0.4/baseline/PReNet/fit.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/PReNet/model.py` & `adbench-0.0.4/baseline/PReNet/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/PReNet/run.py` & `adbench-0.0.4/baseline/PReNet/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/PReNet/utils.py` & `adbench-0.0.4/baseline/PReNet/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/PyOD.py` & `adbench-0.0.4/baseline/PyOD.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/REPEN/model.py` & `adbench-0.0.4/baseline/REPEN/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/REPEN/run.py` & `adbench-0.0.4/baseline/REPEN/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/REPEN/utils.py` & `adbench-0.0.4/baseline/REPEN/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/baseline/Supervised.py` & `adbench-0.0.4/baseline/Supervised.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/demo.ipynb` & `adbench-0.0.4/demo.ipynb`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/figs/ADBench.png` & `adbench-0.0.4/figs/ADBench.png`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/figs/ADBenchV2.png` & `adbench-0.0.4/figs/ADBenchV2.png`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/figs/Algorithms.png` & `adbench-0.0.4/figs/Algorithms.png`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/figs/MNIST-C.png` & `adbench-0.0.4/figs/MNIST-C.png`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/figs/MVTec-AD(ViT).png` & `adbench-0.0.4/figs/MVTec-AD(ViT).png`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/figs/MVTec-AD.png` & `adbench-0.0.4/figs/MVTec-AD.png`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/other_utils/gmm/LICENSE.md` & `adbench-0.0.4/other_utils/gmm/LICENSE.md`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/other_utils/gmm/README.md` & `adbench-0.0.4/other_utils/gmm/README.md`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/other_utils/gmm/example.png` & `adbench-0.0.4/other_utils/gmm/example.png`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/other_utils/gmm/example.py` & `adbench-0.0.4/other_utils/gmm/example.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/other_utils/gmm/gmm.py` & `adbench-0.0.4/other_utils/gmm/gmm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/other_utils/gmm/test.py` & `adbench-0.0.4/other_utils/gmm/test.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/other_utils/gmm/utils.py` & `adbench-0.0.4/other_utils/gmm/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/other_utils/utils.py` & `adbench-0.0.4/other_utils/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.3/setup.py` & `adbench-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # read the contents of requirements.txt
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'requirements.txt'), encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 # 配置
 setup(
     name="adbench",
-    version='0.0.3',
+    version='0.0.4',
     author="Minqi Jiang",
     author_email="<jiangmq95@163.com>",
     url='https://github.com/Minqi824/ADBench',
     description='Python package of ADBench',
     long_description='Python package of ADBench: Anomaly detection benchmark. Fast implementation of the large '
                      'experiments in ADBench and your customized AD algorithm.',
     packages=find_packages(),
```

