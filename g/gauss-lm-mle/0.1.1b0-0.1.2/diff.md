# Comparing `tmp/gauss-lm-mle-0.1.1b0.tar.gz` & `tmp/gauss-lm-mle-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauss-lm-mle-0.1.1b0.tar", last modified: Mon Jul 10 23:18:23 2023, max compression
+gzip compressed data, was "gauss-lm-mle-0.1.2.tar", last modified: Tue Jul 11 17:43:52 2023, max compression
```

## Comparing `gauss-lm-mle-0.1.1b0.tar` & `gauss-lm-mle-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-10 23:18:23.188941 gauss-lm-mle-0.1.1b0/
--rw-r--r--   0 delnatan   (501) staff       (20)    18092 2023-07-10 20:57:55.000000 gauss-lm-mle-0.1.1b0/LICENSE
--rw-r--r--   0 delnatan   (501) staff       (20)      132 2023-07-10 23:18:23.188815 gauss-lm-mle-0.1.1b0/PKG-INFO
--rw-r--r--   0 delnatan   (501) staff       (20)     1338 2023-07-10 22:11:59.000000 gauss-lm-mle-0.1.1b0/README.md
-drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-10 23:18:23.187456 gauss-lm-mle-0.1.1b0/c_src/
--rw-r--r--   0 delnatan   (501) staff       (20)     7946 2023-07-10 20:58:04.000000 gauss-lm-mle-0.1.1b0/c_src/gfit.c
--rw-r--r--   0 delnatan   (501) staff       (20)    15691 2023-07-10 20:58:04.000000 gauss-lm-mle-0.1.1b0/c_src/lm_mle.c
-drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-10 23:18:23.187925 gauss-lm-mle-0.1.1b0/gauss_lm_mle/
--rw-r--r--   0 delnatan   (501) staff       (20)       62 2023-07-10 21:25:27.000000 gauss-lm-mle-0.1.1b0/gauss_lm_mle/__init__.py
--rw-r--r--   0 delnatan   (501) staff       (20)     2359 2023-07-10 20:58:04.000000 gauss-lm-mle-0.1.1b0/gauss_lm_mle/fitters.py
--rw-r--r--   0 delnatan   (501) staff       (20)     1023 2023-07-10 20:58:04.000000 gauss-lm-mle-0.1.1b0/gauss_lm_mle/liblm_mle_de.py
--rw-r--r--   0 delnatan   (501) staff       (20)     2407 2023-07-10 21:29:10.000000 gauss-lm-mle-0.1.1b0/gauss_lm_mle/utils.py
-drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-10 23:18:23.188533 gauss-lm-mle-0.1.1b0/gauss_lm_mle.egg-info/
--rw-r--r--   0 delnatan   (501) staff       (20)      132 2023-07-10 23:18:23.000000 gauss-lm-mle-0.1.1b0/gauss_lm_mle.egg-info/PKG-INFO
--rw-r--r--   0 delnatan   (501) staff       (20)      368 2023-07-10 23:18:23.000000 gauss-lm-mle-0.1.1b0/gauss_lm_mle.egg-info/SOURCES.txt
--rw-r--r--   0 delnatan   (501) staff       (20)        1 2023-07-10 23:18:23.000000 gauss-lm-mle-0.1.1b0/gauss_lm_mle.egg-info/dependency_links.txt
--rw-r--r--   0 delnatan   (501) staff       (20)       19 2023-07-10 23:18:23.000000 gauss-lm-mle-0.1.1b0/gauss_lm_mle.egg-info/requires.txt
--rw-r--r--   0 delnatan   (501) staff       (20)       13 2023-07-10 23:18:23.000000 gauss-lm-mle-0.1.1b0/gauss_lm_mle.egg-info/top_level.txt
--rw-r--r--   0 delnatan   (501) staff       (20)       38 2023-07-10 23:18:23.188974 gauss-lm-mle-0.1.1b0/setup.cfg
--rw-r--r--   0 delnatan   (501) staff       (20)     1070 2023-07-10 23:17:18.000000 gauss-lm-mle-0.1.1b0/setup.py
-drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-10 23:18:23.188649 gauss-lm-mle-0.1.1b0/tests/
--rw-r--r--   0 delnatan   (501) staff       (20)      880 2023-07-10 20:58:04.000000 gauss-lm-mle-0.1.1b0/tests/test_mle_rotated_gaussian.py
+drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-11 17:43:52.085374 gauss-lm-mle-0.1.2/
+-rw-r--r--   0 delnatan   (501) staff       (20)    18092 2023-07-10 20:57:55.000000 gauss-lm-mle-0.1.2/LICENSE
+-rw-r--r--   0 delnatan   (501) staff       (20)      130 2023-07-11 17:43:52.085240 gauss-lm-mle-0.1.2/PKG-INFO
+-rw-r--r--   0 delnatan   (501) staff       (20)     1338 2023-07-10 22:11:59.000000 gauss-lm-mle-0.1.2/README.md
+drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-11 17:43:52.083619 gauss-lm-mle-0.1.2/c_src/
+-rw-r--r--   0 delnatan   (501) staff       (20)    11855 2023-07-11 17:42:20.000000 gauss-lm-mle-0.1.2/c_src/gfit.c
+-rw-r--r--   0 delnatan   (501) staff       (20)    15691 2023-07-10 20:58:04.000000 gauss-lm-mle-0.1.2/c_src/lm_mle.c
+drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-11 17:43:52.084224 gauss-lm-mle-0.1.2/gauss_lm_mle/
+-rw-r--r--   0 delnatan   (501) staff       (20)       76 2023-07-11 17:37:18.000000 gauss-lm-mle-0.1.2/gauss_lm_mle/__init__.py
+-rw-r--r--   0 delnatan   (501) staff       (20)     4553 2023-07-11 17:28:32.000000 gauss-lm-mle-0.1.2/gauss_lm_mle/fitters.py
+-rw-r--r--   0 delnatan   (501) staff       (20)     1549 2023-07-11 17:26:58.000000 gauss-lm-mle-0.1.2/gauss_lm_mle/liblm_mle_de.py
+-rw-r--r--   0 delnatan   (501) staff       (20)     2407 2023-07-10 21:29:10.000000 gauss-lm-mle-0.1.2/gauss_lm_mle/utils.py
+drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-11 17:43:52.084950 gauss-lm-mle-0.1.2/gauss_lm_mle.egg-info/
+-rw-r--r--   0 delnatan   (501) staff       (20)      130 2023-07-11 17:43:52.000000 gauss-lm-mle-0.1.2/gauss_lm_mle.egg-info/PKG-INFO
+-rw-r--r--   0 delnatan   (501) staff       (20)      368 2023-07-11 17:43:52.000000 gauss-lm-mle-0.1.2/gauss_lm_mle.egg-info/SOURCES.txt
+-rw-r--r--   0 delnatan   (501) staff       (20)        1 2023-07-11 17:43:52.000000 gauss-lm-mle-0.1.2/gauss_lm_mle.egg-info/dependency_links.txt
+-rw-r--r--   0 delnatan   (501) staff       (20)       19 2023-07-11 17:43:52.000000 gauss-lm-mle-0.1.2/gauss_lm_mle.egg-info/requires.txt
+-rw-r--r--   0 delnatan   (501) staff       (20)       13 2023-07-11 17:43:52.000000 gauss-lm-mle-0.1.2/gauss_lm_mle.egg-info/top_level.txt
+-rw-r--r--   0 delnatan   (501) staff       (20)       38 2023-07-11 17:43:52.085410 gauss-lm-mle-0.1.2/setup.cfg
+-rw-r--r--   0 delnatan   (501) staff       (20)     1069 2023-07-11 17:33:26.000000 gauss-lm-mle-0.1.2/setup.py
+drwxr-xr-x   0 delnatan   (501) staff       (20)        0 2023-07-11 17:43:52.085081 gauss-lm-mle-0.1.2/tests/
+-rw-r--r--   0 delnatan   (501) staff       (20)      880 2023-07-10 20:58:04.000000 gauss-lm-mle-0.1.2/tests/test_mle_rotated_gaussian.py
```

### Comparing `gauss-lm-mle-0.1.1b0/LICENSE` & `gauss-lm-mle-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gauss-lm-mle-0.1.1b0/README.md` & `gauss-lm-mle-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gauss-lm-mle-0.1.1b0/c_src/gfit.c` & `gauss-lm-mle-0.1.2/c_src/gfit.c`

 * *Files 16% similar despite different names*

```diff
@@ -73,14 +73,70 @@
     jac[i * m + 5] = exp(-wrk);
     // partial bg
     jac[i * m + 6] = 1.0;
   }
     
 }
 
+void gaussian_f(double* p, double* f, int m, int n, void* adata) {
+  double xc, yc, sigma, A, bg;
+  double xarg, yarg, wrk;
+
+  // 'adata' will be a pointer to coord_data
+  // cast to a pointer to `coord_data` to access the struct
+  coord_data* coord = (coord_data*) adata;
+  xc	= p[0];
+  yc	= p[1];
+  sigma = p[2];
+  A	= p[3];
+  bg	= p[4];
+
+  double sigma2 = sigma * sigma;
+  
+  for (int i=0; i<n; i++) {
+    xarg = coord->x[i] - xc;
+    yarg = coord->y[i] - yc;
+    wrk = (xarg*xarg)/(2*sigma2) + (yarg*yarg)/(2*sigma2);
+    f[i] = A * exp(-wrk) + bg;
+  }
+}
+
+// jacobian for symmetric gaussian function
+void gaussian_df(double* p, double* jac, int m, int n, void* adata) {
+  double xc, yc, sigma, A;
+  double xarg, yarg, wrk;
+  coord_data* coord = (coord_data*) adata;
+  xc	= p[0];
+  yc	= p[1];
+  sigma = p[2];
+  A	= p[3];
+
+  double sigma2 = sigma * sigma;
+  double sigma3 = sigma2 * sigma;
+  
+  for (int i=0; i<n; i++) {
+    xarg = coord->x[i] - xc;
+    yarg = coord->y[i] - yc;
+    wrk  = (xarg*xarg)/(2*sigma2) + (yarg*yarg)/(2*sigma2);
+
+    //partial xc
+    jac[i * m] = A * xarg * exp(-wrk) / sigma2;
+    //partial yc
+    jac[i * m + 1] = A * yarg * exp(-wrk) / sigma2;
+    //partial sigma
+    jac[i * m + 2] = A * exp(-wrk) * ((xarg*xarg)/sigma3 + (yarg*yarg)/sigma3);
+    //partial A
+    jac[i * m + 3] = exp(-wrk);
+    //partial bg
+    jac[i * m + 4] = 1.0;
+  }
+  
+}
+
+
 /*
   Function definition for LM minimizer
 
   int dlevmar_mle_der(
   void (*func)(double *p, double *hx, int m, int n, void *adata),
   void (*jacf)(double *p, double *j, int m, int n, void *adata),
   double *p, double *x, int m, int n, int itmax, double *opts,
@@ -162,15 +218,15 @@
 }
 
 void free_results(double* results) {
   free(results);
 }
 
 
-void fit_peaks(
+void fit_rotated_gaussian(
 	       double* image, int* ylocs, int *xlocs, 
 	       int img_height, int img_width, int nlocs, int boxsize, int itermax,
 	       double* results
 	       ) 
 {
   /*
     Perform Gaussian fitting to localize to single-molecule intensities
@@ -233,21 +289,17 @@
 
     // scale parameters a, b, c
     double a0 = 1 / (2 * sigma0 * sigma0);
     double c0 = 1 / (2 * sigma0 * sigma0);
     
     // at the moment start with the same parameters for all
     // todo: get better estimate with first/second moments
-    double pars[7] = {a0, 1e-4, c0, xc0, yc0, roi_max_val, roi_min_val};
+    double pars[7] = {a0, 1e-4, c0, xc0, yc0, roi_max_val - roi_min_val, roi_min_val};
     double info[LM_INFO_SZ];
 
-    // for guess
-    pars[5] = roi_max_val - roi_min_val;
-    pars[6] = roi_min_val;
-
     dlevmar_mle_der(&rotated_gaussian_f, &rotated_gaussian_df,
 		    pars, roi, npars, ndata, itermax, NULL, info,
 		    NULL, NULL, &coords, 0);
 
     // printf("Peak fit #%d ==> A,%.2f \t bg,%.2f\n", n, pars[5], pars[6]);
     /* printf("x0,y0 @ #%d ==> %.3f, %.3f\n", n, xc0, yc0); */
 
@@ -276,7 +328,98 @@
   }
 
   free(roi);
   free_coord_data(&coords);
   
 }
 
+
+void fit_gaussian(
+		   double* image, int* ylocs, int *xlocs, 
+		   int img_height, int img_width, int nlocs, int boxsize, int itermax,
+		   double* results
+		   ) 
+{
+  /*
+    Perform Gaussian fitting to localize to single-molecule intensities
+    using MLE.
+
+   */
+  double roi_min_val, roi_max_val, pixval;
+
+  double sigma0 = 1.4;
+  
+  int s = boxsize / 2;
+  
+  double* roi = malloc(boxsize * boxsize * sizeof(double));
+
+  int npars = 5;
+  int nresults = 7;
+  int ndata = boxsize * boxsize;
+
+  // define box coordinates
+  coord_data coords = meshgrid2d(boxsize);
+  
+  // loop through each maxima
+  for (int n=0; n < nlocs; n++) {
+    // extract ROI from image
+    int yc = ylocs[n];
+    int xc = xlocs[n];
+    
+    // copy pixels of ROI into 'roi'
+    for (int i = -s; i <= s; i++) {
+      for (int j= -s; j <= s; j++) {
+	pixval = image[(yc + i) * img_width + (xc + j)];
+	roi[(i + s) * boxsize + (j + s)] = pixval;
+      }
+    }
+
+    // compute initial estimates
+    // Amplitude and background is initially max(roi) and min(roi)
+    roi_min_val = roi[0];
+    roi_max_val = roi[0];
+
+    for (int i = 0; i < boxsize; i++) {
+      for (int j= 0; j < boxsize; j++) {
+	pixval = roi[i * boxsize + j];
+	if (pixval < roi_min_val) roi_min_val = pixval;
+	if (pixval > roi_max_val) roi_max_val = pixval;
+      }
+    }
+
+    double weight = 0.0;
+    double weighted_sum_x = 0.0;
+    double weighted_sum_y = 0.0;
+    // compute first moment to estimate x,y position
+    for (int i = 0; i < coords.num_coords; i++) {
+      weight += (roi[i] - roi_min_val);
+      weighted_sum_x += coords.x[i] * (roi[i] - roi_min_val);
+      weighted_sum_y += coords.y[i] * (roi[i] - roi_min_val);
+    }
+    double xc0 = weighted_sum_x / weight;
+    double yc0 = weighted_sum_y / weight;
+
+    // at the moment start with the same parameters for all
+    double pars[5] = {xc0, yc0, sigma0, roi_max_val - roi_min_val, roi_min_val};
+    double info[LM_INFO_SZ];
+
+    dlevmar_mle_der(&gaussian_f, &gaussian_df,
+		    pars, roi, npars, ndata, itermax, NULL, info,
+		    NULL, NULL, &coords, 0);
+
+    // populate results
+    // A, bg, xc, yc, sigma_x, sigma_y, theta, asymm; niter, 
+    results[n * nresults] = pars[3]; // Amplitude
+    results[n * nresults + 1] = pars[4]; // background
+    results[n * nresults + 2] = (double) xc + pars[0]; // xc
+    results[n * nresults + 3] = (double) yc + pars[1]; // yc
+    results[n * nresults + 4] = pars[2]; // sigma
+    results[n * nresults + 5] = info[5]; // niter
+    results[n * nresults + 6] = info[1]; // norm2 of error
+   
+  }
+
+  free(roi);
+  free_coord_data(&coords);
+  
+}
+
```

### Comparing `gauss-lm-mle-0.1.1b0/c_src/lm_mle.c` & `gauss-lm-mle-0.1.2/c_src/lm_mle.c`

 * *Files identical despite different names*

### Comparing `gauss-lm-mle-0.1.1b0/gauss_lm_mle/fitters.py` & `gauss-lm-mle-0.1.2/gauss_lm_mle/fitters.py`

 * *Files 21% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     xlocs = np.ascontiguousarray(yxlocs[1].astype(np.intc))
     npeaks = len(ylocs)
 
     # preallocate results
     fitres = np.empty((npeaks, 10), dtype=np.double)
 
     # call C library
-    lib.fit_peaks(
+    lib.fit_rotated_gaussian(
         image,
         ylocs,
         xlocs,
         image.shape[0],
         image.shape[1],
         npeaks,
         boxsize,
@@ -77,8 +77,83 @@
             "niter",
             "norm2_error",
         ],
     )
 
     dfres["niter"] = dfres["niter"].astype(int)
 
+    return dfres
+
+
+def mle_gaussian(
+    image: np.ndarray,
+    yxlocs: tuple,
+    boxsize: int,
+    itermax: int,
+) -> pd.DataFrame:
+    """
+    Perform maximum likelihood estimation (MLE) fitting of a Gaussian function on an image.
+
+    The function calls a C library function that performs the MLE fitting, and returns the results in a pandas DataFrame.
+
+    Parameters
+    ----------
+    image : np.ndarray
+        The image data as a 2D numpy array.
+    yxlocs : tuple of np.ndarray
+        A tuple of two 1D numpy arrays containing the y and x coordinates of the peaks to fit, respectively.
+    boxsize : int
+        The size of the box to extract around each peak for fitting.
+    itermax : int
+        The maximum number of iterations for the MLE fitting algorithm.
+
+    Returns
+    -------
+    pd.DataFrame
+        A DataFrame containing the MLE fitting results. Each row corresponds to one peak, and the columns are:
+        'A' - Amplitude of the Gaussian.
+        'bg' - Background offset.
+        'x' and 'y' - Coordinates of the Gaussian's peak.
+        'sx' and 'sy' - Standard deviations of the Gaussian along the x and y axes, respectively.
+        'theta' - Rotation angle of the Gaussian (in radians).
+        'asymmetry' - Asymmetry parameter of the Gaussian.
+        'niter' - The number of iterations performed by the fitting algorithm.
+        'norm2_error' - The squared error norm of the fit.
+    """
+
+    image = np.ascontiguousarray(image.astype(np.double))
+    ylocs = np.ascontiguousarray(yxlocs[0].astype(np.intc))
+    xlocs = np.ascontiguousarray(yxlocs[1].astype(np.intc))
+    npeaks = len(ylocs)
+
+    # preallocate results
+    fitres = np.empty((npeaks, 7), dtype=np.double)
+
+    # call C library
+    lib.fit_gaussian(
+        image,
+        ylocs,
+        xlocs,
+        image.shape[0],
+        image.shape[1],
+        npeaks,
+        boxsize,
+        itermax,
+        fitres,
+    )
+
+    dfres = pd.DataFrame(
+        fitres,
+        columns=[
+            "A",
+            "bg",
+            "x",
+            "y",
+            "sigma",
+            "niter",
+            "norm2_error",
+        ],
+    )
+
+    dfres["niter"] = dfres["niter"].astype(int)
+
     return dfres
```

### Comparing `gauss-lm-mle-0.1.1b0/gauss_lm_mle/liblm_mle_de.py` & `gauss-lm-mle-0.1.2/gauss_lm_mle/liblm_mle_de.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,22 +12,36 @@
     lib_path = os.path.join(dir_path, lib_filename)
 
     try:
         lib = ctypes.CDLL(lib_path)
     except OSError as e:
         raise OSError(f"Failed to load shared library {lib_path}.") from e
 
-    lib.fit_peaks.argtypes = [
+    lib.fit_rotated_gaussian.argtypes = [
         np.ctypeslib.ndpointer(dtype=np.double, ndim=2, flags="C_CONTIGUOUS"),
         np.ctypeslib.ndpointer(dtype=np.intc, ndim=1, flags="C_CONTIGUOUS"),
         np.ctypeslib.ndpointer(dtype=np.intc, ndim=1, flags="C_CONTIGUOUS"),
         ctypes.c_int,
         ctypes.c_int,
         ctypes.c_int,
         ctypes.c_int,
         ctypes.c_int,
         np.ctypeslib.ndpointer(dtype=np.double, ndim=2, flags="C_CONTIGUOUS"),
     ]
 
-    lib.fit_peaks.restype = None
+    lib.fit_rotated_gaussian.restype = None
 
+    lib.fit_gaussian.argtypes = [
+        np.ctypeslib.ndpointer(dtype=np.double, ndim=2, flags="C_CONTIGUOUS"),
+        np.ctypeslib.ndpointer(dtype=np.intc, ndim=1, flags="C_CONTIGUOUS"),
+        np.ctypeslib.ndpointer(dtype=np.intc, ndim=1, flags="C_CONTIGUOUS"),
+        ctypes.c_int,
+        ctypes.c_int,
+        ctypes.c_int,
+        ctypes.c_int,
+        ctypes.c_int,
+        np.ctypeslib.ndpointer(dtype=np.double, ndim=2, flags="C_CONTIGUOUS"),
+    ]
+
+    lib.fit_gaussian.restype = None
+    
     return lib
```

### Comparing `gauss-lm-mle-0.1.1b0/gauss_lm_mle/utils.py` & `gauss-lm-mle-0.1.2/gauss_lm_mle/utils.py`

 * *Files identical despite different names*

### Comparing `gauss-lm-mle-0.1.1b0/setup.py` & `gauss-lm-mle-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     libraries=libraries,
     extra_compile_args=cflags,
 )
 
 # Setup
 setup(
     name="gauss-lm-mle",
-    version="0.1.1b",
+    version="0.1.2",
     description="MLE Gaussian fitting with Poisson deviates",
     ext_modules=[lm_mle_de_module],
     packages=["gauss_lm_mle"],
     package_data={"gauss_lm_mle": ["c_src/*.h"]},
     install_requires=[  # Add your Python dependencies here
         "numpy",
         "pandas",
```

### Comparing `gauss-lm-mle-0.1.1b0/tests/test_mle_rotated_gaussian.py` & `gauss-lm-mle-0.1.2/tests/test_mle_rotated_gaussian.py`

 * *Files identical despite different names*

