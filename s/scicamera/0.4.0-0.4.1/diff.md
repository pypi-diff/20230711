# Comparing `tmp/scicamera-0.4.0.tar.gz` & `tmp/scicamera-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicamera-0.4.0.tar", max compression
+gzip compressed data, was "scicamera-0.4.1.tar", max compression
```

## Comparing `scicamera-0.4.0.tar` & `scicamera-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0     1357 2023-01-17 22:18:43.688190 scicamera-0.4.0/LICENSE
--rw-r--r--   0        0        0     2529 2023-02-23 21:36:17.369022 scicamera-0.4.0/README.md
--rw-r--r--   0        0        0      590 2023-03-14 22:51:41.672768 scicamera-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      883 2023-03-01 21:17:58.386381 scicamera-0.4.0/scicamera/__init__.py
--rw-r--r--   0        0        0    10276 2023-03-14 22:50:53.425531 scicamera-0.4.0/scicamera/actions.py
--rw-r--r--   0        0        0    17021 2023-03-14 22:50:53.425531 scicamera-0.4.0/scicamera/camera.py
--rw-r--r--   0        0        0    16598 2023-03-14 22:50:53.429531 scicamera-0.4.0/scicamera/configuration.py
--rw-r--r--   0        0        0     2448 2023-03-07 22:57:12.840313 scicamera-0.4.0/scicamera/controls.py
--rw-r--r--   0        0        0     1154 2023-01-17 22:18:43.688190 scicamera-0.4.0/scicamera/converters.py
--rw-r--r--   0        0        0     5354 2023-03-14 22:50:53.429531 scicamera-0.4.0/scicamera/fake.py
--rw-r--r--   0        0        0     1216 2023-01-17 22:18:43.688190 scicamera-0.4.0/scicamera/formats.py
--rw-r--r--   0        0        0      715 2023-03-01 22:35:46.346525 scicamera-0.4.0/scicamera/frame.py
--rw-r--r--   0        0        0     2339 2023-03-14 22:50:53.429531 scicamera-0.4.0/scicamera/info.py
--rw-r--r--   0        0        0     1955 2023-03-14 22:50:53.429531 scicamera-0.4.0/scicamera/lc_helpers.py
--rw-r--r--   0        0        0     1868 2023-02-23 23:01:21.941733 scicamera-0.4.0/scicamera/preview.py
--rw-r--r--   0        0        0     7255 2023-03-14 22:50:53.429531 scicamera-0.4.0/scicamera/request.py
--rw-r--r--   0        0        0     1231 2023-01-17 22:18:43.688190 scicamera-0.4.0/scicamera/sensor_format.py
--rw-r--r--   0        0        0     1623 2023-03-14 22:50:53.429531 scicamera-0.4.0/scicamera/testing.py
--rw-r--r--   0        0        0     1351 2023-03-01 21:17:58.438380 scicamera-0.4.0/scicamera/timing.py
--rw-r--r--   0        0        0     2348 2023-01-17 22:18:43.688190 scicamera-0.4.0/scicamera/tuning.py
--rw-r--r--   0        0        0      896 2023-01-17 22:18:43.688190 scicamera-0.4.0/scicamera/typing.py
--rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 scicamera-0.4.0/setup.py
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 scicamera-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1357 2023-01-20 16:48:50.353808 scicamera-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2529 2023-02-27 23:05:02.464247 scicamera-0.4.1/README.md
+-rw-r--r--   0        0        0      590 2023-07-11 03:29:25.303711 scicamera-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      951 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/__init__.py
+-rw-r--r--   0        0        0    11730 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/actions.py
+-rw-r--r--   0        0        0    16759 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/camera.py
+-rw-r--r--   0        0        0    16574 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/configuration.py
+-rw-r--r--   0        0        0     2448 2023-07-08 06:14:33.432342 scicamera-0.4.1/scicamera/controls.py
+-rw-r--r--   0        0        0     1154 2023-01-20 16:48:50.353808 scicamera-0.4.1/scicamera/converters.py
+-rw-r--r--   0        0        0     5354 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/fake.py
+-rw-r--r--   0        0        0     6112 2023-07-11 03:27:28.103968 scicamera-0.4.1/scicamera/formats.py
+-rw-r--r--   0        0        0      715 2023-07-08 06:14:33.432342 scicamera-0.4.1/scicamera/frame.py
+-rw-r--r--   0        0        0     2339 2023-07-08 06:14:33.432342 scicamera-0.4.1/scicamera/info.py
+-rw-r--r--   0        0        0     2457 2023-07-08 06:54:24.762673 scicamera-0.4.1/scicamera/lc_helpers.py
+-rw-r--r--   0        0        0     7363 2023-07-08 06:14:33.436342 scicamera-0.4.1/scicamera/request.py
+-rw-r--r--   0        0        0     1231 2023-01-20 16:48:50.353808 scicamera-0.4.1/scicamera/sensor_format.py
+-rw-r--r--   0        0        0     1623 2023-07-08 06:14:33.436342 scicamera-0.4.1/scicamera/testing.py
+-rw-r--r--   0        0        0     1356 2023-07-10 04:24:06.046815 scicamera-0.4.1/scicamera/timing.py
+-rw-r--r--   0        0        0     2348 2023-01-20 16:48:50.353808 scicamera-0.4.1/scicamera/tuning.py
+-rw-r--r--   0        0        0      896 2023-01-20 16:48:50.353808 scicamera-0.4.1/scicamera/typing.py
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 scicamera-0.4.1/PKG-INFO
```

### Comparing `scicamera-0.4.0/LICENSE` & `scicamera-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/README.md` & `scicamera-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/pyproject.toml` & `scicamera-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "scicamera"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 readme="README.md"
 authors = ["Exclosure <info@exclosure.io>"]
 repository = "https://github.com/exclosure/scicamera"
 keywords = ["camera", "imaging", "RaspberryPi"]
 license="BSD"
```

### Comparing `scicamera-0.4.0/scicamera/actions.py` & `scicamera-0.4.1/scicamera/actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
 from collections import deque
 from concurrent.futures import Future
 from logging import getLogger
+from threading import Condition, Event, Thread
 from typing import Any, Callable, Deque, Dict, List, Optional, Tuple
 
 import numpy as np
 from PIL import Image
 
 from scicamera.configuration import CameraConfig
 from scicamera.frame import CameraFrame
@@ -15,18 +16,24 @@
 _log = getLogger(__name__)
 
 
 class RequestMachinery(ABC):
     """RequestMachinery is a helper class for the Camera class."""
 
     def __init__(self) -> None:
-        self._requests = deque()
-        self._request_callbacks = []
+        self._requests: Deque[CompletedRequest] = deque()
+        self._request_callbacks: List[Callable[[CompletedRequest], None]] = []
         self._task_deque: Deque[LoopTask] = deque()
 
+        self._runloop_cond = Condition()
+        self._runloop_abort = Event()
+        self._runloop_thread = Thread(target=lambda: 0, daemon=True)
+        self._runloop_thread.start()
+        self._runloop_thread.join()
+
     @abstractmethod
     def close(self):
         raise NotImplementedError()
 
     def __enter__(self):
         return self
 
@@ -51,14 +58,52 @@
         :type callback: Callable[[CompletedRequest], None]
         """
         self._request_callbacks.remove(callback)
 
     def add_completed_request(self, request: CompletedRequest) -> None:
         self._requests.append(request)
 
+        with self._runloop_cond:
+            self._runloop_cond.notify()
+
+    def _runloop(self) -> None:
+        while True:
+            with self._runloop_cond:
+                self._runloop_cond.wait(timeout=0.05)
+
+            if self._runloop_abort.is_set():
+                break
+
+            if len(self._requests) > 0:
+                self.process_requests()
+
+    def start_runloop(self) -> None:
+        """
+        Start the preview loop.
+        """
+        if self._runloop_thread.is_alive():
+            raise RuntimeError("Runloop thread already running?")
+
+        self._runloop_abort.clear()
+        self._runloop_thread = Thread(target=self._runloop, daemon=True)
+        self._runloop_thread.start()
+
+    def is_runloop_running(self):
+        return self._runloop_thread.is_alive()
+
+    def stop_runloop(self) -> None:
+        """Stop preview
+
+        :raises RuntimeError: Unable to stop preview
+        """
+        self._runloop_abort.set()
+        with self._runloop_cond:
+            self._runloop_cond.notify()
+        self._runloop_thread.join()
+
     def has_requests(self) -> bool:
         return len(self._requests) > 0
 
     def process_requests(self) -> None:
         # Safe copy and pop off all requests
         requests = list(self._requests)
         for _ in requests:
@@ -137,15 +182,15 @@
     def switch_mode(self, camera_config: CameraConfig) -> TypedFuture[CameraConfig]:
         """Switch the camera into another mode given by the camera_config."""
         return self._dispatch_loop_tasks(
             LoopTask.without_request(self._switch_mode, camera_config)
         )[0]
 
     def _capture_file(
-        self, name, file_output, format, request: CompletedRequest
+        self, name: str, file_output, format, request: CompletedRequest
     ) -> dict:
         request.make_image(name).convert("RGB").save(file_output, format=format)
         return request.get_metadata()
 
     def capture_file(
         self, file_output, name: str = "main", format=None, config=None
     ) -> TypedFuture[dict]:
@@ -197,32 +242,32 @@
     ) -> TypedFuture[Tuple[List[np.ndarray], dict]]:
         """Make a 1d numpy array from the next frame for each of the named streams."""
         return self._dispatch_loop_tasks(
             LoopTask.with_request(self._capture_buffers_and_metadata, names)
         )[0]
 
     # Array Capture Methods
-    def _capture_array(self, name, request: CompletedRequest):
+    def _capture_array(self, name: str, request: CompletedRequest):
         return request.make_array(name)
 
     def capture_array(
-        self, name="main", config: Optional[dict] = None
+        self, name: str = "main", config: Optional[dict] = None
     ) -> Future[np.ndarray]:
         """Make a 2d image from the next frame in the named stream."""
         return self._dispatch_loop_tasks(
             LoopTask.with_request(self._capture_array, name), config=config
         )[0]
 
     def _capture_arrays_and_metadata(
-        self, names, request: CompletedRequest
+        self, names: List[str], request: CompletedRequest
     ) -> Tuple[List[np.ndarray], Dict[str, Any]]:
         return ([request.make_array(name) for name in names], request.get_metadata())
 
     def capture_arrays_and_metadata(
-        self, names=["main"]
+        self, names: List[str] = ["main"]
     ) -> TypedFuture[Tuple[List[np.ndarray], Dict[str, Any]]]:
         """Make 2d image arrays from the next frames in the named streams."""
         return self._dispatch_loop_tasks(
             LoopTask.with_request(self._capture_arrays_and_metadata, names)
         )[0]
 
     def _capture_image(self, name: str, request: CompletedRequest) -> Image.Image:
@@ -259,13 +304,13 @@
         :type name: str, optional
         """
         return self._dispatch_loop_tasks(
             LoopTask.with_request(self._capture_frame, name), config=config
         )[0]
 
     def capture_serial_frames(
-        self, n_frames: int, name="main"
+        self, n_frames: int, name: str = "main"
     ) -> List[TypedFuture[CameraFrame]]:
         """Capture a number of frames from the named stream, returning a list of CameraFrames."""
         return self._dispatch_loop_tasks(
             *(LoopTask.with_request(self._capture_frame, name) for _ in range(n_frames))
         )
```

### Comparing `scicamera-0.4.0/scicamera/camera.py` & `scicamera-0.4.1/scicamera/camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 import libcamera
 
 import scicamera.formats as formats
 from scicamera.actions import RequestMachinery
 from scicamera.configuration import CameraConfig
 from scicamera.controls import Controls
 from scicamera.info import CameraInfo
-from scicamera.lc_helpers import errno_handle, lc_unpack, lc_unpack_controls
-from scicamera.preview import NullPreview
+from scicamera.lc_helpers import (
+    errno_handle,
+    lc_return_code_helper,
+    lc_unpack,
+    lc_unpack_controls,
+)
 from scicamera.request import CompletedRequest, LoopTask
 from scicamera.sensor_format import SensorFormat
 from scicamera.tuning import TuningContext
 
 _log = logging.getLogger(__name__)
 
 
@@ -142,15 +146,14 @@
         with TuningContext(tuning):
             self._open_camera()
 
     def _reset_flags(self) -> None:
         self.camera = None
         self.is_open = False
         self.camera_ctrl_info = {}
-        self._preview = None
         self.camera_config = None
         self.streams = None
         self.stream_map = None
         self.started = False
         self.stop_count = 0
         self.camera_properties_ = {}
         self.controls = Controls(self)
@@ -202,19 +205,23 @@
 
         self.__identify_camera()
         self.camera_ctrl_info = lc_unpack_controls(self.camera.controls)
         self.camera_properties_ = lc_unpack(self.camera.properties)
 
         # The next two lines could be placed elsewhere?
         self.sensor_resolution = self.camera_properties_["PixelArraySize"]
-        self.sensor_format = str(
-            self.camera.generate_configuration([libcamera.StreamRole.Raw])
-            .at(0)
-            .pixel_format
-        )
+
+        # Poke through the various available raw-formats
+        formats: Dict[int, str] = {}
+        configs = self.camera.generate_configuration([libcamera.StreamRole.Raw])
+        for i in range(configs.size):
+            formats[i] = str(configs.at(i).pixel_format)
+
+        self.sensor_format = formats[0]
+        _log.warning("Available sensor raw formats: %s", list(formats.values()))
 
         _log.info("Initialization successful.")
 
     def __identify_camera(self):
         # TODO(meawoppl) make this a helper on the camera_manager
         for idx, address in enumerate(self._cm.cms.cameras):
             if address == self.camera:
@@ -224,16 +231,16 @@
     def _open_camera(self) -> None:
         """Tries to open camera
 
         :raises RuntimeError: Failed to setup camera
         """
         self._initialize_camera()
 
-        acq_code = self.camera.acquire()
-        errno_handle(acq_code, "camera.acquire()")
+        return_code = self.camera.acquire()
+        lc_return_code_helper(return_code, "camera.acquire()")
 
         self.is_open = True
         _log.info("Camera now open.")
 
     @property
     def sensor_modes(self) -> list:
         """The available sensor modes
@@ -271,46 +278,27 @@
                 cam_mode["crop_limits"] = self.camera_properties["ScalerCropMaximum"]
                 cam_mode["exposure_limits"] = tuple(
                     [i for i in self.camera_controls["ExposureTime"] if i != 0]
                 )
                 self.sensor_modes_.append(cam_mode)
         return self.sensor_modes_
 
-    # TODO(meawoppl) we don't really support previews, so change the language here
-    def start_preview(self) -> None:
-        """
-        Start the preview loop.
-        """
-        if self._preview:
-            raise RuntimeError("An event loop is already running")
-
-        preview = NullPreview()
-        preview.start(self)
-        self._preview = preview
-
-    def stop_preview(self) -> None:
-        """Stop preview the preview thread"""
-        if not self._preview:
-            return
-
-        self._preview.stop()
-        self._preview = None
-
     def close(self) -> None:
         """Close camera
 
         :raises RuntimeError: Closing failed
         """
-        self.stop_preview()
+        if self.is_runloop_running():
+            self.stop_runloop()
         if not self.is_open:
             return
 
         self.stop()
-        code = self.camera.release()
-        errno_handle(code, "camera.release()")
+        release_code = self.camera.release()
+        lc_return_code_helper(release_code, "camera.release()")
 
         self._cm.cleanup(self.camera_idx)
         self.is_open = False
         self.streams = None
         self.stream_map = None
         self.camera = None
         self.camera_ctrl_info = None
@@ -426,29 +414,25 @@
         # Set the controls directly so as to overwrite whatever is there.
         self.controls.set_controls(self.camera_config.controls)
 
     def camera_configuration(self) -> CameraConfig:
         """Return the camera configuration."""
         return self.camera_config
 
-    def stream_configuration(self, name="main") -> dict:
-        """Return the stream configuration for the named stream."""
-        return self.camera_config[name]
-
     def _start(self) -> None:
         """Start the camera system running."""
         if self.camera_config is None:
             raise RuntimeError("Camera has not been configured")
         if self.started:
             raise RuntimeError("Camera already started")
         controls = self.controls.get_libcamera_controls()
         self.controls = Controls(self)
 
-        code = self.camera.start(controls)
-        errno_handle(code, "camera.start()")
+        return_code = self.camera.start(controls)
+        lc_return_code_helper(return_code, "camera.start()")
 
         for request in self._make_requests():
             self.camera.queue_request(request)
         self.started = True
         _log.info("Camera started")
 
     def start(self) -> None:
@@ -457,28 +441,28 @@
         """
         if self.camera_config is None:
             _log.warning("Camera has not been configured, using preview config")
             self.configure(CameraConfig.for_preview(self))
         if self.camera_config is None:
             raise RuntimeError("Camera has not been configured")
         # By default we will create an event loop is there isn't one running already.
-        if not self._preview:
-            self.start_preview()
+        if not self.is_runloop_running():
+            self.start_runloop()
         self._start()
 
     def _stop(self) -> None:
         """Stop the camera.
 
         Only call this function directly from within the camera event
         loop, such as in a Qt application.
         """
         if self.started:
             self.stop_count += 1
-            code = self.camera.stop()
-            errno_handle(code, "camera.stop()")
+            return_code = self.camera.stop()
+            lc_return_code_helper(return_code, "camera.stop()")
 
             # Flush Requests from the event queue.
             # This is needed to prevent old completed Requests from showing
             # up when the camera is started the next time.
             n_flushed = self._cm.handle_request(self.camera_idx)
             self.started = False
             _log.warning("Flushed %s requests", n_flushed)
@@ -486,13 +470,15 @@
             _log.info("Camera stopped")
 
     def stop(self) -> None:
         """Stop the camera."""
         if not self.started:
             _log.debug("Camera was not started")
             return
-        self.stop_preview()
-        self._stop()
+        if self.is_runloop_running():
+            self._dispatch_loop_tasks(LoopTask.without_request(self._stop))[0].result()
+        else:
+            self._stop()
 
     def set_controls(self, controls) -> None:
         """Set camera controls. These will be delivered with the next request that gets submitted."""
         self.controls.set_controls(controls)
```

### Comparing `scicamera-0.4.0/scicamera/configuration.py` & `scicamera-0.4.1/scicamera/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,36 +142,35 @@
     def enable_raw(self, enable: bool = True) -> None:
         self.raw = (
             StreamConfig(size=self.main.size, format=self.camera.sensor_format)
             if enable
             else None
         )
 
-    def align(self, optimal=True):
+    def align(self, optimal: bool = True):
         self.main.align(optimal)
         if self.lores is not None:
             self.lores.align(optimal)
         # No sense trying to align the raw stream.
 
     def get_stream_indices(self) -> Tuple[int, int, int]:
         """Get the main, lores, and raw stream indices.
 
         These indices will be -1 if unset.
         """
         # Get the indices of the streams we want to use.
         index = 1
-        main_index = 0
         lores_index = -1
         raw_index = -1
         if self.lores is not None:
             lores_index = index
             index += 1
         if self.raw is not None:
             raw_index = index
-        return main_index, lores_index, raw_index
+        return 0, lores_index, raw_index
 
     def __post_init__(self) -> None:
         if isinstance(self.controls, dict):
             _log.warning("CameraConfiguration controls should be a Controls object")
             self.controls = Controls(self.camera, self.controls)
         if isinstance(self.main, dict):
             _log.warning("CameraConfiguration 'main' should be a StreamConfiguration")
```

### Comparing `scicamera-0.4.0/scicamera/controls.py` & `scicamera-0.4.1/scicamera/controls.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/scicamera/converters.py` & `scicamera-0.4.1/scicamera/converters.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/scicamera/fake.py` & `scicamera-0.4.1/scicamera/fake.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,18 @@
             rotation=1,
         )
 
     @property
     def camera_controls(self):
         return {}
 
-    def start_preview(self):
+    def start_runloop(self):
         pass
 
-    def stop_preview(self):
+    def stop_runloop(self):
         pass
 
     def start(self) -> None:
         self._t = Thread(target=self._run, daemon=True)
         self._abort.clear()
         self._t.start()
```

### Comparing `scicamera-0.4.0/scicamera/frame.py` & `scicamera-0.4.1/scicamera/frame.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/scicamera/info.py` & `scicamera-0.4.1/scicamera/info.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/scicamera/lc_helpers.py` & `scicamera-0.4.1/scicamera/lc_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,7 +64,19 @@
     """Return ``True`` if the two color spaces are equivalent."""
     return (
         c1.primaries == c2.primaries
         and c1.transferFunction == c2.transferFunction
         and c1.ycbcrEncoding == c2.ycbcrEncoding
         and c1.range == c2.range
     )
+
+
+def lc_return_code_helper(return_code: int, method: str) -> None:
+    """Decode and process a libcamera return code.
+
+    These are generally encoded as negative numbers which map to
+    errno values. This function raises a RuntimeError if the return
+    code is negative, and tries to make the result more ledgible.
+    """
+    if return_code < 0:
+        error_name = errno.errorcode.get(-return_code, "No Errno")
+        raise RuntimeError(f"Error calling {method}: {return_code} ({error_name})")
```

### Comparing `scicamera-0.4.0/scicamera/request.py` & `scicamera-0.4.1/scicamera/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
 import numpy as np
 from PIL import Image
 
 import scicamera.formats as formats
 from scicamera import formats
 from scicamera.configuration import CameraConfig
+from scicamera.formats import unpack_raw
 from scicamera.lc_helpers import lc_unpack
+from scicamera.sensor_format import SensorFormat
 
 _log = getLogger(__name__)
 
 
 class MappedBuffer:
     def __init__(self, lc_buffer):
         self.__fb = lc_buffer
@@ -94,15 +96,15 @@
         elif fmt in ("YUYV", "YVYU", "UYVY", "VYUY"):
             # These dimensions seem a bit strange, but mean that
             # cv2.cvtColor(image, cv2.COLOR_YUV2BGR_YUYV) will convert directly to RGB.
             image = array.reshape(h, stride // 2, 2)
         elif fmt == "MJPEG":
             image = np.array(Image.open(io.BytesIO(array)))
         elif formats.is_raw(fmt):
-            image = array.reshape((h, stride))
+            image = unpack_raw(array, (h, w), SensorFormat(fmt))
         else:
             raise RuntimeError("Format " + config.format + " not supported")
         return image
 
     def make_image(self, name: str) -> Image.Image:
         """Make a PIL image from the named stream's buffer."""
         fmt = self.get_camera_config().get_stream_config(name).format
```

### Comparing `scicamera-0.4.0/scicamera/sensor_format.py` & `scicamera-0.4.1/scicamera/sensor_format.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/scicamera/testing.py` & `scicamera-0.4.1/scicamera/testing.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/scicamera/timing.py` & `scicamera-0.4.1/scicamera/timing.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 
 from scicamera.camera import Camera
 from scicamera.request import CompletedRequest
 
 _log = getLogger(__name__)
 
 
-def calibrate_camera_offset(camera: Camera, n_frames: int = 100) -> int:
+def calibrate_camera_offset(
+    camera: Camera,
+    n_frames: int = 100,
+) -> float:
     """Calibrate the ``SensorTimestamp`` wrt to the epoch time.
 
-    Returns the number of integer nanoseconds you should add to
-    the camera ``SensorTimestamp`` to get the epoch time in nanoseconds.
+    Returns the number of nanoseconds you should add to the camera
+    ``SensorTimestamp`` to get the epoch time in nanoseconds.
     """
     deltas = []
 
     def _capture_timing_callback(request: CompletedRequest):
         # This is the time the request was handed to python
         epoch_nanos = int(request.completion_time * 1_000_000_000)
         # This is the time the "sensor" reports `ktime_get_ns()` in the kernel
@@ -28,9 +31,9 @@
     camera.remove_request_callback(_capture_timing_callback)
 
     # NB: This segment relies on python's integer size growth
     offset = sum(deltas) / len(deltas)
     diffs = sum([(d - offset) ** 2 for d in deltas])
     stdev = math.sqrt(diffs / (len(deltas) - 1))
 
-    _log.warning(f"Camera offset: {offset} +/-{stdev}")
+    _log.warning(f"Camera offset: {offset} ± {stdev}")
     return offset
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scicamera-0.4.0/scicamera/tuning.py` & `scicamera-0.4.1/scicamera/tuning.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/scicamera/typing.py` & `scicamera-0.4.1/scicamera/typing.py`

 * *Files identical despite different names*

### Comparing `scicamera-0.4.0/setup.py` & `scicamera-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,124 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: scicamera
+Version: 0.4.1
+Summary: 
+Home-page: https://github.com/exclosure/scicamera
+License: BSD
+Keywords: camera,imaging,RaspberryPi
+Author: Exclosure
+Author-email: info@exclosure.io
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pillow (>=9.3.0,<10.0.0)
+Project-URL: Repository, https://github.com/exclosure/scicamera
+Description-Content-Type: text/markdown
 
-packages = \
-['scicamera']
+# SciCamera
 
-package_data = \
-{'': ['*']}
+---
+Consistent and reliable imaging for scientific applications.
 
-install_requires = \
-['numpy>=1.23.5,<2.0.0', 'pillow>=9.3.0,<10.0.0']
-
-setup_kwargs = {
-    'name': 'scicamera',
-    'version': '0.4.0',
-    'description': '',
-    'long_description': '# SciCamera\n\n---\nConsistent and reliable imaging for scientific applications.\n\n\n## Why _SciCamera_?\n\nScientific imaging applications often require minimal post-processing pipelines, \nprecise capture timing, near-gapless sequential frames, and easily \nconfigurable settings like gain, resolution, bit-depth, and exposure \nlength. \n\nThis project, which began as fork of the webcam/video-focused [`picamera2`][picamera2]\nlibrary, aims to make it easy to configure and use cameras for scientific applications,\nwith a focus on _performance, reliability, code quality, and maintainability_.\n\n\n### Why not _SciCamera_?\n\nSciCamera currently focuses on high-quality, timing-sensitive, minimally-processed\n_still images_. For low-bandwidth, real-time image and video streaming, we recommend \nthe [`picamera2`][picamera2] library.\n\n\n## Platform support\n\n_SciCamera_ supports\n\n- Raspberry Pi OS (Bullseye or later), 64-bit.\n- x86 Ubuntu\n\nOther debian flavors are likely to be supported. We welcome pull requests to extend\nthe testing toolchains to cover your platform.\n\n## Installation\n\n_SciCamera_ is a pure python package, but relies on the python\nc++ wrapper of _libcamera_.\n\n_SciCamera_ can be installed simply with:\n```\npip install scicamera\n```\n\n### Installing libcamera + python bindings\n\nImport and use of the above pacakge requires that `libcamera` to be built\nwith the python package enabled. On rasbian, this is accomplished by \ninstalling the `libcamera` package from apt. In x86 it must be built \nusing something like the following:\n\n```bash\ngit clone https://github.com/Exclosure/libcamera.git\ncd libcamera\ngit checkout v0.0.4\nmeson setup build -D pycamera=enabled\nninja -C build\nsudo ninja -C build install\n```\n\n## Bugs/Contributing\n\n\nOpen an issue/PR to discuss your bug or feature. Once a course of action\nhas been identified, open a PR, discuss the changes. \n\nFeature creep is not of interest, but we would be happy\nto help you build your more complicated project on top of this.\n\nIf we like them, and the tests pass we will merge them. \nCI requires code has been processed `isort` and `black` toolchains.\n\nDoing this is pretty easy:\n```\nisort .\nblack .\n```\n\nGreat work.\n\n## Publishing to PYPI\n\nShould be added to github action later\n\n1. Add your pypi token\n  ```sh\n  $ poetry config pypi-token.pypi my-token\n  ```\n\n2. Cut a new tag\n  ```sh\n  $ git tag -a v0.1.0 -m "Version 0.1.0"\n  $ git push origin v0.1.0\n  ```\n\n3. Publish\n  ```sh\n  $ poetry publish --build\n  ```\n\n\n[picamera2]:https://github.com/raspberrypi/picamera2\n',
-    'author': 'Exclosure',
-    'author_email': 'info@exclosure.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/exclosure/scicamera',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
 
+## Why _SciCamera_?
+
+Scientific imaging applications often require minimal post-processing pipelines, 
+precise capture timing, near-gapless sequential frames, and easily 
+configurable settings like gain, resolution, bit-depth, and exposure 
+length. 
+
+This project, which began as fork of the webcam/video-focused [`picamera2`][picamera2]
+library, aims to make it easy to configure and use cameras for scientific applications,
+with a focus on _performance, reliability, code quality, and maintainability_.
+
+
+### Why not _SciCamera_?
+
+SciCamera currently focuses on high-quality, timing-sensitive, minimally-processed
+_still images_. For low-bandwidth, real-time image and video streaming, we recommend 
+the [`picamera2`][picamera2] library.
+
+
+## Platform support
+
+_SciCamera_ supports
+
+- Raspberry Pi OS (Bullseye or later), 64-bit.
+- x86 Ubuntu
+
+Other debian flavors are likely to be supported. We welcome pull requests to extend
+the testing toolchains to cover your platform.
+
+## Installation
+
+_SciCamera_ is a pure python package, but relies on the python
+c++ wrapper of _libcamera_.
+
+_SciCamera_ can be installed simply with:
+```
+pip install scicamera
+```
+
+### Installing libcamera + python bindings
+
+Import and use of the above pacakge requires that `libcamera` to be built
+with the python package enabled. On rasbian, this is accomplished by 
+installing the `libcamera` package from apt. In x86 it must be built 
+using something like the following:
+
+```bash
+git clone https://github.com/Exclosure/libcamera.git
+cd libcamera
+git checkout v0.0.4
+meson setup build -D pycamera=enabled
+ninja -C build
+sudo ninja -C build install
+```
+
+## Bugs/Contributing
+
+
+Open an issue/PR to discuss your bug or feature. Once a course of action
+has been identified, open a PR, discuss the changes. 
+
+Feature creep is not of interest, but we would be happy
+to help you build your more complicated project on top of this.
+
+If we like them, and the tests pass we will merge them. 
+CI requires code has been processed `isort` and `black` toolchains.
+
+Doing this is pretty easy:
+```
+isort .
+black .
+```
+
+Great work.
+
+## Publishing to PYPI
+
+Should be added to github action later
+
+1. Add your pypi token
+  ```sh
+  $ poetry config pypi-token.pypi my-token
+  ```
+
+2. Cut a new tag
+  ```sh
+  $ git tag -a v0.1.0 -m "Version 0.1.0"
+  $ git push origin v0.1.0
+  ```
+
+3. Publish
+  ```sh
+  $ poetry publish --build
+  ```
+
+
+[picamera2]:https://github.com/raspberrypi/picamera2
 
-setup(**setup_kwargs)
```

