# Comparing `tmp/py-feat-0.5.1.tar.gz` & `tmp/py-feat-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-feat-0.5.1.tar", last modified: Mon Feb  6 17:54:58 2023, max compression
+gzip compressed data, was "py-feat-0.6.0.tar", last modified: Mon Jul 10 22:59:54 2023, max compression
```

## Comparing `py-feat-0.5.1.tar` & `py-feat-0.6.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.352265 py-feat-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-02-06 17:54:49.000000 py-feat-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-06 17:54:49.000000 py-feat-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-06 17:54:58.352265 py-feat-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-02-06 17:54:49.000000 py-feat-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.332265 py-feat-0.5.1/feat/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.332265 py-feat-0.5.1/feat/au_detectors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.332265 py-feat-0.5.1/feat/au_detectors/StatLearning/
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/au_detectors/StatLearning/SL_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/au_detectors/StatLearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/au_detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78424 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    48013 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.332265 py-feat-0.5.1/feat/emo_detectors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.332265 py-feat-0.5.1/feat/emo_detectors/ResMaskNet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/emo_detectors/ResMaskNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26003 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/emo_detectors/ResMaskNet/resmasknet_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.332265 py-feat-0.5.1/feat/emo_detectors/StatLearning/
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/emo_detectors/StatLearning/EmoSL_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/emo_detectors/StatLearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/emo_detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.336265 py-feat-0.5.1/feat/face_detectors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.336265 py-feat-0.5.1/feat/face_detectors/FaceBoxes/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/FaceBoxes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/FaceBoxes/FaceBoxes_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/FaceBoxes/FaceBoxes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/FaceBoxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/FaceBoxes/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/LICENSE.MIT
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.336265 py-feat-0.5.1/feat/face_detectors/MTCNN/
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/MTCNN/MTCNN_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/MTCNN/MTCNN_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/MTCNN/MTCNN_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/MTCNN/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.336265 py-feat-0.5.1/feat/face_detectors/Retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/Retinaface/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/Retinaface/Retinaface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/Retinaface/Retinaface_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/Retinaface/Retinaface_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/Retinaface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/face_detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.336265 py-feat-0.5.1/feat/facepose_detectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.336265 py-feat-0.5.1/feat/facepose_detectors/img2pose/
--rw-r--r--   0 runner    (1001) docker     (123)    19751 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.336265 py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/generalized_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/image_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/pose_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18111 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/rpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/img2pose_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/facepose_detectors/img2pose/img2pose_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.340265 py-feat-0.5.1/feat/landmark_detectors/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/landmark_detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/landmark_detectors/basenet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/landmark_detectors/mobilefacenet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/landmark_detectors/pfld_compressed_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    43447 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.340265 py-feat-0.5.1/feat/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/resources/model_list.json
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/resources/neutral_face_coordinates.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.340265 py-feat-0.5.1/feat/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.352265 py-feat-0.5.1/feat/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    26683 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/0-f1-su-ph.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/0-f15-hao-ph.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   116632 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/001.csv
--rw-r--r--   0 runner    (1001) docker     (123)    81836 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/002.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21827 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/15-f13-anc-ph.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/45-m7-di-ph.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1332266 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/BWPictureHuman.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/Feat_Test.csv
--rw-r--r--   0 runner    (1001) docker     (123)   335067 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/OpenFace_Test.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1632292 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/WolfgangLanger_Pexels.mp4
--rw-r--r--   0 runner    (1001) docker     (123)  1324450 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/face_noface.mov
--rw-r--r--   0 runner    (1001) docker     (123)    69304 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/free-mountain-vector-01.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   332457 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/iMotions_Test_v5.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)   229168 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/iMotions_Test_v6.txt
--rw-r--r--   0 runner    (1001) docker     (123)   138794 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/multi_face.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   181553 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/no_face.mp4
--rw-r--r--   0 runner    (1001) docker     (123)  2675494 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/noface_face.mov
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/sample_affectiva-api-app_output.json
--rw-r--r--   0 runner    (1001) docker     (123)    81485 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/single_face.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   208428 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/data/single_face.mp4
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/test_detector_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/test_image_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/test_pretrained_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.352265 py-feat-0.5.1/feat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37335 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/utils/image_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-06 17:54:49.000000 py-feat-0.5.1/feat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:58.352265 py-feat-0.5.1/py_feat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-06 17:54:58.000000 py-feat-0.5.1/py_feat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-02-06 17:54:58.000000 py-feat-0.5.1/py_feat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 17:54:58.000000 py-feat-0.5.1/py_feat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 17:54:58.000000 py-feat-0.5.1/py_feat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-06 17:54:58.000000 py-feat-0.5.1/py_feat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-06 17:54:58.000000 py-feat-0.5.1/py_feat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-06 17:54:49.000000 py-feat-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-06 17:54:58.352265 py-feat-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-06 17:54:49.000000 py-feat-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.478644 py-feat-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-10 22:59:45.000000 py-feat-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-10 22:59:45.000000 py-feat-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-10 22:59:54.478644 py-feat-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-10 22:59:45.000000 py-feat-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.458643 py-feat-0.6.0/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.458643 py-feat-0.6.0/feat/au_detectors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.458643 py-feat-0.6.0/feat/au_detectors/StatLearning/
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/au_detectors/StatLearning/SL_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/au_detectors/StatLearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/au_detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80053 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48524 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.458643 py-feat-0.6.0/feat/emo_detectors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.458643 py-feat-0.6.0/feat/emo_detectors/ResMaskNet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/emo_detectors/ResMaskNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26003 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/emo_detectors/ResMaskNet/resmasknet_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.458643 py-feat-0.6.0/feat/emo_detectors/StatLearning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/emo_detectors/StatLearning/EmoSL_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/emo_detectors/StatLearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/emo_detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.458643 py-feat-0.6.0/feat/face_detectors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.462643 py-feat-0.6.0/feat/face_detectors/FaceBoxes/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/FaceBoxes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/FaceBoxes/FaceBoxes_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/FaceBoxes/FaceBoxes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/FaceBoxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/FaceBoxes/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/LICENSE.MIT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.462643 py-feat-0.6.0/feat/face_detectors/MTCNN/
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/MTCNN/MTCNN_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/MTCNN/MTCNN_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/MTCNN/MTCNN_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/MTCNN/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.462643 py-feat-0.6.0/feat/face_detectors/Retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/Retinaface/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/Retinaface/Retinaface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/Retinaface/Retinaface_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/Retinaface/Retinaface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/Retinaface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/face_detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.462643 py-feat-0.6.0/feat/facepose_detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.462643 py-feat-0.6.0/feat/facepose_detectors/img2pose/
+-rw-r--r--   0 runner    (1001) docker     (123)    19751 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.462643 py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/generalized_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/image_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/pose_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18111 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/rpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/img2pose_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/facepose_detectors/img2pose/img2pose_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.462643 py-feat-0.6.0/feat/landmark_detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/landmark_detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/landmark_detectors/basenet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/landmark_detectors/mobilefacenet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/landmark_detectors/pfld_compressed_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43447 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.466643 py-feat-0.6.0/feat/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/resources/model_list.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/resources/neutral_face_coordinates.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.466643 py-feat-0.6.0/feat/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.478644 py-feat-0.6.0/feat/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    26683 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/0-f1-su-ph.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/0-f15-hao-ph.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   116632 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/001.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    81836 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/002.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21827 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/15-f13-anc-ph.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/45-m7-di-ph.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1332266 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/BWPictureHuman.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/Feat_Test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   335067 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/OpenFace_Test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1632292 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/WolfgangLanger_Pexels.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)  1324450 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/face_noface.mov
+-rw-r--r--   0 runner    (1001) docker     (123)    69304 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/free-mountain-vector-01.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   332457 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/iMotions_Test_v5.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)   229168 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/iMotions_Test_v6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   138794 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/multi_face.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   181553 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/no_face.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)  2675494 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/noface_face.mov
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/sample_affectiva-api-app_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    81485 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/single_face.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   208428 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/data/single_face.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/test_detector_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/test_image_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/test_pretrained_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.478644 py-feat-0.6.0/feat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37335 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/utils/image_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 22:59:45.000000 py-feat-0.6.0/feat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:59:54.478644 py-feat-0.6.0/py_feat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-10 22:59:54.000000 py-feat-0.6.0/py_feat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-10 22:59:54.000000 py-feat-0.6.0/py_feat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:59:54.000000 py-feat-0.6.0/py_feat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:59:54.000000 py-feat-0.6.0/py_feat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-10 22:59:54.000000 py-feat-0.6.0/py_feat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 22:59:54.000000 py-feat-0.6.0/py_feat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-10 22:59:45.000000 py-feat-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-10 22:59:54.482645 py-feat-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-10 22:59:45.000000 py-feat-0.6.0/setup.py
```

### Comparing `py-feat-0.5.1/LICENSE` & `py-feat-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/PKG-INFO` & `py-feat-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-feat
-Version: 0.5.1
+Version: 0.6.0
 Summary: Facial Expression Analysis Toolbox
 Home-page: https://github.com/cosanlab/py-feat
 Author: Jin Hyun Cheong, Tiankang Xie, Sophie Byrne, Eshin Jolly, Luke Chang
 Author-email: jcheong0428@gmail.com, eshin.jolly@gmail.com
 License: MIT license
 Keywords: feat,face,facial expression,emotion
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-feat-0.5.1/README.md` & `py-feat-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/data.py` & `py-feat-0.6.0/feat/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 import matplotlib.pyplot as plt
 from matplotlib.patches import Rectangle
 import seaborn as sns
 from textwrap import wrap
 import torch
 from PIL import Image
 import logging
+import av
+from itertools import islice
 
 __all__ = [
     "FexSeries",
     "Fex",
     "ImageDataset",
     "VideoDataset",
     "_inverse_face_transform",
@@ -660,15 +662,14 @@
         """
         attr_list = []
         for name in self._metadata:
             attr_list.append(name + ": " + str(getattr(self, name, None)) + "\n")
         print(f"{self.__class__}\n" + "".join(attr_list))
 
     def _update_extracted_colnames(self, prefix=None, mode="replace"):
-
         cols2update = [
             "au_columns",
             "emotion_columns",
             "facebox_columns",
             "landmark_columns",
             "facepose_columns",
             # "gaze_columns", # doesn't currently exist
@@ -701,15 +702,14 @@
             if i == 0:
                 update = new_vals
             else:
                 update = [current + new for current, new in zip(current_vals, new_vals)]
             _ = [setattr(self, col, val) for col, val in zip(cols2update, update)]
 
     def _parse_features_labels(self, X, y):
-
         feature_groups = [
             "sessions",
             "emotions",
             "aus",
             "poses",
             "landmarks",
             "faceboxes",
@@ -1608,15 +1608,14 @@
                 out.columns = colnames
                 feats = pd.concat([feats, out], axis=1)
         return self.__class__(
             feats, sampling_freq=self.sampling_freq, features=self.features
         )
 
     def _prepare_plot_aus(self, row, muscles, gaze):
-
         """
         Plot one or more faces based on their AU representation. This method is just a
         convenient wrapper for feat.plotting.plot_face. See that function for additional
         plotting args and kwargs.
 
         Args:
             force_separate_plot_per_detection (bool, optional): Whether to create a new
@@ -1719,18 +1718,16 @@
                 au_ax = f.add_subplot(spec[0, col_count])
                 col_count += 1
             if emotion_barplot:
                 emo_ax = f.add_subplot(spec[0, col_count])
                 col_count += 1
 
             for _, row in plot_data.iterrows():
-
                 # DRAW LANDMARKS ON IMAGE OR AU FACE
                 if face_ax is not None:
-
                     facebox = row[self.facebox_columns].values
 
                     if not faces == "aus" and plot_original_image:
                         file_extension = os.path.basename(row["input"]).split(".")[-1]
                         if file_extension.lower() in [
                             "jpg",
                             "jpeg",
@@ -1906,15 +1903,14 @@
         self.preserve_aspect_ratio = preserve_aspect_ratio
         self.padding = padding
 
     def __len__(self):
         return len(self.images)
 
     def __getitem__(self, idx):
-
         # Dimensions are [channels, height, width]
         try:
             img = read_image(self.images[idx])
         except Exception:
             img = Image.open(self.images[idx])
             img = transforms.PILToTensor()(img)
 
@@ -2084,15 +2080,14 @@
         ]
         return df
 
     def __len__(self):
         return self.main_file.shape[0]
 
     def __getitem__(self, idx):
-
         # Dimensions are [channels, height, width]
         img = read_image(self.main_file["image_path"].iloc[idx])
         label = self.main_file.loc[idx, self.avail_AUs].to_numpy().astype(np.int16)
 
         if self.output_size is not None:
             logging.info(
                 f"imageLoader_DISFAPlus: RESCALING WARNING: from {img.shape} to output_size={self.output_size}"
@@ -2160,55 +2155,105 @@
         skip_frames (int): number of frames to skip
 
     Returns:
         Dataset: dataset of [batch, channels, height, width] that can be passed to DataLoader
     """
 
     def __init__(self, video_file, skip_frames=None, output_size=None):
-
-        # Ignore UserWarning: The pts_unit 'pts' gives wrong results. Please use
-        # pts_unit 'sec'. See why it's ok in this issue:
-        # https://github.com/pytorch/vision/issues/1931
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore", UserWarning)
-            # Video dimensions are: [time, height, width, channels]
-            self.video, self.audio, self.info = read_video(video_file)
-        # Swap them to match output of read_image: [time, channels, height, width]
-        # Otherwise detectors face on tensor dimension mismatch
-        self.video = swapaxes(swapaxes(self.video, 1, 3), -1, -2)
         self.file_name = video_file
+        self.skip_frames = skip_frames
         self.output_size = output_size
+        self.get_video_metadata(video_file)
+        # This is the list of frame ids used to slice the video not video_frames
         self.video_frames = np.arange(
-            0, self.video.shape[0], 1 if skip_frames is None else skip_frames
+            0, self.metadata["num_frames"], 1 if skip_frames is None else skip_frames
         )
-        self.video = self.video[self.video_frames, :, :]
 
     def __len__(self):
-        return self.video.shape[0]
+        # Number of frames respective skip_frames
+        return len(self.video_frames)
 
     def __getitem__(self, idx):
+        # Get the frame data and frame number respective skip_frames
+        frame_data, frame_idx = self.load_frame(idx)
+
+        # Swap frame dims to match output of read_image: [time, channels, height, width]
+        # Otherwise detectors face on tensor dimension mismatch
+        frame_data = swapaxes(swapaxes(frame_data, 0, -1), 1, 2)
 
         # Rescale if needed like in ImageDataset
         if self.output_size is not None:
             logging.info(
-                f"VideoDataset: RESCALING WARNING: from {self.video[idx].shape} to output_size={self.output_size}"
+                f"VideoDataset: RESCALING WARNING: from {self.metadata['shape']} to output_size={self.output_size}"
             )
             transform = Compose(
                 [Rescale(self.output_size, preserve_aspect_ratio=True, padding=False)]
             )
-            transformed_img = transform(self.video[idx])
+            transformed_frame_data = transform(frame_data)
 
             return {
-                "Image": transformed_img["Image"],
-                "Frame": self.video_frames[idx],
-                "Scale": transformed_img["Scale"],
-                "Padding": transformed_img["Padding"],
+                "Image": transformed_frame_data["Image"],
+                "Frame": frame_idx,
                 "FileName": self.file_name,
+                "Scale": transformed_frame_data["Scale"],
+                "Padding": transformed_frame_data["Padding"],
             }
         else:
             return {
-                "Image": self.video[idx],
-                "Frame": self.video_frames[idx],
+                "Image": frame_data,
+                "Frame": frame_idx,
                 "FileName": self.file_name,
                 "Scale": 1.0,
                 "Padding": {"Left": 0, "Top": 0, "Right": 0, "Bottom": 0},
             }
+
+    def get_video_metadata(self, video_file):
+        container = av.open(video_file)
+        stream = container.streams.video[0]
+        fps = stream.average_rate
+        height = stream.height
+        width = stream.width
+        num_frames = stream.frames
+        container.close()
+        self.metadata = {
+            "fps": float(fps),
+            "fps_frac": fps,
+            "height": height,
+            "width": width,
+            "num_frames": num_frames,
+            "shape": (height, width),
+        }
+
+    def load_frame(self, idx):
+        """Load in a single frame from the video using a lazy generator"""
+
+        # Get frame number respecting skip_frames
+        frame_idx = int(self.video_frames[idx])
+
+        # Use a py-av generator to load in just this frame
+        container = av.open(self.file_name)
+        stream = container.streams.video[0]
+        frame = next(islice(container.decode(stream), frame_idx, None))
+        frame_data = torch.from_numpy(frame.to_ndarray(format="rgb24"))
+        container.close()
+
+        return frame_data, frame_idx
+
+    def calc_approx_frame_time(self, idx):
+        """Calculate the approximate time of a frame in a video
+
+        Args:
+            frame_idx (int): frame number
+
+        Returns:
+            float: time in seconds
+        """
+        frame_time = idx / self.metadata["fps"]
+        total_time = self.metadata["num_frames"] / self.metadata["fps"]
+        time = total_time if idx >= self.metadata["num_frames"] else frame_time
+        return self.convert_sec_to_min_sec(time)
+
+    @staticmethod
+    def convert_sec_to_min_sec(duration):
+        minutes = int(duration // 60)
+        seconds = int(duration % 60)
+        return f"{minutes:02d}:{seconds:02d}"
```

### Comparing `py-feat-0.5.1/feat/detector.py` & `py-feat-0.6.0/feat/detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,14 @@
         frame = convert_image_to_tensor(frame)
 
         if is_list_of_lists_empty(detected_faces):
             list_concat = detected_faces
         else:
             if self.info["landmark_model"]:
                 if self.info["landmark_model"].lower() == "mobilenet":
-
                     out_size = 224
                 else:
                     out_size = 112
 
             extracted_faces, new_bbox = extract_face_from_bbox(
                 frame, detected_faces, face_size=out_size
             )
@@ -455,15 +454,14 @@
                     .data.numpy()
                 )
 
             landmark = landmark.reshape(landmark.shape[0], -1, 2)
 
             landmark_results = []
             for ik in range(landmark.shape[0]):
-
                 landmark_results.append(
                     new_bbox[ik].inverse_transform_landmark(landmark[ik, :, :])
                 )
 
             length_index = [len(x) for x in detected_faces]
             new_lens = np.insert(np.cumsum(length_index), 0, 0)
             list_concat = []
@@ -570,15 +568,15 @@
                         frame=frames[i],
                         landmarks=frame_landmark[j],
                         face_size=112,
                     )
 
                     hog_features.append(
                         hog(
-                            transforms.ToPILImage()(convex_hull[0]),
+                            transforms.ToPILImage()(convex_hull[0] / 255.0),
                             orientations=8,
                             pixels_per_cell=(8, 8),
                             cells_per_block=(2, 2),
                             visualize=False,
                             channel_axis=-1,
                         ).reshape(1, -1)
                     )
@@ -653,14 +651,15 @@
         batch_data,
         face_detection_threshold,
         face_model_kwargs,
         landmark_model_kwargs,
         facepose_model_kwargs,
         emotion_model_kwargs,
         au_model_kwargs,
+        suppress_torchvision_warnings=True,
     ):
         """
         Main detection "waterfall." Calls each individual detector in the sequence
         required to support any interactions between detections. Called
         behind-the-scenes by .detect_image() and .detect_video()
 
         Args:
@@ -671,14 +670,23 @@
             facepose_model_kwargs (dict): facepose model kwargs
             emotion_model_kwargs (dict): emotion model kwargs
             au_model_kwargs (dict): au model kwargs
 
         Returns:
             tuple: faces, landmarks, poses, aus, emotions
         """
+
+        # Reset warnings
+        warnings.filterwarnings("default", category=UserWarning, module="torchvision")
+
+        if suppress_torchvision_warnings:
+            warnings.filterwarnings(
+                "ignore", category=UserWarning, module="torchvision"
+            )
+
         faces = self.detect_faces(
             batch_data["Image"],
             threshold=face_detection_threshold,
             **face_model_kwargs,
         )
 
         landmarks = self.detect_landmarks(
@@ -767,15 +775,14 @@
                 "Currently using mobilenet for landmark detection with batch_size > 1 may lead to erroneous detections. We recommend either setting batch_size=1 or using mobilefacenet as the landmark detection model. You can follow this issue for more: https://github.com/cosanlab/py-feat/issues/151"
             )
 
         try:
             batch_output = []
 
             for batch_id, batch_data in enumerate(tqdm(data_loader)):
-
                 faces, landmarks, poses, aus, emotions = self._run_detection_waterfall(
                     batch_data,
                     face_detection_threshold,
                     face_model_kwargs,
                     landmark_model_kwargs,
                     facepose_model_kwargs,
                     emotion_model_kwargs,
@@ -836,26 +843,29 @@
         # Keyword arguments than can be passed to the underlying models
         face_model_kwargs = kwargs.pop("face_model_kwargs", dict())
         landmark_model_kwargs = kwargs.pop("landmark_model_kwargs", dict())
         au_model_kwargs = kwargs.pop("au_model_kwargs", dict())
         emotion_model_kwargs = kwargs.pop("emotion_model_kwargs", dict())
         facepose_model_kwargs = kwargs.pop("facepose_model_kwargs", dict())
 
+        dataset = VideoDataset(
+            video_path, skip_frames=skip_frames, output_size=output_size
+        )
+
         data_loader = DataLoader(
-            VideoDataset(video_path, skip_frames=skip_frames, output_size=output_size),
+            dataset,
             num_workers=num_workers,
             batch_size=batch_size,
             pin_memory=pin_memory,
             shuffle=False,
         )
 
         batch_output = []
 
         for batch_data in tqdm(data_loader):
-
             faces, landmarks, poses, aus, emotions = self._run_detection_waterfall(
                 batch_data,
                 face_detection_threshold,
                 face_model_kwargs,
                 landmark_model_kwargs,
                 facepose_model_kwargs,
                 emotion_model_kwargs,
@@ -874,14 +884,17 @@
                 frames,
             )
 
             batch_output.append(output)
 
         batch_output = pd.concat(batch_output)
         batch_output.reset_index(drop=True, inplace=True)
+        batch_output["approx_time"] = [
+            dataset.calc_approx_frame_time(x) for x in batch_output["frame"].to_numpy()
+        ]
         return batch_output.set_index("frame", drop=False)
 
     def _create_fex(
         self, faces, landmarks, poses, aus, emotions, file_names, frame_counter
     ):
         """Helper function to create a Fex instance using detector output
 
@@ -1080,15 +1093,14 @@
             )
 
         if is_list_of_lists_empty(faces):
             # Currently assuming no faces if no face is detected. Not running pose
             return (faces, poses)
 
         else:
-
             overlap_faces = []
             overlap_poses = []
             for frame_face, frame_face_pose, frame_pose in zip(
                 faces, faces_pose, poses
             ):
                 if not frame_face:
                     n_faces = 0
```

### Comparing `py-feat-0.5.1/feat/emo_detectors/ResMaskNet/resmasknet_test.py` & `py-feat-0.6.0/feat/emo_detectors/ResMaskNet/resmasknet_test.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/emo_detectors/StatLearning/EmoSL_test.py` & `py-feat-0.6.0/feat/emo_detectors/StatLearning/EmoSL_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,21 +20,21 @@
     clf = pickle.load(open(cf_path, "rb"))
     return clf
 
 
 class EmoSVMClassifier:
     def __init__(self, **kwargs) -> None:
         self.pca_model = load_classifier(
-            os.path.join(get_resource_path(), "emo_hog_pca.joblib")
+            os.path.join(get_resource_path(), "emo_data_Fullpca_Jun30.pkl")
         )
         self.classifier = load_classifier(
-            os.path.join(get_resource_path(), "emoSVM38.joblib")
+            os.path.join(get_resource_path(), "July4_emo_SVM.pkl")
         )
         self.scaler = load_classifier(
-            os.path.join(get_resource_path(), "emo_hog_scalar.joblib")
+            os.path.join(get_resource_path(), "emo_data_Fullscalar_Jun30.pkl")
         )
 
     def detect_emo(self, frame, landmarks, **kwargs):
         """
         Note that here frame is represented by hogs
         """
         # landmarks = np.array(landmarks)
@@ -43,15 +43,17 @@
         landmarks = np.concatenate(landmarks)
         landmarks = landmarks.reshape(-1, landmarks.shape[1] * landmarks.shape[2])
 
         pca_transformed_frame = self.pca_model.transform(
             self.scaler.fit_transform(frame)
         )
         feature_cbd = np.concatenate((pca_transformed_frame, landmarks), 1)
+        emo_columns = ["anger", "disgust", "fear", "happ", "sad", "sur", "neutral"]
+
         pred_emo = []
-        for keys in self.classifier:
+        for keys in emo_columns:
             emo_pred = self.classifier[keys].predict(feature_cbd)
             emo_pred = emo_pred  # probably need to delete this
             pred_emo.append(emo_pred)
 
         pred_emos = np.array(pred_emo).T
         return pred_emos
```

### Comparing `py-feat-0.5.1/feat/face_detectors/FaceBoxes/FaceBoxes_model.py` & `py-feat-0.6.0/feat/face_detectors/FaceBoxes/FaceBoxes_model.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/FaceBoxes/FaceBoxes_test.py` & `py-feat-0.6.0/feat/face_detectors/FaceBoxes/FaceBoxes_test.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/FaceBoxes/readme.md` & `py-feat-0.6.0/feat/face_detectors/FaceBoxes/readme.md`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/LICENSE.MIT` & `py-feat-0.6.0/feat/face_detectors/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/MTCNN/MTCNN_model.py` & `py-feat-0.6.0/feat/face_detectors/MTCNN/MTCNN_model.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/MTCNN/MTCNN_test.py` & `py-feat-0.6.0/feat/face_detectors/MTCNN/MTCNN_test.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/MTCNN/MTCNN_utils.py` & `py-feat-0.6.0/feat/face_detectors/MTCNN/MTCNN_utils.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/Retinaface/LICENSE.MIT` & `py-feat-0.6.0/feat/face_detectors/Retinaface/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/Retinaface/Retinaface_model.py` & `py-feat-0.6.0/feat/face_detectors/Retinaface/Retinaface_model.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/Retinaface/Retinaface_test.py` & `py-feat-0.6.0/feat/face_detectors/Retinaface/Retinaface_test.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/face_detectors/Retinaface/Retinaface_utils.py` & `py-feat-0.6.0/feat/face_detectors/Retinaface/Retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/facepose_detectors/img2pose/LICENSE` & `py-feat-0.6.0/feat/facepose_detectors/img2pose/LICENSE`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/generalized_rcnn.py` & `py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/generalized_rcnn.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/image_operations.py` & `py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/image_operations.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/models.py` & `py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/models.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/pose_operations.py` & `py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/pose_operations.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/facepose_detectors/img2pose/deps/rpn.py` & `py-feat-0.6.0/feat/facepose_detectors/img2pose/deps/rpn.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/facepose_detectors/img2pose/img2pose_model.py` & `py-feat-0.6.0/feat/facepose_detectors/img2pose/img2pose_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         # are deprecated since 0.13 and may be removed in the future. The current
         # behavior is equivalent to passing
         # `weights=ResNet18_Weights.IMAGENET1K_V1`. You can also use
         # `weights=ResNet18_Weights.DEFAULT` to get the most up-to-date weights.
         # create network backbone
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", UserWarning)
-            backbone = resnet_fpn_backbone(f"resnet{self.depth}", weights=True)
+            backbone = resnet_fpn_backbone(f"resnet{self.depth}", pretrained=True)
 
         if pose_mean is not None:
             pose_mean = torch.tensor(pose_mean)
             pose_stddev = torch.tensor(pose_stddev)
 
         if threed_68_points is not None:
             threed_68_points = torch.tensor(threed_68_points)
```

### Comparing `py-feat-0.5.1/feat/facepose_detectors/img2pose/img2pose_test.py` & `py-feat-0.6.0/feat/facepose_detectors/img2pose/img2pose_test.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/landmark_detectors/basenet_test.py` & `py-feat-0.6.0/feat/landmark_detectors/basenet_test.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/landmark_detectors/mobilefacenet_test.py` & `py-feat-0.6.0/feat/landmark_detectors/mobilefacenet_test.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/landmark_detectors/pfld_compressed_test.py` & `py-feat-0.6.0/feat/landmark_detectors/pfld_compressed_test.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/plotting.py` & `py-feat-0.6.0/feat/plotting.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/pretrained.py` & `py-feat-0.6.0/feat/pretrained.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,15 +160,29 @@
                     verbose=verbose,
                 )
                 download_url(
                     model_urls["au_detectors"]["hog-pca"]["urls"][2],
                     get_resource_path(),
                     verbose=verbose,
                 )
-
+                download_url(
+                    model_urls["au_detectors"]["hog-pca"]["urls"][3],
+                    get_resource_path(),
+                    verbose=verbose,
+                )
+                download_url(
+                    model_urls["au_detectors"]["hog-pca"]["urls"][4],
+                    get_resource_path(),
+                    verbose=verbose,
+                )
+                download_url(
+                    model_urls["au_detectors"]["hog-pca"]["urls"][5],
+                    get_resource_path(),
+                    verbose=verbose,
+                )
     # Emotion model
     if emotion_model is None:
         raise ValueError(
             f"emotion_model must be one of {[list(e.keys())[0] for e in PRETRAINED_MODELS['emotion_model']]}"
         )
     else:
         emotion_model = emotion_model.lower()
```

### Comparing `py-feat-0.5.1/feat/resources/model_list.json` & `py-feat-0.6.0/feat/resources/model_list.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9635416666666666%*

 * *Differences: {"'au_detectors'": "{'svm': {'urls': "*

 * *                   "['https://github.com/cosanlab/py-feat/releases/download/v0.1/svm_60_July2023.pkl']}, "*

 * *                   "'xgb': {'urls': "*

 * *                   "['https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU1_XGB.ubj', "*

 * *                   "'https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU2_XGB.ubj', "*

 * *                   "'https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU4_XGB.ubj', "*

 * *                   "' […]*

```diff
@@ -1,66 +1,69 @@
 {
     "au_detectors": {
         "hog-pca": {
             "urls": [
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/upper_face_pcaSet.pkl",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/lower_face_pcaSet.pkl",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/full_face_pcaSet.pkl"
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/all_data_Upperpca_June30.pkl",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/all_data_Upperscalar_June30.pkl",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/all_data_Lowerpca_June30.pkl",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/all_data_Lowerscalar_June30.pkl",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/all_data_Fullpca_June30.pkl",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/all_data_Fullscalar_June30.pkl"
             ]
         },
         "svm": {
             "urls": [
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/svm_60_Nov22022.pkl"
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/svm_60_July2023.pkl"
             ]
         },
         "xgb": {
             "urls": [
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU1.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU2.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU4.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU5.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU6.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU7.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU9.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU10.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU11.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU12.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU14.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU15.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU17.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU20.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU23.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU24.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU25.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU26.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU28.ubj",
-                "https://github.com/cosanlab/py-feat/releases/download/v0.1/Oct30FinalXGB_AU43.ubj"
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU1_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU2_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU4_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU5_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU6_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU7_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU9_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU10_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU11_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU12_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU14_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU15_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU17_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU20_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU23_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU24_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU25_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU26_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU28_XGB.ubj",
+                "https://github.com/cosanlab/py-feat/releases/download/v0.1/July4_AU43_XGB.ubj"
             ]
         }
     },
     "emotion_detectors": {
         "emo_pca": {
             "urls": [
-                "https://github.com/cosanlab/feat/releases/download/v0.1/emo_hog_pca.joblib"
+                "https://github.com/cosanlab/feat/releases/download/v0.1/emo_data_Fullscalar_Jun30.pkl"
             ]
         },
         "emo_scalar": {
             "urls": [
-                "https://github.com/cosanlab/feat/releases/download/v0.1/emo_hog_scalar.joblib"
+                "https://github.com/cosanlab/feat/releases/download/v0.1/emo_data_Fullpca_Jun30.pkl"
             ]
         },
         "resmasknet": {
             "urls": [
                 "https://github.com/cosanlab/feat/releases/download/v0.1/ResMaskNet_Z_resmasking_dropout1_rot30.pth",
                 "https://github.com/cosanlab/py-feat/releases/download/v0.1/ResMaskNet_fer2013_config.json"
             ]
         },
         "svm": {
             "urls": [
-                "https://github.com/cosanlab/feat/releases/download/v0.1/emoSVM38.joblib"
+                "https://github.com/cosanlab/feat/releases/download/v0.1/July4_emo_SVM.pkl"
             ]
         }
     },
     "face_detectors": {
         "faceboxes": {
             "urls": [
                 "https://github.com/cosanlab/feat/releases/download/v0.1/FaceBoxesProd.pth"
```

### Comparing `py-feat-0.5.1/feat/resources/neutral_face_coordinates.csv` & `py-feat-0.6.0/feat/resources/neutral_face_coordinates.csv`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/conftest.py` & `py-feat-0.6.0/feat/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/0-f1-su-ph.jpg` & `py-feat-0.6.0/feat/tests/data/0-f1-su-ph.jpg`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/0-f15-hao-ph.jpg` & `py-feat-0.6.0/feat/tests/data/0-f15-hao-ph.jpg`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/001.csv` & `py-feat-0.6.0/feat/tests/data/001.csv`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/002.csv` & `py-feat-0.6.0/feat/tests/data/002.csv`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/15-f13-anc-ph.jpg` & `py-feat-0.6.0/feat/tests/data/15-f13-anc-ph.jpg`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/45-m7-di-ph.jpg` & `py-feat-0.6.0/feat/tests/data/45-m7-di-ph.jpg`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/BWPictureHuman.jpg` & `py-feat-0.6.0/feat/tests/data/BWPictureHuman.jpg`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/Feat_Test.csv` & `py-feat-0.6.0/feat/tests/data/Feat_Test.csv`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/OpenFace_Test.csv` & `py-feat-0.6.0/feat/tests/data/OpenFace_Test.csv`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/WolfgangLanger_Pexels.mp4` & `py-feat-0.6.0/feat/tests/data/WolfgangLanger_Pexels.mp4`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/face_noface.mov` & `py-feat-0.6.0/feat/tests/data/face_noface.mov`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/free-mountain-vector-01.jpg` & `py-feat-0.6.0/feat/tests/data/free-mountain-vector-01.jpg`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/iMotions_Test_v5.txt` & `py-feat-0.6.0/feat/tests/data/iMotions_Test_v5.txt`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/iMotions_Test_v6.txt` & `py-feat-0.6.0/feat/tests/data/iMotions_Test_v6.txt`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/multi_face.jpg` & `py-feat-0.6.0/feat/tests/data/multi_face.jpg`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/no_face.mp4` & `py-feat-0.6.0/feat/tests/data/no_face.mp4`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/noface_face.mov` & `py-feat-0.6.0/feat/tests/data/noface_face.mov`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/sample_affectiva-api-app_output.json` & `py-feat-0.6.0/feat/tests/data/sample_affectiva-api-app_output.json`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/single_face.jpg` & `py-feat-0.6.0/feat/tests/data/single_face.jpg`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/data/single_face.mp4` & `py-feat-0.6.0/feat/tests/data/single_face.mp4`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/test_data.py` & `py-feat-0.6.0/feat/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     assert all(map(hasprefix, video_means.facebox_columns))
     assert all(map(hasprefix, video_means.landmark_columns))
     assert all(map(hasprefix, video_means.facepose_columns))
     assert all(map(hasprefix, video_means.time_columns))
 
 
 def test_fex_old(imotions_data):
-
     # Dropped support in >= 0.4.0
     with pytest.raises(Exception):
         Fex().read_facet()
     with pytest.raises(Exception):
         Fex().read_affectiva()
 
     df = imotions_data
@@ -121,15 +120,16 @@
     assert dat.loc[[0], :].sampling_freq == dat.sampling_freq
     assert dat.loc[:, ["Joy"]].sampling_freq == dat.sampling_freq
 
     # Test Downsample
     assert len(dat.downsample(target=10)) == 52
 
     # Test upsample
-    assert len(dat.upsample(target=60, target_type="hz")) == (len(dat) - 1) * 2
+    # Commenting out because of a bug in nltools: https://github.com/cosanlab/nltools/issues/418
+    # assert len(dat.upsample(target=60, target_type="hz")) == (len(dat) - 1) * 2
 
     # Test interpolation
     assert (
         dat.interpolate(method="linear").isnull().sum()["Positive"]
         < dat.isnull().sum()["Positive"]
     )
     dat = dat.interpolate(method="linear")
```

### Comparing `py-feat-0.5.1/feat/tests/test_detector_core.py` & `py-feat-0.6.0/feat/tests/test_detector_core.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/test_image_ops.py` & `py-feat-0.6.0/feat/tests/test_image_ops.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/test_plot.py` & `py-feat-0.6.0/feat/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/test_pretrained_models.py` & `py-feat-0.6.0/feat/tests/test_pretrained_models.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/tests/test_utils.py` & `py-feat-0.6.0/feat/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/transforms.py` & `py-feat-0.6.0/feat/transforms.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/utils/__init__.py` & `py-feat-0.6.0/feat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/utils/image_operations.py` & `py-feat-0.6.0/feat/utils/image_operations.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/utils/io.py` & `py-feat-0.6.0/feat/utils/io.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/feat/utils/stats.py` & `py-feat-0.6.0/feat/utils/stats.py`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/py_feat.egg-info/PKG-INFO` & `py-feat-0.6.0/py_feat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-feat
-Version: 0.5.1
+Version: 0.6.0
 Summary: Facial Expression Analysis Toolbox
 Home-page: https://github.com/cosanlab/py-feat
 Author: Jin Hyun Cheong, Tiankang Xie, Sophie Byrne, Eshin Jolly, Luke Chang
 Author-email: jcheong0428@gmail.com, eshin.jolly@gmail.com
 License: MIT license
 Keywords: feat,face,facial expression,emotion
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-feat-0.5.1/py_feat.egg-info/SOURCES.txt` & `py-feat-0.6.0/py_feat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-feat-0.5.1/setup.py` & `py-feat-0.6.0/setup.py`

 * *Files identical despite different names*

