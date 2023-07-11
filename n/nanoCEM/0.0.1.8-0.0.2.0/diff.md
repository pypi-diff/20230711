# Comparing `tmp/nanoCEM-0.0.1.8.tar.gz` & `tmp/nanoCEM-0.0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.1.8.tar", last modified: Tue Jul 11 09:52:25 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.2.0.tar", last modified: Tue Jul 11 11:03:33 2023, max compression
```

## Comparing `nanoCEM-0.0.1.8.tar` & `nanoCEM-0.0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.8/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9065 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8482 2023-07-11 09:51:03.000000 nanoCEM-0.0.1.8/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9565 2023-07-11 06:38:51.000000 nanoCEM-0.0.1.8/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.8/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.8/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7840 2023-07-10 08:21:18.000000 nanoCEM-0.0.1.8/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.8/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.8/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7872 2023-07-11 09:39:14.000000 nanoCEM-0.0.1.8/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11478 2023-07-10 08:05:02.000000 nanoCEM-0.0.1.8/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-06 04:15:59.000000 nanoCEM-0.0.1.8/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9065 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1134 2023-07-11 09:51:55.000000 nanoCEM-0.0.1.8/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 11:03:33.677532 nanoCEM-0.0.2.0/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.0/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9737 2023-07-11 11:03:33.677532 nanoCEM-0.0.2.0/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9154 2023-07-11 11:01:35.000000 nanoCEM-0.0.2.0/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 11:03:33.673532 nanoCEM-0.0.2.0/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9703 2023-07-11 10:29:09.000000 nanoCEM-0.0.2.0/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.0/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.2.0/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8020 2023-07-11 10:29:09.000000 nanoCEM-0.0.2.0/nanoCEM/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.0/nanoCEM/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.0/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.0/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11478 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.0/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.0/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 11:03:33.677532 nanoCEM-0.0.2.0/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9737 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-11 11:03:33.677532 nanoCEM-0.0.2.0/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1134 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.0/setup.py
```

### Comparing `nanoCEM-0.0.1.8/LICENSE` & `nanoCEM-0.0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.8/PKG-INFO` & `nanoCEM-0.0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.8
+Version: 0.0.2.0
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,33 @@
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
-Here is a quick example help the user confirm the installation that show the difference of A2030 on 23S rRNA.
+Here is an example to help the user confirm the installation of A2030 on 23S rRNA:
+```sh
+pip install nanoCEM
+git clone https://github.com/lrslab/nanoCEM
+cd nanoCEM/example
+# tackle f5c result
+current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
+--chrom NR_103073.1 --strand + \
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--base_shift 2 --rna --norm
+# tackle tombo result
+current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+--chrom NR_103073.1 --strand + \
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--rna --cpu 4 --norm
+```
+Then you can generate the following pdf files.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
 ## Before start, you should know
 ### Re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
@@ -74,14 +92,15 @@
   --len LEN             region around the position (default:10)
   --strand STRAND       Strand of your interest (default:+)
   -t CPU, --cpu CPU     num of process (default:8)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 Turn on the RNA mode 
+  --norm                Turn on the normalization
 ```
 ### read_f5c_resquiggle
 ```sh
 current_events_magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
@@ -97,15 +116,15 @@
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 
                         Turn on the RNA mode
   --base_shift BASE_SHIFT
                         base shift if required (default:0)
-
+  --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
@@ -144,17 +163,20 @@
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
 3. Run current_events_magnifier to plot
 ```sh
-nanoCEM.py tombo -i sample1/single -c sample2/single -o tombo_result\
- --chrom NR_103073.1 --strand + --pos 2030 \
- --len 5 --cpu 4 --ref reference.fasta --rna
+# tackle tombo result
+current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+--chrom NR_103073.1 --strand + \
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--rna --cpu 4 --norm
 ```
 #### 4.2 F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion.
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```fast5/```
 ```sh
 slow5tools f2s fast5/ -d blow5_dir
@@ -166,18 +188,19 @@
 Use ```--rna``` to turn to the rna mode and ```--pore r10``` to re-squiggle reads from R10
 ```sh
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-current_events_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
+current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
---pos 3929 --len 10 \
---ref reference.fasta --base_shift 2 --rna
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--base_shift 2 --rna --norm
 ```
```

### Comparing `nanoCEM-0.0.1.8/README.md` & `nanoCEM-0.0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,33 @@
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
-Here is a quick example help the user confirm the installation that show the difference of A2030 on 23S rRNA.
+Here is an example to help the user confirm the installation of A2030 on 23S rRNA:
+```sh
+pip install nanoCEM
+git clone https://github.com/lrslab/nanoCEM
+cd nanoCEM/example
+# tackle f5c result
+current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
+--chrom NR_103073.1 --strand + \
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--base_shift 2 --rna --norm
+# tackle tombo result
+current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+--chrom NR_103073.1 --strand + \
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--rna --cpu 4 --norm
+```
+Then you can generate the following pdf files.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
 ## Before start, you should know
 ### Re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
@@ -60,14 +78,15 @@
   --len LEN             region around the position (default:10)
   --strand STRAND       Strand of your interest (default:+)
   -t CPU, --cpu CPU     num of process (default:8)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 Turn on the RNA mode 
+  --norm                Turn on the normalization
 ```
 ### read_f5c_resquiggle
 ```sh
 current_events_magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
@@ -83,15 +102,15 @@
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 
                         Turn on the RNA mode
   --base_shift BASE_SHIFT
                         base shift if required (default:0)
-
+  --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
@@ -130,17 +149,20 @@
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
 3. Run current_events_magnifier to plot
 ```sh
-nanoCEM.py tombo -i sample1/single -c sample2/single -o tombo_result\
- --chrom NR_103073.1 --strand + --pos 2030 \
- --len 5 --cpu 4 --ref reference.fasta --rna
+# tackle tombo result
+current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+--chrom NR_103073.1 --strand + \
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--rna --cpu 4 --norm
 ```
 #### 4.2 F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion.
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```fast5/```
 ```sh
 slow5tools f2s fast5/ -d blow5_dir
@@ -152,18 +174,19 @@
 Use ```--rna``` to turn to the rna mode and ```--pore r10``` to re-squiggle reads from R10
 ```sh
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-current_events_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
+current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
---pos 3929 --len 10 \
---ref reference.fasta --base_shift 2 --rna
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--base_shift 2 --rna --norm
 ```
```

### Comparing `nanoCEM-0.0.1.8/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.2.0/nanoCEM/CE_magnifier_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,16 @@
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
     aligned_num_wt = 0
     aligned_num_ivt = 0
     # read reference
+    if args.function is None:
+        raise RuntimeError("Please choose function from f5c or tombo, or use -h to view the help document")
     subsample_num = args.overplot_number
     fasta = read_fasta_to_dic(args.ref)
     # length filter
     args.pos = args.pos - 1
     length_gene = len(fasta[args.chrom])
     if args.pos + args.len + 1 >= length_gene or args.pos - args.len <= 0:
         raise RuntimeError("The position requested is too close to the border (pos-len>0 and pos+len<length of fasta)")
```

### Comparing `nanoCEM-0.0.1.8/nanoCEM/cem_utils.py` & `nanoCEM-0.0.2.0/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.8/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.2.0/nanoCEM/current_events_magnifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument("--ref", required=True, help="fasta file")
-        parser_input.add_argument('--norm', action='store_true', help='normalization mode')
+        parser_input.add_argument('--norm', action='store_true', help='Turn on the normalization mode')
         parser_input.add_argument("--overplot-number", default=500, type=int,
                                   help="Number of read will be used to plot")
-        parser_input.add_argument('--rna', action='store_true', help='RNA mode')
+        parser_input.add_argument('--rna', action='store_true', help='Turn on the RNA mode')
     # Define the argument parser
     parser = argparse.ArgumentParser(description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
     subparsers = parser.add_subparsers(dest='function')
 
     # tombo subparser
     parser_tombo = subparsers.add_parser('tombo', help='tackle tombo re-squiggle')
     parser_tombo.add_argument('--basecall_group', default="RawGenomeCorrected_000",
@@ -53,14 +53,17 @@
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
     aligned_num_wt = 0
     aligned_num_ivt = 0
     # read reference
+    # print(args)
+    if args.function is None:
+        raise RuntimeError("Please choose function from f5c or tombo, or use -h to view the help document")
     subsample_num = args.overplot_number
     fasta = read_fasta_to_dic(args.ref)
     # length filter
     args.pos = args.pos - 1
     length_gene = len(fasta[args.chrom])
     if args.pos + args.len + 1 >= length_gene or args.pos - args.len <= 0:
         raise RuntimeError("The position requested is too close to the border (pos-len>0 and pos+len<length of fasta)")
```

### Comparing `nanoCEM-0.0.1.8/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.2.0/nanoCEM/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.8/nanoCEM/normalization.py` & `nanoCEM-0.0.2.0/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.8/nanoCEM/plot.py` & `nanoCEM-0.0.2.0/nanoCEM/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,22 +96,20 @@
                 raise Exception("Unsupported figure type!")
             # plot.render_matplotlib()
             if item == 'Dwell time':
                 item = 'Dwell_time'
             plot.save(filename=results_path + "/" + item + "_" + plot_type + ".pdf", dpi=300)
     else:
         new_df = None
-
-
         for item in item_list:
             # collect data
             temp = df[[item, 'position', 'type']].copy()
             temp.columns = ['value', 'position', 'Group']
             temp.loc[:, 'stats'] = item
-            if filter and item!='Dwell time':
+            if filter:
                 sig_min, sig_max = np.percentile(temp['value'], SIG_PCTL_RANGE)
                 sig_diff = sig_max - sig_min
                 ylim_tuple = [sig_min - sig_diff * 0.1, sig_max + sig_diff * 0.1]
                 temp = temp[(temp['value'] >= ylim_tuple[0]) & (temp['value'] <= ylim_tuple[1])]
             if new_df is None:
                 new_df = temp
             else:
```

### Comparing `nanoCEM-0.0.1.8/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.2.0/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.8/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.2.0/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.8/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.2.0/nanoCEM.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.8
+Version: 0.0.2.0
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,33 @@
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
-Here is a quick example help the user confirm the installation that show the difference of A2030 on 23S rRNA.
+Here is an example to help the user confirm the installation of A2030 on 23S rRNA:
+```sh
+pip install nanoCEM
+git clone https://github.com/lrslab/nanoCEM
+cd nanoCEM/example
+# tackle f5c result
+current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
+--chrom NR_103073.1 --strand + \
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--base_shift 2 --rna --norm
+# tackle tombo result
+current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+--chrom NR_103073.1 --strand + \
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--rna --cpu 4 --norm
+```
+Then you can generate the following pdf files.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
 ## Before start, you should know
 ### Re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
@@ -74,14 +92,15 @@
   --len LEN             region around the position (default:10)
   --strand STRAND       Strand of your interest (default:+)
   -t CPU, --cpu CPU     num of process (default:8)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 Turn on the RNA mode 
+  --norm                Turn on the normalization
 ```
 ### read_f5c_resquiggle
 ```sh
 current_events_magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
@@ -97,15 +116,15 @@
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 
                         Turn on the RNA mode
   --base_shift BASE_SHIFT
                         base shift if required (default:0)
-
+  --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
@@ -144,17 +163,20 @@
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
 3. Run current_events_magnifier to plot
 ```sh
-nanoCEM.py tombo -i sample1/single -c sample2/single -o tombo_result\
- --chrom NR_103073.1 --strand + --pos 2030 \
- --len 5 --cpu 4 --ref reference.fasta --rna
+# tackle tombo result
+current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+--chrom NR_103073.1 --strand + \
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--rna --cpu 4 --norm
 ```
 #### 4.2 F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion.
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```fast5/```
 ```sh
 slow5tools f2s fast5/ -d blow5_dir
@@ -166,18 +188,19 @@
 Use ```--rna``` to turn to the rna mode and ```--pore r10``` to re-squiggle reads from R10
 ```sh
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-current_events_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
+current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
---pos 3929 --len 10 \
---ref reference.fasta --base_shift 2 --rna
+--pos 2030 \
+--ref data/23S_rRNA.fasta \
+--base_shift 2 --rna --norm
 ```
```

### Comparing `nanoCEM-0.0.1.8/setup.py` & `nanoCEM-0.0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.1.8",
+    version="0.0.2.0",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle program(tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
```

