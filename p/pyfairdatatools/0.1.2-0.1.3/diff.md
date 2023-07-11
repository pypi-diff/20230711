# Comparing `tmp/pyfairdatatools-0.1.2.tar.gz` & `tmp/pyfairdatatools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfairdatatools-0.1.2.tar", max compression
+gzip compressed data, was "pyfairdatatools-0.1.3.tar", max compression
```

## Comparing `pyfairdatatools-0.1.2.tar` & `pyfairdatatools-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1109 2023-05-04 17:42:12.820675 pyfairdatatools-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      257 2023-07-11 20:51:14.926401 pyfairdatatools-0.1.2/pyfairdatatools/__init__.py
--rw-r--r--   0        0        0      199 2023-05-09 00:30:52.905419 pyfairdatatools-0.1.2/pyfairdatatools/__main__.py
--rw-r--r--   0        0        0    15683 2023-06-19 19:50:06.297393 pyfairdatatools-0.1.2/pyfairdatatools/assets/languages.json
--rw-r--r--   0        0        0   251950 2023-05-18 20:27:24.899227 pyfairdatatools-0.1.2/pyfairdatatools/assets/licenses.json
--rw-r--r--   0        0        0      636 2023-05-09 00:54:20.112753 pyfairdatatools-0.1.2/pyfairdatatools/cli.py
--rw-r--r--   0        0        0    12566 2023-07-11 00:10:10.930787 pyfairdatatools-0.1.2/pyfairdatatools/generate.py
--rw-r--r--   0        0        0     3005 2023-05-04 20:33:46.686345 pyfairdatatools-0.1.2/pyfairdatatools/gui.py
--rw-r--r--   0        0        0    71270 2023-07-06 18:02:25.758085 pyfairdatatools-0.1.2/pyfairdatatools/schemas/dataset_description.schema.json
--rw-r--r--   0        0        0     2854 2023-07-06 18:02:25.759069 pyfairdatatools-0.1.2/pyfairdatatools/schemas/folder_structure.schema.json
--rw-r--r--   0        0        0     2222 2023-07-06 18:02:25.759069 pyfairdatatools-0.1.2/pyfairdatatools/schemas/participants.schema.json
--rw-r--r--   0        0        0     3300 2023-07-06 18:02:25.760069 pyfairdatatools-0.1.2/pyfairdatatools/schemas/readme.schema.json
--rw-r--r--   0        0        0    68051 2023-07-10 23:27:33.272942 pyfairdatatools-0.1.2/pyfairdatatools/schemas/study_description.schema.json
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.762076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/activity_monitor/README.md
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/best_corrected_visual_acuity/README.md
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.761077 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/CHANGELOG.md
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/dataset_description.json
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.761077 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/participants.json
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.764075 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/participants.tsv
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.762076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/README.md
--rw-r--r--   0        0        0      442 2023-05-22 21:03:22.914816 pyfairdatatools-0.1.2/pyfairdatatools/templates/readme.mdtxt.template
--rw-r--r--   0        0        0       35 2023-05-04 17:42:12.915909 pyfairdatatools-0.1.2/pyfairdatatools/tests/__init__.py
--rw-r--r--   0        0        0      278 2023-05-04 20:19:34.392045 pyfairdatatools-0.1.2/pyfairdatatools/tests/conftest.py
--rw-r--r--   0        0        0     1417 2023-05-30 22:36:52.736046 pyfairdatatools-0.1.2/pyfairdatatools/utils.py
--rw-r--r--   0        0        0    13715 2023-07-10 23:38:43.990162 pyfairdatatools-0.1.2/pyfairdatatools/validate.py
--rw-r--r--   0        0        0     2997 2023-07-11 20:51:06.840155 pyfairdatatools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8119 2023-07-11 20:12:21.296144 pyfairdatatools-0.1.2/README.md
--rw-r--r--   0        0        0     9465 1970-01-01 00:00:00.000000 pyfairdatatools-0.1.2/setup.py
--rw-r--r--   0        0        0     9271 1970-01-01 00:00:00.000000 pyfairdatatools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-05-04 17:42:12.820675 pyfairdatatools-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0      257 2023-07-11 21:01:49.711560 pyfairdatatools-0.1.3/pyfairdatatools/__init__.py
+-rw-r--r--   0        0        0      199 2023-05-09 00:30:52.905419 pyfairdatatools-0.1.3/pyfairdatatools/__main__.py
+-rw-r--r--   0        0        0    15683 2023-06-19 19:50:06.297393 pyfairdatatools-0.1.3/pyfairdatatools/assets/languages.json
+-rw-r--r--   0        0        0   251950 2023-05-18 20:27:24.899227 pyfairdatatools-0.1.3/pyfairdatatools/assets/licenses.json
+-rw-r--r--   0        0        0      636 2023-05-09 00:54:20.112753 pyfairdatatools-0.1.3/pyfairdatatools/cli.py
+-rw-r--r--   0        0        0    12566 2023-07-11 00:10:10.930787 pyfairdatatools-0.1.3/pyfairdatatools/generate.py
+-rw-r--r--   0        0        0     3005 2023-05-04 20:33:46.686345 pyfairdatatools-0.1.3/pyfairdatatools/gui.py
+-rw-r--r--   0        0        0    71270 2023-07-06 18:02:25.758085 pyfairdatatools-0.1.3/pyfairdatatools/schemas/dataset_description.schema.json
+-rw-r--r--   0        0        0     2854 2023-07-06 18:02:25.759069 pyfairdatatools-0.1.3/pyfairdatatools/schemas/folder_structure.schema.json
+-rw-r--r--   0        0        0     2222 2023-07-06 18:02:25.759069 pyfairdatatools-0.1.3/pyfairdatatools/schemas/participants.schema.json
+-rw-r--r--   0        0        0     3300 2023-07-06 18:02:25.760069 pyfairdatatools-0.1.3/pyfairdatatools/schemas/readme.schema.json
+-rw-r--r--   0        0        0    68063 2023-07-11 20:59:53.521564 pyfairdatatools-0.1.3/pyfairdatatools/schemas/study_description.schema.json
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.762076 pyfairdatatools-0.1.3/pyfairdatatools/templates/high-level-dataset-structure/activity_monitor/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.3/pyfairdatatools/templates/high-level-dataset-structure/best_corrected_visual_acuity/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.761077 pyfairdatatools-0.1.3/pyfairdatatools/templates/high-level-dataset-structure/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.3/pyfairdatatools/templates/high-level-dataset-structure/dataset_description.json
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.761077 pyfairdatatools-0.1.3/pyfairdatatools/templates/high-level-dataset-structure/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.3/pyfairdatatools/templates/high-level-dataset-structure/participants.json
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.764075 pyfairdatatools-0.1.3/pyfairdatatools/templates/high-level-dataset-structure/participants.tsv
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.762076 pyfairdatatools-0.1.3/pyfairdatatools/templates/high-level-dataset-structure/README.md
+-rw-r--r--   0        0        0      442 2023-05-22 21:03:22.914816 pyfairdatatools-0.1.3/pyfairdatatools/templates/readme.mdtxt.template
+-rw-r--r--   0        0        0       35 2023-05-04 17:42:12.915909 pyfairdatatools-0.1.3/pyfairdatatools/tests/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-04 20:19:34.392045 pyfairdatatools-0.1.3/pyfairdatatools/tests/conftest.py
+-rw-r--r--   0        0        0     1417 2023-05-30 22:36:52.736046 pyfairdatatools-0.1.3/pyfairdatatools/utils.py
+-rw-r--r--   0        0        0    13715 2023-07-10 23:38:43.990162 pyfairdatatools-0.1.3/pyfairdatatools/validate.py
+-rw-r--r--   0        0        0     3011 2023-07-11 21:01:46.471084 pyfairdatatools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8119 2023-07-11 20:12:21.296144 pyfairdatatools-0.1.3/README.md
+-rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 pyfairdatatools-0.1.3/setup.py
+-rw-r--r--   0        0        0     9303 1970-01-01 00:00:00.000000 pyfairdatatools-0.1.3/PKG-INFO
```

### Comparing `pyfairdatatools-0.1.2/LICENSE.md` & `pyfairdatatools-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/assets/languages.json` & `pyfairdatatools-0.1.3/pyfairdatatools/assets/languages.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/assets/licenses.json` & `pyfairdatatools-0.1.3/pyfairdatatools/assets/licenses.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/cli.py` & `pyfairdatatools-0.1.3/pyfairdatatools/cli.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/generate.py` & `pyfairdatatools-0.1.3/pyfairdatatools/generate.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/gui.py` & `pyfairdatatools-0.1.3/pyfairdatatools/gui.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/schemas/dataset_description.schema.json` & `pyfairdatatools-0.1.3/pyfairdatatools/schemas/dataset_description.schema.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/schemas/folder_structure.schema.json` & `pyfairdatatools-0.1.3/pyfairdatatools/schemas/folder_structure.schema.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/schemas/participants.schema.json` & `pyfairdatatools-0.1.3/pyfairdatatools/schemas/participants.schema.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/schemas/readme.schema.json` & `pyfairdatatools-0.1.3/pyfairdatatools/schemas/readme.schema.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/schemas/study_description.schema.json` & `pyfairdatatools-0.1.3/pyfairdatatools/schemas/study_description.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999775723563931%*

 * *Differences: {"'definitions'": "{'studyIdType': {'oneOf': {4: {'description': 'Also required to enter a brief "*

 * *                  'description of the identifier (for example, the name of the organization that '*

 * *                  "issued the identifier)..'}}}, 'statusOptions': {'oneOf': {0: {'description': "*

 * *                  "'Study halted prematurely, prior to enrolment of the first participant.'}}}}",*

 * * "'properties'": "{'SponsorCollaboratorsModule': {'properties': {'ResponsibleParty': "*

 * *                 "{'properties' […]*

```diff
@@ -25,15 +25,15 @@
             ],
             "type": "object"
         },
         "statusOptions": {
             "oneOf": [
                 {
                     "const": "Withdrawn",
-                    "description": "Study halted prematurely, prior to enrolment of first participant."
+                    "description": "Study halted prematurely, prior to enrolment of the first participant."
                 },
                 {
                     "const": "Recruiting",
                     "description": "Participants are currently being recruited, whether or not any participants have yet been enrolled."
                 },
                 {
                     "const": "Active, not recruiting",
@@ -78,15 +78,15 @@
                 },
                 {
                     "const": "EudraCT Number",
                     "description": "Identifier assigned by the European Medicines Agency Clinical Trials Database (EudraCT).."
                 },
                 {
                     "const": "Other Identifier",
-                    "description": "Also required to enter a brief description of the identifier (for example, the name of organization that issued the identifier).."
+                    "description": "Also required to enter a brief description of the identifier (for example, the name of the organization that issued the identifier).."
                 }
             ],
             "type": "string"
         }
     },
     "description": "Add a description of the study and the dataset.",
     "properties": {
@@ -271,15 +271,15 @@
             ],
             "type": "object"
         },
         "ContactsLocationsModule": {
             "additionalProperties": false,
             "properties": {
                 "CentralContactList": {
-                    "description": "The name or title, toll-free telephone number and email address of a person to whom questions concerning enrollment at any location of the study can be addressed.",
+                    "description": "The name or title, toll-free telephone number, and email address of a person to whom questions concerning enrollment at any location of the study can be addressed.",
                     "items": {
                         "additionalProperties": false,
                         "properties": {
                             "CentralContactAffiliation": {
                                 "description": "If none, specify Unaffiliated.",
                                 "minLength": 1,
                                 "type": "string"
@@ -290,15 +290,15 @@
                                 "type": "string"
                             },
                             "CentralContactName": {
                                 "minLength": 1,
                                 "type": "string"
                             },
                             "CentralContactPhone": {
-                                "description": "Toll free phone number of the Central Contact Person. Use the format 800-555-5555 within the United States and Canada. If outside the United States and Canada, provide the full phone number, including the country code. 30 characters",
+                                "description": "Toll-free phone number of the Central Contact Person. Use the format 800-555-5555 within the United States and Canada. If outside the United States and Canada, provide the full phone number, including the country code. 30 characters",
                                 "maxLength": 30,
                                 "minLength": 1,
                                 "type": "string"
                             },
                             "CentralContactPhoneExt": {
                                 "description": "phone extension, if needed.",
                                 "minLength": 1,
@@ -568,15 +568,15 @@
                                                         "const": "Triple"
                                                     },
                                                     {
                                                         "const": "Quadruple"
                                                     },
                                                     {
                                                         "const": "N/A",
-                                                        "description": "Explicitly labelled as not applicable - usually because the study is non-interventional"
+                                                        "description": "Explicitly labeled as not applicable - usually because the study is non-interventional"
                                                     }
                                                 ],
                                                 "type": "string"
                                             },
                                             "DesignMaskingDescription": {
                                                 "description": "Provide information about other parties who may be masked in the clinical trial, if any.",
                                                 "minLength": 1,
@@ -769,37 +769,37 @@
                                                 },
                                                 {
                                                     "const": "Case-Only",
                                                     "description": "Single group of individuals with specific characteristics."
                                                 },
                                                 {
                                                     "const": "Case-Crossover",
-                                                    "description": "Characteristics of case immediately prior to disease onset (sometimes called the hazard period) compared to characteristics of same case at a prior time (that is, control period)."
+                                                    "description": "Characteristics of a case immediately prior to disease onset (sometimes called the hazard period) compared to characteristics of the same case at a prior time (that is, control period)."
                                                 },
                                                 {
                                                     "const": "Ecologic or Community",
-                                                    "description": "Geographically defined populations, such as countries or regions within a country, compared on a variety of environmental (for example, air pollution intensity, hours of sunlight) and/or global measures not reducible to individual level characteristics (for example, healthcare system, laws or policies median income, average fat intake, disease rate)."
+                                                    "description": "Geographically defined populations, such as countries or regions within a country, compared on a variety of environmental (for example, air pollution intensity, hours of sunlight) and/or global measures not reducible to individual-level characteristics (for example, healthcare system, laws or policies median income, average fat intake, disease rate)."
                                                 },
                                                 {
                                                     "const": "Family-Based",
-                                                    "description": "Studies conducted among family members, such as genetic studies within families or twin studies and studies of family environment."
+                                                    "description": "Studies conducted among family members, such as genetic studies within families or twin studies and studies of a family environment."
                                                 },
                                                 {
                                                     "const": "Other",
                                                     "description": "Explain in Detailed Description.."
                                                 }
                                             ],
                                             "type": "string"
                                         },
                                         "minItems": 1,
                                         "type": "array",
                                         "uniqueItems": true
                                     },
                                     "DesignTimePerspectiveList": {
-                                        "description": "Temporal relationship of observation period to time of participant enrollment.",
+                                        "description": "Temporal relationship of the observation period to the time of participant enrollment.",
                                         "items": {
                                             "oneOf": [
                                                 {
                                                     "const": "Retrospective",
                                                     "description": "Look back using observations collected predominantly prior to subject selection and enrollment."
                                                 },
                                                 {
@@ -1218,15 +1218,15 @@
                         "type": "object"
                     },
                     "minItems": 1,
                     "type": "array",
                     "uniqueItems": true
                 },
                 "SeeAlsoLinkList": {
-                    "description": "A web site directly relevant to the protocol may be entered, if desired. Do not include sites whose primary goal is to advertise or sell commercial products or services. Links to educational, research, government, and other non-profit web pages are acceptable. All submitted links are subject to review by ClinicalTrials.gov.",
+                    "description": "A website directly relevant to the protocol may be entered, if desired. Do not include sites that aim to advertise or sell commercial products or services. Links to educational, research, government, and other non-profit web pages are acceptable. All submitted links are subject to review by ClinicalTrials.gov.",
                     "items": {
                         "additionalProperties": false,
                         "properties": {
                             "SeeAlsoLinkLabel": {
                                 "description": "Title or brief description of the linked page.",
                                 "minLength": 1,
                                 "type": "string"
@@ -1317,15 +1317,15 @@
                             "oneOf": [
                                 {
                                     "const": "Sponsor",
                                     "description": "The entity (for example, corporation or agency) that initiates the study."
                                 },
                                 {
                                     "const": "Principal Investigator",
-                                    "description": "The individual designated as responsible party by the sponsor."
+                                    "description": "The individual designated as a responsible party by the sponsor."
                                 },
                                 {
                                     "const": "Sponsor-Investigator",
                                     "description": "The individual who both initiates and conducts the study."
                                 }
                             ],
                             "type": "string"
```

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/utils.py` & `pyfairdatatools-0.1.3/pyfairdatatools/utils.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyfairdatatools/validate.py` & `pyfairdatatools-0.1.3/pyfairdatatools/validate.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/pyproject.toml` & `pyfairdatatools-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "pyfairdatatools"
-version = "0.1.2"
+version = "0.1.3"
 description = "Tools for AI-READI"
 
 packages = [{ include = "pyfairdatatools" }]
 
 license = "MIT"
 authors = ["FAIR Data Innovations Hub <contact@fairdataihub.org>"]
 
@@ -38,14 +38,15 @@
 click = "*"
 minilog = "*"
 jsonschema = "^4.17.3"
 dicttoxml = "^1.7.16"
 types-requests = "^2.30.0.0"
 pymdown-extensions = "^10.0.1"
 validators = "^0.20.0"
+art = "^6.0"
 
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
 black = "^22.1"
 tomli = "*" # missing 'black' dependency
```

### Comparing `pyfairdatatools-0.1.2/README.md` & `pyfairdatatools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.2/setup.py` & `pyfairdatatools-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,30 @@
                      'schemas/*',
                      'templates/*',
                      'templates/high-level-dataset-structure/*',
                      'templates/high-level-dataset-structure/activity_monitor/*',
                      'templates/high-level-dataset-structure/best_corrected_visual_acuity/*']}
 
 install_requires = \
-['click',
+['art>=6.0,<7.0',
+ 'click',
  'dicttoxml>=1.7.16,<2.0.0',
  'jsonschema>=4.17.3,<5.0.0',
  'minilog',
  'pymdown-extensions>=10.0.1,<11.0.0',
  'types-requests>=2.30.0.0,<3.0.0.0',
  'urllib3<2.0',
  'validators>=0.20.0,<0.21.0']
 
 entry_points = \
 {'console_scripts': ['pyfairdatatools = pyfairdatatools.cli:main']}
 
 setup_kwargs = {
     'name': 'pyfairdatatools',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Tools for AI-READI',
     'long_description': '<div align="center">\n\n<img src="https://freesvg.org/img/1653682897science-svgrepo-com.png" alt="logo" width="200" height="auto" />\n\n<br />\n\n<h1>pyfairdatatools</h1>\n\n<p>\nPython package for the FAIR tools of fairhub.io\n</p>\n\n<br />\n\n<p>\n  <a href="https://github.com/AI-READI/pyfairdatatools/graphs/contributors">\n    <img src="https://img.shields.io/github/contributors/AI-READI/pyfairdatatools.svg?style=flat-square" alt="contributors" />\n  </a>\n  <a href="https://github.com/AI-READI/pyfairdatatools/stargazers">\n    <img src="https://img.shields.io/github/stars/AI-READI/pyfairdatatools.svg?style=flat-square" alt="stars" />\n  </a>\n  <a href="https://github.com/AI-READI/pyfairdatatools/issues/">\n    <img src="https://img.shields.io/github/issues/AI-READI/pyfairdatatools.svg?style=flat-square" alt="open issues" />\n  </a>\n  <a href="https://github.com/AI-READI/pyfairdatatools/blob/main/LICENSE">\n    <img src="https://img.shields.io/github/license/AI-READI/pyfairdatatools.svg?style=flat-square" alt="license" />\n  </a>\n  <a href="https://fairdataihub.org/fairshare">\n    <img src="https://raw.githubusercontent.com/fairdataihub/FAIRshare/main/badge.svg" alt="Curated with FAIRshare" />\n  </a>\n</p>\n<p>\n  <a href="https://github.com/AI-READI/pyfairdatatools/actions">\n    <img src="https://img.shields.io/github/actions/workflow/status/AI-READI/pyfairdatatools/main.yml?branch=main&label=linux" alt="Unix Build Status" />\n  </a>\n  <a href="https://ci.appveyor.com/project/AI-READI/pyfairdatatools">\n    <img src="https://img.shields.io/appveyor/ci/AI-READI/pyfairdatatools.svg?label=windows" alt="Windows Build Status" />\n  </a>\n  <a href="https://codecov.io/gh/AI-READI/pyfairdatatools">\n    <img src="https://img.shields.io/codecov/c/gh/AI-READI/pyfairdatatools" alt="Coverage Status" />\n  </a>\n  <a href="https://scrutinizer-ci.com/g/AI-READI/pyfairdatatools">\n    <img src="https://img.shields.io/scrutinizer/g/AI-READI/pyfairdatatools.svg" alt="Scrutinizer Code Quality" />\n  </a>\n  <a href="https://pypi.org/project/pyfairdatatools">\n    <img src="https://img.shields.io/pypi/l/pyfairdatatools.svg" alt="PyPI License" />\n  </a>\n  <a href="https://pypi.org/project/pyfairdatatools">\n    <img src="https://img.shields.io/pypi/v/pyfairdatatools.svg" alt="PyPI Version" />\n  </a>\n  <a href="https://pypistats.org/packages/pyfairdatatools">\n    <img src="https://img.shields.io/pypi/dm/pyfairdatatools.svg?color=orange" alt="PyPI Downloads" />\n  </a>\n</p>\n\n<h4>\n    <a href="https://ai-readi.github.io/pyfairdatatools/">Documentation</a>\n  <span> · </span>\n    <a href="https://ai-readi.github.io/pyfairdatatools/about/changelog/">Changelog</a>\n  <span> · </span>\n    <a href="https://github.com/AI-READI/pyfairdatatools/issues/">Report Bug</a>\n  <span> · </span>\n    <a href="#">Request Feature</a>\n  </h4>\n</div>\n\n<br />\n\n---\n\n## Description\n\npyfairdatatools is a Python package that includes functions of fairhub.io for making data FAIR. This consists of a collection of helpful functions for extracting, transforming raw data, generating relevant metadata files and validating the data and metadata files against the FAIR guidelines adopted by the AI-READI project. Beside supporting fairhub.io, our aim is that the package can be used by anyone wanting to make their data FAIR according to the AI-READI FAIR guidelines.\n\n## Getting started\n\n### Prerequisites/Dependencies\n\nYou will need the following installed on your system:\n\n- Python 3.8+\n- [Pip](https://pip.pypa.io/en/stable/)\n- [Poetry](https://poetry.eustace.io/)\n\n### Installing\n\nInstall it directly into an activated virtual environment:\n\n```bash\npip install pyfairdatatools\n```\n\nor add it to your [Poetry](https://poetry.eustace.io/) project:\n\n```bash\npoetry add pyfairdatatools\n```\n\n### Usage\n\nAfter installation, the package can be imported:\n\n```bash\n$ python\n>>> import pyfairdatatools\n>>> pyfairdatatools.__version__\n```\n\n### Inputs and Outputs\n\nThe input of most functions will be a json format schema (see "Standards followed" sections) that contain data and metadata related information. The outputs of most functions will be standards metadata files, structured data, etc.\n\n## Standards followed\n\nThis software is being developed following the [Software Development Best Practices of the AI-READI Project](https://github.com/AI-READI/software-development-best-practices), which include following the [FAIR-BioRS guidelines](https://github.com/FAIR-BioRS/Guidelines). Amongs other, we are following closely the [PEP 8 Style Guide for Python Code](https://peps.python.org/pep-0008/).\n\nThe input structure of the function is currently being developed but anticipated to follow existing schemas such as schema.org and bioschemas.org.\n\n## Contributing\n\n<a href="https://github.com/AI-READI/pyfairdatatools/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=AI-READI/pyfairdatatools" />\n</a>\n\nContributions are always welcome!\n\nIf you are interested in reporting/fixing issues and contributing directly to the code base, please see [CONTRIBUTING.md](CONTRIBUTING.md) for more information on what we\'re looking for and how to get started.\n\n## Issues and Feedback\n\nTo report any issues with the software, suggest improvements, or request a new feature, please open a new issue via the [Issues](https://github.com/AI-READI/pyfairdatatools/issues) tab. Provide adequate information (operating system, steps leading to error, screenshots) so we can help you efficiently.\n\n### Setup\n\nIf you would like to update the package, please follow the instructions below.\n\n1. Create a local virtual environment and activate it:\n\n   ```bash\n   python -m venv .venv\n   source .venv/bin/activate\n   ```\n\n   If you are using Anaconda, you can create a virtual environment with:\n\n   ```bash\n   conda create -n pyfairdatatools-env python\n   conda activate pyfairdatatools-env\n   ```\n\n2. Install the dependencies for this package. We use [Poetry](https://poetry.eustace.io/) to manage the dependencies:\n\n   ```bash\n   pip install poetry==1.3.2\n   poetry install\n   ```\n\n   You can also use version 1.2.0 of Poetry, but you will need to run `poetry lock` after installing the dependencies.\n\n3. Add your modifications and run the tests:\n\n   ```bash\n   poetry run pytest\n   ```\n\n   If you need to add new python packages, you can use Poetry to add them:\n\n   ```bash\n    poetry add <package-name>\n   ```\n\n4. Format the code:\n\n   ```bash\n   poe format\n   ```\n\n5. Check the code quality:\n\n   ```bash\n   poetry run flake8 pyfairdatatools tests\n   ```\n\n6. Run the tests and check the code coverage:\n\n   ```bash\n   poe test\n   poe test --cov=pyfairdatatools\n   ```\n\n7. Build the package:\n\n   Update the version number in `pyproject.toml` and `pyfairdatatools/__init__.py` and then run:\n\n   ```text\n   poetry build\n   ```\n\n8. Publish the package:\n\n   ```bash\n   poetry publish\n   ```\n\n   Set your API token for PyPI in your environment variables:\n\n   ```bash\n   poetry config pypi-token.pypi your-api-token\n   ```\n\n## License\n\nThis work is licensed under\n[MIT](https://opensource.org/licenses/mit). See [LICENSE](https://github.com/AI-READI/pyfairdatatools/blob/main/LICENSE) for more information.\n\n<a href="https://aireadi.org" >\n  <img src="https://www.channelfutures.com/files/2017/04/3_0.png" height="30" />\n</a>\n\n## How to cite\n\nIf you are using this package or reusing the source code from this repository for any purpose, please cite:\n\n```text\n    Coming soon...\n```\n\n## Acknowledgements\n\nThis project is funded by the NIH under award number 1OT2OD032644. The content is solely the responsibility of the authors and does not necessarily represent the official views of the NIH.\n\nAdd any other acknowledgements here.\n\n<br />\n\n---\n\n<br />\n\n<div align="center">\n\n<a href="https://aireadi.org">\n  <img src="https://github.com/AI-READI/AI-READI-logo/raw/main/logo/png/option2.png" height="200" />\n</a>\n\n</div>\n',
     'author': 'FAIR Data Innovations Hub',
     'author_email': 'contact@fairdataihub.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/pyfairdatatools',
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['pyfairdatatools', 'pyfairdatatools.tests'] package_data = \ {'': ['*'],
 'pyfairdatatools': ['assets/*', 'schemas/*', 'templates/*', 'templates/high-
 level-dataset-structure/*', 'templates/high-level-dataset-structure/
 activity_monitor/*', 'templates/high-level-dataset-structure/
-best_corrected_visual_acuity/*']} install_requires = \ ['click',
-'dicttoxml>=1.7.16,<2.0.0', 'jsonschema>=4.17.3,<5.0.0', 'minilog', 'pymdown-
-extensions>=10.0.1,<11.0.0', 'types-requests>=2.30.0.0,<3.0.0.0',
+best_corrected_visual_acuity/*']} install_requires = \ ['art>=6.0,<7.0',
+'click', 'dicttoxml>=1.7.16,<2.0.0', 'jsonschema>=4.17.3,<5.0.0', 'minilog',
+'pymdown-extensions>=10.0.1,<11.0.0', 'types-requests>=2.30.0.0,<3.0.0.0',
 'urllib3<2.0', 'validators>=0.20.0,<0.21.0'] entry_points = \
 {'console_scripts': ['pyfairdatatools = pyfairdatatools.cli:main']}
-setup_kwargs = { 'name': 'pyfairdatatools', 'version': '0.1.2', 'description':
+setup_kwargs = { 'name': 'pyfairdatatools', 'version': '0.1.3', 'description':
 'Tools for AI-READI', 'long_description': '
                                 \n\n[logo]\n\n
                                      \n\n
                          ****** pyfairdatatools ******
                                      \n\n
               \nPython package for the FAIR tools of fairhub.io\n
                                      \n\n
```

### Comparing `pyfairdatatools-0.1.2/PKG-INFO` & `pyfairdatatools-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfairdatatools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for AI-READI
 Home-page: https://pypi.org/project/pyfairdatatools
 License: MIT
 Author: FAIR Data Innovations Hub
 Author-email: contact@fairdataihub.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: art (>=6.0,<7.0)
 Requires-Dist: click
 Requires-Dist: dicttoxml (>=1.7.16,<2.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: minilog
 Requires-Dist: pymdown-extensions (>=10.0.1,<11.0.0)
 Requires-Dist: types-requests (>=2.30.0.0,<3.0.0.0)
 Requires-Dist: urllib3 (<2.0)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pyfairdatatools Version: 0.1.2 Summary: Tools for
+Metadata-Version: 2.1 Name: pyfairdatatools Version: 0.1.3 Summary: Tools for
 AI-READI Home-page: https://pypi.org/project/pyfairdatatools License: MIT
 Author: FAIR Data Innovations Hub Author-email: contact@fairdataihub.org
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: click Requires-Dist: dicttoxml (>=1.7.16,<2.0.0) Requires-Dist:
-jsonschema (>=4.17.3,<5.0.0) Requires-Dist: minilog Requires-Dist: pymdown-
-extensions (>=10.0.1,<11.0.0) Requires-Dist: types-requests
-(>=2.30.0.0,<3.0.0.0) Requires-Dist: urllib3 (<2.0) Requires-Dist: validators
-(>=0.20.0,<0.21.0) Project-URL: Documentation, https://
+Requires-Dist: art (>=6.0,<7.0) Requires-Dist: click Requires-Dist: dicttoxml
+(>=1.7.16,<2.0.0) Requires-Dist: jsonschema (>=4.17.3,<5.0.0) Requires-Dist:
+minilog Requires-Dist: pymdown-extensions (>=10.0.1,<11.0.0) Requires-Dist:
+types-requests (>=2.30.0.0,<3.0.0.0) Requires-Dist: urllib3 (<2.0) Requires-
+Dist: validators (>=0.20.0,<0.21.0) Project-URL: Documentation, https://
 pyfairdatatools.readthedocs.io Project-URL: Repository, https://github.com/AI-
 READI/pyfairdatatools Description-Content-Type: text/markdown
                                     [logo]
                          ****** pyfairdatatools ******
                 Python package for the FAIR tools of fairhub.io
 
     [contributors] [stars] [open_issues] [license] [Curated_with_FAIRshare]
```

