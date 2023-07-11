# Comparing `tmp/jijmodeling-1.0.0rc1-cp39-none-win_amd64.whl.zip` & `tmp/jijmodeling-1.0.0rc2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 745929 bytes, number of entries: 8
--rw-r--r--  4.6 unx     2702 b- defN 23-Jul-04 10:05 jijmodeling-1.0.0rc1.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jul-04 10:05 jijmodeling-1.0.0rc1.dist-info/WHEEL
--rw-r--r--  4.6 unx     3445 b- defN 23-Jul-04 10:05 jijmodeling-1.0.0rc1.dist-info/license_files/LICENSE.txt
--rw-r--r--  4.6 unx      127 b- defN 23-Jul-04 10:05 jijmodeling/__init__.py
--rw-r--r--  4.6 unx    80303 b- defN 23-Jul-04 10:05 jijmodeling/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Jul-04 10:05 jijmodeling/py.typed
--rwxr-xr-x  4.6 unx  2174464 b- defN 23-Jul-04 10:05 jijmodeling/jijmodeling.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      677 b- defN 23-Jul-04 10:05 jijmodeling-1.0.0rc1.dist-info/RECORD
-8 files, 2261812 bytes uncompressed, 744745 bytes compressed:  67.1%
+Zip file size: 740811 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2702 b- defN 23-Jul-11 02:43 jijmodeling-1.0.0rc2.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-11 02:43 jijmodeling-1.0.0rc2.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3445 b- defN 23-Jul-11 02:43 jijmodeling-1.0.0rc2.dist-info/license_files/LICENSE.txt
+-rw-r--r--  4.6 unx      127 b- defN 23-Jul-11 02:43 jijmodeling/__init__.py
+-rw-r--r--  4.6 unx    81515 b- defN 23-Jul-11 02:43 jijmodeling/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-11 02:43 jijmodeling/py.typed
+-rwxr-xr-x  4.6 unx  2157568 b- defN 23-Jul-11 02:43 jijmodeling/jijmodeling.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      677 b- defN 23-Jul-11 02:43 jijmodeling-1.0.0rc2.dist-info/RECORD
+8 files, 2246128 bytes uncompressed, 739627 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: jijmodeling-1.0.0rc1.dist-info/METADATA
+Filename: jijmodeling-1.0.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: jijmodeling-1.0.0rc1.dist-info/WHEEL
+Filename: jijmodeling-1.0.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: jijmodeling-1.0.0rc1.dist-info/license_files/LICENSE.txt
+Filename: jijmodeling-1.0.0rc2.dist-info/license_files/LICENSE.txt
 Comment: 
 
 Filename: jijmodeling/__init__.py
 Comment: 
 
 Filename: jijmodeling/__init__.pyi
 Comment: 
 
 Filename: jijmodeling/py.typed
 Comment: 
 
 Filename: jijmodeling/jijmodeling.cp39-win_amd64.pyd
 Comment: 
 
-Filename: jijmodeling-1.0.0rc1.dist-info/RECORD
+Filename: jijmodeling-1.0.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jijmodeling/__init__.pyi

```diff
@@ -161,14 +161,15 @@
         >>> x = jm.BinaryVar("x", shape=[2, 2])
     
         Create a 1-dimensional binary variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.BinaryVar("x", shape=[124])
         >>> x[123]
+        BinaryVar(name='x', shape=[NumberLit(value=124)])[NumberLit(value=123)]
     """
     def __init__(name: str, *, shape=None, latex=None, description=None):
         pass
 
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
@@ -231,74 +232,74 @@
     
     Expression:
         Create an equality constraint that the sum of $N$ binary variables is equal to one.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
-        >>> x = jm.BinaryVar("x", ndim=1)
+        >>> x = jm.BinaryVar("x", shape=(N,))
         >>> jm.Constraint("constraint", jm.sum(i, x[i]) == 1)
+        {'expression': sum(i in [0..N), x[i]) == 1}
     
         Create an inequality constraint with forall.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
-        >>> x = jm.BinaryVar("x", ndim=2)
+        >>> x = jm.BinaryVar("x", shape=(N, N))
         >>> jm.Constraint("constraint", jm.sum(i, x[i,j]) == 1, forall=j)
+        {'expression': sum(i in [0..N), x[i, j]) == 1, 'forall': [j]}
     
         Create an inequality constraint with conditional forall.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
-        >>> x = jm.BinaryVar("x", ndim=2)
+        >>> x = jm.BinaryVar("x", shape=(N, N))
         >>> jm.Constraint("constraint", x[i,j] <= 2, forall=[i, (j, j != i)])
+        {'expression': x[i, j] <= 2, 'forall': [i, (j, j != i)]}
+        
     """
     def __init__(name: str, expression, *, forall=None):
         pass
 
     def is_equality(self, /):
         """
         Returns true if the constraint is an equality constraint.
         
         Returns:
             bool: True if the constraint is an equality constraint. Otherwise, False.
         
         Examples:
-            ```python
             >>> import jijmodeling as jm
             >>> N = jm.Placeholder("N")
             >>> i = jm.Element("i", belong_to=N)
             >>> x = jm.BinaryVar("x", shape=(N,))
             >>> constraint = jm.Constraint("constraint", jm.sum(i, x[i]) == 1)
             >>> assert constraint.is_equality()
-            ```
         """
         pass
 
 
     def is_inequality(self, /):
         """
         Returns true if the constraint is an inequality constraint.
         
         Returns:
             bool: True if the constraint is an inequality constraint. Otherwise, False.
         
         Examples:
-            ```python
             >>> import jijmodeling as jm
             >>> N = jm.Placeholder("N")
             >>> i = jm.Element("i", belong_to=N)
             >>> x = jm.BinaryVar("x", shape=(N,))
             >>> constraint = jm.Constraint("constraint", jm.sum(i, x[i]) <= 1)
             >>> assert constraint.is_inequality()
-            ```
         """
         pass
 
 
 @typing.final
 class ConstraintSense:
     """
@@ -357,14 +358,15 @@
         >>> x = jm.ContinuousVar("x", shape=[2, 2], lower_bound=0, upper_bound=2)
     
         Create a 1-dimensional continuous variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.ContinuousVar("x", shape=[124], lower_bound=0, upper_bound=2)
         >>> x[123]
+        ContinuousVar(name='x', shape=[NumberLit(value=124)], lower_bound=NumberLit(value=0), upper_bound=NumberLit(value=2))[NumberLit(value=123)]
     """
     def __init__(name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
         pass
 
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
@@ -398,34 +400,37 @@
     
     Expression:
         Create a custom penalty term.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
-        >>> x = jm.BinaryVar("x", ndim=1)
-        >>> jm.CustomPenaltyTerm("custom penalty term", (jm.sum(i, x[i]) - 1)**2)
+        >>> x = jm.BinaryVar("x", shape=(N,))
+        >>> jm.CustomPenaltyTerm("custom penalty term", (jm.sum(i, x[i]) - 1)**2)  # doctest: +ELLIPSIS
+        <jijmodeling.CustomPenaltyTerm object at 0x...>
     
         Create a custom penalty term with forall.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
-        >>> x = jm.BinaryVar("x", ndim=2)
-        >>> jm.CustomPenaltyTerm("custom penalty term", (jm.sum(i, x[i,j]) - 1)**2, forall=j)
+        >>> x = jm.BinaryVar("x", shape=(N, N))
+        >>> jm.CustomPenaltyTerm("custom penalty term", (jm.sum(i, x[i,j]) - 1)**2, forall=j)  # doctest: +ELLIPSIS
+        <jijmodeling.CustomPenaltyTerm object at 0x...>
     
         Create a custom penalty term with conditional forall.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
-        >>> x = jm.BinaryVar("x", ndim=2)
-        >>> jm.CustomPenaltyTerm("custom penalty term", (x[i,j] - 2)**2, forall=(j, j != i))
+        >>> x = jm.BinaryVar("x", shape=(N, N))
+        >>> jm.CustomPenaltyTerm("custom penalty term", (x[i,j] - 2)**2, forall=[i, (j, j != i)])  # doctest: +ELLIPSIS
+        <jijmodeling.CustomPenaltyTerm object at 0x...>
     """
     def __init__(name: str, expression, *, forall=None):
         pass
 
 @typing.final
 class DataType:
     """
@@ -485,14 +490,15 @@
     
         Create a 1-dimensional element with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a", ndim=2)
         >>> e = jm.Element("e", belong_to=a)
         >>> e[123]
+        Element(name='e', belong_to=Placeholder(name='a', ndim=2))[NumberLit(value=123)]
     """
     def __init__(name: str, *, belong_to, latex=None, description=None):
         pass
 
     def len_at(self, /, axis, *, latex=None, description=None):
         """
         
@@ -752,14 +758,15 @@
         >>> x = jm.IntegerVar("x", shape=[2, 2], lower_bound=0, upper_bound=2)
     
         Create a 1-dimensional integer variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.IntegerVar("x", shape=[124], lower_bound=0, upper_bound=2)
         >>> x[123]
+        IntegerVar(name='x', shape=[NumberLit(value=124)], lower_bound=NumberLit(value=0), upper_bound=NumberLit(value=2))[NumberLit(value=123)]
     """
     def __init__(name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
         pass
 
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
@@ -1147,20 +1154,20 @@
     
     The NumberLit class is used to create a number literal.
     Its instance is automatically generated by the return value of
     arithmetic or mathematical functions taking a number literal and
     an object defined by jijmodeling as arguments.
     
     Attributes:
-        value (tuple[int, float]): A numeric value.
+        value (int | float): A numeric value.
         dtype (:obj:`DataType`): A type of the value.
             `dtype` is `DataType.INTEGER` if the type of the value is integer else `dtype` is `DataType.FLOAT`.
     
     Args:
-        value (tuple[int, float]): A numeric value.
+        value (int | float): A numeric value.
     
     Examples:
         Create a number literal with a integer value `123`.
     
         >>> import jijmodeling as jm
         >>> v = jm.NumberLit(123)
         >>> assert v.value == 123
@@ -1244,14 +1251,15 @@
         >>> m = jm.Placeholder("m", ndim=2)
     
         Create a 1-dimensional placeholder with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a", ndim=2)
         >>> a[123]
+        Placeholder(name='a', ndim=2)[NumberLit(value=123)]
     """
     def __init__(name: str, *, ndim=0, latex=None, description=None):
         pass
 
     def len_at(self, /, axis, *, latex=None, description=None):
         """
         
@@ -1776,14 +1784,15 @@
         >>> x = jm.SemiContinuousVar("x", shape=[2, 2], lower_bound=0, upper_bound=2)
     
         Create a 1-dimensional semi-continuous variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.SemiContinuousVar("x", shape=[124], lower_bound=0, upper_bound=2)
         >>> x[123]
+        SemiContinuousVar(name='x', shape=[NumberLit(value=124)], lower_bound=NumberLit(value=0), upper_bound=NumberLit(value=2))[NumberLit(value=123)]
     """
     def __init__(name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
         pass
 
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
@@ -1845,14 +1854,15 @@
         >>> x = jm.SemiIntegerVar("x", shape=[2, 2], lower_bound=0, upper_bound=2)
     
         Create a 1-dimensional semi-integer variable with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> x = jm.SemiIntegerVar("x", shape=[124], lower_bound=0, upper_bound=2)
         >>> x[123]
+        SemiIntegerVar(name='x', shape=[NumberLit(value=124)], lower_bound=NumberLit(value=0), upper_bound=NumberLit(value=2))[NumberLit(value=123)]
     """
     def __init__(name: str, *, shape=None, lower_bound, upper_bound, latex=None, description=None):
         pass
 
     def set_latex(self, /, latex=None):
         """
         Set the LaTeX representation of the object.
```

## Comparing `jijmodeling-1.0.0rc1.dist-info/METADATA` & `jijmodeling-1.0.0rc2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jijmodeling
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

## Comparing `jijmodeling-1.0.0rc1.dist-info/license_files/LICENSE.txt` & `jijmodeling-1.0.0rc2.dist-info/license_files/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `jijmodeling-1.0.0rc1.dist-info/RECORD` & `jijmodeling-1.0.0rc2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jijmodeling-1.0.0rc1.dist-info/METADATA,sha256=kqpu8l5ycqfhBrYMxLdeZG7o9xSBq_xUyrGQTDXGF7w,2702
-jijmodeling-1.0.0rc1.dist-info/WHEEL,sha256=AEr5m1XkYiXdLchbOjtn7VSjoPs_2BeqH39awFrbrB0,94
-jijmodeling-1.0.0rc1.dist-info/license_files/LICENSE.txt,sha256=llUjgcEN5bUeFlj1RqxJxDMxUnlYvowLsldCF6Lwq8c,3445
+jijmodeling-1.0.0rc2.dist-info/METADATA,sha256=fSd2X1GtPK6PoSf89EL-TL15zhJsLgs_Y6DKiuOkrfA,2702
+jijmodeling-1.0.0rc2.dist-info/WHEEL,sha256=AEr5m1XkYiXdLchbOjtn7VSjoPs_2BeqH39awFrbrB0,94
+jijmodeling-1.0.0rc2.dist-info/license_files/LICENSE.txt,sha256=llUjgcEN5bUeFlj1RqxJxDMxUnlYvowLsldCF6Lwq8c,3445
 jijmodeling/__init__.py,sha256=dTz5lvd2qXlLmjsXX3Pq7v2_dptMkGNTWIf37gSrvwE,127
-jijmodeling/__init__.pyi,sha256=PXo4-Fga_YeFm46Dq_l6qjaId-Ij8uCl13368MCFKeE,80303
+jijmodeling/__init__.pyi,sha256=Oz7Eag915tlPXSnkVcQcJPPJrUt12MHQDFFvF3n_mY0,81515
 jijmodeling/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-jijmodeling/jijmodeling.cp39-win_amd64.pyd,sha256=4o1d0tbnAvpRC4kzBavCLFqYYnwUaOJrILfq5FG4-Bg,2174464
-jijmodeling-1.0.0rc1.dist-info/RECORD,,
+jijmodeling/jijmodeling.cp39-win_amd64.pyd,sha256=Xx2j5n_4m79uQAj0GsK4sMaIlQIJMKb5-d0E5enTx9g,2157568
+jijmodeling-1.0.0rc2.dist-info/RECORD,,
```

