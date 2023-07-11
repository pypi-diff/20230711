# Comparing `tmp/webdrivertools-0.0.3.tar.gz` & `tmp/webdrivertools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdrivertools-0.0.3.tar", last modified: Wed May 24 00:49:04 2023, max compression
+gzip compressed data, was "webdrivertools-0.0.4.tar", last modified: Tue Jul 11 19:54:18 2023, max compression
```

## Comparing `webdrivertools-0.0.3.tar` & `webdrivertools-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-24 00:49:04.961232 webdrivertools-0.0.3/
--rw-r--r--   0 leandro    (501) staff       (20)     1127 2023-04-24 02:15:44.000000 webdrivertools-0.0.3/LICENSE
--rw-r--r--   0 leandro    (501) staff       (20)     3340 2023-05-24 00:49:04.961094 webdrivertools-0.0.3/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     2480 2023-05-11 02:02:57.000000 webdrivertools-0.0.3/README.md
--rw-r--r--   0 leandro    (501) staff       (20)     1012 2023-05-24 00:48:26.000000 webdrivertools-0.0.3/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-24 00:49:04.961263 webdrivertools-0.0.3/setup.cfg
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-24 00:49:04.958874 webdrivertools-0.0.3/webdrivertools/
--rw-r--r--   0 leandro    (501) staff       (20)      163 2023-05-11 01:56:46.000000 webdrivertools-0.0.3/webdrivertools/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)     4663 2023-05-23 21:48:05.000000 webdrivertools-0.0.3/webdrivertools/webdrivertools.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-24 00:49:04.960880 webdrivertools-0.0.3/webdrivertools.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)     3340 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      281 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       16 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)       15 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/top_level.txt
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-11 19:54:18.190835 webdrivertools-0.0.4/
+-rw-r--r--   0 leandro    (501) staff       (20)     1127 2023-04-24 02:15:44.000000 webdrivertools-0.0.4/LICENSE
+-rw-r--r--   0 leandro    (501) staff       (20)     3353 2023-07-11 19:54:18.190735 webdrivertools-0.0.4/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     2493 2023-07-11 19:53:33.000000 webdrivertools-0.0.4/README.md
+-rw-r--r--   0 leandro    (501) staff       (20)     1012 2023-07-11 19:53:05.000000 webdrivertools-0.0.4/pyproject.toml
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-07-11 19:54:18.190862 webdrivertools-0.0.4/setup.cfg
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-11 19:54:18.190096 webdrivertools-0.0.4/webdrivertools/
+-rw-r--r--   0 leandro    (501) staff       (20)      163 2023-05-11 01:56:46.000000 webdrivertools-0.0.4/webdrivertools/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4690 2023-07-11 19:53:05.000000 webdrivertools-0.0.4/webdrivertools/webdrivertools.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-11 19:54:18.190606 webdrivertools-0.0.4/webdrivertools.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)     3353 2023-07-11 19:54:18.000000 webdrivertools-0.0.4/webdrivertools.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      281 2023-07-11 19:54:18.000000 webdrivertools-0.0.4/webdrivertools.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-07-11 19:54:18.000000 webdrivertools-0.0.4/webdrivertools.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       16 2023-07-11 19:54:18.000000 webdrivertools-0.0.4/webdrivertools.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       15 2023-07-11 19:54:18.000000 webdrivertools-0.0.4/webdrivertools.egg-info/top_level.txt
```

### Comparing `webdrivertools-0.0.3/LICENSE` & `webdrivertools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `webdrivertools-0.0.3/PKG-INFO` & `webdrivertools-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdrivertools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions to make life with Selenium easier.
 Author-email: Leandro Pereira de Lima e Silva <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/webdrivertools
 Project-URL: Bug Tracker, https://github.com/leandropls/webdrivertools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -56,15 +56,15 @@
 ```
 
 Click on the element area, even if it is covered by an overlay. This function is useful when dealing with elements obstructed by modal overlays or other overlapping elements, which may cause issues when attempting to interact with the intended element using Selenium.
 
 ### find_element
 
 ```python
-find_element(driver: WebDriver, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None) -> WebElement
+find_element(driver: WebDriver | WebElement, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None) -> WebElement
 ```
 
 Find a single HTML element within a webdriver page by attribute or criteria and optional inner text filtering, returning the matched WebElement.
 
 ### click
 
 ```python
```

### Comparing `webdrivertools-0.0.3/README.md` & `webdrivertools-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ```
 
 Click on the element area, even if it is covered by an overlay. This function is useful when dealing with elements obstructed by modal overlays or other overlapping elements, which may cause issues when attempting to interact with the intended element using Selenium.
 
 ### find_element
 
 ```python
-find_element(driver: WebDriver, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None) -> WebElement
+find_element(driver: WebDriver | WebElement, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None) -> WebElement
 ```
 
 Find a single HTML element within a webdriver page by attribute or criteria and optional inner text filtering, returning the matched WebElement.
 
 ### click
 
 ```python
```

### Comparing `webdrivertools-0.0.3/pyproject.toml` & `webdrivertools-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webdrivertools"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Leandro Pereira de Lima e Silva", email="leandro@lls-software.com" },
 ]
 description = "Functions to make life with Selenium easier."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `webdrivertools-0.0.3/webdrivertools/webdrivertools.py` & `webdrivertools-0.0.4/webdrivertools/webdrivertools.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,24 @@
     driver.execute_script("arguments[0].scrollIntoView(true);", element)
 
     # Click the element
     click_element_area(driver, element)
 
 
 def find_element(
-    driver: WebDriver,
+    driver: WebDriver | WebElement,
     value: str,
     by: str = By.CSS_SELECTOR,
     innerText: str | None = None,
 ) -> WebElement:
     """
     Find a single HTML element within a webdriver page by attribute or criteria and optional
     inner text filtering and return the matched WebElement.
 
-    :param driver: A WebDriver instance used to navigate and interact with the page
+    :param driver: A WebDriver or WebElement instance used to navigate and interact with the page
     :param value: The attribute value (e.g., CSS selector, xpath, etc.) to use in element search
     :param by: The attribute type used to search for the element (default: By.CSS_SELECTOR)
     :param innerText: Optional, the innerText to filter the elements by (if provided, only elements
                       with matching innerText will be returned)
     :return: WebElement that matches the search criteria and innerText (if provided)
     :raises ValueError: If the specified element is not found on the page
     """
```

### Comparing `webdrivertools-0.0.3/webdrivertools.egg-info/PKG-INFO` & `webdrivertools-0.0.4/webdrivertools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdrivertools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions to make life with Selenium easier.
 Author-email: Leandro Pereira de Lima e Silva <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/webdrivertools
 Project-URL: Bug Tracker, https://github.com/leandropls/webdrivertools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -56,15 +56,15 @@
 ```
 
 Click on the element area, even if it is covered by an overlay. This function is useful when dealing with elements obstructed by modal overlays or other overlapping elements, which may cause issues when attempting to interact with the intended element using Selenium.
 
 ### find_element
 
 ```python
-find_element(driver: WebDriver, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None) -> WebElement
+find_element(driver: WebDriver | WebElement, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None) -> WebElement
 ```
 
 Find a single HTML element within a webdriver page by attribute or criteria and optional inner text filtering, returning the matched WebElement.
 
 ### click
 
 ```python
```

