# Comparing `tmp/pydra_ants-0.0.2.tar.gz` & `tmp/pydra_ants-0.0.3.tar.gz`

## Comparing `pydra_ants-0.0.2.tar` & `pydra_ants-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.editorconfig
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.github/dependabot.yaml
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/src/pydra/tasks/ants/__init__.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/src/pydra/tasks/ants/apply_transforms.py
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/src/pydra/tasks/ants/bias_correction.py
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/src/pydra/tasks/ants/registration.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/LICENSE
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/README.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/hatch.toml
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.editorconfig
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.github/dependabot.yaml
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/src/pydra/tasks/ants/__init__.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/src/pydra/tasks/ants/apply_transforms.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/src/pydra/tasks/ants/bias_correction.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/src/pydra/tasks/ants/registration.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/README.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/hatch.toml
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/PKG-INFO
```

### Comparing `pydra_ants-0.0.2/.github/workflows/publish.yaml` & `pydra_ants-0.0.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.2/.github/workflows/test.yaml` & `pydra_ants-0.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.2/src/pydra/tasks/ants/apply_transforms.py` & `pydra_ants-0.0.3/src/pydra/tasks/ants/registration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,156 +1,211 @@
 """
-ApplyTransforms
-===============
+Registration
+============
 
 Examples
 --------
 
->>> task = ApplyTransforms(moving_image="moving.nii", fixed_image="fixed.nii")
+>>> task = RegistrationSyNQuick(
+...     dimensionality=3,
+...     fixed_image="reference.nii",
+...     moving_image="structural.nii",
+... )
 >>> task.cmdline    # doctest: +ELLIPSIS
-'antsApplyTransforms -e scalar -i moving.nii -r fixed.nii -o .../moving_warped.nii -n Linear ...'
+'antsRegistrationSyNQuick.sh -d 3 -f reference.nii -m structural.nii ...'
 
->>> task = ApplyTransforms(
-...     moving_image="moving.nii",
-...     fixed_image="fixed.nii",
-...     interpolation="BSpline",
-...     transform_list=["affine.mat"],
+>>> task = RegistrationSyNQuick(
+...     dimensionality=3,
+...     fixed_image="reference.nii",
+...     moving_image="structural.nii", 
+...     transform_type="b",
+...     spline_distance=32,
+...     gradient_step_size=0.2,
+...     random_seed=42,
 ... )
 >>> task.cmdline    # doctest: +ELLIPSIS
-'antsApplyTransforms ... -n BSpline[3] -t affine.mat ...'
+'antsRegistrationSyNQuick.sh ... -t b -s 32 -g 0.2 ... -e 42'
 
->>> task = ApplyTransforms(
-...     moving_image="moving.nii",
-...     fixed_image="fixed.nii",
-...     interpolation="Gaussian",
-...     sigma=4.0,
-...     alpha=1.0,
-...     transform_list=["affine.mat", "warp_field.nii.gz"],
-...     which_to_invert=[True, False],
+>>> task = RegistrationSyNQuick(
+...     dimensionality=3,
+...     fixed_image="reference.nii",
+...     moving_image="structural.nii",
+...     fixed_mask="mask.nii",
 ... )
 >>> task.cmdline    # doctest: +ELLIPSIS
-'antsApplyTransforms ... -n Gaussian[4.0, 1.0] -t [affine.mat, 1] -t [warp_field.nii.gz, 0] ...'
+'antsRegistrationSyNQuick.sh ... -x mask.nii ...'
 """
 
-__all__ = ["ApplyTransforms"]
+__all__ = ["RegistrationSyNQuick"]
 
 from os import PathLike
 from typing import Sequence
 
-from attrs import define, field
-from pydra.engine.specs import ShellSpec, SpecInfo
+from attrs import NOTHING, define, field
+from pydra.engine.specs import File, ShellOutSpec, ShellSpec, SpecInfo
 from pydra.engine.task import ShellCommandTask
 
 
-class ApplyTransforms(ShellCommandTask):
-    """Task definition for antsApplyTransforms."""
+class RegistrationSyNQuick(ShellCommandTask):
+    """Task definition for antsRegistrationSyNQuick."""
 
     @define(kw_only=True)
     class InputSpec(ShellSpec):
         dimensionality: int = field(
             metadata={
-                "help_string": "force image dimensionality (2, 3 or 4)",
+                "help_string": "force image dimensionality (2 or 3)",
+                "mandatory": True,
                 "argstr": "-d",
-                "allowed_values": {2, 3, 4},
+                "allowed_values": {2, 3},
             }
         )
 
-        image_type: str = field(
-            default="scalar",
-            metadata={
-                "help_string": (
-                    "specify the image type (0: scalar, 1: vector, 2: tensor, 3: time-series, 4: multichannel,"
-                    " 5: five-dimensional)"
-                ),
-                "argstr": "-e",
-                "allowed_values": {0, 1, 2, 3, 4, 5},
-            },
-        )
-
-        moving_image: PathLike = field(metadata={"help_string": "moving image", "mandatory": True, "argstr": "-i"})
+        fixed_image: PathLike = field(metadata={"help_string": "fixed image", "mandatory": True, "argstr": "-f"})
 
-        fixed_image: PathLike = field(metadata={"help_string": "fixed image", "mandatory": True, "argstr": "-r"})
+        moving_image: PathLike = field(metadata={"help_string": "moving image", "mandatory": True, "argstr": "-m"})
 
-        output_image: str = field(
-            metadata={"help_string": "output image", "argstr": "-o", "output_file_template": "{moving_image}_warped"}
+        output_prefix: str = field(
+            default="output", metadata={"help_string": "prefix for output files", "argstr": "-o"}
         )
 
-        interpolation: str = field(
-            default="Linear",
+        num_threads: int = field(default=1, metadata={"help_string": "number of threads", "argstr": "-n"})
+
+        initial_transforms: Sequence[PathLike] = field(metadata={"help_string": "initial transforms", "argstr": "-i"})
+
+        transform_type: str = field(
+            default="s",
             metadata={
-                "help_string": "interpolation method",
+                "help_string": "transform type",
+                "argstr": "-t",
                 "allowed_values": {
-                    "Linear",
-                    "NearestNeighbor",
-                    "Gaussian",
-                    "BSpline",
-                    "CosineWindowedSinc",
-                    "WelchWindowedSinc",
-                    "HammingWindowedSinc",
-                    "LanczosWindowedSinc",
+                    "t",  # translation
+                    "r",  # rigid
+                    "a",  # rigid + affine
+                    "s",  # rigid + affine + syn
+                    "sr",  # rigid + syn
+                    "so",  # syn only
+                    "b",  # rigid + affine + b-spline
+                    "br",  # rigid + b-spline
+                    "bo",  # b-spline only
                 },
-                "formatter": lambda interpolation, sigma, alpha, spline_order: (
-                    f"-n {interpolation}"
-                    + (
-                        f"[{spline_order}]"
-                        if interpolation == "BSpline"
-                        else f"[{sigma}, {alpha}]"
-                        if interpolation in ("MultiLabel", "Gaussian")
-                        else ""
-                    )
-                ),
             },
         )
 
-        sigma: float = field(metadata={"help_string": "sigma parameter for MultiLabel and Gaussian interpolation"})
-
-        alpha: float = field(metadata={"help_string": "alpha parameter for MultiLabel and Gaussian interpolation"})
+        num_histogram_bins: int = field(
+            default=32,
+            metadata={
+                "help_string": "number of histogram bins in SyN stage",
+                "formatter": lambda transform_type, num_histogram_bins: (
+                    f"-r {num_histogram_bins}" if "s" in transform_type else ""
+                ),
+            },
+        )
 
-        spline_order: int = field(default=3, metadata={"help_string": "spline order for BSpline interpolation"})
+        spline_distance: float = field(
+            default=26,
+            metadata={
+                "help_string": "spline distance for deformable B-spline SyN transform",
+                "formatter": lambda transform_type, spline_distance: (
+                    f"-s {spline_distance}" if "b" in transform_type else ""
+                ),
+            },
+        )
 
-        output_datatype: str = field(
+        gradient_step_size: float = field(
+            default=0.1,
             metadata={
-                "help_string": "force output image datatype",
-                "argstr": "-u",
-                "allowed_values": {"char", "uchar", "short", "int", "float", "double", "default"},
-            }
+                "help_string": "gradient step size for SyN and B-spline SyN",
+                "formatter": lambda transform_type, gradient_step_size: (
+                    f"-g {gradient_step_size}" if any(c in transform_type for c in ("s", "b")) else ""
+                ),
+            },
         )
 
-        transform_list: Sequence[PathLike] = field(
+        mask_parameters: str = field(
             metadata={
-                "help_string": "list of transforms to apply",
-                "formatter": lambda transform_list, which_to_invert: (
-                    ""
-                    if not transform_list
-                    else " ".join(f"-t {f}" for f in transform_list)
-                    if not which_to_invert
-                    else " ".join(f"-t [{f}, {int(i)}]" for f, i in zip(transform_list, which_to_invert))
+                "help_string": "mask parameters",
+                "readonly": True,
+                "formatter": lambda fixed_mask, moving_mask: (
+                    "" if not fixed_mask else f"-x {fixed_mask},{moving_mask}" if moving_mask else f"-x {fixed_mask}"
                 ),
             }
         )
 
-        which_to_invert: Sequence[bool] = field(
-            metadata={"help_string": "specify which transforms to invert", "requires": {"transform_list"}}
-        )
+        fixed_mask: PathLike = field(metadata={"help_string": "mask applied to the fixed image"})
 
-        default_value: float = field(metadata={"help_string": "default voxel value", "argstr": "-f"})
+        moving_mask: PathLike = field(
+            metadata={"help_string": "mask applied to the moving image", "requires": {"fixed_mask"}}
+        )
 
         precision: str = field(
             default="double",
             metadata={
                 "help_string": "use float or double precision",
                 "allowed_values": {"float", "double"},
-                "formatter": lambda precision: "--float {}".format({"double": 0, "float": 1}.get(precision)),
+                "formatter": lambda precision: f"-p {precision[0]}",
             },
         )
 
-        verbose: bool = field(
+        use_histogram_matching: bool = field(
             default=False,
             metadata={
-                "help_string": "enable verbose output",
-                "formatter": lambda verbose: f"--verbose {int(verbose)}",
+                "help_string": "use histogram matching",
+                "formatter": lambda use_histogram_matching: f"-j {int(use_histogram_matching)}",
             },
         )
 
+        use_reproducible_mode: bool = field(
+            default=False,
+            metadata={
+                "help_string": "use reproducible mode",
+                "formatter": lambda use_reproducible_mode: f"-y {int(use_reproducible_mode)}",
+            },
+        )
+
+        random_seed: int = field(metadata={"help_string": "fix random seed", "argstr": "-e"})
+
     input_spec = SpecInfo(name="Input", bases=(InputSpec,))
 
-    executable = "antsApplyTransforms"
+    @define(kw_only=True)
+    class OutputSpec(ShellOutSpec):
+        warped_moving_image: File = field(
+            metadata={
+                "help_string": "moving image warped to fixed image space",
+                "output_file_template": "{output_prefix}Warped.nii.gz",
+            }
+        )
+
+        warped_fixed_image: File = field(
+            metadata={
+                "help_string": "fixed image warped to moving image space",
+                "output_file_template": "{output_prefix}InverseWarped.nii.gz",
+            }
+        )
+
+        affine_transform: File = field(
+            metadata={
+                "help_string": "affine transform",
+                "output_file_template": "{output_prefix}0GenericAffine.mat",
+            }
+        )
+
+        forward_warp_field: File = field(
+            metadata={
+                "help_string": "forward warp field",
+                "callable": lambda transform_type, output_prefix: (
+                    f"{output_prefix}1Warp.nii.gz" if transform_type not in ("t", "r", "a") else NOTHING
+                ),
+            }
+        )
+
+        inverse_warp_field: File = field(
+            metadata={
+                "help_string": "inverse warp field",
+                "callable": lambda transform_type, output_prefix: (
+                    f"{output_prefix}1InverseWarp.nii.gz" if transform_type not in ("t", "r", "a") else NOTHING
+                ),
+            }
+        )
+
+    output_spec = SpecInfo(name="Output", bases=(OutputSpec,))
+
+    executable = "antsRegistrationSyNQuick.sh"
```

### Comparing `pydra_ants-0.0.2/src/pydra/tasks/ants/bias_correction.py` & `pydra_ants-0.0.3/src/pydra/tasks/ants/bias_correction.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Examples
 --------
 
 >>> task = N4BiasFieldCorrection(input_image="input.nii")
 >>> task.cmdline    # doctest: +ELLIPSIS
 'N4BiasFieldCorrection --input-image input.nii --rescale-intensities 1 --shrink-factor 4 \
 --bspline-fitting [200, 3] --convergence [50x50x50x50, 0.0] --histogram-sharpening [0.15, 0.01, 200] \
---output [.../input_corrected.nii, .../input_biasfield.nii]'
+--output .../input_corrected.nii'
 """
 
 __all__ = ["N4BiasFieldCorrection"]
 
 from os import PathLike
 from typing import Sequence
 
@@ -94,23 +94,27 @@
         wiener_filter_noise: float = field(default=0.01, metadata={"help_string": "Wiener filter noise"})
 
         num_histogram_bins: int = field(default=200, metadata={"help_string": "number of histogram bins"})
 
         output_parameters = field(
             metadata={
                 "help_string": "output parameters",
-                "argstr": "--output [{output_image}, {output_bias_field}]",
                 "readonly": True,
+                "formatter": lambda output_image, save_bias_field, output_bias_field: (
+                    f"--output [{output_image}, {output_bias_field}]" if save_bias_field else f"--output {output_image}"
+                ),
             }
         )
 
         output_image: str = field(
             metadata={"help_string": "output image", "output_file_template": "{input_image}_corrected"}
         )
 
+        save_bias_field: bool = field(default=False, metadata={"help_string": "save bias field"})
+
         output_bias_field: str = field(
             metadata={"help_string": "output bias field", "output_file_template": "{input_image}_biasfield"}
         )
 
     input_spec = SpecInfo(name="Input", bases=(InputSpec,))
 
     executable = "N4BiasFieldCorrection"
```

### Comparing `pydra_ants-0.0.2/src/pydra/tasks/ants/registration.py` & `pydra_ants-0.0.3/src/pydra/tasks/ants/apply_transforms.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,208 +1,199 @@
 """
-Registration
-============
+ApplyTransforms
+===============
 
 Examples
 --------
 
->>> task = RegistrationSyNQuick(
-...     dimensionality=3,
-...     fixed_image="reference.nii",
-...     moving_image="structural.nii",
-... )
+>>> task = ApplyTransforms(moving_image="moving.nii", fixed_image="fixed.nii")
 >>> task.cmdline    # doctest: +ELLIPSIS
-'antsRegistrationSyNQuick.sh -d 3 -f reference.nii -m structural.nii ...'
+'antsApplyTransforms -e scalar -i moving.nii -r fixed.nii -o .../moving_warped.nii -n Linear ...'
 
->>> task = RegistrationSyNQuick(
-...     dimensionality=3,
-...     fixed_image="reference.nii",
-...     moving_image="structural.nii", 
-...     transform_type="b",
-...     spline_distance=32,
-...     gradient_step_size=0.2,
-...     random_seed=42,
+>>> task = ApplyTransforms(
+...     moving_image="moving.nii",
+...     fixed_image="fixed.nii",
+...     interpolation="BSpline",
+...     transform_list=["affine.mat"],
 ... )
 >>> task.cmdline    # doctest: +ELLIPSIS
-'antsRegistrationSyNQuick.sh ... -t b -s 32 -g 0.2 ... -e 42'
+'antsApplyTransforms ... -n BSpline[3] -t affine.mat ...'
 
->>> task = RegistrationSyNQuick(
-...     dimensionality=3,
-...     fixed_image="reference.nii",
-...     moving_image="structural.nii",
-...     fixed_mask="mask.nii",
+>>> task = ApplyTransforms(
+...     moving_image="moving.nii",
+...     fixed_image="fixed.nii",
+...     interpolation="Gaussian",
+...     sigma=4.0,
+...     alpha=1.0,
+...     transform_list=["affine.mat", "warp_field.nii.gz"],
+...     which_to_invert=[True, False],
 ... )
 >>> task.cmdline    # doctest: +ELLIPSIS
-'antsRegistrationSyNQuick.sh ... -x mask.nii ...'
+'antsApplyTransforms ... -n Gaussian[4.0, 1.0] -t [affine.mat, 1] -t [warp_field.nii.gz, 0] ...'
 """
 
-__all__ = ["RegistrationSyNQuick"]
+__all__ = ["ApplyTransforms"]
 
 from os import PathLike
 from typing import Sequence
 
-from attrs import NOTHING, define, field
-from pydra.engine.specs import File, ShellOutSpec, ShellSpec, SpecInfo
+from attrs import define, field
+from pydra.engine.specs import ShellSpec, SpecInfo
 from pydra.engine.task import ShellCommandTask
 
 
-class RegistrationSyNQuick(ShellCommandTask):
-    """Task definition for antsRegistrationSyNQuick."""
+def _format_output_parameters(
+    output_image: PathLike,
+    save_warp_field: bool,
+    output_warp_field: PathLike,
+    save_transform: bool,
+    output_transform: PathLike,
+    invert_transform: bool,
+) -> str:
+    return "-o {}".format(
+        "Linear[{}, {:%d}]".format(output_transform, invert_transform)
+        if save_transform
+        else "[{}, {:%d}]".format(output_warp_field, save_warp_field)
+        if save_warp_field
+        else f"{output_image}"
+    )
+
+
+class ApplyTransforms(ShellCommandTask):
+    """Task definition for antsApplyTransforms."""
 
     @define(kw_only=True)
     class InputSpec(ShellSpec):
         dimensionality: int = field(
             metadata={
-                "help_string": "force image dimensionality (2 or 3)",
-                "mandatory": True,
+                "help_string": "force image dimensionality (2, 3 or 4)",
                 "argstr": "-d",
-                "allowed_values": {2, 3},
+                "allowed_values": {2, 3, 4},
             }
         )
 
-        fixed_image: PathLike = field(metadata={"help_string": "fixed image", "mandatory": True, "argstr": "-f"})
-
-        moving_image: PathLike = field(metadata={"help_string": "moving image", "mandatory": True, "argstr": "-m"})
-
-        output_prefix: str = field(
-            default="output", metadata={"help_string": "prefix for output files", "argstr": "-o"}
-        )
-
-        num_threads: int = field(default=1, metadata={"help_string": "number of threads", "argstr": "-n"})
-
-        initial_transforms: Sequence[PathLike] = field(metadata={"help_string": "initial transforms", "argstr": "-i"})
-
-        transform_type: str = field(
-            default="s",
-            metadata={
-                "help_string": "transform type",
-                "argstr": "-t",
-                "allowed_values": {
-                    "t",  # translation
-                    "r",  # rigid
-                    "a",  # rigid + affine
-                    "s",  # rigid + affine + syn
-                    "sr",  # rigid + syn
-                    "so",  # syn only
-                    "b",  # rigid + affine + b-spline
-                    "br",  # rigid + b-spline
-                    "bo",  # b-spline only
-                },
-            },
-        )
-
-        num_histogram_bins: int = field(
-            default=32,
+        image_type: str = field(
+            default="scalar",
             metadata={
-                "help_string": "number of histogram bins in SyN stage",
-                "formatter": lambda transform_type, num_histogram_bins: (
-                    f"-r {num_histogram_bins}" if "s" in transform_type else ""
+                "help_string": (
+                    "specify the image type (0: scalar, 1: vector, 2: tensor, 3: time-series, 4: multichannel,"
+                    " 5: five-dimensional)"
                 ),
+                "argstr": "-e",
+                "allowed_values": {0, 1, 2, 3, 4, 5},
             },
         )
 
-        spline_distance: float = field(
-            default=26,
-            metadata={
-                "help_string": "spline distance for deformable B-spline SyN transform",
-                "formatter": lambda transform_type, spline_distance: (
-                    f"-s {spline_distance}" if "b" in transform_type else ""
-                ),
-            },
-        )
+        moving_image: PathLike = field(metadata={"help_string": "moving image", "mandatory": True, "argstr": "-i"})
 
-        gradient_step_size: float = field(
-            default=0.1,
-            metadata={
-                "help_string": "gradient step size for SyN and B-spline SyN",
-                "formatter": lambda transform_type, gradient_step_size: (
-                    f"-g {gradient_step_size}" if any(c in transform_type for c in ("s", "b")) else ""
-                ),
-            },
-        )
+        fixed_image: PathLike = field(metadata={"help_string": "fixed image", "mandatory": True, "argstr": "-r"})
 
-        fixed_mask: PathLike = field(
+        output_parameters: str = field(
             metadata={
-                "help_string": "mask applied to the fixed image",
-                "formatter": lambda fixed_mask, moving_mask: (
-                    "" if not fixed_mask else f"-x {fixed_mask},{moving_mask}" if moving_mask else f"-x {fixed_mask}"
-                ),
+                "help_string": "output parameters",
+                "readonly": True,
+                "formatter": _format_output_parameters,
             }
         )
 
-        moving_mask: PathLike = field(
-            metadata={"help_string": "mask applied to the moving image", "requires": {"fixed_mask"}}
+        output_image: str = field(
+            metadata={"help_string": "output image", "output_file_template": "{moving_image}_warped"}
         )
 
-        precision: str = field(
-            default="double",
-            metadata={
-                "help_string": "use float or double precision",
-                "allowed_values": {"float", "double"},
-                "formatter": lambda precision: f"-p {precision[0]}",
-            },
+        save_warp_field: bool = field(metadata={"help_string": "save composite warp field"})
+
+        output_warp_field: str = field(
+            metadata={"help_string": "output warp field", "output_file_template": "{moving_image}_warpfield"}
         )
 
-        use_histogram_matching: bool = field(
-            default=False,
+        save_transform: bool = field(metadata={"help_string": "save composite transform"})
+
+        output_transform: str = field(
             metadata={
-                "help_string": "use histogram matching",
-                "formatter": lambda use_histogram_matching: f"-j {int(use_histogram_matching)}",
-            },
+                "help_string": "output transform",
+                "output_file_template": "{moving_image}_affine.mat",
+                "keep_extension": False,
+            }
         )
 
-        use_reproducible_mode: bool = field(
-            default=False,
+        invert_transform: bool = field(default=False, metadata={"help_string": "invert composite transform"})
+
+        interpolation: str = field(
+            default="Linear",
             metadata={
-                "help_string": "use reproducible mode",
-                "formatter": lambda use_reproducible_mode: f"-y {int(use_reproducible_mode)}",
+                "help_string": "interpolation method",
+                "allowed_values": {
+                    "Linear",
+                    "NearestNeighbor",
+                    "Gaussian",
+                    "BSpline",
+                    "CosineWindowedSinc",
+                    "WelchWindowedSinc",
+                    "HammingWindowedSinc",
+                    "LanczosWindowedSinc",
+                },
+                "formatter": lambda interpolation, sigma, alpha, spline_order: (
+                    f"-n {interpolation}"
+                    + (
+                        f"[{spline_order}]"
+                        if interpolation == "BSpline"
+                        else f"[{sigma}, {alpha}]"
+                        if interpolation in ("MultiLabel", "Gaussian")
+                        else ""
+                    )
+                ),
             },
         )
 
-        random_seed: int = field(metadata={"help_string": "fix random seed", "argstr": "-e"})
+        sigma: float = field(metadata={"help_string": "sigma parameter for MultiLabel and Gaussian interpolation"})
 
-    input_spec = SpecInfo(name="Input", bases=(InputSpec,))
+        alpha: float = field(metadata={"help_string": "alpha parameter for MultiLabel and Gaussian interpolation"})
 
-    @define(kw_only=True)
-    class OutputSpec(ShellOutSpec):
-        warped_moving_image: File = field(
+        spline_order: int = field(default=3, metadata={"help_string": "spline order for BSpline interpolation"})
+
+        output_datatype: str = field(
             metadata={
-                "help_string": "moving image warped to fixed image space",
-                "output_file_template": "{output_prefix}Warped.nii.gz",
+                "help_string": "force output image datatype",
+                "argstr": "-u",
+                "allowed_values": {"char", "uchar", "short", "int", "float", "double", "default"},
             }
         )
 
-        warped_fixed_image: File = field(
+        transform_list: Sequence[PathLike] = field(
             metadata={
-                "help_string": "fixed image warped to moving image space",
-                "output_file_template": "{output_prefix}InverseWarped.nii.gz",
+                "help_string": "list of transforms to apply",
+                "formatter": lambda transform_list, which_to_invert: (
+                    ""
+                    if not transform_list
+                    else " ".join(f"-t {f}" for f in transform_list)
+                    if not which_to_invert
+                    else " ".join(f"-t [{f}, {int(i)}]" for f, i in zip(transform_list, which_to_invert))
+                ),
             }
         )
 
-        affine_transform: File = field(
-            metadata={
-                "help_string": "affine transform",
-                "output_file_template": "{output_prefix}0GenericAffine.mat",
-            }
+        which_to_invert: Sequence[bool] = field(
+            metadata={"help_string": "specify which transforms to invert", "requires": {"transform_list"}}
         )
 
-        forward_warp_field: File = field(
+        default_value: float = field(metadata={"help_string": "default voxel value", "argstr": "-f"})
+
+        precision: str = field(
+            default="double",
             metadata={
-                "help_string": "forward warp field",
-                "callable": lambda transform_type, output_prefix: (
-                    f"{output_prefix}1Warp.nii.gz" if transform_type not in ("t", "r", "a") else NOTHING
-                ),
-            }
+                "help_string": "use float or double precision",
+                "allowed_values": {"float", "double"},
+                "formatter": lambda precision: "--float {}".format({"double": 0, "float": 1}.get(precision)),
+            },
         )
 
-        inverse_warp_field: File = field(
+        verbose: bool = field(
+            default=False,
             metadata={
-                "help_string": "inverse warp field",
-                "callable": lambda transform_type, output_prefix: (
-                    f"{output_prefix}1InverseWarp.nii.gz" if transform_type not in ("t", "r", "a") else NOTHING
-                ),
-            }
+                "help_string": "enable verbose output",
+                "formatter": lambda verbose: f"--verbose {int(verbose)}",
+            },
         )
 
-    output_spec = SpecInfo(name="Output", bases=(OutputSpec,))
+    input_spec = SpecInfo(name="Input", bases=(InputSpec,))
 
-    executable = "antsRegistrationSyNQuick.sh"
+    executable = "antsApplyTransforms"
```

### Comparing `pydra_ants-0.0.2/.gitignore` & `pydra_ants-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.2/LICENSE` & `pydra_ants-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.2/README.md` & `pydra_ants-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.2/pyproject.toml` & `pydra_ants-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydra-ants"
-version = "0.0.2"
+version = "0.0.3"
 description = "Pydra tasks for ANTs"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = [
   "ants",
   "neuroimaging",
```

### Comparing `pydra_ants-0.0.2/PKG-INFO` & `pydra_ants-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydra-ants
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pydra tasks for ANTs
 Project-URL: Documentation, https://github.com/ghisvail/pydra-ants#readme
 Project-URL: Issues, https://github.com/ghisvail/pydra-ants/issues
 Project-URL: Source, https://github.com/ghisvail/pydra-ants
 Author-email: Ghislain Vaillant <ghislain.vaillant@icm-institute.org>
 License-Expression: MIT
 License-File: LICENSE
```

