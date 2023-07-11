# Comparing `tmp/curcheck-1.1.4.tar.gz` & `tmp/curcheck-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curcheck-1.1.4.tar", max compression
+gzip compressed data, was "curcheck-1.1.5.tar", max compression
```

## Comparing `curcheck-1.1.4.tar` & `curcheck-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      473 2023-06-07 10:59:42.004006 curcheck-1.1.4/curcheck/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 11:30:37.676819 curcheck-1.1.4/curcheck/bot.py
--rw-r--r--   0        0        0       61 2023-06-20 20:06:51.342155 curcheck-1.1.4/curcheck/config.py
--rw-r--r--   0        0        0     1061 2023-06-21 19:55:22.368193 curcheck-1.1.4/curcheck/dispatcher.py
--rw-r--r--   0        0        0     6757 2023-06-30 09:48:58.967164 curcheck-1.1.4/curcheck/events.py
--rw-r--r--   0        0        0      810 2023-06-28 08:21:32.835014 curcheck-1.1.4/curcheck/gui.py
--rw-r--r--   0        0        0       47 2023-06-30 09:22:31.315113 curcheck-1.1.4/curcheck/middlewares.py
--rw-r--r--   0        0        0     3106 2023-06-28 08:36:11.961399 curcheck-1.1.4/curcheck/router.py
--rw-r--r--   0        0        0       73 2023-06-20 20:06:13.035766 curcheck-1.1.4/curcheck/utils.py
--rw-r--r--   0        0        0     1086 2023-01-06 12:52:22.705303 curcheck-1.1.4/LICENSE.md
--rw-r--r--   0        0        0      452 2023-07-05 15:46:48.750997 curcheck-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       18 2023-06-21 20:22:04.879283 curcheck-1.1.4/README.md
--rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 curcheck-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      473 2023-06-07 10:59:42.004006 curcheck-1.1.5/curcheck/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 11:30:37.676819 curcheck-1.1.5/curcheck/bot.py
+-rw-r--r--   0        0        0       61 2023-06-20 20:06:51.342155 curcheck-1.1.5/curcheck/config.py
+-rw-r--r--   0        0        0     1163 2023-07-11 17:29:14.308574 curcheck-1.1.5/curcheck/dispatcher.py
+-rw-r--r--   0        0        0     8495 2023-07-11 19:45:15.689203 curcheck-1.1.5/curcheck/events.py
+-rw-r--r--   0        0        0      810 2023-06-28 08:21:32.835014 curcheck-1.1.5/curcheck/gui.py
+-rw-r--r--   0        0        0       47 2023-06-30 09:22:31.315113 curcheck-1.1.5/curcheck/middlewares.py
+-rw-r--r--   0        0        0     4786 2023-07-11 19:44:19.316485 curcheck-1.1.5/curcheck/router.py
+-rw-r--r--   0        0        0       73 2023-06-20 20:06:13.035766 curcheck-1.1.5/curcheck/utils.py
+-rw-r--r--   0        0        0     1086 2023-01-06 12:52:22.705303 curcheck-1.1.5/LICENSE.md
+-rw-r--r--   0        0        0      452 2023-07-11 21:09:35.719115 curcheck-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-06-21 20:22:04.879283 curcheck-1.1.5/README.md
+-rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 curcheck-1.1.5/setup.py
+-rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 curcheck-1.1.5/PKG-INFO
```

### Comparing `curcheck-1.1.4/curcheck/dispatcher.py` & `curcheck-1.1.5/curcheck/dispatcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import asyncio
 
 from typing import List
 
 from pyppeteer import launch
+from pyppeteer.browser import Browser
 
 from .gui import AbstractGUIParser
 from .router import SiteRouter
 
 
 class Dispatcher:
     def __init__(self) -> None:
@@ -20,15 +21,16 @@
 
     def include_router(self, router: SiteRouter):
         if router.is_spa:
             self.spa_routers.append(router)
         else:
             self.mpa_routers.append(router)
 
-    async def start(self):
+    async def start(self, browser: Browser|None = None):
         if len(self.spa_routers) != 0:
-            browser = await launch(headless=False)
+            if not browser:
+                browser = await launch(headless=False)
 
         await asyncio.gather(
             *[router.executor(browser=browser) for router in self.spa_routers],
             *[router.executor() for router in self.mpa_routers],
         )
```

### Comparing `curcheck-1.1.4/curcheck/events.py` & `curcheck-1.1.5/curcheck/events.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,43 +4,68 @@
 
 import functools
 import asyncio
 
 from aiohttp import ClientSession
 from lxml import html
 
-from typing import Any, List, Awaitable
+from typing import List, Awaitable
 
 from pyppeteer.browser import Browser
 
 
 class AbstractEvent:
     task: Awaitable|None = None
 
-    def __init__(self, domain: str, url: str, is_browser: bool = False):
+    def __init__(
+        self, 
+        domain: str, 
+        url: str, 
+        is_browser: bool = False, 
+        cookies: dict|None = None
+    ):
         self.domain = domain
         self.url = url
         self.is_browser = is_browser
+        self.cookies = cookies
 
         if "http://" in self.url and "." in self.url:
             self.link: str = self.url
         elif "//" in self.url and not "http:" in self.url:
             self.link: str = "http:" + self.url
         else:
             self.link: str = self.domain + self.url
+    
+    async def _get_page(self, browser: Browser):
+        page = await browser.newPage()
+        page.setDefaultNavigationTimeout(0)
+        if self.cookies:
+            await page.setCookie(*self.cookies)
+        await page.goto(url=self.link)
 
 
 class EventPage(AbstractEvent):
-    def __init__(self, domain: str, url: str, is_browser: bool = False):
-        super().__init__(domain=domain, url=url, is_browser=is_browser)
+    def __init__(
+        self, 
+        domain: str, 
+        url: str, 
+        is_browser: bool = False, 
+        cookies: dict|None = None
+    ):
+        super().__init__(
+            domain=domain, url=url, is_browser=is_browser, cookies=cookies
+        )
 
     def __call__(self, func: Awaitable):
         @functools.wraps(func) 
         async def spa_task(browser: Browser):
             page = await browser.newPage()
+            page.setDefaultNavigationTimeout(0)
+            if self.cookies:
+                await page.setCookie(*self.cookies)
             await page.goto(url=self.link)
             await func(page)
             await page.close()
 
         @functools.wraps(func) 
         async def mpa_task(session: ClientSession):
             response = await session.request("GET", self.link)
@@ -59,49 +84,70 @@
 class EventPaginator(AbstractEvent):
     def __init__(
         self, 
         domain: str, 
         url: str, 
         pages_links_xpath: str, 
         count_in_approach: int = 10,
-        is_browser: bool = False
+        is_browser: bool = False,
+        auxiliary_function: Awaitable|None = None,
+        paginate_urls: list|None = None,
+        cookies: dict|None = None
     ) -> None:
-        super().__init__(domain=domain, url=url, is_browser=is_browser)
+        super().__init__(
+            domain=domain, url=url, is_browser=is_browser, cookies=cookies
+        )
 
         self.pages_links_xpath = pages_links_xpath
         self.count_in_approach = count_in_approach
+        self.auxiliary_function = auxiliary_function
+        self.paginate_urls = paginate_urls
 
         self.pages: List[EventPage] = []
 
     def __call__(self, func: Awaitable):
         @functools.wraps(func) 
         async def spa_task(browser: Browser):
-            base_page = await browser.newPage()
-            await base_page.goto(url=self.domain+self.url)
-            
-            if self.pages_links_xpath.split("/")[-1][0] == "@":
-                html_attr = f'.getAttribute("{self.pages_links_xpath.split("/")[-1][1:]}")'
-            elif self.pages_links_xpath.split("/")[-1] == "text()":
-                html_attr = ".innerText"
-            else:
-                html_attr = ".innerHTML"
+            if not self.paginate_urls:
+                base_page = await browser.newPage()
+                base_page.setDefaultNavigationTimeout(0)
+                if self.cookies:
+                    await base_page.setCookie(*self.cookies)
+                await base_page.goto(url=self.domain+self.url)
+
+                if self.auxiliary_function:
+                    await self.auxiliary_function(base_page)
+                
+                if self.pages_links_xpath.split("/")[-1][0] == "@":
+                    html_attr = f'.getAttribute("{self.pages_links_xpath.split("/")[-1][1:]}")'
+                elif self.pages_links_xpath.split("/")[-1] == "text()":
+                    html_attr = ".innerText"
+                else:
+                    html_attr = ".innerHTML"
 
-            xpath = "/".join(self.pages_links_xpath.split("/")[:-1])
+                xpath = "/".join(self.pages_links_xpath.split("/")[:-1])
 
-            pages_links = await base_page.xpath(xpath)
+                pages_links = await base_page.xpath(xpath)
 
-            self.pages = [
-                EventPage(
-                    domain=self.domain, 
-                    url=await base_page.evaluate(
-                        f"(link) => link{html_attr}", link
-                    ),
-                    is_browser=True
-                )(func) for link in pages_links
-            ]
+                self.pages = [
+                    EventPage(
+                        domain=self.domain, 
+                        url=await base_page.evaluate(
+                            f"(link) => link{html_attr}", link
+                        ),
+                        is_browser=True,
+                        cookies=self.cookies
+                    )(func) for link in pages_links
+                ]
+            else:
+                self.pages = [
+                    EventPage(
+                        domain=self.domain, url=url, is_browser=True
+                    )(func) for url in self.paginate_urls
+                ]
 
             approach_len = (
                 len(self.pages) // self.count_in_approach 
                 if len(self.pages) % self.count_in_approach == 0 
                 else (len(self.pages) // self.count_in_approach)+1
             ) # кол-во подходов
 
@@ -157,27 +203,31 @@
 class EventLongpoll(AbstractEvent):
     def __init__(
         self, 
         domain: str, 
         url: str, 
         timeout: int = 60, 
         count: int = None,
-        is_browser: bool = False
+        is_browser: bool = False,
+        cookies: dict|None = None,
     ) -> None:
-        super().__init__(domain=domain, url=url, is_browser=is_browser)
+        super().__init__(domain=domain, url=url, is_browser=is_browser, cookies=cookies)
 
         self.count = count
         self.timeout = timeout
         self.i = 0
 
     def __call__(self, func: Awaitable):
         @functools.wraps(func)
         async def spa_task(browser: Browser):
             self.browser = browser
             page = await self.browser.newPage()
+            if self.cookies:
+                await page.setCookie(*self.cookies)
+            page.setDefaultNavigationTimeout(0)
             await self.page.goto(self.link)
             while self.i <= self.count or self.count == None:
                 self.i += 1
                 await func(page)
                 await page.reload()
                 await asyncio.sleep(self.timeout)
```

### Comparing `curcheck-1.1.4/curcheck/gui.py` & `curcheck-1.1.5/curcheck/gui.py`

 * *Files identical despite different names*

### Comparing `curcheck-1.1.4/LICENSE.md` & `curcheck-1.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curcheck-1.1.4/PKG-INFO` & `curcheck-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curcheck
-Version: 1.1.4
+Version: 1.1.5
 Summary: Library for parsing SPA and MPA sites
 License: MIT
 Author: BulatXam
 Author-email: Khamdbulat@yandex.ru
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

