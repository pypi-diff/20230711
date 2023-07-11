# Comparing `tmp/deepbench-0.1.1.tar.gz` & `tmp/deepbench-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepbench-0.1.1.tar", max compression
+gzip compressed data, was "deepbench-0.2.0.tar", max compression
```

## Comparing `deepbench-0.1.1.tar` & `deepbench-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    11357 2022-09-23 14:25:03.589828 deepbench-0.1.1/LICENSE
--rw-r--r--   0        0        0     3359 2023-06-09 16:08:12.763220 deepbench-0.1.1/README.md
--rw-r--r--   0        0        0      901 2023-06-09 16:15:21.068959 deepbench-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-20 16:19:16.528212 deepbench-0.1.1/src/deepbench/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 17:20:37.922821 deepbench-0.1.1/src/deepbench/astro_object/__init__.py
--rw-r--r--   0        0        0     3493 2023-06-07 15:57:36.000784 deepbench-0.1.1/src/deepbench/astro_object/astro_object.py
--rw-r--r--   0        0        0     3035 2023-06-09 15:55:07.028288 deepbench-0.1.1/src/deepbench/astro_object/galaxy_object.py
--rw-r--r--   0        0        0     1076 2023-05-18 19:38:13.746668 deepbench-0.1.1/src/deepbench/astro_object/n_body_object.py
--rw-r--r--   0        0        0     1759 2023-06-09 15:55:07.028646 deepbench-0.1.1/src/deepbench/astro_object/spiral_galaxy.py
--rw-r--r--   0        0        0     3768 2023-06-07 15:57:36.001246 deepbench-0.1.1/src/deepbench/astro_object/star_object.py
--rw-r--r--   0        0        0        0 2023-06-07 15:57:36.001333 deepbench-0.1.1/src/deepbench/collection/__init__.py
--rw-r--r--   0        0        0     6007 2023-06-07 15:57:36.001537 deepbench-0.1.1/src/deepbench/collection/collection.py
--rw-r--r--   0        0        0        0 2023-06-07 15:57:36.001583 deepbench-0.1.1/src/deepbench/collection/read_config.py
--rw-r--r--   0        0        0        0 2023-06-07 15:57:36.001634 deepbench-0.1.1/src/deepbench/collection/save.py
--rw-r--r--   0        0        0      150 2023-06-07 15:57:36.001967 deepbench-0.1.1/src/deepbench/image/__init__.py
--rw-r--r--   0        0        0     2560 2023-06-09 15:55:07.028990 deepbench-0.1.1/src/deepbench/image/image.py
--rw-r--r--   0        0        0     2226 2023-06-09 15:55:07.029513 deepbench-0.1.1/src/deepbench/image/shape_image.py
--rw-r--r--   0        0        0     2829 2023-06-09 15:55:07.029948 deepbench-0.1.1/src/deepbench/image/sky_image.py
--rw-r--r--   0        0        0      141 2023-06-07 15:57:36.003274 deepbench-0.1.1/src/deepbench/physics_object/__init__.py
--rw-r--r--   0        0        0     5646 2023-06-06 21:06:32.265679 deepbench-0.1.1/src/deepbench/physics_object/hamiltonian_pendulum.py
--rw-r--r--   0        0        0    15450 2023-06-06 21:06:32.266222 deepbench-0.1.1/src/deepbench/physics_object/pendulum.py
--rw-r--r--   0        0        0     1563 2023-06-06 21:01:29.305615 deepbench-0.1.1/src/deepbench/physics_object/physics_object.py
--rw-r--r--   0        0        0        0 2023-06-07 15:57:36.003405 deepbench-0.1.1/src/deepbench/settings/default_astro_object.yaml
--rw-r--r--   0        0        0      298 2023-06-07 15:57:36.003645 deepbench-0.1.1/src/deepbench/settings/default_physics_object.yaml
--rw-r--r--   0        0        0      213 2023-06-07 15:57:36.003811 deepbench-0.1.1/src/deepbench/settings/default_shapes.yaml
--rw-r--r--   0        0        0      317 2023-06-07 15:57:36.003958 deepbench-0.1.1/src/deepbench/settings/default_sky_object.yaml
--rw-r--r--   0        0        0    11110 2023-06-07 15:57:36.004593 deepbench-0.1.1/src/deepbench/shape_generator/shape_generator.py
--rw-r--r--   0        0        0     4434 1970-01-01 00:00:00.000000 deepbench-0.1.1/setup.py
--rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 deepbench-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-23 14:25:03.589828 deepbench-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5275 2023-07-11 15:27:55.428761 deepbench-0.2.0/README.md
+-rw-r--r--   0        0        0       21 2023-07-11 17:22:45.028136 deepbench-0.2.0/deepbench/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-11 15:27:55.430001 deepbench-0.2.0/deepbench/astro_object/__init__.py
+-rw-r--r--   0        0        0     3433 2023-07-11 15:27:55.430343 deepbench-0.2.0/deepbench/astro_object/astro_object.py
+-rw-r--r--   0        0        0     3736 2023-07-11 15:27:55.430821 deepbench-0.2.0/deepbench/astro_object/galaxy_object.py
+-rw-r--r--   0        0        0     1006 2023-07-11 15:27:55.431157 deepbench-0.2.0/deepbench/astro_object/n_body_object.py
+-rw-r--r--   0        0        0     4297 2023-07-11 17:21:20.068887 deepbench-0.2.0/deepbench/astro_object/spiral_galaxy.py
+-rw-r--r--   0        0        0     3658 2023-07-11 15:27:55.431802 deepbench-0.2.0/deepbench/astro_object/star_object.py
+-rw-r--r--   0        0        0       98 2023-07-11 15:27:55.432091 deepbench-0.2.0/deepbench/collection/__init__.py
+-rw-r--r--   0        0        0     8972 2023-07-11 15:27:55.432499 deepbench-0.2.0/deepbench/collection/collection.py
+-rw-r--r--   0        0        0        0 2023-07-11 15:27:55.432609 deepbench-0.2.0/deepbench/collection/read_config.py
+-rw-r--r--   0        0        0     1395 2023-07-11 15:27:55.432919 deepbench-0.2.0/deepbench/collection/save.py
+-rw-r--r--   0        0        0       98 2023-07-11 15:27:55.433199 deepbench-0.2.0/deepbench/image/__init__.py
+-rw-r--r--   0        0        0     2542 2023-07-11 15:27:55.433641 deepbench-0.2.0/deepbench/image/image.py
+-rw-r--r--   0        0        0     2768 2023-07-11 15:27:55.433793 deepbench-0.2.0/deepbench/image/shape_image.py
+-rw-r--r--   0        0        0     3825 2023-07-11 15:27:55.434102 deepbench-0.2.0/deepbench/image/sky_image.py
+-rw-r--r--   0        0        0      133 2023-07-11 15:27:55.434324 deepbench-0.2.0/deepbench/physics_object/__init__.py
+-rw-r--r--   0        0        0     6218 2023-07-11 15:27:55.434648 deepbench-0.2.0/deepbench/physics_object/hamiltonian_pendulum.py
+-rw-r--r--   0        0        0    14628 2023-07-11 15:27:55.434991 deepbench-0.2.0/deepbench/physics_object/pendulum.py
+-rw-r--r--   0        0        0     1563 2023-07-11 15:27:55.435183 deepbench-0.2.0/deepbench/physics_object/physics_object.py
+-rw-r--r--   0        0        0        0 2023-07-11 15:27:55.435298 deepbench-0.2.0/deepbench/settings/default_astro_object.yaml
+-rw-r--r--   0        0        0      298 2023-07-11 15:27:55.435707 deepbench-0.2.0/deepbench/settings/default_physics_object.yaml
+-rw-r--r--   0        0        0      213 2023-07-11 15:27:55.436202 deepbench-0.2.0/deepbench/settings/default_shapes.yaml
+-rw-r--r--   0        0        0      323 2023-07-11 15:27:55.436511 deepbench-0.2.0/deepbench/settings/default_sky_object.yaml
+-rw-r--r--   0        0        0       70 2023-07-11 15:27:55.436905 deepbench-0.2.0/deepbench/shapes/__init__.py
+-rw-r--r--   0        0        0    12191 2023-07-11 15:27:55.437251 deepbench-0.2.0/deepbench/shapes/shape_generator.py
+-rw-r--r--   0        0        0      960 2023-07-11 17:22:22.589798 deepbench-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6340 1970-01-01 00:00:00.000000 deepbench-0.2.0/setup.py
+-rw-r--r--   0        0        0     6164 1970-01-01 00:00:00.000000 deepbench-0.2.0/PKG-INFO
```

### Comparing `deepbench-0.1.1/LICENSE` & `deepbench-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepbench-0.1.1/pyproject.toml` & `deepbench-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 [tool.poetry]
 name = "DeepBench"
-version = "0.1.1"
+version = "0.2.0"
 description = "Physics Benchmark Dataset Generator"
 license = "Apache 2.0"
-authors = ["Ashia Lewis <pantagruelspendulum@protonmail.com>", "Maggie Voetberg <maggiev@fnal.gov>"]
-maintainers = ["Ashia Lewis <pantagruelspendulum@protonmail.com>", "Maggie Voetberg <maggiev@fnal.gov>"]
+authors = ["M. Voetberg <maggiev@fnal.gov>", "Ashia Livaudais", "Becky Nevin", "Omari Paul", "Brian Nord"]
+maintainers = ["M. Voetberg <maggiev@fnal.gov>"]
 readme = "README.md"
 homepage = "https://github.com/deepskies/DeepBenchmark"
 repository = "https://github.com/deepskies/DeepBenchmark"
 documentation = "https://github.com/deepskies/DeepBenchmark/tree/main/docs"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11,"
+python = ">=3.8,<4.0,"
 numpy = "^1.24.3"
 matplotlib = "^3.7.1"
 scikit-image = "^0.20.0"
 astropy = "^5.2.2"
 autograd = "^1.5"
 pyyaml = "^6.0"
+h5py = ">=3.9.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "^4.0.0"
 pytest = "^7.3.1"
 pre-commit = "^3.2.2"
 
 
+[tool.poetry.group.dev.dependencies]
+sphinx = "^7.0.1"
+sphinx-autodoc-typehints = "^1.23.2"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `deepbench-0.1.1/src/deepbench/astro_object/astro_object.py` & `deepbench-0.2.0/deepbench/astro_object/astro_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 from abc import ABC, abstractclassmethod, abstractmethod
-from typing import Union, List
+from typing import Union, List, Tuple
 from scipy import ndimage
 import numpy.random as rand
 import numpy as np
 
 
 class AstroObject(ABC):
     """
-    Description container.
+    Args:
+        image_dimensions (Union[tuple(int,int), tuple(float,float)]): The dimension(s) of the object to be produced.
+        radius (Union[int, float]): The radius of the object to be produced.
+        amplitude (Union[int, float]): The amplitude (brightness) of the object to be produced.
+        noise_level (Union[float, list[float]]): The Poisson noise level (lambda, the  expected seperation) to be applied to the object.
+
+    Examples:
+
+        >>> example_obj = AstroObject(image_dimensions=28, radius=5, amplitude=3, noise_level=0.7)
+
     """
 
     def __init__(
         self,
-        image_dimensions: Union[int, float, List[int], List[float]],
+        image_dimensions: Union[Tuple[int, int], Tuple[float, float]],
         radius: Union[int, float],
         amplitude: Union[int, float],
         noise_level: Union[float, List[float]],
     ) -> None:
-        """
-        The initialization function for the Abstract AstroObject class.
-
-        Args:
-            image_dimensions (Union[int, float, List[int], List[float]]): The dimension(s) of the object to be produced.
-            radius (Union[int, float]): The radius of the object to be produced.
-            amplitude (Union[int, float]): The amplitude of the object to be produced.
-            noise_level (Union[float, list[float]]): The Poisson noise level to be applied to the object.
-
-        Examples:
 
-            >>> example_obj = AstroObject(image_dimensions=28, radius=5, amplitude=3, noise_level=0.7)
-        """
-
-        #   TODO:
-        #   - May need a position param: position=(0,0)
-
-        self._image = np.zeros((image_dimensions, image_dimensions))
+        self._image = np.zeros(image_dimensions)
         self._radius = radius
         self._amplitude = amplitude
         self._noise_level = noise_level
 
     @abstractmethod
     def create_object(self):
         """
@@ -69,14 +62,15 @@
 
     def create_noise(self, seed=42, galaxy=False) -> np.ndarray:
         """
         Creates the Poisson noise added to the object.
 
         Args:
             seed (int): The random initialization seed used for reproducibility.
+            galaxy (bool): Scale the weight to keep with the intensity scale of a galaxy
 
         Returns:
             ndarray: A random sample drawn from a Poisson distribution.
 
         Examples:
             >>> example_obj.create_noise()
             >>> example_obj.create_noise(seed=5)
@@ -103,12 +97,14 @@
             np.arange(self._image.shape[1]),
         )
 
         return meshgrid
 
     @abstractmethod
     def displayObject(self):
+        """
+        Display the object created in a 2d plot
 
-        # Yet to implement. Will essentially just display a matplotlib image of the Object.
-
-        print("Code Container.")
+        Raises:
+            NotImplementedError: Raised if not implimented in the child class
+        """
         raise NotImplementedError()
```

### Comparing `deepbench-0.1.1/src/deepbench/astro_object/star_object.py` & `deepbench-0.2.0/deepbench/astro_object/star_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,44 @@
-from src.deepbench.astro_object.astro_object import AstroObject
+from deepbench.astro_object.astro_object import AstroObject
 from astropy.modeling.models import Moffat2D
-from src.deepbench.shape_generator.shape_generator import ShapeGenerator
 
 from typing import Union, List, Tuple
 
 import numpy as np
 
 
 class StarObject(AstroObject):
     """
-    Description Container.
+       Create Stars
+
+       Args:
+    image_dimensions (Union[int, float, List[int], List[float]]): The dimension(s) of the object to be produced.
+           radius (Union[int, float]): The radius of the object to be produced.
+           amplitude (Union[int, float]): The amplitude (brightness) of the object to be produced.
+           noise_level (Union[float, list[float]]): The Poisson noise level (lambda, the  expected seperation) to be applied to the object.
+
+       Examples:
+
+           >>> example_star = StarObject(image_dimensions=28, noise=5.0, center=3, radius=0.7, amplitude=1.2)
+           >>> example_star = StarObject(image_dimensions=(28,28), noise=5.0)
     """
 
     def __init__(
         self,
         image_dimensions: Union[int, float, List[int], List[float]],
-        noise: Union[float, List[float]],
+        noise_level: Union[float, List[float]] = 0.0,
         radius: Union[int, float] = 1.0,
         amplitude: Union[int, float] = 1.0,
     ) -> None:
-        """
-        The initialization function for the StarObject.
 
-        Args:
-            image_dimensions (Union[int, float, List[int], List[float]]): The dimension(s) of the Star to be produced.
-            noise_level (Union[float, list[float]]): The Poisson noise level to be applied to the object.
-            radius (Union[int, float]): The radius of the object to be produced.
-            amplitude (Union[int, float]): The amplitude of the object to be produced.
-
-        Examples:
-
-            >>> example_star = StarObject(image_dimensions=28, noise=5.0, center=3, radius=0.7, amplitude=1.2)
-            >>> example_star = StarObject(image_dimensions=(28,28), noise=5.0)
-        """
         super().__init__(
             image_dimensions=image_dimensions,
             radius=radius,
             amplitude=amplitude,
-            noise_level=noise,
+            noise_level=noise_level,
         )
 
     def create_Moffat_profile(
         self, center_x: float, center_y: float, alpha=1.0
     ) -> np.ndarray:
         """
         Create the Moffat distribution used to simulate star objects.
```

### Comparing `deepbench-0.1.1/src/deepbench/image/image.py` & `deepbench-0.2.0/deepbench/image/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
     def combine_objects(self, objects, object_params, seed=42):
         raise NotImplementedError
 
     def generate_noise(self, seed=42):
         """
         Add noise to an image
-        Updates SkyImage.image
 
         """
         noise_map = {
             "gaussian": self._generate_gaussian_noise,
             "poisson": self._generate_poisson_noise,
         }
 
@@ -52,18 +51,18 @@
         return noise
 
     def save_image(self, save_dir="results", image_name="image_1", image_format="jpg"):
         """
         Save the generated image into the specified directory.
         Will create directory if it does not already exist.
 
-        :param save_dir: Directory to save
-        :param image_name: base name of the saved image
-        :param image_format: file format. Recommended jpg
-        :return: None
+        Args:
+            save_dir (str): Directory to save
+            param image_name (str): base name of the saved image
+            param image_format (str): file format. Recommended jpg
         """
 
         assert self.image is not None, "Image not instantiated"
 
         save_dir = save_dir.rstrip("/")
 
         if not os.path.exists(save_dir):
```

### Comparing `deepbench-0.1.1/src/deepbench/image/shape_image.py` & `deepbench-0.2.0/deepbench/image/shape_image.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 import inspect
 from typing import Tuple
-from src.deepbench.shape_generator.shape_generator import ShapeGenerator
-from src.deepbench.image.image import Image
+from deepbench.shapes import Shapes as ShapeGenerator
+from deepbench.image.image import Image
 
 
 class ShapeImage(Image):
+    """
+    Create an image that is a composition of multiple shapes
+
+    Args:
+        image_shape (Tuple[int, int]): Dimensions of the shape image.
+        object_noise_type (str, optional): Noise distribution applied to image. Defaults to "gaussian".
+        object_noise_level (float, optional): Relative noise level (scale 0 to 1). Defaults to 0.0.
+
+    """
+
     def __init__(
         self,
         image_shape: Tuple[int, int],
         object_noise_type: str = "gaussian",
         object_noise_level: float = 0.0,
     ):
+
         self.shapes = ShapeGenerator(image_shape=image_shape)
         self.method_map = self._get_methods()
         super().__init__(
             image_shape=image_shape,
             object_noise_level=object_noise_level,
             object_noise_type=object_noise_type,
         )
 
     def _get_methods(self):
+
         methods = [
             method
             for method in inspect.getmembers(
                 ShapeGenerator, predicate=inspect.isfunction
             )
             if "create_" in method[0]
         ]
@@ -32,37 +44,43 @@
 
     def _create_object(self, shape, shape_params):
 
         if shape not in self.method_map.keys():
             raise NotImplementedError()
         return self.method_map[shape](self.shapes, **shape_params)
 
-    def combine_objects(self, objects, instance_params, object_params, seed=42):
-
+    def combine_objects(self, objects, object_params, instance_params=None, seed=42):
         """
         Utilize Image._generate_astro_objects to overlay all selected astro objects into one image
         If object parameters are not included in object list, defaults are used.
         Updates SkyImage.image.
 
         Current input parameter assumptions (totally up to change):
         For a single image:
         [{
             "object_type":"<object_type>",
             "object_parameters":{<parameters for that object>}
         }]
 
+        Args:
+            objects (list): str discriptors of the included object
+            object_params (list): Parameters of each object (ie, position in frame)
+            seed (int, optional): random seed for noise. Defaults to 42.
+
+        Returns:
+            ndarray : image with objects and noise
+
         """
         image = self.shapes.create_empty_shape()
 
         if type(objects) == str:
             objects = [objects]
-        if type(instance_params) == dict:
-            instance_params = [instance_params]
+
         if type(object_params) == dict:
             object_params = [object_params]
-
-        for shape, _ in zip(objects, instance_params):
-            for object in object_params:
-                image += self._create_object(shape, object)
+            
+        for shape, params in zip(objects, object_params):
+            image += self._create_object(shape, params)
+     
         noise = self.generate_noise(seed)
         image += noise
         return image
```

### Comparing `deepbench-0.1.1/src/deepbench/image/sky_image.py` & `deepbench-0.2.0/deepbench/image/sky_image.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,109 @@
-from src.deepbench.image.image import Image
-from src.deepbench import astro_object
+from typing import Union
+from deepbench.image.image import Image
+from deepbench import astro_object
+import numpy as np
 
 
 class SkyImage(Image):
-    def __init__(self, image_shape, object_noise_level=0, object_noise_type="gaussian"):
+    def __init__(
+        self,
+        image_shape,
+        object_noise_level=0,
+        object_noise_type="gaussian",
+        scale=True,
+    ):
+        """
+        Create an image that is a composition of multiple astronomy objects
+
+        Args:
+            image_shape (tuple(int, int)): Shape of the output image
+            object_noise_level (int, optional): Level of noise added to the full image. Defaults to 0.
+            object_noise_type (str, optional): Type of noise added. Defaults to "gaussian".
+            scale (bool, optional): Scale objects between 0 and 1 before adding to the composition
 
+        """
+        self.scale = scale
         assert len(image_shape) >= 2, "Image must be 2D or higher."
         super().__init__(image_shape, object_noise_type, object_noise_level)
 
     def _generate_astro_object(self, object_type, object_parameters):
-        """
-        Utilize the astro_object module and generate instances of the classes
-
-        :param object_type: String identifier of the class.
-            Pick from ["star", "strong_lens”, "galaxy", "spiral_galaxy", "n_body"]
-        :param object_parameters: Dictionary of the parameters required for the selected class
-            Any passed image_shape will be overwritten into Image.image_shape.
-        :return: Instance of the selected class initialized with passed object parameters.
-        """
 
         astro_object_map = {
             "star": astro_object.star_object.StarObject,
             "galaxy": astro_object.galaxy_object.GalaxyObject,
             "spiral_galaxy": astro_object.spiral_galaxy.SpiralGalaxyObject,
-            "n_body": astro_object.n_body_object.NBodyObject,
         }
 
         if object_type not in astro_object_map.keys():
             raise NotImplementedError(
                 f"Object type {object_type}, is not available. "
                 f"Please select object from {astro_object_map.keys()}"
             )
 
         return astro_object_map[object_type](**object_parameters)
 
-    def combine_objects(self, objects, instance_params, object_params, seed=42):
+    def _scale(self, input_image):
+        image = input_image.copy()
+        image = (image - input_image.min()) / (input_image.max() - input_image.min())
+        return image
 
+    def combine_objects(
+        self,
+        objects: Union[list, str],
+        instance_params: Union[list, dict],
+        object_params: Union[list, dict],
+        seed: int = 42,
+    ):
         """
         Utilize Image._generate_astro_objects to overlay all selected astro objects into one image
         If object parameters are not included in object list, defaults are used.
         Updates SkyImage.image.
 
         Current input parameter assumptions (totally up to change):
         For a single image:
         [{
             "object_type":"<object_type>",
             "object_parameters":{<parameters for that object>}
         }]
 
+        Args:
+            objects (list): str discriptors of the included object
+            instance_params (list): Parameters for the instance of the object (ei, overall noise)
+            object_params (list): Parameters of each object (ei: position in frame)
+            seed (int, optional): random seed for noise. Defaults to 42.
+
+        Returns:
+            ndarray : image with objects and noise
+
         """
-        image = self.create_empty_shape()
+        object_images = []
+
         if type(objects) == str:
             objects = [objects]
         if type(instance_params) == dict:
             instance_params = [instance_params]
         if type(object_params) == dict:
             object_params = [object_params]
 
-        for sky_object, sky_params in zip(objects, instance_params):
-            sky_params["image_dimensions"] = self.image_shape[0]
+        for sky_object, sky_params, object in zip(
+            objects, instance_params, object_params
+        ):
+            import matplotlib.pyplot as plt
+
+            sky_params["image_dimensions"] = self.image_shape
+            if "noise_level" not in sky_params:
+                sky_params["noise_level"] = 0
+
             additional_sky_object = self._generate_astro_object(sky_object, sky_params)
-            for object in object_params:
-                object_image = additional_sky_object.create_object(**object)
-                image += object_image
+
+            object_image = additional_sky_object.create_object(**object)
+            if self.scale:
+                object_image = self._scale(object_image)
+
+            object_images.append(object_image)
 
         noise = self.generate_noise(seed)
-        image += noise
+        object_images.append(noise)
+        image = np.sum(object_images, axis=0)
+
         return image
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `deepbench-0.1.1/src/deepbench/physics_object/hamiltonian_pendulum.py` & `deepbench-0.2.0/deepbench/physics_object/hamiltonian_pendulum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,139 @@
-from src.deepbench.physics_object.pendulum import Pendulum
+from deepbench.physics_object import Pendulum
 
 import autograd
 import autograd.numpy as np
 from scipy.integrate import solve_ivp
 from typing import Union, Optional
 
 
 class HamiltonianPendulum(Pendulum):
+    """
+    The Hamiltonian Pendulum class.
+
+    Args:
+        pendulum_arm_length (float): The length of the pendulum arm
+        starting_angle_radians (float): The starting angle of the pendulum
+            (angle from the 'ceiling')
+        noise_std_percent (dict): A dictionary of the Gaussian noise
+            level to be applied to each parameter. The default is no
+            noise. Each number is the standard deviation when
+            multiplied by the parameter. See create_noise().
+        acceleration_due_to_gravity (float): little g, local gravity
+            coefficient
+        mass_pendulum_bob (float): Mass of the pendulum bob,
+            this is optional if calculation_type is position only.
+
+    Examples:
+
+        >>> pendulum_obj = HamiltonianPendulum(pendulum_arm_length=10.,
+                                    starting_angle_radians=np.pi/4,
+                                    acceleration_due_to_gravity=9.8,
+                                    noise_std_percent=
+                                    {'pendulum_arm_length': 0.1,
+                                     'starting_angle_radians': 0.1,
+                                     'acceleration_due_to_gravity': 0.1}
+                                    )
+    """
+
     def __init__(
         self,
         pendulum_arm_length: float,
         starting_angle_radians: float,
         acceleration_due_to_gravity: Union[float, None] = None,
         mass_pendulum_bob: Optional[float] = 10.0,
         noise_std_percent: dict = {
             "pendulum_arm_length": 0.0,
             "starting_angle_radians": 0.0,
             "mass_pendulum_bob": 0.0,
             "acceleration_due_to_gravity": None,
         },
     ):
-        """
-        The initialization function for the Hamiltonian Pendulum class.
 
-        Args:
-            pendulum_arm_length (float): The length of the pendulum arm
-            starting_angle_radians (float): The starting angle of the pendulum
-                (angle from the 'ceiling')
-            noise_std_percent (dict): A dictionary of the Gaussian noise
-                level to be applied to each parameter. The default is no
-                noise. Each number is the standard deviation when
-                multiplied by the parameter. See create_noise().
-            acceleration_due_to_gravity (float): little g, local gravity
-                coefficient
-            mass_pendulum_bob (float): Mass of the pendulum bob,
-                this is optional if calculation_type is position only.
-
-        Examples:
-
-            >>> pendulum_obj = HamiltonianPendulum(pendulum_arm_length=10.,
-                                        starting_angle_radians=np.pi/4,
-                                        acceleration_due_to_gravity=9.8,
-                                        noise_std_percent=
-                                        {'pendulum_arm_length': 0.1,
-                                         'starting_angle_radians': 0.1,
-                                         'acceleration_due_to_gravity': 0.1}
-                                        )
-        """
         super().__init__(
             pendulum_arm_length=pendulum_arm_length,
             starting_angle_radians=starting_angle_radians,
             noise_std_percent=noise_std_percent,
             acceleration_due_to_gravity=acceleration_due_to_gravity,
             mass_pendulum_bob=mass_pendulum_bob,
         )
 
-    def hamiltonian_fn(self, coords, m, L, g):
+    def _hamiltonian_fn(self, coords, m, L, g):
+
         q, p = np.split(coords, 2)
-        # m = self.mass_pendulum_bob
-        # L = self.pendulum_arm_length
-        # g = self.acceleration_due_to_gravity
-        # kinetic_term = ((self.pendulum_arm_length**2) * (p**2)) / (
-        #     2 * self.mass_pendulum_bob
-        # )
-        # potential_term = (
-        #     self.mass_pendulum_bob
-        #     * self.acceleration_due_to_gravity
-        #     * self.pendulum_arm_length
-        # ) * (1 - np.cos(q))
-        # H = kinetic_term + potential_term
+
         H = (m * g * L) * (1 - np.cos(q)) + ((L**2) * (p**2)) / (2 * m)
         return H
 
     def dynamics_fn(self, t, coords):
-        # derives the gradient of the hamiltonian function
-        # print(f'mass: {self.mass_pendulum_bob} length: {self.pendulum_arm_length} g: {self.acceleration_due_to_gravity}')
-        dcoords = autograd.grad(self.hamiltonian_fn)(
+        """
+        derives the gradient of the hamiltonian function
+
+        Args:
+            coords (np.ndarray): coordinates of the pendulum
+
+        Returns:
+            np.ndarray:time derivates of p and q.
+        """
+        #
+        dcoords = autograd.grad(self._hamiltonian_fn)(
             coords,
             self.mass_pendulum_bob,
             self.pendulum_arm_length,
             self.acceleration_due_to_gravity,
         )
 
-        # dcoords = autograd.grad(self.hamiltonian_fn)(coords, 2, 10, 9.8)
         dqdt, dpdt = np.split(dcoords, 2)
         S = np.concatenate([dpdt, -dqdt], axis=-1)
         return S
 
-    def create_object(self, time, noiseless=True):
-        assert noiseless
-        return super().create_object(time, noiseless)
+    def create_object(
+        self, time: Union[float, np.array], noiseless: bool = True, seed: int = 42
+    ):
+        """
+        Given a single or array of times, simulates the pendulum position at
+        each of these times and optionally adds Gaussian noise to each
+        parameter.
+
+        Args:
+            time (Union[float, np.array]): A single moment in time, or
+                an array of times (s)
+            noiseless (bool): Add noise to the pendulum parameters
+            seed (int): Random seed for parameters
+
+        Returns:
+            tuple
+            q (np.ndarray): position.
+            p (np.ndarray): momentum.
+            dqdt (np.ndarray): velocity.
+            dpdt (np.ndarray) - force.
+            t_eval (np.ndarray) - times.
+        """
+
+        if not noiseless:
+            raise NotImplementedError
+
+        return super().create_object(time, noiseless, seed=seed)
 
     def simulate_pendulum_dynamics(self, time, **kwargs):
+        """
+        Evaulate the hamilitonian at times `time` and return the position, momentum and time derviates
+
+        Args:
+            time (np.ndarray): Times to simulate
+
+        Returns:
+            tuple
+            q (np.ndarray): position.
+            p (np.ndarray): momentum.
+            dqdt (np.ndarray): velocity.
+            dpdt (np.ndarray) - force.
+            t_eval (np.ndarray) - times.
+        """
+
         assert time.size > 1, "you must enter more than one point in time"
 
         t_eval = np.array(time)
         t_span = np.array([time[0], time[-1]])
 
         radius = np.random.rand() + 1.3
 
@@ -125,15 +163,15 @@
             np.random.randn(*q.shape) * noise_std
         )  # creates a random array of size q.shape and is scaled with noise_std then adds to q for noise
         p += (
             np.random.randn(*p.shape) * noise_std
         )  # creates a random array of size p.shape and is scaled with noise_std then adds to p for noise
         return q, p, dqdt, dpdt, t_eval
 
-    def get_field(self, xmin=-1.2, xmax=1.2, ymin=-1.2, ymax=1.2, gridsize=20):
+    def _get_field(self, xmin=-1.2, xmax=1.2, ymin=-1.2, ymax=1.2, gridsize=20):
         """get_field() is used to visualize the the gradiant vector field."""
         field = {"meta": locals()}
 
         b, a = np.meshgrid(
             np.linspace(xmin, xmax, gridsize), np.linspace(ymin, ymax, gridsize)
         )
         ys = np.stack([b.flatten(), a.flatten()])
```

### Comparing `deepbench-0.1.1/src/deepbench/physics_object/pendulum.py` & `deepbench-0.2.0/deepbench/physics_object/pendulum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.deepbench.physics_object.physics_object import PhysicsObject
+from deepbench.physics_object.physics_object import PhysicsObject
 import numpy as np
 import numpy.random as rand
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
 from typing import Union, Optional, Tuple
 import logging
 import os
@@ -76,19 +76,15 @@
         self.big_G_newton = big_G_newton
         self.phi_planet = phi_planet
         if acceleration_due_to_gravity is None:
             assert (
                 self.big_G_newton is not None and self.phi_planet is not None
             ), "must define big_G_newton and phi_planet if \
                     acceleration_due_to_gravity is not provided"
-            # assert self._noise_level['big_G_newton'] is not None \
-            #    and self._noise_level['phi_planet'] \
-            #    is not None, "must define big_G_newton and phi_planet \
-            #        noise levels if acceleration_due_to_gravity \
-            #        is not provided"
+
             self.acceleration_due_to_gravity = self.big_G_newton * self.phi_planet
             self.initial_parameters = {
                 "pendulum_arm_length": self.pendulum_arm_length,
                 "starting_angle_radians": self.starting_angle_radians,
                 "acceleration_due_to_gravity": self.acceleration_due_to_gravity,
                 "big_G_newton": self.big_G_newton,
                 "phi_planet": self.phi_planet,
@@ -204,25 +200,27 @@
             # acceleration_due_to_gravity = multiple of noisy G and phi
             if self.big_G_newton is not None and self.phi_planet is not None:
                 self.acceleration_due_to_gravity = self.big_G_newton * self.phi_planet
             else:
                 assert f"Either big G or phi_planet is None \
                     (G = {self.big_G_newton}, ø = {self.phi_planet}); \
                         this is not allowed with hierarchical noise"
-        return
 
     def destroy_noise(self):
+        """
+        Remove noise from the parameters
+
+        """
         # Re-modify the global parameters to
         # have the original value
         for key in self._noise_level.keys():
             if key not in self.parameter_map:
                 raise ValueError(f"Invalid parameter name: {key}")
             attribute = self.initial_parameters[key]
             setattr(self, key, attribute)
-        return
 
     def create_object(
         self,
         time: Union[float, np.array],
         noiseless: bool = False,
         seed: int = None,
         verbose: bool = False,
@@ -236,15 +234,15 @@
             time (Union[float, np.array]): A single moment in time, or
                 an array of times (s)
             noiseless (bool): Enables a noise realization if True.
                 Default is set to False
             seed (int): Random seed used to generate Gaussian noise
 
         Example:
-            >>> pendulum = Pendulum(...SEE ABOVE...)
+            >>> pendulum = Pendulum()
             >>> time = np.array(np.linspace(0, 10, 20))
             >>> pend_position = pendulum.create_object(time, noiseless=True)
         """
         time = np.asarray(time)
         assert time.size > 0, "you must enter one or more points in time"
         if isinstance(time, (float, int)):
             n_steps = 1
@@ -255,14 +253,23 @@
         if noiseless:
             self.destroy_noise()
         pendulum = self.simulate_pendulum_dynamics(time)
         self.destroy_noise()
         return pendulum
 
     def simulate_pendulum_dynamics(self, time: Union[float, np.array]):
+        """
+        Simulate a pendulum with Neutonian physics
+
+        Args:
+            time (Union[float, np.array]): times to simulate
+
+        Returns:
+            np.ndarray: position of the pendulum.
+        """
         time = np.asarray(time)
         assert time.size > 0, "you must enter one or more points in time"
         # Check if parameters are single values
         # or arrays with the same length as time
         if isinstance(self.pendulum_arm_length, (float, int)):
             pendulum_arm_length_values = np.full_like(
                 np.asarray(time), self.pendulum_arm_length
@@ -295,14 +302,23 @@
             np.sqrt(acceleration_values / pendulum_arm_length_values)
         )
 
         # Calculate x using the modified parameters and time
         return pendulum_arm_length_values * np.sin(theta_time * time)
 
     def displayObject(self, time: Union[float, np.array]):
+        """
+        Display the pendulum over times.
+
+        Args:
+            time (Union[float, np.array]): times to display the pendulum position
+
+        Returns:
+            tuple(np.ndarray, np.ndarray): noiseless, noisy arrays at times "time"
+        """
         noisy = self.create_object(time)
         noise_free = self.create_object(time, noiseless=True)
         plt.clf()
         plt.plot(time, noisy, color="#EF5D60")
         plt.scatter(time, noisy, label="noisy", color="#EF5D60")
         plt.plot(time, noise_free, color="#0E131F")
         plt.scatter(time, noise_free, label="noise free", color="#0E131F")
@@ -330,35 +346,7 @@
         plt.plot(time, noise_free, color="#0E131F", zorder=100)
         plt.scatter(time, noise_free, label="noise free", color="#0E131F", zorder=100)
         plt.legend()
         plt.ylabel("x position")
         plt.xlabel("time [s]")
         plt.show()
         return noise_free, noisy_ys
-
-    """
-    def animateObject(self, time: Union[float, np.array]):
-        # Right now this just plots x and t
-        # Instantiate the simulator
-        pendulum = self.create_object(time)
-        plt.clf()
-        # Create the figure and axis
-        fig = plt.figure(figsize=(10, 3))
-        ax1 = fig.add_subplot(111)
-
-        def update(i):
-            # Calculate the position and velocity at the current time step
-            # Clear the previous plot
-            # Plot the quantity output from the pendulum
-            pendulum_now = pendulum[i]
-            ax1.plot([time, 0], [pendulum_now, 1.4])
-            ax1.scatter(time[i], pendulum_now)
-            ax1.set_title(f'{self.calculation_type} = '
-                          + str(round(pendulum_now, 1)))
-        if isinstance(time, float):
-            time = [time]
-        anim = FuncAnimation(fig, update,
-                             frames=range(1, len(time)),
-                             interval=100)
-        plt.show(anim)
-        return
-    """
```

### Comparing `deepbench-0.1.1/src/deepbench/physics_object/physics_object.py` & `deepbench-0.2.0/deepbench/physics_object/physics_object.py`

 * *Files identical despite different names*

### Comparing `deepbench-0.1.1/src/deepbench/shape_generator/shape_generator.py` & `deepbench-0.2.0/deepbench/shapes/shape_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,50 @@
+from typing import Union
 import numpy as np
 from matplotlib.path import Path
 from matplotlib import patches
 from skimage import transform
 
 
 class ShapeGenerator:
-    def __init__(self, image_shape=(28, 28)):
+    def __init__(self, image_shape: tuple = (28, 28)):
         self.image_shape = image_shape
         self.n_dimensions = len(self.image_shape)
 
-    def resize(self, image, resize_dimensions=(28, 28)):
+    def resize(self, image: np.ndarray, resize_dimensions: tuple = (28, 28)):
         """
-        Resize a numpy array
-        :param image: Numpy array to resize
-        :param resize_dimensions: tuple(*int) Dimensions to reshape the image to
-        :return: numpy array of shape resize_dimensions
+        Resize an array-like
+
+        Args:
+            image (np.ndarray): shape to resize
+            resize_dimensions (tuple, optional): resize to shape. Defaults to (28, 28).
+
+        Raises:
+            ValueError: invalid size, either too small (0,0) or having the number of incorrect dimensions
+
+        Returns:
+            np.ndarray: array of size (resize_dimensions)
         """
         resize_dimensions = tuple(map(lambda dim: int(np.ceil(dim)), resize_dimensions))
         if len(image.shape) != len(resize_dimensions):
             raise ValueError(
                 f"Number of dimensions of source image ({image.shape} do not make target dimensions ({resize_dimensions})"
             )
         if 0 in resize_dimensions:
             raise ValueError(
                 "Attempting to resize to an invalid size, please increase the size"
             )
 
         resized_image = transform.resize(image, resize_dimensions)
         return resized_image
 
-    def _convert_patch_to_image(self, image, cutout=None):
-        """
-        Converts a matplot path or patch object into a numpy array of the designated size
-        :param image: Matplotlib image object to convert
-        :param image_shape: [tuple(*int)] Size of the desired image
-        :return: numpy array of shape image_shape, containing the image
-        """
+    def _convert_patch_to_image(
+        self, image: patches.Patch, cutout: patches.Path = None
+    ):
+
         n_dim = len(self.image_shape)
         self.image_shape = tuple(map(lambda dim: int(np.ceil(dim)), self.image_shape))
 
         if n_dim < 2:
             raise ValueError(
                 f"Image shape input of length {n_dim}; but input must be length >=2"
             )
@@ -64,30 +69,36 @@
             cutout_points = coordinates[cutout_coords]
             out_array[cutout_points[:, 0], cutout_points[:, 1]] = 0.0
 
         return out_array
 
     def create_rectangle(
         self,
-        center=(14, 14),
-        width=10,
-        height=10,
-        angle=0,
-        line_width=1,
-        fill=False,
+        center: tuple = (np.random.randint(10, 16), np.random.randint(10, 16)),
+        width: int = np.random.randint(10, 16),
+        height: int = np.random.randint(10, 16),
+        angle: Union[float, int] = 0,
+        line_width: int = 1,
+        fill: bool = False,
     ):
+
         """
-        :param image_shape: [tuple(*int)] Shape of the image output
-        :param center: [tuple(*int)] Center of the rectangle (coordinate)
-        :param width: [int] Horizontal width of the rectangle (in pixels)
-        :param height: [int] Vertical height of the rectangle (in pixels)
-        :param angle: [float] Angle to rotate, in degrees
-        :param line_width: [int] Width (in pixels)
-        :param fill: [bool] to color in the center of the rectangle
-        :return: Numpy array of size image_shape containing a rectangle
+        Make a rectangle.
+
+        Args:
+            center (tuple(*int), optional): Center of the rectangle (coordinate). Defaults to (14, 14).
+            width (int, optional): Horizontal width of the rectangle (in pixels). Defaults to random int.
+            height (int, optional): Vertical height of the rectangle (in pixels). Defaults to random int.
+            angle (Union[float, int], optional): tilt the rectangle (degrees). Defaults to 0.
+            line_width (int, optional): line width of the outline. Defaults to 1.
+            fill (bool, optional): Fill in the rectangle. Defaults to False.
+
+
+        Returns:
+           np.ndarray: A Rectangle image
         """
 
         n_center_dim = len(center)
         if self.n_dimensions != n_center_dim:
             raise ValueError(
                 f"Image shape input of length {self.n_dimensions}; but supplied center coordinates with dimension f{n_center_dim}"
             )
@@ -106,38 +117,39 @@
             xy_cutout = (center[0] - (cutout_w / 2), center[1] - (cutout_h / 2))
             cutout = patches.Rectangle(
                 xy=xy_cutout, width=cutout_w, height=cutout_h, angle=angle
             )
 
         rectangle_array = self._convert_patch_to_image(rectangle, cutout=cutout)
 
-        if rectangle_array.ravel().sum() == 0.0:
-            raise UserWarning("Image out of bounds, no shape displayed")
-
         return rectangle_array
 
     def create_regular_polygon(
         self,
-        center=(14, 14),
-        angle=45,
-        vertices=3,
-        radius=10,
-        line_width=2,
+        center: tuple = (np.random.randint(10, 16), np.random.randint(10, 16)),
+        angle: Union[int, float] = np.random.uniform(20, 90),
+        vertices: int = 3,
+        radius: Union[int, float] = np.random.uniform(8, 12),
+        line_width=1,
         fill=False,
     ):
         """
         Create a polygon with equal length sides
-        :param image_shape: tuple[*int] Size of the output image (pixels)
-        :param center: tuple[*int] Where to center the object
-        :param angle: float Angle of rotation (degrees)
-        :param vertices: int number of vertices (3=triangle, 4=square, etc)
-        :param radius: int Distance from vertex to vertex
-        :param line_width: int Width of lines (pixels)
-        :param fill: bool Fill center of the object
-        :return: Numpy array of shape image_shape containing the polygon
+
+        Args:
+            center (tuple[*int], optional): Where to center the object.
+            angle (Union[int, float], optional): Angle of rotation (degrees)
+            vertices (int, optional): Number of verticies. Defaults to 3, a triangle.
+            radius (int, optional): distance from vertex to vertex Defaults to 10.
+            line_width (int, optional): line width of the outline. Defaults to 1.
+            fill (bool, optional): Fill in the rectangle. Defaults to False.
+
+
+        Returns:
+           np.ndarray: A polygon image
         """
 
         radius = abs(radius)
 
         n_center_dim = len(center)
         if self.n_dimensions != n_center_dim:
             raise ValueError(
@@ -162,56 +174,63 @@
                 numVertices=vertices,
                 radius=cutout_radius,
                 orientation=angle,
             )
 
         polygon_array = self._convert_patch_to_image(polygon, cutout=cutout)
 
-        if polygon_array.ravel().sum() == 0.0:
-            raise UserWarning("Image out of bounds, no shape displayed")
-
         return polygon_array
 
     def create_arc(
         self,
-        center=(14, 14),
-        radius=10,
-        theta1=0,
-        theta2=90,
-        line_width=1,
+        center: tuple = (np.random.randint(10, 16), np.random.randint(10, 16)),
+        radius: Union[int, float] = np.random.uniform(8, 12),
+        theta1: Union[int, float] = np.random.uniform(0, 45),
+        theta2: Union[int, float] = np.random.uniform(85, 120),
+        line_width: int = 1,
     ):
         """
-        Create an arc with radius "radius" arcing from theta1 to theta2
-        :param image_shape: Shape of the output array (pixels)
-        :param center: tuple[*int]Center point of the arc
-        :param radius: int distance from the arc to the center point
-        :param theta1: float starting point of the arc (degrees)
-        :param theta2: float ending point of the arc (degrees)
-        :param line_width: int thickness of the arc (pixels)
-        :return: Numpy array of the arc
+        Create an arc with radius "radius" arcing from theta1 to theta2 counter-clockwise
+
+        Args:
+            center (tuple, optional): Center point of the arc. Defaults to (np.random.randint(10, 16), np.random.randint(10, 16)).
+            radius (Union[int, float], optional): distance from the arc to the center point. Defaults to np.random.random(8, 12).
+            theta1 (Union[int, float], optional): starting point of the arc (degrees). Defaults to np.random.random(0, 45).
+            theta2 (Union[int, float], optional): ending point of the arc (degrees). Defaults to np.random.random(85, 120).
+            line_width (int, optional):  thickness of the arc (pixels) Defaults to 1.
+
+
+        Returns:
+            np.ndarray: The arc image
         """
 
         arc = patches.Wedge(
             center=center, r=radius, theta1=theta1, theta2=theta2, width=line_width
         )
         arc_array = self._convert_patch_to_image(arc)
 
-        if arc_array.ravel().sum() == 0.0:
-            raise UserWarning("Image out of bounds, no shape displayed")
-
         return arc_array
 
-    def create_line(self, start=(0, 0), end=(28, 28), line_width=1):
+    def create_line(
+        self,
+        start: tuple = (np.random.randint(0, 10), np.random.randint(0, 10)),
+        end: tuple = (np.random.randint(12, 28), np.random.randint(12, 28)),
+        line_width: int = 1,
+    ):
+
         """
         Generate a numpy array of a line
-        :param image_shape:  tuple(*int) Shape of the output arrray (pixels)
-        :param start: tuple(*int) Starting corner of the line
-        :param end: tuple(*int) Ending corner of the line
-        :param line_width: int Thickness of the line (pixels)
-        :return: Numpy array containing the line
+
+        Args:
+            start (tuple, optional): Starting corner of the line. Defaults to (np.random.randint(0, 10), np.random.randint(0, 10)).
+            end (tuple, optional): Ending corner of the line. Defaults to (np.random.randint(12, 28), np.random.randint(12, 28)).
+            line_width (int, optional): Thickness of the line (pixels). Defaults to 1.
+
+        Returns:
+            np.ndarray
         """
 
         if len(start) != len(end):
             raise ValueError(
                 f"Dimension mismatch, start point had dimensions of {len(start)}, but end point had dimensions of {len(end)}"
             )
 
@@ -234,37 +253,40 @@
             (x_start, y_start),
             width=width_rect,
             height=height_rect,
             angle=angle_degrees,
         )
         line_array = self._convert_patch_to_image(line)
 
-        if line_array.ravel().sum() == 0.0:
-            raise UserWarning("Image out of bounds, no shape displayed")
-
         return line_array
 
     def create_ellipse(
         self,
-        center=(14, 14),
-        width=10,
-        height=10,
-        angle=0,
-        line_width=1,
-        fill=False,
+        center: tuple = (np.random.randint(10, 16), np.random.randint(10, 16)),
+        width: int = np.random.randint(10, 16),
+        height: int = np.random.randint(10, 16),
+        angle: Union[float, int] = 0,
+        line_width: int = 1,
+        fill: bool = False,
     ):
         """
-        :param image_shape: tuple(*int) Shape of the output arrray (pixels)
-        :param center: tuple(*int) Center point of the ellipse
-        :param width: int Horizontal length of the ellipse (pixels)
-        :param height: int Vertical height of the ellipse (pixels)
-        :param angle: float Rotation angle of the ellipse (degrees)
-        :param line_width: int Width of the ellipse's border (pixels)
-        :param fill: bool Fill the center of the ellipse
-        :return: Numpy array containing the ellipse
+        Create an ellipse/circle (where width/height are the same)
+
+        Args:
+            center (tuple, optional): Center point of the ellipse. Defaults to (np.random.randint(10, 16), np.random.randint(10, 16)).
+            width (int, optional): Horizontal length of the ellipse (pixels). Defaults to np.random.randint(10, 16).
+            height (int, optional): Vertical height of the ellipse (pixels). Defaults to np.random.randint(10, 16).
+            angle (Union[float, int], optional):  Rotation angle of the ellipse (degrees). Defaults to 0.
+            line_width (int, optional):  Width of the ellipse's border (pixels). Defaults to 1.
+            fill (bool, optional): Fill the center of the ellipse. Defaults to False.
+
+
+        Returns:
+           np.ndarray
+
         """
 
         if self.n_dimensions != len(center):
             raise ValueError(
                 f"Dimension mismatch, image had dimensions of {self.n_dimensions}, "
                 f"but center point had dimensions of {len(center)}"
             )
@@ -281,21 +303,23 @@
 
             cutout = patches.Ellipse(
                 xy=xy_cutout, width=width_cutout, height=height_cutout, angle=angle
             )
 
         ellipse_array = self._convert_patch_to_image(ellipse, cutout=cutout)
 
-        if ellipse_array.ravel().sum() == 0.0:
-            raise UserWarning("Image out of bounds, no shape displayed")
-
         return ellipse_array
 
     def create_empty_shape(self):
+        """
+        Create an array of 0s with shape self.image_shape
 
+        Returns:
+            np.ndarray
+        """
         if self.n_dimensions < 2:
             raise ValueError(
                 f"Image shape input of length {self.n_dimensions}; but input must be length >=2"
             )
 
         if 0 in self.image_shape:
             raise ValueError(f"Image size must be greater than 0")
```

