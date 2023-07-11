# Comparing `tmp/golfy-1.6.0.tar.gz` & `tmp/golfy-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.6.0.tar", last modified: Mon Jul 10 19:45:27 2023, max compression
+gzip compressed data, was "golfy-1.7.0.tar", last modified: Tue Jul 11 20:48:42 2023, max compression
```

## Comparing `golfy-1.6.0.tar` & `golfy-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-10 19:45:27.521258 golfy-1.6.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.6.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-10 19:45:27.521122 golfy-1.6.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.6.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-10 19:45:27.519090 golfy-1.6.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      630 2023-07-10 19:41:36.000000 golfy-1.6.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-10 19:45:10.000000 golfy-1.6.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     8479 2023-07-07 14:29:26.000000 golfy-1.6.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     8453 2023-07-07 14:00:59.000000 golfy-1.6.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4089 2023-07-07 14:00:08.000000 golfy-1.6.0/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.6.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.6.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.6.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-10 19:45:27.519730 golfy-1.6.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      415 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.6.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.6.0/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-10 19:45:27.521292 golfy-1.6.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-10 19:45:27.520815 golfy-1.6.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.6.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     1660 2023-07-07 14:04:35.000000 golfy-1.6.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.6.0/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 20:48:42.623417 golfy-1.7.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.7.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-11 20:48:42.623285 golfy-1.7.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.7.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 20:48:42.621655 golfy-1.7.0/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      630 2023-07-11 20:48:33.000000 golfy-1.7.0/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.7.0/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     9217 2023-07-11 20:03:28.000000 golfy-1.7.0/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     9777 2023-07-11 20:47:09.000000 golfy-1.7.0/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4089 2023-07-11 19:30:21.000000 golfy-1.7.0/golfy/solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.7.0/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.7.0/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.7.0/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 20:48:42.622202 golfy-1.7.0/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      415 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.7.0/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.7.0/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-11 20:48:42.623454 golfy-1.7.0/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 20:48:42.622995 golfy-1.7.0/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.7.0/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1660 2023-07-07 14:04:35.000000 golfy-1.7.0/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.7.0/tests/test_optimize.py
```

### Comparing `golfy-1.6.0/LICENSE` & `golfy-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.6.0/PKG-INFO` & `golfy-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.6.0
+Version: 1.7.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.6.0/README.md` & `golfy-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `golfy-1.6.0/golfy/__init__.py` & `golfy-1.7.0/golfy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     DeconvolutionResult,
 )
 from .initialization import init
 from .optimization import optimize
 from .solution import Solution
 from .validity import is_valid, count_violations, violations_per_replicate
 
-__version__ = "1.6.0"
+__version__ = "1.7.0"
 
 __all__ = [
     "__version__",
     "Solution",
     "init",
     "optimize",
     "count_violations",
```

### Comparing `golfy-1.6.0/golfy/deconvolution.py` & `golfy-1.7.0/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.6.0/golfy/initialization.py` & `golfy-1.7.0/golfy/initialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import defaultdict
+import math
 from typing import Optional, Literal
 
 import numpy as np
 
 from .solution import Solution
 from .types import PeptidePairList
 from .util import pairs_to_dict, transitive_closure
@@ -182,36 +183,62 @@
     )
 
 
 def init(
     num_peptides: int = 100,
     peptides_per_pool: int = 5,
     num_replicates: int = 3,
-    num_pools: Optional[int] = None,
+    num_pools_per_replicate: Optional[int] = None,
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
     strategy: Literal["greedy", "random"] = "greedy",
     verbose=False,
 ) -> Solution:
+    """
+    Initialize a Solution for a given configuration
+
+    Args
+    ----
+    num_peptides
+        number of peptides (default: 100)
+
+    peptides_per_pool
+        number of peptides per pool (default: 5)
+
+    num_replicates
+        number of replicates in the Solution (default: 3)
+
+    num_pools_per_replicate
+        number of pools in each replicate (default: ceil(num_peptides / peptides_per_pool))
+
+    invalid_neighbors
+        list of peptide pairs that cannot be in the same pool
+
+    preferred_neighbors
+        list of peptide pairs that should be in the same pool
+
+    strategy
+        initialization strategy, either "greedy" or "random" (default: "greedy")
+    """
     if strategy == "greedy":
         s = _greedy_init(
             num_peptides=num_peptides,
             peptides_per_pool=peptides_per_pool,
             num_replicates=num_replicates,
-            num_pools=num_pools,
+            num_pools=num_pools_per_replicate,
             invalid_neighbors=invalid_neighbors,
             preferred_neighbors=preferred_neighbors,
             verbose=verbose,
         )
     elif strategy == "random":
         s = _random_init(
             num_peptides=num_peptides,
             peptides_per_pool=peptides_per_pool,
             num_replicates=num_replicates,
-            num_pools=num_pools,
+            num_pools=num_pools_per_replicate,
             invalid_neighbors=invalid_neighbors,
             preferred_neighbors=preferred_neighbors,
             verbose=verbose,
         )
     else:
         raise ValueError("Unknown initialization strategy: '%s'" % strategy)
```

### Comparing `golfy-1.6.0/golfy/optimization.py` & `golfy-1.7.0/golfy/optimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import random
+import time
+
 import numpy as np
 
 from .solution import Solution
 from .types import SwapCandidateList, ReplicateToNeighborDict
 from .validity import count_violations, violations_per_replicate
 from .util import pairs_to_dict
 
@@ -37,33 +39,37 @@
 
     needs_swap, replicate_to_neighbor_dict = find_violating_peptides(s)
 
     random.shuffle(needs_swap)
 
     swapped_pools = set()
     swapped_peptides = set()
+    empty_pools_per_replicate = {
+        replicate_idx: {
+            pool_idx
+            for (pool_idx, pool_peptides) in pool_to_peptides.items()
+            if len(pool_peptides) == 0
+        }
+        for (replicate_idx, pool_to_peptides) in replicate_to_pool_to_peptides.items()
+    }
     for replicate_idx, pool_idx_a, peptide_a in needs_swap:
         if pool_idx_a in swapped_pools or peptide_a in swapped_peptides:
             continue
 
         pool_to_peptides = replicate_to_pool_to_peptides[replicate_idx]
         pool_a = pool_to_peptides[pool_idx_a]
-
+        empty_pools = empty_pools_per_replicate[replicate_idx]
         # if a pool is empty, just move the offending peptide there
-        empty_pools = {
-            pool_idx
-            for (pool_idx, pool_peptides) in pool_to_peptides.items()
-            if len(pool_peptides) == 0
-        }
         if empty_pools:
             pool_idx_b = random.choice(list(empty_pools))
             s.move_peptide(replicate_idx, pool_idx_a, peptide_a, pool_idx_b)
             swapped_pools.add(pool_idx_a)
             swapped_pools.add(pool_idx_b)
             swapped_peptides.add(peptide_a)
+            empty_pools.remove(pool_idx_b)
         else:
             other_peptides = []
             peptide_to_pool_idx = {}
             for pool_idx_i, pool_peptides_i in pool_to_peptides.items():
                 if pool_idx_i != pool_idx_a and pool_idx_i not in swapped_pools:
                     all_peptides_ok = True
                     for p in pool_peptides_i:
@@ -148,15 +154,15 @@
                 swapped_pools.add(pool_idx_b)
                 swapped_peptides.add(peptide_a)
                 swapped_peptides.add(peptide_b)
 
 
 def optimize(
     s: Solution,
-    max_iters: int = 100,
+    max_iters: int = 2000,
     verbose: bool = False,
     add_pool_if_stuck: bool = True,
     return_history: bool = False,
 ) -> bool:
     """
     Iteratively update solution by randomly swapping a violating peptide with a random other peptide
 
@@ -165,40 +171,70 @@
     solution
         Initial solution which will be modified in-place
 
     max_iters
         Maximum number of swaps to consider performing
 
     verbose
-        Print number of violations for each iteration
+        print number of violations and pools for each iteration
 
     add_pool_if_stuck
         If no improvements have been made for 10 iters, add a pool
         to the last replicate
 
     return_history
         Return array of constraint validation counts per iteration
 
 
     Returns True if non-violating solution found, False if solution still has violations after
     max_iters
     """
-    old_num_violations = count_violations(s)
+    replicate_to_violation_count = violations_per_replicate(s)
+    old_num_violations = sum(replicate_to_violation_count.values())
+
     history = [old_num_violations]
     if verbose:
         print("Initial solution has %s violations" % (old_num_violations,))
+
+    if old_num_violations / s.num_replicates > 1000:
+        # before first iteration, add a lot of empty pools to any replicates with
+        # more than 1000 violations
+        for replicate_idx, violation_count in replicate_to_violation_count.items():
+            if violation_count > 1000:
+                num_new_pools = int(np.ceil(violation_count / 1000))
+                if verbose:
+                    print(
+                        "-- replicate %d has %d violations, adding %d pools"
+                        % (replicate_idx + 1, violation_count, num_new_pools)
+                    )
+                for _ in range(num_new_pools):
+                    s.add_empty_pool(replicate_idx)
+
     num_iters_without_improvement = 0
     for i in range(max_iters):
+        t0 = time.time()
         improve_solution(s)
+
         replicate_to_violation_count = violations_per_replicate(s)
+
         new_num_violations = sum(replicate_to_violation_count.values())
 
         history.append(new_num_violations)
+
         if verbose:
-            print("%d) %d -> %d" % (i + 1, old_num_violations, new_num_violations))
+            print(
+                "%d) %d -> %d violations (%d pools, %0.2fs)"
+                % (
+                    i + 1,
+                    old_num_violations,
+                    new_num_violations,
+                    s.num_pools(),
+                    time.time() - t0,
+                )
+            )
 
         if old_num_violations <= new_num_violations:
             num_iters_without_improvement += 1
         else:
             num_iters_without_improvement = 0
 
         old_num_violations = new_num_violations
@@ -209,22 +245,22 @@
             break
 
         if num_iters_without_improvement >= 3 and add_pool_if_stuck:
             replicates_in_need = [
                 r for (r, v) in replicate_to_violation_count.items() if v > 0
             ]
             assert len(replicates_in_need) > 0
-            replicate_idx = min(replicates_in_need)
-            s.add_empty_pool(replicate_idx)
+            for replicate_idx in replicates_in_need:
+                if verbose:
+                    print(
+                        "-- adding pool %d to replicate %d"
+                        % (len(s.assignments[replicate_idx]), replicate_idx + 1)
+                    )
+                s.add_empty_pool(replicate_idx)
             num_iters_without_improvement = 0
-            if verbose:
-                print(
-                    "Adding pool %d to replicate %d"
-                    % (len(s.assignments[replicate_idx]), replicate_idx + 1)
-                )
 
     result = old_num_violations == 0
 
     # just in case we ended up with any empty pools, remove them from the solution
     s.remove_empty_pools()
 
     if return_history:
```

### Comparing `golfy-1.6.0/golfy/solution.py` & `golfy-1.7.0/golfy/solution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.6.0/golfy/util.py` & `golfy-1.7.0/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-1.6.0/golfy/validity.py` & `golfy-1.7.0/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-1.6.0/golfy.egg-info/PKG-INFO` & `golfy-1.7.0/golfy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.6.0
+Version: 1.7.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.6.0/pyproject.toml` & `golfy-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-1.6.0/tests/test_deconvolution.py` & `golfy-1.7.0/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.6.0/tests/test_init.py` & `golfy-1.7.0/tests/test_init.py`

 * *Files identical despite different names*

