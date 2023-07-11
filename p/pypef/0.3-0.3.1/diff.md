# Comparing `tmp/pypef-0.3.tar.gz` & `tmp/pypef-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypef-0.3.tar", last modified: Fri Jun 23 08:52:35 2023, max compression
+gzip compressed data, was "pypef-0.3.1.tar", last modified: Tue Jul 11 16:01:12 2023, max compression
```

## Comparing `pypef-0.3.tar` & `pypef-0.3.1.tar`

### file list

```diff
@@ -1,641 +1,641 @@
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:35.204268 pypef-0.3/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    20254 2022-07-09 09:31:17.000000 pypef-0.3/LICENSE.md
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       72 2022-07-09 09:31:17.000000 pypef-0.3/MANIFEST.in
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1285 2023-06-23 08:52:35.200769 pypef-0.3/PKG-INFO
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    28270 2023-06-21 09:33:59.000000 pypef-0.3/README.md
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:06.293491 pypef-0.3/pypef/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1002 2023-06-22 13:24:04.000000 pypef-0.3/pypef/__init__.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:06.645495 pypef-0.3/pypef/dca/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.3/pypef/dca/__init__.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5949 2023-06-21 12:24:22.000000 pypef-0.3/pypef/dca/dca_run.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    26612 2023-06-22 08:00:42.000000 pypef-0.3/pypef/dca/gremlin_inference.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    46823 2023-06-18 11:12:50.000000 pypef-0.3/pypef/dca/hybrid_model.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    31392 2023-06-15 16:19:10.000000 pypef-0.3/pypef/dca/plmc_encoding.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    23529 2023-06-13 19:31:08.000000 pypef-0.3/pypef/main.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:06.801492 pypef-0.3/pypef/ml/
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:33.124768 pypef-0.3/pypef/ml/AAindex/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      594 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ANDN920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ARGP820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ARGP820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ARGP820103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      489 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      836 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1161 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      664 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      945 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980118.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      470 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980119.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980120.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      818 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      704 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      639 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      512 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1186 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BAEK050101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2418 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BASU050101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2485 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BASU050102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2873 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BASU050103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      846 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BEGF750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      891 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BEGF750102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      649 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BEGF750103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BHAR880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1002 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BIGC670101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2753 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BIOV880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2581 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BIOV880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      949 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BLAM930101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1880 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BLAS910101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      790 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BROC820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BROC820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1419 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BULH740101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BULH740102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BUNA790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      543 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BUNA790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BUNA790103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      938 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BURA740101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BURA740102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2179 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CASG920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      977 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      993 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1021 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      755 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1069 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      546 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      697 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      968 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      518 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      978 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1042 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1264 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1659 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      913 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1066 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1273 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780201.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780202.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1011 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780203.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780204.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780205.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780206.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780207.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780208.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780209.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780210.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780211.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780212.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      733 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780213.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780214.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780215.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1099 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780216.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1844 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2110 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2479 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2440 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      439 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/COHE430101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1968 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1838 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2012 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2228 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2119 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/COSI940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1140 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/COWR900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CRAJ730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CRAJ730102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      825 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CRAJ730103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      780 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DAWD720101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1038 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DAYM780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DAYM780201.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1472 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DESM900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2134 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DESM900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DIGM050101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1899 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/EISD840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1471 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/EISD860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/EISD860102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1824 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/EISD860103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ENGD860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      444 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      447 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      435 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      454 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2291 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG890101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2454 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1053 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1328 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      931 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      766 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1169 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      767 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      657 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1142 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      865 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      721 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      843 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA910101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1071 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA910102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      827 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA910103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      802 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA910104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      537 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FODM020101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      995 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1276 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1256 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      759 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      823 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      807 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1000 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      826 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      936 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      610 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GARJ730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      902 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      490 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      882 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      923 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      681 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1165 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      529 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      962 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1098 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      592 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      754 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GOLD730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GOLD730102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      499 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GRAR740101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2266 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GRAR740102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      941 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GRAR740103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1884 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUOD860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2253 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1976 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1867 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1686 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1275 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1005 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HARY940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HOPA770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1453 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HOPT810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HUTJ700101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HUTJ700102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      646 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HUTJ700103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1307 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      706 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1171 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JACR890101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1346 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1885 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ780102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1582 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ780103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1240 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      897 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JOND750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      686 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JOND750102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      964 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JOND920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JOND920102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      887 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JUKT750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      842 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JUNJ780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2297 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JURD980101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1090 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KANM800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1397 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KANM800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1356 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KANM800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1078 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KANM800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      972 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARP850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1731 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARP850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARP850103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      536 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      532 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      526 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      528 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      559 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      563 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      547 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      567 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      622 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160118.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160119.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160120.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160121.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160122.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      458 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KHAG800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1837 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KIDA850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      611 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KIMC930101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      527 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KLEP840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KOEP990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KOEP990102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KRIW710101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2101 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KRIW790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1518 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KRIW790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KRIW790103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1615 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUHL950101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      808 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUMS000101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      871 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUMS000102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      557 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUMS000103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUMS000104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2155 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KYTJ820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LAWE840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1272 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1019 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      577 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1035 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1124 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      999 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      919 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      916 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1092 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      525 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEWP710101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1861 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LIFS790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      761 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LIFS790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1004 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LIFS790103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2391 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MANP780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1301 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      723 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      690 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      764 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MCMT640101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEEJ800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1236 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEEJ800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEEJ810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1431 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEEJ810102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2320 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEIH800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2423 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEIH800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2265 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEIH800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      548 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MITS020101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2621 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2635 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2617 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2726 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2703 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2552 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      839 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MONM990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MONM990201.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1157 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1128 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1631 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      845 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2035 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2556 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2296 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1688 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      822 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      888 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAGK730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      782 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAGK730102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      925 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAGK730103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      989 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      756 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      581 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      673 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      545 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      862 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      779 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      894 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      660 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      935 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2079 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NISK800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2601 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NISK860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1331 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NOZY710101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1313 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OLSK800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      880 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ONEK900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      927 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ONEK900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1871 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      672 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2350 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      588 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      973 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1298 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1060 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1362 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      966 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      638 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      599 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      878 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      875 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      598 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      898 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      621 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2385 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PARJ860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1697 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PARS000101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      724 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PARS000102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2257 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PLIV810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1028 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONJ960101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2346 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2238 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2244 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      550 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      909 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1315 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2169 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2388 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP930101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      579 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM820103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1575 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1115 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM900103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1269 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM900104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1271 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PTIO830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1637 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PTIO830102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2481 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PUNT030101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2221 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PUNT030102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      584 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      844 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1127 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1363 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      952 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      996 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      671 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      522 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880118.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1277 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880119.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1622 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880120.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880121.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880122.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880123.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880124.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880125.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880126.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880127.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880128.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880129.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880130.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      881 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880131.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1185 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880132.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1205 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880133.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880134.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1039 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880135.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880136.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880137.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880138.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880139.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1980 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2148 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS770102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1487 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS770103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1155 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      635 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1357 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1089 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      728 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      967 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1245 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2735 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      504 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      630 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1109 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      508 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1261 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      854 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1192 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1327 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      488 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      654 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      507 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      582 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1940 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1107 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSG850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2469 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSG850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1823 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      506 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1197 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2001 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880105.txt
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:34.729297 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_12_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_0_4.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_1_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_0_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_15_0_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_16_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_0_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_1_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_5_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_4_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_8_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_0_7.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_1_4.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1015 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SIMZ760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      456 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SNEP660101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      476 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SNEP660102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SNEP660103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SNEP660104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1158 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SUEM840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      684 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SUEM840102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      494 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SUYM030101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1839 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SWER830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1093 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TAKK010101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      821 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      669 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1100 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1036 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TSAJ990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1040 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TSAJ990102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VASM830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VASM830102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VASM830103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VELV850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1083 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VENT840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      974 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VHEG790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2392 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VINM940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2006 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VINM940102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1701 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VINM940103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      705 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VINM940104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1118 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WARP780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      679 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WEBA780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2230 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WERD780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WERD780102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WERD780103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      624 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WERD780104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WILM950101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WILM950102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      619 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WILM950103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WILM950104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      856 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WIMW960101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOEC730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1070 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLR790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1105 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLR810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2072 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLS870101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      749 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLS870102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLS870103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YANJ020101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YUTK870101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      685 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YUTK870102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YUTK870103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YUTK870104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZASB820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1677 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZHOH040101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1180 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZHOH040102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2314 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZHOH040103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      562 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.3/pypef/ml/__init__.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    10148 2023-06-22 08:25:04.000000 pypef-0.3/pypef/ml/ml_run.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5068 2022-07-02 13:59:04.000000 pypef-0.3/pypef/ml/parallelization.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    46544 2023-06-22 09:06:50.000000 pypef-0.3/pypef/ml/regression.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:35.170768 pypef-0.3/pypef/utils/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.3/pypef/utils/__init__.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    16959 2023-06-22 08:44:57.000000 pypef-0.3/pypef/utils/directed_evolution.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    16653 2023-06-05 11:31:37.000000 pypef-0.3/pypef/utils/learning_test_sets.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    19555 2023-06-08 12:17:07.000000 pypef-0.3/pypef/utils/low_n_mutation_extrapolation.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2238 2023-06-08 12:17:07.000000 pypef-0.3/pypef/utils/performance.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     3712 2023-06-14 07:07:14.000000 pypef-0.3/pypef/utils/plot.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    18580 2023-06-11 17:16:59.000000 pypef-0.3/pypef/utils/prediction_sets.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     4362 2023-06-22 08:26:56.000000 pypef-0.3/pypef/utils/sto2a2m.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1872 2023-06-08 12:17:07.000000 pypef-0.3/pypef/utils/to_file.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    17756 2023-06-22 09:31:05.000000 pypef-0.3/pypef/utils/utils_run.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    15786 2023-06-22 15:38:45.000000 pypef-0.3/pypef/utils/variant_data.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:06.423021 pypef-0.3/pypef.egg-info/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1285 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/PKG-INFO
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    21259 2023-06-23 08:52:06.000000 pypef-0.3/pypef.egg-info/SOURCES.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        1 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/dependency_links.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       46 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/entry_points.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      107 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/requires.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        6 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/top_level.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      117 2023-06-11 11:08:13.000000 pypef-0.3/requirements.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       38 2023-06-23 08:52:35.205300 pypef-0.3/setup.cfg
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2149 2023-06-22 14:53:59.000000 pypef-0.3/setup.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-07-11 16:01:12.622580 pypef-0.3.1/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    20254 2023-06-29 10:33:48.000000 pypef-0.3.1/LICENSE.md
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       72 2023-06-29 10:33:48.000000 pypef-0.3.1/MANIFEST.in
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1308 2023-07-11 16:01:12.620581 pypef-0.3.1/PKG-INFO
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    28651 2023-07-11 11:27:25.000000 pypef-0.3.1/README.md
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-07-11 16:00:49.450941 pypef-0.3.1/pypef/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1004 2023-07-11 11:18:15.000000 pypef-0.3.1/pypef/__init__.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-07-11 16:00:49.719941 pypef-0.3.1/pypef/dca/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/dca/__init__.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     6092 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/dca/dca_run.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    26838 2023-07-11 11:18:15.000000 pypef-0.3.1/pypef/dca/gremlin_inference.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    46545 2023-07-11 11:18:15.000000 pypef-0.3.1/pypef/dca/hybrid_model.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    31535 2023-07-11 11:18:15.000000 pypef-0.3.1/pypef/dca/plmc_encoding.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    23965 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/main.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-07-11 16:00:49.842947 pypef-0.3.1/pypef/ml/
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-07-11 16:01:11.047235 pypef-0.3.1/pypef/ml/AAindex/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      594 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ANDN920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ARGP820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ARGP820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ARGP820103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      489 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      836 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1161 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      664 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      945 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980118.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      470 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980119.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AURR980120.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AVBF000101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      818 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AVBF000102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AVBF000103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      704 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AVBF000104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      639 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AVBF000105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AVBF000106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AVBF000107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AVBF000108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      512 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/AVBF000109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1186 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BAEK050101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2418 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BASU050101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2485 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BASU050102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2873 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BASU050103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      846 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BEGF750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      891 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BEGF750102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      649 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BEGF750103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BHAR880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1002 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BIGC670101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2753 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BIOV880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2581 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BIOV880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      949 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BLAM930101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1880 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BLAS910101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      790 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BROC820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BROC820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1419 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BULH740101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BULH740102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BUNA790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      543 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BUNA790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BUNA790103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      938 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BURA740101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/BURA740102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2179 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CASG920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      977 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CEDJ970101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CEDJ970102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      993 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CEDJ970103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1021 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CEDJ970104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      755 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CEDJ970105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1069 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM830102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      546 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM830103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM830104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      697 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM830105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      968 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM830106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      518 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM830107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHAM830108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      978 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOC750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1042 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOC760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1264 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOC760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1659 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOC760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      913 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOC760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1066 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1273 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780201.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780202.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1011 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780203.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780204.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780205.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780206.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780207.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780208.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780209.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780210.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780211.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780212.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      733 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780213.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780214.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780215.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1099 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CHOP780216.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1520 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CIDH920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1844 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CIDH920102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2110 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CIDH920103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2479 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CIDH920104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2440 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CIDH920105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      439 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/COHE430101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CORJ870101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CORJ870102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1968 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CORJ870103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1838 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CORJ870104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CORJ870105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2012 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CORJ870106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2228 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CORJ870107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2119 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CORJ870108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/COSI940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1140 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/COWR900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CRAJ730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CRAJ730102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      825 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/CRAJ730103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      780 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/DAWD720101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1038 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/DAYM780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/DAYM780201.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1472 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/DESM900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2134 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/DESM900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/DIGM050101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1899 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/EISD840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1471 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/EISD860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/EISD860102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1824 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/EISD860103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ENGD860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FASG760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      444 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FASG760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      447 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FASG760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      435 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FASG760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      454 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FASG760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2291 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FASG890101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2454 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1053 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1328 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      931 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      766 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1169 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      767 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      657 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1142 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      865 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      721 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FAUJ880113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FINA770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      843 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FINA910101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1071 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FINA910102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      827 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FINA910103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      802 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FINA910104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      537 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FODM020101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      995 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1276 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1256 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      759 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      823 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      807 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1000 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      826 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      936 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/FUKS010112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      610 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GARJ730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      902 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      490 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      882 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      923 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      681 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1165 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      529 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      962 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1098 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEIM800111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      592 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEOR030101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEOR030102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEOR030103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEOR030104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEOR030105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEOR030106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEOR030107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEOR030108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      754 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GEOR030109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GOLD730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GOLD730102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      499 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GRAR740101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2266 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GRAR740102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      941 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GRAR740103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1884 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GUOD860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2253 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GUYH850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1976 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GUYH850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1867 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GUYH850103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1686 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GUYH850104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1275 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/GUYH850105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1005 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/HARY940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/HOPA770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1453 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/HOPT810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/HUTJ700101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/HUTJ700102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      646 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/HUTJ700103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1307 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ISOY800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      706 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ISOY800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ISOY800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ISOY800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ISOY800105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ISOY800106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ISOY800107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ISOY800108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1171 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JACR890101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1346 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JANJ780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1885 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JANJ780102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1582 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JANJ780103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1240 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JANJ790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JANJ790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      897 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JOND750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      686 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JOND750102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      964 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JOND920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JOND920102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      887 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JUKT750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      842 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JUNJ780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2297 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/JURD980101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1090 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KANM800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1397 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KANM800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1356 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KANM800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1078 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KANM800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      972 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARP850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1731 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARP850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARP850103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      536 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      532 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      526 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      528 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      559 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      563 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      547 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      567 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      622 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160118.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160119.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160120.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160121.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KARS160122.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      458 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KHAG800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1837 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KIDA850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      611 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KIMC930101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      527 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KLEP840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KOEP990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KOEP990102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KRIW710101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2101 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KRIW790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1518 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KRIW790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KRIW790103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1615 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KUHL950101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      808 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KUMS000101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      871 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KUMS000102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      557 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KUMS000103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KUMS000104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2155 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/KYTJ820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LAWE840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1272 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1019 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      577 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1035 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1124 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM760106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      999 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM760107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      919 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM780102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM780103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM780104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      916 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM780105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1092 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEVM780106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      525 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LEWP710101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1861 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LIFS790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      761 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LIFS790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1004 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/LIFS790103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2391 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MANP780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1301 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MAXF760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      723 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MAXF760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MAXF760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MAXF760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      690 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MAXF760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MAXF760106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      764 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MCMT640101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MEEJ800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1236 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MEEJ800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MEEJ810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1431 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MEEJ810102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2320 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MEIH800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2423 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MEIH800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2265 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MEIH800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      548 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MITS020101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2621 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MIYS850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2635 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MIYS990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2617 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MIYS990102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2726 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MIYS990103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2703 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MIYS990104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2552 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MIYS990105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      839 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MONM990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MONM990201.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1157 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MUNV940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1128 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MUNV940102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1631 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MUNV940103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MUNV940104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      845 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/MUNV940105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2035 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NADH010101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NADH010102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2556 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NADH010103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2296 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NADH010104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1688 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NADH010105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      822 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NADH010106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NADH010107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      888 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAGK730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      782 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAGK730102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      925 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAGK730103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      989 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      756 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      581 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      673 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      545 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      862 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      779 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH900113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      894 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      660 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH920102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH920103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH920104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH920105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      935 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH920106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH920107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NAKH920108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2079 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NISK800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2601 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NISK860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1331 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/NOZY710101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1313 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OLSK800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      880 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ONEK900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      927 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ONEK900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1871 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      672 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM770102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2350 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM770103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM770104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM770105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      588 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM850103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM850104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/OOBM850105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      973 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1298 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1060 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1362 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      966 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      638 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      599 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      878 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      875 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      598 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      898 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      621 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PALJ810116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2385 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PARJ860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1697 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PARS000101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      724 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PARS000102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2257 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PLIV810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1028 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONJ960101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2346 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONP800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2238 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONP800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2244 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONP800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONP800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      550 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONP800105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      909 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONP800106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1315 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONP800107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2169 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONP800108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2388 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PONP930101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PRAM820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      579 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PRAM820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PRAM820103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1575 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PRAM900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1115 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PRAM900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PRAM900103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1269 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PRAM900104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1271 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PTIO830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1637 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PTIO830102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2481 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PUNT030101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2221 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/PUNT030102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      584 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      844 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1127 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1363 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      952 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      996 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      671 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      522 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880118.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1277 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880119.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1622 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880120.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1450 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880121.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880122.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880123.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880124.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880125.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880126.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880127.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880128.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880129.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880130.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      881 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880131.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1185 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880132.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1205 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880133.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880134.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1039 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880135.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880136.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880137.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880138.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/QIAN880139.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1980 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2148 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS770102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1487 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS770103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1155 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      635 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RACS820114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RADA880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1357 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RADA880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1089 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RADA880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RADA880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      728 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RADA880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      967 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RADA880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1245 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RADA880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2735 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RADA880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      504 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      630 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/RICJ880117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1109 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      508 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1261 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      854 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1192 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1327 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      488 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      654 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      507 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      582 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB760113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1940 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROBB790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1107 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROSG850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2469 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROSG850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROSM880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1823 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROSM880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      506 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROSM880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1197 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROSM880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2001 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ROSM880105.txt
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-07-11 16:01:12.270400 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_12_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_0_4.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_1_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_0_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_15_0_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_16_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_0_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_1_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_5_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_4_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_8_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_0_7.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_1_4.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1015 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/SIMZ760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      456 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/SNEP660101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      476 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/SNEP660102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/SNEP660103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/SNEP660104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1158 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/SUEM840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      684 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/SUEM840102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      494 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/SUYM030101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1839 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/SWER830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1093 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TAKK010101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      821 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      669 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1100 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TANS770110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1036 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TSAJ990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1040 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/TSAJ990102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VASM830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VASM830102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VASM830103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VELV850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1083 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VENT840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      974 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VHEG790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2392 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VINM940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2006 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VINM940102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1701 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VINM940103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      705 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/VINM940104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1118 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WARP780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      679 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WEBA780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2230 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WERD780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WERD780102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WERD780103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      624 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WERD780104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WILM950101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WILM950102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      619 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WILM950103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WILM950104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      856 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WIMW960101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WOEC730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1070 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WOLR790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1105 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WOLR810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2072 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WOLS870101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      749 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WOLS870102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/WOLS870103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/YANJ020101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/YUTK870101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      685 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/YUTK870102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/YUTK870103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/YUTK870104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ZASB820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1677 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ZHOH040101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1180 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ZHOH040102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2314 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ZHOH040103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ZIMJ680101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ZIMJ680102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ZIMJ680103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      562 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ZIMJ680104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/AAindex/ZIMJ680105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/__init__.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    10342 2023-07-11 11:18:15.000000 pypef-0.3.1/pypef/ml/ml_run.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5204 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/ml/parallelization.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    47000 2023-07-11 11:18:15.000000 pypef-0.3.1/pypef/ml/regression.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-07-11 16:01:12.594545 pypef-0.3.1/pypef/utils/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/utils/__init__.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    16931 2023-07-11 11:18:15.000000 pypef-0.3.1/pypef/utils/directed_evolution.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    16653 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/utils/learning_test_sets.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    19902 2023-07-11 11:18:15.000000 pypef-0.3.1/pypef/utils/low_n_mutation_extrapolation.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2238 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/utils/performance.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     3712 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/utils/plot.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    18580 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/utils/prediction_sets.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     4362 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/utils/sto2a2m.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1872 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/utils/to_file.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    17756 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/utils/utils_run.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    15786 2023-06-29 10:32:53.000000 pypef-0.3.1/pypef/utils/variant_data.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-07-11 16:00:49.570941 pypef-0.3.1/pypef.egg-info/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1308 2023-07-11 16:00:42.000000 pypef-0.3.1/pypef.egg-info/PKG-INFO
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    21259 2023-07-11 16:00:49.000000 pypef-0.3.1/pypef.egg-info/SOURCES.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        1 2023-07-11 16:00:42.000000 pypef-0.3.1/pypef.egg-info/dependency_links.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       46 2023-07-11 16:00:42.000000 pypef-0.3.1/pypef.egg-info/entry_points.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      107 2023-07-11 16:00:42.000000 pypef-0.3.1/pypef.egg-info/requires.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        6 2023-07-11 16:00:42.000000 pypef-0.3.1/pypef.egg-info/top_level.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      117 2023-06-29 10:33:48.000000 pypef-0.3.1/requirements.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       38 2023-07-11 16:01:12.623581 pypef-0.3.1/setup.cfg
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2221 2023-07-11 11:22:59.000000 pypef-0.3.1/setup.py
```

### Comparing `pypef-0.3/LICENSE.md` & `pypef-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pypef-0.3/PKG-INFO` & `pypef-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pypef
-Version: 0.3
+Version: 0.3.1
 Summary: A command-line interface (CLI) tool for performing data-driven protein engineering by building machine learning (ML)-trained regression models from sequence variant fitness data (in CSV format) based on different techniques for protein sequence encoding. Next to building pure ML models, 'hybrid modeling' is also possible using a blended model optimized for predictive contributions of a statistical and an ML-based prediction.
-Home-page: https://github.com/niklases/PyPEF
+Home-page: https://github.com/Protein-Engineering-Framework/PyPEF
 Author: Niklas Siedhoff & Alexander-Maurice Illig
 Author-email: n.siedhoff@biotec.rwth-aachen.de
 License: CC BY-NC-SA 4.0
 Keywords: Pythonic Protein Engineering Framework
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypef-0.3/README.md` & `pypef-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 - [Preprocessing for DCA-based Sequence Encoding](#dca-preprocessing)
 - [API Usage for Sequence Encoding](#api-usage)
 ---
 
 <a name="pypef"></a>
 # PyPEF: Pythonic Protein Engineering Framework
 [![PyPI version](https://img.shields.io/pypi/v/PyPEF?color=blue)](https://pypi.org/project/pypef/)
-[![Python version](https://img.shields.io/pypi/pyversions/PyPEF)](https://pypi.org/project/pypef/)
+[![Python version](https://img.shields.io/pypi/pyversions/PyPEF)](https://www.python.org/downloads/)
 
 a framework written in Python 3 for performing sequence-based machine learning-assisted protein engineering to predict a protein's fitness from its sequence using different forms of sequence encoding:
 - One-hot encoding
 - Amino acid descriptor sets (taken from AAindex database) encoding
 - Direct coupling analysis (amino acid coevolution based on multiple sequence alignments) encoding
 
 Written by Niklas Siedhoff and Alexander-Maurice Illig.
@@ -56,27 +56,28 @@
 The workflow procedure is explained in the [Jupyter notebook](/workflow/Workflow_PyPEF.ipynb) (.ipynb) protocol (see
 Tutorial section below).
 
 <img src="workflow/Splitting_Workflow.png" alt="drawing" width="1000"/>
 
 <a name="installation"></a>
 ## Quick Installation
-A quick installation of the PyPEF command line framework using PyPI for Linux and Windows for **Python 3.9** can be performed with:
+A quick installation of the PyPEF command line framework using PyPI for Linux and Windows for **Python 3.10** can be performed with:
 
 ```
 pip install -U pypef
 ```
 
 After successful installation, PyPEF should work by calling `pypef` in the shell:
 
 ```
 pypef --help
 ```
 
 The detailed routine for setting up a new virtual environment with Anaconda, installing the necessary Python packages for that environment, and running the Jupyter notebook tutorial can be found below in the Tutorial section.
+For Linux users, a quick file setup and CLI run test can be performed running [/workflow/easy_install_test.sh](/workflow/easy_install_test.sh) in Bash (requires conda, i.e. Miniconda3 or Anaconda3).
 
 <a name="requirements"></a>
 ## Requirements
 - Python >=3.9
     - numpy 
     - scipy
     - pandas
@@ -198,42 +199,42 @@
 Sample files for testing PyPEF routines are provided in the workflow directory, which are also used when running the notebook tutorial. PyPEF's package dependencies are linked [here](https://github.com/niklases/PyPEF/network/dependencies).
 Further, for designing your own API based on the PyPEF workflow, modules can be adapted from the [source code](/pypef).
 
 As standard input files, PyPEF requires the target protein wild-type sequence in [FASTA](https://en.wikipedia.org/wiki/FASTA) format and variant-fitness data in [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) format to split the collected variant-fitness data in learning and test sets that resemble the aligned FASTA format and additionally contain lines indicating the fitness of each corresponding variant (see [ANEH sample files](workflow/test_dataset_aneh), [avGFP sample files](workflow/test_dataset_avgfp), and [MERGE SSM & DMS files](https://github.com/Protein-Engineering-Framework/MERGE/tree/main/Data/_variant_fitness_wtseq)).
 
 <a name="tutorial"></a>
 ## Tutorial
-Before starting running the tutorial, it is a good idea to set up a new Python environment using Anaconda, https://www.anaconda.com/, e.g. using [Anaconda](https://www.anaconda.com/products/individual) ([Anaconda3-2020.11-Linux-x86_64.sh installer download](https://repo.anaconda.com/archive/Anaconda3-2020.11-Linux-x86_64.sh)) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
+Before starting running the tutorial, it is a good idea to set up a new Python environment using Anaconda, https://www.anaconda.com/, e.g. using [Anaconda](https://www.anaconda.com/download#downloads) ([Anaconda3-2023.03-1-Linux-x86_64.sh installer download](https://repo.anaconda.com/archive/Anaconda3-2023.03-1-Linux-x86_64.sh)) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
 Change to the download directory and run the installation, e.g. in Linux:
 
 ```
-bash Anaconda3-2020.11-Linux-x86_64.sh
+bash Anaconda3-2023.03-1-Linux-x86_64.sh
 ```
 
 After accepting all steps, the conda setup should also be written to your `~/.bashrc`file, so that you can call anaconda typing `conda`.
-Next, to download this repository click Code > Download ZIP and unzip the zipped file, e.g. with `unzip PyPEF-main.zip`, or just clone this repository using your bash shell to your local machine `git clone https://github.com/niklases/PyPEF`.
-To setup a new environment with conda you can either create the conda environment from the provided YAML file inside the PyPEF directory (`cd PyPEF` or `cd PyPEF-main` dependent on the downloaded file name and chose YAML file for your operating system):
+Next, to download this repository click Code > Download ZIP and unzip the zipped file, e.g. with `unzip PyPEF-master.zip`, or just clone this repository using your bash shell to your local machine `git clone https://github.com/niklases/PyPEF`.
+To set up a new environment with conda you can either create the conda environment from the provided YAML file inside the PyPEF directory (`cd PyPEF` or `cd PyPEF-master` dependent on the downloaded file name and chose YAML file for your operating system):
 
 ```
 conda env create --file linux_env.yml
 ```
 
 or you can create a new environment yourself. You just need to specify the name of the environment and the Python version, e.g.:
 
 ```
-conda create --name pypef python=3.9
+conda create --name pypef python=3.10
 ```
 
 To activate the environment you can define:
 
 ```
 conda activate pypef
 ```
 
-After activating the environment you can install required packages after changing the directory to the PyPEF directory (`cd PyPEF` or `cd PyPEF-main`) and install required packages with pip if you did not use the YAML file for creating the environment (if using conda, packages will be installed in anaconda3/envs/pypef/lib/python3.9/site-packages):
+After activating the environment you can install required packages after changing the directory to the PyPEF directory (`cd PyPEF` or `cd PyPEF-master`) and install required packages with pip if you did not use the YAML file for creating the environment (if using conda, packages will be installed in anaconda3/envs/pypef/lib/python3.10/site-packages):
 
 ```
 python3 -m pip install -r requirements.txt
 ```
 
 Note that the package [Ray](https://github.com/ray-project/ray) which we use for parallelizing sequence encoding and model validation of AAindices on the test set, is in beta status for [Windows](https://docs.ray.io/en/latest/installation.html#windows-support).
 
@@ -307,44 +308,44 @@
 | MLP | single hidden layer size = {1, 2, ..., 12},<br>solver = {ADAM, L-BFGS},<br>initial learning rate = {0.001, 0.01, 0.1} |
 
 <a name="set-up"></a>
 ## Setting Up the Scripts Yourself
 PyPEF was developed to be run from a command-line interface while `python3 ./pypef/main.py` (when using the downloaded version of this repository and setting the `PYTHONPATH`) is equal to `pypef` when installed with pip. 
 Downloading/cloning the repository files (manually or with `wget`/`git clone`):<br>
 ```
-wget https://github.com/niklases/PyPEF/archive/main.zip
+wget https://github.com/Protein-Engineering-Framework/PyPEF/archive/refs/heads/master.zip
 ```
 
 Unzipping the zipped file (manually or e.g. with `unzip`):
 ```
-unzip main.zip
+unzip master.zip
 ```
 
 Setting the `PYTHONPATH` (so that no import errors occur stating that the package `pypef` and thus dependent absolute imports are unknown):<br>
 &nbsp;&nbsp;Windows (example path, PowerShell)
 ```
-$env:PYTHONPATH="C:\Users\name\path\to\PyPEF-main"
+$env:PYTHONPATH="C:\Users\name\path\to\PyPEF-master"
 ```
 
 &nbsp;&nbsp;Linux (example path)
 ```
-export PYTHONPATH="${PYTHONPATH}:/home/name/path/to/PyPEF-main"
+export PYTHONPATH="${PYTHONPATH}:/home/name/path/to/PyPEF-master"
 ```
 Installing the requirements:<br>
 &nbsp;&nbsp;Windows (PowerShell)
 ```
 python -m pip install -r requirements.txt
 ```
 
 &nbsp;&nbsp;Linux
 ```
 python3 -m pip install -r requirements.txt
 ```
 
-Running the main script (from PyPEF-main directory):<br>
+Running the main script (from PyPEF-master directory):<br>
 &nbsp;&nbsp;Windows (PowerShell)
 ```
 python .\pypef\main.py
 ```
 
 &nbsp;&nbsp;Linux
 ```
@@ -401,12 +402,12 @@
     Or for hybrid modeling:
     ```
     pypef hybrid -l LS.fasl -t TS.fasl --params ANEH_72.6.params
     ```
 
 <a name="api-usage"></a>
 ## API Usage for Sequence Encoding
-For script-based encoding of sequences using PyPEF and the available AAindex-, OneHot- or DCA-based techniques, the classes and corresponding functions can be imported, i.e. `OneHotEncoding`, `AAIndexEncoding`, `GREMLIN` (DCA),  `PLMC` (DCA), and `DCAHybridModel`. In addition, implemented functions for CV-based tuning of regression models can be used to train and validate models, eventually deriving them to obtain performances on retained data for testing. An exemplary script for CV-based (low-*N*) tuning of models and using them for testing is provided at [workflow/api_encoding_train_test.py](workflow/api_encoding_train_test.py).
+For script-based encoding of sequences using PyPEF and the available AAindex-, OneHot- or DCA-based techniques, the classes and corresponding functions can be imported, i.e. `OneHotEncoding`, `AAIndexEncoding`, `GREMLIN` (DCA),  `PLMC` (DCA), and `DCAHybridModel`. In addition, implemented functions for CV-based tuning of regression models can be used to train and validate models, eventually deriving them to obtain performances on retained data for testing. An exemplary script and a Jupyter notebook for CV-based (low-*N*) tuning of models and using them for testing is provided at [workflow/api_encoding_train_test.py](workflow/api_encoding_train_test.py) and [workflow/api_encoding_train_test.ipynb](workflow/api_encoding_train_test.ipynb), respectively.
 
 <p align="center">
     <img src="workflow/low_N_avGFP_extrapolation.png" alt="drawing" width="500"/>
 </p>
```

### Comparing `pypef-0.3/pypef/__init__.py` & `pypef-0.3.1/pypef/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
 
-__version__ = '0.3-alpha'
+__version__ = '0.3.1-alpha'
```

### Comparing `pypef-0.3/pypef/dca/dca_run.py` & `pypef-0.3.1/pypef/dca/dca_run.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Created on 05 October 2020
-# @authors: Niklas Siedhoff, Alexander-Maurice Illig
-# @contact: <n.siedhoff@biotec.rwth-aachen.de>
-# PyPEF - Pythonic Protein Engineering Framework
-# Released under Creative Commons Attribution-NonCommercial 4.0 International Public License (CC BY-NC 4.0)
-# For more information about the license see https://creativecommons.org/licenses/by-nc/4.0/legalcode
-
-# PyPEF – An Integrated Framework for Data-Driven Protein Engineering
-# Journal of Chemical Information and Modeling, 2021, 61, 3463-3476
-# https://doi.org/10.1021/acs.jcim.1c00099
-# Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
-# 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
-# 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
-# *Corresponding author
-# §Equal contribution
-
-import logging
-logger = logging.getLogger('pypef.dca.dca_run')
-import ray
-
-from pypef.utils.variant_data import read_csv, get_wt_sequence
-from pypef.dca.plmc_encoding import save_plmc_dca_encoding_model
-from pypef.dca.hybrid_model import get_model_and_type, performance_ls_ts, predict_ps, generate_model_and_save_pkl
-from pypef.dca.gremlin_inference import save_gremlin_as_pickle, save_corr_csv, plot_all_corr_mtx
-from pypef.utils.low_n_mutation_extrapolation import performance_mutation_extrapolation, low_n
-
-
-def run_pypef_hybrid_modeling(arguments):
-    threads = abs(arguments['--threads']) if arguments['--threads'] is not None else 1
-    threads = threads + 1 if threads == 0 else threads
-    try:
-        _, model_type = get_model_and_type(arguments['--params'], arguments['--mutation_sep'])
-    except TypeError:
-        model_type = 'undefined'
-    except SystemError:
-        model_type = 'undefined'
-    if model_type in ['GREMLIN', 'DCAHybridModel'] and threads > 1:
-        logger.info(f'No (Ray) parallelization for {model_type} model...')
-    elif model_type not in ['GREMLIN', 'DCAHybridModel'] and threads > 1:
-        ray.init()
-        logger.info(f'Using {threads} threads for running...')
-    if model_type == 'DCAHybridModel':
-        logger.info(
-            f"Note that the hybrid model only optimizes model performances in terms of "
-            f"Spearman's correlation of measured versus predicted values. Further, the "
-            f"hybrid approach uses only Ridge regression for supervised ML-based hybrid "
-            f"model contribution. In hybrid modeling, the ranks of predictions are "
-            f"important and not the exact predicted value."
-        )
-
-    if arguments['--ts']:
-        performance_ls_ts(
-            ls_fasta=arguments['--ls'],
-            ts_fasta=arguments['--ts'],
-            threads=threads,
-            params_file=arguments['--params'],
-            model_pickle_file=arguments['--model'],
-            substitution_sep=arguments['--mutation_sep'],
-            label=arguments['--label']
-        )
-
-    elif arguments['--params'] and arguments['--model']:
-        prediction_dict = {}
-        prediction_dict.update({
-            'drecomb': arguments['--drecomb'],
-            'trecomb': arguments['--trecomb'],
-            'qarecomb': arguments['--qarecomb'],
-            'qirecomb': arguments['--qirecomb'],
-            'ddiverse': arguments['--ddiverse'],
-            'tdiverse': arguments['--tdiverse'],
-            'qdiverse': arguments['--qdiverse']
-        })
-
-        predict_ps(
-            prediction_dict=prediction_dict,
-            params_file=arguments['--params'],
-            threads=threads,
-            separator=arguments['--mutation_sep'],
-            model_pickle_file=arguments['--model'],
-            prediction_set=arguments['--ps'],
-            negative=arguments['--negative']
-        )
-
-    elif arguments['train_and_save']:
-        variants, fitnesses, _ = read_csv(arguments['--input'])
-        generate_model_and_save_pkl(
-            variants=variants,
-            ys_true=fitnesses,
-            params_file=arguments['--params'],
-            wt=arguments['--wt'],
-            train_percent_fit=arguments['--fit_size'],
-            test_percent=arguments['--test_size'],
-            random_state=arguments['--rnd_state'],
-            substitution_sep=arguments['--mutation_sep'],
-            threads=arguments['--threads']
-        )
-
-    elif arguments['low_n'] or arguments['extrapolation']:
-        if arguments['low_n']:
-            low_n(
-                encoded_csv=arguments['--input'],
-                hybrid_modeling=arguments['hybrid']
-            )
-        elif arguments['extrapolation']:
-            performance_mutation_extrapolation(
-                encoded_csv=arguments['--input'],
-                cv_regressor=arguments['--regressor'],
-                conc=arguments['--conc'],
-                hybrid_modeling=arguments['hybrid']
-            )
-
-    elif arguments['param_inference']:
-        if arguments['--msa']:
-            save_gremlin_as_pickle(
-                alignment=arguments['--msa'],
-                wt_seq=get_wt_sequence(arguments['--wt']),
-                opt_iter=arguments['--opt_iter']
-            )
-        elif arguments['--params']:
-            save_plmc_dca_encoding_model(
-                params_file=arguments['--params'],
-                substitution_sep=arguments['--mutation_sep']
-            )
-
-    elif arguments['save_msa_info']:
-        gremlin = save_gremlin_as_pickle(
-            alignment=arguments['--msa'],
-            wt_seq=get_wt_sequence(arguments['--wt']),
-            opt_iter=arguments['--opt_iter']
-        )
-        save_corr_csv(gremlin)
-        plot_all_corr_mtx(gremlin)
-
-    else:
-        performance_ls_ts(
-            ls_fasta=arguments['--ls'],
-            ts_fasta=arguments['--ts'],
-            threads=threads,
-            params_file=arguments['--params'],
-            substitution_sep=arguments['--mutation_sep']
-        )
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+# Created on 05 October 2020
+# @authors: Niklas Siedhoff, Alexander-Maurice Illig
+# @contact: <n.siedhoff@biotec.rwth-aachen.de>
+# PyPEF - Pythonic Protein Engineering Framework
+# Released under Creative Commons Attribution-NonCommercial 4.0 International Public License (CC BY-NC 4.0)
+# For more information about the license see https://creativecommons.org/licenses/by-nc/4.0/legalcode
+
+# PyPEF – An Integrated Framework for Data-Driven Protein Engineering
+# Journal of Chemical Information and Modeling, 2021, 61, 3463-3476
+# https://doi.org/10.1021/acs.jcim.1c00099
+# Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
+# 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
+# 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
+# *Corresponding author
+# §Equal contribution
+
+import logging
+logger = logging.getLogger('pypef.dca.dca_run')
+import ray
+
+from pypef.utils.variant_data import read_csv, get_wt_sequence
+from pypef.dca.plmc_encoding import save_plmc_dca_encoding_model
+from pypef.dca.hybrid_model import get_model_and_type, performance_ls_ts, predict_ps, generate_model_and_save_pkl
+from pypef.dca.gremlin_inference import save_gremlin_as_pickle, save_corr_csv, plot_all_corr_mtx
+from pypef.utils.low_n_mutation_extrapolation import performance_mutation_extrapolation, low_n
+
+
+def run_pypef_hybrid_modeling(arguments):
+    threads = abs(arguments['--threads']) if arguments['--threads'] is not None else 1
+    threads = threads + 1 if threads == 0 else threads
+    try:
+        _, model_type = get_model_and_type(arguments['--params'], arguments['--mutation_sep'])
+    except TypeError:
+        model_type = 'undefined'
+    except SystemError:
+        model_type = 'undefined'
+    if model_type in ['GREMLIN', 'DCAHybridModel'] and threads > 1:
+        logger.info(f'No (Ray) parallelization for {model_type} model...')
+    elif model_type not in ['GREMLIN', 'DCAHybridModel'] and threads > 1:
+        ray.init()
+        logger.info(f'Using {threads} threads for running...')
+    if model_type == 'DCAHybridModel':
+        logger.info(
+            f"Note that the hybrid model only optimizes model performances in terms of "
+            f"Spearman's correlation of measured versus predicted values. Further, the "
+            f"hybrid approach uses only Ridge regression for supervised ML-based hybrid "
+            f"model contribution. In hybrid modeling, the ranks of predictions are "
+            f"important and not the exact predicted value."
+        )
+
+    if arguments['--ts']:
+        performance_ls_ts(
+            ls_fasta=arguments['--ls'],
+            ts_fasta=arguments['--ts'],
+            threads=threads,
+            params_file=arguments['--params'],
+            model_pickle_file=arguments['--model'],
+            substitution_sep=arguments['--mutation_sep'],
+            label=arguments['--label']
+        )
+
+    elif arguments['--params'] and arguments['--model']:
+        prediction_dict = {}
+        prediction_dict.update({
+            'drecomb': arguments['--drecomb'],
+            'trecomb': arguments['--trecomb'],
+            'qarecomb': arguments['--qarecomb'],
+            'qirecomb': arguments['--qirecomb'],
+            'ddiverse': arguments['--ddiverse'],
+            'tdiverse': arguments['--tdiverse'],
+            'qdiverse': arguments['--qdiverse']
+        })
+
+        predict_ps(
+            prediction_dict=prediction_dict,
+            params_file=arguments['--params'],
+            threads=threads,
+            separator=arguments['--mutation_sep'],
+            model_pickle_file=arguments['--model'],
+            prediction_set=arguments['--ps'],
+            negative=arguments['--negative']
+        )
+
+    elif arguments['train_and_save']:
+        variants, fitnesses, _ = read_csv(arguments['--input'])
+        generate_model_and_save_pkl(
+            variants=variants,
+            ys_true=fitnesses,
+            params_file=arguments['--params'],
+            wt=arguments['--wt'],
+            train_percent_fit=arguments['--fit_size'],
+            test_percent=arguments['--test_size'],
+            random_state=arguments['--rnd_state'],
+            substitution_sep=arguments['--mutation_sep'],
+            threads=arguments['--threads']
+        )
+
+    elif arguments['low_n'] or arguments['extrapolation']:
+        if arguments['low_n']:
+            low_n(
+                encoded_csv=arguments['--input'],
+                hybrid_modeling=arguments['hybrid']
+            )
+        elif arguments['extrapolation']:
+            performance_mutation_extrapolation(
+                encoded_csv=arguments['--input'],
+                cv_regressor=arguments['--regressor'],
+                conc=arguments['--conc'],
+                hybrid_modeling=arguments['hybrid']
+            )
+
+    elif arguments['param_inference']:
+        if arguments['--msa']:
+            save_gremlin_as_pickle(
+                alignment=arguments['--msa'],
+                wt_seq=get_wt_sequence(arguments['--wt']),
+                opt_iter=arguments['--opt_iter']
+            )
+        elif arguments['--params']:
+            save_plmc_dca_encoding_model(
+                params_file=arguments['--params'],
+                substitution_sep=arguments['--mutation_sep']
+            )
+
+    elif arguments['save_msa_info']:
+        gremlin = save_gremlin_as_pickle(
+            alignment=arguments['--msa'],
+            wt_seq=get_wt_sequence(arguments['--wt']),
+            opt_iter=arguments['--opt_iter']
+        )
+        save_corr_csv(gremlin)
+        plot_all_corr_mtx(gremlin)
+
+    else:
+        performance_ls_ts(
+            ls_fasta=arguments['--ls'],
+            ts_fasta=arguments['--ts'],
+            threads=threads,
+            params_file=arguments['--params'],
+            substitution_sep=arguments['--mutation_sep']
+        )
```

### Comparing `pypef-0.3/pypef/dca/gremlin_inference.py` & `pypef-0.3.1/pypef/dca/gremlin_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,26 +78,29 @@
         self.gap_cutoff = gap_cutoff
         self.eff_cutoff = eff_cutoff
         self.opt_iter = opt_iter
         self.states = len(self.char_alphabet)
         self.a2n = self.a2n_dict()
         self.seqs, _, _ = get_sequences_from_file(alignment)
         self.msa_ori = self.get_msa_ori()
+        self.n_col_ori = self.msa_ori.shape[1]
         if wt_seq is not None:
             self.wt_seq = wt_seq
         else:  # Taking the first sequence in the MSA as wild type sequence
             logger.info("No wild-type sequence provided: The first sequence "
                         "in the MSA is considered the wild-type sequence.")
             self.wt_seq = "".join([self.char_alphabet[i] for i in self.msa_ori[0]])
+        if len(self.wt_seq) != self.n_col_ori:
+            raise SystemError("Length of (provided) wild-type sequence does not match "
+                              "number of MSA columns, i.e., common MSA sequence length.")
         self.msa_trimmed, self.v_idx, self.w_idx, self.w_rel_idx, self.gaps = self.filt_gaps(self.msa_ori)
         self.msa_weights = self.get_eff_msa_weights(self.msa_trimmed)
         self.n_eff = np.sum(self.msa_weights)
         self.n_row = self.msa_trimmed.shape[0]
         self.n_col = self.msa_trimmed.shape[1]
-        self.n_col_ori = self.msa_ori.shape[1]
         self.v_ini, self.w_ini = self.initialize_v_w(remove_gap_entries=False)
         self.optimize = optimize
         if self.optimize:
             self.v_opt, self.w_opt = self.run_opt_tf()
         self.x_wt = self.collect_encoded_sequences(np.atleast_1d(self.wt_seq))
 
     def a2n_dict(self):
@@ -206,15 +209,14 @@
             mt          and
             vt          (greek letter nu) at time steps t, respectively.
         Note by GREMLIN authors: this is a modified version of adam optimizer.
         More specifically, we replace "vt" with sum(g*g) instead of (g*g).
         Furthermore, we find that disabling the bias correction
         (b_fix=False) speeds up convergence for our case.
         """
-
         if var_list is None:
             var_list = tf.compat.v1.trainable_variables()
         gradients = tf.gradients(loss, var_list)
         if b_fix:
             t = tf.Variable(0.0, "t")
         opt = []
         for n, (x, g) in enumerate(zip(var_list, gradients)):
```

### Comparing `pypef-0.3/pypef/dca/hybrid_model.py` & `pypef-0.3.1/pypef/dca/hybrid_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,14 @@
 
 from pypef.dca.plmc_encoding import PLMC, get_dca_data_parallel, get_encoded_sequence, EffectiveSiteError
 from pypef.utils.to_file import predictions_out
 from pypef.utils.plot import plot_y_true_vs_y_pred
 import pypef.dca.gremlin_inference
 from pypef.dca.gremlin_inference import GREMLIN
 
-# np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)  # DEV
-
 
 class DCAHybridModel:
     alphas = np.logspace(-6, 6, 100)  # Grid for the parameter 'alpha'.
     parameter_range = [(0, 1), (0, 1)]  # Parameter range of 'beta_1' and 'beta_2' with lb <= x <= ub
     # TODO: Implementation of other regression techniques (CVRegression models)
 
     def __init__(
@@ -284,19 +282,15 @@
 
         Parameters
         ----------
         x_train : np.ndarray
             Encoded sequences of the variants in the training set.
         y_train : np.ndarray
             Fitness values of the variants in the training set.
-        x_test : np.ndarray
-            Encoded sequences of the variants in the testing set.
-        y_test : np.ndarray
-            Fitness values of the variants in the testing set.
-        train_size_train : float [0,1] (default 0.66)
+        train_size_fit : float [0,1] (default 0.66)
             Fraction to split training set into another
             training and testing set.
         random_state : int (default=224)
             Random state used to split.
 
         Returns
         -------
```

### Comparing `pypef-0.3/pypef/dca/plmc_encoding.py` & `pypef-0.3.1/pypef/dca/plmc_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,16 @@
 import numpy as np
 import ray
 from tqdm import tqdm
 import pickle
 
 from pypef.utils.variant_data import amino_acids
 
-
 _SLICE = np.s_[:]
-# np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)
+
 
 class InvalidVariantError(Exception):
     """
     Description
     -----------
     Exception raised when entered variant does not follow the required scheme
     (integer enclosed by two one-letter code representations of amino acids).
@@ -242,15 +241,15 @@
         # but gap is not part of model alphabet anymore; so if mapping crashes
         # that means there is a non-alphabet character in sequence array
         # and therefore there is no focus sequence.
         try:
             self.target_seq_mapped = np.array([self.alphabet_map[x] for x in self.target_seq])
             self.has_target_seq = (np.sum(self.target_seq_mapped) > 0)
         except KeyError:
-            self.target_seq_mapped = np.zeros((self.L), dtype=np.int32)
+            self.target_seq_mapped = np.zeros(shape=np.shape(self.l), dtype=np.int32)
             self.has_target_seq = False
 
     def __read_plmc_v2(self, filename, precision):
         """
         Read updated Jij file format from plmc.
 
         Parameters
@@ -260,36 +259,36 @@
         precision : {"float32", "float64"}
             Sets if input file has single or double precision
 
         """
         with open(filename, "rb") as f:
             # model length, number of symbols, valid/invalid sequences
             # and iterations
-            self.L, self.num_symbols, self.N_valid, self.N_invalid, self.num_iter = (
+            self.l, self.num_symbols, self.n_valid, self.n_invalid, self.num_iter = (
                 np.fromfile(f, "int32", 5)
             )
 
             # theta, regularization weights, and effective number of samples
-            self.theta, self.lambda_h, self.lambda_J, self.lambda_group, self.N_eff = (
+            self.theta, self.lambda_h, self.lambda_j, self.lambda_group, self.n_eff = (
                 np.fromfile(f, precision, 5)
             )
 
             # Read alphabet (make sure we get proper unicode rather than byte string)
             self.alphabet = np.fromfile(
                 f, "S1", self.num_symbols
             ).astype("U1")
 
             # weights of individual sequences (after clustering)
             self.weights = np.fromfile(
-                f, precision, self.N_valid + self.N_invalid
+                f, precision, self.n_valid + self.n_invalid
             )
 
             # target sequence and index mapping, again ensure unicode
-            self._target_seq = np.fromfile(f, "S1", self.L).astype("U1")
-            self.index_list = np.fromfile(f, "int32", self.L)
+            self._target_seq = np.fromfile(f, "S1", self.l).astype("U1")
+            self.index_list = np.fromfile(f, "int32", self.l)
 
             # Analyzing Positions included in the PLMC file (based on the MSA)
             not_valid, valid = [], []
             for num in range(self.index_list[0], self.index_list[-1] + 1, 1):
                 if num not in self.index_list:
                     not_valid.append(num)
                 else:
@@ -306,46 +305,46 @@
                     logger.info(f'Further, non-included positions are:\n{str(not_valid)[1:-1]}')
                 logger.info(f'Summary of all effective positions represented in the MSA '
                             f'based on wild-type sequence ({len(valid)} encoded positions):\n'
                             f'{str([aa_pos for aa_pos in self.wt_aa_pos])[1:-1]}'.replace("'", ""))
 
             # single site frequencies f_i and fields h_i
             self.f_i, = np.fromfile(
-                f, dtype=(precision, (self.L, self.num_symbols)), count=1
+                f, dtype=(precision, (self.l, self.num_symbols)), count=1
             )
 
             self.h_i, = np.fromfile(
-                f, dtype=(precision, (self.L, self.num_symbols)), count=1
+                f, dtype=(precision, (self.l, self.num_symbols)), count=1
             )
 
             # pair frequencies f_ij and pair couplings J_ij / J_ij
             self.f_ij = np.zeros(
-                (self.L, self.L, self.num_symbols, self.num_symbols)
+                (self.l, self.l, self.num_symbols, self.num_symbols)
             )
 
-            self.J_ij = np.zeros(
-                (self.L, self.L, self.num_symbols, self.num_symbols)
+            self.j_ij = np.zeros(
+                (self.l, self.l, self.num_symbols, self.num_symbols)
             )
 
-            for i in range(self.L - 1):
-                for j in range(i + 1, self.L):
+            for i in range(self.l - 1):
+                for j in range(i + 1, self.l):
                     self.f_ij[i, j], = np.fromfile(
                         f, dtype=(precision, (self.num_symbols, self.num_symbols)),
                         count=1
                     )
                     self.f_ij[j, i] = self.f_ij[i, j].T
 
-            for i in range(self.L - 1):
-                for j in range(i + 1, self.L):
-                    self.J_ij[i, j], = np.fromfile(
+            for i in range(self.l - 1):
+                for j in range(i + 1, self.l):
+                    self.j_ij[i, j], = np.fromfile(
                         f, dtype=(precision, (self.num_symbols, self.num_symbols)),
                         count=1
                     )
 
-                    self.J_ij[j, i] = self.J_ij[i, j].T
+                    self.j_ij[j, i] = self.j_ij[i, j].T
 
     def get_target_seq_and_index(self):
         """
         Gets and returns the target sequence of encodeable positions as
         well as the index list of encodeable positions that are the
         corresponding amino acid positions of the wild type sequence (1-indexed).
 
@@ -374,19 +373,18 @@
 
         Parameters
         ----------
         sequence : str, or list of chars
             Define a new default sequence for relative Hamiltonian
             calculations (e.g. energy difference relative to wild-type
             sequence).
-            Length of sequence must correspond to model length (self.L)
+            Length of sequence must correspond to model length (self.l)
         """
-        if len(sequence) != self.L:
-            raise ValueError(f"Sequence length inconsistent with model length: {len(sequence)} {self.L}")
-
+        if len(sequence) != self.l:
+            raise ValueError(f"Sequence length inconsistent with model length: {len(sequence)} != {self.l}")
 
         if isinstance(sequence, str):
             sequence = list(sequence)
 
         self._target_seq = np.array(sequence)
         self.target_seq_mapped = np.array([self.alphabet_map[x] for x in self.target_seq])
         self.has_target_seq = True
@@ -404,18 +402,18 @@
         """
         Define a new number mapping for sequences
 
         Parameters
         ----------
         mapping: list of int
             Sequence indices of the positions in the model.
-            Length of list must correspond to model length (self.L)
+            Length of list must correspond to model length (self.l)
         """
-        if len(mapping) != self.L:
-            raise ValueError(f"Mapping length inconsistent with model length: {len(mapping)} {self.L}")
+        if len(mapping) != self.l:
+            raise ValueError(f"Mapping length inconsistent with model length: {len(mapping)} != {self.l}")
 
         self._index_list = np.array(mapping)
         self.index_map = {b: a for a, b in enumerate(self.index_list)}
 
     def __map(self, indices, mapping):
         """
         Applies a mapping either to a single index, or to a list of indices
@@ -432,95 +430,92 @@
         """
         if ((isinstance(indices, Iterable) and not isinstance(indices, str)) or
                 (isinstance(indices, str) and len(indices) > 1)):
             return np.array([mapping[i] for i in indices])
         else:
             return mapping[indices]
 
-    def __4d_access(self, matrix, i=None, j=None, A_i=None, A_j=None):
+    def __4d_access(self, matrix, i=None, j=None, a_i=None, a_j=None):
         """
         Provides shortcut access to column pair properties
         (e.g. J_ij or f_ij matrices)
 
         Parameters
         -----------
         i : Iterable(int) or int
             Position(s) on first matrix axis
         j : Iterable(int) or int
             Position(s) on second matrix axis
-        A_i : Iterable(str) or str
+        a_i : Iterable(str) or str
             Symbols corresponding to first matrix axis
-        A_j : Iterable(str) or str
+        a_j : Iterable(str) or str
             Symbols corresponding to second matrix axis
 
         Returns
         -------
         np.array
-            4D matrix "matrix" sliced according to values i, j, A_i and A_j
+            4D matrix "matrix" sliced according to values i, j, a_i and a_j
         """
         i = self.__map(i, self.index_map) if i is not None else _SLICE
         j = self.__map(j, self.index_map) if j is not None else _SLICE
-        A_i = self.__map(A_i, self.alphabet_map) if A_i is not None else _SLICE
-        A_j = self.__map(A_j, self.alphabet_map) if A_j is not None else _SLICE
-
-        return matrix[i, j, A_i, A_j]
+        a_i = self.__map(a_i, self.alphabet_map) if a_i is not None else _SLICE
+        a_j = self.__map(a_j, self.alphabet_map) if a_j is not None else _SLICE
+        return matrix[i, j, a_i, a_j]
 
-    def __2d_access(self, matrix, i=None, A_i=None):
+    def __2d_access(self, matrix, i=None, a_i=None):
         """
         Provides shortcut access to single-column properties
         (e.g. f_i or h_i matrices)
 
         Parameters
         -----------
         i : Iterable(int) or int
             Position(s) on first matrix axis
-        A_i : Iterable(str) or str
+        a_i : Iterable(str) or str
             Symbols corresponding to first matrix axis
 
         Returns
         -------
         np.array
-            2D matrix "matrix" sliced according to values i and A_i
+            2D matrix "matrix" sliced according to values i and a_i
         """
         i = self.__map(i, self.index_map) if i is not None else _SLICE
-        A_i = self.__map(A_i, self.alphabet_map) if A_i is not None else _SLICE
+        a_i = self.__map(a_i, self.alphabet_map) if a_i is not None else _SLICE
+        return matrix[i, a_i]
 
-        return matrix[i, A_i]
-
-    def Jij(self, i=None, j=None, A_i=None, A_j=None):
+    def get_jij(self, i=None, j=None, a_i=None, a_j=None):
         """
         Quick access to J_ij matrix with automatic index mapping.
         See __4d_access for explanation of parameters.
         """
-        return self.__4d_access(self.J_ij, i, j, A_i, A_j)
+        return self.__4d_access(self.j_ij, i, j, a_i, a_j)
 
-    def hi(self, i=None, A_i=None):
+    def get_hi(self, i=None, a_i=None):
         """
         Quick access to h_i matrix with automatic index mapping.
         See __2d_access for explanation of parameters.
         """
-        return self.__2d_access(self.h_i, i, A_i)
+        return self.__2d_access(self.h_i, i, a_i)
 
 
 class PLMC(CouplingsModel):
-    """
-    Class for performing the 'DCA encoding'.
-
-    Attributes
-    ----------
-    params_file: str
-        Binary parameter file outputted by PLMC.
-    """
-
     def __init__(
             self,
             params_file: str,
             separator: str = '/',
             verbose: bool = True
     ):
+        """
+        Class for performing the 'DCA encoding'.
+
+        Attributes
+        ----------
+        params_file: str
+            Binary parameter file outputted by PLMC.
+        """
         super().__init__(filename=params_file)  # inherit functions and variables from class CouplingsModel
         self.verbose = verbose
         self.separator = separator
         target_seq, index = self.get_target_seq_and_index()
         self.x_wt = self.collect_encoded_sequences(target_seq[0] + str(index[0]) + target_seq[0])
 
     def _get_position_internal(self, position: int):
@@ -547,39 +542,39 @@
         offset = 0
         i = position - offset
         if i in self.index_list:
             return i
         else:
             return None
 
-    def Ji(self, i: int, A_i: str, sequence: np.ndarray) -> float:
+    def sum_ji(self, i: int, a_i: str, sequence: np.ndarray) -> float:
         """
         Description
         -----------
-        Caluclates the sum of all site-site interaction terms when site 'i' is occupied with amino acid 'A_i'.
+        Calculates the sum of all site-site interaction terms when site 'i' is occupied with amino acid 'a_i'.
 
         Parameters
         ----------
         i : int
             "Internal position" see '_get_position_internal' for an explanation.
-        A_i : str
-            Introduced amino acid at 'i' in one letter code representation.
+        a_i : str
+            Introduced amino acid at 'i' in one-letter code representation.
         sequence: np.ndarray
             Sequence of the variant as numpy array.
 
         Returns
         -------
-        Ji : float
-            Sum of all site-site interaction terms acting on position 'i' when occupied with 'A_i'.
+        j_i : float
+            Sum J(i) of all site-site interaction terms acting on position 'i' when occupied with 'a_i'.
         """
-        Ji = 0.0
-        for j, A_j in zip(self.index_list, sequence):
-            Ji += self.Jij(i=i, A_i=A_i, j=j, A_j=A_j)
+        j_i_sum = 0.0
+        for j, a_j in zip(self.index_list, sequence):
+            j_i_sum += self.get_jij(i=i, a_i=a_i, j=j, a_j=a_j)
 
-        return Ji
+        return j_i_sum
 
     @staticmethod
     def _unpack_substitution(substitution: str) -> tuple:
         """
         Description
         -----------
         Turns string representation of variant into tuple.
@@ -599,15 +594,15 @@
 
     def check_substitution_naming_against_wt(self, substitution: str, variant: str):
         """
         Checks whether the amino acid to substitute of the variant matches
         the amino acid of the wild type at this position.
         """
         if substitution[:-1] not in self.wt_aa_pos:
-            wild_type_aa, position, A_i = self._unpack_substitution(substitution)
+            wild_type_aa, position, a_i = self._unpack_substitution(substitution)
             raise SystemError(
                 f"The variant naming scheme is not fitting to the PLMC "
                 f"scheme. Substitution {substitution} of variant {variant} has "
                 f"the amino acid {wild_type_aa} at position {position}, which "
                 f"does not match the wild type sequence used as target for DCA-"
                 f"based coupling parameter file generation. See summary of "
                 f"(effective) wild-type positions and amino acids above. Please "
@@ -630,27 +625,27 @@
         Returns
         -------
         x_var : np.ndarray
             Encoded sequence of the variant.
         """
         sequence = self.target_seq.copy()
         for substitution in get_single_substitutions(variant, self.separator):  # e.g. A123C/D234E --> A123C, D234C
-            wild_type_aa, position, A_i = self._unpack_substitution(substitution)
+            wild_type_aa, position, a_i = self._unpack_substitution(substitution)
 
             i = self._get_position_internal(position)
             if not i:
                 raise EffectiveSiteError(position, variant, self.verbose)
 
             self.check_substitution_naming_against_wt(substitution, variant)
             i_mapped = self.index_map[i]
-            sequence[i_mapped] = A_i
+            sequence[i_mapped] = a_i
 
         x_var = np.zeros(sequence.size, dtype=float)
-        for idx, (i, A_i) in enumerate(zip(self.index_list, sequence)):
-            x_var[idx] = self.hi(i, A_i) + 0.5 * self.Ji(i, A_i, sequence)
+        for idx, (i, a_i) in enumerate(zip(self.index_list, sequence)):
+            x_var[idx] = self.get_hi(i, a_i) + 0.5 * self.sum_ji(i, a_i, sequence)
 
         return x_var
 
     def collect_encoded_sequences(self, variants: list) -> np.ndarray:
         """
         Description
         -----------
@@ -802,21 +797,25 @@
     This function allows to generate the encoded sequences based on the variants
     given in 'csv_file' in a parallel manner.
 
     Parameters
     ----------
     variants: list (or np.ndarray)
         Variant names.
+    sequences: list (or np.ndarray)
+        Variant-associated protein sequences.
     fitnesses: list (or np.ndarray)
         Variant-associated fitness values.
     dca_encode : object
         Initialized 'PLMC' class object.
     threads : int
         Number of processes to be used for parallel execution.
         n_cores = 1 defines no threading (not using Ray).
+    verbose: bool
+        Logging message on/off.
 
     Returns
     -------
     data: numpy.ndarray
         Filled numpy array including variant names, fitnesses, and encoded sequences.
     non_effective_subs: list
         List of variant names that cannot be used for modelling as they are not effective
```

### Comparing `pypef-0.3/pypef/main.py` & `pypef-0.3.1/pypef/main.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,436 +1,436 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Created on 05 October 2020
-# @authors: Niklas Siedhoff, Alexander-Maurice Illig
-# @contact: <n.siedhoff@biotec.rwth-aachen.de>
-# PyPEF - Pythonic Protein Engineering Framework
-# Released under Creative Commons Attribution-NonCommercial 4.0 International Public License (CC BY-NC 4.0)
-# For more information about the license see https://creativecommons.org/licenses/by-nc/4.0/legalcode
-
-# PyPEF – An Integrated Framework for Data-Driven Protein Engineering
-# Journal of Chemical Information and Modeling, 2021, 61, 3463-3476
-# https://doi.org/10.1021/acs.jcim.1c00099
-# Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
-# 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
-# 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
-# *Corresponding author
-# §Equal contribution
-
-
-# docstring for argument parsing using docopts
-"""
-PyPEF - Pythonic Protein Engineering Framework
-
-written by Niklas Siedhoff and Alexander-Maurice Illig.
-
-Modeling options
-----------------
-    I. Pure ML modeling
-    -------------------
-        PyPEF provides three encoding options for training machine learning models, i.e.
-        regression models trained by supervised learning:
-
-            1. DCA: Direct coupling analysis (DCA) based on evolutionary couplings (input:
-                       coupling parameter file generated by the C framework plmc) or
-                       generating parameters using TensorFlow-based GREMLIN (input: MSA).
-
-            2. AAidx: Based on AAindex descriptors (566 amino acid descriptor files
-                       taken from the AAindex database).
-
-            3. OneHot: One-hot encoding representing the occurrence of an
-                       amino acid at a sequence position as a single 1 and 19 0's.
-
-        Any encoding technique enables pure ML-based modeling, see
-        https://doi.org/10.1021/acs.jcim.1c00099
-        and DCA-based sequence encoding enables a hybrid modeling approach, see
-        https://doi.org/10.1101/2022.06.07.495081
-
-        If an MSA can be constructed for the target sequence, e.g. using Jackhmmer,
-        encoding option 1 will likely outperform encoding option 2.
-        However, encoding option 2 provides a static encoding technique that is
-        independent from the evolutionary history of a target sequence and
-        without the need for MSA construction.
-        Here, the AAidx encodings for modeling are compared, i.e. validated, with respect
-        to their performance on the test set (comparable to an hyperparameter search
-        for finding the best static encoding set for model inference).
-        Further, one-hot encoding (encoding option 3) provides a simple but fast and often
-        well-performing encoding option that will likely outperform the AAindex-based
-        technique for model generalization.
-
-    II. Hybrid modeling
-    -------------------
-        Constructing a hybrid model that combines pure statistical DCA-based prediction (a
-        variant's relative 'evolutionary energy' to the wild type) and DCA-encoding based
-        training of a ML model similar to pure ML modeling option I.1.
-        Based on features generated from the direct coupling analysis (.params file output
-        using the plmc framework or provided MSA and running GREMLIN).
-        Individual model contributions are optimization only based on Spearman's correlation
-        coefficient and thus, only variant fitness ranks are to be considered for evaluating
-        model performance, not the exact predicted fitness value. For regression, up to now
-        only L2-regularized linear regression (Ridge regression) is provided as modeling option.
-
-
-Running example of training, testing, and using a pure ML model for prediction
-------------------------------------------------------------------------------
-Exemplary running of PyPEF for training a pure ML model using encoding option 2
-based on features generated from the AAIndex database (566 amino acid descriptor
-indices taken from the AAIndex database).
- 1. Create files for training and testing from variant-fitness CSV data:
-       pypef mklsts -i variant_and_fitness.csv -w wt_sequence.fasta
- 2. Train and validate models:
-        pypef ml -e onehot -l LS.fasta -t TS.fasta --regressor pls
- 3. Plot the test set entries against test set predictions (creates PNG figure, MODEL is
-    the chosen AAindex, the ML-DCA model, or here the ONEHOT model):
-        pypef ml -e onehot -m ONEHOT -t TS.fasta
- 4. Create files for prediction:
-    - Single file:
-        pypef mkps -w wt_sequence.fasta -i variant_fitness.csv
-    - Recombinant/diverse prediction files:
-        pypef mkps -w wt_sequence.fasta -i variant_fitness.csv
-            [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
-            [--ddiverse] [--tdiverse] [--qdiverse]
- 5. Predict (unknown/new) variants:
-    - Single file:
-        pypef ml -e aaidx -m MODEL -p Prediction_Set.fasta
-    - Recombinant/diverse prediction files in created prediction set folders:
-        pypef ml -e aaidx -m MODEL --pmult [--drecomb] [...] [--qdiverse]
-    - Directed evolution – for performing and plotting in silico evolution trajectories:
-        pypef ml -e aaidx directevo -m MODEL [...]
-Note: The commands for hybrid modeling are very similar to the commands for pure ML modeling,
-see pypef -h for possible commands.
-
-For generating DCA parameters using GREMLIN, you have to provide an MSA in FASTA or A2M format:
-pypef param_inference --msa MSA_FILE --wt WT_FASTA [--opt_iter 100]
-
-
-Helpful commands for data conversion
------------------------------------------------
-Creation of learning and test sets – splitting CSV variant-fitness data:
-        pypef mklsts --wt WT_FASTA --input CSV_FILE
-            [--drop THRESHOLD] [--numrnd NUMBER]
-
-Creation of prediction sets from CSV data (using single-substituted variant data):
-        pypef mkps --wt WT_FASTA --input CSV_FILE
-            [--drop THRESHOLD] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
-            [--ddiverse] [--tdiverse] [--qdiverse]
-
-Encoding a CSV file (for further performance studies such as "low N" or
-"mutational extrapolation" engineering tasks:
-        pypef encode --input CSV_FILE --encoding ENCODING_TECHNIQUE --wt WT_FASTA
-            [--params PARAM_FILE] [--y_wt WT_FITNESS] [--model MODEL] [--nofft]
-            [--threads THREADS] [--sep CSV_COLUMN_SEPARATOR] [--fitness_key FITNESS_KEY]
-
-Converting a STO alignment file to A2M format:
-        pypef sto2a2m --sto STO_MSA_FILE
-            [--inter_gap INTER_GAP] [--intra_gap INTRA_GAP]
-
-
-Usage:
-    pypef mklsts --wt WT_FASTA --input CSV_FILE
-        [--drop THRESHOLD] [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--numrnd NUMBER]
-    pypef mkps --wt WT_FASTA [--input CSV_FILE]
-        [--drop THRESHOLD] [--ssm] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
-        [--ddiverse] [--tdiverse] [--qdiverse]
-    pypef param_inference
-        [--msa MSA_FILE] [--params PARAM_FILE]
-        [--wt WT_FASTA] [--opt_iter N_ITER]
-    pypef save_msa_info --msa MSA_FILE --wt WT_FASTA
-        [--opt_iter N_ITER]
-    pypef encode --input CSV_FILE --encoding ENCODING_TECHNIQUE --wt WT_FASTA
-        [--params PARAM_FILE] [--y_wt WT_FITNESS] [--model MODEL] [--nofft]
-        [--threads THREADS]
-        [--sep CSV_COLUMN_SEPARATOR] [--fitness_key FITNESS_KEY]
-    pypef reformat_csv --input CSV_FILE
-        [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--fitness_key FITNESS_KEY]
-    pypef shift_pos --input CSV_FILE --offset OFFSET
-        [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--fitness_key FITNESS_KEY]
-    pypef sto2a2m --sto STO_MSA_FILE [--inter_gap INTER_GAP] [--intra_gap INTRA_GAP]
-    pypef hybrid --ts TEST_SET
-        [--model MODEL] [--params PARAM_FILE]
-        [--ls LEARNING_SET] [--label] [--threads THREADS]
-    pypef hybrid --model MODEL --params PARAM_FILE
-        [--ts TEST_SET] [--label]
-        [--ps PREDICTION_SET] [--pmult] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
-                                        [--ddiverse] [--tdiverse] [--qdiverse] [--negative]
-        [--threads THREADS]
-    pypef hybrid directevo --wt WT_FASTA --params PARAM_FILE
-        [--model MODEL]
-        [--input CSV_FILE] [--y_wt WT_FITNESS] [--numiter NUM_ITER]
-        [--numtraj NUM_TRAJ] [--temp TEMPERATURE]
-        [--negative] [--usecsv] [--csvaa] [--drop THRESHOLD]
-    pypef hybrid train_and_save --input CSV_FILE --params PARAM_FILE --wt WT_FASTA
-        [--fit_size REL_LEARN_FIT_SIZE] [--test_size REL_TEST_SIZE]
-        [--threads THREADS] [--sep CSV_COLUMN_SEPARATOR]
-        [--fitness_key FITNESS_KEY] [--rnd_state RND_STATE]
-    pypef hybrid low_n --input ENCODED_CSV_FILE
-    pypef hybrid extrapolation --input ENCODED_CSV_FILE
-        [--conc]
-    pypef ml --encoding ENCODING_TECHNIQUE --ls LEARNING_SET --ts TEST_SET
-        [--save NUMBER] [--regressor TYPE] [--nofft] [--all] [--params PARAM_FILE]
-        [--sort METRIC_INT] [--threads THREADS] [--label]
-    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL --ts TEST_SET
-        [--nofft] [--params PARAM_FILE] [--threads THREADS] [--label]
-    pypef ml --show
-        [MODELS]
-    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL --ps PREDICTION_SET
-        [--params PARAM_FILE] [--threads THREADS] [--nofft] [--negative]
-    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL --pmult
-        [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
-        [--ddiverse] [--tdiverse] [--qdiverse]
-        [--regressor TYPE] [--nofft] [--negative] [--params PARAM_FILE] [--threads THREADS]
-    pypef ml --encoding ENCODING_TECHNIQUE directevo --model MODEL --wt WT_FASTA
-        [--input CSV_FILE] [--y_wt WT_FITNESS] [--numiter NUM_ITER] [--numtraj NUM_TRAJ] [--temp TEMPERATURE]
-        [--nofft] [--negative] [--usecsv] [--csvaa] [--drop THRESHOLD] [--params PARAM_FILE]
-    pypef ml low_n --input ENCODED_CSV_FILE
-        [--regressor TYPE]
-    pypef ml extrapolation --input ENCODED_CSV_FILE
-        [--regressor TYPE] [--conc]
-
-
-Options:
-  --all                             Finally training on all data [default: False].
-  --conc                            Concatenating mutational level variants for predicting variants
-                                    from next higher level [default: False].
-  --csvaa                           Directed evolution csv amino acid substitutions,
-                                    requires flag "--usecsv" [default: False].
-  --ddiverse                        Create/predict double natural diverse variants [default: False].
-  --drecomb                         Create/predict double recombinants [default: False].
-  -d --drop THRESHOLD               Below threshold variants will be discarded from the
-                                    data [default: -9E09].
-  -e --encoding ENCODING_TECHNIQUE  Sets technique used for encoding sequences for constructing regression models;
-                                    choose between 'aaidx' (AAIndex-based encoding), 'onehot' (OneHot-based encoding),
-                                    and DCA encoding using Gremlin/plmc (DCA-based encoding) [default: onehot].
-  --fitness_key FITNESS_KEY         Label of CSV fitness column. Else uses second column.
-  -h --help                         Show this screen [default: False].
-  -i --input CSV_FILE               Input data file in .csv format.
-  --inter_gap INTER_GAP             Fraction to delete all positions with more than
-                                    'inter_gap' * 100 % gaps (columnar trimming) [default: 0.3].
-  --intra_gap INTRA_GAP             Fraction to delete all sequences with more than
-                                    'intra_gap' * 100 % gaps after being columnar trimmed
-                                    (line trimming) [default: 0.5].
-  --label                           Label the plot instances [default: False].
-  -l --ls LEARNING_SET              Input learning set in .fasta format.
-  -m --model MODEL                  Model (pickle file) for plotting of validation or for
-                                    performing predictions.
-  --msa MSA_FILE                    Multiple sequence alignment (MSA) ins FASTA or A2M format for
-                                    inferring DCA parameters.
-  --mutation_sep MUTATION_SEP       Mutation separator [default: /].
-  --mutation_extrapolation          Mutation extrapolation [default: False].
-  --negative                        Set if more negative values define better variants [default: False].
-  --nofft                           Raw sequence input, i.e., no FFT for establishing protein spectra
-                                    as vector inputs, only implemented as option for AAindex-based
-                                    sequence encoding [default: False].
-  -n --numrnd NUMBER                Number of randomly created Learning and Validation
-                                    datasets [default: 0].
-  --numiter NUM_ITER                Number of mutation iterations per evolution trajectory [default: 5].
-  --numtraj NUM_TRAJ                Number of trajectories, i.e., evolution pathways [default: 5].
-  -o --offset OFFSET                Offset for shifting substitution positions of the input CSV file [default: 0].
-  --opt_iter N_ITER                 Number of iterations for GREMLIN-based optimization of local fields
-                                    and couplings [default: 100].
-  --params PARAM_FILE               Input PLMC couplings parameter file.
-  -u --pmult                        Predict for all prediction files in folder for recombinants
-                                    or for diverse variants [default: False].
-  -p --ps PREDICTION_SET            Prediction set for performing predictions using a trained Model.
-  --qdiverse                        Create quadruple natural diverse variants [default: False].
-  --qarecomb                        Create/predict quadruple recombinants [default: False].
-  --qirecomb                        Create/predict quintuple recombinants [default: False].
-  --regressor TYPE                  Type of regression (R.) to use, options: PLS CV R.: pls,
-                                    PLS LOOCV R.: pls_loocv, Random Forest CV R.: rf, SVM CV R.: svr,
-                                    MLP CV R.: mlp, Ridge CV R.: ridge (or l2),
-                                    LassoLars CV R.: lassolars (or l1) [default: pls].
-  --rnd_splits RND_SPLITS           Number of random splits for Low N testing [default: 5].
-  --rnd_state RND_STATE             Sets the random state for reproduction, only implemented
-                                    for hybrid train_and_save [default: 42].
-  -s --save NUMBER                  Number of models to be saved as pickle files [default: 5].
-  --sep CSV_COLUMN_SEPARATOR        CSV Column separator [default: ;].
-  --show                            Show achieved model performances from Model_Results.txt.
-  --sort METRIC_INT                 Rank models based on metric {1: R^2, 2: RMSE, 3: NRMSE,
-                                    4: Pearson's r, 5: Spearman's rho} [default: 1].
-  --ssm                             Create single-saturation mutagenesis prediction set (does not
-                                    require CSV input) [default: False].
-  --sto STO_MSA_FILE                The input MSA file in STO (Stockholm) format.
-  --tdiverse                        Create/predict triple natural diverse variants [default: False].
-  --temp TEMPERATURE                "Temperature" of Metropolis-Hastings criterion [default: 0.01]
-  --threads THREADS                 Parallel computing of training and validation of models.
-                                    Number of threads used in parallel computing, by default
-                                    no hyperthreading.
-  --fit_size REL_LEARN_FIT_SIZE     Relative size of the train set for initial fitting. The remaining data
-                                    for training is used for hyperparameter optimization on train subsets
-                                    used for validation, while in sum the total data for training is
-                                    training data = train_fit data + train_test(validation) data
-                                                  = all data - test data.
-                                    The default of 0.66 means that 34 % of the train data is taken for
-                                    train_test validation [default: 0.66].
-  --test_size REL_TEST_SIZE         Relative size of the test set; if set to 0.0 the trained model
-                                    will not be tested [default: 0.2].
-  --trecomb                         Create/predict triple recombinants [default: False].
-  --usecsv                          Perform directed evolution on single variant csv position
-                                    data [default: False].
-  -t --ts TEST_SET                  Input validation set in .fasta format.
-  --version                         Show version [default: False].
-  -w --wt WT_FASTA                  Input wild-type sequence file (in FASTA format).
-  --wt_pos WT_POSITION              Row position of encoded wild-type in encoding CSV file (0-indexed) [default: 0].
-  -y --y_wt WT_FITNESS              Fitness value (y) of wild-type [default: 1.0].
-  encode                            Encoding [default: False].
-  hybrid                            Hybrid modeling based on DCA-derived sequence encoding [default: False].
-  ml                                Pure machine learning modeling based on encoded sequences [default: False].
-  MODELS                            Number of saved models to show [default: 5].
-  onehot                            OneHot-based encoding [default: False].
-  param_inference                   Inferring DCA params using the GREMLIN approach [default: False].
-  reformat_csv                      Reformat input CSV with indicated column and mutation separators to default
-                                    CSV style (column separator ';' and mutation separator '/') [default: False.]
-  save_msa_info                     Optimize local fields and couplings of MSA based on GREMLIN DCA approach and
-                                    save resulting coupling matrix and highly coevolved amino acids.
-  shift_pos                         Shift positions of all variant substitutions of the input CSV
-                                    file (identical to reformat_csv when setting --offset to 0) [default: False.]
-  sto2a2m                           Transform multiple sequence alignment from STO format to
-                                    A2M format [default: False].
-"""
-
-
-from os import environ
-try:
-    environ['TF_CPP_MIN_LOG_LEVEL'] = '2'  # only print TensorFlow errors, set to '0' or comment
-except KeyError:                           # lines for seeing TensorFlow infos and warnings
-    pass
-
-from sys import argv, version_info
-from pypef import __version__
-if version_info[0] < 3 or version_info[1] < 9:
-    raise SystemError(f"The current version of PyPEF (v {__version__}) "
-                      f"requires at least Python 3.9 or higher.")
-
-import time
-from datetime import timedelta
-import logging
-
-from docopt import docopt
-from schema import Schema, SchemaError, Optional, Or, Use
-
-from pypef.ml.ml_run import run_pypef_pure_ml
-from pypef.dca.dca_run import run_pypef_hybrid_modeling
-from pypef.utils.utils_run import run_pypef_utils
-
-logger = logging.getLogger("pypef")
-logger.setLevel(logging.INFO)
-
-ch = logging.StreamHandler()
-ch.setLevel(logging.DEBUG)
-
-formatter = logging.Formatter(
-    "%(asctime)s.%(msecs)03d %(levelname)s %(filename)s:%(lineno)d -- %(message)s",
-    "%Y-%m-%d %H:%M:%S"
-)
-ch.setFormatter(formatter)
-logger.addHandler(ch)
-
-
-schema = Schema({
-    Optional('--all'): bool,
-    Optional('--conc'): bool,
-    Optional('--csvaa'): bool,
-    Optional('--ddiverse'): bool,
-    Optional('--drecomb'): bool,
-    Optional('--drop'): Use(float),
-    Optional('--encoding'): Use(str),
-    Optional('--fitness_key'): Or(None, str),
-    Optional('--fit_size'): Use(float),
-    Optional('--help'): bool,
-    Optional('--input'): Or(None, str),
-    Optional('--inter_gap'): Use(float),
-    Optional('--intra_gap'): Use(float),
-    Optional('--label'): bool,
-    Optional('--ls'): Or(None, str),
-    Optional('--model'): Or(None, str),
-    Optional('--msa'): Or(None, str),
-    Optional('--mutation_sep'): Or(None, str),
-    Optional('--negative'): bool,
-    Optional('--nofft'): bool,
-    Optional('--numrnd'): Use(int),
-    Optional('--numiter'): Use(int),
-    Optional('--numtraj'): Use(int),
-    Optional('--offset'): Use(int),
-    Optional('--opt_iter'): Use(int),
-    Optional('--params'): Or(None, str),
-    Optional('--pmult'): bool,
-    Optional('--ps'): Or(None, str),
-    Optional('--qdiverse'): bool,
-    Optional('--qarecomb'): bool,
-    Optional('--qirecomb'): bool,
-    Optional('--regressor'): Or(None, str),
-    Optional('--rnd_splits'): Use(int),
-    Optional('--rnd_state'): Use(int),
-    Optional('--save'): Use(int),
-    Optional('--sep'): Or(None, str),
-    Optional('--show'): Use(int),
-    Optional('--sort'): Use(int),
-    Optional('--ssm'): bool,
-    Optional('--sto'): Or(None, str),
-    Optional('--tdiverse'): bool,
-    Optional('--temp'): Use(float),
-    Optional('--test_size'): Use(float),
-    Optional('--threads'): Or(None, Use(int)),
-    Optional('--train_size'): Use(float),
-    Optional('--trecomb'): bool,
-    Optional('--usecsv'): bool,
-    Optional('--ts'): Or(None, str),
-    Optional('--wt'): Or(None, str),
-    Optional('--wt_pos'): Use(int),
-    Optional('--y_wt'): Or(None, Use(float)),
-    Optional('aaidx'): bool,
-    Optional('param_inference'): bool,
-    Optional('hybrid'): bool,
-    Optional('directevo'): bool,
-    Optional('encode'): bool,
-    Optional('extrapolation'): bool,
-    Optional('low_n'): bool,
-    Optional('mklsts'): bool,
-    Optional('mkps'): bool,
-    Optional('ml'): bool,
-    Optional('MODELS'): Or(None, Use(int)),
-    Optional('onehot'): bool,
-    Optional('reformat_csv'): bool,
-    Optional('save_msa_info'): bool,
-    Optional('shift_pos'): bool,
-    Optional('sto2a2m'): bool,
-    Optional('train_and_save'): bool,
-})
-
-
-def validate(args):
-    try:
-        args = schema.validate(args)
-        return args
-    except SchemaError as e:
-        exit(e)
-
-
-def run_main():
-    """
-    Entry point for pip-installed version.
-    """
-    arguments = docopt(__doc__, version=__version__)
-    start_time = time.time()
-    logger.debug(f'main.py __name__: {__name__}, version: {__version__}')
-    logger.debug(str(argv)[1:-1].replace("\'", "").replace(",", ""))
-    logger.debug(f'\n{arguments}')
-    arguments = validate(arguments)
-    if arguments['directevo']:
-        run_pypef_utils(arguments)
-    elif arguments['ml']:
-        run_pypef_pure_ml(arguments)
-    elif arguments['hybrid'] or arguments['param_inference'] or arguments['save_msa_info']:
-        run_pypef_hybrid_modeling(arguments)
-    else:
-        run_pypef_utils(arguments)
-
-    elapsed = str(timedelta(seconds=time.time()-start_time)).split(".")[0]
-    elapsed = f'{elapsed.split(":")[0]} h {elapsed.split(":")[1]} min {elapsed.split(":")[2]} s'
-    logger.info(f'Done! (Run time: {elapsed})')
-
-
-if __name__ == '__main__':
-    """
-    Entry point for direct file run.
-    """
-    run_main()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+# Created on 05 October 2020
+# @authors: Niklas Siedhoff, Alexander-Maurice Illig
+# @contact: <n.siedhoff@biotec.rwth-aachen.de>
+# PyPEF - Pythonic Protein Engineering Framework
+# Released under Creative Commons Attribution-NonCommercial 4.0 International Public License (CC BY-NC 4.0)
+# For more information about the license see https://creativecommons.org/licenses/by-nc/4.0/legalcode
+
+# PyPEF – An Integrated Framework for Data-Driven Protein Engineering
+# Journal of Chemical Information and Modeling, 2021, 61, 3463-3476
+# https://doi.org/10.1021/acs.jcim.1c00099
+# Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
+# 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
+# 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
+# *Corresponding author
+# §Equal contribution
+
+
+# docstring for argument parsing using docopts
+"""
+PyPEF - Pythonic Protein Engineering Framework
+
+written by Niklas Siedhoff and Alexander-Maurice Illig.
+
+Modeling options
+----------------
+    I. Pure ML modeling
+    -------------------
+        PyPEF provides three encoding options for training machine learning models, i.e.
+        regression models trained by supervised learning:
+
+            1. DCA: Direct coupling analysis (DCA) based on evolutionary couplings (input:
+                       coupling parameter file generated by the C framework plmc) or
+                       generating parameters using TensorFlow-based GREMLIN (input: MSA).
+
+            2. AAidx: Based on AAindex descriptors (566 amino acid descriptor files
+                       taken from the AAindex database).
+
+            3. OneHot: One-hot encoding representing the occurrence of an
+                       amino acid at a sequence position as a single 1 and 19 0's.
+
+        Any encoding technique enables pure ML-based modeling, see
+        https://doi.org/10.1021/acs.jcim.1c00099
+        and DCA-based sequence encoding enables a hybrid modeling approach, see
+        https://doi.org/10.1101/2022.06.07.495081
+
+        If an MSA can be constructed for the target sequence, e.g. using Jackhmmer,
+        encoding option 1 will likely outperform encoding option 2.
+        However, encoding option 2 provides a static encoding technique that is
+        independent from the evolutionary history of a target sequence and
+        without the need for MSA construction.
+        Here, the AAidx encodings for modeling are compared, i.e. validated, with respect
+        to their performance on the test set (comparable to an hyperparameter search
+        for finding the best static encoding set for model inference).
+        Further, one-hot encoding (encoding option 3) provides a simple but fast and often
+        well-performing encoding option that will likely outperform the AAindex-based
+        technique for model generalization.
+
+    II. Hybrid modeling
+    -------------------
+        Constructing a hybrid model that combines pure statistical DCA-based prediction (a
+        variant's relative 'evolutionary energy' to the wild type) and DCA-encoding based
+        training of a ML model similar to pure ML modeling option I.1.
+        Based on features generated from the direct coupling analysis (.params file output
+        using the plmc framework or provided MSA and running GREMLIN).
+        Individual model contributions are optimization only based on Spearman's correlation
+        coefficient and thus, only variant fitness ranks are to be considered for evaluating
+        model performance, not the exact predicted fitness value. For regression, up to now
+        only L2-regularized linear regression (Ridge regression) is provided as modeling option.
+
+
+Running example of training, testing, and using a pure ML model for prediction
+------------------------------------------------------------------------------
+Exemplary running of PyPEF for training a pure ML model using encoding option 2
+based on features generated from the AAIndex database (566 amino acid descriptor
+indices taken from the AAIndex database).
+ 1. Create files for training and testing from variant-fitness CSV data:
+       pypef mklsts -i variant_and_fitness.csv -w wt_sequence.fasta
+ 2. Train and validate models:
+        pypef ml -e onehot -l LS.fasta -t TS.fasta --regressor pls
+ 3. Plot the test set entries against test set predictions (creates PNG figure, MODEL is
+    the chosen AAindex, the ML-DCA model, or here the ONEHOT model):
+        pypef ml -e onehot -m ONEHOT -t TS.fasta
+ 4. Create files for prediction:
+    - Single file:
+        pypef mkps -w wt_sequence.fasta -i variant_fitness.csv
+    - Recombinant/diverse prediction files:
+        pypef mkps -w wt_sequence.fasta -i variant_fitness.csv
+            [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
+            [--ddiverse] [--tdiverse] [--qdiverse]
+ 5. Predict (unknown/new) variants:
+    - Single file:
+        pypef ml -e aaidx -m MODEL -p Prediction_Set.fasta
+    - Recombinant/diverse prediction files in created prediction set folders:
+        pypef ml -e aaidx -m MODEL --pmult [--drecomb] [...] [--qdiverse]
+    - Directed evolution – for performing and plotting in silico evolution trajectories:
+        pypef ml -e aaidx directevo -m MODEL [...]
+Note: The commands for hybrid modeling are very similar to the commands for pure ML modeling,
+see pypef -h for possible commands.
+
+For generating DCA parameters using GREMLIN, you have to provide an MSA in FASTA or A2M format:
+pypef param_inference --msa MSA_FILE --wt WT_FASTA [--opt_iter 100]
+
+
+Helpful commands for data conversion
+-----------------------------------------------
+Creation of learning and test sets – splitting CSV variant-fitness data:
+        pypef mklsts --wt WT_FASTA --input CSV_FILE
+            [--drop THRESHOLD] [--numrnd NUMBER]
+
+Creation of prediction sets from CSV data (using single-substituted variant data):
+        pypef mkps --wt WT_FASTA --input CSV_FILE
+            [--drop THRESHOLD] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
+            [--ddiverse] [--tdiverse] [--qdiverse]
+
+Encoding a CSV file (for further performance studies such as "low N" or
+"mutational extrapolation" engineering tasks:
+        pypef encode --input CSV_FILE --encoding ENCODING_TECHNIQUE --wt WT_FASTA
+            [--params PARAM_FILE] [--y_wt WT_FITNESS] [--model MODEL] [--nofft]
+            [--threads THREADS] [--sep CSV_COLUMN_SEPARATOR] [--fitness_key FITNESS_KEY]
+
+Converting a STO alignment file to A2M format:
+        pypef sto2a2m --sto STO_MSA_FILE
+            [--inter_gap INTER_GAP] [--intra_gap INTRA_GAP]
+
+
+Usage:
+    pypef mklsts --wt WT_FASTA --input CSV_FILE
+        [--drop THRESHOLD] [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--numrnd NUMBER]
+    pypef mkps --wt WT_FASTA [--input CSV_FILE]
+        [--drop THRESHOLD] [--ssm] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
+        [--ddiverse] [--tdiverse] [--qdiverse]
+    pypef param_inference
+        [--msa MSA_FILE] [--params PARAM_FILE]
+        [--wt WT_FASTA] [--opt_iter N_ITER]
+    pypef save_msa_info --msa MSA_FILE --wt WT_FASTA
+        [--opt_iter N_ITER]
+    pypef encode --input CSV_FILE --encoding ENCODING_TECHNIQUE --wt WT_FASTA
+        [--params PARAM_FILE] [--y_wt WT_FITNESS] [--model MODEL] [--nofft]
+        [--threads THREADS]
+        [--sep CSV_COLUMN_SEPARATOR] [--fitness_key FITNESS_KEY]
+    pypef reformat_csv --input CSV_FILE
+        [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--fitness_key FITNESS_KEY]
+    pypef shift_pos --input CSV_FILE --offset OFFSET
+        [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--fitness_key FITNESS_KEY]
+    pypef sto2a2m --sto STO_MSA_FILE [--inter_gap INTER_GAP] [--intra_gap INTRA_GAP]
+    pypef hybrid --ts TEST_SET
+        [--model MODEL] [--params PARAM_FILE]
+        [--ls LEARNING_SET] [--label] [--threads THREADS]
+    pypef hybrid --model MODEL --params PARAM_FILE
+        [--ts TEST_SET] [--label]
+        [--ps PREDICTION_SET] [--pmult] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
+                                        [--ddiverse] [--tdiverse] [--qdiverse] [--negative]
+        [--threads THREADS]
+    pypef hybrid directevo --wt WT_FASTA --params PARAM_FILE
+        [--model MODEL]
+        [--input CSV_FILE] [--y_wt WT_FITNESS] [--numiter NUM_ITER]
+        [--numtraj NUM_TRAJ] [--temp TEMPERATURE]
+        [--negative] [--usecsv] [--csvaa] [--drop THRESHOLD]
+    pypef hybrid train_and_save --input CSV_FILE --params PARAM_FILE --wt WT_FASTA
+        [--fit_size REL_LEARN_FIT_SIZE] [--test_size REL_TEST_SIZE]
+        [--threads THREADS] [--sep CSV_COLUMN_SEPARATOR]
+        [--fitness_key FITNESS_KEY] [--rnd_state RND_STATE]
+    pypef hybrid low_n --input ENCODED_CSV_FILE
+    pypef hybrid extrapolation --input ENCODED_CSV_FILE
+        [--conc]
+    pypef ml --encoding ENCODING_TECHNIQUE --ls LEARNING_SET --ts TEST_SET
+        [--save NUMBER] [--regressor TYPE] [--nofft] [--all] [--params PARAM_FILE]
+        [--sort METRIC_INT] [--threads THREADS] [--label]
+    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL --ts TEST_SET
+        [--nofft] [--params PARAM_FILE] [--threads THREADS] [--label]
+    pypef ml --show
+        [MODELS]
+    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL --ps PREDICTION_SET
+        [--params PARAM_FILE] [--threads THREADS] [--nofft] [--negative]
+    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL --pmult
+        [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
+        [--ddiverse] [--tdiverse] [--qdiverse]
+        [--regressor TYPE] [--nofft] [--negative] [--params PARAM_FILE] [--threads THREADS]
+    pypef ml --encoding ENCODING_TECHNIQUE directevo --model MODEL --wt WT_FASTA
+        [--input CSV_FILE] [--y_wt WT_FITNESS] [--numiter NUM_ITER] [--numtraj NUM_TRAJ] [--temp TEMPERATURE]
+        [--nofft] [--negative] [--usecsv] [--csvaa] [--drop THRESHOLD] [--params PARAM_FILE]
+    pypef ml low_n --input ENCODED_CSV_FILE
+        [--regressor TYPE]
+    pypef ml extrapolation --input ENCODED_CSV_FILE
+        [--regressor TYPE] [--conc]
+
+
+Options:
+  --all                             Finally training on all data [default: False].
+  --conc                            Concatenating mutational level variants for predicting variants
+                                    from next higher level [default: False].
+  --csvaa                           Directed evolution csv amino acid substitutions,
+                                    requires flag "--usecsv" [default: False].
+  --ddiverse                        Create/predict double natural diverse variants [default: False].
+  --drecomb                         Create/predict double recombinants [default: False].
+  -d --drop THRESHOLD               Below threshold variants will be discarded from the
+                                    data [default: -9E09].
+  -e --encoding ENCODING_TECHNIQUE  Sets technique used for encoding sequences for constructing regression models;
+                                    choose between 'aaidx' (AAIndex-based encoding), 'onehot' (OneHot-based encoding),
+                                    and DCA encoding using Gremlin/plmc (DCA-based encoding) [default: onehot].
+  --fitness_key FITNESS_KEY         Label of CSV fitness column. Else uses second column.
+  -h --help                         Show this screen [default: False].
+  -i --input CSV_FILE               Input data file in .csv format.
+  --inter_gap INTER_GAP             Fraction to delete all positions with more than
+                                    'inter_gap' * 100 % gaps (columnar trimming) [default: 0.3].
+  --intra_gap INTRA_GAP             Fraction to delete all sequences with more than
+                                    'intra_gap' * 100 % gaps after being columnar trimmed
+                                    (line trimming) [default: 0.5].
+  --label                           Label the plot instances [default: False].
+  -l --ls LEARNING_SET              Input learning set in .fasta format.
+  -m --model MODEL                  Model (pickle file) for plotting of validation or for
+                                    performing predictions.
+  --msa MSA_FILE                    Multiple sequence alignment (MSA) ins FASTA or A2M format for
+                                    inferring DCA parameters.
+  --mutation_sep MUTATION_SEP       Mutation separator [default: /].
+  --mutation_extrapolation          Mutation extrapolation [default: False].
+  --negative                        Set if more negative values define better variants [default: False].
+  --nofft                           Raw sequence input, i.e., no FFT for establishing protein spectra
+                                    as vector inputs, only implemented as option for AAindex-based
+                                    sequence encoding [default: False].
+  -n --numrnd NUMBER                Number of randomly created Learning and Validation
+                                    datasets [default: 0].
+  --numiter NUM_ITER                Number of mutation iterations per evolution trajectory [default: 5].
+  --numtraj NUM_TRAJ                Number of trajectories, i.e., evolution pathways [default: 5].
+  -o --offset OFFSET                Offset for shifting substitution positions of the input CSV file [default: 0].
+  --opt_iter N_ITER                 Number of iterations for GREMLIN-based optimization of local fields
+                                    and couplings [default: 100].
+  --params PARAM_FILE               Input PLMC couplings parameter file.
+  -u --pmult                        Predict for all prediction files in folder for recombinants
+                                    or for diverse variants [default: False].
+  -p --ps PREDICTION_SET            Prediction set for performing predictions using a trained Model.
+  --qdiverse                        Create quadruple natural diverse variants [default: False].
+  --qarecomb                        Create/predict quadruple recombinants [default: False].
+  --qirecomb                        Create/predict quintuple recombinants [default: False].
+  --regressor TYPE                  Type of regression (R.) to use, options: PLS CV R.: pls,
+                                    PLS LOOCV R.: pls_loocv, Random Forest CV R.: rf, SVM CV R.: svr,
+                                    MLP CV R.: mlp, Ridge CV R.: ridge (or l2),
+                                    LassoLars CV R.: lassolars (or l1) [default: pls].
+  --rnd_splits RND_SPLITS           Number of random splits for Low N testing [default: 5].
+  --rnd_state RND_STATE             Sets the random state for reproduction, only implemented
+                                    for hybrid train_and_save [default: 42].
+  -s --save NUMBER                  Number of models to be saved as pickle files [default: 5].
+  --sep CSV_COLUMN_SEPARATOR        CSV Column separator [default: ;].
+  --show                            Show achieved model performances from Model_Results.txt.
+  --sort METRIC_INT                 Rank models based on metric {1: R^2, 2: RMSE, 3: NRMSE,
+                                    4: Pearson's r, 5: Spearman's rho} [default: 1].
+  --ssm                             Create single-saturation mutagenesis prediction set (does not
+                                    require CSV input) [default: False].
+  --sto STO_MSA_FILE                The input MSA file in STO (Stockholm) format.
+  --tdiverse                        Create/predict triple natural diverse variants [default: False].
+  --temp TEMPERATURE                "Temperature" of Metropolis-Hastings criterion [default: 0.01]
+  --threads THREADS                 Parallel computing of training and validation of models.
+                                    Number of threads used in parallel computing, by default
+                                    no hyperthreading.
+  --fit_size REL_LEARN_FIT_SIZE     Relative size of the train set for initial fitting. The remaining data
+                                    for training is used for hyperparameter optimization on train subsets
+                                    used for validation, while in sum the total data for training is
+                                    training data = train_fit data + train_test(validation) data
+                                                  = all data - test data.
+                                    The default of 0.66 means that 34 % of the train data is taken for
+                                    train_test validation [default: 0.66].
+  --test_size REL_TEST_SIZE         Relative size of the test set; if set to 0.0 the trained model
+                                    will not be tested [default: 0.2].
+  --trecomb                         Create/predict triple recombinants [default: False].
+  --usecsv                          Perform directed evolution on single variant csv position
+                                    data [default: False].
+  -t --ts TEST_SET                  Input validation set in .fasta format.
+  --version                         Show version [default: False].
+  -w --wt WT_FASTA                  Input wild-type sequence file (in FASTA format).
+  --wt_pos WT_POSITION              Row position of encoded wild-type in encoding CSV file (0-indexed) [default: 0].
+  -y --y_wt WT_FITNESS              Fitness value (y) of wild-type [default: 1.0].
+  encode                            Encoding [default: False].
+  hybrid                            Hybrid modeling based on DCA-derived sequence encoding [default: False].
+  ml                                Pure machine learning modeling based on encoded sequences [default: False].
+  MODELS                            Number of saved models to show [default: 5].
+  onehot                            OneHot-based encoding [default: False].
+  param_inference                   Inferring DCA params using the GREMLIN approach [default: False].
+  reformat_csv                      Reformat input CSV with indicated column and mutation separators to default
+                                    CSV style (column separator ';' and mutation separator '/') [default: False.]
+  save_msa_info                     Optimize local fields and couplings of MSA based on GREMLIN DCA approach and
+                                    save resulting coupling matrix and highly coevolved amino acids.
+  shift_pos                         Shift positions of all variant substitutions of the input CSV
+                                    file (identical to reformat_csv when setting --offset to 0) [default: False.]
+  sto2a2m                           Transform multiple sequence alignment from STO format to
+                                    A2M format [default: False].
+"""
+
+
+from os import environ
+try:
+    environ['TF_CPP_MIN_LOG_LEVEL'] = '2'  # only print TensorFlow errors, set to '0' or comment
+except KeyError:                           # lines for seeing TensorFlow infos and warnings
+    pass
+
+from sys import argv, version_info
+from pypef import __version__
+if version_info[0] < 3 or version_info[1] < 9:
+    raise SystemError(f"The current version of PyPEF (v {__version__}) "
+                      f"requires at least Python 3.9 or higher.")
+
+import time
+from datetime import timedelta
+import logging
+
+from docopt import docopt
+from schema import Schema, SchemaError, Optional, Or, Use
+
+from pypef.ml.ml_run import run_pypef_pure_ml
+from pypef.dca.dca_run import run_pypef_hybrid_modeling
+from pypef.utils.utils_run import run_pypef_utils
+
+logger = logging.getLogger("pypef")
+logger.setLevel(logging.INFO)
+
+ch = logging.StreamHandler()
+ch.setLevel(logging.DEBUG)
+
+formatter = logging.Formatter(
+    "%(asctime)s.%(msecs)03d %(levelname)s %(filename)s:%(lineno)d -- %(message)s",
+    "%Y-%m-%d %H:%M:%S"
+)
+ch.setFormatter(formatter)
+logger.addHandler(ch)
+
+
+schema = Schema({
+    Optional('--all'): bool,
+    Optional('--conc'): bool,
+    Optional('--csvaa'): bool,
+    Optional('--ddiverse'): bool,
+    Optional('--drecomb'): bool,
+    Optional('--drop'): Use(float),
+    Optional('--encoding'): Use(str),
+    Optional('--fitness_key'): Or(None, str),
+    Optional('--fit_size'): Use(float),
+    Optional('--help'): bool,
+    Optional('--input'): Or(None, str),
+    Optional('--inter_gap'): Use(float),
+    Optional('--intra_gap'): Use(float),
+    Optional('--label'): bool,
+    Optional('--ls'): Or(None, str),
+    Optional('--model'): Or(None, str),
+    Optional('--msa'): Or(None, str),
+    Optional('--mutation_sep'): Or(None, str),
+    Optional('--negative'): bool,
+    Optional('--nofft'): bool,
+    Optional('--numrnd'): Use(int),
+    Optional('--numiter'): Use(int),
+    Optional('--numtraj'): Use(int),
+    Optional('--offset'): Use(int),
+    Optional('--opt_iter'): Use(int),
+    Optional('--params'): Or(None, str),
+    Optional('--pmult'): bool,
+    Optional('--ps'): Or(None, str),
+    Optional('--qdiverse'): bool,
+    Optional('--qarecomb'): bool,
+    Optional('--qirecomb'): bool,
+    Optional('--regressor'): Or(None, str),
+    Optional('--rnd_splits'): Use(int),
+    Optional('--rnd_state'): Use(int),
+    Optional('--save'): Use(int),
+    Optional('--sep'): Or(None, str),
+    Optional('--show'): Use(int),
+    Optional('--sort'): Use(int),
+    Optional('--ssm'): bool,
+    Optional('--sto'): Or(None, str),
+    Optional('--tdiverse'): bool,
+    Optional('--temp'): Use(float),
+    Optional('--test_size'): Use(float),
+    Optional('--threads'): Or(None, Use(int)),
+    Optional('--train_size'): Use(float),
+    Optional('--trecomb'): bool,
+    Optional('--usecsv'): bool,
+    Optional('--ts'): Or(None, str),
+    Optional('--wt'): Or(None, str),
+    Optional('--wt_pos'): Use(int),
+    Optional('--y_wt'): Or(None, Use(float)),
+    Optional('aaidx'): bool,
+    Optional('param_inference'): bool,
+    Optional('hybrid'): bool,
+    Optional('directevo'): bool,
+    Optional('encode'): bool,
+    Optional('extrapolation'): bool,
+    Optional('low_n'): bool,
+    Optional('mklsts'): bool,
+    Optional('mkps'): bool,
+    Optional('ml'): bool,
+    Optional('MODELS'): Or(None, Use(int)),
+    Optional('onehot'): bool,
+    Optional('reformat_csv'): bool,
+    Optional('save_msa_info'): bool,
+    Optional('shift_pos'): bool,
+    Optional('sto2a2m'): bool,
+    Optional('train_and_save'): bool,
+})
+
+
+def validate(args):
+    try:
+        args = schema.validate(args)
+        return args
+    except SchemaError as e:
+        exit(e)
+
+
+def run_main():
+    """
+    Entry point for pip-installed version.
+    """
+    arguments = docopt(__doc__, version=__version__)
+    start_time = time.time()
+    logger.debug(f'main.py __name__: {__name__}, version: {__version__}')
+    logger.debug(str(argv)[1:-1].replace("\'", "").replace(",", ""))
+    logger.debug(f'\n{arguments}')
+    arguments = validate(arguments)
+    if arguments['directevo']:
+        run_pypef_utils(arguments)
+    elif arguments['ml']:
+        run_pypef_pure_ml(arguments)
+    elif arguments['hybrid'] or arguments['param_inference'] or arguments['save_msa_info']:
+        run_pypef_hybrid_modeling(arguments)
+    else:
+        run_pypef_utils(arguments)
+
+    elapsed = str(timedelta(seconds=time.time()-start_time)).split(".")[0]
+    elapsed = f'{elapsed.split(":")[0]} h {elapsed.split(":")[1]} min {elapsed.split(":")[2]} s'
+    logger.info(f'Done! (Run time: {elapsed})')
+
+
+if __name__ == '__main__':
+    """
+    Entry point for direct file run.
+    """
+    run_main()
```

### Comparing `pypef-0.3/pypef/ml/AAindex/ANDN920101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ANDN920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ARGP820101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ARGP820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ARGP820102.txt` & `pypef-0.3.1/pypef/ml/AAindex/ARGP820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ARGP820103.txt` & `pypef-0.3.1/pypef/ml/AAindex/ARGP820103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AURR980108.txt` & `pypef-0.3.1/pypef/ml/AAindex/AURR980108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AURR980109.txt` & `pypef-0.3.1/pypef/ml/AAindex/AURR980109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AURR980110.txt` & `pypef-0.3.1/pypef/ml/AAindex/AURR980110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AURR980111.txt` & `pypef-0.3.1/pypef/ml/AAindex/AURR980111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AURR980112.txt` & `pypef-0.3.1/pypef/ml/AAindex/AURR980112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AURR980113.txt` & `pypef-0.3.1/pypef/ml/AAindex/AURR980113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AURR980114.txt` & `pypef-0.3.1/pypef/ml/AAindex/AURR980114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AURR980115.txt` & `pypef-0.3.1/pypef/ml/AAindex/AURR980115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AVBF000101.txt` & `pypef-0.3.1/pypef/ml/AAindex/AVBF000101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AVBF000102.txt` & `pypef-0.3.1/pypef/ml/AAindex/AVBF000102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AVBF000103.txt` & `pypef-0.3.1/pypef/ml/AAindex/AVBF000103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AVBF000104.txt` & `pypef-0.3.1/pypef/ml/AAindex/AVBF000104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AVBF000105.txt` & `pypef-0.3.1/pypef/ml/AAindex/AVBF000105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AVBF000106.txt` & `pypef-0.3.1/pypef/ml/AAindex/AVBF000106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AVBF000107.txt` & `pypef-0.3.1/pypef/ml/AAindex/AVBF000107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AVBF000108.txt` & `pypef-0.3.1/pypef/ml/AAindex/AVBF000108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/AVBF000109.txt` & `pypef-0.3.1/pypef/ml/AAindex/AVBF000109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BAEK050101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BAEK050101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BASU050101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BASU050101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BASU050102.txt` & `pypef-0.3.1/pypef/ml/AAindex/BASU050102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BASU050103.txt` & `pypef-0.3.1/pypef/ml/AAindex/BASU050103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BEGF750101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BEGF750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BEGF750102.txt` & `pypef-0.3.1/pypef/ml/AAindex/BEGF750102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BEGF750103.txt` & `pypef-0.3.1/pypef/ml/AAindex/BEGF750103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BHAR880101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BHAR880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BIGC670101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BIGC670101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BIOV880101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BIOV880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BIOV880102.txt` & `pypef-0.3.1/pypef/ml/AAindex/BIOV880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BLAM930101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BLAM930101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BLAS910101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BLAS910101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BROC820101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BROC820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BROC820102.txt` & `pypef-0.3.1/pypef/ml/AAindex/BROC820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BULH740101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BULH740101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BULH740102.txt` & `pypef-0.3.1/pypef/ml/AAindex/BULH740102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BUNA790101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BUNA790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BUNA790102.txt` & `pypef-0.3.1/pypef/ml/AAindex/BUNA790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BUNA790103.txt` & `pypef-0.3.1/pypef/ml/AAindex/BUNA790103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BURA740101.txt` & `pypef-0.3.1/pypef/ml/AAindex/BURA740101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/BURA740102.txt` & `pypef-0.3.1/pypef/ml/AAindex/BURA740102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CASG920101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CASG920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CEDJ970101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CEDJ970101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CEDJ970102.txt` & `pypef-0.3.1/pypef/ml/AAindex/CEDJ970102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CEDJ970103.txt` & `pypef-0.3.1/pypef/ml/AAindex/CEDJ970103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CEDJ970104.txt` & `pypef-0.3.1/pypef/ml/AAindex/CEDJ970104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CEDJ970105.txt` & `pypef-0.3.1/pypef/ml/AAindex/CEDJ970105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM810101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM820101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM820102.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM830101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM830102.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM830102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM830103.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM830103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM830104.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM830104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM830105.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM830105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM830106.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM830106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM830107.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM830107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHAM830108.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHAM830108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOC750101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOC750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOC760101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOC760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOC760102.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOC760102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOC760103.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOC760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOC760104.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOC760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780201.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780201.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780202.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780202.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780203.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780203.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780204.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780204.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780205.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780205.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780206.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780206.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780207.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780207.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780208.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780208.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780209.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780209.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780210.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780210.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780211.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780211.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780212.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780212.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780213.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780213.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780214.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780214.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780215.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780215.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CHOP780216.txt` & `pypef-0.3.1/pypef/ml/AAindex/CHOP780216.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CIDH920101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CIDH920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CIDH920102.txt` & `pypef-0.3.1/pypef/ml/AAindex/CIDH920102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CIDH920103.txt` & `pypef-0.3.1/pypef/ml/AAindex/CIDH920103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CIDH920104.txt` & `pypef-0.3.1/pypef/ml/AAindex/CIDH920104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CIDH920105.txt` & `pypef-0.3.1/pypef/ml/AAindex/CIDH920105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CORJ870101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CORJ870101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CORJ870102.txt` & `pypef-0.3.1/pypef/ml/AAindex/CORJ870102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CORJ870103.txt` & `pypef-0.3.1/pypef/ml/AAindex/CORJ870103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CORJ870104.txt` & `pypef-0.3.1/pypef/ml/AAindex/CORJ870104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CORJ870105.txt` & `pypef-0.3.1/pypef/ml/AAindex/CORJ870105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CORJ870106.txt` & `pypef-0.3.1/pypef/ml/AAindex/CORJ870106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CORJ870107.txt` & `pypef-0.3.1/pypef/ml/AAindex/CORJ870107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CORJ870108.txt` & `pypef-0.3.1/pypef/ml/AAindex/CORJ870108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/COSI940101.txt` & `pypef-0.3.1/pypef/ml/AAindex/COSI940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/COWR900101.txt` & `pypef-0.3.1/pypef/ml/AAindex/COWR900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CRAJ730101.txt` & `pypef-0.3.1/pypef/ml/AAindex/CRAJ730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CRAJ730102.txt` & `pypef-0.3.1/pypef/ml/AAindex/CRAJ730102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/CRAJ730103.txt` & `pypef-0.3.1/pypef/ml/AAindex/CRAJ730103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/DAWD720101.txt` & `pypef-0.3.1/pypef/ml/AAindex/DAWD720101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/DAYM780101.txt` & `pypef-0.3.1/pypef/ml/AAindex/DAYM780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/DAYM780201.txt` & `pypef-0.3.1/pypef/ml/AAindex/DAYM780201.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/DESM900101.txt` & `pypef-0.3.1/pypef/ml/AAindex/DESM900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/DESM900102.txt` & `pypef-0.3.1/pypef/ml/AAindex/DESM900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/DIGM050101.txt` & `pypef-0.3.1/pypef/ml/AAindex/DIGM050101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/EISD840101.txt` & `pypef-0.3.1/pypef/ml/AAindex/EISD840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/EISD860101.txt` & `pypef-0.3.1/pypef/ml/AAindex/EISD860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/EISD860102.txt` & `pypef-0.3.1/pypef/ml/AAindex/EISD860102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/EISD860103.txt` & `pypef-0.3.1/pypef/ml/AAindex/EISD860103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ENGD860101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ENGD860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FASG760101.txt` & `pypef-0.3.1/pypef/ml/AAindex/FASG760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FASG890101.txt` & `pypef-0.3.1/pypef/ml/AAindex/FASG890101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ830101.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880101.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880102.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880103.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880104.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880105.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880106.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880107.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880108.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880109.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880110.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880111.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880112.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FAUJ880113.txt` & `pypef-0.3.1/pypef/ml/AAindex/FAUJ880113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FINA770101.txt` & `pypef-0.3.1/pypef/ml/AAindex/FINA770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FINA910101.txt` & `pypef-0.3.1/pypef/ml/AAindex/FINA910101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FINA910102.txt` & `pypef-0.3.1/pypef/ml/AAindex/FINA910102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FINA910103.txt` & `pypef-0.3.1/pypef/ml/AAindex/FINA910103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FINA910104.txt` & `pypef-0.3.1/pypef/ml/AAindex/FINA910104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FODM020101.txt` & `pypef-0.3.1/pypef/ml/AAindex/FODM020101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010101.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010102.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010103.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010104.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010105.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010106.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010107.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010108.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010109.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010110.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010111.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/FUKS010112.txt` & `pypef-0.3.1/pypef/ml/AAindex/FUKS010112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GARJ730101.txt` & `pypef-0.3.1/pypef/ml/AAindex/GARJ730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800101.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800102.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800104.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800105.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800106.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800107.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800108.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800109.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800110.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEIM800111.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEIM800111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEOR030101.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEOR030101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEOR030102.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEOR030102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEOR030103.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEOR030103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEOR030104.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEOR030104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEOR030105.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEOR030105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEOR030106.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEOR030106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEOR030107.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEOR030107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEOR030108.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEOR030108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GEOR030109.txt` & `pypef-0.3.1/pypef/ml/AAindex/GEOR030109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GOLD730101.txt` & `pypef-0.3.1/pypef/ml/AAindex/GOLD730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GOLD730102.txt` & `pypef-0.3.1/pypef/ml/AAindex/GOLD730102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GRAR740102.txt` & `pypef-0.3.1/pypef/ml/AAindex/GRAR740102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GRAR740103.txt` & `pypef-0.3.1/pypef/ml/AAindex/GRAR740103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GUOD860101.txt` & `pypef-0.3.1/pypef/ml/AAindex/GUOD860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GUYH850101.txt` & `pypef-0.3.1/pypef/ml/AAindex/GUYH850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GUYH850102.txt` & `pypef-0.3.1/pypef/ml/AAindex/GUYH850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GUYH850103.txt` & `pypef-0.3.1/pypef/ml/AAindex/GUYH850103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GUYH850104.txt` & `pypef-0.3.1/pypef/ml/AAindex/GUYH850104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/GUYH850105.txt` & `pypef-0.3.1/pypef/ml/AAindex/GUYH850105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/HARY940101.txt` & `pypef-0.3.1/pypef/ml/AAindex/HARY940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/HOPA770101.txt` & `pypef-0.3.1/pypef/ml/AAindex/HOPA770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/HOPT810101.txt` & `pypef-0.3.1/pypef/ml/AAindex/HOPT810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/HUTJ700101.txt` & `pypef-0.3.1/pypef/ml/AAindex/HUTJ700101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/HUTJ700102.txt` & `pypef-0.3.1/pypef/ml/AAindex/HUTJ700102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/HUTJ700103.txt` & `pypef-0.3.1/pypef/ml/AAindex/HUTJ700103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ISOY800101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ISOY800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ISOY800102.txt` & `pypef-0.3.1/pypef/ml/AAindex/ISOY800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ISOY800103.txt` & `pypef-0.3.1/pypef/ml/AAindex/ISOY800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ISOY800104.txt` & `pypef-0.3.1/pypef/ml/AAindex/ISOY800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ISOY800105.txt` & `pypef-0.3.1/pypef/ml/AAindex/ISOY800105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ISOY800106.txt` & `pypef-0.3.1/pypef/ml/AAindex/ISOY800106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ISOY800107.txt` & `pypef-0.3.1/pypef/ml/AAindex/ISOY800107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ISOY800108.txt` & `pypef-0.3.1/pypef/ml/AAindex/ISOY800108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JACR890101.txt` & `pypef-0.3.1/pypef/ml/AAindex/JACR890101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JANJ780101.txt` & `pypef-0.3.1/pypef/ml/AAindex/JANJ780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JANJ780102.txt` & `pypef-0.3.1/pypef/ml/AAindex/JANJ780102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JANJ780103.txt` & `pypef-0.3.1/pypef/ml/AAindex/JANJ780103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JANJ790101.txt` & `pypef-0.3.1/pypef/ml/AAindex/JANJ790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JANJ790102.txt` & `pypef-0.3.1/pypef/ml/AAindex/JANJ790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JOND750101.txt` & `pypef-0.3.1/pypef/ml/AAindex/JOND750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JOND750102.txt` & `pypef-0.3.1/pypef/ml/AAindex/JOND750102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JOND920101.txt` & `pypef-0.3.1/pypef/ml/AAindex/JOND920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JUKT750101.txt` & `pypef-0.3.1/pypef/ml/AAindex/JUKT750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JUNJ780101.txt` & `pypef-0.3.1/pypef/ml/AAindex/JUNJ780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/JURD980101.txt` & `pypef-0.3.1/pypef/ml/AAindex/JURD980101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KANM800101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KANM800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KANM800102.txt` & `pypef-0.3.1/pypef/ml/AAindex/KANM800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KANM800103.txt` & `pypef-0.3.1/pypef/ml/AAindex/KANM800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KANM800104.txt` & `pypef-0.3.1/pypef/ml/AAindex/KANM800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARP850101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARP850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARP850102.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARP850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160102.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160103.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160104.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160105.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160106.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160107.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160108.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160109.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160110.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160111.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160112.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160113.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160114.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160115.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160116.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160116.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160117.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160117.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160118.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160118.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160119.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160119.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160120.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160120.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160121.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160121.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KARS160122.txt` & `pypef-0.3.1/pypef/ml/AAindex/KARS160122.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KIDA850101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KIDA850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KIMC930101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KIMC930101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KLEP840101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KLEP840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KOEP990101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KOEP990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KRIW710101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KRIW710101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KRIW790101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KRIW790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KRIW790102.txt` & `pypef-0.3.1/pypef/ml/AAindex/KRIW790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KRIW790103.txt` & `pypef-0.3.1/pypef/ml/AAindex/KRIW790103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KUHL950101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KUHL950101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KUMS000101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KUMS000101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KUMS000102.txt` & `pypef-0.3.1/pypef/ml/AAindex/KUMS000102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KUMS000103.txt` & `pypef-0.3.1/pypef/ml/AAindex/KUMS000103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KUMS000104.txt` & `pypef-0.3.1/pypef/ml/AAindex/KUMS000104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/KYTJ820101.txt` & `pypef-0.3.1/pypef/ml/AAindex/KYTJ820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LAWE840101.txt` & `pypef-0.3.1/pypef/ml/AAindex/LAWE840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM760101.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM760102.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM760102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM760103.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM760104.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM760105.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM760105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM760106.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM760106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM760107.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM760107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM780101.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM780102.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM780102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM780103.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM780103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM780104.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM780104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM780105.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM780105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEVM780106.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEVM780106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LEWP710101.txt` & `pypef-0.3.1/pypef/ml/AAindex/LEWP710101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LIFS790101.txt` & `pypef-0.3.1/pypef/ml/AAindex/LIFS790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LIFS790102.txt` & `pypef-0.3.1/pypef/ml/AAindex/LIFS790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/LIFS790103.txt` & `pypef-0.3.1/pypef/ml/AAindex/LIFS790103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MANP780101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MANP780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MAXF760101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MAXF760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MAXF760102.txt` & `pypef-0.3.1/pypef/ml/AAindex/MAXF760102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MAXF760103.txt` & `pypef-0.3.1/pypef/ml/AAindex/MAXF760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MAXF760104.txt` & `pypef-0.3.1/pypef/ml/AAindex/MAXF760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MAXF760105.txt` & `pypef-0.3.1/pypef/ml/AAindex/MAXF760105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MAXF760106.txt` & `pypef-0.3.1/pypef/ml/AAindex/MAXF760106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MCMT640101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MCMT640101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MEEJ800101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MEEJ800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MEEJ800102.txt` & `pypef-0.3.1/pypef/ml/AAindex/MEEJ800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MEEJ810101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MEEJ810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MEEJ810102.txt` & `pypef-0.3.1/pypef/ml/AAindex/MEEJ810102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MEIH800101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MEIH800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MEIH800102.txt` & `pypef-0.3.1/pypef/ml/AAindex/MEIH800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MEIH800103.txt` & `pypef-0.3.1/pypef/ml/AAindex/MEIH800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MITS020101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MITS020101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MIYS850101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MIYS850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MIYS990101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MIYS990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MIYS990102.txt` & `pypef-0.3.1/pypef/ml/AAindex/MIYS990102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MIYS990103.txt` & `pypef-0.3.1/pypef/ml/AAindex/MIYS990103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MIYS990104.txt` & `pypef-0.3.1/pypef/ml/AAindex/MIYS990104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MIYS990105.txt` & `pypef-0.3.1/pypef/ml/AAindex/MIYS990105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MONM990101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MONM990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MONM990201.txt` & `pypef-0.3.1/pypef/ml/AAindex/MONM990201.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MUNV940101.txt` & `pypef-0.3.1/pypef/ml/AAindex/MUNV940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MUNV940102.txt` & `pypef-0.3.1/pypef/ml/AAindex/MUNV940102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MUNV940103.txt` & `pypef-0.3.1/pypef/ml/AAindex/MUNV940103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MUNV940104.txt` & `pypef-0.3.1/pypef/ml/AAindex/MUNV940104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/MUNV940105.txt` & `pypef-0.3.1/pypef/ml/AAindex/MUNV940105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NADH010101.txt` & `pypef-0.3.1/pypef/ml/AAindex/NADH010101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NADH010102.txt` & `pypef-0.3.1/pypef/ml/AAindex/NADH010102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NADH010103.txt` & `pypef-0.3.1/pypef/ml/AAindex/NADH010103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NADH010104.txt` & `pypef-0.3.1/pypef/ml/AAindex/NADH010104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NADH010105.txt` & `pypef-0.3.1/pypef/ml/AAindex/NADH010105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NADH010106.txt` & `pypef-0.3.1/pypef/ml/AAindex/NADH010106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NADH010107.txt` & `pypef-0.3.1/pypef/ml/AAindex/NADH010107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAGK730101.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAGK730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAGK730102.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAGK730102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAGK730103.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAGK730103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900101.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900102.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900103.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900104.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900105.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900106.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900107.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900108.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900109.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900110.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900111.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900112.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH900113.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH900113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH920101.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH920102.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH920102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH920103.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH920103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH920104.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH920104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH920105.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH920105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH920106.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH920106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH920107.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH920107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NAKH920108.txt` & `pypef-0.3.1/pypef/ml/AAindex/NAKH920108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NISK800101.txt` & `pypef-0.3.1/pypef/ml/AAindex/NISK800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NISK860101.txt` & `pypef-0.3.1/pypef/ml/AAindex/NISK860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/NOZY710101.txt` & `pypef-0.3.1/pypef/ml/AAindex/NOZY710101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OLSK800101.txt` & `pypef-0.3.1/pypef/ml/AAindex/OLSK800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ONEK900101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ONEK900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ONEK900102.txt` & `pypef-0.3.1/pypef/ml/AAindex/ONEK900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM770101.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM770102.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM770102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM770103.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM770103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM770104.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM770104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM770105.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM770105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM850101.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM850102.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM850103.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM850103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM850104.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM850104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/OOBM850105.txt` & `pypef-0.3.1/pypef/ml/AAindex/OOBM850105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810102.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810103.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810104.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810105.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810106.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810107.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810108.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810109.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810110.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810111.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810112.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810113.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810114.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810115.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PALJ810116.txt` & `pypef-0.3.1/pypef/ml/AAindex/PALJ810116.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PARJ860101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PARJ860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PARS000101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PARS000101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PARS000102.txt` & `pypef-0.3.1/pypef/ml/AAindex/PARS000102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PLIV810101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PLIV810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONJ960101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONJ960101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONP800101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONP800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONP800102.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONP800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONP800103.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONP800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONP800104.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONP800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONP800105.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONP800105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONP800106.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONP800106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONP800107.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONP800107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONP800108.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONP800108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PONP930101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PONP930101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PRAM820101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PRAM820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PRAM820102.txt` & `pypef-0.3.1/pypef/ml/AAindex/PRAM820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PRAM820103.txt` & `pypef-0.3.1/pypef/ml/AAindex/PRAM820103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PRAM900101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PRAM900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PRAM900102.txt` & `pypef-0.3.1/pypef/ml/AAindex/PRAM900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PRAM900103.txt` & `pypef-0.3.1/pypef/ml/AAindex/PRAM900103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PRAM900104.txt` & `pypef-0.3.1/pypef/ml/AAindex/PRAM900104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PTIO830101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PTIO830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PTIO830102.txt` & `pypef-0.3.1/pypef/ml/AAindex/PTIO830102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PUNT030101.txt` & `pypef-0.3.1/pypef/ml/AAindex/PUNT030101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/PUNT030102.txt` & `pypef-0.3.1/pypef/ml/AAindex/PUNT030102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880101.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880102.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880103.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880104.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880105.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880106.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880107.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880108.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880109.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880110.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880111.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880112.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880113.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880114.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880115.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880116.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880116.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880117.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880117.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880118.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880118.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880119.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880119.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880120.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880120.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880121.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880121.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880122.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880122.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880123.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880123.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880124.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880124.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880125.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880125.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880126.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880126.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880127.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880127.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880128.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880128.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880129.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880129.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880130.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880130.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880131.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880131.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880132.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880132.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880133.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880133.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880134.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880134.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880135.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880135.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880136.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880136.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880137.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880137.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880138.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880138.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/QIAN880139.txt` & `pypef-0.3.1/pypef/ml/AAindex/QIAN880139.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS770101.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS770102.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS770102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS770103.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS770103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820101.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820102.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820103.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820104.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820105.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820106.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820107.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820108.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820109.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820110.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820111.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820112.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820113.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RACS820114.txt` & `pypef-0.3.1/pypef/ml/AAindex/RACS820114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RADA880101.txt` & `pypef-0.3.1/pypef/ml/AAindex/RADA880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RADA880102.txt` & `pypef-0.3.1/pypef/ml/AAindex/RADA880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RADA880103.txt` & `pypef-0.3.1/pypef/ml/AAindex/RADA880103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RADA880104.txt` & `pypef-0.3.1/pypef/ml/AAindex/RADA880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RADA880105.txt` & `pypef-0.3.1/pypef/ml/AAindex/RADA880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RADA880106.txt` & `pypef-0.3.1/pypef/ml/AAindex/RADA880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RADA880107.txt` & `pypef-0.3.1/pypef/ml/AAindex/RADA880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RADA880108.txt` & `pypef-0.3.1/pypef/ml/AAindex/RADA880108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RICJ880101.txt` & `pypef-0.3.1/pypef/ml/AAindex/RICJ880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RICJ880102.txt` & `pypef-0.3.1/pypef/ml/AAindex/RICJ880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RICJ880106.txt` & `pypef-0.3.1/pypef/ml/AAindex/RICJ880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RICJ880107.txt` & `pypef-0.3.1/pypef/ml/AAindex/RICJ880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RICJ880109.txt` & `pypef-0.3.1/pypef/ml/AAindex/RICJ880109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RICJ880111.txt` & `pypef-0.3.1/pypef/ml/AAindex/RICJ880111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/RICJ880115.txt` & `pypef-0.3.1/pypef/ml/AAindex/RICJ880115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB760101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB760103.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB760104.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB760105.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB760105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB760106.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB760106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB760108.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB760108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB760110.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB760110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB760112.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB760112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB760113.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB760113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROBB790101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROBB790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROSG850101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROSG850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROSG850102.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROSG850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROSM880101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROSM880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROSM880102.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROSM880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROSM880104.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROSM880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ROSM880105.txt` & `pypef-0.3.1/pypef/ml/AAindex/ROSM880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/SIMZ760101.txt` & `pypef-0.3.1/pypef/ml/AAindex/SIMZ760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/SNEP660103.txt` & `pypef-0.3.1/pypef/ml/AAindex/SNEP660103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/SUEM840101.txt` & `pypef-0.3.1/pypef/ml/AAindex/SUEM840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/SUEM840102.txt` & `pypef-0.3.1/pypef/ml/AAindex/SUEM840102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/SWER830101.txt` & `pypef-0.3.1/pypef/ml/AAindex/SWER830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TAKK010101.txt` & `pypef-0.3.1/pypef/ml/AAindex/TAKK010101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770101.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770102.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770103.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770104.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770105.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770106.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770107.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770108.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770109.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TANS770110.txt` & `pypef-0.3.1/pypef/ml/AAindex/TANS770110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TSAJ990101.txt` & `pypef-0.3.1/pypef/ml/AAindex/TSAJ990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/TSAJ990102.txt` & `pypef-0.3.1/pypef/ml/AAindex/TSAJ990102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VASM830101.txt` & `pypef-0.3.1/pypef/ml/AAindex/VASM830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VASM830102.txt` & `pypef-0.3.1/pypef/ml/AAindex/VASM830102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VASM830103.txt` & `pypef-0.3.1/pypef/ml/AAindex/VASM830103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VELV850101.txt` & `pypef-0.3.1/pypef/ml/AAindex/VELV850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VENT840101.txt` & `pypef-0.3.1/pypef/ml/AAindex/VENT840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VHEG790101.txt` & `pypef-0.3.1/pypef/ml/AAindex/VHEG790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VINM940101.txt` & `pypef-0.3.1/pypef/ml/AAindex/VINM940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VINM940102.txt` & `pypef-0.3.1/pypef/ml/AAindex/VINM940102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VINM940103.txt` & `pypef-0.3.1/pypef/ml/AAindex/VINM940103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/VINM940104.txt` & `pypef-0.3.1/pypef/ml/AAindex/VINM940104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WARP780101.txt` & `pypef-0.3.1/pypef/ml/AAindex/WARP780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WEBA780101.txt` & `pypef-0.3.1/pypef/ml/AAindex/WEBA780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WERD780101.txt` & `pypef-0.3.1/pypef/ml/AAindex/WERD780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WERD780102.txt` & `pypef-0.3.1/pypef/ml/AAindex/WERD780102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WERD780103.txt` & `pypef-0.3.1/pypef/ml/AAindex/WERD780103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WERD780104.txt` & `pypef-0.3.1/pypef/ml/AAindex/WERD780104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WILM950101.txt` & `pypef-0.3.1/pypef/ml/AAindex/WILM950101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WILM950102.txt` & `pypef-0.3.1/pypef/ml/AAindex/WILM950102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WILM950103.txt` & `pypef-0.3.1/pypef/ml/AAindex/WILM950103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WILM950104.txt` & `pypef-0.3.1/pypef/ml/AAindex/WILM950104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WIMW960101.txt` & `pypef-0.3.1/pypef/ml/AAindex/WIMW960101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WOEC730101.txt` & `pypef-0.3.1/pypef/ml/AAindex/WOEC730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WOLR790101.txt` & `pypef-0.3.1/pypef/ml/AAindex/WOLR790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WOLR810101.txt` & `pypef-0.3.1/pypef/ml/AAindex/WOLR810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WOLS870101.txt` & `pypef-0.3.1/pypef/ml/AAindex/WOLS870101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WOLS870102.txt` & `pypef-0.3.1/pypef/ml/AAindex/WOLS870102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/WOLS870103.txt` & `pypef-0.3.1/pypef/ml/AAindex/WOLS870103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/YANJ020101.txt` & `pypef-0.3.1/pypef/ml/AAindex/YANJ020101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/YUTK870101.txt` & `pypef-0.3.1/pypef/ml/AAindex/YUTK870101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/YUTK870102.txt` & `pypef-0.3.1/pypef/ml/AAindex/YUTK870102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/YUTK870103.txt` & `pypef-0.3.1/pypef/ml/AAindex/YUTK870103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/YUTK870104.txt` & `pypef-0.3.1/pypef/ml/AAindex/YUTK870104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ZASB820101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ZASB820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ZHOH040101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ZHOH040101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ZHOH040102.txt` & `pypef-0.3.1/pypef/ml/AAindex/ZHOH040102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ZHOH040103.txt` & `pypef-0.3.1/pypef/ml/AAindex/ZHOH040103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ZIMJ680101.txt` & `pypef-0.3.1/pypef/ml/AAindex/ZIMJ680101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ZIMJ680102.txt` & `pypef-0.3.1/pypef/ml/AAindex/ZIMJ680102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ZIMJ680103.txt` & `pypef-0.3.1/pypef/ml/AAindex/ZIMJ680103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ZIMJ680104.txt` & `pypef-0.3.1/pypef/ml/AAindex/ZIMJ680104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/AAindex/ZIMJ680105.txt` & `pypef-0.3.1/pypef/ml/AAindex/ZIMJ680105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/ml/ml_run.py` & `pypef-0.3.1/pypef/ml/ml_run.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,223 +1,220 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Created on 05 October 2020
-# @authors: Niklas Siedhoff, Alexander-Maurice Illig
-# @contact: <n.siedhoff@biotec.rwth-aachen.de>
-# PyPEF - Pythonic Protein Engineering Framework
-# Released under Creative Commons Attribution-NonCommercial 4.0 International Public License (CC BY-NC 4.0)
-# For more information about the license see https://creativecommons.org/licenses/by-nc/4.0/legalcode
-
-# PyPEF – An Integrated Framework for Data-Driven Protein Engineering
-# Journal of Chemical Information and Modeling, 2021, 61, 3463-3476
-# https://doi.org/10.1021/acs.jcim.1c00099
-# Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
-# 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
-# 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
-# *Corresponding author
-# §Equal contribution
-
-import os
-from os import listdir
-from os.path import isfile, join
-
-import logging
-logger = logging.getLogger('pypef.ml.ml_run')
-import ray
-from pypef.ml.parallelization import aaindex_performance_parallel
-
-# importing own modules
-from pypef.ml.regression import (
-    read_models, formatted_output, performance_list, save_model, predict, predict_ts
-)
-from pypef.utils.to_file import predictions_out
-from pypef.utils.low_n_mutation_extrapolation import low_n, performance_mutation_extrapolation
-
-
-
-def run_pypef_pure_ml(arguments):
-    """
-    Running the program, importing all required self-made modules and
-    running them dependent on user-passed input arguments using docopt
-    for argument parsing.
-    """
-    threads = abs(arguments['--threads']) if arguments['--threads'] is not None else 1
-    threads = threads + 1 if threads == 0 else threads
-    if threads > 1:
-        ray.init()
-    if arguments['--show']:
-        if arguments['MODELS'] != str(5):
-            try:
-                print(read_models(int(arguments['MODELS'])))
-            except ValueError:
-                print(read_models(5))
-            except TypeError:
-                print(read_models(5))
-        else:
-            print(read_models(5))
-
-    else:
-        if arguments['--ls'] is not None and arguments['--ts'] is not None:  # LS --> TS
-            if arguments['--model'] is None:
-                path = os.getcwd()
-                try:
-                    t_save = int(arguments['--save'])
-                except ValueError:
-                    t_save = 5
-                # Parallelization of AAindex iteration if threads is not None (but int)
-                if threads > 1 and arguments['--encoding'] == 'aaidx':
-                    logger.info(f'Using {threads} threads for parallel computing. Running...')
-                    encoding_performance_list = aaindex_performance_parallel(
-                        train_set=arguments['--ls'],
-                        test_set=arguments['--ts'],
-                        cores=threads,
-                        regressor=arguments['--regressor'],
-                        no_fft=arguments['--nofft'],
-                        sort=arguments['--sort']
-                    )
-
-                else:  # run using a single core or use onehot or DCA-based encoding for modeling
-                    encoding_performance_list = performance_list(
-                        train_set=arguments['--ls'],
-                        test_set=arguments['--ts'],
-                        encoding=arguments['--encoding'],
-                        regressor=arguments['--regressor'],
-                        no_fft=arguments['--nofft'],
-                        sort=arguments['--sort'],
-                        couplings_file=arguments['--params'],  # only for DCA
-                        threads=threads  # only for DCA
-                    )
-
-                formatted_output(
-                    performance_list=encoding_performance_list,
-                    no_fft=arguments['--nofft'],
-                    minimum_r2=-1E9
-                )
-
-                # save_model encodes variants again (possibly change)
-                save_model(
-                    path=path,
-                    performances=encoding_performance_list,
-                    training_set=arguments['--ls'],
-                    test_set=arguments['--ts'],
-                    threshold=t_save,
-                    encoding=arguments['--encoding'],
-                    regressor=arguments['--regressor'],
-                    no_fft=arguments['--nofft'],
-                    train_on_all=arguments['--all'],
-                    couplings_file=arguments['--params'],  # only for DCA
-                    threads=threads,  # only for DCA
-                    label=arguments['--label']
-                )
-
-        # Prediction of single .fasta file
-        elif arguments['--ts'] is not None and arguments['--model'] is not None:
-            predict_ts(
-                path=os.getcwd(),
-                model=arguments['--model'],
-                test_set=arguments['--ts'],
-                encoding=arguments['--encoding'],
-                no_fft=arguments['--nofft'],
-                couplings_file=arguments['--params'],  # only for DCA
-                label=arguments['--label'],
-                threads=threads
-            )
-
-        elif arguments['--ps'] is not None and arguments['--model'] is not None:
-            predictions = predict(
-                path=os.getcwd(),
-                prediction_set=arguments['--ps'],
-                model=arguments['--model'],
-                encoding=arguments['--encoding'],
-                mult_path=None,
-                no_fft=arguments['--nofft'],
-                couplings_file=arguments['--params'],  # only for DCA
-                threads=threads  # only for DCA
-            )
-            if predictions == 'skip' and not arguments['--params']:
-                raise SystemError("No couplings file provided. DCA-based sequence encoding "
-                                  "requires a (plmc or GREMLIN) parameter file.")
-            if arguments['--negative']:
-                predictions = sorted(predictions, key=lambda x: x[0], reverse=False)
-            predictions_out(
-                predictions=predictions,
-                model=arguments['--model'],
-                prediction_set=arguments['--ps']
-            )
-
-        # Prediction on recombinant/diverse variant folder data
-        elif arguments['--pmult'] and arguments['--model'] is not None:
-            path = os.getcwd()
-            recombs_total = []
-            recomb_d, recomb_t, recomb_qa, recomb_qi = \
-                '/Recomb_Double_Split/', '/Recomb_Triple_Split/', \
-                '/Recomb_Quadruple_Split/', '/Recomb_Quintuple_Split/'
-            diverse_d, diverse_t, diverse_q = \
-                '/Diverse_Double_Split/', '/Diverse_Triple_Split/', '/Diverse_Quadruple_Split/'
-            if arguments['--drecomb']:
-                recombs_total.append(recomb_d)
-            if arguments['--trecomb']:
-                recombs_total.append(recomb_t)
-            if arguments['--qarecomb']:
-                recombs_total.append(recomb_qa)
-            if arguments['--qirecomb']:
-                recombs_total.append(recomb_qi)
-            if arguments['--ddiverse']:
-                recombs_total.append(diverse_d)
-            if arguments['--tdiverse']:
-                recombs_total.append(diverse_t)
-            if arguments['--qdiverse']:
-                recombs_total.append(diverse_q)
-            if arguments['--drecomb'] is False \
-                    and arguments['--trecomb'] is False \
-                    and arguments['--qarecomb'] is False \
-                    and arguments['--qirecomb'] is False \
-                    and arguments['--ddiverse'] is False \
-                    and arguments['--tdiverse'] is False \
-                    and arguments['--qdiverse'] is False:
-                raise SystemError('Define prediction target for --pmult, e.g. --pmult --drecomb.')
-
-            for args in recombs_total:
-                predictions_total = []
-                logger.info(f'Running predictions for variant-sequence files in directory {args[1:-1]}...')
-                path_recomb = path + args
-                files = [path_recomb + f for f in listdir(path_recomb)
-                         if isfile(join(path_recomb, f)) if f.endswith('.fasta')]
-                for i, file in enumerate(files):
-                    logger.info(f'Encoding files ({i+1}/{len(files)}) for prediction...')
-                    predictions = predict(
-                        path=path,
-                        prediction_set=file,
-                        model=arguments['--model'],
-                        encoding=arguments['--encoding'],
-                        mult_path=path_recomb,
-                        no_fft=arguments['--nofft'],
-                        couplings_file=arguments['--params'],  # only for DCA
-                        threads=threads  # only for DCA
-                    )
-                    for pred in predictions:
-                        predictions_total.append(pred)  # if array gets too large?
-                predictions_total = list(dict.fromkeys(predictions_total))  # removing duplicates from list
-                if arguments['--negative']:
-                    predictions_total = sorted(predictions_total, key=lambda x: x[0], reverse=False)
-                else:
-                    predictions_total = sorted(predictions_total, key=lambda x: x[0], reverse=True)
-
-                predictions_out(
-                    predictions=predictions_total,
-                    model=arguments['--model'],
-                    prediction_set=f'Top{args[1:-1]}',
-                    path=path_recomb
-                )
-
-        elif arguments['extrapolation']:
-            performance_mutation_extrapolation(
-                encoded_csv=arguments['--input'],
-                cv_regressor=arguments['--regressor'],
-                conc=arguments['--conc']
-            )
-
-        elif arguments['low_n']:
-            low_n(
-                encoded_csv=arguments['--input'],
-                cv_regressor=arguments['--regressor']
-            )
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+# Created on 05 October 2020
+# @authors: Niklas Siedhoff, Alexander-Maurice Illig
+# @contact: <n.siedhoff@biotec.rwth-aachen.de>
+# PyPEF - Pythonic Protein Engineering Framework
+# Released under Creative Commons Attribution-NonCommercial 4.0 International Public License (CC BY-NC 4.0)
+# For more information about the license see https://creativecommons.org/licenses/by-nc/4.0/legalcode
+
+# PyPEF – An Integrated Framework for Data-Driven Protein Engineering
+# Journal of Chemical Information and Modeling, 2021, 61, 3463-3476
+# https://doi.org/10.1021/acs.jcim.1c00099
+# Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
+# 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
+# 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
+# *Corresponding author
+# §Equal contribution
+
+import os
+from os import listdir
+from os.path import isfile, join
+import ray
+import logging
+logger = logging.getLogger('pypef.ml.ml_run')
+
+from pypef.ml.parallelization import aaindex_performance_parallel
+from pypef.ml.regression import (
+    read_models, formatted_output, performance_list, save_model, predict, predict_ts
+)
+from pypef.utils.to_file import predictions_out
+from pypef.utils.low_n_mutation_extrapolation import low_n, performance_mutation_extrapolation
+
+
+def run_pypef_pure_ml(arguments):
+    """
+    Running the program, importing all required self-made modules and
+    running them dependent on user-passed input arguments using docopt
+    for argument parsing.
+    """
+    threads = abs(arguments['--threads']) if arguments['--threads'] is not None else 1
+    threads = threads + 1 if threads == 0 else threads
+    if threads > 1:
+        ray.init()
+    if arguments['--show']:
+        if arguments['MODELS'] != str(5):
+            try:
+                print(read_models(int(arguments['MODELS'])))
+            except ValueError:
+                print(read_models(5))
+            except TypeError:
+                print(read_models(5))
+        else:
+            print(read_models(5))
+
+    else:
+        if arguments['--ls'] is not None and arguments['--ts'] is not None:  # LS --> TS
+            if arguments['--model'] is None:
+                path = os.getcwd()
+                try:
+                    t_save = int(arguments['--save'])
+                except ValueError:
+                    t_save = 5
+                # Parallelization of AAindex iteration if threads is not None (but int)
+                if threads > 1 and arguments['--encoding'] == 'aaidx':
+                    logger.info(f'Using {threads} threads for parallel computing. Running...')
+                    encoding_performance_list = aaindex_performance_parallel(
+                        train_set=arguments['--ls'],
+                        test_set=arguments['--ts'],
+                        cores=threads,
+                        regressor=arguments['--regressor'],
+                        no_fft=arguments['--nofft'],
+                        sort=arguments['--sort']
+                    )
+
+                else:  # run using a single core or use onehot or DCA-based encoding for modeling
+                    encoding_performance_list = performance_list(
+                        train_set=arguments['--ls'],
+                        test_set=arguments['--ts'],
+                        encoding=arguments['--encoding'],
+                        regressor=arguments['--regressor'],
+                        no_fft=arguments['--nofft'],
+                        sort=arguments['--sort'],
+                        couplings_file=arguments['--params'],  # only for DCA
+                        threads=threads  # only for DCA
+                    )
+
+                formatted_output(
+                    performance_list=encoding_performance_list,
+                    no_fft=arguments['--nofft'],
+                    minimum_r2=-1E9
+                )
+
+                # save_model encodes variants again (possibly change)
+                save_model(
+                    path=path,
+                    performances=encoding_performance_list,
+                    training_set=arguments['--ls'],
+                    test_set=arguments['--ts'],
+                    threshold=t_save,
+                    encoding=arguments['--encoding'],
+                    regressor=arguments['--regressor'],
+                    no_fft=arguments['--nofft'],
+                    train_on_all=arguments['--all'],
+                    couplings_file=arguments['--params'],  # only for DCA
+                    threads=threads,  # only for DCA
+                    label=arguments['--label']
+                )
+
+        # Prediction of single .fasta file
+        elif arguments['--ts'] is not None and arguments['--model'] is not None:
+            predict_ts(
+                path=os.getcwd(),
+                model=arguments['--model'],
+                test_set=arguments['--ts'],
+                encoding=arguments['--encoding'],
+                no_fft=arguments['--nofft'],
+                couplings_file=arguments['--params'],  # only for DCA
+                label=arguments['--label'],
+                threads=threads
+            )
+
+        elif arguments['--ps'] is not None and arguments['--model'] is not None:
+            predictions = predict(
+                path=os.getcwd(),
+                prediction_set=arguments['--ps'],
+                model=arguments['--model'],
+                encoding=arguments['--encoding'],
+                mult_path=None,
+                no_fft=arguments['--nofft'],
+                couplings_file=arguments['--params'],  # only for DCA
+                threads=threads  # only for DCA
+            )
+            if predictions == 'skip' and not arguments['--params']:
+                raise SystemError("No couplings file provided. DCA-based sequence encoding "
+                                  "requires a (plmc or GREMLIN) parameter file.")
+            if arguments['--negative']:
+                predictions = sorted(predictions, key=lambda x: x[0], reverse=False)
+            predictions_out(
+                predictions=predictions,
+                model=arguments['--model'],
+                prediction_set=arguments['--ps']
+            )
+
+        # Prediction on recombinant/diverse variant folder data
+        elif arguments['--pmult'] and arguments['--model'] is not None:
+            path = os.getcwd()
+            recombs_total = []
+            recomb_d, recomb_t, recomb_qa, recomb_qi = \
+                '/Recomb_Double_Split/', '/Recomb_Triple_Split/', \
+                '/Recomb_Quadruple_Split/', '/Recomb_Quintuple_Split/'
+            diverse_d, diverse_t, diverse_q = \
+                '/Diverse_Double_Split/', '/Diverse_Triple_Split/', '/Diverse_Quadruple_Split/'
+            if arguments['--drecomb']:
+                recombs_total.append(recomb_d)
+            if arguments['--trecomb']:
+                recombs_total.append(recomb_t)
+            if arguments['--qarecomb']:
+                recombs_total.append(recomb_qa)
+            if arguments['--qirecomb']:
+                recombs_total.append(recomb_qi)
+            if arguments['--ddiverse']:
+                recombs_total.append(diverse_d)
+            if arguments['--tdiverse']:
+                recombs_total.append(diverse_t)
+            if arguments['--qdiverse']:
+                recombs_total.append(diverse_q)
+            if arguments['--drecomb'] is False \
+                    and arguments['--trecomb'] is False \
+                    and arguments['--qarecomb'] is False \
+                    and arguments['--qirecomb'] is False \
+                    and arguments['--ddiverse'] is False \
+                    and arguments['--tdiverse'] is False \
+                    and arguments['--qdiverse'] is False:
+                raise SystemError('Define prediction target for --pmult, e.g. --pmult --drecomb.')
+
+            for args in recombs_total:
+                predictions_total = []
+                logger.info(f'Running predictions for variant-sequence files in directory {args[1:-1]}...')
+                path_recomb = path + args
+                files = [path_recomb + f for f in listdir(path_recomb)
+                         if isfile(join(path_recomb, f)) if f.endswith('.fasta')]
+                for i, file in enumerate(files):
+                    logger.info(f'Encoding files ({i+1}/{len(files)}) for prediction...')
+                    predictions = predict(
+                        path=path,
+                        prediction_set=file,
+                        model=arguments['--model'],
+                        encoding=arguments['--encoding'],
+                        mult_path=path_recomb,
+                        no_fft=arguments['--nofft'],
+                        couplings_file=arguments['--params'],  # only for DCA
+                        threads=threads  # only for DCA
+                    )
+                    for pred in predictions:
+                        predictions_total.append(pred)  # if array gets too large?
+                predictions_total = list(dict.fromkeys(predictions_total))  # removing duplicates from list
+                if arguments['--negative']:
+                    predictions_total = sorted(predictions_total, key=lambda x: x[0], reverse=False)
+                else:
+                    predictions_total = sorted(predictions_total, key=lambda x: x[0], reverse=True)
+
+                predictions_out(
+                    predictions=predictions_total,
+                    model=arguments['--model'],
+                    prediction_set=f'Top{args[1:-1]}',
+                    path=path_recomb
+                )
+
+        elif arguments['extrapolation']:
+            performance_mutation_extrapolation(
+                encoded_csv=arguments['--input'],
+                cv_regressor=arguments['--regressor'],
+                conc=arguments['--conc']
+            )
+
+        elif arguments['low_n']:
+            low_n(
+                encoded_csv=arguments['--input'],
+                cv_regressor=arguments['--regressor']
+            )
```

### Comparing `pypef-0.3/pypef/ml/parallelization.py` & `pypef-0.3.1/pypef/ml/parallelization.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Created on 05 October 2020
-# @authors: Niklas Siedhoff, Alexander-Maurice Illig
-# @contact: <n.siedhoff@biotec.rwth-aachen.de>
-# PyPEF - Pythonic Protein Engineering Framework
-# Released under Creative Commons Attribution-NonCommercial 4.0 International Public License (CC BY-NC 4.0)
-# For more information about the license see https://creativecommons.org/licenses/by-nc/4.0/legalcode
-
-# PyPEF – An Integrated Framework for Data-Driven Protein Engineering
-# Journal of Chemical Information and Modeling, 2021, 61, 3463-3476
-# https://doi.org/10.1021/acs.jcim.1c00099
-# Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
-# 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
-# 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
-# *Corresponding author
-# §Equal contribution
-
-"""
-Validation modules from regression.py for AAindex-based encoding
-modified for parallelization of the 566 AAindices used for encoding
-with Ray, see https://docs.ray.io/en/latest/index.html.
-"""
-
-import matplotlib
-matplotlib.use('Agg')
-import os
-import ray
-import warnings
-
-from pypef.utils.variant_data import get_sequences_from_file
-from pypef.ml.regression import (
-    full_aaidx_txt_path, path_aaindex_dir, AAIndexEncoding, get_regressor_performances
-)
-
-# to handle UserWarning for PLS n_components as error and general regression module warnings
-warnings.filterwarnings(action='ignore', category=RuntimeWarning, module='sklearn')
-warnings.filterwarnings(action='ignore', category=UserWarning, module='sklearn')
-
-
-@ray.remote
-def parallel(
-        d,
-        core,
-        aa_indices,
-        train_set,
-        test_set,
-        regressor='pls',
-        no_fft=False
-):
-    """
-    Parallelization of running using the user-defined number of cores.
-    Defining the task for each core.
-    """
-    warnings.filterwarnings("ignore", category=UserWarning)
-    warnings.filterwarnings("ignore", category=RuntimeWarning)
-
-    performances = []
-    for i in range(d[core][0], d[core][1]):
-        aaindex = aa_indices[i]  # Parallelization of AAindex iteration
-        sequences_train, _, y_train = get_sequences_from_file(train_set)
-        sequences_test, _, y_test = get_sequences_from_file(test_set)
-        x_aaidx_train = AAIndexEncoding(full_aaidx_txt_path(aaindex), sequences_train)
-        x_aaidx_test = AAIndexEncoding(full_aaidx_txt_path(aaindex), sequences_test)
-
-        if not no_fft:  # X is FFT-ed of encoded alphabetical sequence
-            x_train, _ = x_aaidx_train.collect_encoded_sequences()
-            x_test, _ = x_aaidx_test.collect_encoded_sequences()
-        else:  # X is raw encoded of alphabetical sequence
-            _, x_train = x_aaidx_train.collect_encoded_sequences()
-            _, x_test = x_aaidx_test.collect_encoded_sequences()
-
-        # If x_learn (or y_learn) is an empty array, the sequence could not be encoded,
-        # because of NoneType value. -> Skip
-        if x_train == 'skip' or x_test == 'skip':
-            continue  # skip the rest and do next iteration
-        r2, rmse, nrmse, pearson_r, spearman_rho, regressor, best_params = \
-            get_regressor_performances(x_train, x_test, y_train, y_test, regressor)
-        if r2 is not None:  # None for metrics if MSE can't be calculated
-            performances.append([
-                aaindex, r2, rmse, nrmse, pearson_r, spearman_rho, regressor, best_params
-            ])
-
-    return performances
-
-
-def aaindex_performance_parallel(
-        train_set,
-        test_set,
-        cores,
-        regressor='pls',
-        no_fft=False,
-        sort='1'
-):
-    """
-    Parallelization of running using the user-defined number of cores.
-    Calling function Parallel to execute the parallel running and
-    getting the results from each core each being defined by a result ID.
-    """
-    aa_indices = [file for file in os.listdir(path_aaindex_dir()) if file.endswith('.txt')]
-
-    split = int(len(aa_indices) / cores)
-    last_split = int(len(aa_indices) % cores) + split
-
-    d = {}
-    for i in range(cores - 1):
-        d[i] = [i * split, i * split + split]
-
-    d[cores - 1] = [(cores - 1) * split, (cores - 1) * split + last_split]
-
-    result_ids = []
-    for j in range(cores):  # Parallel running
-        result_ids.append(parallel.remote(
-            d, j, aa_indices, train_set, test_set, regressor, no_fft))
-
-    results = ray.get(result_ids)
-
-    performances = []
-    for core in range(cores):
-        for j, _ in enumerate(results[core]):
-            performances.append(results[core][j])
-
-    try:
-        sort = int(sort)
-        if sort == 2 or sort == 3:
-            performances.sort(key=lambda x: x[sort])
-        else:
-            performances.sort(key=lambda x: x[sort], reverse=True)
-
-    except ValueError:
-        raise ValueError(
-            "Choose between options 1 to 5 (R2, RMSE, NRMSE, "
-            "Pearson's r, Spearman's rho."
-        )
-
-    return performances
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+# Created on 05 October 2020
+# @authors: Niklas Siedhoff, Alexander-Maurice Illig
+# @contact: <n.siedhoff@biotec.rwth-aachen.de>
+# PyPEF - Pythonic Protein Engineering Framework
+# Released under Creative Commons Attribution-NonCommercial 4.0 International Public License (CC BY-NC 4.0)
+# For more information about the license see https://creativecommons.org/licenses/by-nc/4.0/legalcode
+
+# PyPEF – An Integrated Framework for Data-Driven Protein Engineering
+# Journal of Chemical Information and Modeling, 2021, 61, 3463-3476
+# https://doi.org/10.1021/acs.jcim.1c00099
+# Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
+# 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
+# 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
+# *Corresponding author
+# §Equal contribution
+
+"""
+Validation modules from regression.py for AAindex-based encoding
+modified for parallelization of the 566 AAindices used for encoding
+with Ray, see https://docs.ray.io/en/latest/index.html.
+"""
+
+import matplotlib
+matplotlib.use('Agg')
+import os
+import ray
+import warnings
+
+from pypef.utils.variant_data import get_sequences_from_file
+from pypef.ml.regression import (
+    full_aaidx_txt_path, path_aaindex_dir, AAIndexEncoding, get_regressor_performances
+)
+
+# to handle UserWarning for PLS n_components as error and general regression module warnings
+warnings.filterwarnings(action='ignore', category=RuntimeWarning, module='sklearn')
+warnings.filterwarnings(action='ignore', category=UserWarning, module='sklearn')
+
+
+@ray.remote
+def parallel(
+        d,
+        core,
+        aa_indices,
+        train_set,
+        test_set,
+        regressor='pls',
+        no_fft=False
+):
+    """
+    Parallelization of running using the user-defined number of cores.
+    Defining the task for each core.
+    """
+    warnings.filterwarnings("ignore", category=UserWarning)
+    warnings.filterwarnings("ignore", category=RuntimeWarning)
+
+    performances = []
+    for i in range(d[core][0], d[core][1]):
+        aaindex = aa_indices[i]  # Parallelization of AAindex iteration
+        sequences_train, _, y_train = get_sequences_from_file(train_set)
+        sequences_test, _, y_test = get_sequences_from_file(test_set)
+        x_aaidx_train = AAIndexEncoding(full_aaidx_txt_path(aaindex), sequences_train)
+        x_aaidx_test = AAIndexEncoding(full_aaidx_txt_path(aaindex), sequences_test)
+
+        if not no_fft:  # X is FFT-ed of encoded alphabetical sequence
+            x_train, _ = x_aaidx_train.collect_encoded_sequences()
+            x_test, _ = x_aaidx_test.collect_encoded_sequences()
+        else:  # X is raw encoded of alphabetical sequence
+            _, x_train = x_aaidx_train.collect_encoded_sequences()
+            _, x_test = x_aaidx_test.collect_encoded_sequences()
+
+        # If x_learn (or y_learn) is an empty array, the sequence could not be encoded,
+        # because of NoneType value. -> Skip
+        if x_train == 'skip' or x_test == 'skip':
+            continue  # skip the rest and do next iteration
+        r2, rmse, nrmse, pearson_r, spearman_rho, regressor, best_params = \
+            get_regressor_performances(x_train, x_test, y_train, y_test, regressor)
+        if r2 is not None:  # None for metrics if MSE can't be calculated
+            performances.append([
+                aaindex, r2, rmse, nrmse, pearson_r, spearman_rho, regressor, best_params
+            ])
+
+    return performances
+
+
+def aaindex_performance_parallel(
+        train_set,
+        test_set,
+        cores,
+        regressor='pls',
+        no_fft=False,
+        sort='1'
+):
+    """
+    Parallelization of running using the user-defined number of cores.
+    Calling function Parallel to execute the parallel running and
+    getting the results from each core each being defined by a result ID.
+    """
+    aa_indices = [file for file in os.listdir(path_aaindex_dir()) if file.endswith('.txt')]
+
+    split = int(len(aa_indices) / cores)
+    last_split = int(len(aa_indices) % cores) + split
+
+    d = {}
+    for i in range(cores - 1):
+        d[i] = [i * split, i * split + split]
+
+    d[cores - 1] = [(cores - 1) * split, (cores - 1) * split + last_split]
+
+    result_ids = []
+    for j in range(cores):  # Parallel running
+        result_ids.append(parallel.remote(
+            d, j, aa_indices, train_set, test_set, regressor, no_fft))
+
+    results = ray.get(result_ids)
+
+    performances = []
+    for core in range(cores):
+        for j, _ in enumerate(results[core]):
+            performances.append(results[core][j])
+
+    try:
+        sort = int(sort)
+        if sort == 2 or sort == 3:
+            performances.sort(key=lambda x: x[sort])
+        else:
+            performances.sort(key=lambda x: x[sort], reverse=True)
+
+    except ValueError:
+        raise ValueError(
+            "Choose between options 1 to 5 (R2, RMSE, NRMSE, "
+            "Pearson's r, Spearman's rho."
+        )
+
+    return performances
```

### Comparing `pypef-0.3/pypef/ml/regression.py` & `pypef-0.3.1/pypef/ml/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,18 +312,20 @@
     E.g. 'ACDY' --> [1,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,
                      0,1,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,
                      0,0,1,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,
                      0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,1]
     """
     def __init__(
             self,
-            sequences: list
+            sequences: list,
+            verbose=True
     ):
         self.sequences = sequences
         self.amino_acids = amino_acids  # imported, 20 standard AAs
+        self.verbose = verbose
 
     def encoding_dict(self) -> dict[str, np.ndarray]:
         encoding_dict = {}
         for idx, amino_acid in enumerate(self.amino_acids):
             encoding_vector = np.zeros(20, dtype=int)
             encoding_vector[idx] = 1
             encoding_dict.update({amino_acid: encoding_vector})
@@ -331,17 +333,23 @@
 
     def one_hot_encode_sequence(self, sequence: str) -> np.ndarray:
         encoded_sequence = []
         for aminoacid in sequence:
             encoded_sequence.append(self.encoding_dict()[aminoacid])
         return np.concatenate(encoded_sequence)
 
-    def collect_encoded_sequences(self, silence=False) -> list:
+    def collect_encoded_sequences(self, verbose: bool = None) -> np.ndarray:
+        if verbose is None:
+            disable = not self.verbose
+        else:
+            disable = not verbose
+        if len(np.atleast_1d(self.sequences)) == 1:  # always silence for single (wt) sequence
+            disable = True
         encoded_sequences = []
-        for sequence in tqdm(self.sequences, disable=silence):
+        for sequence in tqdm(self.sequences, disable=disable):
             encoded_sequences.append(self.one_hot_encode_sequence(sequence))
         return np.array(encoded_sequences)
 
 
 def pls_loocv(
         x_train: np.ndarray,
         y_train: np.ndarray
@@ -791,16 +799,20 @@
             x, _ = encoder.collect_encoded_sequences()
         else:  # use raw encoding (no FFT used on encoded sequences)
             _, x = encoder.collect_encoded_sequences()
     elif encoding == 'onehot':  # OneHot encoding technique
         encoder = OneHotEncoding(sequences)
         x = encoder.collect_encoded_sequences()
     elif encoding == 'dca':  # PLMC or GREMLIN-based encoding
+        if len(sequences) == 1:
+            use_global_model = True
+        else:
+            use_global_model = False
         x, variants, sequences, y_true, x_wt, model, model_type = plmc_or_gremlin_encoding(
-            variants, sequences, y_true, couplings_file, substitution_sep, threads, verbose
+            variants, sequences, y_true, couplings_file, substitution_sep, threads, verbose, use_global_model
         )
     else:
         raise SystemError("Unknown encoding option.")
 
     assert len(x) == len(variants) == len(sequences) == len(y_true)
     return x, variants, sequences, y_true
```

### Comparing `pypef-0.3/pypef/utils/directed_evolution.py` & `pypef-0.3.1/pypef/utils/directed_evolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         """
         Making sure that sequence mutations have been introduced correctly
         (for last sequence only).
         """
         for i, variant in enumerate(v_traj[1:]):  # [1:] as not checking for WT
             variant_position = int(re.findall(r"\d+", variant)[0]) - 1
             variant_amino_acid = str(variant[-1])
-            assert variant_amino_acid == s_traj[i+1][variant_position]  # checking AA of last trajactory sequence
+            assert variant_amino_acid == s_traj[i+1][variant_position]  # checking AA of last trajectory sequence
 
     def in_silico_de(self):
         """
         Perform directed evolution by randomly selecting a sequence
         position for substitution and randomly choose the amino acid
         to substitute to. New sequence gets accepted if meeting the
         Metropolis criterion and will be taken for new substitution
@@ -240,15 +240,15 @@
             new_full_variant = str(self.s_wt[int(new_variant[:-1])-1]) + new_variant  # full variant name, e.g. 'F17A'
             new_sequence = new_var_seq[0][1]
             # encode and predict new sequence fitness
             if self.ml_or_hybrid == 'ml':
                 predictions = predict(  # AAidx, OneHot, or DCA-based pure ML prediction
                     path=self.path,
                     model=self.model,
-                    encoding=self.encoding,  # TODO: check names/rename
+                    encoding=self.encoding,
                     variants=np.atleast_1d(new_full_variant),
                     sequences=np.atleast_1d(new_sequence),
                     no_fft=self.no_fft,
                     couplings_file=self.dca_encoder
                 )
 
             else:  # hybrid modeling and prediction
```

### Comparing `pypef-0.3/pypef/utils/learning_test_sets.py` & `pypef-0.3.1/pypef/utils/learning_test_sets.py`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/utils/low_n_mutation_extrapolation.py` & `pypef-0.3.1/pypef/utils/low_n_mutation_extrapolation.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,18 +63,19 @@
     plt.plot(train_sizes, avg_spearmanr, 'ko--', linewidth=1, markersize=1.5)
     plt.fill_between(
         np.array(train_sizes),
         np.array(avg_spearmanr) + np.array(stddev_spearmanr),
         np.array(avg_spearmanr) - np.array(stddev_spearmanr),
         alpha=0.5
     )
-    plt.ylim(0, max(np.array(avg_spearmanr) + np.array(stddev_spearmanr)))
+    plt.ylim(0, max(np.array(avg_spearmanr) * 1.1 + np.array(stddev_spearmanr)))
     plt.xlabel('Train sizes')
     plt.ylabel(r"Spearman's $\rho$")
-    plt.savefig(plt_name + '.png', dpi=500)
+
+    plt.savefig(plt_name.split(os.sep)[-1] + '.png', dpi=500)
     plt.clf()
 
 
 def low_n(
         encoded_csv: str,
         cv_regressor: str = None,
         n_runs: int = 10,
@@ -101,65 +102,70 @@
                 'Please choose another CV regression option.'
             )
         regressor = cv_regression_options(cv_regressor)
     elif hybrid_modeling:
         name = 'hybrid_ridge'
     n_variants = df.shape[0]
     train_sizes = get_train_sizes(n_variants).tolist()
-    variants, X, y = process_df_encoding(df)
+    variants, x, y = process_df_encoding(df)
+    if not x.any():
+        raise SystemError("Provided CSV file seems to have no encoding columns "
+                          "(required input CSV format: column 1: variant, column 2: "
+                          "variant fitness value, column 3 and ongoing columns: "
+                          "encoding feature values).")
 
     avg_spearmanr, stddev_spearmanr = [], []
     # test_sizes = [n_variants - size for size in train_sizes]
     if hybrid_modeling:
         logger.info('Using first CSV row/entry as wild type reference...')
     for size in tqdm(train_sizes):
         spearmanr_nruns = []
         for _ in range(n_runs):
             train_idxs = random.sample(range(n_variants - 1), int(size))
             test_idxs = []
             for n in range(n_variants - 1):
                 if n not in train_idxs:
                     test_idxs.append(n)
-            X_train, y_train = X[train_idxs], y[train_idxs]
-            X_test, y_test = X[test_idxs], y[test_idxs]
+            x_train, y_train = x[train_idxs], y[train_idxs]
+            x_test, y_test = x[test_idxs], y[test_idxs]
 
             if hybrid_modeling:
-                x_wt = X[0]  # WT should be first CSV variant entry
+                x_wt = x[0]  # WT should be first CSV variant entry
                 hybrid_model = DCAHybridModel(
-                    x_train=X_train,
+                    x_train=x_train,
                     y_train=y_train,
-                    x_test=X_test,  # only used for adjusting +/- sign of y_dca, can also be None
+                    x_test=x_test,  # only used for adjusting +/- sign of y_dca, can also be None
                     y_test=y_test,  # only used for adjusting +/- sign of y_dca, can also be None
                     x_wt=x_wt
                 )
                 beta_1, beta_2, reg = hybrid_model.settings(
-                    X_train, y_train, train_size_fit=train_size_train
+                    x_train, y_train, train_size_fit=train_size_train
                 )
                 spearmanr_nruns.append(
                     hybrid_model.spearmanr(
                         y_test,
                         hybrid_model.hybrid_prediction(
-                            X_test, reg, beta_1, beta_2
+                            x_test, reg, beta_1, beta_2
                         )
                     )
                 )
 
             else:  # ML
-                regressor.fit(X_train, y_train)
+                regressor.fit(x_train, y_train)
                 # Best CV params: best_params = regressor.best_params_
-                y_pred = regressor.predict(X_test)
+                y_pred = regressor.predict(x_test)
                 spearmanr_nruns.append(stats.spearmanr(y_test, y_pred)[0])
         avg_spearmanr.append(np.mean(spearmanr_nruns))
         stddev_spearmanr.append(np.std(spearmanr_nruns, ddof=1))
 
     plot_low_n(
         train_sizes,
         avg_spearmanr,
         stddev_spearmanr,
-        'low_N_' + str(encoded_csv[:-4] + '_' + name)
+        'low_N_' + str(encoded_csv).split('.')[0] + '_' + name
     )
 
     return train_sizes, avg_spearmanr, stddev_spearmanr
 
 
 def count_mutation_levels_and_get_dfs(df_encoding) -> tuple:
     """
@@ -260,62 +266,62 @@
     for i_m, mutation_level_df in enumerate(df_mut_lvl):
         if mutation_level_df.shape[0] != 0:
             collected_levels.append(i_m)
     train_idx_appended = []
     if len(collected_levels) > 1:
         train_idx = collected_levels[0]
         train_df = df_mut_lvl[train_idx]
-        train_variants, X_train, y_train = process_df_encoding(train_df)
+        train_variants, x_train, y_train = process_df_encoding(train_df)
         all_higher_df = df_mut_lvl[-1]  # only used for adjusting +/- of y_dca
-        all_higher_variants, X_all_higher, y_all_higher = process_df_encoding(all_higher_df)
+        all_higher_variants, x_all_higher, y_all_higher = process_df_encoding(all_higher_df)
         if hybrid_modeling:
-            x_wt = X_train[0]
+            x_wt = x_train[0]
             hybrid_model = DCAHybridModel(
-                x_train=X_train,
+                x_train=x_train,
                 y_train=y_train,
-                x_test=X_all_higher,  # only used for adjusting +/- of y_dca, can also be None but
+                x_test=x_all_higher,  # only used for adjusting +/- of y_dca, can also be None but
                 y_test=y_all_higher,  # higher risk of wrong sign assignment of beta_1 (y_dca)
                 x_wt=x_wt
             )
             beta_1, beta_2, reg = hybrid_model.settings(
-                X_train, y_train, train_size_fit=train_size)
+                x_train, y_train, train_size_fit=train_size)
             pickle.dump(
                 {'hybrid_model': hybrid_model, 'beta_1': beta_1, 'beta_2': beta_2,
                  'spearman_rho': float('nan'), 'regressor': reg},
                 open(os.path.join('Pickles', 'HYBRID_LVL_1'), 'wb')
             )
         elif cv_regressor:
             logger.info('Fitting regressor on lvl 1 substitution data...')
-            regressor.fit(X_train, y_train)
+            regressor.fit(x_train, y_train)
             if save_model:
                 logger.info(f'Saving model as Pickle file: ML_LVL_1')
                 pickle.dump(regressor, open(os.path.join('Pickles', 'ML_LVL_1'), 'wb'))
         for i, _ in enumerate(tqdm(collected_levels)):
             if i < len(collected_levels) - 1:  # not last i else error, last entry is: lvl 1 --> all higher variants
                 test_idx = collected_levels[i + 1]
                 test_df = df_mut_lvl[test_idx]
-                test_variants, X_test, y_test = process_df_encoding(test_df)
+                test_variants, x_test, y_test = process_df_encoding(test_df)
                 if not conc:
                     # For training on distinct iterated level i, uncomment lines below:
                     # train_idx = collected_levels[i]
                     # train_df = self.mutation_level_dfs[train_idx]
-                    # train_variants, X_train, y_train = self._process_df_encoding(train_df)
+                    # train_variants, x_train, y_train = self._process_df_encoding(train_df)
                     if hybrid_modeling:
                         data.update({
                             test_idx + 1:
                                 {
                                     'hybrid_model': hybrid_model,
                                     'max_train_lvl': train_idx + 1,
                                     'n_y_train': len(y_train),
                                     'test_lvl': test_idx + 1,
                                     'n_y_test': len(y_test),
                                     'spearman_rho': hybrid_model.spearmanr(
                                         y_test,
                                         hybrid_model.hybrid_prediction(
-                                            X_test, reg, beta_1, beta_2
+                                            x_test, reg, beta_1, beta_2
                                         )
                                     ),
                                     'beta_1': beta_1,
                                     'beta_2': beta_2,
                                     'regressor': reg
                                 }
                         })
@@ -326,66 +332,66 @@
                                     'regressor': regressor,
                                     'max_train_lvl': train_idx + 1,
                                     'n_y_train': len(y_train),
                                     'test_lvl': test_idx + 1,
                                     'n_y_test': len(y_test),
                                     'spearman_rho': stats.spearmanr(
                                         y_test,                    # Call predict on the BaseSearchCV estimator
-                                        regressor.predict(X_test)  # with the best found parameters
+                                        regressor.predict(x_test)  # with the best found parameters
                                     )[0]
                                 }
                         })
 
                 else:  # conc mode, training on mutational levels i: 1, ..., max(i)-1
                     train_idx_appended.append(collected_levels[i])
                     if i < len(collected_levels) - 2:  # -2 as not the last (all_higher)  ## i != 0 and
                         train_df_appended_conc = pd.DataFrame()
                         for idx in train_idx_appended:
                             train_df_appended_conc = pd.concat(
                                 [train_df_appended_conc, df_mut_lvl[idx]])
-                        train_variants_conc, X_train_conc, y_train_conc = \
+                        train_variants_conc, x_train_conc, y_train_conc = \
                             process_df_encoding(train_df_appended_conc)
                         if hybrid_modeling:  # updating hybrid model params with newly inputted concatenated train data
                             beta_1_conc, beta_2_conc, reg_conc = hybrid_model.settings(
-                                X_train_conc,
+                                x_train_conc,
                                 y_train_conc,
                                 train_size_fit=train_size
                             )
                             data.update({
                                 test_idx + 1:
                                     {
                                         'hybrid_model': hybrid_model,
                                         'max_train_lvl': train_idx_appended[-1] + 1,
                                         'n_y_train': len(y_train_conc),
                                         'test_lvl': test_idx + 1,
                                         'n_y_test': len(y_test),
                                         'spearman_rho': hybrid_model.spearmanr(
                                             y_test,
                                             hybrid_model.hybrid_prediction(
-                                                X_test, reg_conc, beta_1_conc, beta_2_conc
+                                                x_test, reg_conc, beta_1_conc, beta_2_conc
                                             )
                                         ),
                                         'beta_1': beta_1_conc,
                                         'beta_2': beta_2_conc,
                                         'regressor': reg_conc
                                     }
                             })
                         else:  # ML updating pureML regression model params with newly inputted concatenated train data
                             # Fitting regressor on concatenated substitution data
-                            regressor.fit(X_train_conc, y_train_conc)
+                            regressor.fit(x_train_conc, y_train_conc)
                             data.update({
                                 test_idx + 1:
                                 {
                                     'max_train_lvl': train_idx_appended[-1] + 1,
                                     'n_y_train': len(y_train_conc),
                                     'test_lvl': test_idx + 1,
                                     'n_y_test': len(y_test),
                                     'spearman_rho': stats.spearmanr(
                                         y_test,  # Call predict on the BaseSearchCV estimator
-                                        regressor.predict(X_test)  # with the best found parameters
+                                        regressor.predict(x_test)  # with the best found parameters
                                         )[0],
                                     'regressor': regressor
                                 }
                             })
     plot_extrapolation(data, name, conc)
 
     return data
@@ -423,10 +429,10 @@
     )
     if conc:
         name += '_train_concat_lvls'
     else:
         name += '_train_lvl_1'
     plt.xticks(test_lvls, label_infos, fontsize=5)
     plt.ylabel(r"Spearman's $\rho$")
-    name = name.replace("\\", "").replace(".", "") + '_extrapolation.png'
+    name = name.split(os.sep)[-1] + '_extrapolation.png'
     plt.savefig(name, dpi=500)
     plt.clf()
```

### Comparing `pypef-0.3/pypef/utils/performance.py` & `pypef-0.3.1/pypef/utils/performance.py`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/utils/plot.py` & `pypef-0.3.1/pypef/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/utils/prediction_sets.py` & `pypef-0.3.1/pypef/utils/prediction_sets.py`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/utils/sto2a2m.py` & `pypef-0.3.1/pypef/utils/sto2a2m.py`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/utils/to_file.py` & `pypef-0.3.1/pypef/utils/to_file.py`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/utils/utils_run.py` & `pypef-0.3.1/pypef/utils/utils_run.py`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef/utils/variant_data.py` & `pypef-0.3.1/pypef/utils/variant_data.py`

 * *Files identical despite different names*

### Comparing `pypef-0.3/pypef.egg-info/PKG-INFO` & `pypef-0.3.1/pypef.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pypef
-Version: 0.3
+Version: 0.3.1
 Summary: A command-line interface (CLI) tool for performing data-driven protein engineering by building machine learning (ML)-trained regression models from sequence variant fitness data (in CSV format) based on different techniques for protein sequence encoding. Next to building pure ML models, 'hybrid modeling' is also possible using a blended model optimized for predictive contributions of a statistical and an ML-based prediction.
-Home-page: https://github.com/niklases/PyPEF
+Home-page: https://github.com/Protein-Engineering-Framework/PyPEF
 Author: Niklas Siedhoff & Alexander-Maurice Illig
 Author-email: n.siedhoff@biotec.rwth-aachen.de
 License: CC BY-NC-SA 4.0
 Keywords: Pythonic Protein Engineering Framework
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypef-0.3/pypef.egg-info/SOURCES.txt` & `pypef-0.3.1/pypef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.3/setup.py` & `pypef-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #!/usr/bin/env python3
 # for installation run me with: pip install .
 #                      or with: pip install -e .
 
 
 from setuptools import setup, find_packages
+from pypef import __version__
 
 
 with open("requirements.txt", "r", encoding="utf-8") as install_requirements:
     requirements = install_requirements.read()
 
 setup(
     name='pypef',
-    version='0.3',
+    version=__version__.split('-')[0],
     author='Niklas Siedhoff & Alexander-Maurice Illig',
     author_email='n.siedhoff@biotec.rwth-aachen.de',
     license='CC BY-NC-SA 4.0',
     description='A command-line interface (CLI) tool for performing data-driven protein engineering '
                 'by building machine learning (ML)-trained regression models from sequence variant '
                 'fitness data (in CSV format) based on different techniques for protein sequence encoding. '
                 'Next to building pure ML models, \'hybrid modeling\' is also possible using a blended '
                 'model optimized for predictive contributions of a statistical and an ML-based prediction.',
     long_description='For detailed description including a short Jupyter Notebook-based '
                      'tutorial please refer to the GitHub page.',
     long_description_content_type='text/markdown',
-    url='https://github.com/niklases/PyPEF',
+    url='https://github.com/Protein-Engineering-Framework/PyPEF',
     py_modules=['pypef'],
     packages=find_packages(include=['pypef', 'pypef.*']),
     package_data={'pypef': ['ml/AAindex/*', 'ml/AAindex/Refined_cluster_indices_r0.93_r0.97/*']},
     include_package_data=True,
     install_requires=[requirements],
     python_requires='>= 3.9, < 3.12',
     keywords='Pythonic Protein Engineering Framework',
```

