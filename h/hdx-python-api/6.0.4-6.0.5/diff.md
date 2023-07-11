# Comparing `tmp/hdx_python_api-6.0.4.tar.gz` & `tmp/hdx_python_api-6.0.5.tar.gz`

## Comparing `hdx_python_api-6.0.4.tar` & `hdx_python_api-6.0.5.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0    42394 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/documentation/main.md
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/_version.py
--rwxr-xr-x   0        0        0    24988 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/configuration.py
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/hdx_base_configuration.yaml
--rwxr-xr-x   0        0        0     4540 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/api/locations.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/__init__.py
--rwxr-xr-x   0        0        0   111985 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/dataset.py
--rwxr-xr-x   0        0        0     9458 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/dataset_title_helper.py
--rwxr-xr-x   0        0        0     5798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/date_helper.py
--rwxr-xr-x   0        0        0     3545 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/filestore_helper.py
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0    28599 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/hdxobject.py
--rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/indicator_resource_view_template.yaml
--rwxr-xr-x   0        0        0    11098 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/organization.py
--rwxr-xr-x   0        0        0    24275 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/resource.py
--rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/resource_matcher.py
--rwxr-xr-x   0        0        0     7679 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/resource_view.py
--rwxr-xr-x   0        0        0    15005 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/showcase.py
--rwxr-xr-x   0        0        0     9686 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/user.py
--rwxr-xr-x   0        0        0    22495 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/data/vocabulary.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/facades/infer_arguments.py
--rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/facades/keyword_arguments.py
--rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/src/hdx/facades/simple.py
--rwxr-xr-x   0        0        0     6147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/Accepted_Tags.csv
--rwxr-xr-x   0        0        0   169336 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/Tag_Mapping.csv
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/Tag_Mapping_ChainRuleError.csv
--rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/dataset_search_results.yaml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/empty.csv
--rwxr-xr-x   0        0        0    13842 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/organization_show_results.yaml
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/resource_formats.json
--rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/showcase_all_search_results.yaml
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/test_data.zip
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/empty.yaml
--rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_base_config.json
--rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_base_config.yaml
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_config.yaml
--rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_dataset_static.json
--rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_dataset_static.yaml
--rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_datasource_topline.json
--rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_email_configuration.yaml
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_missing_site_config.json
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_organization_static.json
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_organization_static.yaml
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_static.json
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_static.yaml
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_view_static.json
--rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_view_static.yaml
--rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_showcase_static.json
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_showcase_static.yaml
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_user_static.json
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_user_static.yaml
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_vocabulary_static.json
--rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/hdx_vocabulary_static.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/project_configuration.yaml
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/user_agent_config.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/user_agent_config2.yaml
--rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/user_agent_config3.yaml
--rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/config/user_agent_config_wrong.yaml
--rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
--rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/conflict_data_alg.csv
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/test_data_no_data.csv
--rwxr-xr-x   0        0        0     1534 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/gen_resource/test_data_no_years.csv
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
--rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
--rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
--rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
--rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   842238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
--rw-r--r--   0        0        0    48523 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/unesco_dataset.json
--rw-r--r--   0        0        0    38434 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
--rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_logic/update_logic_resources.yaml
--rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/fixtures/update_logic/update_logic_resources_new.yaml
--rwxr-xr-x   0        0        0    44945 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/conftest.py
--rwxr-xr-x   0        0        0    34761 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/api/test_configuration.py
--rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/api/test_locations.py
--rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/__init__.py
--rwxr-xr-x   0        0        0    49155 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_dataset_core.py
--rwxr-xr-x   0        0        0    75535 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_dataset_noncore.py
--rwxr-xr-x   0        0        0    11869 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_dataset_title_helper.py
--rwxr-xr-x   0        0        0    19578 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_organization.py
--rwxr-xr-x   0        0        0    45959 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_resource.py
--rwxr-xr-x   0        0        0    19114 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_resource_view.py
--rwxr-xr-x   0        0        0    23055 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_showcase.py
--rw-r--r--   0        0        0    10125 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_update_dataset_resources.py
--rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_update_logic.py
--rwxr-xr-x   0        0        0    21181 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_user.py
--rwxr-xr-x   0        0        0   116076 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/data/test_vocabulary.py
--rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/facades/test_infer_arguments.py
--rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/facades/test_keyword_arguments.py
--rwxr-xr-x   0        0        0     5650 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/tests/hdx/facades/test_simple.py
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/workingexample/my_code.py
--rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/workingexample/my_resource.csv
--rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/workingexample/my_resource.xlsx
--rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/workingexample/run.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/LICENSE
--rwxr-xr-x   0        0        0     1307 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/README.md
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/pyproject.toml
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 hdx_python_api-6.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    43789 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/documentation/main.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/_version.py
+-rwxr-xr-x   0        0        0    24988 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/configuration.py
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/hdx_base_configuration.yaml
+-rwxr-xr-x   0        0        0     4540 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/api/locations.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0   112228 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/dataset.py
+-rwxr-xr-x   0        0        0     9458 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/dataset_title_helper.py
+-rwxr-xr-x   0        0        0     5798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/date_helper.py
+-rwxr-xr-x   0        0        0     3770 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/filestore_helper.py
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0    28580 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/hdxobject.py
+-rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/indicator_resource_view_template.yaml
+-rwxr-xr-x   0        0        0    11098 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/organization.py
+-rwxr-xr-x   0        0        0    26488 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/resource.py
+-rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/resource_matcher.py
+-rwxr-xr-x   0        0        0     7679 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/resource_view.py
+-rwxr-xr-x   0        0        0    15005 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/showcase.py
+-rwxr-xr-x   0        0        0     9686 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/user.py
+-rwxr-xr-x   0        0        0    22495 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/data/vocabulary.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/facades/infer_arguments.py
+-rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/facades/keyword_arguments.py
+-rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/src/hdx/facades/simple.py
+-rwxr-xr-x   0        0        0     6147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/Accepted_Tags.csv
+-rwxr-xr-x   0        0        0   169336 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/Tag_Mapping.csv
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/Tag_Mapping_ChainRuleError.csv
+-rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/dataset_search_results.yaml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/empty.csv
+-rwxr-xr-x   0        0        0    13842 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/organization_show_results.yaml
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/resource_formats.json
+-rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/showcase_all_search_results.yaml
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/test_data.zip
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_base_config.json
+-rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_base_config.yaml
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_dataset_static.json
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_dataset_static.yaml
+-rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_datasource_topline.json
+-rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_email_configuration.yaml
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_missing_site_config.json
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_organization_static.json
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_organization_static.yaml
+-rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_static.json
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_static.yaml
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_view_static.json
+-rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_view_static.yaml
+-rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_showcase_static.json
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_showcase_static.yaml
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_user_static.json
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_user_static.yaml
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_vocabulary_static.json
+-rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/hdx_vocabulary_static.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
+-rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/test_data_no_data.csv
+-rwxr-xr-x   0        0        0     1534 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/gen_resource/test_data_no_years.csv
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
+-rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
+-rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
+-rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
+-rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   842238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
+-rw-r--r--   0        0        0    48523 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/unesco_dataset.json
+-rw-r--r--   0        0        0    38434 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
+-rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_logic/update_logic_resources.yaml
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/fixtures/update_logic/update_logic_resources_new.yaml
+-rwxr-xr-x   0        0        0    45085 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0    34761 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/api/test_configuration.py
+-rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/api/test_locations.py
+-rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0    49383 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_dataset_core.py
+-rwxr-xr-x   0        0        0    75535 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_dataset_noncore.py
+-rwxr-xr-x   0        0        0    11869 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_dataset_title_helper.py
+-rwxr-xr-x   0        0        0    19578 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_organization.py
+-rwxr-xr-x   0        0        0    46355 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_resource.py
+-rwxr-xr-x   0        0        0    19114 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_resource_view.py
+-rwxr-xr-x   0        0        0    23055 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_showcase.py
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_update_dataset_resources.py
+-rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_update_logic.py
+-rwxr-xr-x   0        0        0    21181 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_user.py
+-rwxr-xr-x   0        0        0   116076 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/data/test_vocabulary.py
+-rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/facades/test_infer_arguments.py
+-rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/facades/test_keyword_arguments.py
+-rwxr-xr-x   0        0        0     5650 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/tests/hdx/facades/test_simple.py
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/workingexample/my_code.py
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/workingexample/my_resource.csv
+-rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/workingexample/my_resource.xlsx
+-rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/workingexample/run.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/LICENSE
+-rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/README.md
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hdx_python_api-6.0.5/PKG-INFO
```

### Comparing `hdx_python_api-6.0.4/CONTRIBUTING.md` & `hdx_python_api-6.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/requirements.txt` & `hdx_python_api-6.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/.config/pre-commit-config.yaml` & `hdx_python_api-6.0.5/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/.github/workflows/publish.yaml` & `hdx_python_api-6.0.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/.github/workflows/run-python-tests.yaml` & `hdx_python_api-6.0.5/.github/workflows/run-python-tests.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This workflow will install Python dependencies, lint and run tests
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Run tests
 
 on:
+  workflow_dispatch: # add run button in github
   push:
     branches-ignore:
       - gh-pages
   pull_request:
     branches-ignore:
       - gh-pages
```

### Comparing `hdx_python_api-6.0.4/documentation/main.md` & `hdx_python_api-6.0.5/documentation/main.md`

 * *Files 5% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 4. Scroll down to the bottom of the profile page
 5. Copy the API key which will be of the form: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
 6. You can either:
 
     a.  Pass this key as a parameter or within a dictionary
     
     b.  Create a JSON or YAML file. The default path is
-            **.hdx\_configuration.yaml** in the current user's home
+            **.hdx_configuration.yaml** in the current user's home
             directory. Then put in the YAML file:
 
             hdx_key: "HDX API KEY"
 
 ## Installing the Library
 
 To include the HDX Python library in your project, you must **pip install** or add to 
@@ -199,24 +199,25 @@
 8. Setup logging
 
         setup_logging()
 
 9. Use configuration defaults.
 
     If you only want to read data, then connect to the production HDX
-    server, replacing A_Quick_Example with something short that describes your project:
+    server, making sure that you replace MyOrg_MyProject with something that 
+    describes your organisation and project:
 
-        Configuration.create(hdx_site="prod", user_agent="A_Quick_Example", hdx_read_only=True)
+        Configuration.create(hdx_site="prod", user_agent="MyOrg_MyProject", hdx_read_only=True)
 
     If you want to write data, then for experimentation, do not use the
     production HDX server. Instead you can use one of the test servers.
     Assuming you have an API key stored in a file **.hdxkey** in the
     current user's home directory:
 
-        Configuration.create(hdx_site="stage", user_agent="A_Quick_Example")
+        Configuration.create(hdx_site="stage", user_agent="MyOrg_MyProject")
 
 10. Read this dataset 
 [Novel Coronavirus (COVID-19) Cases Data](https://data.humdata.org/dataset/novel-coronavirus-2019-ncov-cases)
      from HDX and view the date of the dataset:
 
         dataset = Dataset.read_from_hdx("novel-coronavirus-2019-ncov-cases")
         print(dataset.get_reference_period())
@@ -243,15 +244,30 @@
         dataset.update_in_hdx()
 
 14. You can view it on HDX before changing it back (if you have an API key):
 
         dataset.set_reference_period("PREVIOUS DATE")
         dataset.update_in_hdx()
 
-15. Exit and remove virtualenv:
+15. If you are storing your data on HDX, you can upload a new file to a 
+    resource:
+
+        resource = dataset.get_resource(0)
+        resource.set_file_to_upload("PATH TO FILE")
+        resource.update_in_hdx()
+
+16. Alternatively, if you are using a URL to point to data held externally from
+    HDX, you can mark that the data has been updated before updating the
+    resource or parent dataset:
+
+        resource = dataset.get_resource(2)
+        resource.mark_data_updated()
+        dataset.update_in_hdx()
+
+17. Exit and remove virtualenv:
 
         exit()
         deactivate
 
      On Windows:
 
         rd /s /q test
@@ -266,15 +282,15 @@
 
 The easiest way to get started is to use the facades and configuration defaults. The 
 facades set up both logging and HDX configuration.
 
 The default configuration loads an internal HDX configuration located within the 
 library, and assumes that there is an API key file called **.hdxkey** in the current 
 user's home directory **\~** and a YAML project configuration located relative to your 
-working directory at **config/project\_configuration.yaml** which you must create. The 
+working directory at **config/project_configuration.yaml** which you must create. The 
 project configuration is used for any configuration specific to your project.
 
 The default logging configuration reads a configuration file internal to the library 
 that sets up an coloured console handler outputting at INFO level and a file handler 
 writing to errors.log at ERROR level.
 
 ## Facades
@@ -331,42 +347,43 @@
 
     from hdx.api.configuration import Configuration
     ...
     Configuration.create([configuration], [user_agent], [user_agent_config_yaml], [remoteckan], KEYWORD ARGUMENTS)
 
 You must supply a user agent using one of the following approaches:
 
-1. Populate parameter **user\_agent** (which can simply be the name of your project)
-2. Supply **user\_agent\_config\_yaml** which should point to a YAML file which 
-contains a parameter **user\_agent**
-3. Supply **user\_agent\_config\_yaml** which should point to a YAML file and populate 
-**user\_agent\_lookup** which is a key to look up in the YAML file which should be of 
-form:
+1. Populate parameter **user_agent** (which should be the name of your 
+organisation and project)
+2. Supply **user_agent_config_yaml** which should point to a YAML file which 
+contains a parameter **user_agent**
+3. Supply **user_agent_config_yaml** which should point to a YAML file and populate
+**user_agent_lookup** which is a key to look up in the YAML file which should 
+be of form:
 
         myproject:
             user_agent: test
         myproject2:
             user_agent: test2
 
-4. Include **user\_agent** in one of the configuration dictionaries or files outlined in 
+4. Include **user_agent** in one of the configuration dictionaries or files outlined in 
 the table below eg. 
-    **hdx\_config\_json** or **project\_config\_dict**.
+    **hdx_config_json** or **project_config_dict**.
 
 **KEYWORD ARGUMENTS** can be:
 
 |Choose|Argument|Type|Value|Default|
 |---|---|---|---|---|
-| |hdx\_site|Optional\[str\]|HDX site to use eg. prod, feature|test|
-| |hdx\_read\_only|bool|Read only or read/write access to HDX|False|
-| |hdx\_key|Optional\[str\]|HDX key (not needed for read only)||
-|Above or one of:|hdx\_config\_dict|dict|Dictionary with hdx\_site, hdx\_read\_only, hdx\_key||
-|or|hdx\_config\_json|str|Path to JSON configuration with values as above||
-|or|hdx\_config\_yaml|str|Path to YAML configuration with values as above||
-|Zero or one of:|project\_config\_dict|dict|Project specific configuration dictionary||
-|or|project\_config\_json|str|Path to JSON Project||
+| |hdx_site|Optional\[str\]|HDX site to use eg. prod, feature|test|
+| |hdx_read_only|bool|Read only or read/write access to HDX|False|
+| |hdx_key|Optional\[str\]|HDX key (not needed for read only)||
+|Above or one of:|hdx_config_dict|dict|Dictionary with hdx_site, hdx_read_only, hdx_key||
+|or|hdx_config_json|str|Path to JSON configuration with values as above||
+|or|hdx_config_yaml|str|Path to YAML configuration with values as above||
+|Zero or one of:|project_config_dict|dict|Project specific configuration dictionary||
+|or|project_config_json|str|Path to JSON Project||
 
 To access the configuration, you use the **read** method of the **Configuration** class as follows:
 
     Configuration.read()
 
 For more advanced users, there are methods to allow you to pass in your own 
 configuration object, remote CKAN object and list of valid locations. See the API 
@@ -379,15 +396,15 @@
     configuration.setup_remoteckan(REMOTE CKAN OBJECT)
     configuration.setup_validlocations(LIST OF VALID LOCATIONS)
     dataset = Dataset(configuration=configuration)
 
 ## Configuring Logging
 
 If you use a facade from **hdx.facades**, then logging will go to console and errors to 
-file. If you are not using a facade, you can call **setup\_logging**  which takes 
+file. If you are not using a facade, you can call **setup_logging**  which takes 
 an argument error_file which is False by default. If set to True, errors will be written
 to a file.
 
 If not using facade:
 
     from hdx.utilities.easy_logging import setup_logging
     ...
@@ -405,21 +422,21 @@
     logger.info("INFORMATION message")
     logger.warning("WARNING message")
     logger.error("ERROR message")
     logger.critical("CRITICAL error message")
 
 ## Operations on HDX Objects
 
-You can read an existing HDX object with the static **read\_from\_hdx** method 
+You can read an existing HDX object with the static **read_from_hdx** method 
 which takes an identifier parameter and returns the an object of the appropriate HDX 
 object type eg. **Dataset** or **None** depending upon whether the object was read eg.
 
     dataset = Dataset.read_from_hdx("DATASET_ID_OR_NAME")
 
-You can search for datasets and resources in HDX using the **search\_in\_hdx** method 
+You can search for datasets and resources in HDX using the **search_in_hdx** method 
 which takes a query parameter and returns the a list of objects of the appropriate HDX 
 object type eg. **list[Dataset]**. Here is an example:
 
     datasets = Dataset.search_in_hdx("QUERY", **kwargs)
 
 The query parameter takes a different format depending upon whether it is for a
 [dataset](https://docs.ckan.org/en/latest/api/index.html#ckan.logic.action.get.package_search)
@@ -460,17 +477,17 @@
 Larger amounts of static metadata are best added from files. YAML is very human readable 
 and recommended, while JSON is also accepted eg.
 
     dataset.update_from_yaml([path])
 
     dataset.update_from_json([path])
 
-The default path if unspecified is **config/hdx\_TYPE\_static.yaml** for YAML and
-**config/hdx\_TYPE\_static.json** for JSON where TYPE is an HDX object's type like 
-dataset or resource eg. **config/hdx\_showcase\_static.json**. The YAML file takes the 
+The default path if unspecified is **config/hdx_TYPE_static.yaml** for YAML and
+**config/hdx_TYPE_static.json** for JSON where TYPE is an HDX object's type like 
+dataset or resource eg. **config/hdx_showcase_static.json**. The YAML file takes the 
 following form:
 
     owner_org: "acled"
     maintainer: "acled"
     ...
     tags:
         - name: "violence and conflict"
@@ -481,97 +498,99 @@
           format: "xlsx"
     ...
 
 Notice how you can define resources (each resource starts with a dash "-") within the 
 file as shown above.
 
 You can check if all the fields required by HDX are populated by 
-calling **check\_required\_fields**. This will throw an exception if any fields are 
+calling **check_required_fields**. This will throw an exception if any fields are 
 missing. Before the library posts data to HDX, it will call this method automatically. 
 You can provide a list of fields to ignore in the check. An example usage:
 
     resource.check_required_fields([ignore_fields])
 
 Once the HDX object is ready ie. it has all the required metadata, you simply 
-call **create\_in\_hdx** eg.
+call **create_in_hdx** eg.
 
     dataset.create_in_hdx(allow_no_resources, update_resources,
                           update_resources_by_name,
                           remove_additional_resources)
 
-Existing HDX objects can be updated by calling **update\_in\_hdx** eg.
+If the object already exists, it will be updated. You can also update
+explicitly by calling **update_in_hdx** eg.
 
     dataset.update_in_hdx(update_resources, update_resources_by_name,
                           remove_additional_resources)
 
-You can delete HDX objects using **delete\_from\_hdx** and update an object that 
-already exists in HDX with the method **update\_in\_hdx**. These take various boolean 
-parameters that all have defaults and are documented in the API docs. They do not return 
-anything and they throw exceptions for failures like the object to update not existing.
+You can delete HDX objects using **delete_from_hdx** and update an object that 
+already exists in HDX with the method **update_in_hdx**. These take various 
+boolean parameters that all have defaults and are documented in the API docs. 
+They do not return anything and they throw exceptions for failures like the 
+object to update not existing.
 
 ## Dataset Specific Operations
 
 A dataset can have resources and can be in a showcase.
 
 If you wish to add resources, you can supply a list and call 
-the **add\_update\_resources** function, for example:
+the **add_update_resources** function, for example:
 
     resources = [{
         "name": xlsx_resourcename,
         "format": "xlsx",
         "url": xlsx_url
      }, {
         "name": csv_resourcename,
         "format": "zipped csv",
         "url": csv_url
      }]
      for resource in resources:
          resource["description"] = resource["url"].rsplit("/", 1)[-1]
      dataset.add_update_resources(resources)
 
-Calling **add\_update\_resources** creates a list of HDX Resource objects in 
+Calling **add_update_resources** creates a list of HDX Resource objects in 
 dataset and operations can be performed on those objects.
 
-To see the list of resources, you use the **get\_resources** function eg.
+To see the list of resources, you use the **get_resources** function eg.
 
     resources = dataset.get_resources()
 
 If you wish to add one resource, you can supply an id string, dictionary or Resource 
-object and call the **add\_update\_resource**\* function, for example:
+object and call the **add_update_resource** function, for example:
 
     dataset.add_update_resource(resource)
 
-You can delete a Resource object from the dataset using the **delete\_resource** function, for example:
+You can delete a Resource object from the dataset using the **delete_resource** function, for example:
 
     dataset.delete_resource(resource)
 
 You can get all the resources from a list of datasets as follows:
 
     resources = Dataset.get_all_resources(datasets)
 
-To see the list of showcases a dataset is in, you use the **get\_showcases** function eg.
+To see the list of showcases a dataset is in, you use the **get_showcases** function eg.
 
     showcases = dataset.get_showcases()
 
 If you wish to add the dataset to a showcase, you must first create the showcase in HDX if it does not already exist:
 
     showcase = Showcase({"name": "new-showcase-1",
                          "title": "MyShowcase1",
                          "notes": "My Showcase",
                          "package_id": "6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d",
                          "image_display_url": "http://myvisual/visual.png",
                          "url": "http://visualisation/url/"})
     showcase.create_in_hdx()
 
-Then you can supply an id, dictionary or Showcase object and call the **add\_showcase** 
+Then you can supply an id, dictionary or Showcase object and call the **add_showcase** 
 function, for example:
 
     dataset.add_showcase(showcase)
 
-You can remove the dataset from a showcase using the **remove\_showcase** function, for 
+You can remove the dataset from a showcase using the **remove_showcase** function, for 
 example:
 
     dataset.remove_showcase(showcase)
 
 ### Reference Period
 
 Reference Period is a mandatory field in HDX. It is the time period for which 
@@ -674,15 +693,15 @@
 If you want to add a region, you do it as follows. If you don't provide a three digit 
 [UNStats M49](https://unstats.un.org/unsd/methodology/m49/overview/) region code, then 
 parsing and conversion will 
 occur if a valid region name is supplied.
 
     dataset.add_region_location("M49 REGION CODE")
 
-**add\_region\_location** accepts regions, intermediate regions or subregions as 
+**add_region_location** accepts regions, intermediate regions or subregions as 
 specified on the 
 [UNStats M49](https://unstats.un.org/unsd/methodology/m49/overview/) website.
 
 If you want to add any other kind of location (which must be in this
 [list of valid locations](https://data.humdata.org/api/action/group_list?all_fields=true)), 
 you do as shown below.
 
@@ -871,38 +890,56 @@
 
 ## Resource Specific Operations
 
 You can download a resource using the **download** function eg.
 
     url, path = resource.download("FOLDER_TO_DOWNLOAD_TO")
 
-If you do not supply **FOLDER\_TO\_DOWNLOAD\_TO**, then a temporary folder is used.
+If you do not supply **FOLDER_TO_DOWNLOAD_TO**, then a temporary folder is used.
 
-Before creating or updating a resource, it is possible to specify the path to a local 
-file to upload to the HDX filestore if that is preferred over hosting the file 
-externally to HDX. Rather than the url of the resource pointing to your server or api, 
-in this case the url will point to a location in the HDX filestore containing a copy of 
-your file.
+Before creating or updating a resource by calling **create_in_hdx** or 
+**update_in_hdx** on the resource or its parent dataset, it is possible to 
+specify the path to a local file to upload to the HDX filestore if that is 
+preferred over hosting the file externally to HDX. Rather than the url of the 
+resource pointing to your server or api, in this case the url will point to a 
+location in the HDX filestore containing a copy of your file.
 
     resource.set_file_to_upload(file_to_upload="PATH_TO_FILE")
 
 There is a getter to read the value back:
 
     file_to_upload = resource.get_file_to_upload()
 
+To indicate that the data in an externally hosted resource (given by a URL) has 
+been updated, call **mark_data_updated** on the resource, before calling 
+**create_in_hdx** or **update_in_hdx** on the resource or parent dataset which 
+will result in the resource `last_modified` field being set to now.
+
+    resource.mark_data_updated()
+    dataset.update_in_hdx()
+
+Alternatively, when calling **create_in_hdx** or **update_in_hdx** on the 
+resource, it is possible to supply the parameter `data_updated` eg.
+
+    resource.update_in_hdx(data_updated=True)
+
+If the method **set_file_to_upload** is used to supply a file, the resource 
+`last_modified` field is set to now automatically regardless of the value of 
+`data_updated` or whether **mark_data_updated** has been called.
+
 ## Showcase Management
 
 The **Showcase** class enables you to manage showcases, creating, deleting and updating 
 (as for other HDX objects) according to your permissions.
 
-To see the list of datasets a showcase is in, you use the **get\_datasets** function eg.
+To see the list of datasets a showcase is in, you use the **get_datasets** function eg.
 
     datasets = showcase.get_datasets()
 
-If you wish to add a dataset to a showcase, you call the **add\_dataset** function, for 
+If you wish to add a dataset to a showcase, you call the **add_dataset** function, for 
 example:
 
     showcase.add_dataset(dataset)
 
 You can remove the dataset from a showcase using the **remove\dataset** function, for 
 example:
 
@@ -1024,18 +1061,18 @@
         dataset = generate_dataset()
         dataset.create_in_hdx()
 
     if __name__ == "__main__":
         facade(main, hdx_site="test")
 
 The above file will create in HDX a dataset generated by a function called 
-**generate\_dataset** that can be found in the file **my\_code.py** which we will now 
+**generate_dataset** that can be found in the file **my_code.py** which we will now 
 write.
 
-Create a file **my\_code.py** and copy into it the code below:
+Create a file **my_code.py** and copy into it the code below:
 
     #!/usr/bin/python
     # -*- coding: utf-8 -*-
     """
     Generate a dataset
 
     """
@@ -1046,26 +1083,26 @@
 
 
     def generate_dataset():
         """Create a dataset
         """
         logger.debug("Generating dataset!")
 
-You can then fill out the function **generate\_dataset** as required.
+You can then fill out the function **generate_dataset** as required.
 
 # IDMC Example
 
 A complete example can be found here: <https://github.com/OCHA-DAP/hdx-scraper-idmc>
 
 In particular, take a look at the files **run.py**, **idmc.py** and the **config** 
 folder. If you run it unchanged, it will overwrite the existing datasets in the IDMC 
 organisation! Therefore, you should run it against a test server. If you use it as a 
 basis for your code, you will need to modify the dataset **name**  in **idmc.py** and 
 change the organisation information to your organisation. Also update metadata in 
-**config/hdx\_dataset\_static.yaml** appropriately.
+**config/hdx_dataset_static.yaml** appropriately.
 
 The IDMC scraper creates a dataset per country in HDX, populating all the required 
 metadata. It then creates resources with files held on the HDX filestore.
 
 # Brief History
 
 The first iteration of a scraper for ACLED was written without the HDX Python library
```

### Comparing `hdx_python_api-6.0.4/documentation/pydoc-markdown.yaml` & `hdx_python_api-6.0.5/documentation/pydoc-markdown.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/api/configuration.py` & `hdx_python_api-6.0.5/src/hdx/api/configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/api/hdx_base_configuration.yaml` & `hdx_python_api-6.0.5/src/hdx/api/hdx_base_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/api/locations.py` & `hdx_python_api-6.0.5/src/hdx/api/locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/data/dataset.py` & `hdx_python_api-6.0.5/src/hdx/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,14 +286,16 @@
             updated_resource = merge_two_dictionaries(
                 self.resources[resource_index], resource
             )
             if resource.get_file_to_upload():
                 updated_resource.set_file_to_upload(
                     resource.get_file_to_upload()
                 )
+            if resource.is_data_updated():
+                updated_resource.mark_data_updated()
 
     def add_update_resources(
         self,
         resources: ListTuple[Union["Resource", Dict, str]],
         ignore_datasetid: bool = False,
     ) -> None:
         """Add new to the dataset or update existing resources with new metadata
@@ -328,14 +330,16 @@
             updated_resource = merge_two_dictionaries(
                 self.resources[resource_index], resource
             )
             if resource.get_file_to_upload():
                 updated_resource.set_file_to_upload(
                     resource.get_file_to_upload()
                 )
+            if resource.is_data_updated():
+                updated_resource.mark_data_updated()
         for resource_index in updated_resource_no_matches:
             resource = resource_objects[resource_index]
             resource.check_url_filetoupload()
             self.resources.append(resource)
 
     def delete_resource(
         self,
@@ -466,15 +470,17 @@
         return None
 
     def _dataset_create_resources(self) -> None:
         """Creates resource objects in dataset"""
 
         if "resources" in self.data:
             self.old_data["resources"] = self._copy_hdxobjects(
-                self.resources, res_module.Resource, "file_to_upload"
+                self.resources,
+                res_module.Resource,
+                ("file_to_upload", "data_updated"),
             )
             self.init_resources()
             self.separate_resources()
 
     def _dataset_load_from_hdx(self, id_or_name: str) -> bool:
         """Loads the dataset given by either id or name from HDX
```

### Comparing `hdx_python_api-6.0.4/src/hdx/data/dataset_title_helper.py` & `hdx_python_api-6.0.5/src/hdx/data/dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/data/date_helper.py` & `hdx_python_api-6.0.5/src/hdx/data/date_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/data/filestore_helper.py` & `hdx_python_api-6.0.5/src/hdx/data/filestore_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Helper to the Dataset class for handling resources with filestores.
 """
+from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict
 
 from hdx.utilities.dictandlist import merge_two_dictionaries
 
 if TYPE_CHECKING:
     from hdx.data.resource import Resource
 
@@ -87,13 +88,17 @@
         Returns:
             None
         """
         file_to_upload = updated_resource.get_file_to_upload()
         if file_to_upload:
             resource.set_file_to_upload(file_to_upload)
             filestore_resources[resource_index] = file_to_upload
+        data_updated = updated_resource.is_data_updated()
         merge_two_dictionaries(resource, updated_resource)
         cls.resource_check_required_fields(
             resource, check_upload=True, **kwargs
         )
         if resource.get_file_to_upload():
             resource["url"] = cls.temporary_url
+        if data_updated:
+            resource["last_modified"] = datetime.utcnow().isoformat()
+            resource.data_updated = False
```

### Comparing `hdx_python_api-6.0.4/src/hdx/data/hdxobject.py` & `hdx_python_api-6.0.5/src/hdx/data/hdxobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,21 +287,21 @@
         Args:
             object_type (str): Description of HDX object type (for messages)
             id_field_name (str): Name of field containing HDX object identifier
             files_to_upload (Dict): Files to upload to HDX
             force_active (bool): Make object state active. Defaults to False.
             **kwargs: See below
             operation (str): Operation to perform eg. patch. Defaults to update.
-            ignore_field (str): Any field to ignore when checking dataset metadata. Defaults to None.
+            ignore_field (str): Any field to ignore when checking metadata. Defaults to None.
 
         Returns:
             None
         """
         self._check_kwargs_fields(object_type, **kwargs)
-        operation = kwargs.get("operation", "update")
+        operation = kwargs.pop("operation", "update")
         self._save_to_hdx(
             operation, id_field_name, files_to_upload, force_active
         )
 
     def _merge_hdx_update(
         self,
         object_type: str,
@@ -315,15 +315,15 @@
         Args:
             object_type (str): Description of HDX object type (for messages)
             id_field_name (str): Name of field containing HDX object identifier
             files_to_upload (Dict): Files to upload to HDX
             force_active (bool): Make object state active. Defaults to False.
             **kwargs: See below
             operation (str): Operation to perform eg. patch. Defaults to update.
-            ignore_field (str): Any field to ignore when checking dataset metadata. Defaults to None.
+            ignore_field (str): Any field to ignore when checking metadata. Defaults to None.
 
         Returns:
             None
         """
         merge_two_dictionaries(self.data, self.old_data)
         self._hdx_update(
             object_type,
@@ -617,35 +617,35 @@
             newhdxobjects.append(hdxobject.data)
         return newhdxobjects
 
     def _copy_hdxobjects(
         self,
         hdxobjects: ListTuple["HDXObject"],
         hdxobjectclass: type,
-        attribute_to_copy: Optional[str] = None,
+        attributes_to_copy: ListTuple[str] = (),
     ) -> List["HDXObject"]:
         """Helper function to make a deep copy of a supplied list of HDX objects
 
         Args:
             hdxobjects (ListTuple[HDXObject]): list of HDX objects to copy
             hdxobjectclass (type): Type of the HDX Objects to be copied
-            attribute_to_copy (Optional[str]): An attribute to copy over from the HDX object. Defaults to None.
+            attributes_to_copy (ListTuple[str]): Attributes to copy over from the HDX object. Defaults to ().
 
         Returns:
             List[HDXObject]: Deep copy of list of HDX objects
         """
         newhdxobjects = list()
         for hdxobject in hdxobjects:
             newhdxobjectdata = copy.deepcopy(hdxobject.data)
             newhdxobject = hdxobjectclass(
                 newhdxobjectdata, configuration=self.configuration
             )
-            if attribute_to_copy:
-                value = getattr(hdxobject, attribute_to_copy)
-                setattr(newhdxobject, attribute_to_copy, value)
+            for attribute in attributes_to_copy:
+                value = getattr(hdxobject, attribute)
+                setattr(newhdxobject, attribute, value)
             newhdxobjects.append(newhdxobject)
         return newhdxobjects
 
     def _separate_hdxobjects(
         self,
         hdxobjects: ListTuple["HDXObject"],
         hdxobjects_name: str,
```

### Comparing `hdx_python_api-6.0.4/src/hdx/data/indicator_resource_view_template.yaml` & `hdx_python_api-6.0.5/src/hdx/data/indicator_resource_view_template.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/data/organization.py` & `hdx_python_api-6.0.5/src/hdx/data/organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/data/resource.py` & `hdx_python_api-6.0.5/src/hdx/data/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         initial_data: Optional[Dict] = None,
         configuration: Optional[Configuration] = None,
     ) -> None:
         if not initial_data:
             initial_data = dict()
         super().__init__(initial_data, configuration=configuration)
         self.file_to_upload = None
+        self.data_updated = False
 
     @staticmethod
     def actions() -> Dict[str, str]:
         """Dictionary of actions that can be performed on object
 
         Returns:
             Dict[str, str]: Dictionary of actions that can be performed on object
@@ -348,48 +349,85 @@
         Returns:
             Dict: files parameter for CKANAPI
         """
         if self.file_to_upload is None:
             return dict()
         return {"upload": self.file_to_upload}
 
+    def _resource_merge_hdx_update(
+        self,
+        **kwargs: Any,
+    ) -> None:
+        """Helper method to update last_modified for external resources if
+        data_updated is True, then check if HDX object exists and update it.
+
+        Args:
+            **kwargs: See below
+            operation (str): Operation to perform eg. patch. Defaults to update.
+            data_updated (bool): If True, set last_modified to now. Defaults to False.
+
+        Returns:
+            None
+        """
+        data_updated = kwargs.pop("data_updated", self.data_updated)
+        if data_updated and not self.file_to_upload:
+            self.old_data["last_modified"] = datetime.utcnow().isoformat()
+            self.data_updated = False
+            # old_data will be merged into data in the next step
+        self._merge_hdx_update(
+            "resource", "id", self._get_files(), True, **kwargs
+        )
+
     def update_in_hdx(self, **kwargs: Any) -> None:
-        """Check if resource exists in HDX and if so, update it
+        """Check if resource exists in HDX and if so, update it. To indicate
+        that the data in an external resource (given by a URL) has been
+        updated, set data_updated to True, which will result in the resource
+        last_modified field being set to now. If the method set_file_to_upload
+        is used to supply a file, the resource last_modified field is set to
+        now automatically regardless of the value of data_updated.
 
         Args:
             **kwargs: See below
             operation (string): Operation to perform eg. patch. Defaults to update.
+            data_updated (bool): If True, set last_modified to now. Defaults to False.
 
         Returns:
             None
         """
         self._check_load_existing_object("resource", "id")
         if self.file_to_upload and "url" in self.data:
             del self.data["url"]
-        self._merge_hdx_update(
-            "resource", "id", self._get_files(), True, **kwargs
-        )
+        self._resource_merge_hdx_update(**kwargs)
 
     def create_in_hdx(self, **kwargs: Any) -> None:
-        """Check if resource exists in HDX and if so, update it, otherwise create it
+        """Check if resource exists in HDX and if so, update it, otherwise
+        create it. To indicate that the data in an external resource (given by
+        a URL) has been updated, set data_updated to True, which will result in
+        the resource last_modified field being set to now. If the method
+        set_file_to_upload is used to supply a file, the resource last_modified
+        field is set to now automatically regardless of the value of
+        data_updated.
+
+        Args:
+            **kwargs: See below
+            data_updated (bool): If True, set last_modified to now. Defaults to False.
 
         Returns:
             None
         """
         if "ignore_check" not in kwargs:  # allow ignoring of field checks
             self.check_required_fields()
         id = self.data.get("id")
-        files = self._get_files()
         if id and self._load_from_hdx("resource", id):
             logger.warning(f"{'resource'} exists. Updating {id}")
             if self.file_to_upload and "url" in self.data:
                 del self.data["url"]
-            self._merge_hdx_update("resource", "id", files, True, **kwargs)
+            self._resource_merge_hdx_update(**kwargs)
         else:
-            self._save_to_hdx("create", "name", files, True)
+            self._save_to_hdx("create", "name", self._get_files(), True)
 
     def delete_from_hdx(self) -> None:
         """Deletes a resource from HDX
 
         Returns:
             None
         """
@@ -702,7 +740,23 @@
             batch_mode="KEEP_OLD",
             skip_validation=True,
         )
         if success:
             self.data = result
         else:
             logger.debug(result)
+
+    def is_data_updated(self) -> bool:
+        """Return if the resource's data is updated
+
+        Returns:
+            bool: Whether resource's data is updated
+        """
+        return self.data_updated
+
+    def mark_data_updated(self) -> None:
+        """Mark resource data as updated
+
+        Returns:
+            None
+        """
+        self.data_updated = True
```

### Comparing `hdx_python_api-6.0.4/src/hdx/data/resource_matcher.py` & `hdx_python_api-6.0.5/src/hdx/data/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/data/resource_view.py` & `hdx_python_api-6.0.5/src/hdx/data/resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/data/showcase.py` & `hdx_python_api-6.0.5/src/hdx/data/showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/data/user.py` & `hdx_python_api-6.0.5/src/hdx/data/user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/data/vocabulary.py` & `hdx_python_api-6.0.5/src/hdx/data/vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/facades/infer_arguments.py` & `hdx_python_api-6.0.5/src/hdx/facades/infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/facades/keyword_arguments.py` & `hdx_python_api-6.0.5/src/hdx/facades/keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/src/hdx/facades/simple.py` & `hdx_python_api-6.0.5/src/hdx/facades/simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/Accepted_Tags.csv` & `hdx_python_api-6.0.5/tests/fixtures/Accepted_Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/Tag_Mapping.csv` & `hdx_python_api-6.0.5/tests/fixtures/Tag_Mapping.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/dataset_search_results.yaml` & `hdx_python_api-6.0.5/tests/fixtures/dataset_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/organization_show_results.yaml` & `hdx_python_api-6.0.5/tests/fixtures/organization_show_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/resource_formats.json` & `hdx_python_api-6.0.5/tests/fixtures/resource_formats.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/showcase_all_search_results.yaml` & `hdx_python_api-6.0.5/tests/fixtures/showcase_all_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/test_data.csv` & `hdx_python_api-6.0.5/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/test_data.zip` & `hdx_python_api-6.0.5/tests/fixtures/test_data.zip`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/config/hdx_dataset_static.json` & `hdx_python_api-6.0.5/tests/fixtures/config/hdx_dataset_static.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/config/hdx_dataset_static.yaml` & `hdx_python_api-6.0.5/tests/fixtures/config/hdx_dataset_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/config/hdx_datasource_topline.json` & `hdx_python_api-6.0.5/tests/fixtures/config/hdx_datasource_topline.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/config/hdx_resource_view_static.yaml` & `hdx_python_api-6.0.5/tests/fixtures/config/hdx_resource_view_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx` & `hdx_python_api-6.0.5/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/gen_resource/conflict_data_alg.csv` & `hdx_python_api-6.0.5/tests/fixtures/gen_resource/conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/gen_resource/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.5/tests/fixtures/gen_resource/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/gen_resource/test_data_no_years.csv` & `hdx_python_api-6.0.5/tests/fixtures/gen_resource/test_data_no_years.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.5/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/dem_data_zwe.csv` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/dem_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_data_zwe.csv` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/unesco_dataset.json` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/unesco_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_dataset_resources/unesco_update_dataset.json` & `hdx_python_api-6.0.5/tests/fixtures/update_dataset_resources/unesco_update_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_logic/update_logic_resources.yaml` & `hdx_python_api-6.0.5/tests/fixtures/update_logic/update_logic_resources.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/fixtures/update_logic/update_logic_resources_new.yaml` & `hdx_python_api-6.0.5/tests/fixtures/update_logic/update_logic_resources_new.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/conftest.py` & `hdx_python_api-6.0.5/tests/hdx/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Global fixtures"""
+import re
 import smtplib
 from os.path import join
 
 import pytest
 
 from hdx.api.configuration import Configuration
 from hdx.api.locations import Locations
@@ -1544,7 +1545,12 @@
 
     class MockSMTP(MockSMTPBase):
         type = "smtp"
 
     monkeypatch.setattr(smtplib, "SMTP_SSL", MockSMTPSSL)
     monkeypatch.setattr(smtplib, "LMTP", MockLMTP)
     monkeypatch.setattr(smtplib, "SMTP", MockSMTP)
+
+
+@pytest.fixture(scope="session")
+def date_pattern():
+    return re.compile(r"[12]\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d.\d\d\d\d\d\d")
```

### Comparing `hdx_python_api-6.0.4/tests/hdx/api/test_configuration.py` & `hdx_python_api-6.0.5/tests/hdx/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/api/test_locations.py` & `hdx_python_api-6.0.5/tests/hdx/api/test_locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/__init__.py` & `hdx_python_api-6.0.5/tests/hdx/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_dataset_core.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_dataset_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -628,15 +628,15 @@
         dataset.add_update_resource(resource)
         dataset.create_in_hdx()
         remove(file.name)
         assert dataset["state"] == "active"
         assert len(dataset.resources) == 3
         # Dataset creates that end up updating are in the test below
 
-    def test_update_in_hdx(self, configuration, post_update):
+    def test_update_in_hdx(self, configuration, post_update, date_pattern):
         dataset = Dataset()
         dataset["id"] = "NOTEXIST"
         with pytest.raises(HDXError):
             dataset.update_in_hdx()
         dataset["name"] = "LALA"
         with pytest.raises(HDXError):
             dataset.update_in_hdx()
@@ -703,18 +703,23 @@
         dataset.create_in_hdx(allow_no_resources=True)
         assert dataset["name"] == "DatasetExist"
         datasetdata["name"] = "MyDataset1"
         datasetdata["id"] = "TEST1"
         dataset = Dataset(datasetdata)
         resourcesdata = copy.deepcopy(resources_data)
         resource = Resource(resourcesdata[0])
+        resource.mark_data_updated()
         dataset.add_update_resources([resource, resource])
         dataset.create_in_hdx()
         assert dataset["state"] == "active"
         assert len(dataset.resources) == 3
+        resource = dataset.get_resource()
+        assert resource.is_data_updated() is False
+        match = date_pattern.search(resource["last_modified"])
+        assert match
 
         dataset = Dataset(datasetdata)
         resourcesdata = copy.deepcopy(resources_data)
         resource = Resource(resourcesdata[0])
         dataset.add_update_resources([resource, resource])
         dataset.create_in_hdx(match_resources_by_metadata=False)
         assert dataset["id"] == "TEST1"
```

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_dataset_noncore.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_dataset_noncore.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_dataset_title_helper.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_organization.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_resource.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -725,15 +725,15 @@
 
     def test_check_required_fields(self, configuration):
         resource_data = copy.deepcopy(TestResource.resource_data)
         resource = Resource(resource_data)
         resource.check_url_filetoupload()
         resource.check_required_fields()
 
-    def test_create_in_hdx(self, configuration, post_create):
+    def test_create_in_hdx(self, configuration, date_pattern, post_create):
         resource = Resource()
         with pytest.raises(HDXError):
             resource.create_in_hdx()
         resource["id"] = "74b74ae1-df0c-4716-829f-4f939a046811"
         resource["name"] = "LALA"
         with pytest.raises(HDXError):
             resource.create_in_hdx()
@@ -774,15 +774,15 @@
             resource.create_in_hdx()
 
         resource_data["name"] = "MyResource3"
         resource = Resource(resource_data)
         with pytest.raises(HDXError):
             resource.create_in_hdx()
 
-    def test_update_in_hdx(self, configuration, post_update):
+    def test_update_in_hdx(self, configuration, date_pattern, post_update):
         resource = Resource()
         resource["id"] = "NOTEXIST"
         with pytest.raises(HDXError):
             resource.update_in_hdx()
         resource["name"] = "LALA"
         with pytest.raises(HDXError):
             resource.update_in_hdx()
@@ -792,28 +792,30 @@
         )
         assert resource["id"] == "de6549d8-268b-4dfe-adaf-a4ae5c8510d5"
         assert resource.get_file_type() == "csv"
 
         resource.set_file_type("XLSX")
         resource["id"] = "74b74ae1-df0c-4716-829f-4f939a046811"
         resource["name"] = "MyResource1"
-        resource.update_in_hdx()
+        resource.update_in_hdx(data_updated=True)
         assert resource["id"] == "74b74ae1-df0c-4716-829f-4f939a046811"
         assert resource["format"] == "xlsx"
         resource.set_file_type(".xsl")
         assert resource.get_file_type() == "xls"
         resource.set_file_type("XLSX")
         assert resource.get_file_type() == "xlsx"
         assert resource["url_type"] == "api"
         assert resource["resource_type"] == "api"
         assert (
             resource["url"]
             == "https://raw.githubusercontent.com/OCHA-DAP/hdx-python-api/main/tests/fixtures/test_data.csv"
         )
         assert resource["state"] == "active"
+        match = date_pattern.search(resource["last_modified"])
+        assert match
 
         filetoupload = join("tests", "fixtures", "test_data.csv")
         resource.set_file_to_upload(
             filetoupload, guess_format_from_suffix=True
         )
         assert resource["format"] == "csv"
         resource.update_in_hdx()
@@ -837,18 +839,24 @@
         with pytest.raises(HDXError):
             resource.update_in_hdx()
 
         resource_data = copy.deepcopy(TestResource.resource_data)
         resource_data["name"] = "MyResource1"
         resource_data["id"] = "74b74ae1-df0c-4716-829f-4f939a046811"
         resource = Resource(resource_data)
+        resource.mark_data_updated()
+        assert resource.data_updated is True
+        assert resource.is_data_updated() is True
         resource.create_in_hdx()
+        assert resource.is_data_updated() is False
         assert resource["id"] == "74b74ae1-df0c-4716-829f-4f939a046811"
         assert resource.get_file_type() == "xlsx"
         assert resource["state"] == "active"
+        match = date_pattern.search(resource["last_modified"])
+        assert match
         resource["format"] = "Geoservice"
         resource.update_in_hdx()
         assert resource.get_file_type() == "geoservice"
         resource["format"] = "NOTEXIST"
         with pytest.raises(HDXError):
             resource.update_in_hdx()
```

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_resource_view.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_showcase.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_update_dataset_resources.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_update_dataset_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             return dataset
 
     def test_dataset_update_resources(
         self, configuration, dataset, new_dataset
     ):
         dataset.old_data = new_dataset.data
         dataset.old_data["resources"] = new_dataset._copy_hdxobjects(
-            new_dataset.resources, Resource, "file_to_upload"
+            new_dataset.resources, Resource, ("file_to_upload", "data_updated")
         )
         (
             resources_to_delete,
             new_resource_order,
             filestore_resources,
         ) = dataset._dataset_merge_update_resources(True, True, True, True)
         assert resources_to_delete == [8, 2, 1, 0]
```

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_update_logic.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_update_logic.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_user.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/data/test_vocabulary.py` & `hdx_python_api-6.0.5/tests/hdx/data/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/facades/__init__.py` & `hdx_python_api-6.0.5/tests/hdx/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/facades/test_infer_arguments.py` & `hdx_python_api-6.0.5/tests/hdx/facades/test_infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/facades/test_keyword_arguments.py` & `hdx_python_api-6.0.5/tests/hdx/facades/test_keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/tests/hdx/facades/test_simple.py` & `hdx_python_api-6.0.5/tests/hdx/facades/test_simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/workingexample/my_resource.xlsx` & `hdx_python_api-6.0.5/workingexample/my_resource.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/.gitignore` & `hdx_python_api-6.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/LICENSE` & `hdx_python_api-6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/README.md` & `hdx_python_api-6.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yaml)
-[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-api/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-api?branch=main)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-api/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-api?branch=main)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-api.svg)](https://pypistats.org/packages/hdx-python-api)
 
 The HDX Python API Library is designed to enable you to easily develop code that 
 interacts with the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) 
 platform. The major goal of the library is to make pushing and pulling data from HDX as 
 simple as possible for the end user.
```

### Comparing `hdx_python_api-6.0.4/pyproject.toml` & `hdx_python_api-6.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.4/PKG-INFO` & `hdx_python_api-6.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-api
-Version: 6.0.4
+Version: 6.0.5
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-api
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: API,CKAN,HDX,humanitarian data exchange
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,16 @@
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-api/actions/workflows/run-python-tests.yaml)
-[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-api/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-api?branch=main)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-api/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-api?branch=main)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-api.svg)](https://pypistats.org/packages/hdx-python-api)
 
 The HDX Python API Library is designed to enable you to easily develop code that 
 interacts with the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) 
 platform. The major goal of the library is to make pushing and pulling data from HDX as 
 simple as possible for the end user.
```

