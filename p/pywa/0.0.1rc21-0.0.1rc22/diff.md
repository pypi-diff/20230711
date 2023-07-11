# Comparing `tmp/pywa-0.0.1rc21-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc22-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 32782 bytes, number of entries: 21
+Zip file size: 32801 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-11 08:11 pywa/__version__.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-11 09:47 pywa/__version__.py
 -rw-rw-r--  2.0 unx    14220 b- defN 23-Jul-10 21:52 pywa/api.py
 -rw-rw-r--  2.0 unx    29401 b- defN 23-Jul-11 08:06 pywa/client.py
 -rw-rw-r--  2.0 unx     7191 b- defN 23-Jul-03 08:28 pywa/errors.py
 -rw-rw-r--  2.0 unx    21046 b- defN 23-Jul-10 21:34 pywa/filters.py
--rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-02 08:19 pywa/handlers.py
+-rw-rw-r--  2.0 unx     3846 b- defN 23-Jul-11 08:37 pywa/handlers.py
 -rw-rw-r--  2.0 unx      873 b- defN 23-Jul-09 12:48 pywa/utils.py
--rw-rw-r--  2.0 unx     4449 b- defN 23-Jul-09 13:09 pywa/webhook.py
+-rw-rw-r--  2.0 unx     4600 b- defN 23-Jul-11 09:43 pywa/webhook.py
 -rw-rw-r--  2.0 unx      336 b- defN 23-Jul-07 13:20 pywa/types/__init__.py
 -rw-rw-r--  2.0 unx     8951 b- defN 23-Jul-10 21:50 pywa/types/base_update.py
--rw-rw-r--  2.0 unx     5653 b- defN 23-Jul-07 13:38 pywa/types/callback.py
+-rw-rw-r--  2.0 unx     5347 b- defN 23-Jul-11 09:47 pywa/types/callback.py
 -rw-rw-r--  2.0 unx     4609 b- defN 23-Jul-09 14:47 pywa/types/media.py
 -rw-rw-r--  2.0 unx    11234 b- defN 23-Jul-09 17:38 pywa/types/message.py
 -rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-07 13:28 pywa/types/message_status.py
 -rw-rw-r--  2.0 unx     9156 b- defN 23-Jul-07 13:38 pywa/types/others.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-11 08:11 pywa-0.0.1rc21.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-11 08:11 pywa-0.0.1rc21.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 08:11 pywa-0.0.1rc21.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-11 08:11 pywa-0.0.1rc21.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-11 08:11 pywa-0.0.1rc21.dist-info/RECORD
-21 files, 128164 bytes uncompressed, 30256 bytes compressed:  76.4%
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/RECORD
+21 files, 130061 bytes uncompressed, 30275 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pywa/types/message_status.py
 Comment: 
 
 Filename: pywa/types/others.py
 Comment: 
 
-Filename: pywa-0.0.1rc21.dist-info/LICENSE
+Filename: pywa-0.0.1rc22.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc21.dist-info/METADATA
+Filename: pywa-0.0.1rc22.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc21.dist-info/WHEEL
+Filename: pywa-0.0.1rc22.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc21.dist-info/top_level.txt
+Filename: pywa-0.0.1rc22.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc21.dist-info/RECORD
+Filename: pywa-0.0.1rc22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc21"
+__version__ = "0.0.1rc22"
```

## pywa/handlers.py

```diff
@@ -7,14 +7,15 @@
     "ButtonCallbackHandler",
     "SelectionCallbackHandler",
     "RawUpdateHandler",
     "MessageStatusHandler"
 )
 
 from typing import Callable, Any, TYPE_CHECKING
+from pywa.types import Message, CallbackButton, CallbackSelection, MessageStatus
 
 if TYPE_CHECKING:
     from pywa import WhatsApp
 
 
 class Handler:
     """Base class for all handlers."""
@@ -23,49 +24,108 @@
     def __init__(
             self,
             handler: Callable[["WhatsApp", Any], Any],
             *filters: Callable[["WhatsApp", Any], bool]
     ):
         """
         Initialize a new handler.
-
-        Args:
-            handler: The handler function. (gets the WhatsApp instance and the data as
-                arguments)
-            filters: The filters to apply to the handler. (gets the WhatsApp instance and
-                the data as arguments and returns a boolean)
         """
         self.handler = handler
         self.filters = filters
 
     def __call__(self, wa: "WhatsApp", data: Any):
         if all([f(wa, data) for f in self.filters]):
             self.handler(wa, data)
 
 
 class MessageHandler(Handler):
-    """A message handler (e.g. text, image, video, audio, etc.)."""
+    """
+    Handler for incoming messages (text, image, video, etc.).
+
+    Args:
+        handler: The handler function. (gets the "WhatsApp" instance and the message as arguments)
+        filters: The filters to apply to the handler. (gets the "WhatsApp" instance and
+            the message as arguments and returns a boolean)
+    """
     __handler_type__ = "message"
 
+    def __init__(
+            self,
+            handler: Callable[["WhatsApp", Message], Any],
+            *filters: Callable[["WhatsApp", Message], bool]
+    ):
+        super().__init__(handler, *filters)
+
 
 class ButtonCallbackHandler(Handler):
-    """A button click handler."""
+    """
+    A button callback handler.
+
+    Args:
+        handler: The handler function. (gets the "WhatsApp" instance and the callback as arguments)
+        filters: The filters to apply to the handler. (gets the "WhatsApp" instance and
+            the callback as arguments and returns a boolean)
+    """
     __handler_type__ = "button"
 
+    def __init__(
+            self,
+            handler: Callable[["WhatsApp", CallbackButton], Any],
+            *filters: Callable[["WhatsApp", CallbackButton], bool]
+    ):
+        super().__init__(handler, *filters)
+
 
 class SelectionCallbackHandler(Handler):
-    """A selection choice handler."""
-    __handler_type__ = "selection"
+    """
+    A selection callback handler.
 
+    Args:
+        handler: The handler function. (gets the "WhatsApp" instance and the callback as arguments)
+        filters: The filters to apply to the handler. (gets the "WhatsApp" instance and
+    """
+    __handler_type__ = "selection"
 
-class RawUpdateHandler(Handler):
-    """A raw update handler."""
-    __handler_type__ = "raw_update"
+    def __init__(
+            self,
+            handler: Callable[["WhatsApp", CallbackSelection], Any],
+            *filters: Callable[["WhatsApp", CallbackSelection], bool]
+    ):
+        super().__init__(handler, *filters)
 
 
 class MessageStatusHandler(Handler):
     """
-    A message status handler (e.g. delivered, read, failed, etc.).
+    A message status handler.
 
-    **DO NOT USE THIS HANDLER TO SEND MESSAGES, IT WILL CAUSE AN INFINITE LOOP!**
+    Args:
+        handler: The handler function. (gets the "WhatsApp" instance and the message status as arguments)
+        filters: The filters to apply to the handler. (gets the "WhatsApp" instance and
+            the message status as arguments and returns a boolean)
     """
     __handler_type__ = "message_status"
+
+    def __init__(
+            self,
+            handler: Callable[["WhatsApp", MessageStatus], Any],
+            *filters: Callable[["WhatsApp", MessageStatus], bool]
+    ):
+        super().__init__(handler, *filters)
+
+
+class RawUpdateHandler(Handler):
+    """
+    A raw update handler.
+
+    Args:
+        handler: The handler function. (gets the "WhatsApp" instance and the data-dict as arguments)
+        filters: The filters to apply to the handler. (gets the "WhatsApp" instance and
+            the data-dict as arguments and returns a boolean)
+    """
+    __handler_type__ = "raw_update"
+
+    def __init__(
+            self,
+            handler: Callable[["WhatsApp", dict], Any],
+            *filters: Callable[["WhatsApp", dict], bool]
+    ):
+        super().__init__(handler, *filters)
```

## pywa/webhook.py

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
+from pywa.handlers import Handler
+from pywa.handlers import *
 
 """The webhook module contains the Webhook class, which is used to register a webhook to listen for incoming 
 messages."""
 
 import collections
 import threading
-from typing import Union, TYPE_CHECKING, Callable, Any
+from typing import Union, TYPE_CHECKING, Callable, Any, Type
 from pywa.types import Message, CallbackButton, CallbackSelection, MessageStatus
 from pywa.types.base_update import BaseUpdate
 from pywa import utils
 
 if TYPE_CHECKING:
     from pywa import WhatsApp
 
@@ -73,33 +75,33 @@
 
     def call_handlers(self, update: dict) -> None:
         """Call the handlers for the given update."""
         try:
             if not self.filter_updates or (
                     update["entry"][0]["changes"][0]["value"]["metadata"][
                         "phone_number_id"] == self.wa_client.phone_id):
-                for raw_update_handler in self.handlers["raw_update"]:
+                for raw_update_handler in self.handlers[RawUpdateHandler.__handler_type__]:
                     raw_update_handler(self.wa_client, update)
                 update, key = self.convert_dict_to_update(client=self.wa_client, d=update)
                 if key is None:
                     return
-                for handler in self.handlers[key]:
+                for handler in self.handlers[key.__handler_type__]:
                     handler(self.wa_client, update)
         except (KeyError, IndexError):  # the update not send to this phone and filter_updates is True
             pass
 
     @staticmethod
-    def convert_dict_to_update(client: WhatsApp, d: dict) -> tuple[BaseUpdate | None, str | None]:
+    def convert_dict_to_update(client: WhatsApp, d: dict) -> tuple[BaseUpdate | None, Type[Handler] | None]:
         """Convert a webhook dict to a BaseUpdate object."""
         value = d["entry"][0]["changes"][0]["value"]
         if 'messages' in value:
             if value["messages"][0]["type"] != "interactive":
-                return Message.from_dict(client=client, value=value), "message"
+                return Message.from_dict(client=client, value=value), MessageHandler
             else:
                 if value["messages"][0]["interactive"]["type"] == "button_reply":
-                    return CallbackButton.from_dict(client=client, value=value), "button"
+                    return CallbackButton.from_dict(client=client, value=value), ButtonCallbackHandler
                 elif value["messages"][0]["interactive"]["type"] == "list_reply":
-                    return CallbackSelection.from_dict(client=client, value=value), "selection"
+                    return CallbackSelection.from_dict(client=client, value=value), SelectionCallbackHandler
 
         elif 'statuses' in value:
-            return MessageStatus.from_dict(client=client, value=value), "message_status"
+            return MessageStatus.from_dict(client=client, value=value), MessageStatusHandler
         return None, None  # the update is not supported
```

## pywa/types/callback.py

```diff
@@ -24,19 +24,14 @@
         data: The data of the button.
         title: The title of the button.
     """
     reply_to_message: ReplyToMessage
     data: str
     title: str
 
-    @property
-    def message_id_to_reply(self) -> str:
-        """The ID of the message to reply to"""
-        return self.reply_to_message.message_id
-
     @classmethod
     def from_dict(cls, client: WhatsApp, value: dict):
         message = value['messages'][0]
         return cls(
             _client=client,
             id=message['id'],
             metadata=Metadata.from_dict(**value['metadata']),
@@ -66,19 +61,14 @@
         description: The description of the selection (optional).
     """
     reply_to_message: ReplyToMessage
     data: str
     title: str
     description: str | None
 
-    @property
-    def message_id_to_reply(self) -> str:
-        """The ID of the message to reply to"""
-        return self.reply_to_message.message_id
-
     @classmethod
     def from_dict(cls, client: WhatsApp, value: dict):
         message = value['messages'][0]
         return cls(
             _client=client,
             id=message['id'],
             metadata=Metadata.from_dict(**value['metadata']),
```

## Comparing `pywa-0.0.1rc21.dist-info/LICENSE` & `pywa-0.0.1rc22.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc21.dist-info/METADATA` & `pywa-0.0.1rc22.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc21
+Version: 0.0.1rc22
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
```

## Comparing `pywa-0.0.1rc21.dist-info/RECORD` & `pywa-0.0.1rc22.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=2rapHuT1ScRlhX1p0c5B2rUjEhkoKQkhNFXOvhxQKFw,26
+pywa/__version__.py,sha256=D-r2u3eVXoo2azIv3_4s8SdhUBwONufpw963nS514CQ,26
 pywa/api.py,sha256=xiFBJ-PHNkzN-3HFUXE0YO4xwgTWPDI1PSbafpmRuF0,14220
 pywa/client.py,sha256=wZLrY-weLF1qeOVzmXAZ7M0mONm8yP3yWVuoRjSxkzc,29401
 pywa/errors.py,sha256=ErB0UGIpIOF5vZXK39WmiSrB_PSYvTJL8PLIp90vTjU,7191
 pywa/filters.py,sha256=thOtWYSeFFmLkTJ-cegfQmOfFT5dxV3PnI9DQo6HY6Y,21046
-pywa/handlers.py,sha256=DTlKr-yvVKpTgh3F0Gsq78gT5XhBIo_VVnYHz3lu25w,1794
+pywa/handlers.py,sha256=VD3Z3gocBbxRoHXscBkaP8SONt-M9CDVaiL8duWiL9w,3846
 pywa/utils.py,sha256=vIPGDuXFo80xAhv88mboE-rU-uDEv594cAxEPsMrIZg,873
-pywa/webhook.py,sha256=XJEJRKLk8Dg4eJ1qE5_B3bUXu0ugt-0cjWe8C9tbvH4,4449
+pywa/webhook.py,sha256=1IjiwZTYSh5RvRI-DTa2qajVg-tqBQepm_dcHO9rogo,4600
 pywa/types/__init__.py,sha256=HwhabvWT9b1bgPLnvXBDOmYNTh-FYjCC-ot-rh8xqzo,336
 pywa/types/base_update.py,sha256=EW5Fl6rWyCfnIzOQVz7PfCvPzDAnvXlVlqqZh-w4w3c,8951
-pywa/types/callback.py,sha256=J7xDPPeGaU_JPpbdyJXJtmVu7hTMMlyquqQI9p95F5w,5653
+pywa/types/callback.py,sha256=5TkToHezrDTWsHw5-4MyzqXHspQGivfhWWlTcXfZMbk,5347
 pywa/types/media.py,sha256=4T5yOsoZwFmJaTUZf49VnMsXACsGLq1crC6wzSBqanA,4609
 pywa/types/message.py,sha256=zNKvifHA3P89TOxKoV4dLnt-B9jbu7whlP8gdu304Xo,11234
 pywa/types/message_status.py,sha256=wgUlrgTCaKKqEZgVaZt_yYY_PKyJMhBGz-Rh3WaXSB0,1934
 pywa/types/others.py,sha256=UeXSWEY1pekZDVBDacbUsXff_OmYbxbAe9P2o_am4es,9156
-pywa-0.0.1rc21.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc21.dist-info/METADATA,sha256=-WZybU51UEqlHT3XclxzdlWRsGLISD8OZb0AvzsZTBU,4420
-pywa-0.0.1rc21.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc21.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc21.dist-info/RECORD,,
+pywa-0.0.1rc22.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc22.dist-info/METADATA,sha256=ZyLhViD4qEkD8WAulMQTdq3y8WIjkRZoilyXAq13dYI,4420
+pywa-0.0.1rc22.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc22.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc22.dist-info/RECORD,,
```

