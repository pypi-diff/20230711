# Comparing `tmp/finra_api_queries-1.2.0.tar.gz` & `tmp/finra_api_queries-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finra_api_queries-1.2.0.tar", max compression
+gzip compressed data, was "finra_api_queries-1.2.1.tar", max compression
```

## Comparing `finra_api_queries-1.2.0.tar` & `finra_api_queries-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       39 2022-12-16 21:49:02.129033 finra_api_queries-1.2.0/finra_api_queries/__init__.py
--rw-r--r--   0        0        0    47915 2023-02-05 19:31:09.573152 finra_api_queries-1.2.0/finra_api_queries/finra_api_queries.py
--rw-r--r--   0        0        0     1091 2022-11-30 00:59:31.879793 finra_api_queries-1.2.0/LICENSE
--rw-r--r--   0        0        0      640 2023-02-05 19:37:11.141098 finra_api_queries-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2626 2023-02-05 18:25:49.759144 finra_api_queries-1.2.0/README.md
--rw-r--r--   0        0        0     3163 1970-01-01 00:00:00.000000 finra_api_queries-1.2.0/setup.py
--rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 finra_api_queries-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       39 2022-12-16 21:49:02.129033 finra_api_queries-1.2.1/finra_api_queries/__init__.py
+-rw-r--r--   0        0        0    47814 2023-07-11 02:36:10.870207 finra_api_queries-1.2.1/finra_api_queries/finra_api_queries.py
+-rw-r--r--   0        0        0     1091 2022-11-30 00:59:31.879793 finra_api_queries-1.2.1/LICENSE
+-rw-r--r--   0        0        0      828 2023-07-11 02:45:14.127887 finra_api_queries-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2626 2023-02-05 18:25:49.759144 finra_api_queries-1.2.1/README.md
+-rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 finra_api_queries-1.2.1/setup.py
+-rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 finra_api_queries-1.2.1/PKG-INFO
```

### Comparing `finra_api_queries-1.2.0/finra_api_queries/finra_api_queries.py` & `finra_api_queries-1.2.1/finra_api_queries/finra_api_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,17 +306,15 @@
                     try:
                         match = re.search(r'^([>=!<]+)\s(\d+)', l)
                         comp_symbol = match.group(1)
                     except:
                         pass
 
                     if comp_symbol in qualifiers.keys():
-                        comp_filters_list.append({'fieldName': i,
-                                                    'fieldValue': match.group(2),
-                                                    'compareType': qualifiers[comp_symbol]})
+                        comp_filters_list.append({'fieldName': i, 'fieldValue': match.group(2), 'compareType': qualifiers[comp_symbol]})
                     else:
                         filters_list.append({'fieldName': i, 'values': j}) # add entry to the filters_list
             else:
                 filters_list.append({'fieldName': i, 'values': j}) # add entry to the filters_list
 
     # make the API call
     # if optional argument for columns has been entered
@@ -425,15 +423,15 @@
                                 json = {'domainFilters': filters_list,
                                           'dateRangeFilters': date_filter,
                                           'limit': rows_returned})
         else:
             response = requests.post(f'https://api.finra.org/data/group/{eligible_groups[dataset_name]}/name/{eligible_datasets[dataset_name]}?limit={rows_returned}',
                                 headers = {'Authorization': 'Bearer ' + my_access_token,
                                            'Accept': 'application/json'},
-                                json = {'fields': filtered_columns,
+                                json = {'domainFilters': filters_list,
                                         'compareFilters': comp_filters_list,
                                           'dateRangeFilters': date_filter,
                                           'limit': rows_returned})
 
 
     # convert to data frame
     response_df = pd.DataFrame(response.json())
@@ -864,8 +862,8 @@
     final_df = grouped_weekly.sort_values(column_to_sort, ascending = False).reset_index()
 
     # drop the excess index column
     final_df.drop('index', axis = 1, inplace = True)
 
     assert len(final_df) > 0, "The keyword search did not yield any results."
 
-    return final_df
+    return final_df
```

### Comparing `finra_api_queries-1.2.0/LICENSE` & `finra_api_queries-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finra_api_queries-1.2.0/pyproject.toml` & `finra_api_queries-1.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 [tool.poetry]
 name = "finra_api_queries"
-version = "1.2.0"
+version = "1.2.1"
 description = "An API wrapper for FINRA's Query API"
 authors = ["Cindy Chen"]
 license = "MIT"
 readme = "README.md"
 
+documentation = 'https://finra_api_queries.readthedocs.io'
+homepage = "https://github.com/chencindyj/finra_api_queries"
+repository = "https://github.com/chencindyj/finra_api_queries"
+
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 myst-nb = "^0.17.1"
```

### Comparing `finra_api_queries-1.2.0/README.md` & `finra_api_queries-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `finra_api_queries-1.2.0/setup.py` & `finra_api_queries-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['finra_api_queries']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'finra-api-queries',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': "An API wrapper for FINRA's Query API",
     'long_description': '# finra_api_queries\n\nFINRA is the Financial Industry Regulatory Authority, which oversees US brokerages and exchanges such as the NYSE and NASDAQ.  They ensure that brokers and dealers in US stock/debt markets are acting according to the laws and rules defined by the Securities and Exchange Commission (SEC) as well as by FINRA.  Their API contains information about historical market activity, such as fixed income market activity, statistics such as the size of trades that major institutional investors make, and over-the-counter (OTC) trading activity.  This information allows regulators as well as the public to understand market trading behavior.\n\nThe finra_api_queries package simplifies the querying of the FINRA Query API including more complex API calls. It also features functions that enable the time series data visualization of fixed income data, summarization of key market breadth data, and keyword filtering for stocks.\n\n## Installation\n\n```bash\n$ pip install finra_api_queries\n```\n\n## How to Use\n\n```bash\n$ from finra_api_queries import finra_api_queries\n```\n\n## Usage\n\n1. Obtain an API key and secret on the FINRA API website.\n2. Input the key and secret using the retrieve_api_token() function to generate the time-limited access token necessary to retrieve data from the API.\n3. Use the various functions to easily extract data sets from the FINRA Query API with a variety of parameters, visualize time series data, as well as filter and aggregate data in pandas data frames and Seaborn plots.\n4. Use API to glean time series-related and aggregated insights about fixed income activity and trading block activity.\n\nThis package features the following 7 functions:\n\n* retrieve_api_token\n* show_filterable_columns\n* retrieve_dataset\n* filter_market_participant\n* summarize_trading_breadth\n* visualize_market_sentiment\n* generate_market_participant_summary\n\n#### readthedocs Package Documentation\nhttps://finra-api-queries.readthedocs.io/en/latest/\n\n#### Test PyPi Link\nhttps://test.pypi.org/project/finra-api-queries/\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`finra_api_queries` was created by Cindy Chen. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`finra_api_queries` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Cindy Chen',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/chencindyj/finra_api_queries',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `finra_api_queries-1.2.0/PKG-INFO` & `finra_api_queries-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: finra-api-queries
-Version: 1.2.0
+Version: 1.2.1
 Summary: An API wrapper for FINRA's Query API
+Home-page: https://github.com/chencindyj/finra_api_queries
 License: MIT
 Author: Cindy Chen
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Project-URL: Documentation, https://finra_api_queries.readthedocs.io
+Project-URL: Repository, https://github.com/chencindyj/finra_api_queries
 Description-Content-Type: text/markdown
 
 # finra_api_queries
 
 FINRA is the Financial Industry Regulatory Authority, which oversees US brokerages and exchanges such as the NYSE and NASDAQ.  They ensure that brokers and dealers in US stock/debt markets are acting according to the laws and rules defined by the Securities and Exchange Commission (SEC) as well as by FINRA.  Their API contains information about historical market activity, such as fixed income market activity, statistics such as the size of trades that major institutional investors make, and over-the-counter (OTC) trading activity.  This information allows regulators as well as the public to understand market trading behavior.
 
 The finra_api_queries package simplifies the querying of the FINRA Query API including more complex API calls. It also features functions that enable the time series data visualization of fixed income data, summarization of key market breadth data, and keyword filtering for stocks.
```

