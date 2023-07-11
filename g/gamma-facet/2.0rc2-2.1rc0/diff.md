# Comparing `tmp/gamma-facet-2.0rc2.tar.gz` & `tmp/gamma_facet-2.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamma-facet-2.0rc2.tar", last modified: Tue Jan 24 11:59:13 2023, max compression
+gzip compressed data, was "gamma_facet-2.1rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamma-facet-2.0rc2.tar` & `gamma_facet-2.1rc0.tar`

### file list

```diff
@@ -1,101 +1,116 @@
--rw-r--r--   0        0        0      666 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      689 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     4886 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/.gitignore
--rw-r--r--   0        0        0     1129 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/LICENSE
--rw-r--r--   0        0        0    20819 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/README.rst
--rw-r--r--   0        0        0     6385 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/RELEASE_NOTES.rst
--rw-r--r--   0        0        0    25478 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/azure-pipelines.yml
--rw-r--r--   0        0        0     2294 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/condabuild/meta.yaml
--rw-r--r--   0        0        0        0 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/config/spelling.dic
--rw-r--r--   0        0        0      124 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/config/test_config.yml
--rwxr-xr-x   0        0        0       93 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/dev-setup.sh
--rw-r--r--   0        0        0      988 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/environment.yml
--rwxr-xr-x   0        0        0      380 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/make.py
--rw-r--r--   0        0        0      751 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/mypy.ini
--rw-r--r--   0        0        0     2717 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/pypi_description.rst
--rw-r--r--   0        0        0     3875 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/pyproject.toml
--rw-r--r--   0        0        0       37 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/.gitignore
--rw-r--r--   0        0        0   199639 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/auxiliary/Diabetes_getting_started_example.ipynb
--rw-r--r--   0        0        0    10223 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb
--rwxr-xr-x   0        0        0      664 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/make.py
--rw-r--r--   0        0        0   130308 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/Facet-Simulator-BlockDiagram.png
--rw-r--r--   0        0        0    19522 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/Facet_Logo_Plain.png
--rw-r--r--   0        0        0     5238 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/Facet_flow.svg
--rw-r--r--   0        0        0     7117 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg
--rw-r--r--   0        0        0    23632 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/facet_banner.png
--rw-r--r--   0        0        0     1429 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/icons/inspect_icon.png
--rw-r--r--   0        0        0     2777 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/icons/pipe_icon.png
--rw-r--r--   0        0        0     2718 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/icons/sim_icon.png
--rw-r--r--   0        0        0   117900 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/ranker_summary.png
--rw-r--r--   0        0        0    27724 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/redundancy_dendrogram.png
--rw-r--r--   0        0        0    31712 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/redundancy_matrix.png
--rw-r--r--   0        0        0    38185 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/simulation_output.png
--rw-r--r--   0        0        0    31278 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/synergy_matrix.png
--rw-r--r--   0        0        0    49407 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Andy_Shora.jpg
--rw-r--r--   0        0        0     9901 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Florent_Martin.jpg
--rw-r--r--   0        0        0    11856 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Jan_Ittner.jpg
--rw-r--r--   0        0        0     8047 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Jason_Bentley.jpg
--rw-r--r--   0        0        0    10116 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg
--rw-r--r--   0        0        0     6673 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg
--rw-r--r--   0        0        0     9583 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Malo_Grisard.jpg
--rw-r--r--   0        0        0    49773 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg
--rw-r--r--   0        0        0    10100 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg
--rw-r--r--   0        0        0    10746 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg
--rw-r--r--   0        0        0      232 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_static/css/facet.css
--rw-r--r--   0        0        0     3673 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/about_us.rst
--rw-r--r--   0        0        0      371 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/api_landing.rst
--rw-r--r--   0        0        0      758 2023-01-24 11:57:26.352291 gamma-facet-2.0rc2/sphinx/source/conf.py
--rw-r--r--   0        0        0    20763 2023-01-24 11:57:26.352291 gamma-facet-2.0rc2/sphinx/source/contribution_guide.rst
--rw-r--r--   0        0        0     5693 2023-01-24 11:57:26.352291 gamma-facet-2.0rc2/sphinx/source/faqs.rst
--rw-r--r--   0        0        0      298 2023-01-24 11:57:26.352291 gamma-facet-2.0rc2/sphinx/source/index.rst
--rw-r--r--   0        0        0  1644456 2023-01-24 11:57:26.364291 gamma-facet-2.0rc2/sphinx/source/tutorial/Classification_with_Facet.ipynb
--rw-r--r--   0        0        0   970457 2023-01-24 11:57:26.368291 gamma-facet-2.0rc2/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv
--rw-r--r--   0        0        0   232448 2023-01-24 11:57:26.368291 gamma-facet-2.0rc2/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb
--rw-r--r--   0        0        0   107691 2023-01-24 11:57:26.368291 gamma-facet-2.0rc2/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb
--rw-r--r--   0        0        0   475484 2023-01-24 11:57:26.372291 gamma-facet-2.0rc2/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb
--rw-r--r--   0        0        0   820532 2023-01-24 11:57:26.376291 gamma-facet-2.0rc2/sphinx/source/tutorial/pre_diab_nhanes.csv
--rw-r--r--   0        0        0    85389 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/sphinx/source/tutorial/water_drilling_classification_data.csv
--rw-r--r--   0        0        0     2402 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/sphinx/source/tutorials.rst
--rw-r--r--   0        0        0      601 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/__init__.py
--rw-r--r--   0        0        0      102 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/data/__init__.py
--rw-r--r--   0        0        0    11804 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/data/_sample.py
--rw-r--r--   0        0        0      272 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/data/partition/__init__.py
--rw-r--r--   0        0        0    14152 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/data/partition/_partition.py
--rw-r--r--   0        0        0      394 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/__init__.py
--rw-r--r--   0        0        0    20829 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_explainer.py
--rw-r--r--   0        0        0     1859 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_inspection.py
--rw-r--r--   0        0        0    42261 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_learner_inspector.py
--rw-r--r--   0        0        0    25729 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_shap.py
--rw-r--r--   0        0        0    24909 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_shap_global_explanation.py
--rw-r--r--   0        0        0    10616 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_shap_projection.py
--rw-r--r--   0        0        0        0 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/py.typed
--rw-r--r--   0        0        0      113 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/__init__.py
--rw-r--r--   0        0        0    13163 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/_parameters.py
--rw-r--r--   0        0        0    17575 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/_selection.py
--rw-r--r--   0        0        0      107 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/base/__init__.py
--rw-r--r--   0        0        0     7599 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/base/_parameters.py
--rw-r--r--   0        0        0      318 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/__init__.py
--rw-r--r--   0        0        0     5452 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/_result.py
--rw-r--r--   0        0        0     9103 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/_simulation.py
--rw-r--r--   0        0        0       58 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/base/__init__.py
--rw-r--r--   0        0        0     9474 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/base/_base.py
--rw-r--r--   0        0        0       95 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/viz/__init__.py
--rw-r--r--   0        0        0     4244 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/viz/_draw.py
--rw-r--r--   0        0        0    12875 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/viz/_style.py
--rw-r--r--   0        0        0      125 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/validation/__init__.py
--rw-r--r--   0        0        0     9263 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/validation/_validation.py
--rw-r--r--   0        0        0        0 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/test/test/__init__.py
--rw-r--r--   0        0        0    15366 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/conftest.py
--rw-r--r--   0        0        0        0 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/__init__.py
--rw-r--r--   0        0        0    24768 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_inspection.py
--rw-r--r--   0        0        0     4351 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_partition.py
--rw-r--r--   0        0        0     5085 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_sample.py
--rw-r--r--   0        0        0    14023 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_selection.py
--rw-r--r--   0        0        0     1797 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_shap_decomposition.py
--rw-r--r--   0        0        0    13500 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_simulation.py
--rw-r--r--   0        0        0     5524 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_validation.py
--rw-r--r--   0        0        0      263 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/paths.py
--rw-r--r--   0        0        0      216 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/test_docs.py
--rw-r--r--   0        0        0     2594 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/tox.ini
--rw-r--r--   0        0        0     4934 1970-01-01 00:00:00.000000 gamma-facet-2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      666 2023-07-11 15:44:27.737008 gamma_facet-2.1rc0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      689 2023-07-11 15:44:27.737008 gamma_facet-2.1rc0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     4886 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/.gitignore
+-rw-r--r--   0        0        0     1103 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/LICENSE
+-rw-r--r--   0        0        0    21630 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/README.rst
+-rw-r--r--   0        0        0     8656 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/RELEASE_NOTES.rst
+-rw-r--r--   0        0        0    26862 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/azure-pipelines.yml
+-rw-r--r--   0        0        0     2555 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/condabuild/meta.yaml
+-rw-r--r--   0        0        0        0 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/config/spelling.dic
+-rw-r--r--   0        0        0      124 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/config/test_config.yml
+-rwxr-xr-x   0        0        0       93 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/dev-setup.sh
+-rw-r--r--   0        0        0      873 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/environment.yml
+-rwxr-xr-x   0        0        0      380 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/make.py
+-rw-r--r--   0        0        0      663 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/mypy.ini
+-rw-r--r--   0        0        0     2717 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/pypi_description.rst
+-rw-r--r--   0        0        0     4083 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-11 15:44:27.741008 gamma_facet-2.1rc0/sphinx/.gitignore
+-rw-r--r--   0        0        0   199625 2023-07-11 15:44:27.749008 gamma_facet-2.1rc0/sphinx/auxiliary/Diabetes_getting_started_example.ipynb
+-rw-r--r--   0        0        0    10223 2023-07-11 15:44:27.749008 gamma_facet-2.1rc0/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb
+-rwxr-xr-x   0        0        0      664 2023-07-11 15:44:27.749008 gamma_facet-2.1rc0/sphinx/make.py
+-rw-r--r--   0        0        0   130308 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/Facet-Simulator-BlockDiagram.png
+-rw-r--r--   0        0        0    19522 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/Facet_Logo_Plain.png
+-rw-r--r--   0        0        0     5238 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/Facet_flow.svg
+-rw-r--r--   0        0        0     7117 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg
+-rw-r--r--   0        0        0    23632 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/facet_banner.png
+-rw-r--r--   0        0        0     1429 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/icons/inspect_icon.png
+-rw-r--r--   0        0        0     2777 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/icons/pipe_icon.png
+-rw-r--r--   0        0        0     2718 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/icons/sim_icon.png
+-rw-r--r--   0        0        0   117900 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/ranker_summary.png
+-rw-r--r--   0        0        0    27724 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/redundancy_dendrogram.png
+-rw-r--r--   0        0        0    31712 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/redundancy_matrix.png
+-rw-r--r--   0        0        0    38185 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/simulation_output.png
+-rw-r--r--   0        0        0    31278 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/synergy_matrix.png
+-rw-r--r--   0        0        0    49407 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Andy_Shora.jpg
+-rw-r--r--   0        0        0     9901 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Florent_Martin.jpg
+-rw-r--r--   0        0        0    11856 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Jan_Ittner.jpg
+-rw-r--r--   0        0        0     8047 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Jason_Bentley.jpg
+-rw-r--r--   0        0        0    10116 2023-07-11 15:44:27.753008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg
+-rw-r--r--   0        0        0     6673 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg
+-rw-r--r--   0        0        0     9583 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Malo_Grisard.jpg
+-rw-r--r--   0        0        0    49773 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg
+-rw-r--r--   0        0        0    10100 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg
+-rw-r--r--   0        0        0    10746 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg
+-rw-r--r--   0        0        0      232 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/_static/css/facet.css
+-rw-r--r--   0        0        0     3673 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/about_us.rst
+-rw-r--r--   0        0        0      371 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/api_landing.rst
+-rw-r--r--   0        0        0      758 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/conf.py
+-rw-r--r--   0        0        0    20763 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/contribution_guide.rst
+-rw-r--r--   0        0        0     5693 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/faqs.rst
+-rw-r--r--   0        0        0      298 2023-07-11 15:44:27.757008 gamma_facet-2.1rc0/sphinx/source/index.rst
+-rw-r--r--   0        0        0  1644442 2023-07-11 15:44:27.773008 gamma_facet-2.1rc0/sphinx/source/tutorial/Classification_with_Facet.ipynb
+-rw-r--r--   0        0        0   970457 2023-07-11 15:44:27.777008 gamma_facet-2.1rc0/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv
+-rw-r--r--   0        0        0   232448 2023-07-11 15:44:27.781008 gamma_facet-2.1rc0/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb
+-rw-r--r--   0        0        0   107691 2023-07-11 15:44:27.781008 gamma_facet-2.1rc0/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb
+-rw-r--r--   0        0        0   475484 2023-07-11 15:44:27.785008 gamma_facet-2.1rc0/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb
+-rw-r--r--   0        0        0   820532 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/sphinx/source/tutorial/pre_diab_nhanes.csv
+-rw-r--r--   0        0        0    85389 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/sphinx/source/tutorial/water_drilling_classification_data.csv
+-rw-r--r--   0        0        0     2402 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/sphinx/source/tutorials.rst
+-rw-r--r--   0        0        0      601 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/__init__.py
+-rw-r--r--   0        0        0      582 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/_types.py
+-rw-r--r--   0        0        0      102 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/data/__init__.py
+-rw-r--r--   0        0        0    11804 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/data/_sample.py
+-rw-r--r--   0        0        0      272 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/data/partition/__init__.py
+-rw-r--r--   0        0        0    14160 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/data/partition/_partition.py
+-rw-r--r--   0        0        0      306 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/explanation/__init__.py
+-rw-r--r--   0        0        0    13800 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/explanation/_explanation.py
+-rw-r--r--   0        0        0      708 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/explanation/_types.py
+-rw-r--r--   0        0        0       89 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/explanation/base/__init__.py
+-rw-r--r--   0        0        0     7935 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/explanation/base/_base.py
+-rw-r--r--   0        0        0      119 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/explanation/parallel/__init__.py
+-rw-r--r--   0        0        0     9169 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/explanation/parallel/_parallel.py
+-rw-r--r--   0        0        0      403 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/inspection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 15:44:27.789008 gamma_facet-2.1rc0/src/facet/inspection/_explainer.py
+-rw-r--r--   0        0        0     4840 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/_function_inspector.py
+-rw-r--r--   0        0        0     1910 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/_inspection.py
+-rw-r--r--   0        0        0    15774 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/_learner_inspector.py
+-rw-r--r--   0        0        0    19115 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/_shap_context.py
+-rw-r--r--   0        0        0    15090 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/_shap_projection.py
+-rw-r--r--   0        0        0       85 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/base/__init__.py
+-rw-r--r--   0        0        0    38123 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/base/_model_inspector.py
+-rw-r--r--   0        0        0       93 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/shap/__init__.py
+-rw-r--r--   0        0        0     1922 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/shap/_function.py
+-rw-r--r--   0        0        0    15295 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/shap/_shap.py
+-rw-r--r--   0        0        0       97 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/shap/sklearn/__init__.py
+-rw-r--r--   0        0        0    11266 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/inspection/shap/sklearn/_sklearn.py
+-rw-r--r--   0        0        0        0 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/py.typed
+-rw-r--r--   0        0        0      113 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/selection/__init__.py
+-rw-r--r--   0        0        0    13220 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/selection/_parameters.py
+-rw-r--r--   0        0        0    17458 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/selection/_selection.py
+-rw-r--r--   0        0        0      107 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/selection/base/__init__.py
+-rw-r--r--   0        0        0     7870 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/selection/base/_parameters.py
+-rw-r--r--   0        0        0      318 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/simulation/__init__.py
+-rw-r--r--   0        0        0     5469 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/simulation/_result.py
+-rw-r--r--   0        0        0     9103 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/simulation/_simulation.py
+-rw-r--r--   0        0        0       58 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/simulation/base/__init__.py
+-rw-r--r--   0        0        0     9564 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/simulation/base/_base.py
+-rw-r--r--   0        0        0       95 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/simulation/viz/__init__.py
+-rw-r--r--   0        0        0     4244 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/simulation/viz/_draw.py
+-rw-r--r--   0        0        0    12875 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/simulation/viz/_style.py
+-rw-r--r--   0        0        0      125 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/validation/__init__.py
+-rw-r--r--   0        0        0     9261 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/src/facet/validation/_validation.py
+-rw-r--r--   0        0        0        0 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/__init__.py
+-rw-r--r--   0        0        0    14736 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/facet/__init__.py
+-rw-r--r--   0        0        0    31524 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/facet/test_inspection.py
+-rw-r--r--   0        0        0     4348 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/facet/test_partition.py
+-rw-r--r--   0        0        0     5085 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/facet/test_sample.py
+-rw-r--r--   0        0        0    14037 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/facet/test_selection.py
+-rw-r--r--   0        0        0     2309 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/facet/test_shap_decomposition.py
+-rw-r--r--   0        0        0    13495 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/facet/test_simulation.py
+-rw-r--r--   0        0        0     5523 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/facet/test_validation.py
+-rw-r--r--   0        0        0      263 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/paths.py
+-rw-r--r--   0        0        0      216 2023-07-11 15:44:27.793008 gamma_facet-2.1rc0/test/test/test_docs.py
+-rw-r--r--   0        0        0     2594 2023-07-11 15:44:27.797008 gamma_facet-2.1rc0/tox.ini
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 gamma_facet-2.1rc0/PKG-INFO
```

### Comparing `gamma-facet-2.0rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `gamma_facet-2.1rc0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/.github/ISSUE_TEMPLATE/feature_request.md` & `gamma_facet-2.1rc0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/.gitignore` & `gamma_facet-2.1rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/.pre-commit-config.yaml` & `gamma_facet-2.1rc0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 repos:
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
     rev: 22.8.0
     hooks:
       - id: black
-        language: python_venv
+        language: python
         language_version: python39
 
-  - repo: https://gitlab.com/pycqa/flake8
+  - repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         name: flake8
         entry: flake8 --config tox.ini
-        language: python_venv
+        language: python
         language_version: python39
         additional_dependencies:
           - flake8-comprehensions ~= 3.10
         types: [ python ]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
       - id: check-added-large-files
       - id: check-json
       - id: check-xml
       - id: check-yaml
-        language: python_venv
+        language: python
         exclude: condabuild/meta.yaml
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.981
+    rev: v1.2.0
     hooks:
       - id: mypy
         files: src|sphinx|test
-        language: python_venv
+        language: python
         language_version: python39
         additional_dependencies:
           - numpy~=1.22
-          - gamma-pytools~=2.1rc
-          - sklearndf~=2.2.dev
+          - gamma-pytools~=2.1
+          - sklearndf~=2.2
```

### Comparing `gamma-facet-2.0rc2/LICENSE` & `gamma_facet-2.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/README.rst` & `gamma_facet-2.1rc0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 .. image:: sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg
 
-|
+.. note:: **FACET 2.0 now available!**
+
+    FACET 2.0 brings numerous API enhancements and improvements, accelerates model
+    inspection by up to a factor of 50 in many practical applications, introduces a new,
+    more flexible and user-friendly API for hyperparameter tuning – with support for
+    `scikit-learn`'s native hyperparameter searchers – and improves the styling of all
+    visualizations.
+
+    See the `release notes <https://bcg-gamma.github.io/facet/docs-version/2-0/_generated/release_notes.html>`__
+    for more details.
 
-**Release Candidate 2.0rc available now!**
 
-|
 
 FACET is an open source library for human-explainable AI.
 It combines sophisticated model inspection and model-based simulation to enable better 
 explanations of your supervised machine learning models.
 
 FACET is composed of the following key components:
 
@@ -56,29 +63,45 @@
 .. End-Badges
 
 
 Installation
 ------------
 
 FACET supports both PyPI and Anaconda.
-
+We recommend to install FACET into a dedicated environment.
 
 Anaconda
 ~~~~~~~~
 
-.. code-block:: RST
+.. code-block:: sh
 
-    conda install gamma-facet -c bcg_gamma -c conda-forge
+    conda create -n facet
+    conda activate facet
+    conda install -c bcg_gamma -c conda-forge gamma-facet
 
 
 Pip
 ~~~
 
-.. code-block:: RST
+macOS and Linux:
+^^^^^^^^^^^^^^^^
+
+.. code-block:: sh
+
+    python -m venv facet
+    source facet/bin/activate
+    pip install gamma-facet
+
+Windows:
+^^^^^^^^
+
+.. code-block:: dosbatch
 
+    python -m venv facet
+    facet\Scripts\activate.bat
     pip install gamma-facet
 
 
 Quickstart
 ----------
 
 The following quickstart guide provides a minimal example workflow to get you
@@ -159,15 +182,15 @@
     # rank your candidate models by performance
     selector = LearnerSelector(
         searcher_type=GridSearchCV,
         parameter_space=rnd_forest_ps,
         cv=rkf_cv,
         n_jobs=-3,
         scoring="r2"
-    ).fit(sample=diabetes_sample)
+    ).fit(diabetes_sample)
 
     # get summary report
     selector.summary_report()
 
 .. image:: sphinx/source/_images/ranker_summary.png
    :width: 600
 
@@ -234,15 +257,15 @@
 .. code-block:: Python
 
     # fit the model inspector
     from facet.inspection import LearnerInspector
     inspector = LearnerInspector(
         pipeline=selector.best_estimator_,
         n_jobs=-3
-    ).fit(sample=diabetes_sample)
+    ).fit(diabetes_sample)
 
 **Synergy**
 
 .. code-block:: Python
 
     # visualise synergy as a matrix
     from pytools.viz.matrix import MatrixDrawer
```

### Comparing `gamma-facet-2.0rc2/RELEASE_NOTES.rst` & `gamma_facet-2.1rc0/RELEASE_NOTES.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,82 @@
-Release Notes
+\Release Notes
 =============
 
 .. |mypy| replace:: :external+mypy:doc:`mypy <index>`
 .. |shap| replace:: :external+shap:doc:`shap <index>`
 .. |nbsp| unicode:: 0xA0
    :trim:
 
+FACET 2.1
+---------
+
+FACET 2.1 introduces the :class:`.NativeLearnerInspector` for inspecting native
+*scikit-learn* models and pipelines.
+
+We still recommend using :mod:`sklearndf` models and learner pipelines along with FACET's
+:class:`.LearnerSelector` for hyperparameter tuning; however the new
+:class:`.NativeLearnerInspector` can be useful for inspecting models that have been
+trained using *scikit-learn* directly.
+
+2.1.0
+~~~~~
+
+- API: new :class:`.NativeLearnerInspector` class for inspecting native *scikit-learn*
+  regressors, classifiers, and pipelines with a regressor or classifier as the final
+  estimator
+
+
 FACET 2.0
 ---------
 
 FACET |nbsp| 2.0 brings numerous API enhancements and improvements, accelerates model
-inspection by factor |nbsp| 50 in many practical settings, makes major improvements to
-visualizations, and is now fully type-checked by |mypy|.
+inspection by up to a factor of 50 in many practical applications, introduces a new,
+more flexible and user-friendly API for hyperparameter tuning – with support for
+`scikit-learn`'s native hyperparameter searchers – and improves the styling of all
+visualizations.
+
+FACET 2.0 requires :mod:`pytools` |nbsp| 2.0 and :mod:`sklearndf` |nbsp| 2.2, and is now
+fully type-checked by |mypy|.
+
+2.0.1
+~~~~~
+
+- API: class :class:`.LearnerInspector` now supports inspecting individual regressors
+  and classifiers; it is no longer necessary to wrap them into a
+  :class:`.RegressorPipelineDF` or :class:`.ClassifierPipelineDF` instance with empty
+  preprocessing
 
 
 2.0.0
 ~~~~~
 
 ``facet.data``
 ^^^^^^^^^^^^^^
 
 - API: class :class:`.Sample` raises an exception if the name of any used column is not
   a string
 - API: class :class:`.RangePartitioner` supports new optional arguments ``lower_bound``
   and ``upper_bound`` in method :meth:`~.RangePartitioner.fit` and no longer accepts
   them in the class initializer
 
+``facet.explanation``
+^^^^^^^^^^^^^^^^^^^^^
+
+- REFACTOR: moved explainer factories from module :mod:`facet.inspection` to new module
+  :mod:`facet.explanation`.
+- API: new explainer factories :class:`.ExactExplainerFactory` and
+  :class:`.PermutationExplainerFactory`, in addition to the
+  :class:`.TreeExplainerFactory` and :class:`.KernelExplainerFactory` introduced in
+  FACET |nbsp| 1.0
+
 ``facet.inspection``
 ^^^^^^^^^^^^^^^^^^^^
 
+- API: new :class:`.FunctionInspector` class for inspecting arbitrary functions,
+  using a :class:`.ExactExplainerFactory` by default
 - API: :class:`.LearnerInspector` no longer uses learner crossfits and instead inspects
   models using a single pass of SHAP calculations, usually leading to performance gains
   of up to a factor of |nbsp| 50
 - API: return :class:`.LearnerInspector` matrix outputs as :class:`~pytools.data.Matrix`
   instances
 - API: diagonals of feature synergy, redundancy, and association matrices are now
   ``nan`` instead of |nbsp| 1.0
@@ -44,21 +88,24 @@
   The old sorting behaviour of FACET |nbsp| 1.x can be restored using method
   :meth:`~pytools.data.LinkageTree.sort_by_weight`
 
 ``facet.selection``
 ^^^^^^^^^^^^^^^^^^^
 
 - API: :class:`.LearnerSelector` replaces FACET |nbsp| 1.x class ``LearnerRanker``, and
-  now supports any CV searcher that supports `scikit-learn`'s CV search API, including
-  `scikit-learn`'s native searchers such as
+  provides a new, more flexible and user-friendly API for hyperparameter tuning
+- API: :class:`.LearnerSelector` introduces support for any CV searcher implementing
+  `scikit-learn`'s CV search API, including `scikit-learn`'s native searchers such as
   :class:`~sklearn.model_selection.GridSearchCV` or
   :class:`~sklearn.model_selection.RandomizedSearchCV`
 - API: new classes :class:`.ParameterSpace` and :class:`.MultiEstimatorParameterSpace`
   offer a more convenient and robust mechanism for declaring options or distributions
   for hyperparameter tuning
+- API: new class :class:`.LearnerSelector` supports a new, more flexible and
+  user-friendly API for hyperparameter tuning
 
 ``facet.simulation``
 ^^^^^^^^^^^^^^^^^^^^
 
 - API: simulations no longer depend on learner crossfits and instead are carried out
   as a single pass on the full dataset, using the *standard error of mean predictions*
   to obtain confidence intervals that less conservative yet more realistic
@@ -69,29 +116,38 @@
 ^^^^^^^^^^^^^^^^^^^^
 
 - API: removed class ``FullSampleValidator``
 
 Other
 ^^^^^
 
+- VIZ: significant updates to the styling of all visualizations, especially those
+  generated for output of :class:`.LearnerInspector`, using the all-new versions of
+  :mod:`pytools` matrix and dendrogram drawers
 - API: class ``LearnerCrossfit`` is no longer needed in FACET |nbsp| 2.0 and has been
   removed
-- API: support new :obj:`~pytools.fit.fitted_only` decorator introduced in *pytools*
-  |nbsp| 2.1.
+- API: support new :obj:`~pytools.fit.fitted_only` decorator introduced in
+  :mod:`pytools` |nbsp| 2.1.
 
 
 FACET 1.2
 ---------
 
 FACET |nbsp| 1.2 adds support for *sklearndf* |nbsp| 1.2 and *scikit-learn* |nbsp| 0.24.
 It also introduces the ability to run simulations on a subsample of the data used to
 fit the underlying crossfit.
 One example where this can be useful is to use only a recent period of a time series as
 the baseline of a simulation.
 
+1.2.3
+~~~~~
+
+- BUILD: pin down *matplotlib* version to < 3.6 and *scipy* version to < 1.9 to ensure
+  compatibility with *pytools* 1.2 and *sklearndf* 1.2
+
 
 1.2.2
 ~~~~~
 
 - catch up with FACET |nbsp| 1.1.2
 
 
@@ -160,17 +216,17 @@
 
 FACET 1.0
 ---------
 
 1.0.3
 ~~~~~
 
-- FIX: restrict package requirements to *gamma-pytools* |nbsp| 1.0.* and
-  *sklearndf* |nbsp| 1.0.x, since FACET |nbsp| 1.0 is not compatible with
-  *gamma-pytools* |nbsp| 1.1.*
+- FIX: restrict package requirements to *gamma-pytools* |nbsp| 1.0 and
+  *sklearndf* |nbsp| 1.0, since FACET |nbsp| 1.0 is not compatible with
+  *gamma-pytools* |nbsp| 1.1
 
 1.0.2
 ~~~~~
 
 This is a maintenance release focusing on enhancements to the CI/CD pipeline and bug
 fixes.
```

### Comparing `gamma-facet-2.0rc2/azure-pipelines.yml` & `gamma_facet-2.1rc0/azure-pipelines.yml`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 resources:
   repositories:
     - repository: pytools
       type: github
       endpoint: BCG-Gamma
       name: BCG-Gamma/pytools
-      ref: 2.0.x
+      ref: 2.1.x
 
 variables:
   ${{ if not(startsWith(variables['Build.SourceBranch'], 'refs/pull/')) }}:
     branchName: $[ replace(variables['Build.SourceBranch'], 'refs/heads/', '') ]
   ${{ if startsWith(variables['Build.SourceBranch'], 'refs/pull/') }}:
     branchName: $[ replace(variables['System.PullRequest.SourceBranch'], 'refs/heads/', '') ]
   source_is_release_branch: $[ startsWith(variables['branchName'], 'release/') ]
@@ -50,15 +50,15 @@
         displayName: 'isort'
         steps:
           - task: UsePythonVersion@0
             inputs:
               versionSpec: '3.9'
             displayName: 'use Python 3.9'
           - script: |
-              python -m pip install isort~=5.10
+              python -m pip install isort~=5.12
               python -m isort --check --diff .
             displayName: 'Run isort'
       - job:
         displayName: 'black'
         steps:
           - task: UsePythonVersion@0
             inputs:
@@ -83,39 +83,42 @@
         displayName: 'mypy'
         steps:
           - task: UsePythonVersion@0
             inputs:
               versionSpec: '3.9'
             displayName: 'use Python 3.9'
           - script: |
-              python -m pip install mypy~=0.981 numpy~=1.22 'gamma-pytools~=2.1rc' sklearndf~=2.2.dev
+              python -m pip install mypy~=1.2.0 numpy~=1.23 gamma-pytools~=2.1 sklearndf~=2.2
               python -m mypy src
             displayName: 'Run mypy'
 
   # detect whether the build config (pyproject.toml) was changed -> then we must run a build test
   - stage: detect_build_config_changes
     displayName: 'Pyproject.toml build config'
 
     jobs:
 
       - job: checkout_and_diff
         displayName: 'detect changes'
         steps:
           - checkout: self
+            fetchDepth: 2
 
           - task: Bash@3
             name: diff
             inputs:
               targetType: 'inline'
               script: |
+                set -eux
+
                 echo Repo: $(Build.DefinitionName)
                 cd $(System.DefaultWorkingDirectory)
-                files_changed=$(git diff $(Build.SourceVersion)^! --name-only)
+                files_changed=$(git diff $(Build.SourceVersion)^ --name-only)
                 echo "Files changed since last commit: ${files_changed}"
-                n_files_changed=$(git diff $(Build.SourceVersion)^! --name-only | grep -i -E 'meta\.yaml|pyproject\.toml|azure-pipelines\.yml|tox\.ini|make\.py'  | wc -l | xargs)
+                n_files_changed=$(git diff $(Build.SourceVersion)^ --name-only | grep -i -E 'meta\.yaml|pyproject\.toml|azure-pipelines\.yml|tox\.ini|make\.py'  | wc -l | xargs)
                 if [ ${n_files_changed} -gt 0 ]
                 then
                 build_changed=1
                 echo "build config has been changed"
                 else
                 build_changed=0
                 echo "build config is unchanged";
@@ -128,40 +131,45 @@
     displayName: 'Unit tests'
     dependsOn: 'detect_build_config_changes'
     variables:
       conda_build_config_changed: $[ stageDependencies.detect_build_config_changes.checkout_and_diff.outputs['diff.conda_build_config_changed'] ]
 
     jobs:
       - job:
-        timeoutInMinutes: 120
-        cancelTimeoutInMinutes: 3
         displayName: 'pytest @ develop environment'
         condition: ne(variables.source_is_release_branch, 'True')
 
         pool:
           vmImage: 'ubuntu-latest'
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - checkout: self
 
           - script: dir $(Build.SourcesDirectory)
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                eval "$(conda shell.bash hook)"
-                conda env create
-                conda activate $(project_name)-develop
+
+                # install micromamba
+                curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba
+                export MAMBA_ROOT_PREFIX=~/micromamba
+                eval "$(./bin/micromamba shell hook -s posix)"
+
+                # install the develop environment
+                micromamba env create --yes --file environment.yml
+                micromamba activate $(project_name)-develop
+
                 export PYTHONPATH=$(System.DefaultWorkingDirectory)/src/
                 export RUN_PACKAGE_VERSION_TEST=$(project_name)
 
                 pytest \
                    --cov $(project_name) \
                    --cov-config "tox.ini" \
                    --cov-report=xml:coverage.xml --cov-report=html:htmlcov \
@@ -231,15 +239,23 @@
 
           - checkout: pytools
           - checkout: self
 
           - script: dir $(Build.SourcesDirectory)
 
           - script: |
-              conda install -y -c anaconda conda-build~=3.21 conda-verify~=3.4 toml~=0.10 flit~=3.6 packaging~=20.9
+              # install micromamba
+              curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba
+              export MAMBA_ROOT_PREFIX=~/micromamba
+              eval "$(./bin/micromamba shell hook -s posix)"
+              
+              # create and activate a build environment, then install the tools we need
+              micromamba create -n build
+              micromamba activate build
+              micromamba install -y -c conda-forge boa~=0.14 toml~=0.10 flit~=3.6 packaging~=20.9
             displayName: 'Install conda-build, flit, toml'
             condition: eq(variables['BUILD_SYSTEM'], 'conda')
 
           - script: |
               python -m pip install "toml~=0.10"
               python -m pip install "flit~=3.7"
               flit --version
@@ -249,15 +265,19 @@
             condition: eq(variables['BUILD_SYSTEM'], 'tox')
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                if [ "$BUILD_SYSTEM" = "conda" ] ; then eval "$(conda shell.bash hook)" ; fi
+                if [ "$BUILD_SYSTEM" = "conda" ] ; then
+                  export MAMBA_ROOT_PREFIX=~/micromamba
+                  eval "$(./bin/micromamba shell hook -s posix)"
+                  micromamba activate build
+                fi
                 export RUN_PACKAGE_VERSION_TEST=$(project_name)
 
                 cd $(Build.SourcesDirectory)/$(project_root)
                 ./make.py $(project_name) $(BUILD_SYSTEM) $(PKG_DEPENDENCIES)
             displayName: "build & test"
 
           - task: CopyFiles@2
@@ -318,15 +338,23 @@
 
           - checkout: pytools
           - checkout: self
 
           - script: dir $(Build.SourcesDirectory)
 
           - script: |
-              conda install -y -c anaconda conda-build~=3.21 conda-verify~=3.4 toml~=0.10 flit~=3.6 packaging~=20.9
+              # install micromamba
+              curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba
+              export MAMBA_ROOT_PREFIX=~/micromamba
+              eval "$(./bin/micromamba shell hook -s posix)"
+              
+              # create and activate a build environment, then install the tools we need
+              micromamba create -n build
+              micromamba activate build
+              micromamba install -y -c conda-forge boa~=0.14 toml~=0.10 flit~=3.6 packaging~=20.9
             displayName: 'Install conda-build, flit, toml'
             condition: eq(variables['BUILD_SYSTEM'], 'conda')
 
           - script: |
               python -m pip install "toml==0.10.*"
               python -m pip install "flit==3.0.*"
               flit --version
@@ -336,15 +364,19 @@
             condition: eq(variables['BUILD_SYSTEM'], 'tox')
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                if [ "$BUILD_SYSTEM" = "conda" ] ; then eval "$(conda shell.bash hook)" ; fi
+                if [ "$BUILD_SYSTEM" = "conda" ] ; then
+                  export MAMBA_ROOT_PREFIX=~/micromamba
+                  eval "$(./bin/micromamba shell hook -s posix)"
+                  micromamba activate build
+                fi
                 export RUN_PACKAGE_VERSION_TEST=$(project_name)
 
                 cd $(Build.SourcesDirectory)/$(project_root)
                 ./make.py $(project_name) $(BUILD_SYSTEM) $(PKG_DEPENDENCIES)
             displayName: "build & test"
 
           - task: CopyFiles@2
@@ -405,16 +437,16 @@
           eq(variables.source_is_release_branch, 'True'),
           eq(variables.source_is_develop_branch, 'True')
           )
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - checkout: pytools
           - checkout: self
 
           - task: Bash@3
             env:
               BRANCH_NAME: $(branchName)
@@ -470,16 +502,16 @@
           eq(variables.source_is_release_branch, 'True'),
           eq(variables.source_is_develop_branch, 'True')
           )
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - checkout: pytools
           - checkout: self
 
           - task: Bash@3
             inputs:
               targetType: inline
@@ -597,16 +629,16 @@
 
         pool:
           vmImage: 'ubuntu-latest'
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - task: InstallSSHKey@0
             inputs:
               knownHostsEntry: $(knownHostsEntry)
               sshPublicKey: $(sshPublicKey)
               sshKeySecureFile: 'deploy_docs_$(project_name)'
             displayName: 'Install the deploy SSH key'
@@ -637,69 +669,64 @@
             displayName: 'Retrieve current documentation versions from github-pages'
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                eval "$(conda shell.bash hook)"
 
                 cd $(System.DefaultWorkingDirectory)
                 echo "Checking out $(branchName)"
                 git checkout $(branchName)
 
-                conda env create
-                conda activate $(project_name)-develop
+                # install micromamba
+                curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba
+                export MAMBA_ROOT_PREFIX=~/micromamba
+                eval "$(./bin/micromamba shell hook -s posix)"
+                # install the develop environment
+                micromamba env create --yes --file environment.yml
+                micromamba activate $(project_name)-develop
 
                 export PYTHONPATH=$(System.DefaultWorkingDirectory)/src/
 
                 python sphinx/make.py html
 
             displayName: 'Build latest documentation'
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                eval "$(conda shell.bash hook)"
+                export MAMBA_ROOT_PREFIX=~/micromamba
+                eval "$(./bin/micromamba shell hook -s posix)"
 
                 # install the tree utility
                 sudo apt-get install tree
 
                 cd $(System.DefaultWorkingDirectory)
 
                 echo "Restoring previous documentation to the docs directory"
                 mkdir -p docs
                 mv $(Build.ArtifactStagingDirectory)/docs-version.bak docs/docs-version
                 ls docs/docs-version
 
                 mkdir -p $(System.DefaultWorkingDirectory)/sphinx/build/
 
-                conda activate $(project_name)-develop
+                micromamba activate $(project_name)-develop
                 python sphinx/make.py prepare_docs_deployment
 
                 echo "Current docs contents:"
                 tree docs
                 mv docs $(Build.ArtifactStagingDirectory)/docs
             displayName: 'Merge previous and latest docs'
 
-          - task: ArchiveFiles@2
-            inputs:
-              rootFolderOrFile: $(Build.ArtifactStagingDirectory)/docs
-              includeRootFolder: false
-              archiveType: 'zip' # Options: zip, 7z, tar, wim
-              archiveFile: $(Build.ArtifactStagingDirectory)/docs.zip
-              replaceExistingArchive: true
-              verbose: false
-              quiet: false
-
           - task: PublishBuildArtifacts@1
             inputs:
-              pathtoPublish: $(Build.ArtifactStagingDirectory)/docs.zip
+              pathtoPublish: $(Build.ArtifactStagingDirectory)/docs
               artifactName: $(project_name)_docs
               publishLocation: Container
 
             displayName: 'Publish docs artifact'
 
           - task: Bash@3
             condition: eq(variables['source_is_release_branch'], 'True')
```

### Comparing `gamma-facet-2.0rc2/condabuild/meta.yaml` & `gamma_facet-2.1rc0/condabuild/meta.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -32,24 +32,27 @@
     - facet.data
     - facet.inspection
     - facet.selection
     - facet.validation
     - facet.simulation
   requires:
     - pytest ~= 7.1
-    # additional requirements of sklearndf
-    - boruta_py      {{ environ.get('FACET_V_BORUTA') }}
-    - lightgbm       {{ environ.get('FACET_V_LIGHTGBM') }}
-    - scikit-learn   {{ environ.get('FACET_V_SCIKIT_LEARN') }}
+    # we always need lightgbm for testing; version spec is optional
+    - lightgbm       {{ environ.get('FACET_V_LIGHTGBM', '') }}
+    # optional libraries of sklearndf, needed for testing
+    - boruta_py      {{ environ.get('FACET_V_BORUTA', '[False]') }}
+    - scikit-learn   {{ environ.get('FACET_V_SCIKIT_LEARN', '[False]') }}
     # additional requirements of gamma-pytools
-    - joblib         {{ environ.get('FACET_V_JOBLIB') }}
-    - typing_inspect {{ environ.get('FACET_V_TYPING_INSPECT') }}
+    - joblib         {{ environ.get('FACET_V_JOBLIB', '[False]') }}
+    - typing_inspect {{ environ.get('FACET_V_TYPING_INSPECT', '[False]') }}
     # additional requirements of shap
-    - ipython        {{ environ.get('FACET_V_IPYTHON') }}
-    - numba          {{ environ.get('FACET_V_NUMBA') }}
+    - ipython        {{ environ.get('FACET_V_IPYTHON', '[False]') }}
+    - numba          {{ environ.get('FACET_V_NUMBA', '[False]') }}
+    # additional requirements for testing
+    - zipp           {{ environ.get('FACET_V_ZIPP', '[False]') }}
   commands:
     - conda list
     - python -c 'import facet;
                  import os;
                  assert facet.__version__ == os.environ["PKG_VERSION"]'
     - cd "${FACET_PATH}/facet"
     - pytest -vs test
```

### Comparing `gamma-facet-2.0rc2/mypy.ini` & `gamma_facet-2.1rc0/mypy.ini`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 ; TODO remove once PEP 561 is supported
 ignore_missing_imports = True
 
 [mypy-pandas.*]
 ; TODO remove once PEP 561 is supported
 ignore_missing_imports = True
 
-[mypy-pytools.*]
-; TODO remove once PEP 561 is supported
-ignore_missing_imports = True
-
 [mypy-scipy.*]
 ; TODO remove once PEP 561 is supported
 ignore_missing_imports = True
 
 [mypy-sklearn.*]
 ; TODO remove once PEP 561 is supported
 ignore_missing_imports = True
```

### Comparing `gamma-facet-2.0rc2/pypi_description.rst` & `gamma_facet-2.1rc0/pypi_description.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/pyproject.toml` & `gamma_facet-2.1rc0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 author = "Boston Consulting Group (BCG)"
 home-page = "https://github.com/BCG-Gamma/facet"
 description-file = "pypi_description.rst"
 dist-name = "gamma-facet"
 license = "Apache Software License v2.0"
 
 requires = [
-    "gamma-pytools  >=2.1rc,<3a",
-    "matplotlib     ~=3.0",
-    "numpy          >=1.21,<2a",  # cannot use ~= due to conda bug
-    "packaging      >=20",
-    "pandas         ~=1.0",
-    "scipy          ~=1.2",
-    "shap           >=0.34,<0.42a",
-    "sklearndf      >=2.2rc,<3a",
+    "gamma-pytools     ~=2.1",
+    "matplotlib        ~=3.0",
+    "numpy             >=1.21,<2a",  # cannot use ~= due to conda bug
+    "packaging         >=20",
+    "pandas            >=1.0",
+    "scipy             ~=1.2",
+    "shap              >=0.39",
+    "scikit-learn      ~=1.0",
+    "sklearndf         ~=2.2",
+    "typing_extensions ~=4.0",
 ]
 
 requires-python = ">=3.7,<4a"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
@@ -42,17 +44,14 @@
     "Topic :: Scientific/Engineering",
 ]
 
 [tool.flit.metadata.requires-extra]
 testing = [
     "pytest ~= 7.1",
     "pytest-cov ~= 2.12",
-    "flake8 ~= 3.8",
-    "flake8-comprehensions ~= 3.2",
-    "isort ~= 5.10",
     "lightgbm ~=3.0.0",
     "xgboost ~= 1.5",
 ]
 docs = [
     "sphinx ~= 4.5",
     "sphinx-autodoc-typehints ~= 1.19",
     "pydata-sphinx-theme ~= 0.8.1",
@@ -70,62 +69,66 @@
 
 [build]
 # comma-separated list of packages to be built from source in pip min builds
 no-binary.min = ["matplotlib", "shap"]
 
 [build.matrix.min]
 # direct requirements of gamma-facet
-gamma-pytools  = "~=2.1rc"
-matplotlib     = "~=3.0.3"
-numpy          = "==1.21.6"  # cannot use ~= due to conda bug
-packaging      = "~=20.9"
-pandas         = "~=1.0.5"
-python         = ">=3.7.12,<3.8a"    # cannot use ~= due to conda bug
-scipy          = "~=1.4.1"
-shap           = "~=0.34.0"
-sklearndf      = "~=2.2rc"
+gamma-pytools     = "~=2.1.0"
+matplotlib        = "~=3.0.3"
+numpy             = "==1.21.6"  # cannot use ~= due to conda bug
+packaging         = "~=20.9"
+pandas            = "~=1.0.5"
+python            = ">=3.7.12,<3.8a"    # cannot use ~= due to conda bug
+scipy             = "~=1.4.1"
+shap              = "~=0.39.0"
+sklearndf         = "~=2.2.0"
+typing_extensions = "~=4.0.0"
 # additional minimum requirements of sklearndf
-boruta         = "~=0.3.0"
-lightgbm       = "~=3.0.0"
-scikit-learn   = "~=0.24.2"
-xgboost        = "~=1.5"
+boruta            = "~=0.3.0"
+lightgbm          = "~=3.0.0"
+scikit-learn      = "~=1.0.2"
+xgboost           = "~=1.5.0"
 # additional minimum requirements of gamma-pytools
-joblib         = "~=0.14.1"
-typing_inspect = "~=0.4.0"
+joblib            = "~=0.14.1"
+typing_inspect    = "~=0.4.0"
 # additional minimum requirements of shap
-ipython        = "==7.0"
-numba          = "~=0.55"  # required to support numpy 1.21
+ipython           = "==7.0"
+numba             = "~=0.55.2"  # required to support numpy 1.21
+# additional requirements for testing
+zipp              = "<3.16"     # required to support python 3.7
 
 [build.matrix.max]
 # direct requirements of gamma-facet
-gamma-pytools  = ">=2.1rc,<3a"
-matplotlib     = "~=3.5"
-numpy          = ">=1.22,<2a"  # cannot use ~= due to conda bug
-packaging      = ">=20"
-pandas         = "~=1.4"
-python         = ">=3.9,<4a"   # cannot use ~= due to conda bug
-scipy          = "~=1.8"
-shap           = "~=0.41"
-sklearndf      = ">=2.2rc,<3a"
+gamma-pytools     = "~=2.1"
+matplotlib        = "~=3.6"
+numpy             = ">=1.23,<2a"  # cannot use ~= due to conda bug
+packaging         = ">=20"
+pandas            = "~=2.0"
+python            = ">=3.9,<4a"   # cannot use ~= due to conda bug
+scipy             = "~=1.10"
+shap              = "~=0.41"
+sklearndf         = "~=2.2"
+typing_extensions = "~=4.3"
 # additional maximum requirements of sklearndf
-boruta         = "~=0.3"
-lightgbm       = "~=3.3"
-scikit-learn   = "~=1.1"
-xgboost        = "~=1.5"
+boruta            = "~=0.3"
+lightgbm          = "~=3.3"
+scikit-learn      = "~=1.2"
+xgboost           = "~=1.5"
 # additional maximum requirements of gamma-pytools
-joblib         = "~=1.1"
-typing_inspect = "~=0.7"
+joblib            = "~=1.1"
+typing_inspect    = "~=0.7"
 # additional maximum requirements of shap
-ipython        = ">=7"
-numba          = ">=0.55.2"  # required to support numpy 1.22
+ipython           = ">=7"
+numba             = "~=0.56"
 
 [tool.black]
 # quiet = "True"
 line-length = 88
-target_version = ['py36']
+target_version = ['py37']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
```

### Comparing `gamma-facet-2.0rc2/sphinx/auxiliary/Diabetes_getting_started_example.ipynb` & `gamma_facet-2.1rc0/sphinx/auxiliary/Diabetes_getting_started_example.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997172619047618%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(7, ').fit(diabetes_sample)\\n')], delete: [7]}}, 7: "*

 * *            "{'source': {insert: [(5, ').fit(diabetes_sample)')], delete: [5]}}}"}*

```diff
@@ -276,15 +276,15 @@
                 "# rank your candidate models by performance\n",
                 "selector = LearnerSelector(\n",
                 "    searcher_type=GridSearchCV,\n",
                 "    parameter_space=rnd_forest_ps, \n",
                 "    cv=rkf_cv, \n",
                 "    n_jobs=-3,\n",
                 "    scoring=\"r2\"\n",
-                ").fit(sample=diabetes_sample)\n",
+                ").fit(diabetes_sample)\n",
                 "\n",
                 "# get summary report\n",
                 "selector.summary_report()"
             ]
         },
         {
             "cell_type": "markdown",
@@ -360,15 +360,15 @@
             "outputs": [],
             "source": [
                 "# fit the model inspector\n",
                 "from facet.inspection import LearnerInspector\n",
                 "inspector = LearnerInspector(\n",
                 "    pipeline=selector.best_estimator_,\n",
                 "    n_jobs=-3\n",
-                ").fit(sample=diabetes_sample)"
+                ").fit(diabetes_sample)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "**Synergy**"
```

### Comparing `gamma-facet-2.0rc2/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb` & `gamma_facet-2.1rc0/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/make.py` & `gamma_facet-2.1rc0/sphinx/make.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/Facet-Simulator-BlockDiagram.png` & `gamma_facet-2.1rc0/sphinx/source/_images/Facet-Simulator-BlockDiagram.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/Facet_Logo_Plain.png` & `gamma_facet-2.1rc0/sphinx/source/_images/Facet_Logo_Plain.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/Facet_flow.svg` & `gamma_facet-2.1rc0/sphinx/source/_images/Facet_flow.svg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg` & `gamma_facet-2.1rc0/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/facet_banner.png` & `gamma_facet-2.1rc0/sphinx/source/_images/facet_banner.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/icons/inspect_icon.png` & `gamma_facet-2.1rc0/sphinx/source/_images/icons/inspect_icon.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/icons/pipe_icon.png` & `gamma_facet-2.1rc0/sphinx/source/_images/icons/pipe_icon.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/icons/sim_icon.png` & `gamma_facet-2.1rc0/sphinx/source/_images/icons/sim_icon.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/ranker_summary.png` & `gamma_facet-2.1rc0/sphinx/source/_images/ranker_summary.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/redundancy_dendrogram.png` & `gamma_facet-2.1rc0/sphinx/source/_images/redundancy_dendrogram.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/redundancy_matrix.png` & `gamma_facet-2.1rc0/sphinx/source/_images/redundancy_matrix.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/simulation_output.png` & `gamma_facet-2.1rc0/sphinx/source/_images/simulation_output.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/synergy_matrix.png` & `gamma_facet-2.1rc0/sphinx/source/_images/synergy_matrix.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Andy_Shora.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Andy_Shora.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Florent_Martin.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Florent_Martin.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Jan_Ittner.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Jan_Ittner.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Jason_Bentley.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Jason_Bentley.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Malo_Grisard.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Malo_Grisard.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/about_us.rst` & `gamma_facet-2.1rc0/sphinx/source/about_us.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/conf.py` & `gamma_facet-2.1rc0/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/contribution_guide.rst` & `gamma_facet-2.1rc0/sphinx/source/contribution_guide.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/faqs.rst` & `gamma_facet-2.1rc0/sphinx/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/tutorial/Classification_with_Facet.ipynb` & `gamma_facet-2.1rc0/sphinx/source/tutorial/Classification_with_Facet.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999128919860627%*

 * *Differences: {"'cells'": "{36: {'source': {insert: [(5, ').fit(prediab_initial_features)')], delete: [5]}}, 55: "*

 * *            "{'source': {insert: [(5, ').fit(prediab_no_redundant_feat)')], delete: [5]}}}"}*

```diff
@@ -1329,15 +1329,15 @@
             "outputs": [],
             "source": [
                 "# run inspector\n",
                 "clf_inspector = LearnerInspector(\n",
                 "    pipeline=clf_selector.best_estimator_,\n",
                 "    n_jobs=-3,\n",
                 "    verbose=False,\n",
-                ").fit(sample=prediab_initial_features)"
+                ").fit(prediab_initial_features)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
@@ -1905,15 +1905,15 @@
             "outputs": [],
             "source": [
                 "# run inspector\n",
                 "inspector_no_redun = LearnerInspector(\n",
                 "    pipeline=clf_selector.best_estimator_,\n",
                 "    n_jobs=-3,\n",
                 "    verbose=False,\n",
-                ").fit(sample=prediab_no_redundant_feat)"
+                ").fit(prediab_no_redundant_feat)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 26,
             "metadata": {},
             "outputs": [
```

### Comparing `gamma-facet-2.0rc2/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv` & `gamma_facet-2.1rc0/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb` & `gamma_facet-2.1rc0/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb` & `gamma_facet-2.1rc0/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb` & `gamma_facet-2.1rc0/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/tutorial/pre_diab_nhanes.csv` & `gamma_facet-2.1rc0/sphinx/source/tutorial/pre_diab_nhanes.csv`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/tutorial/water_drilling_classification_data.csv` & `gamma_facet-2.1rc0/sphinx/source/tutorial/water_drilling_classification_data.csv`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/sphinx/source/tutorials.rst` & `gamma_facet-2.1rc0/sphinx/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/src/facet/__init__.py` & `gamma_facet-2.1rc0/src/facet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Human-explainable AI.
 
 This is the class and function reference of FACET for advanced model selection,
 inspection, and simulation.
 """
 
 
-__version__ = "2.0rc2"
+__version__ = "2.1rc0"
 
 __logo__ = (
     r"""
     _         ____    _                         _       ___        __   ___ _____
  _-´ _-      / ___\  / \    /\  /\   /\  /\    / \     |     /\   /  ` |      |
 | ,-´ , |   | | __  / _ \  /  \/  \ /  \/  \  / _ \    |___ /  \ |     |__    |
 | | | | |   | |_] |/ ___ \/ /\  /\ \ /\  /\ \/ ___ \   |   /----\|     |      |
```

### Comparing `gamma-facet-2.0rc2/src/facet/data/_sample.py` & `gamma_facet-2.1rc0/src/facet/data/_sample.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/src/facet/data/partition/_partition.py` & `gamma_facet-2.1rc0/src/facet/data/partition/_partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         r"""
         Calculate the partitioning for the given observed values.
 
         The lower and upper bounds of the range to be partitioned can be provided
         as optional arguments.
         If no bounds are provided, the partitioner automatically chooses the lower
         and upper outlier thresholds based on the Tukey test, i.e.,
-        :math:`[- 1.5 * \mathit{iqr}, 1.5 * \mathit{iqr}]`
+        :math:`[- 1.5 \cdot \mathit{iqr}, 1.5 \cdot \mathit{iqr}]`
         where :math:`\mathit{iqr}` is the inter-quartile range.
 
         :param values: a sequence of observed values as the empirical basis for
             calculating the partitions
         :param lower_bound: the inclusive lower bound of the elements to partition
         :param upper_bound: the inclusive upper bound of the elements to partition
         :param fit_params: optional fitting parameters
```

### Comparing `gamma-facet-2.0rc2/src/facet/inspection/_inspection.py` & `gamma_facet-2.1rc0/src/facet/inspection/_inspection.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import logging
 from typing import List, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
+from typing_extensions import TypeAlias
 
 from pytools.api import AllTracker
 
 from ..data import Sample
 
 log = logging.getLogger(__name__)
 
@@ -19,15 +20,15 @@
 ]
 
 
 #
 # Type aliases
 #
 
-FloatArray = npt.NDArray[np.float_]
+FloatArray: TypeAlias = npt.NDArray[np.float_]
 
 
 #
 # Ensure all symbols introduced below are included in __all__
 #
 
 __tracker = AllTracker(globals())
```

### Comparing `gamma-facet-2.0rc2/src/facet/inspection/_learner_inspector.py` & `gamma_facet-2.1rc0/src/facet/inspection/base/_model_inspector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,83 +1,70 @@
 """
-Core implementation of :mod:`facet.inspection`
+Implementation of :class:`.ModelInspector`.
 """
 import logging
-from abc import ABCMeta
+from abc import ABCMeta, abstractmethod
 from types import MethodType
 from typing import (
     Any,
     Callable,
     Generic,
     Iterable,
     List,
     Optional,
-    Sequence,
     Tuple,
-    Type,
     TypeVar,
     Union,
     cast,
 )
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 from scipy.cluster import hierarchy
 from scipy.spatial import distance
-from sklearn.base import is_classifier
+from typing_extensions import TypeAlias
 
-from pytools.api import AllTracker, inheritdoc
+from pytools.api import AllTracker
 from pytools.data import LinkageTree, Matrix
 from pytools.fit import FittableMixin, fitted_only
 from pytools.parallelization import ParallelizableMixin
-from sklearndf import ClassifierDF, LearnerDF, RegressorDF
-from sklearndf.pipeline import LearnerPipelineDF
 
-from ..data import Sample
-from ._explainer import ExplainerFactory, TreeExplainerFactory
-from ._inspection import ShapPlotData
-from ._shap import (
-    ClassifierShapInteractionValuesCalculator,
-    ClassifierShapValuesCalculator,
-    RegressorShapInteractionValuesCalculator,
-    RegressorShapValuesCalculator,
-    ShapCalculator,
-    ShapInteractionValuesCalculator,
+from facet.data import Sample
+from facet.inspection._inspection import ShapPlotData
+from facet.inspection._shap_projection import (
+    ShapInteractionVectorProjector,
+    ShapProjector,
+    ShapVectorProjector,
 )
-from ._shap_global_explanation import (
-    ShapGlobalExplainer,
-    ShapInteractionGlobalExplainer,
-)
-from ._shap_projection import ShapInteractionVectorProjector, ShapVectorProjector
+from facet.inspection.shap import ShapCalculator
 
 log = logging.getLogger(__name__)
 
 __all__ = [
-    "LearnerInspector",
     "ModelInspector",
 ]
 
 
 #
 # Type aliases
 #
 
-FloatArray = npt.NDArray[np.float_]
-FloatMatrix = Matrix[np.float_]
+FloatArray: TypeAlias = npt.NDArray[np.float_]
+FloatMatrix: TypeAlias = Matrix[np.float_]
 
 
 #
 # Type variables
 #
 
-T_LearnerInspector = TypeVar("T_LearnerInspector", bound="LearnerInspector[Any]")
-T_LearnerPipelineDF = TypeVar("T_LearnerPipelineDF", bound=LearnerPipelineDF[Any])
-T_SeriesOrDataFrame = TypeVar("T_SeriesOrDataFrame", pd.Series, pd.DataFrame)
+T_Model = TypeVar("T_Model")
+T_ModelInspector = TypeVar("T_ModelInspector", bound="ModelInspector[Any]")
 T_Number = TypeVar("T_Number", bound="np.number[Any]")
+T_SeriesOrDataFrame = TypeVar("T_SeriesOrDataFrame", pd.Series, pd.DataFrame)
 
 
 #
 # Constants
 #
 
 ASSERTION__INSPECTOR_IS_FITTED = "inspector is fitted"
@@ -92,29 +79,23 @@
 
 
 #
 # Class definitions
 #
 
 
-class ModelInspector(FittableMixin[Sample], metaclass=ABCMeta):
-    """
-    Base class of `inspectors` to explain different kinds of `models` based on SHAP
-    values.
-    """
-
-    pass
-
-
-@inheritdoc(match="[see superclass]")
-class LearnerInspector(
-    ModelInspector, ParallelizableMixin, Generic[T_LearnerPipelineDF]
+class ModelInspector(
+    ParallelizableMixin, FittableMixin[Sample], Generic[T_Model], metaclass=ABCMeta
 ):
     """
-    Explain regressors and classifiers based on SHAP values.
+    Explain a model based on SHAP values.
+
+    .. note::
+        This is an abstract base class for inspectors explaining different kinds of
+        models based on SHAP values.
 
     Focus is on explaining the overall model, but the inspector also delivers
     SHAP explanations of the individual observations.
 
     Available inspection methods are:
 
     - SHAP values
@@ -148,178 +129,109 @@
 
     # defined in superclass, repeated here for Sphinx
     pre_dispatch: Optional[Union[str, int]]
 
     # defined in superclass, repeated here for Sphinx
     verbose: Optional[int]
 
+    #: The model to inspect.
+    model: T_Model
+
+    #: If ``True``, calculate SHAP interaction values, else only calculate SHAP
+    #: contribution values.
+    #: SHAP interaction values are needed to determine feature synergy and redundancy.
+    shap_interaction: bool
+
     #: Name for feature importance series or column.
     COL_IMPORTANCE = "importance"
 
-    #: The default explainer factory used by this inspector.
-    #: This is a tree explainer using the tree_path_dependent method for
-    #: feature perturbation, so we can calculate SHAP interaction values.
-    DEFAULT_EXPLAINER_FACTORY = TreeExplainerFactory(
-        feature_perturbation="tree_path_dependent", uses_background_dataset=False
-    )
-
     def __init__(
         self,
+        model: T_Model,
         *,
-        pipeline: T_LearnerPipelineDF,
-        explainer_factory: Optional[ExplainerFactory] = None,
         shap_interaction: bool = True,
         n_jobs: Optional[int] = None,
         shared_memory: Optional[bool] = None,
         pre_dispatch: Optional[Union[str, int]] = None,
         verbose: Optional[int] = None,
     ) -> None:
         """
-        :param pipeline: the learner pipeline to inspect
-        :param explainer_factory: optional function that creates a shap Explainer
-            (default: ``TreeExplainerFactory``)
+        :param model: the model to inspect
         :param shap_interaction: if ``True``, calculate SHAP interaction values, else
-            only calculate SHAP contribution values.
+            only calculate SHAP contribution values;
             SHAP interaction values are needed to determine feature synergy and
-            redundancy.
+            redundancy
             (default: ``True``)
         """
         super().__init__(
             n_jobs=n_jobs,
             shared_memory=shared_memory,
             pre_dispatch=pre_dispatch,
             verbose=verbose,
         )
 
-        if not pipeline.is_fitted:
-            raise ValueError("arg pipeline must be fitted")
-
-        if not isinstance(pipeline.final_estimator, (ClassifierDF, RegressorDF)):
-            raise TypeError(
-                "learner in arg pipeline must be a classifier or a regressor,"
-                f"but is a {type(pipeline.final_estimator).__name__}"
-            )
-
-        if explainer_factory:
-            if not explainer_factory.explains_raw_output:
-                raise ValueError(
-                    "arg explainer_factory is not configured to explain raw output"
-                )
-        else:
-            explainer_factory = self.DEFAULT_EXPLAINER_FACTORY
-            assert explainer_factory.explains_raw_output
-
-        if shap_interaction:
-            if not explainer_factory.supports_shap_interaction_values:
-                log.warning(
-                    "ignoring arg shap_interaction=True: "
-                    f"explainers made by {explainer_factory!r} do not support "
-                    "SHAP interaction values"
-                )
-                shap_interaction = False
-
-        self.pipeline = pipeline
-        self.explainer_factory = explainer_factory
+        self.model = model
         self.shap_interaction = shap_interaction
 
-        self._shap_calculator: Optional[ShapCalculator[T_LearnerPipelineDF]] = None
-        self._shap_global_decomposer: Optional[ShapGlobalExplainer] = None
-        self._shap_global_projector: Optional[ShapGlobalExplainer] = None
+        self._shap_projector: Optional[ShapProjector] = None
         self._sample: Optional[Sample] = None
 
     __init__.__doc__ = cast(str, __init__.__doc__) + cast(
         str, ParallelizableMixin.__init__.__doc__
     )
 
-    def fit(  # type: ignore[override]
-        # todo: remove 'type: ignore' once mypy correctly infers return type
-        self: T_LearnerInspector,
-        sample: Sample,
-        **fit_params: Any,
-    ) -> T_LearnerInspector:
+    def preprocess_features(
+        self, features: Union[pd.DataFrame, pd.Series]
+    ) -> pd.DataFrame:
+        """
+        Preprocess the features prior to calculating SHAP values.
+
+        This method is called by :meth:`.fit` before fitting the inspector.
+        By default, returns the features unchanged.
+
+        :param features: features to preprocess
+        :return: preprocessed features
+        """
+        return features
+
+    def fit(
+        self: T_ModelInspector, __sample: Sample, **fit_params: Any
+    ) -> T_ModelInspector:
         """
         Fit the inspector with the given sample, creating global explanations including
         feature redundancy and synergy.
 
         This will calculate SHAP values and, if enabled in the underlying SHAP
         explainer, also SHAP interaction values.
 
-        :param sample: the background sample to be used for the global explanation
+        :param __sample: the background sample to be used for the global explanation
             of this model
         :param fit_params: additional keyword arguments (ignored; accepted for
             compatibility with :class:`.FittableMixin`)
         :return: ``self``
         """
 
-        learner: LearnerDF = self.pipeline.final_estimator
-
-        _is_classifier = is_classifier(learner)
-        if _is_classifier and isinstance(sample.target_name, list):
-            raise ValueError(
-                "only single-output classifiers (binary or multi-class) are supported, "
-                "but the given classifier has been fitted on multiple columns "
-                f"{sample.target_name}"
-            )
-
-        shap_global_projector: Union[
-            ShapVectorProjector, ShapInteractionVectorProjector, None
-        ]
-
-        shap_calculator_type: Type[ShapCalculator[T_LearnerPipelineDF]]
-        shap_calculator: ShapCalculator[T_LearnerPipelineDF]
-
-        if self.shap_interaction:
-            if _is_classifier:
-                shap_calculator_type = ClassifierShapInteractionValuesCalculator
-            else:
-                shap_calculator_type = RegressorShapInteractionValuesCalculator
-
-            shap_calculator = shap_calculator_type(
-                pipeline=self.pipeline,
-                explainer_factory=self.explainer_factory,
-                n_jobs=self.n_jobs,
-                shared_memory=self.shared_memory,
-                pre_dispatch=self.pre_dispatch,
-                verbose=self.verbose,
-            )
-
-            shap_global_projector = ShapInteractionVectorProjector()
+        shap_calculator: ShapCalculator[Any] = self.shap_calculator
 
-        else:
-            if _is_classifier:
-                shap_calculator_type = ClassifierShapValuesCalculator
-            else:
-                shap_calculator_type = RegressorShapValuesCalculator
+        shap_calculator.fit(self.preprocess_features(__sample.features))
 
-            shap_calculator = shap_calculator_type(
-                pipeline=self.pipeline,
-                explainer_factory=self.explainer_factory,
-                n_jobs=self.n_jobs,
-                shared_memory=self.shared_memory,
-                pre_dispatch=self.pre_dispatch,
-                verbose=self.verbose,
-            )
-
-            shap_global_projector = ShapVectorProjector()
+        shap_global_projector: ShapProjector = (
+            ShapInteractionVectorProjector()
+            if self.shap_interaction
+            else ShapVectorProjector()
+        )
 
-        shap_calculator.fit(sample)
-        shap_global_projector.fit(shap_calculator=shap_calculator)
+        shap_global_projector.fit(shap_calculator, sample_weight=__sample.weight)
 
-        self._sample = sample
-        self._shap_calculator = shap_calculator
-        self._shap_global_projector = shap_global_projector
+        self._sample = __sample
+        self._shap_projector = shap_global_projector
 
         return self
 
     @property
-    def _shap_global_explainer(self) -> ShapGlobalExplainer:
-        assert self._shap_global_projector is not None, ASSERTION__INSPECTOR_IS_FITTED
-        return self._shap_global_projector
-
-    @property
     def is_fitted(self) -> bool:
         """[see superclass]"""
         return self._sample is not None
 
     @property
     @fitted_only
     def sample_(self) -> Sample:
@@ -327,77 +239,75 @@
         The background sample used to fit this inspector.
         """
 
         assert self._sample is not None, ASSERTION__INSPECTOR_IS_FITTED
         return self._sample
 
     @property
-    @fitted_only
-    def output_names_(self) -> Sequence[str]:
+    @abstractmethod
+    def feature_names(self) -> List[str]:
+        """
+        The feature names of the model being inspected.
+
+        These names may differ from the feature names expected for the sample
+        set has been preprocessed before calculating SHAP values.
+
+        :return: the feature names
+        """
+        pass
+
+    @property
+    def output_names(self) -> List[str]:
         """
         The names of the outputs explained by this inspector.
 
         For regressors, these are the names of the target columns.
 
         For binary classifiers, this is a list of length 1 with the name of a single
         class, since the SHAP values of the second class can be trivially derived as
         the negation of the SHAP values of the first class.
 
         For non-binary classifiers, this is the list of all classes.
         """
-
-        assert (
-            self._shap_calculator is not None
-            and self._shap_calculator.output_names_ is not None
-        ), ASSERTION__INSPECTOR_IS_FITTED
-        return self._shap_calculator.output_names_
-
-    @property
-    @fitted_only
-    def features_(self) -> List[str]:
-        """
-        The names of the features used to fit the learner pipeline explained by this
-        inspector.
-        """
-        return cast(List[str], self.pipeline.feature_names_out_.to_list())
+        return self.shap_calculator.output_names
 
     @fitted_only
     def shap_values(self) -> Union[pd.DataFrame, List[pd.DataFrame]]:
         """
         Calculate the SHAP values for all observations and features.
 
         Returns a data frame of SHAP values where each row corresponds to an
         observation, and each column corresponds to a feature.
 
         :return: a data frame with SHAP values
         """
 
-        assert self._shap_calculator is not None, ASSERTION__INSPECTOR_IS_FITTED
-        return self.__split_multi_output_df(self._shap_calculator.get_shap_values())
+        return self.__split_multi_output_df(self.shap_calculator.shap_values)
 
     @fitted_only
     def shap_interaction_values(self) -> Union[pd.DataFrame, List[pd.DataFrame]]:
         """
         Calculate the SHAP interaction values for all observations and pairs of
         features.
 
         Returns a data frame of SHAP interaction values where each row corresponds to an
         observation and a feature (identified by a hierarchical index with two levels),
         and each column corresponds to a feature.
 
         :return: a data frame with SHAP interaction values
         """
         return self.__split_multi_output_df(
-            self.__shap_interaction_values_calculator.get_shap_interaction_values()
+            self.shap_calculator.shap_interaction_values
         )
 
     @fitted_only
     def feature_importance(
         self, *, method: str = "rms"
     ) -> Union[pd.Series, pd.DataFrame]:
+        # noinspection GrazieInspection
         """
         Calculate the relative importance of each feature based on SHAP values.
 
         The importance values of all features always add up to `1.0`.
 
         The calculation applies sample weights if specified in the underlying
         :class:`.Sample`.
@@ -409,16 +319,15 @@
             data frame of shape (n_features, n_outputs) for multi-output models
         """
 
         methods = {"rms", "mav"}
         if method not in methods:
             raise ValueError(f'arg method="{method}" must be one of {methods}')
 
-        assert self._shap_calculator is not None
-        shap_matrix: pd.DataFrame = self._shap_calculator.get_shap_values()
+        shap_matrix: pd.DataFrame = self.shap_calculator.shap_values
         weight: Optional[pd.Series] = self.sample_.weight
 
         abs_importance: pd.Series
         if method == "rms":
             if weight is None:
                 abs_importance = shap_matrix.pow(2).mean().pow(0.5)
             else:
@@ -431,16 +340,16 @@
                 abs_importance = shap_matrix.abs().mul(weight, axis=0).mean()
 
         def _normalize_importance(
             _importance: T_SeriesOrDataFrame,
         ) -> T_SeriesOrDataFrame:
             return _importance.divide(_importance.sum())
 
-        if len(self.output_names_) == 1:
-            return _normalize_importance(abs_importance).rename(self.output_names_[0])
+        if len(self.output_names) == 1:
+            return _normalize_importance(abs_importance).rename(self.output_names[0])
 
         else:
             assert (
                 abs_importance.index.nlevels == 2
             ), "2 index levels in place for multi-output models"
 
             return _normalize_importance(abs_importance.unstack(level=0))
@@ -483,15 +392,15 @@
             ``False``, keep rows and columns in the original features order
             (default: ``True``)
         :return: feature synergy matrix as a data frame of shape
             `(n_features, n_features)`, or a list of data frames for multiple outputs
         """
 
         return self.__feature_affinity_matrix(
-            explainer_fn=self.__interaction_explainer.synergy,
+            explainer_fn=self.__interaction_projector.synergy,
             absolute=absolute,
             symmetrical=symmetrical,
             clustered=clustered,
         )
 
     @fitted_only
     def feature_redundancy_matrix(
@@ -531,15 +440,15 @@
             ``False``, keep rows and columns in the original features order
             (default: ``True``)
         :return: feature redundancy matrix as a data frame of shape
             `(n_features, n_features)`, or a list of data frames for multiple outputs
         """
 
         return self.__feature_affinity_matrix(
-            explainer_fn=self.__interaction_explainer.redundancy,
+            explainer_fn=self.__interaction_projector.redundancy,
             absolute=absolute,
             symmetrical=symmetrical,
             clustered=clustered,
         )
 
     @fitted_only
     def feature_association_matrix(
@@ -580,16 +489,17 @@
             such that association between adjacent rows and columns is maximised; if
             ``False``, keep rows and columns in the original features order
             (default: ``True``)
         :return: feature association matrix as a data frame of shape
             `(n_features, n_features)`, or a list of data frames for multiple outputs
         """
 
+        assert self._shap_projector is not None, ASSERTION__INSPECTOR_IS_FITTED
         return self.__feature_affinity_matrix(
-            explainer_fn=self._shap_global_explainer.association,
+            explainer_fn=self._shap_projector.association,
             absolute=absolute,
             symmetrical=symmetrical,
             clustered=clustered,
         )
 
     @fitted_only
     def feature_synergy_linkage(self) -> Union[LinkageTree, List[LinkageTree]]:
@@ -602,15 +512,15 @@
         In the case of multi-target regression and non-binary classification, returns
         a list of linkage trees per target or class.
 
         :return: linkage tree of feature synergies; list of linkage trees
             for multi-target regressors or non-binary classifiers
         """
 
-        feature_affinity_matrix = self.__interaction_explainer.synergy(
+        feature_affinity_matrix = self.__interaction_projector.synergy(
             symmetrical=True, absolute=False
         )
         assert (
             feature_affinity_matrix is not None
         ), ASSERTION__SHAP_INTERACTION_SUPPORTED
 
         return self.__linkages_from_affinity_matrices(
@@ -628,15 +538,15 @@
         In the case of multi-target regression and non-binary classification, returns
         a list of linkage trees per target or class.
 
         :return: linkage tree of feature redundancies; list of linkage trees
             for multi-target regressors or non-binary classifiers
         """
 
-        feature_affinity_matrix = self.__interaction_explainer.redundancy(
+        feature_affinity_matrix = self.__interaction_projector.redundancy(
             symmetrical=True, absolute=False
         )
         assert (
             feature_affinity_matrix is not None
         ), ASSERTION__SHAP_INTERACTION_SUPPORTED
 
         return self.__linkages_from_affinity_matrices(
@@ -654,15 +564,16 @@
         In the case of multi-target regression and non-binary classification, returns
         a list of linkage trees per target or class.
 
         :return: linkage tree of feature associations; list of linkage trees
             for multi-target regressors or non-binary classifiers
         """
 
-        feature_affinity_matrix = self._shap_global_explainer.association(
+        assert self._shap_projector is not None, ASSERTION__INSPECTOR_IS_FITTED
+        feature_affinity_matrix = self._shap_projector.association(
             absolute=False, symmetrical=True
         )
         assert (
             feature_affinity_matrix is not None
         ), ASSERTION__SHAP_INTERACTION_SUPPORTED
 
         return self.__linkages_from_affinity_matrices(
@@ -719,16 +630,16 @@
         In the case of multi-target regression and non-binary classification, returns
         a list with one matrix per output.
 
         :return: relative shap interaction values as a data frame of shape
             `(n_features, n_features)`; or a list of such data frames
         """
 
-        n_features = len(self.features_)
-        n_outputs = len(self.output_names_)
+        n_features = len(self.feature_names)
+        n_outputs = len(self.output_names)
 
         # get a feature interaction array with shape
         # (n_observations, n_outputs, n_features, n_features)
         # where the innermost feature x feature arrays are symmetrical
         im_matrix_per_observation_and_output: FloatArray = (
             # TODO missing proper handling for list of data frames
             self.shap_interaction_values()  # type: ignore
@@ -779,22 +690,22 @@
     def shap_plot_data(self) -> ShapPlotData:
         """
         Consolidate SHAP values and corresponding feature values from this inspector
         for use in SHAP plots offered by the
         `shap <https://shap.readthedocs.io/en/stable/>`__ package.
 
         The `shap` package provides functions for creating various SHAP plots.
-        Most of these functions require
+        Most of these functions require:
 
         - one or more SHAP value matrices as a single `numpy` array,
           or a list of `numpy` arrays of shape `(n_observations, n_features)`
         - a feature matrix of shape `(n_observations, n_features)`, which can be
           provided as a data frame to preserve feature names
 
-        This method provides this data inside a :class:`.ShapPlotData` object, plus
+        This method provides this data inside a :class:`.ShapPlotData` object, plus:
 
         - the names of all outputs (i.e., the target names in case of regression,
           or the class names in case of classification)
         - corresponding target values as a series, or as a data frame in the case of
           multiple targets
 
         This method also ensures that the rows of all arrays, frames, and series are
@@ -805,15 +716,15 @@
         splits for which SHAP values were calculated.
 
         :return: consolidated SHAP and feature values for use shap plots
         """
 
         shap_values: Union[pd.DataFrame, List[pd.DataFrame]] = self.shap_values()
 
-        output_names: Sequence[str] = self.output_names_
+        output_names: List[str] = self.output_names
         shap_values_numpy: Union[FloatArray, List[FloatArray]]
         included_observations: pd.Index
 
         if len(output_names) > 1:
             shap_values_numpy = [s.values for s in shap_values]
             included_observations = shap_values[0].index
         else:
@@ -824,24 +735,31 @@
         sample: Sample = self.sample_.subsample(loc=included_observations)
 
         return ShapPlotData(
             shap_values=shap_values_numpy,
             sample=sample,
         )
 
+    @property
+    @abstractmethod
+    def shap_calculator(self) -> ShapCalculator[Any]:
+        """
+        The SHAP calculator used by this inspector.
+        """
+
     def __arrays_to_matrix(
         self, matrix: FloatArray, value_label: str
     ) -> Union[FloatMatrix, List[FloatMatrix]]:
         # transform a matrix of shape (n_outputs, n_features, n_features)
         # to a data frame
 
-        feature_index = self.pipeline.feature_names_out_.rename(Sample.IDX_FEATURE)
+        feature_index = self.feature_names
 
         n_features = len(feature_index)
-        assert matrix.shape == (len(self.output_names_), n_features, n_features)
+        assert matrix.shape == (len(self.output_names), n_features, n_features)
 
         # convert array to data frame(s) with features as row and column indices
         if len(matrix) == 1:
             return self.__array_to_matrix(
                 matrix[0],
                 feature_importance=self.feature_importance(),
                 value_label=value_label,
@@ -850,30 +768,30 @@
             return [
                 self.__array_to_matrix(
                     m,
                     feature_importance=feature_importance,
                     value_label=f"{value_label} ({output_name})",
                 )
                 for m, (_, feature_importance), output_name in zip(
-                    matrix, self.feature_importance().items(), self.output_names_
+                    matrix, self.feature_importance().items(), self.output_names
                 )
             ]
 
     def __feature_affinity_matrix(
         self,
         *,
         explainer_fn: Callable[..., FloatArray],
         absolute: bool,
         symmetrical: bool,
         clustered: bool,
     ) -> Union[FloatMatrix, List[FloatMatrix]]:
         affinity_matrices = explainer_fn(symmetrical=symmetrical, absolute=absolute)
 
-        explainer: ShapGlobalExplainer = cast(
-            ShapGlobalExplainer, cast(MethodType, explainer_fn).__self__
+        explainer: ShapProjector = cast(
+            ShapProjector, cast(MethodType, explainer_fn).__self__
         )
         affinity_matrices_df: List[pd.DataFrame] = explainer.to_frames(
             affinity_matrices
         )
 
         if clustered:
             affinity_symmetrical = explainer_fn(symmetrical=True, absolute=False)
@@ -892,15 +810,15 @@
 
     @staticmethod
     def __sort_affinity_matrices(
         affinity_matrices: List[pd.DataFrame],
         symmetrical_affinity_matrices: FloatArray,
     ) -> List[pd.DataFrame]:
         # abbreviate a very long function name to stay within the permitted line length
-        fn_linkage = LearnerInspector.__linkage_matrix_from_affinity_matrix_for_output
+        fn_linkage = ModelInspector.__linkage_matrix_from_affinity_matrix_for_output
 
         return [
             (lambda feature_order: affinity_matrix.iloc[feature_order, feature_order])(
                 feature_order=hierarchy.leaves_list(
                     Z=fn_linkage(feature_affinity_matrix=symmetrical_affinity_matrix)
                 )
             )
@@ -941,18 +859,17 @@
             # we have only a single output
             # feature importance is already a series
             return self.__linkage_tree_from_affinity_matrix_for_output(
                 feature_affinity_matrix[0], feature_importance
             )
 
         else:
-            # noinspection PyCompatibility
             feature_importance_iter: (
                 Iterable[Tuple[Any, pd.Series]]
-            ) = feature_importance.iteritems()
+            ) = feature_importance.items()
 
             return [
                 self.__linkage_tree_from_affinity_matrix_for_output(
                     feature_affinity_for_output,
                     feature_importance_for_output,
                 )
                 for feature_affinity_for_output, (
@@ -961,28 +878,28 @@
                 ) in zip(feature_affinity_matrix, feature_importance_iter)
             ]
 
     @staticmethod
     def __linkage_tree_from_affinity_matrix_for_output(
         feature_affinity_matrix: FloatArray, feature_importance: pd.Series
     ) -> LinkageTree:
-        # calculate the linkage tree from the a given output in a feature distance
+        # calculate the linkage tree from the given output in a feature distance
         # matrix;
         # matrix has shape (n_features, n_features) with values ranging from
         # (1 = closest, 0 = most distant)
 
         linkage_matrix: FloatArray = (
-            LearnerInspector.__linkage_matrix_from_affinity_matrix_for_output(
+            ModelInspector.__linkage_matrix_from_affinity_matrix_for_output(
                 feature_affinity_matrix
             )
         )
 
         # Feature labels and weights will be used as the leaves of the linkage tree.
         # Select only the features that appear in the distance matrix, and in the
-        # correct order
+        # correct order.
 
         # build and return the linkage tree
         return LinkageTree(
             scipy_linkage_matrix=linkage_matrix,
             leaf_names=feature_importance.index,
             leaf_weights=feature_importance.values,
             max_distance=1.0,
@@ -991,15 +908,15 @@
             weight_label="feature importance",
         )
 
     @staticmethod
     def __linkage_matrix_from_affinity_matrix_for_output(
         feature_affinity_matrix: FloatArray,
     ) -> FloatArray:
-        # calculate the linkage matrix from the a given output in a feature distance
+        # calculate the linkage matrix from the given output in a feature distance
         # matrix;
         # matrix has shape (n_features, n_features) with values ranging from
         # (1 = closest, 0 = most distant)
 
         # compress the distance matrix (required by SciPy)
         distance_matrix = 1.0 - abs(feature_affinity_matrix)
         np.fill_diagonal(distance_matrix, 0.0)
@@ -1085,22 +1002,13 @@
                 if feature_importance_category
                 else affinity_metric
             ),
             name_labels=("primary feature", "associated feature"),
         )
 
     @property
-    def __shap_interaction_values_calculator(
-        self,
-    ) -> ShapInteractionValuesCalculator[T_LearnerPipelineDF]:
-        self._ensure_shap_interaction()
-        return cast(
-            ShapInteractionValuesCalculator[T_LearnerPipelineDF], self._shap_calculator
-        )
-
-    @property
-    def __interaction_explainer(self) -> ShapInteractionGlobalExplainer:
+    def __interaction_projector(self) -> ShapInteractionVectorProjector:
         self._ensure_shap_interaction()
-        return cast(ShapInteractionGlobalExplainer, self._shap_global_explainer)
+        return cast(ShapInteractionVectorProjector, self._shap_projector)
 
 
 __tracker.validate()
```

### Comparing `gamma-facet-2.0rc2/src/facet/inspection/_shap_global_explanation.py` & `gamma_facet-2.1rc0/src/facet/inspection/_shap_context.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,33 +2,29 @@
 Projection of SHAP contribution scores (i.e, SHAP importance) of all possible
 pairings of features onto the SHAP importance vector in partitions of for synergy,
 redundancy, and independence.
 """
 from __future__ import annotations
 
 import logging
-from abc import ABCMeta, abstractmethod
-from typing import Any, List, Optional, TypeVar, Union, cast
+from typing import Any, Optional, Union, cast
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
-from pytools.api import AllTracker, inheritdoc
-from pytools.fit import FittableMixin
+from pytools.api import AllTracker
 
-from ._shap import ShapCalculator
+from .shap import ShapCalculator
 
 log = logging.getLogger(__name__)
 
 __all__ = [
     "AffinityMatrix",
     "ShapContext",
-    "ShapGlobalExplainer",
-    "ShapInteractionGlobalExplainer",
     "ShapInteractionValueContext",
     "ShapValueContext",
     "cov",
     "cov_broadcast",
     "diagonal",
     "ensure_last_axis_is_fast",
     "fill_diagonal",
@@ -39,21 +35,14 @@
 
 #: if ``True``, optimize numpy arrays to ensure pairwise partial summation.
 #: But given that we will add floats of the same order of magnitude and only up
 #: to a few thousand of them in the base case, the loss of accuracy with regular
 #: (sequential) summation will be negligible in practice
 _PAIRWISE_PARTIAL_SUMMATION = False
 
-#
-# Type variables
-#
-
-T_ShapGlobalExplainer = TypeVar("T_ShapGlobalExplainer", bound="ShapGlobalExplainer")
-T_ShapCalculator = TypeVar("T_ShapCalculator", bound=ShapCalculator[Any])
-
 
 #
 # Constants
 #
 ASSERTION__CALCULATOR_IS_FITTED = "calculator is fitted"
 
 
@@ -144,149 +133,14 @@
         :return: the affinity matrix
         """
         return cast(
             npt.NDArray[np.float_], self._matrices[int(symmetrical), int(absolute)]
         )
 
 
-@inheritdoc(match="""[see superclass]""")
-class ShapGlobalExplainer(FittableMixin[ShapCalculator[Any]], metaclass=ABCMeta):
-    """
-    Derives feature association as a global metric of SHAP values for multiple
-    observations.
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.feature_index_: Optional[pd.Index] = None
-
-    @property
-    def is_fitted(self) -> bool:
-        """[see superclass]"""
-        return self.feature_index_ is not None
-
-    def fit(  # type: ignore[override]
-        self: T_ShapGlobalExplainer,
-        shap_calculator: ShapCalculator[Any],
-        **fit_params: Any,
-    ) -> T_ShapGlobalExplainer:
-        """
-        Calculate the SHAP decomposition for the shap values produced by the
-        given SHAP calculator.
-
-        :param shap_calculator: the fitted calculator from which to get the shap values
-        """
-
-        try:
-            if len(fit_params) > 0:
-                raise ValueError(
-                    f'unsupported fit parameters: {", ".join(fit_params.values())}'
-                )
-
-            self._fit(shap_calculator=shap_calculator)
-
-            self.feature_index_ = shap_calculator.feature_index_
-
-        except Exception:
-            # reset fit in case we get an exception along the way
-            self._reset_fit()
-            raise
-
-        return self
-
-    @abstractmethod
-    def association(self, absolute: bool, symmetrical: bool) -> npt.NDArray[np.float_]:
-        """
-        The association matrix for all feature pairs.
-
-        Raises an error if this global explainer has not been fitted.
-
-        :param absolute: if ``False``, return relative association as a percentage of
-            total feature importance;
-            if ``True``, return absolute association as a portion of feature importance
-        :param symmetrical: if ``False``, return an asymmetrical matrix
-            quantifying unilateral association of the features represented by rows
-            with the features represented by columns;
-            if ``True``, return a symmetrical matrix quantifying mutual association
-        :returns: the matrix as an array of shape (n_outputs, n_features, n_features)
-        """
-
-    def to_frames(self, matrix: npt.NDArray[np.float_]) -> List[pd.DataFrame]:
-        """
-        Transforms one or more affinity matrices into a list of data frames.
-
-        :param matrix: an array of shape `(n_outputs, n_features, n_features)`,
-            representing one or more affinity matrices
-        :return: a list of `n_outputs` data frames of shape `(n_features, n_features)`
-        """
-        assert self.feature_index_ is not None, "explainer is fitted"
-        index = self.feature_index_
-
-        n_features = len(index)
-        assert matrix.ndim == 3
-        assert matrix.shape[1:] == (n_features, n_features)
-
-        return [
-            pd.DataFrame(
-                m,
-                index=index,
-                columns=index,
-            )
-            for m in matrix
-        ]
-
-    @abstractmethod
-    def _fit(self, shap_calculator: ShapCalculator[Any]) -> None:
-        pass
-
-    def _reset_fit(self) -> None:
-        self.feature_index_ = None
-
-
-class ShapInteractionGlobalExplainer(ShapGlobalExplainer, metaclass=ABCMeta):
-    """
-    Derives feature association, synergy, and redundancy as a global metric of SHAP
-    interaction values for multiple observations.
-    """
-
-    @abstractmethod
-    def synergy(self, symmetrical: bool, absolute: bool) -> npt.NDArray[np.float_]:
-        """
-        The synergy matrix for all feature pairs.
-
-        Raises an error if this global explainer has not been fitted.
-
-        :param absolute: if ``False``, return relative synergy as a percentage of
-            total feature importance;
-            if ``True``, return absolute synergy as a portion of feature importance
-        :param symmetrical: if ``False``, return an asymmetrical matrix
-            quantifying unilateral synergy of the features represented by rows
-            with the features represented by columns;
-            if ``True``, return a symmetrical matrix quantifying mutual synergy
-        :returns: the matrix as an array of shape (n_outputs, n_features, n_features)
-        """
-
-    @abstractmethod
-    def redundancy(self, symmetrical: bool, absolute: bool) -> npt.NDArray[np.float_]:
-        """
-        The redundancy matrix for all feature pairs.
-
-        Raises an error if this global explainer has not been fitted.
-
-        :param absolute: if ``False``, return relative redundancy as a percentage of
-            total feature importance;
-            if ``True``, return absolute redundancy as a portion of feature importance
-        :param symmetrical: if ``False``, return an asymmetrical matrix
-            quantifying unilateral redundancy of the features represented by rows
-            with the features represented by columns;
-            if ``True``, return a symmetrical matrix quantifying mutual redundancy
-        :returns: the matrix as an array of shape (n_outputs, n_features, n_features)
-        """
-
-
 #
 # Utility functions
 #
 
 
 def ensure_last_axis_is_fast(array: npt.NDArray[np.float_]) -> npt.NDArray[np.float_]:
     """
@@ -458,15 +312,15 @@
 
     return cast(
         npt.NDArray[np.float_],
         np.einsum("...io,...ijo->...ij", vectors_weighted, vector_grid) / weight_total,
     )
 
 
-class ShapContext(metaclass=ABCMeta):
+class ShapContext:
     """
     Contextual data for global SHAP calculations.
     """
 
     #: SHAP vectors
     #: with shape `(n_outputs, n_features, n_observations)`
     p_i: npt.NDArray[np.float_]
@@ -514,23 +368,24 @@
 
 
 class ShapValueContext(ShapContext):
     """
     Contextual data for global SHAP calculations based on SHAP values.
     """
 
-    def __init__(self, shap_calculator: ShapCalculator[Any]) -> None:
-        shap_values: pd.DataFrame = shap_calculator.get_shap_values()
+    def __init__(
+        self, shap_calculator: ShapCalculator[Any], sample_weight: Optional[pd.Series]
+    ) -> None:
+        shap_values: pd.DataFrame = shap_calculator.shap_values
 
         def _p_i() -> npt.NDArray[np.float_]:
             assert (
-                shap_calculator.output_names_ is not None
-                and shap_calculator.feature_index_ is not None
+                shap_calculator.feature_index_ is not None
             ), ASSERTION__CALCULATOR_IS_FITTED
-            n_outputs: int = len(shap_calculator.output_names_)
+            n_outputs: int = len(shap_calculator.output_names)
             n_features: int = len(shap_calculator.feature_index_)
             n_observations: int = len(shap_values)
 
             # p[i]
             # shape: (n_outputs, n_features, n_observations)
             # the vector of shap values for every output and feature
             return ensure_last_axis_is_fast(
@@ -541,65 +396,62 @@
             )
 
         def _weight() -> Optional[npt.NDArray[np.float_]]:
             # weights
             # shape: (n_observations)
             # return a 1d array of weights that aligns with the observations axis of the
             # SHAP values tensor (axis 1)
-            assert (
-                shap_calculator.sample_ is not None and ASSERTION__CALCULATOR_IS_FITTED
-            )
-            _weight_sr = shap_calculator.sample_.weight
-            if _weight_sr is not None:
+
+            if sample_weight is not None:
                 return cast(
                     npt.NDArray[np.float_],
-                    _weight_sr.loc[shap_values.index.get_level_values(-1)].values,
+                    sample_weight.loc[shap_values.index.get_level_values(-1)].values,
                 )
             else:
                 return None
 
         super().__init__(p_i=_p_i(), p_ij=None, weight=_weight())
 
 
 class ShapInteractionValueContext(ShapContext):
     """
     Contextual data for global SHAP calculations based on SHAP interaction values.
     """
 
-    def __init__(self, shap_calculator: ShapCalculator[Any]) -> None:
-        shap_values: pd.DataFrame = shap_calculator.get_shap_interaction_values()
+    def __init__(
+        self, shap_calculator: ShapCalculator[Any], sample_weight: Optional[pd.Series]
+    ) -> None:
+        shap_values: pd.DataFrame = shap_calculator.shap_interaction_values
 
         assert (
-            shap_calculator.output_names_ is not None
-            and shap_calculator.feature_index_ is not None
+            shap_calculator.feature_index_ is not None
         ), ASSERTION__CALCULATOR_IS_FITTED
         n_features: int = len(shap_calculator.feature_index_)
-        n_outputs: int = len(shap_calculator.output_names_)
+        n_outputs: int = len(shap_calculator.output_names)
         n_observations: int = len(shap_values) // n_features
 
         assert shap_values.shape == (
             n_observations * n_features,
             n_outputs * n_features,
         )
 
         self.matrix_shape = (n_outputs, n_features, n_features)
 
         # weights
         # shape: (n_observations)
         # return a 1d array of weights that aligns with the observations axis of the
         # SHAP values tensor (axis 1)
         weight: Optional[npt.NDArray[np.float_]]
-        assert shap_calculator.sample_ is not None and ASSERTION__CALCULATOR_IS_FITTED
-        _weight_sr = shap_calculator.sample_.weight
-        if _weight_sr is not None:
+
+        if sample_weight is not None:
             _observation_indices = shap_values.index.get_level_values(
                 -2
             ).values.reshape((n_observations, n_features))[:, 0]
             weight = ensure_last_axis_is_fast(
-                _weight_sr.loc[_observation_indices].values
+                sample_weight.loc[_observation_indices].values
             )
         else:
             weight = None
 
         # p[i, j]
         # shape: (n_outputs, n_features, n_features, n_observations)
         # the vector of interaction values for every output and feature pairing
```

### Comparing `gamma-facet-2.0rc2/src/facet/inspection/_shap_projection.py` & `gamma_facet-2.1rc0/src/facet/inspection/_shap_projection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 """
 Projection of SHAP contribution scores (i.e, SHAP importance) of all possible
 pairings of features onto the SHAP importance vector in partitions of for synergy,
 redundancy, and independence.
 """
 import logging
 from abc import ABCMeta, abstractmethod
-from typing import Any, Optional, Tuple, TypeVar
+from typing import Any, List, Optional, Tuple, TypeVar
 
 import numpy as np
 import numpy.typing as npt
+import pandas as pd
 
 from pytools.api import AllTracker, inheritdoc
-from pytools.fit import fitted_only
+from pytools.fit import FittableMixin, fitted_only
 
-from ._shap import ShapCalculator
-from ._shap_global_explanation import (
+from ._shap_context import (
     AffinityMatrix,
     ShapContext,
-    ShapGlobalExplainer,
-    ShapInteractionGlobalExplainer,
     ShapInteractionValueContext,
     ShapValueContext,
     cov,
     cov_broadcast,
     ensure_last_axis_is_fast,
     fill_diagonal,
     sqrt,
     transpose,
 )
+from .shap import ShapCalculator
 
 log = logging.getLogger(__name__)
 
 __all__ = ["ShapInteractionVectorProjector", "ShapProjector", "ShapVectorProjector"]
 
 #: if ``True``, optimize numpy arrays to ensure pairwise partial summation.
 #: But given that we will add floats of the same order of magnitude and only up
@@ -40,55 +39,134 @@
 _PAIRWISE_PARTIAL_SUMMATION = False
 
 #
 # Type variables
 #
 
 T_Self = TypeVar("T_Self")
+T_Projector = TypeVar("T_Projector", bound="ShapProjector")
 
 #
 # Ensure all symbols introduced below are included in __all__
 #
 
 __tracker = AllTracker(globals())
 
 
 #
 # Class definitions
 #
 
 
 @inheritdoc(match="""[see superclass]""")
-class ShapProjector(ShapGlobalExplainer, metaclass=ABCMeta):
+class ShapProjector(FittableMixin[ShapCalculator[Any]], metaclass=ABCMeta):
     """
     Base class for global pairwise model explanations based on SHAP vector projection.
+
+    Derives feature association as a global metric of SHAP values for multiple
+    observations.
     """
 
     def __init__(self) -> None:
         super().__init__()
+        self.feature_index_: Optional[pd.Index] = None
         self.association_: Optional[AffinityMatrix] = None
 
+    @property
+    def is_fitted(self) -> bool:
+        """[see superclass]"""
+        return self.feature_index_ is not None
+
+    def fit(  # type: ignore[override]
+        self: T_Projector,
+        shap_calculator: ShapCalculator[Any],
+        *,
+        sample_weight: Optional[pd.Series] = None,
+        **fit_params: Any,
+    ) -> T_Projector:
+        """
+        Calculate the SHAP decomposition for the shap values produced by the
+        given SHAP calculator.
+
+        :param shap_calculator: the fitted calculator from which to get the shap values
+        :param sample_weight: optional sample weights to apply for the global
+            explanations; the index must match the index of the features used to
+            fit the SHAP calculator
+        """
+
+        self._reset_fit()
+
+        if len(fit_params) > 0:
+            raise ValueError(
+                f'unsupported fit parameters: {", ".join(fit_params.values())}'
+            )
+
+        self._calculate(
+            self._get_context(
+                shap_calculator=shap_calculator, sample_weight=sample_weight
+            )
+        )
+
+        self.feature_index_ = shap_calculator.feature_index_
+
+        return self
+
     @fitted_only
     def association(self, absolute: bool, symmetrical: bool) -> npt.NDArray[np.float_]:
-        """[see superclass]"""
+        """
+        The association matrix for all feature pairs.
+
+        Raises an error if this global explainer has not been fitted.
+
+        :param absolute: if ``False``, return relative association as a percentage of
+            total feature importance;
+            if ``True``, return absolute association as a portion of feature importance
+        :param symmetrical: if ``False``, return an asymmetrical matrix
+            quantifying unilateral association of the features represented by rows
+            with the features represented by columns;
+            if ``True``, return a symmetrical matrix quantifying mutual association
+        :returns: the matrix as an array of shape (n_outputs, n_features, n_features)
+        """
 
         assert self.association_ is not None
         return self.association_.get_values(symmetrical=symmetrical, absolute=absolute)
 
-    def _fit(self, shap_calculator: ShapCalculator[Any]) -> None:
-        self._reset_fit()
-        self._calculate(self._get_context(shap_calculator=shap_calculator))
+    def to_frames(self, matrix: npt.NDArray[np.float_]) -> List[pd.DataFrame]:
+        """
+        Transforms one or more affinity matrices into a list of data frames.
+
+        :param matrix: an array of shape `(n_outputs, n_features, n_features)`,
+            representing one or more affinity matrices
+        :return: a list of `n_outputs` data frames of shape `(n_features, n_features)`
+        """
+        assert self.feature_index_ is not None, "explainer is fitted"
+        index = self.feature_index_
+
+        n_features = len(index)
+        assert matrix.ndim == 3
+        assert matrix.shape[1:] == (n_features, n_features)
+
+        return [
+            pd.DataFrame(
+                m,
+                index=index,
+                columns=index,
+            )
+            for m in matrix
+        ]
 
     def _reset_fit(self) -> None:
         # revert status of this object to not fitted
-        super()._reset_fit()
+        self.feature_index_ = None
         self.association_ = None
 
     @abstractmethod
-    def _get_context(self, shap_calculator: ShapCalculator[Any]) -> ShapContext:
+    def _get_context(
+        self, shap_calculator: ShapCalculator[Any], sample_weight: Optional[pd.Series]
+    ) -> ShapContext:
         pass
 
     @abstractmethod
     def _calculate(self, context: ShapContext) -> None:
         pass
 
     @staticmethod
@@ -125,25 +203,31 @@
     """
     Decomposes SHAP interaction scores (i.e, SHAP importance) of all possible pairings
     of features into additive components for association and independence.
     This is achieved through scalar projection of redundancy and synergy vectors
     onto a feature's main SHAP vector.
     """
 
-    def _get_context(self, shap_calculator: ShapCalculator[Any]) -> ShapContext:
-        return ShapValueContext(shap_calculator=shap_calculator)
+    def _get_context(
+        self, shap_calculator: ShapCalculator[Any], sample_weight: Optional[pd.Series]
+    ) -> ShapContext:
+        return ShapValueContext(
+            shap_calculator=shap_calculator, sample_weight=sample_weight
+        )
 
     def _calculate(self, context: ShapContext) -> None:
         # calculate association matrices for each SHAP context, then aggregate
         self.association_ = self._calculate_association(context)
 
 
-@inheritdoc(match="""[see superclass]""")
-class ShapInteractionVectorProjector(ShapProjector, ShapInteractionGlobalExplainer):
+class ShapInteractionVectorProjector(ShapProjector):
     """
+    Derives feature association, synergy, and redundancy as a global metric of SHAP
+    interaction values for multiple observations.
+
     Decomposes SHAP interaction scores (i.e, SHAP importance) of all possible pairings
     of features into additive components for synergy, redundancy, and independence.
     This is achieved through scalar projection of redundancy and synergy vectors
     onto a feature's main SHAP vector.
     SHAP interaction scores are calculated as the standard deviation of the individual
     interactions per observation. Using this metric, rather than the mean of absolute
     interactions, allows us to calculate the decomposition without ever constructing
@@ -154,28 +238,58 @@
         super().__init__()
 
         self.synergy_: Optional[AffinityMatrix] = None
         self.redundancy_: Optional[AffinityMatrix] = None
 
     @fitted_only
     def synergy(self, symmetrical: bool, absolute: bool) -> npt.NDArray[np.float_]:
-        """[see superclass]"""
+        """
+        The synergy matrix for all feature pairs.
+
+        Raises an error if this global explainer has not been fitted.
+
+        :param absolute: if ``False``, return relative synergy as a percentage of
+            total feature importance;
+            if ``True``, return absolute synergy as a portion of feature importance
+        :param symmetrical: if ``False``, return an asymmetrical matrix
+            quantifying unilateral synergy of the features represented by rows
+            with the features represented by columns;
+            if ``True``, return a symmetrical matrix quantifying mutual synergy
+        :returns: the matrix as an array of shape (n_outputs, n_features, n_features)
+        """
 
         assert self.synergy_ is not None, "Projector is fitted"
         return self.synergy_.get_values(symmetrical=symmetrical, absolute=absolute)
 
     @fitted_only
     def redundancy(self, symmetrical: bool, absolute: bool) -> npt.NDArray[np.float_]:
-        """[see superclass]"""
+        """
+        The redundancy matrix for all feature pairs.
+
+        Raises an error if this global explainer has not been fitted.
+
+        :param absolute: if ``False``, return relative redundancy as a percentage of
+            total feature importance;
+            if ``True``, return absolute redundancy as a portion of feature importance
+        :param symmetrical: if ``False``, return an asymmetrical matrix
+            quantifying unilateral redundancy of the features represented by rows
+            with the features represented by columns;
+            if ``True``, return a symmetrical matrix quantifying mutual redundancy
+        :returns: the matrix as an array of shape (n_outputs, n_features, n_features)
+        """
 
         assert self.redundancy_ is not None, "Projector is fitted"
         return self.redundancy_.get_values(symmetrical=symmetrical, absolute=absolute)
 
-    def _get_context(self, shap_calculator: ShapCalculator[Any]) -> ShapContext:
-        return ShapInteractionValueContext(shap_calculator=shap_calculator)
+    def _get_context(
+        self, shap_calculator: ShapCalculator[Any], sample_weight: Optional[pd.Series]
+    ) -> ShapContext:
+        return ShapInteractionValueContext(
+            shap_calculator=shap_calculator, sample_weight=sample_weight
+        )
 
     def _calculate(self, context: ShapContext) -> None:
         # calculate association, synergy, and redundancy matrices for the SHAP context
 
         self.association_ = self._calculate_association(context=context)
         self.synergy_, self.redundancy_ = self._calculate_synergy_redundancy(
             context=context
@@ -281,18 +395,20 @@
 
         # we should have the right shape for all resulting matrices
         assert syn_ij.shape == matrix_shape
         assert red_ij.shape == matrix_shape
 
         # Calculate relative synergy and redundancy (ranging from 0.0 to 1.0),
         # as a symmetric and an asymmetric measure.
+        #
         # For the symmetric case, we ensure perfect symmetry by removing potential
-        # round-off errors
+        # round-off errors.
+        #
         # NOTE: we do not store independence, so technically it could be removed from
-        # the code above
+        # the code above.
 
         std_p_i = sqrt(var_p_i)
         return (
             AffinityMatrix.from_relative_affinity(
                 affinity_rel_ij=syn_ij, std_p_i=std_p_i
             ),
             AffinityMatrix.from_relative_affinity(
```

### Comparing `gamma-facet-2.0rc2/src/facet/selection/_parameters.py` & `gamma_facet-2.1rc0/src/facet/selection/_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Type,
     TypeVar,
     Union,
 )
 
 from scipy import stats
 from sklearn.base import BaseEstimator
+from typing_extensions import TypeAlias
 
 from pytools.api import AllTracker, inheritdoc, subsdoc, to_list, validate_element_types
 from pytools.expression import Expression, make_expression
 from pytools.expression.atomic import Id
 from sklearndf import EstimatorDF
 from sklearndf.pipeline import LearnerPipelineDF, PipelineDF
 
@@ -37,19 +38,19 @@
 __all__ = [
     "MultiEstimatorParameterSpace",
     "ParameterSpace",
 ]
 
 
 #
-# Type constants
+# Type aliases
 #
 
-ParameterSet = Union[List[Any], stats.rv_continuous, stats.rv_discrete]
-ParameterDict = Dict[str, ParameterSet]
+ParameterSet: TypeAlias = Union[List[Any], stats.rv_continuous, stats.rv_discrete]
+ParameterDict: TypeAlias = Dict[str, ParameterSet]
 
 try:
     rv_frozen = next(
         t for t in type(stats.uniform()).mro() if t.__name__ == "rv_frozen"
     )
 except StopIteration:
     warnings.warn(
@@ -180,15 +181,14 @@
             "__".join(name): values
             for (name, values) in self._iter_parameters(
                 path_prefix=[] if prefix is None else [prefix]
             )
         }
 
     def _validate_parameter(self, name: str, value: ParameterSet) -> None:
-
         if name not in self._params:
             raise AttributeError(
                 f"unknown parameter name for "
                 f"{type(self.estimator).__name__}: {name}"
             )
 
         if not (
@@ -217,15 +217,14 @@
             self._values[name] = value
 
     def __dir__(self) -> Iterable[str]:
         return {*super().__dir__(), *self._params}
 
     def __getattr__(self, key: str) -> Any:
         if not key.startswith("_"):
-
             result: Union[ParameterSpace[Any], ParameterSet, None]
 
             result = self._children.get(key, None)
             if result is not None:
                 return result
 
             result = self._values.get(key, None)
@@ -236,15 +235,14 @@
 
     def __iter__(self) -> Iterator[Tuple[List[str], ParameterSet]]:
         return self._iter_parameters([])
 
     def _iter_parameters(
         self, path_prefix: List[str]
     ) -> Iterator[Tuple[List[str], ParameterSet]]:
-
         yield from (
             ([*path_prefix, name], value) for name, value in self._values.items()
         )
 
         for name, child in self._children.items():
             yield from child._iter_parameters([*path_prefix, name])
```

### Comparing `gamma-facet-2.0rc2/src/facet/selection/_selection.py` & `gamma_facet-2.1rc0/src/facet/selection/_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,20 +427,15 @@
                 sort_column_processed = None
             else:
                 sort_column_processed = sort_by
                 cv_results_processed[sort_by] = cv_results[sort_by]
 
         # convert the results into a data frame and sort
 
-        report = pd.DataFrame(
-            {
-                name_processed: values
-                for name_processed, values in cv_results_processed.values()
-            }
-        )
+        report = pd.DataFrame(dict(cv_results_processed.values()))
 
         # sort the report, if applicable
 
         if sort_column_processed is not None:
             report = report.sort_values(by=sort_column_processed)
 
         # split column headers containing one or more "__",
```

### Comparing `gamma-facet-2.0rc2/src/facet/selection/base/_parameters.py` & `gamma_facet-2.1rc0/src/facet/selection/base/_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Core implementation of :mod:`facet.selection.base`
 """
 
 import logging
 from abc import ABCMeta, abstractmethod
-from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
+from typing import Any, Dict, Generic, List, Optional, TypeVar, Union, cast
 
 import numpy.typing as npt
 import pandas as pd
 from scipy import stats
 
 from pytools.api import AllTracker, inheritdoc
 from pytools.expression import HasExpressionRepr
@@ -147,74 +147,80 @@
 
         if self.candidate is None:
             raise AttributeError("no candidate has been assigned")
         else:
             return self.candidate
 
     def _get_classes(self) -> Union[npt.NDArray[Any], List[npt.NDArray[Any]]]:
-        return self._get_candidate().classes_
+        return cast(
+            Union[npt.NDArray[Any], List[npt.NDArray[Any]]],
+            self._get_candidate()._get_classes(),
+        )
 
     # noinspection PyPep8Naming
     def predict_proba(
-        self, X: pd.DataFrame, **predict_params: Any
+        self, X: Union[pd.Series, pd.DataFrame], **predict_params: Any
     ) -> Union[pd.DataFrame, List[pd.DataFrame]]:
         """[see superclass]"""
         return self._get_candidate().predict_proba(X, **predict_params)
 
     # noinspection PyPep8Naming
     def predict_log_proba(
-        self, X: pd.DataFrame, **predict_params: Any
+        self, X: Union[pd.Series, pd.DataFrame], **predict_params: Any
     ) -> Union[pd.DataFrame, List[pd.DataFrame]]:
         """[see superclass]"""
         return self._get_candidate().predict_log_proba(X, **predict_params)
 
     # noinspection PyPep8Naming
     def decision_function(
-        self, X: pd.DataFrame, **predict_params: Any
+        self, X: Union[pd.Series, pd.DataFrame], **predict_params: Any
     ) -> Union[pd.Series, pd.DataFrame]:
         """[see superclass]"""
         return self._get_candidate().decision_function(X, **predict_params)
 
     # noinspection PyPep8Naming
     def score(
-        self, X: pd.DataFrame, y: pd.Series, sample_weight: Optional[pd.Series] = None
+        self,
+        X: Union[pd.Series, pd.DataFrame],
+        y: pd.Series,
+        sample_weight: Optional[pd.Series] = None,
     ) -> float:
         """[see superclass]"""
         return self._get_candidate().score(X, y, sample_weight)
 
     # noinspection PyPep8Naming
     def predict(
-        self, X: pd.DataFrame, **predict_params: Any
+        self, X: Union[pd.Series, pd.DataFrame], **predict_params: Any
     ) -> Union[pd.Series, pd.DataFrame]:
         """[see superclass]"""
         return self._get_candidate().predict(X, **predict_params)
 
     # noinspection PyPep8Naming
     def fit(
         self: T_CandidateEstimatorDF,
-        X: pd.DataFrame,
+        X: Union[pd.Series, pd.DataFrame],
         y: Optional[Union[pd.Series, pd.DataFrame]] = None,
         **fit_params: Any,
     ) -> T_CandidateEstimatorDF:
         """[see superclass]"""
         self._get_candidate().fit(X, y, **fit_params)
         return self
 
     @property
     def is_fitted(self) -> bool:
         """[see superclass]"""
         return self.candidate is not None and self.candidate.is_fitted
 
     # noinspection PyPep8Naming
-    def inverse_transform(self, X: pd.DataFrame) -> pd.DataFrame:
+    def inverse_transform(self, X: Union[pd.Series, pd.DataFrame]) -> pd.DataFrame:
         """[see superclass]"""
         return self._get_candidate().inverse_transform(X)
 
     # noinspection PyPep8Naming
-    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
+    def transform(self, X: Union[pd.Series, pd.DataFrame]) -> pd.DataFrame:
         """[see superclass]"""
         return self._get_candidate().transform(X)
 
     @property
     def _estimator_type(self) -> str:
         # noinspection PyProtectedMember
         return self.candidate._estimator_type  # type: ignore
```

### Comparing `gamma-facet-2.0rc2/src/facet/simulation/_result.py` & `gamma_facet-2.1rc0/src/facet/simulation/_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         :param feature_name: name of the simulated feature
         :param output_name: name of the target for which outputs are simulated
         :param output_unit: the unit of the simulated outputs
             (e.g., uplift or class probability)
         :param baseline: the average observed actual output, acting as the baseline
             of the simulation
         :param confidence_level: the width of the confidence interval determined by
-            bootstrapping, ranging between 0.0 and 1.0 (exclusive)
+            the standard error of the mean, ranging between 0.0 and 1.0 (exclusive)
         """
         super().__init__()
 
         if not partitioner.is_fitted:
             raise ValueError("arg partitioner must be fitted")
 
         n_partitions = len(partitioner.partitions_)
```

### Comparing `gamma-facet-2.0rc2/src/facet/simulation/_simulation.py` & `gamma_facet-2.1rc0/src/facet/simulation/_simulation.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/src/facet/simulation/base/_base.py` & `gamma_facet-2.1rc0/src/facet/simulation/base/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 
 import numpy as np
 import pandas as pd
 
 from pytools.api import AllTracker
 from pytools.parallelization import Job, JobRunner, ParallelizableMixin
-from sklearndf import LearnerDF, RegressorDF
+from sklearndf import RegressorDF, SupervisedLearnerDF
 
 from facet.data import Sample
 from facet.data.partition import Partitioner
 from facet.simulation._result import UnivariateSimulationResult
 
 log = logging.getLogger(__name__)
 
@@ -37,26 +37,26 @@
 
 
 #
 # Type variables
 #
 
 T_Value = TypeVar("T_Value", bound=np.generic)
-T_LearnerDF = TypeVar("T_LearnerDF", bound=LearnerDF)
+T_SupervisedLearnerDF = TypeVar("T_SupervisedLearnerDF", bound=SupervisedLearnerDF)
 
 
 #
 # Ensure all symbols introduced below are included in __all__
 #
 
 __tracker = AllTracker(globals())
 
 
 class BaseUnivariateSimulator(
-    ParallelizableMixin, Generic[T_LearnerDF], metaclass=ABCMeta
+    ParallelizableMixin, Generic[T_SupervisedLearnerDF], metaclass=ABCMeta
 ):
     """
     Base class for univariate simulations.
     """
 
     # defined in superclass, repeated here for Sphinx
     n_jobs: Optional[int]
@@ -67,26 +67,26 @@
     # defined in superclass, repeated here for Sphinx
     pre_dispatch: Optional[Union[str, int]]
 
     # defined in superclass, repeated here for Sphinx
     verbose: Optional[int]
 
     #: The learner pipeline used to conduct simulations
-    model: T_LearnerDF
+    model: T_SupervisedLearnerDF
 
     #: The sample to be used in baseline calculations and simulations
     sample: Sample
 
     #: The width of the confidence interval used to calculate the lower/upper bound
     #: of the simulation
     confidence_level: float
 
     def __init__(
         self,
-        model: T_LearnerDF,
+        model: T_SupervisedLearnerDF,
         sample: Sample,
         *,
         confidence_level: float = 0.95,
         n_jobs: Optional[int] = None,
         shared_memory: Optional[bool] = None,
         pre_dispatch: Optional[Union[str, int]] = None,
         verbose: Optional[int] = None,
@@ -195,21 +195,21 @@
 
         :return: the expectation value of the actual model output
         """
         pass
 
     @staticmethod
     @abstractmethod
-    def _expected_learner_type() -> Type[T_LearnerDF]:
+    def _expected_learner_type() -> Type[T_SupervisedLearnerDF]:
         pass
 
     @staticmethod
     @abstractmethod
     def _simulate(
-        model: T_LearnerDF, x: pd.DataFrame, name: str, value: Any
+        model: T_SupervisedLearnerDF, x: pd.DataFrame, name: str, value: Any
     ) -> Tuple[float, float]:
         pass
 
     @staticmethod
     def _set_constant_feature_value(
         x: pd.DataFrame, feature_name: str, value: Any
     ) -> pd.DataFrame:
```

### Comparing `gamma-facet-2.0rc2/src/facet/simulation/viz/_draw.py` & `gamma_facet-2.1rc0/src/facet/simulation/viz/_draw.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/src/facet/simulation/viz/_style.py` & `gamma_facet-2.1rc0/src/facet/simulation/viz/_style.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/src/facet/validation/_validation.py` & `gamma_facet-2.1rc0/src/facet/validation/_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
                     n_samples=n, random_state=rs, y=y
                 )
                 test_mask: npt.NDArray[np.bool_] = np.ones(n, dtype=bool)
                 test_mask[train] = False
                 test: npt.NDArray[np.int_] = indices[test_mask]
                 # make sure test is not empty, else sample another train set
                 if len(test) > 0:
-
                     yield train, test
                     break
 
     @abstractmethod
     def _select_train_indices(
         self,
         n_samples: int,
@@ -250,15 +249,14 @@
 
     def _select_train_indices(
         self,
         n_samples: int,
         random_state: np.random.RandomState,
         y: Union[npt.NDArray[Any], pd.Series, pd.DataFrame, None],
     ) -> npt.NDArray[np.int_]:
-
         mean_block_size = self.mean_block_size
         if mean_block_size < 1:
             # if mean block size was set as a percentage, calculate the actual mean
             # block size
             mean_block_size = n_samples * mean_block_size
 
         p_new_block = 1.0 / mean_block_size
```

### Comparing `gamma-facet-2.0rc2/test/test/conftest.py` & `gamma_facet-2.1rc0/test/test/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
-from typing import Any, Dict, List, Mapping, Optional, Sequence, Set, Tuple, cast
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, cast
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import pytest
 from numpy.testing import assert_allclose, assert_array_equal
 from sklearn import datasets
 from sklearn.datasets import fetch_california_housing
 from sklearn.model_selection import BaseCrossValidator, GridSearchCV, KFold
 from sklearn.utils import Bunch
 
-from sklearndf import TransformerDF
+from sklearndf import RegressorDF, TransformerDF
 from sklearndf.classification import RandomForestClassifierDF
 from sklearndf.pipeline import ClassifierPipelineDF, RegressorPipelineDF
 from sklearndf.regression import (
     SVRDF,
     AdaBoostRegressorDF,
     DecisionTreeRegressorDF,
     ExtraTreeRegressorDF,
@@ -27,26 +27,27 @@
     ColumnTransformerDF,
     OneHotEncoderDF,
     SimpleImputerDF,
 )
 
 import facet
 from facet.data import Sample
-from facet.inspection import LearnerInspector, TreeExplainerFactory
+from facet.inspection import LearnerInspector
 from facet.selection import LearnerSelector, ParameterSpace
 from facet.validation import BootstrapCV, StratifiedBootstrapCV
 
 logging.basicConfig(level=logging.DEBUG)
 log = logging.getLogger(__name__)
 
 # print the FACET logo
 print(facet.__logo__)
 
-# disable SHAP debugging messages
+# disable 3rd party debugging messages
 logging.getLogger("shap").setLevel(logging.WARNING)
+logging.getLogger("numba").setLevel(logging.WARNING)
 
 # configure pandas text output
 
 # get display width from terminal
 pd.set_option("display.width", None)
 # 3 digits precision for easier readability
 pd.set_option("display.precision", 3)
@@ -90,15 +91,15 @@
     # define a CV
     return StratifiedBootstrapCV(n_splits=N_BOOTSTRAPS, random_state=42)
 
 
 @pytest.fixture  # type: ignore
 def regressor_parameters(
     simple_preprocessor: TransformerDF,
-) -> List[ParameterSpace[RegressorPipelineDF[LGBMRegressorDF]]]:
+) -> List[ParameterSpace[RegressorPipelineDF[RegressorDF]]]:
     random_state = {"random_state": 42}
 
     space_1 = ParameterSpace(
         RegressorPipelineDF(
             preprocessing=simple_preprocessor, regressor=LGBMRegressorDF(**random_state)
         )
     )
@@ -154,26 +155,30 @@
 
     return [space_1, space_2, space_3, space_4, space_5, space_6, space_7]
 
 
 @pytest.fixture  # type: ignore
 def regressor_selector(
     cv_kfold: KFold,
-    regressor_parameters: List[ParameterSpace[RegressorPipelineDF[LGBMRegressorDF]]],
+    regressor_parameters: List[ParameterSpace[RegressorPipelineDF[RegressorDF]]],
     sample: Sample,
     n_jobs: int,
-) -> LearnerSelector[RegressorPipelineDF[LGBMRegressorDF], GridSearchCV]:
-    return LearnerSelector(
+) -> LearnerSelector[RegressorPipelineDF[RegressorDF], GridSearchCV]:
+    selector_fitted = LearnerSelector(
         searcher_type=GridSearchCV,
         parameter_space=regressor_parameters,
         cv=cv_kfold,
         scoring="r2",
         n_jobs=n_jobs,
     ).fit(sample=sample)
 
+    log.debug(f"Fitted learner selector:\n{selector_fitted.summary_report()}")
+
+    return selector_fitted
+
 
 PARAM_CANDIDATE__ = "param_candidate__"
 
 
 @pytest.fixture  # type: ignore
 def best_lgbm_model(
     regressor_selector: LearnerSelector[
@@ -204,39 +209,14 @@
             }
         )
         .fit(X=sample.features, y=sample.target)
     )
 
 
 @pytest.fixture  # type: ignore
-def preprocessed_feature_names(
-    best_lgbm_model: RegressorPipelineDF[LGBMRegressorDF],
-) -> Set[str]:
-    """
-    Names of all features after preprocessing
-    """
-    return set(best_lgbm_model.final_estimator.feature_names_in_)
-
-
-@pytest.fixture  # type: ignore
-def regressor_inspector(
-    best_lgbm_model: RegressorPipelineDF[LGBMRegressorDF], sample: Sample, n_jobs: int
-) -> LearnerInspector[RegressorPipelineDF[LGBMRegressorDF]]:
-    inspector = LearnerInspector(
-        pipeline=best_lgbm_model,
-        explainer_factory=TreeExplainerFactory(
-            feature_perturbation="tree_path_dependent", uses_background_dataset=True
-        ),
-        n_jobs=n_jobs,
-    ).fit(sample=sample)
-
-    return inspector
-
-
-@pytest.fixture  # type: ignore
 def simple_preprocessor(sample: Sample) -> TransformerDF:
     features = sample.features
 
     column_transforms: List[Tuple[str, Any, Any]] = []
 
     numeric_columns: pd.Index = features.select_dtypes(np.number).columns
     if numeric_columns is not None and len(numeric_columns) > 0:
@@ -249,15 +229,15 @@
         )
 
     category_columns = features.select_dtypes(object).columns
     if category_columns is not None and len(category_columns) > 0:
         column_transforms.append(
             (
                 STEP_ONE_HOT_ENCODE,
-                OneHotEncoderDF(sparse=False, handle_unknown="ignore"),
+                OneHotEncoderDF(handle_unknown="ignore"),
                 list(map(str, category_columns)),
             )
         )
 
     return ColumnTransformerDF(transformers=column_transforms)
 
 
@@ -453,16 +433,16 @@
 @pytest.fixture  # type: ignore
 def iris_inspector_multi_class(
     iris_classifier_multi_class: ClassifierPipelineDF[RandomForestClassifierDF],
     iris_sample_multi_class: Sample,
     n_jobs: int,
 ) -> LearnerInspector[ClassifierPipelineDF[RandomForestClassifierDF]]:
     return LearnerInspector(
-        pipeline=iris_classifier_multi_class, shap_interaction=True, n_jobs=n_jobs
-    ).fit(sample=iris_sample_multi_class)
+        model=iris_classifier_multi_class, shap_interaction=True, n_jobs=n_jobs
+    ).fit(iris_sample_multi_class)
 
 
 #
 # Utility functions
 #
```

### Comparing `gamma-facet-2.0rc2/test/test/facet/test_inspection.py` & `gamma_facet-2.1rc0/test/test/facet/test_inspection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,235 @@
 """
 Model inspector tests.
 """
 import logging
+import platform
 import warnings
-from typing import List, Optional, Set, TypeVar, cast
+from typing import Any, Dict, List, Optional, Set, Type, TypeVar, Union, cast
 
 import numpy as np
 import pandas as pd
 import pytest
 from numpy.testing import assert_allclose
+from pandas._testing import assert_index_equal
 from pandas.testing import assert_frame_equal, assert_series_equal
 from sklearn.datasets import make_classification
+from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import GridSearchCV
+from sklearn.pipeline import Pipeline
 
 from pytools.data import LinkageTree, Matrix
 from pytools.viz.dendrogram import DendrogramDrawer, DendrogramReportStyle
+from sklearndf import ClassifierDF, __sklearn_1_1__, __sklearn_version__
 from sklearndf.classification import (
     GradientBoostingClassifierDF,
     RandomForestClassifierDF,
 )
 from sklearndf.pipeline import ClassifierPipelineDF, RegressorPipelineDF
 from sklearndf.regression.extra import LGBMRegressorDF
 
 from ..conftest import check_ranking
 from facet.data import Sample
-from facet.inspection import (
+from facet.explanation import (
+    ExactExplainerFactory,
     KernelExplainerFactory,
-    LearnerInspector,
+    PermutationExplainerFactory,
     TreeExplainerFactory,
 )
+from facet.explanation.base import ExplainerFactory
+from facet.inspection import FunctionInspector, LearnerInspector, NativeLearnerInspector
 from facet.selection import LearnerSelector
 
 # noinspection PyMissingOrEmptyDocstring
 
 log = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 def test_regressor_selector(
     regressor_selector: LearnerSelector[
         RegressorPipelineDF[LGBMRegressorDF], GridSearchCV
     ]
 ) -> None:
+    scores_expected: List[float] = (
+        [0.578, 0.530, 0.310, 0.308, 0.294, 0.226, 0.217, 0.217, 0.217, 0.217]
+        if (
+            __sklearn_version__ < __sklearn_1_1__
+            or platform.machine() != "arm64"
+            or platform.system() != "Darwin"
+        )
+        # on M1 macs, we get different results starting with scikit-learn 1.1
+        else [0.579, 0.531, 0.311, 0.308, 0.246, 0.217, 0.217, 0.217, 0.217, 0.217]
+    )
     check_ranking(
         ranking=regressor_selector.summary_report(),
         is_classifier=False,
-        scores_expected=(
-            [0.578, 0.530, 0.310, 0.308, 0.294, 0.226, 0.217, 0.217, 0.217, 0.217]
-        ),
+        scores_expected=scores_expected,
         params_expected=None,
     )
 
 
+@pytest.mark.parametrize(  # type: ignore
+    argnames=("explainer_factory_cls", "explainer_factory_args"),
+    argvalues=[
+        (
+            TreeExplainerFactory,
+            dict(
+                feature_perturbation="tree_path_dependent", uses_background_dataset=True
+            ),
+        ),
+        (KernelExplainerFactory, dict(link="identity", data_size_limit=8)),
+        (ExactExplainerFactory, {}),
+        (PermutationExplainerFactory, {}),
+    ],
+)
+@pytest.mark.parametrize(  # type: ignore
+    argnames="native",
+    argvalues=(False, True),
+)
 def test_model_inspection(
+    explainer_factory_cls: Type[ExplainerFactory[LGBMRegressorDF]],
+    explainer_factory_args: Dict[str, Any],
     best_lgbm_model: RegressorPipelineDF[LGBMRegressorDF],
-    preprocessed_feature_names: Set[str],
-    regressor_inspector: LearnerInspector[RegressorPipelineDF[LGBMRegressorDF]],
     sample: Sample,
     n_jobs: int,
+    native: bool,
 ) -> None:
-    shap_values: pd.DataFrame = regressor_inspector.shap_values()
+    # test the ModelInspector with the given explainer factory:
+
+    explainer_factory: ExplainerFactory[LGBMRegressorDF] = explainer_factory_cls(
+        **explainer_factory_args
+    )
+
+    inspector: Union[
+        LearnerInspector[RegressorPipelineDF[LGBMRegressorDF]],
+        NativeLearnerInspector[Pipeline],
+    ]
+
+    regressor_feature_names: Set[str]  # column index names
+
+    if native:
+        assert (
+            best_lgbm_model.preprocessing is not None
+        ), "preprocessing step must be defined"
+
+        regressor = best_lgbm_model.regressor.native_estimator
+
+        if __sklearn_version__ < __sklearn_1_1__:
+            # scikit-learn 1.0.x does not support output feature names in simple
+            # imputers, so we cannot use this for preprocessing
+            log.warning(
+                f"scikit-learn {__sklearn_version__} does not support output "
+                "feature names in simple imputers, so we will test the native learner "
+                "inspector without preprocessing"
+            )
+            assert (
+                sample.features.notna().all().all()
+            ), "observations must not contain missing values"
+            model = regressor
+            regressor_feature_names = set(sample.feature_names)
+
+        else:
+            # scikit-learn 1.1.x supports output feature names in simple imputers,
+            # so we can use this for preprocessing
+            model = Pipeline(
+                # create a native pipeline from the regressor pipeline
+                steps=[
+                    (
+                        "preprocessing",
+                        best_lgbm_model.preprocessing.native_estimator,
+                    ),
+                    ("regressor", regressor),
+                ]
+            ).fit(X=sample.features, y=sample.target)
+            regressor_feature_names = set(model[:-1].get_feature_names_out())
+
+        # noinspection PyTypeChecker
+        inspector = NativeLearnerInspector(
+            model=model,
+            explainer_factory=explainer_factory,
+            n_jobs=n_jobs,
+        ).fit(sample)
+    else:
+        inspector = LearnerInspector(
+            model=best_lgbm_model,
+            explainer_factory=explainer_factory,
+            n_jobs=n_jobs,
+        ).fit(sample)
+        regressor_feature_names = set(best_lgbm_model.regressor.feature_names_in_)
+
+    shap_values: pd.DataFrame = inspector.shap_values()
 
     # the length of rows in shap_values should be equal to the unique observation
     # indices we have had in the predictions_df
     assert len(shap_values) == len(sample)
 
     # index names
     assert shap_values.index.names == [Sample.IDX_OBSERVATION]
     assert shap_values.columns.names == [Sample.IDX_FEATURE]
 
-    # column index
-    assert set(shap_values.columns) == preprocessed_feature_names
+    # check that the column names are the same as the feature names
+    assert set(shap_values.columns) == set(regressor_feature_names)
+
+    # check that the row order has been preserved
+    assert_index_equal(shap_values.index, sample.index)
 
     # check that the SHAP values add up to the predictions
     shap_totals = shap_values.sum(axis=1)
 
     # calculate the difference between total SHAP values and prediction
     # for every observation. This is always the same constant value,
     # therefore the mean absolute deviation is zero.
 
-    shap_minus_pred = shap_totals - best_lgbm_model.predict(X=sample.features)
-    assert round(shap_minus_pred.mad(), 12) == 0.0, "predictions matching total SHAP"
+    shap_minus_pred = shap_totals - inspector.model.predict(X=sample.features)
+    assert (
+        round((shap_minus_pred - shap_minus_pred.mean()).abs().mean(), 12) == 0.0
+    ), "predictions matching total SHAP"
 
-    #  test the ModelInspector with a KernelExplainer:
+    # validate the linkage tree of the resulting inspector
 
-    inspector_2 = LearnerInspector(
-        pipeline=best_lgbm_model,
-        explainer_factory=KernelExplainerFactory(link="identity", data_size_limit=20),
-        n_jobs=n_jobs,
-    ).fit(sample=sample)
-    inspector_2.shap_values()
+    # if the inspector supports interaction values, test the redundancy linkage
+    # otherwise test the association linkage
+    if inspector.shap_interaction:
+        linkage = inspector.feature_redundancy_linkage()
+        mode = "Redundancy"
+    else:
+        linkage = inspector.feature_association_linkage()
+        mode = "Association"
+
+    # validate the linkage tree
 
-    linkage_tree = cast(LinkageTree, inspector_2.feature_association_linkage())
+    assert isinstance(linkage, LinkageTree)
+    # get the node whose child distance is < 0.8, and confirm it is the only one
+    cluster_nodes = [
+        node
+        for node in linkage.iter_nodes()
+        if not node.is_leaf and node.children_distance < 0.7
+    ]
+    assert len(cluster_nodes) == 1, "only two features form a cluster"
+    # check the child nodes are Longitude and Latitude
+    children = linkage.children(cluster_nodes[0])
+    assert children is not None, "a cluster node has children"
+    assert {child.name.split("__")[-1] for child in children} == (
+        {"Longitude", "Latitude"}
+    ), "the cluster is Longitude and Latitude features"
 
     print()
-    DendrogramDrawer(style="text").draw(data=linkage_tree, title="Test")
+    DendrogramDrawer(style="text").draw(
+        data=linkage,
+        title=f"{inspector.explainer_factory.__class__.__name__} ({mode})",
+    )
 
 
 def test_binary_classifier_ranking(
     iris_classifier_selector_binary: LearnerSelector[
         ClassifierPipelineDF[RandomForestClassifierDF], GridSearchCV
     ]
 ) -> None:
-
     expected_learner_scores = [0.938, 0.936, 0.936, 0.929]
 
     ranking = iris_classifier_selector_binary.summary_report()
 
     log.debug(f"\n{ranking}")
 
     check_ranking(
@@ -123,20 +245,19 @@
 
 # noinspection DuplicatedCode
 def test_model_inspection_classifier_binary(
     iris_classifier_binary: ClassifierPipelineDF[RandomForestClassifierDF],
     iris_sample_binary: Sample,
     n_jobs: int,
 ) -> None:
-
     model_inspector = LearnerInspector(
-        pipeline=iris_classifier_binary,
+        model=iris_classifier_binary,
         shap_interaction=False,
         n_jobs=n_jobs,
-    ).fit(sample=iris_sample_binary)
+    ).fit(iris_sample_binary)
 
     # calculate the shap value matrix, without any consolidation
     shap_values = model_inspector.shap_values()
 
     # do the shap values add up to predictions minus a constant value?
     _validate_shap_values_against_predictions(
         shap_values=shap_values, model=iris_classifier_binary, sample=iris_sample_binary
@@ -175,15 +296,15 @@
 
     print()
     DendrogramDrawer(style=DendrogramReportStyle()).draw(
         data=linkage_tree, title="Iris (binary) feature association linkage"
     )
 
 
-def test_model_inspection_classifier_binary_single_shap_output() -> None:
+def test_model_inspection_classifier_binary_single_shap_output(n_jobs: int) -> None:
     # simulate some data
     x, y = make_classification(
         n_samples=200, n_features=5, n_informative=5, n_redundant=0, random_state=42
     )
     sim_df = pd.DataFrame(
         np.hstack([x, y[:, np.newaxis]]),
         columns=[*(f"f{i}" for i in range(5)), "target"],
@@ -194,24 +315,24 @@
 
     # fit the model
     pipeline = ClassifierPipelineDF(
         classifier=GradientBoostingClassifierDF(random_state=42)
     ).fit(sample_df.features, sample_df.target)
 
     # fit the inspector
-    LearnerInspector(pipeline=pipeline, n_jobs=-3).fit(sample=sample_df)
+    LearnerInspector(model=pipeline, n_jobs=n_jobs).fit(sample_df)
 
 
 # noinspection DuplicatedCode
 def test_model_inspection_classifier_multi_class(
     iris_inspector_multi_class: LearnerInspector[
         ClassifierPipelineDF[RandomForestClassifierDF]
     ],
 ) -> None:
-    iris_classifier = iris_inspector_multi_class.pipeline
+    iris_classifier = iris_inspector_multi_class.model
     iris_sample = iris_inspector_multi_class.sample_
 
     # calculate the shap value matrix, without any consolidation
     shap_values = iris_inspector_multi_class.shap_values()
 
     # do the shap values add up to predictions minus a constant value?
     _validate_shap_values_against_predictions(
@@ -221,15 +342,15 @@
     # Feature importance
 
     feature_importance: pd.DataFrame = iris_inspector_multi_class.feature_importance()
     assert feature_importance.index.equals(
         pd.Index(iris_sample.feature_names, name="feature")
     )
     assert feature_importance.columns.equals(
-        pd.Index(iris_inspector_multi_class.output_names_, name="class")
+        pd.Index(iris_inspector_multi_class.output_names, name="class")
     )
     assert_allclose(
         feature_importance.values,
         np.array(
             [
                 [0.122, 0.086, 0.102],
                 [0.020, 0.021, 0.007],
@@ -311,28 +432,25 @@
         raise
 
     linkage_trees = cast(
         List[LinkageTree], iris_inspector_multi_class.feature_association_linkage()
     )
 
     for output, linkage_tree in zip(
-        iris_inspector_multi_class.output_names_, linkage_trees
+        iris_inspector_multi_class.output_names, linkage_trees
     ):
         print()
         DendrogramDrawer(style=DendrogramReportStyle()).draw(
             data=linkage_tree, title=f"Iris feature association linkage: {output}"
         )
 
 
 def _validate_shap_values_against_predictions(
-    shap_values: pd.DataFrame,
-    model: ClassifierPipelineDF[RandomForestClassifierDF],
-    sample: Sample,
+    shap_values: pd.DataFrame, model: ClassifierDF, sample: Sample
 ) -> None:
-
     # calculate the matching predictions, so we can check if the SHAP values add up
     # correctly
     predicted_probabilities: pd.DataFrame = model.predict_proba(sample.features)
 
     assert isinstance(
         predicted_probabilities, pd.DataFrame
     ), "predicted probabilities are single-output"
@@ -381,37 +499,56 @@
                 -shap_values[class_idx].sum(axis=1).rename("shap")
             )
 
             _check_probabilities(class_probabilities, shap_for_split_and_class)
 
 
 # noinspection DuplicatedCode
+@pytest.mark.parametrize(  # type: ignore
+    argnames="native",
+    argvalues=(False, True),
+)
 def test_model_inspection_classifier_interaction(
     iris_classifier_binary: ClassifierPipelineDF[RandomForestClassifierDF],
     iris_sample_binary: Sample,
     n_jobs: int,
+    native: bool,
 ) -> None:
     warnings.filterwarnings("ignore", message="You are accessing a training score")
 
-    model_inspector = LearnerInspector(
-        pipeline=iris_classifier_binary,
+    cls_inspector: Type[
+        Union[
+            LearnerInspector[RandomForestClassifierDF],
+            NativeLearnerInspector[RandomForestClassifier],
+        ]
+    ]
+    learner: Union[RandomForestClassifierDF, RandomForestClassifier]
+    if native:
+        cls_inspector = NativeLearnerInspector[RandomForestClassifier]
+        learner = iris_classifier_binary.final_estimator.native_estimator
+    else:
+        cls_inspector = LearnerInspector[RandomForestClassifierDF]
+        learner = iris_classifier_binary.final_estimator
+
+    model_inspector = cls_inspector(
+        model=learner,
         explainer_factory=TreeExplainerFactory(
             feature_perturbation="tree_path_dependent", uses_background_dataset=True
         ),
         n_jobs=n_jobs,
-    ).fit(sample=iris_sample_binary)
+    ).fit(iris_sample_binary)
 
-    model_inspector_no_interaction = LearnerInspector(
-        pipeline=iris_classifier_binary,
+    model_inspector_no_interaction = cls_inspector(
+        model=learner,
         shap_interaction=False,
         explainer_factory=TreeExplainerFactory(
             feature_perturbation="tree_path_dependent", uses_background_dataset=True
         ),
         n_jobs=n_jobs,
-    ).fit(sample=iris_sample_binary)
+    ).fit(iris_sample_binary)
 
     # calculate shap interaction values
     shap_interaction_values: pd.DataFrame = model_inspector.shap_interaction_values()
 
     # calculate shap values from interaction values
     shap_values = shap_interaction_values.groupby(by="observation").sum()
 
@@ -668,32 +805,32 @@
     n_jobs: int,
 ) -> None:
     iris_classifier_dual_target = iris_classifier_selector_dual_target.best_estimator_
 
     with pytest.raises(
         ValueError,
         match=(
-            f"only single-output classifiers .* are supported.*"
+            f"only single-target classifiers .* are supported.*"
             f"{iris_target_name}.*{iris_target_name}2"
         ),
     ):
-        LearnerInspector(pipeline=iris_classifier_dual_target, n_jobs=n_jobs).fit(
-            sample=iris_sample_binary_dual_target
+        LearnerInspector(model=iris_classifier_dual_target, n_jobs=n_jobs).fit(
+            iris_sample_binary_dual_target
         )
 
 
 def test_shap_plot_data(
     iris_sample_multi_class: Sample,
     iris_inspector_multi_class: LearnerInspector[
         ClassifierPipelineDF[RandomForestClassifierDF]
     ],
 ) -> None:
     shap_plot_data = iris_inspector_multi_class.shap_plot_data()
     # noinspection SpellCheckingInspection
-    assert tuple(iris_inspector_multi_class.output_names_) == (
+    assert tuple(iris_inspector_multi_class.output_names) == (
         "setosa",
         "versicolor",
         "virginica",
     )
 
     features_shape = shap_plot_data.features.shape
     shap_values = shap_plot_data.shap_values
@@ -707,14 +844,60 @@
         shap_plot_data.features, iris_sample_multi_class.features.loc[shap_index]
     )
     assert_series_equal(
         shap_plot_data.target, iris_sample_multi_class.target.loc[shap_index]
     )
 
 
+def test_function_inspector(n_jobs: int) -> None:
+    # define a function to inspect, taking a 2D array with 3 columns as input,
+    # calculating (x1 + x2) * x3
+
+    pi2 = 2 * np.pi
+
+    def model_function(x: pd.DataFrame) -> pd.Series:
+        return np.sin(pi2 * x.x1) * np.sin(pi2 * (x.x2 + x.x3) / 2.0) + x.x4 + x.x5
+
+    # create a background dataset, with 1000 random samples
+    observations = pd.DataFrame(
+        np.random.random(size=(1000, 4)), columns=["x1", "x2", "x4", "x5"]
+    )
+    # column x3 is the same as x2
+    observations["x3"] = observations["x2"]
+    # add a column with the target values
+    observations["y"] = model_function(observations)
+    # create a sample from the background dataset
+    background = Sample(
+        observations=observations,
+        target_name="y",
+    )
+
+    # create a function inspector
+    inspector = FunctionInspector(
+        model=model_function,
+        feature_names=background.feature_names,
+        explainer_factory=ExactExplainerFactory(),
+        n_jobs=1,
+    )
+
+    # fit the inspector
+    inspector.fit(background)
+
+    # print the redundancy and synergy linkage using dendrogram drawers
+    print()
+    DendrogramDrawer(style="text").draw(
+        data=cast(LinkageTree, inspector.feature_redundancy_linkage()),
+        title="FunctionInspector (Redundancy)",
+    )
+    DendrogramDrawer(style="text").draw(
+        data=cast(LinkageTree, inspector.feature_synergy_linkage()),
+        title="FunctionInspector (Synergy)",
+    )
+
+
 #
 # Utility functions
 #
 
 
 def print_expected_matrix(error: AssertionError, *, split: bool = False) -> None:
     # print expected output for copy/paste into assertion statement
```

### Comparing `gamma-facet-2.0rc2/test/test/facet/test_partition.py` & `gamma_facet-2.1rc0/test/test/facet/test_partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 )
 
 
 def test_discrete_partitioning() -> None:
     np.random.seed(42)
 
     for _ in range(10):
-
         values = np.random.randint(
             low=0, high=10000, size=np.random.randint(low=100, high=200)
         )
 
         dvp = IntegerRangePartitioner(
             max_partitions=IntegerRangePartitioner.DEFAULT_MAX_PARTITIONS
         ).fit(values=values)
@@ -47,15 +46,14 @@
         assert dvp.frequencies_.sum() == len(values)
 
 
 def test_continuous_partitioning() -> None:
     np.random.seed(42)
 
     for _ in range(10):
-
         values = np.random.normal(
             loc=3.0, scale=8.0, size=np.random.randint(low=2000, high=4000)
         )
 
         cvp = ContinuousRangePartitioner(
             max_partitions=ContinuousRangePartitioner.DEFAULT_MAX_PARTITIONS
         ).fit(values=values)
@@ -96,15 +94,14 @@
         assert len(cp.partitions_) == len(np.unique(cp.partitions_))
         assert all(0 <= p <= 10 for p in cp.partitions_)
         for p, f in zip(cp.partitions_, cp.frequencies_):
             assert sum(values == p) == f
 
 
 def test_partition_with_invalid_values() -> None:
-
     arr_empty = np.array([])
     arr_single = np.array([1])
     arr_multi = np.array([1, 1, 1, 10, 1])
 
     with pytest.raises(
         ValueError,
         match=MSG_ARG_VALUES_EMPTY,
```

### Comparing `gamma-facet-2.0rc2/test/test/facet/test_sample.py` & `gamma_facet-2.1rc0/test/test/facet/test_sample.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/test/test/facet/test_selection.py` & `gamma_facet-2.1rc0/test/test/facet/test_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Tests for module facet.selection
 """
 import logging
-from typing import List
+from typing import Any, List, Mapping
 
 import numpy as np
 import pandas as pd
 import pytest
 from scipy.stats import randint, reciprocal
 from sklearn import datasets
 from sklearn.model_selection import GridSearchCV
@@ -36,15 +36,14 @@
 
 
 def test_learner_selector(
     regressor_parameters: List[ParameterSpace[RegressorPipelineDF[LGBMRegressorDF]]],
     sample: Sample,
     n_jobs: int,
 ) -> None:
-
     expected_scores = [
         0.669,
         0.649,
         0.493,
         0.477,
         0.464,
         0.451,
@@ -64,15 +63,15 @@
             AdaBoostRegressorDF,
             LGBMRegressorDF,
             LGBMRegressorDF,
             LGBMRegressorDF,
             LGBMRegressorDF,
         )
     ]
-    expected_parameters = {
+    expected_parameters: Mapping[int, Mapping[str, Any]] = {
         0: dict(fit_intercept=True),
         1: dict(fit_intercept=False),
         3: dict(n_estimators=80),
         4: dict(n_estimators=50),
     }
 
     # define the circular cross validator with just 5 splits (to speed up testing)
@@ -260,15 +259,15 @@
     with pytest.raises(
         TypeError,
         match=(
             r"^all parameter spaces must use the same estimator type, "
             r"but got multiple types: classifier, regressor$"
         ),
     ):
-        MultiEstimatorParameterSpace(  # type: ignore
+        MultiEstimatorParameterSpace(
             ps_1, ps_2, ParameterSpace(ClassifierPipelineDF(classifier=SVCDF()))
         )
 
     mps = MultiEstimatorParameterSpace(ps_1, ps_2)
 
     # test
 
@@ -420,15 +419,15 @@
         TypeError,
         match=(
             r"^all parameter spaces must use the same estimator type, "
             "but got multiple types: classifier, regressor$"
         ),
     ):
         # define an illegal grid list, mixing classification with regression
-        MultiEstimatorParameterSpace(ps1, ps2)  # type: ignore
+        MultiEstimatorParameterSpace(ps1, ps2)
 
     model_selector: LearnerSelector[
         ClassifierPipelineDF[RandomForestClassifierDF], GridSearchCV
     ] = LearnerSelector(
         searcher_type=GridSearchCV,
         parameter_space=ps1,
         cv=cv_stratified_bootstrap,
```

### Comparing `gamma-facet-2.0rc2/test/test/facet/test_simulation.py` & `gamma_facet-2.1rc0/test/test/facet/test_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         model=model, sample=sample, confidence_level=0.8, n_jobs=n_jobs, verbose=50
     )
 
 
 def test_univariate_target_simulation(
     target_simulator: UnivariateTargetSimulator,
 ) -> None:
-
     parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     simulation_result: UnivariateSimulationResult[
         np.float_
     ] = target_simulator.simulate_feature(
         feature_name=parameterized_feature,
@@ -131,15 +130,14 @@
         )
     )
 
 
 def test_univariate_target_subsample_simulation_80(
     model: RegressorPipelineDF[LGBMRegressorDF], subsample: Sample, n_jobs: int
 ) -> None:
-
     parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     target_simulator = UnivariateTargetSimulator(
         model=model, sample=subsample, confidence_level=0.8, n_jobs=n_jobs, verbose=50
     )
 
@@ -197,15 +195,14 @@
         )
     )
 
 
 def test_univariate_uplift_subsample_simulation_95(
     model: RegressorPipelineDF[LGBMRegressorDF], subsample: Sample, n_jobs: int
 ) -> None:
-
     parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     target_simulator = UnivariateUpliftSimulator(
         model=model, sample=subsample, confidence_level=0.95, n_jobs=n_jobs, verbose=50
     )
 
@@ -262,15 +259,14 @@
         )
     )
 
 
 def test_univariate_uplift_simulation(
     uplift_simulator: UnivariateUpliftSimulator,
 ) -> None:
-
     parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     simulation_result: UnivariateSimulationResult[
         np.float_
     ] = uplift_simulator.simulate_feature(
         feature_name=parameterized_feature,
@@ -325,15 +321,14 @@
         )
     )
 
 
 def test_univariate_uplift_subsample_simulation(
     model: RegressorPipelineDF[LGBMRegressorDF], subsample: Sample, n_jobs: int
 ) -> None:
-
     parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     uplift_simulator = UnivariateUpliftSimulator(
         model=model, sample=subsample, confidence_level=0.8, n_jobs=n_jobs, verbose=50
     )
```

### Comparing `gamma-facet-2.0rc2/test/test/facet/test_validation.py` & `gamma_facet-2.1rc0/test/test/facet/test_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
     #   - n_splits < 0
     with pytest.raises(expected_exception=ValueError):
         BootstrapCV(n_splits=-1)
 
 
 def test_get_train_test_splits_as_indices() -> None:
-
     n_test_splits = 200
     test_x = np.arange(0, 1000, 1)
 
     my_cv = BootstrapCV(n_splits=n_test_splits, random_state=42)
 
     def _generate_splits() -> List[npt.NDArray[np.int_]]:
         return [test_split for _, test_split in my_cv.split(X=test_x)]
```

### Comparing `gamma-facet-2.0rc2/tox.ini` & `gamma_facet-2.1rc0/tox.ini`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc2/PKG-INFO` & `gamma_facet-2.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamma-facet
-Version: 2.0rc2
+Version: 2.1rc0
 Summary: Human-explainable AI.
 Home-page: https://github.com/BCG-Gamma/facet
 License: Apache Software License v2.0
 Author: Boston Consulting Group (BCG)
 Requires-Python: >=3.7,<4a
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,36 +16,35 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: gamma-pytools  >=2.1rc,<3a
-Requires-Dist: matplotlib     ~=3.0
-Requires-Dist: numpy          >=1.21,<2a
-Requires-Dist: packaging      >=20
-Requires-Dist: pandas         ~=1.0
-Requires-Dist: scipy          ~=1.2
-Requires-Dist: shap           >=0.34,<0.42a
-Requires-Dist: sklearndf      >=2.2rc,<3a
+Requires-Dist: gamma-pytools     ~=2.1
+Requires-Dist: matplotlib        ~=3.0
+Requires-Dist: numpy             >=1.21,<2a
+Requires-Dist: packaging         >=20
+Requires-Dist: pandas            >=1.0
+Requires-Dist: scipy             ~=1.2
+Requires-Dist: shap              >=0.39
+Requires-Dist: scikit-learn      ~=1.0
+Requires-Dist: sklearndf         ~=2.2
+Requires-Dist: typing_extensions ~=4.0
 Requires-Dist: sphinx ~= 4.5 ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints ~= 1.19 ; extra == "docs"
 Requires-Dist: pydata-sphinx-theme ~= 0.8.1 ; extra == "docs"
 Requires-Dist: jinja2 ~= 2.11 ; extra == "docs"
 Requires-Dist: nbsphinx ~= 0.8.9 ; extra == "docs"
 Requires-Dist: jupyter == 1 ; extra == "docs"
 Requires-Dist: docutils ~= 0.17 ; extra == "docs"
 Requires-Dist: xlrd ~= 1.2 ; extra == "docs"
 Requires-Dist: m2r ~= 0.2 ; extra == "docs"
 Requires-Dist: pytest ~= 7.1 ; extra == "testing"
 Requires-Dist: pytest-cov ~= 2.12 ; extra == "testing"
-Requires-Dist: flake8 ~= 3.8 ; extra == "testing"
-Requires-Dist: flake8-comprehensions ~= 3.2 ; extra == "testing"
-Requires-Dist: isort ~= 5.10 ; extra == "testing"
 Requires-Dist: lightgbm ~=3.0.0 ; extra == "testing"
 Requires-Dist: xgboost ~= 1.5 ; extra == "testing"
 Project-URL: Documentation, https://bcg-gamma.github.io/facet/
 Project-URL: Repository, https://github.com/BCG-Gamma/facet
 Provides-Extra: docs
 Provides-Extra: testing
```

