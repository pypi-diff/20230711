# Comparing `tmp/ndbioimage-2023.7.0.tar.gz` & `tmp/ndbioimage-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2023.7.0.tar", max compression
+gzip compressed data, was "ndbioimage-2023.7.2.tar", max compression
```

## Comparing `ndbioimage-2023.7.0.tar` & `ndbioimage-2023.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2023.7.0/LICENSE
--rw-r--r--   0        0        0     2356 2023-07-04 14:24:16.158015 ndbioimage-2023.7.0/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2023.7.0/ndbioimage/.DS_Store
--rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2023.7.0/ndbioimage/AiryScan.xml
--rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2023.7.0/ndbioimage/Elyra_test.xml
--rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2023.7.0/ndbioimage/Elyra_test2.xml
--rwxr-xr-x   0        0        0    55988 2023-07-04 13:53:41.286790 ndbioimage-2023.7.0/ndbioimage/__init__.py
--rw-r--r--   0        0        0     7736 2022-08-01 13:44:51.766744 ndbioimage-2023.7.0/ndbioimage/bf.py
--rw-r--r--   0        0        0     1749 2023-06-29 11:31:54.170380 ndbioimage-2023.7.0/ndbioimage/jvm.py
--rw-r--r--   0        0        0     8677 2023-05-25 09:24:53.290471 ndbioimage-2023.7.0/ndbioimage/ntransforms.py
--rw-r--r--   0        0        0      146 2023-05-25 09:20:54.527861 ndbioimage-2023.7.0/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8187 2023-06-29 12:01:13.546678 ndbioimage-2023.7.0/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    22889 2023-05-26 07:14:19.001535 ndbioimage-2023.7.0/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     1990 2023-06-02 11:04:25.198511 ndbioimage-2023.7.0/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     5580 2023-07-04 14:24:16.118015 ndbioimage-2023.7.0/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     2657 2023-06-12 12:28:43.438524 ndbioimage-2023.7.0/ndbioimage/readers/tifread.py
--rwxr-xr-x   0        0        0      245 2022-08-16 10:57:07.482485 ndbioimage-2023.7.0/ndbioimage/test.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2023.7.0/ndbioimage/transform.txt
--rw-r--r--   0        0        0     9609 2023-05-24 14:11:27.082389 ndbioimage-2023.7.0/ndbioimage/transforms.py
--rw-r--r--   0        0        0      805 2023-07-04 14:17:45.106181 ndbioimage-2023.7.0/pyproject.toml
--rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 ndbioimage-2023.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2023.7.2/LICENSE
+-rw-r--r--   0        0        0     2356 2023-07-04 14:24:16.158015 ndbioimage-2023.7.2/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2023.7.2/ndbioimage/.DS_Store
+-rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2023.7.2/ndbioimage/AiryScan.xml
+-rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2023.7.2/ndbioimage/Elyra_test.xml
+-rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2023.7.2/ndbioimage/Elyra_test2.xml
+-rwxr-xr-x   0        0        0    56839 2023-07-11 15:09:16.954915 ndbioimage-2023.7.2/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     7736 2022-08-01 13:44:51.766744 ndbioimage-2023.7.2/ndbioimage/bf.py
+-rw-r--r--   0        0        0     1749 2023-06-29 11:31:54.170380 ndbioimage-2023.7.2/ndbioimage/jvm.py
+-rw-r--r--   0        0        0     8677 2023-05-25 09:24:53.290471 ndbioimage-2023.7.2/ndbioimage/ntransforms.py
+-rw-r--r--   0        0        0      191 2023-07-11 08:09:24.299786 ndbioimage-2023.7.2/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8234 2023-07-06 14:55:39.578133 ndbioimage-2023.7.2/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    22926 2023-07-11 14:07:47.789813 ndbioimage-2023.7.2/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     1990 2023-06-02 11:04:25.198511 ndbioimage-2023.7.2/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6113 2023-07-05 08:19:10.133201 ndbioimage-2023.7.2/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     2657 2023-06-12 12:28:43.438524 ndbioimage-2023.7.2/ndbioimage/readers/tifread.py
+-rwxr-xr-x   0        0        0      245 2022-08-16 10:57:07.482485 ndbioimage-2023.7.2/ndbioimage/test.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2023.7.2/ndbioimage/transform.txt
+-rw-r--r--   0        0        0     9609 2023-05-24 14:11:27.082389 ndbioimage-2023.7.2/ndbioimage/transforms.py
+-rw-r--r--   0        0        0      837 2023-07-11 15:20:02.399013 ndbioimage-2023.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 ndbioimage-2023.7.2/PKG-INFO
```

### Comparing `ndbioimage-2023.7.0/LICENSE` & `ndbioimage-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/README.md` & `ndbioimage-2023.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/.DS_Store` & `ndbioimage-2023.7.2/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/AiryScan.xml` & `ndbioimage-2023.7.2/ndbioimage/AiryScan.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/Elyra_test.xml` & `ndbioimage-2023.7.2/ndbioimage/Elyra_test.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/Elyra_test2.xml` & `ndbioimage-2023.7.2/ndbioimage/Elyra_test2.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/__init__.py` & `ndbioimage-2023.7.2/ndbioimage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 from collections import OrderedDict
 from abc import ABCMeta, abstractmethod
 from functools import cached_property
 from parfor import parfor
 from tiffwrite import IJTiffFile
 from numbers import Number
 from argparse import ArgumentParser
-from ndbioimage.transforms import Transform, Transforms
-from ndbioimage.jvm import JVM
 from typing import List
 from pathlib import Path
 from importlib.metadata import version
 from traceback import print_exc
+from ndbioimage.transforms import Transform, Transforms
+from ndbioimage.jvm import JVM
 
 
 try:
     __version__ = version(Path(__file__).parent.name)
 except (Exception,):
     __version__ = 'unknown'
 
@@ -419,14 +419,15 @@
     # TODO: more numpy.ndarray methods as needed
     # TODO: imread.std
     # TODO: metadata in OME format tree
 
     priority = 99
     do_not_pickle = 'base', 'copies', 'cache'
     do_not_copy = 'extrametadata'
+    do_copy = 'ome'
     ureg = ureg
 
     @staticmethod
     @abstractmethod
     def _can_open(path):  # Override this method, and return true when the subclass can open the file
         return False
 
@@ -468,14 +469,19 @@
                 subclass.do_not_pickle = set(do_not_pickle).union(set(subclass_do_not_pickle))
 
                 do_not_copy = (cls.do_not_copy,) if isinstance(cls.do_not_copy, str) else cls.do_not_copy
                 subclass_do_not_copy = (subclass.do_not_copy,) if isinstance(subclass.do_not_copy, str) \
                     else subclass.do_not_copy if hasattr(subclass, 'do_not_copy') else ()
                 subclass.do_not_copy = set(do_not_copy).union(set(subclass_do_not_copy))
 
+                do_copy = (cls.do_copy,) if isinstance(cls.do_copy, str) else cls.do_copy
+                subclass_do_copy = (subclass.do_copy,) if isinstance(subclass.do_copy, str) \
+                    else subclass.do_copy if hasattr(subclass, 'do_copy') else ()
+                subclass.do_copy = set(do_copy).union(set(subclass_do_copy))
+
                 return super().__new__(subclass)
 
     @staticmethod
     def split_path_series(path):
         if isinstance(path, str):
             path = Path(path)
         if isinstance(path, Path) and path.name.startswith('Pos'):
@@ -515,39 +521,50 @@
         self.cache = DequeDict(16)
         self._frame_decorator = None
         self.frameoffset = 0, 0  # how far apart the centers of frame and sensor are
 
         self.open()
 
         # extract some metadata from ome
-        instrument = self.ome.instruments[0]
+        instrument = self.ome.instruments[0] if self.ome.instruments else None
         image = self.ome.images[0]
         pixels = image.pixels
         self.shape = pixels.size_x, pixels.size_y, pixels.size_c, pixels.size_z, pixels.size_t
         self.pxsize = pixels.physical_size_x_quantity
-        self.exposuretime = tuple(find(image.pixels.planes, the_c=c).exposure_time_quantity
-                                  for c in range(self.shape['c']))
+        try:
+            self.exposuretime = tuple(find(image.pixels.planes, the_c=c).exposure_time_quantity
+                                      for c in range(self.shape['c']))
+        except AttributeError:
+            self.exposuretime = ()
+
         if self.zstack:
             self.deltaz = image.pixels.physical_size_z_quantity
             self.deltaz_um = None if self.deltaz is None else self.deltaz.to(self.ureg.um).m
         else:
             self.deltaz = self.deltaz_um = None
         if self.ome.images[0].objective_settings:
             self.objective = find(instrument.objectives, id=self.ome.images[0].objective_settings.id)
         else:
             self.objective = None
-        self.timeval = [find(image.pixels.planes, the_c=0, the_t=t, the_z=0).delta_t for t in range(self.shape['t'])]
-        self.timeinterval = np.diff(self.timeval).mean() if len(self.timeval) > 1 else 0
+        try:
+            t0 = find(image.pixels.planes, the_c=0, the_t=0, the_z=0).delta_t
+            t1 = find(image.pixels.planes, the_c=0, the_t=self.shape['t'] - 1, the_z=0).delta_t
+            self.timeinterval = (t1 - t0) / (self.shape['t'] - 1) if self.shape['t'] > 1 else None
+        except AttributeError:
+            self.timeinterval = None
         try:
             self.binning = [int(i) for i in image.pixels.channels[0].detector_settings.binning.value.split('x')]
             self.pxsize *= self.binning[0]
-        except (Exception,):
+        except (AttributeError, IndexError):
             self.binning = None
         self.cnamelist = [channel.name for channel in image.pixels.channels]
-        optovars = [objective for objective in instrument.objectives if 'tubelens' in objective.id.lower()]
+        try:
+            optovars = [objective for objective in instrument.objectives if 'tubelens' in objective.id.lower()]
+        except AttributeError:
+            optovars = []
         if len(optovars) == 0:
             self.tubelens = None
         else:
             self.tubelens = optovars[0]
         if self.objective:
             if self.tubelens:
                 self.magnification = self.objective.nominal_magnification * self.tubelens.nominal_magnification
@@ -558,18 +575,18 @@
             self.magnification = None
             self.NA = None
 
         self.gain = [find(instrument.detectors, id=channel.detector_settings.id).amplification_gain
                      for channel in image.pixels.channels
                      if channel.detector_settings
                      and find(instrument.detectors, id=channel.detector_settings.id).amplification_gain]
-        self.laserwavelengths = [(channel.emission_wavelength_quantity.to(self.ureg.nm).m,)
-                                 for channel in pixels.channels if channel.emission_wavelength_quantity]
-        self.laserpowers = try_default(lambda channel: [(1 - channel.light_source_settings.attenuation,)
-                                                        for channel in pixels.channels], [])
+        self.laserwavelengths = [(channel.excitation_wavelength_quantity.to(self.ureg.nm).m,)
+                                 for channel in pixels.channels if channel.excitation_wavelength_quantity]
+        self.laserpowers = try_default(lambda: [(1 - channel.light_source_settings.attenuation,)
+                                                for channel in pixels.channels], [])
         self.filter = try_default(lambda: [find(instrument.filter_sets, id=channel.filter_set_ref.id).model
                                            for channel in image.pixels.channels], None)
         self.pxsize_um = None if self.pxsize is None else self.pxsize.to(self.ureg.um).m
         self.exposuretime_s = [None if i is None else i.to(self.ureg.s).m for i in self.exposuretime]
         self.file_shape = self.shape.xyczt
 
         if axes is None:
@@ -602,15 +619,15 @@
         try:
             s = int(re.findall(r'_(\d{3})_', self.duolink)[0]) * ureg.nm
         except (Exception,):
             s = 561 * ureg.nm
         try:
             sigma = []
             for c, d in enumerate(self.detector):
-                emission = np.hstack(self.laserwavelengths[c]) + 22 * ureg.nm
+                emission = (np.hstack(self.laserwavelengths[c]) + 22) * ureg.nm
                 sigma.append([emission[emission > s].max(initial=0), emission[emission < s].max(initial=0)][d])
             sigma = np.hstack(sigma)
             sigma[sigma == 0] = 600 * ureg.nm
             sigma /= 2 * self.NA * self.pxsize
             self.sigma = sigma.magnitude.tolist()
         except (Exception,):
             self.sigma = [2] * self.shape['c']
@@ -693,21 +710,22 @@
         self._frame_decorator = decorator
         self.cache = DequeDict(self.cache.maxlen)
 
     @property
     def summary(self):
         """ gives a helpful summary of the recorded experiment """
         s = [f"path/filename: {self.path}",
+             f"series/pos:    {self.series}",
              f"reader:        {self.__class__.__module__.split('.')[-1]}",
              f"shape ({self.axes}):".ljust(15) + f"{' x '.join(str(i) for i in self.shape)}"]
         if self.pxsize_um:
             s.append(f'pixel size:    {1000 * self.pxsize_um:.2f} nm')
         if self.zstack and self.deltaz_um:
             s.append(f'z-interval:    {1000 * self.deltaz_um:.2f} nm')
-        if self.exposuretime_s[0]:
+        if self.exposuretime_s:
             s.append(f'exposuretime:  {self.exposuretime_s[0]:.2f} s')
         if self.timeseries and self.timeinterval:
             s.append(f'time interval: {self.timeinterval:.3f} s')
         if self.binning:
             s.append('binning:       {}x{}'.format(*self.binning))
         if self.laserwavelengths:
             s.append('laser colors:  ' + ' | '.join([' & '.join(len(w)*('{:.0f}',)).format(*w)
@@ -743,14 +761,16 @@
 
     def __call__(self, c=None, z=None, t=None, x=None, y=None):
         """ same as im[] but allowing keyword axes, but slices need to made with slice() or np.s_ """
         return self[{k: slice(v) if v is None else v for k, v in dict(c=c, z=z, t=t, x=x, y=y).items()}]
 
     def __getitem__(self, n):
         """ slice like a numpy array but return an Imread instance """
+        if self.isclosed:
+            raise IOError("file is closed")
         if isinstance(n, (slice, Number)):  # None = :
             n = (n,)
         elif isinstance(n, type(Ellipsis)):
             n = (None,) * len(self.axes)
         elif isinstance(n, dict):  # allow im[dict(z=0)] etc.
             n = [n.get(i, slice(None)) for i in self.axes]
         n = list(n)
@@ -866,15 +886,15 @@
         return self.copy()
 
     def copy(self):
         new = Imread.__new__(self.__class__)
         new.copies = []
         new.base = self
         for key, value in self.__dict__.items():
-            if key not in self.do_not_copy and not hasattr(new, key):
+            if key in self.do_copy or (key not in self.do_not_copy and not hasattr(new, key)):
                 new.__dict__[key] = value
         self.copies.append(new)
         return new
 
     @property
     def shape(self):
         return self._shape
```

### Comparing `ndbioimage-2023.7.0/ndbioimage/bf.py` & `ndbioimage-2023.7.2/ndbioimage/bf.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/jvm.py` & `ndbioimage-2023.7.2/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/ntransforms.py` & `ndbioimage-2023.7.2/ndbioimage/ntransforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/readers/bfread.py` & `ndbioimage-2023.7.2/ndbioimage/readers/bfread.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 class JVMReader:
     def __init__(self, path, series):
         bf_jar = Path(__file__).parent.parent / 'jars' / 'bioformats_package.jar'
         if not bf_jar.exists():
             print('Downloading bioformats_package.jar.')
             url = 'https://downloads.openmicroscopy.org/bio-formats/latest/artifacts/bioformats_package.jar'
+            bf_jar.parent.mkdir(exist_ok=True)
             bf_jar.write_bytes(request.urlopen(url).read())
 
         mp = multiprocessing.get_context('spawn')
         self.path = path
         self.series = series
         self.queue_in = mp.Queue()
         self.queue_out = mp.Queue()
```

### Comparing `ndbioimage-2023.7.0/ndbioimage/readers/cziread.py` & `ndbioimage-2023.7.2/ndbioimage/readers/cziread.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,31 +356,33 @@
                 binning = model.simple_types.Binning.OTHER
 
             filterset = text(channels_ts[key].find("BeamSplitters")[0].find("Filter"))
             filterset_idx = [filterset.model for filterset in ome.instruments[0].filter_sets].index(filterset)
 
             light_sources_settings = channel.find("LightSourcesSettings")
             # no space in ome for multiple lightsources simultaneously
-            light_source_settings = light_sources_settings[0]
+            if len(light_sources_settings) > idx:
+                light_source_settings = light_sources_settings[idx]
+            else:
+                light_source_settings = light_sources_settings[0]
             light_source_settings = model.LightSourceSettings(
-                id="_".join([light_source_settings.find("LightSource").attrib["Id"]
-                             for light_source_settings in light_sources_settings]),
+                id=light_source_settings.find("LightSource").attrib["Id"],
                 attenuation=float(text(light_source_settings.find("Attenuation"))),
                 wavelength=float(text(light_source_settings.find("Wavelength"))),
                 wavelength_unit=nm)
 
             ome.images[0].pixels.channels.append(
                 model.Channel(
                     id=f"Channel:0:{idx}",
                     name=channel.attrib["Name"],
                     acquisition_mode=text(channel.find("AcquisitionMode")),
                     color=model.simple_types.Color(text(channels_ds[channel.attrib["Id"]].find("Color"))),
                     detector_settings=model.DetectorSettings(id=detector.attrib["Id"], binning=binning),
                     emission_wavelength=text(channel.find("EmissionWavelength")),
-                    excitation_wavelength=text(channel.find("ExcitationWavelength")),
+                    excitation_wavelength=light_source_settings.wavelength,
                     filter_set_ref=model.FilterSetRef(id=ome.instruments[0].filter_sets[filterset_idx].id),
                     illumination_type=text(channel.find("IlluminationType")),
                     light_source_settings=light_source_settings,
                     samples_per_pixel=int(text(laser_scan_info.find("Averaging")))))
 
         exposure_times = [float(text(channel.find("LaserScanInfo").find("FrameTime"))) for channel in
                           channels_im.values()]
```

### Comparing `ndbioimage-2023.7.0/ndbioimage/readers/ndread.py` & `ndbioimage-2023.7.2/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/readers/seqread.py` & `ndbioimage-2023.7.2/ndbioimage/readers/seqread.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,43 @@
 import tifffile
 import yaml
 import re
 from ndbioimage import Imread
 from pathlib import Path
 from functools import cached_property
 from ome_types import model
+from ome_types._base_type import quantity_property
 from itertools import product
 from datetime import datetime
 from abc import ABC
-from parfor import pmap
+
+
+def lazy_property(function, field, *arg_fields):
+    def lazy(self):
+        if self.__dict__.get(field) is None:
+            self.__dict__[field] = function(*[getattr(self, arg_field) for arg_field in arg_fields])
+            self.__fields_set__.add(field)
+        return self.__dict__[field]
+    return property(lazy)
+
+
+class Plane(model.Plane):
+    """ Lazily retrieve delta_t from metadata """
+    def __init__(self, t0, file, **kwargs):
+        super().__init__(**kwargs)
+        setattr(self.__class__, 'delta_t', lazy_property(self.get_delta_t, 'delta_t', 't0', 'file'))
+        setattr(self.__class__, 'delta_t_quantity', quantity_property('delta_t'))
+        self.__dict__['t0'] = t0
+        self.__dict__['file'] = file
+
+    @staticmethod
+    def get_delta_t(t0, file):
+        with tifffile.TiffFile(file) as tif:
+            info = yaml.safe_load(tif.pages[0].tags[50839].value['Info'])
+        return float((datetime.strptime(info["Time"], "%Y-%m-%d %H:%M:%S %z") - t0).seconds)
 
 
 class Reader(Imread, ABC):
     priority = 10
 
     @staticmethod
     def _can_open(path):
@@ -61,27 +86,18 @@
                 pixels=model.Pixels(
                     size_c=size_c, size_z=size_z, size_t=size_t,
                     size_x=metadata['Info']['Width'], size_y=metadata['Info']['Height'],
                     dimension_order="XYCZT", type=pixel_type, physical_size_x=pxsize, physical_size_y=pxsize,
                     physical_size_z=metadata["Info"]["Summary"]["z-step_um"]),
                 objective_settings=model.ObjectiveSettings(id="Objective:0")))
 
-        def timeval_fun(i):
-            with tifffile.TiffFile(self.filedict[i]) as tif:
-                info = yaml.safe_load(tif.pages[0].tags[50839].value['Info'])
-            return (datetime.strptime(info["Time"], "%Y-%m-%d %H:%M:%S %z") - t0).seconds
-
-        length = size_c * size_z * size_t
-        timeval = pmap(timeval_fun, product(range(size_c), range(size_z), range(size_t)), length=length,
-                       serial=length <= 24, desc='Reading metadata')
-
-        for (c, z, t), time in zip(product(range(size_c), range(size_z), range(size_t)), timeval):
+        for c, z, t in product(range(size_c), range(size_z), range(size_t)):
             ome.images[0].pixels.planes.append(
-                model.Plane(
-                    the_c=c, the_z=z, the_t=t, exposure_time=metadata["Info"]["Exposure-ms"] / 1000, delta_t=time))
+                Plane(t0, self.filedict[c, z, t],
+                      the_c=c, the_z=z, the_t=t, exposure_time=metadata["Info"]["Exposure-ms"] / 1000))
 
         # compare channel names from metadata with filenames
         pattern_c = re.compile(r"img_\d{3,}_(.*)_\d{3,}$")
         for c in range(size_c):
             ome.images[0].pixels.channels.append(
                 model.Channel(
                     id=f"Channel:{c}", name=pattern_c.findall(self.filedict[c, 0, 0].stem)[0],
```

### Comparing `ndbioimage-2023.7.0/ndbioimage/readers/tifread.py` & `ndbioimage-2023.7.2/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/ndbioimage/transforms.py` & `ndbioimage-2023.7.2/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.0/pyproject.toml` & `ndbioimage-2023.7.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2023.7.0"
+version = "2023.7.2"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
+exclude = [ "ndbioimage/jars" ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "*"
 pandas = "*"
 tifffile = "*"
 czifile = "*"
```

### Comparing `ndbioimage-2023.7.0/PKG-INFO` & `ndbioimage-2023.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2023.7.0
+Version: 2023.7.2
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.8,<4.0
```

