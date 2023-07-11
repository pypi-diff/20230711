# Comparing `tmp/py-datalab-0.2.2.tar.gz` & `tmp/py-datalab-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-datalab-0.2.2.tar", last modified: Fri Jul  7 17:09:24 2023, max compression
+gzip compressed data, was "py-datalab-0.2.3.tar", last modified: Tue Jul 11 08:40:23 2023, max compression
```

## Comparing `py-datalab-0.2.2.tar` & `py-datalab-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:09:24.693171 py-datalab-0.2.2/
--rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      802 2023-07-07 17:09:24.693171 py-datalab-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2860 2023-07-07 04:02:41.000000 py-datalab-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 17:09:24.669239 py-datalab-0.2.2/datalab/
--rw-rw-rw-   0        0        0    20812 2023-07-07 16:49:22.000000 py-datalab-0.2.2/datalab/Matrix.py
--rw-rw-rw-   0        0        0    12648 2023-07-07 15:11:17.000000 py-datalab-0.2.2/datalab/Vector.py
--rw-rw-rw-   0        0        0      204 2023-07-07 17:04:55.000000 py-datalab-0.2.2/datalab/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-07-07 16:59:02.000000 py-datalab-0.2.2/datalab/functions.py
--rw-rw-rw-   0        0        0     2110 2023-07-07 15:05:10.000000 py-datalab-0.2.2/datalab/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:09:24.691170 py-datalab-0.2.2/py_datalab.egg-info/
--rw-rw-rw-   0        0        0      802 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 17:09:24.694169 py-datalab-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1059 2023-07-07 17:09:20.000000 py-datalab-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:40:23.111597 py-datalab-0.2.3/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      802 2023-07-11 08:40:23.109590 py-datalab-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2860 2023-07-07 04:02:41.000000 py-datalab-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 08:40:23.083366 py-datalab-0.2.3/datalab/
+-rw-rw-rw-   0        0        0    27910 2023-07-11 08:39:26.000000 py-datalab-0.2.3/datalab/Matrix.py
+-rw-rw-rw-   0        0        0    12648 2023-07-07 15:11:17.000000 py-datalab-0.2.3/datalab/Vector.py
+-rw-rw-rw-   0        0        0      204 2023-07-07 17:04:55.000000 py-datalab-0.2.3/datalab/__init__.py
+-rw-rw-rw-   0        0        0     6720 2023-07-07 16:59:02.000000 py-datalab-0.2.3/datalab/functions.py
+-rw-rw-rw-   0        0        0     2110 2023-07-11 06:36:46.000000 py-datalab-0.2.3/datalab/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:40:23.107085 py-datalab-0.2.3/py_datalab.egg-info/
+-rw-rw-rw-   0        0        0      802 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 08:40:23.111597 py-datalab-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2023-07-11 08:39:53.000000 py-datalab-0.2.3/setup.py
```

### Comparing `py-datalab-0.2.2/LICENSE` & `py-datalab-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.2/PKG-INFO` & `py-datalab-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.2.2
+Version: 0.2.3
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.2.2/README.md` & `py-datalab-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.2/datalab/Matrix.py` & `py-datalab-0.2.3/datalab/Matrix.py`

 * *Files 17% similar despite different names*

```diff
@@ -304,40 +304,32 @@
 
         if exponent < 0:
             raise ValueError(
                 "Matrix exponentiation is not supported for negative exponents"
             )
 
         if exponent == 0:
-            return buffer.identity()
+            if self.rows != self.columns:
+                raise ValueError(
+                    "Identity matrix must have same rows and columns number"
+                )
+
+            return Matrix(
+                [
+                    [1 if i == j else 0 for j in range(self.rows)]
+                    for i in range(self.rows)
+                ],
+                dtype=self.dtype,
+            )
 
         for _ in range(exponent - 1):
             buffer *= self
 
         return buffer
 
-    def _estimate_data_type(self, object: Iterable) -> type:
-        type_counts = {int: 0, float: 0, str: 0, bool: 0}
-
-        for row in object:
-            for element in row:
-                if isinstance(element, int):
-                    type_counts[int] += 1
-                elif isinstance(element, float):
-                    type_counts[float] += 1
-                elif isinstance(element, str):
-                    type_counts[str] += 1
-                elif isinstance(element, bool):
-                    type_counts[bool] += 1
-
-        if type_counts[int] > 0 and type_counts[float] > 0:
-            return float
-        else:
-            return max(type_counts, key=type_counts.get)
-
     def _fill_data(
         self,
         object: Optional[Iterable] = None,
         fill: Optional[Union[int, float, str, bool]] = None,
     ) -> None:
         empty_element = self._empty_element() if fill is None else fill
 
@@ -349,14 +341,27 @@
             for i, row in enumerate(object):
                 for j, element in enumerate(row):
                     try:
                         self.__data[i][j] = element
                     except IndexError:
                         self.__data[i][j] = empty_element
 
+    def _empty_element(self) -> Union[int, float, str, bool]:
+        if self.dtype == float:
+            return 0.0
+
+        elif self.dtype == str:
+            return ""
+
+        elif self.dtype == bool:
+            return False
+
+        else:
+            return 0
+
     def _initialize_data_structure(
         self,
         object: Optional[Iterable] = None,
         shape: Optional[tuple[int, int]] = None,
         dtype: Optional[type] = None,
         fill: Optional[Union[int, float, str, bool]] = None,
     ) -> None:
@@ -378,50 +383,32 @@
             self._fill_data(fill=fill)
 
         else:
             raise ValueError(
                 "Matrix._initilize_data_structure() has recived wrong parameters"
             )
 
-    def _empty_element(self) -> Union[int, float, str, bool]:
-        if self.dtype == float:
-            return 0.0
-
-        elif self.dtype == str:
-            return ""
+    def _estimate_data_type(self, object: Iterable) -> type:
+        type_counts = {int: 0, float: 0, str: 0, bool: 0}
 
-        elif self.dtype == bool:
-            return False
+        for row in object:
+            for element in row:
+                if isinstance(element, int):
+                    type_counts[int] += 1
+                elif isinstance(element, float):
+                    type_counts[float] += 1
+                elif isinstance(element, str):
+                    type_counts[str] += 1
+                elif isinstance(element, bool):
+                    type_counts[bool] += 1
 
+        if type_counts[int] > 0 and type_counts[float] > 0:
+            return float
         else:
-            return 0
-
-    def _adjust_dimensions(self) -> None:
-        buffer = self.__data.copy()
-
-        init_item = self._empty_element()
-
-        self.__data = [
-            [init_item for _ in range(self.columns)] for _ in range(self.rows)
-        ]
-
-        for i in range(self.rows):
-            for j in range(self.columns):
-                try:
-                    self.__data[i][j] = buffer[i][j]
-                except:
-                    continue
-
-    def _change_data_type(self, new_dtype: type) -> None:
-        if new_dtype not in self.__supported_types:
-            raise ValueError(
-                f"dl.Matrix.dtype must take one of this value: {self.__supported_types}"
-            )
-
-        self.__data = [[new_dtype(element) for element in row] for row in self.__data]
+            return max(type_counts, key=type_counts.get)
 
     @property
     def size(self) -> int:
         """Number of elements in matrix"""
 
         return self.rows * self.columns
 
@@ -475,27 +462,116 @@
     def rows(self, new_value: int) -> None:
         if isinstance(new_value, int):
             self.__rows = new_value
             self._adjust_dimensions()
         else:
             raise ValueError("`dl.Matrix.rows` property must be an integer")
 
+    def _adjust_dimensions(self) -> None:
+        buffer = self.__data.copy()
+
+        init_item = self._empty_element()
+
+        self.__data = [
+            [init_item for _ in range(self.columns)] for _ in range(self.rows)
+        ]
+
+        for i in range(self.rows):
+            for j in range(self.columns):
+                try:
+                    self.__data[i][j] = buffer[i][j]
+                except:
+                    continue
+
+    @property
+    def permanent(self) -> Union[int, float]:
+        """The permanent of the matrix."""
+
+        if self.rows != self.columns:
+            raise ValueError("Permanent is only defined for square matrices.")
+
+        if self.size == 1:
+            return self.__data[0, 0]
+
+        result = 0
+        for permutation in self._permutations(range(self.rows)):
+            product = 1
+            for i, j in enumerate(permutation):
+                product *= self[i, j]
+            result += product
+
+        return result
+
+    def _permutations(self, last: Iterable) -> Iterable:
+        if len(last) == 1:
+            yield last
+        else:
+            for i in range(len(last)):
+                rest = list(last[:i]) + list(last[i + 1 :])
+                for p in self._permutations(rest):
+                    yield [last[i]] + p
+
+    @property
+    def determinant(self) -> Union[int, float]:
+        """The determinant of the matrix"""
+
+        if self.rows != self.columns:
+            raise ValueError("Determinant is only defined for square matrices.")
+
+        if self.size == 1:
+            return self.__data[0][0]
+
+        if self.rows == 2:
+            return (
+                self.__data[0][0] * self.__data[1][1]
+                - self.__data[0][1] * self.__data[1][0]
+            )
+
+        result = 0
+        for j in range(self.columns):
+            submatrix = self.submatrix(
+                range(1, self.rows),
+                [column for column in range(self.columns) if column != j],
+            )
+            result += self.__data[0][j] * submatrix.determinant() * (-1) ** j
+
+        return result
+
+    @property
+    def trace(self) -> Union[int, float]:
+        """Calculates the trace of a square matrix.
+
+        The trace of a square matrix is the sum of its diagonal elements."""
+
+        if self.rows != self.columns:
+            raise ValueError("Trace is only defined for square matrices.")
+
+        return sum(self[i, i] for i in range(self.rows))
+
     def change_dtype(self, new_dtype: type) -> Self:
         """Changes the data type of the matrix.
 
         Parameters
         ----------
         new_dtype : type
             The new data type for the matrix"""
 
         self.dtype = new_dtype
         self._change_data_type(new_dtype)
 
         return self
 
+    def _change_data_type(self, new_dtype: type) -> None:
+        if new_dtype not in self.__supported_types:
+            raise ValueError(
+                f"dl.Matrix.dtype must take one of this value: {self.__supported_types}"
+            )
+
+        self.__data = [[new_dtype(element) for element in row] for row in self.__data]
+
     def fill(self, value: Union[int, float, str, bool]) -> Self:
         """Fills the matrix with the specified value.
 
         Parameters
         ----------
         value : int or float or str or bool
             Value to fill the matrix with"""
@@ -545,15 +621,15 @@
                         return False
                 else:
                     if self[i, j] != 0:
                         return False
 
         return True
 
-    def transpoze(self) -> Self:
+    def transpose(self) -> Self:
         """Transposes the matrix.
 
         The transpose of a matrix is obtained by interchanging its rows and columns.
         This operation modifies the matrix in place"""
 
         buffer = self.deep_copy()
 
@@ -561,14 +637,166 @@
 
         for i in range(self.rows):
             for j in range(self.columns):
                 self[i, j] = buffer[j, i]
 
         return self
 
+    def inverse(self) -> Self:
+        """Calculates the inverse of a square matrix.
+
+        Returns
+        -------
+        Matrix
+            The inverse matrix.
+
+        Raises
+        ------
+        ValueError
+            If the matrix is not square or it is singular (non-invertible).
+
+        Notes
+        -----
+        The matrix must be square and non-singular (invertible) to have an inverse."""
+
+        if self.rows != self.columns:
+            raise ValueError("Inverse is only defined for square matrices.")
+
+        determinant = self.determinant
+
+        if determinant == 0:
+            raise ValueError("Matrix is singular and does not have an inverse.")
+
+        adjugate = self.adjugate()
+
+        return adjugate * (1 / determinant)
+
+    def adjugate(self) -> Self:
+        """Calculates the adjugate of the matrix.
+
+        Raises
+        ------
+        ValueError
+            If the matrix is not square."""
+
+        if self.rows != self.columns:
+            raise ValueError("Adjugate is only defined for square matrices.")
+
+        cofactors = Matrix(self.shape)
+
+        for i in range(self.rows):
+            for j in range(self.columns):
+                submatrix = self.submatrix(
+                    [row for row in range(self.rows) if row != i],
+                    [col for col in range(self.columns) if col != j],
+                )
+                cofactor = (-1) ** (i + j) * submatrix.determinant
+                cofactors.__data[i][j] = cofactor
+
+        return cofactors.transpose()
+
+    def swap_rows(self, row1: int, row2: int) -> Self:
+        """Swaps two rows in the matrix.
+
+        Parameters
+        ----------
+        row1 : int
+            Index of the first row to swap.
+        row2 : int
+            Index of the second row to swap."""
+
+        self.__data[row1], self.__data[row2] = self.__data[row2], self.__data[row1]
+        return self
+
+    def scale_row(self, row: int, scalar: Union[int, float]) -> Self:
+        """Scales a row in the matrix by a scalar value.
+
+        Parameters
+        ----------
+        row : int
+            Index of the row to scale.
+        scalar : int or float
+            Scalar value to multiply the row by."""
+
+        self.__data[row] = [scalar * element for element in self.__data[row]]
+        return self
+
+    def submatrix(self, rows_index: Iterable, columns_index: Iterable) -> Self:
+        """Creates and returns a submatrix by selecting the specified ranges of rows and columns.
+
+        Parameters
+        ----------
+        rows_index : Iterable
+            The range of row indices to include in the submatrix.
+        columns_index : Iterable
+            The range of column indices to include in the submatrix.
+
+        Returns
+        -------
+        Matrix
+            The submatrix with the specified ranges of rows and columns.
+
+        Notes
+        -----
+        This method creates a new matrix object with dimensions (len(rows_index), len(columns_index)),
+        where the rows and columns within the specified ranges are included. The elements of the submatrix
+        are obtained from the corresponding elements of the original matrix."""
+
+        sub_rows = len(rows_index)
+        sub_columns = len(columns_index)
+        submatrix = Matrix((sub_rows, sub_columns))
+
+        for i, row_index in enumerate(rows_index):
+            for j, column_index in enumerate(columns_index):
+                submatrix.__data[i][j] = self.__data[row_index][column_index]
+
+        return submatrix
+
+    def to_lower_triangular(self) -> Self:
+        """Converts the matrix to lower triangular form.
+
+        Returns
+        -------
+        Matrix
+            The matrix in lower triangular form.
+
+        Notes
+        -----
+        In a lower triangular matrix, all elements above the main diagonal are set to 0.
+        """
+
+        result = self.deep_copy()
+
+        for i in range(result.rows):
+            for j in range(i + 1, result.columns):
+                result.__data[i][j] = 0
+
+        return result
+
+    def to_upper_triangular(self) -> Self:
+        """Converts the matrix to upper triangular form.
+
+        Returns
+        -------
+        Matrix
+            The matrix in upper triangular form.
+
+        Notes
+        -----
+        In an upper triangular matrix, all elements below the main diagonal are set to 0.
+        """
+
+        result = self.deep_copy()
+
+        for i in range(1, result.rows):
+            for j in range(i):
+                result.__data[i][j] = 0
+
+        return result
+
     def to_logical_matrix(self) -> Self:
         """Convert current matrix to logical matrix ((0, 1)-matrix)
 
         This function change all elements in matrix to bool and from this it follows that the matrix becomes a logical matrix
         """
 
         self.change_dtype(bool)
```

### Comparing `py-datalab-0.2.2/datalab/Vector.py` & `py-datalab-0.2.3/datalab/Vector.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.2/datalab/functions.py` & `py-datalab-0.2.3/datalab/functions.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.2/datalab/utils.py` & `py-datalab-0.2.3/datalab/utils.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.2/py_datalab.egg-info/PKG-INFO` & `py-datalab-0.2.3/py_datalab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.2.2
+Version: 0.2.3
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.2.2/setup.py` & `py-datalab-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 10):
     sys.exit("Sorry, Python < 3.10 is not supported")
 
 setup(
     name="py-datalab",
-    version="0.2.2",
+    version="0.2.3",
     author="Mateusz Nowak",
     author_email="mateusz.nowak.pol@gmail.com",
     description="This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.",
     url="https://github.com/matuszen/Python-DataLab",
     packages=find_packages(),
     install_requires=[
         "typing_extensions",
```

