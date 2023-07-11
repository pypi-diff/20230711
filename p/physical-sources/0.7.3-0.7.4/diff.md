# Comparing `tmp/physical_sources-0.7.3.tar.gz` & `tmp/physical_sources-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physical_sources-0.7.3.tar", last modified: Wed Jun 21 16:40:25 2023, max compression
+gzip compressed data, was "physical_sources-0.7.4.tar", last modified: Tue Jul 11 18:12:19 2023, max compression
```

## Comparing `physical_sources-0.7.3.tar` & `physical_sources-0.7.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 16:40:25.446131 physical_sources-0.7.3/
--rw-rw-rw-   0        0        0     2827 2023-06-21 16:40:25.443134 physical_sources-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     1743 2023-05-11 14:32:07.000000 physical_sources-0.7.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 16:40:25.447129 physical_sources-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-06-21 16:40:06.000000 physical_sources-0.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:40:25.343486 physical_sources-0.7.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 16:40:25.361339 physical_sources-0.7.3/src/physical_sources/
--rw-rw-rw-   0        0        0       24 2023-05-11 14:32:08.000000 physical_sources-0.7.3/src/physical_sources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:40:25.428141 physical_sources-0.7.3/src/physical_sources/acoustic/
--rw-rw-rw-   0        0        0    22297 2023-06-21 16:28:18.000000 physical_sources-0.7.3/src/physical_sources/acoustic/NOISEFILE.py
--rw-rw-rw-   0        0        0       99 2023-06-21 16:28:18.000000 physical_sources-0.7.3/src/physical_sources/acoustic/__init__.py
--rw-rw-rw-   0        0        0    42519 2023-06-21 16:28:18.000000 physical_sources-0.7.3/src/physical_sources/acoustic/harmonic_series_representation.py
--rw-rw-rw-   0        0        0     4234 2023-06-21 16:28:18.000000 physical_sources-0.7.3/src/physical_sources/acoustic/ideal_dipole.py
--rw-rw-rw-   0        0        0    10823 2023-06-21 16:28:18.000000 physical_sources-0.7.3/src/physical_sources/acoustic/interpolated_harmonic_series.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:40:25.439139 physical_sources-0.7.3/src/physical_sources/eeg/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:32:08.000000 physical_sources-0.7.3/src/physical_sources/eeg/__init__.py
--rw-rw-rw-   0        0        0     5051 2023-06-21 16:28:18.000000 physical_sources-0.7.3/src/physical_sources/eeg/eeg_equivalent_source.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:40:25.400129 physical_sources-0.7.3/src/physical_sources.egg-info/
--rw-rw-rw-   0        0        0     2827 2023-06-21 16:40:25.000000 physical_sources-0.7.3/src/physical_sources.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-06-21 16:40:25.000000 physical_sources-0.7.3/src/physical_sources.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 16:40:25.000000 physical_sources-0.7.3/src/physical_sources.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-06-21 16:40:25.000000 physical_sources-0.7.3/src/physical_sources.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-21 16:40:25.000000 physical_sources-0.7.3/src/physical_sources.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 18:12:19.836264 physical_sources-0.7.4/
+-rw-rw-rw-   0        0        0     1246 2023-07-11 17:45:55.000000 physical_sources-0.7.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2611 2023-07-11 18:12:19.817132 physical_sources-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1743 2023-05-11 14:32:07.000000 physical_sources-0.7.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:12:19.836264 physical_sources-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      977 2023-07-07 16:01:14.000000 physical_sources-0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:12:19.182408 physical_sources-0.7.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 18:12:19.281373 physical_sources-0.7.4/src/physical_sources/
+-rw-rw-rw-   0        0        0        0 2023-07-07 16:01:14.000000 physical_sources-0.7.4/src/physical_sources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:12:19.613753 physical_sources-0.7.4/src/physical_sources/acoustic/
+-rw-rw-rw-   0        0        0    22297 2023-06-21 16:28:18.000000 physical_sources-0.7.4/src/physical_sources/acoustic/NOISEFILE.py
+-rw-rw-rw-   0        0        0        0 2023-07-07 16:01:14.000000 physical_sources-0.7.4/src/physical_sources/acoustic/__init__.py
+-rw-rw-rw-   0        0        0    41817 2023-06-23 15:55:41.000000 physical_sources-0.7.4/src/physical_sources/acoustic/harmonic_series_representation.py
+-rw-rw-rw-   0        0        0     4234 2023-06-21 16:28:18.000000 physical_sources-0.7.4/src/physical_sources/acoustic/ideal_dipole.py
+-rw-rw-rw-   0        0        0    10823 2023-06-21 16:28:18.000000 physical_sources-0.7.4/src/physical_sources/acoustic/interpolated_harmonic_series.py
+-rw-rw-rw-   0        0        0     1796 2023-06-23 15:55:41.000000 physical_sources-0.7.4/src/physical_sources/acoustic/isphere_source.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:12:19.811183 physical_sources-0.7.4/src/physical_sources/eeg/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:32:08.000000 physical_sources-0.7.4/src/physical_sources/eeg/__init__.py
+-rw-rw-rw-   0        0        0     5051 2023-06-21 16:28:18.000000 physical_sources-0.7.4/src/physical_sources/eeg/eeg_equivalent_source.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:12:19.324328 physical_sources-0.7.4/src/physical_sources.egg-info/
+-rw-rw-rw-   0        0        0     2611 2023-07-11 18:12:17.000000 physical_sources-0.7.4/src/physical_sources.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-07-11 18:12:18.000000 physical_sources-0.7.4/src/physical_sources.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 18:12:17.000000 physical_sources-0.7.4/src/physical_sources.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-07-11 18:12:17.000000 physical_sources-0.7.4/src/physical_sources.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-11 18:12:17.000000 physical_sources-0.7.4/src/physical_sources.egg-info/top_level.txt
```

### Comparing `physical_sources-0.7.3/PKG-INFO` & `physical_sources-0.7.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: physical_sources
-Version: 0.7.3
+Version: 0.7.4
 Summary: A collection of classes that can be used to build acoustic sources from the NOISEFILE format. It also contains classes to read the binary representations born from the author's dissertation
-Home-page: UNKNOWN
+Home-page: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
-License: UNKNOWN
-Description: # ![Image](./GhostEye.png "GhostEye") physical_sources
-        
-        This is a collection of classes meant to provide access to acoustic source levels that were contained within the initial
-        release of the Counter Listener Acoustic Warfare Software (CLAWS). But with the changes to the releasibility of the code
-        and data from CLAWS, a number of classes were removed from the distribution. 
-        
-        ## NOISEFILE
-        The _NOISEFILE_ representation of the various aircraft is retained, since these source descriptions are deemed unclassified
-        and publically available through the various community noise releases. These data come as the static, ground-based measurements
-        that define the semicircular data from the nose to the tail, on the left side of the aircraft. The second set of data exists
-        within the flight database. This data is a collection of single spectra that were integrated as the __loudest__ portion of the
-        over-flight data. As such, it provides an over-estimate at the majority of the locations around the aircraft.
-        
-        These datasets exist in a single library file, that can be loaded and then searched for the specific aircraft/power setting
-        combination that is desired. Each element within the library exists as its own class that can be extracted and then saved
-        externally as another file. These files can then be loaded without consideration for the remainder of the acoustic data.
-        
-        ### Usage - Loading Flight NOISEFILE data extracted from the library previously
-            filename = str(Path(__file__).parents[3]) + "/_test data/physical_sources/acoustic_source/approach power.nf"
-            nfas = NoiseFileAcousticSource(filename)
-            s = SphericalCoordinate()
-        
-            spl1 = nfas._sound_pressure_levels
-            spl2 = nfas.sound_pressure_level(s)
-        
-        
-        
-        # 2023
-        ## May
-        + Creation of the package
-        + Added functions for the plotting of the surface
-        + Moved functions for calculating the harmonic series expansion from separate classes to functions in the harmonic series representation
-        
-        ## June
-        + Updated the class for reading the EEG data to obtain a Waveform object from the selected channel within the listing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# ![Image](./GhostEye.png "GhostEye") physical_sources
+
+This is a collection of classes meant to provide access to acoustic source levels that were contained within the initial
+release of the Counter Listener Acoustic Warfare Software (CLAWS). But with the changes to the releasibility of the code
+and data from CLAWS, a number of classes were removed from the distribution. 
+
+## NOISEFILE
+The _NOISEFILE_ representation of the various aircraft is retained, since these source descriptions are deemed unclassified
+and publically available through the various community noise releases. These data come as the static, ground-based measurements
+that define the semicircular data from the nose to the tail, on the left side of the aircraft. The second set of data exists
+within the flight database. This data is a collection of single spectra that were integrated as the __loudest__ portion of the
+over-flight data. As such, it provides an over-estimate at the majority of the locations around the aircraft.
+
+These datasets exist in a single library file, that can be loaded and then searched for the specific aircraft/power setting
+combination that is desired. Each element within the library exists as its own class that can be extracted and then saved
+externally as another file. These files can then be loaded without consideration for the remainder of the acoustic data.
+
+### Usage - Loading Flight NOISEFILE data extracted from the library previously
+    filename = str(Path(__file__).parents[3]) + "/_test data/physical_sources/acoustic_source/approach power.nf"
+    nfas = NoiseFileAcousticSource(filename)
+    s = SphericalCoordinate()
+
+    spl1 = nfas._sound_pressure_levels
+    spl2 = nfas.sound_pressure_level(s)
+
+
+
+# 2023
+## May
++ Creation of the package
++ Added functions for the plotting of the surface
++ Moved functions for calculating the harmonic series expansion from separate classes to functions in the harmonic series representation
+
+## June
++ Updated the class for reading the EEG data to obtain a Waveform object from the selected channel within the listing
++ Refactored the HarmonicSeries class to inherit from the ISphereSource interface.
```

### Comparing `physical_sources-0.7.3/README.md` & `physical_sources-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `physical_sources-0.7.3/setup.py` & `physical_sources-0.7.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,21 @@
     README = readme_file.read()
 
     with open('HISTORY.md') as history_file:
         HISTORY = history_file.read()
 
 setup(
     name='physical_sources',
-    version='0.7.3',
+    version='0.7.4',
     packages=find_packages('src', exclude=['test*.py']),
     url='',
     license='',
     author='Dr. Frank Mobley',
     author_email='frank.mobley.1@afrl.af.mil',
     description="A collection of classes that can be used to build acoustic sources from the NOISEFILE format. It "
                 "also contains classes to read the binary representations born from the author's dissertation",
     package_dir={'': 'src'},
     long_description=README + '\n\n' + HISTORY,
     long_description_content_type="text/markdown",
     install_requires=['numpy', 'scipy', 'PythonCoordinates>=0.5.0', 'Pytimbre>0.6.1', 'mne>=1.0.0',
-                      'physical_propagation>=0.5.1']
+                      'physical_propagation>=0.5.1', 'matplotlib>=3.3.1']
 )
```

### Comparing `physical_sources-0.7.3/src/physical_sources/acoustic/NOISEFILE.py` & `physical_sources-0.7.4/src/physical_sources/acoustic/NOISEFILE.py`

 * *Files identical despite different names*

### Comparing `physical_sources-0.7.3/src/physical_sources/acoustic/harmonic_series_representation.py` & `physical_sources-0.7.4/src/physical_sources/acoustic/harmonic_series_representation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pytimbre.spectral.fractional_octave_band import FractionalOctaveBandTools
 import numpy as np
 from dateutil import parser
 import warnings
 import sys
 import scipy
 from matplotlib import cm, colors
+from .isphere_source import ISphereSource
 
 
 def plot_irregular_surface(locations, desired_x=None, desired_y=None, ax=None, vmin=None, vmax=None, colormap=cm.jet,
                            invert_z_axis: bool = True):
     """
     We desire the ability to plot the spherical surface in a 3-D representation where the faces will be the color of
     the acoustic level that we are attempting to characterize.
@@ -177,15 +178,15 @@
                     linestyles='solid',
                     colors='k')
     ax.clabel(cs, fontsize=6, inline=1, fmt='%.0f')
 
     return fig, ax
 
 
-class HarmonicSeries:
+class HarmonicSeries(ISphereSource):
     """
     The harmonic source is a collection of coefficient definition sets. This definition is the example of how to
     organize the information, but does not have to be a frequency band. So this was refactored to be more generic.
     """
 
     def __init__(self, series_coefficients: np.ndarray, description: str, r: float = None, mse: float = None):
         """
@@ -214,30 +215,14 @@
         array-like list of complex coefficients.
         :return: array-like
             List of complex coefficients that represent the harmonic expansion
         """
         return self._coefficients
 
     @property
-    def series_description(self):
-        """
-        Initially, these series represented a frequency within the sound pressure level spectrum. However,
-        there was no reason to require this representation has a sound pressure level representation. Rather it is
-        merely an expansion of a spherical dataset. As such this could be any function. So the band number was
-        dropped and a string description was used to determine the function expanded with the harmonic series.
-        :return: str
-            The custom description of the series expansion
-        """
-        return self._description
-
-    @series_description.setter
-    def series_description(self, value):
-        self._description = value
-
-    @property
     def fit_correlation_coefficient(self):
         return self._pearson_r
 
     @property
     def fit_mse(self):
         return self._mse
 
@@ -514,15 +499,15 @@
         class's series expansion and append it directly to the root that is provided.
         :param root: ElementTree
             The parent of the XML node that we are constructing in this function
         :return:
         """
 
         parent = xml.etree.ElementTree.SubElement(root, "series_expansion")
-        parent.attrib['description'] = self.series_description
+        parent.attrib['description'] = self.description
         if self.fit_correlation_coefficient is not None:
             parent.attrib['fit_correlation_coefficient'] = "{:.10f}".format(self.fit_correlation_coefficient)
         if self.fit_mse is not None:
             parent.attrib['fit_mse'] = "{:.10f}".format(self.fit_mse)
 
         coefficients = xml.etree.ElementTree.SubElement(parent, "coefficients")
```

### Comparing `physical_sources-0.7.3/src/physical_sources/acoustic/ideal_dipole.py` & `physical_sources-0.7.4/src/physical_sources/acoustic/ideal_dipole.py`

 * *Files identical despite different names*

### Comparing `physical_sources-0.7.3/src/physical_sources/acoustic/interpolated_harmonic_series.py` & `physical_sources-0.7.4/src/physical_sources/acoustic/interpolated_harmonic_series.py`

 * *Files identical despite different names*

### Comparing `physical_sources-0.7.3/src/physical_sources/eeg/eeg_equivalent_source.py` & `physical_sources-0.7.4/src/physical_sources/eeg/eeg_equivalent_source.py`

 * *Files identical despite different names*

### Comparing `physical_sources-0.7.3/src/physical_sources.egg-info/PKG-INFO` & `physical_sources-0.7.4/src/physical_sources.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: physical-sources
-Version: 0.7.3
+Version: 0.7.4
 Summary: A collection of classes that can be used to build acoustic sources from the NOISEFILE format. It also contains classes to read the binary representations born from the author's dissertation
-Home-page: UNKNOWN
+Home-page: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
-License: UNKNOWN
-Description: # ![Image](./GhostEye.png "GhostEye") physical_sources
-        
-        This is a collection of classes meant to provide access to acoustic source levels that were contained within the initial
-        release of the Counter Listener Acoustic Warfare Software (CLAWS). But with the changes to the releasibility of the code
-        and data from CLAWS, a number of classes were removed from the distribution. 
-        
-        ## NOISEFILE
-        The _NOISEFILE_ representation of the various aircraft is retained, since these source descriptions are deemed unclassified
-        and publically available through the various community noise releases. These data come as the static, ground-based measurements
-        that define the semicircular data from the nose to the tail, on the left side of the aircraft. The second set of data exists
-        within the flight database. This data is a collection of single spectra that were integrated as the __loudest__ portion of the
-        over-flight data. As such, it provides an over-estimate at the majority of the locations around the aircraft.
-        
-        These datasets exist in a single library file, that can be loaded and then searched for the specific aircraft/power setting
-        combination that is desired. Each element within the library exists as its own class that can be extracted and then saved
-        externally as another file. These files can then be loaded without consideration for the remainder of the acoustic data.
-        
-        ### Usage - Loading Flight NOISEFILE data extracted from the library previously
-            filename = str(Path(__file__).parents[3]) + "/_test data/physical_sources/acoustic_source/approach power.nf"
-            nfas = NoiseFileAcousticSource(filename)
-            s = SphericalCoordinate()
-        
-            spl1 = nfas._sound_pressure_levels
-            spl2 = nfas.sound_pressure_level(s)
-        
-        
-        
-        # 2023
-        ## May
-        + Creation of the package
-        + Added functions for the plotting of the surface
-        + Moved functions for calculating the harmonic series expansion from separate classes to functions in the harmonic series representation
-        
-        ## June
-        + Updated the class for reading the EEG data to obtain a Waveform object from the selected channel within the listing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# ![Image](./GhostEye.png "GhostEye") physical_sources
+
+This is a collection of classes meant to provide access to acoustic source levels that were contained within the initial
+release of the Counter Listener Acoustic Warfare Software (CLAWS). But with the changes to the releasibility of the code
+and data from CLAWS, a number of classes were removed from the distribution. 
+
+## NOISEFILE
+The _NOISEFILE_ representation of the various aircraft is retained, since these source descriptions are deemed unclassified
+and publically available through the various community noise releases. These data come as the static, ground-based measurements
+that define the semicircular data from the nose to the tail, on the left side of the aircraft. The second set of data exists
+within the flight database. This data is a collection of single spectra that were integrated as the __loudest__ portion of the
+over-flight data. As such, it provides an over-estimate at the majority of the locations around the aircraft.
+
+These datasets exist in a single library file, that can be loaded and then searched for the specific aircraft/power setting
+combination that is desired. Each element within the library exists as its own class that can be extracted and then saved
+externally as another file. These files can then be loaded without consideration for the remainder of the acoustic data.
+
+### Usage - Loading Flight NOISEFILE data extracted from the library previously
+    filename = str(Path(__file__).parents[3]) + "/_test data/physical_sources/acoustic_source/approach power.nf"
+    nfas = NoiseFileAcousticSource(filename)
+    s = SphericalCoordinate()
+
+    spl1 = nfas._sound_pressure_levels
+    spl2 = nfas.sound_pressure_level(s)
+
+
+
+# 2023
+## May
++ Creation of the package
++ Added functions for the plotting of the surface
++ Moved functions for calculating the harmonic series expansion from separate classes to functions in the harmonic series representation
+
+## June
++ Updated the class for reading the EEG data to obtain a Waveform object from the selected channel within the listing
++ Refactored the HarmonicSeries class to inherit from the ISphereSource interface.
```

### Comparing `physical_sources-0.7.3/src/physical_sources.egg-info/SOURCES.txt` & `physical_sources-0.7.4/src/physical_sources.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+LICENSE.txt
 README.md
 setup.py
 src/physical_sources/__init__.py
 src/physical_sources.egg-info/PKG-INFO
 src/physical_sources.egg-info/SOURCES.txt
 src/physical_sources.egg-info/dependency_links.txt
 src/physical_sources.egg-info/requires.txt
 src/physical_sources.egg-info/top_level.txt
 src/physical_sources/acoustic/NOISEFILE.py
 src/physical_sources/acoustic/__init__.py
 src/physical_sources/acoustic/harmonic_series_representation.py
 src/physical_sources/acoustic/ideal_dipole.py
 src/physical_sources/acoustic/interpolated_harmonic_series.py
+src/physical_sources/acoustic/isphere_source.py
 src/physical_sources/eeg/__init__.py
 src/physical_sources/eeg/eeg_equivalent_source.py
```

