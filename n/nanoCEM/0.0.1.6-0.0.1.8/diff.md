# Comparing `tmp/nanoCEM-0.0.1.6.tar.gz` & `tmp/nanoCEM-0.0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.1.6.tar", last modified: Mon Jul 10 08:05:28 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.1.8.tar", last modified: Tue Jul 11 09:52:25 2023, max compression
```

## Comparing `nanoCEM-0.0.1.6.tar` & `nanoCEM-0.0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.6/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8388 2023-07-03 09:59:45.000000 nanoCEM-0.0.1.6/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9561 2023-07-10 08:02:19.000000 nanoCEM-0.0.1.6/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.6/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.6/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7836 2023-07-10 08:03:26.000000 nanoCEM-0.0.1.6/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.6/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.6/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7818 2023-07-05 10:48:45.000000 nanoCEM-0.0.1.6/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11478 2023-07-10 08:05:02.000000 nanoCEM-0.0.1.6/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-06 04:15:59.000000 nanoCEM-0.0.1.6/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-10 08:05:20.000000 nanoCEM-0.0.1.6/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.8/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9065 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8482 2023-07-11 09:51:03.000000 nanoCEM-0.0.1.8/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9565 2023-07-11 06:38:51.000000 nanoCEM-0.0.1.8/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.8/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.8/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7840 2023-07-10 08:21:18.000000 nanoCEM-0.0.1.8/nanoCEM/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.8/nanoCEM/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.8/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7872 2023-07-11 09:39:14.000000 nanoCEM-0.0.1.8/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11478 2023-07-10 08:05:02.000000 nanoCEM-0.0.1.8/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-06 04:15:59.000000 nanoCEM-0.0.1.8/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9065 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-11 09:52:25.000000 nanoCEM-0.0.1.8/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-11 09:52:25.578189 nanoCEM-0.0.1.8/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1134 2023-07-11 09:51:55.000000 nanoCEM-0.0.1.8/setup.py
```

### Comparing `nanoCEM-0.0.1.6/LICENSE` & `nanoCEM-0.0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.6/PKG-INFO` & `nanoCEM-0.0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.6
-Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
-Home-page: https://github.com/lrslab/current_events_magnifier
+Version: 0.0.1.8
+Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
+Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
-Here is an example that show the difference of A2030 on 23S rRNA.
+Here is a quick example help the user confirm the installation that show the difference of A2030 on 23S rRNA.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
 ## Before start, you should know
 ### Re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
@@ -40,19 +40,22 @@
 This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
 In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo. However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
+```sh
+pip install nanoCEM==0.0.1.8
+```
 
+Other tools if you needed
 ```sh
-pip install nanoCEM==0.0.4.4
-pip install ont-fast5-api
-conda install -c bioconda f5c slow5tools
+pip install ont-fast5-api pod
+conda install -c bioconda f5c slow5tools minimap2 
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 current_events_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
```

### Comparing `nanoCEM-0.0.1.6/README.md` & `nanoCEM-0.0.1.8/nanoCEM.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,30 @@
+Metadata-Version: 2.1
+Name: nanoCEM
+Version: 0.0.1.8
+Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
+Home-page: https://github.com/lrslab/nanoCEM
+Author: GUO Zhihao
+Author-email: qhuozhihao@icloud.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7,<3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nanoCEM
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
-Here is an example that show the difference of A2030 on 23S rRNA.
+Here is a quick example help the user confirm the installation that show the difference of A2030 on 23S rRNA.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
 ## Before start, you should know
 ### Re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
@@ -26,19 +40,22 @@
 This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
 In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo. However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
+```sh
+pip install nanoCEM==0.0.1.8
+```
 
+Other tools if you needed
 ```sh
-pip install nanoCEM==0.0.4.4
-pip install ont-fast5-api
-conda install -c bioconda f5c slow5tools
+pip install ont-fast5-api pod
+conda install -c bioconda f5c slow5tools minimap2 
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 current_events_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
```

### Comparing `nanoCEM-0.0.1.6/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.1.8/nanoCEM/CE_magnifier_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,10 +167,10 @@
     #     else:
     #         args.pos = args.pos + args.base_shift
     percentile_filter=False
     if aligned_num_wt > 50 and aligned_num_ivt > 50:
         percentile_filter=True
 
     signal_plot(df, results_path, args.pos, base_list, title, 'merged',percentile_filter)
-    signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
-    signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
+    # signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
+    # signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `nanoCEM-0.0.1.6/nanoCEM/cem_utils.py` & `nanoCEM-0.0.1.8/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.6/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.1.8/nanoCEM/current_events_magnifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,10 +152,10 @@
     #     else:
     #         args.pos = args.pos + args.base_shift
     percentile_filter=False
     if aligned_num_wt > 50 and aligned_num_ivt > 50:
         percentile_filter=True
 
     signal_plot(df, results_path, args.pos, base_list, title, 'merged',percentile_filter)
-    signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
-    signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
+    # signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
+    # signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `nanoCEM-0.0.1.6/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.1.8/nanoCEM/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.6/nanoCEM/normalization.py` & `nanoCEM-0.0.1.8/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.6/nanoCEM/plot.py` & `nanoCEM-0.0.1.8/nanoCEM/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,44 +101,46 @@
     else:
         new_df = None
 
 
         for item in item_list:
             # collect data
             temp = df[[item, 'position', 'type']].copy()
-            temp.columns = ['value', 'position', 'type']
+            temp.columns = ['value', 'position', 'Group']
             temp.loc[:, 'stats'] = item
             if filter and item!='Dwell time':
                 sig_min, sig_max = np.percentile(temp['value'], SIG_PCTL_RANGE)
                 sig_diff = sig_max - sig_min
                 ylim_tuple = [sig_min - sig_diff * 0.1, sig_max + sig_diff * 0.1]
                 temp = temp[(temp['value'] >= ylim_tuple[0]) & (temp['value'] <= ylim_tuple[1])]
             if new_df is None:
                 new_df = temp
             else:
                 new_df = pd.concat([new_df, temp], axis=0)
 
-        plot = p9.ggplot(new_df, p9.aes(x='position', y="value", fill='type')) \
+        plot = p9.ggplot(new_df, p9.aes(x='position', y="value", fill='Group')) \
                + p9.theme_bw() \
                + p9.scale_fill_manual(values={"Sample": "#ff6f91", "Control": "#7389af", "Single": "#a3abbd"}) \
                + p9.scale_x_discrete(labels=list(base_list)) \
                + p9.theme(
             figure_size=(8, 8),
             panel_grid_minor=p9.element_blank(),
             axis_text=p9.element_text(size=13),
             axis_title=p9.element_text(size=13),
             title=p9.element_text(size=13),
+            legend_position='bottom',
+            legend_title=p9.element_blank(),
             strip_text=p9.element_text(size=13),
-            legend_position='none',
-            strip_background=p9.element_rect(alpha=0)
+            strip_background=p9.element_rect(alpha=0),
+
         ) \
                + p9.facet_grid('stats ~', scales='free_y')
         plot = plot + p9.labs(title=title, x=str(pos + 1), y='')
 
-        if new_df['type'].drop_duplicates().shape[0] == 1:
+        if new_df['Group'].drop_duplicates().shape[0] == 1:
             plot2 = plot + p9.geom_violin(color='none', position=p9.position_dodge(0.9), width=1)
             plot2 = plot2 + p9.geom_boxplot(outlier_shape='', position=p9.position_dodge(0.9), size=0.2, width=0.1)
             plot2.save(filename=results_path + "/Merged_single.pdf", dpi=300)
         else:
             plot1 = plot + p9.geom_boxplot(outlier_shape='', position=p9.position_dodge(0.9), size=0.2, width=0.75,alpha = 0.8)
             plot1.save(filename=results_path + "/Merged_boxplot.pdf", dpi=300)
             plot2 = plot + p9.geom_violin(style='left-right', position=p9.position_dodge(0), color='none', width=1.5,alpha = 0.8)
@@ -166,8 +168,8 @@
     )
     # plot.save(filename="/home/zhguo/Dropbox/@labfiles/projects/GUO/ONT_showcase_tool/plot/signal.pdf", dpi=300)
     for item in start:
         plot = plot + p9.geom_vline(xintercept=item, linetype='dashed', color='red')
     print(plot)
     # plot.save(filename="/home/zhguo/Dropbox/@labfiles/projects/GUO/ONT_showcase_tool/plot/norm_signal_aligned.pdf", dpi=300)
 
-    print(1)
+    # print(1)
```

### Comparing `nanoCEM-0.0.1.6/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.1.8/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.6/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.1.8/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.6/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,16 @@
-Metadata-Version: 2.1
-Name: nanoCEM
-Version: 0.0.1.6
-Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
-Home-page: https://github.com/lrslab/current_events_magnifier
-Author: GUO Zhihao
-Author-email: qhuozhihao@icloud.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nanoCEM
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
-Here is an example that show the difference of A2030 on 23S rRNA.
+Here is a quick example help the user confirm the installation that show the difference of A2030 on 23S rRNA.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
 ## Before start, you should know
 ### Re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
@@ -40,19 +26,22 @@
 This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
 In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo. However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
+```sh
+pip install nanoCEM==0.0.1.8
+```
 
+Other tools if you needed
 ```sh
-pip install nanoCEM==0.0.4.4
-pip install ont-fast5-api
-conda install -c bioconda f5c slow5tools
+pip install ont-fast5-api pod
+conda install -c bioconda f5c slow5tools minimap2 
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 current_events_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
```

### Comparing `nanoCEM-0.0.1.6/setup.py` & `nanoCEM-0.0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.1.6",
+    version="0.0.1.8",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
-    description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
-                It supports two re-squiggle pipeline(Tombo and f5c).',
+    description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
+                It supports two re-squiggle program(tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/lrslab/current_events_magnifier",
+    url="https://github.com/lrslab/nanoCEM",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7,<3.10',
```

