# Comparing `tmp/hopsy-1.1.0-cp39-cp39-win_amd64.whl.zip` & `tmp/hopsy-1.2.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 767200 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      151 b- defN 22-Oct-20 17:46 hopsy/__init__.py
--rw-rw-rw-  2.0 fat  2223616 b- defN 22-Oct-20 21:01 hopsy/core.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1105 b- defN 22-Oct-20 17:46 hopsy/lp.py
--rw-rw-rw-  2.0 fat    24639 b- defN 22-Oct-20 17:46 hopsy/misc.py
--rw-rw-rw-  2.0 fat     1126 b- defN 22-Oct-20 21:01 hopsy-1.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4825 b- defN 22-Oct-20 21:01 hopsy-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Oct-20 21:01 hopsy-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 22-Oct-20 21:01 hopsy-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      678 b- defN 22-Oct-20 21:01 hopsy-1.1.0.dist-info/RECORD
-9 files, 2256257 bytes uncompressed, 766056 bytes compressed:  66.1%
+Zip file size: 820422 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      199 b- defN 23-Jul-10 20:18 hopsy/__init__.py
+-rw-rw-rw-  2.0 fat     6150 b- defN 23-Jul-10 20:18 hopsy/callback.py
+-rw-rw-rw-  2.0 fat  2370560 b- defN 23-Jul-10 20:35 hopsy/core.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2541 b- defN 23-Jul-10 20:18 hopsy/examples.py
+-rw-rw-rw-  2.0 fat     1115 b- defN 23-Jul-10 20:18 hopsy/lp.py
+-rw-rw-rw-  2.0 fat    35110 b- defN 23-Jul-10 20:18 hopsy/misc.py
+-rw-rw-rw-  2.0 fat     1104 b- defN 23-Jul-10 20:35 hopsy-1.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6171 b- defN 23-Jul-10 20:35 hopsy-1.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-10 20:35 hopsy-1.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-10 20:35 hopsy-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      826 b- defN 23-Jul-10 20:35 hopsy-1.2.0.dist-info/RECORD
+11 files, 2423893 bytes uncompressed, 819058 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,28 +1,34 @@
 Filename: hopsy/__init__.py
 Comment: 
 
+Filename: hopsy/callback.py
+Comment: 
+
 Filename: hopsy/core.cp39-win_amd64.pyd
 Comment: 
 
+Filename: hopsy/examples.py
+Comment: 
+
 Filename: hopsy/lp.py
 Comment: 
 
 Filename: hopsy/misc.py
 Comment: 
 
-Filename: hopsy-1.1.0.dist-info/LICENSE
+Filename: hopsy-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: hopsy-1.1.0.dist-info/METADATA
+Filename: hopsy-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: hopsy-1.1.0.dist-info/WHEEL
+Filename: hopsy-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: hopsy-1.1.0.dist-info/top_level.txt
+Filename: hopsy-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: hopsy-1.1.0.dist-info/RECORD
+Filename: hopsy-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hopsy/__init__.py

```diff
@@ -1,5 +1,8 @@
-from . core import *
-del globals()['MarkovChain']
-from . core import __version__, __build__, __is_debug__
-from . misc import *
-from . lp import *
+from .core import *
+
+del globals()["MarkovChain"]
+from .callback import *
+from .core import __build__, __is_debug__, __version__
+from .examples import *
+from .lp import *
+from .misc import *
```

## hopsy/lp.py

```diff
@@ -1,17 +1,20 @@
 """
 
 """
-from PolyRound.settings import PolyRoundSettings
 import threading as _threading
 
+from PolyRound.settings import PolyRoundSettings
+
 
 class LP:
     """Singleton for controlling PolyRound parameters for Linear Programming.
-    Pattern from https://medium.com/analytics-vidhya/how-to-create-a-thread-safe-singleton-class-in-python-822e1170a7f6"""
+    Pattern from https://medium.com/analytics-vidhya/how-to-create-a-thread-safe-singleton-class-in-python-822e1170a7f6
+    """
+
     __instance = None
     settings = None
     _lock = _threading.Lock()
 
     def __new__(self, *args, **kwargs):
         """thread safe instance instantiation"""
         if not self.__instance:
```

## hopsy/misc.py

```diff
@@ -1,126 +1,173 @@
 """
 
 """
+
+
 class _core:
-    from .core import GaussianHitAndRunProposal
-    from .core import MarkovChain
-    from .core import Problem
-    from .core import Proposal
-    from .core import RandomNumberGenerator
+    from .callback import Callback
+    from .core import (
+        GaussianHitAndRunProposal,
+        MarkovChain,
+        Problem,
+        Proposal,
+        RandomNumberGenerator,
+    )
     from .lp import LP
 
+
 _c = _core
 
 
 class _submodules:
-    import numpy
+    import warnings
+
     import arviz
+    import numpy
     import pandas
 
-    import warnings
-
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
 
         from PolyRound.api import PolyRoundApi
         from PolyRound.mutable_classes import polytope
         from PolyRound.static_classes.lp_utils import ChebyshevFinder
 
     import multiprocessing
+    import os
 
-    import numpy.typing
+    if "JPY_PARENT_PID" in os.environ:
+        import tqdm.notebook as tqdm
+    else:
+        import tqdm
     import typing
 
+    import numpy.typing
+
+
 _s = _submodules
 
 
-def MarkovChain(problem: _c.Problem,
-                proposal: _s.typing.Union[_c.Proposal, _s.typing.Type[_c.Proposal]] = _c.GaussianHitAndRunProposal,
-                starting_point: _s.numpy.typing.ArrayLike = None):
+def MarkovChain(
+    problem: _c.Problem,
+    proposal: _s.typing.Union[
+        _c.Proposal, _s.typing.Type[_c.Proposal]
+    ] = _c.GaussianHitAndRunProposal,
+    starting_point: _s.numpy.typing.ArrayLike = None,
+    parallelTemperingSyncRng: _c.RandomNumberGenerator = None,
+    exchangeAttemptProbability: float = 0.1,
+):
     _proposal = None
     if isinstance(proposal, type):
         if starting_point is not None:
             _proposal = proposal(problem, starting_point=starting_point)
         elif problem.starting_point is not None:
             _proposal = proposal(problem, starting_point=problem.starting_point)
         else:
             _proposal = proposal(problem)
     else:
         _proposal = proposal
 
-    return _c.MarkovChain(_proposal, problem)
-
-
-MarkovChain.__doc__ = _core.MarkovChain.__doc__ # propagate docstring
-
-
-def add_box_constraints(problem: _c.Problem,
-                        lower_bound: _s.typing.Union[_s.numpy.typing.ArrayLike, float],
-                        upper_bound: _s.typing.Union[_s.numpy.typing.ArrayLike, float],
-                        simplify = True):
+    return _c.MarkovChain(
+        _proposal,
+        problem,
+        parallelTemperingSyncRng=parallelTemperingSyncRng,
+        exchangeAttemptProbability=exchangeAttemptProbability,
+    )
+
+
+MarkovChain.__doc__ = _core.MarkovChain.__doc__  # propagate docstring
+
+
+def add_box_constraints(
+    problem: _c.Problem,
+    lower_bound: _s.typing.Union[_s.numpy.typing.ArrayLike, float],
+    upper_bound: _s.typing.Union[_s.numpy.typing.ArrayLike, float],
+    simplify=True,
+):
     r"""Adds box constraints to all dimensions. This will extend :attr:`hopsy.Problem.A` and :attr:`hopsy.Problem.A` of the returned :class:`hopsy.Problem` to have :math:`m+2n` rows.
-    Box constraints are added naively, meaning that we do neither check whether the dimension may be already 
+    Box constraints are added naively, meaning that we do neither check whether the dimension may be already
     somehow bound nor check whether the very same constraint already exists. You can remove redundant constraints
     efficiently using the `PolyRound <https://pypi.org/project/PolyRound/>`_ toolbox or by using the :func:`hopsy.round` function, uses PolyRound to remove redundant constraints and also rounds the polytope.
 
-    If ``lower_bound`` and ``upper_bound`` are both ``float``, then every dimension :math:`i` will be bound as 
-    :math:`lb \leq x_i \leq ub`. If `lower_bound`` and ``upper_bound`` are both ``numpy.ndarray`` with 
+    If ``lower_bound`` and ``upper_bound`` are both ``float``, then every dimension :math:`i` will be bound as
+    :math:`lb \leq x_i \leq ub`. If `lower_bound`` and ``upper_bound`` are both ``numpy.ndarray`` with
     appropriate length, then every dimension :math:`i` will be bound as :math:`lb_i \leq x_i \leq ub_i`.
 
     :param hopsy.Problem problem: Problem which should be constrained and which contains the matrix :math:`A` and vector :math:`b` in :math:`Ax \leq b`.
 
-    :param lower_bound: Specifies the lower bound(s). 
+    :param lower_bound: Specifies the lower bound(s).
     :type lower_bound: numpy.ndarray[float64[n,1]] or float
 
-    :param upper_bound: Specifies the upper bound(s). 
+    :param upper_bound: Specifies the upper bound(s).
     :type upper_bound: numpy.ndarray[float64[n,1]] or float
 
     :return: A :class:`hopsy.Problem` bounded in all dimensions.
     :rtype: hopsy.Problem
     """
     if problem.A.shape[1] == 0:
         raise ValueError("Cannot determine dimension for empty inequality Ax <= b.")
 
     if hasattr(lower_bound, "__len__") and len(lower_bound) != problem.A.shape[1]:
-        raise TypeError("Length of array-like lower_bound has to match column space dimension of the problem.")
+        raise TypeError(
+            "Length of array-like lower_bound has to match column space dimension of the problem."
+        )
     if hasattr(upper_bound, "__len__") and len(upper_bound) != problem.A.shape[1]:
-        raise TypeError("Length of array-like upper_bound has to match column space dimension of the problem.")
+        raise TypeError(
+            "Length of array-like upper_bound has to match column space dimension of the problem."
+        )
 
     dim = problem.A.shape[1]
 
-    _l = _s.numpy.array(lower_bound) if hasattr(lower_bound, "__len__") else _s.numpy.array([lower_bound] * dim)
-    _l = -_l # flip sign comes from flipping -x<-l to x>l
-    _u = _s.numpy.array(upper_bound) if hasattr(upper_bound, "__len__") else _s.numpy.array([upper_bound] * dim)
+    _l = (
+        _s.numpy.array(lower_bound)
+        if hasattr(lower_bound, "__len__")
+        else _s.numpy.array([lower_bound] * dim)
+    )
+    _l = -_l  # flip sign comes from flipping -x<-l to x>l
+    _u = (
+        _s.numpy.array(upper_bound)
+        if hasattr(upper_bound, "__len__")
+        else _s.numpy.array([upper_bound] * dim)
+    )
 
     A = _s.numpy.vstack([problem.A, -_s.numpy.eye(dim), _s.numpy.eye(dim)])
     b = _s.numpy.hstack([problem.b.flatten(), _l.flatten(), _u.flatten()]).reshape(-1)
 
-    _problem = _c.Problem(A, b, problem.model, problem.starting_point, problem.transformation, problem.shift)
+    _problem = _c.Problem(
+        A,
+        b,
+        problem.model,
+        problem.starting_point,
+        problem.transformation,
+        problem.shift,
+    )
 
     if simplify:
         with _s.warnings.catch_warnings():
             _s.warnings.simplefilter("ignore")
 
             _problem = _simplify(_problem)
 
     return _problem
 
 
 def compute_chebyshev_center(problem: _c.Problem):
     """
-    Computes the Chebyshev center, that is the midpoint of a (non-unique) largest inscribed ball in the polytope defined by :math:`Ax \leq b`. 
+    Computes the Chebyshev center, that is the midpoint of a (non-unique) largest inscribed ball in the polytope defined by :math:`Ax \leq b`.
 
     :param hopsy.Problem problem: Problem for which the Chebyshev center should be computed and which contains the matrix :math:`A` and vector :math:`b` in :math:`Ax \leq b`.
 
     :return: The Chebyshev center of the passed problem.
     :rtype: numpy.ndarray[float64[n,1]]
     """
     polytope = _s.polytope.Polytope(problem.A, problem.b)
-    chebyshev_center = _s.ChebyshevFinder.chebyshev_center(polytope, _c.LP().settings)[0]
+    chebyshev_center = _s.ChebyshevFinder.chebyshev_center(polytope, _c.LP().settings)[
+        0
+    ]
 
     return chebyshev_center
 
 
 def _compute_maximum_volume_ellipsoid(problem: _c.Problem):
     with _s.warnings.catch_warnings():
         _s.warnings.simplefilter("ignore")
@@ -129,57 +176,85 @@
 
         polytope = _s.PolyRoundApi.simplify_polytope(polytope, _c.LP().settings)
 
         if polytope.S is not None:
             polytope = _s.PolyRoundApi.transform_polytope(polytope, _c.LP().settings)
         else:
             number_of_reactions = polytope.A.shape[1]
-            polytope.transformation = _s.pandas.DataFrame(_s.numpy.identity(number_of_reactions))
-            polytope.transformation.index = [str(i) for i in range(polytope.transformation.to_numpy().shape[0])]
-            polytope.transformation.columns = [str(i) for i in range(polytope.transformation.to_numpy().shape[1])]
+            polytope.transformation = _s.pandas.DataFrame(
+                _s.numpy.identity(number_of_reactions)
+            )
+            polytope.transformation.index = [
+                str(i) for i in range(polytope.transformation.to_numpy().shape[0])
+            ]
+            polytope.transformation.columns = [
+                str(i) for i in range(polytope.transformation.to_numpy().shape[1])
+            ]
             polytope.shift = _s.pandas.Series(_s.numpy.zeros(number_of_reactions))
 
         MaximumVolumeEllipsoidFinder.iterative_solve(polytope, _c.LP().settings)
         return polytope.transform.values
 
+
 def simplify(problem: _c.Problem):
-    """
+    r"""simplify(problem)
+
+    Simplifies the polytope defined in the ``problem`` by removing redundant constraints and refunction inequality constraints to equality constraints in case of dimension width less than thresh.
+    Thresh is defined in the LP settings singleton and refers to `PolyRound <https://pypi.org/project/PolyRound/>`_ settings.
+    Simplification is typically the first step before sampling. It is called automatically when round is called, because it is required for efficient and effective rounding.
 
+    Parameters
+    ----------
+    problem: hopsy.Problem for which the polytope should be simplified
+
+    Returns
+    -------
+    hopsy.Problem
+        Problem with simplified polytope.
     """
+
     with _s.warnings.catch_warnings():
         _s.warnings.simplefilter("ignore")
 
         polytope = _s.polytope.Polytope(problem.A, problem.b)
 
-        polytope = _s.PolyRoundApi.simplify_polytope(polytope, settings=_c.LP().settings)
+        polytope = _s.PolyRoundApi.simplify_polytope(
+            polytope, settings=_c.LP().settings
+        )
         if polytope.S is not None:
             polytope = _s.PolyRoundApi.transform_polytope(polytope, _c.LP().settings)
         else:
             number_of_reactions = polytope.A.shape[1]
-            polytope.transformation = _s.pandas.DataFrame(_s.numpy.identity(number_of_reactions))
-            polytope.transformation.index = [str(i) for i in range(polytope.transformation.to_numpy().shape[0])]
-            polytope.transformation.columns = [str(i) for i in range(polytope.transformation.to_numpy().shape[1])]
+            polytope.transformation = _s.pandas.DataFrame(
+                _s.numpy.identity(number_of_reactions)
+            )
+            polytope.transformation.index = [
+                str(i) for i in range(polytope.transformation.to_numpy().shape[0])
+            ]
+            polytope.transformation.columns = [
+                str(i) for i in range(polytope.transformation.to_numpy().shape[1])
+            ]
             polytope.shift = _s.pandas.Series(_s.numpy.zeros(number_of_reactions))
 
         problem.A = polytope.A.values
         problem.b = polytope.b.values
 
         return problem
 
 
 _simplify = simplify
 
 
 def round(problem: _c.Problem):
     """
-    Rounds the polytope defined by the inequality :math:`Ax \leq b` using 
-    `PolyRound <https://pypi.org/project/PolyRound/>`_. 
+    Rounds the polytope defined by the inequality :math:`Ax \leq b` using
+    `PolyRound <https://pypi.org/project/PolyRound/>`_.
     This function also strips redundant constraints.
     The unrounding transformation :math:`T` and shift :math:`s` will be stored in :attr:`hopsy.UniformProblem.transformation`
-    and :attr:`hopsy.UniformProblem.shift` of the returned problem. Its left-hand side operator :attr:`hopsy.UniformProblem.A` and 
+    and :attr:`hopsy.UniformProblem.shift` of the returned problem. Its left-hand side operator :attr:`hopsy.UniformProblem.A` and
     the right-hand side :attr:`hopsy.UniformProblem.b` of the polytope will be transformed as :math:``
     inequality
 
     :param hopsy.Problem problem: Problem that should be rounded and which contains the matrix :math:`A` and vector :math:`b` in :math:`Ax \leq b`.
 
     :return: The rounded problem.
     :rtype: hopsy.Problem
@@ -191,37 +266,53 @@
 
         polytope = _s.PolyRoundApi.simplify_polytope(polytope, _c.LP().settings)
 
         if polytope.S is not None:
             polytope = _s.PolyRoundApi.transform_polytope(polytope, _c.LP().settings)
         else:
             number_of_reactions = polytope.A.shape[1]
-            polytope.transformation = _s.pandas.DataFrame(_s.numpy.identity(number_of_reactions))
-            polytope.transformation.index = [str(i) for i in range(polytope.transformation.to_numpy().shape[0])]
-            polytope.transformation.columns = [str(i) for i in range(polytope.transformation.to_numpy().shape[1])]
+            polytope.transformation = _s.pandas.DataFrame(
+                _s.numpy.identity(number_of_reactions)
+            )
+            polytope.transformation.index = [
+                str(i) for i in range(polytope.transformation.to_numpy().shape[0])
+            ]
+            polytope.transformation.columns = [
+                str(i) for i in range(polytope.transformation.to_numpy().shape[1])
+            ]
             polytope.shift = _s.pandas.Series(_s.numpy.zeros(number_of_reactions))
 
         polytope = _s.PolyRoundApi.round_polytope(polytope, _c.LP().settings)
 
-        _problem = _c.Problem(polytope.A.values, polytope.b.values, problem.model, transformation=polytope.transformation.values, shift=polytope.shift.values)
+        _problem = _c.Problem(
+            polytope.A.values,
+            polytope.b.values,
+            problem.model,
+            transformation=polytope.transformation.values,
+            shift=polytope.shift.values,
+        )
 
         if problem.starting_point is not None:
             _problem.starting_point = transform(_problem, [problem.starting_point])[0]
 
         return _problem
 
 
 def back_transform(problem: _c.Problem, points: _s.numpy.typing.ArrayLike):
     """
     Transforms samples back from the sampling space (typically rounded) to the original parameter space.
     """
     transformed_points = []
 
     for point in points:
-        _point = problem.transformation @ point if problem.transformation is not None else point
+        _point = (
+            problem.transformation @ point
+            if problem.transformation is not None
+            else point
+        )
         _point = _point + problem.shift if problem.shift is not None else _point
 
         transformed_points.append(_point)
 
     return transformed_points
 
 
@@ -230,367 +321,681 @@
     Transforms samples from the parameter space to the sampling space (typically rounded).
 
     """
     transformed_points = []
 
     for point in points:
         _point = point - problem.shift if problem.shift is not None else point
-        _point = _s.numpy.linalg.solve(problem.transformation, _point) if problem.transformation is not None else _point
+        _point = (
+            _s.numpy.linalg.solve(problem.transformation, _point)
+            if problem.transformation is not None
+            else _point
+        )
 
         transformed_points.append(_point)
 
     return transformed_points
 
 
-def _sample(markov_chain: _c.MarkovChain,
-            rng: _c.RandomNumberGenerator,
-            n_samples: int,
-            thinning: int,
-            record_meta = None):
+def _sequential_sampling(
+    markov_chain: _c.MarkovChain,
+    rng: _c.RandomNumberGenerator,
+    n_samples: int,
+    thinning: int,
+    chain_idx: int,
+    in_memory: bool,
+    record_meta=None,
+    callback: _c.Callback = None,
+    progress_bar: bool = False,
+):
     states = []
-    meta = [] if record_meta is None or record_meta is False else {field: [] for field in record_meta}
 
-    missing_fields = []
+    meta = None
+    if record_meta is None or record_meta is False:
+        meta = []
+    else:
+        meta = {field: [] for field in record_meta}
 
-    for i in range(n_samples):
+    sample_range = (
+        _s.tqdm.trange(n_samples, desc="chain {}".format(chain_idx))
+        if progress_bar
+        else range(n_samples)
+    )
+    for i in sample_range:
         accrate, state = markov_chain.draw(rng, thinning)
 
+        curr_meta = None
         if record_meta is None or record_meta is False:
-            meta.append(accrate)
+            curr_meta = accrate
         else:
+            curr_meta = {}
             for field in record_meta:
-                if field in missing_fields: continue
-
-                if field == "acceptance_rate": # treat acceptance rate differently,
-                                               # as it is no attribute of the markov chain
-                    meta[field].append(accrate)
+                if field == "acceptance_rate":  # treat acceptance rate differently,
+                    # as it is no attribute of the markov chain
+                    curr_meta[field] = accrate
                 else:
                     # recurse through the attribute name and record the final value
-                    attrs = field.split('.')
+                    attrs = field.split(".")
                     base = markov_chain
+                    for attr in attrs:
+                        base = getattr(base, attr)
 
-                    found = True
+                    curr_meta[field] = base
 
-                    for attr in attrs:
-                        if hasattr(base, attr):
-                            base = getattr(base, attr)
-                        else:
-                            found = False
+        if in_memory:
+            states.append(state)
 
-                    if found:
-                        meta[field].append(base)
-                    else:
-                        missing_fields.append(field)
-                        meta[field] = None
+            if record_meta is None or record_meta is False:
+                meta.append(curr_meta)
+            else:
+                for field in record_meta:
+                    meta[field].append(curr_meta[field])
 
-        states.append(state)
+        if callback is not None:
+            callback.record(
+                chain_idx,
+                state,
+                curr_meta
+                if isinstance(curr_meta, dict)
+                else {"acceptance_rate": curr_meta},
+            )
 
-    if record_meta is None or record_meta is False:
+    if (record_meta is None or record_meta is False) and in_memory:
         meta = _s.numpy.mean(meta)
 
+    if callback is not None:
+        callback.finish()
+
     return meta, _s.numpy.array(states)
 
 
-def sample(markov_chains: _s.typing.Union[_c.MarkovChain, _s.typing.List[_c.MarkovChain]],
-           rngs: _s.typing.Union[_c.RandomNumberGenerator, _s.typing.List[_c.RandomNumberGenerator]],
-           n_samples: int,
-           thinning: int = 1,
-           n_threads: int = 1,
-           record_meta = None):
-    r"""sample(markov_chains, rngs, n_samples, thinning=1, n_threads=1)
+def _sample_parallel_chain(
+    markov_chain: _c.MarkovChain,
+    rng: _c.RandomNumberGenerator,
+    n_samples: int,
+    thinning: int,
+    chain_idx: int,
+    in_memory: bool,
+    record_meta=None,
+    queue: _s.multiprocessing.Queue = None,
+):
+    states = []
+
+    meta = None
+    if record_meta is None or record_meta is False:
+        meta = []
+    else:
+        meta = {field: [] for field in record_meta}
+
+    for i in range(n_samples):
+        accrate, state = markov_chain.draw(rng, thinning)
+
+        curr_meta = None
+        if record_meta is None or record_meta is False:
+            curr_meta = accrate
+        else:
+            curr_meta = {}
+            for field in record_meta:
+                if field == "acceptance_rate":  # treat acceptance rate differently,
+                    # as it is no attribute of the markov chain
+                    curr_meta[field] = accrate
+                else:
+                    # recurse through the attribute name and record the final value
+                    attrs = field.split(".")
+                    base = markov_chain
+                    for attr in attrs:
+                        base = getattr(base, attr)
+
+                    curr_meta[field] = base
+
+        if in_memory:
+            states.append(state)
+
+            if record_meta is None or record_meta is False:
+                meta.append(curr_meta)
+            else:
+                for field in record_meta:
+                    meta[field].append(curr_meta[field])
+
+        if queue is not None:
+            queue.put((chain_idx, state, curr_meta))
+
+    if (record_meta is None or record_meta is False) and in_memory:
+        meta = _s.numpy.mean(meta)
+
+    if queue is not None:
+        queue.put((chain_idx, None, None))
+
+    return meta, _s.numpy.array(states), markov_chain.state, rng.state
 
-    Draw ``n_samples`` from every passed chain in ``markov_chains`` 
-    using the respective random number generator from ``rngs``. 
+
+def _process_record_meta(
+    chain: MarkovChain, record_meta
+) -> _s.typing.Tuple[
+    _s.typing.List[str], _s.typing.List[_s.typing.List[int]], _s.typing.Dict[str, None]
+]:
+    shapes = []
+    missing_fields = {}
+    if isinstance(record_meta, list):
+        record_meta = record_meta.copy()
+        for field in record_meta:
+            if field != "acceptance_rate":
+                attrs = field.split(".")
+                base = chain
+
+                for attr in attrs:
+                    if hasattr(base, attr):
+                        base = getattr(base, attr)
+                    else:
+                        record_meta.remove(field)
+                        missing_fields[field] = None
+
+                if field not in missing_fields:
+                    shape = []
+                    if hasattr(base, "shape"):
+                        shape = [i for i in base.shape]
+                    shapes += [shape]
+    else:
+        shapes += [[]]
+    return record_meta, shapes, missing_fields
+
+
+def _parallel_sampling(
+    args: _s.typing.List[_s.typing.Any],
+    n_procs: int,
+    callback: _c.Callback,
+    progress_bar: bool,
+):
+    result_queue = (
+        _s.multiprocessing.Manager().Queue()
+        if callback is not None or progress_bar
+        else None
+    )
+    for i in range(len(args)):
+        args[i] += (result_queue,)
+
+    workers = _s.multiprocessing.Pool(n_procs - 1)
+    result = workers.starmap_async(_sample_parallel_chain, args)
+
+    if callback is not None or progress_bar:
+        pbars = (
+            [
+                _s.tqdm.trange(args[i][2], desc="chain {}".format(i))
+                for i in range(len(args))
+            ]
+            if progress_bar
+            else None
+        )
+        finished = [False for i in range(len(args))]
+        while not _s.numpy.all(finished):
+            chain_idx, state, meta = result_queue.get()
+            if state is not None:
+                if progress_bar:
+                    pbars[chain_idx].update()
+                if callback is not None:
+                    callback.record(
+                        chain_idx,
+                        state,
+                        meta if isinstance(meta, dict) else {"acceptance_rate": meta},
+                    )
+            else:
+                finished[chain_idx] = True
+                if progress_bar:
+                    pbars[chain_idx].close()
+
+        if callback is not None:
+            callback.finish()
+
+    workers.close()
+    workers.join()
+    return result.get()
+
+
+def sample(
+    markov_chains: _s.typing.Union[_c.MarkovChain, _s.typing.List[_c.MarkovChain]],
+    rngs: _s.typing.Union[
+        _c.RandomNumberGenerator, _s.typing.List[_c.RandomNumberGenerator]
+    ],
+    n_samples: int,
+    thinning: int = 1,
+    n_threads: int = 1,
+    n_procs: int = 1,
+    record_meta=None,
+    in_memory: bool = True,
+    callback: _c.Callback = None,
+    progress_bar: bool = False,
+):
+    r"""sample(markov_chains, rngs, n_samples, thinning=1, n_procs=1)
+
+    Draw ``n_samples`` from every passed chain in ``markov_chains``
+    using the respective random number generator from ``rngs``.
     Thus, ``len(rngs)`` has to match ``len(markov_chains)``.
 
     Parameters
     ----------
     markov_chains : list[hopsy.MarkovChain] or hopsy.MarkovChain
         (List of) Markov chain(s) to simulate to generate samples.
     rngs : list[hopsy.RandomNumberGenerator] or hopsy.RandomNumberGenerator
-        (List of) random number generator(s) to simulate the Markov chains. 
+        (List of) random number generator(s) to simulate the Markov chains.
         If a single :class:`hopsy.MarkovChain` was passed to ``sample``, then ``rng`` also must be a single
         :class:`hopsy.RandomNumberGenerator`.
     n_samples : int
         Number of samples to draw from every chain.
     thinning : int
-        Number of samples to discard inbetween two saved states. 
+        Number of samples to discard inbetween two saved states.
         This will increase the number of samples actually produced by the chain
         to ``thinning * n_samples``.
     n_threads : int
-        Number of parallel threads to use.
+        (deprecated) Number of parallel processes to use.
         Parallelization is achieved using ``multiprocessing``.
-        The worker pool size will be ``min(n_threads, len(markov_chains))``
+        The worker pool size will be ``min(n_procs, len(markov_chains))``
+    n_procs : int
+        Number of parallel processes to use.
+        Parallelization is achieved using ``multiprocessing``.
+        The worker pool size will be ``min(n_procs, len(markov_chains))``
     record_meta : list[str] or bool
         Strings defining :class:`hopsy.MarkovChain` attributes or ``acceptance_rate``, which will
         then be recorded and returned. All attributes of :class:`hopsy.MarkovChain` can be used here,
         e.g. ``record_meta=['state_negative_log_likelihood', 'proposal.proposal']``.
+    in_memory : bool
+        Flag for enabling or disabling in-memory saving of states and metadata.
+    callback : derived from hopsy.Callback
+        Observer callback to which states and metadata are passed during the run. The callback is e.g. used
+        to write the obtained information online to permanent storage. This enables online analysis of the
+        MCMC run.
 
     Returns
     -------
-    list or dict
-        Meta information about the states. Without using ``record_meta``,
-        this is a list containing the acceptance rates of each chain. 
-        If ``record_meta`` is used, then this is a dict containing the values of the :class:`hopsy.MarkovChain` 
+    optional[tuple[list or dict, numpy.ndarray]]
+        First value of the tuple holds meta information about the states. Without using ``record_meta``,
+        this is a list containing the acceptance rates of each chain.
+        If ``record_meta`` is used, then this is a dict containing the values of the :class:`hopsy.MarkovChain`
         attributes defined in ``record_meta``.
-        If the attribute was not found (e.g. because of a typo), then it will have value ``None``.
-    numpy.ndarray
-        The produced states. Will have shape ``(n_chains, n_draws, dim)``. For single chains, it will
+        If the attribute was not found (e.g. because of a typo), it will have value ``None``.
+
+        Second value of the tuple holds produced states. Will have shape ``(n_chains, n_draws, dim)``. For single chains, it will
         thus be ``(1, n_draws, dim)``.
 
+        If ``in_memory=False``, ``None`` will be returned.
+
     """
 
+    # multiprocessing and mpi (parallel tempering) do not work together yet
+    # because forked processes do not get a correct rank.
+    if n_procs != 1 and any(
+        [mc.parallelTemperingSyncRng is not None for mc in markov_chains]
+    ):
+        raise ValueError(
+            "n_procs>1 does not work together with parallel tempering with is based on mpi."
+        )
+
     # if both are lists, they have to match in size
-    if hasattr(markov_chains, "__len__") and hasattr(rngs, "__len__") and len(markov_chains) != len(rngs):
-        raise ValueError("Number of Markov chains has to match number of random number generators.")
+    if (
+        hasattr(markov_chains, "__len__")
+        and hasattr(rngs, "__len__")
+        and len(markov_chains) != len(rngs)
+    ):
+        raise ValueError(
+            "Number of Markov chains has to match number of random number generators."
+        )
 
     # if only one is a list, also fail
-    elif not (hasattr(markov_chains, "__len__") and hasattr(rngs, "__len__")) and (hasattr(markov_chains, "__len__") or hasattr(rngs, "__len__")):
-        raise ValueError("markov_chains and rngs have to be either both scalar or both lists with matching size.")
+    elif not (hasattr(markov_chains, "__len__") and hasattr(rngs, "__len__")) and (
+        hasattr(markov_chains, "__len__") or hasattr(rngs, "__len__")
+    ):
+        raise ValueError(
+            "markov_chains and rngs have to be either both scalar or both lists with matching size."
+        )
 
     if not hasattr(markov_chains, "__len__") and not hasattr(rngs, "__len__"):
         markov_chains = [markov_chains]
         rngs = [rngs]
 
-    result = []
-
+    # remove invalid entries from record_meta
+    record_meta, shapes, missing_fields = _process_record_meta(
+        markov_chains[0], record_meta
+    )
+
+    # initialize backend
+    if callback is not None:
+        meta_names = (
+            record_meta if isinstance(record_meta, list) else ["acceptance_rate"]
+        )
+        callback.setup(
+            len(markov_chains),
+            n_samples,
+            len(markov_chains[0].state),
+            meta_names,
+            shapes,
+        )
 
-    if n_threads != 1:
-        if n_threads < 0:
-            n_threads = min(len(markov_chains), _s.multiprocessing.cpu_count()) # do not use more threads than available cpus
+    result = []
 
-        with _s.multiprocessing.Pool(n_threads) as workers:
-            result = workers.starmap(_sample, [(markov_chains[i], rngs[i], n_samples, thinning, record_meta) for i in range(len(markov_chains))])
+    if n_procs != 1 or n_threads != 1:
+        if n_threads != n_procs and n_threads != 1:
+            n_procs = n_threads
+
+        if n_procs < 0:
+            n_procs = min(
+                len(markov_chains), _s.multiprocessing.cpu_count()
+            )  # do not use more procs than available cpus
+        result_states = _parallel_sampling(
+            [
+                (
+                    markov_chains[chain_idx],
+                    rngs[chain_idx],
+                    n_samples,
+                    thinning,
+                    chain_idx,
+                    in_memory,
+                    record_meta,
+                )
+                for chain_idx in range(len(markov_chains))
+            ],
+            n_procs,
+            callback,
+            progress_bar,
+        )
+        for i, chain_result in enumerate(result_states):
+            result.append((chain_result[0], chain_result[1]))
+            markov_chains[i].state = chain_result[2]
+            rngs[i].state = chain_result[3]
     else:
-        for i in range(len(markov_chains)):
-            _accrates, _states = _sample(markov_chains[i], rngs[i], n_samples, thinning, record_meta)
+        for chain_idx in range(len(markov_chains)):
+            _accrates, _states = _sequential_sampling(
+                markov_chains[chain_idx],
+                rngs[chain_idx],
+                n_samples,
+                thinning,
+                chain_idx,
+                in_memory,
+                record_meta,
+                callback,
+                progress_bar,
+            )
             result.append((_accrates, _states))
 
+    if in_memory:
+        states = []
+        meta = (
+            []
+            if record_meta is None or record_meta is False
+            else {field: [] for field in record_meta}
+        )
 
-    states = []
-    meta = [] if record_meta is None or record_meta is False else {field: [] for field in record_meta}
+        for _meta, _states in result:
+            states.append(_states)
 
-    for _meta, _states in result:
-        states.append(_states)
-        
-        if record_meta is None or record_meta is False:
-            meta.append(_meta)
-        else:
+            if record_meta is None or record_meta is False:
+                meta.append(_meta)
+            else:
+                for field in meta:
+                    meta[field].append(_meta[field])
+
+        if record_meta is not None and record_meta is not False:
             for field in meta:
-                meta[field].append(_meta[field])
+                meta[field] = _s.numpy.array(meta[field])
+            meta.update(missing_fields)
 
-    if record_meta is not None and record_meta is not False:
-        for field in meta:
-            all_none = True
-            for val in meta[field]:
-                if val is not None:
-                    all_none = False
+        return meta, _s.numpy.array(states)
 
-            if all_none:
-                meta[field] = None
-            else:
-                meta[field] = _s.numpy.array(meta[field])
 
-    return meta, _s.numpy.array(states)
+def _parallel_execution(
+    func: _s.typing.Callable, args: _s.typing.List[_s.typing.Any], n_procs: int
+):
+    with _s.multiprocessing.Pool(n_procs) as workers:
+        return workers.starmap(func, args)
+
 
 def _is_constant_chains(data: _s.numpy.typing.ArrayLike):
     data = _s.numpy.array(data)
     assert len(data.shape) == 3
     return _s.numpy.sum(_s.numpy.abs(_s.numpy.diff(data, axis=1))) == 0
 
 
-def _arviz(f: _s.typing.Callable,
-           data: _s.numpy.typing.ArrayLike,
-           series: int = 0,
-           *args, **kwargs):
+def _compute_statistic(
+    i: int,
+    n_chains: int,
+    dim: int,
+    f: _s.typing.Callable,
+    data: _s.numpy.typing.ArrayLike,
+    args,
+    kwargs,
+):
+    # if chains are constant, ess = 1, no matter what
+    if _is_constant_chains(data[:, :i]) and f == _s.arviz.ess:
+        relative = (
+            args[3]
+            if len(args) > 4
+            else kwargs["relative"]
+            if "relative" in kwargs
+            else False
+        )
+        return [1 / (n_chains * i) if relative else 1] * dim
+    else:
+        return f(_s.arviz.convert_to_inference_data(data[:, :i]), **kwargs).x.data
+
+
+def _arviz(
+    f: _s.typing.Callable,
+    data: _s.numpy.typing.ArrayLike,
+    series: int = 0,
+    n_procs: int = 1,
+    *args,
+    **kwargs
+):
     data = _s.numpy.array(data)
     assert len(data.shape) == 3
     n_chains, n_samples, dim = data.shape
     result = []
+
     if series:
-        i = series
-        while i <= n_samples:
-            # if chains are constant, ess = 1, no matter what
-            if _is_constant_chains(data[:,:i]) and f == _s.arviz.ess:
-                relative = args[3] if len(args) > 4 else kwargs['relative'] if 'relative' in kwargs else False
-                _result = [1 / (n_chains*i) if relative else 1] * dim
-            else:
-                _result = f(_s.arviz.convert_to_inference_data(data[:,:i]), *args, **kwargs).x.data
-            result.append(_result)
-            i += series
+        if n_procs != 1:
+            indices = list(range(series, n_samples, series))
+            if n_procs < 0:
+                n_procs = min(
+                    len(indices), _s.multiprocessing.cpu_count()
+                )  # do not use more processes than available cpus
+            result = _parallel_execution(
+                _compute_statistic,
+                [(i, n_chains, dim, f, data, args, kwargs) for i in indices],
+                n_procs,
+            )
+        else:
+            i = series
+            while i <= n_samples:
+                result.append(
+                    _compute_statistic(i, n_chains, dim, f, data, args, kwargs)
+                )
+                i += series
     else:
         if _is_constant_chains(data) and f == _s.arviz.ess:
-            relative = args[3] if len(args) > 4 else kwargs['relative'] if 'relative' in kwargs else False
-            _result = [1 / (n_chains*n_samples) if relative else 1] * dim
+            relative = (
+                args[3]
+                if len(args) > 4
+                else kwargs["relative"]
+                if "relative" in kwargs
+                else False
+            )
+            _result = [1 / (n_chains * n_samples) if relative else 1] * dim
         else:
-            _result = f(_s.arviz.convert_to_inference_data(data), *args, **kwargs).x.data
+            _result = f(
+                _s.arviz.convert_to_inference_data(data), *args, **kwargs
+            ).x.data
         result.append(_result)
 
     return _s.numpy.array(result)
 
 
 def ess(*args, **kwargs):
     r"""ess(data, series=0, method="bulk", relative=False, prob=None, dask_kwargs=None)
 
-        Calculate estimate of the effective sample size (ess).
+    Calculate estimate of the effective sample size (ess).
+
+    Parameters
+    ----------
+    data : numpy.ndarray
+        MCMC samples with ``data.shape == (n_chains, n_draws, dim)``.
+    series : int
+        Compute a series of effective sample sizes every ``series`` samples,
+        so ess will be computed for ``data[:,:n] for n in range(series, n_draws+1, series)``.
+        For the default value ``series==0``, ess will be computed only once for the whole data.
+    method : str
+        Select ess method. Valid methods are:
+
+        - "bulk"
+        - "tail"     # prob, optional
+        - "quantile" # prob
+        - "mean" (old ess)
+        - "sd"
+        - "median"
+        - "mad" (mean absolute deviance)
+        - "z_scale"
+        - "folded"
+        - "identity"
+        - "local"
+    relative : bool
+        Return relative ess
+        `ress = ess / n`
+    prob : float, or tuple of two floats, optional
+        probability value for "tail", "quantile" or "local" ess functions.
+    n_procs : int = 1
+        In combination with "series": compute series of ess in parallel using ``n_procs``
+        subprocesses.
+    dask_kwargs : dict, optional
+        Dask related kwargs passed to :func:`~arviz.wrap_xarray_ufunc`.
+
+    Returns
+    -------
+    numpy.ndarray
+        Return the effective sample size, :math:`\hat{N}_{eff}`
+
+    Notes
+    -----
+    The basic ess (:math:`N_{\mathit{eff}}`) diagnostic is computed by:
+
+    .. math:: \hat{N}_{\mathit{eff}} = \frac{MN}{\hat{\tau}}
+
+    .. math:: \hat{\tau} = -1 + 2 \sum_{t'=0}^K \hat{P}_{t'}
+
+    where :math:`M` is the number of chains, :math:`N` the number of draws,
+    :math:`\hat{\rho}_t` is the estimated _autocorrelation at lag :math:`t`, and
+    :math:`K` is the last integer for which :math:`\hat{P}_{K} = \hat{\rho}_{2K} +
+    \hat{\rho}_{2K+1}` is still positive.
+
+    The current implementation is similar to Stan, which uses Geyer's initial monotone sequence
+    criterion (Geyer, 1992; Geyer, 2011).
 
-        Parameters
-        ----------
-        data : numpy.ndarray
-            MCMC samples with ``data.shape == (n_chains, n_draws, dim)``.
-        series : int
-            Compute a series of effective sample sizes every ``series`` samples,
-            so ess will be computed for ``data[:,:n] for n in range(series, n_draws+1, series)``.
-            For the default value ``series==0``, ess will be computed only once for the whole data.
-        method : str
-            Select ess method. Valid methods are:
-
-            - "bulk"
-            - "tail"     # prob, optional
-            - "quantile" # prob
-            - "mean" (old ess)
-            - "sd"
-            - "median"
-            - "mad" (mean absolute deviance)
-            - "z_scale"
-            - "folded"
-            - "identity"
-            - "local"
-        relative : bool
-            Return relative ess
-            `ress = ess / n`
-        prob : float, or tuple of two floats, optional
-            probability value for "tail", "quantile" or "local" ess functions.
-        dask_kwargs : dict, optional
-            Dask related kwargs passed to :func:`~arviz.wrap_xarray_ufunc`.
-
-        Returns
-        -------
-        numpy.ndarray
-            Return the effective sample size, :math:`\hat{N}_{eff}`
-
-        Notes
-        -----
-        The basic ess (:math:`N_{\mathit{eff}}`) diagnostic is computed by:
-
-        .. math:: \hat{N}_{\mathit{eff}} = \frac{MN}{\hat{\tau}}
-
-        .. math:: \hat{\tau} = -1 + 2 \sum_{t'=0}^K \hat{P}_{t'}
-
-        where :math:`M` is the number of chains, :math:`N` the number of draws,
-        :math:`\hat{\rho}_t` is the estimated _autocorrelation at lag :math:`t`, and
-        :math:`K` is the last integer for which :math:`\hat{P}_{K} = \hat{\rho}_{2K} +
-        \hat{\rho}_{2K+1}` is still positive.
-
-        The current implementation is similar to Stan, which uses Geyer's initial monotone sequence
-        criterion (Geyer, 1992; Geyer, 2011).
-
-        References
-        ----------
-        * Vehtari et al. (2019) see https://arxiv.org/abs/1903.08008
-        * https://arviz-devs.github.io/arviz/api/generated/arviz.ess.html
-        * https://mc-stan.org/docs/2_18/reference-manual/effective-sample-size-section.html
-          Section 15.4.2
-        * Gelman et al. BDA (2014) Formula 11.8
+    References
+    ----------
+    * Vehtari et al. (2019) see https://arxiv.org/abs/1903.08008
+    * https://arviz-devs.github.io/arviz/api/generated/arviz.ess.html
+    * https://mc-stan.org/docs/2_18/reference-manual/effective-sample-size-section.html
+      Section 15.4.2
+    * Gelman et al. BDA (2014) Formula 11.8
 
     """
     return _arviz(_s.arviz.ess, *args, **kwargs)
 
 
 def mcse(*args, **kwargs):
     r"""mcse(data, series=0, method="mean", prob=None, dask_kwargs=None)
 
-        Calculate Markov Chain Standard Error statistic.
+    Calculate Markov Chain Standard Error statistic.
+
+    Parameters
+    ----------
+    data : numpy.ndarray
+        MCMC samples with ``data.shape == (n_chains, n_draws, dim)``.
+    series : int
+        Compute a series of statistics every ``series`` samples,
+        so mcse will be computed for ``data[:,:n] for n in range(series, n_draws+1, series)``.
+        For the default value ``series==0``, mcse will be computed only once for the whole data.
+    method : str
+        Select mcse method. Valid methods are:
+        - "mean"
+        - "sd"
+        - "median"
+        - "quantile"
+
+    prob : float
+        Quantile information.
+    n_procs : int = 1
+        In combination with "series": compute series of mcse in parallel using ``n_procs``
+        subprocesses.
+    dask_kwargs : dict, optional
+        Dask related kwargs passed to :func:`~arviz.wrap_xarray_ufunc`.
+
+    Returns
+    -------
+    numpy.ndarray
+        Return the msce dataset
 
-        Parameters
-        ----------
-        data : numpy.ndarray
-            MCMC samples with ``data.shape == (n_chains, n_draws, dim)``.
-        series : int
-            Compute a series of statistics every ``series`` samples,
-            so mcse will be computed for ``data[:,:n] for n in range(series, n_draws+1, series)``.
-            For the default value ``series==0``, mcse will be computed only once for the whole data.
-        method : str
-            Select mcse method. Valid methods are:
-            - "mean"
-            - "sd"
-            - "median"
-            - "quantile"
-
-        prob : float
-            Quantile information.
-        dask_kwargs : dict, optional
-            Dask related kwargs passed to :func:`~arviz.wrap_xarray_ufunc`.
-
-        Returns
-        -------
-        numpy.ndarray
-            Return the msce dataset
-
-        References
-        ----------
-        * https://arviz-devs.github.io/arviz/api/generated/arviz.mcse.html
+    References
+    ----------
+    * https://arviz-devs.github.io/arviz/api/generated/arviz.mcse.html
 
     """
     return _arviz(_s.arviz.mcse, *args, **kwargs)
 
 
 def rhat(*args, **kwargs):
     r"""rhat(data, series=0, method="rank", dask_kwargs=None)
 
-        Compute estimate of rank normalized splitR-hat for a set of traces.
+    Compute estimate of rank normalized splitR-hat for a set of traces.
 
-        The rank normalized R-hat diagnostic tests for lack of convergence by comparing the variance
-        between multiple chains to the variance within each chain. If convergence has been achieved,
-        the between-chain and within-chain variances should be identical. To be most effective in
-        detecting evidence for nonconvergence, each chain should have been initialized to starting
-        values that are dispersed relative to the target distribution.
-
-        Parameters
-        ----------
-        data : numpy.ndarray
-            MCMC samples with ``data.shape == (n_chains, n_draws, dim)``.
-        series : int
-            Compute a series of R-hat statistics every ``series`` samples,
-            so R-hat will be computed for ``data[:,:n] for n in range(series, n_draws+1, series)``.
-            For the default value ``series==0``, R-hat will be computed only once for the whole data.
-        method : str
-            Select R-hat method. Valid methods are:
-            - "rank"        # recommended by Vehtari et al. (2019)
-            - "split"
-            - "folded"
-            - "z_scale"
-            - "identity"
-        dask_kwargs : dict
-            Dask related kwargs passed to :func:`~arviz.wrap_xarray_ufunc`.
-
-        Returns
-        -------
-        numpy.ndarray
-          Returns dataset of the potential scale reduction factors, :math:`\hat{R}`
-
-        Notes
-        -----
-        The diagnostic is computed by:
-
-          .. math:: \hat{R} = \frac{\hat{V}}{W}
-
-        where :math:`W` is the within-chain variance and :math:`\hat{V}` is the posterior variance
-        estimate for the pooled rank-traces. This is the potential scale reduction factor, which
-        converges to unity when each of the traces is a sample from the target posterior. Values
-        greater than one indicate that one or more chains have not yet converged.
-
-        Rank values are calculated over all the chains with `scipy.stats.rankdata`.
-        Each chain is split in two and normalized with the z-transform following Vehtari et al. (2019).
-
-        References
-        ----------
-        * Vehtari et al. (2019) see https://arxiv.org/abs/1903.08008
-        * Gelman et al. BDA (2014)
-        * Brooks and Gelman (1998)
-        * Gelman and Rubin (1992)
-        * https://arviz-devs.github.io/arviz/api/generated/arviz.rhat.html
+    The rank normalized R-hat diagnostic tests for lack of convergence by comparing the variance
+    between multiple chains to the variance within each chain. If convergence has been achieved,
+    the between-chain and within-chain variances should be identical. To be most effective in
+    detecting evidence for nonconvergence, each chain should have been initialized to starting
+    values that are dispersed relative to the target distribution.
 
-    """
-    return _arviz(_s.arviz.rhat, *args, **kwargs)
+    Parameters
+    ----------
+    data : numpy.ndarray
+        MCMC samples with ``data.shape == (n_chains, n_draws, dim)``.
+    series : int
+        Compute a series of R-hat statistics every ``series`` samples,
+        so R-hat will be computed for ``data[:,:n] for n in range(series, n_draws+1, series)``.
+        For the default value ``series==0``, R-hat will be computed only once for the whole data.
+    method : str
+        Select R-hat method. Valid methods are:
+        - "rank"        # recommended by Vehtari et al. (2019)
+        - "split"
+        - "folded"
+        - "z_scale"
+        - "identity"
+    n_procs : int = 1
+        In combination with "series": compute series of R-hat in parallel using ``n_procs``
+        subprocesses.
+    dask_kwargs : dict
+        Dask related kwargs passed to :func:`~arviz.wrap_xarray_ufunc`.
+
+    Returns
+    -------
+    numpy.ndarray
+      Returns dataset of the potential scale reduction factors, :math:`\hat{R}`
+
+    Notes
+    -----
+    The diagnostic is computed by:
+
+      .. math:: \hat{R} = \frac{\hat{V}}{W}
+
+    where :math:`W` is the within-chain variance and :math:`\hat{V}` is the posterior variance
+    estimate for the pooled rank-traces. This is the potential scale reduction factor, which
+    converges to unity when each of the traces is a sample from the target posterior. Values
+    greater than one indicate that one or more chains have not yet converged.
 
+    Rank values are calculated over all the chains with `scipy.stats.rankdata`.
+    Each chain is split in two and normalized with the z-transform following Vehtari et al. (2019).
 
+    References
+    ----------
+    * Vehtari et al. (2019) see https://arxiv.org/abs/1903.08008
+    * Gelman et al. BDA (2014)
+    * Brooks and Gelman (1998)
+    * Gelman and Rubin (1992)
+    * https://arviz-devs.github.io/arviz/api/generated/arviz.rhat.html
+
+    """
+    return _arviz(_s.arviz.rhat, *args, **kwargs)
```

## Comparing `hopsy-1.1.0.dist-info/LICENSE` & `hopsy-1.2.0.dist-info/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2021 Richard Dominik Paul, Johann Fredrik Jadebeck, Katharina Nöh
+MIT License
+
+Copyright (c) 2023 The hopsy development team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -13,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `hopsy-1.1.0.dist-info/METADATA` & `hopsy-1.2.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: hopsy
-Version: 1.1.0
+Version: 1.2.0
 Summary: A python interface for hops, the highly optimized polytope sampling toolbox.
 Author: Richard D. Paul
 Author-email: r.paul@fz-juelich.de
-License: UNKNOWN
 Project-URL: Documentation, https://modsim.github.io/hopsy/
 Project-URL: Gitlab (Sources&CI), https://jugit.fz-juelich.de/IBG-1/ModSim/hopsy
 Project-URL: GitHub (Mirror), https://github.com/modsim/hopsy/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PolyRound
+Requires-Dist: PolyRound (==0.2.10)
+Requires-Dist: sympy (<1.12.0)
 Requires-Dist: arviz
-Requires-Dist: numpy
+Requires-Dist: numpy (<1.24.0)
+Requires-Dist: mcbackend
 Requires-Dist: pandas
 Requires-Dist: tqdm
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 
 # hopsy - Python bindings for HOPS
 
  [![pipeline status](https://jugit.fz-juelich.de/fluxomics/hopsy/badges/develop/pipeline.svg)](https://jugit.fz-juelich.de/fluxomics/hopsy/-/commits/develop)
  [![docstring coverage](https://jugit.fz-juelich.de/fluxomics/hopsy/-/jobs/220246/artifacts/raw/docs/docov.svg?job=test_release)](https://jugit.fz-juelich.de/fluxomics/hopsy/-/jobs/220246/artifacts/file/docs/docov.txt?job=test_release)
- 
+
 A python interface for HOPS - the **H**ighly **O**ptimized toolbox for **P**olytope **S**ampling.
 Built using `pybind11`
 
 <img src="docs/_static/hopsy.png" alt="HOPSY Logo" width="300"/>
 
 **hopsy** is a Python package for Markov chain Monte Carlo sampling on convex polytopes
- 
+
 P = {x : Ax &#8804; b},
 
 which often arises in metabolic flux analysis.
 
 
 
 ## Installation
@@ -58,89 +58,118 @@
 ```
 
 or use the standard CMake routine
 
 ```bash
 mkdir hopsy/cmake-build-release && cd hopsy/cmake-build-release
 cmake ..
-make 
+make
 ```
 
 Note however that the binary wheel produced from ``pip`` can be actually installed using ``pip``, using
 
 ```bash
 pip install hopsy-x.y.z-tag.whl
 ```
 
 where the version `x.y.z` and tag `tag` will depend on the verison you downloaded and your build environment.
-If you use the CMake routine, the compiled shared library will be located in `build/` and can 
-be used within the directory. 
+If you use the CMake routine, the compiled shared library will be located in `build/` and can
+be used within the directory.
 
 To compile binary wheels for distribution (e.g. via the Python Package Index pypi.org), use the `makewheels.sh` script.
 
 
 ### Prerequisites for compiling from source
 
 **On Unix (Linux, OS X)**
 
 * A compiler with C++11 support
 * CMake >= 3.4 or Pip 10+
 * Ninja or Pip 10+
 * Docker (optional, for building wheels)
 
+
+## MPI support for parallel tempering
+
+If you want to use the parallel tempering implemented in hops, you need a working MPI installation, because threads would not work due to the python GIL.
+The next step is to compile hopsy by source and to check that the script  examples/parallel\_tempering.py works.
+Both modes of the distribution should be found, otherwise there is some issue. In this case, please contact us.
+
+In order to use parallel tempering, python interpreter must be called with MPI:
+
+```
+mpirun -np 10 parallel_tempering_application.py
+```
+
+In this case, 10 parallel chains would be constructed.
+
+
 ## Examples
 
 A basic usage example is presented below. More examples can be found in `tests/` directory or in the docs.
 
 ```python
 import hopsy
 import matplotlib.pyplot as plt
 
-# the polytope is defined as 
+# the polytope is defined as
 #          P := {x : Ax <= b}
 # thus we need to define A and b. these constraints form the simple box [0,5]^2.
 A = [[1, 0], [0, 1], [-1, 0], [0, -1]]
 b = [5, 5, 0, 0]
 
 # next we construct a 2-dim standard Gaussian
 model = hopsy.Gaussian(dim=2)
 
-# the complete problem is defined by the target distribution and the constrained domain, 
+# the complete problem is defined by the target distribution and the constrained domain,
 # defined by the above mentioned inequality
 problem = hopsy.Problem(A, b, model)
 
 # the run object contains and constructs the markov chains. in the default case, the
 # Run object will have a single chain using the Hit-and-Run proposal algorithm and is
 # set to produce 10,000 samples.
 mc = hopsy.MarkovChain(problem, proposal=hopsy.GaussianHitAndRunProposal, starting_point=[.5, .5])
 rng = hopsy.RandomNumberGenerator(seed=42)
 
-# call sample on the mc and rng objects 
+# call sample on the mc and rng objects
 acceptance_rate, states = hopsy.sample(mc, rng, n_samples=10_000, thinning=2)
 
 # the states have 3 dimensions: number of chains, number of samples, number of dimensions.
 plt.scatter(states[:,:,0].flatten(), states[:,:,1].flatten())
 plt.show()
 ```
 
 <img src="docs/_static/gaussscatter.png" alt="2-dimensional truncated Gaussian scatter plot" width="600"/>
 
 
 [`cibuildwheel`]:          https://cibuildwheel.readthedocs.io
 [FAQ]: http://pybind11.rtfd.io/en/latest/faq.html#working-with-ancient-visual-studio-2009-builds-on-windows
 [vs2015_runtime]: https://www.microsoft.com/en-us/download/details.aspx?id=48145
 
+## Development
+
+The development of hopsy primarily takes place on (JuGit)[https://jugit.fz-juelich.de/IBG-1/ModSim/hopsy], where we have access to powerful continuous integration and a Docker registry. The GitHub repository is only a mirror, so please report issues and make pull requests on JuGit.
+Please install pre-commit before commiting to our repository, see pre-commit step in .gitlab-ci.yml.
+
+
+### Building docs & updading docs
+
+```
+docs-sources$ make html  # make will tell you which python packages you might be missing
+docs-sources$ rm ../docs/* -r
+docs-sources$ cp _build/html/* ../docs/ -r
+docs-sources$ git add ../ docs && git commit -m "updated docs" && git push  # and so on...
+```
+
+
 ## Links
 - Source Code & CI: https://jugit.fz-juelich.de/IBG-1/ModSim/hopsy
 - PyPI: https://pypi.org/project/hopsy/
 - Documentation: https://modsim.github.io/hopsy/
 - Github Mirror: https://github.com/modsim/hopsy
 - TestPyPI: https://test.pypi.org/project/hopsy/
 - HOPS (C++ backend): https://gitlab-public.fz-juelich.de/IBG-1/ModSim/hops
 
 
 ## License
 
 hopsy is licensed under the [MIT license](LICENSE).
-
-
-
```

