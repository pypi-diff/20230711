# Comparing `tmp/trtpg-1.2.0-py3-none-any.whl.zip` & `tmp/trtpg-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 32416 bytes, number of entries: 20
+Zip file size: 32698 bytes, number of entries: 20
 -rw-r--r--  2.0 unx     1188 b- defN 23-Jun-29 08:06 tpg/__init__.py
--rw-r--r--  2.0 unx     4088 b- defN 23-Jun-29 08:06 tpg/config.py
+-rw-r--r--  2.0 unx     5265 b- defN 23-Jul-11 06:25 tpg/config.py
 -rw-r--r--  2.0 unx     8136 b- defN 23-Jun-29 08:06 tpg/extract_unsupported_operators.py
--rw-r--r--  2.0 unx    25967 b- defN 23-Jun-30 10:11 tpg/generate.py
+-rw-r--r--  2.0 unx    26486 b- defN 23-Jul-11 06:25 tpg/generate.py
 -rw-r--r--  2.0 unx     1438 b- defN 23-Jun-29 08:06 tpg/log.py
 -rw-r--r--  2.0 unx     4198 b- defN 23-Jun-29 08:06 tpg/tpg.py
 -rw-r--r--  2.0 unx     2652 b- defN 23-Jun-29 08:06 tpg/yaml_parser.py
 -rw-r--r--  2.0 unx     9401 b- defN 23-Jun-29 08:06 tpg/plugin_templates/IPluginV2DynamicExt.cpp
 -rw-r--r--  2.0 unx     4895 b- defN 23-Jun-29 08:06 tpg/plugin_templates/IPluginV2DynamicExt.h
 -rw-r--r--  2.0 unx     8977 b- defN 23-Jun-29 08:06 tpg/plugin_templates/IPluginV2IOExt.cpp
 -rw-r--r--  2.0 unx     4706 b- defN 23-Jun-29 08:06 tpg/plugin_templates/IPluginV2IOExt.h
 -rw-r--r--  2.0 unx     1381 b- defN 23-Jun-29 08:06 tpg/plugin_templates/license.template
 -rw-r--r--  2.0 unx     1772 b- defN 23-Jun-29 08:06 tpg/plugin_templates/makefile
 -rw-r--r--  2.0 unx     1976 b- defN 23-Jun-29 08:06 tpg/plugin_templates/supported_operator_trt84.txt
--rw-r--r--  2.0 unx     1084 b- defN 23-Jun-30 10:13 trtpg-1.2.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     5050 b- defN 23-Jun-30 10:13 trtpg-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 10:13 trtpg-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-Jun-30 10:13 trtpg-1.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-30 10:13 trtpg-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1664 b- defN 23-Jun-30 10:13 trtpg-1.2.0.dist-info/RECORD
-20 files, 88709 bytes uncompressed, 29706 bytes compressed:  66.5%
+-rw-r--r--  2.0 unx     1084 b- defN 23-Jul-11 06:25 trtpg-1.3.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     5050 b- defN 23-Jul-11 06:25 trtpg-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 06:25 trtpg-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-Jul-11 06:25 trtpg-1.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-11 06:25 trtpg-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1664 b- defN 23-Jul-11 06:25 trtpg-1.3.0.dist-info/RECORD
+20 files, 90405 bytes uncompressed, 29988 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: tpg/plugin_templates/makefile
 Comment: 
 
 Filename: tpg/plugin_templates/supported_operator_trt84.txt
 Comment: 
 
-Filename: trtpg-1.2.0.dist-info/LICENSE.md
+Filename: trtpg-1.3.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: trtpg-1.2.0.dist-info/METADATA
+Filename: trtpg-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: trtpg-1.2.0.dist-info/WHEEL
+Filename: trtpg-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: trtpg-1.2.0.dist-info/entry_points.txt
+Filename: trtpg-1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: trtpg-1.2.0.dist-info/top_level.txt
+Filename: trtpg-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: trtpg-1.2.0.dist-info/RECORD
+Filename: trtpg-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpg/config.py

```diff
@@ -27,14 +27,31 @@
 
 class Attribute:
     def __init__(self):
         self.name = ""
         self.type = ""
         self.default_value = None
 
+class Format:
+    def __init__(self, datatype, tensor_format):
+        self.datatype = datatype
+        self.tensor_format = tensor_format.upper()
+    def validate(self):
+        assert self.datatype in ['float32', 'float16', 'int8', 'int32'], 'Unsupported datatype'
+        assert self.tensor_format in ['LINEAR', 'CHW32', 'CHW2', 'HWC8', 'HWC16', 'DHWC8', 'CHW4'], 'Unsupported data format'
+        # refer to https://docs.nvidia.com/deeplearning/tensorrt/developer-guide/index.html#ipluginv2
+        if self.datatype == 'float32':
+            assert self.tensor_format in ['LINEAR', 'CHW32'], 'Unsupported data format for float32'
+        if self.datatype == 'float16':
+            assert self.tensor_format in ['LINEAR', 'CHW2', 'HWC8', 'HWC16', 'DHWC8', 'CHW4'], 'Unsupported data format for float16'
+        if self.datatype == 'int8':
+            assert self.tensor_format in ['LINEAR', 'CHW32', 'CHW4'], 'Unsupported data format for int8'
+        if self.datatype == 'int32':
+            assert self.tensor_format in ['LINEAR'], 'Unsupported data format for int32'
+
 class Config:
     '''Config for a custom plugin
     Attributes
         plugin_name: identifier of the operator, as known as the type of an onnx operator.
         plugin_type: TensorRT's plugin type, support type:
             IPluginV2DynamicExt, IPluginV2IOExt
         inputs: inputs information, including name and dimension
@@ -77,20 +94,24 @@
             dim = int(dim)
             t.dims.append(dim)
         self.outputs.append(t)
 
     def AddSupportFormatCombination(self, format_combination):
         l = []
         assert format_combination != "need_user_to_specify", "please specify the format combination"
-        formats = format_combination.split('+')
-        assert len(formats) == (len(self.inputs) + len(self.outputs)), 'error: tensor counts mismatch'
-        for format in formats:
-            assert format in ['float32', 'float16', 'int8', 'int32'], 'unsupported format, please set it like float32+float16+int8'
-            l.append(format)
-        self.support_format_combination.append(l)
+        items = format_combination.split('+')
+        formats = []
+        for item in items:
+            datatype = item.split(':')[0]
+            tensor_format = item.split(':')[1] if len(item.split(':')) > 1 else "LINEAR"
+            format = Format(datatype, tensor_format)
+            format.validate()
+            formats.append(format)
+        assert len(formats) == (len(self.inputs) + len(self.outputs)), 'Error: formats mismatch'
+        self.support_format_combination.append(formats)
 
     def AddAttr(self, attr_name, attr_type, default_value = None):
         a = Attribute()
         a.name = attr_name
         a.type = attr_type
         a.default_value = default_value
         datatype = a.type.split('[')[0]
```

## tpg/generate.py

```diff
@@ -189,28 +189,33 @@
     elif str.startswith("char"):
         return 'kCHAR'
     elif str.startswith("dims"):
         return 'kDIMS'
     else:
         return 'kUNKNOWN'
 
-def get_trt_datatype(str):
+def get_trt_datatype(format):
+    str = format.datatype
     if str.startswith("float16"):
         return 'kHALF'
     elif str.startswith("float32"):
         return 'kFLOAT'
     elif str.startswith("int8"):
         return 'kINT8'
     elif str.startswith("int32"):
         return 'kINT32'
     elif str.startswith("bool"):
         return 'kBOOL'
     else:
         assert False, 'error: wrong datatype: '+str
 
+def get_trt_tensor_format(format):
+    str = format.tensor_format
+    return 'k' + str
+
 def codegen_plugin_attributes_emplace_back(config):
     template = "mPluginAttributes.emplace_back(PluginField(\"$attr_name\", nullptr, PluginFieldType::$field_Type, 1));"
     ret_str = ''
     for attr in config.attrs:
         line = template.replace("$attr_name", attr.name)
         line = line.replace("$field_Type", get_plugin_field_type_str(attr.type))
         ret_str += (line + '\n    ')
@@ -317,18 +322,19 @@
             ret_str += ('        {\n')
             ret_str += ('            {}.{} = *(reinterpret_cast<const {}*>(fields[i].data));\n'.format(PARAMS_NAME, name, cxx_type))
             ret_str += ('        }\n')
     ret_str += ('    }\n')
 
     return ret_str
 
-def get_input_combination_str(param_name, format_combination, num_input, tensor_format):
+def get_input_combination_str(param_name, format_combination, num_input):
     ret_str = ''
     for i in range(num_input):
         datatype = get_trt_datatype(format_combination[i])
+        tensor_format = get_trt_tensor_format(format_combination[i])
         ret_str += f'{param_name}[{i}].type == DataType::{datatype} && {param_name}[{i}].format == TensorFormat::{tensor_format} &&\n            '
     return ret_str
 
 def get_input_combination_str_v2(param_name, format_combination, num_input):
     ret_str = ''
     for i in range(num_input):
         ret_str += '{}[{}] == DataType::{} &&\n           '.format(param_name, i, get_trt_datatype(format_combination[i]))
@@ -420,35 +426,38 @@
 def codegen_get_support_format_combination(config):
     ret_str = ''
     num_input = len(config.inputs)
     num_output = len(config.outputs)
     num_io = num_input + num_output
     support_format_combination = config.support_format_combination
     for i in range(num_io):
-        tensor_format = 'kLINEAR'
         if i < num_input:
             ret_str += ('    if(pos == {})\n'.format(i))
             ret_str += ('    {\n')
             ret_str += ('        is_supported =\n')
             for j in range(len(support_format_combination) - 1):
                 option = get_trt_datatype(support_format_combination[j][i])
+                tensor_format = get_trt_tensor_format(support_format_combination[j][i])
                 ret_str += ('            (inOut[pos].type == DataType::{} && inOut[pos].format == TensorFormat::{}) ||\n'.format(option, tensor_format))
             option = get_trt_datatype(support_format_combination[len(support_format_combination) - 1][i])
+            tensor_format = get_trt_tensor_format(support_format_combination[len(support_format_combination) - 1][i])
             ret_str += ('            (inOut[pos].type == DataType::{} && inOut[pos].format == TensorFormat::{});\n'.format(option, tensor_format))
             ret_str += ('    }\n')
         else:
             ret_str += ('    if(pos == {})\n'.format(i))
             ret_str += ('    {\n')
             ret_str += ('        is_supported =\n')
             for j in range(len(support_format_combination) - 1):
-                inputs_option = get_input_combination_str('inOut', support_format_combination[j], num_input, tensor_format)
+                tensor_format = get_trt_tensor_format(support_format_combination[j][i])
+                inputs_option = get_input_combination_str('inOut', support_format_combination[j], num_input)
                 option = get_trt_datatype(support_format_combination[j][i])
                 ret_str += ('            ({}inOut[pos].type == DataType::{} && inOut[pos].format == TensorFormat::{}) ||\n'.format(inputs_option, option, tensor_format))
-            inputs_option = get_input_combination_str('inOut', support_format_combination[len(support_format_combination) - 1], num_input, tensor_format)
+            inputs_option = get_input_combination_str('inOut', support_format_combination[len(support_format_combination) - 1], num_input)
             option = get_trt_datatype(support_format_combination[len(support_format_combination) - 1][i])
+            tensor_format = get_trt_tensor_format(support_format_combination[len(support_format_combination) - 1][i])
             ret_str += ('            ({}inOut[pos].type == DataType::{} && inOut[pos].format == TensorFormat::{});\n'.format(inputs_option, option, tensor_format))
             ret_str += ('    }\n')
     return ret_str
 
 def generate_plugin_common_api(config, h, cpp):
     capitalized_name = get_capital_name(config.plugin_name)
     # parse attribute
```

## Comparing `trtpg-1.2.0.dist-info/LICENSE.md` & `trtpg-1.3.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `trtpg-1.2.0.dist-info/METADATA` & `trtpg-1.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trtpg
-Version: 1.2.0
+Version: 1.3.0
 Summary: Generate TensorRT plugin in fly
 Home-page: https://github.com/NVIDIA-AI-IOT/tensorrt_plugin_generator
 Author-email: cntse@nvidia.com
 License: UNKNOWN
 Keywords: tensorrt plugin generator
 Platform: linux
 Classifier: Intended Audience :: Developers
```

## Comparing `trtpg-1.2.0.dist-info/RECORD` & `trtpg-1.3.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 tpg/__init__.py,sha256=aUT9KqqX8pxwHpztw-xrAQ63TcsYUsoWVlp-nal1Flo,1188
-tpg/config.py,sha256=dZn52Tf0QgOfmsOctmpQOfh0tZ82OHM-pIlPgzLEfgw,4088
+tpg/config.py,sha256=cnxUviEHrqgiL9L_8zIH1Tix-1C42ytlJHqnxiq0JMg,5265
 tpg/extract_unsupported_operators.py,sha256=4jbT-dsO5EBYcY6dEFicJTVug4249t7TtLdu1m73E5s,8136
-tpg/generate.py,sha256=OVqBIKuqwG37THz5Mf0OvatKwas2f4e537ChxypLFLY,25967
+tpg/generate.py,sha256=Td9UkfY7oJfGasu_93weeKxLsgPProJPFRqyxSSoy4s,26486
 tpg/log.py,sha256=4re8r5e3hgBhYCVBnf_Us5bbvIhBrryY_JRPK9DDjJk,1438
 tpg/tpg.py,sha256=0r_lalBNedtyDWmzAzKgEbHhvXDP01KNHTDids176S0,4198
 tpg/yaml_parser.py,sha256=9RMvO2J2txuIqw6j9Cij1Zjh1ubEvTPbamn_VLa4VD4,2652
 tpg/plugin_templates/IPluginV2DynamicExt.cpp,sha256=EpTOjNl93zJtpRfgyHV5jG67CzvccxmluafSViEYd8w,9401
 tpg/plugin_templates/IPluginV2DynamicExt.h,sha256=Mdi2JWdKLNlO2AomKbTwTYQ99goxvEnPIqJgRYaQ1hM,4895
 tpg/plugin_templates/IPluginV2IOExt.cpp,sha256=2-tJxkGgBulxQ2LJxQVNB3lOt-8sox9S6gFh1dvs3CM,8977
 tpg/plugin_templates/IPluginV2IOExt.h,sha256=qHqifyPEFFmkn697Tj2AGXgr6_B9Y-sDH37mYYMxgdk,4706
 tpg/plugin_templates/license.template,sha256=ScXqVT3Yys-KllzIrPx613rbWt5oruTq277K3hHDllU,1381
 tpg/plugin_templates/makefile,sha256=3t4hIjFJD_wnHB1XhqvEdtSNqdWsZwc8thm_TupmZGc,1772
 tpg/plugin_templates/supported_operator_trt84.txt,sha256=EOlrwRG0u2FVLfXgVoYMr0eqxhKorv21InYcVk1qYCM,1976
-trtpg-1.2.0.dist-info/LICENSE.md,sha256=59W3aI6gNG4CwIWjCSh4yXr937oWCIbPdtlrysRfckY,1084
-trtpg-1.2.0.dist-info/METADATA,sha256=5Od9moB7u-xmQ0sYJd5CRtUMlv0Y_Oek7pWA8rB7ZOk,5050
-trtpg-1.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-trtpg-1.2.0.dist-info/entry_points.txt,sha256=fvhG-i1SULYY5398rJs4MS-hY56euD-b7_1iaIO4Um4,40
-trtpg-1.2.0.dist-info/top_level.txt,sha256=ccJvmBjfWONfJiaL4Qr0Rr75Epz2vYJSJvbJ-LAL8tM,4
-trtpg-1.2.0.dist-info/RECORD,,
+trtpg-1.3.0.dist-info/LICENSE.md,sha256=59W3aI6gNG4CwIWjCSh4yXr937oWCIbPdtlrysRfckY,1084
+trtpg-1.3.0.dist-info/METADATA,sha256=rTQYy3SrzLzcxhwX9v64HgflfJ156d0NVj_qBNlPWAM,5050
+trtpg-1.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+trtpg-1.3.0.dist-info/entry_points.txt,sha256=fvhG-i1SULYY5398rJs4MS-hY56euD-b7_1iaIO4Um4,40
+trtpg-1.3.0.dist-info/top_level.txt,sha256=ccJvmBjfWONfJiaL4Qr0Rr75Epz2vYJSJvbJ-LAL8tM,4
+trtpg-1.3.0.dist-info/RECORD,,
```

