# Comparing `tmp/giant-news-1.2.3.tar.gz` & `tmp/giant-news-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant-news-1.2.3.tar", max compression
+gzip compressed data, was "giant-news-1.2.4.tar", max compression
```

## Comparing `giant-news-1.2.3.tar` & `giant-news-1.2.4.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1069 2021-08-26 14:32:41.238425 giant-news-1.2.3/LICENSE
--rw-r--r--   0        0        0     6113 2022-07-07 10:47:41.334737 giant-news-1.2.3/README.md
--rw-r--r--   0        0        0        0 2022-01-31 08:22:38.108271 giant-news-1.2.3/giant_news/__init__.py
--rw-r--r--   0        0        0     2370 2022-09-12 12:42:53.153204 giant-news-1.2.3/giant_news/admin.py
--rw-r--r--   0        0        0      134 2022-01-31 08:22:38.112271 giant-news-1.2.3/giant_news/apps.py
--rw-r--r--   0        0        0      472 2023-03-20 14:34:48.973933 giant-news-1.2.3/giant_news/cms_apps.py
--rw-r--r--   0        0        0     1424 2022-01-31 08:22:38.112271 giant-news-1.2.3/giant_news/cms_plugins.py
--rw-r--r--   0        0        0     1537 2022-06-01 14:26:30.500441 giant-news-1.2.3/giant_news/forms.py
--rw-r--r--   0        0        0     4599 2022-01-31 08:22:38.112271 giant-news-1.2.3/giant_news/migrations/0001_initial.py
--rw-r--r--   0        0        0     2455 2022-01-31 08:22:38.112271 giant-news-1.2.3/giant_news/migrations/0002_relatedarticlecardplugin_relatedarticleplugin.py
--rw-r--r--   0        0        0      674 2022-06-01 14:06:22.656574 giant-news-1.2.3/giant_news/migrations/0003_alter_article_content.py
--rw-r--r--   0        0        0      789 2022-06-01 14:26:30.500441 giant-news-1.2.3/giant_news/migrations/0004_auto_20220601_0915.py
--rw-r--r--   0        0        0      772 2022-09-12 10:59:37.939952 giant-news-1.2.3/giant_news/migrations/0005_auto_20220912_0459.py
--rw-r--r--   0        0        0     3280 2023-03-20 14:34:48.973933 giant-news-1.2.3/giant_news/migrations/0006_alter_article_author_alter_article_category_and_more.py
--rw-r--r--   0        0        0        0 2022-01-31 08:22:38.112271 giant-news-1.2.3/giant_news/migrations/__init__.py
--rw-r--r--   0        0        0       60 2022-01-31 08:22:38.112271 giant-news-1.2.3/giant_news/models/__init__.py
--rw-r--r--   0        0        0     4506 2023-03-20 14:34:48.973933 giant-news-1.2.3/giant_news/models/article.py
--rw-r--r--   0        0        0     2956 2022-01-31 08:22:38.112271 giant-news-1.2.3/giant_news/models/plugin.py
--rw-r--r--   0        0        0      377 2022-01-31 08:22:38.112271 giant-news-1.2.3/giant_news/sitemaps.py
--rw-r--r--   0        0        0        0 2022-01-31 08:22:38.112271 giant-news-1.2.3/giant_news/templates/base.html
--rw-r--r--   0        0        0      621 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/templates/news/detail.html
--rw-r--r--   0        0        0     2184 2022-06-01 14:26:30.500441 giant-news-1.2.3/giant_news/templates/news/index.html
--rw-r--r--   0        0        0     1327 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/templates/plugins/related_articles/container.html
--rw-r--r--   0        0        0      663 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/templates/plugins/related_articles/item.html
--rw-r--r--   0        0        0        0 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/tests/__init__.py
--rw-r--r--   0        0        0      272 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/tests/test_cms_apps.py
--rw-r--r--   0        0        0     2157 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/tests/test_forms.py
--rw-r--r--   0        0        0     1382 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/tests/test_models.py
--rw-r--r--   0        0        0     2245 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/tests/test_views.py
--rw-r--r--   0        0        0      150 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/tests/urls.py
--rw-r--r--   0        0        0      239 2022-01-31 08:22:38.116271 giant-news-1.2.3/giant_news/urls.py
--rw-r--r--   0        0        0     1423 2022-06-01 14:06:22.660574 giant-news-1.2.3/giant_news/views.py
--rw-r--r--   0        0        0     1420 2023-03-20 14:34:48.973933 giant-news-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     7204 2023-03-20 14:34:54.158398 giant-news-1.2.3/setup.py
--rw-r--r--   0        0        0     7030 2023-03-20 14:34:54.158715 giant-news-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-11 12:01:08.148709 giant-news-1.2.4/LICENSE
+-rw-r--r--   0        0        0     6113 2023-07-11 12:01:08.148861 giant-news-1.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 12:01:08.149068 giant-news-1.2.4/giant_news/__init__.py
+-rw-r--r--   0        0        0     2370 2023-07-11 12:01:08.149192 giant-news-1.2.4/giant_news/admin.py
+-rw-r--r--   0        0        0      134 2023-07-11 12:01:08.149295 giant-news-1.2.4/giant_news/apps.py
+-rw-r--r--   0        0        0      472 2023-07-11 12:01:08.149409 giant-news-1.2.4/giant_news/cms_apps.py
+-rw-r--r--   0        0        0     1424 2023-07-11 12:01:08.149516 giant-news-1.2.4/giant_news/cms_plugins.py
+-rw-r--r--   0        0        0     1537 2023-07-11 12:01:08.149646 giant-news-1.2.4/giant_news/forms.py
+-rw-r--r--   0        0        0     4599 2023-07-11 12:01:08.149818 giant-news-1.2.4/giant_news/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2455 2023-07-11 12:01:08.149937 giant-news-1.2.4/giant_news/migrations/0002_relatedarticlecardplugin_relatedarticleplugin.py
+-rw-r--r--   0        0        0      674 2023-07-11 12:01:08.150033 giant-news-1.2.4/giant_news/migrations/0003_alter_article_content.py
+-rw-r--r--   0        0        0      789 2023-07-11 12:01:08.150148 giant-news-1.2.4/giant_news/migrations/0004_auto_20220601_0915.py
+-rw-r--r--   0        0        0      772 2023-07-11 12:01:08.150269 giant-news-1.2.4/giant_news/migrations/0005_auto_20220912_0459.py
+-rw-r--r--   0        0        0     3280 2023-07-11 12:01:08.150371 giant-news-1.2.4/giant_news/migrations/0006_alter_article_author_alter_article_category_and_more.py
+-rw-r--r--   0        0        0      618 2023-07-11 12:55:54.521690 giant-news-1.2.4/giant_news/migrations/0007_relatedarticleplugin_title.py
+-rw-r--r--   0        0        0        0 2023-07-11 12:01:08.150416 giant-news-1.2.4/giant_news/migrations/__init__.py
+-rw-r--r--   0        0        0       60 2023-07-11 12:01:08.150581 giant-news-1.2.4/giant_news/models/__init__.py
+-rw-r--r--   0        0        0     4506 2023-07-11 12:01:08.150748 giant-news-1.2.4/giant_news/models/article.py
+-rw-r--r--   0        0        0     3154 2023-07-11 12:55:54.522082 giant-news-1.2.4/giant_news/models/plugin.py
+-rw-r--r--   0        0        0      377 2023-07-11 12:01:08.150935 giant-news-1.2.4/giant_news/sitemaps.py
+-rw-r--r--   0        0        0        0 2023-07-11 12:01:08.151021 giant-news-1.2.4/giant_news/templates/base.html
+-rw-r--r--   0        0        0      621 2023-07-11 12:01:08.151178 giant-news-1.2.4/giant_news/templates/news/detail.html
+-rw-r--r--   0        0        0     2184 2023-07-11 12:01:08.151301 giant-news-1.2.4/giant_news/templates/news/index.html
+-rw-r--r--   0        0        0     1421 2023-07-11 12:55:54.522333 giant-news-1.2.4/giant_news/templates/plugins/related_articles/container.html
+-rw-r--r--   0        0        0      663 2023-07-11 12:01:08.151793 giant-news-1.2.4/giant_news/templates/plugins/related_articles/item.html
+-rw-r--r--   0        0        0        0 2023-07-11 12:01:08.151908 giant-news-1.2.4/giant_news/tests/__init__.py
+-rw-r--r--   0        0        0      272 2023-07-11 12:01:08.152047 giant-news-1.2.4/giant_news/tests/test_cms_apps.py
+-rw-r--r--   0        0        0     2157 2023-07-11 12:01:08.152152 giant-news-1.2.4/giant_news/tests/test_forms.py
+-rw-r--r--   0        0        0     1382 2023-07-11 12:01:08.152261 giant-news-1.2.4/giant_news/tests/test_models.py
+-rw-r--r--   0        0        0     2245 2023-07-11 12:01:08.152371 giant-news-1.2.4/giant_news/tests/test_views.py
+-rw-r--r--   0        0        0      150 2023-07-11 12:01:08.152459 giant-news-1.2.4/giant_news/tests/urls.py
+-rw-r--r--   0        0        0      239 2023-07-11 12:01:08.152554 giant-news-1.2.4/giant_news/urls.py
+-rw-r--r--   0        0        0     1423 2023-07-11 12:01:08.152669 giant-news-1.2.4/giant_news/views.py
+-rw-r--r--   0        0        0     1420 2023-07-11 12:55:54.522576 giant-news-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7204 2023-07-11 12:56:00.002158 giant-news-1.2.4/setup.py
+-rw-r--r--   0        0        0     7030 2023-07-11 12:56:00.002461 giant-news-1.2.4/PKG-INFO
```

### Comparing `giant-news-1.2.3/LICENSE` & `giant-news-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/README.md` & `giant-news-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/admin.py` & `giant-news-1.2.4/giant_news/admin.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/cms_plugins.py` & `giant-news-1.2.4/giant_news/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/forms.py` & `giant-news-1.2.4/giant_news/forms.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/migrations/0001_initial.py` & `giant-news-1.2.4/giant_news/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/migrations/0002_relatedarticlecardplugin_relatedarticleplugin.py` & `giant-news-1.2.4/giant_news/migrations/0002_relatedarticlecardplugin_relatedarticleplugin.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/migrations/0003_alter_article_content.py` & `giant-news-1.2.4/giant_news/migrations/0003_alter_article_content.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/migrations/0004_auto_20220601_0915.py` & `giant-news-1.2.4/giant_news/migrations/0004_auto_20220601_0915.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/migrations/0005_auto_20220912_0459.py` & `giant-news-1.2.4/giant_news/migrations/0005_auto_20220912_0459.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/migrations/0006_alter_article_author_alter_article_category_and_more.py` & `giant-news-1.2.4/giant_news/migrations/0006_alter_article_author_alter_article_category_and_more.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/models/article.py` & `giant-news-1.2.4/giant_news/models/article.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/models/plugin.py` & `giant-news-1.2.4/giant_news/models/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,14 +41,23 @@
         help_text="""
         Limit recent articles based on a category. This will
         override the tags that you choose and will filter on this category
         ONLY.
         """,
     )
 
+    title = models.CharField(
+        max_length=255,
+        blank=True,
+        help_text="""
+        If you want to display a title above the articles,
+        enter it here.
+        """,
+    )
+
     def __str__(self):
         """
         String representation of the article card object
         """
         return f"Related article block {self.pk}"
 
     def copy_relations(self, oldinstance):
```

### Comparing `giant-news-1.2.3/giant_news/templates/news/detail.html` & `giant-news-1.2.4/giant_news/templates/news/detail.html`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/templates/news/index.html` & `giant-news-1.2.4/giant_news/templates/news/index.html`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/templates/plugins/related_articles/container.html` & `giant-news-1.2.4/giant_news/templates/plugins/related_articles/container.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 {% load cms_tags %}
 
 <section class="card-block">
     <div class="wrapper">
+        {% if instance.title %}
+            <h3>{{ instance.title }}</h3>
+        {% endif %}
         <div class="card-block__cards card-block__cards--articles three-col">
             {% if instance.tags.all %}
                 {% for article in latest_articles %}
                     <a href="{{ article.get_absolute_url }}" title="Read more" class="card-block__cards__card three-col__col{% if article.category %} {{ article.category.slug }}{% endif %}">
                         <div class="text">
                             {% if article.category %}
                                 <p class="category">{{ article.category }}</p>
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
 {% load cms_tags %}
+{% if instance.title %}
+**** {{ instance.title }} ****
+{% endif %}
 {% if instance.tags.all %} {% for article in latest_articles %}
 {%_if_article.category_%}
 {{_article.category_}}
 {%_endif_%}
 ****_{{_article.title_}}_****
 {{_article.publish_at|date:"jS_F_Y"_}}{%_if_article.author_%}_by_{
 {_article.author|title_}}{%_endif_%}
```

### Comparing `giant-news-1.2.3/giant_news/templates/plugins/related_articles/item.html` & `giant-news-1.2.4/giant_news/templates/plugins/related_articles/item.html`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/tests/test_forms.py` & `giant-news-1.2.4/giant_news/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/tests/test_models.py` & `giant-news-1.2.4/giant_news/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/tests/test_views.py` & `giant-news-1.2.4/giant_news/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/giant_news/views.py` & `giant-news-1.2.4/giant_news/views.py`

 * *Files identical despite different names*

### Comparing `giant-news-1.2.3/pyproject.toml` & `giant-news-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-news"
-version = "1.2.3"
+version = "1.2.4"
 description = "A small reusable package that adds a News app to a project"
 authors = ["Will-Hoey <will.hoey@giantdigital.co.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-news"
 repository = "https://github.com/giantmade/giant-news"
 keywords = ["giant_news", "app"]
```

### Comparing `giant-news-1.2.3/setup.py` & `giant-news-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                 'templates/plugins/related_articles/*']}
 
 install_requires = \
 ['django-filer', 'giant-mixins', 'swapper>=1.3.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'giant-news',
-    'version': '1.2.3',
+    'version': '1.2.4',
     'description': 'A small reusable package that adds a News app to a project',
     'long_description': '# Giant News\n\nA re-usable package which can be used in any project that requires a generic `News` app.\n\nThis will include the basic formatting and functionality such as model creation via the admin.\n\nSupported Django versions:\n\n- Django 2.2, 3.2\n\nSupported django CMS versions:\n\n- django CMS 3.8, 3.9\n\n> &#x26a0;&#xfe0f; For Django 2.x, use giant-news 0.x\n\n> &#x26a0;&#xfe0f; Release 1.0.0-alpha.1 and above are NOT compatible with\n> versions < 1 due to model name changes and a migration reset. Only upgrade to\n> this version if you are aware of what changes need to be made\n\n## Installation and Configuration\n\nTo install with the package manager, run:\n\n    $ poetry add giant-news\n\nYou should then add `"giant_news", "easy_thumbnails" and "filer"` to the `INSTALLED_APPS` in your settings file.\nThe detail pages in this app use plugins which are not contained within this app. It is recommended that you include a set of plugins in your project, or use the `giant-plugins` app.\n\nIt is highly recommended that you override the base Article model at the start\nof a project, even if you have no intention of immediately changing any fields.\nChanging from a non-swappable model to a swappable model is difficult and will require migration\nhacking.\n\n```\n# models.py\n\nfrom giant_news.models import AbstractArticle\n\n\nclass Article(AbstractArticle):\n    pass\n\n\n# in admin.py\n\nfrom django.contrib import admin\nfrom giant_news.admin import ArticleAdmin\nfrom .models import Article\n\n\nadmin.site.register(Article, ArticleAdmin)\n\n```\n\nWhen the migrations are created for this new model it will need some tweaking as\nDjango will not set this up to use swapper. To do this add the following lines to\nthe initial migration file (this will replace the hardcoded dependency on the\n0002 migration from giant_news)\n\n```\nimport swapper\n\nclass Migration...\n\n    dependencies = [\n        ...\n        (\'giant_news\', \'0001_initial\'),\n        swapper.dependency("giant_news", "Article"),\n    ]\n```\nWe also need to tell it run this migration before any other migration inside the\ngiant_news library as the model needs to be "swapped" before any relations are\ncreated. You can do this with another line just under the `dependencies` list.\n\n```\n    run_before = [\n        (\'giant_news\', \'0002_relatedarticlecardplugin_relatedarticleplugin\'),\n    ]\n```\nOnce you have created a model, and only AFTER you run migrations, you\'ll need to\npoint swapper to this new model. You can do this with the following setting:\n\n    GIANT_NEWS_ARTICLE_MODEL = "appname.Article"\n\n\n## Admin\nBy default, the admin for each of the models is not installed. This is so that you can register them as you need within your custom app. To do so add the following lines to your admin.py\n\n```\nfrom giant_news.admin import ArticleAdmin, TagAdmin, CategoryAdmin, AuthorAdmin\nfrom giant_news.models import Article, Tag, Category, Author\n\nadmin.site.register(Article, ArticleAdmin)\nadmin.site.register(Category, CategoryAdmin)\nadmin.site.register(Author, AuthorAdmin)\nadmin.site.register(Tag, TagAdmin)\n```\n\n## CMS App\nBy default this app is not registered as a CMS App. However if you wish to use the builtin CMS app simply add the following line of code to the settings file.\n\n    REGISTER_NEWS_APP = True\n\n## Sitemap\n\nIn order to add published articles to your sitemap, import the sitemaps file and add it to your `sitemaps` dict. This is usually contained within the main `urls.py` file.\n\n## URLs\n\nIt is recommended that the application be added to a CMS page via the apphook. However, if you wish to hardcode the URL, you can do so by adding the following to your main `urls.py` file:\n\n```\n\n    path("news/", include("giant_news.urls"), name="news"),\n```\n\nIf you want to customize the urls to include a different path and/or templates, first you must import `from giant_news import views as news_views` in `core.urls` and then you could add the following:\n\n    path("news/", news_views.ArticleIndex.as_view(template_name="news/index.html"), name="index"),\n    path("news/<slug:slug>/", news_views.ArticleDetail.as_view(template_name="news/detail.html"), name="detail"),\n\n# Local development\n\n## Getting setup\n\nTo get started with local development of this library, you will need access to poetry (or another venv manager). You can set up a virtual environment with poetry by running:\n\n    $ poetry shell\n\nNote: You can update which version of python poetry will use for the virtualenv by using:\n\n    $ poetry env use 3.x\n\nand install all the required dependencies (seen in the pyproject.toml file) with:\n\n    $ poetry install\n\n\n## Management commands\n\nAs the library does not come with a `manage.py` file we need to use `django-admin` instead. However, we will need to set our `DJANGO_SETTINGS_MODULE` file in the environment. You can do this with:  \n\n    $ export DJANGO_SETTINGS_MODULE=settings\n\nFrom here you can run all the standard Django management commands such as `django-admin makemigrations`.\n\n## Testing\n\nThis library uses Pytest in order to run its tests. You can do this (inside the shell) by running:\n\n    $ pytest -v\n\nwhere `-v` is to run in verbose mode which, while not necessary, will show which tests errored/failed/passed a bit more clearly. \n\n## Preparing for release\n\nIn order to prep the package for a new release on TestPyPi and PyPi there is one key thing that you need to do. You need to update the version number in the `pyproject.toml`.\nThis is so that the package can be published without running into version number conflicts. The version numbering must also follow the Semantic Version rules which can be found here https://semver.org/.\n\n## Publishing\n\nPublishing a package with poetry is incredibly easy. Once you have checked that the version number has been updated (not the same as a previous version) then you only need to run two commands.\n\n    $ `poetry build`\n\nwill package the project up for you into a way that can be published.\n\n    $ `poetry publish`\n\nwill publish the package to PyPi. You will need to enter the company username (Giant-Digital) and password for the account which can be found in the company password manager\n',
     'author': 'Will-Hoey',
     'author_email': 'will.hoey@giantdigital.co.uk',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/giantmade/giant-news',
```

### Comparing `giant-news-1.2.3/PKG-INFO` & `giant-news-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giant-news
-Version: 1.2.3
+Version: 1.2.4
 Summary: A small reusable package that adds a News app to a project
 Home-page: https://github.com/giantmade/giant-news
 License: MIT
 Keywords: giant_news,app
 Author: Will-Hoey
 Author-email: will.hoey@giantdigital.co.uk
 Requires-Python: >=3.9,<4.0
```

