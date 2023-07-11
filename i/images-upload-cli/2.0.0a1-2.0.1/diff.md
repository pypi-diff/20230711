# Comparing `tmp/images_upload_cli-2.0.0a1.tar.gz` & `tmp/images_upload_cli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-2.0.0a1.tar", max compression
+gzip compressed data, was "images_upload_cli-2.0.1.tar", max compression
```

## Comparing `images_upload_cli-2.0.0a1.tar` & `images_upload_cli-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     5236 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/README.md
--rw-r--r--   0        0        0     2557 2023-06-22 20:02:25.238057 images_upload_cli-2.0.0a1/pyproject.toml
--rwxr-xr-x   0        0        0      175 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/__init__.py
--rwxr-xr-x   0        0        0      178 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/__main__.py
--rwxr-xr-x   0        0        0     2407 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/cli.py
--rwxr-xr-x   0        0        0    10763 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/upload.py
--rwxr-xr-x   0        0        0     3133 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     6197 1970-01-01 00:00:00.000000 images_upload_cli-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-11 14:54:45.156571 images_upload_cli-2.0.1/LICENSE
+-rw-r--r--   0        0        0     5188 2023-07-11 14:54:45.156571 images_upload_cli-2.0.1/README.md
+-rw-r--r--   0        0        0     2581 2023-07-11 14:55:03.048746 images_upload_cli-2.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0      203 2023-07-11 14:54:45.156571 images_upload_cli-2.0.1/src/images_upload_cli/__init__.py
+-rwxr-xr-x   0        0        0      178 2023-07-11 14:54:45.156571 images_upload_cli-2.0.1/src/images_upload_cli/__main__.py
+-rwxr-xr-x   0        0        0     2414 2023-07-11 14:54:45.156571 images_upload_cli-2.0.1/src/images_upload_cli/cli.py
+-rwxr-xr-x   0        0        0    10763 2023-07-11 14:54:45.156571 images_upload_cli-2.0.1/src/images_upload_cli/upload.py
+-rwxr-xr-x   0        0        0     3316 2023-07-11 14:54:45.156571 images_upload_cli-2.0.1/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     6148 1970-01-01 00:00:00.000000 images_upload_cli-2.0.1/PKG-INFO
```

### Comparing `images_upload_cli-2.0.0a1/LICENSE` & `images_upload_cli-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-2.0.0a1/README.md` & `images_upload_cli-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,15 @@
   Upload images via APIs.
 
 Options:
   -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
                                   [default: imgur]
   -b, --bbcode                    Add bbcode tags.
   -t, --thumbnail                 Add caption thumbnail and bbcode tags.
-  -n, --notify / -N, --no-notify  Send desktop notifications via libnotify.
-                                  [default: N]
+  -n, --notify                    Send desktop notification via libnotify.
   -c, --clipboard / -C, --no-clipboard
                                   Copy result to clipboard.  [default: c]
   --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
 
 ## Env variables
```

### Comparing `images_upload_cli-2.0.0a1/pyproject.toml` & `images_upload_cli-2.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "images-upload-cli"
-version = "2.0.0-alpha.1"
+version = "2.0.1"
 description = "Upload images via APIs"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
 keywords = ["cli", "imgur", "image-upload", "upload-images", "upload-pictures"]
@@ -17,26 +17,26 @@
 [tool.poetry.scripts]
 images-upload-cli = "images_upload_cli.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 httpx = "^0.24.1"
-pillow = "^9.5.0"
+pillow = "^10.0.0"
 pyperclip = "^1.8.2"
 python-dotenv = "^1.0.0"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.3.0"
-mypy = "^1.4.0"
-poethepoet = "^0.20.0"
-ruff = "^0.0.275"
+black = "^23.7.0"
+mypy = "^1.4.1"
+poethepoet = "^0.21.0"
+ruff = "^0.0.277"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.2"
+pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.21.0"
 pytest-httpx = "^0.22.0"
 
 [tool.poe.tasks]
 ruff = "ruff check ."
 black = "black --check ."
@@ -65,15 +65,19 @@
 
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=./src"
 testpaths = ["tests"]
 markers = ["docker", "key_required"]
 
 [tool.coverage.report]
-exclude_lines = ["if TYPE_CHECKING:", "if __name__ == .__main__.:"]
+exclude_lines = [
+  "# pragma: no cover",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
 
 [tool.ruff]
 line-length = 99
 select = ["ALL"]
 ignore = [
   "COM812",  # Trailing comma missing
   "D203",    # 1 blank line required before class docstring
```

### Comparing `images_upload_cli-2.0.0a1/src/images_upload_cli/cli.py` & `images_upload_cli-2.0.1/src/images_upload_cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,34 +7,28 @@
 
 import click
 from dotenv import load_dotenv
 from httpx import AsyncClient
 from pyperclip import copy
 
 from images_upload_cli.upload import HOSTINGS, UPLOAD
-from images_upload_cli.util import get_config_path, make_thumbnail, notify_send
+from images_upload_cli.util import get_config_path, get_font, make_thumbnail, notify_send
 
 
 @click.command(context_settings={"show_default": True})
 @click.argument(
     "images",
     nargs=-1,
     required=True,
     type=click.Path(exists=True, dir_okay=False, path_type=Path),
 )
 @click.option("-h", "--hosting", type=click.Choice(HOSTINGS), default="imgur")
 @click.option("-b", "--bbcode", is_flag=True, help="Add bbcode tags.")
 @click.option("-t", "--thumbnail", is_flag=True, help="Add caption thumbnail and bbcode tags.")
-@click.option(
-    "-n/-N",
-    "--notify/--no-notify",
-    is_flag=True,
-    default=False,
-    help="Send desktop notifications via libnotify.",
-)
+@click.option("-n", "--notify", is_flag=True, help="Send desktop notification via libnotify.")
 @click.option(
     "-c/-C",
     "--clipboard/--no-clipboard",
     is_flag=True,
     default=True,
     help="Copy result to clipboard.",
 )
@@ -75,21 +69,24 @@
     images: tuple[Path],
     bbcode: bool,
     thumbnail: bool,
 ) -> list[str]:
     """Upload images coroutine."""
     links = []
 
+    if thumbnail:
+        font = get_font()
+
     async with AsyncClient() as client:
         for img_path in images:
             img = img_path.read_bytes()
 
             img_link = await upload_func(client, img)
             if not thumbnail:
                 link = f"[img]{img_link}[/img]" if bbcode else img_link
             else:
-                thumb_link = await upload_func(client, make_thumbnail(img))
+                thumb_link = await upload_func(client, make_thumbnail(img, font))
                 link = f"[url={img_link}][img]{thumb_link}[/img][/url]"
 
             links.append(link)
 
     return links
```

### Comparing `images_upload_cli-2.0.0a1/src/images_upload_cli/upload.py` & `images_upload_cli-2.0.1/src/images_upload_cli/upload.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-2.0.0a1/src/images_upload_cli/util.py` & `images_upload_cli-2.0.1/src/images_upload_cli/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 """Utils."""
 
-from functools import lru_cache
 from io import BytesIO
 from os import getenv
 from pathlib import Path
 from shutil import which
 from subprocess import Popen
 
 import click
@@ -41,39 +40,51 @@
 
 
 def get_img_ext(img: bytes) -> str:
     """Get image extension from bytes."""
     return Image.open(BytesIO(img)).format.lower()
 
 
-@lru_cache
-def get_font() -> ImageFont.FreeTypeFont:
+def get_font(size: int = 14) -> ImageFont.FreeTypeFont:
+    """Get caption font."""
+    return (
+        ImageFont.truetype(font_name, size=size)
+        if (font_name := getenv("CAPTION_FONT"))
+        else get_default_font()
+    )
+
+
+def get_default_font(size: int = 14) -> ImageFont.FreeTypeFont:
     """Attempt to retrieve a reasonably-looking TTF font from the system."""
     font_names = [
         "Helvetica",
         "NotoSerif-Regular",
         "Menlo",
         "DejaVuSerif",
         "arial",
     ]
 
     for font_name in font_names:
         try:
-            return ImageFont.truetype(font_name, size=14)
-        except OSError:
+            return ImageFont.truetype(font_name, size=size)
+        except OSError:  # noqa: PERF203
             continue
 
     msg = (
         f"None of the default fonts were found: {font_names}.\n"
         f"Please setup CAPTION_FONT in environment variables or in '{get_config_path()}'.",
-    )
-    raise GetEnvError(msg)
+    )  # pragma: no cover
+    raise GetEnvError(msg)  # pragma: no cover
 
 
-def make_thumbnail(img: bytes, size: tuple[int, int] = (300, 300)) -> bytes:
+def make_thumbnail(
+    img: bytes,
+    font: ImageFont.FreeTypeFont,
+    size: tuple[int, int] = (300, 300),
+) -> bytes:
     """Make this image into a captioned thumbnail."""
     # get a pw
     im = Image.open(BytesIO(img))
     pw = im.copy().convert("RGB")
     pw.thumbnail(size=size, resample=Image.Resampling.LANCZOS)
 
     # make a blank image for the text
@@ -83,21 +94,14 @@
         color=(255, 255, 255),
     )
     pw_with_line.paste(pw, box=(0, 0))
 
     # get a file size info
     fsize = human_size(len(img))
 
-    # get font
-    font = (
-        ImageFont.truetype(font_name, size=14)
-        if (font_name := getenv("CAPTION_FONT"))
-        else get_font()
-    )
-
     # draw text
     d = ImageDraw.Draw(pw_with_line)
     d.text(
         xy=(pw.width / 5, pw.height),
         text=f"{im.width}x{im.height} ({im.format}) [{fsize}]",
         font=font,
         fill=(0, 0, 0),
@@ -115,8 +119,8 @@
 
     return buffer.getvalue()
 
 
 def notify_send(text_to_print: str) -> None:
     """Send desktop notifications via libnotify."""
     if notify_send := which("notify-send"):
-        Popen([notify_send, "-a", "images-upload-cli", text_to_print])
+        Popen([notify_send, "-a", "images-upload-cli", text_to_print])  # pragma: no cover
```

### Comparing `images_upload_cli-2.0.0a1/PKG-INFO` & `images_upload_cli-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: images-upload-cli
-Version: 2.0.0a1
+Version: 2.0.1
 Summary: Upload images via APIs
 Home-page: https://github.com/DeadNews/images-upload-cli
 License: MIT
 Keywords: cli,imgur,image-upload,upload-images,upload-pictures
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.9,<4.0
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/DeadNews/images-upload-cli
 Description-Content-Type: text/markdown
 
 # images-upload-cli
 
@@ -86,16 +86,15 @@
   Upload images via APIs.
 
 Options:
   -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
                                   [default: imgur]
   -b, --bbcode                    Add bbcode tags.
   -t, --thumbnail                 Add caption thumbnail and bbcode tags.
-  -n, --notify / -N, --no-notify  Send desktop notifications via libnotify.
-                                  [default: N]
+  -n, --notify                    Send desktop notification via libnotify.
   -c, --clipboard / -C, --no-clipboard
                                   Copy result to clipboard.  [default: c]
   --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
 
 ## Env variables
```

