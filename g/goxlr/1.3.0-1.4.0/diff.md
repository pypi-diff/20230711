# Comparing `tmp/goxlr-1.3.0.tar.gz` & `tmp/goxlr-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.3.0.tar", last modified: Sat Jul  8 12:49:31 2023, max compression
+gzip compressed data, was "goxlr-1.4.0.tar", last modified: Mon Jul 10 22:34:16 2023, max compression
```

## Comparing `goxlr-1.3.0.tar` & `goxlr-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.335472 goxlr-1.3.0/
--rw-rw-rw-   0        0        0     1134 2023-07-04 22:58:41.000000 goxlr-1.3.0/LICENSE-3RD-PARTY.txt
--rw-rw-rw-   0        0        0     1089 2023-07-04 22:53:25.000000 goxlr-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2504 2023-07-08 12:49:31.335972 goxlr-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2147 2023-07-05 12:48:27.000000 goxlr-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.321973 goxlr-1.3.0/goxlr/
--rw-rw-rw-   0        0        0       62 2023-07-05 11:07:26.000000 goxlr-1.3.0/goxlr/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-08 12:49:08.000000 goxlr-1.3.0/goxlr/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.331471 goxlr-1.3.0/goxlr/commands/
--rw-rw-rw-   0        0        0      106 2023-07-07 18:35:48.000000 goxlr-1.3.0/goxlr/commands/__init__.py
--rw-rw-rw-   0        0        0     1376 2023-07-07 18:15:11.000000 goxlr-1.3.0/goxlr/commands/daemon.py
--rw-rw-rw-   0        0        0    26315 2023-07-08 12:48:03.000000 goxlr-1.3.0/goxlr/commands/goxlr.py
--rw-rw-rw-   0        0        0     4685 2023-07-08 12:39:50.000000 goxlr-1.3.0/goxlr/commands/status.py
--rw-rw-rw-   0        0        0       93 2023-07-07 19:20:53.000000 goxlr-1.3.0/goxlr/error.py
--rw-rw-rw-   0        0        0     7764 2023-07-08 12:42:53.000000 goxlr-1.3.0/goxlr/socket.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.334473 goxlr-1.3.0/goxlr/types/
--rw-rw-rw-   0        0        0       45 2023-07-08 11:41:47.000000 goxlr-1.3.0/goxlr/types/__init__.py
--rw-rw-rw-   0        0        0    11552 2023-07-08 10:59:03.000000 goxlr-1.3.0/goxlr/types/enums.py
--rw-rw-rw-   0        0        0    22457 2023-07-08 12:28:22.000000 goxlr-1.3.0/goxlr/types/models.py
-drwxrwxrwx   0        0        0        0 2023-07-08 12:49:31.326971 goxlr-1.3.0/goxlr.egg-info/
--rw-rw-rw-   0        0        0     2504 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 12:49:31.000000 goxlr-1.3.0/goxlr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-08 12:49:31.336977 goxlr-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-07-08 12:29:52.000000 goxlr-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-10 22:34:06.000000 goxlr-1.4.0/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 22:34:06.000000 goxlr-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-10 22:34:16.078720 goxlr-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-10 22:34:06.000000 goxlr-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/goxlr/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/goxlr/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/commands/goxlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/goxlr/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/goxlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 22:34:06.000000 goxlr-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 22:34:16.078720 goxlr-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-10 22:34:06.000000 goxlr-1.4.0/setup.py
```

### Comparing `goxlr-1.3.0/LICENSE-3RD-PARTY.txt` & `goxlr-1.4.0/LICENSE-3RD-PARTY.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Copyright 2022 Music Tribe Brands CA Ltd.
-
-This code and documentation contain information and intellectual property
-that is owned by MUSIC TRIBE. Permission is hereby granted to any person
-obtaining a copy of this software and associated documentation files to use
-the information without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and to permit
-persons to whom the software and documentation is furnished to do so, subject
-to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright 2022 Music Tribe Brands CA Ltd.
+
+This code and documentation contain information and intellectual property
+that is owned by MUSIC TRIBE. Permission is hereby granted to any person
+obtaining a copy of this software and associated documentation files to use
+the information without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and to permit
+persons to whom the software and documentation is furnished to do so, subject
+to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `goxlr-1.3.0/LICENSE.txt` & `goxlr-1.4.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Samuel Carson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Samuel Carson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `goxlr-1.3.0/PKG-INFO` & `goxlr-1.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-Metadata-Version: 2.1
-Name: goxlr
-Version: 1.3.0
-Summary: A Python wrapper for the GoXLR Utility API.
-Home-page: https://github.com/samcarsonx/goxlr
-Author: Sam Carson
-Author-email: sam@samcarson.co.uk
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE-3RD-PARTY.txt
-License-File: LICENSE.txt
-
-# GoXLR Utility API Python Wrapper
-
- [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
-
-A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio. Disclaimer: This project is not affiliated with the GoXLR brand or TC-Helicon in any way, shape, or form. This is a third-party package made for fun and educational purposes.
-
-## Features
-- Asynchronous connection to the GoXLR utility daemon
-- All methods have been translated to Python
-- Handy enumerators for everything
-- Very simple and easy to get started
-
-## Installation
-```shell
-pip install goxlr
-```
-
-## Getting Started
-Here's some sample code to get started with this package that pings the utility's daemon.
-```py
-import asyncio
-
-from goxlr import GoXLR
-from goxlr.types import Fader, Channel
-
-async def main():
-    async with GoXLR() as xlr:
-        await xlr.set_fader(Fader.A, Channel.Headphones)
-        await xlr.set_volume(Channel.Headphones, 127)
-
-if __name__ == "__main__":
-    asyncio.run(main())
-```
-
-You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
-```py
-async def main():
-    xlr = GoXLR()
-    await xlr.open()
-
-    ping = await xlr.ping()
-    print(ping)  # Ok
-
-    await xlr.close()
-```
-
-## Contributing
-Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
-
-## Documentation
-Please visit the [documentation](https://goxlr.readthedocs.io/en/latest/) for more information on how to use this package.
+Metadata-Version: 2.1
+Name: goxlr
+Version: 1.4.0
+Summary: A Python wrapper for the GoXLR Utility API.
+Home-page: https://github.com/samcarsonx/goxlr
+Author: Sam Carson
+Author-email: sam@samcarson.co.uk
+License: MIT
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE-3RD-PARTY.txt
+License-File: LICENSE.txt
+
+# GoXLR Utility API Python Wrapper
+
+ [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
+
+A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio. Disclaimer: This project is not affiliated with the GoXLR brand or TC-Helicon in any way, shape, or form. This is a third-party package made for fun and educational purposes.
+
+## Features
+- Asynchronous connection to the GoXLR utility daemon
+- All methods have been translated to Python
+- Handy enumerators for everything
+- Very simple and easy to get started
+
+## Installation
+```shell
+pip install goxlr
+```
+
+## Getting Started
+Here's some sample code to get started with this package that pings the utility's daemon.
+```py
+import asyncio
+
+from goxlr import GoXLR
+from goxlr.types import Fader, Channel
+
+async def main():
+    async with GoXLR() as xlr:
+        await xlr.set_fader(Fader.A, Channel.Headphones)
+        await xlr.set_volume(Channel.Headphones, 127)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
+```py
+async def main():
+    xlr = GoXLR()
+    await xlr.open()
+
+    ping = await xlr.ping()
+    print(ping)  # Ok
+
+    await xlr.close()
+```
+
+## Contributing
+Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
+
+## Documentation
+Please visit the [documentation](https://goxlr.readthedocs.io/en/latest/) for more information on how to use this package.
```

### Comparing `goxlr-1.3.0/goxlr/commands/goxlr.py` & `goxlr-1.4.0/goxlr/commands/goxlr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,652 +1,664 @@
-import ctypes
-from ..types.enums import *
-
-
-class GoXLRCommands:
-    # GoXLR commands
-
-    async def __send_command(self, payload, serial=None):
-        payload = {"Command": [serial or self.serial, payload]}
-        return await self.send(payload)
-
-    async def set_shutdown_commands(self, *methods) -> dict | str:
-        """
-        Set the commands to be executed when the GoXLR is shutting down.
-        Commands are accepted as a list of lists, where the first item is
-        the method name and the remaining items are the arguments for that
-        method.
-
-        :param methods: A list of methods to be executed when the GoXLR is shutting down.
-        :type methods: list
-        :return: The response from the GoXLR.
-
-        :Example:
-
-        >>> await xlr.set_shutdown_commands(
-        ...     ["SetFader", Fader.A, Channel.Headphones],
-        ...     ["SetFader", Fader.B, Channel.Chat]
-        ... )
-        """
-
-        # Initialize the command dictionary
-        command = {"SetShutdownCommands": []}
-
-        # Iterate over the provided methods
-        for method in methods:
-            if not isinstance(method, list):
-                raise TypeError("Methods must be provided as a list")
-
-            # Extract the method name and arguments
-            method_name, *args = method
-            args = [arg.name if isinstance(arg, Enum) else arg for arg in args]
-
-            # Create a dictionary for the method and arguments
-            method_dict = {method_name: args}
-
-            # Append the method dictionary to the command
-            command["SetShutdownCommands"].append(method_dict)
-
-        return await self.__send_command(command)
-
-    async def set_sampler_pre_buffer_duration(self, duration: ctypes.c_uint16):
-        return await self.__send_command({"SetSamplerPreBufferDuration": duration})
-
-    async def set_fader(self, fader: Fader, channel: Channel):
-        return await self.__send_command({"SetFader": [fader.name, channel.name]})
-
-    async def set_fader_mute_function(self, fader: Fader, mute_function: MuteFunction):
-        return await self.__send_command(
-            {"SetFaderMuteFunction": [fader.name, mute_function.name]}
-        )
-
-    async def set_volume(self, channel: Channel, volume: ctypes.c_uint8):
-        return await self.__send_command({"SetVolume": [channel.name, volume]})
-
-    async def set_microphone_type(self, microphone_type: MicrophoneType):
-        return await self.__send_command({"SetMicrophoneType": microphone_type.name})
-
-    async def set_microphone_gain(
-        self, microphone_type: MicrophoneType, gain: ctypes.c_uint16
-    ):
-        return await self.__send_command(
-            {"SetMicrophoneGain": [microphone_type.name, gain]}
-        )
-
-    async def set_router(
-        self, input_device: InputDevice, output_device: OutputDevice, enabled: bool
-    ):
-        return await self.__send_command(
-            {"SetRouter": [input_device.name, output_device.name, enabled]}
-        )
-
-    # Cough Button
-    async def set_cough_mute_function(self, mute_function: MuteFunction):
-        return await self.__send_command({"SetCoughMuteFunction": mute_function.name})
-
-    async def set_cough_is_hold(self, is_hold: bool):
-        return await self.__send_command({"SetCoughIsHold": is_hold})
-
-    # Bleep Button
-    async def set_swear_button_volume(self, volume: ctypes.c_int8):
-        return await self.__send_command({"SetSwearButtonVolume": volume})
-
-    # EQ Settings
-    async def set_eq_mini_gain(
-        self, mini_eq_frequency: MiniEqFrequency, gain: ctypes.c_int8
-    ):
-        return await self.__send_command(
-            {"SetEqMiniGain": [mini_eq_frequency.name, gain]}
-        )
-
-    async def set_eq_mini_frequency(
-        self, mini_eq_frequency: MiniEqFrequency, frequency: ctypes.c_float
-    ):
-        return await self.__send_command(
-            {"SetEqMiniFrequency": [mini_eq_frequency.name, frequency]}
-        )
-
-    async def set_eq_gain(self, eq_frequency: EqFrequency, gain: ctypes.c_int8):
-        return await self.__send_command({"SetEqGain": [eq_frequency.name, gain]})
-
-    async def set_eq_frequency(
-        self, eq_frequency: EqFrequency, frequency: ctypes.c_float
-    ):
-        return await self.__send_command(
-            {"SetEqFrequency": [eq_frequency.name, frequency]}
-        )
-
-    # Gate Settings
-    async def set_gate_threshold(self, gate_threshold: ctypes.c_int8):
-        return await self.__send_command({"SetGateThreshold": gate_threshold})
-
-    async def set_gate_attenuation(self, gate_attenuation: ctypes.c_uint8):
-        return await self.__send_command({"SetGateAttenuation": gate_attenuation})
-
-    async def set_gate_attack(self, gate_attack: GateTime):
-        return await self.__send_command({"SetGateAttack": gate_attack.name})
-
-    async def set_gate_release(self, gate_release: GateTime):
-        return await self.__send_command({"SetGateRelease": gate_release.name})
-
-    async def set_gate_active(self, gate_active: bool):
-        return await self.__send_command({"SetGateActive": gate_active})
-
-    # Compressor Settings
-    async def set_compressor_threshold(self, compressor_threshold: ctypes.c_int8):
-        return await self.__send_command(
-            {"SetCompressorThreshold": compressor_threshold}
-        )
-
-    async def set_compressor_ratio(self, compressor_ratio: CompressorRatio):
-        return await self.__send_command({"SetCompressorRatio": compressor_ratio.name})
-
-    async def set_compressor_attack(self, compressor_attack: CompressorAttackTime):
-        return await self.__send_command(
-            {"SetCompressorAttack": compressor_attack.name}
-        )
-
-    async def set_compressor_release_time(
-        self, compressor_release: CompressorReleaseTime
-    ):
-        return await self.__send_command(
-            {"SetCompressorReleaseTime": compressor_release.name}
-        )
-
-    async def set_compressor_makeup_gain(self, compressor_makeup_gain: ctypes.c_int8):
-        return await self.__send_command(
-            {"SetCompressorMakeupGain": compressor_makeup_gain}
-        )
-
-    # Used to switch between display modes
-    async def set_element_display_mode(
-        self, display_mode_component: DisplayModeComponent, display_mode: DisplayMode
-    ):
-        return await self.__send_command(
-            {"SetElementDisplayMode": [display_mode_component.name, display_mode.name]}
-        )
-
-    # DeEss
-    async def set_deeser(self, deesser: ctypes.c_uint8):
-        return await self.__send_command({"SetDeesser": deesser})
-
-    # Colour Related Settings
-    async def set_animation_mode(self, animation_mode: AnimationMode):
-        return await self.__send_command(
-            {
-                "SetAnimationMode": "None"
-                if animation_mode is AnimationMode.NONE
-                else animation_mode.name
-            }
-        )
-
-    async def set_animation_mod1(self, animation_mod1: ctypes.c_uint8):
-        return await self.__send_command({"SetAnimationMod1": animation_mod1})
-
-    async def set_animation_mod2(self, animation_mod2: ctypes.c_uint8):
-        return await self.__send_command({"SetAnimationMod2": animation_mod2})
-
-    async def set_animation_waterfall(self, waterfall_direction: WaterfallDirection):
-        return await self.__send_command(
-            {"SetAnimationWaterfall": waterfall_direction.name}
-        )
-
-    async def set_global_colour(self, colour: str):
-        return await self.__send_command({"SetGlobalColour": colour})
-
-    async def set_fader_display_style(
-        self, fader: Fader, fader_display_style: FaderDisplayStyle
-    ):
-        return await self.__send_command(
-            {"SetFaderDisplayStyle": [fader.name, fader_display_style.name]}
-        )
-
-    async def set_fader_colours(self, fader: Fader, colour1: str, colour2: str):
-        return await self.__send_command(
-            {"SetFaderColours": [fader.name, colour1, colour2]}
-        )
-
-    async def set_all_fader_colours(self, colour1: str, colour2: str):
-        return await self.__send_command({"SetAllFaderColours": [colour1, colour2]})
-
-    async def set_all_fader_display_style(self, fader_display_style: FaderDisplayStyle):
-        return await self.__send_command(
-            {"SetAllFaderDisplayStyle": fader_display_style.name}
-        )
-
-    async def set_button_colours(
-        self, button: Button, colour1: str, colour2: str = None
-    ):
-        return await self.__send_command(
-            {"SetButtonColours": [button.name, colour1, colour2]}
-        )
-
-    async def set_button_off_style(
-        self, button: Button, off_style: ButtonColourOffStyle
-    ):
-        return await self.__send_command(
-            {"SetButtonOffStyle": [button.name, off_style.name]}
-        )
-
-    async def set_button_group_colours(
-        self,
-        button_colour_group: ButtonColourGroup,
-        colour1: str,
-        colour2: str = None,
-    ):
-        return await self.__send_command(
-            {"SetButtonGroupColours": [button_colour_group.name, colour1, colour2]}
-        )
-
-    async def set_button_group_off_style(
-        self, button_colour_group: ButtonColourGroup, off_style: ButtonColourOffStyle
-    ):
-        return await self.__send_command(
-            {"SetButtonGroupOffStyle": [button_colour_group.name, off_style.name]}
-        )
-
-    async def set_simple_colour(
-        self, simple_colour_target: SimpleColourTarget, colour: str
-    ):
-        return await self.__send_command(
-            {"SetSimpleColour": [simple_colour_target.name, colour]}
-        )
-
-    async def set_encoder_colour(self, encoder: EncoderColourTarget, colour: str):
-        return await self.__send_command({"SetEncoderColour": [encoder.name, colour]})
-
-    async def set_sample_colour(self, sample: SamplerColourTarget, colour: str):
-        return await self.__send_command({"SetSampleColour": [sample.name, colour]})
-
-    async def set_sample_off_style(
-        self, sample: SamplerColourTarget, off_style: ButtonColourOffStyle
-    ):
-        return await self.__send_command(
-            {"SetSampleOffStyle": [sample.name, off_style.name]}
-        )
-
-    # Effect Related Settings
-    async def load_effect(self, effect_name: str):
-        return await self.__send_command({"LoadEffect": effect_name})
-
-    async def rename_active_preset(self, new_name: str):
-        return await self.__send_command({"RenameActivePreset": new_name})
-
-    async def save_active_preset(self):
-        return await self.__send_command({"SaveActivePreset": []})
-
-    # Reverb
-    async def set_reverb_style(self, reverb_style: ReverbStyle):
-        return await self.__send_command({"SetReverbStyle": reverb_style.name})
-
-    async def set_reverb_amount(self, reverb_amount: ctypes.c_uint8):
-        return await self.__send_command({"SetReverbAmount": reverb_amount})
-
-    async def set_reverb_decay(self, reverb_decay: ctypes.c_uint16):
-        return await self.__send_command({"SetReverbDecay": reverb_decay})
-
-    async def set_reverb_early_level(self, reverb_early_level: ctypes.c_int8):
-        return await self.__send_command({"SetReverbEarlyLevel": reverb_early_level})
-
-    async def set_reverb_tail_level(self, reverb_tail_level: ctypes.c_int8):
-        return await self.__send_command({"SetReverbTailLevel": reverb_tail_level})
-
-    async def set_reverb_pre_delay(self, reverb_pre_delay: ctypes.c_uint8):
-        return await self.__send_command({"SetReverbPreDelay": reverb_pre_delay})
-
-    async def set_reverb_low_colour(self, reverb_low_colour: ctypes.c_int8):
-        return await self.__send_command({"SetReverbLowColour": reverb_low_colour})
-
-    async def set_reverb_high_colour(self, reverb_high_colour: ctypes.c_int8):
-        return await self.__send_command({"SetReverbHighColour": reverb_high_colour})
-
-    async def set_reverb_high_factor(self, reverb_high_factor: ctypes.c_int8):
-        return await self.__send_command({"SetReverbHighFactor": reverb_high_factor})
-
-    async def set_reverb_diffuse(self, reverb_diffuse: ctypes.c_uint8):
-        return await self.__send_command({"SetReverbDiffuse": reverb_diffuse})
-
-    async def set_reverb_mod_speed(self, reverb_mod_speed: ctypes.c_uint8):
-        return await self.__send_command({"SetReverbModSpeed": reverb_mod_speed})
-
-    async def set_reverb_mod_depth(self, reverb_mod_depth: ctypes.c_uint8):
-        return await self.__send_command({"SetReverbModDepth": reverb_mod_depth})
-
-    # Echo
-    async def set_echo_style(self, echo_style: EchoStyle):
-        return await self.__send_command({"SetEchoStyle": echo_style.name})
-
-    async def set_echo_amount(self, echo_amount: ctypes.c_uint8):
-        return await self.__send_command({"SetEchoAmount": echo_amount})
-
-    async def set_echo_feedback(self, echo_feedback: ctypes.c_uint8):
-        return await self.__send_command({"SetEchoFeedback": echo_feedback})
-
-    async def set_echo_tempo(self, echo_tempo: ctypes.c_uint16):
-        return await self.__send_command({"SetEchoTempo": echo_tempo})
-
-    async def set_echo_delay_left(self, echo_delay_left: ctypes.c_uint16):
-        return await self.__send_command({"SetEchoDelayLeft": echo_delay_left})
-
-    async def set_echo_delay_right(self, echo_delay_right: ctypes.c_uint16):
-        return await self.__send_command({"SetEchoDelayRight": echo_delay_right})
-
-    async def set_echo_feedback_left(self, echo_feedback_left: ctypes.c_uint8):
-        return await self.__send_command({"SetEchoFeedbackLeft": echo_feedback_left})
-
-    async def set_echo_feedback_right(self, echo_feedback_right: ctypes.c_uint8):
-        return await self.__send_command({"SetEchoFeedbackRight": echo_feedback_right})
-
-    async def set_echo_feedback_xfb_l_to_r(
-        self, echo_feedback_xfb_l_to_r: ctypes.c_uint8
-    ):
-        return await self.__send_command(
-            {"SetEchoFeedbackXFBLtoR": echo_feedback_xfb_l_to_r}
-        )
-
-    async def set_echo_feedback_xfb_r_to_l(
-        self, echo_feedback_xfb_r_to_l: ctypes.c_uint8
-    ):
-        return await self.__send_command(
-            {"SetEchoFeedbackXFBRtoL": echo_feedback_xfb_r_to_l}
-        )
-
-    # Pitch
-    async def set_pitch_style(self, pitch_style: PitchStyle):
-        return await self.__send_command({"SetPitchStyle": pitch_style.name})
-
-    async def set_pitch_amount(self, pitch_amount: ctypes.c_int8):
-        return await self.__send_command({"SetPitchAmount": pitch_amount})
-
-    async def set_pitch_character(self, pitch_character: ctypes.c_uint8):
-        return await self.__send_command({"SetPitchCharacter": pitch_character})
-
-    # Gender
-    async def set_gender_style(self, gender_style: GenderStyle):
-        return await self.__send_command({"SetGenderStyle": gender_style.name})
-
-    async def set_gender_amount(self, gender_amount: ctypes.c_int8):
-        return await self.__send_command({"SetGenderAmount": gender_amount})
-
-    # Megaphone
-    async def set_megaphone_style(self, megaphone_style: MegaphoneStyle):
-        return await self.__send_command({"SetMegaphoneStyle": megaphone_style.name})
-
-    async def set_megaphone_amount(self, megaphone_amount: ctypes.c_uint8):
-        return await self.__send_command({"SetMegaphoneAmount": megaphone_amount})
-
-    async def set_megaphone_post_gain(self, megaphone_post_gain: ctypes.c_int8):
-        return await self.__send_command({"SetMegaphonePostGain": megaphone_post_gain})
-
-    # Robot
-    async def set_robot_style(self, robot_style: RobotStyle):
-        return await self.__send_command({"SetRobotStyle": robot_style.name})
-
-    async def set_robot_gain(self, robot_range: RobotRange, robot_gain: ctypes.c_int8):
-        return await self.__send_command(
-            {"SetRobotGain": [robot_range.name, robot_gain]}
-        )
-
-    async def set_robot_frequency(
-        self, robot_range: RobotRange, robot_frequency: ctypes.c_uint8
-    ):
-        return await self.__send_command(
-            {"SetRobotFreq": [robot_range.name, robot_frequency]}
-        )
-
-    async def set_robot_width(
-        self, robot_range: RobotRange, robot_width: ctypes.c_uint8
-    ):
-        return await self.__send_command(
-            {"SetRobotWidth": [robot_range.name, robot_width]}
-        )
-
-    async def set_robot_waveform(self, robot_waveform: ctypes.c_uint8):
-        return await self.__send_command({"SetRobotWaveform": robot_waveform})
-
-    async def set_robot_pulse_width(self, robot_pulse_width: ctypes.c_uint8):
-        return await self.__send_command({"SetRobotPulseWidth": robot_pulse_width})
-
-    async def set_robot_threshold(self, robot_threshold: ctypes.c_int8):
-        return await self.__send_command({"SetRobotThreshold": robot_threshold})
-
-    async def set_robot_dry_mix(self, robot_dry_mix: ctypes.c_int8):
-        return await self.__send_command({"SetRobotDryMix": robot_dry_mix})
-
-    # Hardtune
-    async def set_hardtune_style(self, hardtune_style: HardTuneStyle):
-        return await self.__send_command({"SetHardTuneStyle": hardtune_style.name})
-
-    async def set_hardtune_amount(self, hardtune_amount: ctypes.c_uint8):
-        return await self.__send_command({"SetHardTuneAmount": hardtune_amount})
-
-    async def set_hardtune_rate(self, hardtune_rate: ctypes.c_uint8):
-        return await self.__send_command({"SetHardTuneRate": hardtune_rate})
-
-    async def set_hardtune_window(self, hardtune_window: ctypes.c_uint16):
-        return await self.__send_command({"SetHardTuneWindow": hardtune_window})
-
-    async def set_hardtune_source(self, hardtune_source: HardTuneSource):
-        return await self.__send_command({"SetHardTuneSource": hardtune_source.name})
-
-    # Sampler
-    async def clear_sample_process_error(self):
-        return await self.__send_command({"ClearSampleProcessError": []})
-
-    async def set_sampler_function(
-        self,
-        sample_bank: SampleBank,
-        sample_button: SampleButton,
-        sample_playback_mode: SamplePlaybackMode,
-    ):
-        return await self.__send_command(
-            {
-                "SetSamplerFunction": [
-                    sample_bank.name,
-                    sample_button.name,
-                    sample_playback_mode.name,
-                ]
-            }
-        )
-
-    async def set_sampler_order(
-        self,
-        sample_bank: SampleBank,
-        sample_button: SampleButton,
-        sample_play_order: SamplePlayOrder,
-    ):
-        return await self.__send_command(
-            {
-                "SetSamplerOrder": [
-                    sample_bank.name,
-                    sample_button.name,
-                    sample_play_order.name,
-                ]
-            }
-        )
-
-    async def add_sample(
-        self, sample_bank: SampleBank, sample_button: SampleButton, sample_name: str
-    ):
-        return await self.__send_command(
-            {"AddSample": [sample_bank.name, sample_button.name, sample_name]}
-        )
-
-    async def set_sample_start_percent(
-        self,
-        sample_bank: SampleBank,
-        sample_button: SampleButton,
-        index: int,
-        sample_start_percent: ctypes.c_float,
-    ):
-        return await self.__send_command(
-            {
-                "SetSampleStartPercent": [
-                    sample_bank.name,
-                    sample_button.name,
-                    index,
-                    sample_start_percent,
-                ]
-            }
-        )
-
-    async def set_sample_stop_percent(
-        self,
-        sample_bank: SampleBank,
-        sample_button: SampleButton,
-        index: int,
-        sample_stop_percent: ctypes.c_float,
-    ):
-        return await self.__send_command(
-            {
-                "SetSampleStopPercent": [
-                    sample_bank.name,
-                    sample_button.name,
-                    index,
-                    sample_stop_percent,
-                ]
-            }
-        )
-
-    async def remove_sample_by_index(
-        self, sample_bank: SampleBank, sample_button: SampleButton, index: int
-    ):
-        return await self.__send_command(
-            {"RemoveSampleByIndex": [sample_bank.name, sample_button.name, index]}
-        )
-
-    async def play_sample_by_index(
-        self, sample_bank: SampleBank, sample_button: SampleButton, index: int
-    ):
-        return await self.__send_command(
-            {"PlaySampleByIndex": [sample_bank.name, sample_button.name, index]}
-        )
-
-    async def play_next_sample(
-        self, sample_bank: SampleBank, sample_button: SampleButton
-    ):
-        return await self.__send_command(
-            {"PlayNextSample": [sample_bank.name, sample_button.name]}
-        )
-
-    async def stop_sample_playback(
-        self, sample_bank: SampleBank, sample_button: SampleButton
-    ):
-        return await self.__send_command(
-            {"StopSamplePlayback": [sample_bank.name, sample_button.name]}
-        )
-
-    # Scribbles
-    async def set_scribble_icon(self, fader: Fader, scribble_icon: str = None):
-        return await self.__send_command(
-            {"SetScribbleIcon": [fader.name, scribble_icon]}
-        )
-
-    async def set_scribble_text(self, fader: Fader, scribble_text: str):
-        return await self.__send_command(
-            {"SetScribbleText": [fader.name, scribble_text]}
-        )
-
-    async def set_scribble_number(self, fader: Fader, scribble_number: str):
-        return await self.__send_command(
-            {"SetScribbleNumber": [fader.name, scribble_number]}
-        )
-
-    async def set_scribble_invert(self, fader: Fader, scribble_invert: bool):
-        return await self.__send_command(
-            {"SetScribbleInvert": [fader.name, scribble_invert]}
-        )
-
-    # Profile Handling
-    async def new_profile(self, profile_name: str):
-        return await self.__send_command({"NewProfile": profile_name})
-
-    async def load_profile(self, profile_name: str, save_changes: bool = False):
-        return await self.__send_command({"LoadProfile": [profile_name, save_changes]})
-
-    async def load_profile_colours(self, profile_name: str):
-        return await self.__send_command({"LoadProfileColours": profile_name})
-
-    async def save_profile(self):
-        return await self.__send_command({"SaveProfile": []})
-
-    async def save_profile_as(self, profile_name: str):
-        return await self.__send_command({"SaveProfileAs": profile_name})
-
-    async def delete_profile(self, profile_name: str):
-        return await self.__send_command({"DeleteProfile": profile_name})
-
-    async def new_mic_profile(self, profile_name: str):
-        return await self.__send_command({"NewMicProfile": profile_name})
-
-    async def load_mic_profile(self, profile_name: str, save_changes: bool = False):
-        return await self.__send_command(
-            {"LoadMicProfile": [profile_name, save_changes]}
-        )
-
-    async def save_mic_profile(self):
-        return await self.__send_command({"SaveMicProfile": []})
-
-    async def save_mic_profile_as(self, profile_name: str):
-        return await self.__send_command({"SaveMicProfileAs": profile_name})
-
-    async def delete_mic_profile(self, profile_name: str):
-        return await self.__send_command({"DeleteMicProfile": profile_name})
-
-    # General Settings
-    async def set_mute_hold_duration(self, mute_hold_duration: ctypes.c_uint16):
-        return await self.__send_command({"SetMuteHoldDuration": mute_hold_duration})
-
-    async def set_vc_mute_also_mute_cm(self, vc_mute_also_mute_cm: bool):
-        return await self.__send_command({"SetVCMuteAlsoMuteCM": vc_mute_also_mute_cm})
-
-    # These control the current GoXLR state
-    async def set_active_effect_preset(self, active_effect_preset: EffectBankPreset):
-        return await self.__send_command(
-            {"SetActiveEffectPreset": active_effect_preset.name}
-        )
-
-    async def set_active_sampler_bank(self, active_sampler_bank: SampleBank):
-        return await self.__send_command(
-            {"SetActiveSamplerBank": active_sampler_bank.name}
-        )
-
-    async def set_megaphone_enabled(self, megaphone_enabled: bool):
-        return await self.__send_command({"SetMegaphoneEnabled": megaphone_enabled})
-
-    async def set_robot_enabled(self, robot_enabled: bool):
-        return await self.__send_command({"SetRobotEnabled": robot_enabled})
-
-    async def set_hardtune_enabled(self, hardtune_enabled: bool):
-        return await self.__send_command({"SetHardTuneEnabled": hardtune_enabled})
-
-    async def set_fx_enabled(self, fx_enabled: bool):
-        return await self.__send_command({"SetFXEnabled": fx_enabled})
-
-    async def set_fader_mute_state(self, fader: Fader, mute_state: MuteState):
-        return await self.__send_command(
-            {"SetFaderMuteState": [fader.name, mute_state.name]}
-        )
-
-    async def set_cough_mute_state(self, mute_state: MuteState):
-        return await self.__send_command({"SetCoughMuteState": mute_state.name})
-
-    # Submix commands
-    async def set_submix_enabled(self, enabled: bool):
-        return await self.__send_command({"SetSubMixEnabled": enabled})
-
-    async def set_submix_volume(self, channel: Channel, volume: ctypes.c_uint8):
-        return await self.__send_command({"SetSubMixVolume": [channel.name, volume]})
-
-    async def set_submix_linked(self, channel: Channel, linked: bool):
-        return await self.__send_command({"SetSubMixLinked": [channel.name, linked]})
-
-    async def set_submix_output_mix(self, output_device: OutputDevice, mix: Mix):
-        return await self.__send_command(
-            {"SetSubMixOutputMix": [output_device.name, mix.name]}
-        )
-
-    # Mix monitoring
-    async def set_monitor_mix(self, output_device: OutputDevice):
-        return await self.__send_command({"SetMonitorMix": output_device.name})
-
-    # it's..done..?
+import ctypes
+
+from ..types.models import Colours
+from ..types.enums import *
+
+
+class GoXLRCommands:
+    # GoXLR commands
+
+    async def __send_command(self, payload, serial=None):
+        payload = {"Command": [serial or self.serial, payload]}
+        return await self.send(payload)
+
+    async def set_shutdown_commands(self, *methods) -> dict | str:
+        """
+        Set the commands to be executed when the GoXLR is shutting down.
+        Commands are accepted as a list of lists, where the first item is
+        the method name and the remaining items are the arguments for that
+        method.
+
+        :param methods: A list of methods to be executed when the GoXLR is shutting down.
+        :type methods: list
+        :return: The response from the GoXLR.
+
+        :Example:
+
+        >>> await xlr.set_shutdown_commands(
+        ...     ["SetFader", Fader.A, Channel.Headphones],
+        ...     ["SetFader", Fader.B, Channel.Chat]
+        ... )
+        """
+
+        # Initialize the command dictionary
+        command = {"SetShutdownCommands": []}
+
+        # Iterate over the provided methods
+        for method in methods:
+            if not isinstance(method, list):
+                raise TypeError("Methods must be provided as a list")
+
+            # Extract the method name and arguments
+            method_name, *args = method
+            args = [arg.name if isinstance(arg, Enum) else arg for arg in args]
+
+            # Create a dictionary for the method and arguments
+            method_dict = {method_name: args}
+
+            # Append the method dictionary to the command
+            command["SetShutdownCommands"].append(method_dict)
+
+        return await self.__send_command(command)
+
+    async def set_sampler_pre_buffer_duration(self, duration: ctypes.c_uint16):
+        return await self.__send_command({"SetSamplerPreBufferDuration": duration})
+
+    async def set_fader(self, fader: Fader, channel: Channel):
+        return await self.__send_command({"SetFader": [fader.name, channel.name]})
+
+    async def set_fader_mute_function(self, fader: Fader, mute_function: MuteFunction):
+        return await self.__send_command(
+            {"SetFaderMuteFunction": [fader.name, mute_function.name]}
+        )
+
+    async def set_volume(self, channel: Channel, volume: ctypes.c_uint8):
+        return await self.__send_command({"SetVolume": [channel.name, volume]})
+
+    async def set_microphone_type(self, microphone_type: MicrophoneType):
+        return await self.__send_command({"SetMicrophoneType": microphone_type.name})
+
+    async def set_microphone_gain(
+        self, microphone_type: MicrophoneType, gain: ctypes.c_uint16
+    ):
+        return await self.__send_command(
+            {"SetMicrophoneGain": [microphone_type.name, gain]}
+        )
+
+    async def set_router(
+        self, input_device: InputDevice, output_device: OutputDevice, enabled: bool
+    ):
+        return await self.__send_command(
+            {"SetRouter": [input_device.name, output_device.name, enabled]}
+        )
+
+    # Cough Button
+    async def set_cough_mute_function(self, mute_function: MuteFunction):
+        return await self.__send_command({"SetCoughMuteFunction": mute_function.name})
+
+    async def set_cough_is_hold(self, is_hold: bool):
+        return await self.__send_command({"SetCoughIsHold": is_hold})
+
+    # Bleep Button
+    async def set_bleep_volume(self, volume: ctypes.c_int8):
+        return await self.__send_command({"SetSwearButtonVolume": volume})
+
+    # EQ Settings
+    async def set_eq_mini_gain(
+        self, mini_eq_frequency: MiniEqFrequency, gain: ctypes.c_int8
+    ):
+        return await self.__send_command(
+            {"SetEqMiniGain": [mini_eq_frequency.name, gain]}
+        )
+
+    async def set_eq_mini_frequency(
+        self, mini_eq_frequency: MiniEqFrequency, frequency: ctypes.c_float
+    ):
+        return await self.__send_command(
+            {"SetEqMiniFrequency": [mini_eq_frequency.name, frequency]}
+        )
+
+    async def set_eq_gain(self, eq_frequency: EqFrequency, gain: ctypes.c_int8):
+        return await self.__send_command({"SetEqGain": [eq_frequency.name, gain]})
+
+    async def set_eq_frequency(
+        self, eq_frequency: EqFrequency, frequency: ctypes.c_float
+    ):
+        return await self.__send_command(
+            {"SetEqFrequency": [eq_frequency.name, frequency]}
+        )
+
+    # Gate Settings
+    async def set_gate_threshold(self, gate_threshold: ctypes.c_int8):
+        return await self.__send_command({"SetGateThreshold": gate_threshold})
+
+    async def set_gate_attenuation(self, gate_attenuation: ctypes.c_uint8):
+        return await self.__send_command({"SetGateAttenuation": gate_attenuation})
+
+    async def set_gate_attack(self, gate_attack: GateTime):
+        return await self.__send_command({"SetGateAttack": gate_attack.name})
+
+    async def set_gate_release(self, gate_release: GateTime):
+        return await self.__send_command({"SetGateRelease": gate_release.name})
+
+    async def set_gate_active(self, gate_active: bool):
+        return await self.__send_command({"SetGateActive": gate_active})
+
+    # Compressor Settings
+    async def set_compressor_threshold(self, compressor_threshold: ctypes.c_int8):
+        return await self.__send_command(
+            {"SetCompressorThreshold": compressor_threshold}
+        )
+
+    async def set_compressor_ratio(self, compressor_ratio: CompressorRatio):
+        return await self.__send_command({"SetCompressorRatio": compressor_ratio.name})
+
+    async def set_compressor_attack(self, compressor_attack: CompressorAttackTime):
+        return await self.__send_command(
+            {"SetCompressorAttack": compressor_attack.name}
+        )
+
+    async def set_compressor_release_time(
+        self, compressor_release: CompressorReleaseTime
+    ):
+        return await self.__send_command(
+            {"SetCompressorReleaseTime": compressor_release.name}
+        )
+
+    async def set_compressor_makeup_gain(self, compressor_makeup_gain: ctypes.c_int8):
+        return await self.__send_command(
+            {"SetCompressorMakeupGain": compressor_makeup_gain}
+        )
+
+    # Used to switch between display modes
+    async def set_element_display_mode(
+        self, display_mode_component: DisplayModeComponent, display_mode: DisplayMode
+    ):
+        return await self.__send_command(
+            {"SetElementDisplayMode": [display_mode_component.name, display_mode.name]}
+        )
+
+    # DeEss
+    async def set_deesser(self, deesser: ctypes.c_uint8):
+        return await self.__send_command({"SetDeesser": deesser})
+
+    # Colour Related Settings
+    async def set_animation_mode(self, animation_mode: AnimationMode):
+        return await self.__send_command(
+            {
+                "SetAnimationMode": "None"
+                if animation_mode is AnimationMode.NONE
+                else animation_mode.name
+            }
+        )
+
+    async def set_animation_mod1(self, animation_mod1: ctypes.c_uint8):
+        return await self.__send_command({"SetAnimationMod1": animation_mod1})
+
+    async def set_animation_mod2(self, animation_mod2: ctypes.c_uint8):
+        return await self.__send_command({"SetAnimationMod2": animation_mod2})
+
+    async def set_animation_waterfall(self, waterfall_direction: WaterfallDirection):
+        return await self.__send_command(
+            {"SetAnimationWaterfall": waterfall_direction.name}
+        )
+
+    async def set_global_colour(self, colour: str):
+        return await self.__send_command({"SetGlobalColour": colour})
+
+    async def set_fader_display_style(
+        self, fader: Fader, fader_display_style: FaderDisplayStyle
+    ):
+        return await self.__send_command(
+            {"SetFaderDisplayStyle": [fader.name, fader_display_style.name]}
+        )
+
+    async def set_fader_colours(self, fader: Fader, colour1: str, colour2: str):
+        return await self.__send_command(
+            {"SetFaderColours": [fader.name, colour1, colour2]}
+        )
+
+    async def set_all_fader_colours(self, colour1: str, colour2: str):
+        return await self.__send_command({"SetAllFaderColours": [colour1, colour2]})
+
+    async def set_all_fader_display_style(self, fader_display_style: FaderDisplayStyle):
+        return await self.__send_command(
+            {"SetAllFaderDisplayStyle": fader_display_style.name}
+        )
+
+    async def set_button_colours(
+        self, button: Button, colour1: str, colour2: str = None
+    ):
+        return await self.__send_command(
+            {"SetButtonColours": [button.name, colour1, colour2]}
+        )
+
+    async def set_button_off_style(
+        self, button: Button, off_style: ButtonColourOffStyle
+    ):
+        return await self.__send_command(
+            {"SetButtonOffStyle": [button.name, off_style.name]}
+        )
+
+    async def set_button_group_colours(
+        self,
+        button_colour_group: ButtonColourGroup,
+        colour1: str,
+        colour2: str = None,
+    ):
+        return await self.__send_command(
+            {"SetButtonGroupColours": [button_colour_group.name, colour1, colour2]}
+        )
+
+    async def set_button_group_off_style(
+        self, button_colour_group: ButtonColourGroup, off_style: ButtonColourOffStyle
+    ):
+        return await self.__send_command(
+            {"SetButtonGroupOffStyle": [button_colour_group.name, off_style.name]}
+        )
+
+    async def set_simple_colour(
+        self, simple_colour_target: SimpleColourTarget, colour: str
+    ):
+        return await self.__send_command(
+            {"SetSimpleColour": [simple_colour_target.name, colour]}
+        )
+
+    async def set_encoder_colours(self, encoder: EncoderColourTarget, colours: Colours):
+        colour1 = colours.colour_one
+        colour2 = colours.colour_two
+        colour3 = colours.colour_three
+        return await self.__send_command(
+            {"SetEncoderColour": [encoder.name, colour1, colour2, colour3]}
+        )
+
+    async def set_sample_colours(self, sample: SamplerColourTarget, colours: Colours):
+        colour1 = colours.colour_one
+        colour2 = colours.colour_two
+        colour3 = colours.colour_three
+        return await self.__send_command(
+            {"SetSampleColour": [sample.name, colour1, colour2, colour3]}
+        )
+
+    async def set_sample_off_style(
+        self, sample: SamplerColourTarget, off_style: ButtonColourOffStyle
+    ):
+        return await self.__send_command(
+            {"SetSampleOffStyle": [sample.name, off_style.name]}
+        )
+
+    # Effect Related Settings
+    async def load_effect(self, effect_name: str):
+        return await self.__send_command({"LoadEffect": effect_name})
+
+    async def rename_active_preset(self, new_name: str):
+        return await self.__send_command({"RenameActivePreset": new_name})
+
+    async def save_active_preset(self):
+        return await self.__send_command({"SaveActivePreset": []})
+
+    # Reverb
+    async def set_reverb_style(self, reverb_style: ReverbStyle):
+        return await self.__send_command({"SetReverbStyle": reverb_style.name})
+
+    async def set_reverb_amount(self, reverb_amount: ctypes.c_uint8):
+        return await self.__send_command({"SetReverbAmount": reverb_amount})
+
+    async def set_reverb_decay(self, reverb_decay: ctypes.c_uint16):
+        return await self.__send_command({"SetReverbDecay": reverb_decay})
+
+    async def set_reverb_early_level(self, reverb_early_level: ctypes.c_int8):
+        return await self.__send_command({"SetReverbEarlyLevel": reverb_early_level})
+
+    async def set_reverb_tail_level(self, reverb_tail_level: ctypes.c_int8):
+        return await self.__send_command({"SetReverbTailLevel": reverb_tail_level})
+
+    async def set_reverb_pre_delay(self, reverb_pre_delay: ctypes.c_uint8):
+        return await self.__send_command({"SetReverbPreDelay": reverb_pre_delay})
+
+    async def set_reverb_low_colour(self, reverb_low_colour: ctypes.c_int8):
+        return await self.__send_command({"SetReverbLowColour": reverb_low_colour})
+
+    async def set_reverb_high_colour(self, reverb_high_colour: ctypes.c_int8):
+        return await self.__send_command({"SetReverbHighColour": reverb_high_colour})
+
+    async def set_reverb_high_factor(self, reverb_high_factor: ctypes.c_int8):
+        return await self.__send_command({"SetReverbHighFactor": reverb_high_factor})
+
+    async def set_reverb_diffuse(self, reverb_diffuse: ctypes.c_uint8):
+        return await self.__send_command({"SetReverbDiffuse": reverb_diffuse})
+
+    async def set_reverb_mod_speed(self, reverb_mod_speed: ctypes.c_uint8):
+        return await self.__send_command({"SetReverbModSpeed": reverb_mod_speed})
+
+    async def set_reverb_mod_depth(self, reverb_mod_depth: ctypes.c_uint8):
+        return await self.__send_command({"SetReverbModDepth": reverb_mod_depth})
+
+    # Echo
+    async def set_echo_style(self, echo_style: EchoStyle):
+        return await self.__send_command({"SetEchoStyle": echo_style.name})
+
+    async def set_echo_amount(self, echo_amount: ctypes.c_uint8):
+        return await self.__send_command({"SetEchoAmount": echo_amount})
+
+    async def set_echo_feedback(self, echo_feedback: ctypes.c_uint8):
+        return await self.__send_command({"SetEchoFeedback": echo_feedback})
+
+    async def set_echo_tempo(self, echo_tempo: ctypes.c_uint16):
+        return await self.__send_command({"SetEchoTempo": echo_tempo})
+
+    async def set_echo_delay_left(self, echo_delay_left: ctypes.c_uint16):
+        return await self.__send_command({"SetEchoDelayLeft": echo_delay_left})
+
+    async def set_echo_delay_right(self, echo_delay_right: ctypes.c_uint16):
+        return await self.__send_command({"SetEchoDelayRight": echo_delay_right})
+
+    async def set_echo_feedback_left(self, echo_feedback_left: ctypes.c_uint8):
+        return await self.__send_command({"SetEchoFeedbackLeft": echo_feedback_left})
+
+    async def set_echo_feedback_right(self, echo_feedback_right: ctypes.c_uint8):
+        return await self.__send_command({"SetEchoFeedbackRight": echo_feedback_right})
+
+    async def set_echo_feedback_xfb_l_to_r(
+        self, echo_feedback_xfb_l_to_r: ctypes.c_uint8
+    ):
+        return await self.__send_command(
+            {"SetEchoFeedbackXFBLtoR": echo_feedback_xfb_l_to_r}
+        )
+
+    async def set_echo_feedback_xfb_r_to_l(
+        self, echo_feedback_xfb_r_to_l: ctypes.c_uint8
+    ):
+        return await self.__send_command(
+            {"SetEchoFeedbackXFBRtoL": echo_feedback_xfb_r_to_l}
+        )
+
+    # Pitch
+    async def set_pitch_style(self, pitch_style: PitchStyle):
+        return await self.__send_command({"SetPitchStyle": pitch_style.name})
+
+    async def set_pitch_amount(self, pitch_amount: ctypes.c_int8):
+        return await self.__send_command({"SetPitchAmount": pitch_amount})
+
+    async def set_pitch_character(self, pitch_character: ctypes.c_uint8):
+        return await self.__send_command({"SetPitchCharacter": pitch_character})
+
+    # Gender
+    async def set_gender_style(self, gender_style: GenderStyle):
+        return await self.__send_command({"SetGenderStyle": gender_style.name})
+
+    async def set_gender_amount(self, gender_amount: ctypes.c_int8):
+        return await self.__send_command({"SetGenderAmount": gender_amount})
+
+    # Megaphone
+    async def set_megaphone_style(self, megaphone_style: MegaphoneStyle):
+        return await self.__send_command({"SetMegaphoneStyle": megaphone_style.name})
+
+    async def set_megaphone_amount(self, megaphone_amount: ctypes.c_uint8):
+        return await self.__send_command({"SetMegaphoneAmount": megaphone_amount})
+
+    async def set_megaphone_post_gain(self, megaphone_post_gain: ctypes.c_int8):
+        return await self.__send_command({"SetMegaphonePostGain": megaphone_post_gain})
+
+    # Robot
+    async def set_robot_style(self, robot_style: RobotStyle):
+        return await self.__send_command({"SetRobotStyle": robot_style.name})
+
+    async def set_robot_gain(self, robot_range: RobotRange, robot_gain: ctypes.c_int8):
+        return await self.__send_command(
+            {"SetRobotGain": [robot_range.name, robot_gain]}
+        )
+
+    async def set_robot_frequency(
+        self, robot_range: RobotRange, robot_frequency: ctypes.c_uint8
+    ):
+        return await self.__send_command(
+            {"SetRobotFreq": [robot_range.name, robot_frequency]}
+        )
+
+    async def set_robot_width(
+        self, robot_range: RobotRange, robot_width: ctypes.c_uint8
+    ):
+        return await self.__send_command(
+            {"SetRobotWidth": [robot_range.name, robot_width]}
+        )
+
+    async def set_robot_waveform(self, robot_waveform: ctypes.c_uint8):
+        return await self.__send_command({"SetRobotWaveform": robot_waveform})
+
+    async def set_robot_pulse_width(self, robot_pulse_width: ctypes.c_uint8):
+        return await self.__send_command({"SetRobotPulseWidth": robot_pulse_width})
+
+    async def set_robot_threshold(self, robot_threshold: ctypes.c_int8):
+        return await self.__send_command({"SetRobotThreshold": robot_threshold})
+
+    async def set_robot_dry_mix(self, robot_dry_mix: ctypes.c_int8):
+        return await self.__send_command({"SetRobotDryMix": robot_dry_mix})
+
+    # Hardtune
+    async def set_hardtune_style(self, hardtune_style: HardTuneStyle):
+        return await self.__send_command({"SetHardTuneStyle": hardtune_style.name})
+
+    async def set_hardtune_amount(self, hardtune_amount: ctypes.c_uint8):
+        return await self.__send_command({"SetHardTuneAmount": hardtune_amount})
+
+    async def set_hardtune_rate(self, hardtune_rate: ctypes.c_uint8):
+        return await self.__send_command({"SetHardTuneRate": hardtune_rate})
+
+    async def set_hardtune_window(self, hardtune_window: ctypes.c_uint16):
+        return await self.__send_command({"SetHardTuneWindow": hardtune_window})
+
+    async def set_hardtune_source(self, hardtune_source: HardTuneSource):
+        return await self.__send_command({"SetHardTuneSource": hardtune_source.name})
+
+    # Sampler
+    async def clear_sample_process_error(self):
+        return await self.__send_command({"ClearSampleProcessError": []})
+
+    async def set_sampler_function(
+        self,
+        sample_bank: SampleBank,
+        sample_button: SampleButton,
+        sample_playback_mode: SamplePlaybackMode,
+    ):
+        return await self.__send_command(
+            {
+                "SetSamplerFunction": [
+                    sample_bank.name,
+                    sample_button.name,
+                    sample_playback_mode.name,
+                ]
+            }
+        )
+
+    async def set_sampler_order(
+        self,
+        sample_bank: SampleBank,
+        sample_button: SampleButton,
+        sample_play_order: SamplePlayOrder,
+    ):
+        return await self.__send_command(
+            {
+                "SetSamplerOrder": [
+                    sample_bank.name,
+                    sample_button.name,
+                    sample_play_order.name,
+                ]
+            }
+        )
+
+    async def add_sample(
+        self, sample_bank: SampleBank, sample_button: SampleButton, sample_name: str
+    ):
+        return await self.__send_command(
+            {"AddSample": [sample_bank.name, sample_button.name, sample_name]}
+        )
+
+    async def set_sample_start_percent(
+        self,
+        sample_bank: SampleBank,
+        sample_button: SampleButton,
+        index: int,
+        sample_start_percent: ctypes.c_float,
+    ):
+        return await self.__send_command(
+            {
+                "SetSampleStartPercent": [
+                    sample_bank.name,
+                    sample_button.name,
+                    index,
+                    sample_start_percent,
+                ]
+            }
+        )
+
+    async def set_sample_stop_percent(
+        self,
+        sample_bank: SampleBank,
+        sample_button: SampleButton,
+        index: int,
+        sample_stop_percent: ctypes.c_float,
+    ):
+        return await self.__send_command(
+            {
+                "SetSampleStopPercent": [
+                    sample_bank.name,
+                    sample_button.name,
+                    index,
+                    sample_stop_percent,
+                ]
+            }
+        )
+
+    async def remove_sample_by_index(
+        self, sample_bank: SampleBank, sample_button: SampleButton, index: int
+    ):
+        return await self.__send_command(
+            {"RemoveSampleByIndex": [sample_bank.name, sample_button.name, index]}
+        )
+
+    async def play_sample_by_index(
+        self, sample_bank: SampleBank, sample_button: SampleButton, index: int
+    ):
+        return await self.__send_command(
+            {"PlaySampleByIndex": [sample_bank.name, sample_button.name, index]}
+        )
+
+    async def play_next_sample(
+        self, sample_bank: SampleBank, sample_button: SampleButton
+    ):
+        return await self.__send_command(
+            {"PlayNextSample": [sample_bank.name, sample_button.name]}
+        )
+
+    async def stop_sample_playback(
+        self, sample_bank: SampleBank, sample_button: SampleButton
+    ):
+        return await self.__send_command(
+            {"StopSamplePlayback": [sample_bank.name, sample_button.name]}
+        )
+
+    # Scribbles
+    async def set_scribble_icon(self, fader: Fader, scribble_icon: str = None):
+        return await self.__send_command(
+            {"SetScribbleIcon": [fader.name, scribble_icon]}
+        )
+
+    async def set_scribble_text(self, fader: Fader, scribble_text: str):
+        return await self.__send_command(
+            {"SetScribbleText": [fader.name, scribble_text]}
+        )
+
+    async def set_scribble_number(self, fader: Fader, scribble_number: str):
+        return await self.__send_command(
+            {"SetScribbleNumber": [fader.name, scribble_number]}
+        )
+
+    async def set_scribble_invert(self, fader: Fader, scribble_invert: bool):
+        return await self.__send_command(
+            {"SetScribbleInvert": [fader.name, scribble_invert]}
+        )
+
+    # Profile Handling
+    async def new_profile(self, profile_name: str):
+        return await self.__send_command({"NewProfile": profile_name})
+
+    async def load_profile(self, profile_name: str, save_changes: bool = False):
+        return await self.__send_command({"LoadProfile": [profile_name, save_changes]})
+
+    async def load_profile_colours(self, profile_name: str):
+        return await self.__send_command({"LoadProfileColours": profile_name})
+
+    async def save_profile(self):
+        return await self.__send_command({"SaveProfile": []})
+
+    async def save_profile_as(self, profile_name: str):
+        return await self.__send_command({"SaveProfileAs": profile_name})
+
+    async def delete_profile(self, profile_name: str):
+        return await self.__send_command({"DeleteProfile": profile_name})
+
+    async def new_mic_profile(self, profile_name: str):
+        return await self.__send_command({"NewMicProfile": profile_name})
+
+    async def load_mic_profile(self, profile_name: str, save_changes: bool = False):
+        return await self.__send_command(
+            {"LoadMicProfile": [profile_name, save_changes]}
+        )
+
+    async def save_mic_profile(self):
+        return await self.__send_command({"SaveMicProfile": []})
+
+    async def save_mic_profile_as(self, profile_name: str):
+        return await self.__send_command({"SaveMicProfileAs": profile_name})
+
+    async def delete_mic_profile(self, profile_name: str):
+        return await self.__send_command({"DeleteMicProfile": profile_name})
+
+    # General Settings
+    async def set_mute_hold_duration(self, mute_hold_duration: ctypes.c_uint16):
+        return await self.__send_command({"SetMuteHoldDuration": mute_hold_duration})
+
+    async def set_vc_mute_also_mute_cm(self, vc_mute_also_mute_cm: bool):
+        return await self.__send_command({"SetVCMuteAlsoMuteCM": vc_mute_also_mute_cm})
+
+    # These control the current GoXLR state
+    async def set_active_effect_preset(self, active_effect_preset: EffectBankPreset):
+        return await self.__send_command(
+            {"SetActiveEffectPreset": active_effect_preset.name}
+        )
+
+    async def set_sampler_active_bank(self, active_sampler_bank: SampleBank):
+        return await self.__send_command(
+            {"SetActiveSamplerBank": active_sampler_bank.name}
+        )
+
+    async def set_megaphone_enabled(self, megaphone_enabled: bool):
+        return await self.__send_command({"SetMegaphoneEnabled": megaphone_enabled})
+
+    async def set_robot_enabled(self, robot_enabled: bool):
+        return await self.__send_command({"SetRobotEnabled": robot_enabled})
+
+    async def set_hardtune_enabled(self, hardtune_enabled: bool):
+        return await self.__send_command({"SetHardTuneEnabled": hardtune_enabled})
+
+    async def set_fx_enabled(self, fx_enabled: bool):
+        return await self.__send_command({"SetFXEnabled": fx_enabled})
+
+    async def set_fader_mute_state(self, fader: Fader, mute_state: MuteState):
+        return await self.__send_command(
+            {"SetFaderMuteState": [fader.name, mute_state.name]}
+        )
+
+    async def set_cough_mute_state(self, mute_state: MuteState):
+        return await self.__send_command({"SetCoughMuteState": mute_state.name})
+
+    # Submix commands
+    async def set_submix_enabled(self, enabled: bool):
+        return await self.__send_command({"SetSubMixEnabled": enabled})
+
+    async def set_submix_volume(self, channel: SubMixChannel, volume: ctypes.c_uint8):
+        return await self.__send_command({"SetSubMixVolume": [channel.name, volume]})
+
+    async def set_submix_linked(self, channel: SubMixChannel, linked: bool):
+        return await self.__send_command({"SetSubMixLinked": [channel.name, linked]})
+
+    async def set_submix_output_mix(self, output_device: OutputDevice, mix: Mix):
+        return await self.__send_command(
+            {"SetSubMixOutputMix": [output_device.name, mix.name]}
+        )
+
+    # Mix monitoring
+    async def set_monitor_mix(self, output_device: OutputDevice):
+        return await self.__send_command({"SetMonitorMix": output_device.name})
+
+    # it's..done..?
```

### Comparing `goxlr-1.3.0/goxlr/socket.py` & `goxlr-1.4.0/goxlr/socket.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-import asyncio
-from typing import List
-import websockets
-import json
-
-from goxlr.types.models import Mixer, Status
-
-from .commands import DaemonCommands, GoXLRCommands, StatusCommands
-
-from .error import DaemonError, MixerNotFoundError
-
-
-class Socket:
-    """
-    A class for handling the websocket connection to the daemon.
-    It also handles the heartbeat task and the response queue. The response
-    queue is used to ensure that the correct response is returned for a
-    specific request.
-
-    :param host: The host/IP address of the daemon.
-    :param port: The port of the daemon.
-    """
-
-    def __init__(self, host, port):
-        self.host = host
-        self.port = port
-        self.uri = f"ws://{self.host}:{self.port}/api/websocket"
-        self.socket = None
-        self.heartbeat_interval = 5
-        self.heartbeat_task = None
-        self.heartbeat_payload = {"id": 0, "data": "Ping"}
-        self.response_queue = []
-
-    async def connect(self):
-        """
-        Connects to the daemon and starts the heartbeat task.
-
-        :return: True if the connection was successful, False otherwise.
-        """
-        self.socket = await websockets.connect(self.uri)
-        self.heartbeat_task = asyncio.create_task(self.__send_heartbeat())
-        return self.socket.open
-
-    async def __send_heartbeat(self):
-        while True:
-            await asyncio.sleep(self.heartbeat_interval)
-            await self.socket.send(json.dumps(self.heartbeat_payload))
-
-    async def send(self, payload, id=None):
-        """
-        Sends a payload to the daemon and waits for a response.
-
-        :param payload: The payload to send to the daemon.
-        :param id: The ID of the payload. If not specified, it will
-                   automatically generate one. Used purely for identifying
-                   the correct response, considering that this is an async
-                   function and responses may come in out of order.
-
-        :return: The response from the daemon.
-        """
-        id = id or self.response_queue[-1].get("id") + 1 if self.response_queue else 1
-
-        payload = {"id": id, "data": payload}
-        await self.socket.send(json.dumps(payload))
-
-        response = await self.receive(id)
-        data = response.get("data")
-
-        if data == "Ok":
-            return data
-        elif isinstance(data, dict):
-            if status := data.get("Status"):
-                return status
-            elif patch := data.get("Patch"):
-                return patch
-            elif error := data.get("Error"):
-                raise DaemonError(error)
-
-    async def receive(self, id=None):
-        """
-        Waits for a response from the daemon. If an ID is specified, it will
-        wait until it receives a response with the same ID and queue all other
-        responses.
-
-        If no ID is specified, it will wait for the first response and will
-        not add it to the queue.
-
-        To wait for a heartbeat response, specify an ID of 0.
-        To wait for a patch response, specify an ID of 2**64 - 1.
-
-        :param id: The ID of the response to wait for.
-
-        :return: The response from the daemon.
-
-        :raises: `DaemonError` if the daemon returns an error.
-        """
-        if not id:
-            response = await self.socket.recv()
-            response = json.loads(response)
-            return response
-
-        # if we already have the response, return it
-        for r in self.response_queue:
-            if r.get("id") == id:
-                self.response_queue.remove(r)
-                return r
-
-        # keep receiving until we get a response with the same id
-        while True:
-            response = await self.socket.recv()
-            response = json.loads(response)
-
-            if response.get("id") == id:
-                return response
-            else:
-                if response.get("id") in (0, 2**64 - 1):
-                    # no need to queue heartbeat and patch responses
-                    # if we want to do something with them, either specify
-                    # the id or don't specify one at all
-                    continue
-                self.response_queue.append(response)
-
-    async def open(self):
-        """
-        Alias for `connect()`.
-
-        :return: True if the connection was successful, False otherwise.
-        """
-        return await self.connect()
-
-    async def close(self):
-        """
-        Closes the connection to the daemon.
-
-        :return: True if the connection was closed, False otherwise.
-        """
-        await self.socket.close()
-        self.heartbeat_task.cancel()
-        return self.socket.closed
-
-    async def __aenter__(self):
-        await self.connect()
-        return self
-
-    async def __aexit__(self, exc_type, exc_value, traceback):
-        await self.close()
-
-
-class GoXLR(Socket, DaemonCommands, GoXLRCommands, StatusCommands):
-    """
-    A class for interacting with the GoXLR Utility daemon.
-    """
-
-    def __init__(self, host="localhost", port=14564, serial=None):
-        super().__init__(host, port)
-
-        self.status: Status = None
-
-        self.mixer: Mixer = None  # the currently selected mixer
-        self.serial: str = (
-            serial  # shorthand for self.mixer.hardware_info.serial_number
-        )
-
-    async def ping(self):
-        """
-        Pings the GoXLR Utility daemon.
-
-        :return: "Ok" if the daemon is running.
-        """
-        return await self.send("Ping")
-
-    async def update(self):
-        """
-        Gets the latest data from the GoXLR Utility daemon and updates the status
-        and mixers attributes.
-
-        :return: The status of the daemon.
-
-        :raises DaemonError: If the daemon is not running.
-        :raises MixerNotFoundError: If the specified mixer is not found.
-
-        :note: This method is automatically called when the class is instantiated.
-        You should manually call this method periodically to ensure that the data
-        is up to date.
-        """
-        self.status = await self.get_status()
-
-        if self.serial:
-            self.mixer = self.select_mixer(self.serial)
-
-        return self.status
-
-    def select_mixer(self, serial: str = None):
-        """
-        Chooses a mixer to interact with.
-
-        :param serial: The serial number of the mixer to interact with.
-                       If not specified, it will default to the first mixer.
-
-        :return: The selected mixer.
-
-        :raises DaemonError: If no mixers are found.
-        :raises MixerNotFoundError: If the specified mixer is not found.
-        """
-
-        # set self.serial to serial if specified. if None, default to first mixer
-        if not self.status.mixers:
-            raise DaemonError("No mixers found.")
-
-        if serial:
-            if serial not in self.status.mixers:
-                raise MixerNotFoundError(f"Mixer with serial {serial} not found")
-        else:
-            serial = next(iter(self.status.mixers))
-
-        self.serial = serial
-        self.mixer = self.status.mixers.get(self.serial)
-
-        return self.mixer
-
-    async def connect(self):
-        """
-        Connects to the GoXLR Utility daemon and gets the latest data.
-
-        :return: True if the connection was successful, False otherwise.
-
-        :raises DaemonError: If no mixers are found.
-        """
-        connected = await super().connect()
-        if connected:
-            await self.update()
-            self.select_mixer()  # select the first mixer by default
-
-        return connected
+import asyncio
+from typing import List
+import websockets
+import json
+
+from goxlr.types.models import Mixer, Status
+
+from .commands import DaemonCommands, GoXLRCommands, StatusCommands
+
+from .error import DaemonError, MixerNotFoundError
+
+
+class Socket:
+    """
+    A class for handling the websocket connection to the daemon.
+    It also handles the heartbeat task and the response queue. The response
+    queue is used to ensure that the correct response is returned for a
+    specific request.
+
+    :param host: The host/IP address of the daemon.
+    :param port: The port of the daemon.
+    """
+
+    def __init__(self, host, port):
+        self.host = host
+        self.port = port
+        self.uri = f"ws://{self.host}:{self.port}/api/websocket"
+        self.socket = None
+        self.heartbeat_interval = 5
+        self.heartbeat_task = None
+        self.heartbeat_payload = {"id": 0, "data": "Ping"}
+        self.response_queue = []
+
+    async def connect(self):
+        """
+        Connects to the daemon and starts the heartbeat task.
+
+        :return: True if the connection was successful, False otherwise.
+        """
+        self.socket = await websockets.connect(self.uri)
+        self.heartbeat_task = asyncio.create_task(self.__send_heartbeat())
+        return self.socket.open
+
+    async def __send_heartbeat(self):
+        while True:
+            await asyncio.sleep(self.heartbeat_interval)
+            await self.socket.send(json.dumps(self.heartbeat_payload))
+
+    async def send(self, payload, id=None):
+        """
+        Sends a payload to the daemon and waits for a response.
+
+        :param payload: The payload to send to the daemon.
+        :param id: The ID of the payload. If not specified, it will
+                   automatically generate one. Used purely for identifying
+                   the correct response, considering that this is an async
+                   function and responses may come in out of order.
+
+        :return: The response from the daemon.
+        """
+        id = id or self.response_queue[-1].get("id") + 1 if self.response_queue else 1
+
+        payload = {"id": id, "data": payload}
+        await self.socket.send(json.dumps(payload))
+
+        response = await self.receive(id)
+        data = response.get("data")
+
+        if data == "Ok":
+            return data
+        elif isinstance(data, dict):
+            if status := data.get("Status"):
+                return status
+            elif patch := data.get("Patch"):
+                return patch
+            elif error := data.get("Error"):
+                raise DaemonError(error)
+
+    async def receive(self, id=None):
+        """
+        Waits for a response from the daemon. If an ID is specified, it will
+        wait until it receives a response with the same ID and queue all other
+        responses.
+
+        If no ID is specified, it will wait for the first response and will
+        not add it to the queue.
+
+        To wait for a heartbeat response, specify an ID of 0.
+        To wait for a patch response, specify an ID of 2**64 - 1.
+
+        :param id: The ID of the response to wait for.
+
+        :return: The response from the daemon.
+
+        :raises: `DaemonError` if the daemon returns an error.
+        """
+        if not id:
+            response = await self.socket.recv()
+            response = json.loads(response)
+            return response
+
+        # if we already have the response, return it
+        for r in self.response_queue:
+            if r.get("id") == id:
+                self.response_queue.remove(r)
+                return r
+
+        # keep receiving until we get a response with the same id
+        while True:
+            response = await self.socket.recv()
+            response = json.loads(response)
+
+            if response.get("id") == id:
+                return response
+            else:
+                if response.get("id") in (0, 2**64 - 1):
+                    # no need to queue heartbeat and patch responses
+                    # if we want to do something with them, either specify
+                    # the id or don't specify one at all
+                    continue
+                self.response_queue.append(response)
+
+    async def open(self):
+        """
+        Alias for `connect()`.
+
+        :return: True if the connection was successful, False otherwise.
+        """
+        return await self.connect()
+
+    async def close(self):
+        """
+        Closes the connection to the daemon.
+
+        :return: True if the connection was closed, False otherwise.
+        """
+        await self.socket.close()
+        self.heartbeat_task.cancel()
+        return self.socket.closed
+
+    async def __aenter__(self):
+        await self.connect()
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self.close()
+
+
+class GoXLR(Socket, DaemonCommands, GoXLRCommands, StatusCommands):
+    """
+    A class for interacting with the GoXLR Utility daemon.
+    """
+
+    def __init__(self, host="localhost", port=14564, serial=None):
+        super().__init__(host, port)
+
+        self.status: Status = None
+
+        self.mixer: Mixer = None  # the currently selected mixer
+        self.serial: str = (
+            serial  # shorthand for self.mixer.hardware_info.serial_number
+        )
+
+    async def ping(self):
+        """
+        Pings the GoXLR Utility daemon.
+
+        :return: "Ok" if the daemon is running.
+        """
+        return await self.send("Ping")
+
+    async def update(self):
+        """
+        Gets the latest data from the GoXLR Utility daemon and updates the status
+        and mixers attributes.
+
+        :return: The status of the daemon.
+
+        :raises DaemonError: If the daemon is not running.
+        :raises MixerNotFoundError: If the specified mixer is not found.
+
+        :note: This method is automatically called when the class is instantiated.
+            You should manually call this method periodically to ensure that the data
+            is up to date.
+        """
+        self.status = await self.get_status()
+
+        if self.serial:
+            self.mixer = self.select_mixer(self.serial)
+
+        return self.status
+
+    def select_mixer(self, serial: str = None):
+        """
+        Chooses a mixer to interact with.
+
+        :param serial: The serial number of the mixer to interact with.
+                       If not specified, it will default to the first mixer.
+
+        :return: The selected mixer.
+
+        :raises DaemonError: If no mixers are found.
+        :raises MixerNotFoundError: If the specified mixer is not found.
+        """
+
+        # set self.serial to serial if specified. if None, default to first mixer
+        if not self.status.mixers:
+            raise DaemonError("No mixers found.")
+
+        if serial:
+            if serial not in self.status.mixers:
+                raise MixerNotFoundError(f"Mixer with serial {serial} not found")
+        else:
+            serial = next(iter(self.status.mixers))
+
+        self.serial = serial
+        self.mixer = self.status.mixers.get(self.serial)
+
+        return self.mixer
+
+    async def connect(self):
+        """
+        Connects to the GoXLR Utility daemon and gets the latest data.
+
+        :return: True if the connection was successful, False otherwise.
+
+        :raises DaemonError: If no mixers are found.
+        """
+        connected = await super().connect()
+        if connected:
+            await self.update()
+            self.select_mixer()  # select the first mixer by default
+
+        return connected
```

### Comparing `goxlr-1.3.0/goxlr/types/enums.py` & `goxlr-1.4.0/goxlr/types/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,586 +1,592 @@
-from enum import Enum
-
-# Enumerators used by the GoXLR Utility Daemon. (with slight name changes)
-
-
-class PathType(Enum):
-    Profiles = 1
-    MicProfiles = 2
-    Presets = 3
-    Samples = 4
-    Icons = 5
-    Logs = 6
-
-
-class LogLevel(Enum):
-    Off = 1
-    Error = 2
-    Warn = 3
-    Info = 4
-    Debug = 5
-    Trace = 6
-
-
-class Channel(Enum):
-    Mic = 1
-    LineIn = 2
-    Console = 3
-    System = 4
-    Game = 5
-    Chat = 6
-    Sample = 7
-    Music = 8
-    Headphones = 9
-    MicMonitor = 10
-    LineOut = 11
-
-
-class Mix(Enum):
-    A = 1
-    B = 2
-
-
-class SubMixChannel(Enum):
-    Mic = 1
-    LineIn = 2
-    Console = 3
-    System = 4
-    Game = 5
-    Chat = 6
-    Sample = 7
-    Music = 8
-
-
-class Fader(Enum):
-    A = 1
-    B = 2
-    C = 3
-    D = 4
-
-
-class Encoder(Enum):
-    Pitch = 1
-    Gender = 2
-    Reverb = 3
-    Echo = 4
-
-
-class OutputDevice(Enum):
-    Headphones = 1
-    BroadcastMix = 2
-    ChatMic = 3
-    Sampler = 4
-    LineOut = 5
-
-
-class InputDevice(Enum):
-    Microphone = 1
-    Chat = 2
-    Music = 3
-    Game = 4
-    Console = 5
-    LineIn = 6
-    System = 7
-    Samples = 8
-
-
-class EffectKey(Enum):
-    DisableMic = 0x0158
-    BleepLevel = 0x0073
-    GateMode = 0x0010
-    GateThreshold = 0x0011
-    GateEnabled = 0x0014
-    GateAttenuation = 0x0015
-    GateAttack = 0x0016
-    GateRelease = 0x0017
-    MicCompSelect = 0x014B
-    Equalizer31HzFrequency = 0x0126
-    Equalizer31HzGain = 0x0127
-    Equalizer63HzFrequency = 0x00F8
-    Equalizer63HzGain = 0x00F9
-    Equalizer125HzFrequency = 0x0113
-    Equalizer125HzGain = 0x0114
-    Equalizer250HzFrequency = 0x0129
-    Equalizer250HzGain = 0x012A
-    Equalizer500HzFrequency = 0x0116
-    Equalizer500HzGain = 0x0117
-    Equalizer1KHzFrequency = 0x011D
-    Equalizer1KHzGain = 0x011E
-    Equalizer2KHzFrequency = 0x012C
-    Equalizer2KHzGain = 0x012D
-    Equalizer4KHzFrequency = 0x0120
-    Equalizer4KHzGain = 0x0121
-    Equalizer8KHzFrequency = 0x0109
-    Equalizer8KHzGain = 0x010A
-    Equalizer16KHzFrequency = 0x012F
-    Equalizer16KHzGain = 0x0130
-    CompressorThreshold = 0x013D
-    CompressorRatio = 0x013C
-    CompressorAttack = 0x013E
-    CompressorRelease = 0x013F
-    CompressorMakeUpGain = 0x0140
-    DeEsser = 0x000B
-    ReverbAmount = 0x0076
-    ReverbDecay = 0x002F
-    ReverbEarlyLevel = 0x0037
-    ReverbTailLevel = 0x0039  # Always sent as 0.
-    ReverbPredelay = 0x0030
-    ReverbLowColor = 0x0032
-    ReverbHighColor = 0x0033
-    ReverbHighFactor = 0x0034
-    ReverbDiffuse = 0x0031
-    ReverbModSpeed = 0x0035
-    ReverbModDepth = 0x0036
-    ReverbType = 0x002E
-    EchoAmount = 0x0075
-    EchoFeedback = 0x0028
-    EchoTempo = 0x001F
-    EchoDelayL = 0x0022
-    EchoDelayR = 0x0023
-    EchoFeedbackL = 0x0024
-    EchoFeedbackR = 0x0025
-    EchoXFBLtoR = 0x0026
-    EchoXFBRtoL = 0x0027
-    EchoSource = 0x001E
-    EchoDivL = 0x0020
-    EchoDivR = 0x0021
-    EchoFilterStyle = 0x002A
-    PitchAmount = 0x005D
-    PitchCharacter = 0x0167
-    PitchThreshold = 0x0159
-    GenderAmount = 0x0060
-    MegaphoneAmount = 0x003C
-    MegaphonePostGain = 0x0040
-    MegaphoneStyle = 0x003A
-    MegaphoneHP = 0x003D
-    MegaphoneLP = 0x003E
-    MegaphonePreGain = 0x003F
-    MegaphoneDistType = 0x0041
-    MegaphonePresenceGain = 0x0042
-    MegaphonePresenceFC = 0x0043
-    MegaphonePresenceBW = 0x0044
-    MegaphoneBeatboxEnable = 0x0045
-    MegaphoneFilterControl = 0x0046
-    MegaphoneFilter = 0x0047
-    MegaphoneDrivePotGainCompMid = 0x0048
-    MegaphoneDrivePotGainCompMax = 0x0049
-    RobotLowGain = 0x0134
-    RobotLowFreq = 0x0133
-    RobotLowWidth = 0x0135
-    RobotMidGain = 0x013A
-    RobotMidFreq = 0x0139
-    RobotMidWidth = 0x013B
-    RobotHiGain = 0x0137
-    RobotHiFreq = 0x0136
-    RobotHiWidth = 0x0138
-    RobotWaveform = 0x0147
-    RobotPulseWidth = 0x0146
-    RobotThreshold = 0x0157
-    RobotDryMix = 0x014D
-    RobotStyle = 0x0000
-    HardTuneKeySource = 0x0059  # Always sent as 0.
-    HardTuneAmount = 0x005A
-    HardTuneRate = 0x005C
-    HardTuneWindow = 0x005B
-    HardTuneScale = 0x005E
-    HardTunePitchAmount = 0x005F
-
-    RobotEnabled = 0x014E
-    MegaphoneEnabled = 0x00D7
-    HardTuneEnabled = 0x00D8
-
-    Encoder1Enabled = 0x00D5
-    Encoder2Enabled = 0x00D6
-    Encoder3Enabled = 0x0150
-    Encoder4Enabled = 0x0151
-
-
-class MicrophoneParamKey(Enum):
-    MicType = 0x000
-    DynamicGain = 0x001
-    CondenserGain = 0x002
-    JackGain = 0x003
-    GateThreshold = 0x30200
-    GateAttack = 0x30400
-    GateRelease = 0x30600
-    GateAttenuation = 0x30900
-    CompressorThreshold = 0x60200
-    CompressorRatio = 0x60300
-    CompressorAttack = 0x60400
-    CompressorRelease = 0x60600
-    CompressorMakeUpGain = 0x60700
-    BleepLevel = 0x70100
-
-    """
-     These are the values for the GoXLR mini, it seems there's a difference in how the two
-     are setup, The Mini does EQ via mic parameters, where as the full does it via effects.
-    """
-    Equalizer90HzFrequency = 0x40000
-    Equalizer90HzGain = 0x40001
-    Equalizer250HzFrequency = 0x40003
-    Equalizer250HzGain = 0x40004
-    Equalizer500HzFrequency = 0x40006
-    Equalizer500HzGain = 0x40007
-    Equalizer1KHzFrequency = 0x50000
-    Equalizer1KHzGain = 0x50001
-    Equalizer3KHzFrequency = 0x50003
-    Equalizer3KHzGain = 0x50004
-    Equalizer8KHzFrequency = 0x50006
-    Equalizer8KHzGain = 0x50007
-
-
-class FaderDisplayStyle(Enum):
-    TwoColour = 1
-    Gradient = 2
-    Meter = 3
-    GradientMeter = 4
-
-
-class Button(Enum):
-    # These are all the buttons from the GoXLR Mini.
-    Fader1Mute = 1
-    Fader2Mute = 2
-    Fader3Mute = 3
-    Fader4Mute = 4
-    Bleep = 5
-    Cough = 6
-
-    # The rest are GoXLR Full Buttons. On the mini, they will simply be ignored.
-    EffectSelect1 = 7
-    EffectSelect2 = 8
-    EffectSelect3 = 9
-    EffectSelect4 = 10
-    EffectSelect5 = 11
-    EffectSelect6 = 12
-
-    # FX Button labelled as 'fxClear' in config?
-    EffectFx = 13
-    EffectMegaphone = 14
-    EffectRobot = 15
-    EffectHardTune = 16
-
-    SamplerSelectA = 17
-    SamplerSelectB = 18
-    SamplerSelectC = 19
-
-    SamplerTopLeft = 20
-    SamplerTopRight = 21
-    SamplerBottomLeft = 22
-    SamplerBottomRight = 23
-    SamplerClear = 24
-
-
-class SimpleColourTarget(Enum):
-    Global = 1
-    Accent = 2
-    Scribble1 = 3
-    Scribble2 = 4
-    Scribble3 = 5
-    Scribble4 = 6
-
-
-class SamplerColourTarget(Enum):
-    SamplerSelectA = 1
-    SamplerSelectB = 2
-    SamplerSelectC = 3
-
-
-class EncoderColourTarget(Enum):
-    Reverb = 1
-    Pitch = 2
-    Echo = 3
-    Gender = 4
-
-
-class ButtonColourGroup(Enum):
-    FaderMute = 1
-    EffectSelector = 2
-    EffectTypes = 3
-
-
-class ButtonColourOffStyle(Enum):
-    Dimmed = 1
-    Colour2 = 2
-    DimmedColour2 = 3
-
-
-class MuteFunction(Enum):
-    All = 1
-    ToStream = 2
-    ToVoiceChat = 3
-    ToPhones = 4
-    ToLineOut = 5
-
-
-class MicrophoneType(Enum):
-    Dynamic = 1
-    Condenser = 2
-    Jack = 3
-
-
-class EffectBankPreset(Enum):
-    Preset1 = 1
-    Preset2 = 2
-    Preset3 = 3
-    Preset4 = 4
-    Preset5 = 5
-    Preset6 = 6
-
-
-class SampleBank(Enum):
-    A = 1
-    B = 2
-    C = 3
-
-
-class MiniEqFrequency(Enum):
-    Equalizer90Hz = 1
-    Equalizer250Hz = 2
-    Equalizer500Hz = 3
-    Equalizer1KHz = 4
-    Equalizer3KHz = 5
-    Equalizer8KHz = 6
-
-
-class EqFrequency(Enum):
-    Equalizer31Hz = 1
-    Equalizer63Hz = 2
-    Equalizer125Hz = 3
-    Equalizer250Hz = 4
-    Equalizer500Hz = 5
-    Equalizer1KHz = 6
-    Equalizer2KHz = 7
-    Equalizer4KHz = 8
-    Equalizer8KHz = 9
-    Equalizer16KHz = 10
-
-
-class CompressorRatio(Enum):
-    Ratio1_0 = 1
-    Ratio1_1 = 2
-    Ratio1_2 = 3
-    Ratio1_4 = 4
-    Ratio1_6 = 5
-    Ratio1_8 = 6
-    Ratio2_0 = 7
-    Ratio2_5 = 8
-    Ratio3_2 = 9
-    Ratio4_0 = 10
-    Ratio5_6 = 11
-    Ratio8_0 = 12
-    Ratio16_0 = 13
-    Ratio32_0 = 14
-    Ratio64_0 = 15
-
-
-class GateTime(Enum):
-    Gate10ms = 1
-    Gate20ms = 2
-    Gate30ms = 3
-    Gate40ms = 4
-    Gate50ms = 5
-    Gate60ms = 6
-    Gate70ms = 7
-    Gate80ms = 8
-    Gate90ms = 9
-    Gate100ms = 10
-    Gate110ms = 11
-    Gate120ms = 12
-    Gate130ms = 13
-    Gate140ms = 14
-    Gate150ms = 15
-    Gate160ms = 16
-    Gate170ms = 17
-    Gate180ms = 18
-    Gate190ms = 19
-    Gate200ms = 20
-    Gate250ms = 21
-    Gate300ms = 22
-    Gate350ms = 23
-    Gate400ms = 24
-    Gate450ms = 25
-    Gate500ms = 26
-    Gate550ms = 27
-    Gate600ms = 28
-    Gate650ms = 29
-    Gate700ms = 30
-    Gate750ms = 31
-    Gate800ms = 32
-    Gate850ms = 33
-    Gate900ms = 34
-    Gate950ms = 35
-    Gate1000ms = 36
-    Gate1100ms = 37
-    Gate1200ms = 38
-    Gate1300ms = 39
-    Gate1400ms = 40
-    Gate1500ms = 41
-    Gate1600ms = 42
-    Gate1700ms = 43
-    Gate1800ms = 44
-    Gate1900ms = 45
-    Gate2000ms = 46
-
-
-class CompressorAttackTime(Enum):
-    Comp0ms = 1
-    Comp2ms = 2
-    Comp3ms = 3
-    Comp4ms = 4
-    Comp5ms = 5
-    Comp6ms = 6
-    Comp7ms = 7
-    Comp8ms = 8
-    Comp9ms = 9
-    Comp10ms = 10
-    Comp12ms = 11
-    Comp14ms = 12
-    Comp16ms = 13
-    Comp18ms = 14
-    Comp20ms = 15
-    Comp23ms = 16
-    Comp26ms = 17
-    Comp30ms = 18
-    Comp35ms = 19
-    Comp40ms = 20
-
-
-class CompressorReleaseTime(Enum):
-    Comp0ms = 1
-    Comp15ms = 2
-    Comp25ms = 3
-    Comp35ms = 4
-    Comp45ms = 5
-    Comp55ms = 6
-    Comp65ms = 7
-    Comp75ms = 8
-    Comp85ms = 9
-    Comp100ms = 10
-    Comp115ms = 11
-    Comp140ms = 12
-    Comp170ms = 13
-    Comp230ms = 14
-    Comp340ms = 15
-    Comp680ms = 16
-    Comp1000ms = 17
-    Comp1500ms = 18
-    Comp2000ms = 19
-    Comp3000ms = 20
-
-
-class ReverbStyle(Enum):
-    Library = 1
-    DarkBloom = 2
-    MusicClub = 3
-    RealPlate = 4
-    Chapel = 5
-    HockeyArena = 6
-
-
-class EchoStyle(Enum):
-    Quarter = 1
-    Eighth = 2
-    Triplet = 3
-    PingPong = 4
-    ClassicSlap = 5
-    MultiTap = 6
-
-
-class PitchStyle(Enum):
-    Narrow = 1
-    Wide = 2
-
-
-class GenderStyle(Enum):
-    Narrow = 1
-    Medium = 2
-    Wide = 3
-
-
-class MegaphoneStyle(Enum):
-    Megaphone = 1
-    Radio = 2
-    OnThePhone = 3
-    Overdrive = 4
-    BuzzCutt = 5
-    Tweed = 6
-
-
-class RobotStyle(Enum):
-    Robot1 = 1
-    Robot2 = 2
-    Robot3 = 3
-
-
-class RobotRange(Enum):
-    Low = 1
-    Medium = 2
-    High = 3
-
-
-class HardTuneStyle(Enum):
-    Natural = 1
-    Medium = 2
-    Hard = 3
-
-
-class HardTuneSource(Enum):
-    All = 1
-    Music = 2
-    Game = 3
-    LineIn = 4
-    System = 5
-
-
-class SampleButton(Enum):
-    TopLeft = 1
-    TopRight = 2
-    BottomLeft = 3
-    BottomRight = 4
-
-
-class SamplePlaybackMode(Enum):
-    PlayNext = 1
-    PlayStop = 2
-    PlayFade = 3
-    StopOnRelease = 4
-    FadeOnRelease = 5
-    Loop = 6
-
-
-class SamplePlayOrder(Enum):
-    Sequential = 1
-    Random = 2
-
-
-class DisplayMode(Enum):
-    Simple = 1
-    Advanced = 2
-
-
-class DisplayModeComponent(Enum):
-    NoiseGate = 1
-    Equaliser = 2
-    Compressor = 3
-    EqFineTune = 4
-
-
-class MuteState(Enum):
-    Unmuted = 1
-    MutedToX = 2
-    MutedToAll = 3
-
-
-class AnimationMode(Enum):
-    RetroRainbow = 1
-    RainbowDark = 2
-    RainbowBright = 3
-    Simple = 4
-    Ripple = 5
-    NONE = 6
-
-
-class WaterfallDirection(Enum):
-    Down = 1
-    Up = 2
-    Off = 3
+from enum import Enum
+
+# Enumerators used by the GoXLR Utility Daemon. (with slight name changes)
+
+
+class PathType(Enum):
+    Profiles = 1
+    MicProfiles = 2
+    Presets = 3
+    Samples = 4
+    Icons = 5
+    Logs = 6
+
+
+class LogLevel(Enum):
+    Off = 1
+    Error = 2
+    Warn = 3
+    Info = 4
+    Debug = 5
+    Trace = 6
+
+
+class Channel(Enum):
+    Mic = 1
+    LineIn = 2
+    Console = 3
+    System = 4
+    Game = 5
+    Chat = 6
+    Sample = 7
+    Music = 8
+    Headphones = 9
+    MicMonitor = 10
+    LineOut = 11
+
+
+class Mix(Enum):
+    A = 1
+    B = 2
+
+
+class SubMixChannel(Enum):
+    Mic = 1
+    LineIn = 2
+    Console = 3
+    System = 4
+    Game = 5
+    Chat = 6
+    Sample = 7
+    Music = 8
+
+
+class Fader(Enum):
+    A = 1
+    B = 2
+    C = 3
+    D = 4
+
+
+class Encoder(Enum):
+    Pitch = 1
+    Gender = 2
+    Reverb = 3
+    Echo = 4
+
+
+class OutputDevice(Enum):
+    Headphones = 1
+    BroadcastMix = 2
+    ChatMic = 3
+    Sampler = 4
+    LineOut = 5
+
+
+class InputDevice(Enum):
+    Microphone = 1
+    Chat = 2
+    Music = 3
+    Game = 4
+    Console = 5
+    LineIn = 6
+    System = 7
+    Samples = 8
+
+
+class EffectKey(Enum):
+    DisableMic = 0x0158
+    BleepLevel = 0x0073
+    GateMode = 0x0010
+    GateThreshold = 0x0011
+    GateEnabled = 0x0014
+    GateAttenuation = 0x0015
+    GateAttack = 0x0016
+    GateRelease = 0x0017
+    MicCompSelect = 0x014B
+    Equalizer31HzFrequency = 0x0126
+    Equalizer31HzGain = 0x0127
+    Equalizer63HzFrequency = 0x00F8
+    Equalizer63HzGain = 0x00F9
+    Equalizer125HzFrequency = 0x0113
+    Equalizer125HzGain = 0x0114
+    Equalizer250HzFrequency = 0x0129
+    Equalizer250HzGain = 0x012A
+    Equalizer500HzFrequency = 0x0116
+    Equalizer500HzGain = 0x0117
+    Equalizer1KHzFrequency = 0x011D
+    Equalizer1KHzGain = 0x011E
+    Equalizer2KHzFrequency = 0x012C
+    Equalizer2KHzGain = 0x012D
+    Equalizer4KHzFrequency = 0x0120
+    Equalizer4KHzGain = 0x0121
+    Equalizer8KHzFrequency = 0x0109
+    Equalizer8KHzGain = 0x010A
+    Equalizer16KHzFrequency = 0x012F
+    Equalizer16KHzGain = 0x0130
+    CompressorThreshold = 0x013D
+    CompressorRatio = 0x013C
+    CompressorAttack = 0x013E
+    CompressorRelease = 0x013F
+    CompressorMakeUpGain = 0x0140
+    DeEsser = 0x000B
+    ReverbAmount = 0x0076
+    ReverbDecay = 0x002F
+    ReverbEarlyLevel = 0x0037
+    ReverbTailLevel = 0x0039  # Always sent as 0.
+    ReverbPredelay = 0x0030
+    ReverbLowColor = 0x0032
+    ReverbHighColor = 0x0033
+    ReverbHighFactor = 0x0034
+    ReverbDiffuse = 0x0031
+    ReverbModSpeed = 0x0035
+    ReverbModDepth = 0x0036
+    ReverbType = 0x002E
+    EchoAmount = 0x0075
+    EchoFeedback = 0x0028
+    EchoTempo = 0x001F
+    EchoDelayL = 0x0022
+    EchoDelayR = 0x0023
+    EchoFeedbackL = 0x0024
+    EchoFeedbackR = 0x0025
+    EchoXFBLtoR = 0x0026
+    EchoXFBRtoL = 0x0027
+    EchoSource = 0x001E
+    EchoDivL = 0x0020
+    EchoDivR = 0x0021
+    EchoFilterStyle = 0x002A
+    PitchAmount = 0x005D
+    PitchCharacter = 0x0167
+    PitchThreshold = 0x0159
+    GenderAmount = 0x0060
+    MegaphoneAmount = 0x003C
+    MegaphonePostGain = 0x0040
+    MegaphoneStyle = 0x003A
+    MegaphoneHP = 0x003D
+    MegaphoneLP = 0x003E
+    MegaphonePreGain = 0x003F
+    MegaphoneDistType = 0x0041
+    MegaphonePresenceGain = 0x0042
+    MegaphonePresenceFC = 0x0043
+    MegaphonePresenceBW = 0x0044
+    MegaphoneBeatboxEnable = 0x0045
+    MegaphoneFilterControl = 0x0046
+    MegaphoneFilter = 0x0047
+    MegaphoneDrivePotGainCompMid = 0x0048
+    MegaphoneDrivePotGainCompMax = 0x0049
+    RobotLowGain = 0x0134
+    RobotLowFreq = 0x0133
+    RobotLowWidth = 0x0135
+    RobotMidGain = 0x013A
+    RobotMidFreq = 0x0139
+    RobotMidWidth = 0x013B
+    RobotHiGain = 0x0137
+    RobotHiFreq = 0x0136
+    RobotHiWidth = 0x0138
+    RobotWaveform = 0x0147
+    RobotPulseWidth = 0x0146
+    RobotThreshold = 0x0157
+    RobotDryMix = 0x014D
+    RobotStyle = 0x0000
+    HardTuneKeySource = 0x0059  # Always sent as 0.
+    HardTuneAmount = 0x005A
+    HardTuneRate = 0x005C
+    HardTuneWindow = 0x005B
+    HardTuneScale = 0x005E
+    HardTunePitchAmount = 0x005F
+
+    RobotEnabled = 0x014E
+    MegaphoneEnabled = 0x00D7
+    HardTuneEnabled = 0x00D8
+
+    Encoder1Enabled = 0x00D5
+    Encoder2Enabled = 0x00D6
+    Encoder3Enabled = 0x0150
+    Encoder4Enabled = 0x0151
+
+
+class MicrophoneParamKey(Enum):
+    MicType = 0x000
+    DynamicGain = 0x001
+    CondenserGain = 0x002
+    JackGain = 0x003
+    GateThreshold = 0x30200
+    GateAttack = 0x30400
+    GateRelease = 0x30600
+    GateAttenuation = 0x30900
+    CompressorThreshold = 0x60200
+    CompressorRatio = 0x60300
+    CompressorAttack = 0x60400
+    CompressorRelease = 0x60600
+    CompressorMakeUpGain = 0x60700
+    BleepLevel = 0x70100
+
+    """
+     These are the values for the GoXLR mini, it seems there's a difference in how the two
+     are setup, The Mini does EQ via mic parameters, where as the full does it via effects.
+    """
+    Equalizer90HzFrequency = 0x40000
+    Equalizer90HzGain = 0x40001
+    Equalizer250HzFrequency = 0x40003
+    Equalizer250HzGain = 0x40004
+    Equalizer500HzFrequency = 0x40006
+    Equalizer500HzGain = 0x40007
+    Equalizer1KHzFrequency = 0x50000
+    Equalizer1KHzGain = 0x50001
+    Equalizer3KHzFrequency = 0x50003
+    Equalizer3KHzGain = 0x50004
+    Equalizer8KHzFrequency = 0x50006
+    Equalizer8KHzGain = 0x50007
+
+
+class FaderDisplayStyle(Enum):
+    TwoColour = 1
+    Gradient = 2
+    Meter = 3
+    GradientMeter = 4
+
+
+class Button(Enum):
+    # These are all the buttons from the GoXLR Mini.
+    Fader1Mute = 1
+    Fader2Mute = 2
+    Fader3Mute = 3
+    Fader4Mute = 4
+    Bleep = 5
+    Cough = 6
+
+    # The rest are GoXLR Full Buttons. On the mini, they will simply be ignored.
+    EffectSelect1 = 7
+    EffectSelect2 = 8
+    EffectSelect3 = 9
+    EffectSelect4 = 10
+    EffectSelect5 = 11
+    EffectSelect6 = 12
+
+    # FX Button labelled as 'fxClear' in config?
+    EffectFx = 13
+    EffectMegaphone = 14
+    EffectRobot = 15
+    EffectHardTune = 16
+
+    SamplerSelectA = 17
+    SamplerSelectB = 18
+    SamplerSelectC = 19
+
+    SamplerTopLeft = 20
+    SamplerTopRight = 21
+    SamplerBottomLeft = 22
+    SamplerBottomRight = 23
+    SamplerClear = 24
+
+
+class SimpleColourTarget(Enum):
+    Global = 1
+    Accent = 2
+    Scribble1 = 3
+    Scribble2 = 4
+    Scribble3 = 5
+    Scribble4 = 6
+
+
+class SamplerColourTarget(Enum):
+    SamplerSelectA = 1
+    SamplerSelectB = 2
+    SamplerSelectC = 3
+
+
+class EncoderColourTarget(Enum):
+    Reverb = 1
+    Pitch = 2
+    Echo = 3
+    Gender = 4
+
+
+class ButtonColourGroup(Enum):
+    FaderMute = 1
+    EffectSelector = 2
+    EffectTypes = 3
+
+
+class ButtonColourOffStyle(Enum):
+    Dimmed = 1
+    Colour2 = 2
+    DimmedColour2 = 3
+
+
+class MuteFunction(Enum):
+    All = 1
+    ToStream = 2
+    ToVoiceChat = 3
+    ToPhones = 4
+    ToLineOut = 5
+
+
+class MicrophoneType(Enum):
+    Dynamic = 1
+    Condenser = 2
+    Jack = 3
+
+
+class EffectBankPreset(Enum):
+    Preset1 = 1
+    Preset2 = 2
+    Preset3 = 3
+    Preset4 = 4
+    Preset5 = 5
+    Preset6 = 6
+
+
+class SampleBank(Enum):
+    A = 1
+    B = 2
+    C = 3
+
+
+class MiniEqFrequency(Enum):
+    Equalizer90Hz = 1
+    Equalizer250Hz = 2
+    Equalizer500Hz = 3
+    Equalizer1KHz = 4
+    Equalizer3KHz = 5
+    Equalizer8KHz = 6
+
+
+class EqFrequency(Enum):
+    Equalizer31Hz = 1
+    Equalizer63Hz = 2
+    Equalizer125Hz = 3
+    Equalizer250Hz = 4
+    Equalizer500Hz = 5
+    Equalizer1KHz = 6
+    Equalizer2KHz = 7
+    Equalizer4KHz = 8
+    Equalizer8KHz = 9
+    Equalizer16KHz = 10
+
+
+class CompressorRatio(Enum):
+    Ratio1_0 = 1
+    Ratio1_1 = 2
+    Ratio1_2 = 3
+    Ratio1_4 = 4
+    Ratio1_6 = 5
+    Ratio1_8 = 6
+    Ratio2_0 = 7
+    Ratio2_5 = 8
+    Ratio3_2 = 9
+    Ratio4_0 = 10
+    Ratio5_6 = 11
+    Ratio8_0 = 12
+    Ratio16_0 = 13
+    Ratio32_0 = 14
+    Ratio64_0 = 15
+
+
+class GateTime(Enum):
+    Gate10ms = 1
+    Gate20ms = 2
+    Gate30ms = 3
+    Gate40ms = 4
+    Gate50ms = 5
+    Gate60ms = 6
+    Gate70ms = 7
+    Gate80ms = 8
+    Gate90ms = 9
+    Gate100ms = 10
+    Gate110ms = 11
+    Gate120ms = 12
+    Gate130ms = 13
+    Gate140ms = 14
+    Gate150ms = 15
+    Gate160ms = 16
+    Gate170ms = 17
+    Gate180ms = 18
+    Gate190ms = 19
+    Gate200ms = 20
+    Gate250ms = 21
+    Gate300ms = 22
+    Gate350ms = 23
+    Gate400ms = 24
+    Gate450ms = 25
+    Gate500ms = 26
+    Gate550ms = 27
+    Gate600ms = 28
+    Gate650ms = 29
+    Gate700ms = 30
+    Gate750ms = 31
+    Gate800ms = 32
+    Gate850ms = 33
+    Gate900ms = 34
+    Gate950ms = 35
+    Gate1000ms = 36
+    Gate1100ms = 37
+    Gate1200ms = 38
+    Gate1300ms = 39
+    Gate1400ms = 40
+    Gate1500ms = 41
+    Gate1600ms = 42
+    Gate1700ms = 43
+    Gate1800ms = 44
+    Gate1900ms = 45
+    Gate2000ms = 46
+
+
+class CompressorAttackTime(Enum):
+    Comp0ms = 1
+    Comp2ms = 2
+    Comp3ms = 3
+    Comp4ms = 4
+    Comp5ms = 5
+    Comp6ms = 6
+    Comp7ms = 7
+    Comp8ms = 8
+    Comp9ms = 9
+    Comp10ms = 10
+    Comp12ms = 11
+    Comp14ms = 12
+    Comp16ms = 13
+    Comp18ms = 14
+    Comp20ms = 15
+    Comp23ms = 16
+    Comp26ms = 17
+    Comp30ms = 18
+    Comp35ms = 19
+    Comp40ms = 20
+
+
+class CompressorReleaseTime(Enum):
+    Comp0ms = 1
+    Comp15ms = 2
+    Comp25ms = 3
+    Comp35ms = 4
+    Comp45ms = 5
+    Comp55ms = 6
+    Comp65ms = 7
+    Comp75ms = 8
+    Comp85ms = 9
+    Comp100ms = 10
+    Comp115ms = 11
+    Comp140ms = 12
+    Comp170ms = 13
+    Comp230ms = 14
+    Comp340ms = 15
+    Comp680ms = 16
+    Comp1000ms = 17
+    Comp1500ms = 18
+    Comp2000ms = 19
+    Comp3000ms = 20
+
+
+class ReverbStyle(Enum):
+    Library = 1
+    DarkBloom = 2
+    MusicClub = 3
+    RealPlate = 4
+    Chapel = 5
+    HockeyArena = 6
+
+
+class EchoStyle(Enum):
+    Quarter = 1
+    Eighth = 2
+    Triplet = 3
+    PingPong = 4
+    ClassicSlap = 5
+    MultiTap = 6
+
+
+class PitchStyle(Enum):
+    Narrow = 1
+    Wide = 2
+
+
+class GenderStyle(Enum):
+    Narrow = 1
+    Medium = 2
+    Wide = 3
+
+
+class MegaphoneStyle(Enum):
+    Megaphone = 1
+    Radio = 2
+    OnThePhone = 3
+    Overdrive = 4
+    BuzzCutt = 5
+    Tweed = 6
+
+
+class RobotStyle(Enum):
+    Robot1 = 1
+    Robot2 = 2
+    Robot3 = 3
+
+
+class RobotRange(Enum):
+    Low = 1
+    Medium = 2
+    High = 3
+
+
+class HardTuneStyle(Enum):
+    Natural = 1
+    Medium = 2
+    Hard = 3
+
+
+class HardTuneSource(Enum):
+    All = 1
+    Music = 2
+    Game = 3
+    LineIn = 4
+    System = 5
+
+
+class SampleButton(Enum):
+    TopLeft = 1
+    TopRight = 2
+    BottomLeft = 3
+    BottomRight = 4
+
+
+class SamplePlaybackMode(Enum):
+    PlayNext = 1
+    PlayStop = 2
+    PlayFade = 3
+    StopOnRelease = 4
+    FadeOnRelease = 5
+    Loop = 6
+
+
+class SamplePlayOrder(Enum):
+    Sequential = 1
+    Random = 2
+
+
+class DisplayMode(Enum):
+    Simple = 1
+    Advanced = 2
+
+
+class DisplayModeComponent(Enum):
+    NoiseGate = 1
+    Equaliser = 2
+    Compressor = 3
+    EqFineTune = 4
+
+
+class MuteState(Enum):
+    Unmuted = 1
+    MutedToX = 2
+    MutedToAll = 3
+
+
+class AnimationMode(Enum):
+    RetroRainbow = 1
+    RainbowDark = 2
+    RainbowBright = 3
+    Simple = 4
+    Ripple = 5
+    NONE = 6
+
+
+class WaterfallDirection(Enum):
+    Down = 1
+    Up = 2
+    Off = 3
+
+
+class DeviceType(Enum):
+    Unknown = 1
+    Full = 2
+    Mini = 3
```

### Comparing `goxlr-1.3.0/goxlr.egg-info/PKG-INFO` & `goxlr-1.4.0/goxlr.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-Metadata-Version: 2.1
-Name: goxlr
-Version: 1.3.0
-Summary: A Python wrapper for the GoXLR Utility API.
-Home-page: https://github.com/samcarsonx/goxlr
-Author: Sam Carson
-Author-email: sam@samcarson.co.uk
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE-3RD-PARTY.txt
-License-File: LICENSE.txt
-
-# GoXLR Utility API Python Wrapper
-
- [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
-
-A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio. Disclaimer: This project is not affiliated with the GoXLR brand or TC-Helicon in any way, shape, or form. This is a third-party package made for fun and educational purposes.
-
-## Features
-- Asynchronous connection to the GoXLR utility daemon
-- All methods have been translated to Python
-- Handy enumerators for everything
-- Very simple and easy to get started
-
-## Installation
-```shell
-pip install goxlr
-```
-
-## Getting Started
-Here's some sample code to get started with this package that pings the utility's daemon.
-```py
-import asyncio
-
-from goxlr import GoXLR
-from goxlr.types import Fader, Channel
-
-async def main():
-    async with GoXLR() as xlr:
-        await xlr.set_fader(Fader.A, Channel.Headphones)
-        await xlr.set_volume(Channel.Headphones, 127)
-
-if __name__ == "__main__":
-    asyncio.run(main())
-```
-
-You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
-```py
-async def main():
-    xlr = GoXLR()
-    await xlr.open()
-
-    ping = await xlr.ping()
-    print(ping)  # Ok
-
-    await xlr.close()
-```
-
-## Contributing
-Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
-
-## Documentation
-Please visit the [documentation](https://goxlr.readthedocs.io/en/latest/) for more information on how to use this package.
+Metadata-Version: 2.1
+Name: goxlr
+Version: 1.4.0
+Summary: A Python wrapper for the GoXLR Utility API.
+Home-page: https://github.com/samcarsonx/goxlr
+Author: Sam Carson
+Author-email: sam@samcarson.co.uk
+License: MIT
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE-3RD-PARTY.txt
+License-File: LICENSE.txt
+
+# GoXLR Utility API Python Wrapper
+
+ [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
+
+A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio. Disclaimer: This project is not affiliated with the GoXLR brand or TC-Helicon in any way, shape, or form. This is a third-party package made for fun and educational purposes.
+
+## Features
+- Asynchronous connection to the GoXLR utility daemon
+- All methods have been translated to Python
+- Handy enumerators for everything
+- Very simple and easy to get started
+
+## Installation
+```shell
+pip install goxlr
+```
+
+## Getting Started
+Here's some sample code to get started with this package that pings the utility's daemon.
+```py
+import asyncio
+
+from goxlr import GoXLR
+from goxlr.types import Fader, Channel
+
+async def main():
+    async with GoXLR() as xlr:
+        await xlr.set_fader(Fader.A, Channel.Headphones)
+        await xlr.set_volume(Channel.Headphones, 127)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
+```py
+async def main():
+    xlr = GoXLR()
+    await xlr.open()
+
+    ping = await xlr.ping()
+    print(ping)  # Ok
+
+    await xlr.close()
+```
+
+## Contributing
+Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
+
+## Documentation
+Please visit the [documentation](https://goxlr.readthedocs.io/en/latest/) for more information on how to use this package.
```

### Comparing `goxlr-1.3.0/setup.py` & `goxlr-1.4.0/setup.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from setuptools import setup, find_packages
-
-# Thanks to https://stackoverflow.com/a/7071358
-import re
-
-VERSIONFILE = "goxlr/_version.py"
-verstrline = open(VERSIONFILE, "rt").read()
-VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
-mo = re.search(VSRE, verstrline, re.M)
-if mo:
-    verstr = mo.group(1)
-else:
-    raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
-
-setup(
-    name="goxlr",
-    version=verstr,
-    description="A Python wrapper for the GoXLR Utility API.",
-    url="https://github.com/samcarsonx/goxlr",
-    author="Sam Carson",
-    author_email="sam@samcarson.co.uk",
-    license="MIT",
-    packages=find_packages(),
-    install_requires=["asyncio", "websockets"],
-    python_requires=">=3.10",
-    long_description=open("README.md").read(),
-    long_description_content_type="text/markdown",
-)
+from setuptools import setup, find_packages
+
+# Thanks to https://stackoverflow.com/a/7071358
+import re
+
+VERSIONFILE = "goxlr/_version.py"
+verstrline = open(VERSIONFILE, "rt").read()
+VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
+mo = re.search(VSRE, verstrline, re.M)
+if mo:
+    verstr = mo.group(1)
+else:
+    raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
+
+setup(
+    name="goxlr",
+    version=verstr,
+    description="A Python wrapper for the GoXLR Utility API.",
+    url="https://github.com/samcarsonx/goxlr",
+    author="Sam Carson",
+    author_email="sam@samcarson.co.uk",
+    license="MIT",
+    packages=find_packages(),
+    install_requires=["asyncio", "websockets"],
+    python_requires=">=3.10",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+)
```

