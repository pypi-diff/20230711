# Comparing `tmp/pywa-0.0.1rc19-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 32686 bytes, number of entries: 21
+Zip file size: 32671 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-10 21:35 pywa/__version__.py
--rw-rw-r--  2.0 unx    14440 b- defN 23-Jul-09 17:48 pywa/api.py
--rw-rw-r--  2.0 unx    29315 b- defN 23-Jul-09 21:41 pywa/client.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-10 21:55 pywa/__version__.py
+-rw-rw-r--  2.0 unx    14220 b- defN 23-Jul-10 21:52 pywa/api.py
+-rw-rw-r--  2.0 unx    28886 b- defN 23-Jul-10 21:50 pywa/client.py
 -rw-rw-r--  2.0 unx     7191 b- defN 23-Jul-03 08:28 pywa/errors.py
 -rw-rw-r--  2.0 unx    21046 b- defN 23-Jul-10 21:34 pywa/filters.py
 -rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-02 08:19 pywa/handlers.py
 -rw-rw-r--  2.0 unx      873 b- defN 23-Jul-09 12:48 pywa/utils.py
 -rw-rw-r--  2.0 unx     4449 b- defN 23-Jul-09 13:09 pywa/webhook.py
 -rw-rw-r--  2.0 unx      336 b- defN 23-Jul-07 13:20 pywa/types/__init__.py
--rw-rw-r--  2.0 unx     9301 b- defN 23-Jul-09 17:41 pywa/types/base_update.py
+-rw-rw-r--  2.0 unx     8951 b- defN 23-Jul-10 21:50 pywa/types/base_update.py
 -rw-rw-r--  2.0 unx     5653 b- defN 23-Jul-07 13:38 pywa/types/callback.py
 -rw-rw-r--  2.0 unx     4609 b- defN 23-Jul-09 14:47 pywa/types/media.py
 -rw-rw-r--  2.0 unx    11234 b- defN 23-Jul-09 17:38 pywa/types/message.py
 -rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-07 13:28 pywa/types/message_status.py
 -rw-rw-r--  2.0 unx     9156 b- defN 23-Jul-07 13:38 pywa/types/others.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/RECORD
-21 files, 128648 bytes uncompressed, 30160 bytes compressed:  76.6%
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-10 21:55 pywa-0.0.1rc20.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-10 21:55 pywa-0.0.1rc20.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 21:55 pywa-0.0.1rc20.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-10 21:55 pywa-0.0.1rc20.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-10 21:55 pywa-0.0.1rc20.dist-info/RECORD
+21 files, 127649 bytes uncompressed, 30145 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pywa/types/message_status.py
 Comment: 
 
 Filename: pywa/types/others.py
 Comment: 
 
-Filename: pywa-0.0.1rc19.dist-info/LICENSE
+Filename: pywa-0.0.1rc20.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc19.dist-info/METADATA
+Filename: pywa-0.0.1rc20.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc19.dist-info/WHEEL
+Filename: pywa-0.0.1rc20.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc19.dist-info/top_level.txt
+Filename: pywa-0.0.1rc20.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc19.dist-info/RECORD
+Filename: pywa-0.0.1rc20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc19"
+__version__ = "0.0.1rc20"
```

## pywa/api.py

```diff
@@ -209,15 +209,14 @@
         )
 
     def send_media(
             self,
             to: str | int,
             media_id_or_url: str,
             media_type: str,
-            reply_to_message_id: str | None = None,
             **kwargs
     ) -> dict[str, dict | list]:
         """
         Send a media file to a WhatsApp user.
 
         Return example::
 
@@ -227,22 +226,19 @@
                 'messages': [{'id': 'wamid.XXXXXXXXXXXXXXXX=='}]
             }
 
         Args:
             to: The WhatsApp ID of the recipient.
             media_id_or_url: The ID or URL of the media file to send.
             media_type: The type of the media file.
-            reply_to_message_id: The ID of the message to reply to.
             **kwargs: Additional arguments to send with the message.
 
         Returns:
             The sent message.
         """
-        if reply_to_message_id:
-            kwargs["context"] = {"message_id": reply_to_message_id}
         data = {
             **self._common_keys,
             "to": str(to),
             "type": media_type,
             media_type: {
                 "link" if media_id_or_url.startswith(('https:', 'http:')) else "id": media_id_or_url,
                 **{k: v for k, v in kwargs.items() if v is not None}
```

## pywa/client.py

```diff
@@ -324,29 +324,28 @@
             ...     caption="This is an image!",
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
             image: The image to send (either a media ID, URL, file path, bytes, or a open file object).
             caption: The caption of the image (optional, markdown allowed).
-            reply_to_message_id: The message ID to reply to (optional).
+            reply_to_message_id: The message ID to reply to (optional, only works if buttons provided).
             buttons: The buttons to send with the image (optional).
             body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).
             footer: The footer of the message (if buttons is provided, optional, markdown has no effect).
 
         Returns:
             The message ID of the sent image.
         """
         is_url, image = self._resolve_media_param(media=image, mime_type="image/jpeg", file_name="image.jpg")
         if not buttons:
             return self.api.send_media(
                 to=to,
                 media_id_or_url=image,
                 media_type="image",
-                reply_to_message_id=reply_to_message_id,
                 caption=caption,
             )['messages'][0]['id']
         if not body and not caption:
             raise ValueError("Either body or caption must be provided when sending an image with buttons.")
         return self.api.send_interactive_message(
             to=to,
             keyboard=buttons,
@@ -382,29 +381,28 @@
             ...     caption="This is a video",
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
             video: The video to send (either a media ID, URL, file path, bytes, or a open file object).
             caption: The caption of the video (optional, markdown allowed).
-            reply_to_message_id: The message ID to reply to (optional).
+            reply_to_message_id: The message ID to reply to (optional, only works if buttons provided).
             buttons: The buttons to send with the video (optional).
             body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).
             footer: The footer of the message (if buttons is provided, optional, markdown has no effect).
 
         Returns:
             The message ID of the sent message.
         """
         is_url, video = self._resolve_media_param(media=video, mime_type="video/mp4", file_name="video.mp4")
         if not buttons:
             return self.api.send_media(
                 to=to,
                 media_id_or_url=video,
                 media_type="video",
-                reply_to_message_id=reply_to_message_id,
                 caption=caption,
             )['messages'][0]['id']
         if not body and not caption:
             raise ValueError("Either body or caption must be provided when sending a video with buttons.")
         return self.api.send_interactive_message(
             to=to,
             keyboard=buttons,
@@ -444,30 +442,29 @@
 
 
         Args:
             to: The phone ID of the WhatsApp user.
             document: The document to send (either a media ID, URL, file path, bytes, or a open file object).
             file_name: The filename of the document (optional, The extension of the filename will specify what format the document is displayed as in WhatsApp).
             caption: The caption of the document (optional).
-            reply_to_message_id: The message ID to reply to (optional).
+            reply_to_message_id: The message ID to reply to (optional, only works if buttons provided).
             buttons: The buttons to send with the document (optional).
             body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).
             footer: The footer of the message (if buttons is provided, optional, markdown has no effect).
 
         Returns:
             The message ID of the sent message.
         """
         is_url, document = self._resolve_media_param(media=document, mime_type="text/plain",
                                                      file_name=file_name or "file.text")
         if not buttons:
             return self.api.send_media(
                 to=to,
                 media_id_or_url=document,
                 media_type="document",
-                reply_to_message_id=reply_to_message_id,
                 file_name=file_name,
                 caption=caption,
             )['messages'][0]['id']
         if not body and not caption:
             raise ValueError("Either body or caption must be provided when sending a document with buttons.")
         return self.api.send_interactive_message(
             to=to,
@@ -484,47 +481,43 @@
             reply_to_message_id=reply_to_message_id,
         )['messages'][0]['id']
 
     def send_audio(
             self,
             to: str,
             audio: str | bytes | BinaryIO,
-            reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send an audio file to a WhatsApp user.
 
         Example:
 
             >>> wa.send_audio(
             ...     to='1234567890',
             ...     audio='https://example.com/audio.mp3',
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
             audio: The audio file to send (either a media ID, URL, file path, bytes, or a open file object).
-            reply_to_message_id: The message ID to reply to (optional).
 
         Returns:
             The message ID of the sent message.
         """
         _, audio = self._resolve_media_param(media=audio, mime_type="audio/mpeg", file_name="audio.mp3")
         return self.api.send_media(
             to=to,
             media_id_or_url=audio,
             media_type="audio",
-            reply_to_message_id=reply_to_message_id,
         )['messages'][0]['id']
 
     def send_sticker(
             self,
             to: str,
             sticker: str | bytes | BinaryIO,
-            reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send a sticker to a WhatsApp user.
             - A static sticker needs to be 512x512 pixels and cannot exceed 100 KB.
             - An animated sticker must be 512x512 pixels and cannot exceed 500 KB.
 
         Example:
@@ -533,25 +526,23 @@
             ...     to='1234567890',
             ...     sticker='https://example.com/sticker.webp',
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
             sticker: The sticker to send (either a media ID, URL, file path, bytes, or an open file object).
-            reply_to_message_id: The message ID to reply to (optional).
 
         Returns:
             The message ID of the sent message.
         """
         _, sticker = self._resolve_media_param(media=sticker, mime_type="image/webp", file_name="sticker.webp")
         return self.api.send_media(
             to=to,
             media_id_or_url=sticker,
             media_type="sticker",
-            reply_to_message_id=reply_to_message_id,
         )['messages'][0]['id']
 
     def send_reaction(
             self,
             to: str,
             emoji: str,
             message_id: str,
```

## pywa/types/base_update.py

```diff
@@ -162,51 +162,45 @@
             body=body,
             footer=footer
         )
 
     def reply_audio(
             self,
             audio: str | bytes | BinaryIO,
-            quote: bool = False,
     ) -> str:
         """
         Reply to the message with an audio.
 
         Args:
             audio: The audio to reply with.
-            quote: Whether to quote the message (default: False).
 
         Returns:
             The ID of the sent message.
         """
         return self._client.send_audio(
             to=self.sender,
             audio=audio,
-            reply_to_message_id=self.message_id_to_reply if quote else None
         )
 
     def reply_sticker(
             self,
             sticker: str | bytes | BinaryIO,
-            quote: bool = False,
     ) -> str:
         """
         Reply to the message with a sticker.
 
         Args:
             sticker: The sticker to reply with.
-            quote: Whether to quote the message (default: False).
 
         Returns:
             The ID of the sent message.
         """
         return self._client.send_sticker(
             to=self.sender,
             sticker=sticker,
-            reply_to_message_id=self.message_id_to_reply if quote else None
         )
 
     def reply_location(
             self,
             latitude: float,
             longitude: float,
             name: str | None = None,
```

## Comparing `pywa-0.0.1rc19.dist-info/LICENSE` & `pywa-0.0.1rc20.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc19.dist-info/METADATA` & `pywa-0.0.1rc20.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc19
+Version: 0.0.1rc20
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
```

## Comparing `pywa-0.0.1rc19.dist-info/RECORD` & `pywa-0.0.1rc20.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=X4Zu_d6IDlLaJ4dU_U08K496PYIf5zbTpoaQW75fkCc,26
-pywa/api.py,sha256=334CM6QSpzUbJ5-2BKXZg6ZZWyl09VImxMgbKNwUHOk,14440
-pywa/client.py,sha256=joguy-5GgmKvw_2KD8YGzJXb_V0o7DOmKJeP9a8YfVQ,29315
+pywa/__version__.py,sha256=lfTypGubvY4TyYJjlm12sXOHCq-r6XYCJipyYjyyE5Y,26
+pywa/api.py,sha256=xiFBJ-PHNkzN-3HFUXE0YO4xwgTWPDI1PSbafpmRuF0,14220
+pywa/client.py,sha256=pJQKACjZOfY0gO1rDRU7YDVSBjUYnpZH7m4X5FJoVsQ,28886
 pywa/errors.py,sha256=ErB0UGIpIOF5vZXK39WmiSrB_PSYvTJL8PLIp90vTjU,7191
 pywa/filters.py,sha256=thOtWYSeFFmLkTJ-cegfQmOfFT5dxV3PnI9DQo6HY6Y,21046
 pywa/handlers.py,sha256=DTlKr-yvVKpTgh3F0Gsq78gT5XhBIo_VVnYHz3lu25w,1794
 pywa/utils.py,sha256=vIPGDuXFo80xAhv88mboE-rU-uDEv594cAxEPsMrIZg,873
 pywa/webhook.py,sha256=XJEJRKLk8Dg4eJ1qE5_B3bUXu0ugt-0cjWe8C9tbvH4,4449
 pywa/types/__init__.py,sha256=HwhabvWT9b1bgPLnvXBDOmYNTh-FYjCC-ot-rh8xqzo,336
-pywa/types/base_update.py,sha256=Jd3JW8nhFd2ss0ftBjr8mEKw1gVhxlOcbKosPdQwPhA,9301
+pywa/types/base_update.py,sha256=EW5Fl6rWyCfnIzOQVz7PfCvPzDAnvXlVlqqZh-w4w3c,8951
 pywa/types/callback.py,sha256=J7xDPPeGaU_JPpbdyJXJtmVu7hTMMlyquqQI9p95F5w,5653
 pywa/types/media.py,sha256=4T5yOsoZwFmJaTUZf49VnMsXACsGLq1crC6wzSBqanA,4609
 pywa/types/message.py,sha256=zNKvifHA3P89TOxKoV4dLnt-B9jbu7whlP8gdu304Xo,11234
 pywa/types/message_status.py,sha256=wgUlrgTCaKKqEZgVaZt_yYY_PKyJMhBGz-Rh3WaXSB0,1934
 pywa/types/others.py,sha256=UeXSWEY1pekZDVBDacbUsXff_OmYbxbAe9P2o_am4es,9156
-pywa-0.0.1rc19.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc19.dist-info/METADATA,sha256=f44Ly70xc5gSUSjFI8GJMB8gHKvT2j7Mgkwy8yZVPc4,4420
-pywa-0.0.1rc19.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc19.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc19.dist-info/RECORD,,
+pywa-0.0.1rc20.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc20.dist-info/METADATA,sha256=KNfldQMALMS53JQ8jo7yNZ6ewFYb2elipZ-nCtJtY5Q,4420
+pywa-0.0.1rc20.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc20.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc20.dist-info/RECORD,,
```

