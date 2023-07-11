# Comparing `tmp/gamma_facet-2.1.0.tar.gz` & `tmp/gamma_facet-2.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamma_facet-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamma_facet-2.1rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamma_facet-2.1.0.tar` & `gamma_facet-2.1rc0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0      666 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      689 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     4886 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/.gitignore
--rw-r--r--   0        0        0     1103 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/LICENSE
--rw-r--r--   0        0        0    21630 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/README.rst
--rw-r--r--   0        0        0     8656 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/RELEASE_NOTES.rst
--rw-r--r--   0        0        0    26862 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/azure-pipelines.yml
--rw-r--r--   0        0        0     2555 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/condabuild/meta.yaml
--rw-r--r--   0        0        0        0 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/config/spelling.dic
--rw-r--r--   0        0        0      124 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/config/test_config.yml
--rwxr-xr-x   0        0        0       93 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/dev-setup.sh
--rw-r--r--   0        0        0      873 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/environment.yml
--rwxr-xr-x   0        0        0      380 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/make.py
--rw-r--r--   0        0        0      663 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/mypy.ini
--rw-r--r--   0        0        0     2717 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/pypi_description.rst
--rw-r--r--   0        0        0     4083 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-11 16:34:09.958064 gamma_facet-2.1.0/sphinx/.gitignore
--rw-r--r--   0        0        0   199625 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/auxiliary/Diabetes_getting_started_example.ipynb
--rw-r--r--   0        0        0    10223 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb
--rwxr-xr-x   0        0        0      664 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/make.py
--rw-r--r--   0        0        0   130308 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/source/_images/Facet-Simulator-BlockDiagram.png
--rw-r--r--   0        0        0    19522 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/source/_images/Facet_Logo_Plain.png
--rw-r--r--   0        0        0     5238 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/source/_images/Facet_flow.svg
--rw-r--r--   0        0        0     7117 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg
--rw-r--r--   0        0        0    23632 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/source/_images/facet_banner.png
--rw-r--r--   0        0        0     1429 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/source/_images/icons/inspect_icon.png
--rw-r--r--   0        0        0     2777 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/source/_images/icons/pipe_icon.png
--rw-r--r--   0        0        0     2718 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/source/_images/icons/sim_icon.png
--rw-r--r--   0        0        0   117900 2023-07-11 16:34:09.970064 gamma_facet-2.1.0/sphinx/source/_images/ranker_summary.png
--rw-r--r--   0        0        0    27724 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/redundancy_dendrogram.png
--rw-r--r--   0        0        0    31712 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/redundancy_matrix.png
--rw-r--r--   0        0        0    38185 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/simulation_output.png
--rw-r--r--   0        0        0    31278 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/synergy_matrix.png
--rw-r--r--   0        0        0    49407 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Andy_Shora.jpg
--rw-r--r--   0        0        0     9901 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Florent_Martin.jpg
--rw-r--r--   0        0        0    11856 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Jan_Ittner.jpg
--rw-r--r--   0        0        0     8047 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Jason_Bentley.jpg
--rw-r--r--   0        0        0    10116 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg
--rw-r--r--   0        0        0     6673 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg
--rw-r--r--   0        0        0     9583 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Malo_Grisard.jpg
--rw-r--r--   0        0        0    49773 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg
--rw-r--r--   0        0        0    10100 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg
--rw-r--r--   0        0        0    10746 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg
--rw-r--r--   0        0        0      232 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/_static/css/facet.css
--rw-r--r--   0        0        0     3673 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/about_us.rst
--rw-r--r--   0        0        0      371 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/api_landing.rst
--rw-r--r--   0        0        0      758 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/conf.py
--rw-r--r--   0        0        0    20763 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/contribution_guide.rst
--rw-r--r--   0        0        0     5693 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/faqs.rst
--rw-r--r--   0        0        0      298 2023-07-11 16:34:09.974065 gamma_facet-2.1.0/sphinx/source/index.rst
--rw-r--r--   0        0        0  1644442 2023-07-11 16:34:09.986065 gamma_facet-2.1.0/sphinx/source/tutorial/Classification_with_Facet.ipynb
--rw-r--r--   0        0        0   970457 2023-07-11 16:34:09.990065 gamma_facet-2.1.0/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv
--rw-r--r--   0        0        0   232448 2023-07-11 16:34:09.994065 gamma_facet-2.1.0/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb
--rw-r--r--   0        0        0   107691 2023-07-11 16:34:09.994065 gamma_facet-2.1.0/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb
--rw-r--r--   0        0        0   475484 2023-07-11 16:34:09.998065 gamma_facet-2.1.0/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb
--rw-r--r--   0        0        0   820532 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/sphinx/source/tutorial/pre_diab_nhanes.csv
--rw-r--r--   0        0        0    85389 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/sphinx/source/tutorial/water_drilling_classification_data.csv
--rw-r--r--   0        0        0     2402 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/sphinx/source/tutorials.rst
--rw-r--r--   0        0        0      600 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/__init__.py
--rw-r--r--   0        0        0      582 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/_types.py
--rw-r--r--   0        0        0      102 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/data/__init__.py
--rw-r--r--   0        0        0    11804 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/data/_sample.py
--rw-r--r--   0        0        0      272 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/data/partition/__init__.py
--rw-r--r--   0        0        0    14160 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/data/partition/_partition.py
--rw-r--r--   0        0        0      306 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/explanation/__init__.py
--rw-r--r--   0        0        0    13800 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/explanation/_explanation.py
--rw-r--r--   0        0        0      708 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/explanation/_types.py
--rw-r--r--   0        0        0       89 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/explanation/base/__init__.py
--rw-r--r--   0        0        0     7935 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/explanation/base/_base.py
--rw-r--r--   0        0        0      119 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/explanation/parallel/__init__.py
--rw-r--r--   0        0        0     9169 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/explanation/parallel/_parallel.py
--rw-r--r--   0        0        0      403 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/_explainer.py
--rw-r--r--   0        0        0     4840 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/_function_inspector.py
--rw-r--r--   0        0        0     1910 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/_inspection.py
--rw-r--r--   0        0        0    15774 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/_learner_inspector.py
--rw-r--r--   0        0        0    19115 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/_shap_context.py
--rw-r--r--   0        0        0    15090 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/_shap_projection.py
--rw-r--r--   0        0        0       85 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/base/__init__.py
--rw-r--r--   0        0        0    38123 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/base/_model_inspector.py
--rw-r--r--   0        0        0       93 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/shap/__init__.py
--rw-r--r--   0        0        0     1922 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/shap/_function.py
--rw-r--r--   0        0        0    15295 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/shap/_shap.py
--rw-r--r--   0        0        0       97 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/shap/sklearn/__init__.py
--rw-r--r--   0        0        0    11266 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/inspection/shap/sklearn/_sklearn.py
--rw-r--r--   0        0        0        0 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/py.typed
--rw-r--r--   0        0        0      113 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/selection/__init__.py
--rw-r--r--   0        0        0    13220 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/selection/_parameters.py
--rw-r--r--   0        0        0    17458 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/selection/_selection.py
--rw-r--r--   0        0        0      107 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/selection/base/__init__.py
--rw-r--r--   0        0        0     7870 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/selection/base/_parameters.py
--rw-r--r--   0        0        0      318 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/simulation/__init__.py
--rw-r--r--   0        0        0     5469 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/simulation/_result.py
--rw-r--r--   0        0        0     9103 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/simulation/_simulation.py
--rw-r--r--   0        0        0       58 2023-07-11 16:34:10.002065 gamma_facet-2.1.0/src/facet/simulation/base/__init__.py
--rw-r--r--   0        0        0     9564 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/src/facet/simulation/base/_base.py
--rw-r--r--   0        0        0       95 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/src/facet/simulation/viz/__init__.py
--rw-r--r--   0        0        0     4244 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/src/facet/simulation/viz/_draw.py
--rw-r--r--   0        0        0    12875 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/src/facet/simulation/viz/_style.py
--rw-r--r--   0        0        0      125 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/src/facet/validation/__init__.py
--rw-r--r--   0        0        0     9261 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/src/facet/validation/_validation.py
--rw-r--r--   0        0        0        0 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/__init__.py
--rw-r--r--   0        0        0    14736 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/conftest.py
--rw-r--r--   0        0        0        0 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/facet/__init__.py
--rw-r--r--   0        0        0    31524 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/facet/test_inspection.py
--rw-r--r--   0        0        0     4348 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/facet/test_partition.py
--rw-r--r--   0        0        0     5085 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/facet/test_sample.py
--rw-r--r--   0        0        0    14037 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/facet/test_selection.py
--rw-r--r--   0        0        0     2309 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/facet/test_shap_decomposition.py
--rw-r--r--   0        0        0    13495 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/facet/test_simulation.py
--rw-r--r--   0        0        0     5523 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/facet/test_validation.py
--rw-r--r--   0        0        0      263 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/paths.py
--rw-r--r--   0        0        0      216 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/test/test/test_docs.py
--rw-r--r--   0        0        0     2594 2023-07-11 16:34:10.006065 gamma_facet-2.1.0/tox.ini
--rw-r--r--   0        0        0     4851 1970-01-01 00:00:00.000000 gamma_facet-2.1.0/PKG-INFO
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

### Comparing `gamma_facet-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `gamma_facet-2.1rc0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `gamma_facet-2.1rc0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/.gitignore` & `gamma_facet-2.1rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/.pre-commit-config.yaml` & `gamma_facet-2.1rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/LICENSE` & `gamma_facet-2.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/README.rst` & `gamma_facet-2.1rc0/README.rst`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/RELEASE_NOTES.rst` & `gamma_facet-2.1rc0/RELEASE_NOTES.rst`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/azure-pipelines.yml` & `gamma_facet-2.1rc0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/condabuild/meta.yaml` & `gamma_facet-2.1rc0/condabuild/meta.yaml`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/environment.yml` & `gamma_facet-2.1rc0/environment.yml`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/mypy.ini` & `gamma_facet-2.1rc0/mypy.ini`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/pypi_description.rst` & `gamma_facet-2.1rc0/pypi_description.rst`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/pyproject.toml` & `gamma_facet-2.1rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/auxiliary/Diabetes_getting_started_example.ipynb` & `gamma_facet-2.1rc0/sphinx/auxiliary/Diabetes_getting_started_example.ipynb`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb` & `gamma_facet-2.1rc0/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/make.py` & `gamma_facet-2.1rc0/sphinx/make.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/Facet-Simulator-BlockDiagram.png` & `gamma_facet-2.1rc0/sphinx/source/_images/Facet-Simulator-BlockDiagram.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/Facet_Logo_Plain.png` & `gamma_facet-2.1rc0/sphinx/source/_images/Facet_Logo_Plain.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/Facet_flow.svg` & `gamma_facet-2.1rc0/sphinx/source/_images/Facet_flow.svg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg` & `gamma_facet-2.1rc0/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/facet_banner.png` & `gamma_facet-2.1rc0/sphinx/source/_images/facet_banner.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/icons/inspect_icon.png` & `gamma_facet-2.1rc0/sphinx/source/_images/icons/inspect_icon.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/icons/pipe_icon.png` & `gamma_facet-2.1rc0/sphinx/source/_images/icons/pipe_icon.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/icons/sim_icon.png` & `gamma_facet-2.1rc0/sphinx/source/_images/icons/sim_icon.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/ranker_summary.png` & `gamma_facet-2.1rc0/sphinx/source/_images/ranker_summary.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/redundancy_dendrogram.png` & `gamma_facet-2.1rc0/sphinx/source/_images/redundancy_dendrogram.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/redundancy_matrix.png` & `gamma_facet-2.1rc0/sphinx/source/_images/redundancy_matrix.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/simulation_output.png` & `gamma_facet-2.1rc0/sphinx/source/_images/simulation_output.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/synergy_matrix.png` & `gamma_facet-2.1rc0/sphinx/source/_images/synergy_matrix.png`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Andy_Shora.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Andy_Shora.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Florent_Martin.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Florent_Martin.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Jan_Ittner.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Jan_Ittner.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Jason_Bentley.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Jason_Bentley.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Malo_Grisard.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Malo_Grisard.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg` & `gamma_facet-2.1rc0/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/about_us.rst` & `gamma_facet-2.1rc0/sphinx/source/about_us.rst`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/conf.py` & `gamma_facet-2.1rc0/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/contribution_guide.rst` & `gamma_facet-2.1rc0/sphinx/source/contribution_guide.rst`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/faqs.rst` & `gamma_facet-2.1rc0/sphinx/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/tutorial/Classification_with_Facet.ipynb` & `gamma_facet-2.1rc0/sphinx/source/tutorial/Classification_with_Facet.ipynb`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv` & `gamma_facet-2.1rc0/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb` & `gamma_facet-2.1rc0/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb` & `gamma_facet-2.1rc0/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb` & `gamma_facet-2.1rc0/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/tutorial/pre_diab_nhanes.csv` & `gamma_facet-2.1rc0/sphinx/source/tutorial/pre_diab_nhanes.csv`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/tutorial/water_drilling_classification_data.csv` & `gamma_facet-2.1rc0/sphinx/source/tutorial/water_drilling_classification_data.csv`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/sphinx/source/tutorials.rst` & `gamma_facet-2.1rc0/sphinx/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/__init__.py` & `gamma_facet-2.1rc0/src/facet/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Human-explainable AI.
 
 This is the class and function reference of FACET for advanced model selection,
 inspection, and simulation.
 """
 
 
-__version__ = "2.1.0"
+__version__ = "2.1rc0"
 
 __logo__ = (
     r"""
     _         ____    _                         _       ___        __   ___ _____
  _-´ _-      / ___\  / \    /\  /\   /\  /\    / \     |     /\   /  ` |      |
 | ,-´ , |   | | __  / _ \  /  \/  \ /  \/  \  / _ \    |___ /  \ |     |__    |
 | | | | |   | |_] |/ ___ \/ /\  /\ \ /\  /\ \/ ___ \   |   /----\|     |      |
```

### Comparing `gamma_facet-2.1.0/src/facet/_types.py` & `gamma_facet-2.1rc0/src/facet/_types.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/data/_sample.py` & `gamma_facet-2.1rc0/src/facet/data/_sample.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/data/partition/_partition.py` & `gamma_facet-2.1rc0/src/facet/data/partition/_partition.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/explanation/_explanation.py` & `gamma_facet-2.1rc0/src/facet/explanation/_explanation.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/explanation/_types.py` & `gamma_facet-2.1rc0/src/facet/explanation/_types.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/explanation/base/_base.py` & `gamma_facet-2.1rc0/src/facet/explanation/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/explanation/parallel/_parallel.py` & `gamma_facet-2.1rc0/src/facet/explanation/parallel/_parallel.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/inspection/_function_inspector.py` & `gamma_facet-2.1rc0/src/facet/inspection/_function_inspector.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/inspection/_inspection.py` & `gamma_facet-2.1rc0/src/facet/inspection/_inspection.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/inspection/_learner_inspector.py` & `gamma_facet-2.1rc0/src/facet/inspection/_learner_inspector.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/inspection/_shap_context.py` & `gamma_facet-2.1rc0/src/facet/inspection/_shap_context.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/inspection/_shap_projection.py` & `gamma_facet-2.1rc0/src/facet/inspection/_shap_projection.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/inspection/base/_model_inspector.py` & `gamma_facet-2.1rc0/src/facet/inspection/base/_model_inspector.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/inspection/shap/_function.py` & `gamma_facet-2.1rc0/src/facet/inspection/shap/_function.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/inspection/shap/_shap.py` & `gamma_facet-2.1rc0/src/facet/inspection/shap/_shap.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/inspection/shap/sklearn/_sklearn.py` & `gamma_facet-2.1rc0/src/facet/inspection/shap/sklearn/_sklearn.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/selection/_parameters.py` & `gamma_facet-2.1rc0/src/facet/selection/_parameters.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/selection/_selection.py` & `gamma_facet-2.1rc0/src/facet/selection/_selection.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/selection/base/_parameters.py` & `gamma_facet-2.1rc0/src/facet/selection/base/_parameters.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/simulation/_result.py` & `gamma_facet-2.1rc0/src/facet/simulation/_result.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/simulation/_simulation.py` & `gamma_facet-2.1rc0/src/facet/simulation/_simulation.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/simulation/base/_base.py` & `gamma_facet-2.1rc0/src/facet/simulation/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/simulation/viz/_draw.py` & `gamma_facet-2.1rc0/src/facet/simulation/viz/_draw.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/simulation/viz/_style.py` & `gamma_facet-2.1rc0/src/facet/simulation/viz/_style.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/src/facet/validation/_validation.py` & `gamma_facet-2.1rc0/src/facet/validation/_validation.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/test/test/conftest.py` & `gamma_facet-2.1rc0/test/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/test/test/facet/test_inspection.py` & `gamma_facet-2.1rc0/test/test/facet/test_inspection.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/test/test/facet/test_partition.py` & `gamma_facet-2.1rc0/test/test/facet/test_partition.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/test/test/facet/test_sample.py` & `gamma_facet-2.1rc0/test/test/facet/test_sample.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/test/test/facet/test_selection.py` & `gamma_facet-2.1rc0/test/test/facet/test_selection.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/test/test/facet/test_shap_decomposition.py` & `gamma_facet-2.1rc0/test/test/facet/test_shap_decomposition.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/test/test/facet/test_simulation.py` & `gamma_facet-2.1rc0/test/test/facet/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/test/test/facet/test_validation.py` & `gamma_facet-2.1rc0/test/test/facet/test_validation.py`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/tox.ini` & `gamma_facet-2.1rc0/tox.ini`

 * *Files identical despite different names*

### Comparing `gamma_facet-2.1.0/PKG-INFO` & `gamma_facet-2.1rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamma-facet
-Version: 2.1.0
+Version: 2.1rc0
 Summary: Human-explainable AI.
 Home-page: https://github.com/BCG-Gamma/facet
 License: Apache Software License v2.0
 Author: Boston Consulting Group (BCG)
 Requires-Python: >=3.7,<4a
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
```

