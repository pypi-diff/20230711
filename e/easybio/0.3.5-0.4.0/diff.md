# Comparing `tmp/easybio-0.3.5.tar.gz` & `tmp/easybio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybio-0.3.5.tar", last modified: Sun Jun 25 12:03:23 2023, max compression
+gzip compressed data, was "easybio-0.4.0.tar", last modified: Tue Jul 11 04:08:09 2023, max compression
```

## Comparing `easybio-0.3.5.tar` & `easybio-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 12:03:23.525140 easybio-0.3.5/
--rw-r--r--   0 root         (0) root         (0)      538 2023-06-25 12:03:23.521140 easybio-0.3.5/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)       30 2023-04-21 05:50:43.000000 easybio-0.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 12:03:23.521140 easybio-0.3.5/easyBio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 12:03:23.521140 easybio-0.3.5/easyBio/Utils/
--rw-rw-r--   0 root         (0) root         (0)      496 2023-06-09 04:11:15.000000 easybio-0.3.5/easyBio/Utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8161 2023-06-08 06:24:54.000000 easybio-0.3.5/easyBio/Utils/download.py
--rw-rw-r--   0 root         (0) root         (0)     3047 2023-06-08 08:28:47.000000 easybio-0.3.5/easyBio/Utils/downloadUtils.py
--rw-rw-r--   0 root         (0) root         (0)     9038 2023-06-12 01:27:11.000000 easybio-0.3.5/easyBio/Utils/easyBioUtils.py
--rw-rw-r--   0 root         (0) root         (0)    12656 2023-06-25 07:14:34.000000 easybio-0.3.5/easyBio/Utils/gsaDownLoadUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2117 2023-04-26 10:50:17.000000 easybio-0.3.5/easyBio/Utils/netUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2594 2023-06-16 14:11:54.000000 easybio-0.3.5/easyBio/Utils/runvelocityc.py
--rw-rw-r--   0 root         (0) root         (0)     2840 2023-06-20 03:42:16.000000 easybio-0.3.5/easyBio/Utils/toolsUtils.py
--rw-rw-r--   0 root         (0) root         (0)      329 2023-06-09 04:13:06.000000 easybio-0.3.5/easyBio/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1122 2023-06-08 07:20:20.000000 easybio-0.3.5/easyBio/beifen.py
--rw-rw-r--   0 root         (0) root         (0)     5246 2023-06-09 03:40:58.000000 easybio-0.3.5/easyBio/changeSRAName.py
--rw-rw-r--   0 root         (0) root         (0)     2141 2023-05-26 06:34:13.000000 easybio-0.3.5/easyBio/downloadSRA.py
--rw-rw-r--   0 root         (0) root         (0)      200 2023-04-26 10:50:00.000000 easybio-0.3.5/easyBio/easyBio.py
--rw-rw-r--   0 root         (0) root         (0)     3311 2023-06-09 01:56:23.000000 easybio-0.3.5/easyBio/gsaPipline copy.py
--rw-rw-r--   0 root         (0) root         (0)     2692 2023-06-25 08:30:14.000000 easybio-0.3.5/easyBio/gsaPipline.py
--rw-rw-r--   0 root         (0) root         (0)     4599 2023-06-25 06:55:12.000000 easybio-0.3.5/easyBio/pipline.py
--rw-rw-r--   0 root         (0) root         (0)     1069 2023-06-06 02:41:20.000000 easybio-0.3.5/easyBio/run_cellranger.py
--rw-rw-r--   0 root         (0) root         (0)      110 2023-04-26 10:48:58.000000 easybio-0.3.5/easyBio/run_test.py
--rw-rw-r--   0 root         (0) root         (0)     4236 2023-06-09 04:10:54.000000 easybio-0.3.5/easyBio/runvelocyto.py
--rw-rw-r--   0 root         (0) root         (0)     1479 2023-04-29 17:22:45.000000 easybio-0.3.5/easyBio/splitSRA.py
--rw-rw-r--   0 root         (0) root         (0)     1006 2023-04-29 17:25:20.000000 easybio-0.3.5/easyBio/test.py
--rw-rw-r--   0 root         (0) root         (0)     2301 2023-05-29 01:59:25.000000 easybio-0.3.5/easyBio/tidy.py
--rw-rw-r--   0 root         (0) root         (0)     2841 2023-04-30 05:59:02.000000 easybio-0.3.5/easyBio/velocyto2.py
--rw-rw-r--   0 root         (0) root         (0)     2954 2023-04-26 10:42:04.000000 easybio-0.3.5/easyBio/velocyto3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 12:03:23.521140 easybio-0.3.5/easybio.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      538 2023-06-25 12:03:23.000000 easybio-0.3.5/easybio.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      803 2023-06-25 12:03:23.000000 easybio-0.3.5/easybio.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-06-25 12:03:23.000000 easybio-0.3.5/easybio.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      345 2023-06-25 12:03:23.000000 easybio-0.3.5/easybio.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-22 17:45:52.000000 easybio-0.3.5/easybio.egg-info/not-zip-safe
--rw-rw-r--   0 root         (0) root         (0)       20 2023-06-25 12:03:23.000000 easybio-0.3.5/easybio.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        8 2023-06-25 12:03:23.000000 easybio-0.3.5/easybio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 12:03:23.525140 easybio-0.3.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1483 2023-06-25 07:20:18.000000 easybio-0.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:08:09.217344 easybio-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-11 04:08:09.217344 easybio-0.4.0/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)       30 2023-04-21 05:50:43.000000 easybio-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:08:09.209345 easybio-0.4.0/easyBio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:08:09.217344 easybio-0.4.0/easyBio/Utils/
+-rw-rw-r--   0 root         (0) root         (0)      661 2023-07-07 11:47:13.000000 easybio-0.4.0/easyBio/Utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2854 2023-07-07 09:45:10.000000 easybio-0.4.0/easyBio/Utils/downLoadBAM.py
+-rw-rw-r--   0 root         (0) root         (0)     2901 2023-07-07 02:09:13.000000 easybio-0.4.0/easyBio/Utils/downLoadSRA.py
+-rw-rw-r--   0 root         (0) root         (0)     8221 2023-07-07 02:07:55.000000 easybio-0.4.0/easyBio/Utils/download.py
+-rw-rw-r--   0 root         (0) root         (0)     4193 2023-07-07 11:51:19.000000 easybio-0.4.0/easyBio/Utils/downloadUtils.py
+-rw-rw-r--   0 root         (0) root         (0)     9077 2023-07-06 12:33:28.000000 easybio-0.4.0/easyBio/Utils/easyBioUtils.py
+-rw-rw-r--   0 root         (0) root         (0)     2216 2023-07-06 13:07:59.000000 easybio-0.4.0/easyBio/Utils/easyCellranger.py
+-rw-rw-r--   0 root         (0) root         (0)    12122 2023-07-06 13:13:28.000000 easybio-0.4.0/easyBio/Utils/gsaDownLoadUtils.py
+-rw-rw-r--   0 root         (0) root         (0)     2117 2023-04-26 10:50:17.000000 easybio-0.4.0/easyBio/Utils/netUtils.py
+-rw-rw-r--   0 root         (0) root         (0)     2594 2023-07-07 11:45:29.000000 easybio-0.4.0/easyBio/Utils/runvelocityc.py
+-rw-rw-r--   0 root         (0) root         (0)     7817 2023-07-11 04:04:53.000000 easybio-0.4.0/easyBio/Utils/toFastq.py
+-rw-rw-r--   0 root         (0) root         (0)     3735 2023-07-07 09:45:19.000000 easybio-0.4.0/easyBio/Utils/toolsUtils.py
+-rw-rw-r--   0 root         (0) root         (0)      426 2023-07-06 12:55:32.000000 easybio-0.4.0/easyBio/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6283 2023-07-06 12:31:50.000000 easybio-0.4.0/easyBio/changeSRAName.py
+-rw-rw-r--   0 root         (0) root         (0)     2142 2023-07-07 01:45:29.000000 easybio-0.4.0/easyBio/downloadSRA.py
+-rw-rw-r--   0 root         (0) root         (0)      200 2023-04-26 10:50:00.000000 easybio-0.4.0/easyBio/easyBio.py
+-rw-rw-r--   0 root         (0) root         (0)     2692 2023-07-06 13:12:50.000000 easybio-0.4.0/easyBio/gsaPipline.py
+-rw-rw-r--   0 root         (0) root         (0)     5024 2023-07-10 12:28:56.000000 easybio-0.4.0/easyBio/pipline.py
+-rw-rw-r--   0 root         (0) root         (0)     1324 2023-07-06 13:03:21.000000 easybio-0.4.0/easyBio/run_cellranger.py
+-rw-rw-r--   0 root         (0) root         (0)      110 2023-04-26 10:48:58.000000 easybio-0.4.0/easyBio/run_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1247 2023-07-07 02:24:02.000000 easybio-0.4.0/easyBio/runvelocyto.py
+-rw-rw-r--   0 root         (0) root         (0)     1479 2023-04-29 17:22:45.000000 easybio-0.4.0/easyBio/splitSRA.py
+-rw-rw-r--   0 root         (0) root         (0)     1006 2023-04-29 17:25:20.000000 easybio-0.4.0/easyBio/test.py
+-rw-rw-r--   0 root         (0) root         (0)     2301 2023-05-29 01:59:25.000000 easybio-0.4.0/easyBio/tidy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:08:09.217344 easybio-0.4.0/easybio.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      538 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      831 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      345 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-04-22 17:45:52.000000 easybio-0.4.0/easybio.egg-info/not-zip-safe
+-rw-rw-r--   0 root         (0) root         (0)       43 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        8 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 04:08:09.217344 easybio-0.4.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1539 2023-07-07 02:28:58.000000 easybio-0.4.0/setup.py
```

### Comparing `easybio-0.3.5/PKG-INFO` & `easybio-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.3.5
+Version: 0.4.0
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
```

### Comparing `easybio-0.3.5/easyBio/Utils/download.py` & `easybio-0.4.0/easyBio/Utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,21 +179,21 @@
                 print(f"删除[{partName}]成功---{getNowTime()}")
 
     def start(self):
         totalSize = self.getTotalSize()  # 文件总大小
         if (not totalSize):
             print(
                 "\033[1;31mFile does not support streaming download, program exited---{}\033[0m".format(getNowTime()))
-            return
+            return False
         self.partNum = math.ceil((totalSize/self.perPartSize))  # 计算分块数量
         if (self.checkTask()):
             self.deleteParts()
             print(
                 "\033[1;32m{} file downloaded, task exited---{}\033[0m".format(self.fileName, getNowTime()))
-            return
+            return True
         pool = threadpool.ThreadPool(self.threadNum)  # 创建线程池
         partList = []  # 分块列表(包含序号和大小)
         argsList = []  # 任务参数列表
 
         for i in range(self.partNum):  # 构建参数
             if (i+1 == self.partNum):
                 args = ([i, i*self.perPartSize, totalSize-1], None)
@@ -206,10 +206,12 @@
         for req in reqs:  # 提交任务
             pool.putRequest(req)
         pool.wait()  # 等待线程结束
 
         if (self.checkParts(partList)):  # 检查分块状态
             self.mergeParts()
             self.deleteParts()
+            return True
         else:
             print(
                 "\033[1;31mChunk download incomplete, please rerun the program---{}\033[0m".format(getNowTime()))
+            return False
```

### Comparing `easybio-0.3.5/easyBio/Utils/easyBioUtils.py` & `easybio-0.4.0/easyBio/Utils/easyBioUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import os
 import shutil
 import subprocess
 import concurrent
 
 from .toolsUtils import get_num_threads
 
+
+
 def splitSRAfun(folder, outdir, threads, kind):
     # Get a list of .sra files in the folder
     sra_files = [f for f in os.listdir(folder) if f.endswith('.sra')]
 
     # Iterate over .sra files in the folder and run the provided command
     for sra_file in sra_files:
         sra_base, _ = os.path.splitext(sra_file)
@@ -65,15 +67,17 @@
         if filename.startswith("SRR"):
             sample_id = filename.split("_")[0]
             ## 剔除掉已存在的处理好的文件夹
             if matricespath != "":
                 sample_dir = os.path.join(matricespath, sample_id)
                 if not os.path.isdir(sample_dir):
                     samples.add(sample_id)
-                    
+            else:
+                samples.add(sample_id)
+
     if samples == set():
         print("\033[1;32m All samples have been processed with Cell Ranger\033[0m")
     else:
         print(samples)
          
     
     for sample in samples:
```

### Comparing `easybio-0.3.5/easyBio/Utils/gsaDownLoadUtils.py` & `easybio-0.4.0/easyBio/Utils/gsaDownLoadUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import threading
 
 import pandas as pd
 
 from .toolsUtils import sraMd5Cal
 from .download import Download
 from .netUtils import requestGet
+from .easyCellranger import easyCellranger
 
 class gsaProject:
     def __init__(self, inputName: str, dirs_path="./") -> None:
         if inputName.startswith("PRJCA"):
             pjurl = f"https://ngdc.cncb.ac.cn/gsa-human/hra/getAjax/searchByPrjAccession?prjAccession={inputName}"
             hra = requestGet(pjurl).json()["listHras"][0]["accession"]
         elif inputName.startswith("HRA"):
@@ -156,35 +157,14 @@
         df = self.exceldf
         FileMapping = {}
         for i in range(len(df)):
             FileMapping[df.iloc[i, 0]] = df.iloc[i, 2]
         self.FileMapping = FileMapping
         return self.FileMapping
     
-    # def cpfqFiles(self, threadsNum=16):
-    #     fq_path2 = f"{self.raw_path}/fq2"
-    #     os.makedirs(fq_path2, exist_ok=True)
-    #     files = os.listdir(self.fq_path)
-    #     def copy_file(fq_file, fq_file2):
-    #         if not os.path.exists(fq_file2):
-    #             shutil.copy2(fq_file, fq_file2)
-    #         else:
-    #             print(f"{fq_file} 已复制")
-    #     threads = []
-    #     for file in files:
-    #         fq_file = os.path.join(self.fq_path, file)
-    #         fq_file2 = os.path.join(fq_path2, file)
-    #         thread = threading.Thread(
-    #             target=copy_file, args=(fq_file, fq_file2))
-    #         thread.start()
-    #         threads.append(thread)
-    #     # 等待所有线程完成
-    #     for thread in threads:
-    #         thread.join()
-        
     def cpfqFiles(self, threadsNum=16) -> None:
         print(f"threadsNum: {threadsNum}")
         files = os.listdir(self.fq_path)
         
         semaphore = threading.Semaphore(threadsNum)
 
         def copy_file(fq_file, fq_file2):
@@ -252,15 +232,15 @@
                 if lane_number < 10:
                     lane_number_str = f"00{lane_number}"
                 elif lane_number < 100:
                     lane_number_str = f"0{lane_number}"
                 else:
                     lane_number_str = f"{lane_number}"
 
-                new_name = f"HRX{name}_S1_L{lane_number_str}_{read_type}_001.fastq.gz"
+                new_name = f"{name}_S1_L{lane_number_str}_{read_type}_001.fastq.gz"
                 os.rename(os.path.join(folder_path, file),os.path.join(folder_path, new_name))
                 print(f'Renamed {file} to {new_name}')
 
     def check_fqfile_exists(self, target_suffix='S1_L001_R1_001.fastq.gz') -> bool:
         for file_name in os.listdir(self.fq_path):
             if file_name.endswith(target_suffix):
                 return True
@@ -275,66 +255,74 @@
         else:
             files, srr_counts = self.count_hrr_occurrences_fq(folder_path)
             self.rename_files(self.getFileMapping(), files,
                               srr_counts, folder_path)
             print("\033[1;32m Rename completed\033[0m")
     
     def cellrangerRun(self, db, expectcellnum = 3000, fq_dir = "", otherItem="", matricespath=""):
+
         if matricespath == "":
-            self.matrices_path = f"{self.raw_path}/matrices"
-            os.makedirs(self.matrices_path, exist_ok=True)
-            matricespath = self.matrices_path
+            matricespath = f"{self.raw_path}/matrices"
             
         if fq_dir == "":
             # 获取文件夹中的所有文件名
             fq_dir = self.fq_path
-            filenames = os.listdir(self.fq_path)
-
-        current_dir = os.getcwd()
-        # 获取目录中所有的子目录
-        subdirectories = [d for d in os.listdir(
-            current_dir) if os.path.isdir(os.path.join(current_dir, d))]
-
-        # 遍历子目录，检查是否以“SRR”开头
-        for subdirectory in subdirectories:
-            if subdirectory.startswith("HRX"):
-                print("\033[1;31m Found residual folder, removing it...\033[0m")
-                # 如果以“HRX”开头，则删除这个子目录及其内容
-                subdirectory_path = os.path.join(current_dir, subdirectory)
-                if subdirectory_path != "":
-                    # rm -rf删的更快(*^▽^*)
-                    os.system(f"rm -rf {subdirectory_path}")
-
-        # time.sleep(10000)
-        samples = set()
-        for filename in filenames:
-            if filename.startswith("HRX"):
-                sample_id = filename.split("_")[0]
-                # 剔除掉已存在的处理好的文件夹
-                if matricespath != "":
-                    sample_dir = os.path.join(matricespath, sample_id)
-                    if not os.path.isdir(sample_dir):
-                        samples.add(sample_id)
-
-        if samples == set():
-            print("\033[1;32m All samples have been processed with Cell Ranger\033[0m")
-        else:
-            print(samples)
 
-        for sample in samples:
-            cmd = f"""cellranger count --id={sample} \
-    --transcriptome={db} \
-    --fastqs={fq_dir} \
-    --sample={sample} \
-    --expect-cells={expectcellnum} \
-    --nosecondary {otherItem}"""
-
-            print("\033[1;33m Running command for sample {}:\033[0m".format(sample))
-            print("\033[1;31m{}\033[0m".format(cmd))
-            subprocess.run(cmd, shell=True)
-
-            if matricespath != "":
-                mv_cmd = ["mv", f"{sample}", f"{matricespath}"]
-                subprocess.run(mv_cmd, check=True)
+        ec = easyCellranger(fq_dir, expectcellnum,
+                            db, otherItem, matricespath)
+        ec.cellrangerRun()
+        
+        
+        # if fq_dir == "":
+        #     # 获取文件夹中的所有文件名
+        #     fq_dir = self.fq_path
+        #     filenames = os.listdir(self.fq_path)
+        
+    #     current_dir = os.getcwd()
+    #     # 获取目录中所有的子目录
+    #     subdirectories = [d for d in os.listdir(
+    #         current_dir) if os.path.isdir(os.path.join(current_dir, d))]
+
+    #     # 遍历子目录，检查是否以“SRR”开头
+    #     for subdirectory in subdirectories:
+    #         if subdirectory.startswith("HRX"):
+    #             print("\033[1;31m Found residual folder, removing it...\033[0m")
+    #             # 如果以“HRX”开头，则删除这个子目录及其内容
+    #             subdirectory_path = os.path.join(current_dir, subdirectory)
+    #             if subdirectory_path != "":
+    #                 # rm -rf删的更快(*^▽^*)
+    #                 os.system(f"rm -rf {subdirectory_path}")
+
+    #     # time.sleep(10000)
+    #     samples = set()
+    #     for filename in filenames:
+    #         if filename.startswith("HRX"):
+    #             sample_id = filename.split("_")[0]
+    #             # 剔除掉已存在的处理好的文件夹
+    #             if matricespath != "":
+    #                 sample_dir = os.path.join(matricespath, sample_id)
+    #                 if not os.path.isdir(sample_dir):
+    #                     samples.add(sample_id)
+
+    #     if samples == set():
+    #         print("\033[1;32m All samples have been processed with Cell Ranger\033[0m")
+    #     else:
+    #         print(samples)
+
+    #     for sample in samples:
+    #         cmd = f"""cellranger count --id={sample} \
+    # --transcriptome={db} \
+    # --fastqs={fq_dir} \
+    # --sample={sample} \
+    # --expect-cells={expectcellnum} \
+    # --nosecondary {otherItem}"""
+
+    #         print("\033[1;33m Running command for sample {}:\033[0m".format(sample))
+    #         print("\033[1;31m{}\033[0m".format(cmd))
+    #         subprocess.run(cmd, shell=True)
+
+    #         if matricespath != "":
+    #             mv_cmd = ["mv", f"{sample}", f"{matricespath}"]
+    #             subprocess.run(mv_cmd, check=True)
```

### Comparing `easybio-0.3.5/easyBio/Utils/netUtils.py` & `easybio-0.4.0/easyBio/Utils/netUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.3.5/easyBio/Utils/runvelocityc.py` & `easybio-0.4.0/easyBio/Utils/runvelocityc.py`

 * *Files identical despite different names*

### Comparing `easybio-0.3.5/easyBio/Utils/toolsUtils.py` & `easybio-0.4.0/easyBio/Utils/toolsUtils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # -*- coding: utf-8 -*-
 # Author: Lei
 # Date: 2023-04-20
 # Description:
+import shutil
 import datetime
 import multiprocessing
 import os
 import hashlib
 
+import psutil
+
 def calMd5(filename):
     with open(filename,"rb") as f:
         bytes = f.read() # read file as bytes
         readable_hash = hashlib.md5(bytes).hexdigest();
         return readable_hash
 
-# 我需要读取md5check文件，文件里面每行是一个文件名，判断md5Item是否在md5check文件里，如果是运行下面的操作，然后将结果保存追加在md5check文件里
 
 def sraMd5Cal(folder, md5List, rawdirs):
     sraFiles = os.listdir(folder)
     reDownloadSra = []
     # file= open(f"{rawdirs}/md5check","r")
     # scItems = file.readlines()
     # print(scItems)
@@ -37,17 +39,18 @@
             if md5Item in sraFiles:
                 if not md5Item in scItems:
                     print(f"计算{md5Item}文件的md5值")
                     calMd5filName = f"{folder}/{md5Item}"
                     cd5 = calMd5(calMd5filName)
                     # print(cd5)
                     # print(md5List[md5Item])
-                    print(cd5==md5List[md5Item])
-                    if cd5!=md5List[md5Item]:
+                    print(cd5 == md5List[md5Item])
+                    if cd5 != md5List[md5Item]:
                         os.remove(calMd5filName)
+                        reDownloadSra.append(md5Item)
                     else:
                         # f.write(md5Item)
                         file.writelines(md5Item)
                         file.writelines("\n")
             else:
                 reDownloadSra.append(md5Item)
     print(reDownloadSra)
@@ -78,17 +81,44 @@
     try:
         os.makedirs(str)
     except:
         pass
 
 
 def get_num_threads():
-    num_threads = multiprocessing.cpu_count()
+    # num_threads = multiprocessing.cpu_count()
+    num_threads = os.cpu_count()
     if num_threads <= 16:
         num_threads -= 2
     elif num_threads < 64:
         num_threads -= 4
     elif num_threads < 128:
         num_threads -= 8
     else:
         num_threads -= 10
     return num_threads
+
+
+def get_available_memory(unit="GB"):
+    # num_threads = multiprocessing.cpu_count()
+    memory_info = psutil.virtual_memory()
+    memory_available = memory_info.available
+    total_memory_gb = int(memory_available / (1024 ** 3))
+    total_memory_mb = int(memory_available / (1024 ** 2))
+    total_memory_kb = int(memory_available / (1024 ** 1))
+    total_memory = total_memory_gb if unit == "GB" else (
+        total_memory_mb if unit == "MB" else total_memory_kb)
+    print("总可用内存：", total_memory, unit)
+    return total_memory
+
+
+def copyDirs(source_dir, target_dir):
+    if not os.path.exists(target_dir):
+        os.makedirs(target_dir)
+
+    for file_name in os.listdir(source_dir):
+        source_file = os.path.join(source_dir, file_name)
+        target_file = os.path.join(target_dir, file_name)
+
+        if os.path.isfile(source_file):
+            shutil.copy2(source_file, target_file)
+            print(f"Copied {source_file} to {target_file}")
```

### Comparing `easybio-0.3.5/easyBio/changeSRAName.py` & `easybio-0.4.0/easyBio/changeSRAName.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,21 +20,29 @@
             srr_counts[srr_id] = max(srr_counts.get(srr_id, 0), int(num))
 
     # 根据文件数重命名文件
     for file in os.listdir(folder_path):
         match = re.match(r'(SRR\d+)_(\d)', file)
         if match:
             srr_id, num = match.groups()
-            if srr_counts[srr_id] == 2:
+            if srr_counts[srr_id] == 1 or 2:
                 new_name = f'{srr_id}_S1_L001_R{num}_001.fastq.gz'
             elif srr_counts[srr_id] == 3:
                 if num == "1":
                     new_name = f'{srr_id}_S1_L001_I1_001.fastq.gz'
                 else:
                     new_name = f'{srr_id}_S1_L001_R{int(num)-1}_001.fastq.gz'
+            elif srr_counts[srr_id] == 3:
+                if num == "1":
+                    new_name = f'{srr_id}_S1_L001_I1_001.fastq.gz'
+                if num == "2":
+                    new_name = f'{srr_id}_S1_L001_I2_001.fastq.gz'
+                else:
+                    new_name = f'{srr_id}_S1_L001_R{int(num)-2}_001.fastq.gz'
+            
             os.rename(os.path.join(folder_path, file),
                       os.path.join(folder_path, new_name))
             print(f'Renamed {file} to {new_name}')
 
 def read_mapping_file(list_file):
     with open(list_file, 'r') as f:
         lines = f.readlines()
@@ -83,51 +91,69 @@
     name_add_srr_mapping = {}
     for file in files:
         srr_match = re.match(r'(SRR\d+)_(\d)', file)
         if srr_match:
             srr, number = srr_match.groups()
             name = mapping[srr]
             read_type = ''
-            if srr_counts[srr] == 2:
+            if srr_counts[srr] == 1 or 2:
                 read_type = 'R1' if number == '1' else 'R2'
             elif srr_counts[srr] == 3:
                 read_type = 'I1' if number == '1' else (
                     'R1' if number == '2' else 'R2')
+            elif srr_counts[srr] == 4:
+                read_type = 'I1' if number == '1' else (
+                    'I2' if number == '2' else ('R1' if number == '3' else 'R2'))
+                # match number:
+                #     case '1':
+                #         read_type = "I1"
+                #     case '2':
+                #         read_type = "I2"
+                #     case '3':
+                #         read_type = "R1"
+                #     case '4':
+                #         read_type = "R2"
 
             if srr in name_add_srr_mapping:
                 lane_number = name_add_srr_mapping[srr]
             else:
                 name_add_mapping[name] = name_add_mapping.get(name, 0) + 1
                 name_add_srr_mapping[srr] = name_add_mapping[name]
                 lane_number = name_add_srr_mapping[srr]
 
             new_name = f"SRR{name}_S{lane_number}_L001_{read_type}_001.fastq.gz"
             os.rename(os.path.join(folder_path, file),
-                      os.path.join(folder_path, new_name))
+                     os.path.join(folder_path, new_name))
             print(f'Renamed {file} to {new_name}')
 
 def renames2(list_file, folder_path):
     mapping = read_mapping_file(list_file)
     files, srr_counts = count_srr_occurrences(folder_path)
     rename_files(files, folder_path, mapping, srr_counts)
 
+
 def renames3(list_file, folder_path):
     mapping = read_mapping_file(list_file)
     files, srr_counts = count_srr_occurrences(folder_path)
     rename_files2(files, folder_path, mapping, srr_counts)
 
+def renames4(mapping, folder_path):
+    files, srr_counts = count_srr_occurrences(folder_path)
+    print(mapping)
+    rename_files2(files, folder_path, mapping, srr_counts)
+
 def main():
     parser = argparse.ArgumentParser(
         description="Process list_file and folder_path")
     parser.add_argument("-l", "--list_file", help="matching list")
     parser.add_argument("-f", "--folder_path", default=os.getcwd(),
                         help="Directory (default: current directory)")
 
     args = parser.parse_args()
-        
+
     list_file = args.list_file
     folder_path = args.folder_path
     
     print("\033[1;32m list_file:\033[0m \033[32m{}\033[0m".format(list_file))
     print("\033[1;32m folder_path:\033[0m \033[32m{}\033[0m".format(folder_path))
     
     if list_file:
```

### Comparing `easybio-0.3.5/easyBio/downloadSRA.py` & `easybio-0.4.0/easyBio/downloadSRA.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     md5List = {}
     for result in results:
         run_accession = f'${result["run_accession"]}.sra'
         sra_md5 = result["sra_md5"]
         md5List[run_accession] = sra_md5
     print(md5List)
         
-    check=False
+    check = False
     while not check:
         # print(results)
         check = downLoadSRA(gsenumber, results, dirs, threads)
         
     # 下载 SRA 数据
     results = getProResults(gsenumber)
     
@@ -63,10 +63,9 @@
         check=False
         while not check:
             # print(results)
             check = downLoadSRA(gsenumber, results, dirs, threads)
         reDownloadSra = sraMd5Cal(filedirs, md5List, rawdirs)
     
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `easybio-0.3.5/easyBio/gsaPipline copy.py` & `easybio-0.4.0/easyBio/gsaPipline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,70 @@
-from collections import defaultdict
 import os
 import pandas as pd
 
-from easybio_conda.easyBio.Utils.gsaDownLoadUtils import gsaProject
-
 from .runvelocyto import buildLoomFile
 
+from .Utils import runvelocityc
 from .Utils import tidySummary, getProResults, sraMd5Cal
-from .Utils import get_num_threads, calMd5
+from .Utils import get_num_threads, calMd5, gsaProject
 
 from .changeSRAName import renames1, renames2, renames3
 from .Utils import check_file_exists, cellrangerRun, splitSRAfun, downLoadSRA, cellrangerRun2
 import argparse
-import re
 
-inputName = "PRJCA014236"
+# inputName = "PRJCA014236"
 # inputName = "HRA003747"
 
-dirs = "/home/data/user/lei/SRAData/GSE"
-fq_path = "/home/data/user/lei/SRAData/GSE/PRJCA014236/raw/fq"
-
-gsap = gsaProject(inputName=inputName, dirs_path=dirs)
-mapping = gsap.getFileMapping()
-dirs_path = f"{dirs}/{inputName}"
-raw_path = f"{dirs_path}/raw"
-fq_path = f"{raw_path}/fq"
-
-def rename_files(files, folder_path, mapping, srr_counts):
-    name_add_mapping = {}
-    name_add_srr_mapping = {}
-    for file in files:
-        srr_match = re.match(r'(HRR\d+)_[fr](\d)', file)
-        if srr_match:
-            srr, number = srr_match.groups()
-            name = mapping[srr]
-            read_type = ''
-            if srr_counts[srr] == 2:
-                read_type = 'R1' if number == '1' else 'R2'
-            elif srr_counts[srr] == 3:
-                read_type = 'I1' if number == '1' else (
-                    'R1' if number == '2' else 'R2')
-
-            if srr in name_add_srr_mapping:
-                lane_number = name_add_srr_mapping[srr]
-            else:
-                name_add_mapping[name] = name_add_mapping.get(name, 0) + 1
-                name_add_srr_mapping[srr] = name_add_mapping[name]
-                lane_number = name_add_srr_mapping[srr]
-            
-            lane_number_str = ""
-            if lane_number < 10:
-                lane_number_str = f"00{lane_number}"
-            elif lane_number < 100:
-                lane_number_str = f"0{lane_number}"
-            else:
-                lane_number_str = f"{lane_number}"
-
-            new_name = f"HRR{name}_S1_L{lane_number_str}_{read_type}_001.fastq.gz"
-            # os.rename(os.path.join(folder_path, file),os.path.join(folder_path, new_name))
-            print(f'Renamed {file} to {new_name}')
-
-            
-
-
-
-def renamegsa(gsap, folder_path):
-    mapping = gsap.getFileMapping()
-    files, srr_counts = count_hrr_occurrences(folder_path)
-    rename_files(files, folder_path, mapping, srr_counts)
-
-
-renamegsa(gsap, fq_path)
-
-
 
 def main():
     num_threads = get_num_threads()
     # Set up argument parser
     parser = argparse.ArgumentParser(
-        description="Process GSE number, directory and threads")
+        description="Process GSA number, directory and threads")
     parser.add_argument("-i", "--inputName", help="Project Number")
     parser.add_argument("-d", "--dirs", default=os.getcwd(),
                         help="Directory (default: current directory)")
     parser.add_argument("-t", "--threads", type=int, default=num_threads,
                         help="Number of threads (default: your cpucounts)")
+    
+    parser.add_argument("-db", "--db_path", required=True,
+                        help="Path to the gene reference file (required)")
+    parser.add_argument("-ec", "--expectcellnum", type=int, default=3000,
+                        help="Expected cell number for running cellranger (default: 3000)")
+    parser.add_argument("-oi", "--other_Item", type=str,
+                        default="", help="otherItem for cellranger")
+    parser.add_argument("-rmf", "--rmsk_file", type=str,
+                        help="Path to the hg38_rmsk.gtf file")
+    parser.add_argument("-gtf", "--gtf_file", type=str,
+                        help="Path to the Homo_sapiens.GRCh38.109.gtf file")
+    parser.add_argument("-vm", "--max_memory", type=int,
+                        default=200, help="Maximum memory in GB (default: 200)")
+
 
     args = parser.parse_args()
     inputName = args.inputName
     dirs = args.dirs
     threads = args.threads
+    db_path = args.db_path
+    expectcellnum = args.expectcellnum
+    rmsk_file = args.rmsk_file
+    gtf_file = args.gtf_file
+    max_memory = args.max_memory
+    otherItem = args.other_Item
 
     gsap = gsaProject(inputName=inputName, dirs_path=dirs)
-    gsap.downloadFiles(threads=threads)
+    gsap.downloadFiles(threads=threads, copy=True)
+    gsap.renamegsa()
     
-    dirs_path = f"{dirs}/{inputName}"
-    raw_path = f"{dirs_path}/raw"
-    fq_path = f"{raw_path}/fq"
-    renamegsa(gsap, fq_path)
+    print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
+    gsap.cellrangerRun(db_path, expectcellnum, otherItem)
+    print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
+
+    if rmsk_file and gtf_file:
+        rv = runvelocityc(gsap.matrices_path, rmsk_file, gtf_file, max_memory)
+        rv.buildLoomFile()
     
+    outputpath = f"{gsap.raw_path}/output"
+    os.makedirs(outputpath, exist_ok=True)
+    tidySummary(gsap.matrices_path, outputpath)
 
-
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `easybio-0.3.5/easyBio/pipline.py` & `easybio-0.4.0/easyBio/pipline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,132 +1,134 @@
 # -*- coding: utf-8 -*-
 # Author: Lei
 # Date: 2023-04-20
 # Description:
+import math
 import os
 
-from .runvelocyto import buildLoomFile
-from .Utils import runvelocityc
+from .Utils import runvelocityc, toFastq, easyCellranger
 
 from .Utils import tidySummary, getProResults, sraMd5Cal
-from .Utils import get_num_threads, calMd5
+from .Utils import get_num_threads, Download, downLoadBAM
 
-from .changeSRAName import renames1, renames2, renames3
+from .changeSRAName import renames1, renames2, renames3, renames4, read_mapping_file
 from .Utils import check_file_exists, cellrangerRun, splitSRAfun, downLoadSRA, cellrangerRun2
 import argparse
 
 
-# def writeLog(logname, logcontent):
-#     with open(f"{logFiles}/{logname}", 'w') as file:
-#         file.write(logcontent)
 
 def main():
     num_threads = get_num_threads()
 
     # Set up argument parser
     parser = argparse.ArgumentParser(
         description="Process GSE number, directory and threads")
     parser.add_argument("-g", "--gsenumber", help="GSE number")
     parser.add_argument("-d", "--dirs", default=os.getcwd(),
                         help="Directory (default: current directory)")
     parser.add_argument("-t", "--threads", type=int, default=num_threads,
                         help="Number of threads (default: your cpucounts)")
+    parser.add_argument("-df", "--DownloadFirst", type=bool, default=False,
+                        help="Download sra data first")
     parser.add_argument("-k", "--kind", default="--split-files",
                         help="Zhe kind of split")
     parser.add_argument("-l", "--list_file", help="matching list")
     parser.add_argument("-db", "--db_path", required=True,
                         help="Path to the gene reference file (required)")
     parser.add_argument("-ec", "--expectcellnum", type=int, default=3000,
                         help="Expected cell number for running cellranger (default: 3000)")
-
     parser.add_argument("-rmf", "--rmsk_file", type=str, help="Path to the hg38_rmsk.gtf file")
     parser.add_argument("-gtf", "--gtf_file", type=str, help="Path to the Homo_sapiens.GRCh38.109.gtf file")
     parser.add_argument("-vm", "--max_memory", type=int,
                         default=200, help="Maximum memory in GB (default: 200)")
     parser.add_argument("-oi", "--other_Item", type=str,
                         default="", help="otherItem for cellranger")
     
     args = parser.parse_args()
-
+    
     # Extract values from parsed arguments
-    gsenumber = args.gsenumber
+    gsenumberList = args.gsenumber
     dirs = args.dirs
     threads = args.threads
     kind = args.kind
     db_path = args.db_path
     expectcellnum = args.expectcellnum
     list_file = args.list_file
     rmsk_file = args.rmsk_file
     gtf_file = args.gtf_file
     max_memory = args.max_memory
     otherItem = args.other_Item
-
-    rawdirs = f"{dirs}/{gsenumber}/raw"
-    # logdirs = f"{rawdirs}/log"
-
-    # splitSRA(rawdirs, kind, threads)
-    folder = f"{rawdirs}/sra"
-    os.makedirs(folder, exist_ok=True)
-
-    print("\033[1;33m{}\033[0m".format(folder))   # 黄
+    downloadFist = args.DownloadFirst
     
-    # os.makedirs(logdirs, exist_ok=True)
-
-    # 下载 SRA 数据
-    results = getProResults(gsenumber)
-    
-    md5List = {}
-    for result in results:
-        run_accession = f'{result["run_accession"]}.sra'
-        sra_md5 = result["sra_md5"]
-        md5List[run_accession] = sra_md5
-    # print(md5List)
-    
-    # reDownloadSra = sraMd5Cal(folder, md5List)
+    gList = gsenumberList.split(",")
+    print(gList)
     
-    reDownloadSra = [1, 2, 3]
-    while len(reDownloadSra) > 1:
-        check=False
-        while not check:
-            # print(results)
-            check = downLoadSRA(gsenumber, results, dirs, threads)
-        reDownloadSra = sraMd5Cal(folder, md5List, rawdirs)
-    
-    print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
-
-    fqfiles = f"{rawdirs}/fq"
-    os.makedirs(fqfiles, exist_ok=True)
-    print("\033[1;33m{}\033[0m".format(fqfiles))   # 黄
-    
-    target_suffix = 'S1_L001_R1_001.fastq.gz'
-    file_exists = check_file_exists(fqfiles, target_suffix)
-
-    if file_exists:
-        print(f"fastq文件已进行改名")
-    else:
-        splitSRAfun(folder, fqfiles, threads, kind)
+    if downloadFist:
+        for gsenumber in gList:
+            rawdirs = f"{dirs}/{gsenumber}/raw"
+            # folder = f"{rawdirs}/sra"
+            # os.makedirs(folder, exist_ok=True)
+
+            # print("\033[1;33m{}\033[0m".format(folder))   # 黄
+
+            # 下载 SRA 数据
+            results = getProResults(gsenumber)
+
+            ds = downLoadSRA(results, rawdirs, threads)
+            print(ds.md5List)
+            print(ds.sampleMap)
+            
+            if ds.md5List == {}:
+                db = downLoadBAM(results, rawdirs, threads)
+                db.Download()
+            else:
+               ds.Download()
+            print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
+
+    for gsenumber in gList:
+        rawdirs = f"{dirs}/{gsenumber}/raw"
+        # folder = f"{rawdirs}/sra"
+        # os.makedirs(folder, exist_ok=True)
+
+        # print("\033[1;33m{}\033[0m".format(folder))   # 黄
+
+        # 下载 SRA 数据
+        results = getProResults(gsenumber)
+
+        ds = downLoadSRA(results, rawdirs, threads)
+        print(ds.md5List)
+
+        if ds.md5List == {}:
+            db = downLoadBAM(results, rawdirs, threads)
+            db.Download()
+            tofq = toFastq(db.bamfolder, type="bam", FastqDir=f"{rawdirs}/fq", threads=threads)
+            tofq.BAMtoFastq(f"{rawdirs}/tofq")
+            # exit()
+        else:
+            ds.Download()
+            tofq = toFastq(ds.srafolder, FastqDir=f"{rawdirs}/fq", threads=threads)
+            tofq.SRAtoFastq(kind)
+            if list_file:
+                sampleMap = read_mapping_file(list_file)
+            else:
+                sampleMap = ds.sampleMap
+            tofq.renameFQfiles(sampleMap, folder_path=tofq.FastqDir)
         
         print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
-        if list_file:
-            renames3(list_file, fqfiles)
-        else:
-            renames1(fqfiles)
-        print("\033[1;32m Rename completed\033[0m")
-
-    print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
-    matricespath = f"{rawdirs}/matrices"
-    os.makedirs(matricespath, exist_ok=True)
-    cellrangerRun(db_path, fqfiles, expectcellnum, otherItem, matricespath)
-
-    print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
-    
-    if rmsk_file and gtf_file:
-        rv = runvelocityc(matricespath, rmsk_file, gtf_file, max_memory)
-        rv.buildLoomFile()
-
-    outputpath = f"{rawdirs}/output"
-    os.makedirs(outputpath, exist_ok=True)
-    # 设置源文件夹和目标文件夹的路径
-    tidySummary(matricespath, outputpath)
+        ec = easyCellranger(f"{rawdirs}/fq", expectcellnum,
+                            db_path, otherItem, f"{rawdirs}/matrices")
+        ec.cellrangerRun()
+        
+        print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
+        
+        if rmsk_file and gtf_file:
+            rv = runvelocityc(ec.matricespath,
+                              rmsk_file, gtf_file, max_memory)
+            rv.buildLoomFile()
+
+        outputpath = f"{rawdirs}/output"
+        os.makedirs(outputpath, exist_ok=True)
+        # 设置源文件夹和目标文件夹的路径
+        tidySummary(ec.matricespath, outputpath)
 
 if __name__ == "__main__":
     main()
```

### Comparing `easybio-0.3.5/easyBio/splitSRA.py` & `easybio-0.4.0/easyBio/splitSRA.py`

 * *Files identical despite different names*

### Comparing `easybio-0.3.5/easyBio/test.py` & `easybio-0.4.0/easyBio/test.py`

 * *Files identical despite different names*

### Comparing `easybio-0.3.5/easyBio/tidy.py` & `easybio-0.4.0/easyBio/tidy.py`

 * *Files identical despite different names*

### Comparing `easybio-0.3.5/easybio.egg-info/PKG-INFO` & `easybio-0.4.0/easybio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.3.5
+Version: 0.4.0
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
```

### Comparing `easybio-0.3.5/easybio.egg-info/SOURCES.txt` & `easybio-0.4.0/easybio.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 README.md
 setup.py
 easyBio/__init__.py
-easyBio/beifen.py
 easyBio/changeSRAName.py
 easyBio/downloadSRA.py
 easyBio/easyBio.py
-easyBio/gsaPipline copy.py
 easyBio/gsaPipline.py
 easyBio/pipline.py
 easyBio/run_cellranger.py
 easyBio/run_test.py
 easyBio/runvelocyto.py
 easyBio/splitSRA.py
 easyBio/test.py
 easyBio/tidy.py
-easyBio/velocyto2.py
-easyBio/velocyto3.py
 easyBio/Utils/__init__.py
+easyBio/Utils/downLoadBAM.py
+easyBio/Utils/downLoadSRA.py
 easyBio/Utils/download.py
 easyBio/Utils/downloadUtils.py
 easyBio/Utils/easyBioUtils.py
+easyBio/Utils/easyCellranger.py
 easyBio/Utils/gsaDownLoadUtils.py
 easyBio/Utils/netUtils.py
 easyBio/Utils/runvelocityc.py
+easyBio/Utils/toFastq.py
 easyBio/Utils/toolsUtils.py
 easybio.egg-info/PKG-INFO
 easybio.egg-info/SOURCES.txt
 easybio.egg-info/dependency_links.txt
 easybio.egg-info/entry_points.txt
 easybio.egg-info/not-zip-safe
 easybio.egg-info/requires.txt
```

### Comparing `easybio-0.3.5/setup.py` & `easybio-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-VERSION = '0.3.5'
+VERSION = '0.4.0'
 
 setup(
     name='easybio',  # package name
     version=VERSION,  # package version
     author='Lei Cui',
     author_email='cuilei798@qq.com',
     maintainer='Lei Cui',
@@ -29,15 +29,18 @@
             'easyVelocyto=easyBio.runvelocyto:main',
             'easyscGSEpipline=easyBio.gsaPipline:main',
         ]
     },
     install_requires=[
         # 'biopython',
         'threadpool',
-        'requests'
+        'requests',
+        'pandas',
+        'velocyto',
+        'psutil'
         # Add more dependencies here
     ],
     package_data={
         'Utils': ['Utils/*']
     },
     classifiers=[
         'Operating System :: OS Independent',
```

