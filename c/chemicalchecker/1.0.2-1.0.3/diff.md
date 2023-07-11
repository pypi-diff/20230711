# Comparing `tmp/chemicalchecker-1.0.2.tar.gz` & `tmp/chemicalchecker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chemicalchecker-1.0.2.tar", last modified: Tue Jan 11 15:17:08 2022, max compression
+gzip compressed data, was "dist/chemicalchecker-1.0.3.tar", last modified: Tue Jul 11 15:44:14 2023, max compression
```

## Comparing `chemicalchecker-1.0.2.tar` & `chemicalchecker-1.0.3.tar`

### file list

```diff
@@ -1,293 +1,300 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      780 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     1542 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)     1061 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      432 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8022 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6873 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/
--rw-rw-rw-   0 root         (0) root         (0)     1217 2022-01-10 16:07:34.000000 chemicalchecker-1.0.2/chemicalchecker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/core/
--rw-rw-rw-   0 root         (0) root         (0)      575 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/chemicalchecker/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    34294 2021-12-28 09:53:25.000000 chemicalchecker-1.0.2/chemicalchecker/core/chemcheck.py
--rw-rw-rw-   0 root         (0) root         (0)    24112 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/chemicalchecker/core/clus.py
--rw-rw-rw-   0 root         (0) root         (0)     2927 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/core/data.py
--rw-rw-rw-   0 root         (0) root         (0)    62547 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/core/diagnostics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples/
--rw-rw-rw-   0 root         (0) root         (0)  5997712 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples/ctrp_auc.csv
--rw-rw-rw-   0 root         (0) root         (0)  6479614 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples/fps.pkl
--rw-rw-rw-   0 root         (0) root         (0)    36791 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples/pharmacodb_targets.tsv
--rw-rw-rw-   0 root         (0) root         (0)    20367 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples/toy_matrix.pkl
--rw-rw-rw-   0 root         (0) root         (0)    43320 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples/toy_pairs.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples/validation_sets/
--rw-rw-rw-   0 root         (0) root         (0)  8156424 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples/validation_sets/atc_validation.tsv
--rw-rw-rw-   0 root         (0) root         (0)  6266204 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples/validation_sets/moa_validation.tsv
--rw-rw-rw-   0 root         (0) root         (0)     9223 2021-11-19 09:59:03.000000 chemicalchecker-1.0.2/chemicalchecker/core/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2982 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/molkit.py
--rw-rw-rw-   0 root         (0) root         (0)    17783 2021-12-22 14:16:06.000000 chemicalchecker-1.0.2/chemicalchecker/core/neig.py
--rw-rw-rw-   0 root         (0) root         (0)    22716 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/core/preprocess.py
--rw-rw-rw-   0 root         (0) root         (0)    11417 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/proj.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/core/projector/
--rw-rw-rw-   0 root         (0) root         (0)      130 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/projector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14998 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/projector/default.py
--rw-rw-rw-   0 root         (0) root         (0)     5319 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/projector/pca.py
--rw-rw-rw-   0 root         (0) root         (0)     6979 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/projector/tsne.py
--rw-rw-rw-   0 root         (0) root         (0)     6922 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/projector/umap_.py
--rw-rw-rw-   0 root         (0) root         (0)    24745 2022-01-10 16:07:34.000000 chemicalchecker-1.0.2/chemicalchecker/core/sign0.py
--rw-rw-rw-   0 root         (0) root         (0)    21227 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/sign1.py
--rw-rw-rw-   0 root         (0) root         (0)    26555 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/sign2.py
--rw-rw-rw-   0 root         (0) root         (0)   110451 2021-11-29 15:18:53.000000 chemicalchecker-1.0.2/chemicalchecker/core/sign3.py
--rw-rw-rw-   0 root         (0) root         (0)    17927 2021-12-03 12:10:45.000000 chemicalchecker-1.0.2/chemicalchecker/core/sign4.py
--rw-rw-rw-   0 root         (0) root         (0)    20464 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/core/signature_base.py
--rw-rw-rw-   0 root         (0) root         (0)    33016 2021-12-03 12:10:45.000000 chemicalchecker-1.0.2/chemicalchecker/core/signature_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2140 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/core/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/database/
--rw-rw-rw-   0 root         (0) root         (0)     1207 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10146 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/database/calcdata.py
--rw-rw-rw-   0 root         (0) root         (0)     2175 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/database/database.py
--rw-rw-rw-   0 root         (0) root         (0)    19569 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/database/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    10320 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/database/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     4931 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/database/molecule.py
--rw-rw-rw-   0 root         (0) root         (0)    17859 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/database/molrepo.py
--rw-rw-rw-   0 root         (0) root         (0)     2713 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/database/pubchem.py
--rw-rw-rw-   0 root         (0) root         (0)    12314 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/database/uniprotkb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/
--rw-rw-rw-   0 root         (0) root         (0)      441 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/adanet/
--rw-rw-rw-   0 root         (0) root         (0)      207 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/adanet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25344 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/adanet/adanet_wrap.py
--rw-rw-rw-   0 root         (0) root         (0)     4527 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/adanet/cnn_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2021-12-14 12:08:56.000000 chemicalchecker-1.0.2/chemicalchecker/tool/adanet/dnn_extend_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     7315 2021-12-14 12:08:56.000000 chemicalchecker-1.0.2/chemicalchecker/tool/adanet/dnn_stack_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/autoencoder/
--rw-rw-rw-   0 root         (0) root         (0)      171 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/autoencoder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11213 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/autoencoder/autoencoder.py
--rw-rw-rw-   0 root         (0) root         (0)    13756 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/autoencoder/autoencoder_siamese.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/classifier/
--rw-rw-rw-   0 root         (0) root         (0)       92 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/classifier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/classifier/imbalanced/
--rw-rw-rw-   0 root         (0) root         (0)       34 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/classifier/imbalanced/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14447 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/classifier/imbalanced/imbalanced.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/classifier/multitask/
--rw-rw-rw-   0 root         (0) root         (0)       44 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/classifier/multitask/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10766 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/classifier/multitask/binarymultitask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/
--rw-rw-rw-   0 root         (0) root         (0)       88 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/feat/
--rw-rw-rw-   0 root         (0) root         (0)      455 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/feat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1387 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/feat/base_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    15124 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/feat/graph_features.py
--rw-rw-rw-   0 root         (0) root         (0)    15248 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/graphconv/
--rw-rw-rw-   0 root         (0) root         (0)       95 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/graphconv/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14488 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/graphconv/graph_smiles_sign.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/hotnet/
--rw-rw-rw-   0 root         (0) root         (0)      108 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/hotnet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2536 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/hotnet/hotnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/node2vec/
--rw-rw-rw-   0 root         (0) root         (0)      193 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/node2vec/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19770 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/node2vec/node2vec.py
--rw-rw-rw-   0 root         (0) root         (0)     3080 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/node2vec/word2vec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/siamese/
--rw-rw-rw-   0 root         (0) root         (0)      105 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/siamese/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11641 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/siamese/callbacks.py
--rw-rw-rw-   0 root         (0) root         (0)    17396 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/siamese/siamese.py
--rw-rw-rw-   0 root         (0) root         (0)    48456 2021-12-14 12:08:56.000000 chemicalchecker-1.0.2/chemicalchecker/tool/siamese/siamese_triplets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/smilespred/
--rw-rw-rw-   0 root         (0) root         (0)      118 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/smilespred/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6069 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/smilespred/apppred.py
--rw-rw-rw-   0 root         (0) root         (0)    11591 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/tool/smilespred/smilespred.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/
--rw-rw-rw-   0 root         (0) root         (0)       17 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23275 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/
--rw-rw-rw-   0 root         (0) root         (0)      117 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/chembl/
--rw-rw-rw-   0 root         (0) root         (0)       42 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/chembl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10771 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/chembl/fetch_chembl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/drugbank/
--rw-rw-rw-   0 root         (0) root         (0)       48 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/drugbank/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7010 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/drugbank/fetch_drugbank.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/moleculenet/
--rw-rw-rw-   0 root         (0) root         (0)       42 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/moleculenet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/moleculenet/fetch_moleculenet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/evaluation/
--rw-rw-rw-   0 root         (0) root         (0)       70 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/evaluation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14640 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/evaluation/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     1151 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/evaluation/score.py
--rw-rw-rw-   0 root         (0) root         (0)    33340 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/evaluation/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/examples/example.py
--rw-rw-rw-   0 root         (0) root         (0)    14143 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/ml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4068 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/autosklearnconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/gridconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)     4407 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/hyperoptconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)     6168 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/tpotconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/vanillaconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)     1705 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/multi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/
--rw-rw-rw-   0 root         (0) root         (0)      123 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11969 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/acp.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5286 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/cp.py
--rw-rw-rw-   0 root         (0) root         (0)    14376 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)    16054 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/icp.py
--rw-rw-rw-   0 root         (0) root         (0)    14653 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/nc.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/util.py
--rw-rw-rw-   0 root         (0) root         (0)     6026 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/run.py
--rw-rw-rw-   0 root         (0) root         (0)    18753 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/signaturizer.py
--rw-rw-rw-   0 root         (0) root         (0)    27022 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/tmsetup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/universes/
--rw-rw-rw-   0 root         (0) root         (0)       28 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/universes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16802 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/universes/univs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/
--rw-rw-rw-   0 root         (0) root         (0)       25 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3653 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/chemistry.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/conformal.py
--rw-rw-rw-   0 root         (0) root         (0)     3468 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/hpc.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/log.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2021-11-22 16:32:21.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    15028 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/pairs.py
--rw-rw-rw-   0 root         (0) root         (0)    12322 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/plots.py
--rw-rw-rw-   0 root         (0) root         (0)    16489 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/reportcard.py
--rw-rw-rw-   0 root         (0) root         (0)    20934 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/splitters.py
--rw-rw-rw-   0 root         (0) root         (0)     3174 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/topped.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/
--rw-rw-rw-   0 root         (0) root         (0)     1252 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/aggregate/
--rw-rw-rw-   0 root         (0) root         (0)       93 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/aggregate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5832 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/aggregate/aggregate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/config/
--rw-rw-rw-   0 root         (0) root         (0)     2409 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/config/cc_config.json
--rw-rw-rw-   0 root         (0) root         (0)     2009 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/config/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/decomposition/
--rw-rw-rw-   0 root         (0) root         (0)      375 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/decomposition/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2670 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/decomposition/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/decorator/
--rw-rw-rw-   0 root         (0) root         (0)      169 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/decorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27196 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/decorator/profilehooks.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/decorator/property.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/decorator/safe.py
--rw-rw-rw-   0 root         (0) root         (0)     6326 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/decorator/timeout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/download/
--rw-rw-rw-   0 root         (0) root         (0)      491 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8694 2021-12-07 12:00:13.000000 chemicalchecker-1.0.2/chemicalchecker/util/download/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/hpc/
--rw-rw-rw-   0 root         (0) root         (0)      575 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/hpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5903 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/hpc/hpc.py
--rw-rw-rw-   0 root         (0) root         (0)     6611 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/hpc/local.py
--rw-rw-rw-   0 root         (0) root         (0)    12128 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/util/hpc/sge.py
--rw-rw-rw-   0 root         (0) root         (0)    11441 2021-11-28 04:03:28.000000 chemicalchecker-1.0.2/chemicalchecker/util/hpc/slurm.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/hpc/test_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/keytype/
--rw-rw-rw-   0 root         (0) root         (0)      232 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/keytype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/keytype/detect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/logging/
--rw-rw-rw-   0 root         (0) root         (0)      434 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/util/logging/logging_conf.ini
--rw-rw-rw-   0 root         (0) root         (0)      419 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/logging/our_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/mol2svg/
--rw-rw-rw-   0 root         (0) root         (0)       52 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/mol2svg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/mol2svg/mol2svg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/network/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/network/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12686 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/network/network.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/parser/
--rw-rw-rw-   0 root         (0) root         (0)      218 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4967 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/parser/converter.py
--rw-rw-rw-   0 root         (0) root         (0)    13993 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/util/parser/data_calculator.py
--rw-rw-rw-   0 root         (0) root         (0)    34304 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/parser/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/performance/
--rw-rw-rw-   0 root         (0) root         (0)      183 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/performance/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3888 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/performance/linkprediction.py
--rw-rw-rw-   0 root         (0) root         (0)     4078 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/performance/performance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)      142 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4331 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/task_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      120 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks/python_callable_task.py
--rw-rw-rw-   0 root         (0) root         (0)     8445 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks/task_cc_fit.py
--rw-rw-rw-   0 root         (0) root         (0)     8106 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks/task_cc_predict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/
--rw-rw-rw-   0 root         (0) root         (0)      336 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5589 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_coordinates.py
--rw-rw-rw-   0 root         (0) root         (0)     5779 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_libraries.py
--rw-rw-rw-   0 root         (0) root         (0)     7613 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_molinfo.py
--rw-rw-rw-   0 root         (0) root         (0)     3677 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_plots.py
--rw-rw-rw-   0 root         (0) root         (0)     4696 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_projections.py
--rw-rw-rw-   0 root         (0) root         (0)     4968 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_pubchem.py
--rw-rw-rw-   0 root         (0) root         (0)    16319 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_showtargets.py
--rw-rw-rw-   0 root         (0) root         (0)     5832 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_similars.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/plot/
--rw-rw-rw-   0 root         (0) root         (0)      191 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39062 2021-11-30 16:00:23.000000 chemicalchecker-1.0.2/chemicalchecker/util/plot/diagnosticsplot.py
--rw-rw-rw-   0 root         (0) root         (0)     8635 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/plot/multiccplot.py
--rw-rw-rw-   0 root         (0) root         (0)   151932 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/plot/multiplot.py
--rw-rw-rw-   0 root         (0) root         (0)    79656 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/plot/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     8018 2021-12-03 15:01:12.000000 chemicalchecker-1.0.2/chemicalchecker/util/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/psql/
--rw-rw-rw-   0 root         (0) root         (0)      119 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/psql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1900 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/psql/psql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/remove_near_duplicates/
--rw-rw-rw-   0 root         (0) root         (0)      101 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/remove_near_duplicates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7723 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/remove_near_duplicates/remove_near_duplicates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/sampler/
--rw-rw-rw-   0 root         (0) root         (0)       62 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/sampler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8602 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/sampler/triplets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/sanitize/
--rw-rw-rw-   0 root         (0) root         (0)       60 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/sanitize/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14464 2021-12-03 12:10:45.000000 chemicalchecker-1.0.2/chemicalchecker/util/sanitize/sanitizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/splitter/
--rw-rw-rw-   0 root         (0) root         (0)      427 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/splitter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13100 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/splitter/ae_siam_traintest.py
--rw-rw-rw-   0 root         (0) root         (0)     4678 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/splitter/globalneighbortriplets.py
--rw-rw-rw-   0 root         (0) root         (0)    12117 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/splitter/neighborerror.py
--rw-rw-rw-   0 root         (0) root         (0)    20126 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/splitter/neighborpair.py
--rw-rw-rw-   0 root         (0) root         (0)    36865 2021-11-29 11:50:48.000000 chemicalchecker-1.0.2/chemicalchecker/util/splitter/neighbortriplet.py
--rw-rw-rw-   0 root         (0) root         (0)    10913 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/splitter/pairtraintest.py
--rw-rw-rw-   0 root         (0) root         (0)    18897 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/splitter/traintest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker/util/transform/
--rw-rw-rw-   0 root         (0) root         (0)      121 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/transform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7737 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/util/transform/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/transform/gaussian_scale_impute.py
--rw-rw-rw-   0 root         (0) root         (0)    12027 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/transform/gaussianize.py
--rw-rw-rw-   0 root         (0) root         (0)    10238 2021-11-19 16:56:37.000000 chemicalchecker-1.0.2/chemicalchecker/util/transform/lsi.py
--rw-rw-rw-   0 root         (0) root         (0)     4643 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/transform/metric_learn.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/transform/pca.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/chemicalchecker/util/transform/scale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8022 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9952 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/chemicalchecker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)      617 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/docs/_static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/docs/_static/css/
--rw-rw-rw-   0 root         (0) root         (0)      135 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/_static/css/logo.css
--rw-rw-rw-   0 root         (0) root         (0)      366 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/_static/css/overrides.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/docs/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      712 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/_templates/custom-class-template.rst
--rw-rw-rw-   0 root         (0) root         (0)     1229 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/_templates/custom-module-template.rst
--rw-rw-rw-   0 root         (0) root         (0)     5890 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/docs/img/
--rw-rw-rw-   0 root         (0) root         (0)     1150 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/img/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     4510 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/img/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)   944429 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/img/preprocessing.png
--rw-rw-rw-   0 root         (0) root         (0)     7525 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      777 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     2817 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/manifesto.rst
--rw-rw-rw-   0 root         (0) root         (0)     7584 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/signaturization.rst
--rw-rw-rw-   0 root         (0) root         (0)    31372 2021-11-19 09:59:04.000000 chemicalchecker-1.0.2/docs/sources.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-11 15:17:08.000000 chemicalchecker-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1861 2022-01-10 16:07:34.000000 chemicalchecker-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)      780 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      432 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6873 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-07-11 13:08:45.000000 chemicalchecker-1.0.3/chemicalchecker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/core/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2022-11-30 15:54:21.000000 chemicalchecker-1.0.3/chemicalchecker/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    51739 2023-07-11 13:08:45.000000 chemicalchecker-1.0.3/chemicalchecker/core/char.py
+-rw-rw-rw-   0 root         (0) root         (0)    46727 2023-02-26 04:04:04.000000 chemicalchecker-1.0.3/chemicalchecker/core/chemcheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    24087 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/chemicalchecker/core/clus.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2022-06-30 14:56:09.000000 chemicalchecker-1.0.3/chemicalchecker/core/data.py
+-rw-rw-rw-   0 root         (0) root         (0)    68470 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/chemicalchecker/core/diagnostics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples/
+-rw-rw-rw-   0 root         (0) root         (0)  5997712 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples/ctrp_auc.csv
+-rw-rw-rw-   0 root         (0) root         (0)  6479614 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples/fps.pkl
+-rw-rw-rw-   0 root         (0) root         (0)    36791 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples/pharmacodb_targets.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    20367 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples/toy_matrix.pkl
+-rw-rw-rw-   0 root         (0) root         (0)    43320 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples/toy_pairs.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples/validation_sets/
+-rw-rw-rw-   0 root         (0) root         (0)  8156424 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples/validation_sets/atc_validation.tsv
+-rw-rw-rw-   0 root         (0) root         (0)  6266204 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples/validation_sets/moa_validation.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2022-05-01 04:04:29.000000 chemicalchecker-1.0.3/chemicalchecker/core/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)    40928 2023-07-11 13:08:45.000000 chemicalchecker-1.0.3/chemicalchecker/core/molkit.py
+-rw-rw-rw-   0 root         (0) root         (0)    17811 2022-11-30 15:30:35.000000 chemicalchecker-1.0.3/chemicalchecker/core/neig.py
+-rw-rw-rw-   0 root         (0) root         (0)    22716 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/preprocess.py
+-rw-rw-rw-   0 root         (0) root         (0)    11417 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/proj.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/core/projector/
+-rw-rw-rw-   0 root         (0) root         (0)      130 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/projector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14998 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/projector/default.py
+-rw-rw-rw-   0 root         (0) root         (0)     5319 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/projector/pca.py
+-rw-rw-rw-   0 root         (0) root         (0)     6979 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/projector/tsne.py
+-rw-rw-rw-   0 root         (0) root         (0)     6922 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/projector/umap_.py
+-rw-rw-rw-   0 root         (0) root         (0)    24629 2023-02-26 04:04:04.000000 chemicalchecker-1.0.3/chemicalchecker/core/sign0.py
+-rw-rw-rw-   0 root         (0) root         (0)    21529 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/sign1.py
+-rw-rw-rw-   0 root         (0) root         (0)    26561 2023-02-26 04:04:04.000000 chemicalchecker-1.0.3/chemicalchecker/core/sign2.py
+-rw-rw-rw-   0 root         (0) root         (0)   114384 2023-02-26 04:04:04.000000 chemicalchecker-1.0.3/chemicalchecker/core/sign3.py
+-rw-rw-rw-   0 root         (0) root         (0)    18890 2023-03-29 09:27:39.000000 chemicalchecker-1.0.3/chemicalchecker/core/sign4.py
+-rw-rw-rw-   0 root         (0) root         (0)    22337 2023-03-29 11:08:52.000000 chemicalchecker-1.0.3/chemicalchecker/core/signature_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    39149 2023-03-29 11:08:52.000000 chemicalchecker-1.0.3/chemicalchecker/core/signature_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2140 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/core/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/database/
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10229 2023-03-21 16:45:08.000000 chemicalchecker-1.0.3/chemicalchecker/database/calcdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2023-03-21 16:45:08.000000 chemicalchecker-1.0.3/chemicalchecker/database/database.py
+-rw-rw-rw-   0 root         (0) root         (0)    19569 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/database/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    10320 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/database/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-03-21 16:45:08.000000 chemicalchecker-1.0.3/chemicalchecker/database/molecule.py
+-rw-rw-rw-   0 root         (0) root         (0)    18198 2023-03-21 16:45:08.000000 chemicalchecker-1.0.3/chemicalchecker/database/molrepo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2809 2023-03-21 16:45:08.000000 chemicalchecker-1.0.3/chemicalchecker/database/pubchem.py
+-rw-rw-rw-   0 root         (0) root         (0)    12314 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/database/uniprotkb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      441 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/adanet/
+-rw-rw-rw-   0 root         (0) root         (0)      207 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/adanet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25344 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/adanet/adanet_wrap.py
+-rw-rw-rw-   0 root         (0) root         (0)     4527 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/adanet/cnn_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9190 2023-03-22 12:01:12.000000 chemicalchecker-1.0.3/chemicalchecker/tool/adanet/dnn_extend_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     7337 2023-03-22 12:01:12.000000 chemicalchecker-1.0.3/chemicalchecker/tool/adanet/dnn_stack_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/autoencoder/
+-rw-rw-rw-   0 root         (0) root         (0)      171 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/autoencoder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11213 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/autoencoder/autoencoder.py
+-rw-rw-rw-   0 root         (0) root         (0)    13756 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/autoencoder/autoencoder_siamese.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/classifier/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/classifier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/classifier/imbalanced/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/classifier/imbalanced/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14447 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/classifier/imbalanced/imbalanced.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/classifier/multitask/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/classifier/multitask/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10766 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/classifier/multitask/binarymultitask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/feat/
+-rw-rw-rw-   0 root         (0) root         (0)      455 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/feat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/feat/base_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    15124 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/feat/graph_features.py
+-rw-rw-rw-   0 root         (0) root         (0)    15248 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/graphconv/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/graphconv/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14488 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/graphconv/graph_smiles_sign.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/hotnet/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/hotnet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2536 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/hotnet/hotnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/node2vec/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/node2vec/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19770 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/node2vec/node2vec.py
+-rw-rw-rw-   0 root         (0) root         (0)     3080 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/node2vec/word2vec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/siamese/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/siamese/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11641 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/siamese/callbacks.py
+-rw-rw-rw-   0 root         (0) root         (0)    17397 2022-10-07 13:56:34.000000 chemicalchecker-1.0.3/chemicalchecker/tool/siamese/siamese.py
+-rw-rw-rw-   0 root         (0) root         (0)    47727 2023-01-10 10:24:26.000000 chemicalchecker-1.0.3/chemicalchecker/tool/siamese/siamese_triplets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/smilespred/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/smilespred/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9692 2023-03-29 09:27:39.000000 chemicalchecker-1.0.3/chemicalchecker/tool/smilespred/apppred.py
+-rw-rw-rw-   0 root         (0) root         (0)    15221 2023-03-29 09:27:39.000000 chemicalchecker-1.0.3/chemicalchecker/tool/smilespred/smilespred.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23275 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/chembl/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/chembl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10771 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/chembl/fetch_chembl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/drugbank/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/drugbank/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7010 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/drugbank/fetch_drugbank.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/moleculenet/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/moleculenet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/moleculenet/fetch_moleculenet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/evaluation/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/evaluation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14640 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/evaluation/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/evaluation/score.py
+-rw-rw-rw-   0 root         (0) root         (0)    33340 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/evaluation/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/examples/example.py
+-rw-rw-rw-   0 root         (0) root         (0)    14143 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/ml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/autosklearnconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/gridconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4407 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/hyperoptconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)     6168 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/tpotconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/vanillaconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1705 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/multi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11969 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/acp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5286 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)    14376 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)    16054 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/icp.py
+-rw-rw-rw-   0 root         (0) root         (0)    14653 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/nc.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     6026 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/run.py
+-rw-rw-rw-   0 root         (0) root         (0)    18753 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/signaturizer.py
+-rw-rw-rw-   0 root         (0) root         (0)    27022 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/tmsetup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/universes/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/universes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16802 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/universes/univs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3653 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/chemistry.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/conformal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/hpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    15028 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/pairs.py
+-rw-rw-rw-   0 root         (0) root         (0)    12322 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    16489 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/reportcard.py
+-rw-rw-rw-   0 root         (0) root         (0)    20934 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/splitters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/topped.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/aggregate/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/aggregate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5832 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/aggregate/aggregate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/config/cc_config.json
+-rw-rw-rw-   0 root         (0) root         (0)     2009 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/config/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/decomposition/
+-rw-rw-rw-   0 root         (0) root         (0)      375 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/decomposition/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/decomposition/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/decorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27196 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/decorator/profilehooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/decorator/property.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/decorator/safe.py
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/decorator/timeout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/download/
+-rw-rw-rw-   0 root         (0) root         (0)      491 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8694 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/download/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/filesystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/filesystem/filesystem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/hpc/
+-rw-rw-rw-   0 root         (0) root         (0)      669 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/hpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6042 2022-09-14 12:44:46.000000 chemicalchecker-1.0.3/chemicalchecker/util/hpc/hpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6611 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/hpc/local.py
+-rw-rw-rw-   0 root         (0) root         (0)    12287 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/hpc/sge.py
+-rw-rw-rw-   0 root         (0) root         (0)    11441 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/hpc/slurm.py
+-rw-rw-rw-   0 root         (0) root         (0)    12529 2022-05-31 14:42:32.000000 chemicalchecker-1.0.3/chemicalchecker/util/hpc/slurm_gpu.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/hpc/test_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/keytype/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/keytype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/keytype/detect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/logging/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/logging/logging_conf.ini
+-rw-rw-rw-   0 root         (0) root         (0)      419 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/logging/our_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/mol2svg/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/mol2svg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/mol2svg/mol2svg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker/util/network/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/network/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12686 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/network/network.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      218 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12129 2023-03-10 14:52:51.000000 chemicalchecker-1.0.3/chemicalchecker/util/parser/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)    14209 2023-02-26 04:04:04.000000 chemicalchecker-1.0.3/chemicalchecker/util/parser/data_calculator.py
+-rw-rw-rw-   0 root         (0) root         (0)    34304 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/parser/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/performance/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/performance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2022-05-27 14:08:00.000000 chemicalchecker-1.0.3/chemicalchecker/util/performance/linkprediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4078 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/performance/performance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4331 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/task_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks/python_callable_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     8445 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks/task_cc_fit.py
+-rw-rw-rw-   0 root         (0) root         (0)     8106 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks/task_cc_predict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5589 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_coordinates.py
+-rw-rw-rw-   0 root         (0) root         (0)     5779 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_libraries.py
+-rw-rw-rw-   0 root         (0) root         (0)     7613 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_molinfo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3677 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     4696 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_projections.py
+-rw-rw-rw-   0 root         (0) root         (0)     4968 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_pubchem.py
+-rw-rw-rw-   0 root         (0) root         (0)    16319 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_showtargets.py
+-rw-rw-rw-   0 root         (0) root         (0)     5832 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_similars.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_statsplots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7395 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/plot/ccstatsplot.py
+-rw-rw-rw-   0 root         (0) root         (0)    45369 2022-07-07 15:30:28.000000 chemicalchecker-1.0.3/chemicalchecker/util/plot/diagnosticsplot.py
+-rw-rw-rw-   0 root         (0) root         (0)     8635 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/plot/multiccplot.py
+-rw-rw-rw-   0 root         (0) root         (0)   151932 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/plot/multiplot.py
+-rw-rw-rw-   0 root         (0) root         (0)    79673 2022-05-27 14:08:00.000000 chemicalchecker-1.0.3/chemicalchecker/util/plot/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    10611 2023-03-14 15:20:19.000000 chemicalchecker-1.0.3/chemicalchecker/util/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/psql/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/psql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/psql/psql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/remove_near_duplicates/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/remove_near_duplicates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7723 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/remove_near_duplicates/remove_near_duplicates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/sampler/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/sampler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8602 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/sampler/triplets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/sanitize/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/sanitize/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14464 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/sanitize/sanitizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/splitter/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-10-19 17:15:33.000000 chemicalchecker-1.0.3/chemicalchecker/util/splitter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13100 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/splitter/ae_siam_traintest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4678 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/splitter/globalneighbortriplets.py
+-rw-rw-rw-   0 root         (0) root         (0)    12117 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/splitter/neighborerror.py
+-rw-rw-rw-   0 root         (0) root         (0)    20126 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/splitter/neighborpair.py
+-rw-rw-rw-   0 root         (0) root         (0)    52381 2022-10-25 09:14:27.000000 chemicalchecker-1.0.3/chemicalchecker/util/splitter/neighbortriplet.py
+-rw-rw-rw-   0 root         (0) root         (0)    10913 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/splitter/pairtraintest.py
+-rw-rw-rw-   0 root         (0) root         (0)    18897 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/splitter/traintest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/chemicalchecker/util/transform/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/transform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7845 2022-06-29 10:00:41.000000 chemicalchecker-1.0.3/chemicalchecker/util/transform/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/transform/gaussian_scale_impute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12027 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/transform/gaussianize.py
+-rw-rw-rw-   0 root         (0) root         (0)    10268 2022-05-27 14:08:00.000000 chemicalchecker-1.0.3/chemicalchecker/util/transform/lsi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4833 2022-10-19 17:15:33.000000 chemicalchecker-1.0.3/chemicalchecker/util/transform/metric_learn.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/transform/pca.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/chemicalchecker/util/transform/scale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/chemicalchecker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-07-11 15:44:12.000000 chemicalchecker-1.0.3/chemicalchecker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-07-11 15:44:12.000000 chemicalchecker-1.0.3/chemicalchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:44:12.000000 chemicalchecker-1.0.3/chemicalchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:44:12.000000 chemicalchecker-1.0.3/chemicalchecker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-11 15:44:12.000000 chemicalchecker-1.0.3/chemicalchecker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-11 15:44:12.000000 chemicalchecker-1.0.3/chemicalchecker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:13.000000 chemicalchecker-1.0.3/docs/_static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/docs/_static/css/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/docs/_static/css/logo.css
+-rw-rw-rw-   0 root         (0) root         (0)      366 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/docs/_static/css/overrides.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/docs/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      712 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/docs/_templates/custom-class-template.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/docs/_templates/custom-module-template.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5890 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/docs/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/docs/img/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     4510 2022-05-01 04:04:30.000000 chemicalchecker-1.0.3/docs/img/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)   944429 2022-05-01 04:04:31.000000 chemicalchecker-1.0.3/docs/img/preprocessing.png
+-rw-rw-rw-   0 root         (0) root         (0)     8029 2022-05-24 12:18:12.000000 chemicalchecker-1.0.3/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      777 2022-05-01 04:04:31.000000 chemicalchecker-1.0.3/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2022-05-01 04:04:31.000000 chemicalchecker-1.0.3/docs/manifesto.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8362 2022-05-24 12:18:12.000000 chemicalchecker-1.0.3/docs/signaturization.rst
+-rw-rw-rw-   0 root         (0) root         (0)    31372 2022-05-01 04:04:31.000000 chemicalchecker-1.0.3/docs/sources.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 15:44:14.000000 chemicalchecker-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2023-07-11 13:08:45.000000 chemicalchecker-1.0.3/setup.py
```

### Comparing `chemicalchecker-1.0.2/AUTHORS.rst` & `chemicalchecker-1.0.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/CONTRIBUTING.rst` & `chemicalchecker-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/LICENSE` & `chemicalchecker-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/PKG-INFO` & `chemicalchecker-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemicalchecker
-Version: 1.0.2
+Version: 1.0.3
 Summary: Chemical Checker Package.
 Home-page: http://gitlabsbnb.irbbarcelona.org/packages/chemical_checker
 Author: SBNB
 Author-email: sbnb@irbbarcelona.org
 License: MIT License
 Keywords: chemicalchecker bioactivity signatures chemoinformatics
 Platform: UNKNOWN
```

### Comparing `chemicalchecker-1.0.2/README.rst` & `chemicalchecker-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/__init__.py` & `chemicalchecker-1.0.3/chemicalchecker/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 from .core import ChemicalChecker
 from .util import Config
 
 #ChemicalChecker.set_verbosity(level=Config().VERBOSITY.level)
 
 __author__ = """SBNB"""
 __email__ = 'sbnb@irbbarcelona.org'
-__version__ = '1.0.2'
+__version__ = '1.0.3'
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/__init__.py` & `chemicalchecker-1.0.3/chemicalchecker/core/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 """
 from .data import DataFactory
 from .chemcheck import ChemicalChecker
 from .validation import Validation
 from .signature_data import DataSignature
 from .examples import Example
 from .diagnostics import Diagnosis
-from .molkit import Mol
+from .molkit import Mol, Molset
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/chemcheck.py` & `chemicalchecker-1.0.3/chemicalchecker/core/chemcheck.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,24 +46,26 @@
 import os
 import gzip
 import h5py
 import json
 import shutil
 import itertools
 import numpy as np
+import pandas as pd
 from glob import glob
 from pathlib import Path
 
 from .molkit import Mol
 from .data import DataFactory
 from .signature_data import DataSignature
 
 from chemicalchecker.database import Dataset, Molecule
 from chemicalchecker.database.database import test_connection
 from chemicalchecker.util import logged, Config
+from chemicalchecker.util.filesystem import FileSystem
 from chemicalchecker.util.decorator import cached_property
 
 
 @logged
 class ChemicalChecker():
     """ChemicalChecker class."""
 
@@ -79,17 +81,18 @@
                 If not specified the root is taken from the config file.
             custom_data_path (None, str): Path to one or more h5 files, detect
                 their signature type, molset and dataset code form their
                 'attrs' record.
             dbconnect (True, Bool): if True, try to connect to the DB
         """
         # Default cc_root is taken from config file
-        self.cc_root = cc_root
-        if self.cc_root is None:
-            self.cc_root = Config().PATH.CC_ROOT
+        if cc_root is None:
+            self.cc_root = os.path.realpath(Config().PATH.CC_ROOT)
+        else:
+            self.cc_root = os.path.realpath(cc_root)
 
         self._basic_molsets = ['reference', 'full']
         self._datasets = set()
         self._molsets = set(self._basic_molsets)
         self._exemplary_id = "001"
         self._metadata = None
         self.__log.debug("ChemicalChecker with root: %s", self.cc_root)
@@ -123,22 +126,22 @@
             self._molsets = set(x.split('/')[-6] for x in paths)
             self._datasets = set(x.split('/')[-3] for x in paths)
             if custom_data_path is not None:
                 self.__log.info("CC root directory exists: "
                                 "ignoring 'custom_data_path'.")
                 custom_data_path = None
 
-        # import one or several custom h5 files
+        # import one or several custom signature files and models
         if custom_data_path is not None:
             if os.path.isfile(custom_data_path):
                 raise Exception("'custom_data_path' must be a directory")
 
             custom_data_path = os.path.abspath(custom_data_path)
             self.__log.debug("Linking files from: %s" % custom_data_path)
-            self.link_h5(custom_data_path)
+            self.link(custom_data_path)
 
         self._molsets = sorted(list(self._molsets))
         self._datasets = [x for x in sorted(
             list(self._datasets)) if not x.endswith('000')]
 
     @property
     def coordinates(self):
@@ -271,15 +274,15 @@
             ch.setFormatter(formatter)
             logger.handlers = []
             logger.addHandler(ch)
         logger.setLevel(levels[level])
         log_fn[level]("Logging level %s for logger '%s'." %
                       (level.upper(), logger_name))
 
-    def _available_sign_paths(self, molset='*', dataset='*', signature='*',
+    def _available_sign_paths(self, molset='[!exemplary]*', dataset='*', signature='*',
                               filename='*.h5'):
         paths = glob(os.path.join(self.cc_root, molset, '*',
                                   '*', dataset, signature, filename))
         return paths
 
     def report_available(self, molset='*', dataset='*', signature='*'):
         """Report available signatures in the CC.
@@ -437,23 +440,26 @@
         Args:
             cctype(str): The Chemical Checker datatype (i.e. one of the sign*).
             molset(str): The molecule set name.
             dataset_code(str): The dataset code of the Chemical Checker.
             params(dict): Optional. The set of parameters to initialize and
                 compute the signature. If the signature is already initialized
                 this argument will be ignored.
+            as_dataframe(bool): True to get the signature as pandas DataFrame.
         Returns:
             data(Signature): A `Signature` object, the specific type depends
                 on the cctype passed.
         """
         signature_path = self.get_signature_path(cctype, molset, dataset_code)
-
+        as_dataframe = kwargs.pop('as_dataframe', False)
         # the factory will return the signature with the right class
         data = DataFactory.make_data(
             cctype, signature_path, dataset_code, *args, **kwargs)
+        if as_dataframe:
+            return data.as_dataframe()
         return data
 
     def get_data_signature(self, cctype, dataset_code):
         """Return the data signature for the given dataset code.
 
         Args:
             cctype(str): The Chemical Checker datatype (i.e. one of the sign*).
@@ -475,127 +481,177 @@
         if not os.path.exists(data.data_path):
             self.__log.error(
                 "There is no data for %s and dataset code %s" %
                 (cctype, dataset_code))
             return None
         return DataSignature(data.data_path)
 
-    def signature(self, dataset, cctype):
+    def signature(self, dataset, cctype, as_dataframe=False, **kwargs):
         return self.get_signature(cctype=cctype, molset="full",
-                                  dataset_code=dataset)
+                                  dataset_code=dataset,
+                                  as_dataframe=as_dataframe, **kwargs)
 
-    def link_h5(self, custom_data_path):
-        """Link H5 files from a given custom directory.
-
-        Populates local CC instance with symlinks to external signatures H5s.
+    @staticmethod
+    def get_h5_metadata(fn, format_dict):
+        """ Return H5 metadata.
 
-        Args:
-            custom_data_path(str): Path to a directory signature containing H5s
+        Returns:
+            tuple of the type ('full', 'A', 'A1', 'A1.001','sign3', h5_path) 
+            or None if something's wrong
         """
-        h5files = glob(os.path.join(custom_data_path, "*.h5"))
-
-        if len(h5files) == 0:
-            self.__log.warning("No h5 file found in %s, "
-                               "CC instance will be empty." % custom_data_path)
-            return
-
-        available_files = ", ".join([os.path.basename(f) for f in h5files])
-        self.__log.debug("Found h5 files {}: in {}".format(
-            available_files, custom_data_path))
-
-        # check the format of the imported info data
-        # dataset code (ex: A1.001)
-        formatDC = re.compile(r"[A-Z]\d\.\d\d\d")
-        formatCCTYPE = re.compile(r"sign\d")
-        formatMolset = re.compile(r"(full|reference)", re.IGNORECASE)
-
-        # mapping info and required format
-        formatDict = dict(dataset_code=formatDC,
-                          cctype=formatCCTYPE, molset=formatMolset)
-
-        def filter_dataset(path2h5file):
-            """ returns a tuple of the type ('full', 'A', 'A1', 'A1.001',
-            'sign3', path_to_h5file') or None if something's wrong
-            """
-            out = []
-            with h5py.File(path2h5file, 'r') as ccfile:
-
-                # check if the required info is presents in the h5 file
-                # attrs dict
-                # iterates over ('dataset_code', 'cctype', 'molset') and
-                # the required format for each of them
-                for requiredKey, requiredFormat in formatDict.items():
-                    if requiredKey not in ccfile.attrs:
-                        self.__log.warning(
-                            "Attribute {} cannot be retrieved from {},"
-                            " skipping this file".format(
-                                requiredKey, ccfile))
+        out = []
+        with h5py.File(fn, 'r') as ccfile:
+            # check if the required info is presents in the h5 file
+            for requiredKey, requiredFormat in format_dict.items():
+                if requiredKey not in ccfile.attrs:
+                    ChemicalChecker.__log.warning(
+                        "Attribute {} cannot be retrieved from {},"
+                        " skipping this file".format(
+                            requiredKey, ccfile))
+                    return None
+                else:
+                    # check the format of the provided info
+                    matching = requiredFormat.match(
+                        ccfile.attrs[requiredKey])
+                    if matching is None:
+                        ChemicalChecker.__log.warning(
+                            "Problem with format",
+                            ccfile.attrs[requiredKey])
                         return None
+            # Prepare the signature file name and path
+            out.append(ccfile.attrs['molset'].lower())
+            out.append(ccfile.attrs['dataset_code'][0])
+            out.append(ccfile.attrs['dataset_code'][:2])
+            out.append(ccfile.attrs['dataset_code'])
+            out.append(ccfile.attrs['cctype'].lower())
+            out.append(fn)
+        return tuple(out)
 
-                    else:
-                        # check the format of the provided info
-                        matching = requiredFormat.match(
-                            ccfile.attrs[requiredKey])
-                        if matching is None:
-                            self.__log.warning(
-                                "Problem with format",
-                                ccfile.attrs[requiredKey])
-                            return None
-
-                # Prepare the signature file name and path
-                out.append(ccfile.attrs['molset'].lower())
-                out.append(ccfile.attrs['dataset_code'][0])
-                out.append(ccfile.attrs['dataset_code'][:2])
-                out.append(ccfile.attrs['dataset_code'])
-                out.append(ccfile.attrs['cctype'].lower())
-                out.append(path2h5file)
-            return tuple(out)
-
-        # Keep h5 files containing the required info in the correct format
-        h5tuples = list()
-        for fn in h5files:
-            res = filter_dataset(fn)
-            if res:
-                h5tuples.append(res)
+    @staticmethod
+    def get_model_metadata(fn, format_dict):
+        """ Return model metadata.
+
+        Returns:
+            tuple of the type ('full', 'A', 'A1', 'A1.001','sign3', h5_path) 
+            or None if something's wrong
+        """
+        out = []
+        mdl_meta = json.load(open(os.path.join(fn, 'metadata.json'), 'r'))
+        # check if the required info is presents in the model file
+        for requiredKey, requiredFormat in format_dict.items():
+            if requiredKey not in mdl_meta.keys():
+                ChemicalChecker.__log.warning(
+                    "Attribute {} cannot be retrieved from {},"
+                    " skipping this file".format(
+                        requiredKey, mdl_meta))
+                return None
             else:
-                # guess from filename
-                name = Path(fn).stem
+                # check the format of the provided info
+                matching = requiredFormat.match(
+                    mdl_meta[requiredKey])
+                if matching is None:
+                    ChemicalChecker.__log.warning(
+                        "Problem with format",
+                        mdl_meta[requiredKey])
+                    return None
+        # Prepare the model file name and path
+        out.append(mdl_meta['molset'].lower())
+        out.append(mdl_meta['dataset_code'][0])
+        out.append(mdl_meta['dataset_code'][:2])
+        out.append(mdl_meta['dataset_code'])
+        out.append(mdl_meta['cctype'].lower())
+        out.append(fn)
+        return tuple(out)
+
+    @staticmethod
+    def get_metadatas(files, metadata_func, format_dict):
+        """Extract the metadata from files using a function."""
+        available_files = ", ".join([os.path.basename(f) for f in files])
+        ChemicalChecker.__log.debug(
+            "Importing files {}".format(available_files))
+        # Keep files containing the required info in the correct format
+        metadatas = list()
+        for file in files:
+            res = metadata_func(file, format_dict)
+            if res:
+                metadatas.append(res)
+            else:  # guess from filename
+                name = Path(file).stem
                 cctype, dataset_code, molset = name.split('_')
-                res = []
+                res = list()
                 res.append(molset.lower())
                 res.append(dataset_code[0])
                 res.append(dataset_code[:2])
                 res.append(dataset_code)
                 res.append(cctype.lower())
-                res.append(fn)
-                h5tuples.append(res)
-
-        if len(h5tuples) == 0:
+                res.append(file)
+                metadatas.append(res)
+        if len(metadatas) == 0:
             raise Exception(
                 "None of the provided h5 datasets have sufficient info in"
                 " its attributes! Please ensure myh5file.attrs has the"
                 "folllowing keys: 'dataset_code', 'cctype', 'molset'")
+        return metadatas
 
-        # Now creating the instance folder structure
-        original_umask = os.umask(0)
-        for h5t in h5tuples:
-            # ex: ../../full/A/A1/A1.001/sign3
-            path2sign = os.path.join(self.cc_root, *h5t[:-1])
-            self.__log.debug("Creating: %s", path2sign)
-
-            # The signature should not exist
-            if os.path.exists(path2sign):
-                self.__log.debug("Skipping as path exists: %s", path2sign)
-                continue
+    def link(self, custom_data_path):
+        """Link H5 files and models from a given custom directory.
 
-            # create dir
-            os.makedirs(path2sign, 0o775)
-            # symbolic link to the h5 file in the cc_repo as signx.h5
-            os.symlink(h5t[-1], os.path.join(path2sign, h5t[-2] + '.h5'))
-        os.umask(original_umask)
+        Populates local CC instance with symlinks to external signatures H5s
+        or models.
+
+        Args:
+            custom_data_path(str): Path to a directory signature containing H5s
+                models or symlinks.
+        """
+        # define required format for metadata fields
+        ds_fmt = re.compile(r"[A-Z]\d\.\d\d\d")  # dataset code (ex: A1.001)
+        cctype_fmt = re.compile(r"sign\d")
+        molset_fmt = re.compile(r"(full|reference)", re.IGNORECASE)
+        format_dict = dict(dataset_code=ds_fmt,
+                           cctype=cctype_fmt, molset=molset_fmt)
+
+        # get H5 files metadata
+        files = glob(os.path.join(custom_data_path, "*.h5"))
+        if len(files) == 0:
+            ChemicalChecker.__log.warning(f"No *.h5 file found in {custom_data_path}, "
+                                          "CC instance will be without data.")
+        else:
+            metadatas = self.get_metadatas(
+                files, self.get_h5_metadata, format_dict)
+
+            # Create the CC instance folder structure
+            for meta in metadatas:
+                sign_path = os.path.join(self.cc_root, *meta[:-1])
+                # create dir
+                os.makedirs(sign_path, exist_ok=True)
+                src = meta[-1]
+                # symbolic link to the h5 file in the cc_repo as signx.h5
+                dst = os.path.join(sign_path, meta[-2] + '.h5')
+                self.__log.debug("%s ==> %s" % (src, dst))
+                os.symlink(src, dst)
+
+        # get models metadata
+        files = glob(os.path.join(custom_data_path, "*.models"))
+        if len(files) == 0:
+            ChemicalChecker.__log.warning(f"No *.model found in {custom_data_path}, "
+                                          "CC instance will be without models.")
+        else:
+            metadatas = self.get_metadatas(
+                files, self.get_model_metadata, format_dict)
+
+            # add symlinks to models
+            for meta in metadatas:
+                sign_path = os.path.join(self.cc_root, *meta[:-1])
+                # create dir
+                os.makedirs(sign_path, exist_ok=True)
+                src = meta[-1]
+                # symbolic link to the models path in the cc_repo as models folder
+                dst = os.path.join(sign_path, 'models')
+                self.__log.debug("%s ==> %s" % (src, dst))
+                os.symlink(src, dst)
 
     def export(self, destination, signature, h5_filter=None,
                h5_names_map={}, overwrite=False, version=None):
         """Export a signature h5 file to a given path.
 
         Which dataset to copy can be specified as well as how to rename some
         dataset.
@@ -635,44 +691,189 @@
         if len(dst.attrs) != 3:
             for k, v in attributes.items():
                 dst.attrs[k] = v
 
         src.close()
         dst.close()
 
+    # Export minimum CC zipped folder
+    def export_cc(self, root_destination, folder_destination):
+        """Export a zipped folder containing the minimum files necessary 
+           to run a complete CC protocol
+
+        It includes:
+            - full: all sign0 (.h5 files + fit.ready file in models folder)
+            - reference: sign1 models folder (.pkl files only) 
+              --> sign1 are going to be generated based on sign0
+                  at the initialization of the ChemicalChecker instance
+            - reference: sign2 models (savedmodel folder only) 
+              --> sign2 are going to be generated based on sign1 and neig1
+              (also generated once sign1 is ready)
+
+        Args:
+            root_destination(str): An export destination path
+            folder_destination(str): additional path to append to root_destination
+                --> used to define the base_dir when zipping
+        """
+        destination = os.path.join(root_destination, folder_destination)
+        self.__log.debug('Exporting CC {} to {}'.format(
+            self.cc_root, destination))
+
+        for molset in self._basic_molsets:
+            self.__log.debug('Molset: {}'.format(molset))
+            for dataset in self.datasets_exemplary():
+                self.__log.debug('Dataset: {}'.format(dataset))
+                # 0) root dir of a dataset: full/reference
+                # adding an additional layer inside the folder_destination so that when the
+                # folder is zipped, it remains inside the CC version directory at the same level as
+                # the exported sign3
+                new_dir = os.path.join(
+                    destination, folder_destination, molset, dataset[:1], dataset[:2], dataset)
+                FileSystem.check_dir_existance_create(new_dir)
+                # 1) sign0
+                if molset == 'full':
+                    sign_type = 'sign0'
+                    sign = self.get_signature(sign_type, molset, dataset)
+                    sign_dir = os.path.join(new_dir, '%s' % sign_type)
+                    FileSystem.check_dir_existance_create(sign_dir)
+                    FileSystem.check_dir_existance_create(sign_dir, ['models'])
+                    dst = os.path.join(sign_dir, '%s.h5' % sign_type)
+                    if not os.path.isfile(dst):
+                        self.__log.debug(
+                            "Copying {} to {}".format(sign, sign_dir))
+                        self.export(dst, sign)
+                    fit_file = os.path.join(sign_dir, 'models', 'fit.ready')
+                    FileSystem.check_file_existance_create(fit_file)
+                # 2) sign1
+                if molset == 'reference':
+                    sign_type = 'sign1'
+                    sign = self.get_signature(sign_type, molset, dataset)
+                    sign_dir = os.path.join(new_dir, '%s' % sign_type)
+                    dst_models_path = FileSystem.check_dir_existance_create(sign_dir, [
+                                                                            'models'])
+                    regex = re.compile('(.*pkl$)')
+                    self.__log.debug("Exporting files of {} from \
+                                        {} to {}".format(sign_type, sign.model_path, dst_models_path))
+                    for _, _, src_files in os.walk(sign.model_path):
+                        for src_file in src_files:
+                            if regex.match(src_file):
+                                dst_file = os.path.join(
+                                    dst_models_path, '%s' % src_file)
+                                FileSystem.check_file_existance_create(
+                                    dst_file)
+                                shutil.copyfile(os.path.join(
+                                    sign.model_path, src_file), dst_file)
+                # 3) sign2
+                if molset == 'reference':
+                    sign_type = 'sign2'
+                    model = 'adanet'
+                    sign = self.get_signature(sign_type, molset, dataset)
+                    sign_dir = os.path.join(new_dir, '%s' % sign_type)
+                    dst_models_adanet_path = FileSystem.check_dir_existance_create(sign_dir, [
+                                                                                   'models', model])
+                    if os.path.isdir(os.path.join(dst_models_adanet_path, 'savedmodel')):
+                        self.__log.debug("savedmodel folder already exists in {} models directory\n \
+                                Removing it".format(sign_type))
+                        shutil.rmtree(os.path.join(
+                            dst_models_adanet_path, 'savedmodel'))
+                    src_path = os.path.join(
+                        sign.model_path, model, 'savedmodel')
+                    self.__log.debug("Copying savedmodel folder from {} to {}".format(
+                        os.path.join(sign.model_path, model), dst_models_adanet_path))
+                    shutil.copytree(src_path, os.path.join(
+                        dst_models_adanet_path, 'savedmodel'))
+
+        # zipping the destination folder
+        complete_destination = os.path.join(destination, folder_destination)
+        self.__log.debug(
+            'Zipping exported CC folder {}'.format(complete_destination))
+        shutil.make_archive(complete_destination, 'gztar',
+                            destination, folder_destination)
+        if os.path.isfile(os.path.join(destination, folder_destination + '.tar.gz')):
+            shutil.rmtree(complete_destination)
+
+    def check_dir_existance_create(dir_path, additional_path=None):
+        """Args:
+            dir_path(str): root path
+            additional_path(list) : list of strings including additional
+                                    path parts to append to the root path
+        """
+        path = dir_path
+        if additional_path:
+            for element in additional_path:
+                path = os.path.join(path, element)
+        if not os.path.isdir(path):
+            original_umask = os.umask(0)
+            os.makedirs(path, 0o775)
+            os.umask(original_umask)
+        return path
+
+    def check_file_existance_create(file_path):
+        """
+            This method create an empty file if it doesn't exist already
+        """
+        if not os.path.isfile(file_path):
+            with open(file_path, 'w'):
+                pass
+
     def symlink_to(self, source_cc, cctypes=['sign0'],
-                   molsets=['reference', 'full'], datasets='exemplary'):
-        """Link current CC instane to other via symlinks.
+                   molsets=['reference', 'full'], datasets='exemplary',
+                   rename_dataset=None, models=False):
+        """Link current CC instance to other via symlinks.
 
-        When experimenting with signature parameters it's usefull to have
+        When experimenting with signature parameters it's useful to have
         low cctype (e.g. sign0, sign1) not copied but simply linked.
 
         Args:
             source_cc(ChemicalChecker): A different CC instance to link.
             cctypes(list): The signature (i.e. sign*) to link.
-            molsets(list): The molecule set name to link .
+            molsets(list): The molecule set name to link.
             datasets(list): The codes of dataset to link.
+            rename_dataset(dict): None by default which to no renaming.
+                Otherwise a mapping of source to destination name should be
+                provided.
+            models(bool): If True, models directory will also be linked.
+                This will delete the local models for the specified
+                datasets.
         """
         if datasets == 'exemplary':
             datasets = list(self.datasets_exemplary())
 
+        if rename_dataset is None:
+            rename_dataset = dict(zip(datasets, datasets))
         for molset in molsets:
             for ds in datasets:
+                dst_ds = rename_dataset[ds]
                 dst_ds_dir = os.path.join(
-                    self.cc_root, molset, ds[:1], ds[:2], ds)
+                    self.cc_root, molset, dst_ds[:1], dst_ds[:2], dst_ds)
+                os.makedirs(dst_ds_dir, exist_ok=True)
                 src_ds_dir = os.path.join(
                     source_cc.cc_root, molset, ds[:1], ds[:2], ds)
                 for cctype in cctypes:
                     dst_dir = os.path.join(dst_ds_dir, cctype)
                     src_dir = os.path.join(src_ds_dir, cctype)
                     self.__log.debug("Link %s --> %s", dst_dir, src_dir)
+                    # if the destination already a folder then the user has
+                    # full ownership over it, otherwise just symlink the ref.
                     if os.path.isdir(dst_dir):
                         self.__log.warning("%s already present", dst_dir)
+                        # in case the directory already exists try to link
+                        # the reference model dir
+                        if models:
+                            dst_model_dir = os.path.join(dst_dir, 'models')
+                            if os.path.isdir(dst_model_dir):
+                                if os.path.islink(dst_model_dir):
+                                    os.remove(dst_model_dir)
+                                else:
+                                    shutil.rmtree(dst_model_dir)
+                            src_model_dir = os.path.join(src_dir, 'models')
+                            os.symlink(src_model_dir, dst_model_dir)
                         continue
-                    os.symlink(src_dir, dst_dir)
+                    else:
+                        os.symlink(src_dir, dst_dir)
 
     def copy_signature_from(self, source_cc, cctype, molset, dataset_code,
                             overwrite=False):
         """Copy a signature file from another CC instance.
 
         Args:
             source_cc(ChemicalChecker): A different CC instance.
@@ -757,44 +958,60 @@
                 return global_sign
 
         else:
             self.__log.warning(mol_str + " NOT IN UNIVERSE")
 
         return None
 
-    def export_symlinks(self, dest_path=None, essential_only=True):
-        """Creates symlinks for all available signatures in a single folder.
+    def export_symlinks(self, dest_path=None, signatures=True, models=False):
+        """Creates symlinks for all available signatures H5 or models path
+           in a single folder.
 
         Args:
             dest_path (str): The destination for symlink, if None then the
                 default under the cc_root is generated.
+            signatures (bool): export signature files.
+            models (bool): export models paths.
         """
         if dest_path is None:
             dest_path = os.path.join(self.cc_root, 'sign_links')
 
         if not os.path.exists(dest_path):
             os.makedirs(dest_path)
 
-        for molset in ['full', 'reference']:
-            for cctype in ['sign0', 'sign1', 'sign2', 'sign3', 'sign4']:
-                for ds in self.coordinates:
-                    dataset_code = ds + '.001'
-                    sign = self.get_signature(cctype, molset, dataset_code)
-                    sign_file = sign.data_path
-
-                    if os.path.isfile(sign_file):
-                        dst_name = "_".join([cctype, dataset_code, molset])
-                        dst_name += ".h5"
-                        # Make a symlink into the destination
-                        symlink = os.path.join(dest_path, dst_name)
-                        try:
-                            os.symlink(sign_file, symlink)
-                        except Exception as ex:
-                            self.__log.warning(
-                                "Error creating %s: %s" % (symlink, str(ex)))
+        molsets = ['full', 'reference']
+        cctypes = ['sign0', 'sign1', 'sign2', 'sign3', 'sign4']
+        ds = self.coordinates
+        for molset, cctype, ds in itertools.product(molsets, cctypes, ds):
+            dataset_code = ds + '.001'
+            sign = self.get_signature(cctype, molset, dataset_code)
+            sign_file = sign.data_path
+
+            if signatures and os.path.isfile(sign_file):
+                dst_name = "_".join([cctype, dataset_code, molset])
+                dst_name += ".h5"
+                # Make a symlink into the destination
+                symlink = os.path.join(dest_path, dst_name)
+                try:
+                    os.symlink(sign_file, symlink)
+                except Exception as ex:
+                    self.__log.warning(
+                        "Error creating %s: %s" % (symlink, str(ex)))
+
+            model_path = os.path.join(sign.signature_path, 'models')
+            if models and os.path.isdir(model_path):
+                dst_name = "_".join([cctype, dataset_code, molset])
+                dst_name += ".models"
+                # Make a symlink into the destination
+                symlink = os.path.join(dest_path, dst_name)
+                try:
+                    os.symlink(model_path, symlink)
+                except Exception as ex:
+                    self.__log.warning(
+                        "Error creating %s: %s" % (symlink, str(ex)))
 
     def add_sign_metadata(self, molset='*', dataset='*', signature='*'):
         """Add metadata to available signatures.
 
         Args:
             molset (str, optional): Filter for the moleculeset e.g. 'full' or
                 'reference'
@@ -812,7 +1029,34 @@
                     for k, v in metadata.items():
                         if k in fh.attrs:
                             del fh.attrs[k]
                         fh.attrs.create(name=k, data=v)
             except Exception:
                 self.__log.warning("Could not add metadata to: %s" % path)
                 continue
+
+    def add_model_metadata(self, molsets=['full', 'reference'], dataset='*',
+                           signature='sign*'):
+        """Add metadata to available models.
+
+        Args:
+            molset (str, optional): Filter for the moleculeset e.g. 'full' or
+                'reference'
+            dataset (str, optional): Filter for the dataset e.g. A1.001
+            signature (str, optional): Filter for signature type e.g. 'sign1'
+        """
+        paths = list()
+        for molset in molsets:
+            paths.extend(self._available_sign_paths(molset, dataset, signature,
+                                                    'models'))
+        for path in paths:
+            molset = path.split('/')[-6]
+            dataset = path.split('/')[-3]
+            sign = path.split('/')[-2]
+            metadata = dict(cctype=sign, dataset_code=dataset, molset=molset)
+            metadata_file = os.path.join(path, 'metadata.json')
+            try:
+                with open(metadata_file, 'w') as fh:
+                    json.dump(metadata, fh)
+            except Exception:
+                self.__log.warning("Could not add metadata to: %s" % path)
+                continue
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/clus.py` & `chemicalchecker-1.0.3/chemicalchecker/core/clus.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,17 @@
             if "n_points" in params:
                 self.n_points = params["n_points"]
             if "balance" in params:
                 self.balance = params["balance"]
             if "significance" in params:
                 self.significance = params["significance"]
             if "type" in params:
-                self.significance = params["type"]
+                self.type = params["type"]
 
-    def fit(self, sign1=None, validations=True):
+    def fit(self, sign=None, validations=True):
         """Fit cluster model given a signature."""
         try:
             import faiss
         except ImportError:
             raise ImportError("requires faiss " +
                               "https://github.com/facebookresearch/faiss")
         try:
@@ -116,25 +116,25 @@
                               "https://hdbscan.readthedocs.io/en/latest/")
         BaseSignature.fit(self)
 
         plot = Plot(self.dataset, self.stats_path)
 
         mappings = None
 
-        if sign1 is None:
-            sign1 = self.get_sign(
+        if sign is None:
+            sign = self.get_sign(
                 'sign' + self.cctype[-1]).get_molset("reference")
 
-        if os.path.isfile(sign1.data_path):
-            self.data = sign1.data.astype(np.float32)
+        if os.path.isfile(sign.data_path):
+            self.data = sign.data.astype(np.float32)
             self.data_type = self.data.dtype
-            self.keys = sign1.keys
-            mappings = sign1.mappings
+            self.keys = sign.keys
+            mappings = sign.mappings
         else:
-            raise Exception("The file " + sign1.data_path + " does not exist")
+            raise Exception("The file " + sign.data_path + " does not exist")
 
         tmp_dir = tempfile.mkdtemp(
             prefix='clus_' + self.dataset + "_", dir=Config().PATH.CC_TMP)
 
         self.__log.debug("Temporary files saved in " + tmp_dir)
 
         if self.type == "hdbscan":
@@ -193,15 +193,15 @@
 
             self.metric = "hdbscan"
 
         if self.type == "kmeans":
 
             faiss.omp_set_num_threads(self.cpu)
 
-            with h5py.File(sign1.data_path, 'r') as dh5:
+            with h5py.File(sign.data_path, 'r') as dh5:
                 if "elbow" not in dh5.keys():
                     Vn, Vm = self.data.shape[0], self.data.shape[1] / 2
                 else:
                     Vn, Vm = self.data.shape[0], dh5["elbow"][0]
 
             if self.metric == "cosine":
                 self.data = self._normalizer(self.data, False)
@@ -222,15 +222,15 @@
             if self.k_neig is None:
 
                 cluster_range = np.arange(self.min_k, self.max_k, step=np.max(
                     [int((self.max_k - self.min_k) / self.n_points), 1]))
 
                 inertias = []
                 disps = []
-                bg_distances = sign1.background_distances(self.metric)
+                bg_distances = sign.background_distances(self.metric)
 
                 pvals = bg_distances["pvalue"]
                 distance = bg_distances["distance"]
 
                 sig_dist = distance[
                     bisect.bisect_left(pvals, self.significance)]
 
@@ -346,15 +346,15 @@
                     mappings, DataSignature.string_dtype()))
         # also predict for full if available
         sign_full = self.get_sign('sign' + self.cctype[-1]).get_molset("full")
         if os.path.isfile(sign_full.data_path):
             self.predict(sign_full, self.get_molset("full").data_path)
         self.mark_ready()
 
-    def predict(self, sign1, destination=None, validations=False):
+    def predict(self, sign, destination=None, validations=False):
         """Use the fitted models to go from input to output."""
         try:
             import faiss
         except ImportError:
             raise ImportError("requires faiss " +
                               "https://github.com/facebookresearch/faiss")
         try:
@@ -363,28 +363,28 @@
             raise ImportError("requires hdbscan " +
                               "https://hdbscan.readthedocs.io/en/latest/")
 
         plot = Plot(self.dataset, self.stats_path)
 
         mappings = None
 
-        if os.path.isfile(sign1.data_path):
-            self.data = sign1.data.astype(np.float32)
+        if os.path.isfile(sign.data_path):
+            self.data = sign.data.astype(np.float32)
             self.data_type = self.data.dtype
-            self.keys = sign1.keys
-            mappings = sign1.mappings
+            self.keys = sign.keys
+            mappings = sign.mappings
         else:
-            raise Exception("The file " + sign1.data_path + " does not exist")
+            raise Exception("The file " + sign.data_path + " does not exist")
 
         if destination is None:
             raise Exception(
                 "Predict method requires a destination file to output results")
 
         tmp_dir = tempfile.mkdtemp(
-            prefix='sign1_' + self.dataset + "_", dir=Config().PATH.CC_TMP)
+            prefix='sign_' + self.dataset + "_", dir=Config().PATH.CC_TMP)
 
         self.__log.debug("Temporary files saved in " + tmp_dir)
 
         if self.type == "hdbscan":
             self.__log.info("Reading HDBSCAN clusters")
 
             clusterer = joblib.load(os.path.join(
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/data.py` & `chemicalchecker-1.0.3/chemicalchecker/core/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,18 @@
         from .sign2 import sign2
         from .sign3 import sign3
         from .sign4 import sign4
 
         from .clus import clus
         from .neig import neig  # nearest neighbour class
         from .proj import proj
+        from .char import char  # CC space charts
 
         # DataFactory.__log.debug("initializing object %s", cctype)
-        if cctype[:4] in ['clus', 'neig', 'proj','diag']:
+        if cctype[:4] in ['clus', 'neig', 'proj', 'diag', 'char']:
             # NS, will return an instance of neig or of sign0 etc
             return eval(cctype[:4])(*args, **kwargs)
         else:
             return eval(cctype)(*args, **kwargs)
 
     @staticmethod
     def signaturize(cctype, signature_path, matrix, keys=None, dataset_code=None):
@@ -63,14 +64,15 @@
         from .sign3 import sign3
         from .sign4 import sign4
         from .signature_data import DataSignature
 
         from .clus import clus
         from .neig import neig
         from .proj import proj
+        from .char import char
 
         data_path = os.path.join(signature_path, '%s.h5' % cctype)
         if not keys:
             keys = ["{0:027d}".format(n) for n in range(len(matrix))]
         if not dataset_code:
             dataset_code = "XX.001"
         with h5py.File(data_path, 'w') as hf:
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/diagnostics.py` & `chemicalchecker-1.0.3/chemicalchecker/core/diagnostics.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import collections
 import numpy as np
 import tempfile
 from sklearn.cluster import DBSCAN
 from scipy.stats import gaussian_kde
 from scipy.spatial.distance import pdist
 from sklearn.decomposition import PCA
-from sklearn.metrics import roc_curve, auc
+from sklearn.metrics import roc_curve, auc, precision_recall_curve, average_precision_score
 from sklearn.preprocessing import normalize
 from sklearn.ensemble import IsolationForest
 from sklearn.neighbors import NearestNeighbors
 
 from chemicalchecker.util import logged, Config
 from chemicalchecker.util.plot import DiagnosisPlot
 #from chemicalchecker.util.decorator import safe_return
@@ -168,15 +168,16 @@
 
     def _select_datasets(self, datasets, exemplary):
         if datasets is None:
             datasets = self.ref_cc.datasets
         dss = []
         for ds in datasets:
             if exemplary:
-                if ds[0] in "ABCDE" and ds[-3:] == "001":
+                # TODO: to change in case of CC expansion from 25 spaces
+                if ds[0] in "ABCDE" and ds[1] in "12345" and ds[-3:] == "001":
                     dss += [ds]
             else:
                 dss += [ds]
         return dss
 
     def _get_signatures(self, *args, keys=None, max_keys=10000,
                         max_features=None, shuffle=False, **kwargs):
@@ -248,26 +249,28 @@
         cfg = Config(cc_config)
         job_name = "_".join(["CC", self.sign.cctype.upper(), self.sign.dataset,
                              "DIAGNOSIS"])
         job_path = tempfile.mkdtemp("_" + job_name, dir=tmpdir)
         # create job directory if not available
         if not os.path.isdir(job_path):
             os.mkdir(job_path)
+        # in case some plots of the canvases must be skipped
+        skip_plots = kwargs.get("skip_plots", [])
         # create script file
-        script_lines = """
+        script_lines = f"""
 import sys, os
 import pickle
 from chemicalchecker import ChemicalChecker
 from chemicalchecker.core.diagnostics import Diagnosis
 ChemicalChecker.set_verbosity('DEBUG')
 task_id = sys.argv[1]
 filename = sys.argv[2]
 diag = pickle.load(open(filename, 'rb'))[task_id][0]
-diag.canvas(size='small', savefig=True)
-diag.canvas(size='medium', savefig=True)
+diag.canvas(size='small', savefig=True, skip_plots={skip_plots})
+diag.canvas(size='medium', savefig=True, skip_plots={skip_plots})
 print('JOB DONE')
         """
         script_name = os.path.join(job_path, 'diagnostics_script.py')
         with open(script_name, 'w') as fh:
             fh.write(script_lines)
         # HPC parameters
         params = kwargs
@@ -448,28 +451,29 @@
             plotter_function=self.plotter.cross_coverage,
             kw_plotter={"sign_qualified_name": qualified_name},
             **kwargs)
 
     # @safe_return(None)
     def cross_roc(self, sign, *args, n_samples=10000, n_neighbors=5,
                   neg_pos_ratio=1, apply_mappings=False, try_conn_layer=False,
-                  metric='cosine', redo=False, **kwargs):
+                  metric='cosine', redo=False, val_type='roc', **kwargs):
         """Perform validations.
 
         Args:
             sign (signature): A CC signature object to validate against.
             n_samples (int): Number of samples.
             apply_mappings (bool): Whether to use mappings to compute
                 validation. Signature which have been redundancy-reduced
                 (i.e. `reference`) have fewer molecules. The key are molecules
                 from the `full` signature and values are molecules from the
                 `reference` set.
             try_conn_layer (bool): Try with the inchikey connectivity layer.
                 (default=False)
             metric (str): 'cosine' or 'euclidean'. (default='cosine')
+            val_type (str): 'roc' or 'pr'. (default='roc')
             save (bool): Specific save parameter. If not specified, the global
                 is set. (default=None).
         """
         fn = os.path.join(self.path, "cross_roc_%s" %
                           sign.qualified_name)
         if self._todo(fn) or redo:
             r = self.cross_coverage(sign.dataset, ref_cctype=sign.cctype,
@@ -539,32 +543,42 @@
             # correct negative/positive ratio
             if len(neg_dists) > len(pos_dists) * neg_pos_ratio:
                 np.random.shuffle(neg_dists)
                 neg_dists = neg_dists[:int(len(pos_dists) * neg_pos_ratio)]
             else:
                 np.random.shuffle(pos_dists)
                 pos_dists = pos_dists[:int(len(neg_dists) / neg_pos_ratio)]
-            # final arrays for performnce calculation
+            # final arrays for performance calculation
             y_t = np.array([1] * len(pos_dists) + [0] * len(neg_dists))
             y_p = np.hstack([pos_dists, neg_dists])
             # convert to similarity-respected order
             y_p = -np.abs(np.array(y_p))
             # roc calculation
             fpr, tpr, _ = roc_curve(y_t, y_p)
+            # pr calculation
+            precision, recall, _ = precision_recall_curve(y_t, y_p)
+            # write results dictionary
             results = {
                 "fpr": fpr,
                 "tpr": tpr,
                 "auc": auc(fpr, tpr),
+                "precision": precision,
+                "recall": recall,
+                "average_precision_score": average_precision_score(y_t, y_p)
             }
         else:
             results = None
+        if val_type == 'pr':
+            plotter_function_arg = self.plotter.cross_pr
+        else:
+            plotter_function_arg = self.plotter.cross_roc
         return self._returner(
             results=results,
             fn=fn,
-            plotter_function=self.plotter.cross_roc,
+            plotter_function=plotter_function_arg,
             kw_plotter={"sign": sign},
             **kwargs)
 
     # @safe_return(None)
     def projection(self, *args, keys=None, focus_keys=None, max_keys=10000,
                    perplexity=None, max_pca=100, redo=False, **kwargs):
         """TSNE projection of CC signatures.
@@ -581,14 +595,18 @@
         fn = "projection"
         if self._todo(fn) or redo:
             from MulticoreTSNE import MulticoreTSNE as TSNE
             X, keys = self._get_signatures(keys=keys, max_keys=max_keys)
             self.__log.debug("Fit-transforming t-SNE")
             if X.shape[1] > max_pca:
                 self.__log.debug("First doing a PCA")
+                # check on max_pca value
+                min_samples_features = min(X.shape[0], X.shape[1])
+                if min_samples_features <= max_pca:
+                    max_pca = min_samples_features
                 X = PCA(n_components=max_pca).fit_transform(X)
             init = PCA(n_components=2).fit_transform(X)
             if perplexity is None:
                 perp = int(np.sqrt(X.shape[0]))
                 perp = np.max([5, perp])
                 perp = np.min([50, perp])
             self.__log.debug("Chosen perplexity %d" % perp)
@@ -1011,14 +1029,21 @@
                         metric="minkowski", p=0.9, **kwargs):
         """Sample-specific accuracy.
 
         Estimated as general agreement with the rest of the CC.
         """
         self.__log.debug("Sample-specific agreement to the rest of CC")
         fn = "ranks_agreement"
+
+        if self.sign.shape[0] < min_shared:
+            min_shared = 0.7 * self.sign.shape[0]
+            # self.__log.debug("Not enough molecules in the dataset to generate ranks agreement: \n\
+            #        dataset molecules {}, min_shared molecules {} ".format(self.sign.shape[0], min_shared))
+            # return None
+
         if ref_cctype is None:
             ref_cctype = self.sign.cctype
 
         def q67(r):
             return np.percentile(r, 67)
 
         def stat(R, func):
@@ -1104,14 +1129,23 @@
         Z-global ranking.
         """
         self.__log.debug(
             "Sample-specific agreement to the rest of CC,"
             " based on a Z-global ranking")
         fn = "global_ranks_agreement"
 
+        # to take into consideration the case of very small datasets
+        # with less than min_shared molecules
+        if self.sign.shape[0] < min_shared:
+            # TODO: is this plot significant anyways?
+            min_shared = 0.7 * self.sign.shape[0]
+            # self.__log.debug("Not enough molecules in the dataset to generate global ranks agreement: \n\
+            #        dataset molecules {}, min_shared molecules {} ".format(self.sign.shape[0], min_shared))
+            # return None
+
         if ref_cctype is None:
             ref_cctype = self.ref_cctype
         exemplary_datasets = self._select_datasets(None, True)
         datasets = kwargs.get("datasets", exemplary_datasets)
 
         def q67(r):
             return np.percentile(r, 67)
@@ -1184,38 +1218,44 @@
             results=results,
             fn=fn,
             plotter_function=self.plotter.global_ranks_agreement_projection,
             **kwargs)
 
     # @safe_return(None)
     def across_roc(self, *args, datasets=None, exemplary=True, ref_cctype=None,
-                   redo=False, **kwargs):
+                   redo=False, include_datasets=None, **kwargs):
         """Check coverage against a collection of other CC signatures.
 
         Args:
             datasets (list): List of datasets. If None, all available are used.
                 (default=None).
             exemplary (bool): Whether to use only exemplary datasets
                 (recommended). (default=True)
-            cctype (str): CC signature type. (default='sign0')
-            molset (str): Molecule set to use. Full is recommended.
-                (default='full')
-            kwargs (dict): Parameters of hte cross_coverage method.
+            ref_cctype (str): CC signature type. (default='sign0')
+            redo (bool): redo the plot
+            include_datasets (list): specific datasets to add when exemplary 
+                                     is set to True (default=None)
+            kwargs (dict): Parameters of the cross_roc method.
         """
         self.__log.debug("Across ROC")
         fn = "across_roc"
         if ref_cctype is None:
             ref_cctype = self.ref_cctype
         if self._todo(fn) or redo:
             datasets = self._select_datasets(datasets, exemplary)
             results = {}
             for ds in datasets:
                 sign = self.ref_cc.signature(ds, ref_cctype)
                 results[ds] = self.cross_roc(sign, save=False, redo=True,
                                              plot=False)
+            if include_datasets and exemplary:
+                for incl_ds in include_datasets:
+                    sign = self.ref_cc.signature(incl_ds, ref_cctype)
+                    results[incl_ds] = self.cross_roc(sign, save=False, redo=True,
+                                                      plot=False)
         else:
             results = None
         return self._returner(
             results=results,
             fn=fn,
             plotter_function=self.plotter.across_roc,
             kw_plotter={
@@ -1296,25 +1336,45 @@
     def roc(self, ds, *args, ref_cctype=None, redo=False, **kwargs):
         self.__log.debug("ROC")
         fn = "roc"
         if ref_cctype is None:
             ref_cctype = self.ref_cctype
         if self._todo(fn) or redo:
             sign = self.ref_cc.signature(ds, ref_cctype)
-            results = self.cross_roc(sign, redo=True, save=False, plot=False)
+            results = self.cross_roc(
+                sign, redo=True, save=False, plot=False, val_type='roc')
         else:
             results = None
         return self._returner(
             results=results,
             fn=fn,
             plotter_function=self.plotter.roc,
             kw_plotter={"ds": ds},
             **kwargs)
 
     # @safe_return(None)
+    def pr(self, ds, *args, ref_cctype=None, redo=False, **kwargs):
+        self.__log.debug("PrecisionRecall")
+        fn = "pr"
+        if ref_cctype is None:
+            ref_cctype = self.ref_cctype
+        if self._todo(fn) or redo:
+            sign = self.ref_cc.signature(ds, ref_cctype)
+            results = self.cross_roc(
+                sign, redo=True, save=False, plot=False, val_type='pr')
+        else:
+            results = None
+        return self._returner(
+            results=results,
+            fn=fn,
+            plotter_function=self.plotter.pr,
+            kw_plotter={"ds": ds},
+            **kwargs)
+
+    # @safe_return(None)
     def redundancy(self, *args, **kwargs):
         self.__log.debug("Redundancy")
         fn = "redundancy"
         if self._todo(fn):
             from chemicalchecker.util.remove_near_duplicates import RNDuplicates
             self.__log.debug("Removing near duplicates")
             rnd = RNDuplicates(cpu=self.cpu)
@@ -1357,15 +1417,17 @@
         else:
             n_neighbors = [n_neighbors]
 
         def do_clustering(n_neigh):
             nn = NearestNeighbors(n_neighbors=n_neigh + 1, n_jobs=self.cpu)
             nn.fit(P)
             dists = nn.kneighbors(P)[0][:, n_neigh]
-            h = np.histogram(dists, bins="auto")
+            # FIXME: bins='auto' is preferable, but might trigger memory
+            # errors e.g. C3 sign1
+            h = np.histogram(dists, bins=100)
             y = np.cumsum(h[0]) / np.sum(h[0])
             x = h[1][1:]
             eps = x[np.where(y > expected_coverage)[0][0]]
             self.__log.debug("Running DBSCAN")
             cl = DBSCAN(eps=eps, min_samples=min_samples,
                         n_jobs=self.cpu).fit(P)
             labels = cl.labels_
@@ -1546,74 +1608,132 @@
             fn=fn,
             plotter_function=self.plotter.outliers,
             **kwargs)
 
     def available(self):
         return self.plotter.available()
 
-    def canvas_small(self, title=None):
+    def canvas_small(self, title=None, skip_plots=[]):
         shared_kw = dict(save=True, plot=False)
+        if "cosine_distances" not in skip_plots:
+            self.cosine_distances(**shared_kw)
+        if "euclidean_distances" not in skip_plots:
+            self.euclidean_distances(**shared_kw)
+        if "projection" not in skip_plots:
+            self.projection(**shared_kw)
+        if "image" not in skip_plots:
+            self.image(**shared_kw)
+        if "features_bins" not in skip_plots:
+            self.features_bins(**shared_kw)
+        if "keys_bins" not in skip_plots:
+            self.keys_bins(**shared_kw)
+        if "values" not in skip_plots:
+            self.values(**shared_kw)
+        if "redundancy" not in skip_plots:
+            self.redundancy(**shared_kw)
 
-        self.cosine_distances(**shared_kw)
-        self.euclidean_distances(**shared_kw)
-        self.projection(**shared_kw)
-        self.image(**shared_kw)
-        self.features_bins(**shared_kw)
-        self.keys_bins(**shared_kw)
-        self.values(**shared_kw)
-        self.redundancy(**shared_kw)
+        fig = self.plotter.canvas(
+            size="small", title=title, skip_plots=skip_plots)
+        return fig
+
+    def canvas_medium(self, title=None, skip_plots=[]):
+        shared_kw = dict(save=True, plot=False)
+
+        if "cosine_distances" not in skip_plots:
+            self.cosine_distances(**shared_kw)
+        if "euclidean_distances" not in skip_plots:
+            self.euclidean_distances(**shared_kw)
+        if "projection" not in skip_plots:
+            self.projection(**shared_kw)
+        if "image" not in skip_plots:
+            self.image(**shared_kw)
+        if "features_bins" not in skip_plots:
+            self.features_bins(**shared_kw)
+        if "keys_bins" not in skip_plots:
+            self.keys_bins(**shared_kw)
+        if "values" not in skip_plots:
+            self.values(**shared_kw)
+        if "redundancy" not in skip_plots:
+            self.redundancy(**shared_kw)
+        if "intensities" and "intensities_projection" not in skip_plots:
+            self.intensities(**shared_kw)
+            if "intensities_projection" not in skip_plots:
+                self.intensities_projection(**shared_kw)
+        if self.sign.cctype == 'sign3':
+            if "confidences" not in skip_plots:
+                self.confidences(**shared_kw)
+                if "confidences_projection" not in skip_plots:
+                    self.confidences_projection(**shared_kw)
+        if "cluster_sizes" not in skip_plots:
+            self.cluster_sizes(**shared_kw)
+            if "clusters_projection" not in skip_plots:
+                self.clusters_projection(**shared_kw)
+        if "outliers" not in skip_plots:
+            self.outliers(**shared_kw)
 
-        fig = self.plotter.canvas(size="small", title=title)
+        # these plots requires CC wide metadata
+        if "dimensions" not in skip_plots:
+            self.dimensions(**shared_kw)
+        if "key_coverage" not in skip_plots:
+            self.key_coverage(**shared_kw)
+            if "key_coverage_projection" not in skip_plots:
+                self.key_coverage_projection(**shared_kw)
+        if "across_coverage" not in skip_plots:
+            self.across_coverage(**shared_kw)
+        # these plots requires CC wide signatures
+        if "atc_roc" not in skip_plots:
+            self.atc_roc(**shared_kw)
+        if "moa_roc" not in skip_plots:
+            self.moa_roc(**shared_kw)
+        if "across_roc" not in skip_plots:
+            self.across_roc(**shared_kw)
+        if self.global_ranks_agreement(**shared_kw) is None:
+            self.__log.debug(
+                "Skipping plots Global Ranks Agreement and Global Ranks Agreement Projection")
+            skip_plots.extend("global_ranks_agreement", 
+                              "global_ranks_agreement_projection")
+        else:
+            self.global_ranks_agreement_projection(**shared_kw)
+
+        fig = self.plotter.canvas(
+            size="medium", title=title, skip_plots=skip_plots)
         return fig
 
-    def canvas_medium(self, title=None):
+    def custom_comparative_vertical(self, title=None, skip_plots=[]):
         shared_kw = dict(save=True, plot=False)
 
-        self.cosine_distances(**shared_kw)
-        self.euclidean_distances(**shared_kw)
         self.projection(**shared_kw)
-        self.image(**shared_kw)
-        self.features_bins(**shared_kw)
-        self.keys_bins(**shared_kw)
-        self.values(**shared_kw)
-        self.redundancy(**shared_kw)
-
         self.intensities(**shared_kw)
-        self.intensities_projection(**shared_kw)
         if self.sign.cctype == 'sign3':
             self.confidences(**shared_kw)
-            self.confidences_projection(**shared_kw)
-        self.cluster_sizes(**shared_kw)
         self.clusters_projection(**shared_kw)
-        self.outliers(**shared_kw)
-
-        # these plots requires CC wide metadata
-        self.dimensions(**shared_kw)
-        self.key_coverage(**shared_kw)
-        self.key_coverage_projection(**shared_kw)
-        self.across_coverage(**shared_kw)
-        # these plots requires CC wide signatures
         self.atc_roc(**shared_kw)
         self.moa_roc(**shared_kw)
         self.across_roc(**shared_kw)
-        self.global_ranks_agreement(**shared_kw)
-        self.global_ranks_agreement_projection(**shared_kw)
 
-        fig = self.plotter.canvas(size="medium", title=title)
+        fig = self.plotter.canvas(
+            size="compare_v", title=title, skip_plots=skip_plots)
         return fig
 
+    def canvas_large(self, title=None, skip_plots=[]):
+        pass
+
     def canvas(self, size="medium", title=None, savefig=False, dest_dir=None,
-               savefig_kwargs={'facecolor': 'white'}):
+               savefig_kwargs={'facecolor': 'white'}, skip_plots=[]):
         self.__log.debug("Computing or retrieving data for canvas %s." % size)
+        self.__log.debug("Skipping the following plots: %s" % skip_plots)
         if size == "small":
-            fig = self.canvas_small(title=title)
+            fig = self.canvas_small(title=title, skip_plots=skip_plots)
         elif size == "medium":
-            fig = self.canvas_medium(title=title)
+            fig = self.canvas_medium(title=title, skip_plots=skip_plots)
         elif size == "large":
-            fig = self.canvas_large(title=title)
+            fig = self.canvas_large(title=title, skip_plots=skip_plots)
+        elif size == "compare_v":
+            fig = self.custom_comparative_vertical(
+                title=title, skip_plots=skip_plots)
         else:
             return None
         if savefig:
             fn = "_".join([self.sign.dataset, self.sign.cctype,
                            self.name, size]) + '.png'
             if dest_dir is None:
                 fn_dest = os.path.join(self.path, fn)
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/examples/ctrp_auc.csv` & `chemicalchecker-1.0.3/chemicalchecker/core/examples/ctrp_auc.csv`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/examples/fps.pkl` & `chemicalchecker-1.0.3/chemicalchecker/core/examples/fps.pkl`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/examples/pharmacodb_targets.tsv` & `chemicalchecker-1.0.3/chemicalchecker/core/examples/pharmacodb_targets.tsv`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/examples/toy_matrix.pkl` & `chemicalchecker-1.0.3/chemicalchecker/core/examples/toy_matrix.pkl`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/examples/toy_pairs.pkl` & `chemicalchecker-1.0.3/chemicalchecker/core/examples/toy_pairs.pkl`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/examples/validation_sets/atc_validation.tsv` & `chemicalchecker-1.0.3/chemicalchecker/core/examples/validation_sets/atc_validation.tsv`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/examples/validation_sets/moa_validation.tsv` & `chemicalchecker-1.0.3/chemicalchecker/core/examples/validation_sets/moa_validation.tsv`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/examples.py` & `chemicalchecker-1.0.3/chemicalchecker/core/examples.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/neig.py` & `chemicalchecker-1.0.3/chemicalchecker/core/neig.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,43 +56,43 @@
             if "cpu" in params:
                 self.cpu = params["cpu"]
             if "k_neig" in params:
                 self.k_neig = params["k_neig"]
             if "chunk" in params:
                 self.chunk = params["chunk"]
 
-    def fit(self, sign1=None):
+    def fit(self, sign=None):
         """Fit neighbor model given a signature."""
         try:
             import faiss
         except ImportError:
             raise ImportError("requires faiss " +
                               "https://github.com/facebookresearch/faiss")
 
         # signature specific checks
         if self.molset != "reference":
             self.__log.debug("Fit will be done with the reference neig1")
             self = self.get_molset("reference")
-        if sign1 is None:
-            sign1 = self.get_sign(
+        if sign is None:
+            sign = self.get_sign(
                 'sign' + self.cctype[-1]).get_molset("reference")
-        if sign1.molset != "reference":
-            self.__log.debug("Fit will be done with the reference sign1")
-            sign1 = self.get_sign(
+        if sign.molset != "reference":
+            self.__log.debug("Fit will be done with the reference sign")
+            sign = self.get_sign(
                 'sign' + self.cctype[-1]).get_molset("reference")
-        if not sign1.is_fit():
-            raise Exception("sign1 is not fitted.")
+        if not sign.is_fit():
+            raise Exception("sign is not fitted.")
 
         faiss.omp_set_num_threads(self.cpu)
 
-        if os.path.isfile(sign1.data_path):
-            with h5py.File(sign1.data_path, 'r') as dh5, h5py.File(self.data_path, 'w') as dh5out:
+        if os.path.isfile(sign.data_path):
+            with h5py.File(sign.data_path, 'r') as dh5, h5py.File(self.data_path, 'w') as dh5out:
                 if "keys" not in dh5.keys() or "V" not in dh5.keys():
                     raise Exception(
-                        "H5 file " + sign1.data_path + " does not contain datasets 'keys' and 'V'")
+                        "H5 file " + sign.data_path + " does not contain datasets 'keys' and 'V'")
 
                 self.datasize = dh5["V"].shape
                 self.data_type = dh5["V"].dtype
 
                 k = min(self.datasize[0], self.k_neig)
 
                 dh5out.create_dataset("row_keys", data=dh5["keys"][:])
@@ -108,65 +108,65 @@
                     "metric", data=[self.metric.encode(encoding='UTF-8', errors='strict')])
 
                 if self.metric == "euclidean":
                     index = faiss.IndexFlatL2(self.datasize[1])
                 else:
                     index = faiss.IndexFlatIP(self.datasize[1])
 
-                for chunk in sign1.chunker():
+                for chunk in sign.chunker():
                     data_temp = np.array(dh5["V"][chunk], dtype=np.float32)
                     if self.metric == "cosine":
                         normst = LA.norm(data_temp, axis=1)
                         index.add(data_temp / normst[:, None])
                     else:
                         index.add(data_temp)
 
-                for chunk in sign1.chunker():
+                for chunk in sign.chunker():
                     data_temp = np.array(dh5["V"][chunk], dtype=np.float32)
                     if self.metric == "cosine":
                         normst = LA.norm(data_temp, axis=1)
                         Dt, It = index.search(data_temp / normst[:, None], k)
                     else:
                         Dt, It = index.search(data_temp, k)
 
                     dh5out["indices"][chunk] = It
                     if self.metric == "cosine":
                         dh5out["distances"][chunk] = np.maximum(0.0, 1.0 - Dt)
                     else:
                         dh5out["distances"][chunk] = Dt
 
         else:
-            raise Exception("The file " + sign1.data_path + " does not exist")
+            raise Exception("The file " + sign.data_path + " does not exist")
 
         faiss.write_index(index, self.index_filename)
 
         # also predict for full if available
         sign_full = self.get_sign('sign' + self.cctype[-1]).get_molset("full")
         if os.path.isfile(sign_full.data_path):
             self.predict(sign_full, self.get_molset("full").data_path)
         self.mark_ready()
 
-    def predict(self, sign1, destination=None, validations=False):
+    def predict(self, sign, destination=None, validations=False):
         """Use the fitted models to go from input to output."""
         try:
             import faiss
         except ImportError:
             raise ImportError("requires faiss " +
                               "https://github.com/facebookresearch/faiss")
 
         if destination is None:
             raise Exception("There is no destination file specified")
 
         faiss.omp_set_num_threads(self.cpu)
 
-        if os.path.isfile(sign1.data_path):
-            with h5py.File(sign1.data_path, 'r') as dh5, h5py.File(destination, 'w') as dh5out:
+        if os.path.isfile(sign.data_path):
+            with h5py.File(sign.data_path, 'r') as dh5, h5py.File(destination, 'w') as dh5out:
                 if "keys" not in dh5.keys() or "V" not in dh5.keys():
                     raise Exception(
-                        "H5 file " + sign1.data_path + " does not contain datasets 'keys' and 'V'")
+                        "H5 file " + sign.data_path + " does not contain datasets 'keys' and 'V'")
 
                 self.datasize = dh5["V"].shape
                 self.data_type = dh5["V"].dtype
 
                 index = faiss.read_index(self.index_filename)
 
                 k = min(self.k_neig, index.ntotal)
@@ -180,15 +180,15 @@
                     "distances", (self.datasize[0], k), dtype=np.float32)
                 dh5out.create_dataset("shape", data=(self.datasize[0], k))
                 dh5out.create_dataset(
                     "date", data=[datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S").encode(encoding='UTF-8', errors='strict')])
                 dh5out.create_dataset(
                     "metric", data=[self.metric.encode(encoding='UTF-8', errors='strict')])
 
-                for chunk in sign1.chunker():
+                for chunk in sign.chunker():
                     data_temp = np.array(dh5["V"][chunk], dtype=np.float32)
 
                     if self.metric == "cosine":
                         normst = LA.norm(data_temp, axis=1)
                         Dt, It = index.search(data_temp / normst[:, None], k)
                     else:
                         Dt, It = index.search(data_temp, k)
@@ -196,15 +196,15 @@
                     dh5out["indices"][chunk] = It
                     if self.metric == "cosine":
                         dh5out["distances"][chunk] = np.maximum(0.0, 1.0 - Dt)
                     else:
                         dh5out["distances"][chunk] = Dt
 
         else:
-            raise Exception("The file " + sign1.data_path + " does not exist")
+            raise Exception("The file " + sign.data_path + " does not exist")
 
     @cached_property
     def keys(self):
         """Get the list of keys (usually inchikeys) in the signature."""
         self._check_data()
         self._check_dataset('row_keys')
         return self._get_all('row_keys')
@@ -232,30 +232,30 @@
 
         if not os.path.isfile(self.data_path):
             raise Exception("Data file not available.")
         if isinstance(key, slice):
             with h5py.File(self.data_path, 'r') as hf:
                 predictions["indices"] = hf['indices'][key]
                 predictions["distances"] = hf['distances'][key]
-                keys = hf['col_keys'][:]
+                keys = hf['col_keys'][:].astype(str)
                 predictions["keys"] = keys[predictions["indices"]]
         elif isinstance(key, str):
             if key not in self.unique_keys:
                 raise Exception("Key '%s' not found." % key)
             idx = bisect_left(self.keys, key)
             with h5py.File(self.data_path, 'r') as hf:
                 predictions["indices"] = hf['indices'][idx]
                 predictions["distances"] = hf['distances'][idx]
-                keys = hf['col_keys'][:]
+                keys = hf['col_keys'][:].astype(str)
                 predictions["keys"] = keys[predictions["indices"]]
         elif isinstance(key, int):
             with h5py.File(self.data_path, 'r') as hf:
                 predictions["indices"] = hf['indices'][key]
                 predictions["distances"] = hf['distances'][key]
-                keys = hf['col_keys'][:]
+                keys = hf['col_keys'][:].astype(str)
                 predictions["keys"] = keys[predictions["indices"]]
         else:
             raise Exception("Key type %s not recognized." % type(key))
 
         return predictions
 
     def get_vectors(self, keys, include_nan=False, dataset_name='indices'):
@@ -302,15 +302,15 @@
         if len(inks) == 0:
             self.__log.warn("No requested keys available!")
             return None, None
         inks, signs = np.stack(inks), np.vstack(signs)
         sort_idx = np.argsort(inks)
         return inks[sort_idx], signs[sort_idx]
 
-    def get_kth_nearest(self, signatures, k=None, distances=True, keys=True):
+    def get_kth_nearest(self, signatures, k=1000, distances=True, keys=True):
         """Return up to the k-th nearest neighbor.
 
         This function returns the k-th closest neighbor.
         A k>1 is useful when we expect and want to exclude a perfect match,
         i.e. when the signature we query for are the same that have been used
         to generate the neighbors.
 
@@ -357,15 +357,15 @@
             dists, idx = index.search(data, k)
 
         predictions = dict()
         predictions["indices"] = idx
         if keys:
             with h5py.File(self.data_path, 'r') as hf:
                 keys = hf['col_keys'][:]
-            predictions["keys"] = keys[idx]
+            predictions["keys"] = keys[idx].astype(str)
         if distances:
 
             predictions["distances"] = dists
             if metric_orig == "cosine":
 
                 predictions["distances"] = np.maximum(
                     0.0, 1.0 - predictions["distances"])
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/preprocess.py` & `chemicalchecker-1.0.3/chemicalchecker/core/preprocess.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/proj.py` & `chemicalchecker-1.0.3/chemicalchecker/core/proj.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/projector/default.py` & `chemicalchecker-1.0.3/chemicalchecker/core/projector/default.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/projector/pca.py` & `chemicalchecker-1.0.3/chemicalchecker/core/projector/pca.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/projector/tsne.py` & `chemicalchecker-1.0.3/chemicalchecker/core/projector/tsne.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/projector/umap_.py` & `chemicalchecker-1.0.3/chemicalchecker/core/projector/umap_.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/sign0.py` & `chemicalchecker-1.0.3/chemicalchecker/core/sign0.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,16 +400,15 @@
             hf.create_dataset("agg_method", data=np.array(
                 [str(agg_method)], DataSignature.string_dtype()))
             hf.create_dataset("input_type", data=np.array(
                 [str(input_type)], DataSignature.string_dtype()))
 
         self.refresh()
         # save reference
-        overwrite = kwargs.get('overwrite', False)
-        self.save_reference(overwrite=overwrite)
+        self.save_reference(overwrite=True)
         # Making triplets
         if do_triplets:
             self.update_status("Sampling triplets")
             cc = self.get_cc(cc_root)
             sampler = TripletSampler(cc, self, save=True)
             sampler.sample(**kwargs)
         # finalize signature
@@ -431,15 +430,14 @@
             features(array): Column names (default=None).
             merge(bool): Merge queried data with the currently existing one.
             merge_method(str): Merging method to be applied when a repeated key
                 is found. Can be 'average', 'old' or 'new' (default=new).
             destination(str): Path to the H5 file. If none specified, a
                 (V, keys, features) tuple is returned.
         """
-        assert self.is_fit(), "Signature is not fitted yet"
         self.__log.info("Predict START")
         if merge:
             self.__log.info("Merging. Loading existing signature.")
             V_ = self[:]
             keys_ = self.keys
             keys_raw_ = self.keys_raw
             if merge_method is not None:
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/sign1.py` & `chemicalchecker-1.0.3/chemicalchecker/core/sign1.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from tqdm import tqdm
 from numpy import linalg as LA
 from scipy.signal import savgol_filter
 from scipy.spatial.distance import cosine
 from sklearn.metrics import accuracy_score
 
 from .chemcheck import ChemicalChecker
+from chemicalchecker.util import Config
 from .signature_data import DataSignature
 from .signature_base import BaseSignature
 
 from chemicalchecker.util import logged
 from chemicalchecker.util.transform.pca import Pca
 from chemicalchecker.util.transform.scale import Scale
 
@@ -249,14 +250,16 @@
         with open(fn, "rb") as f:
             pipeline = pickle.load(f)
         self.__log.debug("Starting pipeline")
         if not pipeline["sparse"] and pipeline["scale"]:
             self.__log.debug("Scaling")
             mod = self.load_model("scale")
             mod.model_path = self.model_path
+            # using the config path for the CC_TMP and not the generated model one
+            mod.tmp_path = Config().PATH.CC_TMP
             mod.predict(destination)
 
         self.__log.debug("Transformation")
         if pipeline["metric_learning"]:
             if pipeline["semisupervised"]:
                 mod = self.load_model("semiml")
             else:
@@ -268,14 +271,16 @@
                 else:
                     mod = self.load_model("pca")
             else:
                 mod = None
         if mod is not None:
             # avoid taking the info from pickle in case it is copied
             mod.model_path = self.model_path
+            # using the config path for the CC_TMP and not the generated model one
+            mod.tmp_path = Config().PATH.CC_TMP
             mod.predict(destination)
 
         destination.refresh()
         self.__log.debug("Prediction done!")
 
     def neighbors(self, tmp, metric="cosine", k_neig=1000, cpu=4):
         """Neighbors"""
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/sign2.py` & `chemicalchecker-1.0.3/chemicalchecker/core/sign2.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         # so we overwrite the original embeddings using the predictor
         sign1_ref = cc_tmp.get_signature('sign1', 'reference', self.dataset)
         sign2_ref = cc_tmp.get_signature('sign2', 'reference', self.dataset)
         if oos_predictor:
             self.predict(sign1_full, sign2_full.data_path)
             self.predict(sign1_ref, sign2_ref.data_path)
         else:
-            self.map(sign2_full.data_path)
+            self.save_full(sign2_full.data_path)
         # finalize signature
         BaseSignature.fit_end(self,  **kwargs)
 
     def predict(self, sign1, destination=None):
         """Use the learned model to predict the signature.
 
         Args:
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/sign3.py` & `chemicalchecker-1.0.3/chemicalchecker/core/sign3.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from sklearn.preprocessing import robust_scale, StandardScaler
 
 from .signature_base import BaseSignature
 from .signature_data import DataSignature
 from .preprocess import Preprocess
 
 from chemicalchecker.util import logged
-from chemicalchecker.util.splitter import NeighborTripletTraintest
-from chemicalchecker.util.splitter import Traintest
+from chemicalchecker.util.splitter import OldTripletSampler, TripletIterator
+from chemicalchecker.util.splitter import BaseTripletSampler
 from chemicalchecker.util.parser.converter import Converter
 
 
 @logged
 class sign3(BaseSignature, DataSignature):
     """Signature type 3 class."""
 
@@ -66,18 +66,19 @@
             'batch_size': 128,
             'patience': 200,
             'loss_func': 'only_self_loss',
             'margin': 1.0,
             'alpha': 1.0,
             'num_triplets': 1000000,
             't_per': 0.01,
-            'standard': False,
+            'onlyself_notself': True,
             'augment_fn': subsample,
             'augment_kwargs': {
                 'dataset': [dataset],
+                'p_self': 0.1,
             },
             'limit_mols': 100000
         }
 
         if not self.is_fit():
             # we load this param only if signature is not fitted yet
             s1_ref = self.get_sign('sign1').get_molset("reference")
@@ -92,14 +93,15 @@
         default_sign2.update(params.get('sign2', {}))
         self.params['sign2_lr'] = default_sign2.copy()
         self.params['sign2'] = default_sign2
         self._sharedx = None
         self._sharedx_trim = None
         self.traintest_file = None
         self.trim_mask = None
+        #np.seterr(divide='ignore', invalid='ignore')
 
     @property
     def sharedx(self):
         if self._sharedx is None:
             if self.traintest_file is None:
                 self.__log.debug("traintest_file is not set.")
                 return None
@@ -190,16 +192,16 @@
                 # including NaN we have the correct number of molecules
                 coverage = np.isin(
                     list(inchikeys), list(sign.keys), assume_unique=True)
                 sign3.__log.info("%s has %s Signature 2." %
                                  (sign.dataset, np.count_nonzero(coverage)))
                 fh['x_test'][:, idx:(idx + 1)] = np.expand_dims(coverage, 1)
 
-    def complete_sign2_universe(self, sign2_self, sign2_universe, 
-                                sign2_coverage, tmp_path=None, 
+    def complete_sign2_universe(self, sign2_self, sign2_universe,
+                                sign2_coverage, tmp_path=None,
                                 calc_ds_idx=[0, 1, 2, 3, 4],
                                 calc_ds_names=['A1.001', 'A2.001', 'A3.001',
                                                'A4.001', 'A5.001'],
                                 ref_cc=None):
         """Completes the universe for extra molecules.
 
         Important if the dataset we are fitting is defined on molecules
@@ -265,18 +267,17 @@
                 # new inks must be sorted
                 assert(all(mi[i] <= mi[i + 1] for i in range(len(mi) - 1)))
                 sign3.__log.info('Getting InChI for %s molecules' %
                                  (len(miss_ink)))
                 miss_count = 0
                 for ink in miss_ink:
                     try:
-                        inchi = conv.inchikey_to_inchi(ink)[0]["standardinchi"]
+                        inchi = conv.inchikey_to_inchi(ink)
                     except Exception as ex:
-                        sign3.__log.warning(
-                            "Molecule %s: %s" % (ink, str(ex)))
+                        sign3.__log.warning(str(ex))
                         continue
                     fh.write('%s\t%s\n' % (ink, inchi))
                     miss_count += 1
                 fh.close()
                 sign3.__log.info('Adding %s molecules to %s' %
                                  (miss_count, ds))
                 if miss_count == 0:
@@ -323,15 +324,16 @@
             upd_uni.close()
             upd_cov.close()
         # final report
         upd_uni = h5py.File(sign2_universe_ext, "r")
         upd_cov = h5py.File(sign2_coverage_ext, "r")
         old_cov = h5py.File(sign2_coverage, "r")
         sign3.__log.info('Checking updated universe...')
-        for col, name in enumerate(cc_ref.datasets):
+
+        for col, name in enumerate(self.src_datasets):  # cc_ref.datasets
             tot_upd = sum(upd_cov['x_test'][:, col])
             cov_delta = int(tot_upd - sum(old_cov['x_test'][:, col]))
             if cov_delta == 0:
                 continue
             sign3.__log.info('Added %s molecules to %s' % (cov_delta, name))
             # check head and tail of signature
             sig_head = upd_uni['x_test'][:, col * 128]
@@ -355,15 +357,16 @@
         mask = np.isin(list(universe.keys), list(self.sign2_self.keys))
         universe.make_filtered_copy(destination, mask)
         # rename the dataset to what the splitter expects
         with h5py.File(destination, 'a') as hf:
             hf['x'] = hf['x_test']
             del hf['x_test']
 
-    def train_SNN(self, params, reuse=True, suffix=None, evaluate=True):
+    def train_SNN(self, params, reuse=True, suffix=None, evaluate=True,
+                  plots_train=True, triplets_sampler=None):
         """Train the Siamese Neural Network model.
 
         This method is used twice. First to evaluate the performances of the
         Siamese model. Second to train the final model on the full set of data.
         Triplets file are generated and SNN are trained. When evaluating also
         save the confidence model.
 
@@ -372,14 +375,15 @@
             reuse(bool): Whether to reuse intermediate files (e.g. the
                 aggregated signature 2 matrix).
             suffix(str): A suffix for the Siamese model path (e.g.
                 'sign3/models/siamese_<suffix>').
             evaluate(bool): Whether we are performing a train-test split and
                 evaluating the performances (N.B. this is required for complete
                 confidence scores)
+            plots_train(bool): plotting outcomes of train models.
         """
         try:
             from chemicalchecker.tool.siamese import SiameseTriplets
         except ImportError:
             raise ImportError("requires tensorflow https://tensorflow.org")
         # get params and set folder
         self.update_status("Training %s model" % suffix)
@@ -392,48 +396,60 @@
                 'traintest_file', traintest_file)
         else:
             siamese_path = os.path.join(self.model_path, 'siamese')
         if 'model_dir' in params:
             siamese_path = params.get('model_dir')
         if not reuse or not os.path.isdir(siamese_path):
             os.makedirs(siamese_path)
-        # generate input matrix
+        # generate input matrix, how molecules will be represented
         sign2_matrix = os.path.join(self.model_path, 'train.h5')
         if not reuse or not os.path.isfile(sign2_matrix):
             self.save_sign2_matrix(sign2_matrix)
-        # if evaluating, perform the train-test split
-        self.traintest_file = params.get('traintest_file')
         X = DataSignature(sign2_matrix)
+        # initialize triplet sampler
+        self.traintest_file = params.get('traintest_file')
+        num_triplets = params.get('num_triplets', 1e6)
+        cpu = params.get('cpu', 1)
+        if triplets_sampler is None:
+            sampler_class = OldTripletSampler
+            sampler_args = (self.triplet_sign, X, self.traintest_file)
+            sample_obj = sampler_class(*sampler_args)
+            sampler_kwargs = {'t_per': params['t_per'],
+                              'limit': params['limit_mols'], 'cpu': cpu,
+                              'num_triplets': num_triplets}
+        else:
+            sampler_class = triplets_sampler[0]
+            sampler_args = triplets_sampler[1]
+            if sampler_args is None:
+                sampler_args = (self.triplet_sign, X, self.traintest_file)
+            sample_obj = sampler_class(*sampler_args)
+            sampler_kwargs = triplets_sampler[2]
+        # if evaluating, perform the train-test split
         if evaluate:
-            num_triplets = params.get('num_triplets', 1e6)
-            cpu = params.get('cpu', 1)
-            if not reuse or not os.path.isfile(self.traintest_file):
-                NeighborTripletTraintest.create(
-                    X, self.traintest_file, self.neig_sign,
-                    split_names=['train', 'test'],
-                    split_fractions=[.8, .2],
-                    suffix=suffix,
-                    num_triplets=num_triplets,
-                    t_per=params['t_per'],
-                    cpu=cpu,
-                    limit=params['limit_mols'])
+            save_kwargs = {
+                'mean_center_x': True,
+                'shuffle': True,
+                'split_names': ['train', 'test'],
+                'split_fractions': [.8, .2],
+                'suffix': suffix
+            }
         else:
-            num_triplets = params.get('num_triplets', 1e6)
-            cpu = params.get('cpu', 1)
-            if not reuse or not os.path.isfile(self.traintest_file):
-                NeighborTripletTraintest.create(
-                    X, self.traintest_file, self.neig_sign,
-                    split_names=['train'],
-                    split_fractions=[1.0],
-                    suffix=suffix,
-                    num_triplets=num_triplets,
-                    t_per=params['t_per'],
-                    cpu=cpu,
-                    limit=params['limit_mols'])
-        # update the subsampling parameter
+            save_kwargs = {
+                'mean_center_x': True,
+                'shuffle': True,
+                'split_names': ['train'],
+                'split_fractions': [1.0],
+                'suffix': suffix
+            }
+        # generate triplets
+        sample_obj = sampler_class(*sampler_args, save_kwargs=save_kwargs)
+        if not reuse or not os.path.isfile(self.traintest_file):
+            sample_obj.generate_triplets(**sampler_kwargs)
+
+        # define the augment with the dataset subsampling parameter
         if 'augment_kwargs' in params:
             ds = params['augment_kwargs']['dataset']
             dataset_idx = np.argwhere(np.isin(self.src_datasets, ds)).flatten()
             if len(dataset_idx) > 1:
                 self.__log.warning('Dataset %s is repeated' % ds)
             dataset_idx = np.array(dataset_idx[:1])
             # compute probabilities for subsampling
@@ -448,34 +464,39 @@
             params['trim_mask'] = trim_mask
             self.trim_mask = trim_mask
         # train siamese network
         self.__log.debug('Siamese training on %s' % traintest_file)
         siamese = SiameseTriplets(
             siamese_path, evaluate=evaluate, sharedx=self.sharedx,
             sharedx_trim=self.sharedx_trim, **params)
+        self.__log.info('Plot Subsampling (what the SNN will get).')
+        fname = 'known_unknown_sampling.png'
+        plot_file = os.path.join(siamese.model_dir, fname)
+        plot_subsample(self, plot_file, self.sign2_coverage, traintest_file,
+                       ds=self.dataset, sign2_list=self.sign2_list)
         siamese.fit()
         self.__log.debug('Model saved to: %s' % siamese_path)
         # if final we are done
         if not evaluate:
             return siamese
         # save validation plots
         try:
             self.plot_validations(siamese, dataset_idx, traintest_file)
         except Exception as ex:
             self.__log.debug('Plot problem: %s' % str(ex))
         # when evaluating also save prior and confidence models
-        conf_res = self.train_confidence(siamese)
+        conf_res = self.train_confidence(siamese, plots_train=plots_train)
         prior_model, prior_sign_model, confidence_model = conf_res
         # update the parameters with the new nr_of epochs and lr
         self.params['sign2']['epochs'] = siamese.last_epoch
         return siamese, prior_model, prior_sign_model, confidence_model
 
     def train_confidence(self, siamese, suffix='eval', traintest_file=None,
                          train_file=None, max_x=10000, max_neig=50000,
-                         p_self=0.0):
+                         p_self=0.0, plots_train=True):
         """Train confidence and prior models."""
         # get sorted keys from siamese traintest file
         self.update_status('Training applicability')
         if traintest_file is None:
             traintest_file = os.path.join(self.model_path,
                                           'traintest_%s.h5' % suffix)
         if not os.path.isfile(traintest_file):
@@ -486,93 +507,107 @@
             raise Exception('Train_file not found: %s' % train_file)
         self.traintest_file = traintest_file
         traintest = DataSignature(self.traintest_file)
         test_inks = traintest.get_h5_dataset('keys_test')[:max_x]
         train_inks = traintest.get_h5_dataset('keys_train')[:max_neig]
         # confidence is going to be trained only on siamese test data
         test_mask = np.isin(list(self.sign2_self.keys), list(test_inks),
-                                  assume_unique=True)
+                            assume_unique=True)
         train_mask = np.isin(list(self.sign2_self.keys), list(train_inks),
-                                   assume_unique=True)
+                             assume_unique=True)
         train = DataSignature(train_file)
         confidence_train_x = train.get_h5_dataset('x', mask=test_mask)
         #s2_test = self.sign2_self.get_h5_dataset('V', mask=test_mask)
         _, s2_test = self.sign2_self.get_vectors(test_inks)
         s2_test_x = confidence_train_x[:, self.dataset_idx[0]
                                        * 128: (self.dataset_idx[0] + 1) * 128]
         assert(np.all(s2_test == s2_test_x))
         # siamese train is going to be used for appticability domain
         known_x = train.get_h5_dataset('x', mask=train_mask)
         # generate train-test split for confidence estimation
         split_names = ['train', 'test']
         split_fractions = [0.8, 0.2]
-        split_idxs = Traintest.get_split_indeces(
-            confidence_train_x.shape[0], split_fractions, random_state=42)
+
+        def get_split_indeces(rows, fractions):
+            """Get random indexes for different splits."""
+            if not sum(fractions) == 1.0:
+                raise Exception("Split fractions should sum to 1.0")
+            # shuffle indexes
+            idxs = list(range(rows))
+            np.random.shuffle(idxs)
+            # from frequencies to indices
+            splits = np.cumsum(fractions)
+            splits = splits[:-1]
+            splits *= len(idxs)
+            splits = splits.round().astype(np.int)
+            return np.split(idxs, splits)
+
+        split_idxs = get_split_indeces(confidence_train_x.shape[0], split_fractions)
         splits = list(zip(split_names, split_fractions, split_idxs))
 
         # train prior model
         prior_path = os.path.join(self.model_path, 'prior_%s' % suffix)
         os.makedirs(prior_path, exist_ok=True)
         prior_model = self.train_prior_model(siamese, confidence_train_x,
                                              splits, prior_path,
-                                             max_x=max_x, p_self=p_self)
+                                             max_x=max_x, p_self=p_self, plots=plots_train)
 
         # train prior signature model
         prior_sign_path = os.path.join(self.model_path,
                                        'prior_sign_%s' % suffix)
         os.makedirs(prior_sign_path, exist_ok=True)
         prior_sign_model = self.train_prior_signature_model(
             siamese, confidence_train_x, splits, prior_sign_path,
-            max_x=max_x, p_self=p_self)
+            max_x=max_x, p_self=p_self, plots=plots_train)
 
         # train confidence model
         confidence_path = os.path.join(self.model_path,
                                        'confidence_%s' % suffix)
         os.makedirs(confidence_path, exist_ok=True)
         confidence_model = self.train_confidence_model(
             siamese, known_x, confidence_train_x, splits,
             prior_model, prior_sign_model,
-            confidence_path, p_self=p_self)
+            confidence_path, p_self=p_self, plots=plots_train)
         return prior_model, prior_sign_model, confidence_model
 
     def rerun_confidence(self, cc, suffix, train=True, update_sign=True,
                          chunk_size=10000, sign2_universe=None,
-                         sign2_coverage=None):
+                         sign2_coverage=None, plots_train=True):
         """Rerun confidence trainining and estimation"""
         try:
             import faiss
             from chemicalchecker.tool.siamese import SiameseTriplets
         except ImportError:
             raise ImportError("requires tensorflow https://tensorflow.org")
-        sign1_self = cc.get_signature("sign1", "full", self.dataset)
+        triplet_sign = cc.get_signature("sign1", "full", self.dataset)
         sign2_self = cc.get_signature("sign2", "full", self.dataset)
         sign2_list = [cc.get_signature("sign2", "full", d)
                       for d in cc.datasets_exemplary()]
         if sign2_universe is None:
             sign2_universe = os.path.join(cc.cc_root, 'full', 'all_sign2.h5')
         if sign2_coverage is None:
             sign2_coverage = os.path.join(
                 cc.cc_root, 'full', 'all_sign2_coverage.h5')
 
         self.src_datasets = [sign.dataset for sign in sign2_list]
-        self.neig_sign = sign1_self
+        self.triplet_sign = triplet_sign
         self.sign2_self = sign2_self
         self.sign2_list = sign2_list
         self.sign2_coverage = sign2_coverage
         self.sign2_universe = sign2_universe
         self.dataset_idx = np.argwhere(
             np.isin(self.src_datasets, self.dataset)).flatten()
 
         siamese_path = os.path.join(self.model_path, 'siamese_%s' % suffix)
         siamese = SiameseTriplets(siamese_path, predict_only=True)
         siamese_cp = SiameseTriplets(siamese.model_dir, predict_only=True)
 
         if train:
             prior_mdl, prior_sign_mdl, conf_mdl = self.train_confidence(
-                siamese, suffix=suffix)
+                siamese, suffix=suffix, plots_train=plots_train)
             if not update_sign:
                 return
         else:
             # part of confidence is the priors
             prior_path = os.path.join(self.model_path, 'prior_eval')
             prior_file = os.path.join(prior_path, 'prior.pkl')
             prior_mdl = pickle.load(open(prior_file, 'rb'))
@@ -692,15 +727,15 @@
                                p_nr=p_nr, p_keep=p_keep)
         return realistic_fn, trim_mask
 
     def train_prior_model(self, siamese, train_x, splits, save_path,
                           max_x=10000, n_samples=5, p_self=0.0, plots=True):
         """Train prior predictor."""
         def get_weights(y, p=2):
-            h, b = np.histogram(y, 20)
+            h, b = np.histogram(y[~np.isnan(y)], 20)
             b = [np.mean([b[i], b[i + 1]]) for i in range(0, len(h))]
             w = np.interp(y, b, h).ravel()
             w = -(w / np.sum(w)) + 1e-10
             w = (w - np.min(w)) / (np.max(w) - np.min(w))
             w = w**p
             return w
 
@@ -738,15 +773,16 @@
                 ax.set_ylim(lim)
                 ax.plot([lim[0], lim[1]], [lim[0], lim[1]],
                         color="gray", ls='--', lw=1)
             slope, intercept, r, p_val, stde = stats.linregress(x, y)
             line = slope * x + intercept
             ax.plot(x, line, 'r',
                     label='y={:.2f}x+{:.2f}'.format(slope, intercept))
-            title = "rho = %.2f" % pearsonr(x, y)[0]
+            nas = np.logical_or(np.isnan(x), np.isnan(y))
+            title = "rho = %.2f" % pearsonr(x[~nas], y[~nas])[0]
             ax.set_title(title)
             ax.legend()
 
         def importances(ax, mod, trim_mask):
             from chemicalchecker.util.plot import coord_color
             y = mod.feature_importances_
             datasets = [s.dataset[:2] for s in self.sign2_list]
@@ -774,17 +810,19 @@
             fig = plt.figure(constrained_layout=True, figsize=(8, 6))
             gs = fig.add_gridspec(2, 3)
             ax = fig.add_subplot(gs[0, 0])
             histograms(ax, y_tr_p, y_tr, "Train")
             ax = fig.add_subplot(gs[0, 1])
             histograms(ax, y_te_p, y_te, "Test")
             ax = fig.add_subplot(gs[1, 0])
-            scatter(ax, y_tr_p, y_tr)
+            nas = np.logical_or(np.isnan(y_tr_p), np.isnan(y_tr))
+            scatter(ax, y_tr_p[~nas], y_tr[~nas])
             ax = fig.add_subplot(gs[1, 1])
-            scatter(ax, y_te_p, y_te)
+            nas = np.logical_or(np.isnan(y_te_p), np.isnan(y_te))
+            scatter(ax, y_te_p[~nas], y_te[~nas])
             ax = fig.add_subplot(gs[0:2, 2])
             importances(ax, mod, trim_mask)
             if plots:
                 try:
                     plt.savefig(os.path.join(save_path, 'prior_stats.png'))
                     plt.close()
                 except Exception as ex:
@@ -857,28 +895,42 @@
                         # the prior is only-self vs not-self predictions
                         corrs = row_wise_correlation(
                             preds_onlyself, preds_noself, scaled=True)
                         Y[dst_chunk] = np.expand_dims(corrs, 1)
                         # the X is the dataset presence in the not-self
                         presence = ~np.isnan(feat[:, ::128])[:, trim_mask]
                         X[dst_chunk] = presence.astype(int)
-                        # check if enought
+                        # check if enough
                         if reached_max:
                             break
                 variables = [X, Y, feat, preds_onlyselfs, preds_noselfs]
                 names = ['x', 'y', 'feat', 'preds_onlyselfs', 'preds_noselfs']
                 for var, name in zip(variables, names):
                     ds_name = '%s_%s' % (name, split_name)
                     self.__log.debug('writing %s: %s' % (ds_name, var.shape))
                     fh.create_dataset(ds_name, data=var)
         traintest = DataSignature(out_file)
         x_tr = traintest.get_h5_dataset('x_train')
         y_tr = traintest.get_h5_dataset('y_train').ravel()
         x_te = traintest.get_h5_dataset('x_test')
         y_te = traintest.get_h5_dataset('y_test').ravel()
+        # TODO: check the generation of data.h5 file: NaNs?
+        if np.isnan(x_tr).any():
+            nans_xtr = np.argwhere(np.isnan(x_tr))
+            self.__log.debug("Len NaNs in x_tr: {}".format(len(nans_xtr)))
+        if np.isnan(y_tr).any():
+            nans_ytr = np.argwhere(np.isnan(y_tr))
+            self.__log.debug("Len NaNs in y_tr: {}".format(len(nans_ytr)))
+        if np.isnan(x_te).any():
+            nans_xte = np.argwhere(np.isnan(x_te))
+            self.__log.debug("Len NaNs in x_te: {}".format(len(nans_xte)))
+        if np.isnan(y_te).any():
+            nans_yte = np.argwhere(np.isnan(y_te))
+            self.__log.debug("Len NaNs in y_te: {}".format(len(nans_yte)))
+
         # fit model
         model = RandomForestRegressor(n_estimators=1000, max_features=None,
                                       min_samples_leaf=0.01, n_jobs=4)
         p = find_p(model, x_tr, y_tr, x_te, y_te)
         model.fit(x_tr, y_tr, sample_weight=get_weights(y_tr, p=p))
         if plots:
             analyze(model, x_tr, y_tr, x_te, y_te, trim_mask)
@@ -887,15 +939,15 @@
         return model
 
     def train_prior_signature_model(self, siamese, train_x, splits,
                                     save_path, max_x=10000, n_samples=5,
                                     p_self=0.0, plots=True):
         """Train prior predictor."""
         def get_weights(y, p=2):
-            h, b = np.histogram(y, 20)
+            h, b = np.histogram(y[~np.isnan(y)], 20)
             b = [np.mean([b[i], b[i + 1]]) for i in range(0, len(h))]
             w = np.interp(y, b, h).ravel()
             w = -(w / np.sum(w)) + 1e-10
             w = (w - np.min(w)) / (np.max(w) - np.min(w))
             w = w**p
             return w
 
@@ -933,15 +985,16 @@
                 ax.set_ylim(lim)
                 ax.plot([lim[0], lim[1]], [lim[0], lim[1]],
                         color="gray", ls='--', lw=1)
             slope, intercept, r, p_val, stde = stats.linregress(x, y)
             line = slope * x + intercept
             ax.plot(x, line, 'r',
                     label='y={:.2f}x+{:.2f}'.format(slope, intercept))
-            title = "rho = %.2f" % pearsonr(x, y)[0]
+            nas = np.logical_or(np.isnan(x), np.isnan(y))
+            title = "rho = %.2f" % pearsonr(x[~nas], y[~nas])[0]
             ax.set_title(title)
             ax.legend()
 
         def importances(ax, mod):
             y = mod.feature_importances_
             datasets = np.arange(128)
             datasets = np.array(datasets)
@@ -964,17 +1017,19 @@
             fig = plt.figure(constrained_layout=True, figsize=(8, 6))
             gs = fig.add_gridspec(2, 3)
             ax = fig.add_subplot(gs[0, 0])
             histograms(ax, y_tr_p, y_tr, "Train")
             ax = fig.add_subplot(gs[0, 1])
             histograms(ax, y_te_p, y_te, "Test")
             ax = fig.add_subplot(gs[1, 0])
-            scatter(ax, y_tr_p, y_tr)
+            nas = np.logical_or(np.isnan(y_tr_p), np.isnan(y_tr))
+            scatter(ax, y_tr_p[~nas], y_tr[~nas])
             ax = fig.add_subplot(gs[1, 1])
-            scatter(ax, y_te_p, y_te)
+            nas = np.logical_or(np.isnan(y_te_p), np.isnan(y_te))
+            scatter(ax, y_te_p[~nas], y_te[~nas])
             ax = fig.add_subplot(gs[0:2, 2])
             importances(ax, mod)
             if plots:
                 try:
                     plt.savefig(os.path.join(save_path, 'prior_stats.png'))
                     plt.close()
                 except Exception as ex:
@@ -1059,14 +1114,27 @@
                     self.__log.debug('writing %s: %s' % (ds_name, var.shape))
                     fh.create_dataset(ds_name, data=var)
         traintest = DataSignature(out_file)
         x_tr = traintest.get_h5_dataset('x_train')
         y_tr = traintest.get_h5_dataset('y_train').ravel()
         x_te = traintest.get_h5_dataset('x_test')
         y_te = traintest.get_h5_dataset('y_test').ravel()
+        # TODO: check the generation of data.h5 file: NaNs?
+        if np.isnan(x_tr).any():
+            nans_xtr = np.argwhere(np.isnan(x_tr))
+            self.__log.debug("Len NaNs in x_tr: {}".format(len(nans_xtr)))
+        if np.isnan(y_tr).any():
+            nans_ytr = np.argwhere(np.isnan(y_tr))
+            self.__log.debug("Len NaNs in y_tr: {}".format(len(nans_ytr)))
+        if np.isnan(x_te).any():
+            nans_xte = np.argwhere(np.isnan(x_te))
+            self.__log.debug("Len NaNs in x_te: {}".format(len(nans_xte)))
+        if np.isnan(y_te).any():
+            nans_yte = np.argwhere(np.isnan(y_te))
+            self.__log.debug("Len NaNs in y_te: {}".format(len(nans_yte)))
         # fit model
         model = RandomForestRegressor(n_estimators=1000, max_features='sqrt',
                                       min_samples_leaf=0.01, n_jobs=4)
         p = find_p(model, x_tr, y_tr, x_te, y_te)
         model.fit(x_tr, y_tr, sample_weight=get_weights(y_tr, p=p))
         if plots:
             analyze(model, x_tr, y_tr, x_te, y_te)
@@ -1402,15 +1470,15 @@
         return features, correlation
 
     def applicability_domain(self, neig_index, features, siamese,
                              dropout_fn=None, app_range=None, n_samples=1,
                              p_self=0.0, subsampling=False):
         # applicability is whether not-self preds is close to only-self preds
         # neighbors between 5 and 25 depending on the size of the dataset
-        app_thr = int(np.clip(np.log10(self.neig_sign.shape[0])**2, 5, 25))
+        app_thr = int(np.clip(np.log10(self.triplet_sign.shape[0])**2, 5, 25))
         if subsampling:
             if dropout_fn is None:
                 dropout_fn, _ = self.realistic_subsampling_fn()
             preds, dists, ranges = list(), list(), list()
             for i in range(n_samples):
                 pred = siamese.predict(features,
                                        dropout_fn=partial(
@@ -1659,42 +1727,39 @@
         axes[1][1].scatter(dist_os[:, 0], dist_os[:, 1], s=10, color="#d62728")
 
         fname = 'known_unknown_projection.png'
         plot_file = os.path.join(siamese.model_dir, fname)
         plt.savefig(plot_file)
         plt.close()
 
-        self.__log.info('VALIDATION: Plot Subsampling.')
-        fname = 'known_unknown_sampling.png'
-        plot_file = os.path.join(siamese.model_dir, fname)
-        plot_subsample(self, plot_file, self.sign2_coverage, traintest_file,
-                       ds=self.dataset, sign2_list=self.sign2_list)
 
     def get_universe_inchikeys(self):
         # get sorted universe inchikeys
         if hasattr(self, 'universe_inchikeys'):
             return self.universe_inchikeys
         inchikeys = set()
         for ds, sign in zip(self.src_datasets, self.sign2_list):
             inchikeys.update(sign.unique_keys)
         inchikeys = sorted(list(inchikeys))
         return inchikeys
 
-    def fit(self, sign2_list=None, sign2_self=None, sign1_self=None,
+    def fit(self, sign2_list=None, sign2_self=None, triplet_sign=None,
             sign2_universe=None, complete_universe='full',
             sign2_coverage=None,
             model_confidence=True, save_correlations=False,
             predict_novelty=False, update_preds=True,
-            chunk_size=1000, suffix=None, **kwargs):
+            chunk_size=1000, suffix=None, plots_train=True,
+            triplets_sampler=None, **kwargs):
         """Fit signature 3 given a list of signature 2.
 
         Args:
             sign2_list(list): List of signature 2 objects to learn from.
             sign2_self(sign2): Signature 2 of the current space.
-            sign2_self(sign1): Signature 1 of the current space.
+            triplet_sign(sign1): Signature used to define acnhor positive and 
+                negative in triplets.
             sign2_universe(str): Path to the union of all signatures 2 for all
                 molecules in the CC universe. (~1M x 3200)
             complete_universe(str): add chemistry information for molecules not
                 in the universe. 'full' use all A* spaces while, 'fast' skips
                 A2 (3D conformation) which is slow. False by default, not
                 adding any signature to the universe.
             sign2_coverage(str): Path to the coverage of all signatures 2 for
@@ -1705,14 +1770,18 @@
                 tertile, max) for the given input dataset (result of the
                 evaluation).
             predict_novelty(bool) Whether to predict molecule novelty score.
             update_preds(bool): Whether to write or update the sign3.h5
             normalize_scores(bool): Whether to normalize confidence scores.
             chunk_size(int): Chunk size when writing to sign3.h5
             suffix(str): Suffix of the generated model.
+            plots_train(bool): plotting trained models outcomes defaulted to True.
+                               it applies to train_prior_model, 
+                               train_prior_signature_model,
+                               train_confidence_model
         """
         try:
             from chemicalchecker.tool.siamese import SiameseTriplets
         except ImportError:
             raise ImportError("requires tensorflow https://tensorflow.org")
         try:
             import faiss
@@ -1734,17 +1803,17 @@
             for ds in cc.datasets_exemplary():
                 sign2_list.append(cc.get_signature('sign2', 'full', ds))
         self.sign2_list = sign2_list
         self.src_datasets = [sign.dataset for sign in sign2_list]
         if sign2_self is None:
             sign2_self = self.get_sign('sign2')
         self.sign2_self = sign2_self
-        if sign1_self is None:
-            sign1_self = self.get_sign('sign1')
-        self.neig_sign = sign1_self
+        if triplet_sign is None:
+            triplet_sign = self.get_sign('sign1')
+        self.triplet_sign = triplet_sign
 
         self.sign2_coverage = sign2_coverage
         self.dataset_idx = np.argwhere(
             np.isin(self.src_datasets, self.dataset)).flatten()
         if self.sign2_coverage is None:
             self.sign2_coverage = os.path.join(self.model_path,
                                                'all_sign2_coverage.h5')
@@ -1787,50 +1856,54 @@
         conf_mdl = None
 
         if suffix is None:
             eval_model_path = os.path.join(self.model_path, 'siamese_eval')
             eval_file = os.path.join(eval_model_path, 'siamesetriplets.h5')
             if not os.path.isfile(eval_file):
                 res = self.train_SNN(
-                    self.params['sign2'].copy(), suffix='eval', evaluate=True)
+                    self.params['sign2'].copy(), suffix='eval', evaluate=True,
+                    plots_train=plots_train, triplets_sampler=triplets_sampler)
                 siamese, prior_mdl, prior_sign_mdl, conf_mdl = res
         else:
             eval_model_path = os.path.join(self.model_path,
                                            'siamese_%s' % suffix)
             eval_file = os.path.join(eval_model_path, 'siamesetriplets.h5')
             if not os.path.isfile(eval_file):
                 res = self.train_SNN(
-                    self.params['sign2'].copy(), suffix=suffix, evaluate=True)
+                    self.params['sign2'].copy(), suffix=suffix, evaluate=True,
+                    plots_train=plots_train, triplets_sampler=triplets_sampler)
                 siamese, prior_mdl, prior_sign_mdl, conf_mdl = res
             return False
 
         # check if we have the final trained model
         final_model_path = os.path.join(self.model_path, 'siamese_final')
         final_file = os.path.join(final_model_path, 'siamesetriplets.h5')
         if not os.path.isfile(final_file):
             # get the learning rate from the siamese eval
             siamese_eval = SiameseTriplets(eval_model_path, predict_only=True)
             self.params['sign2']['learning_rate'] = siamese_eval.learning_rate
             siamese = self.train_SNN(
-                self.params['sign2'].copy(), suffix='final', evaluate=False)
+                self.params['sign2'].copy(), suffix='final', evaluate=False,
+                triplets_sampler=triplets_sampler)
 
         # load models if not already available
         if siamese is None:
             siamese = SiameseTriplets(final_model_path, predict_only=True)
         siamese_cp = SiameseTriplets(siamese.model_dir, predict_only=True)
 
         if model_confidence:
             # part of confidence is the priors
             if prior_mdl is None:
                 prior_path = os.path.join(self.model_path, 'prior_eval')
                 prior_file = os.path.join(prior_path, 'prior.pkl')
                 # if prior model is not there, retrain confidence
                 if not os.path.isfile(prior_file):
                     siamese_eval = SiameseTriplets(eval_model_path)
-                    self.train_confidence(siamese_eval)
+                    self.train_confidence(
+                        siamese_eval, plots_train=plots_train)
                 prior_mdl = pickle.load(open(prior_file, 'rb'))
 
             # part of confidence is the priors based on signatures
             if prior_sign_mdl is None:
                 prior_sign_path = os.path.join(
                     self.model_path, 'prior_sign_eval')
                 prior_sign_file = os.path.join(prior_sign_path, 'prior.pkl')
@@ -1841,15 +1914,15 @@
             if conf_mdl is None:
                 confidence_file = os.path.join(
                     confidence_path, 'confidence.pkl')
                 if not os.path.isfile(confidence_file):
                     self.rerun_confidence(
                         cc, 'eval', train=True, update_sign=False,
                         sign2_universe=self.sign2_universe,
-                        sign2_coverage=self.sign2_coverage)
+                        sign2_coverage=self.sign2_coverage, plots_train=plots_train)
                 calibration_file = os.path.join(
                     confidence_path, 'calibration.pkl')
                 conf_mdl = (pickle.load(open(confidence_file, 'rb')),
                             pickle.load(open(calibration_file, 'rb')))
 
             # another part of confidence is the applicability
             neig_file = os.path.join(confidence_path, 'neig.index')
@@ -1966,15 +2039,15 @@
 
         # use semi-supervised anomaly detection algorithm to predict novelty
         if predict_novelty:
             self.update_status("Predicting novelty")
             self.predict_novelty()
 
         # save reference
-        self.save_reference()
+        self.save_reference(overwrite=True)
         # finalize signature
         BaseSignature.fit_end(self, **kwargs)
 
     def predict_novelty(self, retrain=False, update_sign3=True, cpu=4):
         """Model novelty score via LocalOutlierFactor (semi-supervised).
 
         Args:
@@ -2137,14 +2210,15 @@
                       min_unknown=10000):
     """Extract probabilities for known and unknown of a given dataset."""
     if type(sign2_coverage) == str:
         with h5py.File(sign2_coverage, "r") as cov_matrix:
             cov = cov_matrix['x_test'][:]
     else:
         cov = sign2_coverage
+    max_ds = cov.shape[1]
     unknown = cov[(cov[:, dataset_idx] == 0).ravel()]
     known = cov[(cov[:, dataset_idx] == 1).ravel()]
     if unknown.shape[0] < min_unknown:
         unknown = known[:min_unknown]
     # decide which spaces are frequent enought in known (used for trainint)
     trim_mask = (np.sum(known, axis=0) / known.shape[0]) > trim_threshold
 
@@ -2164,17 +2238,17 @@
         # normalize (sum of probabilities must be one)
         min_p_nr = min_p_nr / np.sum(min_p_nr)
         # print(np.log10(min_p_nr + 1e-10).astype(int))
         # probabilities to keep a dataset?
         p_keep = np.sum(coverage, axis=0) / coverage.shape[0]
         return min_p_nr, p_keep
 
-    p_nr_known, p_keep_known = compute_probs(known[:, trim_mask])
+    p_nr_known, p_keep_known = compute_probs(known[:, trim_mask], max_nr=max_ds)
     unknown[:, dataset_idx] = 0
-    p_nr_unknown, p_keep_unknown = compute_probs(unknown[:, trim_mask])
+    p_nr_unknown, p_keep_unknown = compute_probs(unknown[:, trim_mask], max_nr=max_ds)
     return trim_mask, p_nr_unknown, p_keep_unknown, p_nr_known, p_keep_known
 
 
 def subsample(tensor, sign_width=128,
               p_nr=(np.array([1 / 25.] * 25), np.array([1 / 25.] * 25)),
               p_keep=(np.array([1 / 25.] * 25), np.array([1 / 25.] * 25)),
               p_only_self=0.0,
@@ -2230,64 +2304,63 @@
         mask[idx] = np.repeat(presence_add, sign_width)
     # make masked dataset NaN
     new_data[~mask] = np.nan
     return new_data
 
 
 def plot_subsample(sign, plot_file, sign2_coverage, traintest_file,
-                   ds='B1.001', p_self=.1, p_only_self=0., limit=10000,
-                   max_ds=25, sign2_list=None):
+                   ds='B1.001', p_self=0.1, p_only_self=0.0, limit=10000,
+                   sign2_list=None):
+    """ Validation plot for the subsampling procedure."""
     import numpy as np
     import pandas as pd
     import seaborn as sns
     import matplotlib.pyplot as plt
     from chemicalchecker import ChemicalChecker
-
     cc = sign.get_cc()
 
-    # NICO sign2_list
     if sign2_list is not None:
         sign2_ds_list = [s.dataset for s in sign2_list]
     else:
         sign2_ds_list = list(cc.datasets_exemplary())
+    max_ds = len(sign2_list)
 
     # get triplet generator
     dataset_idx = np.argwhere(
         np.isin(sign2_ds_list, ds)).flatten()
     res = subsampling_probs(sign2_coverage, dataset_idx)
     trim_mask, p_nr_unknown, p_keep_unknown, p_nr_known, p_keep_known = res
     trim_dataset_idx = np.argwhere(np.arange(len(trim_mask))[
         trim_mask] == dataset_idx).ravel()[0]
     augment_kwargs = {
         'p_nr': (p_nr_unknown, p_nr_known),
         'p_keep': (p_keep_unknown, p_keep_known),
         'dataset_idx': [trim_dataset_idx],
         'p_only_self': 0.0}
     realistic_fn, trim_mask = sign.realistic_subsampling_fn()
-    tr_shape_type_gen = NeighborTripletTraintest.generator_fn(
+    tr_shape_type_gen = TripletIterator.generator_fn(
         traintest_file,
         'train_train',
         batch_size=10,
-        replace_nan=np.nan,
+        train=True,
         augment_fn=realistic_fn,
         augment_kwargs=augment_kwargs,
         trim_mask=trim_mask,
-        train=True,
-        standard=False)
+        onlyself_notself=True)
     tr_gen = tr_shape_type_gen[2]
 
     # get known unknown
     with h5py.File(sign2_coverage, "r") as cov_matrix:
         cov = cov_matrix['x_test'][:]
     unknown = cov[(cov[:, dataset_idx] == 0).flatten()]
     known = cov[(cov[:, dataset_idx] == 1).flatten()]
 
     # get dataset probabilities
     probs_ds = {
-        'space': np.array([d[:2] for d in cc.datasets_exemplary()])[trim_mask],
+        'space': np.array([d[:2] for d in sign2_ds_list])[trim_mask],
         'p_keep_known': p_keep_known,
         'p_keep_unknown': p_keep_unknown}
     df_probs_ds = pd.DataFrame(probs_ds)
     df_probs_ds = df_probs_ds.melt(id_vars=['space'])
     df_probs_ds['probabilities'] = df_probs_ds['value']
 
     # get nr probabilities
@@ -2319,15 +2392,15 @@
         ds_p += np.sum(~np.isnan(p[:, ::128]), axis=0)
         ds_n += np.sum(~np.isnan(n[:, ::128]), axis=0)
         ds_o += np.sum(~np.isnan(o[:, ::128]), axis=0)
         ds_ns += np.sum(~np.isnan(ns[:, ::128]), axis=0)
         batch += 1
         if batch == 1000:
             break
-    trimmed_ds = np.array(list(cc.datasets_exemplary()))[trim_mask]
+    trimmed_ds = np.array(sign2_ds_list)[trim_mask]
     sampled_ds = {
         'space': np.array([d[:2] for d in trimmed_ds]),
         'anchor': ds_a,
         'positive': ds_p,
         'negative': ds_n,
         'only-self': ds_o,
         'not-self': ds_ns}
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/sign4.py` & `chemicalchecker-1.0.3/chemicalchecker/core/sign4.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,50 +22,52 @@
     def __init__(self, signature_path, dataset, **params):
         """Initialize a Signature.
 
         Args:
             signature_path(str): The signature root directory.
             dataset(`Dataset`): `chemicalchecker.database.Dataset` object.
             params(): Parameters, expected keys are:
-                * 'sign2' for learning based on sign2
-                * 'sign0' for learning based on sign0 (Morgan Fingerprint)
-                * 'sign0_conf' for learning confidences based on MFP
-                * 'prior' for learning prior in predictions
+                * 'sign0_params' for learning based on sign0 
+                    (Morgan Fingerprint)
+                * 'sign0_conf_params' for learning confidences based on MFP
         """
         # Calling init on the base class to trigger file existence checks
         BaseSignature.__init__(self, signature_path,
                                dataset, **params)
         self.data_path = os.path.join(self.signature_path, 'sign4.h5')
         DataSignature.__init__(self, self.data_path)
         # get parameters or default values
         self.params = dict()
         # parameters to learn from sign0
         default_sign0 = {
-            'epochs': 5,
+            'epochs': 30,
             'cpu': 8,
             'learning_rate': 1e-3,
             'layers': ['Dense', 'Dense', 'Dense', 'Dense'],
             'layers_sizes': [1024, 512, 256, 128],
-            'activations': ['selu', 'selu', 'selu', 'tanh'],
-            'dropouts': [0.2, 0.2, 0.2, None],
-            'batch_size': 128,
-            'num_triplets': 100000,
-            'margin': 1.0,
-            'alpha': 0.5,
+            'activations': ['relu', 'relu', 'relu', 'tanh'],
+            'dropouts': [0.1, 0.1, 0.1, None],
         }
-        # default_sign0.update(params.get('sign0', {}))
+        default_sign0.update(params.get('sign0_params', {}))
         self.params['sign0'] = default_sign0
         # parameters to learn confidence from sign0
-        default_sign0_conf = {}
-        default_sign0_conf.update(params.get('sign0_conf', {}))
+        default_sign0_conf = {
+            'epochs': 30,
+            'cpu': 8,
+            'learning_rate': 1e-3,
+            'layers': ['Dense', 'Dense', 'Dense', 'Dense'],
+            'layers_sizes': [1024, 512, 256, 1],
+            'activations': ['relu', 'relu', 'relu', 'linear'],
+            'dropouts': [0.5, 0.2, 0.2, None]
+        }
+        default_sign0_conf.update(params.get('sign0_conf_params', {}))
         self.params['sign0_conf'] = default_sign0_conf
         self._sign0_V = None
         self._sign3_V = None
 
-
     @property
     def shared_keys(self):
         return sorted(list(self.sign0.unique_keys & self.sign3.unique_keys))
 
     @property
     def sign0_vectors(self):
         if self._sign0_V is None:
@@ -83,15 +85,15 @@
     def sign3_vectors(self):
         if self._sign3_V is None:
             self.__log.debug("Reading sign3, this should only be loaded once.")
             _, self._sign3_V = self.sign3.get_vectors(self.shared_keys)
         self.__log.debug("sign3 shape: %s" % str(self._sign3_V.shape))
         return self._sign3_V
 
-    def learn_sign0(self, sign0, sign3, suffix=None, evaluate=True):
+    def learn_sign0(self, sign0, sign3, params, suffix=None, evaluate=True):
         """Learn the signature 3 from sign0.
 
         This method is used twice. First to evaluate the performances of the
         model. Second to train the final model on the full set of data.
 
         Args:
             sign0(list): Signature 0 object to learn from.
@@ -111,24 +113,24 @@
             raise ImportError("requires tensorflow https://tensorflow.org")
         # get params and set folder
         model_path = os.path.join(self.model_path, 'smiles_%s' % suffix)
         if not os.path.isdir(model_path):
             os.makedirs(model_path)
         # initialize model and start learning
         smpred = Smilespred(
-            model_dir=model_path, sign0=self.sign0_vectors, 
-            sign3=self.sign3_vectors, evaluate=evaluate)
+            model_dir=model_path, sign0=self.sign0_vectors,
+            sign3=self.sign3_vectors, evaluate=evaluate, **params)
         self.__log.debug('Smiles pred training on %s' % model_path)
         smpred.fit()
         self.smiles_predictor = smpred
         self.__log.debug('model saved to %s' % model_path)
         if evaluate:
             smpred.evaluate()
 
-    def learn_sign0_conf(self, sign0, sign3, reuse=True, suffix=None,
+    def learn_sign0_conf(self, sign0, sign3, params, reuse=True, suffix=None,
                          evaluate=True):
         """Learn the signature 3 applicability from sign0.
 
         This method is used twice. First to evaluate the performances of the
         model. Second to train the final model on the full set of data.
 
         Args:
@@ -148,21 +150,21 @@
             raise ImportError("requires tensorflow https://tensorflow.org")
         # get params and set folder
         model_path = os.path.join(self.model_path,
                                   'smiles_applicability_%s' % suffix)
         if not os.path.isdir(model_path):
             reuse = False
             os.makedirs(model_path)
-        _, sign3_app_V = self.sign3.get_vectors(self.shared_keys, 
-            dataset_name='confidence')
+        _, sign3_app_V = self.sign3.get_vectors(self.shared_keys,
+                                                dataset_name='confidence')
         sign3_app_V = sign3_app_V.ravel()
         # initialize model and start learning
         apppred = ApplicabilityPredictor(
             model_dir=model_path, sign0=self.sign0_vectors,
-            applicability=sign3_app_V, evaluate=evaluate)
+            applicability=sign3_app_V, evaluate=evaluate, **params)
         self.__log.debug('Applicability pred training on %s' % model_path)
         if not reuse:
             apppred.fit()
         self.smiles_predictor = apppred
         self.__log.debug('model saved to %s' % model_path)
         if evaluate:
             apppred.evaluate()
@@ -172,15 +174,15 @@
         """Fit signature 4 from Morgan Fingerprint.
 
         This method is fitting a model that uses Morgan fingerprint as features
         to predict signature 3. In future other featurization approaches can be
         tested.
 
         Args:
-            sign0(str): Path to the MF file (e.g. sign0 of A1.001).
+            sign0(str): Path to the MFP file (i.e. sign0 of A1.001).
             include_confidence(bool): Whether to include confidence score in
                 regression problem.
             only_confidence(bool): Whether to only train an additional
                 regressor exclusively devoted to confidence.
         """
         BaseSignature.fit(self, **kwargs)
         # signature specific checks
@@ -195,108 +197,121 @@
             self.__log.debug("Fit will be done using full sign0")
             sign0 = sign0.get_molset("full")
         self.sign0 = sign0
         if sign3.molset != "full":
             self.__log.debug("Fit will be done using full sign3")
             sign3 = sign3.get_molset("full")
         self.sign3 = sign3
+        if sign0.shape[0] != sign3.shape[0]:
+            self.__log.warning("sign3 and MFP do not have the same nr of "
+                               "molecules. This might give bad sign0 recap.")
 
         # check if performance evaluations need to be done
         if not only_confidence:
             self.update_status("Training SMILES-based signature predictor")
             if suffix is not None:
-                self.learn_sign0(sign0, sign3, suffix=suffix, evaluate=True)
+                self.learn_sign0(sign0, sign3, self.params['sign0'].copy(),
+                                 suffix=suffix, evaluate=True)
                 return False
             else:
-                self.learn_sign0(sign0, sign3, suffix='eval', evaluate=True)
+                self.learn_sign0(sign0, sign3, self.params['sign0'].copy(),
+                                 suffix='eval', evaluate=True)
             # check if we have the final trained model
             self.update_status("Fitting final SMILES model")
-            self.learn_sign0(sign0, sign3, suffix='final', evaluate=False)
+            self.learn_sign0(sign0, sign3, self.params['sign0'].copy(),
+                             suffix='final', evaluate=False)
         if include_confidence:
             self.update_status("Training SMILES-based confidence predictor")
             if suffix is not None:
                 self.learn_sign0_conf(
-                    sign0, sign3, suffix=suffix, evaluate=True)
+                    sign0, sign3, self.params['sign0_conf'].copy(),
+                    suffix=suffix, evaluate=True)
                 return False
             else:
                 dest_file = os.path.join(
                     self.model_path, 'smiles_applicability_eval',
                     'applicabilitypredictor.h5')
                 if not os.path.isfile(dest_file):
                     self.learn_sign0_conf(
-                        sign0, sign3, suffix='eval', evaluate=True)
+                        sign0, sign3, self.params['sign0_conf'].copy(),
+                        suffix='eval', evaluate=True)
             # check if we have the final trained model
             dest_file = os.path.join(self.model_path,
                                      'smiles_applicability_final',
                                      'applicabilitypredictor.h5')
             if not os.path.isfile(dest_file):
                 self.update_status("Fitting final confidence model")
                 self.learn_sign0_conf(
-                    sign0, sign3, suffix='final', evaluate=False)
+                    sign0, sign3, self.params['sign0_conf'].copy(),
+                    suffix='final', evaluate=False)
         # predict for CC universe
         self.update_status("Predicting for CC universe")
         self.predict_from_sign0(sign0, self.data_path)
         # save reference
-        self.save_reference()
+        self.save_reference(overwrite=True)
         # finalize signature
         BaseSignature.fit_end(self, **kwargs)
 
     def get_predict_fn(self, model='smiles_final'):
         try:
             from chemicalchecker.tool.smilespred import Smilespred
         except ImportError as err:
             raise err
         model_path = os.path.join(self.model_path, model)
-        model = Smilespred(model_path)
+        model = Smilespred(model_path, save_params=False)
         return model.predict
 
     def get_applicability_predict_fn(self, model='smiles_applicability_final'):
         try:
             from chemicalchecker.tool.smilespred import ApplicabilityPredictor
         except ImportError as err:
             raise err
         model_path = os.path.join(self.model_path, model)
-        model = ApplicabilityPredictor(model_path)
+        model = ApplicabilityPredictor(model_path, save_params=False)
         return model.predict
 
     def predict_from_smiles(self, smiles, dest_file, **kwargs):
         return self.predict_from_string(smiles, dest_file, keytype='SMILES',
                                         **kwargs)
 
-    def predict_from_sign0(self, sign0, dest_file, chunk_size=1000, **kwargs):
+    def predict_from_sign0(self, sign0, dest_file, chunk_size=1000, y_order=None,
+                           **kwargs):
         # load NN
         predict_fn = self.get_predict_fn()
         appl_fn = self.get_applicability_predict_fn()
         # we return a simple DataSignature object (basic HDF5 access)
         pred_s3 = DataSignature(dest_file)
         # load novelty model for more accurate novelty scores (slower)
         with h5py.File(dest_file, "w") as results:
             results.create_dataset('keys', data=np.array(
-                    sign0.keys, DataSignature.string_dtype()))
+                sign0.keys, DataSignature.string_dtype()))
+            results.create_dataset(
+                'applicability', (len(sign0.keys), 1), dtype=np.float32)
             results.create_dataset(
-                    'applicability', (len(sign0.keys), 1), dtype=np.float32)
-            results.create_dataset( 
                 'V', (len(sign0.keys), 128), dtype=np.float32)
             results.create_dataset("shape", data=(len(sign0.keys), 128))
-            # sign0 must be reordered
-            order = np.argsort(sign0.get_h5_dataset('features').astype(int))
+            # sign0 reorder
+            if y_order is None:
+                y_order = np.arange(2048)
+            if 'features' in sign0.info_h5:
+                y_order = np.argsort(sign0.get_h5_dataset('features').astype(int))
             cs = chunk_size
             for chunk, rows in sign0.chunk_iter('V', cs, axis=0, chunk=True):
-                rows = rows[:, order]
+                rows = rows[:, y_order]
                 preds = predict_fn(rows)
                 # save chunk to H5
                 results['V'][chunk] = preds[:]
                 # also run applicability prediction
                 apreds = appl_fn(rows)
                 results['applicability'][chunk] = apreds[:]
         return pred_s3
 
-    def predict_from_string(self, molecules, dest_file, keytype='SMILES', 
-                chunk_size=1000, predict_fn=None, keys=None, components=128,
-                applicability=True, y_order=None):
+    def predict_from_string(self, molecules, dest_file, keytype='SMILES',
+                            chunk_size=1000, predict_fn=None, keys=None,
+                            components=128, applicability=True, y_order=None):
         """Given molecuel string, generate MFP and predict sign3.
 
         Args:
             molecules(list): A list of molecules strings.
             dest_file(str): File where to save the predictions.
             keytype(str): Wether to interpret molecules as InChI or SMILES.
         Returns:
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/signature_base.py` & `chemicalchecker-1.0.3/chemicalchecker/core/signature_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,27 +149,27 @@
         """Remove everything from this signature."""
         self.__log.debug("Clearing signature %s" % self.signature_path)
         if os.path.exists(self.data_path):
             # self.__log.debug("Removing %s" % self.data_path)
             os.remove(self.data_path)
         if os.path.exists(self.model_path):
             # self.__log.debug("Removing %s" % self.model_path)
-            shutil.rmtree(self.model_path)
+            shutil.rmtree(self.model_path, ignore_errors=True)
             original_umask = os.umask(0)
             os.makedirs(self.model_path, 0o775)
             os.umask(original_umask)
         if os.path.exists(self.stats_path):
             # self.__log.debug("Removing %s" % self.stats_path)
-            shutil.rmtree(self.stats_path)
+            shutil.rmtree(self.stats_path, ignore_errors=True)
             original_umask = os.umask(0)
             os.makedirs(self.stats_path, 0o775)
             os.umask(original_umask)
         if os.path.exists(self.diags_path):
             # self.__log.debug("Removing %s" % self.diags_path)
-            shutil.rmtree(self.diags_path)
+            shutil.rmtree(self.diags_path, ignore_errors=True)
             original_umask = os.umask(0)
             os.makedirs(self.diags_path, 0o775)
             os.umask(original_umask)
 
     def clear_all(self):
         """Remove everything from this signature for both referene and full."""
         ref = self.get_molset('reference')
@@ -303,27 +303,35 @@
         Args:
             args(tuple): the arguments for of the fit method
             kwargs(dict): arguments for the HPC method.
         """
         # read config file,# NS: get the cc_config var otherwise set it to
         # os.environ['CC_CONFIG']
         cc_config = kwargs.get("cc_config", os.environ['CC_CONFIG'])
+        self.__log.debug(
+            "CC_Config for function {} is: {}".format(func_name, cc_config))
         cfg = Config(cc_config)
 
         # create job directory if not available
         job_base_path = cfg.PATH.CC_TMP
-        tmp_dir = tempfile.mktemp(prefix='tmp_', dir=job_base_path)
+
+        job_name = "_".join(["CC", self.cctype.upper(), self.dataset,
+                             func_name, '_'])
+        tmp_dir = tempfile.mktemp(prefix=job_name, dir=job_base_path)
+
         job_path = kwargs.get("job_path", tmp_dir)
         if not os.path.isdir(job_path):
             os.mkdir(job_path)
         # check cpus
         cpu = kwargs.get("cpu", 1)
         # create script file
         script_lines = [
             "import os, sys",
+            "from chemicalchecker import ChemicalChecker",
+            "ChemicalChecker.set_verbosity('DEBUG')",
             "os.environ['OMP_NUM_THREADS'] = str(%s)" % cpu,
             "import pickle",
             "sign, args = pickle.load(open(sys.argv[1], 'rb'))",
             "sign.%s(*args)" % func_name,
             "print('JOB DONE')"
         ]
         if kwargs.get("delete_job_path", False):
@@ -343,26 +351,27 @@
         pickle_path = os.path.join(job_path, pickle_file)
         pickle.dump((self, args), open(pickle_path, 'wb'))
 
         # hpc parameters
         params = kwargs
         params["num_jobs"] = 1
         params["jobdir"] = job_path
-        params["job_name"] = script_name
-        params["wait"] = False
+        params["job_name"] = job_name
+        params["wait"] = kwargs.get("wait", False)
 
         # job command
         singularity_image = cfg.PATH.SINGULARITY_IMAGE
         command = "SINGULARITYENV_PYTHONPATH={} SINGULARITYENV_CC_CONFIG={}" +\
             " singularity exec {} python {} {}"
         command = command.format(
             os.path.join(cfg.PATH.CC_REPO, 'package'), cc_config,
             singularity_image, script_name, pickle_file)
         # submit jobs
-        cluster = HPC.from_config(cfg)
+        hpc_cfg = kwargs.get("hpc_cfg", cfg)
+        cluster = HPC.from_config(hpc_cfg)
         cluster.submitMultiJob(command, **params)
         return cluster
 
     def fit_hpc(self, *args, **kwargs):
         """Execute the fit method on the configured HPC.
 
         Args:
@@ -411,19 +420,28 @@
     @property
     def qualified_name(self):
         """Signature qualified name (e.g. 'B1.001-sign1-full')."""
         return "%s_%s_%s" % (self.dataset, self.cctype, self.molset)
 
     def get_molset(self, molset):
         '''Return a signature from a different molset'''
+        from .sign0 import sign0
+        from .sign1 import sign1
+        from .sign2 import sign2
+        from .sign3 import sign3
+        from .sign4 import sign4
+        from .neig import neig
         folds = self.signature_path.split('/')
         folds[-5] = molset
         new_path = '/'.join(folds)
-        newsign = self.__class__(new_path, self.dataset)
-        return newsign
+        if self.cctype.startswith('sign'):
+            sign_molset = eval(self.cctype)(new_path, self.dataset)
+        else:
+            sign_molset = eval(self.cctype[:-1])(new_path, self.dataset)
+        return sign_molset
 
     def get_neig(self):
         '''Return the neighbors signature, given a signature'''
         from .neig import neig
         folds = self.signature_path.split('/')
         folds[-1] = "neig%s" % folds[-1][-1]
         new_path = "/".join(folds)
@@ -499,19 +517,43 @@
         if 'features' in f5.keys():
             features = f5['features'][:]
             f5.close()
             with h5py.File(sign_ref.data_path, 'a') as hf:
                 hf.create_dataset('features', data=features)
         return sign_ref
 
-    def background_distances(self, metric):
+    def save_full(self, overwrite=False):
+        """Map the non redundant signature in explicit full molset.
+
+        It generates a new signature in the full folders.
+
+        Args:
+            overwrite(bool): Overwrite existing (default=False).
+        """
+        if "sign" not in self.cctype:
+            raise Exception("Only sign* are allowed.")
+        if self.molset == 'full':
+            raise Exception("This is already `full` molset.")
+        sign_full = self.get_molset("full")
+        if os.path.exists(sign_full.data_path):
+            if not overwrite:
+                raise Exception("%s exists" % sign_full.data_path)
+        self.apply_mappings(sign_full.data_path)
+
+    def background_distances(self, metric, limit_inks=None, name=None):
         """Return the background distances according to the selected metric.
 
         Args:
             metric(str): the metric name (cosine or euclidean).
         """
         sign_ref = self
         if self.molset != 'reference':
             sign_ref = self.get_molset("reference")
-        bg_file = os.path.join(sign_ref.model_path,
-                               "bg_%s_distances.h5" % metric)
-        return sign_ref.compute_distance_pvalues(bg_file, metric)
+        if limit_inks is None and name is None:
+            bg_file = os.path.join(sign_ref.model_path,
+                                   "bg_%s_distances.h5" % metric)
+            return sign_ref.compute_distance_pvalues(bg_file, metric)
+        else:
+            bg_file = os.path.join(sign_ref.model_path,
+                                   "bg_%s_%s_distances.h5" % (metric, name))
+            return sign_ref.compute_distance_pvalues(bg_file, metric,
+                                                     limit_inks=limit_inks)
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/signature_data.py` & `chemicalchecker-1.0.3/chemicalchecker/core/signature_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,52 +5,63 @@
 brackets [:] operator). It expose utility methods to fetch, stack, copy
 check for consistency, index, subsample or map signatures.
 """
 import os
 import sys
 import h5py
 import numpy as np
+import pandas as pd
 from tqdm import tqdm
 from bisect import bisect_left
 from scipy.spatial.distance import euclidean, cosine
 from scipy.spatial.distance import jaccard as tanimoto
 
 from chemicalchecker.util import logged
 from chemicalchecker.util.decorator import cached_property
 
+try:
+    import torch
+except:
+    pass
+
 
 @logged
 class DataSignature(object):
     """DataSignature class."""
 
     def __init__(self, data_path, ds_data='V', keys_name='keys'):
         """Initialize a DataSignature instance."""
         self.data_path = os.path.abspath(data_path)
         self.ds_data = ds_data
         self.keys_name = keys_name
         self.PVALRANGES = np.array(
             [0, 0.001, 0.01, 0.1] + list(np.arange(1, 100)) + [100]) / 100.
 
-    def add_datasets(self, data_dict, overwrite=True):
+    def add_datasets(self, data_dict, overwrite=True, chunks=None,
+                     compression=None):
         """Add dataset to a H5"""
         for k, v in data_dict.items():
             with h5py.File(self.data_path, 'a') as hf:
                 if k in hf.keys():
                     if overwrite:
                         del hf[k]
                     else:
                         self.__log.info('Skipping `%s~`: already there')
                         continue
                 if isinstance(v, list):
-                    if hasattr(v[0], 'decode') or isinstance(v[0], str) or isinstance(v[0], np.str_):
+                    if (hasattr(v[0], 'decode') or isinstance(v[0], str) or
+                            isinstance(v[0], np.str_)):
                         v = self.h5_str(v)
                 else:
-                    if hasattr(v.flat[0], 'decode') or isinstance(v.flat[0], str) or isinstance(v.flat[0], np.str_):
+                    if (hasattr(v.flat[0], 'decode')
+                        or isinstance(v.flat[0], str)
+                            or isinstance(v.flat[0], np.str_)):
                         v = self.h5_str(v)
-                hf.create_dataset(k, data=v)
+                hf.create_dataset(k, data=v, chunks=chunks,
+                                  compression=compression)
 
     def _check_data(self):
         """Test if data file is available"""
         if not os.path.isfile(self.data_path):
             raise Exception("Data file %s not available." % self.data_path)
 
     def _check_dataset(self, key):
@@ -63,34 +74,34 @@
         with h5py.File(self.data_path, 'w') as hf:
             pass
 
     def _get_shape(self, key, axis=None):
         """Get shape of dataset"""
         with h5py.File(self.data_path, 'r') as hf:
             data = hf[key].shape
-            if axis != None:
-                if len(data) == axis:
-                    return data[0]
-                return data[axis]
-            else:
-                return data
+        if axis != None:
+            if len(data) == axis:
+                return data[0]
+            return data[axis]
+        else:
+            return data
 
     def _get_dtype(self, key):
         """Get shape of dataset"""
         with h5py.File(self.data_path, 'r') as hf:
             data = hf[key][0].flat[0].dtype
-            return data
+        return data
 
     def _get_all(self, key):
         """Get complete dataset"""
         with h5py.File(self.data_path, 'r') as hf:
             data = hf[key][:]
-            if hasattr(data.flat[0], 'decode'):
-                return data.astype(str)
-            return data
+        if hasattr(data.flat[0], 'decode'):
+            return data.astype(str)
+        return data
 
     def _get_data_chunk(self, handle, key, chunk, axis=0):
         """Get chunk of dataset"""
         if axis == 0:
             data = handle[key][chunk]
         else:
             data = handle[key][:, chunk]
@@ -99,23 +110,25 @@
         return data
 
     def chunk_iter(self, key, chunk_size, axis=0, chunk=False, bar=True):
         """Iterator on chunks of data"""
         self._check_data()
         self._check_dataset(key)
         tot_size = self._get_shape(key, axis)
-        with h5py.File(self.data_path, 'r') as hf:
-            myrange = range(0, tot_size, chunk_size)
-            desc = 'Iterating on `%s` axis %s' % (key, axis)
-            for i in tqdm(myrange, disable=not bar, desc=desc):
-                mychunk = slice(i, i + chunk_size)
-                if chunk:
-                    yield mychunk, self._get_data_chunk(hf, key, mychunk, axis)
-                else:
-                    yield self._get_data_chunk(hf, key, mychunk, axis)
+        if not hasattr(self, 'hdf5'):
+            self.open_hdf5()
+        hf = self.hdf5
+        myrange = range(0, tot_size, chunk_size)
+        desc = 'Iterating on `%s` axis %s' % (key, axis)
+        for i in tqdm(myrange, disable=not bar, desc=desc):
+            mychunk = slice(i, i + chunk_size)
+            if chunk:
+                yield mychunk, self._get_data_chunk(hf, key, mychunk, axis)
+            else:
+                yield self._get_data_chunk(hf, key, mychunk, axis)
 
     def __iter__(self):
         """By default iterate on signatures V."""
         self._check_data()
         self._check_dataset(self.ds_data)
         with h5py.File(self.data_path, 'r') as hf:
             for i in range(self.shape[0]):
@@ -239,23 +252,25 @@
 
     @property
     def shape(self):
         """Get the V matrix shape."""
         self._check_data()
         self._check_dataset(self.ds_data)
         with h5py.File(self.data_path, 'r') as hf:
-            return hf[self.ds_data].shape
+            shape = hf[self.ds_data].shape
+        return shape
 
     @property
     def size(self):
         """Get the V matrix size."""
         self._check_data()
         self._check_dataset(self.ds_data)
         with h5py.File(self.data_path, 'r') as hf:
-            return hf[self.ds_data].size
+            size = hf[self.ds_data].size
+        return size
 
     @staticmethod
     def string_dtype():
         if sys.version_info[0] == 2:
             import unicode
             # this works in py2 and fails in py3
             return h5py.special_dtype(vlen=unicode)
@@ -264,94 +279,113 @@
             # return h5py.special_dtype(vlen=str)
             return h5py.string_dtype(encoding='utf-8', length=None)  # NS test
 
     @staticmethod
     def h5_str(lst):
         return np.array(lst, dtype=DataSignature.string_dtype())
 
-    def copy_from(self, sign, key):
+    def copy_from(self, sign, key, chunk=None):
         """Copy dataset 'key' to current signature.
 
         Args:
             sign(SignatureBase): The source signature.
             key(str): The dataset to copy from.
         """
         sign._check_data()
         sign._check_dataset(key)
         with h5py.File(sign.data_path, 'r') as hf:
-            src = hf[key][:]
+            if chunk is not None:
+                src = hf[key][chunk]
+            else:
+                src = hf[key][:]
         with h5py.File(self.data_path, 'a') as hf:
             # delete if already there
             if key in hf:
                 del hf[key]
             hf[key] = src
 
     def make_filtered_copy(self, destination, mask, include_all=False,
-                           data_file=None):
+                           data_file=None, datasets=None, dst_datasets=None,
+                           chunk_size=1000, compression=None):
         """Make a copy of applying a filtering mask on rows.
 
         destination (str): The destination file path.
         mask (bool array): A numpy mask array (e.g. result of `np.isin`)
         include_all (bool): Whether to copy other dataset (e.g. features,
             date, name...)
         data_file (str): A specific file to copy (by default is the signature
             h5)
         """
 
         if data_file is None:
             data_file = self.data_path
 
         with h5py.File(data_file, 'r') as hf_in:
-            with h5py.File(destination, 'w') as hf_out:
-                for dset in hf_in.keys():
+            with h5py.File(destination, 'a') as hf_out:
+                if datasets is None:
+                    datasets = hf_in.keys()
+                if dst_datasets is None:
+                    dst_datasets = datasets
+                for dset, dst_dset in zip(datasets, dst_datasets):
+
                     # skip dataset incompatible with mask (or copy unmasked)
                     if hf_in[dset].shape[0] != mask.shape[0]:
                         if not include_all:
                             continue
                         else:
                             masked = hf_in[dset][:][:]
-                            hf_out.create_dataset(dset, data=masked)
+                            hf_out.create_dataset(dst_dset, data=masked,
+                                                  compression=compression)
                             self.__log.debug("Copy dataset %s of shape %s" %
                                              (dset, str(masked.shape)))
                             continue
+
                     # never mask features
                     if dset == 'features':
                         masked = hf_in[dset][:][:]
                         self.__log.debug("Copy dataset %s of shape %s" %
                                          (dset, str(masked.shape)))
-                        hf_out.create_dataset(dset, data=masked)
+                        hf_out.create_dataset(dst_dset, data=masked,
+                                              compression=compression)
                         continue
-                    # memory safe masked copy for other datasets
+
+                    # mask single value dataset all at once
                     if len(hf_in[dset].shape) == 1:
-                        final_shape = (sum(mask),)
-                    else:
-                        final_shape = (sum(mask), hf_in[dset].shape[1])
+                        masked = hf_in[dset][:][mask]
+                        self.__log.debug("Copy dataset %s of shape %s" %
+                                         (dset, str(masked.shape)))
+                        hf_out.create_dataset(dst_dset, data=masked,
+                                              compression=compression)
+                        continue
+
+                    # memory safe masked copy for other datasets
+                    final_shape = (sum(mask), hf_in[dset].shape[1])
                     hf_out.create_dataset(
-                        dset, final_shape, dtype=hf_in[dset].dtype)
+                        dst_dset, final_shape, dtype=hf_in[dset].dtype,
+                        compression=compression)
                     self.__log.debug("Copy dataset %s of shape %s" %
                                      (dset, str(final_shape)))
-                    idx_dst = 0
-                    for idx_src in np.argwhere(mask).ravel():
-                        hf_out[dset][idx_dst] = hf_in[dset][idx_src]
-                        idx_dst += 1
+                    for chunk, data in self.chunk_iter(dset, 100, 1, True):
+                        hf_out[dst_dset][:, chunk] = data[mask]
 
     def filter_h5_dataset(self, key, mask, axis, chunk_size=1000):
         """Apply a maks to a dataset, dropping columns or rows.
 
         key (str): The H5 dataset to filter.
         mask (np.array): A bool one dimensional mask array. True values will
             be kept.
         axis (int): Wether the mask refers to rows (0) or columns (1).
         """
         self._check_dataset(key)
         if self._get_shape(key, axis) != mask.shape[0]:
             raise Exception("Shape mismatch:", self._get_shape(
                 key, axis), mask.shape[0])
         key_tmp = "%s_tmp" % key
-        with h5py.File(self.data_path, "a") as hf:
+        self.close_hdf5()
+        with h5py.File(self.data_path, 'a') as hf:
             if key_tmp in hf.keys():
                 self.__log.debug('Deleting pre-existing `%s`' % key_tmp)
                 del hf[key_tmp]
             # if we have a list directly apply the mask
             if hf[key].ndim == 1:
                 hf.create_dataset(key_tmp, (sum(mask),), dtype=hf[key].dtype)
                 hf[key_tmp][:] = hf[key][mask]
@@ -404,63 +438,82 @@
                     tmp = list()
                     for idx, sign in enumerate(sign_list):
                         with h5py.File(sign.data_path, 'r') as hf_in:
                             tmp.append(hf_in[key][:])
                     results.create_dataset(key, data=np.vstack(tmp).T)
 
     @staticmethod
-    def vstack_signatures(sign_list, destination, chunk_size=1000):
-        """Merge horizontally a list of signatures."""
+    def vstack_signatures(sign_list, destination, chunk_size=10000,
+                          vchunk_size=100):
+        """Merge vertically a list of signatures."""
         hsizes = [s.shape[1] for s in sign_list]
         vsizes = [s.shape[0] for s in sign_list]
         if not all([hsizes[0] == h for h in hsizes]):
             raise ValueError('All signatures must have same features.')
+        # the set of keys must be disjoint
+        all_keys = [s.keys for s in sign_list]
+        if len(set.intersection(*[set(x) for x in all_keys])) != 0:
+            raise ValueError('All signatures must have different molecules.')
 
         with h5py.File(destination, "w") as results:
-            results.create_dataset('keys', data=np.array(
-                np.hstack([s.keys for s in sign_list]),
-                DataSignature.string_dtype()))
+            # we reorder already keys
+            all_keys_array = np.array(np.hstack(all_keys),
+                                      DataSignature.string_dtype())
+            order = np.argsort(all_keys_array)
+            results.create_dataset('keys', data=all_keys_array[order])
             results.create_dataset("V", (sum(vsizes), hsizes[0]))
-
+            # copy the stacked V matrices
             for idx, sign in enumerate(sign_list):
                 with h5py.File(sign.data_path, 'r') as hf_in:
-                    for i in range(0, vsizes[idx], chunk_size):
+                    for i in tqdm(range(0, vsizes[idx], chunk_size),
+                                  desc='copying V'):
                         if i + chunk_size > vsizes[idx]:
                             end = vsizes[idx]
                         else:
                             end = i + chunk_size
                         vchunk_src = slice(i, end)
                         vchunk_dst = slice(sum(vsizes[:idx]) + i,
                                            sum(vsizes[:idx]) + end)
                         results['V'][vchunk_dst] = hf_in['V'][vchunk_src]
+            # reorder vertical chunks
+            vrange = range(0, hsizes[0], vchunk_size)
+            for i in tqdm(vrange, desc='reordering rows'):
+                vchunk = slice(i, i + vchunk_size)
+                results['V'][:, vchunk] = results['V'][:, vchunk][order]
 
     def get_h5_dataset(self, h5_dataset_name, mask=None):
         """Get a specific dataset in the signature."""
         self.__log.debug("Fetching dataset %s" % h5_dataset_name)
         self._check_data()
         with h5py.File(self.data_path, 'r') as hf:
             if h5_dataset_name not in hf.keys():
                 raise Exception("HDF5 file has no '%s'." % h5_dataset_name)
             if mask is None:
                 ndim = hf[h5_dataset_name].ndim
                 if hasattr(hf[h5_dataset_name][(0,) * ndim], 'decode'):
-                    return hf[h5_dataset_name][:].astype(str)
+                    data = hf[h5_dataset_name][:].astype(str)
                 else:
-                    return hf[h5_dataset_name][:]
+                    data = hf[h5_dataset_name][:]
             else:
                 tmp = mask.ravel()[0]
                 if isinstance(tmp, np.bool_) or isinstance(tmp, bool):
                     mask = np.argwhere(mask.ravel()).ravel()
                 ndim = hf[h5_dataset_name].ndim
                 if hasattr(hf[h5_dataset_name][(0,) * ndim], 'decode'):
-                    return hf[h5_dataset_name][mask].astype(str)
+                    data = hf[h5_dataset_name][mask].astype(str)
                 else:
-                    return hf[h5_dataset_name][mask, :]
+                    data = hf[h5_dataset_name][mask, :]
+        return data
+
+    def as_dataframe(self):
+        df = pd.DataFrame(self[:], columns=self.features, index=self.keys)
+        return df
 
-    def get_vectors(self, keys, include_nan=False, dataset_name='V', output_missing=False):
+    def get_vectors(self, keys, include_nan=False, dataset_name='V',
+                    output_missing=False):
         """Get vectors for a list of keys, sorted by default.
 
         Args:
             keys(list): a List of string, only the overlapping subset to the
                 signature keys is considered.
             include_nan(bool): whether to include requested but absent
                 molecule signatures as NaNs.
@@ -500,15 +553,14 @@
         sort_idx = np.argsort(inks)
         if output_missing:
             return inks[sort_idx], signs[sort_idx], missed_inks
         return inks[sort_idx], signs[sort_idx]
 
     def get_vectors_lite(self, keys, chunk_size=2000, chunk_above=10000):
         """Iterate on signatures."""
-        from tqdm import tqdm
         keys = set(keys)
         idxs = []
         mask = []
         kept_keys = []
         for i, key in enumerate(self.keys):
             if key not in keys:
                 mask += [False]
@@ -553,50 +605,73 @@
             index(int): Index in the matrix
         """
         if key not in self.unique_keys:
             raise Exception("Key '%s' not found." % key)
         idx = bisect_left(self.keys, key)
         return idx
 
+    def open_hdf5(self, mode='r'):
+        self.close_hdf5()
+        self.hdf5 = h5py.File(self.data_path, mode, rdcc_nbytes=100*1024**2)
+
+    def close_hdf5(self):
+        if hasattr(self, 'hdf5'):
+            self.hdf5.close()
+            del self.hdf5
+
+    def __del__(self):
+        self.close_hdf5()
+
+    def __len__(self):
+        if not hasattr(self, 'hdf5'):
+            self.open_hdf5()
+        return len(self.hdf5[self.ds_data])
+
     def __getitem__(self, key):
         """Return the vector corresponding to the key.
 
         The key can be a string (then it's mapped though self.keys) or and
         int.
         Works fast with bisect, but should return None if the key is not in
         keys (ideally, keep a set to do this)."""
         self._check_data()
+        #self.__log.debug("__getitem__  key: %s type: %s" % (key, type(key)))
+        if not hasattr(self, 'hdf5'):
+            self.open_hdf5()
+        if isinstance(key, int):
+            self.hdf5[self.ds_data][key]
+            return self.hdf5[self.ds_data][key]
+        if isinstance(key, list):
+            key = slice(min(key), max(key)+1)
+        if isinstance(key, slice):
+            return self.hdf5[self.ds_data][key]
         if isinstance(key, bytes):
             key = key.decode("utf-8")
-        if isinstance(key, slice):
-            with h5py.File(self.data_path, 'r') as hf:
-                return hf[self.ds_data][key]
-        elif isinstance(key, str):
+        if isinstance(key, str):
             if key not in self.unique_keys:
                 raise Exception("Key '%s' not found." % key)
             idx = bisect_left(self.keys, key)
-            with h5py.File(self.data_path, 'r') as hf:
-                return hf[self.ds_data][idx]
-        elif isinstance(key, int):
-            with h5py.File(self.data_path, 'r') as hf:
-                return hf[self.ds_data][key]
+            return self.hdf5[self.ds_data][idx]
         else:
             raise Exception("Key type %s not recognized." % type(key))
 
     def compute_distance_pvalues(self, bg_file, metric, sample_pairs=None,
-                                 unflat=True, memory_safe=False):
+                                 unflat=True, memory_safe=False,
+                                 limit_inks=None):
         """Compute the distance pvalues according to the selected metric.
 
         Args:
             bg_file(Str): The file where to store the distances.
             metric(str): the metric name (cosine or euclidean).
             sample_pairs(int): Amount of pairs for distance calculation.
             unflat(bool): Remove flat regions whenever we observe them.
             memory_safe(bool): Computing distances is much faster if we can
                 load the full matrix in memory.
+            limit_inks(list): Compute distances only for this subset on
+                inchikeys.
         Returns:
             bg_distances(dict): Dictionary with distances and Pvalues
         """
         # lazily read already computed distance
         metric = metric.lower()
         if os.path.isfile(bg_file):
             self.__log.info("Reading bg_distances file for metric: " + metric)
@@ -612,49 +687,68 @@
             raise Exception("Specified metric %s not available." % metric)
         # the 'tanimoto' distance is what is implemented in scipy as 'jaccard'
         # but we prefere tanimoto as a name
         if metric == 'jaccard':
             metric = 'tanimoto'
         metric_fn = eval(metric)
         # sample distances
-        if memory_safe:
+        keys = self.keys
+        nr_mols = len(keys)
+        if limit_inks is not None:
+            nr_mols = len(limit_inks)
+            mask = np.isin(keys, limit_inks)
+            matrix = self[:][mask]
+        elif memory_safe:
             matrix = self
         else:
             matrix = self[:]
         # how many molecules gives a proper sampling?
         if sample_pairs is None:
             # p and q are fixed parameters
             p, q = 0.5, 0.5
-            # 5% confidence, 95% precision
+            # 5% confidence, 95% precision (1.96 is stddev for 95% AUC)
             d, Z = 0.05, 1.96
             coef = Z**2 * p * q
-            k = (coef * len(self.keys)) / (d**2 * (len(self.keys) - 1) + coef)
+            k = (coef * nr_mols) / (d**2 * (nr_mols - 1) + coef)
             sample_pairs = int(np.ceil(k**2))
         self.__log.info("Background distances sample_pairs: %s" % sample_pairs)
-        if matrix.shape[0]**2 < sample_pairs:
+        if nr_mols**2 < sample_pairs:
             self.__log.warn("Requested more pairs then possible combinations")
-            sample_pairs = matrix.shape[0]**2 - matrix.shape[0]
+            sample_pairs = nr_mols**2 - nr_mols
         bg = list()
         done = set()
         tries = 1e6
         tr = 0
+        identical = 0
+        nan = 0
         while len(bg) < sample_pairs and tr < tries:
             tr += 1
             i = np.random.randint(0, matrix.shape[0] - 1)
             j = np.random.randint(i + 1, matrix.shape[0])
             if (i, j) not in done:
                 dist = metric_fn(matrix[i], matrix[j])
                 if dist == 0.0:
-                    self.__log.warn("Identical signatures for %s %s" % (i, j))
+                    identical += 1
+                    continue
                 if np.isnan(dist):
-                    self.__log.warn("NaN distance for %s %s" % (i, j))
+                    nan += 1
                     continue
                 bg.append(dist)
                 done.add((i, j))
-        # pavalues as percentiles
+            if identical > 10000:
+                self.__log.warn("Identical signatures for 1000 pairs")
+                identical = 0
+            if nan > 10000:
+                self.__log.warn("NaN distances for 1000 pairs")
+                nan = 0
+        if tr == tries:
+            self.__log.warn("Something went wrong... we reached the maximum "
+                            "number of trials in computing distances. "
+                            "Please disregard the thresholds, double check!")
+        # pvalues as percentiles
         i = 0
         PVALS = [(0, 0., i)]  # DISTANCE, RANK, INTEGER
         i += 1
         percs = self.PVALRANGES[1:-1] * 100
         for perc in percs:
             PVALS += [(np.percentile(bg, perc), perc / 100., i)]
             i += 1
@@ -694,15 +788,15 @@
             Returns:
                V(matrix): A (samples, features) matrix.
                keys(array): The list of keys.
         """
         np.random.seed(seed)
         if n >= len(self.keys):
             self.__log.debug("Full dataset sampled (n=%d)" % len(self.keys))
-            V = self[:]
+            V = self.get_h5_dataset('V')
             keys = self.keys
         else:
             self.__log.debug("Subsampling dataset (n=%d)" % n)
             idxs = np.array(sorted(np.random.choice(
                 len(self.keys), n, replace=False)))
             with h5py.File(self.data_path, "r") as hf:
                 V = hf["V"][idxs]
@@ -746,63 +840,68 @@
         V_full = self_full.get_vectors(ref_inks)[1]
         V_ref = self_ref.get_vectors(ref_inks)[1]
         try:
             np.testing.assert_allclose(V_full, V_ref)
         except Exception:
             raise Exception("`reference` to `full` mismatch.")
 
-    def map(self, out_file):
+    def apply_mappings(self, out_file, mappings=None):
         """Map signature throught mappings."""
-        if "mappings" not in self.info_h5:
-            raise Exception("Data file has no mappings.")
-        with h5py.File(self.data_path, 'r') as hf:
-            mappings_raw = hf['mappings'][:]
-        mappings = dict(mappings_raw)
+        if mappings is None:
+            if "mappings" not in self.info_h5:
+                raise Exception("Data file has no mappings.")
+            mappings_raw = self.get_h5_dataset('mappings')
+            mappings = dict(mappings_raw)
         # avoid trivial mappings (where key==value)
         to_map = list(set(mappings.keys()) - set(mappings.values()))
         if len(to_map) == 0:
             # corner case where there's nothing to map
             with h5py.File(self.data_path, 'r') as hf:
                 src_keys = hf['keys'][:]
                 src_vectors = hf['V'][:]
             with h5py.File(out_file, "w") as hf:
                 hf.create_dataset('keys', data=np.array(
-                    src_keys, DataSignature.string_dtype()), dtype=DataSignature.string_dtype())
+                    src_keys, DataSignature.string_dtype()),
+                    dtype=DataSignature.string_dtype())
                 hf.create_dataset('V', data=src_vectors, dtype=np.float32)
                 hf.create_dataset("shape", data=src_vectors.shape)
             return
         # prepare key-vector arrays
         dst_keys = list()
         dst_vectors = list()
         for dst_key in sorted(to_map):
             dst_keys.append(dst_key)
             dst_vectors.append(self[mappings[dst_key]])
+        self.close_hdf5()
         # to numpy arrays
         dst_keys = np.array(dst_keys)
         matrix = np.vstack(dst_vectors)
         # join with current key-signatures
         with h5py.File(self.data_path, 'r') as hf:
             src_vectors = hf['V'][:]
         dst_keys = np.concatenate((dst_keys, self.keys))
         matrix = np.concatenate((matrix, src_vectors))
         # get them sorted
         sorted_idx = np.argsort(dst_keys)
         with h5py.File(out_file, "w") as hf:
             hf.create_dataset('keys', data=np.array(
-                dst_keys[sorted_idx], DataSignature.string_dtype()), dtype=DataSignature.string_dtype())
+                dst_keys[sorted_idx], DataSignature.string_dtype()),
+                dtype=DataSignature.string_dtype())
             hf.create_dataset('V', data=matrix[sorted_idx], dtype=np.float32)
             hf.create_dataset("shape", data=matrix.shape)
 
-    def generator_fn(self, batch_size=None):
+    def generator_fn(self, weak_shuffle=False, batch_size=None):
         """Return the generator function that we can query for batches."""
         hf = h5py.File(self.data_path, 'r')
         dset = hf['V']
         total = dset.shape[0]
         if not batch_size:
             batch_size = total
+            weak_shuffle = False
+        n_batches = total / batch_size
 
         def _generator_fn():
             beg_idx, end_idx = 0, batch_size
             while True:
                 if beg_idx >= total:
                     self.__log.debug("EPOCH completed")
                     beg_idx = 0
@@ -810,10 +909,74 @@
                 yield dset[beg_idx: end_idx]
                 beg_idx, end_idx = beg_idx + batch_size, end_idx + batch_size
 
         return _generator_fn
 
     def export_features(self, destination='.'):
         features = self.features
-        with h5py.File(os.path.join(destination, "features_sign.h5"), 'w') as hf_out:
+        with h5py.File(os.path.join(destination,
+                                    "features_sign.h5"), 'w') as hf_out:
             hf_out.create_dataset("features", data=np.array(
                 features, DataSignature.string_dtype()))
+
+    def dataloader(self, batch_size=32, num_workers=1, shuffle=False,
+                   weak_shuffle=False, drop_last=False):
+        """Return a pytorch DataLoader object for quick signature iteration."""
+        if weak_shuffle:
+            return torch.utils.data.DataLoader(
+                self,
+                batch_size=None,  # must be disabled when using samplers
+                num_workers=num_workers,
+                shuffle=False,
+                sampler=torch.utils.data.BatchSampler(
+                    RandomBatchSampler(self, batch_size),
+                    batch_size=batch_size,
+                    drop_last=drop_last)
+            )
+        else:
+            return torch.utils.data.DataLoader(
+                self,
+                batch_size=batch_size,
+                num_workers=num_workers,
+                shuffle=shuffle
+            )
+
+
+try:
+    class RandomBatchSampler(torch.utils.data.Sampler):
+        """Sampling class to create random sequential batches of a dataset.
+
+        E.g. if data is [1,2,3,4] with bs=2. Then first batch, [[1,2], [3,4]]
+        then shuffle batches -> [[3,4],[1,2]]
+        This is useful for cases when you are interested in 'weak shuffling'
+        https://towardsdatascience.com/
+        reading-h5-files-faster-with-pytorch-datasets-3ff86938cc
+
+        :param dataset: dataset you want to batch
+        :type dataset: torch.utils.data.Dataset
+        :param batch_size: batch size
+        :type batch_size: int
+        :returns: generator object of shuffled batch indices
+        """
+
+        def __init__(self, dataset, batch_size):
+            self.batch_size = batch_size
+            self.dataset_length = len(dataset)
+            self.n_batches = self.dataset_length / self.batch_size
+            self.batch_ids = torch.randperm(int(self.n_batches))
+
+        def __len__(self):
+            return self.batch_size
+
+        def __iter__(self):
+            for id in self.batch_ids:
+                idx = torch.arange(id * self.batch_size,
+                                   (id + 1) * self.batch_size)
+                for index in idx:
+                    yield int(index)
+            if int(self.n_batches) < self.n_batches:
+                idx = torch.arange(int(self.n_batches) *
+                                   self.batch_size, self.dataset_length)
+                for index in idx:
+                    yield int(index)
+except:
+    pass
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/core/validation.py` & `chemicalchecker-1.0.3/chemicalchecker/core/validation.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/database/__init__.py` & `chemicalchecker-1.0.3/chemicalchecker/database/__init__.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/database/calcdata.py` & `chemicalchecker-1.0.3/chemicalchecker/database/calcdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import h5py
 import datetime
 import numpy as np
 from time import time
 
 from sqlalchemy import Column, Text
 from sqlalchemy.dialects import postgresql
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declarative_base
 
 from .database import get_session, get_engine
 from .molecule import Molecule
 
 from chemicalchecker.util import logged, Config
 from chemicalchecker.util.hpc import HPC
 from chemicalchecker.util.parser import DataCalculator
@@ -134,15 +134,15 @@
                 for ele in res:
                     present.add(ele[0])
 
             session.close()
 
             GenericCalcdata.__log.debug(
                 "Found already present: " + str(len(present)))
-            
+
             return set(keys).difference(present)
 
         @staticmethod
         def from_inchikey(inchikey, **kwargs):
             inchikey_inchi = Molecule.get_inchikey_inchi_mapping(inchikey)
             GenericCalcdata.from_inchikey_inchi(inchikey_inchi, **kwargs)
 
@@ -173,23 +173,25 @@
 
             Molecule.add_missing_only(inchikey_inchi_final)
             # parse_fn yield a list of dictionaries with keys as a molprop
             parse_fn = DataCalculator.calc_fn(GenericCalcdata.__tablename__)
             # profile time
             t_start = time()
             engine = get_engine(GenericCalcdata.dbname)
-            for chunk in parse_fn(dict_inchikey_inchi, chunksize):
-                if len(chunk) == 0:
-                    continue
-                GenericCalcdata.__log.debug(
-                    "Loading chunk of size: " + str(len(chunk)))
-                engine.execute(
-                    postgresql.insert(GenericCalcdata.__table__).values(
-                        chunk).on_conflict_do_nothing(
-                        index_elements=[GenericCalcdata.inchikey]))
+            with engine.begin() as conn:
+                for chunk in parse_fn(dict_inchikey_inchi, chunksize):
+                    if len(chunk) == 0:
+                        continue
+                    GenericCalcdata.__log.debug(
+                        "Loading chunk of size: " + str(len(chunk)))
+
+                    conn.execute(
+                        postgresql.insert(GenericCalcdata.__table__).values(
+                            chunk).on_conflict_do_nothing(
+                            index_elements=[GenericCalcdata.inchikey]))
             t_end = time()
             t_delta = str(datetime.timedelta(seconds=t_end - t_start))
             GenericCalcdata.__log.info(
                 "Loading Mol properties Name %s took %s",
                 GenericCalcdata.__tablename__, t_delta)
 
         @staticmethod
@@ -247,16 +249,17 @@
             params["elements"] = inchikey
             params["wait"] = wait
             params["cpu"] = cpu
             params["memory"] = memory
             params["compress"] = False
             # job command
             singularity_image = cfg.PATH.SINGULARITY_IMAGE
-            command = "SINGULARITYENV_PYTHONPATH={} SINGULARITYENV_CC_CONFIG={}" +\
-                " singularity exec {} python {} <TASK_ID> <FILE>"
+            command = ("SINGULARITYENV_PYTHONPATH={}"
+                       "SINGULARITYENV_CC_CONFIG={}"
+                       " singularity exec {} python {} <TASK_ID> <FILE>")
             command = command.format(
                 os.path.join(cfg.PATH.CC_REPO, 'package'), cc_config,
                 singularity_image, script_name)
             # submit jobs
             cluster = HPC.from_config(cfg)
             cluster.submitMultiJob(command, **params)
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/database/database.py` & `chemicalchecker-1.0.3/chemicalchecker/database/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 These utility functions allow class from this module to get engine and
 open session to the desired database. Also preppare the base class that will
 be extended by each :mod:`~chemicalchecker.database` class.
 """
 from sqlalchemy import create_engine
 from sqlalchemy.pool import NullPool
-from sqlalchemy.orm import sessionmaker
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import sessionmaker, declarative_base
 
 from chemicalchecker.util import Config
 
 # Construct a base class for declarative class definitions.
 Base = declarative_base()
 
 
@@ -73,15 +72,15 @@
     session = Session()
     return session
 
 
 def test_connection(dbname=None):
     engine = get_engine(dbname=dbname)
     try:
-        conn = engine.connect()
-        conn.close()
+        with engine.begin() as connection:
+            connection.close()
         engine.dispose()
 
     except Exception as e:
         return False
     else:
         return True
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/database/dataset.py` & `chemicalchecker-1.0.3/chemicalchecker/database/dataset.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/database/datasource.py` & `chemicalchecker-1.0.3/chemicalchecker/database/datasource.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/database/molecule.py` & `chemicalchecker-1.0.3/chemicalchecker/database/molecule.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,28 +57,29 @@
 
         Args:
             data(list): The data in list format. Each list member is a new row.
                 The order is important.
             chunk(int): The size of the chunks to load data to the database.
         """
         engine = get_engine()
-        for pos in range(0, len(data), chunk):
-            if on_conflict_do_nothing:
-                engine.execute(
-                    postgresql.insert(Molecule.__table__).values(
+        with engine.begin() as conn:
+            for pos in range(0, len(data), chunk):
+                if on_conflict_do_nothing:
+                    conn.execute(
+                        postgresql.insert(Molecule.__table__).values(
+                            [{"inchikey": row[0], "inchi": row[1]}
+                             for row in data[pos:pos + chunk]]
+                        ).on_conflict_do_nothing(
+                            index_elements=[Molecule.inchikey]))
+                else:
+                    conn.execute(
+                        Molecule.__table__.insert(),
                         [{"inchikey": row[0], "inchi": row[1]}
-                         for row in data[pos:pos + chunk]]
-                    ).on_conflict_do_nothing(
-                        index_elements=[Molecule.inchikey]))
-            else:
-                engine.execute(
-                    Molecule.__table__.insert(),
-                    [{"inchikey": row[0], "inchi": row[1]}
-                        for row in data[pos:pos + chunk]]
-                )
+                            for row in data[pos:pos + chunk]]
+                    )
 
     @staticmethod
     def get(key):
         """Method to query table."""
         session = get_session()
         query = session.query(Molecule).filter_by(inchikey=key)
         res = query.one_or_none()
@@ -91,15 +92,16 @@
     def get_inchikey_inchi_mapping(inchikeys, batch=10000):
         mapping = dict()
         for ink in inchikeys:
             mapping[ink] = None
 
         session = get_session()
         desc = 'Fetching InChIKey-InChI mapping'
-        for idx in trange(0, len(inchikeys), batch, desc=desc):
+        dis = len(inchikeys) < batch
+        for idx in trange(0, len(inchikeys), batch, desc=desc, disable=dis):
             query = session.query(Molecule).filter(
                 Molecule.inchikey.in_(inchikeys[idx:idx + batch]))
             res = query.with_entities(Molecule.inchikey, Molecule.inchi).all()
             mapping.update(dict(res))
 
         return mapping
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/database/molrepo.py` & `chemicalchecker-1.0.3/chemicalchecker/database/molrepo.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,17 +49,17 @@
     __tablename__ = 'molrepo'
     molrepo_name = Column(Text, primary_key=True)
     description = Column(Text)
     universe = Column(Boolean)
     essential = Column(Boolean)
 
     datasources = relationship("Datasource",
-                            secondary="molrepo_has_datasource",
-                            back_populates="molrepos",
-                            lazy='joined')
+                               secondary="molrepo_has_datasource",
+                               back_populates="molrepos",
+                               lazy='joined')
 
     def __repr__(self):
         """String representation."""
         return str(self.molrepo_name)
 
     @staticmethod
     def _create_table():
@@ -138,33 +138,35 @@
         """Write molecules InChI-Key, source_id, InChI and SMILES to CSV file.
 
         Args:
             filename(str): Path to a CSV file.
         """
         import pandas as pd
         molecules = Molrepo.get_by_molrepo_name(molrepo_name)
-        df = pd.DataFrame(molecules, columns=['molrepo','source_id','SMILES','InChIKey','InChI'])
+        df = pd.DataFrame(molecules, columns=['molrepo', 'source_id',
+                                              'SMILES', 'InChIKey', 'InChI'])
         df.dropna(inplace=True)
         df.sort_values('InChIKey', inplace=True)
-        df[['InChIKey', 'source_id', 'SMILES','InChI']].to_csv(filename, index=False)
-
+        df[['InChIKey', 'source_id', 'SMILES', 'InChI']].to_csv(
+            filename, index=False)
 
     @staticmethod
     def from_csv(filename):
         """Add entries from CSV file.
 
         Args:
             filename(str): Path to a CSV file.
         """
         import pandas as pd
         df = pd.read_csv(filename)
         # The boolean columns must be changed to boolean values otherwise
         # SQLalchmy passes strings
         df.universe = df.universe.apply(lambda x: False if x == 'f' else True)
-        df.essential = df.essential.apply(lambda x: False if x == 'f' else True)
+        df.essential = df.essential.apply(
+            lambda x: False if x == 'f' else True)
 
         # check columns
         needed_cols = Molrepo._table_attributes()
         if needed_cols != list(df.columns):
             raise Exception("Input missing columns: %s", ' '.join(needed_cols))
         # add them
         for row_nr, row in df.iterrows():
@@ -242,16 +244,18 @@
                 else:
                     query_fields.append("MolrepoHasMolecule." + field)
 
         if len(query_fields) == 0:
             return None
 
         session = get_session()
-        query = session.query(MolrepoHasMolecule).outerjoin(Molecule, Molecule.inchikey == MolrepoHasMolecule.inchikey).filter(
-            MolrepoHasMolecule.molrepo_name == molrepo_name, MolrepoHasMolecule.inchikey.isnot(None))
+        query = session.query(MolrepoHasMolecule).outerjoin(
+            Molecule, Molecule.inchikey == MolrepoHasMolecule.inchikey).filter(
+            MolrepoHasMolecule.molrepo_name ==
+            molrepo_name, MolrepoHasMolecule.inchikey.isnot(None))
         res = query.with_entities(*[eval(f) for f in query_fields]).all()
 
         session.close()
         return res
 
     @staticmethod
     def count(molrepo_name=None):
@@ -292,30 +296,35 @@
         molrepo_parser = molrepo_name
 
         # parser_fn yield a list of dictionaries with keys as a molrepo entry
         parse_fn = Parser.parse_fn(molrepo_parser)
         # profile time
         t_start = time()
         engine = get_engine()
-        for chunk in parse_fn(map_files, molrepo_name, 1000):
-            if len(chunk) == 0:
-                continue
-            chunk_inchi = []
-            chunk_molrepo = []
-            for data in chunk:
-                if data["inchikey"] is not None:
-                    chunk_inchi.append(
-                        {"inchikey": data["inchikey"], "inchi": data["inchi"]})
-                del data["inchi"]
-                chunk_molrepo.append(data)
-            if len(chunk_inchi) > 0:
-                engine.execute(postgresql.insert(Molecule.__table__).values(
-                    chunk_inchi).on_conflict_do_nothing(index_elements=[Molecule.inchikey]))
-            engine.execute(postgresql.insert(MolrepoHasMolecule.__table__).values(
-                chunk_molrepo).on_conflict_do_nothing(index_elements=[MolrepoHasMolecule.id]))
+        with engine.begin() as conn:
+            for chunk in parse_fn(map_files, molrepo_name, 1000):
+                if len(chunk) == 0:
+                    continue
+                chunk_inchi = []
+                chunk_molrepo = []
+                for data in chunk:
+                    if data["inchikey"] is not None:
+                        chunk_inchi.append({"inchikey": data["inchikey"],
+                                            "inchi": data["inchi"]})
+                    del data["inchi"]
+                    chunk_molrepo.append(data)
+                if len(chunk_inchi) > 0:
+                    conn.execute(postgresql.insert(
+                        Molecule.__table__).values(
+                        chunk_inchi).on_conflict_do_nothing(
+                        index_elements=[Molecule.inchikey]))
+                conn.execute(postgresql.insert(
+                    MolrepoHasMolecule.__table__).values(
+                    chunk_molrepo).on_conflict_do_nothing(
+                    index_elements=[MolrepoHasMolecule.id]))
         t_end = time()
         t_delta = str(datetime.timedelta(seconds=t_end - t_start))
         Molrepo.__log.info(
             "Importing Molrepo Name %s took %s", molrepo_name, t_delta)
 
     @staticmethod
     def molrepo_hpc(tmpdir, only_essential=False, **kwargs):
@@ -349,15 +358,15 @@
         with open(script_name, 'w') as fh:
             for line in script_lines:
                 fh.write(line + '\n')
         # hpc parameters
         molrepos_names = set()
         molrepos = Molrepo.get()
         for molrepo in molrepos:
-            if only_essential and not molrepo.essential: 
+            if only_essential and not molrepo.essential:
                 continue
             molrepos_names.add(molrepo.molrepo_name)
 
         params = {}
         params["num_jobs"] = len(molrepos_names)
         params["jobdir"] = job_path
         params["job_name"] = "CC_MOLREPO"
@@ -417,15 +426,16 @@
     def _drop_table():
         engine = get_engine()
         MolrepoHasMolecule.__table__.drop(engine)
 
     @staticmethod
     def _table_exists():
         engine = get_engine()
-        return sqlalchemy.inspect(engine).has_table(MolrepoHasMolecule.__tablename__)
+        return sqlalchemy.inspect(engine).has_table(
+            MolrepoHasMolecule.__tablename__)
 
     @staticmethod
     def _table_attributes():
         attrs = [a for a in class_mapper(
             MolrepoHasMolecule).iterate_properties]
         col_attrs = [a.key for a in attrs if isinstance(a, ColumnProperty)]
         input_attrs = [a for a in col_attrs if a != 'id']
@@ -449,18 +459,18 @@
 class MolrepoHasDatasource(Base):
     """Molrepo-Datasource relationship.
 
     Many-to-Many relationship.
     """
 
     __tablename__ = 'molrepo_has_datasource'
-    molrepo_name = Column(Text,
-                          ForeignKey("molrepo.molrepo_name"), primary_key=True)
-    datasource_name = Column(Text,
-                             ForeignKey("datasource.datasource_name"), primary_key=True)
+    molrepo_name = Column(Text, ForeignKey("molrepo.molrepo_name"),
+                          primary_key=True)
+    datasource_name = Column(Text, ForeignKey("datasource.datasource_name"),
+                             primary_key=True)
 
     def __repr__(self):
         """String representation."""
         return self.molrepo_name + " maps to " + self.datasource_name
 
     @staticmethod
     def _create_table():
@@ -472,15 +482,16 @@
     def _drop_table():
         engine = get_engine()
         MolrepoHasDatasource.__table__.drop(engine)
 
     @staticmethod
     def _table_exists():
         engine = get_engine()
-        return sqlalchemy.inspect(engine).has_table(MolrepoHasDatasource.__tablename__)
+        return sqlalchemy.inspect(engine).has_table(
+            MolrepoHasDatasource.__tablename__)
 
     @staticmethod
     def _table_attributes():
         attrs = [a for a in class_mapper(
             MolrepoHasDatasource).iterate_properties]
         col_attrs = [a.key for a in attrs if isinstance(a, ColumnProperty)]
         input_attrs = [a for a in col_attrs if a != 'id']
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/database/pubchem.py` & `chemicalchecker-1.0.3/chemicalchecker/database/pubchem.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,25 +44,27 @@
 
         Args:
             data(list): The data in list format. Each list member is a new row.
                 The order is important.
             chunk(int): The size of the chunks to load data to the database.
         """
         engine = get_engine()
-        for pos in range(0, len(data), chunk):
-
-            engine.execute(
-                Pubchem.__table__.insert(),
-                [{"cid": row[0], "inchikey_pubchem": row[1], "inchikey": row[2], "name": row[3],
-                  "synonyms": row[4]}
-                    for row in data[pos:pos + chunk]]
-            )
+        with engine.begin() as conn:
+            for pos in range(0, len(data), chunk):
+                conn.execute(
+                    Pubchem.__table__.insert(),
+                    [{"cid": row[0], "inchikey_pubchem": row[1],
+                      "inchikey": row[2], "name": row[3],
+                      "synonyms": row[4]}
+                        for row in data[pos:pos + chunk]]
+                )
 
     @staticmethod
-    def get(cid=None, inchikey_pubchem=None, inchikey=None, name=None, synonyms=None):
+    def get(cid=None, inchikey_pubchem=None, inchikey=None, name=None,
+            synonyms=None):
         """Method to query table.
 
         Args:
             cid(int): The cid that want to find
             inchikey_pubchem(str): The inchikey_pubchem to query
             inchikey(str): The inchikey to query
         """
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/database/uniprotkb.py` & `chemicalchecker-1.0.3/chemicalchecker/database/uniprotkb.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/adanet/adanet_wrap.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/adanet/adanet_wrap.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/adanet/cnn_generator.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/adanet/cnn_generator.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/adanet/dnn_extend_generator.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/adanet/dnn_extend_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import adanet
 # import tensorflow as tf
 # from tensorflow.keras import layers
 # from tensorflow.keras.layers import Dense, Dropout
 import numpy as np
 import tensorflow.compat.v1 as tf
 from tensorflow.compat.v1 import layers
-from tensorflow.compat.v1.layers import Dense, Dropout
+#from tensorflow.compat.v1.layers import Dense, Dropout
 from chemicalchecker.util import logged
 
 
 class NanMaskingLayer(layers.Layer):
 
     def __init__(self, mask_value=0.0):
         super(NanMaskingLayer, self).__init__()
@@ -71,21 +71,21 @@
         input_layer = tf.cast(features['x'], tf.float32)
         # forcing to input shape as dataset uses tf.py_func (loosing shape)
         input_layer = tf.reshape(features['x'], [-1, self._input_shape])
         last_layer = input_layer
         if self._nan_mask_value is not None:
             last_layer = NanMaskingLayer(self._nan_mask_value)(last_layer)
         for layer_size in self._layer_sizes:
-            last_layer = Dense(
+            last_layer = layers.Dense(
                 layer_size * self._layer_block_size,
                 activation=self._activation)(last_layer)
-            last_layer = Dropout(
+            last_layer = layers.Dropout(
                 rate=self._dropout,
                 seed=self._seed)(last_layer, training=training)(last_layer)
-        logits = Dense(logits_dimension)(last_layer)
+        logits = layers.Dense(logits_dimension)(last_layer)
 
         shared_tensors = {
             "num_layers": tf.constant(self._num_layers),
             "layer_sizes": tf.constant(self._layer_sizes),
         }
         return adanet.Subnetwork(
             last_layer=last_layer,
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/adanet/dnn_stack_generator.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/adanet/dnn_stack_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import adanet
 import numpy as np
 import tensorflow.compat.v1 as tf
 from tensorflow.compat.v1 import layers
-from tensorflow.compat.v1.layers import Dense, Dropout
+#from tensorflow.compat.v1.layers import Dense, Dropout
 # import tensorflow as tf
 # from tensorflow.keras import layers
 # from tensorflow.keras.layers import Dense, Dropout
 from chemicalchecker.util import logged
 
 
 class NanMaskingLayer(layers.Layer):
@@ -71,22 +71,22 @@
         input_layer = tf.cast(features['x'], tf.float32)
         # forcing to input shape as dataset uses tf.py_func (loosing shape)
         input_layer = tf.reshape(features['x'], [-1, self._input_shape])
         last_layer = input_layer
         if self._nan_mask_value is not None:
             last_layer = NanMaskingLayer(self._nan_mask_value)(last_layer)
         for _ in range(self._num_layers):
-            last_layer = Dense(
+            last_layer = layers.Dense(
                 self._layer_size,
                 activation=self._activation)(last_layer)
-            last_layer = Dropout(
+            last_layer = layers.Dropout(
                 rate=self._dropout,
                 seed=self._seed)(last_layer, training=training)
 
-        logits = Dense(units=logits_dimension)(last_layer)
+        logits = layers.Dense(units=logits_dimension)(last_layer)
 
         persisted_tensors = {"num_layers": tf.constant(self._num_layers)}
         return adanet.Subnetwork(
             last_layer=last_layer,
             logits=logits,
             complexity=self._measure_complexity(),
             persisted_tensors=persisted_tensors)
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/autoencoder/autoencoder.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/autoencoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/autoencoder/autoencoder_siamese.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/autoencoder/autoencoder_siamese.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/classifier/imbalanced/imbalanced.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/classifier/imbalanced/imbalanced.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/classifier/multitask/binarymultitask.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/classifier/multitask/binarymultitask.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/feat/base_classes.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/feat/graph_features.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/deepchem/feat/mol_graphs.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/graphconv/graph_smiles_sign.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/graphconv/graph_smiles_sign.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/hotnet/hotnet.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/hotnet/hotnet.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/node2vec/node2vec.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/node2vec/node2vec.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/node2vec/word2vec.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/node2vec/word2vec.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/siamese/callbacks.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/siamese/callbacks.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/siamese/siamese.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/siamese/siamese.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from tensorflow import keras
 from tensorflow.keras import backend as K
 from tensorflow.keras.models import Model, Sequential
 from tensorflow.keras.callbacks import EarlyStopping, Callback
 from tensorflow.keras.layers import Input, Dropout, Lambda, Dense
 
 from chemicalchecker.util import logged
-from chemicalchecker.util.splitter import NeighborPairTraintest
+#from chemicalchecker.util.splitter import NeighborPairTraintest
 
 
 @logged
 class Siamese(object):
     """Siamese class.
 
     This class implements a simple siamese neural network based on Keras that
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/siamese/siamese_triplets.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/siamese/siamese_triplets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
 import pickle
 import numpy as np
 from time import time
 from functools import partial
 
+import tensorflow as tf
 from tensorflow import keras
 from tensorflow.keras import backend as K
 from tensorflow.keras.layers import concatenate
 from tensorflow.keras.models import Model, Sequential
 from tensorflow.keras.callbacks import EarlyStopping, Callback
 from tensorflow.keras.layers import Input, Dropout, Lambda, Dense
 from tensorflow.keras.layers import Activation, Masking, BatchNormalization
 from tensorflow.keras.layers import GaussianNoise, AlphaDropout, GaussianDropout
 from tensorflow.keras import regularizers
 
 from chemicalchecker.util import logged
-from chemicalchecker.util.splitter import NeighborTripletTraintest
+from chemicalchecker.util.splitter import TripletIterator
 from .callbacks import CyclicLR, LearningRateFinder
 
 MIN_LR = 1e-8
 MAX_LR = 1e-1
 
 
 class AlphaDropoutCP(keras.layers.AlphaDropout):
@@ -105,20 +106,20 @@
                 self.layers.append(l)
         self.activations = kwargs.get("activations",
                                       ['relu'])
         self.dropouts = kwargs.get(
             "dropouts", [None])
         self.augment_fn = kwargs.get("augment_fn", None)
         self.augment_kwargs = kwargs.get("augment_kwargs", {})
-        self.loss_func = str(kwargs.get("loss_func", 'orthogonal_tloss'))
+        self.loss_func = str(kwargs.get("loss_func", 'only_self_loss'))
         self.margin = float(kwargs.get("margin", 1.0))
         self.alpha = float(kwargs.get("alpha", 1.0))
         self.patience = float(kwargs.get("patience", self.epochs))
         self.traintest_file = kwargs.get("traintest_file", None)
-        self.standard = kwargs.get("standard", True)
+        self.onlyself_notself = kwargs.get("onlyself_notself", False)
         self.trim_mask = kwargs.get("trim_mask", None)
         self.steps_per_epoch = kwargs.get("steps_per_epoch", None)
         self.validation_steps = kwargs.get("validation_steps", None)
 
         # internal variables
         self.name = self.__class__.__name__.lower()
         self.time = 0
@@ -147,37 +148,37 @@
                 if generator is None:
                     if self.sharedx is None:
                         self.__log.info("Reading sign2 universe lookup,"
                                         " this should only be loaded once.")
                         self.sharedx = traintest_data.get_h5_dataset('x')
                         full_trim = np.argwhere(np.repeat(self.trim_mask, 128))
                         self.sharedx_trim = self.sharedx[:, full_trim.ravel()]
-                    tr_shape_type_gen = NeighborTripletTraintest.generator_fn(
+                    tr_shape_type_gen = TripletIterator.generator_fn(
                         self.traintest_file,
                         'train_train',
-                        epochs=self.epochs,
                         batch_size=self.batch_size,
                         replace_nan=self.replace_nan,
-                        sharedx=self.sharedx,
+                        train=True, 
                         augment_fn=self.augment_fn,
                         augment_kwargs=self.augment_kwargs,
-                        train=True, standard=self.standard,
                         trim_mask=self.trim_mask,
-                        sharedx_trim=self.sharedx_trim)
+                        sharedx=self.sharedx,
+                        sharedx_trim=self.sharedx_trim,
+                        onlyself_notself=self.onlyself_notself)
                 else:
                     tr_shape_type_gen = generator
                 self.generator = tr_shape_type_gen
                 self.tr_shapes = tr_shape_type_gen[0]
                 self.tr_gen = tr_shape_type_gen[2]()
                 if self.steps_per_epoch is None:
                     self.steps_per_epoch = np.ceil(
                         self.tr_shapes[0][0] / self.batch_size)
 
             # load the scaler
-            if not self.standard:
+            if self.onlyself_notself:
                 scaler_path = os.path.join(self.model_dir, 'scaler.pkl')
                 if os.path.isfile(scaler_path):
                     self.scaler = pickle.load(open(scaler_path, 'rb'))
                     self.__log.info("Using scaler: %s", scaler_path)
                 elif 'scaler' in traintest_data.info_h5:
                     scaler_path_tt = traintest_data.get_h5_dataset('scaler')[0]
                     self.__log.info("Using scaler: %s", scaler_path_tt)
@@ -191,27 +192,27 @@
             traintest_data = DataSignature(self.traintest_file)
             if self.sharedx is None:
                 self.__log.info("Reading sign2 universe lookup,"
                                 " this should only be loaded once.")
                 self.sharedx = traintest_data.get_h5_dataset('x')
                 full_trim = np.argwhere(np.repeat(self.trim_mask, 128))
                 self.sharedx_trim = self.sharedx[:, full_trim.ravel()]
-            val_shape_type_gen = NeighborTripletTraintest.generator_fn(
+            val_shape_type_gen = TripletIterator.generator_fn(
                 self.traintest_file,
                 'test_test',
                 batch_size=self.batch_size,
+                shuffle=False,
+                train=False,
                 replace_nan=self.replace_nan,
                 augment_kwargs=self.augment_kwargs,
                 augment_fn=self.augment_fn,
-                sharedx=self.sharedx,
-                train=False,
-                shuffle=False,
-                standard=self.standard, 
                 trim_mask=self.trim_mask,
-                sharedx_trim=self.sharedx_trim)
+                sharedx=self.sharedx,
+                sharedx_trim=self.sharedx_trim,
+                onlyself_notself=self.onlyself_notself)
             self.val_shapes = val_shape_type_gen[0]
             self.val_gen = val_shape_type_gen[2]()
             if self.validation_steps is None:
                 self.validation_steps = np.ceil(
                     self.val_shapes[0][0] / self.batch_size)
         else:
             self.val_shapes = None
@@ -220,24 +221,22 @@
 
         # log parameters
         self.__log.info("**** %s Parameters: ***" % self.__class__.__name__)
         self.__log.info("{:<22}: {:>12}".format("model_dir", self.model_dir))
         if self.traintest_file is not None and not predict_only:
             self.__log.info("{:<22}: {:>12}".format(
                 "traintest_file", self.traintest_file))
-            tmp = NeighborTripletTraintest(self.traintest_file, 'train_train')
+            tmp = TripletIterator(self.traintest_file, 'train_train')
             self.__log.info("{:<22}: {:>12}".format(
                 'train_train', str(tmp.get_ty_shapes())))
             if evaluate:
-                tmp = NeighborTripletTraintest(
-                    self.traintest_file, 'train_test')
+                tmp = TripletIterator(self.traintest_file, 'train_test')
                 self.__log.info("{:<22}: {:>12}".format(
                     'train_test', str(tmp.get_ty_shapes())))
-                tmp = NeighborTripletTraintest(
-                    self.traintest_file, 'test_test')
+                tmp = TripletIterator(self.traintest_file, 'test_test')
                 self.__log.info("{:<22}: {:>12}".format(
                     'test_test', str(tmp.get_ty_shapes())))
         self.__log.info("{:<22}: {:>12}".format(
             "learning_rate", self.learning_rate))
         self.__log.info("{:<22}: {:>12}".format(
             "epochs", self.epochs))
         self.__log.info("{:<22}: {:>12}".format(
@@ -252,14 +251,19 @@
             "dropouts", str(self.dropouts)))
         self.__log.info("{:<22}: {:>12}".format(
             "augment_fn", str(self.augment_fn)))
         self.__log.info("{:<22}: {:>12}".format(
             "augment_kwargs", str(self.augment_kwargs)))
         self.__log.info("**** %s Parameters: ***" % self.__class__.__name__)
 
+        if not os.path.isfile(param_file) and save_params:
+            self.__log.debug("Saving temporary parameters to %s" % param_file)
+            with open(param_file+'.tmp', "wb") as f:
+                pickle.dump(kwargs, f, protocol=pickle.HIGHEST_PROTOCOL)
+
         if self.learning_rate == 'auto':
             self.__log.debug("Searching for optimal learning rates.")
             lr = self.find_lr(kwargs, generator=self.generator)
             self.learning_rate = lr
             kwargs['learning_rate'] = self.learning_rate
 
         if not os.path.isfile(param_file) and save_params:
@@ -313,15 +317,15 @@
                 else:
                     net.add(Dropout(dropout))
 
         # we have two inputs
         input_a = Input(shape=input_shape)
         input_p = Input(shape=input_shape)
         input_n = Input(shape=input_shape)
-        if not self.standard:
+        if self.onlyself_notself:
             input_o = Input(shape=input_shape)
             input_s = Input(shape=input_shape)
 
         # Update layers
         if self.layers_sizes == None:
             self.layers_sizes = get_model_arch(
                 input_shape[0], num_layers=len(self.layers))
@@ -337,94 +341,77 @@
             if i == 0:
                 i_shape = input_shape
             if i == (len(self.layers) - 1):
                 dropout = None
             add_layer(basenet, layer, layer_size, activation,
                       dropout, input_shape=i_shape)
 
-        # first layer
-        """add_layer(basenet, self.layers[0], self.layers_sizes[0],
-                  self.activations[0], self.dropouts[0],
-                  input_shape=input_shape)
-        hidden_layers = zip(self.layers[1:-1],
-                            self.layers_sizes[1:-1],
-                            self.activations[1:-1],
-                            self.dropouts[1:-1])
-        for layer, layer_size, activation, dropout in hidden_layers:
-            add_layer(basenet, layer, layer_size, activation, dropout)
-        add_layer(basenet, self.layers[-1], self.layers_sizes[-1],
-                  self.activations[-1], None)"""
         # last normalization layer for loss
         basenet.add(Lambda(lambda x: K.l2_normalize(x, axis=-1)))
         basenet.summary()
 
         encodeds = list()
         encodeds.append(basenet(input_a))
         encodeds.append(basenet(input_p))
         encodeds.append(basenet(input_n))
-        if not self.standard:
+        if self.onlyself_notself:
             encodeds.append(basenet(input_o))
             encodeds.append(basenet(input_s))
         merged_vector = concatenate(encodeds, axis=-1, name='merged_layer')
 
         inputs = [input_a, input_p, input_n]
-        if not self.standard:
+        if self.onlyself_notself:
             inputs.extend([input_o, input_s])
         model = Model(inputs=inputs, outputs=merged_vector)
 
-        # TODO NEED TO CHANGE IF WE USE 4 INPUTS INSTEAD OF 3
-        if self.standard:
+        def split_array(array, sections):
+            length = array.shape.as_list()[-1]
+            splitted = list()
+            for i in range(sections):
+                start = int(length * i / sections)
+                end = int(length * (i+1) / sections)
+                splitted.append(array[:, start:end])
+            return splitted
+
+        if self.onlyself_notself:
             def split_output(y_pred):
-                total_lenght = y_pred.shape.as_list()[-1]
-                anchor = y_pred[:, 0: int(total_lenght * 1 / 3)]
-                positive = y_pred[
-                    :, int(total_lenght * 1 / 3): int(total_lenght * 2 / 3)]
-                negative = y_pred[
-                    :, int(total_lenght * 2 / 3): int(total_lenght * 3 / 3)]
-                return anchor, positive, negative, None, None
+                anchor, positive, negative, only, n_self = split_array(y_pred, 5)
+                return anchor, positive, negative, only, n_self
         else:
             def split_output(y_pred):
-                total_lenght = y_pred.shape.as_list()[-1]
-                anchor = y_pred[:, 0: int(total_lenght * 1 / 5)]
-                positive = y_pred[
-                    :, int(total_lenght * 1 / 5): int(total_lenght * 2 / 5)]
-                negative = y_pred[
-                    :, int(total_lenght * 2 / 5): int(total_lenght * 3 / 5)]
-                only = y_pred[
-                    :, int(total_lenght * 3 / 5): int(total_lenght * 4 / 5)]
-                n_self = y_pred[
-                    :, int(total_lenght * 4 / 5): int(total_lenght * 5 / 5)]
+                anchor, positive, negative, = split_array(y_pred, 3)
+                only, n_self = None, None
                 return anchor, positive, negative, only, n_self
 
         # define monitored metrics
         def accTot(y_true, y_pred):
             anchor, positive, negative, _, _ = split_output(y_pred)
             acc = K.cast(euclidean_distance(anchor, positive) <
                          euclidean_distance(anchor, negative), anchor.dtype)
             return K.mean(acc)
 
-        def accE(y_true, y_pred):
+        def AccEasy(y_true, y_pred):
             anchor, positive, negative, _, _ = split_output(y_pred)
             msk = K.cast(K.equal(y_true, 0), 'float32')
             prd = self.batch_size / K.sum(msk)
             acc = K.cast(
                 euclidean_distance(anchor * msk, positive * msk) <
                 euclidean_distance(anchor * msk, negative * msk), anchor.dtype)
             return K.mean(acc) * prd
 
-        def accM(y_true, y_pred):
+        def AccMed(y_true, y_pred):
             anchor, positive, negative, _, _ = split_output(y_pred)
             msk = K.cast(K.equal(y_true, 1), 'float32')
             prd = self.batch_size / K.sum(msk)
             acc = K.cast(
                 euclidean_distance(anchor * msk, positive * msk) <
                 euclidean_distance(anchor * msk, negative * msk), anchor.dtype)
             return K.mean(acc) * prd
 
-        def accH(y_true, y_pred):
+        def AccHard(y_true, y_pred):
             anchor, positive, negative, _, _ = split_output(y_pred)
             msk = K.cast(K.equal(y_true, 2), 'float32')
             prd = self.batch_size / K.sum(msk)
             acc = K.cast(
                 euclidean_distance(anchor * msk, positive * msk) <
                 euclidean_distance(anchor * msk, negative * msk), anchor.dtype)
             return K.mean(acc) * prd
@@ -438,37 +425,37 @@
             r_num = K.sum(xm * ym)
             x_square_sum = K.sum(xm * xm)
             y_square_sum = K.sum(ym * ym)
             r_den = K.sqrt(x_square_sum * y_square_sum)
             r = r_num / r_den
             return K.mean(r)
 
-        def cor1(y_true, y_pred):
+        def CorANotself(y_true, y_pred):
             anchor, positive, negative, only_self, not_self = split_output(
                 y_pred)
             return pearson_r(anchor, not_self)
 
-        def cor2(y_true, y_pred):
+        def CorAOnlyself(y_true, y_pred):
             anchor, positive, negative, only_self, not_self = split_output(
                 y_pred)
             return pearson_r(anchor, only_self)
 
-        def cor3(y_true, y_pred):
+        def CorNotselfOnlyself(y_true, y_pred):
             anchor, positive, negative, only_self, not_self = split_output(
                 y_pred)
             return pearson_r(not_self, only_self)
 
         metrics = [accTot]
-        if not self.standard:
-            metrics.extend([accE,
-                            accM,
-                            accH,
-                            cor1,
-                            cor2,
-                            cor3])
+        if self.onlyself_notself:
+            metrics.extend([AccEasy,
+                            AccMed,
+                            AccHard,
+                            CorANotself,
+                            CorAOnlyself,
+                            CorNotselfOnlyself])
 
         def tloss(y_true, y_pred):
             anchor, positive, negative, _, _ = split_output(y_pred)
             pos_dist = K.sum(K.square(anchor - positive), axis=1)
             neg_dist = K.sum(K.square(anchor - negative), axis=1)
             basic_loss = pos_dist - neg_dist + self.margin
             loss = K.maximum(basic_loss, 0.0)
@@ -746,27 +733,27 @@
                     'ALL': None
                 }
             validation_sets = list()
 
             for split in vsets:
                 for set_name, mask_fn in mask_fns.items():
                     name = '_'.join([split, set_name])
-                    shapes, dtypes, gen = NeighborTripletTraintest.generator_fn(
+                    shapes, dtypes, gen = TripletIterator.generator_fn(
                         self.traintest_file, split,
                         batch_size=self.batch_size,
+                        shuffle=False,
                         replace_nan=self.replace_nan,
-                        mask_fn=mask_fn,
-                        sharedx=self.sharedx,
+                        train=False,
                         augment_kwargs=self.augment_kwargs,
                         augment_fn=self.augment_fn,
-                        train=False,
-                        shuffle=False,
-                        standard=self.standard,
+                        mask_fn=mask_fn,
                         trim_mask=self.trim_mask,
-                        sharedx_trim=self.sharedx_trim)
+                        sharedx=self.sharedx,
+                        sharedx_trim=self.sharedx_trim,
+                        onlyself_notself=self.onlyself_notself)
                     validation_sets.append((gen, shapes, name))
             additional_vals = AdditionalValidationSets(
                 validation_sets, self.model, batch_size=self.batch_size,
                 validation_steps=self.validation_steps)
             callbacks.append(additional_vals)
 
         class CustomEarlyStopping(EarlyStopping):
@@ -873,15 +860,15 @@
         history_file = os.path.join(
             self.model_dir, "%s_history.pkl" % self.name)
         pickle.dump(self.history.history, open(history_file, 'wb'),protocol=pickle.HIGHEST_PROTOCOL)
         history_file = os.path.join(self.model_dir, "history.png")
         anchor_file = os.path.join(self.model_dir, "anchor_distr.png")
         if self.evaluate and self.plot:
             self._plot_history(self.history.history, vsets, history_file)
-        if not self.standard and self.plot:
+        if self.onlyself_notself and self.plot:
             self._plot_anchor_dist(anchor_file)
 
     def predict(self, x_matrix, dropout_fn=None, dropout_samples=10, cp=False):
         """Do predictions.
 
         prediction_file(str): Path to input file containing Xs.
         split(str): which split to predict.
@@ -960,53 +947,53 @@
         import matplotlib.pyplot as plt
         import seaborn as sns
 
         def sim(a, b):
             return -(cosine(a, b) - 1)
 
         # Need to create a new train_train generator without train=False
-        tr_shape_type_gen = NeighborTripletTraintest.generator_fn(
+        tr_shape_type_gen = TripletIterator.generator_fn(
             self.traintest_file,
             'train_train',
             batch_size=self.batch_size,
+            shuffle=False,
             replace_nan=self.replace_nan,
-            sharedx=self.sharedx,
+            train=False,
             augment_fn=self.augment_fn,
             augment_kwargs=self.augment_kwargs,
-            train=False,
-            shuffle=False,
-            standard=self.standard)
+            sharedx=self.sharedx,
+            onlyself_notself=self.onlyself_notself)
 
         tr_gen = tr_shape_type_gen[2]()
 
         if self.evaluate:
-            trval_shape_type_gen = NeighborTripletTraintest.generator_fn(
+            trval_shape_type_gen = TripletIterator.generator_fn(
                 self.traintest_file,
                 'train_test',
                 batch_size=self.batch_size,
+                shuffle=False,
                 replace_nan=self.replace_nan,
-                sharedx=self.sharedx,
+                train=False,
                 augment_fn=self.augment_fn,
                 augment_kwargs=self.augment_kwargs,
-                train=False,
-                shuffle=False,
-                standard=self.standard)
+                sharedx=self.sharedx,
+                onlyself_notself=self.onlyself_notself)
             trval_gen = trval_shape_type_gen[2]()
 
-            val_shape_type_gen = NeighborTripletTraintest.generator_fn(
+            val_shape_type_gen = TripletIterator.generator_fn(
                 self.traintest_file,
                 'test_test',
                 batch_size=self.batch_size,
+                shuffle=False,
                 replace_nan=self.replace_nan,
-                sharedx=self.sharedx,
+                train=False,
                 augment_fn=self.augment_fn,
                 augment_kwargs=self.augment_kwargs,
-                train=False,
-                shuffle=False,
-                standard=self.standard)
+                sharedx=self.sharedx,
+                onlyself_notself=self.onlyself_notself)
             val_gen = val_shape_type_gen[2]()
 
             vset_dict = {'train_train': tr_gen,
                          'train_test': trval_gen, 'test_test': val_gen}
         else:
             vset_dict = {'train_train': tr_gen}
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/smilespred/smilespred.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/smilespred/smilespred.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,160 @@
 import os
-import faiss
 import pickle
 import numpy as np
 import pandas as pd
+from time import time
 from tqdm import tqdm
+from functools import partial
 
+import tensorflow as tf
+from tensorflow import keras
 from tensorflow.keras import backend as K
-from tensorflow.keras.models import Sequential
-from tensorflow.keras.layers import Dropout, Lambda, Dense, Activation
+from tensorflow.keras.layers import concatenate
+from tensorflow.keras.models import Model, Sequential
+from tensorflow.keras.callbacks import EarlyStopping, Callback
+from tensorflow.keras.layers import Input, Dropout, Lambda, Dense
+from tensorflow.keras.layers import Activation, Masking, BatchNormalization
+from tensorflow.keras.layers import GaussianNoise, GaussianDropout
+from tensorflow.keras.layers import AlphaDropout
+from tensorflow.keras import regularizers
 
 from MulticoreTSNE import MulticoreTSNE
 from scipy.spatial.distance import cosine
 
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 from chemicalchecker.util import logged
 
 
 @logged
 class Smilespred(object):
 
-    def __init__(self, model_dir, sign0=[], sign3=[], evaluate=False):
+    def __init__(self, model_dir, sign0=[], sign3=[], evaluate=False,
+                 save_params=True, **kwargs):
         self.sign0 = sign0
         self.sign3 = sign3[:]
         self.name = self.__class__.__name__.lower()
         self.model_dir = os.path.abspath(model_dir)
         self.model_file = os.path.join(self.model_dir, "%s.h5" % self.name)
         if evaluate:
             self.e_split = 0.2
             self.t_split = 1 - self.e_split
         else:
             self.e_split = 0
             self.t_split = 1
         self.model = None
 
+        # check if parameter file exists
+        param_file = os.path.join(model_dir, 'params.pkl')
+        if os.path.isfile(param_file):
+            with open(param_file, 'rb') as h:
+                kwargs = pickle.load(h)
+            self.__log.info('Parameters loaded from: %s' % param_file)
+        self.epochs = int(kwargs.get("epochs", 10))
+        self.learning_rate = kwargs.get("learning_rate", 1e-3)
+        self.layers_sizes = kwargs.get("layers_sizes", [1024, 512, 256, 128])
+        self.layers = list()
+        # we can pass layers type as strings
+        layers = kwargs.get("layers", ['Dense', 'Dense', 'Dense', 'Dense'])
+        for l in layers:
+            if isinstance(l, str):
+                self.layers.append(eval(l))
+            else:
+                self.layers.append(l)
+        self.activations = kwargs.get(
+            "activations", ['relu', 'relu', 'relu', 'tanh'])
+        self.dropouts = kwargs.get("dropouts", [0.1, 0.1, 0.1, None])
+
+        # save params
+        if not os.path.isfile(param_file) and save_params:
+            self.__log.debug("Saving parameters to %s" % param_file)
+            with open(param_file, "wb") as f:
+                pickle.dump(kwargs, f, protocol=pickle.HIGHEST_PROTOCOL)
+
     def build_model(self, load=False):
         def corr(y_true, y_pred):
             x = y_true
             y = y_pred
             mx = K.mean(x, axis=0)
             my = K.mean(y, axis=0)
             xm, ym = x - mx, y - my
             r_num = K.sum(xm * ym)
             x_square_sum = K.sum(xm * xm)
             y_square_sum = K.sum(ym * ym)
             r_den = K.sqrt(x_square_sum * y_square_sum)
             r = r_num / r_den
             return K.mean(r)
 
+        def add_layer(net, layer, layer_size, activation, dropout,
+                      use_bias=True, input_shape=False):
+            if input_shape is not None:
+                if activation == 'selu':
+                    net.add(GaussianDropout(rate=0.1, input_shape=input_shape))
+                    net.add(layer(layer_size, use_bias=use_bias,
+                                  kernel_initializer='lecun_normal'))
+                else:
+                    net.add(layer(layer_size, use_bias=use_bias,
+                                  input_shape=input_shape))
+            else:
+                if activation == 'selu':
+                    net.add(layer(layer_size, use_bias=use_bias,
+                                  kernel_initializer='lecun_normal'))
+                else:
+                    net.add(layer(layer_size, use_bias=use_bias))
+            net.add(Activation(activation))
+            if dropout is not None:
+                net.add(Dropout(dropout))
+
+        def get_model_arch(input_dim, space_dim=128, num_layers=3):
+            if input_dim >= space_dim * (2**num_layers):
+                layers = [int(space_dim * 2**i)
+                          for i in reversed(range(num_layers))]
+            else:
+                layers = [max(128, int(input_dim / 2**i))
+                          for i in range(1, num_layers + 1)]
+            return layers
+
+        # Update layers
+        if self.layers_sizes == None:
+            self.layers_sizes = get_model_arch(
+                2048, num_layers=len(self.layers))
+
+        # each goes to a network with the same architechture
+        assert(len(self.layers) == len(self.layers_sizes) ==
+               len(self.activations) == len(self.dropouts))
         model = Sequential()
-        drop = 0.1
-        model.add(Dense(1024, input_dim=2048))
-        model.add(Dropout(drop))
-        model.add(Activation('relu'))
-
-        model.add(Dense(512))
-        model.add(Dropout(drop))
-        model.add(Activation('relu'))
-
-        model.add(Dense(256))
-        model.add(Dropout(drop))
-        model.add(Activation('relu'))
+        for i, tple in enumerate(zip(self.layers, self.layers_sizes,
+                                     self.activations, self.dropouts)):
+            layer, layer_size, activation, dropout = tple
+            i_shape = None
+            if i == 0:
+                i_shape = (2048,)
+            if i == (len(self.layers) - 1):
+                dropout = None
+            add_layer(model, layer, layer_size, activation,
+                      dropout, input_shape=i_shape)
 
-        model.add(Dense(128))
-        model.add(Activation('tanh'))
+        # last normalization layer for loss
         model.add(Lambda(lambda x: K.l2_normalize(x, axis=-1)))
 
-        model.compile(loss='mse', optimizer='adam', metrics=[corr])
+        opt = keras.optimizers.Adam(learning_rate=self.learning_rate)
+        model.compile(loss='mse', optimizer=opt, metrics=[corr])
         if load:
             model.load_weights(self.model_file)
         else:
             model.summary()
         self.model = model
 
     def fit(self, save=True):
         self.build_model()
-        self.history = self.model.fit(x=self.sign0, y=self.sign3, epochs=30,
-                                      batch_size=128, validation_split=self.e_split, verbose=2)
+        self.history = self.model.fit(
+            x=self.sign0, y=self.sign3, epochs=self.epochs,
+            batch_size=128, validation_split=self.e_split, verbose=2)
         if save:
             self.model.save(self.model_file)
         history_file = os.path.join(
             self.model_dir, "%s_history.pkl" % self.name)
         pickle.dump(self.history.history, open(history_file, 'wb'))
         history_file = os.path.join(self.model_dir, "history.png")
         self._plot_history(history_file)
@@ -109,14 +182,15 @@
         axes[1].set_xlabel('Epochs', fontsize=15)
         axes[1].set_ylim(0.5, 1.0)
         fig.tight_layout()
         plt.savefig(h_file)
         plt.close('all')
 
     def evaluate(self):
+        import faiss
         def sim(a, b):
             return -(cosine(a, b) - 1)
         self.__log.info('Predicting all sign0')
         signp = self.model.predict(self.sign0)
 
         self.__log.info('VALIDATION: Plot distances.')
         subsample = min(int(len(self.sign0) * self.e_split), 100000)
@@ -145,38 +219,38 @@
             self.sign3[ts_idxs[:p]], self.sign3[ts_idxs[p:]])]
         ts_s_p = [sim(a, b)
                   for a, b in zip(signp[ts_idxs[:p]], signp[ts_idxs[p:]])]
         ts_dif = np.linalg.norm(self.sign3[ts_idxs] - signp[ts_idxs], axis=1)
 
         fig, axes = plt.subplots(2, 3, figsize=(15, 10), sharex='col')
         axes[0][0].set_title('Train Euclidean distances', fontsize=19)
-        sns.distplot(tr_e_o, label='original', ax=axes[0][0])
-        sns.distplot(tr_e_p, label='predicted', ax=axes[0][0])
+        sns.histplot(tr_e_o, label='original', ax=axes[0][0])
+        sns.histplot(tr_e_p, label='predicted', ax=axes[0][0])
         axes[0][0].legend(fontsize=15)
 
         axes[0][1].set_title('Train Cosine sims', fontsize=19)
-        sns.distplot(tr_s_o, label='original', ax=axes[0][1])
-        sns.distplot(tr_s_p, label='predicted', ax=axes[0][1])
+        sns.histplot(tr_s_o, label='original', ax=axes[0][1])
+        sns.histplot(tr_s_p, label='predicted', ax=axes[0][1])
         axes[0][1].legend(fontsize=15)
 
         axes[0][2].set_title('Train Distance original-predicted', fontsize=19)
-        sns.distplot(tr_dif, ax=axes[0][2])
+        sns.histplot(tr_dif, ax=axes[0][2])
 
         axes[1][0].set_title('Test Euclidean distances', fontsize=19)
-        sns.distplot(ts_e_o, label='original', ax=axes[1][0])
-        sns.distplot(ts_e_p, label='predicted', ax=axes[1][0])
+        sns.histplot(ts_e_o, label='original', ax=axes[1][0])
+        sns.histplot(ts_e_p, label='predicted', ax=axes[1][0])
         axes[1][0].legend(fontsize=15)
 
         axes[1][1].set_title('Test Cosine sims', fontsize=19)
-        sns.distplot(ts_s_o, label='original', ax=axes[1][1])
-        sns.distplot(ts_s_p, label='predicted', ax=axes[1][1])
+        sns.histplot(ts_s_o, label='original', ax=axes[1][1])
+        sns.histplot(ts_s_p, label='predicted', ax=axes[1][1])
         axes[1][1].legend(fontsize=15)
 
         axes[1][2].set_title('Test Distance original-predicted', fontsize=19)
-        sns.distplot(ts_dif, ax=axes[1][2])
+        sns.histplot(ts_dif, ax=axes[1][2])
 
         fname = 'distances.png'
         plot_file = os.path.join(self.model_dir, fname)
         plt.savefig(plot_file)
         plt.close()
 
         self.__log.info('VALIDATION: Plot projections.')
@@ -244,27 +318,27 @@
                 i_num = len(o_row & p_row)
                 tmp.append(i_num)
             shared_nn.append(tmp)
         shared_nn = np.array(shared_nn)
 
         fig, axes = plt.subplots(2, 2, figsize=(10, 10))
         axes[0][0].set_title('5 NN')
-        sns.distplot(shared_nn[:, 0], ax=axes[0][0])
+        sns.histplot(shared_nn[:, 0], ax=axes[0][0])
         axes[0][0].set_xlabel('Num overlap NN')
 
         axes[0][1].set_title('20 NN')
-        sns.distplot(shared_nn[:, 1], ax=axes[0][1], color='#ff7f0e')
+        sns.histplot(shared_nn[:, 1], ax=axes[0][1], color='#ff7f0e')
         axes[0][1].set_xlabel('Num overlap NN')
 
         axes[1][0].set_title('50 NN')
-        sns.distplot(shared_nn[:, 2], ax=axes[1][0], color='#2ca02c')
+        sns.histplot(shared_nn[:, 2], ax=axes[1][0], color='#2ca02c')
         axes[1][0].set_xlabel('Num overlap NN')
 
         axes[1][1].set_title('100 NN')
-        sns.distplot(shared_nn[:, 3], ax=axes[1][1], color='#d62728')
+        sns.histplot(shared_nn[:, 3], ax=axes[1][1], color='#d62728')
         axes[1][1].set_xlabel('Num overlap NN')
         fname = 'NN_overlap.png'
         plot_file = os.path.join(self.model_dir, fname)
         plt.savefig(plot_file)
         plt.close()
 
         self.__log.info('VALIDATION: Plot NN distances.')
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/base.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/base.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/chembl/fetch_chembl.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/chembl/fetch_chembl.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/datasets/drugbank/fetch_drugbank.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/datasets/drugbank/fetch_drugbank.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/evaluation/prediction.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/evaluation/prediction.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/evaluation/score.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/evaluation/score.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/evaluation/validation.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/evaluation/validation.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/io.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/io.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/ml.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/ml.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/autosklearnconfigs.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/autosklearnconfigs.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/gridconfigs.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/gridconfigs.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/hyperoptconfigs.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/hyperoptconfigs.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/tpotconfigs.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/tpotconfigs.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/models/vanillaconfigs.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/models/vanillaconfigs.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/multi.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/multi.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/acp.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/acp.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/base.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/base.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/cp.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/cp.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/evaluation.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/evaluation.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/icp.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/icp.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/nonconformist/nc.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/nonconformist/nc.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/run.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/run.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/signaturizer.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/signaturizer.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/tmsetup.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/tmsetup.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/universes/univs.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/universes/univs.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/chemistry.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/chemistry.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/conformal.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/conformal.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/hpc.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/hpc.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/metrics.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/pairs.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/pairs.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/plots.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/plots.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/reportcard.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/reportcard.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/splitters.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/splitters.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/tasks.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/tool/targetmate/utils/topped.py` & `chemicalchecker-1.0.3/chemicalchecker/tool/targetmate/utils/topped.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/__init__.py` & `chemicalchecker-1.0.3/chemicalchecker/util/__init__.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/aggregate/aggregate.py` & `chemicalchecker-1.0.3/chemicalchecker/util/aggregate/aggregate.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/config/__init__.py` & `chemicalchecker-1.0.3/chemicalchecker/util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/config/cc_config.json` & `chemicalchecker-1.0.3/chemicalchecker/util/config/cc_config.json`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/config/config.py` & `chemicalchecker-1.0.3/chemicalchecker/util/config/config.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/decomposition/correlation.py` & `chemicalchecker-1.0.3/chemicalchecker/util/decomposition/correlation.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/decorator/profilehooks.py` & `chemicalchecker-1.0.3/chemicalchecker/util/decorator/profilehooks.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/decorator/property.py` & `chemicalchecker-1.0.3/chemicalchecker/util/decorator/property.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/decorator/safe.py` & `chemicalchecker-1.0.3/chemicalchecker/util/decorator/safe.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/decorator/timeout.py` & `chemicalchecker-1.0.3/chemicalchecker/util/decorator/timeout.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/download/download.py` & `chemicalchecker-1.0.3/chemicalchecker/util/download/download.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/hpc/__init__.py` & `chemicalchecker-1.0.3/chemicalchecker/util/hpc/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,11 +4,12 @@
 This class allows to send any task to any HPC environmment.
 According to the config parameters this class will send the job
 in the right format to the specified queueing technology.
 The support queing system are:
 
   * **SGE**: :mod:`~chemicalchecker.util.hpc.sge` for Sun Grid Engine
   * **SLURM**: :mod:`~chemicalchecker.util.hpc.slurm` for Slurm Workload
+  * **SLURM**: :mod:`~chemicalchecker.util.hpc.slurm_gpu` for Slurm Workload using GPU server
     Manager
   * **local**: :mod:`~chemicalchecker.util.hpc.local` for local processes.
 """
 from .hpc import HPC
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/hpc/hpc.py` & `chemicalchecker-1.0.3/chemicalchecker/util/hpc/hpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 compress log output.
 """
 import os
 import shutil
 import pathlib
 from .sge import sge
 from .slurm import slurm
+from .slurm_gpu import slurmGPU
 from .local import local
 
 from chemicalchecker.util import logged
 
 
 @logged
 class HPC():
@@ -50,15 +51,18 @@
             self.hpc = eval(self.system)(**kwargs)
         else:
             raise Exception("HPC system %s not available" % self.system)
 
     @classmethod
     def from_config(cls, config):
         if "HPC" in config.keys():
-            return cls(**config.HPC.asdict())
+            if isinstance(config, dict):
+                return cls(**config["HPC"])
+            else:
+                return cls(**config.HPC.asdict())
         else:
             raise Exception("Config does not contain HPC fields")
 
     def submitMultiJob(self, command, **kwargs):
         """Submit multiple job/task.
 
          Args:
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/hpc/local.py` & `chemicalchecker-1.0.3/chemicalchecker/util/hpc/local.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/hpc/sge.py` & `chemicalchecker-1.0.3/chemicalchecker/util/hpc/sge.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 # Loads default environment configuration
 if [[ -f $HOME/.bashrc ]]
 then
   source $HOME/.bashrc
 fi
 
+
 %(command)s
 
     """
 
     defaultOptions = """\
 #$ -S /bin/bash
 #$ -r yes
@@ -127,14 +128,15 @@
         membycore = int(kwargs.get("mem_by_core", 2))
         # total memory that must be available when starting the job
         # does not influence the job being killed or not
         # correspond to mem_free
         memory = kwargs.get("memory", membycore*cpu*0.8)
         # when the job exceeds membycore*cpu il get killed, to start it
         # we ask to have a node with at least 80% of the maximum we can reach
+        max_jobs = kwargs.get("max_jobs", None)
 
         submit_string = 'qsub -terse '
 
         if self.queue is not None:
             submit_string += " -q " + self.queue + " "
 
         if wait:
@@ -169,15 +171,18 @@
                              "G,h_vmem=" + str(membycore + 0.2) + "G")
         else:
             jobParams.append("#$ -l h_vmem=" + str(membycore) + "G")
 
         if maxtime is not None:
             jobParams.append(
                 "#$ -l h_rt=" + str(datetime.timedelta(minutes=maxtime)))
-
+        
+        if max_jobs is not None:
+            jobParams.append("#$ -tc " + str(max_jobs))
+            
         # NS, where elements turns into <FILE>
         if len(elements) > 0:
             self.__log.debug("Num elements submitted " + str(len(elements)))
             self.__log.debug("Num Job submitted " + str(num_jobs))
 
             input_dict = dict()
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/hpc/slurm.py` & `chemicalchecker-1.0.3/chemicalchecker/util/hpc/slurm.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/hpc/test_script.py` & `chemicalchecker-1.0.3/chemicalchecker/util/hpc/test_script.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/keytype/detect.py` & `chemicalchecker-1.0.3/chemicalchecker/util/keytype/detect.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/logging/logging_conf.ini` & `chemicalchecker-1.0.3/chemicalchecker/util/logging/logging_conf.ini`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/mol2svg/mol2svg.py` & `chemicalchecker-1.0.3/chemicalchecker/util/mol2svg/mol2svg.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/network/__init__.py` & `chemicalchecker-1.0.3/chemicalchecker/util/network/__init__.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/network/network.py` & `chemicalchecker-1.0.3/chemicalchecker/util/network/network.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/parser/data_calculator.py` & `chemicalchecker-1.0.3/chemicalchecker/util/parser/data_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Each molecule is loaded, and properties/descriptors/features are computed.
 The raw features are yielded in chunks as dictionaries.
 These methods are used to populate the
 :mod:`~chemicalchecker.database.calcdata`
 database where the table has the same name as functions defined here.
 """
 import os
+import numpy as np
 
 from chemicalchecker.util import logged
 from chemicalchecker.util.decorator import timeout
 
 
 @logged
 class DataCalculator():
@@ -25,15 +26,15 @@
             return eval('DataCalculator.' + function)
         except Exception as ex:
             DataCalculator.__log.error(
                 "Cannot find calculator function %s", function)
             raise ex
 
     @staticmethod
-    def morgan_fp_r2_2048(inchikey_inchi, chunks=1000):
+    def morgan_fp_r2_2048(inchikey_inchi, chunks=1000, dense=True):
         try:
             from rdkit.Chem import AllChem as Chem
         except ImportError:
             raise ImportError("requires rdkit " +
                               "https://www.rdkit.org/")
         iks = inchikey_inchi.keys()
         nBits = 2048
@@ -49,20 +50,26 @@
                 DataCalculator.__log.debug("Skipping molecule %s" % ik)
                 DataCalculator.__log.debug(str(ex))
                 continue
             info = {}
             # print mol
             fp = Chem.GetMorganFingerprintAsBitVect(
                 mol, radius, nBits=nBits, bitInfo=info)
-            dense = ",".join("%d" % s for s in sorted(
-                [x for x in fp.GetOnBits()]))
-            result = {
-                "inchikey": ik,
-                "raw": dense
-            }
+            if dense:
+                dense = ",".join("%d" % s for s in sorted(
+                    [x for x in fp.GetOnBits()]))
+                result = {
+                    "inchikey": ik,
+                    "raw": dense
+                }
+            else:
+                result = {
+                    "inchikey": ik,
+                    "raw": np.array(fp)
+                }
             chunk.append(result)
             if len(chunk) == chunks:
                 yield chunk
                 chunk = list()
         yield chunk
 
     @staticmethod
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/parser/parser.py` & `chemicalchecker-1.0.3/chemicalchecker/util/parser/parser.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/performance/linkprediction.py` & `chemicalchecker-1.0.3/chemicalchecker/util/performance/linkprediction.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         all_nodes_emb = set(range(self.sign2.shape[0]))
         if not all_nodes_net == all_nodes_emb:
             self.__log.warn("Network and embedding do not have same nodes!")
         all_nodes_set = all_nodes_net & all_nodes_emb
         if limit_nodes:
             all_nodes_set = all_nodes_set & limit_nodes
         all_nodes = list(all_nodes_set)
-        matrix = self.sign2[:]
+        matrix = self.sign2.get_h5_dataset('V')
         if len(all_nodes) < 100:
             raise Exception(
                 "Insufficient nodes for validation: %s" % len(all_nodes))
         for node in tqdm(all_nodes):
             node_sign2 = matrix[node]
             # get edges_to_sample true and distances
             neig = list(self.network.neighbors(node))
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/performance/performance.py` & `chemicalchecker-1.0.3/chemicalchecker/util/performance/performance.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/pipeline.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/task_base.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/task_base.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks/python_callable_task.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks/python_callable_task.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks/task_cc_fit.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks/task_cc_fit.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks/task_cc_predict.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks/task_cc_predict.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_coordinates.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_coordinates.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_libraries.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_libraries.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_molinfo.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_molinfo.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_plots.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_plots.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_projections.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_projections.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_pubchem.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_pubchem.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_showtargets.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_showtargets.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/pipeline/tasks_web/task_web_similars.py` & `chemicalchecker-1.0.3/chemicalchecker/util/pipeline/tasks_web/task_web_similars.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/plot/diagnosticsplot.py` & `chemicalchecker-1.0.3/chemicalchecker/util/plot/diagnosticsplot.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     def available(self):
         d = {
             "across_coverage": "Coverage of other CC signatures",
             "across_roc": "ROC against other CC signatures",
             "atc_roc": "ROC for the ATC CC space (E1)",
             "cosine_distances": "Cosine distance distribution",
             "cross_coverage": "Coverage of another signature",
+            "cross_pr": "PR curve against another signature",
             "cross_roc": "ROC curve against another signature",
             "cluster_sizes": "Size of identified clusters",
             "clusters_projection": "Projection of the clusters",
             "dimensions": "Latent dimensions",
             "euclidean_distances": "Euclidean distance distribution",
             "features_bins": "Binned features values",
             "features_iqr": "IQR of the features values",
@@ -87,14 +88,15 @@
             "key_coverage_projection":
             "Projections with coverage of keys across the CC",
             "keys_iqr": "IQR of the keys values",
             "moa_roc": "ROC for the MoA CC space (B1)",
             "roc": "ROC for any specified space",
             "orthogonality": "Orthogonality of features",
             "outliers": "Detected outliers",
+            "pr": "Precision recall for any specified space",
             "projection": "tSNE 2D projection",
             "ranks_agreement":
             "Agreement between similarity ranks across the CC",
             "ranks_agreement_projection": "Projections of ranks agreements",
             "redundancy": "Redundant keys",
             "values": "Values distibution of the signature"
         }
@@ -121,67 +123,124 @@
         ax.set_xticklabels(["T / R", "R / T"])
         if title is None:
             title = "T = %s | R = %s" % (self.diag.sign.qualified_name,
                                          sign_qualified_name)
         ax.set_title(title)
 
     def _roc(self, ax, results, color, dataset_code=None, alpha=0.25,
-             label=None):
+             label=None, xylabels=True):
         step = 0.001
         fpr = np.arange(0, 1 + step, step)
         tpr = np.interp(fpr, results["fpr"], results["tpr"])
         if color is None:
             color = coord_color(dataset_code)
         ax.plot(fpr, tpr, color=color, label=label)
         ax.plot([0, 1], [0, 1], color="gray", linestyle="--")
         ax.fill_between(fpr, tpr, color=color, alpha=alpha)
         ax.set_xlim(-0.05, 1.05)
         ax.set_ylim(-0.05, 1.05)
-        ax.set_xlabel("FPR")
-        ax.set_ylabel("TPR")
+        if xylabels:
+            ax.set_xlabel("FPR")
+            ax.set_ylabel("TPR")
+        return ax
+
+    def _pr(self, ax, results, color, dataset_code=None, alpha=0.25,
+            label=None, xylabels=True):
+        recall = results["recall"]
+        precision = results["precision"]
+        if color is None:
+            color = coord_color(dataset_code)
+        ax.plot(recall, precision, color=color, label=label)
+        ax.axhline(0.5, color="gray", linestyle="--")
+        ax.fill_between(recall, precision, color=color, alpha=alpha)
+        ax.set_xlim(-0.05, 1.05)
+        ax.set_ylim(-0.05, 1.05)
+        if xylabels:
+            ax.set_xlabel("Recall")
+            ax.set_ylabel("Precision")
+        return ax
+
+    def _pr(self, ax, results, color, dataset_code=None, alpha=0.25,
+            label=None):
+        recall = results["recall"]
+        precision = results["precision"]
+        if color is None:
+            color = coord_color(dataset_code)
+        ax.plot(recall, precision, color=color, label=label)
+        ax.axhline(0.5, color="gray", linestyle="--")
+        ax.fill_between(recall, precision, color=color, alpha=alpha)
+        ax.set_xlim(-0.05, 1.05)
+        ax.set_ylim(-0.05, 1.05)
+        ax.set_xlabel("Recall")
+        ax.set_ylabel("Precision")
         return ax
 
     # @safe_return(None)
     def cross_roc(self, results=None, sign=None, ax=None, title=None,
-                  color=None):
+                  color=None, xylabels=True):
         ax = self._get_ax(ax)
         color = self._get_color(color)
         fn = os.path.join(self.diag.path,
                           "cross_roc_%s.pkl" % sign.qualified_name)
         if results is None:
             results = self.load_diagnosis_pickle(fn)
-        ax = self._roc(ax, results, color)
-        if title is None:
-            title = "%s | %s (%.3f)" % (self.diag.sign.qualified_name,
-                                        sign.qualified_name, results["auc"])
+        ax = self._roc(ax, results, color, xylabels=xylabels)
+        if title != False:
+            if title is None:
+                title = "%s | %s (%.3f)" % (self.diag.sign.qualified_name,
+                                            sign.qualified_name, results["auc"])
         ax.set_title(title)
         return ax
 
     # @safe_return(None)
-    def atc_roc(self, results=None, ax=None, title=None):
+    def cross_pr(self, results=None, sign=None, ax=None, title=None,
+                 color=None, xylabels=True):
         ax = self._get_ax(ax)
-        color = coord_color("E1.001")
+        color = self._get_color(color)
+        fn = os.path.join(self.diag.path,
+                          "cross_roc_%s.pkl" % sign.qualified_name)
+        if results is None:
+            results = self.load_diagnosis_pickle(fn)
+        ax = self._pr(ax, results, color, xylabels=xylabels)
+        if title != False:
+            if title is None:
+                title = "%s | %s (%.3f)" % (self.diag.sign.qualified_name,
+                                            sign.qualified_name,
+                                            results["average_precision_score"])
+        ax.set_title(title)
+        return ax
+
+    # @safe_return(None)
+    def atc_roc(self, results=None, ax=None, title=None, color=None,
+                xylabels=True):
+        ax = self._get_ax(ax)
+        if color is None:
+            color = coord_color("E1.001")
         if results is None:
             results = self.load_diagnosis_pickle("atc_roc.pkl")
-        ax = self._roc(ax, results, color)
-        if title is None:
-            title = "ATC (%.3f)" % results["auc"]
+        ax = self._roc(ax, results, color, xylabels=xylabels)
+        if title != False:
+            if title is None:
+                title = "ATC (%.3f)" % results["auc"]
         ax.set_title(title)
         return ax
 
     # @safe_return(None)
-    def moa_roc(self, results=None, ax=None, title=None):
+    def moa_roc(self, results=None, ax=None, title=None, color=None,
+                xylabels=True):
         ax = self._get_ax(ax)
-        color = coord_color("B1.001")
+        if color is None:
+            color = coord_color("B1.001")
         if results is None:
             results = self.load_diagnosis_pickle("moa_roc.pkl")
-        ax = self._roc(ax, results, color)
-        if title is None:
-            title = "MoA (%.3f)" % results["auc"]
-        ax.set_title(title)
+        ax = self._roc(ax, results, color, xylabels=xylabels)
+        if title != False:
+            if title is None:
+                title = "MoA (%.3f)" % results["auc"]
+            ax.set_title(title)
         return ax
 
     # @safe_return(None)
     def roc(self, ds, results=None, ax=None, title=None):
         ax = self._get_ax(ax)
         color = coord_color(ds)
         if results is None:
@@ -189,24 +248,37 @@
         ax = self._roc(ax, results, color)
         if title is None:
             title = "AUROC (%.3f)" % results["auc"]
         ax.set_title(title)
         return ax
 
     # @safe_return(None)
+    def pr(self, ds, results=None, ax=None, title=None):
+        ax = self._get_ax(ax)
+        color = coord_color(ds)
+        if results is None:
+            results = self.load_diagnosis_pickle("pr.pkl")
+        ax = self._pr(ax, results, color)
+        if title is None:
+            title = "Average precision score (%.3f)" % results["average_precision_score"]
+        ax.set_title(title)
+        return ax
+
+    # @safe_return(None)
     def neigh_roc(self, ds, results=None, ax=None, title=None):
         ax = self._get_ax(ax)
         color = coord_color(ds)
         if results is None:
             results = self.load_diagnosis_pickle("neigh_roc.pkl")
         for nn, res in results.items():
             if res is None:
                 continue
             ax = self._roc(
-                ax, res, color, label='NN {:<5} (AUC {:.3f})'.format(nn, res['auc']))
+                ax, res, color,
+                label='NN {:<5} (AUC {:.3f})'.format(nn, res['auc']))
         ax.legend()
         return ax
 
     # @safe_return(None)
     def image(self, results=None, ax=None, title=None, cmap="coolwarm",
               cap_percentile=None):
         ax = self._get_ax(ax)
@@ -950,102 +1022,165 @@
             ax.text(0.1, i + 1, s="%s: %s" % r, va="center")
         ax.set_axis_off()
         ax.set_ylim(6, 0)
         ax.set_xlim(-0.1, 1)
         ax.set_title("CC levels")
         return ax
 
-    def canvas_small(self, title):
+    def canvas_small(self, title, skip_plots):
         fig = plt.figure(figsize=(14, 4))
         gs = fig.add_gridspec(2, 6, wspace=0.6, hspace=0.6)
-
-        self.image(ax=fig.add_subplot(gs[0, :2]))
-        self.features_bins(ax=fig.add_subplot(gs[1, 0]))
-        self.keys_bins(ax=fig.add_subplot(gs[1, 1]))
-        self.values(ax=fig.add_subplot(gs[0, 2]))
-        self.redundancy(ax=fig.add_subplot(gs[1, 2]))
-        self.projection(ax=fig.add_subplot(gs[0:2, 3:5]))
-        self.euclidean_distances(ax=fig.add_subplot(gs[0, 5]))
-        self.cosine_distances(ax=fig.add_subplot(gs[1, 5]))
+        if "image" not in skip_plots:
+            self.image(ax=fig.add_subplot(gs[0, :2]))
+        if "features_bins" not in skip_plots:
+            self.features_bins(ax=fig.add_subplot(gs[1, 0]))
+        if "keys_bins" not in skip_plots:
+            self.keys_bins(ax=fig.add_subplot(gs[1, 1]))
+        if "values" not in skip_plots:
+            self.values(ax=fig.add_subplot(gs[0, 2]))
+        if "redundancy" not in skip_plots:
+            self.redundancy(ax=fig.add_subplot(gs[1, 2]))
+        if "projection" not in skip_plots:
+            self.projection(ax=fig.add_subplot(gs[0:2, 3:5]))
+        if "euclidean_distances" not in skip_plots:
+            self.euclidean_distances(ax=fig.add_subplot(gs[0, 5]))
+        if "cosine_distances" not in skip_plots:
+            self.cosine_distances(ax=fig.add_subplot(gs[1, 5]))
 
         if title is None:
             title = "%s %s" % (self.diag.sign.dataset, self.diag.sign.cctype)
         fig.suptitle(title, fontweight="bold", y=1, size='xx-large')
         plt.close()
         return fig
 
-    def canvas_medium(self, title):
+    def canvas_medium(self, title, skip_plots):
         fig = plt.figure(figsize=(14, 14))
         gs = fig.add_gridspec(6, 6, wspace=0.6, hspace=0.6)
         ax = fig.add_subplot(gs[0, 0])
         self.legend(ax=ax)
-        ax = fig.add_subplot(gs[1, 5])
-        self.redundancy(ax=ax)
-        ax = fig.add_subplot(gs[0, 5])
-        self.outliers(ax=ax)
-        ax = fig.add_subplot(gs[1, 0])
-        self.values(ax=ax)
-        ax = fig.add_subplot(gs[0, 1])
+        if "redundancy" not in skip_plots:
+            ax = fig.add_subplot(gs[1, 5])
+            self.redundancy(ax=ax)
+        if "outliers" not in skip_plots:
+            ax = fig.add_subplot(gs[0, 5])
+            self.outliers(ax=ax)
+        if "values" not in skip_plots:
+            ax = fig.add_subplot(gs[1, 0])
+            self.values(ax=ax)
+        if "confidences" or "intensities" not in skip_plots:
+            ax = fig.add_subplot(gs[0, 1])
+            if self.diag.sign.cctype == 'sign3':
+                if "confidences" not in skip_plots:
+                    self.confidences(ax=ax)
+                    if "confidences_projection" not in skip_plots:
+                        ax = fig.add_subplot(gs[0, 2])
+                        self.confidences_projection(ax=ax)
+            else:
+                if "intensities" not in skip_plots:
+                    self.intensities(ax=ax)
+                    if "intensities_projection" not in skip_plots:
+                        ax = fig.add_subplot(gs[0, 2])
+                        self.intensities_projection(ax=ax)
+        if "key_coverage" not in skip_plots:
+            ax = fig.add_subplot(gs[1, 1])
+            self.key_coverage(ax=ax)
+            if "key_coverage_projection" not in skip_plots:
+                ax = fig.add_subplot(gs[1, 2])
+                self.key_coverage_projection(ax=ax)
+        if "global_ranks_agreement" not in skip_plots:
+            ax = fig.add_subplot(gs[0, 4])
+            self.global_ranks_agreement(ax=ax)
+            if "global_ranks_agreement_projection" not in skip_plots:
+                ax = fig.add_subplot(gs[0, 3])
+                self.global_ranks_agreement_projection(ax=ax)
+        if "cluster_sizes" not in skip_plots:
+            ax = fig.add_subplot(gs[1, 4])
+            self.cluster_sizes(ax=ax)
+            if "clusters_projection" not in skip_plots:
+                ax = fig.add_subplot(gs[1, 3])
+                self.clusters_projection(ax=ax)
+        if "euclidean_distances" not in skip_plots:
+            ax = fig.add_subplot(gs[2, 4])
+            self.euclidean_distances(ax=ax)
+        if "cosine_distances" not in skip_plots:
+            ax = fig.add_subplot(gs[2, 5])
+            self.cosine_distances(ax=ax)
+        if "features_bins" not in skip_plots:
+            ax = fig.add_subplot(gs[3, 0])
+            self.features_bins(ax=ax)
+        if "keys_bins" not in skip_plots:
+            ax = fig.add_subplot(gs[3, 1])
+            self.keys_bins(ax=ax)
+        if "projection" not in skip_plots:
+            ax = fig.add_subplot(gs[2:4, 2:4])
+            self.projection(ax=ax)
+        if "image" not in skip_plots:
+            ax = fig.add_subplot(gs[2, :2])
+            self.image(ax=ax)
+        if "moa_roc" not in skip_plots:
+            ax = fig.add_subplot(gs[3, 4])
+            self.moa_roc(ax=ax)
+        if "atc_roc" not in skip_plots:
+            ax = fig.add_subplot(gs[3, 5])
+            self.atc_roc(ax=ax)
+        if "dimensions" not in skip_plots:
+            ax = fig.add_subplot(gs[-2:, :2])
+            self.dimensions(ax=ax)
+        if "across_coverage" not in skip_plots:
+            ax = fig.add_subplot(gs[-2, 2:4])
+            self.across_coverage(ax=ax, vs=True)
+            ax = fig.add_subplot(gs[-1, 2:4])
+            self.across_coverage(ax=ax, vs=False)
+        if "across_roc" not in skip_plots:
+            ax = fig.add_subplot(gs[-2:, 4:6])
+            self.across_roc(ax=ax)
+        if title is None:
+            title = "%s %s" % (self.diag.sign.dataset, self.diag.sign.cctype)
+        fig.suptitle(title, fontweight="bold", y=0.92, size='xx-large')
+        plt.close()
+        return fig
+
+    def canvas_large(self, title, skip_plots):
+        pass
+
+    def custom_comparative_vertical(self, title, skip_plots):
+        fig = plt.figure(figsize=(9, 9))
+        gs = fig.add_gridspec(4, 4, wspace=0.6, hspace=0.6)
+        #plt.figtext(0.02, 0.5, 'TEST', fontsize=12, fontweight="bold")
+        ax = fig.add_subplot(gs[0:2, 0:2])
+        self.projection(ax=ax)
+        #text = ax.text(-55,45,"A)",fontsize=12, fontweight="bold")
+        ax = fig.add_subplot(gs[2, 1])
+        self.legend(ax=ax)
+        ax = fig.add_subplot(gs[0, 2])
         if self.diag.sign.cctype == 'sign3':
             self.confidences(ax=ax)
         else:
             self.intensities(ax=ax)
-        ax = fig.add_subplot(gs[0, 2])
-        if self.diag.sign.cctype == 'sign3':
-            self.confidences_projection(ax=ax)
-        else:
-            self.intensities_projection(ax=ax)
-        ax = fig.add_subplot(gs[1, 1])
-        self.key_coverage(ax=ax)
-        ax = fig.add_subplot(gs[1, 2])
-        self.key_coverage_projection(ax=ax)
+        #text1 = ax.text(-1,1,"B)",fontsize=12, fontweight="bold")
         ax = fig.add_subplot(gs[0, 3])
-        self.global_ranks_agreement_projection(ax=ax)
-        ax = fig.add_subplot(gs[0, 4])
-        self.global_ranks_agreement(ax=ax)
-        ax = fig.add_subplot(gs[1, 3])
         self.clusters_projection(ax=ax)
-        ax = fig.add_subplot(gs[1, 4])
-        self.cluster_sizes(ax=ax)
-        ax = fig.add_subplot(gs[2, 4])
-        self.euclidean_distances(ax=ax)
-        ax = fig.add_subplot(gs[2, 5])
-        self.cosine_distances(ax=ax)
-        ax = fig.add_subplot(gs[3, 0])
-        self.features_bins(ax=ax)
-        ax = fig.add_subplot(gs[3, 1])
-        self.keys_bins(ax=ax)
-        ax = fig.add_subplot(gs[2:4, 2:4])
-        self.projection(ax=ax)
-        ax = fig.add_subplot(gs[2, :2])
-        self.image(ax=ax)
-        ax = fig.add_subplot(gs[3, 4])
+        #text1 = ax.text(-50,-50,"C)",fontsize=12, fontweight="bold")
+        ax = fig.add_subplot(gs[1, 2])
         self.moa_roc(ax=ax)
-        ax = fig.add_subplot(gs[3, 5])
+        ax = fig.add_subplot(gs[1, 3])
         self.atc_roc(ax=ax)
-        ax = fig.add_subplot(gs[-2:, :2])
-        self.dimensions(ax=ax)
-        ax = fig.add_subplot(gs[-2, 2:4])
-        self.across_coverage(ax=ax, vs=True)
-        ax = fig.add_subplot(gs[-1, 2:4])
-        self.across_coverage(ax=ax, vs=False)
-        ax = fig.add_subplot(gs[-2:, 4:6])
+        ax = fig.add_subplot(gs[2:4, 2:4])
         self.across_roc(ax=ax)
         if title is None:
             title = "%s %s" % (self.diag.sign.dataset, self.diag.sign.cctype)
-        fig.suptitle(title, fontweight="bold", y=0.92, size='xx-large')
+        fig.suptitle(title, fontweight="bold", y=0.95, size='xx-large')
         plt.close()
         return fig
 
-    def canvas_large(self, title):
-        pass
-
-    def canvas(self, size="medium", title=None):
+    def canvas(self, size="medium", title=None, skip_plots=[]):
         self.__log.debug("Plotting Canvas %s" % size)
         if size == "small":
-            return self.canvas_small(title=title)
+            return self.canvas_small(title=title, skip_plots=skip_plots)
         elif size == "medium":
-            return self.canvas_medium(title=title)
+            return self.canvas_medium(title=title, skip_plots=skip_plots)
         elif size == "large":
-            return self.canvas_large(title=title)
+            return self.canvas_large(title=title, skip_plots=skip_plots)
+        elif size == "compare_v":
+            return self.custom_comparative_vertical(title=title, skip_plots=skip_plots)
         else:
             return None
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/plot/multiccplot.py` & `chemicalchecker-1.0.3/chemicalchecker/util/plot/multiccplot.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/plot/multiplot.py` & `chemicalchecker-1.0.3/chemicalchecker/util/plot/multiplot.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/plot/plot.py` & `chemicalchecker-1.0.3/chemicalchecker/util/plot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -964,15 +964,15 @@
         plt.close()
 
     def sign_feature_distribution_plot(self, sign, max_samples=10000):
         if sign.shape[0] > max_samples:
             keys = np.random.choice(sign.keys, max_samples, replace=False)
             matrix = sign.get_vectors(keys)[1]
         else:
-            matrix = sign[:]
+            matrix = sign.get_h5_dataset('V')
         df = pd.DataFrame(matrix).melt()
 
         coord = self.dataset_code
         fig = plt.figure(figsize=(10, 3), dpi=100)
         ax = fig.add_subplot(111)
         sns.pointplot(x='variable', y='value', data=df,
                       ax=ax, ci='sd', join=False, markers='.',
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/plot/util.py` & `chemicalchecker-1.0.3/chemicalchecker/util/plot/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,38 +25,44 @@
 
 
 def rgb2hex(r, g, b):
     """RGB to hexadecimal."""
     return '#%02x%02x%02x' % (r, g, b)
 
 
+def cc_palette(order='ABCDE', lighness=0):
+    return [predefined_cc_colors(s, lighness) for s in order]
+
+
 def predefined_cc_colors(coord, lighness=0):
     """Predefined CC colors."""
     colors = {
-        'A': '#EA5A49', # '#EE7B6D', '#F7BDB6'],
-        'B': '#B16BA8', # '#C189B9', '#D0A6CB'],
-        'C': '#5A72B5', # '#7B8EC4', '#9CAAD3'],
-        'D': '#7CAF2A', # '#96BF55', '#B0CF7F'],
-        'E': '#F39426', # '#F5A951', '#F8BF7D'],
-        'Z': '#000000', # '#666666', '#999999']
+        'A': '#EA5A49',  # '#EE7B6D', '#F7BDB6'],
+        'B': '#B16BA8',  # '#C189B9', '#D0A6CB'],
+        'C': '#5A72B5',  # '#7B8EC4', '#9CAAD3'],
+        'D': '#7CAF2A',  # '#96BF55', '#B0CF7F'],
+        'E': '#F39426',  # '#F5A951', '#F8BF7D'],
+        'Z': '#000000',  # '#666666', '#999999']
     }
     if not coord in colors:
         coord = 'Z'
-    return lighten_color(colors[coord[:1]], amount=1-lighness)
+    return lighten_color(colors[coord[:1]], amount=1 - lighness)
+
 
 def lighten_color(color, amount=0):
     if amount == 0:
         return color
     try:
         c = mc.cnames[color]
     except:
         c = color
     c = colorsys.rgb_to_hls(*mc.to_rgb(c))
     return colorsys.hls_to_rgb(c[0], 1 - amount * (1 - c[1]), c[2])
 
+
 def cc_colors(coordinate, lighness=0, alternate=False, dark_first=True):
     """CC coordinate to CC color."""
     if alternate:
         return _cc_colors_alternate(coordinate, lighness, dark_first)
     else:
         return predefined_cc_colors(coordinate[0], lighness)
 
@@ -80,14 +86,48 @@
 def cc_coords():
     coords = list()
     for name, code in itertools.product("ABCDE", "12345"):
         coords.append(name + code)
     return coords
 
 
+def cc_coords_name(ds):
+    fullnames = {
+        "A1": "2D fingerprints",
+        "A2": "3D fingerprints",
+        "A3": "Scaffolds",
+        "A4": "Structural keys",
+        "A5": "Physicochemistry",
+        "B1": "Mechanism of action",
+        "B2": "Metabolic genes",
+        "B3": "Crystals",
+        "B4": "Binding",
+        "B5": "HTS bioassays",
+        "C1": "Small molecule roles",
+        "C2": "Small molecule pahtways",
+        "C3": "Signaling pathways",
+        "C4": "Biological processes",
+        "C5": "Networks",
+        "D1": "Gene expression",
+        "D2": "Cancer cell lines",
+        "D3": "Chemical genetics",
+        "D4": "Morphology",
+        "D5": "Cell bioassays",
+        "E1": "Therapeutic areas",
+        "E2": "Indications",
+        "E3": "Side effects",
+        "E4": "Diseases and toxicology",
+        "E5": "Drug-drug interactions"
+    }
+    if ds[:2] in fullnames:
+        return fullnames[ds[:2]]
+    else:
+        return 'New space'
+
+
 def lighten_color(color, amount=0.5):
     """Lighthen a color."""
     try:
         c = mc.cnames[color]
     except Exception:
         c = color
     c = colorsys.rgb_to_hls(*mc.to_rgb(c))
@@ -151,99 +191,133 @@
         plt.subplots_adjust(**margins)
     grid = fig.add_gridspec(*grid, wspace=0.25, hspace=0.35,
                             width_ratios=width_ratios,
                             height_ratios=height_ratios)
     return fig, grid
 
 
-def cc_grid(fig, grid, legend_out=True):
+def cc_grid(fig, grid, legend_out=True, cc_space_names=False, wspace=0,
+            hspace=0, shared_xlabel=None, shared_ylabel=None):
     axes = list()
     if legend_out:
         subgrid = grid[:, :].subgridspec(
-            2, 1, height_ratios=(1, 40), wspace=0, hspace=0.02)
+            2, 1, height_ratios=(1, 40), wspace=wspace, hspace=hspace + 0.02)
         ax_legend = fig.add_subplot(subgrid[0])
         axes.append(ax_legend)
-        subgrid = subgrid[1].subgridspec(5, 5, wspace=-0.15, hspace=0)
+        subgrid = subgrid[1].subgridspec(
+            5, 5, wspace=wspace - 0.15, hspace=hspace)
     else:
-        subgrid = grid[:, :].subgridspec(5, 5, wspace=0, hspace=0)
+        subgrid = grid[:, :].subgridspec(5, 5, wspace=wspace, hspace=hspace)
     for idx, (gs, ds) in enumerate(zip(subgrid, cc_coords())):
         ax = fig.add_subplot(gs)
         ax.set_aspect('equal')
         homogenous_ticks(ax, 2)
         ax.tick_params(axis='both', length=2, left=False, bottom=False,
                        right=False)
         if idx % 5 == 0:
             ax.tick_params(axis='y', left=True)
             ax.set_ylabel(ds[0], labelpad=2, rotation='horizontal',
                           va='center', ha='center')
+
         if idx >= 20:
             ax.tick_params(axis='x', bottom=True)
             # ax.xaxis.set_label_position('top')
             ax.set_xlabel(ds[1], labelpad=-1)
+        if cc_space_names:
+            ax.set_title(cc_coords_name(ds))
+            ax.set_ylabel('')
+            ax.set_xlabel('')
         axes.append(ax)
+    if shared_xlabel:
+        fig.text(0.5, 0.02, shared_xlabel, ha='center')
+    if shared_ylabel:
+        fig.text(0.02, 0.5, shared_ylabel, va='center', rotation='vertical')
     return axes
 
 
 def make_cbar_ax(ax, cmap=plt.get_cmap('viridis'), title=''):
     cbar = colorbar.ColorbarBase(ax, orientation='horizontal',
                                  ticklocation='top', cmap=cmap)
     cbar.ax.set_xlabel(title, labelpad=0)
     cbar.ax.tick_params(axis='x', pad=0)
     cbar.set_ticks([1, .8, .6, .4, .2, .0])
     cbar.set_ticklabels(['High', '', '', '', '', 'Low'])
     # cbar.ax.invert_xaxis()
     cbar.ax.set_aspect(0.04)
 
 
-def projection(front, back=None, front_kwargs=[], back_kwargs={}, ax=None,
-               density_subsample=1000):
+def projection(front, back=None, front_kwargs=[], ax=None,
+               density_subsample=1000, update_proj_limits=True,
+               min_point=5, proj_margin_perc=0.05):
 
-    def _proj_lims(P):
+    def _proj_range(P, margin_perc):
         xlim = [np.min(P[:, 0]), np.max(P[:, 0])]
         ylim = [np.min(P[:, 1]), np.max(P[:, 1])]
-        xscale = (xlim[1] - xlim[0]) * 0.05
-        yscale = (ylim[1] - ylim[0]) * 0.05
-        xlim[0] -= xscale
-        xlim[1] += xscale
-        ylim[0] -= yscale
-        ylim[1] += yscale
         abs_lim = np.max(np.abs(np.vstack([xlim, ylim])))
-        return (-abs_lim, abs_lim),(-abs_lim, abs_lim)
+        margin = abs_lim * 2 * margin_perc
+        proj_range = (- abs_lim - margin, abs_lim + margin)
+        return proj_range, proj_range
 
     if ax is None:
         fig, ax = plt.subplots(1, 1, figsize=(7, 7))
 
     if not isinstance(front, list):
         front = [front]
 
-    if back is not None:
-        ax.scatter(back[:, 0], back[:, 1], **back_kwargs)
+    if not isinstance(front_kwargs, list):
+        front_kwargs = [front_kwargs]
 
     for proj, kwargs in zip(front, front_kwargs):
         x = proj[:, 0]
         y = proj[:, 1]
+
         density = kwargs.pop('density', False)
-        color = kwargs.pop('color', 'black')
-        cmap = kwargs.pop('cmap', 'viridis')
-        lw = kwargs.pop('lw', 0)
-        s_min = kwargs.pop('s_min', 5)
-        s_max = kwargs.pop('s_max', 500)
-        if len(x) <= 2:
-            density = False
-            color = 'black'
+        density_kw = dict(cmap='viridis', s_min=5, s_max=20,
+                          lw=0, density_subsample=1000)
+        density_kw.update(kwargs.pop('density_kwargs', {}))
+
+        contour = kwargs.pop('contour', False)
+        contour_kw = dict(thresh=0, linewidths=0.8, levels=10,
+                          contour_subsample=1000)
+        contour_kw.update(kwargs.pop('contour_kwargs', {}))
+
+        scatter_kw = dict()
+        scatter_kw.update(kwargs.pop('scatter_kwargs', {}))
+
+        if len(x) <= min_point and (contour or density):
+            if contour:
+                contour = False
+                cmap = contour_kw['cmap']
+            if density:
+                density = False
+                cmap = density_kw['cmap']
+            if not callable(cmap):
+                cmap = matplotlib.cm.get_cmap(cmap)
+            scatter_kw = {'c':cmap(1.0), 's':density_kw['s_max']}
+
         if density:
             xy = np.vstack([x, y])
+            density_subsample = density_kw.pop('density_subsample')
             z = gaussian_kde(xy[:, :density_subsample])(xy)
             idx = z.argsort()
             x, y, z = x[idx], y[idx], z[idx]
-            ax.scatter(x, y, c=z, s=minmax_scale(z, (s_min, s_max)),
-                       cmap=cmap, lw=lw, **kwargs)
+            if 'c' not in density_kw:
+                density_kw['c'] = z
+            if 's' not in density_kw:
+                s_min = density_kw.pop('s_min')
+                s_max = density_kw.pop('s_max')
+                density_kw['s'] = minmax_scale(z, (s_min, s_max))
+            ax.scatter(x, y, **density_kw)
+        elif contour:
+            contour_subsample = contour_kw.pop('contour_subsample')
+            sns.kdeplot(x=x[:contour_subsample], y=y[:contour_subsample],
+                        ax=ax, **contour_kw)
         else:
-            ax.scatter(x, y, c=color, **kwargs)
+            ax.scatter(x, y, **scatter_kw)
 
     all_projs = np.vstack(front)
-    if back is not None:
-        all_projs = np.vstack([all_projs, back])
-    xlim, ylim = _proj_lims(all_projs)
-    ax.set_xlim(xlim)
-    ax.set_ylim(ylim)
-    return ax
+
+    if update_proj_limits:
+        xlim, ylim = _proj_range(all_projs, margin_perc=proj_margin_perc)
+        ax.set_xlim(xlim)
+        ax.set_ylim(ylim)
+    return ax
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/psql/psql.py` & `chemicalchecker-1.0.3/chemicalchecker/util/psql/psql.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/remove_near_duplicates/remove_near_duplicates.py` & `chemicalchecker-1.0.3/chemicalchecker/util/remove_near_duplicates/remove_near_duplicates.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/sampler/triplets.py` & `chemicalchecker-1.0.3/chemicalchecker/util/sampler/triplets.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/sanitize/sanitizer.py` & `chemicalchecker-1.0.3/chemicalchecker/util/sanitize/sanitizer.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/splitter/ae_siam_traintest.py` & `chemicalchecker-1.0.3/chemicalchecker/util/splitter/ae_siam_traintest.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/splitter/globalneighbortriplets.py` & `chemicalchecker-1.0.3/chemicalchecker/util/splitter/globalneighbortriplets.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/splitter/neighborerror.py` & `chemicalchecker-1.0.3/chemicalchecker/util/splitter/neighborerror.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/splitter/neighborpair.py` & `chemicalchecker-1.0.3/chemicalchecker/util/splitter/neighborpair.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/splitter/pairtraintest.py` & `chemicalchecker-1.0.3/chemicalchecker/util/splitter/pairtraintest.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/splitter/traintest.py` & `chemicalchecker-1.0.3/chemicalchecker/util/splitter/traintest.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/transform/base.py` & `chemicalchecker-1.0.3/chemicalchecker/util/transform/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         self.sign_ref = self.sign.get_molset("reference")
         self.name = name
         self.model_path = self.sign_ref.model_path
         self.max_keys = max_keys
         self.categorical = self.is_categorical()
         self.tmp = tmp
 
+
     def reindex_triplets(self, sign1, keys):
         fn = os.path.join(sign1.model_path, "triplets.h5")
         if not os.path.exists(fn):
             self.__log.debug("No triplets file found in %s" % fn)
             return
         keys_old = sign1.keys
         if not np.any(keys != keys_old):
@@ -99,14 +100,15 @@
                 mappings, DataSignature.string_dtype()))
         sign1.refresh()
 
     def overwrite(self, sign1, V, keys):
         sign1.refresh()
         self.reindex_triplets(sign1, keys)
         data_path = sign1.data_path
+        sign1.close_hdf5()
         with h5py.File(data_path, "r+") as hf:
             if self.tmp:
                 keys_ = hf["keys"][:]
                 mask = np.isin(list(keys_), list(keys))
                 del hf["V_tmp"]
                 hf["V_tmp"] = V
                 V = hf["V"][:][mask]
@@ -135,17 +137,17 @@
 
     def subsample(self):
         max_keys = self.max_keys
         if max_keys is None or max_keys >= self.sign_ref.shape[0]:
             self.__log.debug("Considering all reference data")
             keys = self.sign_ref.keys
             if self.tmp:
-                V = self.sign_ref.get_h5_dataset("V_tmp")[:]
+                V = self.sign_ref.get_h5_dataset("V_tmp")
             else:
-                V = self.sign_ref[:]
+                V = self.sign_ref.get_h5_dataset("V")
         else:
             self.__log.debug(
                 "Subsampling data (ensuring coverage of at least one feature)")
             idxs = set()
             with h5py.File(self.sign_ref.data_path, "r") as hf:
                 if self.tmp:
                     dkey = "V_tmp"
@@ -187,16 +189,18 @@
     def chunker(n, size=2000):
         for i in range(0, n, size):
             yield slice(i, i + size)
 
     def is_categorical(self, n=1000):
         self.__log.debug("Checking continuous or categorical")
         V = self.sign_ref[:n]
+        self.sign_ref.close_hdf5()
         is_cat = np.all(V == V.astype(np.int))
         if not is_cat:
             return False
         V = self.sign[:n]
+        self.sign.close_hdf5()
         is_cat = np.all(V == V.astype(np.int))
         if is_cat:
             return True
         else:
             return False
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/transform/gaussian_scale_impute.py` & `chemicalchecker-1.0.3/chemicalchecker/util/transform/gaussian_scale_impute.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/transform/gaussianize.py` & `chemicalchecker-1.0.3/chemicalchecker/util/transform/gaussianize.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/transform/lsi.py` & `chemicalchecker-1.0.3/chemicalchecker/util/transform/lsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,14 @@
                     'Getting only zero rows: %s', str(only_zeros))
                 self.num_topics += 50
                 self.variance_explained = min(
                     self.variance_explained + 0.05, 1)
                 self.__log.warning(
                     'Repeating LSI with: variance_explained: %.2f num_topics: %s',
                     self.variance_explained, str(self.num_topics))
-
         self.predict(self.sign_ref)
         self.predict(self.sign)
         self.save()
 
     def predict(self, sign1):
         self.predict_check(sign1)
         # corpus for the predict
@@ -199,14 +198,15 @@
                 ks = sign1.keys[chunk]
                 for i in range(0, len(ks)):
                     # save dense represantation (feat with 1 values only)
                     row = vs[i]
                     mask = np.argwhere(row > 0).ravel()
                     val = ",".join(self.features[mask])
                     f.write("%s %s\n" % (ks[i], val))
+            sign1.close_hdf5()
         # load dictionary
         dictionary = corpora.Dictionary.load(
             os.path.join(self.model_path, self.name + ".dict.pkl"))
         # init corpus object
         c = Corpus(plain_corpus, dictionary)
         tfidf = models.TfidfModel.load(os.path.join(
             self.model_path, self.name + ".tfidf.pkl"))
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/transform/metric_learn.py` & `chemicalchecker-1.0.3/chemicalchecker/util/transform/metric_learn.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pickle
 import numpy as np
 
 from .base import BaseTransform
 
 from chemicalchecker.util import logged
 from chemicalchecker.tool.siamese import SiameseTriplets
-from chemicalchecker.util.splitter import NeighborTripletTraintest
+from chemicalchecker.util.splitter import PrecomputedTripletSampler
 
 
 @logged
 class MetricLearn(BaseTransform):
     """MetricLearn class."""
 
     def __init__(self, sign1, tmp, name, max_keys):
@@ -48,26 +48,30 @@
 
     def _fit(self, triplets):
         params = self.params
         # Get signatures
         V = self.sign_ref[:]
         dest_h5 = os.path.join(self.model_path, self.name + "_eval.h5")
         # generate traintest file
-        NeighborTripletTraintest.precomputed_triplets(
-            V, triplets, dest_h5,
+        triplet_sampler = PrecomputedTripletSampler(
+            None, self.sign_ref, dest_h5)
+        triplet_sampler.generate_triplets(
+            V, self.sign_ref.keys, triplets,
             mean_center_x=True,  shuffle=True,
             split_names=['train_train', 'train_test', 'test_test'],
             split_fractions=[.8, .1, .1])
         # train siamese network
         model_dir = os.path.join(self.model_path, self.name + "_eval")
         params["traintest_file"] = dest_h5
         mod = SiameseTriplets(model_dir, evaluate=True, plot=False, **params)
         mod.fit()
         # generate traintest file for the final model
         dest_h5 = os.path.join(self.model_path, self.name + ".h5")
+        triplet_sampler = PrecomputedTripletSampler(
+            None, self.sign_ref, dest_h5)
         NeighborTripletTraintest.precomputed_triplets(
             V, triplets, dest_h5,
             mean_center_x=True,  shuffle=True,
             split_names=['train_train'],
             split_fractions=[1.])
         # train siamese network
         model_dir = os.path.join(self.model_path, self.name)
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/transform/pca.py` & `chemicalchecker-1.0.3/chemicalchecker/util/transform/pca.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker/util/transform/scale.py` & `chemicalchecker-1.0.3/chemicalchecker/util/transform/scale.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/chemicalchecker.egg-info/PKG-INFO` & `chemicalchecker-1.0.3/chemicalchecker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemicalchecker
-Version: 1.0.2
+Version: 1.0.3
 Summary: Chemical Checker Package.
 Home-page: http://gitlabsbnb.irbbarcelona.org/packages/chemical_checker
 Author: SBNB
 Author-email: sbnb@irbbarcelona.org
 License: MIT License
 Keywords: chemicalchecker bioactivity signatures chemoinformatics
 Platform: UNKNOWN
```

### Comparing `chemicalchecker-1.0.2/chemicalchecker.egg-info/SOURCES.txt` & `chemicalchecker-1.0.3/chemicalchecker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 chemicalchecker.egg-info/PKG-INFO
 chemicalchecker.egg-info/SOURCES.txt
 chemicalchecker.egg-info/dependency_links.txt
 chemicalchecker.egg-info/not-zip-safe
 chemicalchecker.egg-info/requires.txt
 chemicalchecker.egg-info/top_level.txt
 chemicalchecker/core/__init__.py
+chemicalchecker/core/char.py
 chemicalchecker/core/chemcheck.py
 chemicalchecker/core/clus.py
 chemicalchecker/core/data.py
 chemicalchecker/core/diagnostics.py
 chemicalchecker/core/examples.py
 chemicalchecker/core/molkit.py
 chemicalchecker/core/neig.py
@@ -143,19 +144,22 @@
 chemicalchecker/util/decorator/__init__.py
 chemicalchecker/util/decorator/profilehooks.py
 chemicalchecker/util/decorator/property.py
 chemicalchecker/util/decorator/safe.py
 chemicalchecker/util/decorator/timeout.py
 chemicalchecker/util/download/__init__.py
 chemicalchecker/util/download/download.py
+chemicalchecker/util/filesystem/__init__.py
+chemicalchecker/util/filesystem/filesystem.py
 chemicalchecker/util/hpc/__init__.py
 chemicalchecker/util/hpc/hpc.py
 chemicalchecker/util/hpc/local.py
 chemicalchecker/util/hpc/sge.py
 chemicalchecker/util/hpc/slurm.py
+chemicalchecker/util/hpc/slurm_gpu.py
 chemicalchecker/util/hpc/test_script.py
 chemicalchecker/util/keytype/__init__.py
 chemicalchecker/util/keytype/detect.py
 chemicalchecker/util/logging/__init__.py
 chemicalchecker/util/logging/logging_conf.ini
 chemicalchecker/util/logging/our_logging.py
 chemicalchecker/util/mol2svg/__init__.py
@@ -181,15 +185,17 @@
 chemicalchecker/util/pipeline/tasks_web/task_web_libraries.py
 chemicalchecker/util/pipeline/tasks_web/task_web_molinfo.py
 chemicalchecker/util/pipeline/tasks_web/task_web_plots.py
 chemicalchecker/util/pipeline/tasks_web/task_web_projections.py
 chemicalchecker/util/pipeline/tasks_web/task_web_pubchem.py
 chemicalchecker/util/pipeline/tasks_web/task_web_showtargets.py
 chemicalchecker/util/pipeline/tasks_web/task_web_similars.py
+chemicalchecker/util/pipeline/tasks_web/task_web_statsplots.py
 chemicalchecker/util/plot/__init__.py
+chemicalchecker/util/plot/ccstatsplot.py
 chemicalchecker/util/plot/diagnosticsplot.py
 chemicalchecker/util/plot/multiccplot.py
 chemicalchecker/util/plot/multiplot.py
 chemicalchecker/util/plot/plot.py
 chemicalchecker/util/plot/util.py
 chemicalchecker/util/psql/__init__.py
 chemicalchecker/util/psql/psql.py
```

### Comparing `chemicalchecker-1.0.2/docs/Makefile` & `chemicalchecker-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/docs/_templates/custom-class-template.rst` & `chemicalchecker-1.0.3/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/docs/_templates/custom-module-template.rst` & `chemicalchecker-1.0.3/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/docs/conf.py` & `chemicalchecker-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/docs/img/favicon.ico` & `chemicalchecker-1.0.3/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/docs/img/logo.svg` & `chemicalchecker-1.0.3/docs/img/logo.svg`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/docs/img/preprocessing.png` & `chemicalchecker-1.0.3/docs/img/preprocessing.png`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/docs/index.rst` & `chemicalchecker-1.0.3/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -107,23 +107,30 @@
 |             |             |             | Capture     |             |
 |             |             |             | global      |             |
 |             |             |             | properties  |             |
 |             |             |             | of the      |             |
 |             |             |             | similarity  |             |
 |             |             |             | network.    |             |
 +-------------+-------------+-------------+-------------+-------------+
-| Type 3      | ``sign3``   | Networ      | Fixed       | Possibly    |
-|             |             | k-embedding | dimension   | very noisy, |
-|             |             | of the      | and         | hence       |
-|             |             | inferred    | available   | useless,    |
-|             |             | similarity  | for *any*   | especially  |
-|             |             | network.    | molecule.   | for         |
-|             |             |             |             | low-data    |
+| Type 3      | ``sign3``   | Siamese     | Fixed       | Possibly    |
+|             |             | Neural      | dimension   | very noisy, |
+|             |             | Network     | and         | hence       |
+|             |             | embedding   | available   | useless,    |
+|             |             | derived from| for *many*  | especially  |
+|             |             | all 25      | molecule.   | for         |
+|             |             | spaces.     |             | low-data    |
 |             |             |             |             | datasets.   |
 +-------------+-------------+-------------+-------------+-------------+
+| Type 4      | ``sign4``   | DNN         | Fixed       | Possibly    |
+|             |             | multioutput | dimension   | very noisy, |
+|             |             | regression  | and         | subject to  |
+|             |             | of sign3.   | available   | out of      |
+|             |             |             | for *any*   | distribution|
+|             |             |             | molecule.   | bias.       |
++-------------+-------------+-------------+-------------+-------------+
 
 For further details see the :doc:`Signaturization <signaturization>` section.
 
 .. note::
     A `Signaturizer`_ module for direct molecule signaturization is also available.
 
 .. _scikit-learn: https://scikit-learn.org/
```

### Comparing `chemicalchecker-1.0.2/docs/make.bat` & `chemicalchecker-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/docs/manifesto.rst` & `chemicalchecker-1.0.3/docs/manifesto.rst`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/docs/signaturization.rst` & `chemicalchecker-1.0.3/docs/signaturization.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Signaturization
 ===============
 
 The main feature of the CC is the automatic conversion of virtually any compound-related data into a standard format ready-to-be-used by machine learning algorithms. All CC data is stored as ``HDF5`` files following a folder structure organized by datasets (described in :mod:`chemicalchecker.core.chemcheck`).
 
-The central type of data is the **signature** (one numerical vector per molecule). There are 4 types of signatures:
+The central type of data is the **signature** (one numerical vector per molecule). There are 5 types of signatures:
 
     * **Signatures type 0** :class:`~chemicalchecker.core.sign0`: A sufficiently-processed version of the raw data. They usually show explicit knowledge, which enables connectivity and interpretation.
     * **Signatures type 1** :class:`~chemicalchecker.core.sign1`: A mildly compressed (usually latent) representation of the signatures, with a dimensionality that typically retains 90% of the original variance. They keep most of the complexity of the original data and they can be used for similarity calculations.
     * **Signatures type 2** :class:`~chemicalchecker.core.sign2`: Network embedding of the similarity matrix derived from signatures type 1. These signatures have a fixed length (e.g. 128-d), which is convenient for machine learning, and capture both explicit *and* implicit similarity relationships in the data.
-    * **Signatures type 3** :class:`~chemicalchecker.core.sign3`: Fixed-length (e.g. 128-d) representation of the data, capturing *and* inferring the original (signature type 1) similarity of the data. Signatures type 3 are available for any molecule of interest and have a confidence measure assigned to them.
+    * **Signatures type 3** :class:`~chemicalchecker.core.sign3`: Fixed-length (e.g. 128-d) representation of the data, capturing *and* inferring the original (signature type 1) similarity of the data. Signatures type 3 are available for any molecule in the Chemical Checker universe (~1 Million) and have a confidence measure assigned to them.
+    * **Signatures type 4** :class:`~chemicalchecker.core.sign4`: Fixed-length (e.g. 128-d) representation of the data, inferring the signature type 3. Signatures type 4 are available for any molecule of interest and have a confidence measure assigned to them. Are convinently generated with the *signaturizer* tool.
 
 Besides, there are other auxiliary types of data that can be computed for each of the signature types. 
 
     * **Nearest neighbors** :class:`~chemicalchecker.core.neig`: Nearest neighbors search result. Currently, we consider the 1000-nearest neighbors, which is more than sufficient in any realistic scenario.
     * **Clusters** :class:`~chemicalchecker.core.clus`: Centroids and labels of a k-means clustering.
     * **2D Projections** :class:`~chemicalchecker.core.proj`: Various (t-SNE, UMAP, PCA) 2D projections of the data.
 
@@ -79,15 +80,15 @@
    2.  Network embedding (using :mod:`~chemicalchecker.tool.node2vec`).
 
 See implementation details in :mod:`~chemicalchecker.core.sign2`
 
 Signatures type 3
 '''''''''''''''''
 
-These signatures are fixed-length vectors available for *any* molecule of interest. Thus, they are mostly *inferred* properties.
+These signatures are fixed-length vectors available for all molecules of the Chemical Checker universe (~1 Million). Thus, they are mostly *inferred* properties.
 
 To learn signatures type 3:
 
 * Triplets are sampled from type 1 similarities
 * Signatures type 2 across the CC are used as input for a deep siamese neural network. Thus, 25 fixed-length vectors are stacked.
 * A signature-dropout (subsampling) procedure is applied to ensure that the data seen in the training set are *realistic*, meaning that the signature coverage resembles the coverage available for those molecules that do *not* have data available for the CC space in question.
 
@@ -109,8 +110,19 @@
   over these predictions indicate a robust output.
 * *Expectancy a priori*: We calculated the accuracy that is expected given the input signatures
   available for a particular molecule. Some CC signature types are highly predictive for others;
   thus, having these informative signatures at hand will in principle favor reliable predictions. This
   prior expectancy was calculated by fitting a random forest classifier having 25
   absence/presence features as covariates and prediction accuracy as outcome.
 
-See implementation details in :mod:`~chemicalchecker.core.sign3`
+See implementation details in :mod:`~chemicalchecker.core.sign3`
+
+
+Signatures type 4
+'''''''''''''''''
+
+These signatures are fixed-length vectors available for *any* molecule of interest. They are completely *inferred*.
+
+To learn signatures type 4:
+
+* A DNN for multi-output regression problem is trained to predict signatures type 3 from a simple ECFP4 (Morgan fingerprint) representation.
+* These signatures correspond to *signaturizer* produced signatures
```

### Comparing `chemicalchecker-1.0.2/docs/sources.rst` & `chemicalchecker-1.0.3/docs/sources.rst`

 * *Files identical despite different names*

### Comparing `chemicalchecker-1.0.2/setup.py` & `chemicalchecker-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 __author__ = """SBNB"""
 __email__ = 'sbnb@irbbarcelona.org'
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 requirements = [
     'numpy',
     'h5py',
     'psycopg2-binary',
     'pandas',
     'networkx',
     'autologging',
     'scipy',
     'sqlalchemy',
     'paramiko',
-    'sklearn',
+    'scikit-learn',
     'csvsort',
     'matplotlib<3.0',
     'seaborn',
     'tqdm',
 ]
 
 setup_requirements = ['pytest-runner']
@@ -33,15 +33,15 @@
     version=__version__,
     author=__author__,
     author_email=__email__,
     description="Chemical Checker Package.",
     long_description=open('README.rst').read().strip(),
     long_description_content_type='text/x-rst',
     url='http://gitlabsbnb.irbbarcelona.org/packages/chemical_checker',
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests","scripts","docs"]),
     install_requires=requirements,
     setup_requires=setup_requirements,
     tests_require=test_requirements,
     test_suite='tests',
     zip_safe=False,
     include_package_data=True,
     license="MIT License",
```

