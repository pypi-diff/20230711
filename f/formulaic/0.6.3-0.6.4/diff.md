# Comparing `tmp/formulaic-0.6.3.tar.gz` & `tmp/formulaic-0.6.4.tar.gz`

## Comparing `formulaic-0.6.3.tar` & `formulaic-0.6.4.tar`

### file list

```diff
@@ -1,131 +1,133 @@
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/README.md
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/benchmark.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/benchmarks.csv
--rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/benchmarks.png
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/plot.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/requirements.txt
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/mkdocs.yml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/requirements.in
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/requirements.txt
--rw-r--r--   0        0        0    17079 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/changelog.md
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/formulas.md
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/index.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/installation.md
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/migration.md
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/assets/images/logo.png
--rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/assets/images/logo.svg
--rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/assets/images/logo_with_text.png
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/concepts/index.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/dev/index.md
--rw-r--r--   0        0        0    46448 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/contrasts.ipynb
--rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/formulae.ipynb
--rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/grammar.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/index.md
--rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/integration.ipynb
--rw-r--r--   0        0        0    27554 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/model_specs.ipynb
--rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/quickstart.ipynb
--rw-r--r--   0        0        0   162005 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/splines.ipynb
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/transforms.ipynb
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/_version.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/errors.py
--rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/formula.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/model_matrix.py
--rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/model_spec.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/sugar.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/arrow.py
--rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/base.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/pandas.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/enums.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/evaluated_factor.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/factor_values.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/scoped_factor.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/scoped_term.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/__init__.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/parser.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/utils.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/algos/__init__.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/algos/tokenize.py
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/algos/tokens_to_ast.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/__init__.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/ast_node.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/factor.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/formula_parser.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/operator.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/operator_resolver.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/ordered_set.py
--rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/structured.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/term.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/token.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/__init__.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/basis_spline.py
--rw-r--r--   0        0        0    26786 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/contrasts.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/identity.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/patsy_compat.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/poly.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/__init__.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/calculus.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/cast.py
--rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/constraints.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/context.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/iterators.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/layered_mapping.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/sentinels.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/sparse.py
--rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/stateful_transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/__init__.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/test_formula.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/test_model_matrix.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/test_model_spec.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/test_sugar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/__init__.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/test_arrow.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/test_base.py
--rw-r--r--   0        0        0    15530 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/test_pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/test_evaluated_factor.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/test_factor_values.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/test_scoped_factor.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/test_scoped_term.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/__init__.py
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/test_parser.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/algos/__init__.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/algos/test_tokenize.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/algos/test_tokens_to_ast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_ast_node.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_factor.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_formula_parser.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_operator.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_operator_resolver.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_ordered_set.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_structured.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_term.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/__init__.py
--rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_basis_spline.py
--rw-r--r--   0        0        0    29890 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_contrasts.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_identity.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_patsy_compat.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_poly.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_calculus.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_capture_context.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_cast.py
--rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_constraints.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_iterators.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_layered_mapping.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_sentinels.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_sparse.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_stateful_transforms.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.6.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.6.3/LICENSE
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 formulaic-0.6.3/README.md
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 formulaic-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 formulaic-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.6.4/benchmarks/README.md
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.6.4/benchmarks/benchmark.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.6.4/benchmarks/benchmarks.csv
+-rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.6.4/benchmarks/benchmarks.png
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.6.4/benchmarks/plot.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.6.4/benchmarks/requirements.txt
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/mkdocs.yml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/requirements.in
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/requirements.txt
+-rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/changelog.md
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/formulas.md
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/index.md
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/installation.md
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/migration.md
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/assets/images/logo_with_text.png
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/concepts/index.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/dev/index.md
+-rw-r--r--   0        0        0    46448 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/guides/contrasts.ipynb
+-rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/guides/formulae.ipynb
+-rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/guides/grammar.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/guides/index.md
+-rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/guides/integration.ipynb
+-rw-r--r--   0        0        0    28831 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/guides/model_specs.ipynb
+-rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/guides/quickstart.ipynb
+-rw-r--r--   0        0        0   162005 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/guides/splines.ipynb
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 formulaic-0.6.4/docsite/docs/guides/transforms.ipynb
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/_version.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/errors.py
+-rw-r--r--   0        0        0    10493 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/formula.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/model_matrix.py
+-rw-r--r--   0        0        0    19800 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/model_spec.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/sugar.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/arrow.py
+-rw-r--r--   0        0        0    35238 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/base.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/pandas.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/types/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/types/enums.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/types/evaluated_factor.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/types/factor_values.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/types/scoped_factor.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/materializers/types/scoped_term.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/__init__.py
+-rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/parser.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/utils.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/algos/__init__.py
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/algos/tokenize.py
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/algos/tokens_to_ast.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/__init__.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/ast_node.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/factor.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/formula_parser.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/operator.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/operator_resolver.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/ordered_set.py
+-rw-r--r--   0        0        0    17465 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/structured.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/term.py
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/parser/types/token.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/transforms/__init__.py
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/transforms/basis_spline.py
+-rw-r--r--   0        0        0    30627 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/transforms/contrasts.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/transforms/identity.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/transforms/patsy_compat.py
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/transforms/poly.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/transforms/scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/__init__.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/calculus.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/cast.py
+-rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/constraints.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/context.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/iterators.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/layered_mapping.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/sentinels.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/sparse.py
+-rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/stateful_transforms.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 formulaic-0.6.4/formulaic/utils/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/__init__.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/test_formula.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/test_model_matrix.py
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/test_model_spec.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/test_sugar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/materializers/__init__.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/materializers/test_arrow.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/materializers/test_base.py
+-rw-r--r--   0        0        0    15910 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/materializers/test_pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/materializers/types/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/materializers/types/test_evaluated_factor.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/materializers/types/test_factor_values.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/materializers/types/test_scoped_factor.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/materializers/types/test_scoped_term.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/__init__.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/test_parser.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/algos/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/algos/test_tokenize.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/algos/test_tokens_to_ast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/test_ast_node.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/test_factor.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/test_formula_parser.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/test_operator.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/test_operator_resolver.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/test_ordered_set.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/test_structured.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/test_term.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/parser/types/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/transforms/__init__.py
+-rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/transforms/test_basis_spline.py
+-rw-r--r--   0        0        0    29891 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/transforms/test_contrasts.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/transforms/test_identity.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/transforms/test_patsy_compat.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/transforms/test_poly.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/transforms/test_scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_calculus.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_capture_context.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_cast.py
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_constraints.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_iterators.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_layered_mapping.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_sentinels.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_sparse.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_stateful_transforms.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 formulaic-0.6.4/tests/utils/test_variables.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.6.4/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 formulaic-0.6.4/README.md
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 formulaic-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 formulaic-0.6.4/PKG-INFO
```

### Comparing `formulaic-0.6.3/benchmarks/README.md` & `formulaic-0.6.4/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/benchmarks/benchmark.py` & `formulaic-0.6.4/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/benchmarks/benchmarks.csv` & `formulaic-0.6.4/benchmarks/benchmarks.csv`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/benchmarks/benchmarks.png` & `formulaic-0.6.4/benchmarks/benchmarks.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/benchmarks/plot.py` & `formulaic-0.6.4/benchmarks/plot.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/mkdocs.yml` & `formulaic-0.6.4/docsite/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/requirements.txt` & `formulaic-0.6.4/docsite/requirements.txt`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/changelog.md` & `formulaic-0.6.4/docsite/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 For changes since the latest tagged release, please refer to the
 [git commit log](https://github.com/matthewwardrop/formulaic/commits/main).
 
 ---
 
+## 0.6.4 (10 July 2023)
+
+This is a minor release with several new features and cleanups.
+
+**New features and enhancements:**
+
+* Added support for keeping track of the source of variables being used to
+  evaluate a formula. Refer to the `ModelSpec` documentation for more details.
+
+**Bugfixes and cleanups:**
+
+* All functions and methods now have type signatures that are statically checked
+  during unit testing.
+* Removed `OrderedDict` usage, since Python guarantees the orderedness of
+  dictionaries in Python 3.7+.
+* Suppress terms/factors in model matrices for which the factors evaluate to
+  `None`.
+
 ## 0.6.3 (26 June 2023)
 
 This is a minor release with a bugfix.
 
 **Bugfixes and cleanups:**
 
 * Fixed a regression introduced in the previous release when materializing
```

### Comparing `formulaic-0.6.3/docsite/docs/formulas.md` & `formulaic-0.6.4/docsite/docs/formulas.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/index.md` & `formulaic-0.6.4/docsite/docs/index.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/installation.md` & `formulaic-0.6.4/docsite/docs/installation.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/migration.md` & `formulaic-0.6.4/docsite/docs/migration.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/assets/images/favicon.png` & `formulaic-0.6.4/docsite/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/assets/images/logo.png` & `formulaic-0.6.4/docsite/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/assets/images/logo.svg` & `formulaic-0.6.4/docsite/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/assets/images/logo_with_text.png` & `formulaic-0.6.4/docsite/docs/assets/images/logo_with_text.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/concepts/index.md` & `formulaic-0.6.4/docsite/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/guides/contrasts.ipynb` & `formulaic-0.6.4/docsite/docs/guides/contrasts.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/guides/formulae.ipynb` & `formulaic-0.6.4/docsite/docs/guides/formulae.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/guides/grammar.md` & `formulaic-0.6.4/docsite/docs/guides/grammar.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/guides/integration.ipynb` & `formulaic-0.6.4/docsite/docs/guides/integration.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/guides/model_specs.ipynb` & `formulaic-0.6.4/docsite/docs/guides/model_specs.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996433452580445%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(47, '    * **term_variables**: An order mapping of `Term` "*

 * *            "instances to `Variable`\\n'), (48, '        instances (a string subclass with "*

 * *            "addition attributes of `roles` and \\n'), (49, '        `source`), indicating the "*

 * *            "variables used by that term.\\n'), (50, '    * **variable_terms**: The reverse lookup "*

 * *            "of the above.\\n'), (51, '    * **variable_indices**: A mapping from `Variable` "*

 * *            "instance to th […]*

```diff
@@ -83,14 +83,25 @@
                 "    * **terms**: A sequence of `Term` instances that were used to generate this\n",
                 "        model matrix.\n",
                 "    * **term_indices**: An ordered mapping of `Term` instances to the generated\n",
                 "        column indices.\n",
                 "    * **term_slices**: An ordered mapping of `Term` instances to a slice that \n",
                 "        when used on the columns of the model matrix will subsample the model\n",
                 "        matrix down to those corresponding to each term.\n",
+                "    * **term_variables**: An order mapping of `Term` instances to `Variable`\n",
+                "        instances (a string subclass with addition attributes of `roles` and \n",
+                "        `source`), indicating the variables used by that term.\n",
+                "    * **variable_terms**: The reverse lookup of the above.\n",
+                "    * **variable_indices**: A mapping from `Variable` instance to the indices\n",
+                "        of the columns in the model matrix that variable.\n",
+                "    * **variables**: A set of `Variable` instances describing the variables\n",
+                "        used in entire formula.\n",
+                "    * **variables_by_source**: A mapping from source name (typically one of \n",
+                "        `\"data\"`, `\"context\"`, or `\"transforms\"`) to the variables derived from\n",
+                "        that source.\n",
                 "* Utility methods:\n",
                 "    * **get_model_matrix(...)**: Build a model matrix using this spec. This \n",
                 "        allows a new dataset to be generated using exactly the same encoding \n",
                 "        process as an earlier dataset.\n",
                 "    * **get_linear_constraints(...)**: Build a set of linear constraints for use\n",
                 "        during constrained linear regressions.\n",
                 "    * **get_slice(...)**: Build a slice instance that can subset a matrix down \n",
@@ -223,23 +234,25 @@
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'column_names': ('Intercept', 'center(a)', 'b[T.B]', 'b[T.C]'),\n",
-                            " 'column_indices': OrderedDict([('Intercept', 0),\n",
-                            "              ('center(a)', 1),\n",
-                            "              ('b[T.B]', 2),\n",
-                            "              ('b[T.C]', 3)]),\n",
+                            " 'column_indices': {'Intercept': 0, 'center(a)': 1, 'b[T.B]': 2, 'b[T.C]': 3},\n",
                             " 'terms': [1, center(a), b],\n",
-                            " 'term_indices': OrderedDict([(1, [0]), (center(a), [1]), (b, [2, 3])]),\n",
-                            " 'term_slices': OrderedDict([(1, slice(0, 1, None)),\n",
-                            "              (center(a), slice(1, 2, None)),\n",
-                            "              (b, slice(2, 4, None))])}"
+                            " 'term_indices': {1: [0], center(a): [1], b: [2, 3]},\n",
+                            " 'term_slices': {1: slice(0, 1, None),\n",
+                            "  center(a): slice(1, 2, None),\n",
+                            "  b: slice(2, 4, None)},\n",
+                            " 'term_variables': {1: set(), center(a): {'a', 'center'}, b: {'b'}},\n",
+                            " 'variable_terms': {'center': {center(a)}, 'a': {center(a)}, 'b': {b}},\n",
+                            " 'variable_indices': {'center': [1], 'a': [1], 'b': [2, 3]},\n",
+                            " 'variables': {'a', 'b', 'center'},\n",
+                            " 'variables_by_source': {'data': {'a', 'b'}, 'transforms': {'center'}}}"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -247,14 +260,19 @@
                 "# We can now interrogate it for various column and term related metadata\n",
                 "{\n",
                 "    \"column_names\": ms.column_names,\n",
                 "    \"column_indices\": ms.column_indices,\n",
                 "    \"terms\": ms.terms,\n",
                 "    \"term_indices\": ms.term_indices,\n",
                 "    \"term_slices\": ms.term_slices,\n",
+                "    \"term_variables\": ms.term_variables,\n",
+                "    \"variable_terms\": ms.variable_terms,\n",
+                "    \"variable_indices\": ms.variable_indices,\n",
+                "    \"variables\": ms.variables,\n",
+                "    \"variables_by_source\": ms.variables_by_source,\n",
                 "}"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
@@ -418,15 +436,15 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/home/matthew/Repositories/github/formulaic/formulaic/transforms/contrasts.py:124: DataMismatchWarning: Data has categories outside of the nominated levels (or that were not seen in original dataset): {'D'}. They are being  cast to nan, which will likely skew the results of your analyses.\n",
+                        "/home/matthew/Repositories/github/formulaic/formulaic/transforms/contrasts.py:155: DataMismatchWarning: Data has categories outside of the nominated levels (or that were not seen in original dataset): {'D'}. They are being  cast to nan, which will likely skew the results of your analyses.\n",
                         "  warnings.warn(\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
```

### Comparing `formulaic-0.6.3/docsite/docs/guides/quickstart.ipynb` & `formulaic-0.6.4/docsite/docs/guides/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/guides/splines.ipynb` & `formulaic-0.6.4/docsite/docs/guides/splines.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/docsite/docs/guides/transforms.ipynb` & `formulaic-0.6.4/docsite/docs/guides/transforms.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/formulaic/__init__.py` & `formulaic-0.6.4/formulaic/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .model_spec import ModelSpec, ModelSpecs
 from .sugar import model_matrix
 
 try:
     from ._version import __version__, __version_tuple__
 except ImportError:  # pragma: no cover
     __version__ = version = "unknown"
-    __version_tuple__ = version_tuple = ("unknown",)
+    __version_tuple__ = version_tuple = ("unknown",)  # type: ignore
 
 __author__ = "Matthew Wardrop"
 __author_email__ = "mpwardrop@gmail.com"
 
 __all__ = [
     "__author__",
     "__author_email__",
```

### Comparing `formulaic-0.6.3/formulaic/errors.py` & `formulaic-0.6.4/formulaic/errors.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/formulaic/formula.py` & `formulaic-0.6.4/formulaic/formula.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import warnings
 from enum import Enum
-from typing import Any, Dict, List, Mapping, Optional, Set, Tuple, Union
+from typing import Any, Callable, Dict, List, Mapping, Optional, Set, Tuple, Union, cast
 
 from typing_extensions import TypeAlias
 
 from .errors import FormulaInvalidError
 from .model_matrix import ModelMatrix
 from .parser import DefaultFormulaParser
 from .parser.types import FormulaParser, OrderedSet, Structured, Term
@@ -117,56 +117,57 @@
             return spec
         return Formula(
             spec, _parser=parser, _nested_parser=nested_parser, _ordering=ordering
         )
 
     def __init__(
         self,
-        *args,
+        *args: FormulaSpec,
         _parser: Optional[FormulaParser] = None,
         _nested_parser: Optional[FormulaParser] = None,
         _ordering: Union[OrderingMethod, str] = OrderingMethod.DEGREE,
-        **kwargs,
+        **kwargs: Any,
     ):
         self._parser = _parser or self.DEFAULT_PARSER
         self._nested_parser = _nested_parser or _parser or self.DEFAULT_NESTED_PARSER
         self._ordering = OrderingMethod(_ordering)
         super().__init__(*args, **kwargs)
         self._simplify(unwrap=False, inplace=True)
 
-    def _prepare_item(self, key: str, item: FormulaSpec) -> Union[List[Term], Formula]:
+    def _prepare_item(self, key: str, item: FormulaSpec) -> Union[List[Term], Formula]:  # type: ignore[override]
         """
         Convert incoming formula items into either a list of Terms or a nested
         `Formula` instance.
 
         Note: Where parsing of strings is required, the nested-parser is used
         except for the root element of the parent formula.
 
         Args:
             key: The structural key where the item will be stored.
             item: The specification to convert.
         """
 
         if isinstance(item, str):
-            item = (
+            item = cast(
+                FormulaSpec,
                 (self._parser if key == "root" else self._nested_parser)
                 .get_terms(item)
-                ._simplify()
+                ._simplify(),
             )
 
         if isinstance(item, Structured):
             formula_or_terms = Formula(
                 _parser=self._nested_parser, **item._structure
             )._simplify()
         elif isinstance(item, (list, set, OrderedSet)):
             formula_or_terms = [
                 term
                 for value in item
                 for term in (
-                    self._nested_parser.get_terms(value)
+                    self._nested_parser.get_terms(value)  # type: ignore[attr-defined]
                     if isinstance(value, str)
                     else [value]
                 )
             ]
             self.__validate_terms(formula_or_terms)
         else:
             raise FormulaInvalidError(
@@ -184,18 +185,18 @@
 
         if orderer is not None:
             if isinstance(formula_or_terms, Structured):
                 formula_or_terms = formula_or_terms._map(orderer)
             else:
                 formula_or_terms = orderer(formula_or_terms)
 
-        return formula_or_terms
+        return cast(Union[List[Term], Formula], formula_or_terms)
 
     @classmethod
-    def __validate_terms(cls, formula_or_terms: Any):
+    def __validate_terms(cls, formula_or_terms: Any) -> None:
         """
         Verify that all terms are of the appropriate type. The acceptable types
         are:
             - List[Terms]
             - Tuple[List[Terms], ...]
             - Formula
         """
@@ -207,15 +208,18 @@
         for term in formula_or_terms:
             if not isinstance(term, Term):
                 raise FormulaInvalidError(
                     f"All terms in formula should be instances of `formulaic.parser.types.Term`; received term {repr(term)} of type `{type(term)}`."
                 )
 
     def get_model_matrix(
-        self, data: Any, context: Optional[Mapping[str, Any]] = None, **spec_overrides
+        self,
+        data: Any,
+        context: Optional[Mapping[str, Any]] = None,
+        **spec_overrides: Any,
     ) -> Union[ModelMatrix, Structured[ModelMatrix]]:
         """
         Build the model matrix (or matrices) realisation of this formula for the
         nominated `data`.
 
         Args:
             data: The data for which to build the model matrices.
@@ -228,58 +232,61 @@
 
         return ModelSpec.from_spec(self, **spec_overrides).get_model_matrix(
             data, context=context
         )
 
     def differentiate(  # pylint: disable=redefined-builtin
         self,
-        *vars: Tuple[str, ...],
+        *wrt: str,
         use_sympy: bool = False,
     ) -> Formula:
         """
         EXPERIMENTAL: Take the gradient of this formula. When used a linear
         regression, evaluating a trained model on model matrices generated by
         this formula is equivalent to estimating the gradient of that fitted
-        form with respect to `vars`.
+        form with respect to `wrt`.
 
         Args:
-            vars: The variables with respect to which the gradient should be
+            wrt: The variables with respect to which the gradient should be
                 taken.
             use_sympy: Whether to use sympy to perform symbolic differentiation.
 
 
         Notes:
             This method is provisional and may be removed in any future major
             version.
         """
-        return self._map(
-            lambda terms: [
-                differentiate_term(term, vars, use_sympy=use_sympy) for term in terms
-            ]
+        return cast(
+            Formula,
+            self._map(
+                lambda terms: [
+                    differentiate_term(term, wrt, use_sympy=use_sympy) for term in terms
+                ]
+            ),
         )
 
     @property
     def terms(self) -> Formula:
         warnings.warn(
             "`Formula.terms` is deprecated. Please index/iterate over `Formula` directly instead.",
             DeprecationWarning,
         )
         return self
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> Any:
         # Keep substructures wrapped to retain access to helper functions.
         subformula = super().__getattr__(attr)
         if attr != "root":
             return Formula.from_spec(subformula)
         return subformula
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: Any) -> Any:
         # Keep substructures wrapped to retain access to helper functions.
         subformula = super().__getitem__(key)
         if key != "root":
             return Formula.from_spec(subformula)
         return subformula
 
-    def __repr__(self, to_str: bool = False):
+    def __repr__(self, to_str: Callable[..., str] = repr) -> str:
         if not self._has_structure and self._has_root:
             return " + ".join([str(t) for t in self])
         return str(self._map(lambda terms: " + ".join([str(t) for t in terms])))
```

### Comparing `formulaic-0.6.3/formulaic/model_matrix.py` & `formulaic-0.6.4/formulaic/model_matrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import copy
-from typing import Any, Generic, Optional, TypeVar, TYPE_CHECKING
+from typing import Any, Generic, Optional, TypeVar, TYPE_CHECKING, cast
 
 import wrapt
 
 from formulaic.parser.types.structured import Structured
 
 if TYPE_CHECKING:  # pragma: no cover
     from .model_spec import ModelSpec, ModelSpecs
@@ -37,23 +37,23 @@
         This `ModelSpec` instance can be used to create other `ModelMatrix`s
         that respect all the choices (including feature selection and encoding)
         that were made in the construction of this `ModelMatrix` instance.
 
         """
         return self._self_model_spec
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.__wrapped__.__repr__()  # pragma: no cover
 
     # Handle copying behaviour
 
-    def __copy__(self):
+    def __copy__(self) -> ModelMatrix[MatrixType]:
         return type(self)(copy.copy(self.__wrapped__), spec=self._self_model_spec)
 
-    def __deepcopy__(self, memo=None):
+    def __deepcopy__(self, memo: Any = None) -> ModelMatrix[MatrixType]:
         return type(self)(
             copy.deepcopy(self.__wrapped__, memo),
             spec=copy.deepcopy(self._self_model_spec),
         )
 
 
 class ModelMatrices(Structured[ModelMatrix]):
@@ -81,10 +81,11 @@
         """
         The `ModelSpecs` instance representing the structured set of `ModelSpec`
         instances associated with the `ModelMatrix` instances stored in this
         `Structured` instance.
         """
         from .model_spec import ModelSpecs
 
-        return self._map(
-            lambda model_matrix: model_matrix.model_spec, as_type=ModelSpecs
+        return cast(
+            ModelSpecs,
+            self._map(lambda model_matrix: model_matrix.model_spec, as_type=ModelSpecs),
         )
```

### Comparing `formulaic-0.6.3/formulaic/model_spec.py` & `formulaic-0.6.4/formulaic/model_spec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from __future__ import annotations
 
 import warnings
-from collections import OrderedDict
+from collections import defaultdict
 from dataclasses import dataclass, field, replace
 from typing import (
     Any,
     Dict,
     List,
     Mapping,
     Optional,
     Sequence,
-    Tuple,
+    Set,
     Union,
     TYPE_CHECKING,
+    cast,
 )
 
 from formulaic.materializers.base import EncodedTermStructure
 from formulaic.parser.types import Structured, Term
 from formulaic.utils.constraints import LinearConstraintSpec, LinearConstraints
+from formulaic.utils.variables import Variable
 
 from .formula import Formula, FormulaSpec
 from .materializers import FormulaMaterializer, NAAction, ClusterBy
 
 if TYPE_CHECKING:  # pragma: no cover
     from .model_matrix import ModelMatrices, ModelMatrix
 
 # Cached property was introduced in Python 3.8 (we currently support 3.7)
 try:
     from functools import cached_property
 except ImportError:  # pragma: no cover
-    from cached_property import cached_property
+    from cached_property import cached_property  # type: ignore
 
 
 @dataclass(frozen=True)
 class ModelSpec:
     """
     A container for the metadata used to generate a `ModelMatrix` instance.
 
@@ -61,87 +63,100 @@
 
         State (these attributes are only populated during materialization):
             structure: The model matrix structure resulting from materialization.
             transform_state: The state of any stateful transformations that took
                 place during factor evaluation.
             encoder_state: The state of any stateful transformations that took
                 place during encoding.
+
+    Class attributes:
+        SENTINEL: Can be used as a default fallback in signatures (e.g. stateful
+            transforms) to aid in typing. Must not be modified.
     """
 
     @classmethod
     def from_spec(
         cls,
         spec: Union[FormulaSpec, ModelMatrix, ModelMatrices, ModelSpec, ModelSpecs],
-        **attrs,
+        **attrs: Any,
     ) -> Union[ModelSpec, ModelSpecs]:
         """
         Construct a `ModelSpec` (or `Structured[ModelSpec]`) instance for the
         nominated `spec`, setting and/or overriding any `ModelSpec` attributes
         present in `attrs`.
 
         Args:
             spec: The specification for which to generate a `ModelSpec`
                 instance or structured set of `ModelSpec` instances.
             attrs: Any `ModelSpec` attributes to set and/or override on all
                 generated `ModelSpec` instances.
         """
         from .model_matrix import ModelMatrix
 
-        def prepare_model_spec(obj):
+        def prepare_model_spec(obj: Any) -> ModelSpec:
             if isinstance(obj, ModelMatrix):
                 obj = obj.model_spec
             if isinstance(obj, ModelSpec):
                 return obj.update(**attrs)
             formula = Formula.from_spec(obj)
             if not formula._has_root or formula._has_structure:
-                return formula._map(prepare_model_spec, as_type=ModelSpecs)
+                return cast(
+                    ModelSpec, formula._map(prepare_model_spec, as_type=ModelSpecs)
+                )
             return ModelSpec(formula=formula, **attrs)
 
         if isinstance(spec, Formula) or not isinstance(spec, Structured):
             return prepare_model_spec(spec)
-        return spec._map(prepare_model_spec, as_type=ModelSpecs)
+        return cast(ModelSpecs, spec._map(prepare_model_spec, as_type=ModelSpecs))
 
     # Configuration attributes
     formula: Formula
     materializer: Optional[str] = None
     materializer_params: Optional[Dict[str, Any]] = None
     ensure_full_rank: bool = True
-    na_action: NAAction = "drop"
+    na_action: NAAction = NAAction.DROP
     output: Optional[str] = None
-    cluster_by: ClusterBy = "none"
+    cluster_by: ClusterBy = ClusterBy.NONE
 
     # State attributes
     structure: Optional[List[EncodedTermStructure]] = None
     transform_state: Dict = field(default_factory=dict)
     encoder_state: Dict = field(default_factory=dict)
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.__dict__["formula"] = Formula.from_spec(self.formula)
 
         if not self.formula._has_root or self.formula._has_structure:
             raise ValueError(
                 "Nominated `Formula` instance has structure, which is not permitted when attaching to a `ModelSpec` instance."
             )
 
         # Materializer
         if self.materializer is not None and not isinstance(self.materializer, str):
             self.__dict__["materializer"] = FormulaMaterializer.for_materializer(
                 self.materializer
             ).REGISTER_NAME
 
+        # Handle string to enum mapping for values passed in during instantiation
         self.__dict__["na_action"] = NAAction(self.na_action)
         self.__dict__["cluster_by"] = ClusterBy(self.cluster_by)
 
     # Derived features
 
     @cached_property
     def column_names(self) -> Sequence[str]:
         """
         The names associated with the columns of the generated model matrix.
         """
+        if self.structure is None:
+            raise RuntimeError(
+                "`ModelSpec.structure` has not yet been populated. This will "
+                "likely be resolved by using the `ModelSpec` instance attached "
+                "to the model matrix generated when calling `.get_model_matrix()`."
+            )
         return tuple(feature for row in self.structure for feature in row.columns)
 
     @property
     def feature_names(self) -> Sequence[str]:
         """
         A deprecated reference to `ModelSpec.column_names`. Will be removed in
         v1.0.0.
@@ -149,23 +164,23 @@
         warnings.warn(
             "`ModelSpec.feature_names` is deprecated and will be removed in v1.0.0. Use `ModelSpec.column_names` instead.",
             DeprecationWarning,
         )
         return self.column_names
 
     @cached_property
-    def column_indices(self) -> OrderedDict[str, int]:
+    def column_indices(self) -> Dict[str, int]:
         """
         An ordered mapping from column names to the column index in generated
         model matrices.
         """
-        return OrderedDict([(name, i) for i, name in enumerate(self.column_names)])
+        return {name: i for i, name in enumerate(self.column_names)}
 
     @property
-    def feature_indices(self) -> Sequence[str]:
+    def feature_indices(self) -> Dict[str, int]:
         """
         A deprecated reference to `ModelSpec.column_indices`. Will be removed in
         v1.0.0.
         """
         warnings.warn(
             "`ModelSpec.feature_indices` is deprecated and will be removed in v1.0.0. Use `ModelSpec.column_indices` instead.",
             DeprecationWarning,
@@ -177,80 +192,152 @@
         """
         The terms used to generate model matrices from this `ModelSpec`
         instance.
         """
         return self.formula.root
 
     @cached_property
-    def term_indices(self) -> OrderedDict[Term, Tuple[int, ...]]:
+    def term_indices(self) -> Dict[Term, List[int]]:
         """
         An ordered mapping of `Term` instances to the generated column indices.
 
         Note: Since terms hash using their string representation, you can look
         up elements of this mapping using the string representation of the
         `Term`.
         """
-        slices = OrderedDict()
+        if self.structure is None:
+            raise RuntimeError(
+                "`ModelSpec.structure` has not yet been populated. This will "
+                "likely be resolved by using the `ModelSpec` instance attached "
+                "to the model matrix generated when calling `.get_model_matrix()`."
+            )
+        slices = {}
         start = 0
         for row in self.structure:
             end = start + len(row[2])
             slices[row[0]] = list(range(start, end))
             start = end
         return slices
 
     @cached_property
-    def term_slices(self) -> OrderedDict[Term, slice]:
+    def term_slices(self) -> Dict[Term, slice]:
         """
         An ordered mapping of `Term` instances to a slice that when used on
         the columns of the model matrix will subsample the model matrix down to
         those corresponding to each term.
 
         Note: Since terms hash using their string representation, you can look
         up elements of this mapping using the string representation of the
         `Term`.
         """
-        return OrderedDict(
-            {k: slice(v[0], v[-1] + 1) for k, v in self.term_indices.items()}
+        return {k: slice(v[0], v[-1] + 1) for k, v in self.term_indices.items()}
+
+    @cached_property
+    def term_variables(self) -> Dict[Term, Set[Variable]]:
+        """
+        An ordered mapping of `Term` instances to the set of `Variable`
+        instances corresponding to the variables used in the evaluation of that
+        term. `Variable` instances are enriched strings, with the additional
+        attributes `.roles` and `.source`.
+        """
+        if self.structure is None:
+            raise RuntimeError(
+                "`ModelSpec.structure` has not yet been populated. This will "
+                "likely be resolved by using the `ModelSpec` instance attached "
+                "to the model matrix generated when calling `.get_model_matrix()`."
+            )
+        term_variables = {}
+        start = 0
+        for row in self.structure:
+            end = start + len(row[2])
+            term_variables[row[0]] = Variable.union(
+                *(term.variables for term in row[1]),
+            )
+            start = end
+        return term_variables
+
+    @cached_property
+    def variable_terms(self) -> Dict[Variable, Set[Term]]:
+        """
+        A mapping from `Variable` instances to the terms which used it. This is
+        the reverse mapping of `.term_variables`.
+        """
+        variable_terms: Dict[Variable, Set[Term]] = defaultdict(set)
+        for term, variables in self.term_variables.items():
+            for variable in variables:
+                variable_terms[variable].add(term)
+        return dict(variable_terms)
+
+    @cached_property
+    def variable_indices(self) -> Dict[Variable, List[int]]:
+        """
+        A mapping from `Variable` instances to the indices in the model matrix
+        where they were used.
+        """
+        return {
+            variable: sorted(
+                {index for term in terms for index in self.term_indices[term]}
+            )
+            for variable, terms in self.variable_terms.items()
+        }
+
+    @cached_property
+    def variables(self) -> Set[Variable]:
+        return Variable.union(
+            *(variables for variables in self.term_variables.values())
         )
 
+    @cached_property
+    def variables_by_source(self) -> Dict[Optional[str], Set[Variable]]:
+        """
+        A mapping of source name to the set of variables drawn from that source.
+        Formulaic, by default, has three top-level sources of variables:
+        'data', 'transforms', and 'context'.
+        """
+        variables_by_source: Dict[Optional[str], Set[Variable]] = defaultdict(set)
+        for variable in self.variables:
+            variables_by_source[variable.source].add(variable)
+        return dict(variables_by_source)
+
     # Transforms
 
-    def update(self, **kwargs):
+    def update(self, **kwargs: Any) -> ModelSpec:
         """
         Create a copy of this `ModelSpec` instance with the nominated attributes
         mutated.
         """
         return replace(self, **kwargs)
 
-    def differentiate(
-        self, *vars, use_sympy=False  # pylint: disable=redefined-builtin
-    ):
+    def differentiate(self, *wrt: str, use_sympy: bool = False) -> ModelSpec:
         """
         EXPERIMENTAL: Take the gradient of this model spec. When used a linear
         regression, evaluating a trained model on model matrices generated by
         this formula is equivalent to estimating the gradient of that fitted
         form with respect to `vars`.
 
         Args:
-            vars: The variables with respect to which the gradient should be
+            wrt: The variables with respect to which the gradient should be
                 taken.
             use_sympy: Whether to use sympy to perform symbolic differentiation.
 
         Notes:
             This method is provisional and may be removed in any future major
             version.
         """
         return self.update(
-            formula=self.formula.differentiate(*vars, use_sympy=use_sympy),
+            formula=self.formula.differentiate(*wrt, use_sympy=use_sympy),
         )
 
     # Utility methods
 
     def get_model_matrix(
-        self, data: Any, context: Optional[Mapping[str, Any]] = None, **attr_overrides
+        self,
+        data: Any,
+        context: Optional[Mapping[str, Any]] = None,
+        **attr_overrides: Any,
     ) -> ModelMatrix:
         """
         Build the model matrix (or matrices) realisation of this model spec for
         the nominated `data`.
 
         Args:
             data: The data for which to build the model matrices.
@@ -303,27 +390,27 @@
         if isinstance(columns_identifier, Term):
             if columns_identifier not in term_slices:
                 raise ValueError(
                     f"Model matrices built using this spec do not include term: `{columns_identifier}`."
                 )
             return term_slices[columns_identifier]
         if columns_identifier in term_slices:
-            return term_slices[columns_identifier]
+            return term_slices[columns_identifier]  # type: ignore # Terms hash equivalent to their string repr
 
         column_indices = self.column_indices
         if columns_identifier in column_indices:
             idx = column_indices[columns_identifier]
             return slice(idx, idx + 1)
 
         raise ValueError(
             f"Model matrices built using this spec do not have any columns related to: `{repr(columns_identifier)}`."
         )
 
     # Only include dataclass fields when pickling.
-    def __getstate__(self):
+    def __getstate__(self) -> Dict[str, Any]:
         return {
             k: v for k, v in self.__dict__.items() if k in self.__dataclass_fields__
         }
 
 
 class ModelSpecs(Structured[ModelSpec]):
     """
@@ -338,15 +425,18 @@
                 "`ModelSpecs` instances expect all items to be instances of "
                 f"`ModelSpec`. [Got: {repr(item)} of type {repr(type(item))} "
                 f"for key {repr(key)}."
             )
         return item
 
     def get_model_matrix(
-        self, data: Any, context: Optional[Mapping[str, Any]] = None, **attr_overrides
+        self,
+        data: Any,
+        context: Optional[Mapping[str, Any]] = None,
+        **attr_overrides: Any,
     ) -> ModelMatrices:
         """
         This method proxies the `ModelSpec.get_model_matrix(...)` API and allows
         it to be called on a structured set of `ModelSpec` instances. If all
         `ModelSpec.materializer` and `ModelSpec.materializer_params` values are
         unset or the same, then they are jointly evaluated allowing re-use of
         the same cached across the specs.
@@ -390,27 +480,31 @@
             jointly_generate = True
 
         if jointly_generate:
             if materializer is None:
                 materializer = FormulaMaterializer.for_data(data)
             else:
                 materializer = FormulaMaterializer.for_materializer(materializer)
-            return materializer(
+            return materializer(  # type: ignore
                 data, context=context, **(materializer_params or {})
             ).get_model_matrix(self)
 
-        return self._map(
-            lambda model_spec: model_spec.get_model_matrix(data, context=context),
-            as_type=ModelMatrices,
+        return cast(
+            ModelMatrices,
+            self._map(
+                lambda model_spec: model_spec.get_model_matrix(data, context=context),
+                as_type=ModelMatrices,
+            ),
         )
 
-    def differentiate(
-        self, *vars, use_sympy=False  # pylint: disable=redefined-builtin
-    ) -> ModelSpecs:
+    def differentiate(self, *wrt: str, use_sympy: Any = False) -> ModelSpecs:
         """
         This method proxies the experimental `ModelSpec.differentiate(...)` API.
         See `ModelSpec.differentiate` for more details.
         """
-        return self._map(
-            lambda model_spec: model_spec.differentiate(*vars, use_sympy=use_sympy),
-            as_type=ModelSpecs,
+        return cast(
+            ModelSpecs,
+            self._map(
+                lambda model_spec: model_spec.differentiate(*wrt, use_sympy=use_sympy),
+                as_type=ModelSpecs,
+            ),
         )
```

### Comparing `formulaic-0.6.3/formulaic/sugar.py` & `formulaic-0.6.4/formulaic/sugar.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def model_matrix(
     spec: Union[FormulaSpec, ModelMatrix, ModelMatrices, ModelSpec, ModelSpecs],
     data: Any,
     *,
     context: Union[int, Mapping[str, Any]] = 0,
-    **spec_overrides,
+    **spec_overrides: Any,
 ) -> Union[ModelMatrix, ModelMatrices]:
     """
     Generate a model matrix directly from a formula or model spec.
 
     This method is syntactic sugar for:
     ```
     Formula(spec).get_model_matrix(data, context=LayeredMapping(locals(), globals()), **kwargs)
@@ -43,12 +43,11 @@
         spec_overrides: Any `ModelSpec` attributes to set/override. See
             `ModelSpec` for more details.
 
     Returns:
         The data transformed in to the model matrix with the requested
         nominated structure.
     """
-    if isinstance(context, int):
-        context = capture_context(context + 1)
+    _context = capture_context(context + 1) if isinstance(context, int) else context
     return ModelSpec.from_spec(spec, **spec_overrides).get_model_matrix(
-        data, context=context
+        data, context=_context
     )
```

### Comparing `formulaic-0.6.3/formulaic/materializers/arrow.py` & `formulaic-0.6.4/formulaic/materializers/arrow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,45 @@
-from interface_meta import override
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Dict
 
 import pandas
+from interface_meta import override
+
 
 from .pandas import PandasMaterializer
 
+if TYPE_CHECKING:  # pragma: no cover
+    import pyarrow
+
 
 class ArrowMaterializer(PandasMaterializer):
 
     REGISTER_NAME = "arrow"
     REGISTER_INPUTS = ("pyarrow.lib.Table",)
 
     @override
-    def _init(self):
+    def _init(self) -> None:
         self.__data_context = LazyArrowTableProxy(self.data)
 
-    @override
+    @override  # type: ignore
     @property
     def data_context(self):
         return self.__data_context
 
 
 class LazyArrowTableProxy:
-    def __init__(self, table):
+    def __init__(self, table: pyarrow.Table):
         self.table = table
         self.column_names = set(self.table.column_names)
-        self._cache = {}
+        self._cache: Dict[str, pandas.Series] = {}
         self.index = pandas.RangeIndex(len(table))
 
-    def __contains__(self, value):
+    def __contains__(self, value: Any) -> Any:
         return value in self.column_names
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> Any:
         if key not in self.column_names:
             raise KeyError(key)
         if key not in self._cache:
             self._cache[key] = self.table.column(key).to_pandas()
         return self._cache[key]
```

### Comparing `formulaic-0.6.3/formulaic/materializers/base.py` & `formulaic-0.6.4/formulaic/materializers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 from __future__ import annotations
+import ast
 
 import functools
 import inspect
 import itertools
 import operator
 from abc import abstractmethod
-from collections import defaultdict, OrderedDict, namedtuple
+from collections import defaultdict, namedtuple
 from typing import (
     Any,
     Dict,
     Generator,
+    Hashable,
     List,
     Iterable,
+    Mapping,
+    Optional,
+    Sequence,
+    Set,
     Tuple,
+    Type,
     Union,
     TYPE_CHECKING,
+    cast,
 )
 
 from interface_meta import InterfaceMeta, inherit_docs
 
 from formulaic.errors import (
     FactorEncodingError,
     FactorEvaluationError,
     FormulaMaterializationError,
     FormulaMaterializerInvalidError,
     FormulaMaterializerNotFoundError,
 )
-from formulaic.materializers.types.enums import ClusterBy
+from formulaic.materializers.types.enums import ClusterBy, NAAction
 from formulaic.materializers.types.factor_values import FactorValuesMetadata
 from formulaic.model_matrix import ModelMatrices, ModelMatrix
 from formulaic.parser.types import Factor, Term
 from formulaic.parser.types.ordered_set import OrderedSet
 from formulaic.transforms import TRANSFORMS
 from formulaic.utils.cast import as_columns
 from formulaic.utils.layered_mapping import LayeredMapping
 from formulaic.utils.stateful_transforms import stateful_eval
+from formulaic.utils.variables import Variable, get_expression_variables
 
 from .types import EvaluatedFactor, FactorValues, ScopedFactor, ScopedTerm
 
 if TYPE_CHECKING:  # pragma: no cover
     from formulaic import FormulaSpec, ModelSpec, ModelSpecs
 
 
@@ -47,45 +56,47 @@
 )
 
 
 class FormulaMaterializerMeta(InterfaceMeta):
 
     INTERFACE_RAISE_ON_VIOLATION = True
 
-    REGISTERED_NAMES = {}
-    REGISTERED_INPUTS = defaultdict(list)
+    REGISTERED_NAMES: Dict[str, Type[FormulaMaterializer]] = {}
+    REGISTERED_INPUTS: Dict[str, List[Type[FormulaMaterializer]]] = defaultdict(list)
 
-    def __register_implementation__(cls):
+    def __register_implementation__(cls) -> None:
         if "REGISTER_NAME" in cls.__dict__ and cls.REGISTER_NAME:
             cls.REGISTERED_NAMES[cls.REGISTER_NAME] = cls
 
             if "REGISTER_INPUTS" in cls.__dict__:
                 for input_type in cls.REGISTER_INPUTS:
                     cls.REGISTERED_INPUTS[input_type] = sorted(
                         cls.REGISTERED_INPUTS[input_type] + [cls],
                         key=lambda x: x.REGISTER_PRECEDENCE,
                         reverse=True,
                     )
 
-    def for_materializer(cls, materializer):
+    def for_materializer(
+        cls, materializer: Union[str, FormulaMaterializer, Type[FormulaMaterializer]]
+    ) -> Type[FormulaMaterializer]:
         if isinstance(materializer, str):
             if materializer not in cls.REGISTERED_NAMES:
                 raise FormulaMaterializerNotFoundError(materializer)
             return cls.REGISTERED_NAMES[materializer]
         if isinstance(materializer, FormulaMaterializer):
             return type(materializer)
         if not inspect.isclass(materializer) or not issubclass(
             materializer, FormulaMaterializer
         ):
             raise FormulaMaterializerInvalidError(
                 "Materializers must be subclasses of `formulaic.materializers.FormulaMaterializer`."
             )
         return materializer
 
-    def for_data(cls, data, output=None):
+    def for_data(cls, data: Any, output: Hashable = None) -> Type[FormulaMaterializer]:
         datacls = data.__class__
         input_type = f"{datacls.__module__}.{datacls.__qualname__}"
 
         if input_type not in cls.REGISTERED_INPUTS:
             raise FormulaMaterializerNotFoundError(
                 f"No materializer has been registered for input type {repr(input_type)}. Available input types are: {set(cls.REGISTER_INPUTS)}."
             )
@@ -93,66 +104,68 @@
         if output is None:
             return cls.REGISTERED_INPUTS[input_type][0]
 
         for materializer in cls.REGISTERED_INPUTS[input_type]:
             if output in materializer.REGISTER_OUTPUTS:
                 return materializer
 
-        output_types = set(
+        output_types: Set[Hashable] = set(
             *itertools.chain(
                 materializer.REGISTER_OUTPUTS
                 for materializer in cls.REGISTERED_INPUTS[input_type]
             )
         )
         raise FormulaMaterializerNotFoundError(
             f"No materializer has been registered for input type {repr(input_type)} that supports output type {repr(output)}. Available output types for {repr(input_type)} are: {output_types}."
         )
 
 
 class FormulaMaterializer(metaclass=FormulaMaterializerMeta):
 
-    REGISTER_NAME = None
-    REGISTER_INPUTS = set()
-    REGISTER_OUTPUTS = set()
-    REGISTER_PRECEDENCE = 100
+    REGISTER_NAME: Optional[str] = None
+    REGISTER_INPUTS: Sequence[str] = ()
+    REGISTER_OUTPUTS: Sequence[Hashable] = ()
+    REGISTER_PRECEDENCE: float = 100
 
     # Public API
 
     @inherit_docs(method="_init")
-    def __init__(self, data, context=None, **params):
+    def __init__(
+        self, data: Any, context: Optional[Mapping[str, Any]] = None, **params: Any
+    ):
         self.data = data
         self.context = context or {}
         self.params = params
         self._init()
 
         self.layered_context = LayeredMapping(
             LayeredMapping(self.data_context, name="data"),
             LayeredMapping(self.context, name="context"),
             LayeredMapping(TRANSFORMS, name="transforms"),
         )
 
-        self.factor_cache = {}
-        self.encoded_cache = {}
+        self.factor_cache: Dict[str, EvaluatedFactor] = {}
+        self.encoded_cache: Dict[Union[str, Tuple[str, bool]], Any] = {}
 
-    def _init(self):
+    def _init(self) -> None:
         pass  # pragma: no cover
 
     @property
-    def data_context(self):
+    def data_context(self) -> Mapping[str, Any]:
         return self.data
 
     @property
-    def nrows(self):
+    def nrows(self) -> int:
         return len(self.data)
 
     def get_model_matrix(
         self,
         spec: Union[FormulaSpec, ModelMatrix, ModelMatrices, ModelSpec, ModelSpecs],
-        **spec_overrides,
-    ):
+        **spec_overrides: Any,
+    ) -> Union[ModelMatrix, ModelMatrices]:
         from formulaic import ModelSpec
 
         # Prepare ModelSpec(s)
         spec: Union[ModelSpec, ModelSpecs] = ModelSpec.from_spec(spec, **spec_overrides)
         should_simplify = isinstance(spec, ModelSpec)
         model_specs: ModelSpecs = self._prepare_model_specs(spec)
 
@@ -161,18 +174,18 @@
         (
             factors,
             factor_evaluation_model_spec,
         ) = self._prepare_factor_evaluation_model_spec(model_specs)
 
         # Step 1: Evaluate all factors and cache the results, keeping track of
         # which rows need dropping (if `self.config.na_action == 'drop'`).
-        drop_rows = set()
+        drop_rows: Set[int] = set()
         for factor in factors:
             self._evaluate_factor(factor, factor_evaluation_model_spec, drop_rows)
-        drop_rows = sorted(drop_rows)
+        drop_rows: Sequence[int] = sorted(drop_rows)
 
         # Step 2: Update the structured model specs with the information from
         # the shared transform state pool.
         model_specs._map(
             lambda ms: ms.transform_state.update(
                 {
                     factor.expr: factor_evaluation_model_spec.transform_state[
@@ -183,43 +196,48 @@
                     if factor.expr in factor_evaluation_model_spec.transform_state
                 }
             )
         )
 
         # Step 3: Build the model matrices using the shared factor cache, and
         # by recursing over the structured model matrices.
-        model_matrices = model_specs._map(
-            lambda model_spec: self._build_model_matrix(
-                model_spec, drop_rows=drop_rows
+        model_matrices = cast(
+            ModelMatrices,
+            model_specs._map(
+                lambda model_spec: self._build_model_matrix(
+                    model_spec, drop_rows=drop_rows
+                ),
+                as_type=ModelMatrices,
             ),
-            as_type=ModelMatrices,
         )
 
         if should_simplify:
-            return model_matrices._simplify()
+            return cast(Union[ModelMatrix, ModelMatrices], model_matrices._simplify())
         return model_matrices
 
-    def _build_model_matrix(self, spec: ModelSpec, drop_rows):
+    def _build_model_matrix(
+        self, spec: ModelSpec, drop_rows: Sequence[int]
+    ) -> ModelMatrix:
 
         # Step 0: Apply any requested column/term clustering
         # This must happen before Step 1 otherwise the greedy rank reduction
         # below would result in a different outcome than if the columns had
         # always been in the generated order.
-        terms = self._cluster_terms(spec.formula, cluster_by=spec.cluster_by)
+        terms = self._cluster_terms(spec.formula.root, cluster_by=spec.cluster_by)
 
         # Step 1: Determine strategy to maintain structural full-rankness of output matrix
         scoped_terms_for_terms = self._get_scoped_terms(
             terms,
             ensure_full_rank=spec.ensure_full_rank,
         )
 
         # Step 2: Generate the columns which will be collated into the full matrix
         cols = []
         for term, scoped_terms in scoped_terms_for_terms:
-            scoped_cols = OrderedDict()
+            scoped_cols = {}
             for scoped_term in scoped_terms:
                 if not scoped_term.factors:
                     scoped_cols[
                         "Intercept"
                     ] = scoped_term.scale * self._encode_constant(
                         1, None, {}, spec, drop_rows
                     )
@@ -239,15 +257,15 @@
                             scale=scoped_term.scale,
                         )
                     )
             cols.append((term, scoped_terms, scoped_cols))
 
         # Step 3: Populate remaining model spec fields
         if spec.structure:
-            cols = self._enforce_structure(cols, spec, drop_rows)
+            cols = self._enforce_structure(cols, spec, drop_rows)  # type: ignore
         else:
             spec = spec.update(
                 structure=[
                     EncodedTermStructure(
                         term,
                         list(st.copy(without_values=True) for st in scoped_terms),
                         list(scoped_cols),
@@ -274,41 +292,43 @@
 
     def _prepare_model_specs(self, spec: Union[ModelSpec, ModelSpecs]) -> ModelSpecs:
         from formulaic.model_spec import ModelSpecs
 
         if not isinstance(spec, ModelSpecs):
             spec = ModelSpecs(spec)
 
-        def prepare_model_spec(model_spec: ModelSpec):
-            overrides = {
+        def prepare_model_spec(model_spec: ModelSpec) -> ModelSpec:
+            overrides: Dict[str, Any] = {
                 "materializer": self.REGISTER_NAME,
                 "materializer_params": self.params,
             }
 
             if model_spec.output is None:
                 overrides["output"] = self.REGISTER_OUTPUTS[0]
             elif model_spec.output not in self.REGISTER_OUTPUTS:
                 raise FormulaMaterializationError(
                     f"Nominated output {repr(model_spec.output)} is invalid. Available output types are: {set(self.REGISTER_OUTPUTS)}."
                 )
 
             return model_spec.update(**overrides)
 
-        return spec._map(prepare_model_spec, as_type=ModelSpecs)
+        return cast(ModelSpecs, spec._map(prepare_model_spec, as_type=ModelSpecs))
 
-    def _prepare_factor_evaluation_model_spec(self, model_specs: ModelSpecs):
+    def _prepare_factor_evaluation_model_spec(
+        self, model_specs: ModelSpecs
+    ) -> Tuple[Set[Factor], ModelSpec]:
         from formulaic.model_spec import ModelSpec
 
         output = set()
         na_action = set()
         ensure_full_rank = set()
-        factors = set()
+        factors: Set[Factor] = set()
         transform_state = {}
 
-        def update_pooled_spec(model_spec: ModelSpec):
+        def update_pooled_spec(model_spec: ModelSpec) -> None:
             output.add(model_spec.output)
             na_action.add(model_spec.na_action)
             ensure_full_rank.add(model_spec.ensure_full_rank)
             factors.update(
                 itertools.chain(*(term.factors for term in model_spec.formula))
             )
             transform_state.update(
@@ -318,23 +338,28 @@
         model_specs._map(update_pooled_spec)
 
         if len(output) != 1 or len(na_action) != 1 or len(ensure_full_rank) != 1:
             raise RuntimeError(
                 "Provided `ModelSpec` instances are not consistent."
             )  # pragma: no cover; will only occur if users manually construct a structured model spec.
 
-        return factors, ModelSpec(
-            formula=[],
-            ensure_full_rank=next(iter(ensure_full_rank)),
-            na_action=next(iter(na_action)),
-            output=next(iter(output)),
-            transform_state=transform_state,
+        return factors, cast(
+            ModelSpec,
+            ModelSpec.from_spec(
+                [],
+                ensure_full_rank=next(iter(ensure_full_rank)),
+                na_action=next(iter(na_action)),
+                output=next(iter(output)),
+                transform_state=transform_state,
+            ),
         )
 
-    def _cluster_terms(self, terms, cluster_by: ClusterBy = ClusterBy.NONE):
+    def _cluster_terms(
+        self, terms: Sequence[Term], cluster_by: ClusterBy = ClusterBy.NONE
+    ) -> Sequence[Term]:
         if cluster_by is not ClusterBy.NUMERICAL_FACTORS:
             return terms
 
         term_clusters = defaultdict(list)
         for term in terms:
             numerical_factors = tuple(
                 factor
@@ -345,15 +370,17 @@
 
         return [
             term for term_cluster in term_clusters.values() for term in term_cluster
         ]
 
     # Methods related to ensuring out matrices are structurally full-rank
 
-    def _get_scoped_terms(self, terms, ensure_full_rank=True):
+    def _get_scoped_terms(
+        self, terms: Iterable[Term], ensure_full_rank: bool = True
+    ) -> Generator[Tuple[Term, Iterable[ScopedTerm]], None, None]:
         """
         Generate the terms to be used in the model matrix.
 
         This method first evaluates each factor in the context of the data
         (and environment), and then determines the correct "scope" (full vs.
         reduced rank) for each term. If `ensure_full_rank` is `True`, then the
         resulting terms when combined is guaranteed to be structurally full-rank.
@@ -364,25 +391,34 @@
             ensure_full_rank (bool): Whether evaluated terms should be scoped
                 to ensure that their combination will result in a full-rank
                 matrix.
 
         Returns:
             list<ScopedTerm>: A list of appropriately scoped terms.
         """
-        spanned = set()
+        spanned: Set[ScopedTerm] = set()
 
         for term in terms:
-            evaled_factors = [self.factor_cache[factor.expr] for factor in term.factors]
+            evaled_factors = [
+                self.factor_cache[factor.expr]
+                for factor in term.factors
+                if self.factor_cache[factor.expr].values.__wrapped__ is not None
+            ]
+            if not evaled_factors:
+                yield term, []
+                continue
 
             if ensure_full_rank:
                 term_span = (
                     self._get_scoped_terms_spanned_by_evaled_factors(evaled_factors)
                     - spanned
                 )
-                scoped_terms = self._simplify_scoped_terms(term_span)
+                scoped_terms: Iterable[ScopedTerm] = self._simplify_scoped_terms(
+                    term_span
+                )
                 spanned.update(term_span)
             else:
                 scoped_terms = [
                     ScopedTerm(
                         factors=(
                             ScopedFactor(evaled_factor, reduced=False)
                             for evaled_factor in evaled_factors
@@ -414,15 +450,15 @@
             evaled_factors: The evaluated factors for which to generated scoped
                 terms.
 
         Returns:
             The scoped terms for the nominated `evaled_factors`.
         """
         scale = 1
-        factors = []
+        factors: List[Tuple[Union[ScopedFactor, int], ...]] = []
         for factor in evaled_factors:
             if factor.metadata.kind is Factor.Kind.CONSTANT:
                 scale *= factor.values
             elif factor.metadata.spans_intercept:
                 factors.append((ScopedFactor(factor, reduced=True), 1))
             else:
                 factors.append((ScopedFactor(factor),))
@@ -430,78 +466,82 @@
             ScopedTerm(factors=(p for p in prod if p != 1), scale=scale)
             for prod in itertools.product(*factors)
         )
 
     @classmethod
     def _simplify_scoped_terms(
         cls, scoped_terms: Iterable[ScopedTerm]
-    ) -> Iterable[ScopedTerm]:
+    ) -> OrderedSet[ScopedTerm]:
         """
         Return the minimal set of ScopedTerm instances that spans the same
         vectorspace, matching as closely as possible the intended order of the
         terms.
 
         This is an iterative algorithm that applies the rule:
             (anything):(reduced rank) + (anything) |-> (anything):(full rank)
         To be safe, we recurse whenever we apply the rule to make sure that
         we have fully simplified the set of terms before adding new ones.
 
         This is guaranteed to minimially span the vector space, keeping
         everything full-rank by avoiding overlaps.
         """
-        terms = OrderedSet()
+        terms: OrderedSet[ScopedTerm] = OrderedSet()
         for scoped_term in sorted(scoped_terms, key=lambda x: len(x.factors)):
             factors = set(scoped_term.factors)
             combined = False
             for existing_term in terms:
                 # Check whether existing term only differs by one factor
                 cofactors = set(existing_term.factors)
                 factors_diff = factors - cofactors
                 if len(factors) - 1 != len(cofactors) or len(factors_diff) != 1:
                     continue
                 # If the different factor is a reduced factor, we can apply the
                 # rule and recurse to see if there is anything else to pick up.
                 factor_new = next(iter(factors_diff))
                 if factor_new.reduced:
                     terms = cls._simplify_scoped_terms(
-                        terms - (existing_term,)
-                        | (
+                        terms - (existing_term,)  # type: ignore
+                        | (  # type: ignore
                             ScopedTerm(
                                 (
                                     ScopedFactor(factor_new.factor, reduced=False)
                                     if factor == factor_new
                                     else factor
                                     for factor in scoped_term.factors
                                 ),
                                 scale=existing_term.scale * scoped_term.scale,
                             ),
                         )
                     )
                     combined = True
                     break
             if not combined:
-                terms = terms | (scoped_term,)
+                terms = terms | (scoped_term,)  # type: ignore
         return terms
 
     # Methods related to looking-up, evaluating and encoding terms and factors
 
     def _evaluate_factor(
-        self, factor: Factor, spec: ModelSpec, drop_rows: set
+        self, factor: Factor, spec: ModelSpec, drop_rows: Set[int]
     ) -> EvaluatedFactor:
         if factor.expr not in self.factor_cache:
             try:
                 if factor.eval_method.value == "lookup":
-                    value = self._lookup(factor.expr)
+                    value, variables = self._lookup(factor.expr)
                 elif factor.eval_method.value == "python":
-                    value = self._evaluate(factor.expr, factor.metadata, spec)
+                    value, variables = self._evaluate(
+                        factor.expr, factor.metadata, spec
+                    )
                 elif factor.eval_method.value == "literal":
                     value = FactorValues(
-                        self._evaluate(factor.expr, factor.metadata, spec),
+                        ast.literal_eval(factor.expr),
+                        # self._evaluate(factor.expr, factor.metadata, spec),
                         kind=Factor.Kind.CONSTANT,
                     )
+                    variables = None
                 else:  # pragma: no cover; future proofing against new eval methods
                     raise FactorEvaluationError(
                         f"The evaluation method `{factor.eval_method.value}` for factor `{factor}` is not understood."
                     )
             except FactorEvaluationError:  # pragma: no cover; future proofing against new eval methods
                 raise
             except Exception as e:
@@ -541,58 +581,76 @@
                 raise FactorEncodingError(
                     f"The model specification expects factor `{factor}` to have values of kind "
                     f"`{spec.encoder_state[factor.expr][0]}`, but they are actually of kind "
                     f"`{value.__formulaic_metadata__.kind.value}`."
                 )
             self._check_for_nulls(factor.expr, value, spec.na_action, drop_rows)
             self.factor_cache[factor.expr] = EvaluatedFactor(
-                factor=factor, values=value
+                factor=factor, values=value, variables=variables
             )
         return self.factor_cache[factor.expr]
 
-    def _lookup(self, name):
-        return self.layered_context[name]
-
-    def _evaluate(self, expr, metadata, spec):
-        return stateful_eval(
-            expr, self.layered_context, {expr: metadata}, spec.transform_state, spec
+    def _lookup(self, name: str) -> Tuple[Any, Set[Variable]]:
+        values, layer = self.layered_context.get_with_layer_name(name)
+        return values, {Variable(name, roles=("value",), source=layer)}
+
+    def _evaluate(
+        self, expr: str, metadata: Any, spec: ModelSpec
+    ) -> Tuple[Any, Set[Variable]]:
+        return (
+            stateful_eval(
+                expr,
+                self.layered_context,
+                {expr: metadata},
+                spec.transform_state,
+                spec,
+            ),
+            get_expression_variables(expr, self.layered_context),
         )
 
-    def _is_categorical(self, values):
+    def _is_categorical(self, values: Any) -> bool:
         if hasattr(values, "__formulaic_metadata__"):
             return values.__formulaic_metadata__.kind is Factor.Kind.CATEGORICAL
         return False
 
-    def _check_for_nulls(self, name, values, na_action, drop_rows):
+    def _check_for_nulls(
+        self, name: str, values: Any, na_action: NAAction, drop_rows: Set[int]
+    ) -> None:
         pass  # pragma: no cover
 
     def _encode_evaled_factor(
         self,
         factor: EvaluatedFactor,
         spec: ModelSpec,
-        drop_rows: set,
+        drop_rows: Sequence[int],
         reduced_rank: bool = False,
     ) -> Dict[str, Any]:
         if not factor.metadata.encoded:
             if factor.expr in self.encoded_cache:
                 encoded = self.encoded_cache[factor.expr]
             elif (factor.expr, reduced_rank) in self.encoded_cache:
                 encoded = self.encoded_cache[(factor.expr, reduced_rank)]
             else:
 
-                def map_dict(f):
+                def map_dict(f: Any) -> Any:
                     """
                     This decorator allows an encoding function to operator on
                     dictionaries (which should be mapped over). This allows
                     transforms to output multiple non-encoded columns and still
                     have everything work as expected.
                     """
 
                     @functools.wraps(f)
-                    def wrapped(values, metadata, state, *args, **kwargs):
+                    def wrapped(
+                        values: Any,
+                        metadata: Any,
+                        state: Dict[str, Any],
+                        *args: Any,
+                        **kwargs: Any,
+                    ) -> Any:
                         if isinstance(values, dict):
                             encoded = {}
                             for k, v in values.items():
                                 if isinstance(k, str) and k.startswith("__"):
                                     encoded[k] = v
                                 else:
                                     nested_state = state.get(k, {})
@@ -606,30 +664,32 @@
                                     encoded, metadata=values.__formulaic_metadata__
                                 )
                             return encoded  # pragma: no cover; nothing in formulaic uses this, but is here for generality.
                         return f(values, metadata, state, *args, **kwargs)
 
                     return wrapped
 
-                encoder_state = spec.encoder_state.get(factor.expr, [None, {}])[1]
+                encoder_state: Dict[str, Any] = spec.encoder_state.get(
+                    factor.expr, [None, {}]
+                )[1]
 
                 if factor.metadata.encoder is not None:
                     encoded = as_columns(
-                        factor.metadata.encoder(
+                        factor.metadata.encoder(  # type: ignore
                             factor.values,
                             reduced_rank=reduced_rank,
                             drop_rows=drop_rows,
                             encoder_state=encoder_state,
                             model_spec=spec,
                         )
                     )
                 else:
                     # If we need to unpack values into columns, we do this here.
                     # Otherwise, we pass through the original values.
-                    factor_values = FactorValues(
+                    factor_values: FactorValues = FactorValues(
                         self._extract_columns_for_encoding(factor),
                         metadata=factor.metadata,
                     )
 
                     if factor.metadata.kind is Factor.Kind.CATEGORICAL:
                         encoded = map_dict(self._encode_categorical)(
                             factor_values,
@@ -659,19 +719,19 @@
                         raise FactorEncodingError(
                             factor
                         )  # pragma: no cover; it is not currently possible to reach this sentinel
                 spec.encoder_state[factor.expr] = (factor.metadata.kind, encoder_state)
 
                 # Only encode once for encodings where we can just drop a field
                 # later on below.
-                if isinstance(encoded, dict) and factor.metadata.drop_field:
-                    cache_key = factor.expr
-                else:
-                    cache_key = (factor.expr, reduced_rank)
-
+                cache_key: Union[str, Tuple[str, bool]] = (
+                    factor.expr
+                    if isinstance(encoded, dict) and factor.metadata.drop_field
+                    else (factor.expr, reduced_rank)
+                )
                 self.encoded_cache[cache_key] = encoded
         else:
             encoded = as_columns(
                 factor.values
             )  # pragma: no cover; we don't use this in formulaic yet.
 
         encoded = FactorValues(
@@ -679,19 +739,19 @@
             metadata=getattr(encoded, "__formulaic_metadata__", factor.metadata),
             encoded=True,
         )
 
         # Encoded factors will now all be dicts
         if (
             isinstance(encoded, dict)
-            and encoded.__formulaic_metadata__.spans_intercept
+            and encoded.__formulaic_metadata__.spans_intercept  # type: ignore
             and reduced_rank
         ):
             encoded = FactorValues(
-                encoded.copy(), metadata=encoded.__formulaic_metadata__
+                encoded.copy(), metadata=encoded.__formulaic_metadata__  # type: ignore
             )
             del encoded[encoded.__formulaic_metadata__.drop_field]
 
         return self._flatten_encoded_evaled_factor(factor.expr, encoded)
 
     def _extract_columns_for_encoding(
         self, factor: EvaluatedFactor
@@ -718,54 +778,75 @@
 
         flattened = {}
         for subfield, value in values.items():
             if isinstance(subfield, str) and subfield.startswith("__"):
                 continue
             subname = name_format.format(name=name, field=subfield)
             if isinstance(value, dict):
-                flattened.update(self._flatten_encoded_evaled_factor(subname, value))
+                flattened.update(self._flatten_encoded_evaled_factor(subname, value))  # type: ignore
             else:
                 flattened[subname] = value
 
         return flattened
 
     @abstractmethod
-    def _encode_constant(self, value, metadata, encoder_state, spec, drop_rows):
+    def _encode_constant(
+        self,
+        value: Any,
+        metadata: Any,
+        encoder_state: Dict[str, Any],
+        spec: ModelSpec,
+        drop_rows: Sequence[int],
+    ) -> Any:
         pass  # pragma: no cover
 
     @abstractmethod
     def _encode_categorical(
-        self, values, metadata, encoder_state, spec, drop_rows, reduced_rank=False
-    ):
+        self,
+        values: Any,
+        metadata: Any,
+        encoder_state: Dict[str, Any],
+        spec: ModelSpec,
+        drop_rows: Sequence[int],
+        reduced_rank: bool = False,
+    ) -> None:
         pass  # pragma: no cover
 
     @abstractmethod
-    def _encode_numerical(self, values, metadata, encoder_state, spec, drop_rows):
+    def _encode_numerical(
+        self,
+        values: Any,
+        metadata: Any,
+        encoder_state: Dict[str, Any],
+        spec: ModelSpec,
+        drop_rows: Sequence[int],
+    ) -> Any:
         pass  # pragma: no cover
 
     # Methods related to ModelMatrix output
 
     def _enforce_structure(
         self,
         cols: List[Tuple[Term, List[ScopedTerm], Dict[str, Any]]],
-        spec,
-        drop_rows: set,
-    ) -> Generator[Tuple[Term, List[ScopedTerm], Dict[str, Any]]]:
+        spec: ModelSpec,
+        drop_rows: Sequence[int],
+    ) -> Generator[Tuple[Term, List[ScopedTerm], Dict[str, Any]], None, None]:
         # TODO: Verify that imputation strategies are intuitive and make sense.
-        assert len(cols) == len(spec.structure)
+        structure = cast(List[EncodedTermStructure], spec.structure)
+        assert len(cols) == len(structure)
         for i, col_spec in enumerate(cols):
             scoped_cols = col_spec[2]
-            target_cols = spec.structure[i][2]
+            target_cols = structure[i][2]
             if len(scoped_cols) > len(target_cols):
                 raise FactorEncodingError(
                     f"Term `{col_spec[0]}` has generated too many columns compared to specification: generated {list(scoped_cols)}, expecting {target_cols}."
                 )
             if len(scoped_cols) < len(target_cols):
                 if len(scoped_cols) == 0:
-                    col = self._encode_constant(0, None, None, spec, drop_rows)
+                    col = self._encode_constant(0, None, {}, spec, drop_rows)
                 elif len(scoped_cols) == 1:
                     col = tuple(scoped_cols.values())[0]
                 else:
                     raise FactorEncodingError(
                         f"Term `{col_spec[0]}` has generated insufficient columns compared to specification: generated {list(scoped_cols)}, expecting {target_cols}."
                     )
                 scoped_cols = {name: col for name in target_cols}
@@ -774,35 +855,39 @@
                     f"Term `{col_spec[0]}` has generated columns that are inconsistent with specification: generated {list(scoped_cols)}, expecting {target_cols}."
                 )
 
             yield col_spec[0], col_spec[1], {
                 col: scoped_cols[col] for col in target_cols
             }
 
-    def _get_columns_for_term(self, factors, spec, scale=1):
+    def _get_columns_for_term(
+        self, factors: List[Dict[str, Any]], spec: ModelSpec, scale: float = 1
+    ) -> Dict[str, Any]:
         """
         Assemble the columns for a model matrix given factors and a scale.
 
         This performs the row-wise Kronecker product of the factors. For greater
         compatibility with R and patsy, we reverse this product so that we
         iterate first over the latter terms.
 
         Args:
             factors
             scale
 
         Returns:
             dict
         """
-        out = OrderedDict()
+        out = {}
         for reverse_product in itertools.product(
             *(factor.items() for factor in reversed(factors))
         ):
             product = reverse_product[::-1]
             out[":".join(p[0] for p in product)] = scale * functools.reduce(
                 operator.mul, (p[1] for p in product)
             )
         return out
 
     @abstractmethod
-    def _combine_columns(self, cols, spec, drop_rows):
+    def _combine_columns(
+        self, cols: Sequence[Tuple[str, Any]], spec: ModelSpec, drop_rows: Sequence[int]
+    ) -> Any:
         pass  # pragma: no cover
```

### Comparing `formulaic-0.6.3/formulaic/materializers/pandas.py` & `formulaic-0.6.4/formulaic/materializers/pandas.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,44 @@
+from __future__ import annotations
+
 import functools
 import itertools
-from collections import OrderedDict
+from typing import Any, Dict, List, Sequence, Set, Tuple, cast, TYPE_CHECKING
 
 import numpy
 import pandas
 import scipy.sparse as spsparse
 from interface_meta import override
 from formulaic.utils.cast import as_columns
 
 from .base import FormulaMaterializer
 from .types import NAAction
 
+if TYPE_CHECKING:  # pragma: no cover
+    from formulaic.model_spec import ModelSpec
+
 
 class PandasMaterializer(FormulaMaterializer):
 
     REGISTER_NAME = "pandas"
     REGISTER_INPUTS = ("pandas.core.frame.DataFrame",)
     REGISTER_OUTPUTS = ("pandas", "numpy", "sparse")
 
     @override
-    def _is_categorical(self, values):
+    def _is_categorical(self, values: Any) -> bool:
         if isinstance(values, (pandas.Series, pandas.Categorical)):
             return values.dtype == object or isinstance(
                 values.dtype, pandas.CategoricalDtype
             )
         return super()._is_categorical(values)
 
     @override
-    def _check_for_nulls(self, name, values, na_action, drop_rows):
+    def _check_for_nulls(
+        self, name: str, values: Any, na_action: NAAction, drop_rows: Set[int]
+    ) -> None:
 
         if na_action is NAAction.IGNORE:
             return
 
         if isinstance(
             values, dict
         ):  # pragma: no cover; no formulaic transforms return dictionaries any more
@@ -48,36 +55,56 @@
 
         else:
             raise ValueError(
                 f"Do not know how to interpret `na_action` = {repr(na_action)}."
             )  # pragma: no cover; this is currently impossible to reach
 
     @override
-    def _encode_constant(self, value, metadata, encoder_state, spec, drop_rows):
+    def _encode_constant(
+        self,
+        value: Any,
+        metadata: Any,
+        encoder_state: Dict[str, Any],
+        spec: ModelSpec,
+        drop_rows: Sequence[int],
+    ) -> Any:
         if spec.output == "sparse":
             return spsparse.csc_matrix(
                 numpy.array([value] * self.nrows).reshape(
                     (self.nrows - len(drop_rows), 1)
                 )
             )
         series = value * numpy.ones(self.nrows - len(drop_rows))
         return series
 
     @override
-    def _encode_numerical(self, values, metadata, encoder_state, spec, drop_rows):
+    def _encode_numerical(
+        self,
+        values: Any,
+        metadata: Any,
+        encoder_state: Dict[str, Any],
+        spec: ModelSpec,
+        drop_rows: Sequence[int],
+    ) -> Any:
         if drop_rows:
             values = values.drop(index=values.index[drop_rows])
         if spec.output == "sparse":
             return spsparse.csc_matrix(numpy.array(values).reshape((self.nrows, 1)))
         return values
 
     @override
     def _encode_categorical(
-        self, values, metadata, encoder_state, spec, drop_rows, reduced_rank=False
-    ):
+        self,
+        values: Any,
+        metadata: Any,
+        encoder_state: Dict[str, Any],
+        spec: ModelSpec,
+        drop_rows: Sequence[int],
+        reduced_rank: bool = False,
+    ) -> Any:
         # Even though we could reduce rank here, we do not, so that the same
         # encoding can be cached for both reduced and unreduced rank. The
         # rank will be reduced in the _encode_evaled_factor method.
         from formulaic.transforms import encode_contrasts
 
         if drop_rows:
             values = values.drop(index=values.index[drop_rows])
@@ -88,16 +115,18 @@
                 _metadata=metadata,
                 _state=encoder_state,
                 _spec=spec,
             )
         )
 
     @override
-    def _get_columns_for_term(self, factors, spec, scale=1):
-        out = OrderedDict()
+    def _get_columns_for_term(
+        self, factors: List[Dict[str, Any]], spec: ModelSpec, scale: float = 1
+    ) -> Dict[str, Any]:
+        out = {}
 
         names = [
             ":".join(reversed(product))
             for product in itertools.product(*reversed(factors))
         ]
 
         # Pre-multiply factors with only one set of values (improves performance)
@@ -140,21 +169,25 @@
                 out[names[i]] = scale * functools.reduce(
                     numpy.multiply,
                     (numpy.array(p[1]) for p in reversed(reversed_product)),
                 )
         return out
 
     @override
-    def _combine_columns(self, cols, spec, drop_rows):
+    def _combine_columns(
+        self, cols: Sequence[Tuple[str, Any]], spec: ModelSpec, drop_rows: Sequence[int]
+    ) -> pandas.DataFrame:
         # If we are outputing a pandas DataFrame, explicitly override index
         # in case transforms/etc have lost track of it.
         if spec.output == "pandas":
-            pandas_index = self.data_context.index
+            pandas_index = cast(pandas.DataFrame, self.data_context).index
             if drop_rows:
-                pandas_index = pandas_index.drop(self.data_context.index[drop_rows])
+                pandas_index = pandas_index.drop(
+                    cast(pandas.DataFrame, self.data_context).index[drop_rows]
+                )
 
         # Special case no columns to empty csc_matrix, array, or DataFrame
         if not cols:
             values = numpy.empty((self.data.shape[0], 0))
             if spec.output == "sparse":
                 return spsparse.csc_matrix(values)
             if spec.output == "numpy":
```

### Comparing `formulaic-0.6.3/formulaic/materializers/types/evaluated_factor.py` & `formulaic-0.6.4/formulaic/materializers/types/evaluated_factor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, replace
-from typing import Any, Optional
+from typing import Any, Optional, Set
 
 from formulaic.parser.types import Factor
+from formulaic.utils.variables import Variable
 
 from .factor_values import FactorValues, FactorValuesMetadata
 
 
 @dataclass
 class EvaluatedFactor:
     """
@@ -15,18 +16,22 @@
 
     This class acts as the glue between an abstract `Factor` specification and
     the realisation of that factor in a specific data context.
 
     Attributes:
         factor: The `Factor` instance for which values have been computed.
         values: The evaluated values for the factor.
+        variables: A mapping from the names of variables used during evaluation
+            to the name of the `LayeredMapping` instance from which it was
+            drawn.
     """
 
-    factor: Optional[Factor] = None
-    values: Optional[FactorValues[Any]] = None
+    factor: Factor
+    values: FactorValues[Any]
+    variables: Optional[Set[Variable]] = None
 
     @property
     def expr(self) -> str:
         """
         The expression of the evaluated factor.
         """
         return self.factor.expr
@@ -37,23 +42,23 @@
         The metadata associated with the evaluated values.
         """
         return self.values.__formulaic_metadata__
 
     def __repr__(self) -> str:
         return repr(self.factor)
 
-    def __eq__(self, other) -> bool:
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, EvaluatedFactor):
             return self.factor == other.factor
         return NotImplemented
 
-    def __lt__(self, other) -> bool:
+    def __lt__(self, other: Any) -> bool:
         if isinstance(other, EvaluatedFactor):
             return self.factor < other.factor
         return NotImplemented
 
-    def replace(self, **changes) -> EvaluatedFactor:
+    def replace(self, **changes: Any) -> EvaluatedFactor:
         """
         Return a copy of this `EvaluatedFactor` instance with the nominated
         attributes mutated.
         """
         return replace(self, **changes)
```

### Comparing `formulaic-0.6.3/formulaic/materializers/types/factor_values.py` & `formulaic-0.6.4/formulaic/materializers/types/factor_values.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 from __future__ import annotations
 import copy
 
 from dataclasses import dataclass, replace
-from typing import Any, Callable, Dict, Generic, List, Optional, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Hashable,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+    TYPE_CHECKING,
+)
 
 import wrapt
 
 from formulaic.parser.types import Factor
-from formulaic.utils.sentinels import MISSING
+from formulaic.utils.sentinels import MISSING, _MissingType
+
+if TYPE_CHECKING:  # pragma: no cover
+    from formulaic.model_spec import ModelSpec
 
 
 T = TypeVar("T")
 
 
 @dataclass
 class FactorValuesMetadata:
@@ -39,17 +54,19 @@
 
     kind: Factor.Kind = Factor.Kind.UNKNOWN
     column_names: Optional[Tuple[str]] = None
     spans_intercept: bool = False
     drop_field: Optional[str] = None
     format: str = "{name}[{field}]"
     encoded: bool = False
-    encoder: Optional[Callable[[Any, bool, List[int], Dict[str, Any]], Any]] = None
+    encoder: Optional[
+        Callable[[Any, bool, List[int], Dict[str, Any], ModelSpec], Any]
+    ] = None
 
-    def replace(self, **kwargs) -> FactorValuesMetadata:
+    def replace(self, **kwargs: Any) -> FactorValuesMetadata:
         """
         Return a copy of this `FactorValuesMetadata` instance with the nominated
         attributes replaced.
         """
         if not kwargs:
             return self
         return replace(self, **kwargs)
@@ -62,26 +79,28 @@
     object and behaves just like that object.
     """
 
     def __init__(
         self,
         values: Any,
         *,
-        metadata: FactorValuesMetadata = MISSING,
-        kind: Union[str, Factor.Kind] = MISSING,
-        column_names: Tuple[str] = MISSING,
-        spans_intercept: bool = MISSING,
-        drop_field: Optional[str] = MISSING,
-        format: str = MISSING,  # pylint: disable=redefined-builtin
-        encoded: bool = MISSING,
-        encoder: Optional[
-            Callable[[Any, bool, List[int], Dict[str, Any]], Any]
+        metadata: Union[FactorValuesMetadata, _MissingType] = MISSING,
+        kind: Union[str, Factor.Kind, _MissingType] = MISSING,
+        column_names: Union[Tuple[Hashable, ...], _MissingType] = MISSING,
+        spans_intercept: Union[bool, _MissingType] = MISSING,
+        drop_field: Union[None, Hashable, _MissingType] = MISSING,
+        format: Union[str, _MissingType] = MISSING,  # pylint: disable=redefined-builtin
+        encoded: Union[bool, _MissingType] = MISSING,
+        encoder: Union[
+            None,
+            Callable[[Any, bool, List[int], Dict[str, Any], ModelSpec], Any],
+            _MissingType,
         ] = MISSING,
     ):
-        metadata_constructor = FactorValuesMetadata
+        metadata_constructor: Callable = FactorValuesMetadata
         metadata_kwargs = dict(
             kind=Factor.Kind(kind) if kind is not MISSING else kind,
             column_names=column_names,
             spans_intercept=spans_intercept,
             drop_field=drop_field,
             format=format,
             encoded=encoded,
@@ -92,30 +111,30 @@
                 metadata_kwargs.pop(key)
 
         if hasattr(values, "__formulaic_metadata__"):
             metadata_constructor = values.__formulaic_metadata__.replace
             if isinstance(values, FactorValues):
                 values = values.__wrapped__
 
-        if metadata:
+        if metadata and not isinstance(metadata, _MissingType):
             metadata_constructor = metadata.replace
 
         wrapt.ObjectProxy.__init__(self, values)
         self._self_metadata = metadata_constructor(**metadata_kwargs)
 
     @property
     def __formulaic_metadata__(self) -> FactorValuesMetadata:
         return self._self_metadata
 
     def __repr__(self) -> str:
         return self.__wrapped__.__repr__()  # pragma: no cover
 
     # Handle copying behaviour
 
-    def __copy__(self):
+    def __copy__(self) -> FactorValues[T]:
         return type(self)(copy.copy(self.__wrapped__), metadata=self._self_metadata)
 
-    def __deepcopy__(self, memo=None):
+    def __deepcopy__(self, memo: Any = None) -> FactorValues[T]:
         return type(self)(
             copy.deepcopy(self.__wrapped__, memo),
             metadata=copy.deepcopy(self._self_metadata),
         )
```

### Comparing `formulaic-0.6.3/formulaic/parser/parser.py` & `formulaic-0.6.4/formulaic/parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 import itertools
 import functools
 import re
 from dataclasses import dataclass, field
-from typing import List, Iterable, Set, Tuple, Union
+from typing import List, Iterable, Sequence, Tuple, Union, cast
 
 from .algos.tokenize import tokenize
 from .types import (
     FormulaParser,
     Operator,
     OperatorResolver,
     OrderedSet,
@@ -123,43 +123,46 @@
     other implementations of Wilkinson formulas. It can be extended via
     subclassing to support other kinds of operators, in which case `.operators`
     and/or `.resolve` can be overridden. For more details about which operators
     are implemented, review the code or the documentation website.
     """
 
     @property
-    def operators(self):
+    def operators(self) -> List[Operator]:
         def formula_part_expansion(
-            lhs: Set[Term], rhs: Set[Term]
-        ) -> Tuple[Set[Term], Set[Term]]:
+            lhs: OrderedSet[Term], rhs: OrderedSet[Term]
+        ) -> Tuple[OrderedSet[Term], ...]:
             terms = (lhs, rhs)
 
             out = []
             for termset in terms:
                 if isinstance(termset, tuple):
                     out.extend(termset)
                 else:
                     out.append(termset)
             return tuple(out)
 
         def nested_product_expansion(
             parents: OrderedSet[Term], nested: OrderedSet[Term]
         ) -> OrderedSet[Term]:
             common = functools.reduce(lambda x, y: x * y, parents)
-            return parents | OrderedSet(common * term for term in nested)
+            return cast(
+                OrderedSet, parents | OrderedSet(common * term for term in nested)
+            )
 
         def power(arg: OrderedSet[Term], power: OrderedSet[Term]) -> OrderedSet[Term]:
             power_term = next(iter(power))
             if (
                 not len(power_term.factors) == 1
+                or not power_term.factors[0].token
                 or power_term.factors[0].token.kind is not Token.Kind.VALUE
                 or not isinstance(ast.literal_eval(power_term.factors[0].expr), int)
             ):
                 raise exc_for_token(
-                    power_term.factors[0].token,
+                    power_term.factors[0].token or Token(),
                     "The right-hand argument of `**` must be a positive integer.",
                 )
             return OrderedSet(
                 functools.reduce(lambda x, y: x * y, term)
                 for term in itertools.product(*[arg] * int(power_term.factors[0].expr))
             )
 
@@ -269,15 +272,15 @@
             Operator(
                 "^", arity=2, precedence=500, associativity="right", to_terms=power
             ),
         ]
 
     def resolve(
         self, token: Token, max_prefix_arity: int, context: List[Union[Token, Operator]]
-    ) -> Iterable[Operator]:
+    ) -> Sequence[Operator]:
         if token.token in self.operator_table:
             return super().resolve(token, max_prefix_arity, context)
 
         symbol = token.token
 
         # Keep track the number of "+" and "-" characters; if an odd number "-"
         # than "-", else "+"
```

### Comparing `formulaic-0.6.3/formulaic/parser/utils.py` & `formulaic-0.6.4/formulaic/parser/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,18 +60,18 @@
     purposes (note that this token will not be valid `Token` for use other than
     in reporting errors).
     """
     if isinstance(ast, Token):
         return ast
     lhs_token = ast
     while isinstance(lhs_token, ASTNode):
-        lhs_token = lhs_token.args[0]
+        lhs_token = lhs_token.args[0]  # type: ignore
     rhs_token = ast
     while isinstance(rhs_token, ASTNode):
-        rhs_token = rhs_token.args[-1]
+        rhs_token = rhs_token.args[-1]  # type: ignore
     return Token(
         token=lhs_token.source[lhs_token.source_start : rhs_token.source_end + 1]
         if lhs_token.source
         else "",
         source=lhs_token.source,
         source_start=lhs_token.source_start,
         source_end=rhs_token.source_end,
@@ -87,24 +87,26 @@
     `Token`s for use other than in reporting errors). Three tokens will be
     returned: the left-hand side token, the right-hand-side token, and the
     "middle" token where a new operator/token should be inserted (may not
     be empty depending on context).
     """
     lhs_token = lhs
     while isinstance(lhs_token, ASTNode):
-        lhs_token = lhs_token.args[-1]
+        lhs_token = lhs_token.args[-1]  # type: ignore
     rhs_token = rhs or lhs
     while isinstance(rhs_token, ASTNode):
-        rhs_token = rhs_token.args[0]
+        rhs_token = rhs_token.args[0]  # type: ignore
     return (
         lhs_token,
         rhs_token,
         Token(
             lhs_token.source[lhs_token.source_start : rhs_token.source_end + 1]
             if lhs_token.source
+            and lhs_token.source_start is not None
+            and rhs_token.source_end is not None
             else "",
             source=lhs_token.source,
             source_start=lhs_token.source_start,
             source_end=rhs_token.source_end,
         ),
     )
 
@@ -170,21 +172,19 @@
         kind: The type of tokens to be considered for insertion. If not
             specified, any matching token (part) will result in insertions.
         join_operator: If the insertion of tokens would result the joining of
             the added tokens with existing tokens, the value set here will be
             used to create a joining operator token. If not provided, not
             additional operators are added.
     """
+    tokens = list(tokens)
 
     if not isinstance(pattern, re.Pattern):
         pattern = re.compile(pattern)
 
-    if join_operator:
-        tokens = list(tokens)
-
     for i, token in enumerate(tokens):
         if (
             kind is not None
             and token.kind is not kind
             or not pattern.search(token.token)
         ):
             yield token
```

### Comparing `formulaic-0.6.3/formulaic/parser/algos/tokenize.py` & `formulaic-0.6.4/formulaic/parser/algos/tokenize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Iterable, Pattern
+from typing import Iterable, List, Pattern
 
 from ..types import Token
 from ..utils import exc_for_token
 
 
 def tokenize(
     formula: str,
@@ -49,15 +49,15 @@
         whitespace_chars: The regex pattern use to recognize (ignored)
             whitespace characters.
 
     Returns:
         A generator over the tokens found in the formula string.
 
     """
-    quote_context = []
+    quote_context: List[str] = []
     take = 0
 
     token = Token(source=formula)
 
     for i, char in enumerate(formula):
         if take > 0:
             token.update(char, i)
```

### Comparing `formulaic-0.6.3/formulaic/parser/algos/tokens_to_ast.py` & `formulaic-0.6.4/formulaic/parser/algos/tokens_to_ast.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import namedtuple
-from typing import Iterable, Optional
+from typing import Iterable, List, Union
 
 from ..types import ASTNode, Operator, OperatorResolver, Token
 from ..utils import exc_for_token, exc_for_missing_operator
 
 
 OrderedOperator = namedtuple("OrderedOperator", ("operator", "token", "index"))
 CONTEXT_OPENERS = {"(", "["}
@@ -11,15 +11,15 @@
     ")": "(",
     "]": "[",
 }
 
 
 def tokens_to_ast(
     tokens: Iterable[Token], operator_resolver: OperatorResolver
-) -> Optional[ASTNode]:
+) -> Union[None, Token, ASTNode]:
     """
     Convert a iterable of `Token` instances into an abstract syntax tree.
 
     This implementation is intentionally as simple and abstract as possible, and
     makes few assumptions about the form of the operators that will be present
     in the token sequence. Instead, it relies on the `OperatorResolver` instance
     to evaluate based on the context which operator should be invoked to handle
@@ -37,21 +37,23 @@
             generated.
         operator_resolver: The `OperatorResolver` instance to be used to lookup
             operators (only the `.resolve()` method is used).
 
     Returns:
         The generated abstract syntax tree as a nested `ASTNode` instance.
     """
-    output_queue = []
-    operator_stack = []
+    output_queue: List[Union[Token, ASTNode]] = []
+    operator_stack: List[OrderedOperator] = []
 
-    def stack_operator(operator, token):
+    def stack_operator(operator: Union[Token, Operator], token: Token) -> None:
         operator_stack.append(OrderedOperator(operator, token, len(output_queue)))
 
-    def operate(ordered_operator, output_queue):
+    def operate(
+        ordered_operator: OrderedOperator, output_queue: List[Union[Token, ASTNode]]
+    ) -> List[Union[Token, ASTNode]]:
         operator, token, index = ordered_operator
 
         if operator.fixity is Operator.Fixity.INFIX:
             assert operator.arity == 2
             min_index = index - 1
             max_index = index + 1
         elif operator.fixity is Operator.Fixity.PREFIX:
@@ -128,7 +130,9 @@
             )
         output_queue = operate(operator_stack.pop(), output_queue)
 
     if output_queue:
         if len(output_queue) > 1:
             raise exc_for_missing_operator(output_queue[0], output_queue[1])
         return output_queue[0]
+
+    return None
```

### Comparing `formulaic-0.6.3/formulaic/parser/types/ast_node.py` & `formulaic-0.6.4/formulaic/parser/types/ast_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import graphlib
-from typing import Any, Dict, Iterable, List
+from typing import Any, Dict, Generic, Iterable, List, Tuple, TypeVar, Union
 
 from .operator import Operator
 from .structured import Structured
 from .term import Term
 
 
-class ASTNode:
+ItemType = TypeVar("ItemType")
+
+
+class ASTNode(Generic[ItemType]):
     """
     Represents a node in an Abstract Syntax Tree (AST).
 
     An `ASTNode` instance is composed of an `Operator` instance and a set of
     arguments to be passed into that operator. The arguments may include nested
     `ASTNode`s or other arguments. Once evaluated, a set of `Term` instances
     is returned.
@@ -22,26 +25,26 @@
         args: The arguments associated with this node.
     """
 
     def __init__(self, operator: Operator, args: Iterable[Any]):
         self.operator = operator
         self.args = args
 
-    def to_terms(self) -> Iterable[Term]:
+    def to_terms(self) -> Union[List[Term], Structured[List[Term]], Tuple]:
         """
         Evaluate this AST node and return the resulting set of `Term` instances.
 
         Note: We use topological evaluation here to avoid recursion issues for
         long formula (exceeding ~700 terms, though this depends on the recursion
         limit set in the interpreter).
         """
         g = graphlib.TopologicalSorter(self.__generate_evaluation_graph())
         g.prepare()
 
-        results = {}
+        results: Dict[ASTNode, Any] = {}
 
         while g.is_active():
             for node in g.get_ready():
                 node_args = (
                     (results[arg] if isinstance(arg, ASTNode) else arg.to_terms())
                     for arg in node.args
                 )
@@ -52,15 +55,15 @@
                         *node_args,
                         merger=node.operator.to_terms,
                     )
                 g.done(node)
 
         return results[self]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         try:
             return f"<ASTNode {self.operator}: {self.args}>"
         except RecursionError:
             return f"<ASTNode {self.operator}: ...>"
 
     def flatten(self, str_args: bool = False) -> List[Any]:
         """
```

### Comparing `formulaic-0.6.3/formulaic/parser/types/factor.py` & `formulaic-0.6.4/formulaic/parser/types/factor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import Dict, Optional, Union, TYPE_CHECKING
+from typing import Any, Dict, Optional, Union, TYPE_CHECKING
 
 from .ordered_set import OrderedSet
 from .term import Term
 
 if TYPE_CHECKING:
     from .token import Token  # pragma: no cover
 
@@ -51,52 +51,52 @@
         *,
         eval_method: Optional[Union[str, EvalMethod]] = None,
         kind: Optional[Union[str, Kind]] = None,
         metadata: Optional[Dict] = None,
         token: Optional[Token] = None,
     ):
         self.expr = expr
-        self.eval_method = eval_method
-        self.kind = kind
+        self.eval_method = eval_method  # type: ignore
+        self.kind = kind  # type: ignore
         self.metadata = metadata or {}
         self.token = token
 
     @property
     def eval_method(self) -> EvalMethod:
         return self._eval_method
 
     @eval_method.setter
-    def eval_method(self, eval_method):
+    def eval_method(self, eval_method: Union[str, EvalMethod]) -> None:
         self._eval_method = Factor.EvalMethod(eval_method or "lookup")
 
     @property
     def kind(self) -> Kind:
         return self._kind
 
     @kind.setter
-    def kind(self, kind):
+    def kind(self, kind: Union[str, Factor.Kind]) -> None:
         self._kind = Factor.Kind(kind or "unknown")
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, str):
             return self.expr == other
         if isinstance(other, Factor):
             return self.expr == other.expr
         return NotImplemented
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return self.expr.__hash__()
 
-    def __lt__(self, other):
+    def __lt__(self, other: Any) -> bool:
         if isinstance(other, Factor):
             return self.expr < other.expr
         return NotImplemented
 
     def to_terms(self) -> OrderedSet[Term]:
         """
         Convert this `Factor` instance into a `Term` instance, and expose it as
         a single-element ordered set.
         """
         return OrderedSet((Term([self]),))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.expr
```

### Comparing `formulaic-0.6.3/formulaic/parser/types/formula_parser.py` & `formulaic-0.6.4/formulaic/parser/types/formula_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Iterable, List
+from typing import Iterable, List, Union
 
 from .ast_node import ASTNode
 from .operator_resolver import OperatorResolver
 from .structured import Structured
 from .term import Term
 from .token import Token
 
@@ -41,15 +41,15 @@
         Args:
             formula: The formula string to be tokenized.
         """
         from ..algos.tokenize import tokenize
 
         return tokenize(formula)
 
-    def get_ast(self, formula: str) -> ASTNode:
+    def get_ast(self, formula: str) -> Union[None, Token, ASTNode]:
         """
         Assemble an abstract syntax tree for the nominated `formula` string.
 
         Args:
             formula: The formula for which an AST should be generated.
         """
         from ..algos.tokens_to_ast import tokens_to_ast
@@ -70,10 +70,10 @@
         """
         ast = self.get_ast(formula)
         if ast is None:
             return Structured([])
 
         terms = ast.to_terms()
         if not isinstance(terms, Structured):
-            terms = Structured(terms)
+            terms = Structured[List[Term]](terms)
 
         return terms
```

### Comparing `formulaic-0.6.3/formulaic/parser/types/operator.py` & `formulaic-0.6.4/formulaic/parser/types/operator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from __future__ import annotations
 
 from enum import Enum
-from numbers import Number
-from typing import Callable, List, Iterable, Union
+from typing import Any, Callable, List, Optional, Union
 
-from .ordered_set import OrderedSet
-from .term import Term
 from .token import Token
 
 
 class Operator:
     """
     Specification for how an operator in a formula string should behave.
 
@@ -51,60 +48,62 @@
         POSTFIX = "postfix"
 
     def __init__(
         self,
         symbol: str,
         *,
         arity: int,
-        precedence: Number,
-        associativity: Union[str, Associativity] = "none",
-        fixity: Union[str, Fixity] = "infix",
-        to_terms: Callable[..., Iterable[Term]] = None,
-        accepts_context: Callable[[List[Union[Token, Operator]]], bool] = None,
+        precedence: float,
+        associativity: Union[None, str, Associativity] = Associativity.NONE,
+        fixity: Union[str, Fixity] = Fixity.INFIX,
+        to_terms: Optional[Callable[..., Any]] = None,
+        accepts_context: Optional[
+            Callable[[List[Union[Token, Operator]]], bool]
+        ] = None,
         structural: bool = False,
     ):
         self.symbol = symbol
         self.arity = arity
         self.precedence = precedence
-        self.associativity = associativity
-        self.fixity = fixity
+        self.associativity = associativity  # type: ignore
+        self.fixity = fixity  # type: ignore
         self._to_terms = to_terms
         self._accepts_context = accepts_context
         self.structural = structural
 
     @property
-    def associativity(self):
+    def associativity(self) -> Operator.Associativity:
         return self._associativity
 
     @associativity.setter
-    def associativity(self, associativity):
+    def associativity(self, associativity: Union[str, Operator.Associativity]) -> None:
         self._associativity = Operator.Associativity(associativity or "none")
 
     @property
-    def fixity(self):
+    def fixity(self) -> Operator.Fixity:
         return self._fixity
 
     @fixity.setter
-    def fixity(self, fixity):
+    def fixity(self, fixity: Union[str, Operator.Fixity]) -> None:
         self._fixity = Operator.Fixity(fixity)
 
-    def to_terms(self, *args) -> OrderedSet[Term]:
+    def to_terms(self, *args: Any) -> Any:
         if self._to_terms is None:
             raise RuntimeError(f"`to_terms` is not implemented for '{self.symbol}'.")
         return self._to_terms(*args)
 
-    def accepts_context(self, context: List[Union[Token, Operator]]):
+    def accepts_context(self, context: List[Union[Token, Operator]]) -> bool:
         if self._accepts_context:
             # We only need to pass on tokens and operators with precedence less
             # than or equal to ourselves, since all other operators will be
             # evaluated before us.
             return self._accepts_context(
                 [
                     c
                     for c in context
                     if isinstance(c, Token) or c.precedence <= self.precedence
                 ]
             )
         return True
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.symbol
```

### Comparing `formulaic-0.6.3/formulaic/parser/types/operator_resolver.py` & `formulaic-0.6.4/formulaic/parser/types/operator_resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import abc
 from collections import defaultdict
-from typing import List, Union
+from typing import Dict, List, Sequence, Union
 
 from ..utils import exc_for_token
 from .operator import Operator
 from .token import Token
 
 # Cached property was introduced in Python 3.8 (we currently support 3.7)
 try:
     from functools import cached_property
 except ImportError:  # pragma: no cover
-    from cached_property import cached_property
+    from cached_property import cached_property  # type: ignore
 
 
 class OperatorResolver(metaclass=abc.ABCMeta):
     """
     Resolves which `Operator` instance should be used for a given operator
     `Token`.
 
@@ -36,27 +36,27 @@
     def operators(self) -> List[Operator]:
         """
         The `Operator` instance pool which can be matched to tokens by
         `.resolve()`.
         """
 
     @cached_property
-    def operator_table(self):
+    def operator_table(self) -> Dict[str, List[Operator]]:
         operator_table = defaultdict(list)
         for operator in self.operators:
             operator_table[operator.symbol].append(operator)
         for symbol in operator_table:
             operator_table[symbol] = sorted(
                 operator_table[symbol], key=lambda op: op.precedence, reverse=True
             )
         return operator_table
 
     def resolve(
         self, token: Token, max_prefix_arity: int, context: List[Union[Token, Operator]]
-    ) -> List[Operator]:
+    ) -> Sequence[Operator]:
         """
         Return a list of operators to apply for a given token in the AST
         generation.
 
         Args:
             token: The operator `Token` instance for which `Operator`(s) should
                 be resolved.
@@ -97,9 +97,9 @@
             raise exc_for_token(
                 token,
                 f"Ambiguous operator `{symbol}`. This is not usually a user error. Please report this!",
             )
         return candidates[0]
 
     # The operator table cache may not be pickleable, so let's drop it.
-    def __getstate__(self):
+    def __getstate__(self) -> Dict:
         return {}
```

### Comparing `formulaic-0.6.3/formulaic/parser/types/structured.py` & `formulaic-0.6.4/formulaic/parser/types/structured.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     Generic,
     Iterable,
+    List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
@@ -84,31 +85,31 @@
 
     __slots__ = ("_structure", "_metadata")
 
     def __init__(
         self,
         root: Any = _MISSING,
         *,
-        _metadata: Dict[str, Any] = None,
-        **structure,
+        _metadata: Optional[Dict[str, Any]] = None,
+        **structure: Any,
     ):
         if any(key.startswith("_") for key in structure):
             raise ValueError(
                 "Substructure keys cannot start with an underscore. "
                 f"The invalid keys are: {set(key for key in structure if key.startswith('_'))}."
             )
         if root is not _MISSING:
             structure["root"] = self.__prepare_item("root", root)
         self._metadata = _metadata
 
         self._structure = {
             key: self.__prepare_item(key, item) for key, item in structure.items()
         }
 
-    def __prepare_item(self, key: str, item: Any) -> ItemType:
+    def __prepare_item(self, key: str, item: Any) -> Any:
         if isinstance(item, Structured):
             return item._map(
                 lambda x: self._prepare_item(key, x), as_type=self.__class__
             )
         if isinstance(item, tuple):
             return tuple(self.__prepare_item(key, v) for v in item)
         return self._prepare_item(key, item)
@@ -163,26 +164,26 @@
                 values. If not provided, the base `Structured` type is used.
 
         Returns:
             A `Structured` instance with the same structure as this instance,
             but with all objects transformed under `func`.
         """
 
-        def apply_func(obj):
+        def apply_func(obj: Any) -> Any:
             if recurse and isinstance(obj, Structured):
                 return obj._map(func, recurse=True, as_type=as_type)
             if isinstance(obj, tuple):
                 return tuple(apply_func(o) for o in obj)
             return func(obj)
 
         return (as_type or Structured)(
             **{key: apply_func(obj) for key, obj in self._structure.items()}
         )
 
-    def _flatten(self) -> Generator[ItemType]:
+    def _flatten(self) -> Generator[ItemType, None, None]:
         """
         Flatten any nested structure into a sequence of all values stored in
         this `Structured` instance. The order is currently that yielded by a
         depth-first iteration, however this is not guaranteed and should not
         be relied upon.
         """
         for value in self._structure.values():
@@ -207,15 +208,15 @@
                 `Structured` instances will be surfaced in the generated
                 dictionary.
 
         Returns:
             The dictionary representation of this `Structured` instance.
         """
 
-        def do_recursion(obj):
+        def do_recursion(obj: Any) -> Any:
             if recurse and isinstance(obj, Structured):
                 return obj._to_dict()
             if isinstance(obj, tuple):
                 return tuple(do_recursion(o) for o in obj)
             return obj
 
         return {key: do_recursion(value) for key, value in self._structure.items()}
@@ -258,15 +259,15 @@
         if not isinstance(structured, Structured):
             return structured
 
         structure = structured._structure
 
         if recurse:
 
-            def simplify_obj(obj):
+            def simplify_obj(obj: Any) -> Any:
                 if isinstance(obj, Structured):
                     return obj._simplify(recurse=True)
                 if isinstance(obj, tuple):
                     return tuple(simplify_obj(o) for o in obj)
                 return obj
 
             structure = {
@@ -277,15 +278,15 @@
             self._structure = structure
             return self
         return self.__class__(
             _metadata=self._metadata,
             **structure,
         )
 
-    def _update(self, root=_MISSING, **structure) -> Structured[ItemType]:
+    def _update(self, root: Any = _MISSING, **structure: Any) -> Structured[ItemType]:
         """
         Return a new `Structured` instance that is identical to this one but
         the root and/or keys replaced with the nominated values.
 
         Args:
             root: The (optional) replacement of the root node.
             structure: Any additional key/values to update in the structure.
@@ -303,17 +304,17 @@
             }
         )
 
     @classmethod
     def _merge(
         cls,
         *objects: Any,
-        merger: Callable[..., ItemType] = None,
+        merger: Optional[Callable] = None,
         _context: Tuple[str, ...] = (),
-    ) -> Union[ItemType, Structured[ItemType]]:
+    ) -> Union[ItemType, Structured[ItemType], Tuple]:
         """
         Merge arbitrarily many objects into a single `Structured` instance.
 
         If any of `objects` are `Structured` or `tuple` instances, then all
         `objects` will be treated as `Structured` instances (being upcast as
         necessary) and then merged recursively; otherwise the objects will be
         merged directly by `merger`.
@@ -354,15 +355,15 @@
                 return merged
             return cls(merged)
 
         # Check whether all objects are not Structured instances (or tuples,
         # already excluded by above). If so, just call `merger` on them
         # directly.
         if all(not isinstance(obj, Structured) for obj in objects):
-            return merger(*objects)
+            return merger(*objects)  # type: ignore
 
         # Otherwise,iterate over objects, upcasting to `Structured` as necessary
         # and recursively merge them by merging their structure dictionaries.
         values_to_merge = defaultdict(list)
 
         for obj in objects:
             if isinstance(obj, Structured):
@@ -379,91 +380,93 @@
                     else values[0]
                 )
                 for key, values in values_to_merge.items()
             }
         )
 
     @staticmethod
-    def __merger_default(*items):
+    def __merger_default(*items: Any) -> Union[list, set, dict]:
         if all(isinstance(item, list) for item in items):
             return list(itertools.chain(*items))
         if all(isinstance(item, set) for item in items):
             return set.union(*items)
         if all(isinstance(item, dict) for item in items):
             return dict(itertools.chain(*(d.items() for d in items)))
         raise NotImplementedError(
             "The fallback `merger` for `Structured._merge` does not know how to "
             f"merge objects of types {repr(tuple(type(item) for item in items))}. "
             "Please specify `merger` explicitly."
         )
 
-    def __dir__(self):
-        return super().__dir__() + list(self._structure)
+    def __dir__(self) -> List[str]:
+        return [*super().__dir__(), *self._structure]
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> Any:
         if attr.startswith("_"):
             raise AttributeError(attr)
         if attr in self._structure:
             return self._structure[attr]
         raise AttributeError(
             f"This `{self.__class__.__name__}` instance does not have structure @ `{repr(attr)}`."
         )
 
-    def __setattr__(self, attr, value):
+    def __setattr__(self, attr: str, value: Any) -> None:
         if attr.startswith("_"):
             super().__setattr__(attr, value)
             return
         self._structure[attr] = self.__prepare_item(attr, value)
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: Any) -> Any:
         if self._has_root and not self._has_keys:
             return self.root[key]
         if key in (None, "root") and self._has_root:
             return self.root
         if isinstance(key, str) and not key.startswith("_") and key in self._structure:
             return self._structure[key]
         raise KeyError(
             f"This `{self.__class__.__name__}` instance does not have structure @ `{repr(key)}`."
         )
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: Any, value: Any) -> Any:
         if not isinstance(key, str) or not key.isidentifier():
             raise KeyError(key)
         if key.startswith("_"):
             raise KeyError(
                 "Substructure keys cannot start with an underscore. "
                 f"The invalid keys are: {set(key for key in self._structure if key.startswith('_'))}."
             )
         self._structure[key] = self.__prepare_item(key, value)
 
-    def __iter__(self) -> Generator[Union[ItemType, Structured[ItemType]]]:
-        if self._has_root and not self._has_keys and isinstance(self.root, Iterable):
+    def __iter__(self) -> Generator[Any, None, None]:
+        if (
+            self._has_root and not self._has_keys and isinstance(self.root, Iterable)
+        ):  # pylint: disable=isinstance-second-argument-not-valid-type
             yield from self.root
         else:
             if self._has_root:  # Always yield root first.
                 yield self.root
             for key, value in self._structure.items():
                 if key != "root":
                     yield value
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, Structured):
             return self._structure == other._structure
         return False
 
-    def __contains__(self, key):
+    def __contains__(self, key: Any) -> bool:
         return key in self._structure
 
     def __len__(self) -> int:
         return sum(1 for _ in self)
 
-    def __str__(self):
-        return self.__repr__(to_str=str)
+    def __str__(self) -> str:
+        return self.__repr__(to_str=str)  # type: ignore
 
-    def __repr__(self, to_str=repr):
+    def __repr__(self, to_str: Callable[..., str] = repr) -> str:
         import textwrap
 
         d = self._to_dict(recurse=False)
         keys = [key for key in d if key != "root"]
         if self._has_root:
             keys.insert(0, "root")
```

### Comparing `formulaic-0.6.3/formulaic/parser/types/term.py` & `formulaic-0.6.4/formulaic/parser/types/term.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Iterable, TYPE_CHECKING
+from __future__ import annotations
+
+from typing import Any, Iterable, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .factor import Factor  # pragma: no cover
 
 
 class Term:
     """
@@ -18,33 +20,33 @@
     def __init__(self, factors: Iterable["Factor"]):
         self.factors = tuple(dict.fromkeys(factors))
         self._factor_key = tuple(factor.expr for factor in sorted(self.factors))
         self._hash = hash(":".join(self._factor_key))
 
     # Transforms and comparisons
 
-    def __mul__(self, other):
+    def __mul__(self, other: Any) -> Term:
         if isinstance(other, Term):
             return Term([*self.factors, *other.factors])
         return NotImplemented
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return self._hash
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, Term):
             return self._factor_key == other._factor_key
         if isinstance(other, str):
             return self._factor_key == tuple(sorted(other.split(":")))
         return NotImplemented
 
-    def __lt__(self, other):
+    def __lt__(self, other: Any) -> bool:
         if isinstance(other, Term):
             if len(self.factors) == len(other.factors):
                 return sorted(self.factors) < sorted(other.factors)
             if len(self.factors) < len(other.factors):
                 return True
             return False
         return NotImplemented
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return ":".join(factor.expr for factor in self.factors)
```

### Comparing `formulaic-0.6.3/formulaic/parser/types/token.py` & `formulaic-0.6.4/formulaic/parser/types/token.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,29 +55,29 @@
         *,
         kind: Optional[Union[str, Kind]] = None,
         source: Optional[str] = None,
         source_start: Optional[int] = None,
         source_end: Optional[int] = None,
     ):
         self.token = token
-        self.kind = kind
+        self.kind = kind  # type: ignore
         self.source = source
         self.source_start = source_start
         self.source_end = source_end or source_start
 
     @property
     def kind(self) -> Optional[Kind]:
-        return self._kind
+        return self._kind  # type: ignore
 
     @kind.setter
-    def kind(self, kind: Optional[Union[str, Kind]]):
+    def kind(self, kind: Optional[Union[str, Kind]]) -> None:
         self._kind = self.Kind(kind) if kind else kind
 
     def update(
-        self, char: str, source_index: int, kind: Optional[Kind] = None
+        self, char: str, source_index: int, kind: Union[None, str, Kind] = None
     ) -> "Token":
         """
         Add a character to the token string, keeping track of the source
         indices.
 
         Args:
             char: The character to add.
@@ -89,48 +89,50 @@
             A reference to this token instance.
         """
         self.token += char
         if self.source_start is None:
             self.source_start = source_index
         self.source_end = source_index
         if kind is not None:
-            self.kind = kind
+            self.kind = Token.Kind(kind)
         return self
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return bool(self.token)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, str):
             return self.token == other
         if isinstance(other, Token):
             return self.token == other.token and self.kind == other.kind
         return NotImplemented
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return self.token.__hash__()
 
-    def __lt__(self, other):
+    def __lt__(self, other: Any) -> bool:
         if isinstance(other, Token):
             return self.token < other.token
         return NotImplemented
 
     @property
-    def source_loc(self) -> Tuple[int, int]:
+    def source_loc(self) -> Tuple[Optional[int], Optional[int]]:
         """
         The indices of the first and last character represented by this token in
         the source string.
         """
         return (self.source_start, self.source_end)
 
     def to_factor(self) -> Factor:
         """
         A `Factor` instance corresponding to this token. Note that operator
         tokens cannot be converted to tokens.
         """
+        if self.kind is None:  # pragma: no cover
+            raise RuntimeError("`Token.kind` has not been set.")
         kind_to_eval_method = {
             Token.Kind.NAME: "lookup",
             Token.Kind.PYTHON: "python",
             Token.Kind.VALUE: "literal",
         }
         return Factor(
             expr=self.token,
@@ -143,26 +145,26 @@
         An order set of `Term` instances for this token. This will just be
         an iterable with one `Term` having one `Factor` (that generated by
         `.to_factor()`). Operator tokens cannot be converted to an iterable of
         `Term`s.
         """
         return OrderedSet((Term([self.to_factor()]),))
 
-    def flatten(self, str_args=False) -> Any:
+    def flatten(self, str_args: bool = False) -> Any:
         """
         Return this token (or if `str_args` is `True`, a string representation
         of this token).
 
         Args:
             str_args: Whether to convert this token to a string during
             flattening.
         """
         return str(self) if str_args else self
 
-    def get_source_context(self, colorize: bool = False) -> str:
+    def get_source_context(self, colorize: bool = False) -> Optional[str]:
         """
         Render a string that highlights the location of this token in the source
         string.
 
         Args:
             colorize: Whether to highlight the location of this token in bold
                 red font.
@@ -171,34 +173,34 @@
             return None
         if colorize:
             RED_BOLD = "\x1b[1;31m"
             RESET = "\x1b[0m"
             return f"{self.source[:self.source_start]}⧛{RED_BOLD}{self.source[self.source_start:self.source_end+1]}{RESET}⧚{self.source[self.source_end+1:]}"
         return f"{self.source[:self.source_start]}⧛{self.source[self.source_start:self.source_end+1]}⧚{self.source[self.source_end+1:]}"
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.token
 
     # Additional methods for later mutation
 
-    def copy_with_attrs(self, **attrs) -> Token:
+    def copy_with_attrs(self, **attrs: Any) -> Token:
         """
         Return a copy of this `Token` instance with attributes set from attrs.
 
         Args:
             attrs: Attribute keys and values to set on the copy of this
                 instance.
         """
         new_token = copy.copy(self)
         for attr, value in attrs.items():
             setattr(new_token, attr, value)
         return new_token
 
     def split(
-        self, pattern: Union[str, re.Pattern], after=False, before=False
+        self, pattern: Union[str, re.Pattern], after: bool = False, before: bool = False
     ) -> Iterable[Token]:
         """
         Split this instance into multple tokens around all non-overlapping
         matches of `pattern`.
 
         Args:
             pattern: The pattern by which to split this `Token` instance.
@@ -211,15 +213,15 @@
 
         if not isinstance(pattern, re.Pattern):
             pattern = re.compile(pattern)
 
         last_index = 0
         separators = pattern.finditer(self.token)
 
-        def get_next_token(next_index):
+        def get_next_token(next_index: int) -> Tuple[int, Token]:
             return next_index, self.copy_with_attrs(
                 token=self.token[last_index:next_index]
             )
 
         for separator in separators:
             if before:
                 last_index, new_token = get_next_token(separator.span()[0])
```

### Comparing `formulaic-0.6.3/formulaic/transforms/__init__.py` & `formulaic-0.6.4/formulaic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/formulaic/transforms/basis_spline.py` & `formulaic-0.6.4/formulaic/transforms/basis_spline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import defaultdict
 from enum import Enum
-from typing import Iterable, Optional, Union
+from typing import Dict, Iterable, Optional, Union, cast
 
 import numpy
 import pandas
 
 from formulaic.materializers.types import FactorValues
 from formulaic.utils.stateful_transforms import stateful_transform
 
@@ -19,24 +19,24 @@
     CLIP = "clip"
     NA = "na"
     ZERO = "zero"
     EXTEND = "extend"
 
 
 @stateful_transform
-def basis_spline(
+def basis_spline(  # pylint: disable=dangerous-default-value  # always replaced by stateful-transform
     x: Union[pandas.Series, numpy.ndarray],
     df: Optional[int] = None,
     knots: Optional[Iterable[float]] = None,
     degree: int = 3,
     include_intercept: bool = False,
     lower_bound: Optional[float] = None,
     upper_bound: Optional[float] = None,
     extrapolation: Union[str, SplineExtrapolation] = "raise",
-    _state: dict = None,
+    _state: dict = {},
 ) -> FactorValues[dict]:
     """
     Evaluates the B-Spline basis vectors for given inputs `x`.
 
     This is especially useful in the context of allowing non-linear fits to data
     in linear regression. Except for the addition of the `extrapolation`
     parameter, this implementation shares its API with `patsy.splines.bs`, and
@@ -135,25 +135,25 @@
             if nknots < 0:
                 raise ValueError(
                     f"Invalid value for `df`. `df` must be greater than {degree + (1 if include_intercept else 0)} [`degree` (+ 1 if `include_intercept` is `True`)]."
                 )
             knots = list(
                 numpy.quantile(x, numpy.linspace(0, 1, nknots + 2))[1:-1].ravel()
             )
-        knots.insert(0, lower_bound)
-        knots.append(upper_bound)
+        knots.insert(0, cast(float, lower_bound))
+        knots.append(cast(float, upper_bound))
         knots = list(numpy.pad(knots, degree, mode="edge"))
         _state["knots"] = knots
     knots = _state["knots"]
 
     # Compute basis splines
     # The following code is equivalent to [B(i, j=degree) for in range(len(knots)-d-1)], with B(i, j) as defined below.
     # B = lambda i, j: ((x >= knots[i]) & (x < knots[i+1])).astype(float) if j == 0 else alpha(i, j, x) * B(i, j-1, x) + (1 - alpha(i+1, j, x)) * B(i+1, j-1, x)
     # We don't directly use this recurrence relation so that we can memoise the B(i, j).
-    cache = defaultdict(dict)
+    cache: Dict[int, Dict[int, float]] = defaultdict(dict)
     alpha = (
         lambda i, j: (x - knots[i]) / (knots[i + j] - knots[i])
         if knots[i + j] != knots[i]
         else 0
     )
     for i in range(len(knots) - 1):
         if extrapolation is SplineExtrapolation.EXTEND:
```

### Comparing `formulaic-0.6.3/formulaic/transforms/contrasts.py` & `formulaic-0.6.4/formulaic/transforms/contrasts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 from __future__ import annotations
 from abc import abstractmethod
 
 import inspect
 import warnings
 from numbers import Number
-from typing import Any, Union, Dict, Iterable, List, Optional, TYPE_CHECKING
+from typing import (
+    Any,
+    Hashable,
+    Sequence,
+    Tuple,
+    Union,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    TYPE_CHECKING,
+    cast,
+)
 
 import numpy
 import pandas
 import scipy.sparse as spsparse
 import scipy.sparse.linalg
 from interface_meta import InterfaceMeta
 
@@ -27,15 +39,15 @@
     data: Any,
     contrasts: Optional[
         Union[Contrasts, Dict[str, Iterable[Number]], numpy.ndarray]
     ] = None,
     *,
     levels: Optional[Iterable[str]] = None,
     spans_intercept: bool = True,
-):
+) -> FactorValues:
     """
     Mark data as being categorical, and optionally specify the contrasts to be
     used during encoding.
 
     Args:
         data: The data to be marked as categorical.
         contrasts:  The specification of the contrasts that are to be computed.
@@ -55,15 +67,15 @@
 
     def encoder(
         values: Any,
         reduced_rank: bool,
         drop_rows: List[int],
         encoder_state: Dict[str, Any],
         model_spec: ModelSpec,
-    ):
+    ) -> FactorValues:
         values = pandas.Series(values)
         values = values.drop(index=values.index[drop_rows])
         return encode_contrasts(
             values,
             contrasts=contrasts,
             levels=levels,
             reduced_rank=reduced_rank,
@@ -76,25 +88,29 @@
         kind="categorical",
         spans_intercept=spans_intercept,
         encoder=encoder,
     )
 
 
 @stateful_transform
-def encode_contrasts(
-    data,
+def encode_contrasts(  # pylint: disable=dangerous-default-value  # always replaced by stateful-transform
+    data: Any,
     contrasts: Union[
-        Contrasts, Dict[str, Iterable[Number]], numpy.ndarray, None
+        Contrasts,
+        Dict[Hashable, Sequence[float]],
+        Sequence[Sequence[float]],
+        numpy.ndarray,
+        None,
     ] = None,
     *,
     levels: Optional[Iterable[str]] = None,
     reduced_rank: bool = False,
     output: Optional[str] = None,
-    _state=None,
-    _spec=None,
+    _state: Dict[str, Any] = {},
+    _spec: Optional[ModelSpec] = None,
 ) -> FactorValues[Union[pandas.DataFrame, spsparse.spmatrix]]:
     """
     Encode a categorical dataset into one or more "contrasts".
 
     Args:
         data: The categorical data array/series to be encoded.
         contrasts: The specification of the contrasts that are to be computed.
@@ -107,25 +123,35 @@
             the data. This can also be used to reorder the levels as needed.
         reduced_rank: Whether to reduce the rank of output encoded columns in
             order to avoid spanning the intercept.
         output: The type of data to output. Must be one of "pandas", "numpy", or
             "sparse".
     """
     # Prepare arguments
+    _spec = cast("ModelSpec", _spec)
     output = output or _spec.output or "pandas"
     levels = (
         levels if levels is not None else _state.get("categories")
     )  # TODO: Is this too early to provide useful feedback to users?
 
     if contrasts is None:
         contrasts = TreatmentContrasts()
     elif inspect.isclass(contrasts) and issubclass(contrasts, Contrasts):
-        contrasts = contrasts()
+        contrasts = contrasts()  # type: ignore[misc]
     if not isinstance(contrasts, Contrasts):
-        contrasts = CustomContrasts(contrasts)
+        contrasts = CustomContrasts(
+            cast(
+                Union[
+                    Dict[Hashable, Sequence[float]],
+                    Sequence[Sequence[float]],
+                    numpy.ndarray,
+                ],
+                contrasts,
+            )
+        )
 
     if levels is not None:
         extra_categories = set(pandas.unique(data)).difference(levels)
         if extra_categories:
             warnings.warn(
                 "Data has categories outside of the nominated levels (or that were "
                 f"not seen in original dataset): {extra_categories}. They are being "
@@ -163,19 +189,19 @@
 
     INTERFACE_RAISE_ON_VIOLATION = True
 
     FACTOR_FORMAT = "{name}[{field}]"
 
     def apply(
         self,
-        dummies,
-        levels,
-        reduced_rank=True,
+        dummies: Union[pandas.DataFrame, numpy.ndarray, spsparse.spmatrix],
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
         output: Optional[str] = None,
-    ):
+    ) -> FactorValues[Union[pandas.DataFrame, numpy.ndarray, spsparse.spmatrix]]:
         """
         Apply the contrasts defined by this `Contrasts` instance to `dummies`
         (the dummy encoding of the values of interest).
 
         Args:
             dummies: Dummy encoded representation of the values.
             levels: The names of the levels/categories in the data.
@@ -218,15 +244,15 @@
             else:  # pragma: no cover
                 raise ValueError(
                     "Short-circuiting is only implemented for output types: 'pandas', 'numpy' or 'sparse'."
                 )
             return FactorValues(
                 encoded,
                 kind="categorical",
-                column_names=[],
+                column_names=cast(Tuple[Hashable], ()),
                 spans_intercept=False,
                 format=self.get_factor_format(levels, reduced_rank=reduced_rank),
                 encoded=True,
             )
 
         sparse = output == "sparse"
         encoded = self._apply(
@@ -243,28 +269,39 @@
             )
         elif output == "numpy":
             encoded = numpy.array(encoded)
 
         return FactorValues(
             encoded,
             kind="categorical",
-            column_names=coding_column_names,
+            column_names=tuple(coding_column_names),
             spans_intercept=self.get_spans_intercept(levels, reduced_rank=reduced_rank),
             drop_field=self.get_drop_field(levels, reduced_rank=reduced_rank),
             format=self.get_factor_format(levels, reduced_rank=reduced_rank),
             encoded=True,
         )
 
-    def _apply(self, dummies, levels, reduced_rank=True, sparse=False):
+    def _apply(
+        self,
+        dummies: Union[pandas.DataFrame, spsparse.spmatrix],
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[pandas.DataFrame, numpy.ndarray, spsparse.spmatrix]:
         coding_matrix = self.get_coding_matrix(levels, reduced_rank, sparse=sparse)
         return (dummies if sparse else dummies.values) @ coding_matrix
 
     # Coding matrix methods
 
-    def get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
+    def get_coding_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[pandas.DataFrame, spsparse.spmatrix]:
         """
         Generate the coding matrix; i.e. the matrix with column vectors
         representing the encoding to use for the corresponding level.
 
         Args:
             levels: The names of the levels/categories in the data.
             reduced_rank: Whether to output a reduced rank matrix. When this is
@@ -282,40 +319,52 @@
         return pandas.DataFrame(
             coding_matrix,
             columns=self.get_coding_column_names(levels, reduced_rank=reduced_rank),
             index=levels,
         )
 
     @abstractmethod
-    def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
+    def _get_coding_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[numpy.ndarray, spsparse.spmatrix]:
         """
         Subclasses must override this method to implement the generation of the
         coding matrix.
 
         Args:
             levels: The names of the levels/categories in the data.
             reduced_rank: Whether to output the reduced rank coding matrix.
             sparse: Whether to output sparse results.
         """
 
     @abstractmethod
-    def get_coding_column_names(self, levels, reduced_rank=True):
+    def get_coding_column_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         """
         Generate the names for the columns of the coding matrix (the encoded
         features to be added to the model matrix).
 
         Args:
             levels: The names of the levels/categories in the data.
             reduced_rank: Whether to output the coefficients for reduced rank
                 encodings.
         """
 
     # Coefficient matrix methods
 
-    def get_coefficient_matrix(self, levels, reduced_rank=True, sparse=False):
+    def get_coefficient_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[pandas.DataFrame, spsparse.spmatrix]:
         """
         Generate the coefficient matrix; i.e. the matrix with rows representing
         the contrasts effectively computed during a regression, with columns
         indicating the weights given to the origin categories. This is primarily
         used for debugging/introspection.
 
         Args:
@@ -331,15 +380,20 @@
             return coefficient_matrix
         return pandas.DataFrame(
             coefficient_matrix,
             columns=levels,
             index=self.get_coefficient_row_names(levels, reduced_rank=reduced_rank),
         )
 
-    def _get_coefficient_matrix(self, levels, reduced_rank=True, sparse=False):
+    def _get_coefficient_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[numpy.ndarray, spsparse.spmatrix]:
         coding_matrix = self.get_coding_matrix(
             levels, reduced_rank=reduced_rank, sparse=sparse
         )
 
         if reduced_rank:
             coding_matrix = (spsparse if sparse else numpy).hstack(
                 [
@@ -349,52 +403,60 @@
             )
 
         if sparse:
             return scipy.sparse.linalg.inv(coding_matrix.tocsc())
         return numpy.linalg.inv(coding_matrix)
 
     @abstractmethod
-    def get_coefficient_row_names(self, levels, reduced_rank=True):
+    def get_coefficient_row_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[str]:
         """
         Generate the names for the rows of the coefficient matrix (the
         interpretation of the contrasts generated by the coding matrix).
 
         Args:
             levels: The names of the levels/categories in the data.
             reduced_rank: Whether to output the coefficients for reduced rank
                 encodings.
         """
 
     # Additional metadata
 
-    def get_spans_intercept(self, levels, reduced_rank=True) -> bool:
+    def get_spans_intercept(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> bool:
         """
         Determine whether the encoded contrasts span the intercept.
 
         Args:
             levels: The names of the levels/categories in the data.
             reduced_rank: Whether the contrast encoding used had reduced rank.
         """
         return len(levels) > 0 and not reduced_rank
 
-    def get_drop_field(self, levels, reduced_rank=True) -> Union[int, str]:
+    def get_drop_field(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Hashable:
         """
         Determine which column to drop to be full rank after this encoding.
         If this contrast encoding is already reduced in rank, then this method
         should return `None`.
 
         Args:
             levels: The names of the levels/categories in the data.
             reduced_rank: Whether the contrast encoding used had reduced rank.
         """
         if reduced_rank:
             return None
         return self.get_coding_column_names(levels, reduced_rank=reduced_rank)[0]
 
-    def get_factor_format(self, levels, reduced_rank=True):
+    def get_factor_format(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> str:
         """
         The format to use when assigning feature names to each encoded feature.
         Formats can use two named substitutions: `name` and `field`; for
         example: "{name}[{field}]".
 
         Args:
             levels: The names of the levels/categories in the data.
@@ -412,95 +474,114 @@
     is taken to be the first level.
     """
 
     FACTOR_FORMAT = "{name}[T.{field}]"
 
     MISSING = object()
 
-    def __init__(self, base=MISSING):
+    def __init__(self, base: Hashable = MISSING):
         self.base = base
 
     @Contrasts.override
-    def _apply(self, dummies, levels, reduced_rank=True, sparse=False):
+    def _apply(
+        self,
+        dummies: Union[pandas.DataFrame, spsparse.spmatrix],
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[pandas.DataFrame, numpy.ndarray, spsparse.spmatrix]:
         if reduced_rank:
             drop_index = self._find_base_index(levels)
             mask = numpy.ones(len(levels), dtype=bool)
             mask[drop_index] = False
             return (
                 dummies
                 if sparse or isinstance(dummies, numpy.ndarray)
                 else dummies.iloc
             )[:, mask]
         return dummies
 
-    def _find_base_index(self, levels):
+    def _find_base_index(self, levels: Sequence[Hashable]) -> int:
         if self.base is self.MISSING:
             return 0
         try:
             return levels.index(self.base)
         except ValueError as e:
             raise ValueError(
                 f"Value `{repr(self.base)}` for `TreatmentContrasts.base` is not among the provided levels."
             ) from e
 
     @Contrasts.override
-    def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
+    def _get_coding_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[numpy.ndarray, spsparse.spmatrix]:
         n = len(levels)
         if sparse:
             matrix = spsparse.eye(n).tocsc()
         else:
             matrix = numpy.eye(n)
         if reduced_rank:
             drop_level = self._find_base_index(levels)
             matrix = matrix[:, [i for i in range(matrix.shape[1]) if i != drop_level]]
         return matrix
 
     @Contrasts.override
-    def get_coding_column_names(self, levels, reduced_rank=True):
+    def get_coding_column_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         base_index = self._find_base_index(levels)
         if reduced_rank:
             return [level for i, level in enumerate(levels) if i != base_index]
         return levels
 
     @Contrasts.override
-    def get_coefficient_row_names(self, levels, reduced_rank=True):
+    def get_coefficient_row_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         base = levels[self._find_base_index(levels)]
         if reduced_rank:
             return [base, *(f"{level}-{base}" for level in levels if level != base)]
         return levels
 
     @Contrasts.override
-    def get_drop_field(self, levels, reduced_rank=True) -> Union[int, str]:
+    def get_drop_field(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Hashable:
         if reduced_rank:
             return None
         return self.base if self.base is not self.MISSING else levels[0]
 
 
 class SASContrasts(TreatmentContrasts):
     """
     SAS (treatment) contrast coding.
 
     This contrasts generated by this class are the same as
     `TreatmentContrasts`, but with the reference level defaulting to the last
     level (the default in SAS).
     """
 
-    @TreatmentContrasts.override
-    def _find_base_index(self, levels):
+    @TreatmentContrasts.override  # type: ignore[attr-defined]
+    def _find_base_index(self, levels: Sequence[Hashable]) -> int:
         if self.base is self.MISSING:
             return len(levels) - 1
         try:
             return levels.index(self.base)
         except ValueError as e:
             raise ValueError(
                 f"Value `{repr(self.base)}` for `SASContrasts.base` is not among the provided levels."
             ) from e
 
-    @TreatmentContrasts.override
-    def get_drop_field(self, levels, reduced_rank=True) -> Union[int, str]:
+    @TreatmentContrasts.override  # type: ignore[attr-defined]
+    def get_drop_field(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Hashable:
         if reduced_rank:
             return None
         return self.base if self.base is not self.MISSING else levels[-1]
 
 
 class SumContrasts(Contrasts):
     """
@@ -509,30 +590,39 @@
     These contrasts compare the mean of the dependent variable for each level
     (except the last, which is redundant) to the global average of all levels.
     """
 
     FACTOR_FORMAT = "{name}[S.{field}]"
 
     @Contrasts.override
-    def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
+    def _get_coding_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[numpy.ndarray, spsparse.spmatrix]:
         n = len(levels)
         if not reduced_rank:
             return spsparse.eye(n).tocsc() if sparse else numpy.eye(n)
         contr = spsparse.eye(n, n - 1).tolil() if sparse else numpy.eye(n, n - 1)
         contr[-1, :] = -1
         return contr.tocsc() if sparse else contr
 
     @Contrasts.override
-    def get_coding_column_names(self, levels, reduced_rank=True):
+    def get_coding_column_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         if reduced_rank:
             return levels[:-1]
         return levels
 
     @Contrasts.override
-    def get_coefficient_row_names(self, levels, reduced_rank=True):
+    def get_coefficient_row_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         if reduced_rank:
             return ["avg", *(f"{level} - avg" for level in levels[:-1])]
         return levels
 
 
 class HelmertContrasts(Contrasts):
     """
@@ -553,15 +643,20 @@
     FACTOR_FORMAT = "{name}[H.{field}]"
 
     def __init__(self, *, reverse: bool = True, scale: bool = False):
         self.reverse = reverse
         self.scale = scale
 
     @Contrasts.override
-    def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
+    def _get_coding_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[numpy.ndarray, spsparse.spmatrix]:
         n = len(levels)
         if not reduced_rank:
             return spsparse.eye(n).tocsc() if sparse else numpy.eye(n)
 
         contr = spsparse.lil_matrix((n, n - 1)) if sparse else numpy.zeros((n, n - 1))
         for i in range(len(levels) - 1):
             if self.reverse:
@@ -575,21 +670,25 @@
         if self.scale:
             for i in range(n - 1):
                 contr[:, i] /= i + 2 if self.reverse else n - i
 
         return contr
 
     @Contrasts.override
-    def get_coding_column_names(self, levels, reduced_rank=True):
+    def get_coding_column_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         if reduced_rank:
             return levels[1:] if self.reverse else levels[:-1]
         return levels
 
     @Contrasts.override
-    def get_coefficient_row_names(self, levels, reduced_rank=True):
+    def get_coefficient_row_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         if reduced_rank:
             return [
                 "avg",
                 *(
                     f"{level} - rolling_avg"
                     for level in (levels[1:] if self.reverse else levels[:-1])
                 ),
@@ -613,34 +712,43 @@
 
     FACTOR_FORMAT = "{name}[D.{field}]"
 
     def __init__(self, backward: bool = True):
         self.backward = backward
 
     @Contrasts.override
-    def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
+    def _get_coding_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[numpy.ndarray, spsparse.spmatrix]:
         n = len(levels)
         if not reduced_rank:
             return spsparse.eye(n).tocsc() if sparse else numpy.eye(n)
         contr = numpy.repeat([numpy.arange(1, n)], n, axis=0) / n
         contr[numpy.triu_indices(n, m=n - 1)] -= 1
         if not self.backward:
             contr *= -1
         if sparse:
             return spsparse.csc_matrix(contr)
         return contr
 
     @Contrasts.override
-    def get_coding_column_names(self, levels, reduced_rank=True):
+    def get_coding_column_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         if reduced_rank:
             return levels[1:] if self.backward else levels[:-1]
         return levels
 
     @Contrasts.override
-    def get_coefficient_row_names(self, levels, reduced_rank=True):
+    def get_coefficient_row_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         if reduced_rank:
             return [
                 "avg",
                 *(
                     f"{level} - {ref}"
                     for level, ref in (
                         zip(levels[1:], levels)
@@ -668,55 +776,70 @@
     FACTOR_FORMAT = "{name}{field}"
     NAME_ALIASES = {
         1: ".L",
         2: ".Q",
         3: ".C",
     }
 
-    def __init__(self, scores=None):
+    def __init__(self, scores: Optional[Sequence[float]] = None):
         self.scores = scores
 
     @Contrasts.override
-    def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
+    def _get_coding_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[numpy.ndarray, spsparse.spmatrix]:
         n = len(levels)
         if not reduced_rank:
             return spsparse.eye(n).tocsc() if sparse else numpy.eye(n)
         if self.scores and not len(self.scores) == n:
             raise ValueError(
                 "`PolyContrasts.scores` must have the same cardinality as the categories."
             )
         scores = self.scores or numpy.arange(n)
         coding_matrix = poly(scores, degree=n - 1)
         if sparse:
             return spsparse.csc_matrix(coding_matrix)
         return coding_matrix
 
     @Contrasts.override
-    def get_coding_column_names(self, levels, reduced_rank=True):
+    def get_coding_column_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         if reduced_rank:
             return [
                 self.NAME_ALIASES[d] if d in self.NAME_ALIASES else f"^{d}"
                 for d in range(1, len(levels))
             ]
         return levels
 
     @Contrasts.override
-    def get_coefficient_row_names(self, levels, reduced_rank=True):
+    def get_coefficient_row_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         if reduced_rank:
             return ["avg", *self.get_coding_column_names(levels, reduced_rank=True)]
         return levels
 
 
 class CustomContrasts(Contrasts):
     """
     Handle the custom contrast case when users pass in hand-coded contrast
     matrices.
     """
 
-    def __init__(self, contrasts, names=None):
+    def __init__(
+        self,
+        contrasts: Union[
+            Dict[Hashable, Sequence[float]], Sequence[Sequence[float]], numpy.ndarray
+        ],
+        names: Optional[Sequence[Hashable]] = None,
+    ):
         if isinstance(contrasts, dict):
             if names is None:
                 names = list(contrasts)
             contrasts = numpy.array([*contrasts.values()]).T
         else:
             contrasts = numpy.array(contrasts)
 
@@ -725,35 +848,48 @@
                 "Names must be aligned with the columns of the contrast array."
             )
 
         self.contrasts = contrasts
         self.contrast_names = names
 
     @Contrasts.override
-    def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
+    def _get_coding_matrix(
+        self,
+        levels: Sequence[Hashable],
+        reduced_rank: bool = True,
+        sparse: bool = False,
+    ) -> Union[numpy.ndarray, spsparse.spmatrix]:
         if sparse:
             return spsparse.csc_matrix(self.contrasts)
         return self.contrasts
 
     @Contrasts.override
-    def get_coding_column_names(self, levels, reduced_rank=True):
+    def get_coding_column_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         if self.contrast_names:
             return self.contrast_names
         return list(range(1, self.contrasts.shape[1] + 1))
 
     @Contrasts.override
-    def get_coefficient_row_names(self, levels, reduced_rank=True):
+    def get_coefficient_row_names(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Sequence[Hashable]:
         return list(range(1, len(levels) + (0 if not reduced_rank else 1)))
 
     @Contrasts.override
-    def get_spans_intercept(self, levels, reduced_rank=True) -> bool:
+    def get_spans_intercept(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> bool:
         return False
 
     @Contrasts.override
-    def get_drop_field(self, levels, reduced_rank=True) -> Union[int, str]:
+    def get_drop_field(
+        self, levels: Sequence[Hashable], reduced_rank: bool = True
+    ) -> Hashable:
         return None
 
 
 class ContrastsRegistry(type):
     """
     The contrast registry, which is exposed in formulae as "contr".
     """
```

### Comparing `formulaic-0.6.3/formulaic/transforms/patsy_compat.py` & `formulaic-0.6.4/formulaic/transforms/patsy_compat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,38 @@
+from typing import Any, Dict, Mapping, Optional
 from formulaic.utils.stateful_transforms import stateful_transform
 
 from .contrasts import (
     TreatmentContrasts,
     PolyContrasts,
     SumContrasts,
     HelmertContrasts,
     DiffContrasts,
 )
 from .scale import scale
 
 
 @stateful_transform
-def standardize(x, center=True, rescale=True, ddof=0, _state=None):
+def standardize(
+    x: Any,
+    center: bool = True,
+    rescale: bool = True,
+    ddof: int = 0,
+    _state: Optional[Dict[str, Any]] = None,
+) -> Any:
     return scale(x, center=center, scale=rescale, ddof=ddof, _state=_state)
 
 
-def Treatment(reference=TreatmentContrasts.MISSING):
+def Treatment(reference: Any = TreatmentContrasts.MISSING) -> TreatmentContrasts:
     return TreatmentContrasts(base=reference)
 
 
 @stateful_transform
-def Q(variable, _context=None):
-    return _context.data[variable]
+def Q(variable: str, _context: Optional[Mapping[str, Any]] = None) -> Any:
+    return _context.data[variable]  # type: ignore
 
 
 PATSY_COMPAT_TRANSFORMS = {
     "standardize": standardize,
     "Q": Q,
     "Treatment": Treatment,
     "Poly": PolyContrasts,
```

### Comparing `formulaic-0.6.3/formulaic/transforms/poly.py` & `formulaic-0.6.4/formulaic/transforms/poly.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     import numpy.typing
 except ImportError as e:  # pragma: no cover
     if TYPE_CHECKING:
         raise RuntimeError("Numpy >=1.20 is required for type-checking.") from e
 
 
 @stateful_transform
-def poly(
-    x: numpy.typing.ArrayLike, degree: int = 1, raw: bool = False, _state=None
+def poly(  # pylint: disable=dangerous-default-value  # always replaced by stateful-transform
+    x: numpy.typing.ArrayLike, degree: int = 1, raw: bool = False, _state: dict = {}
 ) -> numpy.ndarray:
     """
     Generate a basis for a polynomial vector-space representation of `x`.
 
     The basis vectors returned by this transform can be used, for example, to
     capture non-linear dependence on `x` in a linear regression.
 
@@ -85,25 +85,25 @@
         norms2 = {}
 
     # Build polynomials iteratively using the monic three-term recurrence relation
     # Note that alpha and beta are fixed if not in "training" mode.
     P = numpy.empty((x.shape[0], degree + 1))
     P[:, 0] = 1
 
-    def get_alpha(k):
+    def get_alpha(k: int) -> float:
         if training and k not in alpha:
-            alpha[k] = numpy.sum(x * P[:, k] ** 2) / numpy.sum(P[:, k] ** 2)
+            alpha[k] = numpy.sum(x * P[:, k] ** 2) / numpy.sum(P[:, k] ** 2)  # type: ignore[operator]
         return alpha[k]
 
-    def get_norm(k):
-        if training and k not in norms2:
-            norms2[k] = numpy.sum(P[:, k] ** 2)
-        return norms2[k]
+    def get_norm(k: int) -> float:
+        if training and k not in norms2:  # type: ignore[operator]
+            norms2[k] = numpy.sum(P[:, k] ** 2)  # type: ignore[index]
+        return norms2[k]  # type: ignore[index]
 
-    def get_beta(k):
+    def get_beta(k: int) -> float:
         return get_norm(k) / get_norm(k - 1)
 
     for i in range(1, degree + 1):
         P[:, i] = (x - get_alpha(i - 1)) * P[:, i - 1]
         if i >= 2:
             P[:, i] -= get_beta(i - 1) * P[:, i - 2]
```

### Comparing `formulaic-0.6.3/formulaic/transforms/scale.py` & `formulaic-0.6.4/formulaic/transforms/scale.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+from typing import Any
 import numpy
 import scipy.sparse as spsparse
 
 from formulaic.utils.stateful_transforms import stateful_transform
 
 
 @stateful_transform
-def scale(data, center=True, scale=True, ddof=1, _state=None):
+def scale(  # pylint: disable=dangerous-default-value  # always replaced by stateful-transform
+    data: Any,
+    center: bool = True,
+    scale: bool = True,
+    ddof: float = 1,
+    _state: dict = {},
+) -> numpy.ndarray:
     """
     Rescale `data` by centering and re-scaling it.
 
     Args:
         center: Whether to center the data (subtract the mean).
         scale: Whether to rescale the data such that the standard deviation is
             1.
@@ -47,19 +54,21 @@
             _state["scale"] = None
     if _state["scale"] is not None:
         data = data / _state["scale"]
 
     return data
 
 
-@scale.register(spsparse.spmatrix)
-def _(data, *args, **kwargs):
+@scale.register  # type: ignore[attr-defined]
+def _(data: spsparse.spmatrix, *args: Any, **kwargs: Any) -> numpy.ndarray:
     assert data.shape[1] == 1
     return scale(data.toarray()[:, 0], *args, **kwargs)
 
 
 @stateful_transform
-def center(data, _state=None):
+def center(  # pylint: disable=dangerous-default-value  # always replaced by stateful-transform
+    data: Any, _state: dict = {}
+) -> numpy.ndarray:
     """
     Centers the data by subtracting the mean.
     """
     return scale(data, scale=False, _state=_state)
```

### Comparing `formulaic-0.6.3/formulaic/utils/calculus.py` & `formulaic-0.6.4/formulaic/utils/calculus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Iterable, Set
+from typing import Iterable, Set, cast
 
 from formulaic.parser.types import Factor, Term
 from formulaic.parser.types.ordered_set import OrderedSet
 
 
 def differentiate_term(
     term: Term,
-    vars: Iterable[str],  # pylint: disable=redefined-builtin
+    wrt: Iterable[str],  # pylint: disable=redefined-builtin
     use_sympy: bool = False,
 ) -> Term:
     """
-    Symbolically differentiate a `Term` instance with respect to one or more `vars`.
+    Symbolically differentiate a `Term` instance with respect to one or more `wrt`.
 
     Args:
         term: The `Term` instance to differentiate.
-        vars: The variables by which to differentiate.
+        wrt: The variables by which to differentiate.
         use_sympy: Whether to interpret factor token strings using sympy. If
             `True`, symbolic factors like `log(x)` can be differentiated with
             respect to `x`. If `False`, factor token strings must match the
             variable exactly in order to be detected.
 
     Returns:
         A new `Term` instance representing the differentiated term.
@@ -27,24 +27,26 @@
         - This method takes into account the chain rule/etc.
         - Care must be taken to make sure that the symbolic representation of
             the factors can be properly interpreted by `sympy`. For example, `I(x)`
             would not be understood.
     """
     factors = OrderedSet(term.factors)
 
-    for var in vars:
+    for var in wrt:
         affected_factors = set(
             factor
             for factor in factors
             if var in _factor_symbols(factor, use_sympy=use_sympy)
         )
         if not affected_factors:
             return Term({Factor("0", eval_method="literal")})
-        factors = (factors - affected_factors) | (
-            _differentiate_factors(affected_factors, var, use_sympy=use_sympy)
+        factors = cast(
+            OrderedSet,
+            (factors - affected_factors)
+            | (_differentiate_factors(affected_factors, var, use_sympy=use_sympy)),
         )
 
     return Term(factors or {Factor("1", eval_method="literal")})
 
 
 def _factor_symbols(factor: Factor, use_sympy: bool = False) -> Set[str]:
     """
@@ -90,15 +92,15 @@
     if use_sympy:
         try:
             import sympy
 
             expr = sympy.S(
                 "(" + ") * (".join(factor.expr for factor in factors) + ")"
             ).diff(var)
-            eval_method = "python"
+            eval_method = Factor.EvalMethod.PYTHON
         except ImportError as e:  # pragma: no cover
             raise ImportError(
                 "`sympy` is not available. Install it using `pip install formulaic[calculus]` or `pip install sympy`."
             ) from e
     else:
         assert len(factors) == 1
         expr = 1
```

### Comparing `formulaic-0.6.3/formulaic/utils/cast.py` & `formulaic-0.6.4/formulaic/utils/cast.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from functools import singledispatch, wraps
-from typing import Any
+from typing import Any, Callable, Dict, Hashable, Union
 
 import numpy
 import pandas
 import scipy.sparse
 
 from formulaic.materializers.types.factor_values import FactorValues
 
 
-def propagate_metadata(func):
+def propagate_metadata(func: Callable) -> Callable:
     @wraps(func)
-    def wrapper(data, *args, **kwargs):
+    def wrapper(data, *args, **kwargs):  # type: ignore[no-untyped-def]
         evaluated = func(data, *args, **kwargs)
         if isinstance(data, FactorValues):
             return FactorValues(
                 evaluated,
                 metadata=data.__formulaic_metadata__,
             )
         return evaluated
@@ -30,21 +30,21 @@
     dictionary (the format used to store columns), it is returned as is.
     """
     return data
 
 
 @as_columns.register
 @propagate_metadata
-def _(data: pandas.DataFrame):
+def _(data: pandas.DataFrame) -> Dict[Hashable, pandas.Series]:
     return dict(data.items())
 
 
 @as_columns.register
 @propagate_metadata
-def _(data: numpy.ndarray):
+def _(data: numpy.ndarray) -> Union[numpy.ndarray, Dict[Hashable, numpy.ndarray]]:
     if len(data.shape) == 1:
         return data
     if len(data.shape) > 2:
         raise ValueError(
             "Formulaic does not know how to convert numpy arrays with more than "
             "two dimensions into columns."
         )
@@ -56,15 +56,15 @@
     else:
         column_names = list(range(data.shape[1]))
     return {column_names[i]: data[:, i] for i in range(data.shape[1])}
 
 
 @as_columns.register
 @propagate_metadata
-def _(data: scipy.sparse.csc_matrix):
+def _(data: scipy.sparse.csc_matrix) -> Dict[Hashable, scipy.sparse.spmatrix]:
     if (
         hasattr(data, "__formulaic_metadata__")
         and data.__formulaic_metadata__.column_names
     ):
         column_names = data.__formulaic_metadata__.column_names
     else:
         column_names = list(range(data.shape[1]))
```

### Comparing `formulaic-0.6.3/formulaic/utils/constraints.py` & `formulaic-0.6.4/formulaic/utils/constraints.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 from __future__ import annotations
 
 import ast
 import functools
 import itertools
 from numbers import Number
-from typing import Dict, Iterable, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Union,
+    cast,
+)
+from typing_extensions import Literal
 
 import numpy
 
 from formulaic.parser.algos.tokenize import tokenize
 from formulaic.parser.algos.tokens_to_ast import tokens_to_ast
 from formulaic.parser.types import (
     ASTNode,
     Factor,
     OperatorResolver,
     Operator,
-    Term,
     Token,
 )
 from formulaic.parser.utils import exc_for_token
 
 
 LinearConstraintSpec = Union[
     str,
@@ -45,15 +56,15 @@
         constraint_values: The vector of constant values ($b$ from above).
         variable_names: The ordered names of the variables represented by $x$;
             typically the column names of a `ModelMatrix` instance.
     """
 
     @classmethod
     def from_spec(
-        cls, spec: LinearConstraintSpec, variable_names: Sequence[str] = None
+        cls, spec: LinearConstraintSpec, variable_names: Optional[Sequence[str]] = None
     ) -> LinearConstraints:
         """
         Construct a `LinearConstraints` instance from a specification.
 
         Args:
             spec: The specification from which to derive the constraints. Can be
                 a:
@@ -68,38 +79,45 @@
                     * numpy.ndarray: a constraint matrix (with all values
                         assumed to be zero).
             variable_names: The ordered names of the variables represented by
                 $x$; typically the column names of a `ModelMatrix` instance.
         """
         if isinstance(spec, LinearConstraints):
             return spec
-        if isinstance(spec, str):
-            matrix, values = LinearConstraintParser(
-                variable_names=variable_names
-            ).get_matrix(spec)
-            return cls(matrix, values, variable_names)
-        if isinstance(spec, dict):
+        if isinstance(spec, (str, dict)):
+            if variable_names is None:
+                raise ValueError(
+                    "`variable_names` must be provided when parsing constraints from a formula."
+                )
+            if isinstance(spec, str):
+                matrix, values = LinearConstraintParser(
+                    variable_names=variable_names
+                ).get_matrix(spec)
+                return cls(matrix, values, variable_names)
             matrices, constants = [], []
             for key, constant in spec.items():
                 matrix, values = LinearConstraintParser(
                     variable_names=variable_names
                 ).get_matrix(key)
                 matrices.append(matrix)
                 constants.append(values + numpy.array(constant))
             return cls(
                 numpy.vstack(matrices),
                 numpy.hstack(constants),
                 variable_names=variable_names,
             )
         if isinstance(spec, tuple) and len(spec) == 2:
-            return cls(*spec, variable_names=variable_names)
-        return cls(spec, 0, variable_names=variable_names)
+            return cls(*spec, variable_names=variable_names)  # type: ignore
+        return cls(spec, 0, variable_names=variable_names)  # type: ignore
 
     def __init__(
-        self, constraint_matrix, constraint_values, variable_names: Sequence[str] = None
+        self,
+        constraint_matrix: "numpy.typing.ArrayLike",
+        constraint_values: "numpy.typing.ArrayLike",
+        variable_names: Optional[Sequence[str]] = None,
     ):
         """
         Attributes:
             constraint_matrix: The matrix of coefficients on the features ($A$ from
                 above). Each row is one constraint.
             constraint_values: The vector of constant values ($b$ from above).
             variable_names: The ordered names of the variables represented by $x$;
@@ -135,40 +153,40 @@
 
         self.constraint_matrix = constraint_matrix
         self.constraint_values = constraint_values
         self.variable_names = variable_names or [
             f"x{i}" for i in range(len(constraint_matrix))
         ]
 
-    def __str__(self):
+    def __str__(self) -> str:
         out = []
         for i in range(self.constraint_matrix.shape[0]):
             out_one = []
             for nonzero_col in numpy.where(self.constraint_matrix[i, :])[0]:
                 out_one.append(
                     f"{self.constraint_matrix[i, nonzero_col]} * {self.variable_names[nonzero_col]}"
                 )
             out.append(" + ".join(out_one) + f" = {self.constraint_values[i]}")
         return "\n".join(out)
 
-    def show(self):
+    def show(self) -> None:
         """
         Pretty-print the constraints.
         """
         print(str(self))
 
     @property
-    def n_constraints(self):
+    def n_constraints(self) -> int:
         """
         The number of constraints represented by this `LinearConstraints`
         instance.
         """
         return self.constraint_matrix.shape[0]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<LinearConstraints: {self.n_constraints} constraints>"
 
 
 class LinearConstraintParser:
     """
     A linear constraint parser.
 
@@ -197,38 +215,46 @@
         Tokenize a constraint formula.
 
         Args:
             formula: The constraint formula to tokenize.
         """
         return [ConstraintToken.for_token(token) for token in tokenize(formula)]
 
-    def get_ast(self, formula: str) -> ASTNode:
+    def get_ast(self, formula: str) -> Optional[ASTNode]:
         """
         Assemble an abstract syntax tree for the nominated `formula` string.
 
         Args:
             formula: The constraint formula for which an AST should be
                 generated.
         """
-        return tokens_to_ast(
-            self.get_tokens(formula),
-            operator_resolver=self.operator_resolver,
+        return cast(
+            Optional[ASTNode],
+            tokens_to_ast(
+                self.get_tokens(formula),
+                operator_resolver=self.operator_resolver,
+            ),
         )
 
-    def get_terms(self, formula: str) -> Union[Sequence[Term], Tuple[Sequence[Term]]]:
+    def get_terms(
+        self, formula: str
+    ) -> Union[None, List[ScaledFactor], Tuple[List[ScaledFactor], ...]]:
         """
-        Build the `Term` instances for a constraint formula string.
+        Build the `ScaledFactor` instances for a constraint formula string.
 
         Args:
             formula: The constraint formula for which to build terms.
         """
         ast = self.get_ast(formula)
         if not ast:
             return None
-        return ast.to_terms()
+        return cast(
+            Union[None, List[ScaledFactor], Tuple[List[ScaledFactor], ...]],
+            ast.to_terms(),
+        )
 
     def get_matrix(
         self, formula: str
     ) -> Tuple["numpy.typing.ArrayLike", "numpy.typing.ArrayLike"]:
         """
         Build the constraint matrix and constraint values vector associated with
         the parsed string.
@@ -252,45 +278,48 @@
         )
 
         matrix = []
         constants = []
 
         for constraint in constraints:
             vector = numpy.zeros(len(self.variable_names))
-            constant = 0
-            for term in constraint:
-                if term.factor == 1:
-                    constant += term.scale
+            constant: float = 0
+            for scaled_factor in constraint:
+                if scaled_factor.factor == 1:
+                    constant += scaled_factor.scale
                 else:
-                    vector += term.scale * col_vectors[term.factor.expr]
+                    vector += (
+                        scaled_factor.scale
+                        * col_vectors[cast(Factor, scaled_factor.factor).expr]
+                    )
             matrix.append(vector)
             constants.append(-constant)
 
         return numpy.array(matrix), numpy.array(constants)
 
 
 class ConstraintToken(Token):
     """
     An enriched `Token` subclass that overrides `.to_terms()` to return
     a set of `ScaledFactor`s rather than `Terms`s.
     """
 
     @classmethod
-    def for_token(cls, token: Token):
+    def for_token(cls, token: Token) -> ConstraintToken:
         return cls(
             **{
                 attr: getattr(token, attr)
                 for attr in ("token", "kind", "source", "source_start", "source_end")
             }
         )
 
-    def to_terms(self):
+    def to_terms(self) -> Set[ScaledFactor]:  # type: ignore[override]
         if self.kind is Token.Kind.VALUE:
             factor = ast.literal_eval(self.token)
-            if isinstance(factor, Number):
+            if isinstance(factor, (int, float)):
                 return {ScaledFactor(1, scale=factor)}
             raise exc_for_token(
                 self,
                 message="Only numeric literal values are permitted in constraint formulae.",
             )
         return {ScaledFactor(self.to_factor())}
 
@@ -302,78 +331,82 @@
     `Factor`.
 
     Attributes:
         factor: The wrapped `Factor` instance.
         scale: The scalar value to be used as the coefficient of this factor.
     """
 
-    def __init__(self, factor: Factor, *, scale: Number = 1):
+    def __init__(self, factor: Union[Factor, Literal[1]], *, scale: float = 1):
         self.factor = factor
         self.scale = scale
 
-    def __add__(self, other):
+    def __add__(self, other: Any) -> ScaledFactor:
         if isinstance(other, ScaledFactor):
             return ScaledFactor(self.factor, scale=self.scale + other.scale)
         return NotImplemented  # pragma: no cover
 
-    def __sub__(self, other):
+    def __sub__(self, other: Any) -> ScaledFactor:
         if isinstance(other, ScaledFactor):
             return ScaledFactor(self.factor, scale=self.scale - other.scale)
         return NotImplemented  # pragma: no cover
 
-    def __neg__(self):
+    def __neg__(self) -> ScaledFactor:
         return ScaledFactor(self.factor, scale=-self.scale)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(self.factor)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, ScaledFactor):
             return self.factor == other.factor
         return NotImplemented  # pragma: no cover
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.scale}*{self.factor}"  # pragma: no cover
 
 
 class ConstraintOperatorResolver(
     OperatorResolver
 ):  # pylint: disable=unnecessary-lambda
     """
     The default constraint `OperatorResolver` implementation.
 
     These operators describe a regular algebra rather than a Wikinson formula
     one.
     """
 
     @property
-    def operators(self):
-        def join_tuples(lhs, rhs):
+    def operators(self) -> List[Operator]:
+        def join_tuples(lhs: Any, rhs: Any) -> Tuple:
             if not isinstance(lhs, tuple):
                 lhs = (lhs,)
             if not isinstance(rhs, tuple):
                 rhs = (rhs,)
             return lhs + rhs
 
-        def add_terms(terms_left, terms_right):
+        def add_terms(
+            terms_left: Set[ScaledFactor], terms_right: Set[ScaledFactor]
+        ) -> Set[ScaledFactor]:
 
             terms_left = {term: term for term in terms_left}
             terms_right = {term: term for term in terms_right}
 
             added = set()
 
             for term in terms_left:
                 if term in terms_right:
                     term = term + terms_right[term]
                 added.add(term)
             added.update({term for term in terms_right if term not in added})
 
             return added
 
-        def sub_terms(terms_left, terms_right):
+        def sub_terms(
+            terms_left: Set[ScaledFactor], terms_right: Set[ScaledFactor]
+        ) -> Set[ScaledFactor]:
 
             terms_left = {term: term for term in terms_left}
             terms_right = {term: term for term in terms_right}
 
             added = set()
 
             for term in terms_left:
@@ -382,53 +415,57 @@
                 added.add(term)
             added.update(
                 negate_terms({term for term in terms_right if term not in added})
             )
 
             return added
 
-        def negate_terms(terms):
+        def negate_terms(terms: Set[ScaledFactor]) -> Set[ScaledFactor]:
             return {-term for term in terms}
 
-        def mul_terms(terms_left, terms_right):
+        def mul_terms(
+            terms_left: Set[ScaledFactor], terms_right: Set[ScaledFactor]
+        ) -> Set[ScaledFactor]:
             terms_left = {term: term for term in terms_left}
             terms_right = {term: term for term in terms_right}
 
-            terms = set()
+            terms: Set[ScaledFactor] = set()
 
             for term_left, term_right in itertools.product(terms_left, terms_right):
                 terms = add_terms(terms, {mul_term(term_left, term_right)})
 
             return terms
 
-        def mul_term(term_left, term_right):
+        def mul_term(term_left: ScaledFactor, term_right: ScaledFactor) -> ScaledFactor:
             if term_left.factor == 1:
                 return ScaledFactor(
                     term_right.factor, scale=term_left.scale * term_right.scale
                 )
             if term_right.factor == 1:
                 return ScaledFactor(
                     term_left.factor, scale=term_left.scale * term_right.scale
                 )
             raise RuntimeError(
                 "Only one non-scalar factor can be involved in a linear constraint multiplication."
             )
 
-        def div_terms(terms_left, terms_right):
+        def div_terms(
+            terms_left: Set[ScaledFactor], terms_right: Set[ScaledFactor]
+        ) -> Set[ScaledFactor]:
             terms_left = {term: term for term in terms_left}
             terms_right = {term: term for term in terms_right}
 
-            terms = set()
+            terms: Set[ScaledFactor] = set()
 
             for term_left, term_right in itertools.product(terms_left, terms_right):
                 terms = add_terms(terms, {div_term(term_left, term_right)})
 
             return terms
 
-        def div_term(term_left, term_right):
+        def div_term(term_left: ScaledFactor, term_right: ScaledFactor) -> ScaledFactor:
             if term_right.factor == 1:
                 return ScaledFactor(
                     term_left.factor, scale=term_left.scale / term_right.scale
                 )
             raise RuntimeError(
                 "The right-hand operand must be a scalar in linear constraint division operations."
             )
@@ -436,15 +473,17 @@
         return [
             Operator(
                 ",",
                 arity=2,
                 precedence=-200,
                 associativity=None,
                 to_terms=join_tuples,
-                accepts_context=lambda context: all(c.symbol == "," for c in context),
+                accepts_context=lambda context: all(
+                    c.symbol == "," for c in context if isinstance(c, Operator)
+                ),
                 structural=True,
             ),
             Operator(
                 "=",
                 arity=2,
                 precedence=-100,
                 associativity=None,
```

### Comparing `formulaic-0.6.3/formulaic/utils/context.py` & `formulaic-0.6.4/formulaic/utils/context.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/formulaic/utils/iterators.py` & `formulaic-0.6.4/formulaic/utils/iterators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import Any, Iterable
+from typing import Any, Iterable, Iterator, List
 
 from .sentinels import MISSING
 
 
 class peekable_iter:
     """
     An iterator that allows you to peek at the next element during iteration.
     """
 
     def __init__(self, it: Iterable):
         self._it = iter(it)
-        self._next = []
+        self._next: List[Any] = []
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator:
         return self
 
-    def __next__(self):
+    def __next__(self) -> Any:
         if self._next:
             return self._next.pop(0)
         return next(self._it)
 
     def peek(self, default: Any = MISSING) -> Any:
         """
         Retrieve the object that will be next returned by the iterator.
```

### Comparing `formulaic-0.6.3/formulaic/utils/sparse.py` & `formulaic-0.6.4/formulaic/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/formulaic/utils/stateful_transforms.py` & `formulaic-0.6.4/formulaic/utils/stateful_transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import ast
 import functools
 import inspect
 import keyword
 import re
-from typing import Any, Callable, Mapping, MutableMapping, Optional, TYPE_CHECKING
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Mapping,
+    MutableMapping,
+    Optional,
+    TYPE_CHECKING,
+    cast,
+)
 
 import astor
 import numpy
 
 from .iterators import peekable_iter
 from .layered_mapping import LayeredMapping
 
@@ -38,15 +47,15 @@
     Returns:
         The stateful transform callable.
     """
     func = functools.singledispatch(func)
     params = set(inspect.signature(func).parameters.keys())
 
     @functools.wraps(func)
-    def wrapper(
+    def wrapper(  # type: ignore[no-untyped-def]
         data, *args, _metadata=None, _state=None, _spec=None, _context=None, **kwargs
     ):
         from formulaic.model_spec import ModelSpec
 
         _state = {} if _state is None else _state
         extra_params = {}
         if "_metadata" in params:
@@ -74,23 +83,23 @@
             data,
             *args,
             **({"_state": _state} if "_state" in params else {}),
             **extra_params,
             **kwargs,
         )
 
-    wrapper.__is_stateful_transform__ = True
+    wrapper.__is_stateful_transform__ = True  # type: ignore[attr-defined]
     return wrapper
 
 
 def stateful_eval(
     expr: str,
     env: Optional[Mapping],
     metadata: Optional[Mapping],
-    state: Optional[Mapping],
+    state: Optional[MutableMapping],
     spec: Optional["ModelSpec"],
 ) -> Any:
     """
     Evaluate an expression in a nominated environment and with a nominated state.
 
     Under the hood this calls out to `eval`, and so if incoming expressions are
     not safe, you should make sure that your `env` is properly isolated from
@@ -126,18 +135,20 @@
     # If not, create new variable in mutable env layer, and update code.
     expr = sanitize_variable_names(expr, env)
 
     # Parse Python code
     code = ast.parse(expr, mode="eval")
 
     # Extract the nodes of the graph that correspond to stateful transforms
-    stateful_nodes = {}
+    stateful_nodes: Dict[str, ast.Call] = {}
     for node in ast.walk(code):
         if _is_stateful_transform(node, env):
-            stateful_nodes[astor.to_source(node).strip().replace("\n    ", "")] = node
+            stateful_nodes[astor.to_source(node).strip().replace("\n    ", "")] = cast(
+                ast.Call, node
+            )
 
     # Mutate stateful nodes to pass in state from a shared dictionary.
     for name, node in stateful_nodes.items():
         name = name.replace('"', r'\\\\"')
         if name not in state:
             state[name] = {}
         node.keywords.append(
@@ -158,24 +169,24 @@
             )
         )
         node.keywords.append(
             ast.keyword("_spec", ast.parse("__FORMULAIC_SPEC__", mode="eval").body)
         )
 
     # Compile mutated AST
-    code = compile(ast.fix_missing_locations(code), "", "eval")
+    compiled = compile(ast.fix_missing_locations(code), "", "eval")
 
     assert "__FORMULAIC_CONTEXT__" not in env
     assert "__FORMULAIC_METADATA__" not in env
     assert "__FORMULAIC_STATE__" not in env
     assert "__FORMULAIC_SPEC__" not in env
 
     # Evaluate and return
     return eval(
-        code,
+        compiled,
         {},
         LayeredMapping(
             {
                 "__FORMULAIC_CONTEXT__": env,
                 "__FORMULAIC_METADATA__": metadata,
                 "__FORMULAIC_SPEC__": spec,
                 "__FORMULAIC_STATE__": state,
@@ -215,15 +226,15 @@
 
 
 UNQUOTED_BACKTICK_MATCHER = re.compile(
     r"(\\\"|\"(?:\\\"|[^\"])*\"|\\'|'(?:\\'|[^'])*'|`)"
 )
 
 
-def sanitize_variable_names(expr: str, env: Mapping) -> str:
+def sanitize_variable_names(expr: str, env: MutableMapping) -> str:
     """
     Sanitize any variables names in the expression that are not valid Python
     identifiers and are surrounded by backticks (`). This allows use of field
     names that are not valid Python names.
 
     This function transforms `expr` into a new expression where identifiers that
     would cause `SyntaxError`s are transformed into valid Python identifiers.
```

### Comparing `formulaic-0.6.3/tests/test_formula.py` & `formulaic-0.6.4/tests/test_formula.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/test_model_matrix.py` & `formulaic-0.6.4/tests/test_model_matrix.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/test_model_spec.py` & `formulaic-0.6.4/tests/test_model_spec.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import OrderedDict
 from pyexpat import model
 import re
 
 import pytest
 
 import numpy
 import pandas
@@ -67,34 +66,43 @@
                 "A[T.b]:a",
                 "A[T.c]:a",
             )
         )
         assert (
             model_spec.column_indices
             == model_spec.feature_indices
-            == OrderedDict(
-                [
-                    ("Intercept", 0),
-                    ("a", 1),
-                    ("A[T.b]", 2),
-                    ("A[T.c]", 3),
-                    ("A[T.b]:a", 4),
-                    ("A[T.c]:a", 5),
-                ]
-            )
-        )
-        assert model_spec.term_slices == OrderedDict(
-            [
-                ("1", slice(0, 1)),
-                ("a", slice(1, 2)),
-                ("A", slice(2, 4)),
-                ("A:a", slice(4, 6)),
-            ]
+            == {
+                "Intercept": 0,
+                "a": 1,
+                "A[T.b]": 2,
+                "A[T.c]": 3,
+                "A[T.b]:a": 4,
+                "A[T.c]:a": 5,
+            }
         )
+        assert model_spec.term_slices == {
+            "1": slice(0, 1),
+            "a": slice(1, 2),
+            "A": slice(2, 4),
+            "A:a": slice(4, 6),
+        }
         assert model_spec.terms == ["1", "a", "A", "A:a"]
+        assert model_spec.term_variables == {
+            "1": set(),
+            "a": {"a"},
+            "A": {"A"},
+            "A:a": {"a", "A"},
+        }
+        assert model_spec.variable_terms == {"a": {"a", "A:a"}, "A": {"A", "A:a"}}
+        assert model_spec.variable_indices == {
+            "a": [1, 4, 5],
+            "A": [2, 3, 4, 5],
+        }
+        assert model_spec.variables == {"a", "A"}
+        assert model_spec.variables_by_source == {"data": {"a", "A"}}
 
     @pytest.mark.filterwarnings(
         r"ignore:`ModelSpec\.feature_names` is deprecated.*:DeprecationWarning"
     )
     def test_get_model_matrix(self, model_spec, data2):
         m = model_spec.get_model_matrix(data2)
 
@@ -181,7 +189,40 @@
 
         # Validate differentiation
         assert model_specs.differentiate("a").a == model_spec.differentiate("a")
 
         # Validate invalid type checking
         with pytest.raises(TypeError, match="`ModelSpecs` instances expect all.*"):
             ModelSpecs("invalid type!")
+
+    def test_empty(self):
+        model_spec = ModelSpec([])
+
+        with pytest.raises(
+            RuntimeError,
+            match=re.escape(
+                "`ModelSpec.structure` has not yet been populated. This will "
+                "likely be resolved by using the `ModelSpec` instance attached "
+                "to the model matrix generated when calling `.get_model_matrix()`."
+            ),
+        ):
+            model_spec.column_names
+
+        with pytest.raises(
+            RuntimeError,
+            match=re.escape(
+                "`ModelSpec.structure` has not yet been populated. This will "
+                "likely be resolved by using the `ModelSpec` instance attached "
+                "to the model matrix generated when calling `.get_model_matrix()`."
+            ),
+        ):
+            model_spec.term_indices
+
+        with pytest.raises(
+            RuntimeError,
+            match=re.escape(
+                "`ModelSpec.structure` has not yet been populated. This will "
+                "likely be resolved by using the `ModelSpec` instance attached "
+                "to the model matrix generated when calling `.get_model_matrix()`."
+            ),
+        ):
+            model_spec.term_variables
```

### Comparing `formulaic-0.6.3/tests/test_sugar.py` & `formulaic-0.6.4/tests/test_sugar.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/materializers/test_arrow.py` & `formulaic-0.6.4/tests/materializers/test_arrow.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/materializers/test_base.py` & `formulaic-0.6.4/tests/materializers/test_base.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/materializers/test_pandas.py` & `formulaic-0.6.4/tests/materializers/test_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from formulaic import ModelMatrices
 from formulaic.errors import (
     FactorEncodingError,
     FactorEvaluationError,
     FormulaMaterializationError,
 )
 from formulaic.materializers import PandasMaterializer
+from formulaic.materializers.base import EncodedTermStructure
 from formulaic.materializers.types import EvaluatedFactor, FactorValues, NAAction
 from formulaic.model_spec import ModelSpec
 from formulaic.parser.types import Factor, Structured
 
 
 PANDAS_TESTS = {
     # '<formula>': (<full_rank_names>, <names>, <full_rank_null_names>, <null_rows>)
@@ -414,18 +415,24 @@
 
     def test_no_levels_encoding(self, data):
         mm = PandasMaterializer(data, output="pandas").get_model_matrix("a + D")
 
         assert mm.model_spec.column_names == ("Intercept", "a")
         assert mm.shape == (3, 2)
 
-        print(mm)
-
         mm = PandasMaterializer(data, output="sparse").get_model_matrix("a + D")
 
         assert mm.model_spec.column_names == ("Intercept", "a")
         assert mm.shape == (3, 2)
 
         mm = PandasMaterializer(data, output="numpy").get_model_matrix("a + D")
 
         assert mm.model_spec.column_names == ("Intercept", "a")
         assert mm.shape == (3, 2)
+
+    def test_none_values(self, data):
+        mm = PandasMaterializer(data, output="pandas").get_model_matrix("{None} -1")
+        assert mm.shape == (3, 0)
+        assert len(mm.model_spec.structure) == 1
+        assert mm.model_spec.structure == [
+            EncodedTermStructure(term="None", scoped_terms=[], columns=[]),
+        ]
```

### Comparing `formulaic-0.6.3/tests/materializers/types/test_evaluated_factor.py` & `formulaic-0.6.4/tests/materializers/types/test_evaluated_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/materializers/types/test_scoped_factor.py` & `formulaic-0.6.4/tests/materializers/types/test_scoped_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/test_parser.py` & `formulaic-0.6.4/tests/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/test_utils.py` & `formulaic-0.6.4/tests/parser/test_utils.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/algos/test_tokenize.py` & `formulaic-0.6.4/tests/parser/algos/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/algos/test_tokens_to_ast.py` & `formulaic-0.6.4/tests/parser/algos/test_tokens_to_ast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/types/test_ast_node.py` & `formulaic-0.6.4/tests/parser/types/test_ast_node.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/types/test_factor.py` & `formulaic-0.6.4/tests/parser/types/test_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/types/test_formula_parser.py` & `formulaic-0.6.4/tests/parser/types/test_formula_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/types/test_operator.py` & `formulaic-0.6.4/tests/parser/types/test_operator.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/types/test_operator_resolver.py` & `formulaic-0.6.4/tests/parser/types/test_operator_resolver.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/types/test_structured.py` & `formulaic-0.6.4/tests/parser/types/test_structured.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/types/test_term.py` & `formulaic-0.6.4/tests/parser/types/test_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/parser/types/test_token.py` & `formulaic-0.6.4/tests/parser/types/test_token.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/transforms/test_basis_spline.py` & `formulaic-0.6.4/tests/transforms/test_basis_spline.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/transforms/test_contrasts.py` & `formulaic-0.6.4/tests/transforms/test_contrasts.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                         "a": [1, 0, 0, 1, 0, 0],
                         "b": [0, 1, 0, 0, 1, 0],
                         "c": [0, 0, 1, 0, 0, 1],
                     }
                 ),
                 kind="categorical",
                 spans_intercept=True,
-                column_names=["a", "b", "c"],
+                column_names=("a", "b", "c"),
                 drop_field="a",
                 format="{name}[T.{field}]",
                 encoded=True,
             ),
         )
         assert state["categories"] == ["a", "b", "c"]
 
@@ -66,15 +66,15 @@
                             "a": [1, 0, 0, 1, 0, 0],
                             "b": [0, 1, 0, 0, 1, 0],
                             "c": [0, 0, 0, 0, 0, 0],
                         }
                     ),
                     kind="categorical",
                     spans_intercept=True,
-                    column_names=["a", "b", "c"],
+                    column_names=("a", "b", "c"),
                     drop_field="a",
                     format="{name}[T.{field}]",
                     encoded=True,
                 ),
             )
             assert state["categories"] == ["a", "b", "c"]
 
@@ -90,15 +90,15 @@
                     {
                         "b": [0, 1, 0, 0, 1, 0],
                         "c": [0, 0, 1, 0, 0, 1],
                     }
                 ),
                 kind="categorical",
                 spans_intercept=False,
-                column_names=["b", "c"],
+                column_names=("b", "c"),
                 drop_field=None,
                 format="{name}[T.{field}]",
                 encoded=True,
             ),
         )
         assert state["categories"] == ["a", "b", "c"]
 
@@ -115,15 +115,15 @@
                         "a": [1, 0, 0, 1, 0, 0],
                         "b": [0, 1, 0, 0, 1, 0],
                         "c": [0, 0, 1, 0, 0, 1],
                     }
                 ).values,
                 kind="categorical",
                 spans_intercept=True,
-                column_names=["a", "b", "c"],
+                column_names=("a", "b", "c"),
                 drop_field="a",
                 format="{name}[T.{field}]",
                 encoded=True,
             ),
         )
         assert state["categories"] == ["a", "b", "c"]
 
@@ -139,15 +139,15 @@
                     {
                         "b": [0, 1, 0, 0, 1, 0],
                         "c": [0, 0, 1, 0, 0, 1],
                     }
                 ).values,
                 kind="categorical",
                 spans_intercept=False,
-                column_names=["b", "c"],
+                column_names=("b", "c"),
                 drop_field=None,
                 format="{name}[T.{field}]",
                 encoded=True,
             ),
         )
         assert state["categories"] == ["a", "b", "c"]
 
@@ -162,15 +162,15 @@
                             "a": [1, 0, 0, 1, 0, 0],
                             "b": [0, 1, 0, 0, 1, 0],
                             "c": [0, 0, 0, 0, 0, 0],
                         }
                     ).values,
                     kind="categorical",
                     spans_intercept=True,
-                    column_names=["a", "b", "c"],
+                    column_names=("a", "b", "c"),
                     drop_field="a",
                     format="{name}[T.{field}]",
                     encoded=True,
                 ),
             )
             assert state["categories"] == ["a", "b", "c"]
 
@@ -194,15 +194,15 @@
                         "a": [1, 0, 0, 1, 0, 0],
                         "b": [0, 1, 0, 0, 1, 0],
                         "c": [0, 0, 1, 0, 0, 1],
                     }
                 ),
                 kind="categorical",
                 spans_intercept=True,
-                column_names=["a", "b", "c"],
+                column_names=("a", "b", "c"),
                 drop_field="c",
                 format="{name}[T.{field}]",
                 encoded=True,
             ),
         )
         assert state["categories"] == ["a", "b", "c"]
 
@@ -220,15 +220,15 @@
                         "a": [1, 0, 0, 1, 0, 0],
                         "b": [0, 1, 0, 0, 1, 0],
                         "c": [0, 0, 1, 0, 0, 1],
                     }
                 ),
                 kind="categorical",
                 spans_intercept=True,
-                column_names=["a", "b", "c"],
+                column_names=("a", "b", "c"),
                 drop_field="a",
                 format="{name}[T.{field}]",
                 encoded=True,
             ),
         )
         assert state["categories"] == ["a", "b", "c"]
 
@@ -244,15 +244,15 @@
                 pandas.DataFrame(
                     {
                         "ordinal": [1, 2, 3, 1, 2, 3],
                     }
                 ),
                 kind="categorical",
                 spans_intercept=False,
-                column_names=["ordinal"],
+                column_names=("ordinal",),
                 drop_field=None,
                 format="{name}[{field}]",
                 encoded=True,
             ),
         )
         assert state["categories"] == ["a", "b", "c"]
 
@@ -356,42 +356,42 @@
         ):
             contr.treatment("invalid").apply(category_dummies, ["a", "b", "c"])
 
     def test_sparse(self, category_dummies_sparse):
         contrasts = contr.treatment()
 
         encoded = contrasts.apply(*category_dummies_sparse)
-        assert encoded.__formulaic_metadata__.column_names == ["b", "c"]
+        assert encoded.__formulaic_metadata__.column_names == ("b", "c")
         assert encoded.__formulaic_metadata__.drop_field is None
         assert numpy.all(
             encoded.toarray()
             == numpy.array(
                 [
                     [0, 1, 0, 0, 1, 0],  # b
                     [0, 0, 1, 0, 0, 1],  # c
                 ]
             ).T
         )
 
         encoded_spanning = contrasts.apply(*category_dummies_sparse, reduced_rank=False)
-        assert encoded_spanning.__formulaic_metadata__.column_names == ["a", "b", "c"]
+        assert encoded_spanning.__formulaic_metadata__.column_names == ("a", "b", "c")
         assert encoded_spanning.__formulaic_metadata__.drop_field == "a"
         assert numpy.all(
             encoded_spanning.toarray()
             == numpy.array(
                 [
                     [1, 0, 0, 1, 0, 0],  # a
                     [0, 1, 0, 0, 1, 0],  # b
                     [0, 0, 1, 0, 0, 1],  # c
                 ]
             ).T
         )
 
         encoded_base = contr.treatment("b").apply(*category_dummies_sparse)
-        assert encoded_base.__formulaic_metadata__.column_names == ["a", "c"]
+        assert encoded_base.__formulaic_metadata__.column_names == ("a", "c")
         assert encoded_base.__formulaic_metadata__.drop_field is None
         assert numpy.all(
             encoded_base.toarray()
             == numpy.array(
                 [
                     [1, 0, 0, 1, 0, 0],  # a
                     [0, 0, 1, 0, 0, 1],  # c
```

### Comparing `formulaic-0.6.3/tests/transforms/test_patsy_compat.py` & `formulaic-0.6.4/tests/transforms/test_patsy_compat.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/transforms/test_poly.py` & `formulaic-0.6.4/tests/transforms/test_poly.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/transforms/test_scale.py` & `formulaic-0.6.4/tests/transforms/test_scale.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/utils/test_calculus.py` & `formulaic-0.6.4/tests/utils/test_calculus.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/utils/test_cast.py` & `formulaic-0.6.4/tests/utils/test_cast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/utils/test_constraints.py` & `formulaic-0.6.4/tests/utils/test_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,21 @@
         with pytest.raises(
             ValueError,
             match=re.escape(
                 "Number of column names does not match the number of columns in the linear constraint matrix."
             ),
         ):
             LinearConstraints([[1, 2, 3]], [0], variable_names=["a"])
+        with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "`variable_names` must be provided when parsing constraints from a formula."
+            ),
+        ):
+            LinearConstraints.from_spec("a + b")
 
     def test_n_constraints(self):
         assert (
             LinearConstraints.from_spec(
                 "a = 0", variable_names=["a", "b", "c"]
             ).n_constraints
             == 1
```

### Comparing `formulaic-0.6.3/tests/utils/test_layered_mapping.py` & `formulaic-0.6.4/tests/utils/test_layered_mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,7 +60,14 @@
     ) == ["context", "data", "toplevel"]
 
     with pytest.raises(
         AttributeError,
         match=re.escape("'missing' does not correspond to a named layer."),
     ):
         layers.missing
+
+    full_layers = LayeredMapping(data_layer, context_layer, name="toplevel")
+    full_layers["local"] = True
+    assert full_layers.get_with_layer_name("local") == (True, "toplevel")
+    assert full_layers.get_with_layer_name("data") == (1, "toplevel:data")
+    assert full_layers.get_with_layer_name("missing") == (None, None)
+    assert full_layers.get_layer_name_for_key("data") == "toplevel:data"
```

### Comparing `formulaic-0.6.3/tests/utils/test_sparse.py` & `formulaic-0.6.4/tests/utils/test_sparse.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/tests/utils/test_stateful_transforms.py` & `formulaic-0.6.4/tests/utils/test_stateful_transforms.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/.gitignore` & `formulaic-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/LICENSE` & `formulaic-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/README.md` & `formulaic-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.3/pyproject.toml` & `formulaic-0.6.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -103,24 +103,27 @@
 ]
 
 [tool.hatch.envs.lint]
 dependencies = [
     "black==22.6",
     "flake8==5.0.4",
     "flake8-pyproject",
-    "pylint==2.14.5",
+    "mypy==1.4.1",
+    "mypy-extensions==1.0.0",
+    "pylint==2.17.4",
     "pytest-cov==3.0.0",
     "pytest==6.2.5",
 ]
 
 [tool.hatch.envs.lint.scripts]
 check = [
     "black --check formulaic tests",
     "flake8 formulaic",
     "pylint formulaic",
+    "mypy formulaic",
 ]
 format = "black formulaic tests"
 
 # Linting configuration
 
 [tool.flake8]
 ignore = [
@@ -149,8 +152,15 @@
     "too-many-arguments",
     "too-many-branches",
     "too-many-instance-attributes",
     "too-many-statements",
     "ungrouped-imports",
     "unnecessary-lambda-assignment",
     "unused-argument",
+    "use-dict-literal",
 ]
+
+[tool.mypy]
+allow_redefinition = true
+disallow_untyped_defs = true
+disallow_any_generics = false
+ignore_missing_imports = true
```

### Comparing `formulaic-0.6.3/PKG-INFO` & `formulaic-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formulaic
-Version: 0.6.3
+Version: 0.6.4
 Summary: An implementation of Wilkinson formulas.
 Project-URL: repository, https://github.com/matthewwardrop/formulaic
 Project-URL: documentation, https://matthewwardrop.github.io/formulaic
 Author-email: Matthew Wardrop <mpwardrop@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

