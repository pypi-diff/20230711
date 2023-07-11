# Comparing `tmp/lesscode_tag-0.0.4.tar.gz` & `tmp/lesscode_tag-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_tag-0.0.4.tar", last modified: Tue Jun 13 03:18:59 2023, max compression
+gzip compressed data, was "dist/lesscode_tag-0.0.5.tar", last modified: Tue Jul 11 10:11:29 2023, max compression
```

## Comparing `lesscode_tag-0.0.4.tar` & `lesscode_tag-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/
--rw-r--r--   0 baai       (501) staff       (20)      379 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       52 2023-05-25 01:34:02.000000 lesscode_tag-0.0.4/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-25 01:04:19.000000 lesscode_tag-0.0.4/lesscode_tag/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1807 2023-05-25 02:53:36.000000 lesscode_tag-0.0.4/lesscode_tag/aes.py
--rw-r--r--   0 baai       (501) staff       (20)     8078 2023-06-13 03:18:47.000000 lesscode_tag-0.0.4/lesscode_tag/business.py
--rw-r--r--   0 baai       (501) staff       (20)     9603 2023-05-25 02:53:36.000000 lesscode_tag-0.0.4/lesscode_tag/es_util.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-06-13 03:18:47.000000 lesscode_tag-0.0.4/lesscode_tag/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      379 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      280 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       13 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1273 2023-05-25 07:46:43.000000 lesscode_tag-0.0.4/setup.py
+drwxr-xr-x   0 zhengy     (501) staff       (20)        0 2023-07-11 10:11:29.000000 lesscode_tag-0.0.5/
+-rw-r--r--   0 zhengy     (501) staff       (20)      379 2023-07-11 10:11:29.000000 lesscode_tag-0.0.5/PKG-INFO
+-rw-r--r--   0 zhengy     (501) staff       (20)       52 2023-05-25 10:25:23.000000 lesscode_tag-0.0.5/README.md
+drwxr-xr-x   0 zhengy     (501) staff       (20)        0 2023-07-11 10:11:29.000000 lesscode_tag-0.0.5/lesscode_tag/
+-rw-r--r--   0 zhengy     (501) staff       (20)        0 2023-05-25 10:25:23.000000 lesscode_tag-0.0.5/lesscode_tag/__init__.py
+-rw-r--r--   0 zhengy     (501) staff       (20)     1807 2023-05-25 10:25:23.000000 lesscode_tag-0.0.5/lesscode_tag/aes.py
+-rw-r--r--   0 zhengy     (501) staff       (20)     9131 2023-07-11 10:11:03.000000 lesscode_tag-0.0.5/lesscode_tag/business.py
+-rw-r--r--   0 zhengy     (501) staff       (20)     9603 2023-05-25 10:25:23.000000 lesscode_tag-0.0.5/lesscode_tag/es_util.py
+-rw-r--r--   0 zhengy     (501) staff       (20)       22 2023-07-11 10:11:15.000000 lesscode_tag-0.0.5/lesscode_tag/version.py
+drwxr-xr-x   0 zhengy     (501) staff       (20)        0 2023-07-11 10:11:29.000000 lesscode_tag-0.0.5/lesscode_tag.egg-info/
+-rw-r--r--   0 zhengy     (501) staff       (20)      379 2023-07-11 10:11:29.000000 lesscode_tag-0.0.5/lesscode_tag.egg-info/PKG-INFO
+-rw-r--r--   0 zhengy     (501) staff       (20)      280 2023-07-11 10:11:29.000000 lesscode_tag-0.0.5/lesscode_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengy     (501) staff       (20)        1 2023-07-11 10:11:29.000000 lesscode_tag-0.0.5/lesscode_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengy     (501) staff       (20)       13 2023-07-11 10:11:29.000000 lesscode_tag-0.0.5/lesscode_tag.egg-info/top_level.txt
+-rw-r--r--   0 zhengy     (501) staff       (20)       38 2023-07-11 10:11:29.000000 lesscode_tag-0.0.5/setup.cfg
+-rw-r--r--   0 zhengy     (501) staff       (20)     1273 2023-05-25 10:25:23.000000 lesscode_tag-0.0.5/setup.py
```

### Comparing `lesscode_tag-0.0.4/lesscode_tag/aes.py` & `lesscode_tag-0.0.5/lesscode_tag/aes.py`

 * *Files identical despite different names*

### Comparing `lesscode_tag-0.0.4/lesscode_tag/business.py` & `lesscode_tag-0.0.5/lesscode_tag/business.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,81 +40,113 @@
         should.append({"bool": {"must": [{"terms": {"tags.market_tag.status": [tag]}}]}})
     if tag in ["规上企业"]:
         should.append({"bool": {"must": [{"terms": {"tags.nonpublic_tag": [tag]}}]}})
     condition = {"bool": {"should": should}}
     return condition
 
 
-def format_param_tag(bool_should_more_list, especial_tag_list, is_need_decrypt=False, aes_key="haohaoxuexi"):
+def format_param_tag(bool_should_more_list, especial_tag_list):
     bool_should_list = []
     if especial_tag_list is not None:
         for tag in especial_tag_list:
-
             if tag == "省级专精特新":
-                bool_should_list.append({"bool": {"must": [
-                    {"terms": {"tags.diy_tag": ["省级专精特新企业"]}},
-                    {"bool": {"must_not": [{"terms": {"tags.diy_tag": ["国家级专精特新企业"]}}]}}
-                ]
-                }
-                })
+                bool_should_list.append(
+                    {"bool":
+                        {"must": [
+                            {"terms": {"tags.diy_tag": ["省级专精特新企业"]}},
+                            {"bool": {"must_not": [{"terms": {"tags.diy_tag": ["国家级专精特新企业"]}}]}}
+                        ]
+                        }
+                    })
             if tag in ["国家级专精特新", "国家级单项冠军", "瞪羚"]:
-                es_condition_by_terms(bool_must_list=bool_should_list, column="tags.diy_tag", param_list=[tag + "企业"],
-                                      is_need_decrypt=is_need_decrypt, key=aes_key)
+                es_condition_by_terms(bool_should_list, "tags.diy_tag", [tag + "企业"])
             if tag in ["高新技术企业", "央企", "瞪羚企业", "中国企业500强"]:
-                es_condition_by_terms(bool_must_list=bool_should_list, column="tags.diy_tag", param_list=[tag],
-                                      is_need_decrypt=is_need_decrypt, key=aes_key)
+                es_condition_by_terms(bool_should_list, "tags.diy_tag", [tag])
             if tag in ["单项冠军"]:
-                es_condition_by_terms(bool_must_list=bool_should_list, column="tags.diy_tag",
-                                      param_list=["国家级单项冠军企业"],
-                                      is_need_decrypt=is_need_decrypt, key=aes_key)
+                es_condition_by_terms(bool_should_list, "tags.diy_tag", ["国家级单项冠军企业"])
             if tag in ["专精特新"]:
-                es_condition_by_terms(bool_must_list=bool_should_list, column="tags.diy_tag",
-                                      param_list=["省级专精特新企业", "国家级专精特新企业"],
-                                      is_need_decrypt=is_need_decrypt, key=aes_key)
-            # 上市信息
+                es_condition_by_terms(bool_should_list, "tags.diy_tag", ["省级专精特新企业", "国家级专精特新企业"])
+            # 需评估 "A股上市" 是不是还有存在的额必要  是不是都用 "上市企业"
             if tag in ["A股上市"]:
-                bool_should_list.append({"bool": {"must": [
-                    {"terms": {"tags.market_tag.block": ["主板上市", "科创板上市", "创业板上市", "北交所"]}},
-                    {"terms": {"tags.market_tag.status": ["已上市"]}}
-                ]
-                }
-                })
+                bool_should_list.append(
+                    {"bool":
+                        {"must": [
+                            {"terms": {"tags.market_tag.block": ["主板上市", "科创板上市", "创业板上市", "北交所"]}},
+                            {"terms": {"tags.market_tag.status": ["已上市"]}}
+                        ]
+                        }
+                    })
+            if tag in ["上市企业"]:
+                bool_should_list.append(
+                    {"bool":
+                        {"must": [
+                            {"terms": {
+                                "tags.market_tag.block": ["主板上市", "创业板上市", "科创板上市", "北交所", "港股主板",
+                                                          "港股创业板", "中概股主板", "中概股创业板"]}},
+                            {"terms": {"tags.market_tag.status": ["已上市"]}}
+                        ]
+                        }
+                    })
             if tag in ["新三板"]:
-                es_condition_by_terms(bool_must_list=bool_should_list, column="tags.market_tag.status",
-                                      param_list=["新三板挂牌"],
-                                      is_need_decrypt=is_need_decrypt, key=aes_key)
+                es_condition_by_terms(bool_should_list, "tags.market_tag.status", ["新三板挂牌"])
             if tag in ["已上市", "排队上市", "已退市"]:
-                es_condition_by_terms(bool_must_list=bool_should_list, column="tags.market_tag.status",
-                                      param_list=[tag],
-                                      is_need_decrypt=is_need_decrypt, key=aes_key)
+                es_condition_by_terms(bool_should_list, "tags.market_tag.status", [tag])
             if tag in ["主板上市", "创业板上市", "科创板上市", "新三板-基础层", "新三板-创新层", "新三板-精选层",
                        "北交所"]:
-                es_condition_by_terms(bool_must_list=bool_should_list, column="tags.market_tag.block", param_list=[tag],
-                                      is_need_decrypt=is_need_decrypt, key=aes_key)
+                es_condition_by_terms(bool_should_list, "tags.market_tag.block", [tag])
             # 其他  -此类不标准，尽量不要使用
             if tag in ["小巨人", "一条龙"]:
                 es_condition_by_wildcard(bool_should_list, "tags.national_tag.tag_name", tag)
             if tag in ["隐形冠军", "成长", "小巨人", "首台套", "雏鹰", "省级单项冠军"]:
                 es_condition_by_wildcard(bool_should_list, "tags.province_tag.tag_name", tag)
             if tag in ["雏鹰"]:
                 es_condition_by_wildcard(bool_should_list, "tags.city_tag.tag_name", tag)
             if tag in ["雏鹰"]:
                 es_condition_by_wildcard(bool_should_list, "tags.district_tag.tag_name", tag)
             if tag in ["独角兽"]:
                 es_condition_by_wildcard(bool_should_list, "tags.rank_tag.rank_name", tag)
             if tag in ["科技型中小企业"]:
-                es_condition_by_terms(bool_must_list=bool_should_list, column="tags.certification.certification_name",
-                                      param_list=[tag],
-                                      is_need_decrypt=is_need_decrypt, key=aes_key)
+                es_condition_by_terms(bool_should_list, "tags.certification.certification_name", [tag])
             if tag in ["规上企业"]:
-                es_condition_by_terms(bool_must_list=bool_should_list, column="tags.nonpublic_tag", param_list=[tag],
-                                      is_need_decrypt=is_need_decrypt, key=aes_key)
+                es_condition_by_terms(bool_should_list, "tags.nonpublic_tag", [tag])
     bool_should_more_list.append(bool_should_list)
 
 
+def parse_special_tag_new(tags, tags_param_list=None):
+    """新版产业通 特色标签 解析，临时用等数据组将标签添加到diy_tag修改此方法"""
+    result = []
+    for tag in tags.get("market_tag", []):
+        if tag.get("status", "") == "已上市" and tag.get("block", "") in ["主板上市", "科创板上市", "创业板上市", "北交所"]:
+            result.append("A股上市")
+        if tag.get("status", "") == "新三板挂牌":
+            result.append("新三板")
+    for tag in tags.get("diy_tag", []):
+        for t in ["国家级专精特新", "省级专精特新", "国家级单项冠军", '瞪羚']:
+            if t in tag:
+                result.append(t)
+        if tag in ["央企"]:
+            result.append(tag)
+    for tag in tags.get("province_tag", []):
+        if "单项冠军" in tag.get("tag_name", ""):
+            result.append("省级单项冠军")
+    for tag in tags.get("rank_tag", []):
+        if "独角兽" in tag.get("rank_name", ""):
+            result.append("独角兽")
+        if "中国企业500强" in tag.get("rank_name", ""):
+            result.append("中国企业500强")
+    for tag in tags.get("certification", []):
+        if tag.get("certification_name", "") in ["科技型中小企业", "高新技术企业"]:
+            result.append(tag.get("certification_name", ""))
+    if tags_param_list:
+        result = list(set(tags_param_list) & set(result))
+    else:
+        result = list(set(result))
+    return result
+
+
 def format_special_tag_list(special_tag_list=None):
     bool_should_list = []
     if special_tag_list:
         for special_tag in special_tag_list:
             if isinstance(special_tag, list):
                 bool_must_list = []
                 for _tag in special_tag:
```

### Comparing `lesscode_tag-0.0.4/lesscode_tag/es_util.py` & `lesscode_tag-0.0.5/lesscode_tag/es_util.py`

 * *Files identical despite different names*

### Comparing `lesscode_tag-0.0.4/setup.py` & `lesscode_tag-0.0.5/setup.py`

 * *Files identical despite different names*

