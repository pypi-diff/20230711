# Comparing `tmp/zyte-common-items-0.6.0.tar.gz` & `tmp/zyte-common-items-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte-common-items-0.6.0.tar", last modified: Wed Jul  5 10:33:14 2023, max compression
+gzip compressed data, was "zyte-common-items-0.7.0.tar", last modified: Tue Jul 11 14:16:42 2023, max compression
```

## Comparing `zyte-common-items-0.6.0.tar` & `zyte-common-items-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/zyte_common_items/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    30046 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/zyte_common_items.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/zyte_common_items/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34865 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/zyte_common_items.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/top_level.txt
```

### Comparing `zyte-common-items-0.6.0/LICENSE` & `zyte-common-items-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.6.0/PKG-INFO` & `zyte-common-items-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.6.0
+Version: 0.7.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-common-items-0.6.0/README.rst` & `zyte-common-items-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.6.0/setup.py` & `zyte-common-items-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     package_data={
         "zyte_common_items": ["py.typed", "VERSION"],
     },
     install_requires=[
         "attrs>=21.3.0",
         "itemadapter>=0.8.0",
         "web-poet>=0.7.0",
+        "zyte-parsers",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `zyte-common-items-0.6.0/zyte_common_items/adapter.py` & `zyte-common-items-0.7.0/zyte_common_items/adapter.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.6.0/zyte_common_items/base.py` & `zyte-common-items-0.7.0/zyte_common_items/base.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.6.0/zyte_common_items/components.py` & `zyte-common-items-0.7.0/zyte_common_items/components.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,118 @@
 """Classes for data nested within items."""
-from typing import Optional
+from typing import List, Optional, Type
 
 import attrs
 
 from zyte_common_items.base import Item
-from zyte_common_items.util import url_to_str
+from zyte_common_items.util import convert_to_class, url_to_str
+
+# Metadata ####################################################################
+
+
+@attrs.define(kw_only=True)
+class ProbabilityMetadata(Item):
+    """Data extraction process metadata that indicates a probability."""
+
+    #: The probability (0 for 0%, 1 for 100%) that the resource features the
+    #: expected data type.
+    #:
+    #: For example, if the extraction of a product from a given URL is
+    #: requested, and that URL points to the webpage of a product with complete
+    #: certainty, the value should be `1`. If with complete certainty the
+    #: webpage features a job listing instead of a product, the value should be
+    #: `0`. When there is no complete certainty, the value could be anything in
+    #: between (e.g. `0.96`).
+    probability: Optional[float] = 1.0
+
+
+@attrs.define(kw_only=True)
+class _ListMetadata(Item):
+    """Data extraction process metadata that indicates the download date.
+
+    See
+    :class:`ArticleList.metadata <zyte_common_items.ArticleList.metadata>`.
+    """
+
+    #: Date and time when the product data was downloaded, in UTC timezone and
+    #: the following format: ``YYYY-MM-DDThh:mm:ssZ``.
+    dateDownloaded: Optional[str] = None
+
+
+@attrs.define(kw_only=True)
+class _DetailsMetadata(_ListMetadata):
+    """Data extraction process metadata that indicates the download date and a
+    probability."""
+
+    #: The probability (0 for 0%, 1 for 100%) that the resource features the
+    #: expected data type.
+    #:
+    #: For example, if the extraction of a product from a given URL is
+    #: requested, and that URL points to the webpage of a product with complete
+    #: certainty, the value should be `1`. If with complete certainty the
+    #: webpage features a job listing instead of a product, the value should be
+    #: `0`. When there is no complete certainty, the value could be anything in
+    #: between (e.g. `0.96`).
+    probability: Optional[float] = 1.0
+
+
+@attrs.define(kw_only=True)
+class Metadata(_DetailsMetadata):
+    """Generic metadata class.
+
+    It defines all attributes of metadata classes for specific item types, so
+    that it can be used during extraction instead of a more specific class, and
+    later converted to the corresponding, more specific metadata class.
+    """
+
+    #: The search text used to find the item.
+    searchText: Optional[str] = None
+
+
+@attrs.define(kw_only=True)
+class ArticleMetadata(_DetailsMetadata):
+    pass
+
+
+@attrs.define(kw_only=True)
+class ArticleListMetadata(_ListMetadata):
+    pass
+
+
+@attrs.define(kw_only=True)
+class ArticleNavigationMetadata(_ListMetadata):
+    pass
+
+
+@attrs.define(kw_only=True)
+class BusinessPlaceMetadata(Metadata):
+    pass
+
+
+@attrs.define(kw_only=True)
+class ProductMetadata(_DetailsMetadata):
+    pass
+
+
+@attrs.define(kw_only=True)
+class ProductListMetadata(_ListMetadata):
+    pass
+
+
+@attrs.define(kw_only=True)
+class ProductNavigationMetadata(_ListMetadata):
+    pass
+
+
+@attrs.define(kw_only=True)
+class RealEstateMetadata(_DetailsMetadata):
+    pass
+
+
+###############################################################################
 
 
 @attrs.define
 class _Media(Item):
     #: URL.
     #:
     #: When multiple URLs exist for a given media element, pointing to
@@ -170,52 +274,14 @@
     #: Target URL.
     url: Optional[str] = attrs.field(
         default=None, converter=attrs.converters.optional(url_to_str), kw_only=True
     )
 
 
 @attrs.define(kw_only=True)
-class DateDownloadedMetadata(Item):
-    """Data extraction process metadata that only indicates the download date.
-
-    See
-    :class:`ArticleList.metadata <zyte_common_items.ArticleList.metadata>`.
-    """
-
-    #: Date and time when the product data was downloaded, in UTC timezone and
-    #: the following format: ``YYYY-MM-DDThh:mm:ssZ``.
-    dateDownloaded: Optional[str] = None
-
-
-@attrs.define(kw_only=True)
-class Metadata(DateDownloadedMetadata):
-    #: The probability (0 for 0%, 1 for 100%) that the webpage features the
-    #: requested data type.
-    #:
-    #: For example, if the extraction of a product from a given URL is
-    #: requested, and that URL points to the webpage of a product with complete
-    #: certainty, the value should be `1`. If with complete certainty the
-    #: webpage features a job listing instead of a product, the value should be
-    #: `0`. When there is no complete certainty, the value could be anything in
-    #: between (e.g. `0.96`).
-    probability: Optional[float] = None
-
-
-@attrs.define(kw_only=True)
-class BusinessPlaceMetadata(Metadata):
-    """Data extraction process metadata.
-
-    See :class:`BusinessPlace.metadata <zyte_common_items.BusinessPlace.metadata>`.
-    """
-
-    #: The search text the place was found with.
-    searchText: Optional[str] = None
-
-
-@attrs.define(kw_only=True)
 class Address(Item):
     """Address item."""
 
     #: The raw address information, as it appears on the website.
     addressRaw: Optional[str] = None
 
     #: The street address of the place.
@@ -321,13 +387,63 @@
     #: Type of area, one of: LOT, FLOOR
     areaType: Optional[str] = None
 
     #: Area in the raw format, as it appears on the website.
     raw: str
 
 
+@attrs.define(kw_only=True)
+class Header(Item):
+    """An HTTP header"""
+
+    #: Name of the header
+    name: str
+
+    #: Value of the header
+    value: str
+
+
+@attrs.define(kw_only=True)
+class Request(Item):
+    """Describe a web request to load a page"""
+
+    #: Name of the page being requested.
+    name: Optional[str] = None
+
+    #: HTTP URL
+    url: str = attrs.field(converter=url_to_str)
+
+    #: HTTP method
+    method: str = "GET"
+
+    #: HTTP request body, Base64-encoded
+    body: Optional[str] = None
+
+    #: HTTP headers
+    headers: Optional[List[Header]] = None
+
+
 @attrs.define
 class Video(_Media):
     """Video.
 
     See :class:`Article.videos <zyte_common_items.Article.videos>`.
     """
+
+
+def cast_request(value: Request, cls: Type[Request]) -> Request:
+    new_value = convert_to_class(value, cls)
+    if type(value) is Request and cls is ProbabilityRequest:
+        new_value.metadata = ProbabilityMetadata(probability=1.0)
+    return new_value
+
+
+def request_list_processor(request_list):
+    return [cast_request(request, ProbabilityRequest) for request in request_list]
+
+
+@attrs.define(kw_only=True)
+class ProbabilityRequest(Request):
+    """A :class:`Request` that includes a probability value."""
+
+    #: Data extraction process metadata.
+    metadata: Optional[ProbabilityMetadata] = None
```

### Comparing `zyte-common-items-0.6.0/zyte_common_items/items.py` & `zyte-common-items-0.7.0/zyte_common_items/items.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,32 +4,41 @@
 
 from zyte_common_items.base import Item
 from zyte_common_items.components import (
     AdditionalProperty,
     Address,
     AggregateRating,
     Amenity,
+    ArticleListMetadata,
+    ArticleMetadata,
+    ArticleNavigationMetadata,
     Audio,
     Author,
     Brand,
     Breadcrumb,
     BusinessPlaceMetadata,
-    DateDownloadedMetadata,
     Gtin,
     Image,
     Link,
-    Metadata,
     NamedLink,
     OpeningHoursItem,
     ParentPlace,
+    ProbabilityMetadata,
+    ProbabilityRequest,
+    ProductListMetadata,
+    ProductMetadata,
+    ProductNavigationMetadata,
     RealEstateArea,
+    RealEstateMetadata,
+    Request,
     StarRating,
     Video,
+    cast_request,
 )
-from zyte_common_items.util import url_to_str
+from zyte_common_items.util import MetadataCaster, url_to_str
 
 
 @attrs.define(slots=True, kw_only=True)
 class ArticleFromList(Item):
     """Article from an article list from an article listing page.
 
     See :class:`ArticleList`.
@@ -77,17 +86,18 @@
 
     #: Main image.
     mainImage: Optional[Image] = None
 
     #: All images.
     images: Optional[List[Image]] = None
 
-    #: The probability (0 for 0%, 1 for 100%) that this record represents an
-    #: actual article.
-    probability: Optional[float] = None
+    #: Data extraction process metadata.
+    metadata: Optional[ProbabilityMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(ProbabilityMetadata)), kw_only=True  # type: ignore
+    )
 
     #: Main URL.
     url: Optional[str] = attrs.field(
         default=None, converter=attrs.converters.optional(url_to_str), kw_only=True
     )
 
 
@@ -188,15 +198,17 @@
     #: Required attribute.
     #:
     #: In case there is no article data on the page or the page was not
     #: reached, the returned "empty" item would still contain this URL field.
     url: str = attrs.field(converter=url_to_str)
 
     #: Data extraction process metadata.
-    metadata: Optional[DateDownloadedMetadata] = None
+    metadata: Optional[ArticleMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(ArticleMetadata)), kw_only=True  # type: ignore
+    )
 
 
 @attrs.define(slots=True, kw_only=True)
 class ArticleList(Item):
     """Article list from an article listing page.
 
     The :attr:`url` attribute is the only required attribute, all other fields
@@ -228,15 +240,17 @@
 
     #: Webpage `breadcrumb trail`_.
     #:
     #: .. _Breadcrumb trail: https://en.wikipedia.org/wiki/Breadcrumb_navigation
     breadcrumbs: Optional[List[Breadcrumb]] = None
 
     #: Data extraction process metadata.
-    metadata: Optional[DateDownloadedMetadata] = None
+    metadata: Optional[ArticleListMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(ArticleListMetadata)), kw_only=True  # type: ignore
+    )
 
 
 @attrs.define(kw_only=True)
 class ProductVariant(Item):
     """:class:`Product` variant.
 
     See :attr:`Product.variants`.
@@ -496,15 +510,17 @@
     #: Images only displayed as part of the product description are excluded.
     images: Optional[List[Image]] = None
 
     #: Main product image.
     mainImage: Optional[Image] = None
 
     #: Data extraction process metadata.
-    metadata: Optional[Metadata] = None
+    metadata: Optional[ProductMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(ProductMetadata)), kw_only=True  # type: ignore
+    )
 
     #: `Manufacturer part number (MPN)`_.
     #:
     #: A product should have the same MPN across different e-commerce websites.
     #:
     #: See also: ``gtin``, ``productId``, ``sku``.
     #:
@@ -625,15 +641,17 @@
     #: See also ``currency``.
     currencyRaw: Optional[str] = None
 
     #: Main product image.
     mainImage: Optional[Image] = None
 
     #: Data extraction process metadata.
-    metadata: Optional[Metadata] = None
+    metadata: Optional[ProbabilityMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(ProbabilityMetadata)), kw_only=True  # type: ignore
+    )
 
     #: Name as it appears on the webpage (no post-processing).
     name: Optional[str] = None
 
     #: Price at which the product is being offered.
     #:
     #: It is a string with the price amount, with a full stop as decimal
@@ -694,15 +712,17 @@
     #: (no post-processing).
     #:
     #: For example, if the webpage is one of the pages of the Robots category,
     #: ``categoryName`` is ``'Robots'``.
     categoryName: Optional[str] = None
 
     #: Data extraction process metadata.
-    metadata: Optional[Metadata] = None
+    metadata: Optional[ProductListMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(ProductListMetadata)), kw_only=True  # type: ignore
+    )
 
     #: Current page number, if displayed explicitly on the list page.
     #:
     #: Numeration starts with 1.
     pageNumber: Optional[int] = None
 
     #: Link to the next page.
@@ -816,15 +836,17 @@
         default=None, converter=attrs.converters.optional(url_to_str), kw_only=True
     )
 
     #:  List of the tags associated with the place.
     tags: Optional[List[str]] = None
 
     #: Data extraction process metadata.
-    metadata: Optional[BusinessPlaceMetadata] = None
+    metadata: Optional[BusinessPlaceMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(BusinessPlaceMetadata)), kw_only=True  # type: ignore
+    )
 
 
 @attrs.define(slots=True, kw_only=True)
 class RealEstate(Item):
     #: The url of the final response, after any redirects.
     url: str = attrs.field(converter=url_to_str)
 
@@ -915,8 +937,104 @@
     #: The year the real estate was built.
     yearBuilt: Optional[int] = None
 
     #: The URL of the virtual tour of the real estate.
     virtualTourUrl: Optional[str] = None
 
     #: Contains metadata about the data extraction process.
-    metadata: Optional[Metadata] = None
+    metadata: Optional[RealEstateMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(RealEstateMetadata)), kw_only=True  # type: ignore
+    )
+
+
+class RequestListCaster:
+    def __init__(self, target):
+        self._target = target
+
+    def __call__(self, value):
+        return [cast_request(item, self._target) for item in value]
+
+
+@attrs.define(kw_only=True)
+class ProductNavigation(Item):
+    """Represents the navigational aspects of a product listing page on an
+    e-commerce website"""
+
+    #: Main URL from which the data is extracted.
+    url: str = attrs.field(converter=url_to_str)
+
+    #: Name of the category/page with the product list.
+    #:
+    #: Format:
+    #:
+    #: - trimmed (no whitespace at the beginning or the end of the description string)
+    categoryName: Optional[str] = None
+
+    #: List of sub-category links ordered by their position in the page.
+    subCategories: Optional[List[ProbabilityRequest]] = attrs.field(
+        default=None, converter=attrs.converters.optional(RequestListCaster(ProbabilityRequest)), kw_only=True  # type: ignore
+    )
+
+    #: List of product links found on the page category ordered by their position in the page.
+    items: Optional[List[ProbabilityRequest]] = attrs.field(
+        default=None, converter=attrs.converters.optional(RequestListCaster(ProbabilityRequest)), kw_only=True  # type: ignore
+    )
+
+    #: A link to the next page, if available.
+    nextPage: Optional[Request] = None
+
+    #: Number of the current page.
+    #:
+    #: It should only be extracted if the webpage shows a page number.
+    #:
+    #: It must be 1-based. For example, if the first page of a listing is
+    #: numbered as 0 on the website, it should be extracted as `1` nonetheless.
+    pageNumber: Optional[int] = None
+
+    #: Data extraction process metadata.
+    metadata: Optional[ProductNavigationMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(ProductNavigationMetadata)), kw_only=True  # type: ignore
+    )
+
+
+@attrs.define(kw_only=True)
+class ArticleNavigation(Item):
+    """Represents the navigational aspects of an article listing webpage.
+
+    See :class:`ArticleList`.
+    """
+
+    #: Main URL from which the data is extracted.
+    url: str = attrs.field(converter=url_to_str)
+
+    #: Name of the category/page.
+    #:
+    #: Format:
+    #:
+    #: - trimmed (no whitespace at the beginning or the end of the description string)
+    categoryName: Optional[str] = None
+
+    #: List of sub-category links ordered by their position in the page.
+    subCategories: Optional[List[ProbabilityRequest]] = attrs.field(
+        default=None, converter=attrs.converters.optional(RequestListCaster(ProbabilityRequest)), kw_only=True  # type: ignore
+    )
+
+    #: Links to listed items in order of appearance.
+    items: Optional[List[ProbabilityRequest]] = attrs.field(
+        default=None, converter=attrs.converters.optional(RequestListCaster(ProbabilityRequest)), kw_only=True  # type: ignore
+    )
+
+    #: A link to the next page, if available.
+    nextPage: Optional[Request] = None
+
+    #: Number of the current page.
+    #:
+    #: It should only be extracted if the webpage shows a page number.
+    #:
+    #: It must be 1-based. For example, if the first page of a listing is
+    #: numbered as 0 on the website, it should be extracted as `1` nonetheless.
+    pageNumber: Optional[int] = None
+
+    #: Data extraction process metadata.
+    metadata: Optional[ArticleNavigationMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(ArticleNavigationMetadata)), kw_only=True  # type: ignore
+    )
```

### Comparing `zyte-common-items-0.6.0/zyte_common_items.egg-info/PKG-INFO` & `zyte-common-items-0.7.0/zyte_common_items.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.6.0
+Version: 0.7.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

