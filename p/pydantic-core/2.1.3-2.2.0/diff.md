# Comparing `tmp/pydantic_core-2.1.3.tar.gz` & `tmp/pydantic_core-2.2.0.tar.gz`

## Comparing `pydantic_core-2.1.3.tar` & `pydantic_core-2.2.0.tar`

### file list

```diff
@@ -1,206 +1,206 @@
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 pydantic_core-2.1.3/Cargo.toml
--rw-r--r--   0     1001      123      312 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/.cargo/config.toml
--rw-r--r--   0     1001      123     1080 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/LICENSE
--rw-r--r--   0     1001      123     5052 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/Makefile
--rw-r--r--   0     1001      123     3704 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/README.md
--rw-r--r--   0     1001      123     1366 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/build.rs
--rw-r--r--   0     1001      123     8313 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/generate_self_schema.py
--rw-r--r--   0     1001      123     3340 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/pyproject.toml
--rw-r--r--   0     1001      123     3065 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/argument_markers.rs
--rw-r--r--   0     1001      123     5811 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/build_tools.rs
--rw-r--r--   0     1001      123     4486 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/definitions.rs
--rw-r--r--   0     1001      123     5441 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/errors/line_error.rs
--rw-r--r--   0     1001      123     7101 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/errors/location.rs
--rw-r--r--   0     1001      123     1065 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/errors/mod.rs
--rw-r--r--   0     1001      123    33615 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/errors/types.rs
--rw-r--r--   0     1001      123    17567 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/errors/validation_exception.rs
--rw-r--r--   0     1001      123     5046 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/errors/value_exception.rs
--rw-r--r--   0     1001      123    13976 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/input/datetime.rs
--rw-r--r--   0     1001      123     8292 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/input/input_abstract.rs
--rw-r--r--   0     1001      123    17728 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/input/input_json.rs
--rw-r--r--   0     1001      123    26556 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/input/input_python.rs
--rw-r--r--   0     1001      123      981 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/input/mod.rs
--rw-r--r--   0     1001      123     5342 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/input/parse_json.rs
--rw-r--r--   0     1001      123    31974 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/input/return_enums.rs
--rw-r--r--   0     1001      123     3426 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/input/shared.rs
--rw-r--r--   0     1001      123     1756 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/lazy_index_map.rs
--rw-r--r--   0     1001      123     3556 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/lib.rs
--rw-r--r--   0     1001      123    17853 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/lookup_key.rs
--rw-r--r--   0     1001      123     2484 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/recursion_guard.rs
--rw-r--r--   0     1001      123     5605 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/computed_fields.rs
--rw-r--r--   0     1001      123     5486 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/config.rs
--rw-r--r--   0     1001      123     2779 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/errors.rs
--rw-r--r--   0     1001      123    11523 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/extra.rs
--rw-r--r--   0     1001      123    12294 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/fields.rs
--rw-r--r--   0     1001      123    14578 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/filter.rs
--rw-r--r--   0     1001      123    25370 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/infer.rs
--rw-r--r--   0     1001      123     7814 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/mod.rs
--rw-r--r--   0     1001      123    11222 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/ob_type.rs
--rw-r--r--   0     1001      123    14829 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/shared.rs
--rw-r--r--   0     1001      123     1419 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/any.rs
--rw-r--r--   0     1001      123     2507 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/bytes.rs
--rw-r--r--   0     1001      123     6558 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/dataclass.rs
--rw-r--r--   0     1001      123     3921 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/datetime_etc.rs
--rw-r--r--   0     1001      123     3226 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/definitions.rs
--rw-r--r--   0     1001      123     5250 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/dict.rs
--rw-r--r--   0     1001      123     6534 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/format.rs
--rw-r--r--   0     1001      123    22198 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/function.rs
--rw-r--r--   0     1001      123     7344 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/generator.rs
--rw-r--r--   0     1001      123     2961 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/json.rs
--rw-r--r--   0     1001      123     2196 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/json_or_python.rs
--rw-r--r--   0     1001      123     4053 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/list.rs
--rw-r--r--   0     1001      123     5517 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/literal.rs
--rw-r--r--   0     1001      123     1077 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/mod.rs
--rw-r--r--   0     1001      123     8181 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/model.rs
--rw-r--r--   0     1001      123     2388 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/nullable.rs
--rw-r--r--   0     1001      123     3513 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/other.rs
--rw-r--r--   0     1001      123     4489 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/set_frozenset.rs
--rw-r--r--   0     1001      123     5912 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/simple.rs
--rw-r--r--   0     1001      123     2576 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/string.rs
--rw-r--r--   0     1001      123     2464 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/timedelta.rs
--rw-r--r--   0     1001      123    12727 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/tuple.rs
--rw-r--r--   0     1001      123     2482 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/typed_dict.rs
--rw-r--r--   0     1001      123     6947 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/union.rs
--rw-r--r--   0     1001      123     3114 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/url.rs
--rw-r--r--   0     1001      123     2054 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/serializers/type_serializers/with_default.rs
--rw-r--r--   0     1001      123     2736 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/tools.rs
--rw-r--r--   0     1001      123    11321 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/url.rs
--rw-r--r--   0     1001      123     1468 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/any.rs
--rw-r--r--   0     1001      123    15665 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/arguments.rs
--rw-r--r--   0     1001      123     1662 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/bool.rs
--rw-r--r--   0     1001      123     3769 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/bytes.rs
--rw-r--r--   0     1001      123     4399 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/call.rs
--rw-r--r--   0     1001      123     1504 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/callable.rs
--rw-r--r--   0     1001      123     3391 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/chain.rs
--rw-r--r--   0     1001      123     3928 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/custom_error.rs
--rw-r--r--   0     1001      123    24975 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/dataclass.rs
--rw-r--r--   0     1001      123     7033 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/date.rs
--rw-r--r--   0     1001      123     9231 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/datetime.rs
--rw-r--r--   0     1001      123     6801 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/definitions.rs
--rw-r--r--   0     1001      123     6528 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/dict.rs
--rw-r--r--   0     1001      123     6276 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/float.rs
--rw-r--r--   0     1001      123     2035 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/frozenset.rs
--rw-r--r--   0     1001      123    18903 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/function.rs
--rw-r--r--   0     1001      123    11183 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/generator.rs
--rw-r--r--   0     1001      123     4929 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/int.rs
--rw-r--r--   0     1001      123     3256 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/is_instance.rs
--rw-r--r--   0     1001      123     2201 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/is_subclass.rs
--rw-r--r--   0     1001      123     2600 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/json.rs
--rw-r--r--   0     1001      123     2568 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/json_or_python.rs
--rw-r--r--   0     1001      123     2752 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/lax_or_strict.rs
--rw-r--r--   0     1001      123     5826 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/list.rs
--rw-r--r--   0     1001      123     6500 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/literal.rs
--rw-r--r--   0     1001      123    23341 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/mod.rs
--rw-r--r--   0     1001      123    14906 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/model.rs
--rw-r--r--   0     1001      123    17050 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/model_fields.rs
--rw-r--r--   0     1001      123     1477 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/none.rs
--rw-r--r--   0     1001      123     1953 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/nullable.rs
--rw-r--r--   0     1001      123     3158 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/set.rs
--rw-r--r--   0     1001      123     6190 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/string.rs
--rw-r--r--   0     1001      123     3888 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/time.rs
--rw-r--r--   0     1001      123     3927 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/timedelta.rs
--rw-r--r--   0     1001      123     9993 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/tuple.rs
--rw-r--r--   0     1001      123    12699 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/typed_dict.rs
--rw-r--r--   0     1001      123    16840 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/union.rs
--rw-r--r--   0     1001      123    17932 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/url.rs
--rw-r--r--   0     1001      123     6970 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/src/validators/with_default.rs
--rw-r--r--   0     1001      123        0 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/__init__.py
--rw-r--r--   0     1001      123        0 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/benchmarks/__init__.py
--rw-r--r--   0     1001      123    15198 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/benchmarks/complete_schema.py
--rw-r--r--   0     1001      123     4950 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/benchmarks/test_complete_benchmark.py
--rw-r--r--   0     1001      123    38992 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/benchmarks/test_micro_benchmarks.py
--rw-r--r--   0     1001      123    14015 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/benchmarks/test_serialization_micro.py
--rw-r--r--   0     1001      123     4110 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/conftest.py
--rw-r--r--   0     1001      123     3272 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/emscripten_runner.js
--rw-r--r--   0     1001      123       72 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/requirements-linting.txt
--rw-r--r--   0     1001      123      190 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/requirements.txt
--rw-r--r--   0     1001      123        0 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/__init__.py
--rw-r--r--   0     1001      123    23747 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_any.py
--rw-r--r--   0     1001      123     4342 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_bytes.py
--rw-r--r--   0     1001      123     5571 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_dataclasses.py
--rw-r--r--   0     1001      123     4798 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_datetime.py
--rw-r--r--   0     1001      123     3901 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_definitions.py
--rw-r--r--   0     1001      123     4164 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_definitions_recursive.py
--rw-r--r--   0     1001      123     7509 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_dict.py
--rw-r--r--   0     1001      123     4659 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_format.py
--rw-r--r--   0     1001      123    22938 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_functions.py
--rw-r--r--   0     1001      123     5424 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_generator.py
--rw-r--r--   0     1001      123     1853 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_json.py
--rw-r--r--   0     1001      123      540 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_json_or_python.py
--rw-r--r--   0     1001      123    18385 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_list_tuple.py
--rw-r--r--   0     1001      123     2172 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_literal.py
--rw-r--r--   0     1001      123      517 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_misc.py
--rw-r--r--   0     1001      123    32725 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_model.py
--rw-r--r--   0     1001      123     5749 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_model_root.py
--rw-r--r--   0     1001      123      953 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_none.py
--rw-r--r--   0     1001      123      566 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_nullable.py
--rw-r--r--   0     1001      123     2174 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_other.py
--rw-r--r--   0     1001      123     2052 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_set_frozenset.py
--rw-r--r--   0     1001      123     2172 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_simple.py
--rw-r--r--   0     1001      123     2503 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_string.py
--rw-r--r--   0     1001      123     1665 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_timedelta.py
--rw-r--r--   0     1001      123    12753 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_typed_dict.py
--rw-r--r--   0     1001      123    13375 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_union.py
--rw-r--r--   0     1001      123     4287 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/serializers/test_url.py
--rw-r--r--   0     1001      123     2065 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test.rs
--rw-r--r--   0     1001      123     4764 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_build.py
--rw-r--r--   0     1001      123     4675 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_config.py
--rw-r--r--   0     1001      123     1246 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_docstrings.py
--rw-r--r--   0     1001      123    29152 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_errors.py
--rw-r--r--   0     1001      123     2187 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_garbage_collection.py
--rw-r--r--   0     1001      123     6159 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_hypothesis.py
--rw-r--r--   0     1001      123     2184 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_isinstance.py
--rw-r--r--   0     1001      123    11675 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_json.py
--rw-r--r--   0     1001      123     7069 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_misc.py
--rw-r--r--   0     1001      123    12707 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_schema_functions.py
--rw-r--r--   0     1001      123     1795 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_strict.py
--rw-r--r--   0     1001      123     9150 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_typing.py
--rw-r--r--   0     1001      123     5013 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/test_validation_context.py
--rw-r--r--   0     1001      123        0 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/__init__.py
--rw-r--r--   0     1001      123    35676 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_arguments.py
--rw-r--r--   0     1001      123     4108 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_bool.py
--rw-r--r--   0     1001      123     4396 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_bytes.py
--rw-r--r--   0     1001      123     7161 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_call.py
--rw-r--r--   0     1001      123     1492 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_callable.py
--rw-r--r--   0     1001      123     4083 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_chain.py
--rw-r--r--   0     1001      123     1699 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_custom_error.py
--rw-r--r--   0     1001      123    50588 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_dataclasses.py
--rw-r--r--   0     1001      123    12100 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_date.py
--rw-r--r--   0     1001      123    20109 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_datetime.py
--rw-r--r--   0     1001      123     4913 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_definitions.py
--rw-r--r--   0     1001      123    31995 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_definitions_recursive.py
--rw-r--r--   0     1001      123     9074 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_dict.py
--rw-r--r--   0     1001      123    11686 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_float.py
--rw-r--r--   0     1001      123    11389 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_frozenset.py
--rw-r--r--   0     1001      123    29953 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_function.py
--rw-r--r--   0     1001      123     6819 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_generator.py
--rw-r--r--   0     1001      123    14055 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_int.py
--rw-r--r--   0     1001      123     5119 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_is_instance.py
--rw-r--r--   0     1001      123     2065 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_is_subclass.py
--rw-r--r--   0     1001      123     5260 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_json.py
--rw-r--r--   0     1001      123     1027 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_json_or_python.py
--rw-r--r--   0     1001      123     1640 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_lax_or_strict.py
--rw-r--r--   0     1001      123    16913 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_list.py
--rw-r--r--   0     1001      123    12324 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_literal.py
--rw-r--r--   0     1001      123    39054 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_model.py
--rw-r--r--   0     1001      123    62078 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_model_fields.py
--rw-r--r--   0     1001      123    13996 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_model_init.py
--rw-r--r--   0     1001      123     7108 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_model_root.py
--rw-r--r--   0     1001      123      760 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_none.py
--rw-r--r--   0     1001      123     1056 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_nullable.py
--rw-r--r--   0     1001      123    10405 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_set.py
--rw-r--r--   0     1001      123     8318 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_string.py
--rw-r--r--   0     1001      123    22574 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_tagged_union.py
--rw-r--r--   0     1001      123    12215 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_time.py
--rw-r--r--   0     1001      123    12659 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_timedelta.py
--rw-r--r--   0     1001      123    18166 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_tuple.py
--rw-r--r--   0     1001      123    41936 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_typed_dict.py
--rw-r--r--   0     1001      123    15403 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_union.py
--rw-r--r--   0     1001      123    53089 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_url.py
--rw-r--r--   0     1001      123    21767 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/tests/validators/test_with_default.py
--rw-r--r--   0     1001      123    16513 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/Cargo.lock
--rw-r--r--   0     1001      123        1 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/python/pydantic_core/py.typed
--rw-r--r--   0     1001      123     8766 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/python/pydantic_core/_pydantic_core.pyi
--rw-r--r--   0     1001      123   128560 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/python/pydantic_core/core_schema.py
--rw-r--r--   0     1001      123     2190 2023-07-11 01:04:22.000000 pydantic_core-2.1.3/python/pydantic_core/__init__.py
--rw-r--r--   0        0        0     5116 1970-01-01 00:00:00.000000 pydantic_core-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 pydantic_core-2.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      312 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/.cargo/config.toml
+-rw-r--r--   0     1001      123     1080 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/LICENSE
+-rw-r--r--   0     1001      123     5052 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/Makefile
+-rw-r--r--   0     1001      123     3704 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/README.md
+-rw-r--r--   0     1001      123     1366 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/build.rs
+-rw-r--r--   0     1001      123     8313 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/generate_self_schema.py
+-rw-r--r--   0     1001      123     3340 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/pyproject.toml
+-rw-r--r--   0     1001      123     3065 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/argument_markers.rs
+-rw-r--r--   0     1001      123     5811 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/build_tools.rs
+-rw-r--r--   0     1001      123     4486 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/definitions.rs
+-rw-r--r--   0     1001      123     5441 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/line_error.rs
+-rw-r--r--   0     1001      123     7101 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/location.rs
+-rw-r--r--   0     1001      123     1065 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/mod.rs
+-rw-r--r--   0     1001      123    33615 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/types.rs
+-rw-r--r--   0     1001      123    17567 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/validation_exception.rs
+-rw-r--r--   0     1001      123     5046 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/value_exception.rs
+-rw-r--r--   0     1001      123    13976 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/datetime.rs
+-rw-r--r--   0     1001      123     8292 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/input_abstract.rs
+-rw-r--r--   0     1001      123    18291 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/input_json.rs
+-rw-r--r--   0     1001      123    26556 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/input_python.rs
+-rw-r--r--   0     1001      123      981 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/mod.rs
+-rw-r--r--   0     1001      123     7700 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/parse_json.rs
+-rw-r--r--   0     1001      123    32794 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/return_enums.rs
+-rw-r--r--   0     1001      123     3426 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/shared.rs
+-rw-r--r--   0     1001      123     1756 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/lazy_index_map.rs
+-rw-r--r--   0     1001      123     3556 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/lib.rs
+-rw-r--r--   0     1001      123    17853 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/lookup_key.rs
+-rw-r--r--   0     1001      123     2484 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/recursion_guard.rs
+-rw-r--r--   0     1001      123     5605 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/computed_fields.rs
+-rw-r--r--   0     1001      123     5486 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/config.rs
+-rw-r--r--   0     1001      123     2779 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/errors.rs
+-rw-r--r--   0     1001      123    11523 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/extra.rs
+-rw-r--r--   0     1001      123    12294 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/fields.rs
+-rw-r--r--   0     1001      123    14578 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/filter.rs
+-rw-r--r--   0     1001      123    25393 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/infer.rs
+-rw-r--r--   0     1001      123     7814 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/mod.rs
+-rw-r--r--   0     1001      123    11222 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/ob_type.rs
+-rw-r--r--   0     1001      123    14829 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/shared.rs
+-rw-r--r--   0     1001      123     1419 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/any.rs
+-rw-r--r--   0     1001      123     2507 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/bytes.rs
+-rw-r--r--   0     1001      123     6558 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/dataclass.rs
+-rw-r--r--   0     1001      123     3921 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/datetime_etc.rs
+-rw-r--r--   0     1001      123     3226 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/definitions.rs
+-rw-r--r--   0     1001      123     5250 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/dict.rs
+-rw-r--r--   0     1001      123     6534 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/format.rs
+-rw-r--r--   0     1001      123    22198 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/function.rs
+-rw-r--r--   0     1001      123     7344 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/generator.rs
+-rw-r--r--   0     1001      123     2961 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/json.rs
+-rw-r--r--   0     1001      123     2196 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/json_or_python.rs
+-rw-r--r--   0     1001      123     4053 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/list.rs
+-rw-r--r--   0     1001      123     5517 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/literal.rs
+-rw-r--r--   0     1001      123     1077 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/mod.rs
+-rw-r--r--   0     1001      123     8181 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/model.rs
+-rw-r--r--   0     1001      123     2388 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/nullable.rs
+-rw-r--r--   0     1001      123     3513 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/other.rs
+-rw-r--r--   0     1001      123     4489 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/set_frozenset.rs
+-rw-r--r--   0     1001      123     5926 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/simple.rs
+-rw-r--r--   0     1001      123     2576 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/string.rs
+-rw-r--r--   0     1001      123     2464 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/timedelta.rs
+-rw-r--r--   0     1001      123    12727 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/tuple.rs
+-rw-r--r--   0     1001      123     2482 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/typed_dict.rs
+-rw-r--r--   0     1001      123     6947 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/union.rs
+-rw-r--r--   0     1001      123     3114 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/url.rs
+-rw-r--r--   0     1001      123     2054 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/with_default.rs
+-rw-r--r--   0     1001      123     2736 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/tools.rs
+-rw-r--r--   0     1001      123    16394 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/url.rs
+-rw-r--r--   0     1001      123     1468 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/any.rs
+-rw-r--r--   0     1001      123    15665 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/arguments.rs
+-rw-r--r--   0     1001      123     1662 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/bool.rs
+-rw-r--r--   0     1001      123     3769 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/bytes.rs
+-rw-r--r--   0     1001      123     4399 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/call.rs
+-rw-r--r--   0     1001      123     1504 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/callable.rs
+-rw-r--r--   0     1001      123     3391 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/chain.rs
+-rw-r--r--   0     1001      123     3928 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/custom_error.rs
+-rw-r--r--   0     1001      123    24975 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/dataclass.rs
+-rw-r--r--   0     1001      123     7033 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/date.rs
+-rw-r--r--   0     1001      123     9231 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/datetime.rs
+-rw-r--r--   0     1001      123     6801 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/definitions.rs
+-rw-r--r--   0     1001      123     6528 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/dict.rs
+-rw-r--r--   0     1001      123     6276 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/float.rs
+-rw-r--r--   0     1001      123     2035 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/frozenset.rs
+-rw-r--r--   0     1001      123    18903 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/function.rs
+-rw-r--r--   0     1001      123    11183 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/generator.rs
+-rw-r--r--   0     1001      123     4929 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/int.rs
+-rw-r--r--   0     1001      123     3256 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/is_instance.rs
+-rw-r--r--   0     1001      123     2201 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/is_subclass.rs
+-rw-r--r--   0     1001      123     2600 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/json.rs
+-rw-r--r--   0     1001      123     2568 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/json_or_python.rs
+-rw-r--r--   0     1001      123     2752 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/lax_or_strict.rs
+-rw-r--r--   0     1001      123     5826 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/list.rs
+-rw-r--r--   0     1001      123     6500 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/literal.rs
+-rw-r--r--   0     1001      123    23341 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/mod.rs
+-rw-r--r--   0     1001      123    14906 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/model.rs
+-rw-r--r--   0     1001      123    17050 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/model_fields.rs
+-rw-r--r--   0     1001      123     1477 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/none.rs
+-rw-r--r--   0     1001      123     1953 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/nullable.rs
+-rw-r--r--   0     1001      123     3158 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/set.rs
+-rw-r--r--   0     1001      123     6301 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/string.rs
+-rw-r--r--   0     1001      123     3888 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/time.rs
+-rw-r--r--   0     1001      123     3927 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/timedelta.rs
+-rw-r--r--   0     1001      123     9993 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/tuple.rs
+-rw-r--r--   0     1001      123    12699 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/typed_dict.rs
+-rw-r--r--   0     1001      123    16840 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/union.rs
+-rw-r--r--   0     1001      123    17932 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/url.rs
+-rw-r--r--   0     1001      123     6970 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/with_default.rs
+-rw-r--r--   0     1001      123        0 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/__init__.py
+-rw-r--r--   0     1001      123        0 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/__init__.py
+-rw-r--r--   0     1001      123    15198 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/complete_schema.py
+-rw-r--r--   0     1001      123     4950 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/test_complete_benchmark.py
+-rw-r--r--   0     1001      123    38992 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/test_micro_benchmarks.py
+-rw-r--r--   0     1001      123    14015 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/test_serialization_micro.py
+-rw-r--r--   0     1001      123     4110 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/conftest.py
+-rw-r--r--   0     1001      123     3272 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/emscripten_runner.js
+-rw-r--r--   0     1001      123       72 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/requirements-linting.txt
+-rw-r--r--   0     1001      123      190 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/requirements.txt
+-rw-r--r--   0     1001      123        0 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/__init__.py
+-rw-r--r--   0     1001      123    23747 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_any.py
+-rw-r--r--   0     1001      123     4342 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_bytes.py
+-rw-r--r--   0     1001      123     5571 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_dataclasses.py
+-rw-r--r--   0     1001      123     4798 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_datetime.py
+-rw-r--r--   0     1001      123     3901 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_definitions.py
+-rw-r--r--   0     1001      123     4164 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_definitions_recursive.py
+-rw-r--r--   0     1001      123     7509 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_dict.py
+-rw-r--r--   0     1001      123     4659 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_format.py
+-rw-r--r--   0     1001      123    22938 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_functions.py
+-rw-r--r--   0     1001      123     5424 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_generator.py
+-rw-r--r--   0     1001      123     1853 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_json.py
+-rw-r--r--   0     1001      123      540 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_json_or_python.py
+-rw-r--r--   0     1001      123    18385 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_list_tuple.py
+-rw-r--r--   0     1001      123     2172 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_literal.py
+-rw-r--r--   0     1001      123      517 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_misc.py
+-rw-r--r--   0     1001      123    32725 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_model.py
+-rw-r--r--   0     1001      123     5749 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_model_root.py
+-rw-r--r--   0     1001      123      953 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_none.py
+-rw-r--r--   0     1001      123      566 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_nullable.py
+-rw-r--r--   0     1001      123     2174 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_other.py
+-rw-r--r--   0     1001      123     2052 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_set_frozenset.py
+-rw-r--r--   0     1001      123     2334 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_simple.py
+-rw-r--r--   0     1001      123     2503 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_string.py
+-rw-r--r--   0     1001      123     1665 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_timedelta.py
+-rw-r--r--   0     1001      123    12753 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_typed_dict.py
+-rw-r--r--   0     1001      123    13375 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_union.py
+-rw-r--r--   0     1001      123     4287 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_url.py
+-rw-r--r--   0     1001      123     2065 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test.rs
+-rw-r--r--   0     1001      123     4764 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_build.py
+-rw-r--r--   0     1001      123     4675 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_config.py
+-rw-r--r--   0     1001      123     1246 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_docstrings.py
+-rw-r--r--   0     1001      123    29152 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_errors.py
+-rw-r--r--   0     1001      123     2187 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_garbage_collection.py
+-rw-r--r--   0     1001      123     6159 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_hypothesis.py
+-rw-r--r--   0     1001      123     2184 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_isinstance.py
+-rw-r--r--   0     1001      123    11916 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_json.py
+-rw-r--r--   0     1001      123     7069 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_misc.py
+-rw-r--r--   0     1001      123    12707 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_schema_functions.py
+-rw-r--r--   0     1001      123     1795 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_strict.py
+-rw-r--r--   0     1001      123     9150 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_typing.py
+-rw-r--r--   0     1001      123     5013 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_validation_context.py
+-rw-r--r--   0     1001      123        0 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/__init__.py
+-rw-r--r--   0     1001      123    35676 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_arguments.py
+-rw-r--r--   0     1001      123     4108 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_bool.py
+-rw-r--r--   0     1001      123     4396 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_bytes.py
+-rw-r--r--   0     1001      123     7161 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_call.py
+-rw-r--r--   0     1001      123     1492 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_callable.py
+-rw-r--r--   0     1001      123     4083 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_chain.py
+-rw-r--r--   0     1001      123     1699 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_custom_error.py
+-rw-r--r--   0     1001      123    50588 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_dataclasses.py
+-rw-r--r--   0     1001      123    12100 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_date.py
+-rw-r--r--   0     1001      123    20109 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_datetime.py
+-rw-r--r--   0     1001      123     4913 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_definitions.py
+-rw-r--r--   0     1001      123    31995 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_definitions_recursive.py
+-rw-r--r--   0     1001      123     9074 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_dict.py
+-rw-r--r--   0     1001      123    11686 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_float.py
+-rw-r--r--   0     1001      123    11389 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_frozenset.py
+-rw-r--r--   0     1001      123    29953 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_function.py
+-rw-r--r--   0     1001      123     6819 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_generator.py
+-rw-r--r--   0     1001      123    13642 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_int.py
+-rw-r--r--   0     1001      123     5119 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_is_instance.py
+-rw-r--r--   0     1001      123     2065 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_is_subclass.py
+-rw-r--r--   0     1001      123     5260 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_json.py
+-rw-r--r--   0     1001      123     1027 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_json_or_python.py
+-rw-r--r--   0     1001      123     1640 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_lax_or_strict.py
+-rw-r--r--   0     1001      123    16913 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_list.py
+-rw-r--r--   0     1001      123    12324 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_literal.py
+-rw-r--r--   0     1001      123    39054 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_model.py
+-rw-r--r--   0     1001      123    62078 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_model_fields.py
+-rw-r--r--   0     1001      123    13996 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_model_init.py
+-rw-r--r--   0     1001      123     7108 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_model_root.py
+-rw-r--r--   0     1001      123      760 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_none.py
+-rw-r--r--   0     1001      123     1056 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_nullable.py
+-rw-r--r--   0     1001      123    10405 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_set.py
+-rw-r--r--   0     1001      123     9016 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_string.py
+-rw-r--r--   0     1001      123    22574 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_tagged_union.py
+-rw-r--r--   0     1001      123    12215 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_time.py
+-rw-r--r--   0     1001      123    12659 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_timedelta.py
+-rw-r--r--   0     1001      123    18166 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_tuple.py
+-rw-r--r--   0     1001      123    41936 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_typed_dict.py
+-rw-r--r--   0     1001      123    15403 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_union.py
+-rw-r--r--   0     1001      123    56241 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_url.py
+-rw-r--r--   0     1001      123    21767 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_with_default.py
+-rw-r--r--   0     1001      123    16807 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/Cargo.lock
+-rw-r--r--   0     1001      123        1 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/python/pydantic_core/py.typed
+-rw-r--r--   0     1001      123     9532 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/python/pydantic_core/_pydantic_core.pyi
+-rw-r--r--   0     1001      123   128560 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/python/pydantic_core/core_schema.py
+-rw-r--r--   0     1001      123     2190 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/python/pydantic_core/__init__.py
+-rw-r--r--   0        0        0     5116 1970-01-01 00:00:00.000000 pydantic_core-2.2.0/PKG-INFO
```

### Comparing `pydantic_core-2.1.3/Cargo.toml` & `pydantic_core-2.2.0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pydantic-core"
-version = "2.1.3"
+version = "2.2.0"
 edition = "2021"
 license = "MIT"
 homepage = "https://github.com/pydantic/pydantic-core"
 repository = "https://github.com/pydantic/pydantic-core.git"
 readme = "README.md"
 include = [
     "/pyproject.toml",
@@ -26,17 +26,17 @@
 ]
 
 [dependencies]
 pyo3 = { version = "0.19.1", features = ["generate-import-lib", "num-bigint"] }
 regex = "1.6.0"
 strum = { version = "0.25.0", features = ["derive"] }
 strum_macros = "0.24.3"
-serde_json = {version = "1.0.87", features = ["preserve_order"]}
+serde_json = {version = "1.0.87", features = ["arbitrary_precision", "preserve_order"]}
 enum_dispatch = "0.3.8"
-serde = "1.0.147"
+serde = { version = "1.0.147", features = ["derive"] }
 # disabled for benchmarks since it makes microbenchmark performance more flakey
 mimalloc = { version = "0.1.30", optional = true, default-features = false, features = ["local_dynamic_tls"] }
 speedate = "0.9.1"
 ahash = "0.8.0"
 url = "2.3.1"
 # idna is already required by url, added here to be explicit
 idna = "0.3.0"
```

### Comparing `pydantic_core-2.1.3/LICENSE` & `pydantic_core-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/Makefile` & `pydantic_core-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/README.md` & `pydantic_core-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/build.rs` & `pydantic_core-2.2.0/build.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/generate_self_schema.py` & `pydantic_core-2.2.0/generate_self_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/pyproject.toml` & `pydantic_core-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/argument_markers.rs` & `pydantic_core-2.2.0/src/argument_markers.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/build_tools.rs` & `pydantic_core-2.2.0/src/build_tools.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/definitions.rs` & `pydantic_core-2.2.0/src/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/errors/line_error.rs` & `pydantic_core-2.2.0/src/errors/line_error.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/errors/location.rs` & `pydantic_core-2.2.0/src/errors/location.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/errors/mod.rs` & `pydantic_core-2.2.0/src/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/errors/types.rs` & `pydantic_core-2.2.0/src/errors/types.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/errors/validation_exception.rs` & `pydantic_core-2.2.0/src/errors/validation_exception.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/errors/value_exception.rs` & `pydantic_core-2.2.0/src/errors/value_exception.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/input/datetime.rs` & `pydantic_core-2.2.0/src/input/datetime.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/input/input_abstract.rs` & `pydantic_core-2.2.0/src/input/input_abstract.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/input/input_json.rs` & `pydantic_core-2.2.0/src/input/input_json.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+use std::borrow::Cow;
+
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
+use strum::EnumMessage;
 
 use crate::errors::{ErrorType, InputValue, LocItem, ValError, ValResult};
 
 use super::datetime::{
     bytes_as_date, bytes_as_datetime, bytes_as_time, bytes_as_timedelta, float_as_datetime, float_as_duration,
     float_as_time, int_as_datetime, int_as_duration, int_as_time, EitherDate, EitherDateTime, EitherTime,
 };
@@ -114,25 +117,27 @@
         }
     }
 
     fn strict_int(&'a self) -> ValResult<EitherInt<'a>> {
         match self {
             JsonInput::Int(i) => Ok(EitherInt::I64(*i)),
             JsonInput::Uint(u) => Ok(EitherInt::U64(*u)),
+            JsonInput::BigInt(b) => Ok(EitherInt::BigInt(b.clone())),
             _ => Err(ValError::new(ErrorType::IntType, self)),
         }
     }
     fn lax_int(&'a self) -> ValResult<EitherInt<'a>> {
         match self {
             JsonInput::Bool(b) => match *b {
                 true => Ok(EitherInt::I64(1)),
                 false => Ok(EitherInt::I64(0)),
             },
             JsonInput::Int(i) => Ok(EitherInt::I64(*i)),
             JsonInput::Uint(u) => Ok(EitherInt::U64(*u)),
+            JsonInput::BigInt(b) => Ok(EitherInt::BigInt(b.clone())),
             JsonInput::Float(f) => float_as_int(self, *f),
             JsonInput::String(str) => str_as_int(self, str),
             _ => Err(ValError::new(ErrorType::IntType, self)),
         }
     }
 
     fn ultra_strict_float(&'a self) -> ValResult<EitherFloat<'a>> {
@@ -266,14 +271,24 @@
         }
     }
     fn lax_time(&self) -> ValResult<EitherTime> {
         match self {
             JsonInput::String(v) => bytes_as_time(self, v.as_bytes()),
             JsonInput::Int(v) => int_as_time(self, *v, 0),
             JsonInput::Float(v) => float_as_time(self, *v),
+            JsonInput::BigInt(_) => Err(ValError::new(
+                ErrorType::TimeParsing {
+                    error: Cow::Borrowed(
+                        speedate::ParseError::TimeTooLarge
+                            .get_documentation()
+                            .unwrap_or_default(),
+                    ),
+                },
+                self,
+            )),
             _ => Err(ValError::new(ErrorType::TimeType, self)),
         }
     }
 
     fn strict_datetime(&self) -> ValResult<EitherDateTime> {
         match self {
             JsonInput::String(v) => bytes_as_datetime(self, v.as_bytes()),
```

### Comparing `pydantic_core-2.1.3/src/input/input_python.rs` & `pydantic_core-2.2.0/src/input/input_python.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/input/mod.rs` & `pydantic_core-2.2.0/src/input/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/input/return_enums.rs` & `pydantic_core-2.2.0/src/input/return_enums.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use std::borrow::Cow;
 use std::cmp::Ordering;
 use std::ops::Rem;
 use std::slice::Iter as SliceIter;
+use std::str::FromStr;
 
 use num_bigint::BigInt;
 
 use pyo3::exceptions::PyTypeError;
 use pyo3::prelude::*;
 use pyo3::types::iter::PyDictIterator;
 use pyo3::types::{
@@ -13,14 +14,15 @@
 };
 use pyo3::{ffi, intern, AsPyPointer, PyNativeType};
 
 #[cfg(not(PyPy))]
 use pyo3::types::PyFunction;
 #[cfg(not(PyPy))]
 use pyo3::PyTypeInfo;
+use serde::{ser::Error, Serialize, Serializer};
 
 use crate::errors::{py_err_string, ErrorType, InputValue, ValError, ValLineError, ValResult};
 use crate::recursion_guard::RecursionGuard;
 use crate::tools::py_err;
 use crate::validators::{CombinedValidator, Extra, Validator};
 
 use super::parse_json::{JsonArray, JsonInput, JsonObject};
@@ -922,20 +924,34 @@
         match self {
             Self::F64(float) => float.into_py(py),
             Self::Py(float) => float.into_py(py),
         }
     }
 }
 
-#[derive(Debug, Clone)]
+#[derive(Debug, Clone, Serialize)]
+#[serde(untagged)]
 pub enum Int {
     I64(i64),
+    #[serde(serialize_with = "serialize_bigint_as_number")]
     Big(BigInt),
 }
 
+// The default serialization for BigInt is some internal representation which roundtrips efficiently
+// but is not the JSON value which users would expect to see.
+fn serialize_bigint_as_number<S>(big_int: &BigInt, serializer: S) -> Result<S::Ok, S::Error>
+where
+    S: Serializer,
+{
+    serde_json::Number::from_str(&big_int.to_string())
+        .map_err(S::Error::custom)
+        .expect("a valid number")
+        .serialize(serializer)
+}
+
 impl PartialOrd for Int {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
         match (self, other) {
             (Int::I64(i1), Int::I64(i2)) => Some(i1.cmp(i2)),
             (Int::Big(b1), Int::Big(b2)) => Some(b1.cmp(b2)),
             (Int::I64(i), Int::Big(b)) => Some(BigInt::from(*i).cmp(b)),
             (Int::Big(b), Int::I64(i)) => Some(b.cmp(&BigInt::from(*i))),
@@ -969,7 +985,16 @@
         } else if let Ok(b) = obj.extract::<BigInt>() {
             Ok(Int::Big(b))
         } else {
             py_err!(PyTypeError; "Expected int, got {}", obj.get_type())
         }
     }
 }
+
+impl ToPyObject for Int {
+    fn to_object(&self, py: Python<'_>) -> PyObject {
+        match self {
+            Self::I64(i) => i.to_object(py),
+            Self::Big(big_i) => big_i.to_object(py),
+        }
+    }
+}
```

### Comparing `pydantic_core-2.1.3/src/input/shared.rs` & `pydantic_core-2.2.0/src/input/shared.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/lazy_index_map.rs` & `pydantic_core-2.2.0/src/lazy_index_map.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/lib.rs` & `pydantic_core-2.2.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/lookup_key.rs` & `pydantic_core-2.2.0/src/lookup_key.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/recursion_guard.rs` & `pydantic_core-2.2.0/src/recursion_guard.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/computed_fields.rs` & `pydantic_core-2.2.0/src/serializers/computed_fields.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/config.rs` & `pydantic_core-2.2.0/src/serializers/config.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/errors.rs` & `pydantic_core-2.2.0/src/serializers/errors.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/extra.rs` & `pydantic_core-2.2.0/src/serializers/extra.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/fields.rs` & `pydantic_core-2.2.0/src/serializers/fields.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/filter.rs` & `pydantic_core-2.2.0/src/serializers/filter.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/infer.rs` & `pydantic_core-2.2.0/src/serializers/infer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 use pyo3::types::{
     PyByteArray, PyBytes, PyDate, PyDateTime, PyDelta, PyDict, PyFrozenSet, PyIterator, PyList, PySet, PyString,
     PyTime, PyTuple,
 };
 
 use serde::ser::{Error, Serialize, SerializeMap, SerializeSeq, Serializer};
 
+use crate::input::Int;
 use crate::serializers::errors::SERIALIZATION_ERR_MARKER;
 use crate::serializers::filter::SchemaFilter;
 use crate::serializers::shared::{PydanticSerializer, TypeSerializer};
 use crate::serializers::SchemaSerializer;
 use crate::tools::{extract_i64, py_err, safe_repr};
 use crate::url::{PyMultiHostUrl, PyUrl};
 
@@ -402,15 +403,15 @@
             }
             map.end()
         }};
     }
 
     let ser_result = match ob_type {
         ObType::None => serializer.serialize_none(),
-        ObType::Int | ObType::IntSubclass => serialize!(i64),
+        ObType::Int | ObType::IntSubclass => serialize!(Int),
         ObType::Bool => serialize!(bool),
         ObType::Float | ObType::FloatSubclass => serialize!(f64),
         ObType::Decimal => value.to_string().serialize(serializer),
         ObType::Str | ObType::StrSubclass => {
             let py_str: &PyString = value.downcast().map_err(py_err_se_err)?;
             super::type_serializers::string::serialize_py_str(py_str, serializer)
         }
```

### Comparing `pydantic_core-2.1.3/src/serializers/mod.rs` & `pydantic_core-2.2.0/src/serializers/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/ob_type.rs` & `pydantic_core-2.2.0/src/serializers/ob_type.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/shared.rs` & `pydantic_core-2.2.0/src/serializers/shared.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/any.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/any.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/bytes.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/bytes.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/dataclass.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/dataclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/datetime_etc.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/datetime_etc.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/definitions.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/dict.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/format.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/format.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/function.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/function.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/generator.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/generator.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/json.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/json_or_python.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/json_or_python.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/list.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/list.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/literal.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/literal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/mod.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/model.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/model.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/nullable.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/nullable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/other.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/other.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/set_frozenset.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/set_frozenset.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/simple.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/simple.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 use std::borrow::Cow;
 
 use serde::Serialize;
 
-use crate::definitions::DefinitionsBuilder;
+use crate::{definitions::DefinitionsBuilder, input::Int};
 
 use super::{
     infer_json_key, infer_serialize, infer_to_python, BuildSerializer, CombinedSerializer, Extra, IsType, ObType,
     SerMode, TypeSerializer,
 };
 
 #[derive(Debug, Clone)]
@@ -159,15 +159,15 @@
     };
 }
 
 pub(crate) fn to_str_json_key(key: &PyAny) -> PyResult<Cow<str>> {
     Ok(key.str()?.to_string_lossy())
 }
 
-build_simple_serializer!(IntSerializer, "int", i64, ObType::Int, to_str_json_key);
+build_simple_serializer!(IntSerializer, "int", Int, ObType::Int, to_str_json_key);
 
 pub(crate) fn bool_json_key(key: &PyAny) -> PyResult<Cow<str>> {
     let v = if key.is_true().unwrap_or(false) {
         "true"
     } else {
         "false"
     };
```

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/string.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/string.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/timedelta.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/timedelta.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/tuple.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/tuple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/typed_dict.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/typed_dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/union.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/union.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/url.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/serializers/type_serializers/with_default.rs` & `pydantic_core-2.2.0/src/serializers/type_serializers/with_default.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/tools.rs` & `pydantic_core-2.2.0/src/tools.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/url.rs` & `pydantic_core-2.2.0/src/url.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 use std::collections::hash_map::DefaultHasher;
+use std::fmt;
+use std::fmt::Formatter;
 use std::hash::{Hash, Hasher};
 
 use idna::punycode::decode_to_string;
+use pyo3::exceptions::PyValueError;
 use pyo3::once_cell::GILOnceCell;
-use pyo3::prelude::*;
 use pyo3::pyclass::CompareOp;
-use pyo3::types::PyDict;
+use pyo3::types::{PyDict, PyType};
+use pyo3::{intern, prelude::*};
 use url::Url;
 
+use crate::tools::SchemaDict;
 use crate::SchemaValidator;
 
 static SCHEMA_DEFINITION_URL: GILOnceCell<SchemaValidator> = GILOnceCell::new();
 
 #[pyclass(name = "Url", module = "pydantic_core._pydantic_core", subclass)]
 #[derive(Clone)]
 #[cfg_attr(debug_assertions, derive(Debug))]
@@ -146,14 +150,50 @@
     pub fn __deepcopy__(&self, py: Python, _memo: &PyDict) -> Py<PyAny> {
         self.clone().into_py(py)
     }
 
     fn __getnewargs__(&self) -> (&str,) {
         (self.__str__(),)
     }
+
+    #[classmethod]
+    #[pyo3(signature=(*, scheme, host, username=None, password=None, port=None, path=None, query=None, fragment=None))]
+    #[allow(clippy::too_many_arguments)]
+    pub fn build<'a>(
+        cls: &'a PyType,
+        scheme: &str,
+        host: &str,
+        username: Option<&str>,
+        password: Option<&str>,
+        port: Option<u16>,
+        path: Option<&str>,
+        query: Option<&str>,
+        fragment: Option<&str>,
+    ) -> PyResult<&'a PyAny> {
+        let url_host = UrlHostParts {
+            username: username.map(Into::into),
+            password: password.map(Into::into),
+            host: Some(host.into()),
+            port,
+        };
+        let mut url = format!("{scheme}://{url_host}");
+        if let Some(path) = path {
+            url.push('/');
+            url.push_str(path);
+        }
+        if let Some(query) = query {
+            url.push('?');
+            url.push_str(query);
+        }
+        if let Some(fragment) = fragment {
+            url.push('#');
+            url.push_str(fragment);
+        }
+        cls.call1((url,))
+    }
 }
 
 #[pyclass(name = "MultiHostUrl", module = "pydantic_core._pydantic_core", subclass)]
 #[derive(Clone)]
 #[cfg_attr(debug_assertions, derive(Debug))]
 pub struct PyMultiHostUrl {
     ref_url: PyUrl,
@@ -310,14 +350,122 @@
     pub fn __deepcopy__(&self, py: Python, _memo: &PyDict) -> Py<PyAny> {
         self.clone().into_py(py)
     }
 
     fn __getnewargs__(&self) -> (String,) {
         (self.__str__(),)
     }
+
+    #[classmethod]
+    #[pyo3(signature=(*, scheme, hosts=None, path=None, query=None, fragment=None, host=None, username=None, password=None, port=None))]
+    #[allow(clippy::too_many_arguments)]
+    pub fn build<'a>(
+        cls: &'a PyType,
+        scheme: &str,
+        hosts: Option<Vec<UrlHostParts>>,
+        path: Option<&str>,
+        query: Option<&str>,
+        fragment: Option<&str>,
+        // convenience parameters to build with a single host
+        host: Option<&str>,
+        username: Option<&str>,
+        password: Option<&str>,
+        port: Option<u16>,
+    ) -> PyResult<&'a PyAny> {
+        let mut url =
+            if hosts.is_some() && (host.is_some() || username.is_some() || password.is_some() || port.is_some()) {
+                return Err(PyValueError::new_err(
+                    "expected one of `hosts` or singular values to be set.",
+                ));
+            } else if let Some(hosts) = hosts {
+                // check all of host / user / password / port empty
+                // build multi-host url
+                let mut multi_url = format!("{scheme}://");
+                for (index, single_host) in hosts.iter().enumerate() {
+                    if single_host.is_empty() {
+                        return Err(PyValueError::new_err(
+                            "expected one of 'host', 'username', 'password' or 'port' to be set",
+                        ));
+                    }
+                    multi_url.push_str(&single_host.to_string());
+                    if index != hosts.len() - 1 {
+                        multi_url.push(',');
+                    };
+                }
+                multi_url
+            } else if host.is_some() {
+                let url_host = UrlHostParts {
+                    username: username.map(Into::into),
+                    password: password.map(Into::into),
+                    host: host.map(Into::into),
+                    port: port.map(Into::into),
+                };
+                format!("{scheme}://{url_host}")
+            } else {
+                return Err(PyValueError::new_err("expected either `host` or `hosts` to be set"));
+            };
+
+        if let Some(path) = path {
+            url.push('/');
+            url.push_str(path);
+        }
+        if let Some(query) = query {
+            url.push('?');
+            url.push_str(query);
+        }
+        if let Some(fragment) = fragment {
+            url.push('#');
+            url.push_str(fragment);
+        }
+        cls.call1((url,))
+    }
+}
+
+pub struct UrlHostParts {
+    username: Option<String>,
+    password: Option<String>,
+    host: Option<String>,
+    port: Option<u16>,
+}
+
+impl UrlHostParts {
+    fn is_empty(&self) -> bool {
+        self.host.is_none() && self.password.is_none() && self.host.is_none() && self.port.is_none()
+    }
+}
+
+impl FromPyObject<'_> for UrlHostParts {
+    fn extract(ob: &'_ PyAny) -> PyResult<Self> {
+        let py = ob.py();
+        let dict = ob.downcast::<PyDict>()?;
+        Ok(UrlHostParts {
+            username: dict.get_as(intern!(py, "username"))?,
+            password: dict.get_as(intern!(py, "password"))?,
+            host: dict.get_as(intern!(py, "host"))?,
+            port: dict.get_as(intern!(py, "port"))?,
+        })
+    }
+}
+
+impl fmt::Display for UrlHostParts {
+    fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
+        match (&self.username, &self.password) {
+            (Some(username), None) => write!(f, "{username}@")?,
+            (None, Some(password)) => write!(f, ":{password}@")?,
+            (Some(username), Some(password)) => write!(f, "{username}:{password}@")?,
+            (None, None) => {}
+        };
+        if let Some(host) = &self.host {
+            write!(f, "{host}")?;
+        }
+        if let Some(port) = self.port {
+            write!(f, ":{port}")?;
+        }
+        Ok(())
+    }
 }
 
 fn host_to_dict<'a>(py: Python<'a>, lib_url: &Url) -> PyResult<&'a PyDict> {
     let dict = PyDict::new(py);
     dict.set_item(
         "username",
         match lib_url.username() {
```

### Comparing `pydantic_core-2.1.3/src/validators/any.rs` & `pydantic_core-2.2.0/src/validators/any.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/arguments.rs` & `pydantic_core-2.2.0/src/validators/arguments.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/bool.rs` & `pydantic_core-2.2.0/src/validators/bool.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/bytes.rs` & `pydantic_core-2.2.0/src/validators/bytes.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/call.rs` & `pydantic_core-2.2.0/src/validators/call.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/callable.rs` & `pydantic_core-2.2.0/src/validators/callable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/chain.rs` & `pydantic_core-2.2.0/src/validators/chain.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/custom_error.rs` & `pydantic_core-2.2.0/src/validators/custom_error.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/dataclass.rs` & `pydantic_core-2.2.0/src/validators/dataclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/date.rs` & `pydantic_core-2.2.0/src/validators/date.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/datetime.rs` & `pydantic_core-2.2.0/src/validators/datetime.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/definitions.rs` & `pydantic_core-2.2.0/src/validators/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/dict.rs` & `pydantic_core-2.2.0/src/validators/dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/float.rs` & `pydantic_core-2.2.0/src/validators/float.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/frozenset.rs` & `pydantic_core-2.2.0/src/validators/frozenset.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/function.rs` & `pydantic_core-2.2.0/src/validators/function.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/generator.rs` & `pydantic_core-2.2.0/src/validators/generator.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/int.rs` & `pydantic_core-2.2.0/src/validators/int.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/is_instance.rs` & `pydantic_core-2.2.0/src/validators/is_instance.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/is_subclass.rs` & `pydantic_core-2.2.0/src/validators/is_subclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/json.rs` & `pydantic_core-2.2.0/src/validators/json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/json_or_python.rs` & `pydantic_core-2.2.0/src/validators/json_or_python.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/lax_or_strict.rs` & `pydantic_core-2.2.0/src/validators/lax_or_strict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/list.rs` & `pydantic_core-2.2.0/src/validators/list.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/literal.rs` & `pydantic_core-2.2.0/src/validators/literal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/mod.rs` & `pydantic_core-2.2.0/src/validators/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/model.rs` & `pydantic_core-2.2.0/src/validators/model.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/model_fields.rs` & `pydantic_core-2.2.0/src/validators/model_fields.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/none.rs` & `pydantic_core-2.2.0/src/validators/none.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/nullable.rs` & `pydantic_core-2.2.0/src/validators/nullable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/set.rs` & `pydantic_core-2.2.0/src/validators/set.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/string.rs` & `pydantic_core-2.2.0/src/validators/string.rs`

 * *Files 6% similar despite different names*

```diff
@@ -89,25 +89,31 @@
     ) -> ValResult<'data, PyObject> {
         let either_str = input.validate_str(extra.strict.unwrap_or(self.strict))?;
         let cow = either_str.as_cow()?;
         let mut str = cow.as_ref();
         if self.strip_whitespace {
             str = str.trim();
         }
+
+        let str_len: Option<usize> = if self.min_length.is_some() | self.max_length.is_some() {
+            Some(str.chars().count())
+        } else {
+            None
+        };
         if let Some(min_length) = self.min_length {
-            if str.len() < min_length {
-                // return py_schema_err!("{} is shorter than {}", str, min_length);
+            if str_len.unwrap() < min_length {
                 return Err(ValError::new(ErrorType::StringTooShort { min_length }, input));
             }
         }
         if let Some(max_length) = self.max_length {
-            if str.len() > max_length {
+            if str_len.unwrap() > max_length {
                 return Err(ValError::new(ErrorType::StringTooLong { max_length }, input));
             }
         }
+
         if let Some(pattern) = &self.pattern {
             if !pattern.is_match(str) {
                 return Err(ValError::new(
                     ErrorType::StringPatternMismatch {
                         pattern: pattern.to_string(),
                     },
                     input,
```

### Comparing `pydantic_core-2.1.3/src/validators/time.rs` & `pydantic_core-2.2.0/src/validators/time.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/timedelta.rs` & `pydantic_core-2.2.0/src/validators/timedelta.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/tuple.rs` & `pydantic_core-2.2.0/src/validators/tuple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/typed_dict.rs` & `pydantic_core-2.2.0/src/validators/typed_dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/union.rs` & `pydantic_core-2.2.0/src/validators/union.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/url.rs` & `pydantic_core-2.2.0/src/validators/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/src/validators/with_default.rs` & `pydantic_core-2.2.0/src/validators/with_default.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/benchmarks/complete_schema.py` & `pydantic_core-2.2.0/tests/benchmarks/complete_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/benchmarks/test_complete_benchmark.py` & `pydantic_core-2.2.0/tests/benchmarks/test_complete_benchmark.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/benchmarks/test_micro_benchmarks.py` & `pydantic_core-2.2.0/tests/benchmarks/test_micro_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/benchmarks/test_serialization_micro.py` & `pydantic_core-2.2.0/tests/benchmarks/test_serialization_micro.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/conftest.py` & `pydantic_core-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/emscripten_runner.js` & `pydantic_core-2.2.0/tests/emscripten_runner.js`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_any.py` & `pydantic_core-2.2.0/tests/serializers/test_any.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_bytes.py` & `pydantic_core-2.2.0/tests/serializers/test_bytes.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_dataclasses.py` & `pydantic_core-2.2.0/tests/serializers/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_datetime.py` & `pydantic_core-2.2.0/tests/serializers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_definitions.py` & `pydantic_core-2.2.0/tests/serializers/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_definitions_recursive.py` & `pydantic_core-2.2.0/tests/serializers/test_definitions_recursive.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_dict.py` & `pydantic_core-2.2.0/tests/serializers/test_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_format.py` & `pydantic_core-2.2.0/tests/serializers/test_format.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_functions.py` & `pydantic_core-2.2.0/tests/serializers/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_generator.py` & `pydantic_core-2.2.0/tests/serializers/test_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_json.py` & `pydantic_core-2.2.0/tests/serializers/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_json_or_python.py` & `pydantic_core-2.2.0/tests/serializers/test_json_or_python.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_list_tuple.py` & `pydantic_core-2.2.0/tests/serializers/test_list_tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_literal.py` & `pydantic_core-2.2.0/tests/serializers/test_literal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_misc.py` & `pydantic_core-2.2.0/tests/serializers/test_misc.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_model.py` & `pydantic_core-2.2.0/tests/serializers/test_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_model_root.py` & `pydantic_core-2.2.0/tests/serializers/test_model_root.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_none.py` & `pydantic_core-2.2.0/tests/serializers/test_none.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_nullable.py` & `pydantic_core-2.2.0/tests/serializers/test_nullable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_other.py` & `pydantic_core-2.2.0/tests/serializers/test_other.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_set_frozenset.py` & `pydantic_core-2.2.0/tests/serializers/test_set_frozenset.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_simple.py` & `pydantic_core-2.2.0/tests/serializers/test_simple.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,19 +15,24 @@
     two = 2
 
 
 class FloatSubClass(float):
     pass
 
 
+# A number well outside of i64 range
+_BIG_NUMBER_BYTES = b'1' + (b'0' * 40)
+
+
 @pytest.mark.parametrize('custom_type_schema', [None, 'any'])
 @pytest.mark.parametrize(
     'schema_type,value,expected_python,expected_json',
     [
         ('int', 1, 1, b'1'),
+        ('int', int(_BIG_NUMBER_BYTES), int(_BIG_NUMBER_BYTES), _BIG_NUMBER_BYTES),
         ('bool', True, True, b'true'),
         ('bool', False, False, b'false'),
         ('float', 1.0, 1.0, b'1.0'),
         ('float', 42.31415, 42.31415, b'42.31415'),
         ('none', None, None, b'null'),
         ('int', IntSubClass(42), IntSubClass(42), b'42'),
         ('int', MyIntEnum.one, MyIntEnum.one, b'1'),
```

### Comparing `pydantic_core-2.1.3/tests/serializers/test_string.py` & `pydantic_core-2.2.0/tests/serializers/test_string.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_timedelta.py` & `pydantic_core-2.2.0/tests/serializers/test_timedelta.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_typed_dict.py` & `pydantic_core-2.2.0/tests/serializers/test_typed_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_union.py` & `pydantic_core-2.2.0/tests/serializers/test_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/serializers/test_url.py` & `pydantic_core-2.2.0/tests/serializers/test_url.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test.rs` & `pydantic_core-2.2.0/tests/test.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_build.py` & `pydantic_core-2.2.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_config.py` & `pydantic_core-2.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_docstrings.py` & `pydantic_core-2.2.0/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_errors.py` & `pydantic_core-2.2.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_garbage_collection.py` & `pydantic_core-2.2.0/tests/test_garbage_collection.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_hypothesis.py` & `pydantic_core-2.2.0/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_isinstance.py` & `pydantic_core-2.2.0/tests/test_isinstance.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_json.py` & `pydantic_core-2.2.0/tests/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,22 +59,28 @@
     assert s.validate_json('"foobar"') == b'foobar'
     with pytest.raises(ValidationError, match=r'Input should be a valid bytes \[type=bytes_type,'):
         s.validate_json('false')
     with pytest.raises(ValidationError, match=r'Input should be a valid bytes \[type=bytes_type,'):
         s.validate_json('123')
 
 
+# A number well outside of i64 range
+_BIG_NUMBER_STR = '1' + ('0' * 40)
+
+
 @pytest.mark.parametrize(
     'input_value,expected',
     [
         ('123', 123),
         ('"123"', 123),
         ('123.0', 123),
         ('"123.0"', 123),
+        (_BIG_NUMBER_STR, int(_BIG_NUMBER_STR)),
         ('123.4', Err('Input should be a valid integer, got a number with a fractional part [type=int_from_float,')),
+        ('"123.4"', Err('Input should be a valid integer, unable to parse string as an integer [type=int_parsing,')),
         ('"string"', Err('Input should be a valid integer, unable to parse string as an integer [type=int_parsing,')),
     ],
 )
 def test_int(input_value, expected):
     v = SchemaValidator({'type': 'int'})
     if isinstance(expected, Err):
         with pytest.raises(ValidationError, match=re.escape(expected.message)):
```

### Comparing `pydantic_core-2.1.3/tests/test_misc.py` & `pydantic_core-2.2.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_schema_functions.py` & `pydantic_core-2.2.0/tests/test_schema_functions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_strict.py` & `pydantic_core-2.2.0/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_typing.py` & `pydantic_core-2.2.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/test_validation_context.py` & `pydantic_core-2.2.0/tests/test_validation_context.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_arguments.py` & `pydantic_core-2.2.0/tests/validators/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_bool.py` & `pydantic_core-2.2.0/tests/validators/test_bool.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_bytes.py` & `pydantic_core-2.2.0/tests/validators/test_bytes.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_call.py` & `pydantic_core-2.2.0/tests/validators/test_call.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_callable.py` & `pydantic_core-2.2.0/tests/validators/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_chain.py` & `pydantic_core-2.2.0/tests/validators/test_chain.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_custom_error.py` & `pydantic_core-2.2.0/tests/validators/test_custom_error.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_dataclasses.py` & `pydantic_core-2.2.0/tests/validators/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_date.py` & `pydantic_core-2.2.0/tests/validators/test_date.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_datetime.py` & `pydantic_core-2.2.0/tests/validators/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_definitions.py` & `pydantic_core-2.2.0/tests/validators/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_definitions_recursive.py` & `pydantic_core-2.2.0/tests/validators/test_definitions_recursive.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_dict.py` & `pydantic_core-2.2.0/tests/validators/test_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_float.py` & `pydantic_core-2.2.0/tests/validators/test_float.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_frozenset.py` & `pydantic_core-2.2.0/tests/validators/test_frozenset.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_function.py` & `pydantic_core-2.2.0/tests/validators/test_function.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_generator.py` & `pydantic_core-2.2.0/tests/validators/test_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_int.py` & `pydantic_core-2.2.0/tests/validators/test_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,21 +158,15 @@
 @pytest.mark.parametrize(
     'input_value,expected',
     [
         (1, 1),
         (i64_max, i64_max),
         (i64_max + 1, i64_max + 1),
         (i64_max * 2, i64_max * 2),
-        (
-            int(1e30),
-            Err(
-                'Unable to parse input string as an integer, exceeded maximum size '
-                '[type=int_parsing_size, input_value=1e+30, input_type=float]'
-            ),
-        ),
+        (int(1e30), int(1e30)),
         (0, Err('Input should be greater than 0 [type=greater_than, input_value=0, input_type=int]')),
         (-1, Err('Input should be greater than 0 [type=greater_than, input_value=-1, input_type=int]')),
         pytest.param(
             [1, 2],
             Err('Input should be a valid integer [type=int_type, input_value=[1, 2], input_type=list]'),
             id='list',
         ),
@@ -193,18 +187,15 @@
 @pytest.mark.parametrize(
     'input_value,expected',
     [
         (-1, -1),
         (0, Err('Input should be less than 0 [type=less_than, input_value=0, input_type=int]')),
         (-i64_max, -i64_max),
         (-i64_max - 1, -i64_max - 1),
-        (
-            -i64_max * 2,
-            Err(' Unable to parse input string as an integer, exceeded maximum size [type=int_parsing_size'),
-        ),
+        (-i64_max * 2, -i64_max * 2),
     ],
 )
 def test_negative_json(input_value, expected):
     v = SchemaValidator({'type': 'int', 'lt': 0})
     json_input = json.dumps(input_value)
     if isinstance(expected, Err):
         with pytest.raises(ValidationError, match=re.escape(expected.message)):
@@ -387,16 +378,15 @@
     with pytest.raises(ValidationError, match='Input should be less than 1'):
         v.validate_python(s)
 
 
 def test_long_json():
     v = SchemaValidator({'type': 'int'})
 
-    with pytest.raises(ValidationError, match=r'number out of range at line 1 column 401 \[type=json_invalid,'):
-        v.validate_json('-' + '1' * 400)
+    assert v.validate_json('-' + '1' * 400) == int('-' + '1' * 400)
 
     with pytest.raises(ValidationError, match=r'expected ident at line 1 column 2 \[type=json_invalid,'):
         v.validate_json('nan')
 
 
 def test_int_key(py_and_json: PyAndJson):
     v = py_and_json({'type': 'dict', 'keys_schema': {'type': 'int'}, 'values_schema': {'type': 'int'}})
```

### Comparing `pydantic_core-2.1.3/tests/validators/test_is_instance.py` & `pydantic_core-2.2.0/tests/validators/test_is_instance.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_is_subclass.py` & `pydantic_core-2.2.0/tests/validators/test_is_subclass.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_json.py` & `pydantic_core-2.2.0/tests/validators/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_json_or_python.py` & `pydantic_core-2.2.0/tests/validators/test_json_or_python.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_lax_or_strict.py` & `pydantic_core-2.2.0/tests/validators/test_lax_or_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_list.py` & `pydantic_core-2.2.0/tests/validators/test_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_literal.py` & `pydantic_core-2.2.0/tests/validators/test_literal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_model.py` & `pydantic_core-2.2.0/tests/validators/test_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_model_fields.py` & `pydantic_core-2.2.0/tests/validators/test_model_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_model_init.py` & `pydantic_core-2.2.0/tests/validators/test_model_init.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_model_root.py` & `pydantic_core-2.2.0/tests/validators/test_model_root.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_none.py` & `pydantic_core-2.2.0/tests/validators/test_none.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_nullable.py` & `pydantic_core-2.2.0/tests/validators/test_nullable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_set.py` & `pydantic_core-2.2.0/tests/validators/test_set.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_string.py` & `pydantic_core-2.2.0/tests/validators/test_string.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from decimal import Decimal
-from typing import Any, Dict
+from typing import Any, Dict, Union
 
 import pytest
 
 from pydantic_core import SchemaError, SchemaValidator, ValidationError, core_schema
 
 from ..conftest import Err, PyAndJson, plain_repr
 
@@ -130,20 +130,36 @@
             'loc': (),
             'msg': 'Input should be a valid string, unable to parse raw data as a unicode string',
             'input': '🐈 Hello \ud800World',
         }
     ]
 
 
-def test_str_constrained():
-    v = SchemaValidator({'type': 'str', 'max_length': 5})
-    assert v.validate_python('test') == 'test'
-
-    with pytest.raises(ValidationError, match='String should have at most 5 characters'):
-        v.validate_python('test long')
+@pytest.mark.parametrize(
+    ('data', 'max_length', 'error'),
+    [
+        pytest.param('test', 5, None, id='short string'),
+        pytest.param('test long', 5, 'String should have at most 5 characters', id='long string'),
+        pytest.param('␛⯋℃▤', 5, None, id='short string with unicode characters'),
+        pytest.param(
+            '␛⯋℃▤⩥⠫⳼⣪⨺✒⧐♳⩚⏭⏣⍥┙⧃Ⰴ┽⏏♜',
+            5,
+            'String should have at most 5 characters',
+            id='long string with unicode characters',
+        ),
+        pytest.param('а' * 25, 32, None, id='a lot of `а`s'),
+    ],
+)
+def test_str_constrained(data: str, max_length: int, error: Union[re.Pattern, None]):
+    v = SchemaValidator({'type': 'str', 'max_length': max_length})
+    if error is None:
+        assert v.validate_python(data) == data
+    else:
+        with pytest.raises(ValidationError, match=error):
+            v.validate_python(data)
 
 
 def test_str_constrained_config():
     v = SchemaValidator({'type': 'str'}, {'str_max_length': 5})
     assert v.validate_python('test') == 'test'
 
     with pytest.raises(ValidationError, match='String should have at most 5 characters'):
```

### Comparing `pydantic_core-2.1.3/tests/validators/test_tagged_union.py` & `pydantic_core-2.2.0/tests/validators/test_tagged_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_time.py` & `pydantic_core-2.2.0/tests/validators/test_time.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_timedelta.py` & `pydantic_core-2.2.0/tests/validators/test_timedelta.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_tuple.py` & `pydantic_core-2.2.0/tests/validators/test_tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_typed_dict.py` & `pydantic_core-2.2.0/tests/validators/test_typed_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_union.py` & `pydantic_core-2.2.0/tests/validators/test_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/tests/validators/test_url.py` & `pydantic_core-2.2.0/tests/validators/test_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1212,7 +1212,90 @@
 
     data[Url('http://example.com')] = 3
     assert data == {Url('http://example.com/'): 3, Url('http://example.com/123'): 2}
 
 
 def test_url_deepcopy() -> None:
     assert deepcopy(Url('http://example.com')) == Url('http://example.com/')
+
+
+def test_multi_url_build() -> None:
+    url = MultiHostUrl.build(
+        scheme='postgresql',
+        username='testuser',
+        password='testpassword',
+        host='127.0.0.1',
+        port=5432,
+        path='database',
+        query='sslmode=require',
+        fragment='test',
+    )
+    assert url == MultiHostUrl('postgresql://testuser:testpassword@127.0.0.1:5432/database?sslmode=require#test')
+    assert str(url) == 'postgresql://testuser:testpassword@127.0.0.1:5432/database?sslmode=require#test'
+
+
+@pytest.mark.parametrize('field', ['host', 'password', 'username', 'port'])
+def test_multi_url_build_hosts_set_with_single_value(field) -> None:
+    """Hosts can't be provided with any single url values."""
+    hosts = [
+        {'host': '127.0.0.1', 'password': 'testpassword', 'username': 'testuser', 'port': 5432},
+        {'host': '127.0.0.1', 'password': 'testpassword', 'username': 'testuser', 'port': 5432},
+    ]
+    kwargs = dict(scheme='postgresql', hosts=hosts, path='database', query='sslmode=require', fragment='test')
+    if field == 'port':
+        kwargs[field] = 5432
+    else:
+        kwargs[field] = 'test'
+    with pytest.raises(ValueError):
+        MultiHostUrl.build(**kwargs)
+
+
+def test_multi_url_build_hosts_empty_host() -> None:
+    """Hosts can't be provided with any single url values."""
+    hosts = [{}]
+    with pytest.raises(ValueError):
+        MultiHostUrl.build(scheme='postgresql', hosts=hosts, path='database', query='sslmode=require', fragment='test')
+
+
+def test_multi_url_build_hosts() -> None:
+    """Hosts can't be provided with any single url values."""
+    hosts = [
+        {'host': '127.0.0.1', 'password': 'testpassword', 'username': 'testuser', 'port': 5431},
+        {'host': '127.0.0.1', 'password': 'testpassword', 'username': 'testuser', 'port': 5433},
+    ]
+    kwargs = dict(scheme='postgresql', hosts=hosts, path='database', query='sslmode=require', fragment='test')
+    url = MultiHostUrl.build(**kwargs)
+    assert url == MultiHostUrl(
+        'postgresql://testuser:testpassword@127.0.0.1:5431,testuser:testpassword@127.0.0.1:5433/database?sslmode=require#test'
+    )
+    assert (
+        str(url)
+        == 'postgresql://testuser:testpassword@127.0.0.1:5431,testuser:testpassword@127.0.0.1:5433/database?sslmode=require#test'
+    )
+
+
+def test_multi_url_build_neither_host_and_hosts_set() -> None:
+    with pytest.raises(ValueError):
+        MultiHostUrl.build(
+            scheme='postgresql',
+            username='testuser',
+            password='testpassword',
+            port=5432,
+            path='database',
+            query='sslmode=require',
+            fragment='test',
+        )
+
+
+def test_url_build() -> None:
+    url = Url.build(
+        scheme='postgresql',
+        username='testuser',
+        password='testpassword',
+        host='127.0.0.1',
+        port=5432,
+        path='database',
+        query='sslmode=require',
+        fragment='test',
+    )
+    assert url == Url('postgresql://testuser:testpassword@127.0.0.1:5432/database?sslmode=require#test')
+    assert str(url) == 'postgresql://testuser:testpassword@127.0.0.1:5432/database?sslmode=require#test'
```

### Comparing `pydantic_core-2.1.3/tests/validators/test_with_default.py` & `pydantic_core-2.2.0/tests/validators/test_with_default.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/Cargo.lock` & `pydantic_core-2.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pydantic-core"
-version = "2.1.3"
+version = "2.2.0"
 dependencies = [
  "ahash",
  "base64",
  "enum_dispatch",
  "idna",
  "mimalloc",
  "num-bigint",
@@ -401,14 +401,28 @@
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
 version = "1.0.159"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+dependencies = [
+ "serde_derive",
+]
+
+[[package]]
+name = "serde_derive"
+version = "1.0.159"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
 
 [[package]]
 name = "serde_json"
 version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
 dependencies = [
```

### Comparing `pydantic_core-2.1.3/python/pydantic_core/_pydantic_core.pyi` & `pydantic_core-2.2.0/python/pydantic_core/_pydantic_core.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import decimal
 import sys
-from typing import Any, Callable, Generic, Type, TypeVar
+from typing import Any, Callable, Generic, Optional, Type, TypeVar
 
 from pydantic_core import ErrorDetails, ErrorTypeInfo, InitErrorDetails, MultiHostHost
 from pydantic_core.core_schema import CoreConfig, CoreSchema, ErrorType
 
 if sys.version_info < (3, 8):
     from typing_extensions import final
 else:
@@ -187,14 +187,27 @@
     def fragment(self) -> str | None: ...
     def unicode_host(self) -> str | None: ...
     def query_params(self) -> list[tuple[str, str]]: ...
     def unicode_string(self) -> str: ...
     def __repr__(self) -> str: ...
     def __str__(self) -> str: ...
     def __deepcopy__(self, memo: dict) -> str: ...
+    @classmethod
+    def build(
+        cls,
+        *,
+        scheme: str,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        host: str,
+        port: Optional[int] = None,
+        path: Optional[str] = None,
+        query: Optional[str] = None,
+        fragment: Optional[str] = None,
+    ) -> str: ...
 
 class MultiHostUrl(SupportsAllComparisons):
     def __new__(cls, url: str) -> Self: ...
     @property
     def scheme(self) -> str: ...
     @property
     def path(self) -> str | None: ...
@@ -204,14 +217,28 @@
     def fragment(self) -> str | None: ...
     def hosts(self) -> list[MultiHostHost]: ...
     def query_params(self) -> list[tuple[str, str]]: ...
     def unicode_string(self) -> str: ...
     def __repr__(self) -> str: ...
     def __str__(self) -> str: ...
     def __deepcopy__(self, memo: dict) -> Self: ...
+    @classmethod
+    def build(
+        cls,
+        *,
+        scheme: str,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        host: Optional[str] = None,
+        hosts: Optional[list[MultiHostHost]] = None,
+        port: Optional[int] = None,
+        path: Optional[str] = None,
+        query: Optional[str] = None,
+        fragment: Optional[str] = None,
+    ) -> str: ...
 
 @final
 class SchemaError(Exception):
     def error_count(self) -> int: ...
     def errors(self) -> list[ErrorDetails]: ...
 
 @final
```

### Comparing `pydantic_core-2.1.3/python/pydantic_core/core_schema.py` & `pydantic_core-2.2.0/python/pydantic_core/core_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/python/pydantic_core/__init__.py` & `pydantic_core-2.2.0/python/pydantic_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.1.3/PKG-INFO` & `pydantic_core-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_core
-Version: 2.1.3
+Version: 2.2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

