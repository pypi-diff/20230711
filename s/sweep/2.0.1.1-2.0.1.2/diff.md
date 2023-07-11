# Comparing `tmp/sweep-2.0.1.1-py3.10.egg` & `tmp/sweep-2.0.1.2-py3.10.egg`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 16086 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat     6201 b- defN 23-Jul-05 03:28 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      671 b- defN 23-Jul-05 03:28 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-05 03:28 EGG-INFO/dependency_links.txt
+Zip file size: 16008 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat     6036 b- defN 23-Jul-11 05:04 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      671 b- defN 23-Jul-11 05:04 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-11 05:04 EGG-INFO/dependency_links.txt
 -rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-05 03:28 EGG-INFO/not-zip-safe
--rw-rw-rw-  2.0 fat       32 b- defN 23-Jul-05 03:28 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-05 03:28 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat      316 b- defN 23-Jul-05 03:28 sweep/__init__.pyc
--rw-rw-rw-  2.0 fat      698 b- defN 23-Jul-05 03:28 sweep/calc_proj_mat_size.pyc
--rw-rw-rw-  2.0 fat     3244 b- defN 23-Jul-05 03:28 sweep/default_proj_mat_ope.pyc
--rw-rw-rw-  2.0 fat     5282 b- defN 23-Jul-05 03:28 sweep/fas2sweep.pyc
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jul-05 03:28 sweep/fastaread.pyc
--rw-rw-rw-  2.0 fat      565 b- defN 23-Jul-05 03:28 sweep/is_orthonormal.pyc
--rw-rw-rw-  2.0 fat      662 b- defN 23-Jul-05 03:28 sweep/orthbase.pyc
--rw-rw-rw-  2.0 fat      350 b- defN 23-Jul-05 03:28 sweep/sweep_support/__init__.pyc
--rw-rw-rw-  2.0 fat      601 b- defN 23-Jul-05 03:28 sweep/sweep_support/aa2idx.pyc
--rw-rw-rw-  2.0 fat      807 b- defN 23-Jul-05 03:28 sweep/sweep_support/aa2int.pyc
--rw-rw-rw-  2.0 fat      578 b- defN 23-Jul-05 03:28 sweep/sweep_support/generate_chunk.pyc
--rw-rw-rw-  2.0 fat      301 b- defN 23-Jul-05 03:28 sweep/sweep_support/ij2inds.pyc
--rw-rw-rw-  2.0 fat      815 b- defN 23-Jul-05 03:28 sweep/sweep_support/mask2vec_bin.pyc
--rw-rw-rw-  2.0 fat      894 b- defN 23-Jul-05 03:28 sweep/sweep_support/mask2vec_count.pyc
--rw-rw-rw-  2.0 fat      762 b- defN 23-Jul-05 03:28 sweep/sweep_support/nt2int.pyc
--rw-rw-rw-  2.0 fat      451 b- defN 23-Jul-05 03:28 sweep/sweep_support/orth.pyc
--rw-rw-rw-  2.0 fat      483 b- defN 23-Jul-05 03:28 sweep/sweep_support/seq2list.pyc
-23 files, 24237 bytes uncompressed, 13094 bytes compressed:  46.0%
+-rw-rw-rw-  2.0 fat       32 b- defN 23-Jul-11 05:04 EGG-INFO/requires.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-11 05:04 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Jul-11 05:04 sweep/__init__.pyc
+-rw-rw-rw-  2.0 fat      698 b- defN 23-Jul-11 05:04 sweep/calc_proj_mat_size.pyc
+-rw-rw-rw-  2.0 fat     3244 b- defN 23-Jul-11 05:04 sweep/default_proj_mat_ope.pyc
+-rw-rw-rw-  2.0 fat     5282 b- defN 23-Jul-11 05:04 sweep/fas2sweep.pyc
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jul-11 05:04 sweep/fastaread.pyc
+-rw-rw-rw-  2.0 fat      565 b- defN 23-Jul-11 05:04 sweep/is_orthonormal.pyc
+-rw-rw-rw-  2.0 fat      662 b- defN 23-Jul-11 05:04 sweep/orthbase.pyc
+-rw-rw-rw-  2.0 fat      350 b- defN 23-Jul-11 05:04 sweep/sweep_support/__init__.pyc
+-rw-rw-rw-  2.0 fat      601 b- defN 23-Jul-11 05:04 sweep/sweep_support/aa2idx.pyc
+-rw-rw-rw-  2.0 fat      807 b- defN 23-Jul-11 05:04 sweep/sweep_support/aa2int.pyc
+-rw-rw-rw-  2.0 fat      578 b- defN 23-Jul-11 05:04 sweep/sweep_support/generate_chunk.pyc
+-rw-rw-rw-  2.0 fat      301 b- defN 23-Jul-11 05:04 sweep/sweep_support/ij2inds.pyc
+-rw-rw-rw-  2.0 fat      815 b- defN 23-Jul-11 05:04 sweep/sweep_support/mask2vec_bin.pyc
+-rw-rw-rw-  2.0 fat      894 b- defN 23-Jul-11 05:04 sweep/sweep_support/mask2vec_count.pyc
+-rw-rw-rw-  2.0 fat      762 b- defN 23-Jul-11 05:04 sweep/sweep_support/nt2int.pyc
+-rw-rw-rw-  2.0 fat      451 b- defN 23-Jul-11 05:04 sweep/sweep_support/orth.pyc
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Jul-11 05:04 sweep/sweep_support/seq2list.pyc
+23 files, 24072 bytes uncompressed, 13016 bytes compressed:  45.9%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: sweep
-Version: 2.0.1.1
+Version: 2.0.1.2
 Summary: SWeeP is a tool for representing large biological sequences datasets in compact vectors
 Home-page: https://github.com/diogomachado-bioinfo/sweep
 Author: Diogo de J. S. Machado
 Author-email: diogomachado.bioinfo@gmail.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 
   -----------------------------------
-  SWeeP: Sequence Window Projection
+  SWeeP: Spaced Words Projection
   -----------------------------------
 
-This Python package implements the SWeeP (Spaced Words Projection)
-algorithm for representing large biological sequence datasets in compact
-vectors. SWeeP allows efficient processing and analysis of sequence data
-by converting sequences into fixed-length feature vectors.
+This Python package implements the SWeeP (Spaced Words Projection), a
+algorithm for representing biological sequences in compact and fixed-length
+feature vectors.
 
 # Installation
 
 To use SWeeP in Python, install the package with the following command:
 
     pip install sweep
 
@@ -27,57 +26,62 @@
 
 ## Downloading the Default Projection Matrix
 
 In the first use of fas2sweep with the default parameter, it will be
 necessary to download the default projection matrix. It is not necessary
 for use with custom projection matrix, as demonstrated in the "Changing
 Projection Matrix" topic. Here is how to perform the default matrix download:
-
+```python
     from sweep import down_proj_mat
+
     down_proj_mat() # Downloads the default projection matrix file
+```
 
 ## Handling Amino Acid Sequences
 
 The default configurations of SWeeP are intended for vectorization of
 amino acid sequences. The default output is a matrix already projected
 with 600 columns. Here is an example of how to use SWeeP with amino acid
 sequences:
-
+```python
     from sweep import fastaread, fas2sweep
 
     fasta = fastaread("fasta_file_path")
     vect = fas2sweep(fasta)
+```
 
 ## Changing Projection Matrix
 
 To change the projection matrix, a new orthonormal matrix can be
 generated using the orthbase function. Here is an example of how
 to change the projection size to 300:
-
+```python
     from sweep import fastaread, fas2sweep, orthbase
 
     ob = orthbase(160000, 300)
     fasta = fastaread("fasta_file_path")
     vect = fas2sweep(fasta, orth_mat=ob)
+```
 
 ## Handling Nucleotide Sequences
 
 For nucleotide sequences, there is no default projection matrix
 available in this version. Therefore, to work with nucleotides
 is possible to create a custom projection matrix using the
 orthbase function. The matrix size can be calculated using
 the calc_proj_mat_size function. Here is an example:
-
+```python
     from sweep import fastaread, fas2sweep, orthbase, calc_proj_mat_size
 
     mask = [4, 7, 4]
     matrix_size = calc_proj_mat_size(mask, 'NT')
     ob = orthbase(matrix_size, 600)
     fasta = fastaread("fasta_file_path")
     vect = fas2sweep(fasta, mask=mask, orth_mat=ob, fasta_type='NT')
+```
 
 ## Available Functions
 
 Here is a summary of the
 functions available in the SWeeP package:
 
 | Function                            | Description                                                                      | Input                                                          | Output                                          |
@@ -89,27 +93,24 @@
 | ``down_proj_mat``                   | Downloads the default projection matrix file                                     | ``destination`` (str): Path to the destination file (optional) | None                                            |
 | ``return_proj_mat_not_found_error`` | Raises an exception indicating that the default projection matrix is not found   | None                                                           | None                                            |
 | ``check_default_proj_mat``          | Checks if the default projection matrix exists and matches the expected MD5 hash | ``file`` (str): Path to the projection matrix file             | None                                            |
 | ``get_default_proj_mat``            | Retrieves the default projection matrix                                          | None                                                           | ``orth_mat`` (numpy.ndarray): Projection matrix |
 
 ## Article Reference
 
-If you use the SWeeP algorithm or this Python package in your research work, please cite the
+If you use the SWeeP algorithm or this Python package in your work, please cite the
 following article:
 
-```
+```bib
 @article{Pierri2020,
   title={SWeeP: representing large biological sequences datasets in compact vectors},
   author={De Pierri, Camilla Reginatto and Voyceik, Ricardo and Santos de Mattos, LetÃ­cia Graziela Costa and Kulik, Mariane GonÃ§alves and Camargo, JosuÃ© Oliveira and Repula de Oliveira, Aryel Marlus and de Lima Nichio, Bruno Thiago and Marchaukoski, Jeroniza Nunes and da Silva Filho, Antonio Camilo and Guizelini, Dieval and Ortega, J. Miguel and Pedrosa, Fabio O. and Raittz, Roberto Tadeu},
   journal={Scientific Reports},
   volume={10},
   number={1},
   pages={91},
   year={2020},
   doi={10.1038/s41598-019-55627-4},
   url={https://doi.org/10.1038/s41598-019-55627-4},
   issn={2045-2322}
 }
 ```
-
-Please refer to the article for a detailed description of the SWeeP
-algorithm and its applications.
```

