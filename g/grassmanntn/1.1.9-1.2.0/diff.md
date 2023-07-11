# Comparing `tmp/grassmanntn-1.1.9.tar.gz` & `tmp/grassmanntn-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.1.9.tar", last modified: Thu Jul  6 09:28:13 2023, max compression
+gzip compressed data, was "grassmanntn-1.2.0.tar", last modified: Tue Jul 11 05:16:53 2023, max compression
```

## Comparing `grassmanntn-1.1.9.tar` & `grassmanntn-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.9/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.9/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109895 2023-07-06 09:24:54.000000 grassmanntn-1.1.9/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.9/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-06 08:59:36.000000 grassmanntn-1.1.9/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.9/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-06 09:27:31.000000 grassmanntn-1.1.9/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.2.0/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.2.0/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   108809 2023-07-11 05:12:08.000000 grassmanntn-1.2.0/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.2.0/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-06 08:59:36.000000 grassmanntn-1.2.0/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.2.0/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-11 05:16:53.000000 grassmanntn-1.2.0/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-11 05:16:53.519706 grassmanntn-1.2.0/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-11 05:13:36.000000 grassmanntn-1.2.0/setup.py
```

### Comparing `grassmanntn-1.1.9/LICENSE.txt` & `grassmanntn-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.9/PKG-INFO` & `grassmanntn-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.9
+Version: 1.2.0
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_119.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_120.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.9/README.md` & `grassmanntn-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.9/grassmanntn/__init__.py` & `grassmanntn-1.2.0/grassmanntn/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -780,146 +780,131 @@
     def eig(self,string_inp,cutoff=None,debug_mode=False,save_memory=False):
         return eig(self,string_inp,cutoff,debug_mode,save_memory)
 
 ####################################################
 ##       Parity Calculation (internal tools)      ##
 ####################################################
 
-def absolute_parity(permutation, individual_parity):
+def absolute_sign(object_set, parity):
     """
-    Compute the absolute_parity of a permutation, assuming that some elements always commute
-    with every other element.
+    Compute the absolute sign of an object_set, assuming that some elements always commute with every other element.
     
     Parameters:
-    permutation (list[int]): A list object.
-    individual_parity (list[int]): A list of object's grassmann parity.
-    
+    object_set (list[int]): A list object.
+    parity (list[int]): A list of object's grassmann parity.
+
     Returns:
     int: 1 if the permutation is even, -1 if the permutation is odd.
     """
-    
-    def get_commutative_elements(permutation, individual_parity):
-        """
-        Return a set of commutine elements (individual_parity = even)
-        """
-        if(len(permutation)!=len(individual_parity)):
-            error("Error[absolute_parity.get_commutative_elements]: Inconsistent array sizes!")
-            
-        else:
-            commutative_elements = [x for i,x in enumerate(permutation) if (-1)**individual_parity[i]==1]
-            return set(commutative_elements)
-            
-    
-    commutative_elements = get_commutative_elements(permutation, individual_parity)
-    n = len(permutation)
-    noncommutative_elements = [x for x in permutation if x not in commutative_elements]
+    noncommutative_elements = [x for i,x in enumerate(object_set)
+                                if parity[i]%2==1]
     inversions = 0
     for i in range(len(noncommutative_elements)):
         for j in range(i+1, len(noncommutative_elements)):
             if noncommutative_elements[i] > noncommutative_elements[j]:
                 inversions += 1
     return (-1)**inversions
 
-def relative_parity_int(permutation1, permutation2, individual_parity1):
+def relative_sign_int(object_set1, object_set2, parity1):
     """
-    Compute the relative_parity from permuting permutation1 to permutation2 with the individual parity given by individual_parity1 of the list permutation1
+    Compute the relative sign from permuting object_set1 to object_set2 with the parity given by parity1 of the list object_set1
     
     Parameters:
-    permutation1 (list): first list
-    permutation2 (list): target list
-    individual_parity1 (list): grassmann parity of the first list
+    object_set1 (list): first list
+    object_set2 (list): target list
+    parity1 (list): Grassmann parity of the first list
     
     Returns:
     int: relative parity of the permutation
     """
     
     def permute_c(a, b, c):
         """
-        Permute the elements of c according to the permutation that maps a to b.
+        Permute elements of c according to the permutation that maps a to b.
         """
         x = list(np.argsort(a))
         xc = [ c[i] for i in x ]
         bxc = [ xc[i] for i in b ]
         return bxc
-
-    def get_noncommutative_elements(permutation, individual_parity):
+    def get_noncommutative(object_set, parity):
         """
-        Return a LIST of commutine elements (individual_parity = even)
+        Return a list of noncommutative elements
         """
-        if(len(permutation)!=len(individual_parity)):
-            error("Error[relative_parity_int.get_noncommutative_elements]: Inconsistent array sizes!")
-            
-        else:
-            noncommutative_elements = [x for i,x in enumerate(permutation) if (-1)**individual_parity[i]==-1]
-            return noncommutative_elements
+        noncommutative_elements = [x for i,x in enumerate(object_set)
+                                    if parity[i]%2==1]
+        return noncommutative_elements
+    # get parity of object_set2
+    parity2 = permute_c(object_set1, object_set2, parity1)
+    
+    noncommutative_elements1 = get_noncommutative(object_set1,parity1)
+    noncommutative_elements2 = get_noncommutative(object_set2,parity2)
+    
+    absolute_sign1 = absolute_sign(object_set1, parity1)
+    absolute_sign2 = absolute_sign(object_set2, parity2)
+    return absolute_sign1*absolute_sign2
 
-    individual_parity2 = permute_c(permutation1, permutation2, individual_parity1)
-    
-    noncommutative_elements1 = get_noncommutative_elements(permutation1,individual_parity1)
-    noncommutative_elements2 = get_noncommutative_elements(permutation2,individual_parity2)
-    
-    if(sorted(noncommutative_elements1) != sorted(noncommutative_elements2)):
-        error("Error[relative_parity_int]: Inconsistent grassmann-odd indices!")
-        
-    
-    absolute_parity1 = absolute_parity(permutation1, individual_parity1)
-    absolute_parity2 = absolute_parity(permutation2, individual_parity2)
-    return absolute_parity1*absolute_parity2
-    
-def relative_parity_single_input(string, individual_parity1):
+def relative_sign_string(string, parity1):
+    [string1,string2] = list(string.split("->"))
+    unique_chars = list(set(string1+string2))
+    char_to_int = {char: i for i, char in enumerate(unique_chars)}
+    object_set1 = [char_to_int[char] for char in string1]
+    object_set2 = [char_to_int[char] for char in string2]
+    return relative_sign_int(object_set1, object_set2, parity1)
+
+def relative_sign_single_input(string, parity1):
     """
-    the string version of relative_parity_int
+    the string version of relative_sign_int
     the sign factor version of single input einsum
     """
     [string1,string2] = list(string.split("->"))
     unique_chars = list(set(string1+string2))
     char_to_int = {char: i for i, char in enumerate(unique_chars)}
     permutation1 = [char_to_int[char] for char in string1]
     permutation2 = [char_to_int[char] for char in string2]
-    return relative_parity_int(permutation1, permutation2, individual_parity1)
+    return relative_sign_int(permutation1, permutation2, parity1)
 
-def relative_parity(string, individual_parity):
+def relative_sign(string, parity):
     """
     Imagine doing Grassmann version of Einsum.
     This function returns the sign factor of that sum.
-    You have to enter the parity of the input indices in [individual_parity]
+    You have to enter the parity of the input indices in [parity]
     The grassmann indices must not be added or removed!
     Use a different function to integrate them out!
     Examples:
-    >> relative_parity( "abCdE,aXdYb->XCEY", [0,0,1,0,1,0,1,0,1,0] )
+    >> relative_sign( "abCdE,aXdYb->XCEY", [0,0,1,0,1,0,1,0,1,0] )
     >> 1
     
-    >> relative_parity( "abCdE,aXYb->CXEY", [0,0,1,0,1,0,1,1,0] )
+    >> relative_sign( "abCdE,aXYb->CXEY", [0,0,1,0,1,0,1,1,0] )
     >> -1
     
     """
     [string_input,string_output] = list(string.split("->"))
     string_list = list(string_input.split(","))
     
     join_string = ""
     for i in range(len(string_list)):
         join_string = join_string + string_list[i]
         
-    if(len(join_string)!=len(individual_parity)):
-        error("Error[relative_parity]: The number of input list and parity list are not consistent!")
+    if(len(join_string)!=len(parity)):
+        error("Error[relative_sign]: The number of input list and parity list are not consistent!")
         
         
     #remove the summed indices
     def remove_duplicates(list1, list2):
         new_list1 = []
         new_list2 = []
         for i, val in enumerate(list1):
             if list1.count(val)==1 :
                 new_list1.append(val)
                 new_list2.append(list2[i])
         return new_list1, new_list2
         
-    join_string_list,individual_parity = remove_duplicates(list(join_string), individual_parity)
+    join_string_list,parity = remove_duplicates(list(join_string), parity)
     join_string = ''.join(join_string_list)+"->"+string_output
-    return relative_parity_single_input(join_string, individual_parity)
+    return relative_sign_single_input(join_string, parity)
 
 def reordering(stringa,stringb,mylist):
 
     rC = []
     for b in stringb:
         
         # locate the location of b in the original string
@@ -1287,36 +1272,36 @@
         
     # sign factor computation -------------------------------------------------------------------------
     
     if S1dim>0 and not skip_S1:
 
         S1 = np.zeros(S1_shape,dtype=int)
         iterator = np.nditer(S1, flags=['multi_index'])
-        individual_parity_list = []
+        parity_list = []
         sgn_list = []
 
         k=1
         kmax = getsize(S1_shape)
 
         s0 = time.time()
         s00 = s0
         progress_space() # << Don't remove this. This is for the show_progress!
 
         for element in iterator:
             coords = iterator.multi_index
             dupped_coords = use_copy_map(copy_map,coords)
             
-            individual_parity = [ param.gparity(i)%2 for i in dupped_coords ]
+            parity = [ param.gparity(i)%2 for i in dupped_coords ]
 
-            if individual_parity not in individual_parity_list:
-                individual_parity_list += individual_parity,
-                sgn = relative_parity(S1_sgn_computation_string,individual_parity)
+            if parity not in parity_list:
+                parity_list += parity,
+                sgn = relative_sign(S1_sgn_computation_string,parity)
                 sgn_list += sgn,
             else:
-                index = individual_parity_list.index(individual_parity)
+                index = parity_list.index(parity)
                 sgn = sgn_list[index]
 
             S1[coords] = sgn
 
             if time.time()-s0 > 2 :
                 show_progress(k,kmax+1,process_name = "einsum_sgn1",ratio = False,color="red",time=time.time()-s00)
                 s0 = time.time()
@@ -1422,27 +1407,27 @@
 
             s0 = time.time()
             s00 = s0
             progress_space() # << Don't remove this. This is for the show_progress!
 
             S3 = np.zeros(S3_shape,dtype=int)
             iterator = np.nditer(S3, flags=['multi_index'])
-            individual_parity_list = []
+            parity_list = []
             sgn_list = []
             for element in iterator:
                 coords = iterator.multi_index
 
-                individual_parity = [ param.gparity(i)%2 for i in coords ]
+                parity = [ param.gparity(i)%2 for i in coords ]
 
-                if individual_parity not in individual_parity_list:
-                    individual_parity_list += individual_parity,
-                    sgn = relative_parity(S3_sgn_computation_string,individual_parity)
+                if parity not in parity_list:
+                    parity_list += parity,
+                    sgn = relative_sign(S3_sgn_computation_string,parity)
                     sgn_list += sgn,
                 else:
-                    index = individual_parity_list.index(individual_parity)
+                    index = parity_list.index(parity)
                     sgn = sgn_list[index]
 
                 S3[coords] = sgn
 
                 if time.time()-s0 > 0.5 :
                     show_progress(k,kmax+1,process_name = "einsum_sgn3",ratio = False,color="red",time=time.time()-s00)
                     s0 = time.time()
```

### Comparing `grassmanntn-1.1.9/grassmanntn/example.py` & `grassmanntn-1.2.0/grassmanntn/example.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.9/grassmanntn/gauge2d.py` & `grassmanntn-1.2.0/grassmanntn/gauge2d.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.9/grassmanntn/param.py` & `grassmanntn-1.2.0/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.9/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.2.0/grassmanntn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.9
+Version: 1.2.0
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_119.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_120.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.9/setup.py` & `grassmanntn-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.1.9',      # Start with a small number and increase it with every change you make
+  version = '1.2.0',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_119.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_120.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

