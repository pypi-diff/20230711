# Comparing `tmp/FigureGenerator-0.0.3.tar.gz` & `tmp/FigureGenerator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FigureGenerator-0.0.3.tar", last modified: Tue Jul 11 02:18:40 2023, max compression
+gzip compressed data, was "FigureGenerator-0.0.4.tar", last modified: Tue Jul 11 13:55:39 2023, max compression
```

## Comparing `FigureGenerator-0.0.3.tar` & `FigureGenerator-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 02:18:40.287713 FigureGenerator-0.0.3/
--rw-rw-rw-   0        0        0     3432 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1504 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2023-07-11 02:18:40.257713 FigureGenerator-0.0.3/FigureGenerator/
--rw-rw-rw-   0        0        0      117 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/FigureGenerator/__init__.py
--rw-rw-rw-   0        0        0    15592 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/FigureGenerator/screenshot_maker.py
--rw-rw-rw-   0        0        0    10350 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/FigureGenerator/utils.py
--rw-rw-rw-   0        0        0       72 2023-07-11 02:06:55.000000 FigureGenerator-0.0.3/FigureGenerator/version.py
-drwxrwxrwx   0        0        0        0 2023-07-11 02:18:40.283715 FigureGenerator-0.0.3/FigureGenerator.egg-info/
--rw-rw-rw-   0        0        0     6557 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-11 02:17:53.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       97 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      282 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       29 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6557 2023-07-11 02:18:40.286713 FigureGenerator-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5788 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/README.md
--rw-rw-rw-   0        0        0      538 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/SECURITY.md
--rw-rw-rw-   0        0        0     3804 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/figure_generator
--rw-rw-rw-   0        0        0       42 2023-07-11 02:18:40.287713 FigureGenerator-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1789 2023-07-11 02:07:37.000000 FigureGenerator-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:55:39.601111 FigureGenerator-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:55:39.597111 FigureGenerator-0.0.4/FigureGenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/FigureGenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/FigureGenerator/screenshot_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/FigureGenerator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/FigureGenerator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:55:39.601111 FigureGenerator-0.0.4/FigureGenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-11 13:55:39.000000 FigureGenerator-0.0.4/FigureGenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-11 13:55:39.000000 FigureGenerator-0.0.4/FigureGenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:55:39.000000 FigureGenerator-0.0.4/FigureGenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:55:30.000000 FigureGenerator-0.0.4/FigureGenerator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-11 13:55:39.000000 FigureGenerator-0.0.4/FigureGenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 13:55:39.000000 FigureGenerator-0.0.4/FigureGenerator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-11 13:55:39.601111 FigureGenerator-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/figure_generator
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:55:39.601111 FigureGenerator-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-11 13:55:09.000000 FigureGenerator-0.0.4/setup.py
```

### Comparing `FigureGenerator-0.0.3/CODE_OF_CONDUCT.md` & `FigureGenerator-0.0.4/CODE_OF_CONDUCT.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# Contributor Covenant Code of Conduct
-
-## Our Pledge
-
-In the interest of fostering an open and welcoming environment, we as
-contributors and maintainers pledge to making participation in our project and
-our community a harassment-free experience for everyone, regardless of age, body
-size, disability, ethnicity, sex characteristics, gender identity and expression,
-level of experience, education, socio-economic status, nationality, personal
-appearance, race, religion, or sexual identity and orientation.
-
-## Our Standards
-
-Examples of behavior that contributes to creating a positive environment
-include:
-
-* Using welcoming and inclusive language
-* Being respectful of differing viewpoints and experiences
-* Gracefully accepting constructive criticism
-* Focusing on what is best for the community
-* Showing empathy towards other community members
-
-Examples of unacceptable behavior by participants include:
-
-* The use of sexualized language or imagery and unwelcome sexual attention or
- advances
-* Trolling, insulting/derogatory comments, and personal or political attacks
-* Public or private harassment
-* Publishing others' private information, such as a physical or electronic
- address, without explicit permission
-* Other conduct which could reasonably be considered inappropriate in a
- professional setting
-
-## Our Responsibilities
-
-Project maintainers are responsible for clarifying the standards of acceptable
-behavior and are expected to take appropriate and fair corrective action in
-response to any instances of unacceptable behavior.
-
-Project maintainers have the right and responsibility to remove, edit, or
-reject comments, commits, code, wiki edits, issues, and other contributions
-that are not aligned to this Code of Conduct, or to ban temporarily or
-permanently any contributor for other behaviors that they deem inappropriate,
-threatening, offensive, or harmful.
-
-## Scope
-
-This Code of Conduct applies both within project spaces and in public spaces
-when an individual is representing the project or its community. Examples of
-representing a project or community include using an official project e-mail
-address, posting via an official social media account, or acting as an appointed
-representative at an online or offline event. Representation of a project may be
-further defined and clarified by project maintainers.
-
-## Enforcement
-
-Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported by contacting the project team at software@cbica.upenn.edu. All
-complaints will be reviewed and investigated and will result in a response that
-is deemed necessary and appropriate to the circumstances. The project team is
-obligated to maintain confidentiality with regard to the reporter of an incident.
-Further details of specific enforcement policies may be posted separately.
-
-Project maintainers who do not follow or enforce the Code of Conduct in good
-faith may face temporary or permanent repercussions as determined by other
-members of the project's leadership.
-
-## Attribution
-
-This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
-available at https://www.contributor-covenant.org/version/1/4/code-of-conduct.html
-
-[homepage]: https://www.contributor-covenant.org
-
-For answers to common questions about this code of conduct, see
-https://www.contributor-covenant.org/faq
+# Contributor Covenant Code of Conduct
+
+## Our Pledge
+
+In the interest of fostering an open and welcoming environment, we as
+contributors and maintainers pledge to making participation in our project and
+our community a harassment-free experience for everyone, regardless of age, body
+size, disability, ethnicity, sex characteristics, gender identity and expression,
+level of experience, education, socio-economic status, nationality, personal
+appearance, race, religion, or sexual identity and orientation.
+
+## Our Standards
+
+Examples of behavior that contributes to creating a positive environment
+include:
+
+* Using welcoming and inclusive language
+* Being respectful of differing viewpoints and experiences
+* Gracefully accepting constructive criticism
+* Focusing on what is best for the community
+* Showing empathy towards other community members
+
+Examples of unacceptable behavior by participants include:
+
+* The use of sexualized language or imagery and unwelcome sexual attention or
+ advances
+* Trolling, insulting/derogatory comments, and personal or political attacks
+* Public or private harassment
+* Publishing others' private information, such as a physical or electronic
+ address, without explicit permission
+* Other conduct which could reasonably be considered inappropriate in a
+ professional setting
+
+## Our Responsibilities
+
+Project maintainers are responsible for clarifying the standards of acceptable
+behavior and are expected to take appropriate and fair corrective action in
+response to any instances of unacceptable behavior.
+
+Project maintainers have the right and responsibility to remove, edit, or
+reject comments, commits, code, wiki edits, issues, and other contributions
+that are not aligned to this Code of Conduct, or to ban temporarily or
+permanently any contributor for other behaviors that they deem inappropriate,
+threatening, offensive, or harmful.
+
+## Scope
+
+This Code of Conduct applies both within project spaces and in public spaces
+when an individual is representing the project or its community. Examples of
+representing a project or community include using an official project e-mail
+address, posting via an official social media account, or acting as an appointed
+representative at an online or offline event. Representation of a project may be
+further defined and clarified by project maintainers.
+
+## Enforcement
+
+Instances of abusive, harassing, or otherwise unacceptable behavior may be
+reported by contacting the project team at software@cbica.upenn.edu. All
+complaints will be reviewed and investigated and will result in a response that
+is deemed necessary and appropriate to the circumstances. The project team is
+obligated to maintain confidentiality with regard to the reporter of an incident.
+Further details of specific enforcement policies may be posted separately.
+
+Project maintainers who do not follow or enforce the Code of Conduct in good
+faith may face temporary or permanent repercussions as determined by other
+members of the project's leadership.
+
+## Attribution
+
+This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
+available at https://www.contributor-covenant.org/version/1/4/code-of-conduct.html
+
+[homepage]: https://www.contributor-covenant.org
+
+For answers to common questions about this code of conduct, see
+https://www.contributor-covenant.org/faq
```

### Comparing `FigureGenerator-0.0.3/CONTRIBUTING.md` & `FigureGenerator-0.0.4/CONTRIBUTING.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# Contribution Guidelines
-
-FigureGenerator is a package that is primarily worked on by the CBICA Software Development team and its collaborators - additional members from the community are welcome!
-
-## Issues
-
-The easiest way to contribute is by reporting issues is through the [GitHub](https://github.com/CBICA/FigureGenerator/issues). 
-When reporting an issue, please ensure you fill out as much information from the templates as possible for us to debug and diagnose it.
-
-## Feature Requests
-
-If you have a particular feature in mind, please submit it via the new Feature Request system via [GitHub](https://github.com/CBICA/FigureGenerator/issues). 
-
-Depending on our bandwidth, one of the team members will get around to it (we will always respond ASAP).
-
-## Pull Requests
-
-Thank you for your interest in contributing to **FigureGenerator**! To make the process as smooth as possible, please follow these guidelines for speedy reviews and merges:
-
-- Ensure your PR addresses an existing issue (if none exists, please open one so that it can be triaged by the admins).
-- Your PR should be from a branch that either contains the issue number it fixes and/or contains as much top-level information as possible to help moderators review and merge it.
-- Include tests for your PR
-- Update documentation for the added functionality (if any)
-
-## Details
-
-Please feel free to email us at software@cbica.upenn.edu, where we will be more than happy to answer any and all questions.
+# Contribution Guidelines
+
+FigureGenerator is a package that is primarily worked on by the CBICA Software Development team and its collaborators - additional members from the community are welcome!
+
+## Issues
+
+The easiest way to contribute is by reporting issues is through the [GitHub](https://github.com/CBICA/FigureGenerator/issues). 
+When reporting an issue, please ensure you fill out as much information from the templates as possible for us to debug and diagnose it.
+
+## Feature Requests
+
+If you have a particular feature in mind, please submit it via the new Feature Request system via [GitHub](https://github.com/CBICA/FigureGenerator/issues). 
+
+Depending on our bandwidth, one of the team members will get around to it (we will always respond ASAP).
+
+## Pull Requests
+
+Thank you for your interest in contributing to **FigureGenerator**! To make the process as smooth as possible, please follow these guidelines for speedy reviews and merges:
+
+- Ensure your PR addresses an existing issue (if none exists, please open one so that it can be triaged by the admins).
+- Your PR should be from a branch that either contains the issue number it fixes and/or contains as much top-level information as possible to help moderators review and merge it.
+- Include tests for your PR
+- Update documentation for the added functionality (if any)
+
+## Details
+
+Please feel free to email us at software@cbica.upenn.edu, where we will be more than happy to answer any and all questions.
```

### Comparing `FigureGenerator-0.0.3/FigureGenerator/utils.py` & `FigureGenerator-0.0.4/FigureGenerator/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,285 +1,285 @@
-import math, os
-import SimpleITK as sitk
-
-## color_map look-up table
-# colomap_lut = {
-#     "red": sitk.ScalarToRGBColormapImageFilter.Red,
-#     "green": sitk.ScalarToRGBColormapImageFilter.Green,
-#     "blue": sitk.ScalarToRGBColormapImageFilter.Blue,
-#     "grey": sitk.ScalarToRGBColormapImageFilter.Grey,
-#     "hot": sitk.ScalarToRGBColormapImageFilter.Hot,
-#     "cool": sitk.ScalarToRGBColormapImageFilter.Cool,
-#     "spring": sitk.ScalarToRGBColormapImageFilter.Spring,
-#     "summer": sitk.ScalarToRGBColormapImageFilter.Summer,
-#     "autumn": sitk.ScalarToRGBColormapImageFilter.Autumn,
-#     "winter": sitk.ScalarToRGBColormapImageFilter.Winter,
-#     "copper": sitk.ScalarToRGBColormapImageFilter.Copper,
-#     "jet": sitk.ScalarToRGBColormapImageFilter.Jet,
-#     "hsv": sitk.ScalarToRGBColormapImageFilter.HSV,
-#     "overunder": sitk.ScalarToRGBColormapImageFilter.OverUnder,
-# }
-
-
-def get_basename_sanitized(file_name):
-    """
-    Get the basename of the input file, without the extension.
-
-    Args:
-        file_name (str): The input file name.
-
-    Returns:
-        str: The basename of the input file.
-    """
-    temp_file = file_name
-    if file_name.endswith(".nii.gz"):
-        temp_file = file_name.replace(".nii.gz", "")
-    return os.path.splitext(os.path.basename(temp_file))[0]
-
-
-def sanity_checker_base(file_reader_base, images_to_check):
-    """
-    This function performs sanity check on a list of images to ensure presence of consistent header information WITHOUT loading images into memory.
-
-    Args:
-        file_reader_base (SimpleITK.ImageFileReader): File reader for the base image.
-        images_to_check (list): List of images paths to check.
-
-    Raises:
-        ValueError: Dimension mismatch in the images.
-        ValueError: Origin mismatch in the images.
-        ValueError: Orientation mismatch in the images.
-        ValueError: Spacing mismatch in the images.
-
-    Returns:
-        bool: Result of sanity checking.
-    """
-    if images_to_check is None:
-        return True
-
-    for image in images_to_check:
-        file_reader_current = sitk.ImageFileReader()
-        file_reader_current.SetFileName(image)
-        file_reader_current.ReadImageInformation()
-
-        if file_reader_base.GetDimension() != file_reader_current.GetDimension():
-            raise ValueError("Dimensions for subject are not consistent.")
-
-        if file_reader_base.GetOrigin() != file_reader_current.GetOrigin():
-            raise ValueError("Origin for subject are not consistent.")
-
-        if file_reader_base.GetDirection() != file_reader_current.GetDirection():
-            raise ValueError("Orientation for subject are not consistent.")
-
-        if file_reader_base.GetSpacing() != file_reader_current.GetSpacing():
-            raise ValueError("Spacing for subject are not consistent.")
-
-    return True
-
-
-def sanity_checker_with_files(image_file_1, image_file_2):
-    """
-    This function performs sanity check on 2 image files WITHOUT loading images into memory.
-
-    Args:
-        image_file_1 (str): First image to check.
-        image_file_2 (str): Second image to check.
-
-    Raises:
-        ValueError: Dimension mismatch in the images.
-        ValueError: Origin mismatch in the images.
-        ValueError: Orientation mismatch in the images.
-        ValueError: Spacing mismatch in the images.
-
-    Returns:
-        bool: Result of sanity checking.
-    """
-    file_reader_current = sitk.ImageFileReader()
-    file_reader_current.SetFileName(image_file_1)
-    file_reader_current.ReadImageInformation()
-    return sanity_checker_base(file_reader_current, [image_file_2])
-
-
-def rescale_intensity(image):
-    """
-    Rescale the intensity of an image.
-
-    Args:
-        image (SimpleITK.Image): The input image.
-
-    Returns:
-        SimpleITK.Image: The rescaled image.
-    """
-    rescaler = sitk.RescaleIntensityImageFilter()
-    rescaler.SetOutputMinimum(0)
-    rescaler.SetOutputMaximum(255)
-    return rescaler.Execute(image)
-
-
-def resample_image(
-    img, spacing=None, size=None, interpolator=sitk.sitkLinear, outsideValue=0
-):
-    """
-    Resample image to certain spacing and size.
-
-    Args:
-        img (SimpleITK.Image): The input image to resample.
-        spacing (list): List of length 3 indicating the voxel spacing as [x, y, z].
-        size (list, optional): List of length 3 indicating the number of voxels per dim [x, y, z], which will use compute the appropriate size based on the spacing. Defaults to [].
-        interpolator (SimpleITK.InterpolatorEnum, optional): The interpolation type to use. Defaults to SimpleITK.sitkLinear.
-        origin (list, optional): The location in physical space representing the [0,0,0] voxel in the input image.  Defaults to [0,0,0].
-        outsideValue (int, optional): value used to pad are outside image.  Defaults to 0.
-
-    Raises:
-        Exception: Spacing/resolution mismatch.
-        Exception: Size mismatch.
-
-    Returns:
-        SimpleITK.Image: The resampled input image.
-    """
-    # initialize spacing to '1' for isotropic
-    if spacing is None:
-        spacing = []
-        min_org_spacing = min(img.GetSpacing())
-        spacing = [min_org_spacing for _ in range(0, img.GetDimension())]
-    elif len(spacing) != img.GetDimension():
-        raise Exception("len(spacing) != " + str(img.GetDimension()))
-
-    # Set Size
-    if size == None:
-        inSpacing = img.GetSpacing()
-        inSize = img.GetSize()
-        size = [
-            int(math.ceil(inSize[i] * (inSpacing[i] / spacing[i])))
-            for i in range(img.GetDimension())
-        ]
-    else:
-        if len(size) != img.GetDimension():
-            raise Exception("len(size) != " + str(img.GetDimension()))
-
-    # Resample input image
-    resampled_image = sitk.Resample(
-        img,
-        size,
-        sitk.Transform(),
-        interpolator,
-        img.GetOrigin(),
-        spacing,
-        img.GetDirection(),
-        outsideValue,
-    )
-
-    orienter = sitk.DICOMOrientImageFilter()
-    orienter.SetDesiredCoordinateOrientation("RAI")
-    oriented_image = orienter.Execute(resampled_image)
-
-    if oriented_image.GetDimension() == 3:
-        oriented_image.SetOrigin((0, 0, 0))
-        oriented_image.SetDirection((1, 0, 0, 0, 1, 0, 0, 0, 1))
-    elif oriented_image.GetDimension() == 2:
-        oriented_image.SetOrigin((0, 0))
-        oriented_image.SetDirection((1, 0, 0, 1))
-
-    size = oriented_image.GetSize()
-    max_size = max(size)
-
-    padding = [0] * oriented_image.GetDimension()
-
-    for i in range(oriented_image.GetDimension()):
-        padding[i] = int(math.floor(max_size - size[i]) / 2.0)
-
-    padded_image = sitk.ConstantPad(oriented_image, padding, padding, 0.0)
-
-    return padded_image
-
-
-def binarize_image(image):
-    """
-    Binarize the input image.
-
-    Args:
-        image (SimpleITK.Image): The input image, all pixel values are expected to be between 0 and 255.
-
-    Returns:
-        SimpleITK.Image: The binarized image.
-    """
-    max_filter = sitk.MinimumMaximumImageFilter()
-    max_filter.Execute(image)
-    thresholder = sitk.BinaryThresholdImageFilter()
-    thresholder.SetOutsideValue(0)
-    thresholder.SetInsideValue(1)
-    thresholder.SetLowerThreshold(1)
-    thresholder.SetUpperThreshold(max_filter.GetMaximum())
-    return thresholder.Execute(image)
-
-
-def get_bounding_box(image, mask, border_pc):
-    """
-    Get the bounding box of the image based on the first mask after it is binarized.
-
-    Args:
-        image (SimpleITK.Image): The input image.
-        mask (SimpleITK.Image): The ground truth mask.
-        border_pc (float): The percentage of the image size to consider as the border.
-
-    Returns:
-        list: The bounding box in the form of [x_min, x_max, y_min, y_max, z_min, z_max]
-    """
-    size = image.GetSize()
-    if mask is not None:
-        extractor = sitk.LabelStatisticsImageFilter()
-        extractor.Execute(image, binarize_image(mask))
-        bb = list(extractor.GetBoundingBox(1))
-        bb[0] = max(0, math.floor(bb[0] - border_pc * size[0]))
-        bb[2] = max(0, math.floor(bb[2] - border_pc * size[1]))
-        bb[4] = max(0, math.floor(bb[4] - border_pc * size[2]))
-
-        full_min = min(bb[0], bb[2], bb[4])
-        bb[0], bb[2], bb[4] = full_min, full_min, full_min
-
-        bb[1] = min(size[0], math.floor(bb[1] + border_pc * size[0]))
-        bb[3] = min(size[1], math.floor(bb[3] + border_pc * size[1]))
-        bb[5] = min(size[2], math.floor(bb[5] + border_pc * size[2]))
-        full_max = max(bb[1], bb[3], bb[5])
-        bb[1], bb[3], bb[5] = full_max, full_max, full_max
-
-        return bb
-    else:
-        if len(size) == 3:
-            return (0, size[0] - 1, 0, size[1] - 1, 0, size[2] - 1)
-        elif len(size) == 2:
-            return (0, size[0] - 1, 0, size[1] - 1)
-
-
-def alpha_blend(image, mask=None, alpha=0.5):
-    """
-    Alpha blend an image and a mask with specified opacity.
-
-    Adapted from https://github.com/SimpleITK/NIH2019_COURSE/blob/master/09_results_visualization.ipynb
-
-    Args:
-        image (SimpleITK.Image): The input image.
-        mask (SimpleITK.Image): The input mask. Defaults to None.
-        alpha (float): The alpha value to use. Defaults to 0.5.
-
-    Returns:
-        list: The bounding box in the form of [x_min, x_max, y_min, y_max, z_min, z_max]
-    """
-
-    if not mask:
-        mask = sitk.Image(image.GetSize(), sitk.sitkUInt8)
-        mask.CopyInformation(image)
-
-    ## the r was not getting visualized, so commented out
-    # r = [255,0,0]
-    # g = [0,255,0]
-    # b = [0,0,255]
-    # return sitk.LabelOverlay(image=sitk.Cast(image, sitk.sitkUInt8),
-    #                                  labelImage=mask,
-    #                                  opacity=alpha, backgroundValue = 0,
-    #                                  colormap=r+g+b)
-
-    filter_overlay = sitk.LabelOverlayImageFilter()
-    filter_overlay.SetOpacity(alpha)
-    # filter_overlay.SetBackgroundValue(0)
-    # filter_overlay.SetColormap(r+g+b)
-    return filter_overlay.Execute(sitk.Cast(image, sitk.sitkUInt8), sitk.Cast(mask, sitk.sitkUInt8))
+import math, os
+import SimpleITK as sitk
+
+## color_map look-up table
+# colomap_lut = {
+#     "red": sitk.ScalarToRGBColormapImageFilter.Red,
+#     "green": sitk.ScalarToRGBColormapImageFilter.Green,
+#     "blue": sitk.ScalarToRGBColormapImageFilter.Blue,
+#     "grey": sitk.ScalarToRGBColormapImageFilter.Grey,
+#     "hot": sitk.ScalarToRGBColormapImageFilter.Hot,
+#     "cool": sitk.ScalarToRGBColormapImageFilter.Cool,
+#     "spring": sitk.ScalarToRGBColormapImageFilter.Spring,
+#     "summer": sitk.ScalarToRGBColormapImageFilter.Summer,
+#     "autumn": sitk.ScalarToRGBColormapImageFilter.Autumn,
+#     "winter": sitk.ScalarToRGBColormapImageFilter.Winter,
+#     "copper": sitk.ScalarToRGBColormapImageFilter.Copper,
+#     "jet": sitk.ScalarToRGBColormapImageFilter.Jet,
+#     "hsv": sitk.ScalarToRGBColormapImageFilter.HSV,
+#     "overunder": sitk.ScalarToRGBColormapImageFilter.OverUnder,
+# }
+
+
+def get_basename_sanitized(file_name):
+    """
+    Get the basename of the input file, without the extension.
+
+    Args:
+        file_name (str): The input file name.
+
+    Returns:
+        str: The basename of the input file.
+    """
+    temp_file = file_name
+    if file_name.endswith(".nii.gz"):
+        temp_file = file_name.replace(".nii.gz", "")
+    return os.path.splitext(os.path.basename(temp_file))[0]
+
+
+def sanity_checker_base(file_reader_base, images_to_check):
+    """
+    This function performs sanity check on a list of images to ensure presence of consistent header information WITHOUT loading images into memory.
+
+    Args:
+        file_reader_base (SimpleITK.ImageFileReader): File reader for the base image.
+        images_to_check (list): List of images paths to check.
+
+    Raises:
+        ValueError: Dimension mismatch in the images.
+        ValueError: Origin mismatch in the images.
+        ValueError: Orientation mismatch in the images.
+        ValueError: Spacing mismatch in the images.
+
+    Returns:
+        bool: Result of sanity checking.
+    """
+    if images_to_check is None:
+        return True
+
+    for image in images_to_check:
+        file_reader_current = sitk.ImageFileReader()
+        file_reader_current.SetFileName(image)
+        file_reader_current.ReadImageInformation()
+
+        if file_reader_base.GetDimension() != file_reader_current.GetDimension():
+            raise ValueError("Dimensions for subject are not consistent.")
+
+        if file_reader_base.GetOrigin() != file_reader_current.GetOrigin():
+            raise ValueError("Origin for subject are not consistent.")
+
+        if file_reader_base.GetDirection() != file_reader_current.GetDirection():
+            raise ValueError("Orientation for subject are not consistent.")
+
+        if file_reader_base.GetSpacing() != file_reader_current.GetSpacing():
+            raise ValueError("Spacing for subject are not consistent.")
+
+    return True
+
+
+def sanity_checker_with_files(image_file_1, image_file_2):
+    """
+    This function performs sanity check on 2 image files WITHOUT loading images into memory.
+
+    Args:
+        image_file_1 (str): First image to check.
+        image_file_2 (str): Second image to check.
+
+    Raises:
+        ValueError: Dimension mismatch in the images.
+        ValueError: Origin mismatch in the images.
+        ValueError: Orientation mismatch in the images.
+        ValueError: Spacing mismatch in the images.
+
+    Returns:
+        bool: Result of sanity checking.
+    """
+    file_reader_current = sitk.ImageFileReader()
+    file_reader_current.SetFileName(image_file_1)
+    file_reader_current.ReadImageInformation()
+    return sanity_checker_base(file_reader_current, [image_file_2])
+
+
+def rescale_intensity(image):
+    """
+    Rescale the intensity of an image.
+
+    Args:
+        image (SimpleITK.Image): The input image.
+
+    Returns:
+        SimpleITK.Image: The rescaled image.
+    """
+    rescaler = sitk.RescaleIntensityImageFilter()
+    rescaler.SetOutputMinimum(0)
+    rescaler.SetOutputMaximum(255)
+    return rescaler.Execute(image)
+
+
+def resample_image(
+    img, spacing=None, size=None, interpolator=sitk.sitkLinear, outsideValue=0
+):
+    """
+    Resample image to certain spacing and size.
+
+    Args:
+        img (SimpleITK.Image): The input image to resample.
+        spacing (list): List of length 3 indicating the voxel spacing as [x, y, z].
+        size (list, optional): List of length 3 indicating the number of voxels per dim [x, y, z], which will use compute the appropriate size based on the spacing. Defaults to [].
+        interpolator (SimpleITK.InterpolatorEnum, optional): The interpolation type to use. Defaults to SimpleITK.sitkLinear.
+        origin (list, optional): The location in physical space representing the [0,0,0] voxel in the input image.  Defaults to [0,0,0].
+        outsideValue (int, optional): value used to pad are outside image.  Defaults to 0.
+
+    Raises:
+        Exception: Spacing/resolution mismatch.
+        Exception: Size mismatch.
+
+    Returns:
+        SimpleITK.Image: The resampled input image.
+    """
+    # initialize spacing to '1' for isotropic
+    if spacing is None:
+        spacing = []
+        min_org_spacing = min(img.GetSpacing())
+        spacing = [min_org_spacing for _ in range(0, img.GetDimension())]
+    elif len(spacing) != img.GetDimension():
+        raise Exception("len(spacing) != " + str(img.GetDimension()))
+
+    # Set Size
+    if size == None:
+        inSpacing = img.GetSpacing()
+        inSize = img.GetSize()
+        size = [
+            int(math.ceil(inSize[i] * (inSpacing[i] / spacing[i])))
+            for i in range(img.GetDimension())
+        ]
+    else:
+        if len(size) != img.GetDimension():
+            raise Exception("len(size) != " + str(img.GetDimension()))
+
+    # Resample input image
+    resampled_image = sitk.Resample(
+        img,
+        size,
+        sitk.Transform(),
+        interpolator,
+        img.GetOrigin(),
+        spacing,
+        img.GetDirection(),
+        outsideValue,
+    )
+
+    orienter = sitk.DICOMOrientImageFilter()
+    orienter.SetDesiredCoordinateOrientation("RAI")
+    oriented_image = orienter.Execute(resampled_image)
+
+    if oriented_image.GetDimension() == 3:
+        oriented_image.SetOrigin((0, 0, 0))
+        oriented_image.SetDirection((1, 0, 0, 0, 1, 0, 0, 0, 1))
+    elif oriented_image.GetDimension() == 2:
+        oriented_image.SetOrigin((0, 0))
+        oriented_image.SetDirection((1, 0, 0, 1))
+
+    size = oriented_image.GetSize()
+    max_size = max(size)
+
+    padding = [0] * oriented_image.GetDimension()
+
+    for i in range(oriented_image.GetDimension()):
+        padding[i] = int(math.floor(max_size - size[i]) / 2.0)
+
+    padded_image = sitk.ConstantPad(oriented_image, padding, padding, 0.0)
+
+    return padded_image
+
+
+def binarize_image(image):
+    """
+    Binarize the input image.
+
+    Args:
+        image (SimpleITK.Image): The input image, all pixel values are expected to be between 0 and 255.
+
+    Returns:
+        SimpleITK.Image: The binarized image.
+    """
+    max_filter = sitk.MinimumMaximumImageFilter()
+    max_filter.Execute(image)
+    thresholder = sitk.BinaryThresholdImageFilter()
+    thresholder.SetOutsideValue(0)
+    thresholder.SetInsideValue(1)
+    thresholder.SetLowerThreshold(1)
+    thresholder.SetUpperThreshold(max_filter.GetMaximum())
+    return thresholder.Execute(image)
+
+
+def get_bounding_box(image, mask, border_pc):
+    """
+    Get the bounding box of the image based on the first mask after it is binarized.
+
+    Args:
+        image (SimpleITK.Image): The input image.
+        mask (SimpleITK.Image): The ground truth mask.
+        border_pc (float): The percentage of the image size to consider as the border.
+
+    Returns:
+        list: The bounding box in the form of [x_min, x_max, y_min, y_max, z_min, z_max]
+    """
+    size = image.GetSize()
+    if mask is not None:
+        extractor = sitk.LabelStatisticsImageFilter()
+        extractor.Execute(image, binarize_image(mask))
+        bb = list(extractor.GetBoundingBox(1))
+        bb[0] = max(0, math.floor(bb[0] - border_pc * size[0]))
+        bb[2] = max(0, math.floor(bb[2] - border_pc * size[1]))
+        bb[4] = max(0, math.floor(bb[4] - border_pc * size[2]))
+
+        full_min = min(bb[0], bb[2], bb[4])
+        bb[0], bb[2], bb[4] = full_min, full_min, full_min
+
+        bb[1] = min(size[0], math.floor(bb[1] + border_pc * size[0]))
+        bb[3] = min(size[1], math.floor(bb[3] + border_pc * size[1]))
+        bb[5] = min(size[2], math.floor(bb[5] + border_pc * size[2]))
+        full_max = max(bb[1], bb[3], bb[5])
+        bb[1], bb[3], bb[5] = full_max, full_max, full_max
+
+        return bb
+    else:
+        if len(size) == 3:
+            return (0, size[0] - 1, 0, size[1] - 1, 0, size[2] - 1)
+        elif len(size) == 2:
+            return (0, size[0] - 1, 0, size[1] - 1)
+
+
+def alpha_blend(image, mask=None, alpha=0.5):
+    """
+    Alpha blend an image and a mask with specified opacity.
+
+    Adapted from https://github.com/SimpleITK/NIH2019_COURSE/blob/master/09_results_visualization.ipynb
+
+    Args:
+        image (SimpleITK.Image): The input image.
+        mask (SimpleITK.Image): The input mask. Defaults to None.
+        alpha (float): The alpha value to use. Defaults to 0.5.
+
+    Returns:
+        list: The bounding box in the form of [x_min, x_max, y_min, y_max, z_min, z_max]
+    """
+
+    if not mask:
+        mask = sitk.Image(image.GetSize(), sitk.sitkUInt8)
+        mask.CopyInformation(image)
+
+    ## the r was not getting visualized, so commented out
+    # r = [255,0,0]
+    # g = [0,255,0]
+    # b = [0,0,255]
+    # return sitk.LabelOverlay(image=sitk.Cast(image, sitk.sitkUInt8),
+    #                                  labelImage=mask,
+    #                                  opacity=alpha, backgroundValue = 0,
+    #                                  colormap=r+g+b)
+
+    filter_overlay = sitk.LabelOverlayImageFilter()
+    filter_overlay.SetOpacity(alpha)
+    # filter_overlay.SetBackgroundValue(0)
+    # filter_overlay.SetColormap(r+g+b)
+    return filter_overlay.Execute(sitk.Cast(image, sitk.sitkUInt8), sitk.Cast(mask, sitk.sitkUInt8))
```

### Comparing `FigureGenerator-0.0.3/FigureGenerator.egg-info/PKG-INFO` & `FigureGenerator-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,152 +1,132 @@
-Metadata-Version: 2.1
-Name: FigureGenerator
-Version: 0.0.3
-Summary: Making screenshots for presentations and manuscripts.
-Author: Sarthak Pati
-Author-email: software@cbica.upenn.edu
-License: BSD-3-Clause License
-Keywords: medical-imaging,screenshot,figure-generator,publication
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Figure Generator
-
-[![PyPi](https://img.shields.io/pypi/v/FigureGenerator)](https://pypi.org/project/FigureGenerator/)
-[![Conda](https://anaconda.org/conda-forge/figuregenerator/badges/version.svg)](https://anaconda.org/conda-forge/figuregenerator)
-[![Build & Tests](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CBICA/FigureGenerator&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CBICA/FigureGenerator&utm_campaign=Badge_Coverage)
-[![Code style](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
-
-This project helps create high quality figures for medical images for use in presentations and/or manuscripts.
-
-## Installation
-
-```powershell
-git clone https://github.com/CBICA/FigureGenerator.git
-cd screenshot_maker
-conda create -n venv_screenshot python=3.7 -y
-conda activate venv_screenshot
-pip install -e .
-```
-
-OR directly via Pip:
-
-```powershell
-pip install FigureGenerator
-```
-
-## Usage
-
-```
-python ./figure_generator -h
-usage: FigureGenerator [-h] -images IMAGES [-masks MASKS] [-opacity OPACITY]
-                       [-ylabels YLABELS] -output OUTPUT [-axisrow AXISROW]
-                       [-boundtype BOUNDTYPE] [-fontsize FONTSIZE]
-                       [-borderpc BORDERPC] [-v]
-
-Constructing screenshots from medical images.
-
-Contact: software@cbica.upenn.edu
-
-This program is NOT FDA/CE approved and NOT intended for clinical use.
-Copyright (c) 2021 University of Pennsylvania. All rights reserved.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -images IMAGES        Input image files (comma-separated without any spaces in path and co-registered)
-  -masks MASKS          Mask files (comma-separated without any spaces in path and co-registered with images); if multiple files are passed, first is ground truth
-  -opacity OPACITY      Mask opacity between 0-1
-  -ylabels YLABELS      The comma-separated ylabels that will be displayed on the subplots' y-axis
-  -output OUTPUT        Output screenshot file
-  -axisrow AXISROW      Put all axes views across each column and stack images and blends in rows, defaults to False
-  -boundtype BOUNDTYPE  Construct bounding box around specified region; can be 'none, image or mask'
-  -fontsize FONTSIZE    Font size for all text on the figure
-  -borderpc BORDERPC    Percentage of size to use as border around bounding box (used only when mask and bounded are defined)
-  -v, --version         Show program's version number and exit.
-```
-
-## Examples
-
-### **Vertical** screenshot of multiple images **without** bounding:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow False \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-<p align="center">
-  <img width="450" src="images/fig_axisrowfalse.png">
-</p>
-<!-- full-size image
-[<img src="images/fig_axisrowfalse.png" width="450"/>](axisrow_false)
-![axisrow_false](images/fig_axisrowfalse.png)
- -->
-
-### **Horizontal** screenshot of multiple images **without** bounding:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow True \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-[<img src="images/fig_axisrowtrue.png" width="900"/>](axisrow_true)
-<!-- full-size image
-![axisrow_true](images/fig_axisrowtrue.png)
- -->
-
-### Horizontal screenshot of multiple images with **image-based bounding**:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow True \
--boundtype image \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-[<img src="images/fig_axisrowtrue_boundedimage.png" width="900"/>](axistrue_boundedimage)
-<!-- full-size image
-![axisrow_true](images/fig_axisrowtrue_boundedimage.png)
- -->
-
-**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
-
-### Horizontal screenshot of multiple images with **mask-based bounding**:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow True \
--boundtype mask \
--borderpc 0.001 \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-[<img src="images/fig_axisrowtrue_boundedmask.png" width="900"/>](axistrue_boundedmask)
-<!-- full-size image
-![axisrow_true](images/fig_axisrowtrue_boundedmask.png)
- -->
-
-**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
-
-## Feedback
-
-Please post on GitHub [Discussions](https://github.com/CBICA/FigureGenerator/discussions) or post an [issue](https://github.com/CBICA/FigureGenerator/issues/new/choose).
+# Figure Generator
+
+[![PyPi](https://img.shields.io/pypi/v/FigureGenerator)](https://pypi.org/project/FigureGenerator/)
+[![Conda](https://anaconda.org/conda-forge/figuregenerator/badges/version.svg)](https://anaconda.org/conda-forge/figuregenerator)
+[![Build & Tests](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CBICA/FigureGenerator&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CBICA/FigureGenerator&utm_campaign=Badge_Coverage)
+[![Code style](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
+
+This project helps create high quality figures for medical images for use in presentations and/or manuscripts.
+
+## Installation
+
+```powershell
+git clone https://github.com/CBICA/FigureGenerator.git
+cd screenshot_maker
+conda create -n venv_screenshot python=3.7 -y
+conda activate venv_screenshot
+pip install -e .
+```
+
+OR directly via Pip:
+
+```powershell
+pip install FigureGenerator
+```
+
+## Usage
+
+```
+python ./figure_generator -h
+usage: FigureGenerator [-h] -images IMAGES [-masks MASKS] [-opacity OPACITY]
+                       [-ylabels YLABELS] -output OUTPUT [-axisrow AXISROW]
+                       [-boundtype BOUNDTYPE] [-fontsize FONTSIZE]
+                       [-borderpc BORDERPC] [-v]
+
+Constructing screenshots from medical images.
+
+Contact: software@cbica.upenn.edu
+
+This program is NOT FDA/CE approved and NOT intended for clinical use.
+Copyright (c) 2021 University of Pennsylvania. All rights reserved.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -images IMAGES        Input image files (comma-separated without any spaces in path and co-registered)
+  -masks MASKS          Mask files (comma-separated without any spaces in path and co-registered with images); if multiple files are passed, first is ground truth
+  -opacity OPACITY      Mask opacity between 0-1
+  -ylabels YLABELS      The comma-separated ylabels that will be displayed on the subplots' y-axis
+  -output OUTPUT        Output screenshot file
+  -axisrow AXISROW      Put all axes views across each column and stack images and blends in rows, defaults to False
+  -boundtype BOUNDTYPE  Construct bounding box around specified region; can be 'none, image or mask'
+  -fontsize FONTSIZE    Font size for all text on the figure
+  -borderpc BORDERPC    Percentage of size to use as border around bounding box (used only when mask and bounded are defined)
+  -v, --version         Show program's version number and exit.
+```
+
+## Examples
+
+### **Vertical** screenshot of multiple images **without** bounding:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow False \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+<p align="center">
+  <img width="450" src="images/fig_axisrowfalse.png">
+</p>
+<!-- full-size image
+[<img src="images/fig_axisrowfalse.png" width="450"/>](axisrow_false)
+![axisrow_false](images/fig_axisrowfalse.png)
+ -->
+
+### **Horizontal** screenshot of multiple images **without** bounding:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow True \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+[<img src="images/fig_axisrowtrue.png" width="900"/>](axisrow_true)
+<!-- full-size image
+![axisrow_true](images/fig_axisrowtrue.png)
+ -->
+
+### Horizontal screenshot of multiple images with **image-based bounding**:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow True \
+-boundtype image \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+[<img src="images/fig_axisrowtrue_boundedimage.png" width="900"/>](axistrue_boundedimage)
+<!-- full-size image
+![axisrow_true](images/fig_axisrowtrue_boundedimage.png)
+ -->
+
+**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
+
+### Horizontal screenshot of multiple images with **mask-based bounding**:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow True \
+-boundtype mask \
+-borderpc 0.001 \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+[<img src="images/fig_axisrowtrue_boundedmask.png" width="900"/>](axistrue_boundedmask)
+<!-- full-size image
+![axisrow_true](images/fig_axisrowtrue_boundedmask.png)
+ -->
+
+**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
+
+## Feedback
+
+Please post on GitHub [Discussions](https://github.com/CBICA/FigureGenerator/discussions) or post an [issue](https://github.com/CBICA/FigureGenerator/issues/new/choose).
```

### Comparing `FigureGenerator-0.0.3/PKG-INFO` & `FigureGenerator-0.0.4/FigureGenerator.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-Metadata-Version: 2.1
-Name: FigureGenerator
-Version: 0.0.3
-Summary: Making screenshots for presentations and manuscripts.
-Author: Sarthak Pati
-Author-email: software@cbica.upenn.edu
-License: BSD-3-Clause License
-Keywords: medical-imaging,screenshot,figure-generator,publication
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Figure Generator
-
-[![PyPi](https://img.shields.io/pypi/v/FigureGenerator)](https://pypi.org/project/FigureGenerator/)
-[![Conda](https://anaconda.org/conda-forge/figuregenerator/badges/version.svg)](https://anaconda.org/conda-forge/figuregenerator)
-[![Build & Tests](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CBICA/FigureGenerator&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CBICA/FigureGenerator&utm_campaign=Badge_Coverage)
-[![Code style](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
-
-This project helps create high quality figures for medical images for use in presentations and/or manuscripts.
-
-## Installation
-
-```powershell
-git clone https://github.com/CBICA/FigureGenerator.git
-cd screenshot_maker
-conda create -n venv_screenshot python=3.7 -y
-conda activate venv_screenshot
-pip install -e .
-```
-
-OR directly via Pip:
-
-```powershell
-pip install FigureGenerator
-```
-
-## Usage
-
-```
-python ./figure_generator -h
-usage: FigureGenerator [-h] -images IMAGES [-masks MASKS] [-opacity OPACITY]
-                       [-ylabels YLABELS] -output OUTPUT [-axisrow AXISROW]
-                       [-boundtype BOUNDTYPE] [-fontsize FONTSIZE]
-                       [-borderpc BORDERPC] [-v]
-
-Constructing screenshots from medical images.
-
-Contact: software@cbica.upenn.edu
-
-This program is NOT FDA/CE approved and NOT intended for clinical use.
-Copyright (c) 2021 University of Pennsylvania. All rights reserved.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -images IMAGES        Input image files (comma-separated without any spaces in path and co-registered)
-  -masks MASKS          Mask files (comma-separated without any spaces in path and co-registered with images); if multiple files are passed, first is ground truth
-  -opacity OPACITY      Mask opacity between 0-1
-  -ylabels YLABELS      The comma-separated ylabels that will be displayed on the subplots' y-axis
-  -output OUTPUT        Output screenshot file
-  -axisrow AXISROW      Put all axes views across each column and stack images and blends in rows, defaults to False
-  -boundtype BOUNDTYPE  Construct bounding box around specified region; can be 'none, image or mask'
-  -fontsize FONTSIZE    Font size for all text on the figure
-  -borderpc BORDERPC    Percentage of size to use as border around bounding box (used only when mask and bounded are defined)
-  -v, --version         Show program's version number and exit.
-```
-
-## Examples
-
-### **Vertical** screenshot of multiple images **without** bounding:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow False \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-<p align="center">
-  <img width="450" src="images/fig_axisrowfalse.png">
-</p>
-<!-- full-size image
-[<img src="images/fig_axisrowfalse.png" width="450"/>](axisrow_false)
-![axisrow_false](images/fig_axisrowfalse.png)
- -->
-
-### **Horizontal** screenshot of multiple images **without** bounding:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow True \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-[<img src="images/fig_axisrowtrue.png" width="900"/>](axisrow_true)
-<!-- full-size image
-![axisrow_true](images/fig_axisrowtrue.png)
- -->
-
-### Horizontal screenshot of multiple images with **image-based bounding**:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow True \
--boundtype image \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-[<img src="images/fig_axisrowtrue_boundedimage.png" width="900"/>](axistrue_boundedimage)
-<!-- full-size image
-![axisrow_true](images/fig_axisrowtrue_boundedimage.png)
- -->
-
-**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
-
-### Horizontal screenshot of multiple images with **mask-based bounding**:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow True \
--boundtype mask \
--borderpc 0.001 \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-[<img src="images/fig_axisrowtrue_boundedmask.png" width="900"/>](axistrue_boundedmask)
-<!-- full-size image
-![axisrow_true](images/fig_axisrowtrue_boundedmask.png)
- -->
-
-**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
-
-## Feedback
-
-Please post on GitHub [Discussions](https://github.com/CBICA/FigureGenerator/discussions) or post an [issue](https://github.com/CBICA/FigureGenerator/issues/new/choose).
+Metadata-Version: 2.1
+Name: FigureGenerator
+Version: 0.0.4
+Summary: Making screenshots for presentations and manuscripts.
+Author: Sarthak Pati
+Author-email: software@cbica.upenn.edu
+License: BSD-3-Clause License
+Keywords: medical-imaging,screenshot,figure-generator,publication
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Figure Generator
+
+[![PyPi](https://img.shields.io/pypi/v/FigureGenerator)](https://pypi.org/project/FigureGenerator/)
+[![Conda](https://anaconda.org/conda-forge/figuregenerator/badges/version.svg)](https://anaconda.org/conda-forge/figuregenerator)
+[![Build & Tests](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CBICA/FigureGenerator&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CBICA/FigureGenerator&utm_campaign=Badge_Coverage)
+[![Code style](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
+
+This project helps create high quality figures for medical images for use in presentations and/or manuscripts.
+
+## Installation
+
+```powershell
+git clone https://github.com/CBICA/FigureGenerator.git
+cd screenshot_maker
+conda create -n venv_screenshot python=3.7 -y
+conda activate venv_screenshot
+pip install -e .
+```
+
+OR directly via Pip:
+
+```powershell
+pip install FigureGenerator
+```
+
+## Usage
+
+```
+python ./figure_generator -h
+usage: FigureGenerator [-h] -images IMAGES [-masks MASKS] [-opacity OPACITY]
+                       [-ylabels YLABELS] -output OUTPUT [-axisrow AXISROW]
+                       [-boundtype BOUNDTYPE] [-fontsize FONTSIZE]
+                       [-borderpc BORDERPC] [-v]
+
+Constructing screenshots from medical images.
+
+Contact: software@cbica.upenn.edu
+
+This program is NOT FDA/CE approved and NOT intended for clinical use.
+Copyright (c) 2021 University of Pennsylvania. All rights reserved.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -images IMAGES        Input image files (comma-separated without any spaces in path and co-registered)
+  -masks MASKS          Mask files (comma-separated without any spaces in path and co-registered with images); if multiple files are passed, first is ground truth
+  -opacity OPACITY      Mask opacity between 0-1
+  -ylabels YLABELS      The comma-separated ylabels that will be displayed on the subplots' y-axis
+  -output OUTPUT        Output screenshot file
+  -axisrow AXISROW      Put all axes views across each column and stack images and blends in rows, defaults to False
+  -boundtype BOUNDTYPE  Construct bounding box around specified region; can be 'none, image or mask'
+  -fontsize FONTSIZE    Font size for all text on the figure
+  -borderpc BORDERPC    Percentage of size to use as border around bounding box (used only when mask and bounded are defined)
+  -v, --version         Show program's version number and exit.
+```
+
+## Examples
+
+### **Vertical** screenshot of multiple images **without** bounding:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow False \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+<p align="center">
+  <img width="450" src="images/fig_axisrowfalse.png">
+</p>
+<!-- full-size image
+[<img src="images/fig_axisrowfalse.png" width="450"/>](axisrow_false)
+![axisrow_false](images/fig_axisrowfalse.png)
+ -->
+
+### **Horizontal** screenshot of multiple images **without** bounding:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow True \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+[<img src="images/fig_axisrowtrue.png" width="900"/>](axisrow_true)
+<!-- full-size image
+![axisrow_true](images/fig_axisrowtrue.png)
+ -->
+
+### Horizontal screenshot of multiple images with **image-based bounding**:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow True \
+-boundtype image \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+[<img src="images/fig_axisrowtrue_boundedimage.png" width="900"/>](axistrue_boundedimage)
+<!-- full-size image
+![axisrow_true](images/fig_axisrowtrue_boundedimage.png)
+ -->
+
+**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
+
+### Horizontal screenshot of multiple images with **mask-based bounding**:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow True \
+-boundtype mask \
+-borderpc 0.001 \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+[<img src="images/fig_axisrowtrue_boundedmask.png" width="900"/>](axistrue_boundedmask)
+<!-- full-size image
+![axisrow_true](images/fig_axisrowtrue_boundedmask.png)
+ -->
+
+**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
+
+## Feedback
+
+Please post on GitHub [Discussions](https://github.com/CBICA/FigureGenerator/discussions) or post an [issue](https://github.com/CBICA/FigureGenerator/issues/new/choose).
```

### Comparing `FigureGenerator-0.0.3/README.md` & `FigureGenerator-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,132 +1,152 @@
-# Figure Generator
-
-[![PyPi](https://img.shields.io/pypi/v/FigureGenerator)](https://pypi.org/project/FigureGenerator/)
-[![Conda](https://anaconda.org/conda-forge/figuregenerator/badges/version.svg)](https://anaconda.org/conda-forge/figuregenerator)
-[![Build & Tests](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CBICA/FigureGenerator&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CBICA/FigureGenerator&utm_campaign=Badge_Coverage)
-[![Code style](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
-
-This project helps create high quality figures for medical images for use in presentations and/or manuscripts.
-
-## Installation
-
-```powershell
-git clone https://github.com/CBICA/FigureGenerator.git
-cd screenshot_maker
-conda create -n venv_screenshot python=3.7 -y
-conda activate venv_screenshot
-pip install -e .
-```
-
-OR directly via Pip:
-
-```powershell
-pip install FigureGenerator
-```
-
-## Usage
-
-```
-python ./figure_generator -h
-usage: FigureGenerator [-h] -images IMAGES [-masks MASKS] [-opacity OPACITY]
-                       [-ylabels YLABELS] -output OUTPUT [-axisrow AXISROW]
-                       [-boundtype BOUNDTYPE] [-fontsize FONTSIZE]
-                       [-borderpc BORDERPC] [-v]
-
-Constructing screenshots from medical images.
-
-Contact: software@cbica.upenn.edu
-
-This program is NOT FDA/CE approved and NOT intended for clinical use.
-Copyright (c) 2021 University of Pennsylvania. All rights reserved.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -images IMAGES        Input image files (comma-separated without any spaces in path and co-registered)
-  -masks MASKS          Mask files (comma-separated without any spaces in path and co-registered with images); if multiple files are passed, first is ground truth
-  -opacity OPACITY      Mask opacity between 0-1
-  -ylabels YLABELS      The comma-separated ylabels that will be displayed on the subplots' y-axis
-  -output OUTPUT        Output screenshot file
-  -axisrow AXISROW      Put all axes views across each column and stack images and blends in rows, defaults to False
-  -boundtype BOUNDTYPE  Construct bounding box around specified region; can be 'none, image or mask'
-  -fontsize FONTSIZE    Font size for all text on the figure
-  -borderpc BORDERPC    Percentage of size to use as border around bounding box (used only when mask and bounded are defined)
-  -v, --version         Show program's version number and exit.
-```
-
-## Examples
-
-### **Vertical** screenshot of multiple images **without** bounding:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow False \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-<p align="center">
-  <img width="450" src="images/fig_axisrowfalse.png">
-</p>
-<!-- full-size image
-[<img src="images/fig_axisrowfalse.png" width="450"/>](axisrow_false)
-![axisrow_false](images/fig_axisrowfalse.png)
- -->
-
-### **Horizontal** screenshot of multiple images **without** bounding:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow True \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-[<img src="images/fig_axisrowtrue.png" width="900"/>](axisrow_true)
-<!-- full-size image
-![axisrow_true](images/fig_axisrowtrue.png)
- -->
-
-### Horizontal screenshot of multiple images with **image-based bounding**:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow True \
--boundtype image \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-[<img src="images/fig_axisrowtrue_boundedimage.png" width="900"/>](axistrue_boundedimage)
-<!-- full-size image
-![axisrow_true](images/fig_axisrowtrue_boundedimage.png)
- -->
-
-**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
-
-### Horizontal screenshot of multiple images with **mask-based bounding**:
-```powershell
-python ./figure_generator \
--images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
--masks C:/input/subject_001_seg.nii.gz \
--axisrow True \
--boundtype mask \
--borderpc 0.001 \
--output C:/input/fig.png 
-```
-Gives the following output:
-
-[<img src="images/fig_axisrowtrue_boundedmask.png" width="900"/>](axistrue_boundedmask)
-<!-- full-size image
-![axisrow_true](images/fig_axisrowtrue_boundedmask.png)
- -->
-
-**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
-
-## Feedback
-
-Please post on GitHub [Discussions](https://github.com/CBICA/FigureGenerator/discussions) or post an [issue](https://github.com/CBICA/FigureGenerator/issues/new/choose).
+Metadata-Version: 2.1
+Name: FigureGenerator
+Version: 0.0.4
+Summary: Making screenshots for presentations and manuscripts.
+Author: Sarthak Pati
+Author-email: software@cbica.upenn.edu
+License: BSD-3-Clause License
+Keywords: medical-imaging,screenshot,figure-generator,publication
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Figure Generator
+
+[![PyPi](https://img.shields.io/pypi/v/FigureGenerator)](https://pypi.org/project/FigureGenerator/)
+[![Conda](https://anaconda.org/conda-forge/figuregenerator/badges/version.svg)](https://anaconda.org/conda-forge/figuregenerator)
+[![Build & Tests](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CBICA/FigureGenerator&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CBICA/FigureGenerator&utm_campaign=Badge_Coverage)
+[![Code style](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
+
+This project helps create high quality figures for medical images for use in presentations and/or manuscripts.
+
+## Installation
+
+```powershell
+git clone https://github.com/CBICA/FigureGenerator.git
+cd screenshot_maker
+conda create -n venv_screenshot python=3.7 -y
+conda activate venv_screenshot
+pip install -e .
+```
+
+OR directly via Pip:
+
+```powershell
+pip install FigureGenerator
+```
+
+## Usage
+
+```
+python ./figure_generator -h
+usage: FigureGenerator [-h] -images IMAGES [-masks MASKS] [-opacity OPACITY]
+                       [-ylabels YLABELS] -output OUTPUT [-axisrow AXISROW]
+                       [-boundtype BOUNDTYPE] [-fontsize FONTSIZE]
+                       [-borderpc BORDERPC] [-v]
+
+Constructing screenshots from medical images.
+
+Contact: software@cbica.upenn.edu
+
+This program is NOT FDA/CE approved and NOT intended for clinical use.
+Copyright (c) 2021 University of Pennsylvania. All rights reserved.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -images IMAGES        Input image files (comma-separated without any spaces in path and co-registered)
+  -masks MASKS          Mask files (comma-separated without any spaces in path and co-registered with images); if multiple files are passed, first is ground truth
+  -opacity OPACITY      Mask opacity between 0-1
+  -ylabels YLABELS      The comma-separated ylabels that will be displayed on the subplots' y-axis
+  -output OUTPUT        Output screenshot file
+  -axisrow AXISROW      Put all axes views across each column and stack images and blends in rows, defaults to False
+  -boundtype BOUNDTYPE  Construct bounding box around specified region; can be 'none, image or mask'
+  -fontsize FONTSIZE    Font size for all text on the figure
+  -borderpc BORDERPC    Percentage of size to use as border around bounding box (used only when mask and bounded are defined)
+  -v, --version         Show program's version number and exit.
+```
+
+## Examples
+
+### **Vertical** screenshot of multiple images **without** bounding:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow False \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+<p align="center">
+  <img width="450" src="images/fig_axisrowfalse.png">
+</p>
+<!-- full-size image
+[<img src="images/fig_axisrowfalse.png" width="450"/>](axisrow_false)
+![axisrow_false](images/fig_axisrowfalse.png)
+ -->
+
+### **Horizontal** screenshot of multiple images **without** bounding:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow True \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+[<img src="images/fig_axisrowtrue.png" width="900"/>](axisrow_true)
+<!-- full-size image
+![axisrow_true](images/fig_axisrowtrue.png)
+ -->
+
+### Horizontal screenshot of multiple images with **image-based bounding**:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow True \
+-boundtype image \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+[<img src="images/fig_axisrowtrue_boundedimage.png" width="900"/>](axistrue_boundedimage)
+<!-- full-size image
+![axisrow_true](images/fig_axisrowtrue_boundedimage.png)
+ -->
+
+**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
+
+### Horizontal screenshot of multiple images with **mask-based bounding**:
+```powershell
+python ./figure_generator \
+-images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
+-masks C:/input/subject_001_seg.nii.gz \
+-axisrow True \
+-boundtype mask \
+-borderpc 0.001 \
+-output C:/input/fig.png 
+```
+Gives the following output:
+
+[<img src="images/fig_axisrowtrue_boundedmask.png" width="900"/>](axistrue_boundedmask)
+<!-- full-size image
+![axisrow_true](images/fig_axisrowtrue_boundedmask.png)
+ -->
+
+**Note**: This can be used with vertical orientation as well, by passing `-axisrow False` to the command.
+
+## Feedback
+
+Please post on GitHub [Discussions](https://github.com/CBICA/FigureGenerator/discussions) or post an [issue](https://github.com/CBICA/FigureGenerator/issues/new/choose).
```

### Comparing `FigureGenerator-0.0.3/SECURITY.md` & `FigureGenerator-0.0.4/SECURITY.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Security Policy
-
-## Supported Versions
-
-Use this section to tell people about which versions of your project are
-currently being supported with security updates.
-
-| Version | Supported          |
-| ------- | ------------------ |
-| 0.0.x   | :white_check_mark: |
-
-## Reporting a Vulnerability
-
-Use this section to tell people how to report a vulnerability.
-
-Tell them where to go, how often they can expect to get an update on a
-reported vulnerability, what to expect if the vulnerability is accepted or
-declined, etc.
+# Security Policy
+
+## Supported Versions
+
+Use this section to tell people about which versions of your project are
+currently being supported with security updates.
+
+| Version | Supported          |
+| ------- | ------------------ |
+| 0.0.x   | :white_check_mark: |
+
+## Reporting a Vulnerability
+
+Use this section to tell people how to report a vulnerability.
+
+Tell them where to go, how often they can expect to get an update on a
+reported vulnerability, what to expect if the vulnerability is accepted or
+declined, etc.
```

### Comparing `FigureGenerator-0.0.3/setup.py` & `FigureGenerator-0.0.4/setup.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-from setuptools import setup, find_packages
-
-with open("README.md") as readme_file:
-    readme = readme_file.read()
-
-# read version.py
-import sys, re
-
-try:
-    filepath = "FigureGenerator/version.py"
-    version_file = open(filepath)
-    (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
-
-except Exception as error:
-    __version__ = "0.0.1"
-    sys.stderr.write("Warning: Could not open '%s' due %s\n" % (filepath, error))
-
-requirements = [
-    "numpy>=1.19.2",
-    "SimpleITK!=2.0.*",
-    "SimpleITK!=2.2.1",  # https://github.com/mlcommons/GaNDLF/issues/536
-    "pytest",
-    "coverage",
-    "psutil",
-    "black",
-    "matplotlib",
-    "requests",
-]
-
-setup(
-    name="FigureGenerator",
-    version=__version__,
-    author="Sarthak Pati",  # alphabetical order
-    author_email="software@cbica.upenn.edu",
-    python_requires=">=3.6",
-    packages=find_packages(),
-    scripts=["figure_generator"],
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: BSD License",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-    ],
-    description=("Making screenshots for presentations and manuscripts."),
-    install_requires=requirements,
-    license="BSD-3-Clause License",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    include_package_data=True,
-    keywords="medical-imaging, screenshot, figure-generator, publication",
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+from setuptools import setup, find_packages
+
+with open("README.md") as readme_file:
+    readme = readme_file.read()
+
+# read version.py
+import sys, re
+
+try:
+    filepath = "FigureGenerator/version.py"
+    version_file = open(filepath)
+    (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
+
+except Exception as error:
+    __version__ = "0.0.1"
+    sys.stderr.write("Warning: Could not open '%s' due %s\n" % (filepath, error))
+
+requirements = [
+    "numpy>=1.19.2",
+    "SimpleITK!=2.0.*",
+    "SimpleITK!=2.2.1",  # https://github.com/mlcommons/GaNDLF/issues/536
+    "pytest",
+    "coverage",
+    "psutil",
+    "black",
+    "matplotlib",
+    "requests",
+]
+
+setup(
+    name="FigureGenerator",
+    version=__version__,
+    author="Sarthak Pati",  # alphabetical order
+    author_email="software@cbica.upenn.edu",
+    python_requires=">=3.6",
+    packages=find_packages(),
+    scripts=["figure_generator"],
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: BSD License",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+    ],
+    description=("Making screenshots for presentations and manuscripts."),
+    install_requires=requirements,
+    license="BSD-3-Clause License",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    include_package_data=True,
+    keywords="medical-imaging, screenshot, figure-generator, publication",
+    zip_safe=False,
+)
```

