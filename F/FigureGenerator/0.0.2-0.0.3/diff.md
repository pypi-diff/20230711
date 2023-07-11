# Comparing `tmp/FigureGenerator-0.0.2.tar.gz` & `tmp/FigureGenerator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FigureGenerator-0.0.2.tar", last modified: Mon Aug  9 22:26:50 2021, max compression
+gzip compressed data, was "FigureGenerator-0.0.3.tar", last modified: Tue Jul 11 02:18:40 2023, max compression
```

## Comparing `FigureGenerator-0.0.2.tar` & `FigureGenerator-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/
--rw-rw-rw-   0        0        0     3432 2021-03-02 12:23:59.000000 FigureGenerator-0.0.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1495 2021-07-30 16:29:31.000000 FigureGenerator-0.0.2/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/FigureGenerator/
--rw-rw-rw-   0        0        0      117 2021-07-30 12:52:33.000000 FigureGenerator-0.0.2/FigureGenerator/__init__.py
--rw-rw-rw-   0        0        0    14113 2021-08-06 23:27:57.000000 FigureGenerator-0.0.2/FigureGenerator/screenshot_maker.py
--rw-rw-rw-   0        0        0    10350 2021-08-06 23:27:57.000000 FigureGenerator-0.0.2/FigureGenerator/utils.py
--rw-rw-rw-   0        0        0       72 2021-08-09 22:26:20.000000 FigureGenerator-0.0.2/FigureGenerator/version.py
-drwxrwxrwx   0        0        0        0 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/FigureGenerator.egg-info/
--rw-rw-rw-   0        0        0     7501 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/FigureGenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/FigureGenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/FigureGenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-07-30 12:58:04.000000 FigureGenerator-0.0.2/FigureGenerator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       80 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/FigureGenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/FigureGenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      282 2021-07-30 12:52:33.000000 FigureGenerator-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       29 2021-07-30 12:52:33.000000 FigureGenerator-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7501 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5655 2021-08-06 23:27:57.000000 FigureGenerator-0.0.2/README.md
--rw-rw-rw-   0        0        0      538 2021-08-03 03:22:32.000000 FigureGenerator-0.0.2/SECURITY.md
--rw-rw-rw-   0        0        0     3833 2021-08-09 22:26:45.000000 FigureGenerator-0.0.2/figure_generator
--rw-rw-rw-   0        0        0       42 2021-08-09 22:26:50.000000 FigureGenerator-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1714 2021-08-03 14:30:52.000000 FigureGenerator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:18:40.287713 FigureGenerator-0.0.3/
+-rw-rw-rw-   0        0        0     3432 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     1504 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2023-07-11 02:18:40.257713 FigureGenerator-0.0.3/FigureGenerator/
+-rw-rw-rw-   0        0        0      117 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/FigureGenerator/__init__.py
+-rw-rw-rw-   0        0        0    15592 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/FigureGenerator/screenshot_maker.py
+-rw-rw-rw-   0        0        0    10350 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/FigureGenerator/utils.py
+-rw-rw-rw-   0        0        0       72 2023-07-11 02:06:55.000000 FigureGenerator-0.0.3/FigureGenerator/version.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:18:40.283715 FigureGenerator-0.0.3/FigureGenerator.egg-info/
+-rw-rw-rw-   0        0        0     6557 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 02:17:53.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       97 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-11 02:18:40.000000 FigureGenerator-0.0.3/FigureGenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      282 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       29 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6557 2023-07-11 02:18:40.286713 FigureGenerator-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5788 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/README.md
+-rw-rw-rw-   0        0        0      538 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/SECURITY.md
+-rw-rw-rw-   0        0        0     3804 2023-07-11 02:06:42.000000 FigureGenerator-0.0.3/figure_generator
+-rw-rw-rw-   0        0        0       42 2023-07-11 02:18:40.287713 FigureGenerator-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1789 2023-07-11 02:07:37.000000 FigureGenerator-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `FigureGenerator-0.0.2/CODE_OF_CONDUCT.md` & `FigureGenerator-0.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `FigureGenerator-0.0.2/CONTRIBUTING.md` & `FigureGenerator-0.0.3/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Contribution Guidelines
 
-GaNDLF is a package that is primarily worked on by the CBICA Software Development team and its collaborators - additional members from the community are welcome!
+FigureGenerator is a package that is primarily worked on by the CBICA Software Development team and its collaborators - additional members from the community are welcome!
 
 ## Issues
 
 The easiest way to contribute is by reporting issues is through the [GitHub](https://github.com/CBICA/FigureGenerator/issues). 
 When reporting an issue, please ensure you fill out as much information from the templates as possible for us to debug and diagnose it.
 
 ## Feature Requests
```

### Comparing `FigureGenerator-0.0.2/FigureGenerator/screenshot_maker.py` & `FigureGenerator-0.0.3/FigureGenerator/screenshot_maker.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         # if args.slice is not None:
         #     self.slice_numbers = args.slice.split(",")
         # else:
         #     self.slice_numbers = None
         self.mask_opacity = args.opacity
         self.border_pc = args.borderpc
         self.axisrow = args.axisrow
+        self.font_size = args.fontsize
 
         ## this is used for y-axis in subplots
         self.ylabel_titles = args.ylabels
         # if ylabels have been defined, then use that but perform sanity checks
         if self.ylabel_titles is not None:
             self.ylabel_titles = self.ylabel_titles.split(",")
             # the length of the ylabels needs to be appropriate based on the axisrow
@@ -74,29 +75,55 @@
                         for j in range(len(self.masks)):
                             self.ylabel_titles.append(
                                 get_basename_sanitized(self.images[i])
                                 + " + "
                                 + get_basename_sanitized(self.masks[j])
                             )
 
-        self.calculate_bounds = args.boundimg
+        # deduce bounding type
+        self.calculate_bounds = args.boundtype.lower()
+        if self.calculate_bounds in ["image", "img"]:
+            self.calculate_bounds = True
+            self.calculate_bounds_mask = False
+        elif self.calculate_bounds in ["mask", "msk"]:
+            self.calculate_bounds_mask = True
+            self.calculate_bounds = False
+            if not (self.mask_present):
+                raise ValueError(
+                    "If mask is not provided, then boundtype must be 'image'"
+                )
+        else:
+            self.calculate_bounds = False
+            self.calculate_bounds_mask = False
+
+        # do not let border get below 0.001% of the image if bounding type is image
         if self.calculate_bounds:
-            self.border_pc = 0.001
-        self.calculate_bounds_mask = args.boundmask
+            self.border_pc = min(0.001, self.border_pc)
         if self.calculate_bounds and self.calculate_bounds_mask:
             print(
                 "WARNING: Both image and mask bounding cannot be enabled, using only image bounding."
             )
             self.calculate_bounds_mask = False
+
+        # if a file is not present in output, use a default value
         self.output = args.output
         _, ext = os.path.splitext(self.output)
         if ext == "" or ext is None:
             pathlib.Path(self.output).mkdir(parents=True, exist_ok=True)
             self.output = os.path.join(self.output, "screenshot.png")
+            # if screenshot exists before, then do not overwrite
+            if os.path.exists(self.output):
+                print(
+                    "Default output file was existing before, using process ID to ensure overwriting does not occur"
+                )
+                self.output = os.path.join(
+                    self.output, "screenshot_" + os.getpid() + ".png"
+                )
 
+        # adjust the layout for plotting
         if self.axisrow:
             self.layout = (3 * len(self.images), 1 + len(self.masks), 0)
         else:
             self.layout = (3, len(self.images) + len(self.images) * len(self.masks), 0)
 
         ## sanity checker
         # read the first image and save that for comparison
@@ -131,19 +158,19 @@
                 )
                 for mask in self.masks
             ]
 
         ## 3d-specific calculations start here.
         if self.calculate_bounds:
             bounding_box = get_bounding_box(
-                input_images[0], [input_images[0]], self.border_pc
+                input_images[0], input_images[0], self.border_pc
             )
         elif self.calculate_bounds_mask:
             bounding_box = get_bounding_box(
-                input_images[0], input_masks, self.border_pc
+                input_images[0], input_masks[0], self.border_pc
             )
         else:
             bounding_box = get_bounding_box(input_images[0], None, None)
 
         extract = sitk.ExtractImageFilter()
         extract.SetSize(
             [
@@ -319,14 +346,15 @@
                 "grid.color": "lightgray",
                 "figure.facecolor": "black",
                 "figure.edgecolor": "black",
                 "savefig.facecolor": "black",
                 "savefig.edgecolor": "black",
             }
         )
+        plt.rc("font", size=self.font_size)
 
         # we only want the titles for first row
         counter = 0
         ylabel_counter = 0
         for ax, img in zip(self.fig.axes, images_blended):
             ax.imshow(sitk.GetArrayFromImage(img))
             # ax.axis("off")
@@ -339,15 +367,23 @@
                 elif counter % 3 == 2:
                     ax.set_title("Coronal")
                 elif counter % 3 == 0:
                     ax.set_title("Axial")
                 ax.title.set_color("white")
 
             if counter == 1:
-                ax.set_ylabel(self.ylabel_titles[ylabel_counter], color="white")
+                ax.set_ylabel(
+                    self.ylabel_titles[ylabel_counter],
+                    color="white",
+                    size=self.font_size,
+                )
                 ylabel_counter += 1
             elif (counter - 1) % self.layout[0] == 0:
-                ax.set_ylabel(self.ylabel_titles[ylabel_counter], color="white")
+                ax.set_ylabel(
+                    self.ylabel_titles[ylabel_counter],
+                    color="white",
+                    size=self.font_size,
+                )
                 ylabel_counter += 1
 
         plt.tight_layout()
         plt.savefig(os.path.join(output_file))
```

### Comparing `FigureGenerator-0.0.2/FigureGenerator/utils.py` & `FigureGenerator-0.0.3/FigureGenerator/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,30 +208,30 @@
     thresholder.SetOutsideValue(0)
     thresholder.SetInsideValue(1)
     thresholder.SetLowerThreshold(1)
     thresholder.SetUpperThreshold(max_filter.GetMaximum())
     return thresholder.Execute(image)
 
 
-def get_bounding_box(image, mask_list, border_pc):
+def get_bounding_box(image, mask, border_pc):
     """
     Get the bounding box of the image based on the first mask after it is binarized.
 
     Args:
         image (SimpleITK.Image): The input image.
-        mask_list (list of SimpleITK.Image): The list of masks.
+        mask (SimpleITK.Image): The ground truth mask.
         border_pc (float): The percentage of the image size to consider as the border.
 
     Returns:
         list: The bounding box in the form of [x_min, x_max, y_min, y_max, z_min, z_max]
     """
     size = image.GetSize()
-    if mask_list is not None:
+    if mask is not None:
         extractor = sitk.LabelStatisticsImageFilter()
-        extractor.Execute(image, binarize_image(mask_list[0]))
+        extractor.Execute(image, binarize_image(mask))
         bb = list(extractor.GetBoundingBox(1))
         bb[0] = max(0, math.floor(bb[0] - border_pc * size[0]))
         bb[2] = max(0, math.floor(bb[2] - border_pc * size[1]))
         bb[4] = max(0, math.floor(bb[4] - border_pc * size[2]))
 
         full_min = min(bb[0], bb[2], bb[4])
         bb[0], bb[2], bb[4] = full_min, full_min, full_min
@@ -278,8 +278,8 @@
     #                                  opacity=alpha, backgroundValue = 0,
     #                                  colormap=r+g+b)
 
     filter_overlay = sitk.LabelOverlayImageFilter()
     filter_overlay.SetOpacity(alpha)
     # filter_overlay.SetBackgroundValue(0)
     # filter_overlay.SetColormap(r+g+b)
-    return filter_overlay.Execute(sitk.Cast(image, sitk.sitkUInt8), mask)
+    return filter_overlay.Execute(sitk.Cast(image, sitk.sitkUInt8), sitk.Cast(mask, sitk.sitkUInt8))
```

### Comparing `FigureGenerator-0.0.2/README.md` & `FigureGenerator-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Figure Generator
 
 [![PyPi](https://img.shields.io/pypi/v/FigureGenerator)](https://pypi.org/project/FigureGenerator/)
+[![Conda](https://anaconda.org/conda-forge/figuregenerator/badges/version.svg)](https://anaconda.org/conda-forge/figuregenerator)
 [![Build & Tests](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/CBICA/FigureGenerator/actions/workflows/python-package.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CBICA/FigureGenerator&amp;utm_campaign=Badge_Grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/608de602c1bd4bec810efb0d08f269e6)](https://www.codacy.com/gh/CBICA/FigureGenerator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CBICA/FigureGenerator&utm_campaign=Badge_Coverage)
 [![Code style](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
 
 This project helps create high quality figures for medical images for use in presentations and/or manuscripts.
 
@@ -26,15 +27,15 @@
 
 ## Usage
 
 ```
 python ./figure_generator -h
 usage: FigureGenerator [-h] -images IMAGES [-masks MASKS] [-opacity OPACITY]
                        [-ylabels YLABELS] -output OUTPUT [-axisrow AXISROW]
-                       [-boundimg BOUNDIMG] [-boundmask BOUNDMASK]
+                       [-boundtype BOUNDTYPE] [-fontsize FONTSIZE]
                        [-borderpc BORDERPC] [-v]
 
 Constructing screenshots from medical images.
 
 Contact: software@cbica.upenn.edu
 
 This program is NOT FDA/CE approved and NOT intended for clinical use.
@@ -44,16 +45,16 @@
   -h, --help            show this help message and exit
   -images IMAGES        Input image files (comma-separated without any spaces in path and co-registered)
   -masks MASKS          Mask files (comma-separated without any spaces in path and co-registered with images); if multiple files are passed, first is ground truth
   -opacity OPACITY      Mask opacity between 0-1
   -ylabels YLABELS      The comma-separated ylabels that will be displayed on the subplots' y-axis
   -output OUTPUT        Output screenshot file
   -axisrow AXISROW      Put all axes views across each column and stack images and blends in rows, defaults to False
-  -boundimg BOUNDIMG    Construct bounding box around non-zero pixels of input images
-  -boundmask BOUNDMASK  Construct bounding box around binarized ground truth
+  -boundtype BOUNDTYPE  Construct bounding box around specified region; can be 'none, image or mask'
+  -fontsize FONTSIZE    Font size for all text on the figure
   -borderpc BORDERPC    Percentage of size to use as border around bounding box (used only when mask and bounded are defined)
   -v, --version         Show program's version number and exit.
 ```
 
 ## Examples
 
 ### **Vertical** screenshot of multiple images **without** bounding:
@@ -91,15 +92,15 @@
 
 ### Horizontal screenshot of multiple images with **image-based bounding**:
 ```powershell
 python ./figure_generator \
 -images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
 -masks C:/input/subject_001_seg.nii.gz \
 -axisrow True \
--bounded True \
+-boundtype image \
 -output C:/input/fig.png 
 ```
 Gives the following output:
 
 [<img src="images/fig_axisrowtrue_boundedimage.png" width="900"/>](axistrue_boundedimage)
 <!-- full-size image
 ![axisrow_true](images/fig_axisrowtrue_boundedimage.png)
@@ -109,15 +110,15 @@
 
 ### Horizontal screenshot of multiple images with **mask-based bounding**:
 ```powershell
 python ./figure_generator \
 -images C:/input/subject_001_flair.nii.gz,C:/input/subject_001_t1ce.nii.gz,C:/input/subject_001_t1.nii.gz,C:/input/subject_001_t2.nii.gz \
 -masks C:/input/subject_001_seg.nii.gz \
 -axisrow True \
--boundmask True \
+-boundtype mask \
 -borderpc 0.001 \
 -output C:/input/fig.png 
 ```
 Gives the following output:
 
 [<img src="images/fig_axisrowtrue_boundedmask.png" width="900"/>](axistrue_boundedmask)
 <!-- full-size image
```

### Comparing `FigureGenerator-0.0.2/SECURITY.md` & `FigureGenerator-0.0.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `FigureGenerator-0.0.2/figure_generator` & `FigureGenerator-0.0.3/figure_generator`

 * *Files 14% similar despite different names*

```diff
@@ -72,25 +72,25 @@
         "-axisrow",
         type=ast.literal_eval,
         default=False,
         help="Put all axes views across each column and stack images and blends in rows, defaults to False",
         required=False,
     )
     parser.add_argument(
-        "-boundimg",
-        type=ast.literal_eval,
-        default=False,
-        help="Construct bounding box around non-zero pixels of input images",
+        "-boundtype",
+        type=str,
+        default="None",
+        help="Construct bounding box around specified region; can be 'none, image or mask'",
         required=False,
     )
     parser.add_argument(
-        "-boundmask",
-        type=ast.literal_eval,
-        default=False,
-        help="Construct bounding box around binarized ground truth",
+        "-fontsize",
+        type=int,
+        default=15,
+        help="Font size for all text on the figure",
         required=False,
     )
     parser.add_argument(
         "-borderpc",
         type=float,
         default=0.05,
         help="Percentage of size to use as border around bounding box (used only when mask and bounded are defined)",
```

### Comparing `FigureGenerator-0.0.2/setup.py` & `FigureGenerator-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
 
 except Exception as error:
     __version__ = "0.0.1"
     sys.stderr.write("Warning: Could not open '%s' due %s\n" % (filepath, error))
 
 requirements = [
-    "numpy==1.19.2",
-    "SimpleITK==2.1.0",
+    "numpy>=1.19.2",
+    "SimpleITK!=2.0.*",
+    "SimpleITK!=2.2.1",  # https://github.com/mlcommons/GaNDLF/issues/536
     "pytest",
     "coverage",
     "psutil",
     "black",
     "matplotlib",
     "requests",
 ]
```

