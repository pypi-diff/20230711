# Comparing `tmp/wgd-2.0.19.tar.gz` & `tmp/wgd-2.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wgd-2.0.19.tar", last modified: Sun Jun 18 07:45:54 2023, max compression
+gzip compressed data, was "dist/wgd-2.0.20.tar", last modified: Tue Jul 11 15:20:58 2023, max compression
```

## Comparing `wgd-2.0.19.tar` & `wgd-2.0.20.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-18 07:45:54.949756 wgd-2.0.19/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.19/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    48426 2023-06-18 07:45:54.949756 wgd-2.0.19/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    48188 2023-06-18 07:41:38.000000 wgd-2.0.19/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)    52989 2023-06-18 07:39:20.000000 wgd-2.0.19/cli.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-06-18 07:45:54.949756 wgd-2.0.19/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-06-18 07:42:00.000000 wgd-2.0.19/setup.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-18 07:45:54.933493 wgd-2.0.19/test/
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-06-06 22:05:06.000000 wgd-2.0.19/test/test_core.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-18 07:45:54.949756 wgd-2.0.19/wgd/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.19/wgd/__init__.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.19/wgd/beast.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.19/wgd/cluster.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.19/wgd/codeml.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   135263 2023-06-15 13:48:21.000000 wgd-2.0.19/wgd/core.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.19/wgd/mcmctree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.19/wgd/mix.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   103616 2023-06-06 22:05:06.000000 wgd-2.0.19/wgd/peak.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4722 2023-06-06 22:05:06.000000 wgd-2.0.19/wgd/postplot.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17378 2023-06-15 09:47:26.000000 wgd-2.0.19/wgd/syn.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    28647 2023-06-06 22:05:06.000000 wgd-2.0.19/wgd/utils.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   145288 2023-06-18 06:57:28.000000 wgd-2.0.19/wgd/viz.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-18 07:45:54.949756 wgd-2.0.19/wgd.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    48426 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      385 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/top_level.txt
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-07-11 15:20:58.183107 wgd-2.0.20/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.20/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    48708 2023-07-11 15:20:58.183107 wgd-2.0.20/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    48470 2023-06-19 20:26:51.000000 wgd-2.0.20/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    55914 2023-07-11 15:15:15.000000 wgd-2.0.20/cli.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-07-11 15:20:58.183107 wgd-2.0.20/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-07-11 15:19:42.000000 wgd-2.0.20/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-07-11 15:20:58.157382 wgd-2.0.20/test/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-06-06 22:05:06.000000 wgd-2.0.20/test/test_core.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-07-11 15:20:58.173016 wgd-2.0.20/wgd/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.20/wgd/__init__.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.20/wgd/beast.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.20/wgd/cluster.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.20/wgd/codeml.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   144746 2023-07-11 14:22:15.000000 wgd-2.0.20/wgd/core.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.20/wgd/mcmctree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.20/wgd/mix.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   117915 2023-07-11 15:14:38.000000 wgd-2.0.20/wgd/peak.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4722 2023-06-06 22:05:06.000000 wgd-2.0.20/wgd/postplot.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    18160 2023-06-22 10:03:12.000000 wgd-2.0.20/wgd/syn.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31523 2023-06-23 20:25:14.000000 wgd-2.0.20/wgd/utils.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   159099 2023-06-26 11:43:50.000000 wgd-2.0.20/wgd/viz.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-07-11 15:20:58.183107 wgd-2.0.20/wgd.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    48708 2023-07-11 15:20:58.000000 wgd-2.0.20/wgd.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      385 2023-07-11 15:20:58.000000 wgd-2.0.20/wgd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-07-11 15:20:58.000000 wgd-2.0.20/wgd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-07-11 15:20:58.000000 wgd-2.0.20/wgd.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-07-11 15:20:58.000000 wgd-2.0.20/wgd.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-07-11 15:20:58.000000 wgd-2.0.20/wgd.egg-info/top_level.txt
```

### Comparing `wgd-2.0.19/LICENSE` & `wgd-2.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `wgd-2.0.19/PKG-INFO` & `wgd-2.0.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgd
-Version: 2.0.19
+Version: 2.0.20
 Summary: wgd
 Home-page: http://github.com/heche-psb/wgd
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,15 +41,15 @@
 
 Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
 
 The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
 
 ## Installation
 
-The easiest way to install `wgd v2` is using PYPI
+The easiest way to install `wgd v2` is using PYPI. Note that if you want to get the latest update, we suggest installing from the source, since the update on PYPI will be delayed compared to here in the source.
 
 ```
 pip install wgd
 ```
 
 To install `wgd v2` in a virtual environment, the following command lines could be used.
 
@@ -500,15 +500,15 @@
 (((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
 ```
 
 ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
 
 As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
 
-If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below. Note that the order of given `spair` options decides the color of the *K*<sub>S</sub> distribution of each species pair.
 
 ```
 wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
 ```
 
 Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
```

### Comparing `wgd-2.0.19/README.md` & `wgd-2.0.20/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
 
 The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
 
 ## Installation
 
-The easiest way to install `wgd v2` is using PYPI
+The easiest way to install `wgd v2` is using PYPI. Note that if you want to get the latest update, we suggest installing from the source, since the update on PYPI will be delayed compared to here in the source.
 
 ```
 pip install wgd
 ```
 
 To install `wgd v2` in a virtual environment, the following command lines could be used.
 
@@ -489,15 +489,15 @@
 (((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
 ```
 
 ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
 
 As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
 
-If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below. Note that the order of given `spair` options decides the color of the *K*<sub>S</sub> distribution of each species pair.
 
 ```
 wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
 ```
 
 Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
```

### Comparing `wgd-2.0.19/cli.py` & `wgd-2.0.20/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         bsog(s,buscohmm,outdir,eval,nthreads,buscocutoff)
         endt(tmpdir,start,s)
     if collinearcoalescence:
         logging.info("Analyzing collinear coalescence")
         segmentsaps(genetable,listelements,anchorpoints,segments,outdir,s,nthreads,tree_method,treeset,msogcut)
         endt(tmpdir,start,s)
     if geneassign:
-        genes2fams(assign_method,seq2assign,fam2assign,outdir,s,nthreads,tmpdir,to_stop,cds,cscore,eval,start,normalizedpercent)
+        genes2fams(assign_method,seq2assign,fam2assign,outdir,s,nthreads,tmpdir,to_stop,cds,cscore,eval,start,normalizedpercent,tree_method,treeset)
     if orthoinfer:
         logging.info("Infering orthologous gene families")
         ortho_infer(sequences,s,outdir,tmpdir,to_stop,cds,cscore,inflation,eval,nthreads,getnsog,tree_method,treeset,msogcut,concat,testsog,normalizedpercent,bins=bins,nonormalization=nonormalization)
         if onlyortho: endt(tmpdir,start,s)
     if len(s) == 0:
         logging.error("No sequences provided!")
         return
@@ -325,30 +325,34 @@
 @click.option('--n_medoids', type=int, default=2, show_default=True, help="number of medoids to generate")
 @click.option('--kdemethod', '-km', type=click.Choice(['scipy', 'naivekde', 'treekde', 'fftkde']), default='scipy', show_default=True, help="kde method")
 @click.option('--n_clusters',type=int, default=5, show_default=True, help="number of clusters to plot Elbow loss function")
 @click.option('--kmedoids', is_flag=True,help="K-Medoids clustering method")
 @click.option('--guide', '-gd', type=click.Choice(['multiplicon', 'basecluster', 'segment']), default='segment', show_default=True, help="regime residing anchors")
 @click.option('--prominence_cutoff', '-prct', type=float, default=0.1, show_default=True, help='prominence cutoff of acceptable peaks')
 @click.option('--kstodate', '-kd', nargs=2, type=float, default=(0.5, 1.5), show_default=True, help='range of Ks to be dated')
+@click.option('--xlim', '-xl', nargs=2, type=float, default=(None, None), show_default=True, help='xlim of GMM Ks distribution')
+@click.option('--ylim', '-yl', nargs=2, type=float, default=(None, None), show_default=True, help='ylim of GMM Ks distribution')
 @click.option('--family', '-f', default=None, show_default=True, help='family to filter Ks upon')
 @click.option('--manualset', is_flag=True,help="Manually set Ks range of anchor pairs or multiplicons as CI")
 @click.option('--rel_height', '-rh', type=float, default=0.4, show_default=True, help='relative height at which the peak width is measured')
 @click.option('--ci', default=95, show_default=True,type=int, help='confidence level of log-normal distribution to date')
 @click.option('--hdr', default=95, show_default=True,type=int, help='highest density region (HDR) in a given distribution to date')
 @click.option('--heuristic', is_flag=True,help="heuristic CI for dating")
 @click.option('--kscutoff', '-kc', default=5, show_default=True, type=float, help='Ks Saturation cutoff for genes in Dating')
+@click.option('--showci', is_flag=True,help="show CI for original anchor Ks gmm analysis")
 def peak(**kwargs):
     """
     Infer peak and CI of Ks distribution.
     """
     _peak(**kwargs)
 
-def _peak(ks_distribution, anchorpoints, outdir, alignfilter, ksrange, bin_width, weights_outliers_included, method, seed, em_iter, n_init, components, boots, weighted, plot, bw_method, n_medoids, kdemethod, n_clusters, kmedoids, guide, prominence_cutoff, kstodate, family, rel_height, ci,manualset,segments,hdr,heuristic,listelements,multipliconpairs,kscutoff,gamma):
-    from wgd.peak import alnfilter, group_dS, log_trans, fit_gmm, fit_bgmm, add_prediction, bootstrap_kde, default_plot, get_kde, draw_kde_CI, draw_components_kde_bootstrap, fit_kmedoids, default_plot_kde, fit_apgmm_guide, fit_apgmm_ap, find_apeak, find_mpeak, retreive95CI, formatv2
+def _peak(ks_distribution, anchorpoints, outdir, alignfilter, ksrange, bin_width, weights_outliers_included, method, seed, em_iter, n_init, components, boots, weighted, plot, bw_method, n_medoids, kdemethod, n_clusters, kmedoids, guide, prominence_cutoff, kstodate, family, rel_height, ci,manualset,segments,hdr,heuristic,listelements,multipliconpairs,kscutoff,gamma,showci,xlim,ylim):
+    from wgd.peak import alnfilter, group_dS, log_trans, fit_gmm, fit_bgmm, add_prediction, bootstrap_kde, default_plot, get_kde, draw_kde_CI, draw_components_kde_bootstrap, fit_kmedoids, default_plot_kde, fit_apgmm_guide, fit_apgmm_ap, find_apeak, find_mpeak, retreive95CI
     from wgd.core import _mkdir
+    from wgd.utils import formatv2
     outpath = _mkdir(outdir)
     ksdf = pd.read_csv(ks_distribution,header=0,index_col=0,sep='\t')
     ksdf = formatv2(ksdf)
     if len(ksdf.columns) <4:
         logging.info("Begin to analyze peak of WGD dates")
         draw_kde_CI(kdemethod, outdir,ksdf,boots,bw_method,date_lower = 0,date_upper=4)
         exit()
@@ -357,22 +361,22 @@
         retreive95CI(family,ksdf_filtered,outdir,kstodate[0],kstodate[1])
         logging.info('Done')
         exit()
     fn_ksdf, weight_col = group_dS(ksdf_filtered)
     train_in = log_trans(fn_ksdf)
     if anchorpoints!= None:
         if kmedoids:
-            df_ap = fit_kmedoids(guide, anchorpoints, boots, kdemethod, bin_width, weighted, ksdf, ksdf_filtered, outdir, seed, n_medoids, em_iter=em_iter, plot=plot, n_kmedoids = n_clusters, segment = segments, multipliconpairs=multipliconpairs,listelement=listelements)
+            df_ap = fit_kmedoids(guide, anchorpoints, boots, kdemethod, bin_width, weighted, ksdf, ksdf_filtered, outdir, seed, n_medoids, em_iter=em_iter, plot=plot, n_kmedoids = n_clusters, segment = segments, multipliconpairs=multipliconpairs,listelement=listelements,user_xlim=xlim,user_ylim=ylim)
         else:
-            df_ap_mp = fit_apgmm_guide(hdr,guide,anchorpoints,ksdf,ksdf_filtered,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot,segment=segments,multipliconpairs=multipliconpairs,listelement=listelements,cutoff = kscutoff)
-            df_ap = fit_apgmm_ap(hdr,anchorpoints,ksdf_filtered,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot)
+            df_ap_mp = fit_apgmm_guide(hdr,guide,anchorpoints,ksdf,ksdf_filtered,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot,segment=segments,multipliconpairs=multipliconpairs,listelement=listelements,cutoff = kscutoff,user_xlim=xlim,user_ylim=ylim)
+            df_ap = fit_apgmm_ap(hdr,anchorpoints,ksdf_filtered,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot,heuristic,showCI=showci,cutoff = kscutoff,peak_threshold=prominence_cutoff,rel_height=rel_height,user_xlim=xlim,user_ylim=ylim)
         if heuristic:
-            find_apeak(df_ap,anchorpoints,os.path.basename(ks_distribution),outdir,peak_threshold=prominence_cutoff,na=False,rel_height=rel_height,ci=ci,user_low=kstodate[0],user_upp=kstodate[1],user=manualset)
-            find_apeak(df_ap,anchorpoints,os.path.basename(ks_distribution),outdir,peak_threshold=prominence_cutoff,na=True,rel_height=rel_height,ci=ci,user_low=kstodate[0],user_upp=kstodate[1],user=manualset)
-            find_mpeak(df_ap_mp,anchorpoints,os.path.basename(ks_distribution),outdir,guide,peak_threshold=prominence_cutoff,rel_height=rel_height,ci=ci,user_low=kstodate[0],user_upp=kstodate[1],user=manualset)
+            find_apeak(df_ap,anchorpoints,os.path.basename(ks_distribution),outdir,peak_threshold=prominence_cutoff,na=False,rel_height=rel_height,ci=ci,user_low=kstodate[0],user_upp=kstodate[1],user=manualset, kscutoff=kscutoff)
+            find_apeak(df_ap,anchorpoints,os.path.basename(ks_distribution),outdir,peak_threshold=prominence_cutoff,na=True,rel_height=rel_height,ci=ci,user_low=kstodate[0],user_upp=kstodate[1],user=manualset, kscutoff=kscutoff)
+            find_mpeak(df_ap_mp,anchorpoints,os.path.basename(ks_distribution),outdir,guide,peak_threshold=prominence_cutoff,rel_height=rel_height,ci=ci,user_low=kstodate[0],user_upp=kstodate[1],user=manualset,kscutoff=kscutoff)
         logging.info('Done')
         exit()
     get_kde(kdemethod,outdir,fn_ksdf,ksdf_filtered,weighted,ksrange[0],ksrange[1])
     if method == 'gmm':
         out_file = os.path.join(outdir, "AIC_BIC.pdf")
         models, aic, bic, besta, bestb, N = fit_gmm(out_file, train_in, seed, components[0], components[1], em_iter=em_iter, n_init=n_init)
     if method == 'bgmm':
@@ -382,19 +386,19 @@
         ksdf_predict = add_prediction(ksdf,fn_ksdf,train_in,m)
         ksdf_predict.to_csv(fname,header=True,index=True,sep='\t')
         logging.info("Plotting components-annotated Ks distribution for {} components model".format(n))
         #fig = default_plot(ksdf_predict, title=os.path.basename(fname), bins=50, ylabel="Duplication events", nums = int(n),plot = plot)
         #fig.savefig(fname + "_Ks.svg")
         #fig.savefig(fname + "_Ks.pdf")
         #plt.close()
-        fig,ylim,yticks = default_plot_kde(ksdf_predict, title=os.path.basename(fname), bins=50, ylabel="Duplication events", nums = int(n),plot = 'identical')
+        fig,ylim,yticks = default_plot_kde(ksdf_predict, title=os.path.basename(fname), bins=50, ylabel="Duplication events", nums = int(n),plot = 'identical',user_xlim=xlim,user_ylim=ylim)
         fig.savefig(fname + "_Ks_kde.svg")
         fig.savefig(fname + "_Ks_kde.pdf")
         plt.close()
-        fig = default_plot(ksdf_predict, title=os.path.basename(fname), bins=50, ylabel="Duplication events", nums = int(n),plot = plot, ylim=ylim,yticks=yticks)
+        fig = default_plot(ksdf_predict, title=os.path.basename(fname), bins=50, ylabel="Duplication events", nums = int(n),plot = plot, ylim=ylim,yticks=yticks,user_xlim=xlim,user_ylim=ylim)
         fig.savefig(fname + "_Ks.svg")
         fig.savefig(fname + "_Ks.pdf")
         plt.close()
         #ksdf_predict_filter = alnfilter(ksdf_predict,weights_outliers_included,alignfilter[0],alignfilter[1],alignfilter[2],ksrange[0],ksrange[1])
         #draw_components_kde_bootstrap(kdemethod,outdir,int(n),ksdf_predict_filter,weighted,boots,bin_width)
     #mean_modes, std_modes, mean_medians, std_medians = bootstrap_kde(kdemethod,outdir, train_in, ksrange[0], ksrange[1], boots, bin_width, ksdf_filtered, weight_col, weighted = weighted)
     logging.info("Done")
@@ -480,15 +484,17 @@
     logging.info("Making plots")
     df = apply_filters(ksdb.df, [("dS", 0., 5.)])
     ylabel = "Duplications"
     if len(sequences) == 2:
         ylabel = "RBH orthologs"
     elif len(sequences) > 2:
         ylabel = "Homologous pairs"
-    if len(spair)!= 0:  multi_sp_plot(df,spair,spgenemap,outdir,onlyrootout,title=prefix,ylabel=ylabel,ksd=True,reweight=reweight,sptree=speciestree,extraparanomeks=extraparanomeks, ap = anchorpoints,plotkde=plotkde,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components)
+    if len(spair)!= 0:
+        multi_sp_plot(df,spair,spgenemap,outdir,onlyrootout,title=prefix,ylabel=ylabel,ksd=True,reweight=reweight,sptree=speciestree,extraparanomeks=extraparanomeks, ap = anchorpoints,plotkde=plotkde,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components,na=True)
+        multi_sp_plot(df,spair,spgenemap,outdir,onlyrootout,title=prefix,ylabel=ylabel,ksd=True,reweight=reweight,sptree=speciestree,extraparanomeks=extraparanomeks, ap = anchorpoints,plotkde=plotkde,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components)
     fig = default_plot(df, title=prefix, bins=50, ylabel=ylabel)
     fig.savefig(os.path.join(outdir, "{}.ksd.svg".format(prefix)))
     fig.savefig(os.path.join(outdir, "{}.ksd.pdf".format(prefix)))
     plt.close()
     if tmpdir is None:
         [x.remove_tmp(prompt=False) for x in seqs]
     end = timer()
@@ -521,26 +527,28 @@
 @click.option('--plotapgmm', '-pag', is_flag=True, help='plot mixture modeling of anchor pairs')
 @click.option('--plotelmm', '-pem', is_flag=True, help='plot elmm mixture modeling')
 @click.option('--components', '-n', nargs=2, default=(1, 4), show_default=True, help="range of number of components to fit")
 @click.option('--mingenenum', '-mgn', default=30, type=int, show_default=True, help="minimum number of genes on segments to be considered")
 @click.option('--plotsyn', '-psy', is_flag=True, help='plot synteny')
 @click.option('--dotsize', '-ds', type=float, default=1, show_default=True, help='size of dots')
 @click.option('--apalpha', '-aa', type=float, default=1, show_default=True, help='opacity of anchor dots')
-@click.option('--hoalpha', '-ha', type=float, default=0.1, show_default=True, help='opacity of homolog dots')
+@click.option('--hoalpha', '-ha', type=float, default=0, show_default=True, help='opacity of homolog dots')
+@click.option('--showrealtick', '-srt', is_flag=True, help='show the real tick in genes or bases')
+@click.option('--ticklabelsize', '-tls', type=float, default=5, show_default=True, help='label size of tick')
 def viz(**kwargs):
     """
     Visualization of Ks distribution or synteny
     """
     _viz(**kwargs)
 
-def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun,extraparanomeks,plotapgmm,plotelmm,components,mingenenum,plotsyn,dotsize,apalpha,hoalpha):
-    from wgd.viz import elmm_plot, apply_filters, multi_sp_plot, default_plot,all_dotplots,filter_by_minlength,dotplotunitgene,dotplotingene,filter_mingenumber
+def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun,extraparanomeks,plotapgmm,plotelmm,components,mingenenum,plotsyn,dotsize,apalpha,hoalpha,showrealtick,ticklabelsize):
+    from wgd.viz import elmm_plot, apply_filters, multi_sp_plot, default_plot,all_dotplots,filter_by_minlength,dotplotunitgene,dotplotingene,filter_mingenumber,dotplotingeneoverall
     from wgd.core import _mkdir
     from wgd.syn import get_anchors,get_multi,get_segments_profile,get_chrom_gene,get_mp_geneorder,transformunit
-    from wgd.peak import formatv2
+    from wgd.utils import formatv2
     if datafile!=None: prefix = os.path.basename(datafile)
     _mkdir(outdir)
     if plotsyn:
         df = None
         if datafile!=None:
             ksdb_df = pd.read_csv(datafile,header=0,index_col=0,sep='\t')
             ksdb_df = formatv2(ksdb_df)
@@ -550,28 +558,32 @@
         df_anchor,orig_anchors = get_anchors('',userdf=anchorpoints)
         df_multi = get_multi('',userdf2=multiplicon)
         ordered_genes_perchrom_allsp, gene_orders = get_chrom_gene(table,outdir)
         #ordered_mp = get_mp_geneorder(gene_orders,'',outdir,table,userdf4=multipliconpairs)
         segs = get_segments_profile(df_multi,keepredun,'',userdf3=segments)
         segs,table,df_multi,removed_scfa = filter_by_minlength(table,segs,minlen,df_multi,keepredun,outdir,minseglen)
         segs_gene_unit, gene_order_dict_allsp = transformunit(segs,ordered_genes_perchrom_allsp,outdir)
-        segs = filter_mingenumber(segs_gene_unit,mingenenum)
-        dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=df_anchor,ksdf=df,maxsize=maxsize,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha)
+        segs = filter_mingenumber(segs_gene_unit,mingenenum,outdir,len(gene_order_dict_allsp))
+        dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=df_anchor,ksdf=df,maxsize=maxsize,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha,showrealtick=showrealtick, las = ticklabelsize)
+        if len(ordered_genes_perchrom_allsp)>1: dotplotingeneoverall(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=df_anchor,ksdf=df,maxsize=maxsize,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha,showrealtick=showrealtick, las=ticklabelsize)
         #dotplotunitgene(ordered_genes_perchrom_allsp,segs_gene_unit,removed_scfa,outdir,mingenenum,table_orig,ordered_mp,ksdf=df)
-        figs = all_dotplots(table, segs, df_multi, minseglen, anchors=df_anchor, maxsize=maxsize, minlen=minlen, outdir=outdir, Ks = df, dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha)
+        figs = all_dotplots(table, segs, df_multi, minseglen, anchors=df_anchor, maxsize=maxsize, minlen=minlen, outdir=outdir, Ks = df, dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha, showrealtick=showrealtick, las=ticklabelsize)
         for k, v in figs.items():
             v.savefig(os.path.join(outdir, "{}.dot.svg".format(k)))
             v.savefig(os.path.join(outdir, "{}.dot.pdf".format(k)))
             v.savefig(os.path.join(outdir, "{}.dot.png".format(k)),dpi=500)
         logging.info('Done')
         exit()
     ksdb_df = pd.read_csv(datafile,header=0,index_col=0,sep='\t')
+    ksdb_df = formatv2(ksdb_df)
     df = apply_filters(ksdb_df, [("dS", 0., 5.)])
     ylabel = "Duplications" if spair == () else "Homologous pairs"
-    if len(spair)!= 0: multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title=prefix,ylabel=ylabel,viz=True,plotkde=plotkde,reweight=reweight,sptree=speciestree,ap = anchorpoints, extraparanomeks=extraparanomeks,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components,max_EM_iterations=em_iterations,num_EM_initializations=em_initializations,peak_threshold=prominence_cutoff,rel_height=rel_height)
+    if len(spair)!= 0:
+        multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title=prefix,ylabel=ylabel,viz=True,plotkde=plotkde,reweight=reweight,sptree=speciestree,ap = anchorpoints, extraparanomeks=extraparanomeks,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components,max_EM_iterations=em_iterations,num_EM_initializations=em_initializations,peak_threshold=prominence_cutoff,rel_height=rel_height, na=True)
+        multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title=prefix,ylabel=ylabel,viz=True,plotkde=plotkde,reweight=reweight,sptree=speciestree,ap = anchorpoints, extraparanomeks=extraparanomeks,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components,max_EM_iterations=em_iterations,num_EM_initializations=em_initializations,peak_threshold=prominence_cutoff,rel_height=rel_height)
     fig = default_plot(df, title=prefix, bins=50, ylabel=ylabel)
     fig.savefig(os.path.join(outdir, "{}.ksd.svg".format(prefix)))
     fig.savefig(os.path.join(outdir, "{}.ksd.pdf".format(prefix)))
     plt.close()
     if spair == ():
         logging.info('Exponential-Lognormal mixture modeling on node-weighted Ks distribution')
         elmm_plot(df,prefix,outdir,max_EM_iterations=em_iterations,num_EM_initializations=em_initializations,peak_threshold=prominence_cutoff,rel_height=rel_height)
@@ -586,14 +598,15 @@
     help="ks distribution tsv file (optional, see `wgd ksd`)")
 @click.option('--outdir', '-o', default='wgd_syn', show_default=True, 
     help='output directory')
 @click.option('--feature', '-f', default='gene', show_default=True,
     help="keyword for parsing the genes from the GFF file (column 3)")
 @click.option('--attribute', '-a', default='ID', show_default=True,
     help="keyword for parsing the gene IDs from the GFF file (column 9)")
+@click.option('--additionalgffinfo', '-atg', default=None,multiple=True, show_default=True, help='the feature and attribute info of additional gff3 if different')
 @click.option('--minlen', '-ml', default=-1, show_default=True,
     help="minimum length of a genomic element to be included in dotplot.")
 @click.option('--maxsize', '-ms', default=200, show_default=True,
     help="maximum family size to include in analysis.")
 @click.option('--ks_range', '-r', nargs=2, default=(0, 5), show_default=True,
     type=float, help='Ks range to use for colored dotplot')
 @click.option('--iadhore_options', default="",
@@ -601,39 +614,41 @@
          "e.g. gap_size=30,q_value=0.75,prob_cutoff=0.05")
 @click.option('--ancestor', '-ac', default=None,show_default=True,help='assumed ancestor species')
 @click.option('--minseglen', '-mg', default=10000, show_default=True, help="min length of segments in ratio if <= 1")
 @click.option('--keepredun', '-kr', is_flag=True, help='keep redundant multiplicons')
 @click.option('--mingenenum', '-mgn', default=30, type=int, show_default=True, help="minimum number of genes on segments to be considered")
 @click.option('--dotsize', '-ds', type=float, default=1, show_default=True, help='size of dots')
 @click.option('--apalpha', '-aa', type=float, default=1, show_default=True, help='opacity of anchor dots')
-@click.option('--hoalpha', '-ha', type=float, default=0.1, show_default=True, help='opacity of homolog dots')
+@click.option('--hoalpha', '-ha', type=float, default=0, show_default=True, help='opacity of homolog dots')
+@click.option('--showrealtick', '-srt', is_flag=True, help='show the real tick in genes or bases')
+@click.option('--ticklabelsize', '-tls', type=float, default=5, show_default=True, help='label size of tick')
 def syn(**kwargs):
     """
     Co-linearity and anchor inference using I-ADHoRe.
     """
     _syn(**kwargs)
 
 def _syn(families, gff_files, ks_distribution, outdir, feature, attribute,
-        minlen, maxsize, ks_range, iadhore_options, ancestor, minseglen, keepredun, mingenenum, dotsize, apalpha, hoalpha):
+        minlen, maxsize, ks_range, iadhore_options, ancestor, minseglen, keepredun, mingenenum, dotsize, apalpha, hoalpha, additionalgffinfo, showrealtick, ticklabelsize):
     """
     Co-linearity and anchor inference using I-ADHoRe.
     """
     from wgd.syn import make_gene_table, configure_adhore, run_adhore
     from wgd.syn import get_anchors, get_anchor_ksd, get_segments_profile, get_multi, get_chrom_gene, transformunit, get_mp_geneorder
-    from wgd.viz import default_plot, apply_filters, all_dotplots, syntenic_dotplot_ks_colored,filter_by_minlength,dotplotunitgene,dotplotingene,filter_mingenumber
-    from wgd.peak import formatv2
+    from wgd.viz import default_plot, apply_filters, all_dotplots, syntenic_dotplot_ks_colored,filter_by_minlength,dotplotunitgene,dotplotingene,filter_mingenumber,dotplotingeneoverall
+    from wgd.utils import formatv2
     # non-default options for I-ADHoRe
     iadhore_opts = {x.split("=")[0].strip(): x.split("=")[1].strip()
                for x in iadhore_options.split(",") if x != ""}
     if len(iadhore_opts) > 0:
         logging.info("I-ADHoRe 3.0 options: {}".format(iadhore_opts))
     # read families and make table
     prefix = os.path.basename(families)
     fams = pd.read_csv(families, index_col=0, sep="\t")
-    table = make_gene_table(gff_files, fams, feature, attribute)
+    table = make_gene_table(gff_files, fams, feature, attribute, additionalgffinfo)
     table_orig = table.copy()
     if len(table.dropna().index) == 0:
         logging.error("No genes from families file `{}` found in the GFF file "
                 "for `feature={}` and `attribute={}`, please double check command " 
                 "settings.".format(families, feature, attribute))
         exit(1)
     if len(table.dropna()) < 1000:
@@ -659,38 +674,40 @@
         exit(1)
     anchors.to_csv(os.path.join(outdir, "anchors.csv"))
     #ap_order_permlt = getmltorder(orig_anchors,multi,gene_orders)
     segs = get_segments_profile(multi,keepredun,out_path)
     #segmentpair_order = get_segmentpair_order(orig_anchors,segs,table,gene_orders)
     segs,table,multi,removed_scfa = filter_by_minlength(table,segs,minlen,multi,keepredun,outdir,minseglen)
     segs_gene_unit, gene_order_dict_allsp = transformunit(segs,ordered_genes_perchrom_allsp,outdir)
-    segs = filter_mingenumber(segs_gene_unit,mingenenum)
+    segs = filter_mingenumber(segs_gene_unit,mingenenum,outdir,len(gene_order_dict_allsp))
     #if ks_distribution: segs_gene_unit_ks = getsegks(segs_gene_unit,ks_distribution,ordered_genes_perchrom_allsp)
     df_ks = None
     if ks_distribution!=None:
         ksdb_df = pd.read_csv(ks_distribution,header=0,index_col=0,sep='\t')
         ksdb_df = formatv2(ksdb_df)
         df_ks = apply_filters(ksdb_df, [("dS", 0., 5.)])
-    dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=anchors,ksdf=df_ks,maxsize=maxsize,dotsize=dotsize,apalpha=apalpha, hoalpha=hoalpha)
+    dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=anchors,ksdf=df_ks,maxsize=maxsize,dotsize=dotsize,apalpha=apalpha, hoalpha=hoalpha, showrealtick=showrealtick, las = ticklabelsize)
+    if len(gff_files)>1: dotplotingeneoverall(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=anchors,ksdf=df_ks,maxsize=maxsize,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha, showrealtick=showrealtick, las = ticklabelsize)
     #dotplotunitgene(ordered_genes_perchrom_allsp,segs_gene_unit,removed_scfa,outdir,mingenenum,table_orig,ordered_mp,ksdf=df_ks)
     # dotplot
     #logging.info("Generating dot plots")
-    figs = all_dotplots(table, segs, multi, minseglen, anchors=anchors, maxsize=maxsize, minlen=minlen, outdir=outdir, ancestor=ancestor, Ks = df_ks, dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha) 
+    figs = all_dotplots(table, segs, multi, minseglen, anchors=anchors, maxsize=maxsize, minlen=minlen, outdir=outdir, ancestor=ancestor, Ks = df_ks, dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha, las = ticklabelsize) 
     for k, v in figs.items():
         v.savefig(os.path.join(outdir, "{}.dot.svg".format(k)))
         v.savefig(os.path.join(outdir, "{}.dot.pdf".format(k)))
         v.savefig(os.path.join(outdir, "{}.dot.png".format(k)),dpi=500)
     plt.close()
 
     # anchor Ks distributions
     if ks_distribution:
         ylabel = "Duplications"
         if len(gff_files) == 2:
             ylabel = "RBH orthologs"
         ksd = pd.read_csv(ks_distribution, sep="\t", index_col=0)
+        ksd = formatv2(ksd)
         anchor_ks = get_anchor_ksd(ksd, anchors)
         anchor_ks.to_csv(os.path.join(outdir, "{}.anchors.ks.tsv".format(prefix)),sep='\t')
         a = apply_filters(ksd,       [("dS", 0, 5.)])
         b = apply_filters(anchor_ks, [("dS", 0, 5.)])
         logging.info("Generating anchor Ks distribution")
         fig = default_plot(a, b, title=prefix, bins=50, ylabel=ylabel)
         fig.savefig(os.path.join(outdir, "{}.ksd.svg".format(prefix)))
```

### Comparing `wgd-2.0.19/setup.py` & `wgd-2.0.20/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='wgd',
-    version='2.0.19',
+    version='2.0.20',
     packages=['wgd'],
     url='http://github.com/heche-psb/wgd',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='wgd',
     long_description=long_description,
```

### Comparing `wgd-2.0.19/test/test_core.py` & `wgd-2.0.20/test/test_core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.19/wgd/__init__.py` & `wgd-2.0.20/wgd/__init__.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.19/wgd/beast.py` & `wgd-2.0.20/wgd/beast.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.19/wgd/cluster.py` & `wgd-2.0.20/wgd/cluster.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.19/wgd/codeml.py` & `wgd-2.0.20/wgd/codeml.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.19/wgd/core.py` & `wgd-2.0.20/wgd/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1510,35 +1510,45 @@
     for i in range(3,end):
         pair = dfo.iloc[i,0].split()
         f,g,score = pair[0][:-4],pair[2],float(pair[5])
         f_g_score[f][g] = score
     for fid in df.index:
         genes_genes = df.loc[[fid],:].dropna(axis=1).loc[fid,:]
         for genes in genes_genes:
-            for gene in genes.split(', '): score_per_f[fid].append(f_g_score[fid][gene])
-    for fid,vs in score_per_f.items(): cutoff_per_f[fid] = min(vs)*0.9
+            for gene in genes.split(', '):
+                if f_g_score[fid].get(gene) == None:
+                    logging.info("{0} in {1} has no hits, please double check this perhaps misassigned gene".format(gene,fid))
+                    continue
+                score_per_f[fid].append(f_g_score[fid][gene])
+    for fid,vs in score_per_f.items():
+        if len(vs) == 0:
+            logging.info("Genes in {} all have no hits, please double check the authenticity of this family".format(fid))
+            cutoff_per_f[fid] = 0
+        else: cutoff_per_f[fid] = min(vs)*0.9
     for fid,cutoff in cutoff_per_f.items(): logging.info('The cutoff score for family {} is {:.2f}'.format(fid,cutoff))
     return cutoff_per_f
 
 def scanrefer(refer_fp,hmmf,outdir,eval):
     cmd = ['hmmpress'] + [hmmf]
     sp.run(cmd, stdout=sp.PIPE,stderr=sp.PIPE)
-    pf = os.path.join(outdir,os.path.basename(refer_fp).strip('.pep'))
+    #pf = os.path.join(outdir,os.path.basename(refer_fp).strip('.pep'))
+    pf = os.path.join(outdir,os.path.basename(refer_fp)[:-4])
     cmd = ['hmmscan','-o', '{}.txt'.format(pf), '--tblout', '{}.tbl'.format(pf), '--domtblout', '{}.dom'.format(pf), '--pfamtblout', '{}.pfam'.format(pf), '--noali', '-E', '{}'.format(eval), hmmf, refer_fp]
     sp.run(cmd, stdout=sp.PIPE,stderr=sp.PIPE)
     out = '{}.tbl'.format(pf)
     return out
 
 def hmmerscan(outdir,querys,hmmf,eval,nthreads,skipress=False):
     if not skipress:
         cmd = ['hmmpress'] + [hmmf]
         sp.run(cmd, stdout=sp.PIPE,stderr=sp.PIPE)
     cmds = []
     outs = []
-    yprefix = lambda i: os.path.join(outdir,os.path.basename(i).strip('.pep'))
+    #yprefix = lambda i: os.path.join(outdir,os.path.basename(i).strip('.pep'))
+    yprefix = lambda i: os.path.join(outdir,os.path.basename(i)[:-4])
     for s in querys:
         s.orig_profasta()
         pf = yprefix(s.orig_pro_fasta)
         cmd = ['hmmscan','-o', '{}.txt'.format(pf), '--tblout', '{}.tbl'.format(pf), '--domtblout', '{}.dom'.format(pf), '--pfamtblout', '{}.pfam'.format(pf), '--noali', '-E', '{}'.format(eval), hmmf, s.orig_pro_fasta]
         cmds.append(cmd)
         outs.append('{}.tbl'.format(pf))
     Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(sp.run)(cmd,stdout=sp.PIPE,stderr=sp.PIPE) for cmd in cmds)
@@ -1558,16 +1568,18 @@
                 df.loc[f,sp] = outdict[sp][f][0]
     df.to_csv(fname,header = True, index = True,sep = '\t')
     return df
 
 def modifydf(df,outs,outdir,fam2assign,sogtest = False, bhmm = False, cutoff = None, use_cf = None):
     if cutoff != None: ctf = pd.read_csv(cutoff, header = None,index_col = 0,sep='\t')
     if not bhmm: fname = os.path.join(outdir,os.path.basename(fam2assign)+'.assigned')
-    yb = lambda i:os.path.basename(i).strip('.tbl')
-    if sogtest: yb = lambda i:os.path.basename(i).strip('.tbl') + '_assigned'
+    #yb = lambda i:os.path.basename(i).strip('.tbl')
+    yb = lambda i:os.path.basename(i)[:-4]
+    #if sogtest: yb = lambda i:os.path.basename(i).strip('.tbl') + '_assigned'
+    if sogtest: yb = lambda i:os.path.basename(i)[:-4] + '_assigned'
     outdict = {yb(i):{} for i in outs}
     if not bhmm: f_g_score = {fid:{} for fid in df.index}
     for out in outs:
         #print(yb(out))
         dfo = pd.read_csv(out,header = None, index_col=False,sep ='\t')
         end = dfo.shape[0] - 10
         for i in range(3,end):
@@ -1623,44 +1635,253 @@
         if sogtest:
             l = int(len(df.columns)/2)
             df2 = df.iloc[:,:l]
             df2.to_csv(fname,header = True, index = True,sep = '\t')
         else: df.to_csv(fname,header = True, index = True,sep = '\t')
     return df
 
-def getassignfasta(df,s,querys,outdir):
+def getassignfasta(df,s,querys,outdir,second=False,third=False):
     yids = lambda i: ', '.join(list(df.loc[i,:].dropna())).split(', ')
     for i in querys: s.merge_seq(i)
-    p = _mkdir(os.path.join(outdir,'Orthologues_Sequence_Assigned'))
+    if second:
+        p = _mkdir(os.path.join(outdir,'Orthologues_Sequence_Assigned_Furtherscorefiltered'))
+    elif third:
+        p = _mkdir(os.path.join(outdir,'Orthologues_Sequence_Assigned_Furtherscorefiltered_Tree-based'))
+    else:
+        p = _mkdir(os.path.join(outdir,'Orthologues_Sequence_Assigned'))
     pc = _mkdir(os.path.join(p,'cds'))
     pp = _mkdir(os.path.join(p,'pep'))
+    pps,glength = [],{}
     for i in df.index:
         fc = os.path.join(pc,i+'.cds')
         fp = os.path.join(pp,i+'.pep')
-        for gi in yids(i):
-            with open(fc,'a') as f: f.write('>{}\n{}\n'.format(gi,s.cds_sequence[s.idmap[gi]]))
-            with open(fp,'a') as f: f.write('>{}\n{}\n'.format(gi,s.pro_sequence[s.idmap[gi]]))
+        pps.append(fp)
+        with open(fc,'w') as f:
+            for gi in yids(i):
+                if gi == '':
+                    continue
+                f.write('>{}\n{}\n'.format(gi,s.cds_sequence[s.idmap[gi]]))
+        with open(fp,'w') as f:
+            for gi in yids(i):
+                if gi == '':
+                    continue
+                f.write('>{}\n{}\n'.format(gi,s.pro_sequence[s.idmap[gi]]))
+                glength[gi] = len(s.pro_sequence[s.idmap[gi]])
+        #for gi in yids(i):
+        #    with open(fc,'a') as f: f.write('>{}\n{}\n'.format(gi,s.cds_sequence[s.idmap[gi]]))
+        #    with open(fp,'a') as f: f.write('>{}\n{}\n'.format(gi,s.pro_sequence[s.idmap[gi]]))
+    return pps,glength
 
-def hmmer4g2f(outdir,s,nthreads,querys,df,eval,fam2assign):
+def hmmer4g2f(outdir,s,nthreads,querys,df,eval,fam2assign,Noldsp,Nnewsp,gsmap,tmpdir,tree_method,treeset):
     hmmerbuild(df,s,outdir,nthreads)
     hmmf = concathmm(outdir,df)
     c_f = reference_hmmscan(df,s,hmmf,outdir,eval)
     outs = hmmerscan(outdir,querys,hmmf,eval,nthreads,skipress=True)
     df = modifydf(df,outs,outdir,fam2assign,use_cf=c_f)
     fromgene2count(df,outdir,fam2assign)
-    getassignfasta(df,s,querys,outdir)
+    pps,glength = getassignfasta(df,s,querys,outdir)
+    df = postrbhcutoff(df,nthreads,eval,outdir,pps,glength,Noldsp,Nnewsp,gsmap,fam2assign,tmpdir)
+    pps,glength = getassignfasta(df,s,querys,outdir,second=True)
+    logging.info("Inferring gene trees using {}".format(tree_method))
+    treepaths = Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(finalinfertree)(fp,tree_method,treeset) for fp in pps)
+    logging.info("The path of tree files is at {}".format(os.path.join(outdir,'Orthologues_Sequence_Assigned_Furtherscorefiltered','pep')))
+    logging.info("Pruning the tree")
+    df = filtersp(treepaths,gsmap,Nnewsp,df)
+    fname = os.path.join(outdir,os.path.basename(fam2assign)+".assigned.furtherscorefiltered.tree-based")
+    df.to_csv(fname,header=True,index=True,sep='\t')
+    fromgene2count(df,outdir,fam2assign,third=True)
+    getassignfasta(df,s,querys,outdir,third=True)
+
+def prunebranch(allchildren,newsps,df,gsmaps,fam):
+    for sp in newsps: df.loc[fam,sp] = ''
+    for gene in allchildren:
+        if gsmaps[gene] not in newsps:
+            continue
+        df.loc[fam,gsmaps[gene]] = gene if df.loc[fam,gsmaps[gene]] == '' else ", ".join([df.loc[fam,gsmaps[gene]],gene])
+    return df
+
+def findsubfamily(tree,oldsps,newsps,df,fam,gsmaps):
+    tree.root_at_midpoint()
+    oldseqs = []
+    for sp in df.columns:
+        if sp in oldsps:
+            content = df.loc[fam,sp]
+            if type(content) == float or type(content) == np.float64 or content == '':
+                continue
+            oldseqs = oldseqs + content.split(", ")
+    mrca = tree.common_ancestor(*oldseqs)
+    tips = mrca.get_terminals()
+    allchildren = [tip.name for tip in tips]
+    df = prunebranch(allchildren,newsps,df,gsmaps,fam)
+    return df
+
+def filtersp(treepaths,gsmap,Nnewsp,df):
+    Noldsp = [i for i in df.columns if i not in Nnewsp]
+    treepaths = {fam:tp for tp,fam in zip(treepaths,df.index)}
+    for fam,tp in treepaths.items():
+        tree = Phylo.read(tp,'newick')
+        df = findsubfamily(tree,Noldsp,Nnewsp,df,fam,gsmap)
+    return df
+
+def waln(fpep,faln):
+    cmd = ["mafft"] + ["--amino", fpep]
+    out = sp.run(cmd, stdout=sp.PIPE, stderr=sp.PIPE)
+    with open(faln, 'w') as f: f.write(out.stdout.decode('utf-8'))
+
+def runiqree(faln,treeset):
+    if not treeset is None:
+        treesetfull = []
+        cmd = ["iqtree", "-s", faln]
+        for i in treeset:
+            i = i.strip(" ").split(" ")
+            treesetfull = treesetfull + i
+        cmd = cmd + treesetfull
+    else:
+        cmd = ["iqtree", "-s", faln]
+    sp.run(cmd, stdout=sp.PIPE)
+
+def runfastree(faln,treeset):
+    if not treeset is None:
+        treesetfull = []
+        cmd = ["FastTree", "-out", faln+".fasttree", faln]
+        for i in treeset:
+            i = i.strip(" ").split(" ")
+            treesetfull = treesetfull + i
+        cmd = cmd[:1] + treesetfull + cmd[1:]
+    else:
+        cmd = ["FastTree", "-out", faln+".fasttree", faln]
+    sp.run(cmd, stdout=sp.PIPE, stderr=sp.PIPE)
+
+def wgenetree(faln,tree_method,treeset):
+    if tree_method == 'iqtree':
+        runiqree(faln,treeset)
+        return faln+".treefile"
+    if tree_method == 'fasttree':
+        runfastree(faln,treeset)
+        return faln+".fasttree"
+
+def finalinfertree(fp,tree_method,treeset):
+    waln(fp,fp+".aln")
+    treepath = wgenetree(fp+".aln",tree_method,treeset)
+    return treepath
+
+
+def postrbhcutoff(df,nthreads,eval,outdir,pps,glength,Noldsp,Nnewsp,gsmap,fam2assign,tmpdir):
+    outfiles = Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(runselfdiamond)(fnamep,eval,nthreads,fam) for fam,fnamep in zip(df.index,pps))
+    dfs = normalizedout(outfiles,glength,gsmap)
+    df = filterbymin(dfs,df,Noldsp,Nnewsp)
+    fname = os.path.join(outdir,os.path.basename(fam2assign)+".assigned.furtherscorefiltered")
+    df.to_csv(fname,header=True,index=True,sep='\t')
+    fromgene2count(df,outdir,fam2assign,second=True)
+    if tmpdir ==None: rmtmpp(outdir)
+    return df
+
+def rmtmpp(outdir):
+    parent = os.getcwd()
+    target = os.path.join(outdir,'Orthologues_Sequence_Assigned','pep')
+    os.chdir(target)
+    with open('rm.sh','w') as f: f.write('rm *.dmnd *.tsv *.tsv_normalized')
+    sp.run(['sh','rm.sh'],stdout=sp.PIPE,stderr=sp.PIPE)
+    sp.run(['rm','rm.sh'],stdout=sp.PIPE,stderr=sp.PIPE)
+    os.chdir(parent)
+
+def filterbymin(dfs,df,Noldsp,Nnewsp):
+    fams = list(df.index)
+    for d,fam in zip(dfs,fams):
+        cutoff = getreferencecutoff(d,Noldsp)
+        logging.info("The normalized bit-score cutoff for {0} is {1:.2f}".format(fam,cutoff))
+        retainednewseqs = realfilter(d,cutoff,Noldsp,Nnewsp)
+        df = filterdf(df,retainednewseqs,fam,Nnewsp)
+    return df
+
+def filterdf(df,retainednewseqs,fam,Nnewsp):
+    for sp in Nnewsp: df.loc[fam,sp] = ''
+    for gene, sp in retainednewseqs:
+        if df.loc[fam,sp] == '':
+            df.loc[fam,sp] = gene
+        else:
+            df.loc[fam,sp] = ", ".join([df.loc[fam,sp],gene])
+    return df
+
+def realfilter(d,cutoff,Noldsp,Nnewsp):
+    retainednewseqs = []
+    for i in d.index:
+        sp1,sp2 = d.loc[i,14],d.loc[i,15]
+        if sp1 in Noldsp and sp2 in Nnewsp:
+            if d.loc[i,13] >= cutoff:
+                retainednewseqs.append((d.loc[i,1],sp2))
+        if sp1 in Nnewsp and sp2 in Noldsp:
+            if d.loc[i,13] >= cutoff:
+                retainednewseqs.append((d.loc[i,0],sp1))
+    retainednewseqs = [i for i in set(retainednewseqs)]
+    return retainednewseqs
+
+def getreferencecutoff(d,Noldsp):
+    scores_olds = []
+    for i in d.index:
+        sp1,sp2 = d.loc[i,14],d.loc[i,15]
+        if sp1 in Noldsp and sp2 in Noldsp:
+            scores_olds.append(d.loc[i,13])
+    cutoff = min(scores_olds)
+    return cutoff
+
+def normalizedout(outfiles,glength,gsmap):
+    dfs = []
+    for out in outfiles:
+        df = pd.read_csv(out,header=None,index_col=None,sep='\t',usecols=[0,1,11])
+        df = addgleng(df,glength)
+        df = fitall_linear(df)
+        df = addspn(df,gsmap)
+        fname = out + "_normalized"
+        df.to_csv(fname,header=False,index=False,sep='\t')
+        dfs.append(df)
+    return dfs
+
+def addspn(df,gsmap):
+    df[14] = df[0].apply(lambda x:gsmap[x])
+    df[15] = df[1].apply(lambda x:gsmap[x])
+    return df
 
-def fromgene2count(df,outdir,fam2assign):
+def fitall_linear(df):
+    slope, intercept, r, p, se = stats.linregress(np.log10(df[12]), np.log10(df[11]))
+    df[13] = [j/(pow(10, intercept)*(l**slope)) for j,l in zip(df[11],df[12])]
+    return df
+
+def addgleng(df,glength):
+    df[12] = df[0].apply(lambda x:glength[x])
+    df[13] = df[1].apply(lambda x:glength[x])
+    df[14] = [g1*g2 for g1,g2 in zip(df[12],df[13])]
+    df = df.drop(columns=[12, 13]).rename(columns={14: 12})
+    return df
+
+def runselfdiamond(fnamep,eval,nthreads,fam):
+    if not os.path.isfile(fnamep[:-4] + '.dmnd'):
+        cmd = ["diamond", "makedb", "--in", fnamep, "-d", fnamep[:-4], "-p", str(nthreads)]
+        out = sp.run(cmd, stdout=sp.PIPE, stderr=sp.PIPE)
+        logging.debug(out.stderr.decode())
+        if out.returncode == 1: logging.error(out.stderr.decode())
+    outfile = "_".join([fnamep[:-4],fam+".tsv"])
+    cmd = ["diamond", "blastp", "-d", fnamep[:-4] + '.dmnd', "-q", fnamep, "-e", str(eval), "-o", outfile, "-p", str(nthreads)]
+    out = sp.run(cmd, stdout=sp.PIPE, stderr=sp.PIPE)
+    logging.debug(out.stderr.decode())
+    return outfile
+
+
+def fromgene2count(df,outdir,fam2assign,second = False,third=False):
     fname = os.path.join(outdir,os.path.basename(fam2assign)+'.assigned.genecount')
+    if second: fname = os.path.join(outdir,os.path.basename(fam2assign)+'.assigned.furtherscorefiltered.genecount')
+    if third: fname = os.path.join(outdir,os.path.basename(fam2assign)+'.assigned.furtherscorefiltered.tree-based.genecount')
     Index = df.index
     columns = {c:[] for c in df.columns}
     for indice in df.index:
         for c in df.columns:
             if type(df.loc[indice,c]) != str:
                 columns[c].append(0)
+            elif df.loc[indice,c] == '':
+                columns[c].append(0)
             else:
                 columns[c].append(len(df.loc[indice,c].split(", ")))
     df_out = pd.DataFrame.from_dict(columns)
     df_out.index = Index
     df_out.to_csv(fname,header=True,index=True,sep='\t')
 
 def rmtmp(tmpdir,outdir,querys):
@@ -1673,20 +1894,25 @@
         sp.run(['sh','rm.sh'],stdout=sp.PIPE,stderr=sp.PIPE)
         sp.run(['rm','rm.sh'],stdout=sp.PIPE,stderr=sp.PIPE)
         os.chdir(cwd)
         
 def dmd4g2f(outdir,s,nthreads,querys,df):
     return None
 
-def genes2fams(assign_method,seq2assign,fam2assign,outdir,s,nthreads,tmpdir,to_stop,cds,cscore,eval,start,normalizedpercent):
+def genes2fams(assign_method,seq2assign,fam2assign,outdir,s,nthreads,tmpdir,to_stop,cds,cscore,eval,start,normalizedpercent,tree_method,treeset):
+    Noldsp = [i.prefix for i in s]
+    gsmap = {}
+    for seq in s: gsmap.update({gid:seq.prefix for gid in seq.idmap.keys()})
     logging.info("Assigning sequences into given gene families")
     seqs_query = [SequenceData(s, out_path=outdir, tmp_path=tmpdir, to_stop=to_stop, cds=cds, cscore=cscore, threads=nthreads, normalizedpercent=normalizedpercent) for s in seq2assign]
+    for seq in seqs_query: gsmap.update({gid:seq.prefix for gid in seq.idmap.keys()})
+    Nnewsp = [i.prefix for i in seqs_query]
     df = pd.read_csv(fam2assign,header=0,index_col=0,sep='\t')
     for i in range(1, len(s)): s[0].merge_seq(s[i])
-    if assign_method == 'hmmer': hmmer4g2f(outdir,s[0],nthreads,seqs_query,df,eval,fam2assign)
+    if assign_method == 'hmmer': hmmer4g2f(outdir,s[0],nthreads,seqs_query,df,eval,fam2assign,Noldsp,Nnewsp,gsmap,tmpdir,tree_method,treeset)
     else: dmd4g2f(outdir,s[0],nthreads,seqs_query,df)
     rmtmp(tmpdir,outdir,seqs_query)
     endt(tmpdir,start,s)
 
 def run_or(i,j,s,eval,orthoinfer):
     s[i].run_diamond(s[j], orthoinfer, eval=eval, savememory=True)
```

### Comparing `wgd-2.0.19/wgd/mcmctree.py` & `wgd-2.0.20/wgd/mcmctree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.19/wgd/mix.py` & `wgd-2.0.20/wgd/mix.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.19/wgd/peak.py` & `wgd-2.0.20/wgd/peak.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import itertools
 import os
 from wgd.core import _mkdir
 from sklearn_extra.cluster import KMedoids
 from wgd.viz import reflect_logks,find_peak_init_parameters
 from io import StringIO
 from sklearn import metrics
+from wgd.utils import formatv2
 warnings.filterwarnings("ignore", category=np.VisibleDeprecationWarning)
 
 def alnfilter(df,weights_outliers_included, identity, aln_len, coverage, min_ks, max_ks):
     """
     Filter alignment stats and Ks
     """
     df = df.dropna(subset=['dS'])
@@ -60,15 +61,15 @@
         weight = m.weights_[j]
         precision = m.precisions_[j][0][0]
         means.append(mean)
         covariances.append(covariance)
         stds.append(std)
         weights.append(weight)
         precisions.append(precision)
-        logging.info("Component {0} has mean {1:.3f} ,std {2:.3f} ,weight {3:.3f}, precision {4:.3f}".format(j+1,mean,std,weight,precision))
+        logging.info("Component {0} has mean {1:.3f}, std {2:.3f}, weight {3:.3f}, precision {4:.3f}".format(j+1,mean,std,weight,precision))
     info_table['{}component'.format(i)] = {'mean':means,'covariance':covariances,'weight':weights,'precision':precisions,'stds':stds}
 
 def aic_info(aic,n1):
     besta_loc = np.argmin(aic)
     #logging.info("Relative probabilities compared to the AIC-best model (with {} components):".format(besta_loc + 1))
     #for i, aic_i in enumerate(aic):
     #    if i != besta_loc:
@@ -162,47 +163,91 @@
     return mode, max(kde_y)
 
 def get_totalH(Hs):
     CHF = 0
     for i in Hs: CHF = CHF + i
     return CHF
 
-def plot_mp_component_lognormal(X,hdr,means,stds,weights,labels,n,bins=50,ylabel="Counts",regime='multiplicon'):
+def plot_mpbackap_lognormal(df,kdexs,kdeys,modes,guide):
+    colors = cm.viridis(np.linspace(0, 1, len(modes)))
+    fig, ax = plt.subplots()
+    x = np.array(list(df['dS']))
+    y = x[np.isfinite(x)]
+    Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, color = 'g', alpha=1, rwidth=0.8)
+    Hs_max = max(Hs)
+    y_lim_beforekde = ax.get_ylim()[1]
+    CHF = get_totalH(Hs)
+    scaling = CHF*0.1
+    for kde_x,kde_y,mode,color,i in zip(kdexs,kdeys,modes,colors,range(len(modes))):
+        ax.plot(kde_x,scaling*kde_y, alpha=0)
+        y_lim_afterkde = ax.get_ylim()[1]
+        #print(y_lim_afterkde)
+        scalingtmp=y_lim_beforekde/y_lim_afterkde*scaling
+        #print((scalingtmp,mode))
+        ax.plot(kde_x,scalingtmp*kde_y, c=color, ls='-', lw=1.5, alpha=0.8, label='{} component {} mode {:.2f}'.format(guide,i,mode))
+    ax.set_ylim(0, max([Hs_max,y_lim_beforekde]))
+    ax.legend(loc='upper right', frameon=False)
+    ax.set_xlabel("$K_\mathrm{S}$")
+    ax.set_ylabel("Duplication events")
+    ax.set_xticks([0,1,2,3,4,5])
+    sns.despine(offset=1)
+    plt.title('Anchor '+'$K_\mathrm{S}$'+'components')
+    fig.tight_layout()
+    return fig
+
+def plot_mp_component_lognormal(X,hdr,means,stds,weights,labels,n,bins=50,ylabel="Counts",regime='multiplicon',user_xlim=None,user_ylim=None):
     #labels = labels[(X<5) & (X>0)]
     #X = X[(X<5) & (X>0)]
     colors = cm.viridis(np.linspace(0, 1, n))
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     fig, ax = plt.subplots()
     df = pd.DataFrame.from_dict({'label':labels,'dS':X})
+    Hs_maxs,y_lim_beforekde_s = [],[]
+    kdexs,kdeys,modes=[],[],[]
     for i,color in enumerate(colors):
         # here I recover the std by sqrt
         mean,std,weight = means[i][0],np.sqrt(stds[i][0][0]),weights[i]
         df_comp = df[df['label']==i]
         x = np.array(list(df_comp['dS']))
         y = x[np.isfinite(x)]
         Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, alpha=0.5, rwidth=0.8, label = "component {}".format(i))
+        Hs_max = max(Hs)
+        Hs_maxs.append(Hs_max)
+        y_lim_beforekde = ax.get_ylim()[1]
+        y_lim_beforekde_s.append(y_lim_beforekde)
         CHF = get_totalH(Hs)
         scaling = CHF*0.1
         #upper_HPD,lower_HPD = calculateHPD(y,hdr)
         #plt.axvline(x = upper_HPD, color = color, alpha = 0.8, ls = '-.', lw = 1,label="{}% HDR CI Upper {:.2f}".format(hdr,upper_HPD))
         #plt.axvline(x = lower_HPD, color = color, alpha = 0.8, ls = '-.', lw = 1,label="{}% HDR CI Lower {:.2f}".format(hdr,lower_HPD))
-        ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(i,np.exp(mean - std**2)))
+        kde_y = np.array([stats.lognorm.pdf(j, scale=np.exp(mean),s=std) for j in kde_x])
+        #ax.plot(kde_x,scaling*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(i,np.exp(mean - std**2)))
+        ax.plot(kde_x,scaling*kde_y, c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(i,np.exp(mean - std**2)))
+        kdexs.append(kde_x)
+        kdeys.append(kde_y)
+        modes.append(np.exp(mean - std**2))
+        y_lim_afterkde = ax.get_ylim()[1]
+        if y_lim_afterkde > y_lim_beforekde: ax.set_ylim(0, y_lim_beforekde)
+    safe_max = max([max(y_lim_beforekde_s),max(Hs_maxs)])
+    ax.set_ylim(0, safe_max)
     ax.legend(loc='upper right', fontsize='small',frameon=False)
     ax.set_xlabel("$K_\mathrm{S}$")
     ax.set_ylabel(ylabel)
     ax.set_xticks([0,1,2,3,4,5])
+    if not (user_ylim[0]) is None: ax.set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: ax.set_xlim(user_xlim[0],user_xlim[1])
     sns.despine(offset=1)
     if regime== 'multiplicon': plt.title('Multiplicon $K_\mathrm{S}$ GMM modeling')
     elif regime== 'segment': plt.title('Segment $K_\mathrm{S}$ GMM modeling')
     else: plt.title('Basecluster $K_\mathrm{S}$ GMM modeling')
     fig.tight_layout()
-    return fig
+    return fig, kdexs, kdeys, modes
 
-def plot_mp_component(X,labels,n,bins=50,plot = 'identical',ylabel="Counts",regime='multiplicon'):
+def plot_mp_component(X,labels,n,bins=50,plot = 'identical',ylabel="Counts",regime='multiplicon',user_xlim=None,user_ylim=None):
     labels = labels[(X<5) & (X>0)]
     X = X[(X<5) & (X>0)]
     colors = cm.viridis(np.linspace(0, 1, n))
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     fig, ax = plt.subplots()
     df = pd.DataFrame.from_dict({'label':labels,'dS':X})
@@ -217,22 +262,24 @@
         xs = [np.array(list(i['dS'])) for i in dist_comps]
         ys = [x[np.isfinite(x)] for x in xs]
         ax.hist(ys, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color=colors, stacked=True, alpha=0.5, rwidth=0.8, label = ["component {}".format(int(i)) for i in range(n)])
     ax.legend(loc='upper right', fontsize='small',frameon=False)
     ax.set_xlabel("$K_\mathrm{S}$")
     ax.set_ylabel(ylabel)
     ax.set_xticks([0,1,2,3,4,5])
+    if not (user_ylim[0]) is None: ax.set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: ax.set_xlim(user_xlim[0],user_xlim[1])
     sns.despine(offset=1)
     if regime== 'multiplicon': plt.title('Multiplicon $K_\mathrm{S}$ GMM modeling')
     elif regime== 'segment': plt.title('Segment $K_\mathrm{S}$ GMM modeling')
     else: plt.title('Basecluster $K_\mathrm{S}$ GMM modeling')
     fig.tight_layout()
     return fig
 
-def plot_ak_component(df,nums,bins=50,plot = 'identical',ylabel="Duplication events",weighted=True,regime='multiplicon'):
+def plot_ak_component(df,nums,bins=50,plot = 'identical',ylabel="Duplication events",weighted=True,regime='multiplicon',user_xlim=None,user_ylim=None):
     colors = cm.viridis(np.linspace(0, 1, nums))
     fig, ax = plt.subplots()
     if plot == 'identical':
         if weighted:
             for num,color in zip(range(nums),colors):
                 if nums == 1: df_comp = df
                 #if nums == 1: df_comp = df.drop_duplicates(subset=['family','node'])
@@ -264,27 +311,100 @@
             xs = [np.array(list(i['node_averaged_dS_outlierexcluded'])) for i in dist_comps]
             ys = [x[np.isfinite(x)] for x in xs]
             ax.hist(ys, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color=colors, stacked=True, alpha=0.5, rwidth=0.8, label = ["component {}".format(int(i)) for i in range(nums)])
     ax.legend(loc='upper right', fontsize='small',frameon=False)
     ax.set_xlabel("$K_\mathrm{S}$")
     ax.set_ylabel(ylabel)
     ax.set_xticks([0,1,2,3,4,5])
+    if not (user_ylim[0]) is None: ax.set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: ax.set_xlim(user_xlim[0],user_xlim[1])
     sns.despine(offset=1)
     if regime== 'multiplicon': plt.title('Multilplicon-guided Anchor $K_\mathrm{S}$ GMM modeling')
     elif regime== 'segment': plt.title('Segment-guided Syntelog $K_\mathrm{S}$ GMM modeling')
     elif regime== 'original': plt.title('Original Anchor $K_\mathrm{S}$ GMM modeling')
     else: plt.title('Basecluster-guided Anchor $K_\mathrm{S}$ GMM modeling')
     fig.tight_layout()
     return fig
 
-def plot_ak_component_lognormal(df,means,stds,weights,nums,bins=50,ylabel="Duplication events",weighted=True,regime='multiplicon'):
+def getcompheuri(df,peak_threshold,rel_height,na=False,ci=95):
+    gs_ks = df.loc[:,['gene1','gene2','dS']]
+    if na:
+        df = df.drop_duplicates(subset=['family','node'])
+        df = df.loc[:,['node_averaged_dS_outlierexcluded']].copy().rename(columns={'node_averaged_dS_outlierexcluded':'dS'})
+        df['weightoutlierexcluded'] = 1
+    df = df.dropna(subset=['dS','weightoutlierexcluded'])
+    df = df.loc[(df['dS']>0) & (df['dS']<5),:]
+    ks_or = np.array(df['dS'])
+    w = np.array(df['weightoutlierexcluded'])
+    ks = np.log(ks_or)
+    max_ks,min_ks = ks.max(),ks.min()
+    ks_refed,cutoff,w_refed = reflect_logks(ks,w)
+    kde_x = np.linspace(min_ks-cutoff, max_ks+cutoff,num=500)
+    kde = stats.gaussian_kde(ks_refed,weights=w_refed,bw_method="scott")
+    kde_y = kde(kde_x)
+    spl = interpolate.UnivariateSpline(kde_x, kde_y)
+    spl.set_smoothing_factor(0.01)
+    spl_x = np.linspace(min_ks, max_ks+0.1, num=int(round((abs(min_ks) + (max_ks+0.1)) *100)))
+    spl_y = spl(spl_x)
+    #if na: logging.info('Detecting likely peaks from node-averaged data')
+    #else: logging.info('Detecting likely peaks from node-weighted data')
+    init_means, init_stdevs, good_prominences = onlyfind_peak_init_parameters(spl_x,spl_y,peak_threshold=peak_threshold,rel_height=rel_height)
+    x_points_strictly_positive = np.linspace(0, 5, int(5 * 100))
+    if len(init_means) == 0:
+        return None
+    else:
+        mean,std = init_means[0],init_stdevs[0]
+        lowc, upperc = (1-ci/100)/2, 1-(1-ci/100)/2
+        CI_95 = stats.lognorm.ppf([lowc, upperc], scale=np.exp(mean), s=std)
+        return CI_95
+
+def onlyfind_peak_init_parameters(spl_x,spl_y,peak_threshold=0.1,rel_height=0.4):
+    peaks, properties = signal.find_peaks(spl_y)
+    prominences = signal.peak_prominences(spl_y, peaks)[0]
+    prominences_refed_R1,width_refed_R1,prominences_refed_L1,width_refed_L1 = [],[],[],[]
+    for i in range(len(peaks)):
+        peak_index = peaks[i]
+        spl_peak_refl_y = np.concatenate((np.flip(spl_y[peak_index+1:]), spl_y[peak_index:]))
+        spl_peak_refl_x = np.concatenate((np.flip(spl_x[peak_index+1:] * -1 + 2 * spl_x[peak_index]), spl_x[peak_index:]))
+        current_peak_index = int((len(spl_peak_refl_x)-1)/2)
+        new_prominences = signal.peak_prominences(spl_peak_refl_y,[current_peak_index])[0][0]
+        new_width,new_height,left_ips,right_ips = signal.peak_widths(spl_peak_refl_y, [current_peak_index], rel_height=rel_height)
+        if new_width[0] > 150: new_width[0] = 150
+        prominences_refed_R1.append(new_prominences)
+        width_refed_R1.append(new_width[0])
+        c = "r" if new_prominences >= peak_threshold else 'gray'
+        w = new_width[0]/2/100
+        spl_peak_refl_y_L = np.concatenate((spl_y[:peak_index+1], np.flip(spl_y[:peak_index])))
+        spl_peak_refl_x_L = np.concatenate((spl_x[:peak_index+1], np.flip(spl_x[:peak_index]) * -1 + 2*spl_x[peak_index]))
+        current_peak_index = int((len(spl_peak_refl_x_L)-1)/2)
+        new_prominences = signal.peak_prominences(spl_peak_refl_y_L,[current_peak_index])[0][0]
+        new_width,new_height,left_ips,right_ips = signal.peak_widths(spl_peak_refl_y_L, [current_peak_index], rel_height=rel_height)
+        if new_width[0] > 150: new_width[0] = 150
+        prominences_refed_L1.append(new_prominences)
+        width_refed_L1.append(new_width[0])
+        c = "r" if new_prominences >= peak_threshold else 'gray'
+        w = new_width[0]/2/100
+    good_peaks_R1,good_peaks_L1 = [i>=peak_threshold for i in prominences_refed_R1],[i>=peak_threshold for i in prominences_refed_L1]
+    good_prominences,init_means,init_stdevs = [],[],[]
+    for i in range(len(peaks)):
+        if good_peaks_R1[i] or good_peaks_L1[i]:
+            init_means.append(spl_x[peaks[i]])
+            best = np.argmax((prominences_refed_R1[i], prominences_refed_L1[i]))
+            good_prominences.append(max([prominences_refed_R1[i], prominences_refed_L1[i]]))
+            width = [width_refed_R1[i], width_refed_L1[i]][best]
+            init_stdevs.append(width/2/100)
+    return init_means, init_stdevs,good_prominences
+
+def plot_ak_component_lognormal(df,means,stds,weights,nums,bins=50,ylabel="Duplication events",weighted=True,regime='multiplicon',showCI=False,heuristic=False, peak_threshold=0.1, rel_height=0.4, user_xlim=None,user_ylim=None):
     colors = cm.viridis(np.linspace(0, 1, nums))
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     fig, ax = plt.subplots()
+    CI_dict, CI_dict_heri = {},{}
+    Hs_maxs,y_lim_beforekde_s=[],[]
     if weighted:
         for num,color in zip(range(nums),colors):
             # here I recover the std by sqrt
             mean,std,weight = means[num][0],np.sqrt(stds[num][0][0]),weights[num]
             if nums == 1: df_comp = df.copy()
             else: df_comp = df[df['AnchorKs_GMM_Component']==num]
             w = df_comp['weightoutlierexcluded']
@@ -293,43 +413,105 @@
             w = w[np.isfinite(x)]
             if len(y) < 2:
                 logging.info("Detected one component with less than 2 elements, will skip it")
                 continue
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, weights=w, alpha=0.5, rwidth=0.8, label = "component {}".format(num))
             CHF = get_totalH(Hs)
             scaling = CHF*0.1
-            ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(num,np.exp(mean - std**2)))
+            Hs_max = max(Hs)
+            Hs_maxs.append(Hs_max)
+            y_lim_beforekde = ax.get_ylim()[1]
+            y_lim_beforekde_s.append(y_lim_beforekde)
+            ax.plot(kde_x,scaling*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(num,np.exp(mean - std**2)))
+            y_lim_afterkde = ax.get_ylim()[1]
+            if y_lim_afterkde > y_lim_beforekde: ax.set_ylim(0, y_lim_beforekde)
+            safe_max = max([max(y_lim_beforekde_s),max(Hs_maxs)])
+            ax.set_ylim(0, safe_max)
+            if showCI and heuristic:
+                CI_95 = getcompheuri(df_comp,peak_threshold,rel_height,na=False,ci=95)
+                CI_dict_heri[num]=CI_95
+                if not (CI_95 is None):
+                    CI_95_y0 = scaling*stats.lognorm.pdf(CI_95[0], scale=np.exp(mean),s=std)
+                    CI_95_y1 = scaling*stats.lognorm.pdf(CI_95[1], scale=np.exp(mean),s=std)
+                    plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='Peak {} lower {}%CI {:.2f}'.format(num,95,CI_95[0]))
+                    plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1,label='Peak {} upper {}%CI {:.2f}'.format(num,95,CI_95[1]))
+            if showCI:
+                CI_95 = stats.lognorm.ppf([0.025, 0.975], scale=np.exp(mean), s=std)
+                #CI_95 = stats.lognorm(std,loc=0,scale=np.exp(mean)).interval(0.95)
+                CI_dict[num]=CI_95
+                CI_95_y0 = scaling*stats.lognorm.pdf(CI_95[0], scale=np.exp(mean),s=std)
+                CI_95_y1 = scaling*stats.lognorm.pdf(CI_95[1], scale=np.exp(mean),s=std)
+                plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} lower {}%CI {:.2f}'.format(num,95,CI_95[0]))
+                plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} upper {}%CI {:.2f}'.format(num,95,CI_95[1]))
     else:
         for num,color in zip(range(nums),colors):
             mean,std,weight = means[num][0],np.sqrt(stds[num][0][0]),weights[num]
             if nums == 1: df_comp = df.drop_duplicates(subset=['family','node'])
             else: df_comp = df[df['AnchorKs_GMM_Component']==num].drop_duplicates(subset=['family','node'])
             x = np.array(list(df_comp['node_averaged_dS_outlierexcluded']))
             y = x[np.isfinite(x)]
             if len(y) < 2:
                 logging.info("Detected one component with less than 2 elements, will skip it")
                 continue
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, alpha=0.5, rwidth=0.8, label = "component {}".format(num))
             CHF = get_totalH(Hs)
             scaling = CHF*0.1
-            ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(num,np.exp(mean - std**2)))
+            Hs_max = max(Hs)
+            Hs_maxs.append(Hs_max)
+            y_lim_beforekde = ax.get_ylim()[1]
+            y_lim_beforekde_s.append(y_lim_beforekde)
+            ax.plot(kde_x,scaling*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(num,np.exp(mean - std**2)))
+            y_lim_afterkde = ax.get_ylim()[1]
+            if y_lim_afterkde > y_lim_beforekde: ax.set_ylim(0, y_lim_beforekde)
+            safe_max = max([max(y_lim_beforekde_s),max(Hs_maxs)])
+            ax.set_ylim(0, safe_max)
+            if showCI and heuristic:
+                CI_95 = getcompheuri(df_comp,peak_threshold,rel_height,na=True,ci=95)
+                CI_dict_heri[num]=CI_95
+                if not (CI_95 is None):
+                    CI_95_y0 = scaling*stats.lognorm.pdf(CI_95[0], scale=np.exp(mean),s=std)
+                    CI_95_y1 = scaling*stats.lognorm.pdf(CI_95[1], scale=np.exp(mean),s=std)
+                    plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='Peak {} lower {}%CI {:.2f}'.format(num,95,CI_95[0]))
+                    plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1,label='Peak {} upper {}%CI {:.2f}'.format(num,95,CI_95[1]))
+            if showCI:
+                CI_95 = stats.lognorm.ppf([0.025, 0.975], scale=np.exp(mean), s=std)
+                CI_dict[num]=CI_95
+                CI_95_y0 = scaling*stats.lognorm.pdf(CI_95[0], scale=np.exp(mean),s=std)
+                CI_95_y1 = scaling*stats.lognorm.pdf(CI_95[1], scale=np.exp(mean),s=std)
+                plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} lower {}%CI {:.2f}'.format(num,95,CI_95[0]))
+                plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} upper {}%CI {:.2f}'.format(num,95,CI_95[1]))
     #ax.legend(loc='upper right', fontsize='small',frameon=False)
-    ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
+    ax.legend(loc='upper right',frameon=False)
+    #ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
     ax.set_xlabel("$K_\mathrm{S}$")
     ax.set_ylabel(ylabel)
     ax.set_xticks([0,1,2,3,4,5])
+    if not (user_ylim[0]) is None: ax.set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: ax.set_xlim(user_xlim[0],user_xlim[1])
     sns.despine(offset=1)
     if regime=='multiplicon': plt.title('Multilplicon-guided Anchor $K_\mathrm{S}$ GMM modeling')
     elif regime=='segment': plt.title('Segment-guided Syntelog $K_\mathrm{S}$ GMM modeling')
     elif regime== 'original': plt.title('Original Anchor $K_\mathrm{S}$ GMM modeling')
     else: plt.title('Basecluster-guided Anchor $K_\mathrm{S}$ GMM modeling')
     fig.tight_layout()
-    return fig
+    return fig, {'showci':CI_dict,'heuristic':CI_dict_heri}
 
-def plot_ak_component_kde(df,nums,hdr,bins=50,ylabel="Duplication events",weighted=True,regime='multiplicon'):
+def getmediankdexy(kdex,kdey):
+    weights = [kdex[i]*kdey[i] for i in range(len(kdex))]
+    half_weight = sum(weights)/2
+    cum_weight = 0
+    medianx = 0
+    for i,weight in enumerate(weights):
+        cum_weight = cum_weight + weight
+        if cum_weight >= half_weight:
+            medianx = kdex[i]
+            break
+    return medianx
+
+def plot_ak_component_kde(df,nums,hdr,bins=50,ylabel="Duplication events",weighted=True,regime='multiplicon',user_xlim=None,user_ylim=None):
     colors = cm.viridis(np.linspace(0, 1, nums))
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     fig, ax = plt.subplots()
     Hs_maxs,y_lim_beforekde_s,HDRs = [],[],{}
     if weighted:
         for num,color in zip(range(nums),colors):
@@ -339,77 +521,94 @@
             w = df_comp['weightoutlierexcluded']
             x = np.array(list(df_comp['dS']))
             y = x[np.isfinite(x)]
             w = w[np.isfinite(x)]
             if len(y) < 2:
                 logging.info("Detected one component with less than 2 elements, will skip it")
                 continue
-            kde = stats.gaussian_kde(y,weights=w,bw_method=0.1)
+            kde = stats.gaussian_kde(y,weights=w,bw_method='scott')
             kde_y = kde(kde_x)
             mode, maxim = kde_mode(kde_x, kde_y)
+            #median = getmediankdexy(kde_x,kde_y)
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, weights=w, alpha=0.5, rwidth=0.8, label = "component {} (mode {:.2f})".format(num,mode))
+            #Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, weights=w, alpha=0.5, rwidth=0.8, label = "component {} (mode {:.2f} median {:.2f})".format(num,mode,median))
             Hs_max = max(Hs)
             Hs_maxs.append(Hs_max)
             y_lim_beforekde = ax.get_ylim()[1]
             y_lim_beforekde_s.append(y_lim_beforekde)
             CHF = get_totalH(Hs)
             scaling = CHF*0.1
             ax.plot(kde_x, kde_y*scaling, color=color,alpha=0.4, ls = '--',lw = 1)
             y_lim_afterkde = ax.get_ylim()[1]
             if y_lim_afterkde > y_lim_beforekde: ax.set_ylim(0, y_lim_beforekde)
             safe_max = max([max(y_lim_beforekde_s),max(Hs_maxs)])
             ax.set_ylim(0, safe_max)
-            ax.axvline(x = mode, color = color, alpha = 0.8, ls = ':', lw = 1)
+            #ax.axvline(x = mode, ymin=0,ymax=scaling*maxim/Hs_max, color = color, alpha = 0.8, ls = ':', lw = 1)
+            plt.plot([mode,mode], [0,scaling*maxim], color=color,alpha = 0.8,linestyle='-.')
+            #plt.plot([median,median], [0,scaling*kde(median)], color=color,alpha = 0.8,linestyle='-.')
             upper_HPD,lower_HPD = calculateHPD(y,hdr)
-            ax.axvline(x = upper_HPD, color = color, alpha = 0.8, ls = '-.', lw = 1,label='HDR {:.2f}-{:.2f}'.format(lower_HPD,upper_HPD))
-            ax.axvline(x = lower_HPD, color = color, alpha = 0.8, ls = '-.', lw = 1)
+            plt.plot([upper_HPD,upper_HPD], [0,scaling*kde(upper_HPD)], color=color,alpha = 0.8,linestyle=':')
+            plt.plot([lower_HPD,lower_HPD], [0,scaling*kde(lower_HPD)], color=color,alpha = 0.8,linestyle=':')
+            #ax.axvline(x = upper_HPD, ymin=0, ymax=upper_HPD_y, color = color, alpha = 0.8, ls = '-.', lw = 1,label='HDR {:.2f}-{:.2f}'.format(lower_HPD,upper_HPD))
+            #ax.axvline(x = lower_HPD, ymin=0, ymax=lower_HPD_y, color = color, alpha = 0.8, ls = '-.', lw = 1)
             HDRs[num] = (lower_HPD,upper_HPD)
     else:
         for num,color in zip(range(nums),colors):
             if nums == 1: df_comp = df.drop_duplicates(subset=['family','node'])
             else: df_comp = df[df['AnchorKs_GMM_Component']==num].drop_duplicates(subset=['family','node'])
             x = np.array(list(df_comp['node_averaged_dS_outlierexcluded']))
             y = x[np.isfinite(x)]
             if len(y) < 2:
                 logging.info("Detected one component with less than 2 elements, will skip it")
                 continue
-            kde = stats.gaussian_kde(y,bw_method=0.1)
+            kde = stats.gaussian_kde(y,bw_method='scott')
             kde_y = kde(kde_x)
             mode, maxim = kde_mode(kde_x, kde_y)
+            #median = getmediankdexy(kde_x,kde_y)
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, alpha=0.5, rwidth=0.8, label = "component {} (mode {:.2f})".format(num,mode))
+            #Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, alpha=0.5, rwidth=0.8, label = "component {} (mode {:.2f} median {:.2f})".format(num,mode,median))
             Hs_max = max(Hs)
             Hs_maxs.append(Hs_max)
             y_lim_beforekde = ax.get_ylim()[1]
             y_lim_beforekde_s.append(y_lim_beforekde)
             CHF = get_totalH(Hs)
             scaling = CHF*0.1
             ax.plot(kde_x, kde_y*scaling, color=color,alpha=0.4, ls = '--',lw = 1)
             y_lim_afterkde = ax.get_ylim()[1]
             if y_lim_afterkde > y_lim_beforekde: ax.set_ylim(0, y_lim_beforekde)
             safe_max = max([max(y_lim_beforekde_s),max(Hs_maxs)])
             ax.set_ylim(0, safe_max)
-            ax.axvline(x = mode, color = color, alpha = 0.8, ls = ':', lw = 1)
+            plt.plot([mode,mode], [0,scaling*maxim], color=color,alpha = 0.8,linestyle='-.')
+            #plt.plot([median,median], [0,scaling*kde(median)], color=color,alpha = 0.8,linestyle='-.')
+            #ax.axvline(x = mode, ymin=0, ymax=scaling*maxim/Hs_max, color = color, alpha = 0.8, ls = ':', lw = 1)
             upper_HPD,lower_HPD = calculateHPD(y,hdr)
-            ax.axvline(x = upper_HPD, color = color, alpha = 0.8, ls = '-.', lw = 1,label='HDR {:.2f}-{:.2f}'.format(lower_HPD,upper_HPD))
-            ax.axvline(x = lower_HPD, color = color, alpha = 0.8, ls = '-.', lw = 1)
+            #upper_HPD_y = scaling*kde(upper_HPD)/Hs_max
+            #lower_HPD_y = scaling*kde(lower_HPD)/Hs_max
+            plt.plot([upper_HPD,upper_HPD], [0,scaling*kde(upper_HPD)], color=color,alpha = 0.8,linestyle=':')
+            plt.plot([lower_HPD,lower_HPD], [0,scaling*kde(lower_HPD)], color=color,alpha = 0.8,linestyle=':')
+            #ax.axvline(x = upper_HPD, ymin=0, ymax=upper_HPD_y, color = color, alpha = 0.8, ls = '-.', lw = 1,label='HDR {:.2f}-{:.2f}'.format(lower_HPD,upper_HPD))
+            #ax.axvline(x = lower_HPD, ymin=0, ymax=lower_HPD_y, color = color, alpha = 0.8, ls = '-.', lw = 1)
             HDRs[num] = (lower_HPD,upper_HPD)
     #ax.legend(loc='upper right', fontsize='small',frameon=False)
-    ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
+    ax.legend(loc='upper right', frameon=False)
+    #ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
     ax.set_xlabel("$K_\mathrm{S}$")
     ax.set_ylabel(ylabel)
     ax.set_xticks([0,1,2,3,4,5])
+    if not (user_ylim[0]) is None: ax.set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: ax.set_xlim(user_xlim[0],user_xlim[1])
     sns.despine(offset=1)
     if regime=='multiplicon': plt.title('Multilplicon-guided Anchor $K_\mathrm{S}$ GMM modeling')
     elif regime=='segment': plt.title('Segment-guided Syntelog $K_\mathrm{S}$ GMM modeling')
     elif regime== 'original': plt.title('Original Anchor $K_\mathrm{S}$ GMM modeling')
     else: plt.title('Basecluster-guided Anchor $K_\mathrm{S}$ GMM modeling')
     fig.tight_layout()
     return fig,HDRs
 
-def default_plot_kde(*args,bins=50,alphas=None,colors=None,weighted=True,title="",ylabel="Duplication events",nums = "", plot = 'identical',**kwargs):
+def default_plot_kde(*args,bins=50,alphas=None,colors=None,weighted=True,title="",ylabel="Duplication events",nums = "", plot = 'identical',user_xlim=None,user_ylim=None,**kwargs):
     ndists = len(args)
     alphas = alphas or list(np.linspace(0.2, 1, ndists))
     colors = colors or ['black'] * ndists
     # assemble panels
     keys = ["dS", "dS", "dN", "dN/dS"]
     np.seterr(divide='ignore')
     funs = [lambda x: x, np.log10, np.log10, np.log10]
@@ -506,22 +705,24 @@
     #print(safe_max)
     #print(yticklabels)
     axs[0,0].set_ylabel(ylabel)
     axs[0,0].set_yticks(axs[0,0].get_yticks())
     axs[0,0].set_ylim(0, safe_max)
     axs[1,0].set_ylabel(ylabel)
     axs[0,0].set_xticks([0,1,2,3,4,5])
+    if not (user_ylim[0]) is None: axs[0,0].set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: axs[0,0].set_xlim(user_xlim[0],user_xlim[1])
     # finalize plot
     sns.despine(offset=1)
     fig.suptitle(title, x=0.125, y=0.9, ha="left", va="top")
     fig.tight_layout()
     plt.subplots_adjust(top=0.85)  # prevent suptitle from overlapping
     return fig,safe_max,yticks
 
-def default_plot(*args,bins=50,alphas=None,colors=None,weighted=True,title="",ylabel="Duplication events",nums = "", plot = 'identical', ylim=1500,yticks='',**kwargs):
+def default_plot(*args,bins=50,alphas=None,colors=None,weighted=True,title="",ylabel="Duplication events",nums = "", plot = 'identical', ylim=1500,yticks='',user_xlim=None,user_ylim=None,**kwargs):
     ndists = len(args)
     alphas = alphas or list(np.linspace(0.2, 1, ndists))
     colors = colors or ['black'] * ndists
     # assemble panels
     keys = ["dS", "dS", "dN", "dN/dS"]
     np.seterr(divide='ignore')
     funs = [lambda x: x, np.log10, np.log10, np.log10]
@@ -586,14 +787,16 @@
             xlabel = _labels[k]
             if f == np.log10:
                 xlabel = "$\log_{10}" + xlabel[1:-1] + "$"
             ax.set_xlabel(xlabel)
     axs[0,0].set_ylabel(ylabel)
     axs[1,0].set_ylabel(ylabel)
     axs[0,0].set_xticks([0,1,2,3,4,5])
+    if not (user_ylim[0]) is None: axs[0,0].set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: axs[0,0].set_xlim(user_xlim[0],user_xlim[1])
     # finalize plot
     sns.despine(offset=1)
     fig.suptitle(title, x=0.125, y=0.9, ha="left", va="top")
     fig.tight_layout()
     plt.subplots_adjust(top=0.85)  # prevent suptitle from overlapping
     return fig
 
@@ -788,15 +991,15 @@
     if kdemethod == 'treekde': kde_y = TreeKDE(bw=bw_method).fit(modes).evaluate(kde_x)
     if kdemethod == 'fftkde': kde_y = FFTKDE(bw=bw_method).fit(modes).evaluate(kde_x)
     mode_of_modes, maxim_of_modes = kde_mode(kde_x, kde_y)
     plt.axvline(x = mode_of_modes, color = 'red', alpha = 0.8, ls = '-.', lw = 1)
     logging.info("The kde-mode of original WGD dates is {} billion years".format(mode_orig))
     plt.xlabel("Billion years ago", fontsize = 10)
     plt.ylabel("Frequency", fontsize = 10)
-    print(Ten_multi(int(maxim_orig)))
+    #print(Ten_multi(int(maxim_orig)))
     plt.yticks(np.linspace(0,Ten_multi(int(maxim_orig))+10,num=10,dtype=int))
     plt.hist(train_in,bins = np.linspace(minm, maxm, num=50),density=True,color = 'black', alpha=0.15, rwidth=0.8)
     props = dict(boxstyle='round', facecolor='grey', alpha=0.1)
     text = "\n".join(["Raw mode: {:4.4f}".format(mode_of_modes),"Peak: {:4.4f}".format(mode_orig),"CI: {:4.4f}-{:4.4f}".format(lower, upper),"OGs: {}".format(len(train_in))])
     plt.text(0.75,0.95,text,transform=ax.transAxes,fontsize=8,verticalalignment='top',bbox=props)
     fname = os.path.join(outdir, "WGD_peak.pdf")
     plt.tight_layout()
@@ -936,15 +1139,15 @@
         kde.set_bandwidth(kde.factor * bw_modifier)
         kde_y = kde(kde_x)
     if kdemethod == 'naivekde': kde_y = NaiveKDE(bw=bw).fit(X,weights=w).evaluate(kde_x)
     if kdemethod == 'treekde': kde_y = TreeKDE(bw=bw).fit(X,weights=w).evaluate(kde_x)
     if kdemethod == 'fftkde': kde_y = FFTKDE(bw=bw).fit(X,weights=w).evaluate(kde_x)
     return kde_y
 
-def plot_kmedoids_kde(boots,kdemethod,dfo,outdir,n,bin_width,bins=50,weighted=True,title="",plot='identical',alpha=0.50,regime='multiplicon'):
+def plot_kmedoids_kde(boots,kdemethod,dfo,outdir,n,bin_width,bins=50,weighted=True,title="",plot='identical',alpha=0.50,regime='multiplicon',user_xlim=None,user_ylim=None):
     fname = os.path.join(outdir,"{}-guide_AnchorKs_KMedoids_Clustering_{}components_kde.pdf".format(regime,n))
     f, ax = plt.subplots()
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     modes = {i:[] for i in range(n)}
     orig_modes = []
     css = []
@@ -997,46 +1200,50 @@
         cs = [c for c in cm.viridis(np.linspace(0, 1, n))]
         Xs = [getX(df,'node_averaged_dS_outlierexcluded') for df in dfs]
         labels = ['component {}'.format(i) for i in range(n)]
         plt.hist(Xs,bins = np.linspace(0, 5, num=int(5/bin_width)+1),color=cs,alpha=0.5,rwidth=0.8,stacked=True,label=labels)
     plt.xlabel("$K_\mathrm{S}$", fontsize = 10)
     plt.ylabel("Frequency", fontsize = 10)
     ax.legend(loc=1,fontsize='large',frameon=False)
+    if not (user_ylim[0]) is None: ax.set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: ax.set_xlim(user_xlim[0],user_xlim[1])
     sns.despine(offset=1)
     if regime=='multiplicon': plt.title('Multilplicon-guided Anchor $K_\mathrm{S}$ KMedoid modeling')
     elif regime=='segment': plt.title('Segment-guided Anchor $K_\mathrm{S}$ KMedoid modeling')
     else: plt.title('Basecluster-guided Anchor $K_\mathrm{S}$ KMedoid modeling')
     plt.tight_layout()
     plt.savefig(fname,format ='pdf', bbox_inches='tight')
     plt.close()
 
-def plot_segment_kmedoids(labels,X,outdir,bin_width,n,regime='segment'):
+def plot_segment_kmedoids(labels,X,outdir,bin_width,n,regime='segment',user_xlim=None,user_ylim=None):
     fname = os.path.join(outdir,"{}_Ks_KMedoids_Clustering_{}components.pdf".format(regime,n))
     f, ax = plt.subplots()
     df = pd.DataFrame(labels,columns=['KMedoids_Cluster'])
     df.index.name = 'label'
     df.loc[:,['Segment_Ks']] = X
     df = df.reset_index()
     for i,c in zip(range(n),cm.viridis(np.linspace(0, 1, n))):
         if n == 1: dfo = df.copy()
         else: dfo = df[df['KMedoids_Cluster']==i]
         data = getX(dfo,'Segment_Ks')
         ax.hist(data,bins = np.linspace(0, 5, num=int(5/bin_width)+1),color=c,alpha=0.5,rwidth=0.8,label='component {}'.format(i))
     plt.xlabel("$K_\mathrm{S}$", fontsize = 10)
     plt.ylabel("Number of segment pair", fontsize = 10)
     ax.legend(loc=1,fontsize='small',frameon=False)
+    if not (user_ylim[0]) is None: ax.set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: ax.set_xlim(user_xlim[0],user_xlim[1])
     sns.despine(offset=1)
     if regime=='multiplicon': plt.title('Multilplicon $K_\mathrm{S}$ KMedoid modeling')
     elif regime=='segment': plt.title('Segment  $K_\mathrm{S}$ KMedoid modeling')
     else: plt.title('Basecluster $K_\mathrm{S}$ KMedoid modeling')
     plt.tight_layout()
     plt.savefig(fname,format ='pdf', bbox_inches='tight')
     plt.close()
 
-def plot_kmedoids(boots,kdemethod,dfo,outdir,n,bin_width,bins=50,weighted=True,title="",plot='identical',alpha=0.50,regime='multiplicon'):
+def plot_kmedoids(boots,kdemethod,dfo,outdir,n,bin_width,bins=50,weighted=True,title="",plot='identical',alpha=0.50,regime='multiplicon',user_xlim=None,user_ylim=None):
     fname = os.path.join(outdir,"{}-guided_AnchorKs_KMedoids_Clustering_{}components.pdf".format(regime,n))
     f, ax = plt.subplots()
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     modes = {i:[] for i in range(n)}
     orig_modes = []
     css = []
@@ -1069,14 +1276,16 @@
         dfs = [dfo[dfo['KMedoids_Cluster']==i] for i in range(n)]
         cs = [c for c in cm.viridis(np.linspace(0, 1, n))]
         Xs = [getX(df,'node_averaged_dS_outlierexcluded') for df in dfs]
         plt.hist(Xs,bins = np.linspace(0, 5, num=int(5/bin_width)+1),color=cs,alpha=0.5,rwidth=0.8,stacked=True,label='component {}'.format(i))
     plt.xlabel("$K_\mathrm{S}$", fontsize = 10)
     plt.ylabel("Frequency", fontsize = 10)
     ax.legend(loc=1,fontsize='large',frameon=False)
+    if not (user_ylim[0]) is None: ax.set_ylim(user_ylim[0],user_ylim[1])
+    if not (user_xlim[0]) is None: ax.set_xlim(user_xlim[0],user_xlim[1])
     sns.despine(offset=1)
     if regime=='multiplicon': plt.title('Multilplicon-guided Anchor $K_\mathrm{S}$ KMedoid modeling')
     elif regime=='segment': plt.title('Segment-guided Anchor $K_\mathrm{S}$ KMedoid modeling')
     else: plt.title('Basecluster-guided Anchor $K_\mathrm{S}$ KMedoid modeling')
     plt.tight_layout()
     plt.savefig(fname,format ='pdf', bbox_inches='tight')
     plt.close()
@@ -1094,15 +1303,15 @@
         for x,l in zip(X_log,labels):
             if l == i:
                 sum_d = sum_d + (x - c)**2
         D.append(sum_d)
     Loss = sum(D)
     return Loss
 
-def find_mpeak(df,anchor,sp,outdir,guide,peak_threshold=0.1,rel_height=0.4,ci=95,user_low=0,user_upp=1,user=False):
+def find_mpeak(df,anchor,sp,outdir,guide,peak_threshold=0.1,rel_height=0.4,ci=95,user_low=0,user_upp=1,user=False,kscutoff=5):
     gs_ks = df.loc[:,['gene1','gene2',guide,'dS']]
     df_withindex,ks_or = bc_group_anchor(df,regime=guide)
     mpKs = pd.DataFrame.from_dict({guide:df_withindex.index,'Median_Ks':ks_or}).set_index(guide)
     df_m = df_withindex.copy()
     df_m['weightoutlierexcluded'] = 1
     w = np.array(df_m['weightoutlierexcluded'])
     ks = np.log(ks_or)
@@ -1129,18 +1338,18 @@
     ax.set_ylim(0, ax.get_ylim()[1] * 1.1)
     fig.tight_layout()
     fig.savefig(os.path.join(outdir, "{}_guided_{}_Ks_spline.pdf".format(guide,sp)))
     plt.close(fig)
     logging.info('Detecting likely peaks from {}-guided Ks data '.format(guide))
     init_means, init_stdevs, good_prominences = find_peak_init_parameters(spl_x,spl_y,sp,outdir,peak_threshold=peak_threshold,guide=guide,rel_height=rel_height)
     lower95CI,upper95CI = plot_95CI_lognorm_hist(init_means, init_stdevs, ks_or, w, outdir, False, sp, ci=ci,guide=guide)
-    if user: get95CIap_MP(user_low,user_upp,anchor,gs_ks,outdir,sp,ci,guide,mpKs,user=user)
-    else: get95CIap_MP(lower95CI,upper95CI,anchor,gs_ks,outdir,sp,ci,guide,mpKs,user=user)
+    if user: get95CIap_MP(user_low,user_upp,anchor,gs_ks,outdir,sp,ci,guide,mpKs,user=user,kscutoff=kscutoff)
+    else: get95CIap_MP(lower95CI,upper95CI,anchor,gs_ks,outdir,sp,ci,guide,mpKs,user=user,kscutoff=kscutoff)
 
-def find_apeak(df,anchor,sp,outdir,peak_threshold=0.1,na=False,rel_height=0.4,ci=95,user_low=0,user_upp=1,user=False):
+def find_apeak(df,anchor,sp,outdir,peak_threshold=0.1,na=False,rel_height=0.4,ci=95,user_low=0,user_upp=1,user=False,kscutoff=5):
     gs_ks = df.loc[:,['gene1','gene2','dS']]
     if na:
         df = df.drop_duplicates(subset=['family','node'])
         df = df.loc[:,['node_averaged_dS_outlierexcluded']].copy().rename(columns={'node_averaged_dS_outlierexcluded':'dS'})
         df['weightoutlierexcluded'] = 1
     df = df.dropna(subset=['dS','weightoutlierexcluded'])
     df = df.loc[(df['dS']>0) & (df['dS']<5),:]
@@ -1177,32 +1386,34 @@
         fig.savefig(os.path.join(outdir, "{}.spline_weighted.pdf".format(sp)))
     plt.close(fig)
     if na: logging.info('Detecting likely peaks from node-averaged data')
     else: logging.info('Detecting likely peaks from node-weighted data')
     init_means, init_stdevs, good_prominences = find_peak_init_parameters(spl_x,spl_y,sp,outdir,peak_threshold=peak_threshold,na=na,rel_height=rel_height)
     #lower95CI,upper95CI = plot_95CI_hist(init_means, init_stdevs, ks_or, w, outdir, na, sp)
     lower95CI,upper95CI = plot_95CI_lognorm_hist(init_means, init_stdevs, ks_or, w, outdir, na, sp, ci=ci)
-    if user: get95CIap(user_low,user_upp,anchor,gs_ks,outdir,na,sp,ci,user=user)
-    else: get95CIap(lower95CI,upper95CI,anchor,gs_ks,outdir,na,sp,ci,user=user)
+    if user: get95CIap(user_low,user_upp,anchor,gs_ks,outdir,na,sp,ci,user=user,kscutoff=kscutoff)
+    else: get95CIap(lower95CI,upper95CI,anchor,gs_ks,outdir,na,sp,ci,user=user,kscutoff=kscutoff)
 
-def get95CIap(lower,upper,anchor,gs_ks,outdir,na,sp,ci,user=False):
+def get95CIap(lower,upper,anchor,gs_ks,outdir,na,sp,ci,user=False,kscutoff=5):
     if type(lower) == float:
+        upper = min([upper,kscutoff])
         ap_95CI = gs_ks.loc[(gs_ks['dS']<=upper) & (gs_ks['dS']>=lower),:]
         sp_m = '{}'.format(sp)
         if na: fname = os.path.join(outdir, "{}_Manual_CI_AP_for_dating_node_averaged.tsv".format(sp_m))
         else: fname = os.path.join(outdir, "{}_Manual_CI_AP_for_dating_weighted.tsv".format(sp_m))
         ap_95CI.to_csv(fname,header=True,index=True,sep='\t')
         anchors = pd.read_csv(anchor, sep="\t", index_col=0)
         anchors["pair"] = anchors[["gene_x", "gene_y"]].apply(lambda x: "__".join(sorted([x[0], x[1]])), axis=1)
         ap_format = anchors.merge(ap_95CI.reset_index(),on='pair').drop(columns=['gene1', 'gene2','dS','pair'])
         ap_format.index.name = 'id'
         if na: fname = os.path.join(outdir, "{}_Manual_CI_AP_for_dating_node_averaged_format.tsv".format(sp_m))
         else: fname = os.path.join(outdir, "{}_Manual_CI_AP_for_dating_weighted_format.tsv".format(sp_m))
         ap_format.to_csv(fname,header=True,index=True,sep='\t')
     elif len(lower) == 1:
+        upper[0] = min([upper[0],kscutoff])
         ap_95CI = gs_ks.loc[(gs_ks['dS']<=upper[0]) & (gs_ks['dS']>=lower[0]),:]
         sp_m = '{}'.format(sp)
         if user:
             if na: fname = os.path.join(outdir, "{}_Manual_CI_AP_for_dating_node_averaged.tsv".format(sp_m))
             else: fname = os.path.join(outdir, "{}_Manual_CI_AP_for_dating_weighted.tsv".format(sp_m))
         else:
             if na: fname = os.path.join(outdir, "{}_{}%CI_AP_for_dating_node_averaged.tsv".format(sp_m,ci))
@@ -1217,15 +1428,15 @@
             else: fname = os.path.join(outdir, "{}_Manual_CI_AP_for_dating_weighted_format.tsv".format(sp_m))
         else:
             if na: fname = os.path.join(outdir, "{}_{}%CI_AP_for_dating_node_averaged_format.tsv".format(sp_m,ci))
             else: fname = os.path.join(outdir, "{}_{}%CI_AP_for_dating_weighted_format.tsv".format(sp_m,ci))
         ap_format.to_csv(fname,header=True,index=True,sep='\t')
     else:
         for indice,i in enumerate(zip(lower,upper)):
-            lower,upper = i[0],i[1]
+            lower,upper = i[0],min([i[1],kscutoff])
             text = 'Peak_{}_'.format(indice+1)
             ap_95CI = gs_ks.loc[(gs_ks['dS']<=upper) & (gs_ks['dS']>=lower),:]
             sp_m = text + '{}'.format(sp)
             if user:
                 if na: fname = os.path.join(outdir, "{}_Manual_CI_AP_for_dating_node_averaged.tsv".format(sp_m))
                 else: fname = os.path.join(outdir, "{}_Manual_CI_AP_for_dating_weighted.tsv".format(sp_m))
             else:
@@ -1249,28 +1460,30 @@
     predict_column = pd.DataFrame(labels,index=df_index.index,columns=['AnchorKs_GMM_Component']).reset_index()
     df = df.reset_index().merge(predict_column, on = [regime])
     df = df.set_index('pair')
     fname = os.path.join(outdir,'AnchorKs_GMM_{}components_prediction.tsv'.format(n))
     df.to_csv(fname,header=True,index=True,sep='\t')
     return df
 
-def get95CIap_MP(lower,upper,anchor,gs_ks,outdir,sp,ci,guide,mpKs,user=False):
+def get95CIap_MP(lower,upper,anchor,gs_ks,outdir,sp,ci,guide,mpKs,user=False,kscutoff=5):
     gs_ks = gs_ks.reset_index().set_index(guide).join(mpKs)
     if type(lower) == float:
+        upper = min([kscutoff,upper])
         ap_95CI = gs_ks.loc[(gs_ks['Median_Ks']<=upper) & (gs_ks['Median_Ks']>=lower),:]
         sp_m = '{}_guided_{}'.format(guide,sp)
         fname = os.path.join(outdir, "{}_Manual_CI_MP_for_dating.tsv".format(sp_m))
         ap_95CI.to_csv(fname,header=True,index=True,sep='\t')
         anchors = pd.read_csv(anchor, sep="\t", index_col=0)
         anchors["pair"] = anchors[["gene_x", "gene_y"]].apply(lambda x: "__".join(sorted([x[0], x[1]])), axis=1)
         ap_format = anchors.merge(ap_95CI.reset_index(),on='pair').drop(columns=['gene1', 'gene2','dS','pair','Median_Ks'])
         ap_format.index.name = 'id'
         fname = os.path.join(outdir, "{}_Manual_CI_MP_for_dating_format.tsv".format(sp_m))
         ap_format.to_csv(fname,header=True,index=True,sep='\t')
     elif len(lower) == 1:
+        upper[0] = min([upper[0],kscutoff])
         ap_95CI = gs_ks.loc[(gs_ks['Median_Ks']<=upper[0]) & (gs_ks['Median_Ks']>=lower[0]),:]
         sp_m = '{}_guided_{}'.format(guide,sp)
         if user: fname = os.path.join(outdir, "{}_Manual_CI_MP_for_dating.tsv".format(sp_m))
         else: fname = os.path.join(outdir, "{}_{}%CI_MP_for_dating.tsv".format(sp_m,ci))
         ap_95CI.to_csv(fname,header=True,index=True,sep='\t')
         anchors = pd.read_csv(anchor, sep="\t", index_col=0)
         anchors["pair"] = anchors[["gene_x", "gene_y"]].apply(lambda x: "__".join(sorted([x[0], x[1]])), axis=1)
@@ -1278,81 +1491,29 @@
         ap_format.index.name = 'id'
         if user: fname = os.path.join(outdir, "{}_Manual_CI_MP_for_dating_format.tsv".format(sp_m))
         else: fname = os.path.join(outdir, "{}_{}%CI_MP_for_dating_format.tsv".format(sp_m,ci))
         ap_format.to_csv(fname,header=True,index=True,sep='\t')
     else:
         for indice,i in enumerate(zip(lower,upper)):
             text = 'Peak_{}_'.format(indice+1)
-            lower,upper = i[0],i[1]
+            lower,upper = i[0],min([i[1],kscutoff])
             ap_95CI = gs_ks.loc[(gs_ks['Median_Ks']<=upper) & (gs_ks['Median_Ks']>=lower),:]
             sp_m = text + '{}_guided_{}'.format(guide,sp)
             if user: fname = os.path.join(outdir, "{}_Manual_CI_MP_for_dating.tsv".format(sp_m))
             else: fname = os.path.join(outdir, "{}_{}%CI_MP_for_dating.tsv".format(sp_m,ci))
             ap_95CI.to_csv(fname,header=True,index=True,sep='\t')
             anchors = pd.read_csv(anchor, sep="\t", index_col=0)
             anchors["pair"] = anchors[["gene_x", "gene_y"]].apply(lambda x: "__".join(sorted([x[0], x[1]])), axis=1)
             ap_format = anchors.merge(ap_95CI.reset_index(),on='pair').drop(columns=['gene1', 'gene2','dS','pair','Median_Ks'])
             ap_format.index.name = 'id'
             if user: fname = os.path.join(outdir, "{}_Manual_CI_MP_for_dating_format.tsv".format(sp_m))
             else: fname = os.path.join(outdir, "{}_{}%CI_MP_for_dating_format.tsv".format(sp_m,ci))
             ap_format.to_csv(fname,header=True,index=True,sep='\t')
 
 
-def get_outlierexcluded(df,cutoff = 5):
-    df = df[df['dS']<cutoff]
-    weight_exc = 1/df.groupby(['family', 'node'])['dS'].transform('count')
-    weight_exc = weight_exc.to_frame(name='weightoutlierexcluded')
-    return weight_exc
-
-def get_outlierincluded(df):
-    weight_inc = 1/df.groupby(['family', 'node'])['dS'].transform('count')
-    weight_inc = weight_inc.to_frame(name='weightoutlierincluded')
-    return weight_inc
-
-def get_nodeaverged_dS_outlierincluded(df):
-    node_averaged_dS_inc = df.groupby(["family", "node"])["dS"].mean()
-    node_averaged_dS_inc = node_averaged_dS_inc.to_frame(name='node_averaged_dS_outlierincluded')
-    return node_averaged_dS_inc
-
-def get_nodeaverged_dS_outlierexcluded(df,cutoff = 5):
-    df = df[df['dS']<cutoff]
-    node_averaged_dS_exc = df.groupby(["family", "node"])["dS"].mean()
-    node_averaged_dS_exc = node_averaged_dS_exc.to_frame(name='node_averaged_dS_outlierexcluded')
-    return node_averaged_dS_exc
-
-def formatv2(ksdf):
-    if "Ks" in ksdf.columns: ksdf = ksdf.rename(columns={"Ks":"dS"})
-    if "Ka" in ksdf.columns: ksdf = ksdf.rename(columns={"Ka":"dN"})
-    if "Omega" in ksdf.columns: ksdf = ksdf.rename(columns={"Omega":"dN/dS"})
-    if "Family" in ksdf.columns: ksdf = ksdf.rename(columns={"Family":"family"})
-    if "Node" in ksdf.columns: ksdf = ksdf.rename(columns={"Node":"node"})
-    if "AlignmentIdentity" in ksdf.columns: ksdf = ksdf.rename(columns={"AlignmentIdentity":"alignmentidentity"})
-    if "AlignmentLength" in ksdf.columns: ksdf = ksdf.rename(columns={"AlignmentLength":"alignmentlength"})
-    if "AlignmentCoverage" in ksdf.columns: ksdf = ksdf.rename(columns={"AlignmentCoverage":"alignmentcoverage"})
-    if "Paralog1" in ksdf.columns: ksdf = ksdf.rename(columns={"Paralog1":"gene1"})
-    if "Paralog2" in ksdf.columns: ksdf = ksdf.rename(columns={"Paralog2":"gene2"})
-    if "WeightOutliersIncluded" in ksdf.columns: ksdf = ksdf.drop(columns=["WeightOutliersIncluded"])
-    if "WeightOutliersExcluded" in ksdf.columns: ksdf = ksdf.drop(columns=["WeightOutliersExcluded"])
-    if "weightoutlierexcluded" not in ksdf.columns: weight_inc = get_outlierincluded(ksdf)
-    if "weightoutlierincluded" not in ksdf.columns:
-        weight_exc = get_outlierexcluded(ksdf,cutoff = 5)
-        ksdf = ksdf.join(weight_inc).join(weight_exc)
-    if "node_averaged_dS_outlierincluded" not in ksdf.columns:
-        node_averaged_dS_inc = get_nodeaverged_dS_outlierincluded(ksdf)
-    if "node_averaged_dS_outlierexcluded" not in ksdf.columns:
-        node_averaged_dS_exc = get_nodeaverged_dS_outlierexcluded(ksdf,cutoff = 5)
-        ksdf = ksdf.reset_index().merge(node_averaged_dS_inc,on = ['family', 'node'])
-        ksdf = ksdf.merge(node_averaged_dS_exc,on = ['family', 'node'],how = 'left')
-    #ksdf = ksdf.join(weight_inc).join(weight_exc) # here I kept the NaN value
-    #ksdf = ksdf.reset_index().merge(node_averaged_dS_inc,on = ['family', 'node'])
-    #ksdf = ksdf.merge(node_averaged_dS_exc,on = ['family', 'node'],how = 'left')
-    if "index" in ksdf.columns: ksdf = ksdf.set_index('index')
-    ksdf.index.name = 'pair'
-    return ksdf
-
 def plot_95CI_hist(init_means, init_stdevs, ks_or, w, outdir, na, sp, guide = None):
     text = "AnchorKs_PeakCI_"
     #if guide != None: text = "AnchorKs_PeakCI_{}_guided_".format(guide)
     if guide != None: fname = os.path.join(outdir, "{}{}_guided_{}.pdf".format(text,guide,sp))
     elif na: fname = os.path.join(outdir, "{}{}_node_averaged.pdf".format(text,sp))
     else: fname = os.path.join(outdir, "{}{}_node_weighted.pdf".format(text,sp))
     f, ax = plt.subplots()
@@ -1383,27 +1544,29 @@
     if guide != None: fname = os.path.join(outdir, "{}Ks_PeakCI_{}.pdf".format(guide,sp))
     elif na: fname = os.path.join(outdir, "AnchorKs_PeakCI_{}_node_averaged.pdf".format(sp))
     else: fname = os.path.join(outdir, "AnchorKs_PeakCI_{}_node_weighted.pdf".format(sp))
     f, ax = plt.subplots()
     x_points_strictly_positive = np.linspace(0, 5, int(5 * 100))
     bin_width = 0.1
     cs = ['b','g','y','r','k']
-    alphas = np.linspace(0.3, 0.7, len(init_means))
+    #alphas = np.linspace(0.3, 0.7, len(init_means))
     ci_l = (1-ci/100)/2
     ci_u = 1-(1-ci/100)/2
     CI_95s = []
     for mean,std,i in zip(init_means, init_stdevs,range(len(init_means))):
         Hs, Bins, patches = ax.hist(ks_or,bins = np.linspace(0, 5, num=int(5/bin_width)+1),weights=w,color='gray', alpha=1, rwidth=0.8)
         CHF = get_totalH(Hs)
         scaling = CHF*0.1
         ax.plot(x_points_strictly_positive,scaling*stats.lognorm.pdf(x_points_strictly_positive, scale=np.exp(mean),s=std), c=cs[i], ls='-', lw=1.5, alpha=0.8, label='Peak {} mode {:.2f}'.format(i+1,np.exp(mean - std**2)))
         CI_95 = stats.lognorm.ppf([ci_l, ci_u], scale=np.exp(mean), s=std)
         CI_95s.append(CI_95)
-        plt.axvline(x = CI_95[0], color = cs[i], alpha = alphas[i], ls = ':', lw = 1,label='Peak {} lower {}%CI {:.2f}'.format(i+1,ci,CI_95[0]))
-        plt.axvline(x = CI_95[1], color = cs[i], alpha = alphas[i], ls = ':', lw = 1,label='Peak {} upper {}%CI {:.2f}'.format(i+1,ci,CI_95[1]))
+        CI_95_y0 = scaling*stats.lognorm.pdf(CI_95[0], scale=np.exp(mean),s=std)/ax.get_ylim()[1]
+        CI_95_y1 = scaling*stats.lognorm.pdf(CI_95[1], scale=np.exp(mean),s=std)/ax.get_ylim()[1]
+        plt.axvline(x = CI_95[0], ymin=0, ymax=CI_95_y0, color = cs[i], alpha = 0.8, ls = ':', lw = 1,label='Peak {} lower {}%CI {:.2f}'.format(i+1,ci,CI_95[0]))
+        plt.axvline(x = CI_95[1], ymin=0, ymax=CI_95_y1, color = cs[i], alpha = 0.8, ls = ':', lw = 1,label='Peak {} upper {}%CI {:.2f}'.format(i+1,ci,CI_95[1]))
     plt.xlabel("$K_\mathrm{S}$", fontsize = 10)
     if guide == 'segment': plt.ylabel("Number of segment pair", fontsize = 10)
     elif guide != None: plt.ylabel("Number of {}".format(guide), fontsize = 10)
     elif na: plt.ylabel("Number of retained duplicates (node averaged)", fontsize = 10)
     else: plt.ylabel("Number of retained duplicates (weighted)", fontsize = 10)
     ax.legend(loc=1,fontsize='large',frameon=False)
     ax.set_xlim(0, 5)
@@ -1440,15 +1603,15 @@
     anchors = pd.read_csv(anchor, sep="\t", index_col=0)
     anchors["pair"] = anchors[["gene_x", "gene_y"]].apply(lambda x: "__".join(sorted([x[0], x[1]])), axis=1)
     df = anchors[["pair", "basecluster",'multiplicon']].drop_duplicates("pair").set_index("pair")
     return df
 
 def get_anchor_ksd(ksdf, apdf):
     return ksdf.join(apdf).dropna()
-    # here any NA occurred per row is dropped
+    # here any NA occurred per row is dropped, normally a row has all NaN or only weightexclu and nodeKsexcl NaN
 
 def bc_group_anchor(df,regime='multiplicon'):
     #median_df = df.groupby(["basecluster"]).median()
     median_df = df.groupby([regime]).median()
     X = getX(median_df,'dS')
     return median_df,X
 
@@ -1469,38 +1632,42 @@
 
 def add_seg(df,listelement,multipliconpairs,segment):
     #Here the df should be Ks 0-5 filter
     #It hasn't to be ap in listelement note that a same pair of syntelogs can be in different multiplicon
     mp = pd.read_csv(multipliconpairs, sep="\t", index_col=0)
     if len(mp.columns) == 5: mp = mp.drop(columns=['gene_y']).rename(columns = {'gene_x':'gene_y'}).rename(columns = {'Unnamed: 2':'gene_x'})
     mp = mp.loc[:,['multiplicon','gene_x','gene_y']]
-    mp.loc[:,['pair']] = ["__".join(sorted([x,y])) for x,y in zip(list(mp['gene_x']),list(mp['gene_y']))]
-    mp = mp.drop_duplicates(subset=['pair'])
+    mp.loc[:,['pair']] = ["__".join(sorted([x,y])) for x,y in zip(mp['gene_x'],mp['gene_y'])]
+    mp = mp.drop_duplicates(subset=['pair']) # at this step half of the data will be filtered out
     mp.loc[:,['id']] = [i for i in range(mp.shape[0])]
     #mp= mp.drop_duplicates(subset=['pair']) #Here the same gene pair can be in different multiplicon
     df_seg = pd.read_csv(segment,header=0,index_col=None,sep='\t').rename(columns = {'id':'segment'}).loc[:,['segment','multiplicon']]
     df_le = pd.read_csv(listelement,header=0,index_col=0,sep='\t').merge(df_seg,on='segment').rename(columns = {'multiplicon':'multiplicon_x'}).loc[:,['segment','multiplicon_x','gene']]
     #mp_segment_pools = {mt:list(set(df_seg[df_seg['multiplicon']==mt]['segment'])) for mt in df_seg['multiplicon']}
     #segment_gene_pools = {sg:list(set(df_le[df_le['segment']==sg]['gene'])) for sg in df_le['segment']}
     df_mp_le = mp.merge(df_le,left_on='gene_x',right_on='gene')
     df_mp_le = df_mp_le[df_mp_le['multiplicon_x'] == df_mp_le['multiplicon']]
     df_mp_le = df_mp_le.rename(columns = {'segment':'segment_x'})
     # here the genes belonging to two segments in the same multiplicon were removed because of indeterminacy
-    df_mp_le = df_mp_le.drop_duplicates(subset=['id'],keep=False)
+    #df_mp_le = df_mp_le.drop_duplicates(subset=['id'],keep=False)
     df_mp_le_r = df_mp_le.drop(columns=['multiplicon_x','gene']).merge(df_le,left_on='gene_y',right_on='gene')
     df_mp_le_r = df_mp_le_r[df_mp_le_r['multiplicon_x'] == df_mp_le_r['multiplicon']]
     df_mp_le_r = df_mp_le_r.rename(columns = {'segment':'segment_y'})
-    df_mp_le_r = df_mp_le_r.drop_duplicates(subset=['id'],keep=False)
+    #df_mp_le_r = df_mp_le_r.drop_duplicates(subset=['id'],keep=False)
+    df_mp_le_r = df_mp_le_r.drop_duplicates() # only drop those fully duplicated
     df_mp_le_r = df_mp_le_r.loc[:,['multiplicon','gene_x','gene_y','segment_x','segment_y','pair']].set_index('pair')
     df_mp_le_r.loc[:,['segment_pair']] = ["__".join(sorted([x,y])) for x,y in zip(list(df_mp_le_r['segment_x'].astype(str)),list(df_mp_le_r['segment_y'].astype(str)))]
-    df_cal_medKs = df_mp_le_r.loc[:,['segment_pair','multiplicon']].join(df).rename(columns = {'segment_pair':'segment'}).dropna(subset=['dS']) # here I kept Ks > 5 and duplicated index (pair)
+    df_cal_medKs = df_mp_le_r.loc[:,['segment_pair','multiplicon']].join(df).rename(columns = {'segment_pair':'segment'}).dropna(subset=['dS'])
+    # here I filter  Ks >= 5
     dS_median = df_cal_medKs.groupby(['segment'])['dS'].median()
+    seg_weight = {seg:len(df_tmp) for seg, df_tmp in list(df_cal_medKs.groupby(['segment']))}
     dS_median = dS_median[dS_median<5]
     dS_median.name = 'Segment_dS'
     df_cal_medKs = df_cal_medKs.reset_index().merge(dS_median.reset_index(),on='segment').dropna(subset=['Segment_dS']).set_index('pair')
+    segment_weight = list(df_cal_medKs['segment'].apply(lambda x:seg_weight[x]))
     #df_cal_medKs = df.join(df_mp_le_r.loc[:,['segment_pair','multiplicon']]).rename(columns = {'segment_pair':'segment'}) # here I did keep the NaN value, which impacted and changed the median Ks values afterwards
     #df_mp_le_r = mp.merge(df_le,left_on='gene_y',right_on='gene')
     #df_mp_le_r = df_mp_le_r[df_mp_le_r['multiplicon_x'] == df_mp_le_r['multiplicon']]
     #df_mp_le_r = df_mp_le_r.rename(columns = {'segment':'segment_y'})
     #df_mp_le_lr = df_mp_le.loc[:,['multiplicon','gene_x','gene_y','segment_x','pair']].merge(df_mp_le_r.loc[:,['pair','segment_y']],on='pair').set_index('pair')
     #df_mp_le_lr.loc[:,['segment_pair']] = ["__".join(sorted([x,y])) for x,y in zip(list(df_mp_le_lr['segment_x'].astype(str)),list(df_mp_le_lr['segment_y'].astype(str)))]
     #df_cal_medKs = df.join(df_mp_le_lr.loc[:,['segment_pair','multiplicon']]).dropna().rename(columns = {'segment_pair':'segment'})
@@ -1512,15 +1679,15 @@
     #df_cal_medKs = df_withKs.drop_duplicates(subset=['segment','gene_y']).drop_duplicates(subset=['segment','gene_x'])
     #df_cal_medKs = df_cal_medKs.drop(columns=['gene_y','multiplicon_x','gene_x','gene'])
     #Here we retrive the duplicates information for segment age clustering
     #dup_le = df_withKs[df_withKs.duplicated(subset=['segment','gene_y'], keep=False)]
     #dup_ri = df_withKs[df_withKs.duplicated(subset=['segment','gene_x'], keep=False)]
     #dup_combined = pd.concat([dup_le,dup_ri], ignore_index=True).drop_duplicates()
     #dup_combined_work = dup_combined.loc[:,['segment','gene_x','gene_y','dS']]
-    return df_cal_medKs
+    return df_cal_medKs, segment_weight
 
 def getDM(X):
     dm = np.zeros((len(X), len(X)))
     for i in range(len(X)):
         for j in range(i+1, len(X)):
             dm[i,j] = dm[j,i] = (abs(X[i][0] - X[j][0]))**2
     return dm
@@ -1596,125 +1763,165 @@
     #        lower_bound_indice = i
     #        break
     for (x,y) in itertools.product(np.arange(0,lower_bound_indice,1,dtype=int), np.arange(upper_bound_indice,len(sorted_in),1,dtype=int)):
         if (y-x+1) >= cutoff: candidates.append((sorted_in[y] - sorted_in[x],(x,y)))
     lower,upper = sorted(candidates, key=lambda y: y[0])[0][1][0],sorted(candidates, key=lambda y: y[0])[0][1][1]
     return sorted_in[upper],sorted_in[lower]
 
-def fit_apgmm_guide(hdr,guide,anchor,df_nofilter,dfor,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot,segment=None,multipliconpairs=None,listelement=None,cutoff=None):
+def get_mp_ksd(multipliconpairs,df):
+    mp = pd.read_csv(multipliconpairs, sep="\t", index_col=0)
+    if len(mp.columns) == 5: mp = mp.drop(columns=['gene_y']).rename(columns = {'gene_x':'gene_y'}).rename(columns = {'Unnamed: 2':'gene_x'})
+    mp.loc[:,['pair']] = ["__".join(sorted([x,y])) for x,y in zip(mp['gene_x'],mp['gene_y'])]
+    mp = mp.drop_duplicates(subset=['pair']).set_index('pair').loc[:,['multiplicon','gene_x','gene_y']]
+    mp_ks = mp.join(df).dropna()
+    return mp_ks
+
+def weighttransform(X_log,seg_weight):
+    new_X_log = np.array([])
+    for ks,times in zip(X_log,seg_weight):
+        new_X_log = np.append(new_X_log,np.repeat(ks, times))
+    return new_X_log.reshape(-1, 1)
+
+def fit_apgmm_guide(hdr,guide,anchor,df_nofilter,dfor,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot,segment=None,multipliconpairs=None,listelement=None,cutoff=None,user_xlim=None,user_ylim=None):
+    logging.info("GMM modeling on Log-scale segment Ks data")
     if anchor == None:
         logging.error('Please provide anchorpoints.txt file for Anchor Ks GMM Clustering')
         exit(0)
     df_ap = get_anchors(anchor)
     df = get_anchor_ksd(dfor, df_ap)
+    df_mp = get_mp_ksd(multipliconpairs,df_nofilter)
     df_nofilter = df_nofilter[df_nofilter['dS']>0]
     if segment!= None:
-        df = add_seg(df_nofilter,listelement,multipliconpairs,segment)
+        df, seg_weight = add_seg(df_nofilter,listelement,multipliconpairs,segment)
         df.to_csv(os.path.join(outdir, "Segment_Ks.tsv"),header=True,index=True,sep='\t')
     df_withindex,X = bc_group_anchor(df,regime=guide)
     X_log = np.log(X).reshape(-1, 1)
     out_file = os.path.join(outdir, "{}_Ks_GMM_AIC_BIC.pdf".format(guide))
+    #X_log = weighttransform(X_log,seg_weight)
     if method == 'gmm': models, aic, bic, besta, bestb, N = fit_gmm(out_file, X_log, seed, components[0], components[1], em_iter=em_iter, n_init=n_init)
     if method == 'bgmm': models, N = fit_bgmm(X_log, seed, gamma, components[0], components[1], em_iter=em_iter, n_init=n_init)
     if components[0] == 1 and components[1] > 1:
         plot_silhouette_score(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:],outdir,guide+'_Ks','GMM')
-        significance_test_cluster(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:])
+        #significance_test_cluster(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:])
     else:
         plot_silhouette_score(X_log,components[0],components[1],[m.predict(X_log) for m in models],outdir,guide+'_Ks','GMM')
-        significance_test_cluster(X_log,components[0],components[1],[m.predict(X_log) for m in models])
+        #significance_test_cluster(X_log,components[0],components[1],[m.predict(X_log) for m in models])
     Losses = []
     for n, m in zip(N,models):
         labels = m.predict(X_log)
         df_c = add_apgmmlabels(df,df_withindex,labels,outdir,n,regime=guide)
         means,stds,weights = m.means_,m.covariances_,m.weights_
         Losses.append(Elbow_lossf(X_log,[i[0] for i in means],labels))
-        fig = plot_mp_component(X,labels,n,bins=50,plot = plot,ylabel="Number of segment pair",regime=guide)
+        fig = plot_mp_component(X,labels,n,bins=50,plot = plot,ylabel="Number of segment pair",regime=guide,user_xlim=user_xlim,user_ylim=user_ylim)
         fname = os.path.join(outdir, "{}_Ks_Clusters_GMM_Component{}.pdf".format(guide,n))
         fig.savefig(fname)
         plt.close()
-        fig = plot_mp_component_lognormal(X,hdr,means,stds,weights,labels,n,bins=50,ylabel="Number of segment pair",regime=guide)
+        fig, kdexs, kdeys, modes = plot_mp_component_lognormal(X,hdr,means,stds,weights,labels,n,bins=50,ylabel="Number of segment pair",regime=guide,user_xlim=user_xlim,user_ylim=user_ylim)
         #hdr_ap(hdr,df,df_withindex)
         fname = os.path.join(outdir, "{}_Ks_Clusters_Lognormal_GMM_Component{}.pdf".format(guide,n))
         fig.savefig(fname)
         plt.close()
-    plot_Elbow_loss(Losses,outdir,n1=components[0],n2=components[1],method='GMM',regime=guide)
-    for n, m in zip(N,models):
-        fig = plot_ak_component(df_c.dropna(),n,bins=50,plot = plot,ylabel="Duplication events",weighted=weighted,regime=guide)
+        #fig = plot_mpbackap_lognormal(df_mp,kdexs,kdeys,modes,guide)
+        #fname = os.path.join(outdir, "Syntelogs_Ks_Clusters_From_{}_Component{}.pdf".format(guide,n))
+        #fig.savefig(fname)
+        plt.close()
+    #for n, m in zip(N,models):
+        fig = plot_ak_component(df_c.dropna(),n,bins=50,plot = plot,ylabel="Duplication events",weighted=weighted,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim)
         if weighted: fname = os.path.join(outdir, "{}-guided_AnchorKs_GMM_Component{}_node_weighted.pdf".format(guide,n))
         else: fname = os.path.join(outdir, "{}-guided_AnchorKs_GMM_Component{}_node_averaged.pdf".format(guide,n))
         fig.savefig(fname)
         plt.close()
-        fig,HDRs = plot_ak_component_kde(df_c.dropna(),n,hdr,bins=50,ylabel="Duplication events",weighted=weighted,regime=guide)
+        fig,HDRs = plot_ak_component_kde(df_c.dropna(),n,hdr,bins=50,ylabel="Duplication events",weighted=weighted,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim)
         getGuided_AP_HDR(HDRs,hdr,n,df_c,outdir,guide,cutoff)
         if weighted: fname = os.path.join(outdir, "{}-guided_AnchorKs_GMM_Component{}_node_weighted_kde.pdf".format(guide,n))
         else: fname = os.path.join(outdir, "{}-guided_AnchorKs_GMM_Component{}_node_averaged_kde.pdf".format(guide,n))
         fig.savefig(fname)
         plt.close()
+    plot_Elbow_loss(Losses,outdir,n1=components[0],n2=components[1],method='GMM',regime=guide)
     return df
 
 def getGuided_AP_HDR(HDRs,hdr,n,df_c,outdir,regime,cutoff):
     for num in HDRs.keys():
         df_tmp = df_c[df_c['AnchorKs_GMM_Component']==num]
         df_tmp = df_tmp.loc[(df_tmp['dS']<=min([cutoff,HDRs[num][1]])) & (df_tmp['dS']>=HDRs[num][0]),:]
         df_tmp = df_tmp.loc[:,['gene1','gene2','dS','Segment_dS','AnchorKs_GMM_Component']].rename(columns={"gene1":"gene_x","gene2":"gene_y"})
         fname = os.path.join(outdir,"{}_guided_{}%HDR_Syntelogs_Component{}_Model{}_WGDating.tsv".format(regime,hdr,num,n))
         df_tmp.to_csv(fname,sep='\t',header=True,index=True)
 
-def fit_apgmm_ap(hdr,anchor,df,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot):
+def fit_apgmm_ap(hdr,anchor,df,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot,heuristic,showCI=False,cutoff = 5,peak_threshold=0.1,rel_height=0.4,user_xlim=None,user_ylim=None):
     if anchor == None:
         logging.error('Please provide anchorpoints.txt file for Anchor Ks GMM Clustering')
         exit(0)
     df_ap = get_anchors(anchor)
     df = get_anchor_ksd(df, df_ap)
     df_withindex,X = df.index,getX(df,'dS')
     X_log = np.log(X).reshape(-1, 1)
     out_file = os.path.join(outdir, "Original_AnchorKs_GMM_AIC_BIC.pdf")
     logging.info("GMM modeling on Log-scale original anchor Ks data")
     if method == 'gmm': models, aic, bic, besta, bestb, N = fit_gmm(out_file, X_log, seed, components[0], components[1], em_iter=em_iter, n_init=n_init)
     if method == 'bgmm': models, N = fit_bgmm(X_log, seed, gamma, components[0], components[1], em_iter=em_iter, n_init=n_init)
     if components[0] == 1 and components[1] > 1:
         plot_silhouette_score(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:],outdir,'Original_AnchorKs','GMM')
-        significance_test_cluster(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:])
+        #significance_test_cluster(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:])
     else:
         plot_silhouette_score(X_log,components[0],components[1],[m.predict(X_log) for m in models],outdir,'Original_AnchorKs','GMM')
-        significance_test_cluster(X_log,components[0],components[1],[m.predict(X_log) for m in models])
+        #significance_test_cluster(X_log,components[0],components[1],[m.predict(X_log) for m in models])
     Losses = []
     for n, m in zip(N,models):
         labels = m.predict(X_log)
         means,stds,weights = m.means_,m.covariances_,m.weights_
         Losses.append(Elbow_lossf(X_log,[i[0] for i in means],labels))
         df_c = add_apgmmlabels_pairs(df,df_withindex,labels,outdir,n)
-        fig = plot_ak_component(df_c,n,bins=50,plot = plot,ylabel="Duplication events",weighted=weighted,regime='original')
+        fig = plot_ak_component(df_c,n,bins=50,plot = plot,ylabel="Duplication events",weighted=weighted,regime='original',user_xlim=user_xlim,user_ylim=user_ylim)
         if weighted: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_weighted.pdf".format(n))
         else: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_averaged.pdf".format(n))
         fig.savefig(fname)
         plt.close()
         #fig = plot_ak_component_kde(df_c,n,bins=50,ylabel="Duplication events",weighted=weighted,regime='original')
         #if weighted: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_weighted_kde.pdf".format(n))
         #else: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_averaged_kde.pdf".format(n))
         #fig.savefig(fname)
         #plt.close()
-        fig = plot_ak_component_lognormal(df_c.dropna(),means,stds,weights,n,bins=50,ylabel="Duplication events",weighted=weighted,regime='original')
+        fig, CI = plot_ak_component_lognormal(df_c.dropna(),means,stds,weights,n,bins=50,ylabel="Duplication events",weighted=weighted,regime='original',showCI=showCI,heuristic=heuristic,peak_threshold=peak_threshold,rel_height=rel_height,user_xlim=user_xlim,user_ylim=user_ylim)
+        if showCI or heuristic: df_c_CI = add_apCI(df_c,outdir,CI,n,cutoff)
         if weighted: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_weighted_Lognormal.pdf".format(n))
         else: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_averaged_Lognormal.pdf".format(n))
         fig.savefig(fname)
         plt.close()
     plot_Elbow_loss(Losses,outdir,n1=components[0],n2=components[1],method='GMM',regime='original')
     return df
 
-def fit_kmedoids(guide,anchor, boots, kdemethod, bin_width, weighted, df_nofilter, df, outdir, seed, n, em_iter=100, metric='euclidean', method='pam', init ='k-medoids++', plot = 'identical', n_kmedoids = 5, segment= None, multipliconpairs=None,listelement=None):
+def add_apCI(df,outdir,CI,n,cutoff):
+    for categ, content in CI.items():
+        if len(content) == 0:
+            continue
+        for comp, ci in content.items():
+            if ci is None:
+                continue
+            df_tmp = df[df['AnchorKs_GMM_Component']==comp]
+            maxi = min([ci[1],cutoff])
+            df_tmp = df_tmp[ci[0]<=df_tmp['dS']]
+            df_tmp = df_tmp[df_tmp['dS']<=maxi].loc[:,['dS']].copy()
+            df_tmp['gene_x'], df_tmp['gene_y'] = [pair.split("__")[0] for pair in df_tmp.index], [pair.split("__")[1] for pair in df_tmp.index]
+            if categ == 'showci':
+                fname = os.path.join(outdir,'Original_AnchorKs_GMM_{0}components_C{1}_95%CI.tsv'.format(n,comp))
+            elif categ == 'heuristic':
+                fname = os.path.join(outdir,'Original_AnchorKs_GMM_{0}components_P{1}_95%CI.tsv'.format(n,comp))
+            df_tmp.to_csv(fname,header=True,index=True,sep='\t')
+
+
+def fit_kmedoids(guide,anchor, boots, kdemethod, bin_width, weighted, df_nofilter, df, outdir, seed, n, em_iter=100, metric='euclidean', method='pam', init ='k-medoids++', plot = 'identical', n_kmedoids = 5, segment= None, multipliconpairs=None,listelement=None,user_xlim=None,user_ylim=None):
     """
     Clustering with KMedoids to delineate different anchor groups from anchor Ks distribution
     """
     if anchor == None:
         logging.error('Please provide anchorpoints.txt file for Anchor Ks KMedoids Clustering')
         exit(0)
     df_ap = get_anchors(anchor)
     df = get_anchor_ksd(df, df_ap)
-    #if segment!= None: df = add_seg(df,segment)
     df_nofilter = df_nofilter[df_nofilter['dS']>0]
     if segment!= None:
         df = add_seg(df_nofilter,listelement,multipliconpairs,segment)
         df.to_csv(os.path.join(outdir, "Segment_Ks.tsv"),header=True,index=True,sep='\t')
     df_withindex,X = bc_group_anchor(df,regime=guide)
     #df = df.dropna(subset=['node_averaged_dS_outlierexcluded'])
     #df_rmdup = df.drop_duplicates(subset=['family', 'node'])
@@ -1722,35 +1929,35 @@
     X_log = np.log(X).reshape(-1, 1)
     logging.info("KMedoids clustering with {} component".format(n))
     if n > 1: kmedoids = KMedoids(n_clusters=n,metric=metric,method=method,init=init,max_iter=em_iter,random_state=seed).fit(X_log)
     else: kmedoids = KMedoids(n_clusters=n,metric=metric,method='alternate',init=init,max_iter=em_iter,random_state=seed).fit(X_log)
     cluster_centers = kmedoids.cluster_centers_
     centers = info_centers(cluster_centers)
     labels = kmedoids.labels_
-    plot_segment_kmedoids(labels,X,outdir,bin_width,n,regime=guide)
+    plot_segment_kmedoids(labels,X,outdir,bin_width,n,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim)
     #labels = kmedoids.predict(X_log)
     Losses,labels_plot = [],[]
     for p in range(1,n_kmedoids+1):
         if p == 1: kmedoids = KMedoids(n_clusters=p,metric=metric,method='alternate',init=init,max_iter=em_iter,random_state=seed).fit(X_log)
         else: kmedoids = KMedoids(n_clusters=p,metric=metric,method=method,init=init,max_iter=em_iter,random_state=seed).fit(X_log)
         Cluster_centers = kmedoids.cluster_centers_
         Labels = kmedoids.labels_
         labels_plot.append(Labels)
         loss = Elbow_lossf(X_log,Cluster_centers,Labels)
         Losses.append(loss)
     if n_kmedoids > 0:
         plot_silhouette_score(X_log,2,n_kmedoids+1,labels_plot[1:],outdir,guide+'_Ks','KMedoids')
-        print((len(range(2,n_kmedoids+1)),len(labels_plot[1:])))
+        #print((len(range(2,n_kmedoids+1)),len(labels_plot[1:])))
         significance_test_cluster(X_log,2,n_kmedoids+1,labels_plot[1:])
     plot_Elbow_loss(Losses,outdir,regime=guide)
     #loss = Elbow_lossf(X_log,cluster_centers,labels)
     #df_labels = pd.DataFrame(labels,columns=['KMedoids_Cluster'])
     df_c = write_labels(df,df_withindex,labels,outdir,n,regime=guide)
-    plot_kmedoids(boots,kdemethod,df_c,outdir,n,bin_width,bins=50,weighted=weighted,title="",plot=plot,alpha=0.5,regime=guide)
-    plot_kmedoids_kde(boots,kdemethod,df_c,outdir,n,bin_width,bins=50,weighted=weighted,title="",plot=plot,alpha=0.5,regime=guide)
+    plot_kmedoids(boots,kdemethod,df_c,outdir,n,bin_width,bins=50,weighted=weighted,title="",plot=plot,alpha=0.5,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim)
+    plot_kmedoids_kde(boots,kdemethod,df_c,outdir,n,bin_width,bins=50,weighted=weighted,title="",plot=plot,alpha=0.5,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim)
     return df
 
 def retreive95CI(family,ksdf_filtered,outdir,lower,upper):
     df = pd.read_csv(family,header=0,index_col=0,sep='\t')
     cs = list(df.columns)
     focus_ids = [i for i in cs if i.endswith('_ap1') or i.endswith('_ap2')]
     df['ap12'] = ["__".join(sorted([x,y])) for x,y in zip(list(df[focus_ids[0]]),list(df[focus_ids[1]]))]
```

### Comparing `wgd-2.0.19/wgd/postplot.py` & `wgd-2.0.20/wgd/postplot.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.19/wgd/syn.py` & `wgd-2.0.20/wgd/syn.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,41 @@
 from wgd.peak import formatv2
 from wgd.viz import apply_filters
 
 gff_header = ["gene", "scaffold", "start", "orientation"] 
 
 # we construct first a table with each row a gene containing it's family,
 # scaffold, location and orientation
-def make_gene_table(gffs, families, feature, attribute):
+def make_gene_table(gffs, families, feature, attribute, additionalgffinfo):
     """
     Construct a table from a bunch of gff files and gene families such that all
     information for synteny and co-linearity related analyses is in one place.
     
     :param gffs: a list of GFF *file names*
     :param families: a pandas data frame with the gene families
     :param feature: feature tag for the GFF files
     :param attribute: attribute tag for parsing out gene IDs from last column
     
     Note: currently we assume the same attribute/feature is required for all
     GFF files, and the burden is on the user to make sure this is the case. We
     may wish, for flexibility, to allow a list of feature/attribute arguments
     in the future, one for each GFF file.
     """
-    gfftables = [gff2table(gff, feature, attribute) for gff in gffs]
+    if not (additionalgffinfo is None) and len(additionalgffinfo) > 0:
+        # ignore the info in the original feature and attribute
+        features, attributes = [i.split(";")[0].strip() for i in additionalgffinfo], [i.split(";")[1].strip() for i in additionalgffinfo]
+        if len(features) != len(attributes):
+            logging.error("Please give the additional feature and attribute info of gff in the format of (feature;attribute)")
+            exit(1)
+        if len(features) != len(gffs):
+            logging.error("Please give the same number and order of gff files and its associated additional feature and attribute info")
+            exit(1)
+        gfftables = [gff2table(gff, f, a) for gff,f,a in zip(gffs,features,attributes)]
+    else:
+        gfftables = [gff2table(gff, feature, attribute) for gff in gffs]
     familytable = gene2family(families)
     df = pd.concat(gfftables)
     df = familytable.join(df)
     return df
 
 def getattr(s, attribute):
     for x in s.split(";"):
```

### Comparing `wgd-2.0.19/wgd/utils.py` & `wgd-2.0.20/wgd/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,63 @@
 import numpy as np
 import json
 import subprocess
 from progressbar import ProgressBar
 from numpy import mean, std
 from scipy.spatial.distance import cdist
 
+def formatv2(ksdf):
+    if "Ks" in ksdf.columns: ksdf = ksdf.rename(columns={"Ks":"dS"})
+    if "Ka" in ksdf.columns: ksdf = ksdf.rename(columns={"Ka":"dN"})
+    if "Omega" in ksdf.columns: ksdf = ksdf.rename(columns={"Omega":"dN/dS"})
+    if "Family" in ksdf.columns: ksdf = ksdf.rename(columns={"Family":"family"})
+    if "Node" in ksdf.columns: ksdf = ksdf.rename(columns={"Node":"node"})
+    if "AlignmentIdentity" in ksdf.columns: ksdf = ksdf.rename(columns={"AlignmentIdentity":"alignmentidentity"})
+    if "AlignmentLength" in ksdf.columns: ksdf = ksdf.rename(columns={"AlignmentLength":"alignmentlength"})
+    if "AlignmentCoverage" in ksdf.columns: ksdf = ksdf.rename(columns={"AlignmentCoverage":"alignmentcoverage"})
+    if "Paralog1" in ksdf.columns: ksdf = ksdf.rename(columns={"Paralog1":"gene1"})
+    if "Paralog2" in ksdf.columns: ksdf = ksdf.rename(columns={"Paralog2":"gene2"})
+    if "WeightOutliersIncluded" in ksdf.columns: ksdf = ksdf.drop(columns=["WeightOutliersIncluded"])
+    if "WeightOutliersExcluded" in ksdf.columns: ksdf = ksdf.drop(columns=["WeightOutliersExcluded"])
+    if "weightoutlierexcluded" not in ksdf.columns: weight_inc = get_outlierincluded(ksdf)
+    if "weightoutlierincluded" not in ksdf.columns:
+        weight_exc = get_outlierexcluded(ksdf,cutoff = 5)
+        ksdf = ksdf.join(weight_inc).join(weight_exc)
+    if "node_averaged_dS_outlierincluded" not in ksdf.columns:
+        node_averaged_dS_inc = get_nodeaverged_dS_outlierincluded(ksdf)
+    if "node_averaged_dS_outlierexcluded" not in ksdf.columns:
+        node_averaged_dS_exc = get_nodeaverged_dS_outlierexcluded(ksdf,cutoff = 5)
+        ksdf = ksdf.reset_index().merge(node_averaged_dS_inc,on = ['family', 'node'])
+        ksdf = ksdf.merge(node_averaged_dS_exc,on = ['family', 'node'],how = 'left')
+    if "index" in ksdf.columns: ksdf = ksdf.set_index('index')
+    ksdf.index.name = 'pair'
+    return ksdf
+
+def get_outlierexcluded(df,cutoff = 5):
+    df = df[df['dS']<cutoff]
+    weight_exc = 1/df.groupby(['family', 'node'])['dS'].transform('count')
+    weight_exc = weight_exc.to_frame(name='weightoutlierexcluded')
+    return weight_exc
+
+def get_outlierincluded(df):
+    weight_inc = 1/df.groupby(['family', 'node'])['dS'].transform('count')
+    weight_inc = weight_inc.to_frame(name='weightoutlierincluded')
+    return weight_inc
+
+def get_nodeaverged_dS_outlierincluded(df):
+    node_averaged_dS_inc = df.groupby(["family", "node"])["dS"].mean()
+    node_averaged_dS_inc = node_averaged_dS_inc.to_frame(name='node_averaged_dS_outlierincluded')
+    return node_averaged_dS_inc
+
+def get_nodeaverged_dS_outlierexcluded(df,cutoff = 5):
+    df = df[df['dS']<cutoff]
+    node_averaged_dS_exc = df.groupby(["family", "node"])["dS"].mean()
+    node_averaged_dS_exc = node_averaged_dS_exc.to_frame(name='node_averaged_dS_outlierexcluded')
+    return node_averaged_dS_exc
+
 def can_i_run_software(software):
     """
     Test if external software is executable
 
     :param software: list or string of executable(s)
     :return: 1 (failure) or 0 (success)
     """
```

### Comparing `wgd-2.0.19/wgd/viz.py` & `wgd-2.0.20/wgd/viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import matplotlib.patches as patches
 from matplotlib.pyplot import cm
 from matplotlib.cm import ScalarMappable
 from scipy import stats,interpolate,signal
 from io import StringIO
 from Bio import Phylo
 from sklearn import mixture
+from wgd.utils import formatv2
 
 def node_averages(df):
     # note that this returns a df with fewer rows, i.e. one for every
     # node in the gene family trees.
     return df.groupby(["family", "node"])["dS"].mean()
 
 def node_weights(df):
@@ -315,23 +316,24 @@
     models, aic, bic, besta, bestb, N = fit_gmm(aic_bic_fplot, X_log, 2352890, components[0], components[1], em_iter=200, n_init=200)
     means,covariances,weights = besta.means_,besta.covariances_,besta.weights_
     CHF = get_totalH(Hs)
     scaling = CHF*0.1
     cs = cm.tab20b(np.linspace(0, 1, len(weights)))
     for num in range(len(weights)):
         mean,std,weight = means[num][0],np.sqrt(covariances[num][0][0]),weights[num]
-        ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=cs[num], ls='-', lw=1, alpha=0.8, label='Anchor Ks component {} mode {:.2f}'.format(num+1,np.exp(mean - std**2)))
+        ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=cs[num], ls='--', lw=1, alpha=0.8, label='Anchor '+'$K_\mathrm{S}$ '+'component {} (mode {:.2f})'.format(num+1,np.exp(mean - std**2)))
     return ax
 
-def addelmm(ax,df,max_EM_iterations=200,num_EM_initializations=200,peak_threshold=0.1,rel_height=0.4):
+def addelmm(ax,df,max_EM_iterations=200,num_EM_initializations=200,peak_threshold=0.1,rel_height=0.4, na = False):
     df = df.dropna(subset=['dS','weightoutlierexcluded'])
     df = df.loc[(df['dS']>0) & (df['dS']<5),:]
     ks_or = np.array(df['dS'])
     w = np.array(df['weightoutlierexcluded'])
-    deconvoluted_data = get_deconvoluted_data(ks_or,w)
+    if na: deconvoluted_data = ks_or.copy()
+    else: deconvoluted_data = get_deconvoluted_data(ks_or,w)
     hist_property = np.histogram(ks_or, weights=w, bins=50, density=True)
     init_lambd = hist_property[0][0]
     ks = np.log(ks_or)
     max_ks,min_ks = ks.max(),ks.min()
     ks_refed,cutoff,w_refed = reflect_logks(ks,w)
     kde = stats.gaussian_kde(ks_refed, bw_method="scott", weights=w_refed)
     bw_modifier = 0.4
@@ -469,59 +471,131 @@
     colors = ["b", "r", "c", "m", "k"][:len(final_stdevs)-1] + ["y"]
     for comp, color in zip(lognormals_sorted_by_peak, colors):
         ax.plot(x_points_strictly_positive,scaling*final_weights[comp+1]*stats.lognorm.pdf(x_points_strictly_positive, scale=np.exp(final_means[comp]),s=final_stdevs[comp]), c=color, ls='-', lw=1.5, alpha=0.8, label=f'Lognormal {letter_dict[comp]} optimized (mode {lognormal_peaks[comp]})')
         total_pdf = total_pdf + final_weights[comp+1]*stats.lognorm.pdf(x_points_strictly_positive,scale=np.exp(final_means[comp]),s=final_stdevs[comp])
     ax.plot(x_points_strictly_positive, scaling*total_pdf, "k-", lw=1.5, label=f'Exp-lognormal mixture model')
     return ax
 
-def multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title='',ylabel='',viz=False,plotkde=False,reweight=True,sptree=None,ksd=False,ap=None,extraparanomeks=None,plotapgmm=False,components=(1,4),plotelmm=False,max_EM_iterations=200,num_EM_initializations=200,peak_threshold=0.1,rel_height=0.4):
+def multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title='',ylabel='',viz=False,plotkde=False,reweight=True,sptree=None,ksd=False,ap=None,extraparanomeks=None,plotapgmm=False,components=(1,4),plotelmm=False,max_EM_iterations=200,num_EM_initializations=200,peak_threshold=0.1,rel_height=0.4, na = False):
+    if na:
+        df = df.drop_duplicates(subset=['family','node'])
+        df = df.loc[:,['node_averaged_dS_outlierexcluded','gene1','gene2']].copy().rename(columns={'node_averaged_dS_outlierexcluded':'dS'})
+        df['weightoutlierexcluded'] = 1
+        logging.info("Implementing node-averaged Ks analysis")
+    else: logging.info("Implementing node-weighted Ks analysis")
+    df = df.dropna(subset=['dS','weightoutlierexcluded'])
+    df = df.loc[(df['dS']>0) & (df['dS']<5),:]
+    df_para = None
     if extraparanomeks != None:
         df_para = pd.read_csv(extraparanomeks,header=0,index_col=0,sep='\t')
+        df_para = formatv2(df_para)
         df_para = apply_filters(df_para, [("dS", 0., 5.)])
         df_para["family"] = df_para["family"].apply(lambda x:"ExtraParalog_"+x)
         df = pd.concat([df,df_para])
     # I add this dropduplicates to prevent the same paralogous pair from occuring twice and also use preferentially paranome
     df = df[~df.index.duplicated(keep='last')]
     if not ksd: spgenemap = getgsmap(gsmap)
     else: spgenemap = gsmap
     if not viz: writespgenemap(spgenemap,outdir)
     df_perspair,allspair,paralog_pair,corrected_ks_spair,Outgroup_spnames = getspair_ks(spair,df,spgenemap,reweight,onlyrootout,sptree=sptree)
-    if len(paralog_pair) != 0:
-        fnames = os.path.join(outdir,'{}_Corrected.ksd.svg'.format(paralog_pair[0].split('__')[0]))
-        fnamep = os.path.join(outdir,'{}_Corrected.ksd.pdf'.format(paralog_pair[0].split('__')[0]))
+    if len(paralog_pair) == 1:
+        if len(df_perspair) == 1:
+            if na:
+                fnames = os.path.join(outdir,'{}.ksd.averaged.svg'.format(paralog_pair[0].split('__')[0]))
+                fnamep = os.path.join(outdir,'{}.ksd.averaged.pdf'.format(paralog_pair[0].split('__')[0]))
+            else:
+                fnames = os.path.join(outdir,'{}.ksd.weighted.svg'.format(paralog_pair[0].split('__')[0]))
+                fnamep = os.path.join(outdir,'{}.ksd.weighted.pdf'.format(paralog_pair[0].split('__')[0]))
+        else:
+            if na:
+                fnames = os.path.join(outdir,'{}_Corrected.ksd.averaged.svg'.format(paralog_pair[0].split('__')[0]))
+                fnamep = os.path.join(outdir,'{}_Corrected.ksd.averaged.pdf'.format(paralog_pair[0].split('__')[0]))
+            else:
+                fnames = os.path.join(outdir,'{}_Corrected.ksd.weighted.svg'.format(paralog_pair[0].split('__')[0]))
+                fnamep = os.path.join(outdir,'{}_Corrected.ksd.weighted.pdf'.format(paralog_pair[0].split('__')[0]))
+    elif len(paralog_pair) > 1:
+        if na:
+            fnames = os.path.join(outdir,'Mixed_Paralogues_Orthologues.ksd.averaged.svg')
+            fnamep = os.path.join(outdir,'Mixed_Paralogues_Orthologues.ksd.averaged.pdf')
+        else:
+            fnames = os.path.join(outdir,'Mixed_Paralogues_Orthologues.ksd.weighted.svg')
+            fnamep = os.path.join(outdir,'Mixed_Paralogues_Orthologues.ksd.weighted.pdf')
     else:
-        fnames = os.path.join(outdir,'Raw_Orthologues.ksd.svg')
-        fnamep = os.path.join(outdir,'Raw_Orthologues.ksd.pdf')
+        if na:
+            fnames = os.path.join(outdir,'Raw_Orthologues.ksd.averaged.svg')
+            fnamep = os.path.join(outdir,'Raw_Orthologues.ksd.averaged.pdf')
+        else:
+            fnames = os.path.join(outdir,'Raw_Orthologues.ksd.weighted.svg')
+            fnamep = os.path.join(outdir,'Raw_Orthologues.ksd.weighted.pdf')
     cs = cm.viridis(np.linspace(0, 1, len(allspair)))
     keys = ["dS", "dS", "dN", "dN/dS"]
     np.seterr(divide='ignore')
     funs = [lambda x: x, np.log10, np.log10, np.log10]
     #fig, axs = plt.subplots(2, 2)
     fig, ax = plt.subplots()
     #df_pers = [df_perspair[i] for i in allspair]
     bins = 50
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     if reweight: logging.info('Recalculating the weights per species pair')
-    else: logging.info('De-redundancy via the weights from overall species')
+    elif not na: logging.info('De-redundancy via the weights from overall species')
     if plotkde: logging.info('Plotting kde curve over histogram')
     else: logging.info('Plotting histogram without kde curve')
-    #np.warnings.filterwarnings('ignore', category=np.VisibleDeprecationWarning)
+    drawtime = 0
+    if plotelmm:
+        if not (df_para is None):
+            logging.info("ELMM analysis on extra paralogous Ks")
+            ax = addelmm(ax,df_para,max_EM_iterations=max_EM_iterations,num_EM_initializations=num_EM_initializations,peak_threshold=peak_threshold,rel_height=rel_height,na=na)
+            drawtime = drawtime + 1
+    Hs_maxs,y_lim_beforekdes = [],[]
     for i,item in enumerate(df_perspair.items()):
         pair,df_per = item[0],item[1]
+        df_per = df_per.copy()
         #for ax, k, f in zip(axs.flatten(), keys, funs):
-        w = reweighted(df_per) if reweight else df_per['weightoutlierexcluded']
+        if reweight:
+            w = reweighted(df_per)
+            df_per['weightoutlierexcluded'] = w
+        else:
+            w = df_per['weightoutlierexcluded']
         x = df_per['dS']
         y = x[np.isfinite(x)]
         w = w[np.isfinite(x)]
         if pair in paralog_pair:
-            Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, color=cs[i], alpha=0.8, rwidth=0.8,label=pair,edgecolor='black',linewidth=0.8)
-            if plotelmm: ax = addelmm(ax,df_para,max_EM_iterations=max_EM_iterations,num_EM_initializations=num_EM_initializations,peak_threshold=peak_threshold,rel_height=rel_height)
+            if len(df_perspair) == 1:
+                Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, color='gray', alpha=1, rwidth=0.8,label='Whole paranome')
+            else:
+                Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, color=cs[i], alpha=0.8, rwidth=0.8,label=pair,edgecolor='black',linewidth=0.8)
+            y_lim_beforekde = ax.get_ylim()[1]
+            y_lim_beforekdes.append(y_lim_beforekde)
+            Hs_maxs.append(max(Hs))
+            if not (df_para is None):
+                continue
+            if not plotelmm:
+                if plotkde:
+                    kde = stats.gaussian_kde(y,weights=w,bw_method='scott')
+                    kde_y = kde(kde_x)
+                    CHF = get_totalH(Hs)
+                    scaling = CHF*0.1
+                    ax.plot(kde_x, kde_y*scaling, color=cs[i],alpha=0.4, ls = '-', label = "{}".format(pair))
+            if plotelmm and drawtime < 1:
+                drawtime = drawtime + 1
+                logging.info("ELMM analysis on paralogous Ks of {}".format(pair.split("__")[0]))
+                ax = addelmm(ax,df_per,max_EM_iterations=max_EM_iterations,num_EM_initializations=num_EM_initializations,peak_threshold=peak_threshold,rel_height=rel_height,na=na)
+                continue
+            if plotkde:
+                kde = stats.gaussian_kde(y,weights=w,bw_method='scott')
+                kde_y = kde(kde_x)
+                CHF = get_totalH(Hs)
+                scaling = CHF*0.1
+                ax.plot(kde_x, kde_y*scaling, color=cs[i],alpha=0.4, ls = '-', label = "{}".format(pair))
         else:
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, color=cs[i], alpha=0.5, rwidth=0.8,label=pair)
+            y_lim_beforekde = ax.get_ylim()[1]
+            y_lim_beforekdes.append(y_lim_beforekde)
+            Hs_maxs.append(max(Hs))
         if corrected_ks_spair != None:
             if pair in corrected_ks_spair.keys():
                 #since paralogous genes and orthologous genes between focus and outgroup speices have no corrected Ks data
                 ax.axvline(x = corrected_ks_spair[pair], color = cs[i], alpha = 0.8, ls = '-.', lw = 1,label = 'Corrected mode {:.2f} of {}'.format(corrected_ks_spair[pair],pair))
                 logging.info('The corrected mode of species pair {} is {:.2f}'.format(pair,corrected_ks_spair[pair]))
         if pair not in paralog_pair:
             kde = stats.gaussian_kde(y,weights=w,bw_method=0.1)
@@ -530,32 +604,48 @@
             logging.info('The mode of species pair {} is {:.2f}'.format(pair,mode))
             CHF = get_totalH(Hs)
             scaling = CHF*0.1
             if plotkde: ax.plot(kde_x, kde_y*scaling, color=cs[i],alpha=0.4, ls = '--')
             ax.axvline(x = mode, color = cs[i], alpha = 0.8, ls = ':', lw = 1,label = 'Original mode {:.2f} of {}'.format(mode,pair))
             if corrected_ks_spair != None:
                 if pair in corrected_ks_spair.keys():
-                    ax.quiver(mode,maxim*scale, corrected_ks_spair[pair]-mode, 0, angles='xy', scale_units='xy', scale=1,color=cs[i],width=0.005,headwidth=2,headlength=2,headaxislength=2)
+                    ax.quiver(mode,maxim*scaling, corrected_ks_spair[pair]-mode, 0, angles='xy', scale_units='xy', scale=1,color=cs[i],width=0.005,headwidth=2,headlength=2,headaxislength=2)
     if ap != None:
         df_ap = pd.read_csv(ap,header=0,index_col=0,sep='\t')
         df_ap.loc[:,"pair"] = df_ap[["gene_x", "gene_y"]].apply(lambda x: "__".join(sorted([x[0], x[1]])), axis=1)
         df_working = df_ap.set_index('pair').join(df).dropna(subset=['dS','weightoutlierexcluded'])
         w = reweighted(df_working) if reweight else df_working['weightoutlierexcluded']
         x = df_working['dS']
         y = x[np.isfinite(x)]
         w = w[np.isfinite(x)]
-        Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, fill=False, rwidth=0.8,label='Anchor pairs',linewidth=0,hatch = '////////',edgecolor='black')
+        if len(df_perspair) == 1:
+            Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, color='g', rwidth=0.8,label='Anchor pairs')
+        else:
+            Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, fill=False, rwidth=0.8,label='Anchor pairs',linewidth=0,hatch = '////////',edgecolor='black')
+        Hs_maxs.append(max(Hs))
+        y_lim_beforekde = ax.get_ylim()[1]
+        y_lim_beforekdes.append(y_lim_beforekde)
         if plotapgmm: ax = addapgmm(ax,y,w,components,outdir,Hs)
     ax.set_xlabel(_labels["dS"])
+    safe_max = max([max(y_lim_beforekdes),max(Hs_maxs)])
+    ax.set_ylim(0, safe_max)
     #ax.legend(loc=1,fontsize=5,bbox_to_anchor=(0.95, 0.95),frameon=False)
-    ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
-    ax.set_ylabel(ylabel)
+    if len(df_perspair) == 1 and len(paralog_pair) == 1:
+        ax.legend(loc=1,fontsize=7,frameon=False)
+    else:
+        ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
+    if len(df_perspair) == 1 and len(paralog_pair) == 1:
+        ax.set_ylabel('Number of retained duplicates')
+    else:
+        ax.set_ylabel(ylabel)
     ax.set_xticks([0,1,2,3,4,5])
     sns.despine(offset=1)
-    if len(paralog_pair) !=0: title = 'Corrected $K_\mathrm{S}$ ' + 'distribution of {}'.format(paralog_pair[0].split('__')[0])
+    if len(df_perspair) == 1:
+        title = '$K_\mathrm{S}$ ' + 'distribution of {}'.format(paralog_pair[0].split('__')[0])
+    elif len(paralog_pair) !=0: title = 'Corrected $K_\mathrm{S}$ ' + 'distribution of {}'.format(paralog_pair[0].split('__')[0])
     else: title = 'Orthologous $K_\mathrm{S}$ distribution'
     ax.set_title(title)
     #fig.tight_layout()
     #plt.subplots_adjust(top=0.85)
     fig.savefig(fnames,bbox_inches='tight')
     fig.savefig(fnamep,bbox_inches='tight')
     plt.close()
@@ -867,18 +957,23 @@
     sum_comp_perpoint = sum(products)
     log_sum_comp_perpoint = np.log(sum_comp_perpoint)
     fit_loglikelihood = sum(log_sum_comp_perpoint)
     posteriors = [products[i] / sum_comp_perpoint for i in range(num_comp)]
     return fit_loglikelihood, posteriors
 
 def m_step(num_comp, ks, posteriors):
+    # The mean of Exponential distribution is 1/lambda
     new_lambda = sum(posteriors[0]) / sum(posteriors[0] * ks)
     points_per_k = [sum(posteriors[i]) for i in range(num_comp)]
     # here the new weights is overall weight instead of weight per datapoint
-    new_weights = [points_per_k[i]/len(ks) for i in range(num_comp)]
+    new_weights = [round(points_per_k[i]/len(ks),2) for i in range(num_comp)]
+    for indice in range(len(points_per_k)):
+        if not points_per_k[indice]>0:
+            logging.info("Found component weight as zero")
+            points_per_k[indice] = 1e-6
     new_means = [sum(posteriors[i+1] * np.log(ks)) / points_per_k[i+1] for i in range(num_comp-1)]
     new_stdevs = [np.sqrt(sum(posteriors[i+1]*pow(np.log(ks)-new_means[i],2))/points_per_k[i+1]) for i in range(num_comp-1)]
     return new_means, new_stdevs, new_weights, new_lambda
 
 def EM_step(num_comp,data,means,stds,lambd,weights,max_EM_iterations=200,max_num_comp = 5, reduced_gaussians_flag=None):
     #data = np.array(deconvoluted_data).reshape(-1, 1)
     convergence,ks = False,data[data>0]
@@ -1037,14 +1132,15 @@
     plt.subplots_adjust(top=0.85)  # prevent suptitle from overlapping
     return fig
 
 def syntenic_depth_plot(segprofile):
     cols = segprofile.columns
     n = len(cols)
     fig, axs = plt.subplots(1, int(n + n*(n-1)/2))
+    fig.set_size_inches(5*int(n + n*(n-1)/2), 10)
     if n == 1:
         axs = [axs]  # HACK
     k = 0
     for i in range(n):
         for j in range(i, n):
             pairs, counts = dupratios(segprofile[cols[i]], segprofile[cols[j]])
             ax = axs[k]
@@ -1056,15 +1152,16 @@
             k += 1
     for ax in axs:
         ymn, ymx = ax.get_ylim()
         ax.set_ylim(-0.5, ymx)
         #ax.set_xlabel("# segments")
     #axs[0].set_ylabel("A:B ratio")
     fig.suptitle('Collinear ratio', x=0.5, y=1.02, ha='center', va='top')
-    plt.figtext(0.5, 0.02, 'Number of segments', ha='center', va='top')
+    #plt.figtext(0.5, 0.02, 'Number of segments', ha='center', va='top')
+    plt.figtext(0.5, 0.01, 'Number of segments', ha='center', va='top')
     sns.despine(trim=False, offset=3)
     plt.tight_layout()
     return fig
 
 
 def dupratios(col1, col2, by="first"):
     d = {}
@@ -1780,15 +1877,111 @@
     else:
         return np.median(Ks)
 
 def getpairks(pair,ksdf):
     Ks_dict = {pair:ks for pair,ks in zip(ksdf.index,ksdf['dS'])}
     return Ks_dict.get(pair,None)
 
-def plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False,dotsize=0.8,apalpha=1, hoalpha=0.1):
+def plotdp_igoverall(removed_scfa,ax,ordered_genes_perchrom_allsp,sp_list,table,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False,dotsize=0.8,apalpha=1, hoalpha=0.1, showrealtick=False, las = 5):
+    dfs = {sp:ordered_genes_perchrom_allsp[sp].copy().drop(removed_scfa[sp],axis=1).set_index('Coordinates') for sp in sp_list}
+    leng_info = {sp:{} for sp in sp_list}
+    gene_list = {gene:li for gene,li in zip(table.index,table['scaffold'])}
+    for sp in sp_list:
+        for scfa in dfs[sp].columns:
+            leng_info[sp][scfa] = len(dfs[sp][scfa].dropna())
+    sorted_labels, sorted_lengs = [],[]
+    tick_strip = []
+    for sp in sp_list:
+        sorted_leng = [i[1] for i in sorted(leng_info[sp].items(),key=lambda x: x[1],reverse=True)]
+        tick_strip.append(sum(sorted_leng))
+        sorted_lengs = sorted_lengs + sorted_leng
+        sorted_label = [sp[:3]+'_'+str(i[0]) for i in sorted(leng_info[sp].items(),key=lambda x: x[1],reverse=True)]
+        sorted_labels = sorted_labels + sorted_label
+    tick = list(np.cumsum(sorted_lengs))
+    tick_strip = list(np.cumsum(tick_strip))
+    tick_addable = [0] + tick[:-1]
+    tick_addable_dict = {scfa:scfastart for scfa,scfastart in zip(sorted_labels,tick_addable)}
+    xs,ys,co,xs_ap,ys_ap,co_ap,Ks_ages = [],[],[],[],[],[],[]
+    if showks: Ks_dict = {pair:ks for pair,ks in zip(ksdf.index,ksdf['dS'])}
+    for fam, df_tmp in list(table.groupby('family')):
+        all_cooris,allgenes = [],[]
+        for sp in set(df_tmp['species']):
+            if len(df_tmp[df_tmp['species']==sp]) >= maxsize or len(df_tmp[df_tmp['species']==sp]) == 0:
+                continue
+            df_tmp_sp = df_tmp[df_tmp['species']==sp]
+            for g in df_tmp_sp.index:
+                allgenes.append(g)
+                g_coori = gene_orders[g] + tick_addable_dict[sp[:3]+"_"+gene_list[g]]
+                all_cooris.append(g_coori)
+        for (gx,gy), (x,y) in zip(itertools.product(allgenes,allgenes),itertools.product(all_cooris,all_cooris)):
+            if gx == gy:
+                continue
+            if showks:
+                if not (ksdf is None):
+                    ks = Ks_dict.get("__".join(sorted([gx,gy])),None)
+                    if ks is None:
+                        continue
+                    Ks_ages.append(ks)
+            xs.append(x)
+            ys.append(y)
+            if showks: co.append(ks)
+            if not (anchor is None):
+                if "__".join(sorted([gx,gy])) in anchor.index:
+                    xs_ap.append(x)
+                    ys_ap.append(y)
+                    if showks: co_ap.append(ks)
+    if showks:
+        if not (ksdf is None):
+            norm = matplotlib.colors.Normalize(vmin=np.min(Ks_ages), vmax=np.max(Ks_ages))
+            c_m = matplotlib.cm.rainbow
+            s_m = ScalarMappable(cmap=c_m, norm=norm)
+            s_m.set_array([])
+    if not showks:
+        ax.scatter(xs, ys, s=dotsize, color = 'k', alpha=hoalpha)
+        ax.scatter(xs_ap, ys_ap, s=dotsize, color = 'r', alpha=apalpha)
+    else:
+        ax.scatter(xs, ys, s=dotsize, color=[c_m(norm(c)) for c in co], alpha=hoalpha)
+        ax.scatter(xs_ap, ys_ap, s=dotsize, color=[c_m(norm(c)) for c in co_ap], alpha=apalpha)
+    xlim = ylim = tick[-1]
+    ax.set_xlim(-400, xlim)
+    ax.set_ylim(-400, ylim)
+    #ax.vlines(tick, ymin=0, ymax=ylim, alpha=0.8, color="k", linewidths=0.5)
+    #ax.hlines(tick, xmin=0, xmax=xlim, alpha=0.8, color="k", linewidths=0.5)
+    ax.set_xticks(tick)
+    ax.set_xticklabels(sorted_labels,rotation=45)
+    ax.set_yticks(tick)
+    ax.set_yticklabels(sorted_labels,rotation=45)
+    ax.spines['bottom'].set_visible(False)
+    ax.spines['left'].set_visible(False)
+    ax.grid(True, linestyle='-', linewidth=0.5, color='gray')
+    ax.plot([0,xlim], [0,ylim], color='k', alpha=0.8,linewidth=0.5)
+    cs = cm.viridis(np.linspace(0, 1, len(tick_strip)))
+    for indice,s,c in zip(range(len(tick_strip)),tick_strip,cs):
+        if indice == 0: s_add = 0
+        else: s_add = tick_strip[indice-1]
+        ax.axhline(y=s, color='k', linestyle='-',linewidth=1)
+        ax.axvline(x=s, color='k', linestyle='-',linewidth=1)
+        ax.add_patch(Rectangle((-400, 0+s_add), 400, s-s_add, color=c, alpha=1,linewidth=0,zorder = 0))
+        ax.add_patch(Rectangle((0+s_add, -400), s-s_add, 400, color=c, alpha=1,linewidth=0,zorder = 0))
+    #ax.spines['left'].set_visible(False)
+    if showrealtick:
+        ax2 = ax.twinx()
+        ax3 = ax.twiny()
+        ax2.set_yticks(tick)
+        ax2.set_ylabel("{} (genes)".format(spy))
+        ax2.tick_params(axis='y', labelrotation=45)
+        ax3.set_xticks(tick)
+        ax3.set_xlabel("{} (genes)".format(spx))
+        ax3.tick_params(axis='x', labelrotation=45)
+    if showks:
+        if not (ksdf is None): plt.colorbar(s_m, label="$K_\mathrm{S}$", orientation="vertical",fraction=0.03,pad=0.1)
+    ax.tick_params(axis='both', which='major', labelsize=las)
+    return ax
+
+def plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False,dotsize=0.8,apalpha=1, hoalpha=0.1, showrealtick=False, las = 5):
     dfx,dfy = dfx.set_index('Coordinates'),dfy.set_index('Coordinates')
     leng_info_x,leng_info_y = {},{}
     gene_list = {gene:li for gene,li in zip(table.index,table['scaffold'])}
     if spx != spy:
         gene_list = {spx:{},spy:{}}
         for gene,sp,li in zip(table.index,table['species'],table['scaffold']):
             if sp != spx and sp != spy:
@@ -1832,47 +2025,51 @@
             if showks: co.append(ks)
             if not (anchor is None):
                 if "__".join(sorted([ggx,ggy])) in anchor.index:
                     xs_ap.append(x)
                     ys_ap.append(y)
                     if showks: co_ap.append(ks)
     if showks:
-        if not (ksdf is None):
+        if len(Ks_ages) !=0 and not (ksdf is None):
             norm = matplotlib.colors.Normalize(vmin=np.min(Ks_ages), vmax=np.max(Ks_ages))
             c_m = matplotlib.cm.rainbow
             s_m = ScalarMappable(cmap=c_m, norm=norm)
             s_m.set_array([])
     if not showks:
         ax.scatter(xs, ys, s=dotsize, color = 'k', alpha=hoalpha)
         ax.scatter(xs_ap, ys_ap, s=dotsize, color = 'r', alpha=apalpha)
-    else:
+    elif len(Ks_ages) !=0:
         ax.scatter(xs, ys, s=dotsize, color=[c_m(norm(c)) for c in co], alpha=hoalpha)
         ax.scatter(xs_ap, ys_ap, s=dotsize, color=[c_m(norm(c)) for c in co_ap], alpha=apalpha)
     #ax.scatter(xs_ap, ys_ap, s=0.4, alpha=0.5)
     xlim,ylim = xtick[-1],ytick[-1]
     ax.set_xlim(0, xlim)
     ax.set_ylim(0, ylim)
-    ax.vlines(xtick, ymin=0, ymax=ylim, alpha=0.8, color="k")
-    ax.hlines(ytick, xmin=0, xmax=xlim, alpha=0.8, color="k")
+    if spx == spy: ax.plot([0,xlim], [0,ylim], color='k', alpha=0.8,linewidth=0.5)
+    #ax.vlines(xtick, ymin=0, ymax=ylim, alpha=0.8, color="k")
+    #ax.hlines(ytick, xmin=0, xmax=xlim, alpha=0.8, color="k")
+    ax.grid(True, linestyle='-', linewidth=0.5, color='gray')
     ax.set_xlabel("{}".format(spx))
     ax.set_ylabel("{}".format(spy))
     ax.set_xticks(xtick)
     ax.set_xticklabels(sorted_labels_x,rotation=45)
     ax.set_yticks(ytick)
     ax.set_yticklabels(sorted_labels_y,rotation=45)
-    ax2 = ax.twinx()
-    ax3 = ax.twiny()
-    ax2.set_yticks(ytick)
-    ax2.set_ylabel("{} (genes)".format(spy))
-    ax2.tick_params(axis='y', labelrotation=45)
-    ax3.set_xticks(xtick)
-    ax3.set_xlabel("{} (genes)".format(spx))
-    ax3.tick_params(axis='x', labelrotation=45)
+    if showrealtick:
+        ax2 = ax.twinx()
+        ax3 = ax.twiny()
+        ax2.set_yticks(ytick)
+        ax2.set_ylabel("{} (genes)".format(spy))
+        ax2.tick_params(axis='y', labelrotation=45)
+        ax3.set_xticks(xtick)
+        ax3.set_xlabel("{} (genes)".format(spx))
+        ax3.tick_params(axis='x', labelrotation=45)
     if showks:
-        if not (ksdf is None): plt.colorbar(s_m, label="$K_\mathrm{S}$", orientation="vertical",fraction=0.03,pad=0.1)
+        if len(Ks_ages)!=0 and not (ksdf is None): plt.colorbar(s_m, label="$K_\mathrm{S}$", orientation="vertical",fraction=0.03,pad=0.1)
+    ax.tick_params(axis='both', which='major', labelsize=las)
     return ax
 
 def plotbb_dpug(ax,dfx,dfy,spx,spy,segs,mingenenum,mp,gene_genome,ksdf=None):
     dfx,dfy = dfx.set_index('Coordinates'),dfy.set_index('Coordinates')
     leng_info_x,leng_info_y = {},{}
     for scfa in dfx.columns: leng_info_x[scfa] = len(dfx[scfa].dropna())
     for scfa in dfy.columns: leng_info_y[scfa] = len(dfy[scfa].dropna())
@@ -2063,48 +2260,78 @@
             spx,spy = sp_list[i],sp_list[j]
             fig, ax = plotbackbone_dpug(spx,spy,ordered_genes_perchrom_allsp,removed_scfa,segs,mingenenum,MP,gene_genome,ksdf=ksdf)
             figs[spx + "-vs-" + spy] = fig
     for prefix, fig in figs.items():
         fname = os.path.join(outdir, "{}.line_unit_gene.svg".format(prefix))
         fig.savefig(fname)
 
-def plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False,dotsize=0.8, apalpha=1, hoalpha=0.1):
+def plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False,dotsize=0.8, apalpha=1, hoalpha=0.1, showrealtick= False, las=5):
     fig, ax = plt.subplots(1, 1, figsize=(10,10))
     dfx = ordered_genes_perchrom_allsp[spx].copy().drop(removed_scfa[spx],axis=1)
     dfy = ordered_genes_perchrom_allsp[spy].copy().drop(removed_scfa[spy],axis=1)
-    ax = plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=anchor,ksdf=ksdf,maxsize=maxsize,showks=showks,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha)
+    ax = plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=anchor,ksdf=ksdf,maxsize=maxsize,showks=showks,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha, showrealtick=showrealtick, las=las)
     fig.tight_layout()
     return fig, ax
 
-def dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=None,ksdf=None,maxsize=200,dotsize=0.8, apalpha=1, hoalpha=0.1):
+def plotdotplotingeneoverall(sp_list,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False,dotsize=0.8, apalpha=1, hoalpha=0.1, showrealtick=False, las = 5):
+    fig, ax = plt.subplots(1, 1, figsize=(10,10))
+    ax = plotdp_igoverall(removed_scfa,ax,ordered_genes_perchrom_allsp,sp_list,table,gene_orders,anchor=anchor,ksdf=ksdf,maxsize=maxsize,showks=showks,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha, showrealtick=showrealtick, las = las)
+    fig.tight_layout()
+    return fig, ax
+
+def dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=None,ksdf=None,maxsize=200,dotsize=0.8, apalpha=1, hoalpha=0.1, showrealtick=False, las = 5):
     sp_list = list(ordered_genes_perchrom_allsp.keys())
     gene_list = {gene:li for gene,li in zip(table.index,table['scaffold'])}
     gene_genome = {gene:sp for gene,sp in zip(table.index,table['species'])}
     figs = {}
     logging.info("Making dotplot (in unit of genes)")
     for i in range(len(sp_list)):
         for j in range(i,len(sp_list)):
             spx,spy = sp_list[i],sp_list[j]
             logging.info("{0} vs. {1}".format(spx,spy))
-            fig, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,dotsize=dotsize,apalpha=apalpha, hoalpha=hoalpha)
+            fig, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,dotsize=dotsize,apalpha=apalpha, hoalpha=hoalpha, showrealtick=showrealtick, las = las)
             figs[spx + "-vs-" + spy] = fig
+            plt.close()
             if not (ksdf is None):
-                figks, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,showks=True,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha)
+                figks, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,showks=True,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha, showrealtick=showrealtick, las=las)
                 figs[spx + "-vs-" + spy + "_Ks"] = figks
+                plt.close()
+    for prefix, fig in figs.items():
+        fname = os.path.join(outdir, "{}.dot_unit_gene.svg".format(prefix))
+        fig.savefig(fname)
+        fname = os.path.join(outdir, "{}.dot_unit_gene.png".format(prefix))
+        fig.savefig(fname,dpi=500)
+        fname = os.path.join(outdir, "{}.dot_unit_gene.pdf".format(prefix))
+        fig.savefig(fname)
+    plt.close()
+
+def dotplotingeneoverall(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=None,ksdf=None,maxsize=200,dotsize=0.8, apalpha=1, hoalpha=0.1, showrealtick = False, las = 5):
+    sp_list = list(ordered_genes_perchrom_allsp.keys())
+    gene_list = {gene:li for gene,li in zip(table.index,table['scaffold'])}
+    gene_genome = {gene:sp for gene,sp in zip(table.index,table['species'])}
+    figs = {}
+    logging.info("Making overall dotplot (in unit of genes)")
+    fig, ax = plotdotplotingeneoverall(sp_list,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,dotsize=dotsize,apalpha=apalpha, hoalpha=hoalpha, showrealtick=showrealtick, las = las)
+    figs["Overallspecies"] = fig
+    plt.close()
+    if not (ksdf is None):
+        figks, axks = plotdotplotingeneoverall(sp_list,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,showks=True,dotsize=dotsize,apalpha=apalpha, hoalpha=hoalpha, showrealtick=showrealtick, las = las)
+        figs["Overallspecies_Ks"] = figks
+        plt.close()
     for prefix, fig in figs.items():
         fname = os.path.join(outdir, "{}.dot_unit_gene.svg".format(prefix))
         fig.savefig(fname)
         fname = os.path.join(outdir, "{}.dot_unit_gene.png".format(prefix))
         fig.savefig(fname,dpi=500)
         fname = os.path.join(outdir, "{}.dot_unit_gene.pdf".format(prefix))
         fig.savefig(fname)
     plt.close()
 
 # dot plot stuff
-def all_dotplots(df, segs, multi, minseglen, anchors=None, ancestor=None, Ks=None, dotsize = 0.8, apalpha=1, hoalpha=0.1, **kwargs):
+def all_dotplots(df, segs, multi, minseglen, anchors=None, ancestor=None, Ks=None, dotsize = 0.8, apalpha=1, hoalpha=0.1, showrealtick=False, las = 5, **kwargs):
     """
     Generate dot plots for all pairs of species in `df`, coloring anchor pairs.
     """
     # Note that the Chr ID in gff3 file should not be alleen int or float
     if not (Ks is None):
         ks_dict = {pair:ks for pair,ks in zip(Ks.index,Ks['dS'])}
     gdf = list(df.groupby("species"))
@@ -2120,27 +2347,28 @@
     logging.info("Making dupStack plot")
     for i in range(n):
         for j in range(n):
             spx, dfx = gdf[i]
             spy, dfy = gdf[j]
             logging.info("{} vs. {}".format(spx, spy))
             get_dots(dfx, dfy, segs, multi, minseglen, dupStack = True, **kwargs)
-    logging.info("Making dotplots (in unit of bases) and marco-synteny plots")
+    logging.info("Making dotplots (in unit of bases)")
     getscafflength(n,gdf,**kwargs)
-    if n > 1: get_marco_whole(list(map(lambda x:x[1],gdf)),segs, multi, minseglen,**kwargs)
-    for i in range(n):
-        for j in range(i, n):
-            xxs,yys,ksages,xxs_ap,yys_ap,ksages_ap,Ksages = [],[],[],[],[],[],[]
+    #if n > 1: get_marco_whole(list(map(lambda x:x[1],gdf)),segs, multi, minseglen,**kwargs)
+    for ii in range(n):
+        for jj in range(ii, n):
             fig, ax = plt.subplots(1, 1, figsize=(10,10))
-            ax2 = ax.twinx()
-            ax3 = ax.twiny()
-            spx, dfx = gdf[i]
-            spy, dfy = gdf[j]
+            xxs,yys,ksages,xxs_ap,yys_ap,ksages_ap,Ksages = [],[],[],[],[],[],[]
+            if showrealtick:
+                ax2 = ax.twinx()
+                ax3 = ax.twiny()
+            spx, dfx = gdf[ii]
+            spy, dfy = gdf[jj]
             logging.info("{} vs. {}".format(spx, spy))
-            get_marco(dfx, dfy, segs, multi, minseglen, **kwargs)
+            #get_marco(dfx, dfy, segs, multi, minseglen, **kwargs)
             df, xs, ys, scaffxlabels, scaffylabels, scaffxtick, scaffytick = get_dots(dfx, dfy, segs, multi, minseglen, dupStack = False, **kwargs)
             #print(xs)
             #print(ys)
             #for i,j in zip(df.x,df.y): print((i,j))
             if df is None:  # HACK, in case we're dealing with RBH orthologs...
                 continue
             #for x,y in zip(df.x,df.y): ax.scatter(x, y, s=1, color="k", alpha=0.1)
@@ -2170,57 +2398,68 @@
                         yys_ap.append(y)
             xlim = max(scaffxtick)
             ylim = max(scaffytick)
             ax.set_xlim(0, xlim)
             ax.set_ylim(0, ylim)
             ymin, ymax = ax.get_ylim()
             xmin, xmax = ax.get_xlim()
-            ax.vlines(xs+[xmax], ymin=0, ymax=ylim, alpha=0.8, color="k")
-            ax.hlines(ys+[ymax], xmin=0, xmax=xlim, alpha=0.8, color="k")
+            #ax.vlines(xs+[xmax], ymin=0, ymax=ylim, alpha=0.8, color="k")
+            #ax.hlines(ys+[ymax], xmin=0, xmax=xlim, alpha=0.8, color="k")
+            if spx == spy: ax.plot([0,xlim], [0,ylim], color='k', alpha=0.8,linewidth=0.5)
+            ax.grid(True, linestyle='-', linewidth=0.5, color='gray')
             ax.set_xlabel("{}".format(spx))
             ax.set_ylabel("{}".format(spy))
-            ax2.set_yticklabels(ax.get_yticks() / 1e6)
-            ax3.set_xticklabels(ax.get_xticks() / 1e6)
-            ax.tick_params(axis='both', which='major')
+            if showrealtick:
+                ax2.set_yticklabels(ax.get_yticks() / 1e6)
+                ax3.set_xticklabels(ax.get_xticks() / 1e6)
+            ax.tick_params(axis='both', which='major', labelsize=las)
             ax.set_xticks(scaffxtick)
             ax.set_xticklabels(scaffxlabels,rotation=45)
             ax.set_yticks(scaffytick)
             ax.set_yticklabels(scaffylabels,rotation=45)
-            ax2.set_ylabel("{} (Mb)".format(spy))
-            ax3.set_xlabel("{} (Mb)".format(spx))
+            if showrealtick:
+                ax2.set_ylabel("{} (Mb)".format(spy))
+                ax3.set_xlabel("{} (Mb)".format(spx))
             fig.tight_layout()
             figs[spx + "-vs-" + spy] = fig
-            if not (Ks is None):
+            plt.close()
+            if len(Ksages) != 0 and not (Ks is None):
                 figks, axks = plt.subplots(1, 1, figsize=(10,10))
-                axks2 = axks.twinx()
-                axks3 = axks.twiny()
+                if showrealtick:
+                    axks2 = axks.twinx()
+                    axks3 = axks.twiny()
                 norm = matplotlib.colors.Normalize(vmin=np.min(Ksages), vmax=np.max(Ksages))
                 c_m = matplotlib.cm.rainbow
                 s_m = ScalarMappable(cmap=c_m, norm=norm)
                 s_m.set_array([])
                 axks.scatter(xxs, yys, s=dotsize, color=[c_m(norm(c)) for c in ksages], alpha=hoalpha)
                 axks.scatter(xxs_ap, yys_ap, s=dotsize, color=[c_m(norm(c)) for c in ksages_ap], alpha=apalpha)
                 axks.set_xlim(0, xlim)
                 axks.set_ylim(0, ylim)
-                axks.vlines(xs+[xmax], ymin=0, ymax=ylim, alpha=0.8, color="k")
-                axks.hlines(ys+[ymax], xmin=0, xmax=xlim, alpha=0.8, color="k")
+                #axks.vlines(xs+[xmax], ymin=0, ymax=ylim, alpha=0.8, color="k")
+                #axks.hlines(ys+[ymax], xmin=0, xmax=xlim, alpha=0.8, color="k")
+                axks.grid(True, linestyle='-', linewidth=0.5, color='gray')
                 axks.set_xlabel("{}".format(spx))
                 axks.set_ylabel("{}".format(spy))
-                axks2.set_yticklabels(axks.get_yticks() / 1e6)
-                axks3.set_xticklabels(axks.get_xticks() / 1e6)
-                axks.tick_params(axis='both', which='major')
+                if showrealtick:
+                    axks2.set_yticklabels(axks.get_yticks() / 1e6)
+                    axks3.set_xticklabels(axks.get_xticks() / 1e6)
+                axks.tick_params(axis='both', which='major', labelsize=las)
                 axks.set_xticks(scaffxtick)
                 axks.set_xticklabels(scaffxlabels,rotation=45)
                 axks.set_yticks(scaffytick)
                 axks.set_yticklabels(scaffylabels,rotation=45)
-                axks2.set_ylabel("{} (Mb)".format(spy))
-                axks3.set_xlabel("{} (Mb)".format(spx))
+                if showrealtick:
+                    axks2.set_ylabel("{} (Mb)".format(spy))
+                    axks3.set_xlabel("{} (Mb)".format(spx))
+                if spx == spy: axks.plot([0,xlim], [0,ylim], color='k', alpha=0.8,linewidth=0.5)
                 plt.colorbar(s_m, label="$K_\mathrm{S}$", orientation="vertical",fraction=0.03,pad=0.1)
                 figks.tight_layout()
                 figs[spx + "-vs-" + spy + "_Ks"] = figks
+                plt.close()
     return figs
 
 def filter_by_minlength(genetable,segs,minlen,multi,keepredun,outdir,minseglen):
     gdf,Index_torm,I2,I3,I4 = list(genetable.copy().groupby("species")),[],[],[],[]
     Sf_len_lab_persp = {sp:{} for sp,df in gdf}
     removed_scfa = {}
     for sp,df in gdf:
@@ -2255,28 +2494,37 @@
     if not keepredun:
         Mul_to_rm = list(multi[multi['is_redundant']==-1].loc[:,'id'])
         Segs_to_rm = segs.loc[segs['multiplicon'].isin(Mul_to_rm),:]
         for i in Segs_to_rm.index: I3.append(i)
         segs = segs.drop(I3)
         multi = multi[multi['is_redundant']==0]
     segs = Filter_miniseglen(segs,Sf_len_lab_persp,minseglen,genetable)
-    counted = segs.groupby(["multiplicon", "genome"])["segment"].aggregate(lambda x: len(set(x)))
-    profile = counted.unstack(level=-1).fillna(0)
-    fig = syntenic_depth_plot(profile)
-    fig.savefig(os.path.join(outdir, "Syndepth.svg"),bbox_inches='tight')
-    fig.savefig(os.path.join(outdir, "Syndepth.pdf"),bbox_inches='tight')
-    profile.to_csv(os.path.join(outdir, "Segprofile.csv"))
+    #counted = segs.groupby(["multiplicon", "genome"])["segment"].aggregate(lambda x: len(set(x)))
+    #profile = counted.unstack(level=-1).fillna(0)
+    #if len(gdf) <=5 :
+    #    fig = syntenic_depth_plot(profile)
+    #    fig.savefig(os.path.join(outdir, "Syndepth.svg"),bbox_inches='tight')
+    #    fig.savefig(os.path.join(outdir, "Syndepth.pdf"),bbox_inches='tight')
+    #profile.to_csv(os.path.join(outdir, "Segprofile.csv"))
     return segs,genetable,multi,removed_scfa
 
-def filter_mingenumber(segs,mingenenum):
+def filter_mingenumber(segs,mingenenum,outdir,N):
     rm_indice = []
     for indice, f, l in zip(segs.index,segs['first_coordinate'],segs['last_coordinate']):
         if (l-f+1) < mingenenum:
             rm_indice.append(indice)
     segs = segs.drop(rm_indice)
+    counted = segs.groupby(["multiplicon", "genome"])["segment"].aggregate(lambda x: len(set(x)))
+    profile = counted.unstack(level=-1).fillna(0)
+    if N <=5 :
+        logging.info("Making Syndepth plot")
+        fig = syntenic_depth_plot(profile)
+        fig.savefig(os.path.join(outdir, "Syndepth.svg"),bbox_inches='tight')
+        fig.savefig(os.path.join(outdir, "Syndepth.pdf"),bbox_inches='tight')
+    profile.to_csv(os.path.join(outdir, "Segprofile.csv"))
     return segs
 
 def Filter_miniseglen(segs,scaf_info,minseglen,genetable):
     rm_indice = []
     gene_start_info = {sp:{} for sp in scaf_info.keys()}
     work1 = genetable.reset_index().loc[:,['gene','species','start']]
     work2 = work1.groupby('species')
```

### Comparing `wgd-2.0.19/wgd.egg-info/PKG-INFO` & `wgd-2.0.20/wgd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgd
-Version: 2.0.19
+Version: 2.0.20
 Summary: wgd
 Home-page: http://github.com/heche-psb/wgd
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,15 +41,15 @@
 
 Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
 
 The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
 
 ## Installation
 
-The easiest way to install `wgd v2` is using PYPI
+The easiest way to install `wgd v2` is using PYPI. Note that if you want to get the latest update, we suggest installing from the source, since the update on PYPI will be delayed compared to here in the source.
 
 ```
 pip install wgd
 ```
 
 To install `wgd v2` in a virtual environment, the following command lines could be used.
 
@@ -500,15 +500,15 @@
 (((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
 ```
 
 ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
 
 As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
 
-If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below. Note that the order of given `spair` options decides the color of the *K*<sub>S</sub> distribution of each species pair.
 
 ```
 wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
 ```
 
 Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
```

### Comparing `wgd-2.0.19/wgd.egg-info/requires.txt` & `wgd-2.0.20/wgd.egg-info/requires.txt`

 * *Files identical despite different names*

