# Comparing `tmp/miniature-lighting-desk-0.1.1.tar.gz` & `tmp/miniature_lighting_desk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniature-lighting-desk-0.1.1.tar", max compression
+gzip compressed data, was "miniature_lighting_desk-0.2.0.tar", max compression
```

## Comparing `miniature-lighting-desk-0.1.1.tar` & `miniature_lighting_desk-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1063 2021-12-27 10:10:11.637812 miniature-lighting-desk-0.1.1/LICENSE
--rw-r--r--   0        0        0       43 2021-12-27 10:10:11.641146 miniature-lighting-desk-0.1.1/miniature_lighting_desk/__init__.py
--rw-r--r--   0        0        0     6668 2021-12-27 10:10:11.641146 miniature-lighting-desk-0.1.1/miniature_lighting_desk/async_hal.py
--rw-r--r--   0        0        0      580 2021-12-27 10:10:11.641146 miniature-lighting-desk-0.1.1/miniature_lighting_desk/cli.py
--rw-r--r--   0        0        0     2829 2021-12-27 11:44:22.554723 miniature-lighting-desk-0.1.1/miniature_lighting_desk/local_gui.py
--rw-r--r--   0        0        0     4587 2021-12-27 10:10:11.641146 miniature-lighting-desk-0.1.1/miniature_lighting_desk/server.py
--rw-r--r--   0        0        0      712 2021-12-27 11:44:30.398063 miniature-lighting-desk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      887 2021-12-27 11:44:36.026907 miniature-lighting-desk-0.1.1/setup.py
--rw-r--r--   0        0        0      601 2021-12-27 11:44:36.027535 miniature-lighting-desk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.2.0/LICENSE
+-rw-r--r--   0        0        0       43 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.2.0/miniature_lighting_desk/__init__.py
+-rw-r--r--   0        0        0    10130 2023-07-10 21:44:26.485799 miniature_lighting_desk-0.2.0/miniature_lighting_desk/async_hal.py
+-rw-r--r--   0        0        0     1089 2023-07-10 21:50:30.169129 miniature_lighting_desk-0.2.0/miniature_lighting_desk/cli.py
+-rw-r--r--   0        0        0     3000 2023-07-10 21:46:19.949131 miniature_lighting_desk-0.2.0/miniature_lighting_desk/local_gui.py
+-rw-r--r--   0        0        0     4404 2023-07-10 21:52:08.892461 miniature_lighting_desk-0.2.0/miniature_lighting_desk/server.py
+-rw-r--r--   0        0        0      815 2023-07-11 21:03:17.451758 miniature_lighting_desk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 miniature_lighting_desk-0.2.0/PKG-INFO
```

### Comparing `miniature-lighting-desk-0.1.1/LICENSE` & `miniature_lighting_desk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miniature-lighting-desk-0.1.1/miniature_lighting_desk/async_hal.py` & `miniature_lighting_desk-0.2.0/miniature_lighting_desk/async_hal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,136 +1,231 @@
 import asyncio
+from abc import ABC, abstractmethod
 from functools import partial
 from re import search
 from threading import Thread
 from time import sleep
 
 import usb
+from aioserial import AioSerial
+from jsonrpcclient import parse, parse_json, request_json
 
 
 class ControllerError(Exception):
     """Controller failed to respond correctly after retries."""
 
 
-class Controller:
+class ControllerABC(ABC):
     """
     (Semi) Asynchronous class to represent a controller.
 
     Note that we do block, we just await between writes.
     """
 
-    def __init__(self, timeout=100):
+    no_channels: int
+    max_brightness: int
+
+    def __init__(self, *args, **kwargs) -> None:
+        self._start_async()
+
+    @abstractmethod
+    async def _async_set_brightness(
+        self, channel: int, brightness: int, pause: float = 0
+    ) -> None:
+        """Set brightness."""
+
+    @abstractmethod
+    async def _async_get_brightness(self, channel: int) -> int:
+        """Get brightness."""
+
+    @abstractmethod
+    def scale_brightness(self, unscaled: int) -> int:
+        """Scale brightness from controller to real world."""
+
+    @abstractmethod
+    def unscale_brightness(self, scaled: int) -> int:
+        """Scale brightness from real world to controller."""
+
+    def _start_async(self):
+        """Start an asyncio loop in the background."""
+        self.loop = asyncio.new_event_loop()
+        t = Thread(target=self.loop.run_forever)
+        t.daemon = True
+        t.start()
+
+    def stop_async(self):
+        """Stop background asyncio loop."""
+        self.loop.call_soon_threadsafe(self.loop.stop)
+
+    def submit_async(self, awaitable, block=False):
+        """Submit an awaitable to the background asyncio loop, returning a future for
+        it."""
+        future = asyncio.run_coroutine_threadsafe(awaitable(), self.loop)
+        if block:
+            while not future.done():
+                sleep(0.000_1)
+        return future
+
+    async def async_fade_brightness(
+        self, channel: int, start: int, end: int, fade_time_s: float
+    ) -> None:
+        steps = abs(end - start)
+        pause = fade_time_s / steps
+        if end > start:
+            steps = range(start, end + 1)
+        else:
+            steps = range(start, end - 1, -1)
+        for step in steps:
+            await self._async_set_brightness(
+                channel, self.scale_brightness(step), pause
+            )
+
+    def fade_brightness(self, channel, start, end, fade_time):
+        """Queue fading control."""
+        return self.submit_async(
+            partial(self.async_fade_brightness, channel, start, end, fade_time)
+        )
+
+    def set_brightness(self, channel: int, brightness: int, pause: float = 0):
+        """Queue setting brightness."""
+        brightness = self.scale_brightness(brightness)
+        return self.submit_async(
+            partial(self._async_set_brightness, channel, brightness, pause)
+        )
+
+    def get_brightness(self, channel, pause=0):
+        """Queue getting brightness."""
+        future = self.submit_async(
+            partial(self._async_get_brightness, channel), block=True
+        )
+        return self.unscale_brightness(future.result())
+
+
+class MockController(ControllerABC):
+    def __init__(self, *args, no_channels=8, **kwargs):
+        self.no_channels = no_channels
+        self.vals = [0] * no_channels
+        self.max_brightness = 100
+        super().__init__(*args, **kwargs)
+
+    async def _async_set_brightness(
+        self, channel: int, brightness: int, pause: float = 0
+    ) -> None:
+        self.vals[channel] = brightness
+        print(f"Setting channel {channel} to {brightness}")
+        await asyncio.sleep(pause)
+
+    async def _async_get_brightness(self, channel: int) -> int:
+        print(f"Getting brightness for channel {channel}")
+        return self.vals[channel]
+
+    scale_brightness = unscale_brightness = lambda s, x: x
+
+
+class PinguinoController(ControllerABC):
+    def __init__(self, *args, timeout=100, **kwargs):
         VENDOR = 0x04D8
         PRODUCT = 0xFEAA
         CONFIGURATION = 0x01
-        self._start_async()
         # find pinguino
         pinguino = None
         for bus in usb.busses():
             for dev in bus.devices:
                 if dev.idVendor == VENDOR and dev.idProduct == PRODUCT:
                     pinguino = dev
         if not pinguino:
             raise ControllerError("No Controller Found!")
         self.dh = pinguino.open()
         self.dh.setConfiguration(CONFIGURATION)
         self.dh.claimInterface(0)
         self.retries = 2
         self.timeout = timeout
-
-    def _start_async(self):
-        """Start an asyncio loop in the background."""
-        self.loop = asyncio.new_event_loop()
-        t = Thread(target=self.loop.run_forever)
-        t.daemon = True
-        t.start()
-
-    def stop_async(self):
-        """Stop background asyncio loop."""
-        self.loop.call_soon_threadsafe(self.loop.stop)
-
-    def submit_async(self, awaitable):
-        """Submit an awaitable to the background asyncio loop, returning a future for
-        it."""
-        return asyncio.run_coroutine_threadsafe(awaitable(), self.loop)
+        self.max_brightness = 256
+        self.no_channels = 8
+        super().__init__(*args, **kwargs)
 
     def _read(self, length):
         ENDPOINT_IN = 0x81
         buf = self.dh.bulkRead(ENDPOINT_IN, length, self.timeout)
         return "".join([chr(i) for i in buf])
 
     def _write(self, buf):
         ENDPOINT_OUT = 0x01
         return self.dh.bulkWrite(ENDPOINT_OUT, buf.encode(), self.timeout)
 
     def send(self, msg: str):
-        for i in range(self.retries):
+        for _ in range(self.retries):
             self._write(msg)
             ret = self._read(64)
             if "Error" not in ret:
                 return ret
         raise ControllerError(ret)
 
-    async def __await__set_brightness(self, channel, brightness, pause=0):
+    async def _async_set_brightness(self, channel, brightness, pause=0):
         msg = f"s{channel}{brightness:03d}"
         ret = self.send(msg)
         await asyncio.sleep(pause)
         return ret
 
-    async def __await__get_brightness(self, channel):
+    async def _async_get_brightness(self, channel):
         msg = f"g{channel:01d}"
         ret = self.send(msg)
         await asyncio.sleep(0)
-        return ret
-
-    async def __await__fade_brightness(self, channel, start, end, fade_time):
-        steps = abs(end - start)
-        pause = fade_time / steps
-        if end > start:
-            steps = range(start, end + 1)
-        else:
-            steps = range(start, end - 1, -1)
-        for step in steps:
-            await self.__await__set_brightness(channel, 256 - step, pause)
-            start = 256 - step
-
-    def fade_brightness(self, channel, start, end, fade_time):
-        """Queue fading control."""
-        return self.submit_async(
-            partial(self.__await__fade_brightness, channel, start, end, fade_time)
-        )
-
-    def set_brightness(self, channel, brightness, pause=0):
-        """Queue setting brightness."""
-        brightness = 256 - brightness
-        return self.submit_async(
-            partial(self.__await__set_brightness, channel, brightness, pause)
-        )
-
-    def get_brightness(self, channel, pause=0):
-        """Queue getting brightness."""
-        future = self.submit_async(partial(self.__await__get_brightness, channel))
-        while not future.done():
-            sleep(0.0001)  # wait in case we queue
-        match = search(r"Channel ([0-9]) is ([0-9]+)", future.result())
+        match = search(r"Channel ([0-9]) is ([0-9]+)", ret)
         if not match:
-            raise ControllerError(f"Garbage returned: {future.result()}")
+            raise ControllerError(f"Garbage returned: {ret}")
         chan, brightness = match.groups()
         if int(chan) == channel:
-            return 256 - int(brightness)
+            return int(brightness)
         else:
             raise ControllerError("Wrong channel returned!")
 
+    def scale_brightness(self, unscaled: int) -> int:
+        return self.max_brightness - unscaled
+
+    def unscale_brightness(self, scaled: int) -> int:
+        return self.max_brightness - scaled
+
+
+class SerialRpcController(ControllerABC):
+    def __init__(self, *args, port="/dev/ttyUSB0", **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.serial = AioSerial(port=port, baudrate=460800)
+        self.lock = asyncio.Lock()
+        future = self.submit_async(partial(self.call, "channel_count"), block=True)
+        self.no_channels = future.result()
+        future = self.submit_async(partial(self.call, "max_brightness"), block=True)
+        self.max_brightness = future.result()
+
+    async def call(self, method: str, **kwargs):
+        async with self.lock:  # dunno, might be needed...
+            cmd = request_json(method, params=kwargs).encode()
+            await self.serial.write_async(cmd)
+            await self.serial.write_async(b"\n\r")
+            resp = await self.serial.readline_async()
+            data = parse_json(resp.decode())
+            return data.result
+
+    async def _async_get_brightness(self, channel: int) -> int:
+        return await self.call("get_brightness", channel=channel)
+
+    async def _async_set_brightness(
+        self, channel: int, brightness: int, pause: float = 0
+    ) -> None:
+        return await self.call("set_brightness", channel=channel, brightness=brightness)
+
+    scale_brightness = unscale_brightness = lambda s, x: x
+
 
 class Channel:
     """Class to represent a particular channel on the controller."""
 
     def __init__(
         self,
-        controller: Controller,
+        controller: ControllerABC,
         channel_number,
         on_brightness=256,
         off_brightness=0,
     ):
         self.controller = controller
         self.channel_number = channel_number
         self._query()  # get brightness
@@ -194,12 +289,19 @@
 
     def cancel_fade(self):
         """Cancel ongoing fade and then query controller for actual channel value."""
         self.fade_future.cancel()
         self._query()
 
 
+controllers = {
+    "pinguino": PinguinoController,
+    "mock": MockController,
+    "16chan": SerialRpcController,
+}
+
+
 if __name__ == "__main__":
     # for testing or example
-    cont = Controller()
+    cont = PinguinoController()
     green = Channel(cont, 7)
     red = Channel(cont, 0)
```

### Comparing `miniature-lighting-desk-0.1.1/miniature_lighting_desk/local_gui.py` & `miniature_lighting_desk-0.2.0/miniature_lighting_desk/local_gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from . import async_hal as hal
 
 
 class ChannelSlider:
     """Channel Slider."""
 
-    def __init__(self, controller, channel, root):
+    def __init__(self, controller: hal.ControllerABC, channel, root):
         self.channel = hal.Channel(controller, channel)
         self.slider = Scale(
             root,
-            from_=256,
+            from_=controller.max_brightness,
             to=0,
             command=self._slider_changed,
             length=300,
             orient="vertical",
         )
         self.slider.grid(column=channel, row=0, padx=10)
         self.label = Label(root, text=f"Channel {channel}")
@@ -37,22 +37,22 @@
         self.slider.set(int(float(val)))
 
     def get(self):
         return self.slider.get()
 
 
 class App:
-    def __init__(self):
+    def __init__(self, channels: int, controller: hal.ControllerABC):
         self.root = Tk()
         self.root.title("Miniature Lighting Controller")
 
-        self.lighting_controller = hal.Controller()
+        self.lighting_controller = controller
         self.channels = []
 
-        for i in range(8):
+        for i in range(channels):
             self.channels.append(ChannelSlider(self.lighting_controller, i, self.root))
 
         load_button = Button(self.root, text="Load State", command=self.load_state)
         load_button.grid(column=2, row=3)
 
         save_button = Button(self.root, text="Save State", command=self.save_state)
         save_button.grid(column=8 - 3, row=3)
@@ -88,10 +88,10 @@
             ) as f:
                 writer = csv.writer(f)
                 writer.writerow([channel.get() for channel in self.channels])
         except Exception as e:
             print(f"Error: {e}")
 
 
-def main():
-    app = App()
+def main(controller: hal.ControllerABC):
+    app = App(channels=controller.no_channels, controller=controller)
     app()
```

### Comparing `miniature-lighting-desk-0.1.1/miniature_lighting_desk/server.py` & `miniature_lighting_desk-0.2.0/miniature_lighting_desk/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,14 @@
 from unittest.mock import MagicMock
 
 from autobahn.asyncio.component import Component, run
 
 from . import async_hal as hal
 
 
-class MockChannel:
-    def __init__(self, *args):
-        self.val = 0
-
-    def get_brightness(self):
-        return self.val
-
-    def set_brightness(self, val):
-        self.val = max(0, min(255, val))
-
-
 class Timer:
     def __init__(self, func, delay_ms: int):
         self._func = func
         self._delay_ms = int(delay_ms / 100)
         self.remaining_ms = self._delay_ms
         self.running = False
         self._started = False
@@ -57,25 +46,26 @@
 
     instances = []
 
     def __init__(
         self,
         *,
         component: Component,
-        channels: int = 8,
+        controller: hal.ControllerABC,
         channel=None,
-        controller=None,
     ):
         self.name = f"ControllerServer-{len(self.instances)}"
         self.instances.append(self.name)
         self._logger = getLogger(self.name)
 
-        self.controller = controller() if controller else hal.Controller()
+        self.controller = controller
         channel = channel or hal.Channel
-        self.channels = [channel(self.controller, i) for i in range(channels)]
+        self.channels = [
+            channel(self.controller, i) for i in range(controller.no_channels)
+        ]
         self.vals = []
         self.sync()
         self.component = component
         component.on_join(self.join)
         self.timer = Timer(self.publish, 5_000)
 
         component.register("sync")(self.sync)
@@ -90,49 +80,54 @@
         self.session = session
         self._logger.info(f"Joined {session} {details}")
 
     async def ping(self):
         return "hello"
 
     async def details(self):
-        return dict(channels=len(self.vals), name=self.name, vals=self.vals)
+        return dict(
+            channels=len(self.vals),
+            name=self.name,
+            vals=self.vals,
+            max_brightness=self.controller.max_brightness,
+        )
 
     async def set_brightness(self, *, channel: int, val: int):
         if self.vals[channel] != val:
             await self.timer.reset()
             await self.timer.start()
             self._logger.info(f"Setting channel {channel} to val {val}")
             self.channels[channel].set_brightness(val)
             self.vals[channel] = val
 
     async def publish(self):
-        self._logger.info("Publishing satechange")
+        self._logger.info("Publishing statechange")
         self.session.publish("controller.statechange", self.vals)
 
     async def get_brightness(self, *, channel: int):
         self._logger.debug(f"Got {self.vals[channel]} for channel {channel}")
         return self.vals[channel]
 
     def sync(self):
         self.vals = [channel.get_brightness() for channel in self.channels]
 
 
-class MockBackend(Backend):
-    """A backend with the hardware mocked away."""
+# class MockBackend(Backend):
+#     """A backend with the hardware mocked away."""
 
-    def __init__(
-        self,
-        **kwargs,
-    ):
-        kwargs["channel"] = MockChannel
-        kwargs["controller"] = MagicMock
-        super().__init__(**kwargs)
+#     def __init__(
+#         self,
+#         **kwargs,
+#     ):
+#         kwargs["channel"] = MockChannel
+#         kwargs["controller"] = MagicMock
+#         super().__init__(**kwargs)
 
 
-def main(mock, password):
+def main(password, controller):
     import ssl
 
     context = ssl.create_default_context()
     context.check_hostname = False
     context.verify_mode = ssl.CERT_NONE
     component = Component(
         transports=[
@@ -151,18 +146,11 @@
         authentication={
             "ticket": {
                 "authid": "public",
                 "ticket": password,
             },
         },
     )
-    if mock:
-        server = MockBackend(component=component)
-    else:
-        server = Backend(component=component)
+    server = Backend(controller=controller, component=component)
 
     print("\n Starting Backend\n Press Ctrl-c to exit\n")
     server.run()
-
-
-if __name__ == "__main__":
-    main()
```

