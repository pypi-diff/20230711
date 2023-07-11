# Comparing `tmp/cqlpy-0.2.6.tar.gz` & `tmp/cqlpy-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlpy-0.2.6.tar", max compression
+gzip compressed data, was "cqlpy-0.2.7.tar", max compression
```

## Comparing `cqlpy-0.2.6.tar` & `cqlpy-0.2.7.tar`

### file list

```diff
@@ -1,93 +1,95 @@
--rw-r--r--   0        0        0     1070 2023-06-05 20:37:29.512299 cqlpy-0.2.6/LICENSE
--rw-r--r--   0        0        0        8 2023-06-05 20:37:29.512299 cqlpy-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/__init__.py
--rw-r--r--   0        0        0     5339 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/context.py
--rw-r--r--   0        0        0     1801 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/cql_value_set_provider.py
--rw-r--r--   0        0        0   342427 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/fhir/r4/map.py
--rw-r--r--   0        0        0    16754 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/fhir/r4/model.py
--rw-r--r--   0        0        0      689 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/parameter_provider.py
--rw-r--r--   0        0        0     3016 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/resource_query.py
--rw-r--r--   0        0        0     1696 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/type_factory.py
--rw-r--r--   0        0        0      143 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/exceptions.py
--rw-r--r--   0        0        0      123 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/aggregate/count.py
--rw-r--r--   0        0        0      339 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/arithmetic/max_value.py
--rw-r--r--   0        0        0      320 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/arithmetic/min_value.py
--rw-r--r--   0        0        0      691 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/clinical/any_in_valueset.py
--rw-r--r--   0        0        0     1052 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/clinical/in_valueset.py
--rw-r--r--   0        0        0      120 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/equal.py
--rw-r--r--   0        0        0      511 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/equivalent.py
--rw-r--r--   0        0        0      735 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/greater.py
--rw-r--r--   0        0        0      763 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/greater_or_equal.py
--rw-r--r--   0        0        0      507 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/in_list.py
--rw-r--r--   0        0        0      726 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/less.py
--rw-r--r--   0        0        0      753 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/less_or_equal.py
--rw-r--r--   0        0        0      741 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/not_equal.py
--rw-r--r--   0        0        0      671 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/cql_in.py
--rw-r--r--   0        0        0     1165 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/add.py
--rw-r--r--   0        0        0      541 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/after.py
--rw-r--r--   0        0        0      558 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/before.py
--rw-r--r--   0        0        0      588 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/calculate_age_at.py
--rw-r--r--   0        0        0      157 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/date_time_precision.py
--rw-r--r--   0        0        0      898 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/difference_between.py
--rw-r--r--   0        0        0      890 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/duration_between.py
--rw-r--r--   0        0        0      378 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/same_or_before.py
--rw-r--r--   0        0        0     1181 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/subtract.py
--rw-r--r--   0        0        0     3800 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/collapse.py
--rw-r--r--   0        0        0      381 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/end.py
--rw-r--r--   0        0        0     1411 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/in_interval.py
--rw-r--r--   0        0        0     1546 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/included_in.py
--rw-r--r--   0        0        0      587 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/overlaps.py
--rw-r--r--   0        0        0      976 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/start.py
--rw-r--r--   0        0        0      348 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/distinct.py
--rw-r--r--   0        0        0      230 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/exists.py
--rw-r--r--   0        0        0      324 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/first.py
--rw-r--r--   0        0        0      291 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/flatten.py
--rw-r--r--   0        0        0     2195 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/intersect.py
--rw-r--r--   0        0        0      306 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/last.py
--rw-r--r--   0        0        0      404 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/singleton_from.py
--rw-r--r--   0        0        0      236 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/union.py
--rw-r--r--   0        0        0      409 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/nullological/coalesce.py
--rw-r--r--   0        0        0      212 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/nullological/is_false.py
--rw-r--r--   0        0        0      358 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/nullological/is_null.py
--rw-r--r--   0        0        0      193 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/nullological/is_true.py
--rw-r--r--   0        0        0      254 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/sort/sort_by_column.py
--rw-r--r--   0        0        0      134 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/sort/sort_by_direction.py
--rw-r--r--   0        0        0      173 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/sort/sort_by_expression.py
--rw-r--r--   0        0        0       51 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/sort/tuple_sort.py
--rw-r--r--   0        0        0      166 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/string/ends_with.py
--rw-r--r--   0        0        0      170 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/string/split.py
--rw-r--r--   0        0        0      149 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/to_list.py
--rw-r--r--   0        0        0      162 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/type/to_concept.py
--rw-r--r--   0        0        0      280 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/type/to_datetime.py
--rw-r--r--   0        0        0      509 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/parameter.py
--rw-r--r--   0        0        0     9733 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/scripts/fhir_map_generator.py
--rw-r--r--   0        0        0        0 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/__init__.py
--rw-r--r--   0        0        0     2901 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/any.py
--rw-r--r--   0        0        0      988 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/boolean.py
--rw-r--r--   0        0        0     1700 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/code.py
--rw-r--r--   0        0        0      851 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/code_system.py
--rw-r--r--   0        0        0     2459 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/concept.py
--rw-r--r--   0        0        0     1001 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/date.py
--rw-r--r--   0        0        0     2986 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/datetime.py
--rw-r--r--   0        0        0     1128 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/decimal.py
--rw-r--r--   0        0        0      756 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/integer.py
--rw-r--r--   0        0        0     3674 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/interval.py
--rw-r--r--   0        0        0     1605 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/list.py
--rw-r--r--   0        0        0       81 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/long.py
--rw-r--r--   0        0        0      416 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/null.py
--rw-r--r--   0        0        0      887 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/quantity.py
--rw-r--r--   0        0        0     1053 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/string.py
--rw-r--r--   0        0        0     2003 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/value_set.py
--rw-r--r--   0        0        0      735 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/value_set_scope.py
--rw-r--r--   0        0        0      372 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/valueset_provider.py
--rw-r--r--   0        0        0      451 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/context.py
--rw-r--r--   0        0        0     4227 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/operators.py
--rw-r--r--   0        0        0        0 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/providers/__init__.py
--rw-r--r--   0        0        0      216 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/providers/logger.py
--rw-r--r--   0        0        0       15 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/providers/requirements.txt
--rw-r--r--   0        0        0     4949 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/providers/rosetta_valueset_provider.py
--rw-r--r--   0        0        0        0 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/py.typed
--rw-r--r--   0        0        0     1089 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/types.py
--rw-r--r--   0        0        0      670 2023-06-05 20:37:53.996531 cqlpy-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 cqlpy-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-11 12:26:06.242231 cqlpy-0.2.7/LICENSE
+-rw-r--r--   0        0        0        8 2023-07-11 12:26:06.242231 cqlpy-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/_internal/__init__.py
+-rw-r--r--   0        0        0     5335 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/_internal/context/context.py
+-rw-r--r--   0        0        0     2077 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/_internal/context/cql_valueset_provider.py
+-rw-r--r--   0        0        0      829 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/_internal/context/fhir/fhir_cql_type.py
+-rw-r--r--   0        0        0  1023948 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/fhir/r4/map.py
+-rw-r--r--   0        0        0    18950 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/fhir/r4/model.py
+-rw-r--r--   0        0        0      689 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/parameter_provider.py
+-rw-r--r--   0        0        0     3013 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/resource_query.py
+-rw-r--r--   0        0        0     2532 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/type_factory.py
+-rw-r--r--   0        0        0      143 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/exceptions.py
+-rw-r--r--   0        0        0      123 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/aggregate/count.py
+-rw-r--r--   0        0        0      339 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/arithmetic/max_value.py
+-rw-r--r--   0        0        0      320 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/arithmetic/min_value.py
+-rw-r--r--   0        0        0      688 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/clinical/any_in_valueset.py
+-rw-r--r--   0        0        0     1041 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/clinical/in_valueset.py
+-rw-r--r--   0        0        0      120 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/equal.py
+-rw-r--r--   0        0        0      511 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/equivalent.py
+-rw-r--r--   0        0        0      735 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/greater.py
+-rw-r--r--   0        0        0      763 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/greater_or_equal.py
+-rw-r--r--   0        0        0      507 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/in_list.py
+-rw-r--r--   0        0        0      726 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/less.py
+-rw-r--r--   0        0        0      753 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/less_or_equal.py
+-rw-r--r--   0        0        0      741 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/not_equal.py
+-rw-r--r--   0        0        0      671 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/cql_in.py
+-rw-r--r--   0        0        0     1326 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/add.py
+-rw-r--r--   0        0        0      541 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/after.py
+-rw-r--r--   0        0        0      558 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/before.py
+-rw-r--r--   0        0        0      588 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/calculate_age_at.py
+-rw-r--r--   0        0        0      170 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/date_time_precision.py
+-rw-r--r--   0        0        0      898 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/difference_between.py
+-rw-r--r--   0        0        0      890 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/duration_between.py
+-rw-r--r--   0        0        0      378 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/same_or_before.py
+-rw-r--r--   0        0        0     1342 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/subtract.py
+-rw-r--r--   0        0        0     3800 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/collapse.py
+-rw-r--r--   0        0        0      381 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/end.py
+-rw-r--r--   0        0        0     1411 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/in_interval.py
+-rw-r--r--   0        0        0     1546 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/included_in.py
+-rw-r--r--   0        0        0      587 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/overlaps.py
+-rw-r--r--   0        0        0      976 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/start.py
+-rw-r--r--   0        0        0      348 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/distinct.py
+-rw-r--r--   0        0        0      230 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/exists.py
+-rw-r--r--   0        0        0      324 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/first.py
+-rw-r--r--   0        0        0      291 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/flatten.py
+-rw-r--r--   0        0        0     2195 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/intersect.py
+-rw-r--r--   0        0        0      306 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/list/last.py
+-rw-r--r--   0        0        0      404 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/list/singleton_from.py
+-rw-r--r--   0        0        0      236 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/list/union.py
+-rw-r--r--   0        0        0      409 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/nullological/coalesce.py
+-rw-r--r--   0        0        0      212 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/nullological/is_false.py
+-rw-r--r--   0        0        0      358 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/nullological/is_null.py
+-rw-r--r--   0        0        0      193 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/nullological/is_true.py
+-rw-r--r--   0        0        0      254 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/sort/sort_by_column.py
+-rw-r--r--   0        0        0      134 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/sort/sort_by_direction.py
+-rw-r--r--   0        0        0      173 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/sort/sort_by_expression.py
+-rw-r--r--   0        0        0       51 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/sort/tuple_sort.py
+-rw-r--r--   0        0        0      166 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/string/ends_with.py
+-rw-r--r--   0        0        0      170 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/string/split.py
+-rw-r--r--   0        0        0      149 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/to_list.py
+-rw-r--r--   0        0        0      162 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/type/to_concept.py
+-rw-r--r--   0        0        0      280 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/type/to_datetime.py
+-rw-r--r--   0        0        0      509 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/parameter.py
+-rw-r--r--   0        0        0        0 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/providers/__init__.py
+-rw-r--r--   0        0        0     4258 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/providers/local_valueset_provider.py
+-rw-r--r--   0        0        0      216 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/providers/logger.py
+-rw-r--r--   0        0        0     4946 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/providers/rosetta_valueset_provider.py
+-rw-r--r--   0        0        0    10714 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/scripts/fhir_map_generator.py
+-rw-r--r--   0        0        0        0 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/__init__.py
+-rw-r--r--   0        0        0     2901 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/any.py
+-rw-r--r--   0        0        0      988 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/boolean.py
+-rw-r--r--   0        0        0     1700 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/code.py
+-rw-r--r--   0        0        0      851 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/code_system.py
+-rw-r--r--   0        0        0     2457 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/concept.py
+-rw-r--r--   0        0        0     1001 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/date.py
+-rw-r--r--   0        0        0     2986 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/datetime.py
+-rw-r--r--   0        0        0     1128 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/decimal.py
+-rw-r--r--   0        0        0      756 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/integer.py
+-rw-r--r--   0        0        0     3674 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/interval.py
+-rw-r--r--   0        0        0     1605 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/list.py
+-rw-r--r--   0        0        0       81 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/long.py
+-rw-r--r--   0        0        0      416 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/null.py
+-rw-r--r--   0        0        0      887 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/quantity.py
+-rw-r--r--   0        0        0     1053 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/string.py
+-rw-r--r--   0        0        0     1997 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/valueset.py
+-rw-r--r--   0        0        0      731 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/valueset_scope.py
+-rw-r--r--   0        0        0      372 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/valueset_provider.py
+-rw-r--r--   0        0        0      450 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/context.py
+-rw-r--r--   0        0        0     4227 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/operators.py
+-rw-r--r--   0        0        0      319 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/providers.py
+-rw-r--r--   0        0        0        0 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/py.typed
+-rw-r--r--   0        0        0     1088 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/types.py
+-rw-r--r--   0        0        0      670 2023-07-11 12:26:30.598128 cqlpy-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 cqlpy-0.2.7/PKG-INFO
```

### Comparing `cqlpy-0.2.6/LICENSE` & `cqlpy-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/context/context.py` & `cqlpy-0.2.7/cqlpy/_internal/context/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from typing import Optional, Union
-from cqlpy._internal.context.cql_value_set_provider import CqlValueSetProvider
+from cqlpy._internal.context.cql_valueset_provider import CqlValuesetProvider
 
 from cqlpy._internal.context.fhir.r4.model import FhirR4DataModel
 from cqlpy._internal.context.parameter_provider import ParameterProvider
 from cqlpy._internal.parameter import Parameter
 from cqlpy._internal.types.code import Code
-from cqlpy._internal.types.value_set import ValueSet
-from cqlpy._internal.types.value_set_scope import ValueSetScope
-from cqlpy._internal.valueset_provider import ValueSetProvider
+from cqlpy._internal.types.valueset import Valueset
+from cqlpy._internal.types.valueset_scope import ValuesetScope
+from cqlpy._internal.valueset_provider import ValuesetProvider
 
 
 class Context:
     """
     A context is a required parameter on every CQL expression that is converted to python as a function.
     The expected signature of every function that implements a CQL Expression is:
 
@@ -21,39 +21,39 @@
     The Context provides access to the data model, parameter values, and value set codes as needed by the internal elements
     of a python function that implements a CQL expression. The Context provides access to these concepts via a retrieve operation
     that is implemented with syntax such as:
 
         context["Encounter"]    # if a string is requested (assumed to be a FHIR resource type), context returns a
                                 # list of Resources from the model, in this case all Encounter resources.
 
-        context["Encounter", ValueSet, "type"]
+        context["Encounter", Valueset, "type"]
                                 # if a tuple is requested (assumed to be a FHIR resource type), context returns a
                                 # list of Resources from the model, in this case Encounter resources, filtered by
                                 # checking the specified property to see if it has a coded value in the specified value set.
 
         context[Parameter]      # if a Parameter is requested, context returns the type specified by the Parameter
                                 # with value determined by the parameter_provider from external parameters or the default value.
 
-        context[ValueSet]       # if a ValueSet is requested, context returns a ValueSet that includes with Codes property populated
-                                # from the value_set_provider.
+        context[Valueset]       # if a Valueset is requested, context returns a Valueset that includes with Codes property populated
+                                # from the valueset_provider.
 
     The Context iterates through the bundle (as a json object) to retrieve a list of Resources.
 
     Properties of Resources can be obtained using syntax such as:
 
         Encounter["period"]     # The property of the resource is properly typed when requested (in this case, Interval)
                                 # by parsing the related bundle json element.
 
     Context Resource retrieve operations and Resource property retrieve operations are cached so that iterating through the bundle
     and parsing json is only performed once (at time of the first request).
     """
 
     def __init__(
         self,
-        valueset_provider: ValueSetProvider,
+        valueset_provider: ValuesetProvider,
         bundle: Optional[Union[str, dict]] = None,
         bundle_file_name: Optional[str] = None,
         parameters: Optional[dict] = None,
     ):
         parsed_bundle = None
         if bundle_file_name:
             with open(bundle_file_name, encoding="utf-8") as f:
@@ -66,35 +66,35 @@
             parsed_bundle = bundle
 
         if parsed_bundle is None:
             raise ValueError("bundle or bundle_file_name must be specified")
 
         self.parameter_provider = ParameterProvider(parameters)
         self.model = FhirR4DataModel(parsed_bundle, self.parameter_provider)
-        self.cql_valueset_provider = CqlValueSetProvider(
+        self.cql_valueset_provider = CqlValuesetProvider(
             valueset_provider=valueset_provider
         )
 
     def __getitem__(
         self,
         requested_concept: Union[
             Parameter,
-            ValueSet,
-            ValueSetScope,
+            Valueset,
+            ValuesetScope,
             str,
-            tuple[str, Union[ValueSet, list[Code], Code], str],
+            tuple[str, Union[Valueset, list[Code], Code], str],
         ],
     ):
         if isinstance(requested_concept, Parameter):
             # In this case, the return type will be the Cql Type specified by the parameter,
             # i.e. Interval<DateTime>, CqlString, etc.
             return self.parameter_provider[requested_concept]
 
-        if isinstance(requested_concept, ValueSet) or isinstance(
-            requested_concept, ValueSetScope
+        if isinstance(requested_concept, Valueset) or isinstance(
+            requested_concept, ValuesetScope
         ):
             # In this case, the return type will be ValueSet (which includes all codes specified by the value set).
             return self.cql_valueset_provider[requested_concept]
 
         if isinstance(requested_concept, Code):
             # In this case, there is nothing to lookup... the Code is fully populated.
             return requested_concept
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/context/cql_value_set_provider.py` & `cqlpy-0.2.7/cqlpy/_internal/context/cql_valueset_provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,63 @@
 from typing import Union
-from cqlpy._internal.exceptions import ValueSetProviderError
-from cqlpy._internal.types.value_set import ValueSet
-from cqlpy._internal.types.value_set_scope import ValueSetScope
-from cqlpy._internal.valueset_provider import ValueSetProvider, ValueSetScopeProvider
+from cqlpy._internal.exceptions import ValuesetProviderError
+from cqlpy._internal.types.valueset import Valueset
+from cqlpy._internal.types.valueset_scope import ValuesetScope
+from cqlpy._internal.valueset_provider import ValuesetProvider, ValuesetScopeProvider
+
+_COMMON_URL_PREFIXES = [
+    "http://cts.nlm.nih.gov/fhir/ValueSet/",
+    "http://hl7.org/fhir/ValueSet/",
+]
+
+
+def _clean_name(name: str) -> str:
+    for prefix in _COMMON_URL_PREFIXES:
+        if name.startswith(prefix):
+            return name[len(prefix) :]
+    return name
 
 
-class CqlValueSetProvider:
-    def __init__(self, valueset_provider: ValueSetProvider) -> None:
+class CqlValuesetProvider:
+    def __init__(self, valueset_provider: ValuesetProvider) -> None:
         self._valueset_provider = valueset_provider
 
-    def __get_valueset(self, item: ValueSet) -> ValueSet:
+    def __get_valueset(self, item: Valueset) -> Valueset:
         if item.id is None:
             raise ValueError("value set id must be specified")
 
-        name = item.id.replace("http://cts.nlm.nih.gov/fhir/ValueSet/", "")
+        name = _clean_name(item.id)
         result = self._valueset_provider.get_valueset(name=name, scope=None)
 
         if result:
-            return ValueSet.parse_fhir_json(result)
+            return Valueset.parse_fhir_json(result)
 
         print(f"value set 'scopeless:{item.name}' not found")
 
         return item
 
-    def __get_valueset_scope(self, item: ValueSetScope) -> list[ValueSet]:
-        if not isinstance(self._valueset_provider, ValueSetScopeProvider):
-            raise ValueSetProviderError(
+    def __get_valueset_scope(self, item: ValuesetScope) -> list[Valueset]:
+        if not isinstance(self._valueset_provider, ValuesetScopeProvider):
+            raise ValuesetProviderError(
                 "The value set provider does not support scope-based value set retrieval"
             )
 
         if item.id is None:
             raise ValueError("value set scope id must be specified")
 
         result = self._valueset_provider.get_valuesets_in_scope(scope=item.id)
 
         if result:
-            return [ValueSet.parse_fhir_json(value_set) for value_set in result]
+            return [
+                Valueset.parse_fhir_json(valueset["resource"]) for valueset in result
+            ]
 
         print(f"value set scope '{item.id}' not found")
 
         return []
 
     def __getitem__(
-        self, item: Union[ValueSet, ValueSetScope]
-    ) -> Union[ValueSet, list[ValueSet]]:
-        if isinstance(item, ValueSetScope):
+        self, item: Union[Valueset, ValuesetScope]
+    ) -> Union[Valueset, list[Valueset]]:
+        if isinstance(item, ValuesetScope):
             return self.__get_valueset_scope(item)
         return self.__get_valueset(item)
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/context/fhir/r4/model.py` & `cqlpy-0.2.7/cqlpy/_internal/context/fhir/r4/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,89 +10,156 @@
 from cqlpy._internal.operators.list.intersect import intersect
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.parameter import Parameter
 from cqlpy._internal.types.any import CqlAny
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.concept import Concept
 from cqlpy._internal.types.datetime import DateTime
+from cqlpy._internal.types.date import Date
 from cqlpy._internal.types.interval import Interval
 from cqlpy._internal.types.null import Null
-from cqlpy._internal.types.value_set import ValueSet
+from cqlpy._internal.types.valueset import Valueset
 from cqlpy._internal.types.string import String
 from cqlpy._internal.context.fhir.r4.map import FHIR_TO_CQL_MAP
+from cqlpy._internal.context.fhir.fhir_cql_type import (
+    FhirCqlType,
+    FhirChoice,
+    FhirList,
+    FhirInterval,
+)
+from cqlpy._internal.types.boolean import Boolean
+
+from cqlpy._internal.types.list import List
 
 
 class FhirBase:
     def __init__(self, fhir_json: dict, base_type: str):
         self._fhir_json = fhir_json
         self._base_type = base_type
 
     def __str__(self) -> str:
         return json.dumps(self._fhir_json)
 
-    def __getitem__(self, property_name: str):
-        if property_name in ["resourceType", "derivedFromResourceType"]:
+    def __handle_choice(
+        self, property_name: str, fhir_cql_type: FhirChoice
+    ) -> Optional[CqlAny]:
+        value: Optional[CqlAny] = None
+        if any(
+            choice.item_type == "DateTime"
+            for choice in fhir_cql_type.choices
+            if isinstance(choice, FhirInterval)
+        ):
+            if f"{property_name}DateTime" in self._fhir_json:
+                value = DateTime.parse_fhir_json(
+                    self._fhir_json[f"{property_name}DateTime"]
+                )
+                return Interval(value, True, value, True)
+
+        elif any(choice.name == "DateTime" for choice in fhir_cql_type.choices):
+            if f"{property_name}DateTime" in self._fhir_json:
+                value = DateTime.parse_fhir_json(
+                    self._fhir_json[f"{property_name}DateTime"]
+                )
+                return value
+
+        elif any(
+            choice.item_type == "Date"
+            for choice in fhir_cql_type.choices
+            if isinstance(choice, FhirInterval)
+        ):
+            if f"{property_name}Date" in self._fhir_json:
+                value = Date.parse_fhir_json(self._fhir_json[f"{property_name}Date"])
+                return Interval(value, True, value, True)
+
+        elif any(choice.name == "Date" for choice in fhir_cql_type.choices):
+            if f"{property_name}Date" in self._fhir_json:
+                value = Date.parse_fhir_json(self._fhir_json[f"{property_name}Date"])
+                return value
+
+        elif any(choice.name == "Boolean" for choice in fhir_cql_type.choices):
+            if f"{property_name}Boolean" in self._fhir_json:
+                value = Boolean.parse_fhir_json(
+                    self._fhir_json[f"{property_name}Boolean"]
+                )
+                return value
+
+        elif any(choice.name == "String" for choice in fhir_cql_type.choices):
+            if any(prop.startswith(property_name) for prop in self._fhir_json):
+                return String.parse_fhir_json(self._fhir_json[property_name])
+
+        return None
+
+    def __handle_list(
+        self, property_name: str, fhir_cql_type: FhirList
+    ) -> Optional[list]:
+        if fhir_cql_type.item_type.is_backbone_element:
             if property_name in self._fhir_json:
-                return self._fhir_json[property_name]
+                return [
+                    BackboneElement(item, fhir_cql_type.item_type.name)
+                    for item in self._fhir_json[property_name]
+                ]
             else:
-                return None
+                return []
 
-        elif (self._base_type in FHIR_TO_CQL_MAP) and (
-            property_name in FHIR_TO_CQL_MAP[self._base_type]
-        ):
-            cql_type_name = FHIR_TO_CQL_MAP[self._base_type][property_name]
+        if property_name in self._fhir_json:
+            _, subtype = TypeFactory.get_type_from_fhir_cql(fhir_cql_type)
+            return List.parse_fhir_json(self._fhir_json[property_name], subtype)
 
-            if cql_type_name == "Choice:Interval<DateTime>":
-                if f"{property_name}DateTime" in self._fhir_json:
-                    cql_type, _ = TypeFactory.get_type("DateTime")
-                    value = cql_type.parse_fhir_json(
-                        self._fhir_json[f"{property_name}DateTime"]
-                    )
-                    assert isinstance(value, DateTime)
-                    return Interval(value, True, value, True)
+        return None
 
-            elif cql_type_name == "Choice:String":
-                if any(prop.startswith(property_name) for prop in self._fhir_json):
-                    cql_type, _ = TypeFactory.get_type("String")
-                    value = cql_type.parse_fhir_json(self._fhir_json[property_name])
-                    assert isinstance(value, str)
-                    return String(value)
-
-            elif "List<BackboneElement:" in cql_type_name:
-                element_name = cql_type_name.split(":")[1].replace(">", "")
-
-                if property_name in self._fhir_json:
-                    return [
-                        BackboneElement(item, element_name)
-                        for item in self._fhir_json[property_name]
-                    ]
-                else:
-                    return []
+    def __handle_backbone_element(
+        self, property_name: str, fhir_cql_type: FhirCqlType
+    ) -> "BackboneElement":
+        element_name = fhir_cql_type.name
 
-            elif cql_type_name.startswith("List<"):
-                element_name = cql_type_name.split("<")[1].replace(">", "")
+        if property_name in self._fhir_json:
+            return BackboneElement(self._fhir_json[property_name], element_name)
 
-                if property_name in self._fhir_json:
-                    cql_type, subtype = TypeFactory.get_type(element_name)
-                    return [
-                        cql_type.parse_fhir_json(item, subtype)
-                        for item in self._fhir_json[property_name]
-                    ]
+        return BackboneElement({}, element_name)
 
-            elif cql_type_name.startswith("BackboneElement:"):
-                element_name = cql_type_name.split(":")[1]
+    def __handle_flat_property(
+        self, property_name: str, fhir_cql_type: FhirCqlType
+    ) -> CqlAny:
+        cql_type, subtype = TypeFactory.get_type_from_fhir_cql(fhir_cql_type)
+        return cql_type.parse_fhir_json(self._fhir_json[property_name], subtype)
 
-                if property_name in self._fhir_json:
-                    return BackboneElement(self._fhir_json[property_name], element_name)
-                else:
-                    return BackboneElement({}, element_name)
+    def __get_property(self, property_name: str):
+        fhir_cql_type = FHIR_TO_CQL_MAP[self._base_type][property_name]
+
+        if isinstance(fhir_cql_type, FhirChoice):
+            handled_choice = self.__handle_choice(property_name, fhir_cql_type)
+            if handled_choice is not None:
+                return handled_choice
+
+        elif isinstance(fhir_cql_type, FhirList):
+            handled_list = self.__handle_list(property_name, fhir_cql_type)
+            if handled_list is not None:
+                return handled_list
+
+        elif fhir_cql_type.is_backbone_element:
+            return self.__handle_backbone_element(property_name, fhir_cql_type)
+
+        elif property_name in self._fhir_json:
+            return self.__handle_flat_property(property_name, fhir_cql_type)
+
+        return None
+
+    def __getitem__(self, property_name: str):
+        if property_name in ["resourceType", "derivedFromResourceType"]:
+            if property_name in self._fhir_json:
+                return self._fhir_json[property_name]
+            else:
+                return None
 
-            elif property_name in self._fhir_json:
-                cql_type, subtype = TypeFactory.get_type(cql_type_name)
-                return cql_type.parse_fhir_json(self._fhir_json[property_name], subtype)
+        elif (self._base_type in FHIR_TO_CQL_MAP) and (
+            property_name in FHIR_TO_CQL_MAP[self._base_type]
+        ):
+            property = self.__get_property(property_name)
+            if property is not None:
+                return property
 
         return Null()
 
     @property
     def value(self) -> str:
         return json.dumps(self._fhir_json)
 
@@ -175,22 +242,22 @@
     },
 }
 
 
 def _get_filter_codes(filter_: Optional[ResourceQueryFilter]) -> list[Code]:
     if filter_ is None:
         return []
-    if isinstance(filter_, ValueSet):
+    if isinstance(filter_, Valueset):
         return filter_.codes
     if isinstance(filter_, Code):
         return [filter_]
     if isinstance(filter_, list):
         codes: list[Code] = []
         for item in filter_:
-            if isinstance(item, ValueSet):
+            if isinstance(item, Valueset):
                 codes.extend(item.codes)
             elif isinstance(item, Code):
                 codes.append(item)
             else:
                 raise ValueError(f"Unsupported filter item type: {type(item)}")
         return codes
 
@@ -351,15 +418,15 @@
 
             else:
                 yield self.__generate_resource_proxy(resource, resource_type)
 
     def __getitem__(
         self,
         resource_query: Union[
-            str, tuple[str, Union[ValueSet, list[Code], Code, list[ValueSet]], str]
+            str, tuple[str, Union[Valueset, list[Code], Code, list[Valueset]], str]
         ],
     ) -> Sequence[FhirBase]:
         duration_start_time = datetime.now()
 
         query = ResourceQuery.from_query(resource_query)
 
         if query in self.retrieve_cache:
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/context/parameter_provider.py` & `cqlpy-0.2.7/cqlpy/_internal/context/parameter_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/context/resource_query.py` & `cqlpy-0.2.7/cqlpy/_internal/context/resource_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass, field
 from functools import cached_property
 from typing import Optional, Union
 
 from cqlpy._internal.types.code import Code
-from cqlpy._internal.types.value_set import ValueSet
+from cqlpy._internal.types.valueset import Valueset
 
-ResourceQueryFilter = Union[ValueSet, list[Code], Code, list[ValueSet]]
+ResourceQueryFilter = Union[Valueset, list[Code], Code, list[Valueset]]
 
 
 @dataclass(frozen=True, eq=True)
 class ResourceQuery:
     resource_type: str = field()
     property_filter: Optional[ResourceQueryFilter] = field(default=None)
     property_name: Optional[str] = field(default=None)
@@ -38,43 +38,43 @@
             property_name=property_name,
         )
 
     @cached_property
     def description(self) -> str:
         if self.property_filter is None:
             return f"All {self.resource_type} resources"
-        if isinstance(self.property_filter, ValueSet):
+        if isinstance(self.property_filter, Valueset):
             return (
-                f"{self.resource_type} filter on ValueSet: {self.property_filter.name}"
+                f"{self.resource_type} filter on Valueset: {self.property_filter.name}"
             )
         if isinstance(self.property_filter, Code):
             return f"{self.resource_type} filter on Code: {self.property_filter.code} {str(self.property_filter.system)}"
         return f"{self.resource_type} filter on list"
 
     def __hash__(self):
         if self.property_filter is None:
             return hash(self.resource_type)
         if isinstance(self.property_filter, Code):
             return hash((self.resource_type, self.property_filter, self.property_name))
 
-        if isinstance(self.property_filter, ValueSet):
+        if isinstance(self.property_filter, Valueset):
             property_filter_hash = hash(tuple(self.property_filter.codes))
         elif isinstance(self.property_filter, list) and isinstance(
             self.property_filter[0], Code
         ):
             property_filter_hash = hash(tuple(self.property_filter))
         elif isinstance(self.property_filter, list) and isinstance(
-            self.property_filter[0], ValueSet
+            self.property_filter[0], Valueset
         ):
             property_filter_hash = hash(
                 tuple(
                     [
                         code
-                        for value_set in self.property_filter
-                        for code in value_set.codes
+                        for valueset in self.property_filter
+                        for code in valueset.codes
                     ]
                 )
             )
         else:
             raise NotImplementedError(
                 f"Unsupported property_filter type: {type(self.property_filter)}"
             )
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/clinical/any_in_valueset.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/clinical/any_in_valueset.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from typing import Union
 from cqlpy._internal.operators.clinical.in_valueset import in_valueset
 from cqlpy._internal.operators.nullological.is_null import is_null
 
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.concept import Concept
 from cqlpy._internal.types.null import Some
-from cqlpy._internal.types.value_set import ValueSet
+from cqlpy._internal.types.valueset import Valueset
 
 
 def any_in_valueset(
-    argument: list[Some[Union[str, Code, Concept]]], value_set: ValueSet
+    argument: list[Some[Union[str, Code, Concept]]], valueset: Valueset
 ) -> bool:
     if not is_null(argument):
         for item in argument:
-            if in_valueset(item, value_set):
+            if in_valueset(item, valueset):
                 return True
 
     return False
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/clinical/in_valueset.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/clinical/in_valueset.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 from typing import Union
 from cqlpy._internal.operators.nullological.is_null import is_null
 
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.concept import Concept
 from cqlpy._internal.types.null import Some
-from cqlpy._internal.types.value_set import ValueSet
+from cqlpy._internal.types.valueset import Valueset
 
 
-def in_valueset(argument: Some[Union[str, Code, Concept]], value_set: ValueSet) -> bool:
+def in_valueset(argument: Some[Union[str, Code, Concept]], valueset: Valueset) -> bool:
     if is_null(argument):
         return False
 
     elif isinstance(argument, str):
-        for value_set_code in value_set.codes:
-            if argument == value_set_code:
+        for valueset_code in valueset.codes:
+            if argument == valueset_code:
                 return True
 
     elif isinstance(argument, Code):
-        for value_set_code in value_set.codes:
-            if argument.code == value_set_code.code:
+        for valueset_code in valueset.codes:
+            if argument.code == valueset_code.code:
                 return True
 
     elif isinstance(argument, Concept):
         for code in argument.codes:
-            for value_set_code in value_set.codes:
-                if code.code == value_set_code.code:
+            for valueset_code in valueset.codes:
+                if code.code == valueset_code.code:
                     return True
 
     return False
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/greater.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/comparison/greater.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/greater_or_equal.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/comparison/greater_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/less.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/comparison/less.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/less_or_equal.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/comparison/less_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/not_equal.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/comparison/not_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/cql_in.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/cql_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/add.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/add.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 def add(left: DateTime, right: Quantity) -> Some[DateTime]:
     if is_null(left) or is_null(right):
         return Null()
     assert right.value is not None
 
     if (right.unit == "days") or (right.unit == DateTimePrecision.Day):
         return DateTime().parse_datetime(left.value + timedelta(days=right.value))
+    if (right.unit == "weeks") or (right.unit == DateTimePrecision.Week):
+        return DateTime().parse_datetime(left.value + timedelta(days=7 * right.value))
     if (right.unit == "months") or (right.unit == DateTimePrecision.Month):
         months = int(right.value)
         return DateTime().parse_datetime(left.value + relativedelta(months=months))
     if (right.unit == "years") or (right.unit == DateTimePrecision.Year):
         years = int(right.value)
         return DateTime().parse_datetime(left.value + relativedelta(years=years))
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/after.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/after.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/before.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/before.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/calculate_age_at.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/calculate_age_at.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/difference_between.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/difference_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/duration_between.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/duration_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/subtract.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/subtract.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 def subtract(left: DateTime, right: Quantity) -> Some[DateTime]:
     if is_null(left) or is_null(right):
         return Null()
     assert right.value is not None
 
     if (right.unit == "days") or (right.unit == DateTimePrecision.Day):
         return DateTime().parse_datetime(left.value - timedelta(days=right.value))
+    if (right.unit == "weeks") or (right.unit == DateTimePrecision.Week):
+        return DateTime().parse_datetime(left.value - timedelta(days=7 * right.value))
     if (right.unit == "months") or (right.unit == DateTimePrecision.Month):
         months = int(right.value)
         return DateTime().parse_datetime(left.value - relativedelta(months=months))
     if (right.unit == "years") or (right.unit == DateTimePrecision.Year):
         years = int(right.value)
         return DateTime().parse_datetime(left.value - relativedelta(years=years))
     return Null()
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/interval/collapse.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/interval/collapse.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/interval/in_interval.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/interval/in_interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/interval/included_in.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/interval/included_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/interval/overlaps.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/interval/overlaps.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/interval/start.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/interval/start.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/operators/list/intersect.py` & `cqlpy-0.2.7/cqlpy/_internal/operators/list/intersect.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/scripts/fhir_map_generator.py` & `cqlpy-0.2.7/cqlpy/_internal/scripts/fhir_map_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # %%
 from argparse import ArgumentParser
 from dataclasses import dataclass, field
 from pathlib import Path
 from itertools import groupby
 from typing import Optional
+from cqlpy._internal.context.fhir.fhir_cql_type import (
+    FhirCqlType,
+    FhirChoice,
+    FhirList,
+    FhirInterval,
+)
 import json
 
 
 # %%
 def identify_shared_prefix(texts: list[str]) -> str:
     shared_text = None
     for text in texts:
@@ -146,14 +152,43 @@
         if self.type == "choice":
             declared_type = (
                 f"choice<{'|'.join([str(choice) for choice in self.choices])}>"
             )
         return f"PropertyDeclaration({self.name}, {declared_type})"
 
 
+_CHOICE_SUFFIXES = {
+    "DateTime": "dateTime",
+    "Date": "date",
+}
+
+
+def infer_type_from_choice(
+    choice: str, declaration: PropertyDeclaration
+) -> PropertyDeclaration:
+    if declaration.type == "choice":
+        raise ValueError("Cannot infer type from choice with choice type")
+
+    choice_suffix = declaration.name[len(choice) :]
+    if choice_suffix == "":
+        return declaration
+
+    inferred_type = _CHOICE_SUFFIXES.get(choice_suffix, None)
+
+    if inferred_type is None:
+        return declaration
+
+    return PropertyDeclaration(
+        name=choice_suffix,
+        type=inferred_type,
+        ref=declaration.ref,
+        item_type=declaration.item_type,
+    )
+
+
 def build_resource_declaration(resource: dict) -> dict[str, PropertyDeclaration]:
     choices = extract_choices(resource)
     property_declarations = {
         prop: PropertyDeclaration.from_schema(prop, attributes)
         for prop, attributes in resource["properties"].items()
         if any(
             type_property in attributes for type_property in ["$ref", "type", "enum"]
@@ -165,88 +200,87 @@
         choice = next(
             (choice for choice, values in choices.items() if name in values), None
         )
         if choice is None:
             choice_declarations[name] = declaration
             continue
 
+        choice_inferred_declaration = infer_type_from_choice(choice, declaration)
         if choice not in choice_declarations:
             choice_declarations[choice] = PropertyDeclaration(
                 name=choice,
                 type="choice",
-                choices=[declaration],
+                choices=[choice_inferred_declaration],
             )
             continue
 
-        choice_declarations[choice].choices.append(declaration)
+        choice_declarations[choice].choices.append(choice_inferred_declaration)
 
     return choice_declarations
 
 
 _DIRECTLY_MAPPED_TYPES = {
-    "boolean": "Boolean",
-    "integer": "Integer",
-    "decimal": "Decimal",
-    "date": "Date",
-    "dateTime": "DateTime",
-    "code": "Code",
-    "Coding": "Code",
-    "CodeableConcept": "Concept",
-    "Quantity": "Decimal",
-    "Period": "Interval<DateTime>",
-    "Range": "Interval<Decimal>",
+    "boolean": FhirCqlType("Boolean"),
+    "integer": FhirCqlType("Integer"),
+    "decimal": FhirCqlType("Decimal"),
+    "date": FhirCqlType("Date"),
+    "dateTime": FhirCqlType("DateTime"),
+    "code": FhirCqlType("Code"),
+    "Coding": FhirCqlType("Code"),
+    "CodeableConcept": FhirCqlType("Concept"),
+    "Quantity": FhirCqlType("Decimal"),
+    "Period": FhirInterval(item_type=FhirCqlType("DateTime")),
+    "Range": FhirInterval(item_type=FhirCqlType("Decimal")),
 }
 
 
 class DeclarationMapper:
     def __init__(
         self,
         backbone_elements: list[str],
     ) -> None:
         self.__backbone_elements = backbone_elements
 
-    def map_fhir_to_cql_type(self, fhir_type: str) -> str:
+    def map_fhir_to_cql_type(self, fhir_type: str) -> FhirCqlType:
         directly_mapped_type = _DIRECTLY_MAPPED_TYPES.get(fhir_type)
         if directly_mapped_type is not None:
             return directly_mapped_type
-        return "String"
+        return FhirCqlType("String")
 
-    def map_ref_to_cql_type(self, ref: Optional[str]) -> str:
+    def map_ref_to_cql_type(self, ref: Optional[str]) -> FhirCqlType:
         if ref is None:
             raise ValueError("PropertyDeclaration must have ref for ref")
         identifier = ref.replace("#/definitions/", "")
         if identifier in _DIRECTLY_MAPPED_TYPES:
             return self.map_fhir_to_cql_type(identifier)
         if identifier in self.__backbone_elements:
-            return f"BackboneElement:{identifier}"
+            return FhirCqlType(identifier, is_backbone_element=True)
 
         return self.map_fhir_to_cql_type(identifier)
 
-    def map_array_to_cql_type(self, item_type: Optional[str]) -> str:
+    def map_array_to_cql_type(self, item_type: Optional[str]) -> FhirCqlType:
         if item_type is None:
             raise ValueError("PropertyDeclaration must have item_type for array")
         if item_type.startswith("#/definitions/"):
-            return f"List<{self.map_ref_to_cql_type(item_type)}>"
-        return f"List<{self.map_fhir_to_cql_type(item_type)}>"
+            return FhirList(item_type=self.map_ref_to_cql_type(item_type))
+        return FhirList(item_type=self.map_fhir_to_cql_type(item_type))
 
-    def map_declaration_to_cql_type(self, declaration: PropertyDeclaration) -> str:
+    def map_declaration_to_cql_type(
+        self, declaration: PropertyDeclaration
+    ) -> FhirCqlType:
         if declaration.type == "choice":
-            choices = "|".join(
-                list(
-                    {
-                        self.map_declaration_to_cql_type(choice)
-                        for choice in declaration.choices
-                    }
-                )
+            choices = list(
+                {
+                    self.map_declaration_to_cql_type(choice)
+                    for choice in declaration.choices
+                }
             )
-            if "Interval<DateTime>" in choices:
-                return "Choice:Interval<DateTime>"
-            return f"Choice:String"
+            return FhirChoice(choices=choices)
         if declaration.type == "enum":
-            return "String"
+            return FhirCqlType("String")
         if declaration.type == "array":
             return self.map_array_to_cql_type(declaration.item_type)
         if declaration.type == "ref":
             return self.map_ref_to_cql_type(declaration.ref)
 
         return self.map_fhir_to_cql_type(declaration.type)
 
@@ -297,8 +331,10 @@
 
 # %%
 if __name__ == "__main__":
     argument_parser = ArgumentParser()
     argument_parser.add_argument("file_path", type=str)
     args = argument_parser.parse_args()
     print(main(args.file_path))
-    # print(main("C:/Users/jerem/Downloads/fhir.schema.json/fhir.schema.json"))
+
+
+# %%
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/any.py` & `cqlpy-0.2.7/cqlpy/_internal/types/any.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/boolean.py` & `cqlpy-0.2.7/cqlpy/_internal/types/boolean.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/code.py` & `cqlpy-0.2.7/cqlpy/_internal/types/code.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/code_system.py` & `cqlpy-0.2.7/cqlpy/_internal/types/code_system.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/concept.py` & `cqlpy-0.2.7/cqlpy/_internal/types/concept.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,14 @@
     def parse_fhir_json(
         cls,
         fhir_json: dict[str, list[dict[str, str]]],
         subtype: Optional[Type["CqlAny"]] = None,
     ) -> "Concept":
         if "coding" in fhir_json:
             codes = [
-                Code().parse_fhir_json(fhir_code) for fhir_code in fhir_json["coding"]
+                Code.parse_fhir_json(fhir_code) for fhir_code in fhir_json["coding"]
             ]
         else:
             codes = []
         display = ""
 
         return cls(codes=codes)
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/date.py` & `cqlpy-0.2.7/cqlpy/_internal/types/date.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/datetime.py` & `cqlpy-0.2.7/cqlpy/_internal/types/datetime.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/decimal.py` & `cqlpy-0.2.7/cqlpy/_internal/types/decimal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/integer.py` & `cqlpy-0.2.7/cqlpy/_internal/types/integer.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/interval.py` & `cqlpy-0.2.7/cqlpy/_internal/types/interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/list.py` & `cqlpy-0.2.7/cqlpy/_internal/types/list.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/quantity.py` & `cqlpy-0.2.7/cqlpy/_internal/types/quantity.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/string.py` & `cqlpy-0.2.7/cqlpy/_internal/types/string.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/value_set.py` & `cqlpy-0.2.7/cqlpy/_internal/types/valueset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Any, Optional, Type
 from cqlpy._internal.types.any import CqlAny
 from cqlpy._internal.types.code import Code
 
 
-class ValueSet(CqlAny[dict[str, Any], list[Code]]):
+class Valueset(CqlAny[dict[str, Any], list[Code]]):
     def __init__(
         self,
-        value_set_id: Optional[str] = None,
+        valueset_id: Optional[str] = None,
         name: Optional[str] = None,
         version: Optional[str] = None,
         use_context: Optional[str] = None,
         codes: Optional[list[Code]] = None,
     ):
-        self.id = value_set_id
+        self.id = valueset_id
         self.name = name
         self.version = version
         self.use_context = use_context
         self.codes: list[Code] = codes or []
 
     def __str__(self) -> str:
         return (
@@ -29,31 +29,31 @@
         )
 
     @property
     def value(self) -> list[Code]:
         return self.codes
 
     @classmethod
-    def parse_cql(cls, cql: str, subtype: Optional[Type[CqlAny]] = None) -> "ValueSet":
-        value_set_id = ""
+    def parse_cql(cls, cql: str, subtype: Optional[Type[CqlAny]] = None) -> "Valueset":
+        valueset_id = ""
         version = ""
         name = ""
 
         return cls(
-            value_set_id=value_set_id,
+            valueset_id=valueset_id,
             name=name,
             version=version,
         )
 
     @classmethod
     def parse_fhir_json(
         cls,
         fhir_json: dict[str, Any],
         subtype: Optional[Type["CqlAny"]] = None,
-    ) -> "ValueSet":
+    ) -> "Valueset":
         version: str = fhir_json["version"]
         name: str = fhir_json["name"]
         includes: list[dict[str, Any]] = fhir_json["compose"]["include"]
 
         codes = [
             Code(
                 system=include.get("system", ""),
@@ -62,12 +62,12 @@
                 version=include.get("version", ""),
             )
             for include in includes
             for concept in include["concept"]
         ]
 
         return cls(
-            value_set_id="",
+            valueset_id="",
             name=name,
             version=version,
             codes=codes,
         )
```

### Comparing `cqlpy-0.2.6/cqlpy/_internal/types/value_set_scope.py` & `cqlpy-0.2.7/cqlpy/_internal/types/valueset_scope.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any, Optional, Type
 from cqlpy._internal.types.any import CqlAny
 from cqlpy._internal.types.code import Code
-from cqlpy._internal.types.value_set import ValueSet
+from cqlpy._internal.types.valueset import Valueset
 
 
-class ValueSetScope:
+class ValuesetScope:
     """
     Represents named collection of value sets. This is used for some
     value set providers to indicate that the value sets are related in
     some way, usually by provenance.
 
     This class is not a part of the CQL specification.
 
-    :param value_set_scope_id: The id of the value set scope. This
+    :param valueset_scope_id: The id of the value set scope. This
         must be unique to the provider.
     """
 
-    def __init__(self, value_set_scope_id: Optional[str] = None):
-        self.id = value_set_scope_id
+    def __init__(self, valueset_scope_id: Optional[str] = None):
+        self.id = valueset_scope_id
 
     def __str__(self) -> str:
         return "id:" + (self.id or "")
```

### Comparing `cqlpy-0.2.6/cqlpy/operators.py` & `cqlpy-0.2.7/cqlpy/operators.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.6/cqlpy/providers/rosetta_valueset_provider.py` & `cqlpy-0.2.7/cqlpy/_internal/providers/rosetta_valueset_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from datetime import datetime
 import urllib
 import requests
 
 from typing import Optional, Any
 
-from cqlpy._internal.types.value_set import ValueSet
+from cqlpy._internal.types.valueset import Valueset
 
 
 FHIR_VERSION = "R4"
 ROSETTA_BASE_URL = (
     f"https://api.rosetta.careevolution.com/terminology/v1/fhir/{FHIR_VERSION}"
 )
 ROSETTA_PAGE_SIZE = 250
 
 
-class RosettaValueSetProvider:
+class RosettaValuesetProvider:
     def __init__(self, logger: Any, api_key: str):
         self._logger = logger
         self._api_key = api_key
 
     def _get_valueset_url(
         self,
         name: Optional[str] = None,
@@ -30,16 +30,16 @@
 
         if scope is None and name is None:
             raise ValueError("Either scope or name must be provided")
 
         if scope:
             extension = f"&extension.scope={scope}"
         if name:
-            value_set_id = urllib.parse.quote_plus(name)
-            name_param = f"name={value_set_id}"
+            valueset_id = urllib.parse.quote_plus(name)
+            name_param = f"name={valueset_id}"
 
         url = f"{ROSETTA_BASE_URL}/ValueSet?{name_param}&page.num={page_number}&_count={ROSETTA_PAGE_SIZE}{extension}"
 
         return url
 
     def _get_request_headers(self, zip_encoding):
         header = {
```

### Comparing `cqlpy-0.2.6/cqlpy/types.py` & `cqlpy-0.2.7/cqlpy/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from cqlpy._internal.types.code_system import CodeSystem
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.concept import Concept
 from cqlpy._internal.types.date import Date
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.interval import Interval
 from cqlpy._internal.types.quantity import Quantity
-from cqlpy._internal.types.value_set import ValueSet
+from cqlpy._internal.types.valueset import Valueset
 from cqlpy._internal.parameter import Parameter
 from cqlpy._internal.types.boolean import Boolean
 from cqlpy._internal.types.string import String
 from cqlpy._internal.types.decimal import Decimal
 from cqlpy._internal.types.long import Long
 from cqlpy._internal.types.integer import Integer
 from cqlpy._internal.types.list import List
@@ -22,15 +22,15 @@
     "CodeSystem",
     "Code",
     "Concept",
     "Date",
     "DateTime",
     "Interval",
     "Quantity",
-    "ValueSet",
+    "Valueset",
     "Parameter",
     "Boolean",
     "String",
     "Decimal",
     "Long",
     "Integer",
     "List",
```

### Comparing `cqlpy-0.2.6/pyproject.toml` & `cqlpy-0.2.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "John Wyderko <john@careevolution.com>",
   "Jeremy Fortune <jeremy@careevolution.com>",
 ]
 description = "Tooling to execute CQL-like Python against FHIR resources."
 license = "MIT"
 name = "cqlpy"
 readme = "README.md"
-version = "0.2.6"
+version = "0.2.7"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^23.3.0"}
```

### Comparing `cqlpy-0.2.6/PKG-INFO` & `cqlpy-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqlpy
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tooling to execute CQL-like Python against FHIR resources.
 License: MIT
 Author: John Wyderko
 Author-email: john@careevolution.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

