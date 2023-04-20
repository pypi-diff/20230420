# Comparing `tmp/pydantic-2.0a2.tar.gz` & `tmp/pydantic-2.0a3.tar.gz`

## Comparing `pydantic-2.0a2.tar` & `pydantic-2.0a3.tar`

### file list

```diff
@@ -1,165 +1,187 @@
--rw-r--r--   0        0        0    79249 2020-02-02 00:00:00.000000 pydantic-2.0a2/HISTORY.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 pydantic-2.0a2/Makefile
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydantic-2.0a2/README.md
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/__init__.py
--rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_hypothesis_plugin.py
--rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/analyzed_type.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/annotated_arguments.py
--rw-r--r--   0        0        0    21194 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/color.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/config.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/dataclasses.py
--rw-r--r--   0        0        0    10239 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/decorator.py
--rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/decorators.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/errors.py
--rw-r--r--   0        0        0    22697 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/fields.py
--rw-r--r--   0        0        0    56158 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/json_schema.py
--rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/main.py
--rw-r--r--   0        0        0    38032 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/mypy.py
--rw-r--r--   0        0        0    10041 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/networks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/py.typed
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/tools.py
--rw-r--r--   0        0        0    27028 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/types.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    23749 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0    21314 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0    54529 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    19390 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_serializers.py
--rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    16243 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0    16778 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/README.md
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/all.in
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/all.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/docs-constrained.in
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/docs.in
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/docs.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/linting-constrained.in
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/linting.in
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/linting.txt
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/pyproject-all.txt
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/pyproject-min.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/pyproject.toml-constrained.in
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/pyproject.toml-extras-constrained.in
--rwxr-xr-x   0        0        0      374 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/rebuild.sh
--rwxr-xr-x   0        0        0     1327 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/refresh.sh
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-constrained.in
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-extra-constrained.in
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-extra.in
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-extra.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-mypy-constrained.in
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-mypy.in
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-mypy.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing.in
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/conftest.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_abc.py
--rw-r--r--   0        0        0    12622 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_aliases.py
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_annotated.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_assert_in_validators.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_callable.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_color.py
--rw-r--r--   0        0        0    18778 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_config.py
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_construction.py
--rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_create_model.py
--rw-r--r--   0        0        0    43910 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_dataclasses.py
--rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_datetime.py
--rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_decorator.py
--rw-r--r--   0        0        0    15412 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_deprecated.py
--rw-r--r--   0        0        0    40131 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_discriminated_union.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_docs.py
--rw-r--r--   0        0        0    70040 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_edge_cases.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_errors.py
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_fastapi.sh
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_fastapi_json_schema.py
--rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_forward_ref.py
--rw-r--r--   0        0        0    62435 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_generics.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_hypothesis_plugin.py
--rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_json.py
--rw-r--r--   0        0        0   107645 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_json_schema.py
--rw-r--r--   0        0        0    61586 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_main.py
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_model_signature.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_model_validator.py
--rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_networks.py
--rw-r--r--   0        0        0    15512 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_networks_ipaddress.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_parse.py
--rw-r--r--   0        0        0     8552 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_private_attributes.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_rich_repr.py
--rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_serialize.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_strict.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_structural_pattern_matching.py
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_tools.py
--rw-r--r--   0        0        0   122508 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_types.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_types_namedtuple.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_types_payment_card_number.py
--rw-r--r--   0        0        0    19655 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_types_typeddict.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_typing.py
--rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_utils.py
--rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_validator.py
--rw-r--r--   0        0        0    66969 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_validators.py
--rwxr-xr-x   0        0        0     4663 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_validators_dataclass.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/__init__.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/test_mypy.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/mypy-plugin-strict-no-any.ini
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/mypy-plugin-strict.ini
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/mypy-plugin.ini
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/pyproject-default.toml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/pyproject-plugin-bad-param.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/pyproject-plugin-strict.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/pyproject-plugin.toml
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/custom_constructor.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/dataclass_no_any.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail1.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail2.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail3.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail4.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail_defaults.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_default_factory.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_fail.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_success.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/success.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/custom_constructor.txt
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail1.txt
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail2.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail3.txt
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail4.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail_defaults.txt
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-strict.txt
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-success-strict.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin_default_factory.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin_success.txt
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/v1.0.1/fail1.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/v1.0.1/fail2.txt
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/v1.0.1/plugin_success.txt
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/pyright/pyproject.toml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/pyright/pyright_example.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydantic-2.0a2/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.0a2/LICENSE
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 pydantic-2.0a2/pyproject.toml
--rw-r--r--   0        0        0   114550 2020-02-02 00:00:00.000000 pydantic-2.0a2/PKG-INFO
+-rw-r--r--   0        0        0    79396 2020-02-02 00:00:00.000000 pydantic-2.0a3/HISTORY.md
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pydantic-2.0a3/Makefile
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydantic-2.0a3/README.md
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/__init__.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_hypothesis_plugin.py
+-rw-r--r--   0        0        0    10119 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_migration.py
+-rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/analyzed_type.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/annotated_arguments.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21259 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/color.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/config.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/dataclasses.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/decorator.py
+-rw-r--r--   0        0        0    20748 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/decorators.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/env_settings.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/errors.py
+-rw-r--r--   0        0        0    33198 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/fields.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/generics.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/json.py
+-rw-r--r--   0        0        0    56048 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/json_schema.py
+-rw-r--r--   0        0        0    45064 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/main.py
+-rw-r--r--   0        0        0    38033 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/mypy.py
+-rw-r--r--   0        0        0    10106 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/networks.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/py.typed
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/schema.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/tools.py
+-rw-r--r--   0        0        0    27400 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/types.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/typing.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/utils.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/validate_call.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/validators.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    15745 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    19880 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    21314 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0     9365 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    60064 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    20567 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0    12565 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_serializers.py
+-rw-r--r--   0        0        0    16973 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    17278 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0    16973 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pydantic-2.0a3/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/README.md
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/all.in
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/all.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/docs-constrained.in
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/docs.in
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/docs.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/linting-constrained.in
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/linting.in
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/linting.txt
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/pyproject-all.txt
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/pyproject-min.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/pyproject.toml-constrained.in
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/pyproject.toml-extras-constrained.in
+-rwxr-xr-x   0        0        0      374 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/rebuild.sh
+-rwxr-xr-x   0        0        0     1327 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/refresh.sh
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/testing-constrained.in
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/testing-extra-constrained.in
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/testing-extra.in
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/testing-extra.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/testing-mypy-constrained.in
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/testing-mypy.in
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/testing-mypy.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/testing.in
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pydantic-2.0a3/requirements/testing.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/conftest.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_abc.py
+-rw-r--r--   0        0        0    14115 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_aliases.py
+-rw-r--r--   0        0        0     8764 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_annotated.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_assert_in_validators.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_callable.py
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_color.py
+-rw-r--r--   0        0        0    13553 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_computed_fields.py
+-rw-r--r--   0        0        0    17810 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_config.py
+-rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_construction.py
+-rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_create_model.py
+-rw-r--r--   0        0        0    49123 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_dataclasses.py
+-rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_datetime.py
+-rw-r--r--   0        0        0    21201 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_deprecated.py
+-rw-r--r--   0        0        0    12032 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_deprecated_validate_arguments.py
+-rw-r--r--   0        0        0    40302 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_discriminated_union.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_docs.py
+-rw-r--r--   0        0        0    72517 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_edge_cases.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_errors.py
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_fastapi.sh
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_fastapi_json_schema.py
+-rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_forward_ref.py
+-rw-r--r--   0        0        0    64920 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_generics.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_hypothesis_plugin.py
+-rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_json.py
+-rw-r--r--   0        0        0   107438 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_json_schema.py
+-rw-r--r--   0        0        0    61586 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_main.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_migration.py
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_model_signature.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_model_validator.py
+-rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_networks.py
+-rw-r--r--   0        0        0    15512 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_networks_ipaddress.py
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_parse.py
+-rw-r--r--   0        0        0     8953 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_private_attributes.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_rich_repr.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_serialize.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_strict.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_structural_pattern_matching.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_tools.py
+-rw-r--r--   0        0        0   129558 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_types.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_types_namedtuple.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_types_payment_card_number.py
+-rw-r--r--   0        0        0    19655 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_types_typeddict.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_typing.py
+-rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_utils.py
+-rw-r--r--   0        0        0    17324 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_validate_call.py
+-rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_validator.py
+-rw-r--r--   0        0        0    67125 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_validators.py
+-rwxr-xr-x   0        0        0     4622 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_validators_dataclass.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/__init__.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/test_mypy.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/configs/mypy-plugin-strict-no-any.ini
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/configs/mypy-plugin-strict.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/configs/mypy-plugin.ini
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/configs/pyproject-default.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/configs/pyproject-plugin-bad-param.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/configs/pyproject-plugin-strict.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/configs/pyproject-plugin.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/computed_fields.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/custom_constructor.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/dataclass_no_any.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/fail1.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/fail2.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/fail3.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/fail4.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/fail_defaults.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/plugin_default_factory.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/plugin_fail.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/plugin_success.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/modules/success.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/computed_fields.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/custom_constructor.txt
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/fail1.txt
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/fail2.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/fail3.txt
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/fail4.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/fail_defaults.txt
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/plugin-fail-strict.txt
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/plugin-fail.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/plugin-success-strict.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/plugin_default_factory.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/plugin_success.txt
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/v1.0.1/fail1.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/v1.0.1/fail2.txt
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/v1.0.1/plugin_success.txt
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/pyright/pyproject.toml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.0a3/tests/pyright/pyright_example.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydantic-2.0a3/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.0a3/LICENSE
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pydantic-2.0a3/pyproject.toml
+-rw-r--r--   0        0        0   114697 2020-02-02 00:00:00.000000 pydantic-2.0a3/PKG-INFO
```

### Comparing `pydantic-2.0a2/HISTORY.md` & `pydantic-2.0a3/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v2.0a3 (2023-04-20)
+
+Third pre-release of Pydantic V2
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0a3)
+
 ## v2.0a2 (2023-04-12)
 
 Second pre-release of Pydantic V2
 
 See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0a2)
 
 ## v2.0a1 (2023-04-03)
```

### Comparing `pydantic-2.0a2/Makefile` & `pydantic-2.0a3/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 	ruff --fix $(sources)
 
 .PHONY: lint
 lint:
 	ruff $(sources)
 	black $(sources) --check --diff
 
+.PHONY: codespell
+codespell:
+	pre-commit run codespell --all-files
+
 .PHONY: typecheck
 typecheck:
 	pre-commit run typecheck --all-files
 
 .PHONY: test-mypy
 test-mypy:
 	coverage run -m pytest tests/mypy --test-mypy
@@ -60,15 +64,15 @@
 
 .PHONY: test-fastapi
 test-fastapi:
 	git clone https://github.com/tiangolo/fastapi.git --single-branch
 	./tests/test_fastapi.sh
 
 .PHONY: all
-all: lint typecheck testcov
+all: lint typecheck codespell testcov
 
 .PHONY: clean
 clean:
 	rm -rf `find . -name __pycache__`
 	rm -f `find . -type f -name '*.py[co]'`
 	rm -f `find . -type f -name '*~'`
 	rm -f `find . -type f -name '.*~'`
```

### Comparing `pydantic-2.0a2/README.md` & `pydantic-2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/pydantic/__init__.py` & `pydantic-2.0a3/pydantic/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,25 +5,26 @@
     SerializationInfo,
     SerializerFunctionWrapHandler,
     ValidationInfo,
     ValidatorFunctionWrapHandler,
 )
 
 from . import dataclasses
+from ._migration import getattr_migration
 from .analyzed_type import AnalyzedType
 from .config import ConfigDict, Extra
-from .decorator import validate_arguments
 from .decorators import field_serializer, field_validator, model_serializer, root_validator, validator
 from .deprecated.config import BaseConfig
+from .deprecated.tools import *
 from .errors import *
-from .fields import Field, PrivateAttr
+from .fields import AliasChoices, AliasPath, Field, PrivateAttr, computed_field
 from .main import *
 from .networks import *
-from .tools import *
 from .types import *
+from .validate_call import validate_call
 from .version import VERSION
 
 __version__ = VERSION
 
 # WARNING __all__ from .errors is not included here, it will be removed as an export here in v2
 # please use "from pydantic.errors import ..." instead
 __all__ = [
@@ -42,23 +43,27 @@
     'FieldSerializationInfo',
     'ValidatorFunctionWrapHandler',
     'SerializerFunctionWrapHandler',
     # config
     'BaseConfig',
     'ConfigDict',
     'Extra',
-    # decorator
-    'validate_arguments',
+    # validate_call
+    'validate_call',
     # error_wrappers
     'ValidationError',
     'PydanticUserError',
     'PydanticSchemaGenerationError',
+    'PydanticImportError',
     'PydanticUndefinedAnnotation',
     # fields
+    'AliasPath',
+    'AliasChoices',
     'Field',
+    'computed_field',
     # main
     'BaseModel',
     'create_model',
     # network
     'AnyUrl',
     'AnyHttpUrl',
     'FileUrl',
@@ -125,7 +130,10 @@
     'PastDate',
     'FutureDate',
     'AwareDatetime',
     'NaiveDatetime',
     # version
     'VERSION',
 ]
+
+
+__getattr__ = getattr_migration(__name__)
```

### Comparing `pydantic-2.0a2/pydantic/_hypothesis_plugin.py` & `pydantic-2.0a3/pydantic/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/pydantic/analyzed_type.py` & `pydantic-2.0a3/pydantic/analyzed_type.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/pydantic/color.py` & `pydantic-2.0a3/pydantic/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 In these cases the _last_ color when sorted alphabetically takes preferences,
 eg. `Color((0, 255, 255)).as_named() == 'cyan'` because "cyan" comes after "aqua".
 """
 import math
 import re
 from colorsys import hls_to_rgb, rgb_to_hls
-from typing import Any, Dict, Optional, Tuple, Union, cast
+from typing import Any, Callable, Dict, Optional, Tuple, Type, Union, cast
 
-from pydantic_core import PydanticCustomError, core_schema
+from pydantic_core import CoreSchema, PydanticCustomError, core_schema
 
 from ._internal import _repr, _utils
 
 ColorTuple = Union[Tuple[int, int, int], Tuple[int, int, int, float]]
 ColorType = Union[ColorTuple, str]
 HslColorTuple = Union[Tuple[float, float, float], Tuple[float, float, float, float]]
 
@@ -221,15 +221,17 @@
             # alpha is False
             return h, s, l
 
     def _alpha_float(self) -> float:
         return 1 if self._rgba.alpha is None else self._rgba.alpha
 
     @classmethod
-    def __get_pydantic_core_schema__(cls, **_kwargs: Any) -> core_schema.PlainValidatorFunctionSchema:
+    def __get_pydantic_core_schema__(
+        cls, source: Type[Any], handler: Callable[[Any], CoreSchema]
+    ) -> core_schema.CoreSchema:
         return core_schema.general_plain_validator_function(
             cls._validate, serialization=core_schema.to_string_ser_schema()
         )
 
     @classmethod
     def _validate(cls, __input_value: Any, _: Any) -> 'Color':
         return cls(__input_value)
```

### Comparing `pydantic-2.0a2/pydantic/config.py` & `pydantic-2.0a3/pydantic/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 from __future__ import annotations as _annotations
 
 from typing import Any, Callable
 from warnings import warn
 
 from typing_extensions import Literal, TypedDict
 
-__all__ = 'ConfigDict', 'Extra'
+from ._migration import getattr_migration
+from .deprecated.config import BaseConfig
+
+__all__ = 'BaseConfig', 'ConfigDict', 'Extra'
 
 
 class _Extra:
     allow: Literal['allow'] = 'allow'
     ignore: Literal['ignore'] = 'ignore'
     forbid: Literal['forbid'] = 'forbid'
 
     def __getattribute__(self, __name: str) -> Any:
         warn(
             '`pydantic.config.Extra` is deprecated, use literal values instead' " (e.g. `extra='allow'`)",
             DeprecationWarning,
+            stacklevel=2,
         )
         return super().__getattribute__(__name)
 
 
 Extra = _Extra()
 
 ExtraValues = Literal['allow', 'ignore', 'forbid']
@@ -83,7 +87,12 @@
     strict: bool
     # whether instances of models and dataclasses (including subclass instances) should re-validate, default 'never'
     revalidate_instances: Literal['always', 'never', 'subclass-instances']
     ser_json_timedelta: Literal['iso8601', 'float']
     ser_json_bytes: Literal['utf8', 'base64']
     # whether to validate default values during validation, default False
     validate_default: bool
+    # whether to validate the return value from call validator
+    validate_return: bool
+
+
+__getattr__ = getattr_migration(__name__)
```

### Comparing `pydantic-2.0a2/pydantic/decorator.py` & `pydantic-2.0a3/pydantic/deprecated/decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-"""
-TODO this should be removed when we implement `validate` #4669
-"""
+import warnings
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Mapping, Optional, Tuple, Type, TypeVar, Union, overload
 
-from ._internal import _config, _typing_extra, _utils
-from .decorators import field_validator
-from .errors import PydanticUserError
-from .main import BaseModel, create_model
+from typing_extensions import deprecated
+
+from .._internal import _config, _typing_extra, _utils
+from ..decorators import field_validator
+from ..errors import PydanticUserError
+from ..main import BaseModel, create_model
 
 __all__ = ('validate_arguments',)
 
 if TYPE_CHECKING:
     AnyCallable = Callable[..., Any]
 
     AnyCallableT = TypeVar('AnyCallableT', bound=AnyCallable)
     ConfigType = Union[None, Type[Any], Dict[str, Any]]
 
 
 @overload
+@deprecated('The `validate_arguments` method is deprecated; use `validate_call` instead.')
 def validate_arguments(func: None = None, *, config: 'ConfigType' = None) -> Callable[['AnyCallableT'], 'AnyCallableT']:
     ...
 
 
 @overload
+@deprecated('The `validate_arguments` method is deprecated; use `validate_call` instead.')
 def validate_arguments(func: 'AnyCallableT') -> 'AnyCallableT':
     ...
 
 
 def validate_arguments(func: Optional['AnyCallableT'] = None, *, config: 'ConfigType' = None) -> Any:
     """
     Decorator to validate the arguments passed to a function.
     """
+    warnings.warn(
+        'The `validate_arguments` method is deprecated; use `validate_call` instead.', DeprecationWarning, stacklevel=2
+    )
 
     def validate(_func: 'AnyCallable') -> 'AnyCallable':
         vd = ValidatedFunction(_func, config)
 
         @wraps(_func)
         def wrapper_function(*args: Any, **kwargs: Any) -> Any:
             return vd.call(*args, **kwargs)
```

### Comparing `pydantic-2.0a2/pydantic/decorators.py` & `pydantic-2.0a3/pydantic/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,123 +1,117 @@
 """
-Public methods related to:
-
-* `validator` - a decorator to add validation to a field on a model
-* `root_validator` - a decorator to add validation to a model as a whole
-* `serializer` - a decorator to add serialization to a field on a model
+Public methods used as decorators within pydantic models and dataclasses
 """
 
 from __future__ import annotations as _annotations
 
 from functools import partial, partialmethod
 from types import FunctionType
-from typing import Any, Callable, TypeVar, Union, overload
+from typing import TYPE_CHECKING, Any, Callable, TypeVar, Union, overload
 from warnings import warn
 
 from pydantic_core import core_schema as _core_schema
 from typing_extensions import Literal, Protocol, TypeAlias
 
-from ._internal import _decorators
+from ._internal import _decorators, _decorators_v1
 from .errors import PydanticUserError
 
 _ALLOW_REUSE_WARNING_MESSAGE = '`allow_reuse` is deprecated and will be ignored; it should no longer be necessary'
 
 
-class _OnlyValueValidatorClsMethod(Protocol):
-    def __call__(self, __cls: Any, __value: Any) -> Any:
-        ...
-
-
-class _V1ValidatorWithValuesClsMethod(Protocol):
-    def __call__(self, __cls: Any, __value: Any, values: dict[str, Any]) -> Any:
-        ...
-
-
-class _V1ValidatorWithValuesKwOnlyClsMethod(Protocol):
-    def __call__(self, __cls: Any, __value: Any, *, values: dict[str, Any]) -> Any:
-        ...
-
-
-class _V1ValidatorWithKwargsClsMethod(Protocol):
-    def __call__(self, __cls: Any, **kwargs: Any) -> Any:
-        ...
-
-
-class _V1ValidatorWithValuesAndKwargsClsMethod(Protocol):
-    def __call__(self, __cls: Any, values: dict[str, Any], **kwargs: Any) -> Any:
-        ...
-
-
-class _V2ValidatorClsMethod(Protocol):
-    def __call__(self, __cls: Any, __input_value: Any, __info: _core_schema.FieldValidationInfo) -> Any:
-        ...
-
-
-class _V2WrapValidatorClsMethod(Protocol):
-    def __call__(
-        self,
-        __cls: Any,
-        __input_value: Any,
-        __validator: _core_schema.ValidatorFunctionWrapHandler,
-        __info: _core_schema.ValidationInfo,
-    ) -> Any:
-        ...
-
-
-class _V1RootValidatorClsMethod(Protocol):
-    def __call__(self, __cls: Any, __values: _decorators.RootValidatorValues) -> _decorators.RootValidatorValues:
-        ...
+if TYPE_CHECKING:
 
-
-V1Validator = Union[
-    _OnlyValueValidatorClsMethod,
-    _V1ValidatorWithValuesClsMethod,
-    _V1ValidatorWithValuesKwOnlyClsMethod,
-    _V1ValidatorWithKwargsClsMethod,
-    _V1ValidatorWithValuesAndKwargsClsMethod,
-    _decorators.V1ValidatorWithValues,
-    _decorators.V1ValidatorWithValuesKwOnly,
-    _decorators.V1ValidatorWithKwargs,
-    _decorators.V1ValidatorWithValuesAndKwargs,
-]
-
-V2Validator = Union[
-    _V2ValidatorClsMethod,
-    _core_schema.FieldValidatorFunction,
-    _OnlyValueValidatorClsMethod,
-    _decorators.OnlyValueValidator,
-]
-
-V2WrapValidator = Union[
-    _V2WrapValidatorClsMethod,
-    _core_schema.GeneralWrapValidatorFunction,
-    _core_schema.FieldWrapValidatorFunction,
-]
-
-V1RootValidator = Union[
-    _V1RootValidatorClsMethod,
-    _decorators.V1RootValidatorFunction,
-]
-
-_PartialClsOrStaticMethod: TypeAlias = 'Union[classmethod[Any, Any, Any], staticmethod[Any, Any], partialmethod[Any]]'
-
-
-# Allow both a V1 (assumed pre=False) or V2 (assumed mode='after') validator
-# We lie to type checkers and say we return the same thing we get
-# but in reality we return a proxy object that _mostly_ behaves like the wrapped thing
-_V1ValidatorType = TypeVar('_V1ValidatorType', bound=Union[V1Validator, _PartialClsOrStaticMethod])
-_V2BeforeAfterOrPlainValidatorType = TypeVar(
-    '_V2BeforeAfterOrPlainValidatorType',
-    bound=Union[V2Validator, _PartialClsOrStaticMethod],
-)
-_V2WrapValidatorType = TypeVar('_V2WrapValidatorType', bound=Union[V2WrapValidator, _PartialClsOrStaticMethod])
-_V1RootValidatorFunctionType = TypeVar(
-    '_V1RootValidatorFunctionType',
-    bound=Union[_decorators.V1RootValidatorFunction, _V1RootValidatorClsMethod, _PartialClsOrStaticMethod],
-)
+    class _OnlyValueValidatorClsMethod(Protocol):
+        def __call__(self, __cls: Any, __value: Any) -> Any:
+            ...
+
+    class _V1ValidatorWithValuesClsMethod(Protocol):
+        def __call__(self, __cls: Any, __value: Any, values: dict[str, Any]) -> Any:
+            ...
+
+    class _V1ValidatorWithValuesKwOnlyClsMethod(Protocol):
+        def __call__(self, __cls: Any, __value: Any, *, values: dict[str, Any]) -> Any:
+            ...
+
+    class _V1ValidatorWithKwargsClsMethod(Protocol):
+        def __call__(self, __cls: Any, **kwargs: Any) -> Any:
+            ...
+
+    class _V1ValidatorWithValuesAndKwargsClsMethod(Protocol):
+        def __call__(self, __cls: Any, values: dict[str, Any], **kwargs: Any) -> Any:
+            ...
+
+    class _V2ValidatorClsMethod(Protocol):
+        def __call__(self, __cls: Any, __input_value: Any, __info: _core_schema.FieldValidationInfo) -> Any:
+            ...
+
+    class _V2WrapValidatorClsMethod(Protocol):
+        def __call__(
+            self,
+            __cls: Any,
+            __input_value: Any,
+            __validator: _core_schema.ValidatorFunctionWrapHandler,
+            __info: _core_schema.ValidationInfo,
+        ) -> Any:
+            ...
+
+    class _V1RootValidatorClsMethod(Protocol):
+        def __call__(
+            self, __cls: Any, __values: _decorators_v1.RootValidatorValues
+        ) -> _decorators_v1.RootValidatorValues:
+            ...
+
+    V1Validator = Union[
+        _OnlyValueValidatorClsMethod,
+        _V1ValidatorWithValuesClsMethod,
+        _V1ValidatorWithValuesKwOnlyClsMethod,
+        _V1ValidatorWithKwargsClsMethod,
+        _V1ValidatorWithValuesAndKwargsClsMethod,
+        _decorators_v1.V1ValidatorWithValues,
+        _decorators_v1.V1ValidatorWithValuesKwOnly,
+        _decorators_v1.V1ValidatorWithKwargs,
+        _decorators_v1.V1ValidatorWithValuesAndKwargs,
+    ]
+
+    V2Validator = Union[
+        _V2ValidatorClsMethod,
+        _core_schema.FieldValidatorFunction,
+        _OnlyValueValidatorClsMethod,
+        _core_schema.NoInfoValidatorFunction,
+    ]
+
+    V2WrapValidator = Union[
+        _V2WrapValidatorClsMethod,
+        _core_schema.GeneralWrapValidatorFunction,
+        _core_schema.FieldWrapValidatorFunction,
+    ]
+
+    V1RootValidator = Union[
+        _V1RootValidatorClsMethod,
+        _decorators_v1.V1RootValidatorFunction,
+    ]
+
+    _PartialClsOrStaticMethod: TypeAlias = Union[classmethod[Any, Any, Any], staticmethod[Any, Any], partialmethod[Any]]
+
+    # Allow both a V1 (assumed pre=False) or V2 (assumed mode='after') validator
+    # We lie to type checkers and say we return the same thing we get
+    # but in reality we return a proxy object that _mostly_ behaves like the wrapped thing
+    _V1ValidatorType = TypeVar('_V1ValidatorType', V1Validator, _PartialClsOrStaticMethod)
+    _V2BeforeAfterOrPlainValidatorType = TypeVar(
+        '_V2BeforeAfterOrPlainValidatorType',
+        V2Validator,
+        _PartialClsOrStaticMethod,
+    )
+    _V2WrapValidatorType = TypeVar('_V2WrapValidatorType', V2WrapValidator, _PartialClsOrStaticMethod)
+    _V1RootValidatorFunctionType = TypeVar(
+        '_V1RootValidatorFunctionType',
+        _decorators_v1.V1RootValidatorFunction,
+        _V1RootValidatorClsMethod,
+        _PartialClsOrStaticMethod,
+    )
 
 
 def validator(
     __field: str,
     *fields: str,
     pre: bool = False,
     each_item: bool = False,
@@ -169,30 +163,30 @@
         ' see the migration guide for more details',
         DeprecationWarning,
         stacklevel=2,
     )
 
     mode: Literal['before', 'after'] = 'before' if pre is True else 'after'
 
-    def dec(f: Any) -> _decorators.PydanticDecoratorMarker[Any]:
+    def dec(f: Any) -> _decorators.PydanticDescriptorProxy[Any]:
         if _decorators.is_instance_method_from_sig(f):
             raise PydanticUserError(
                 '`@validator` cannot be applied to instance methods', code='validator-instance-method'
             )
         # auto apply the @classmethod decorator
         f = _decorators.ensure_classmethod_based_on_signature(f)
-        wrap = _decorators.make_generic_v1_field_validator
+        wrap = _decorators_v1.make_generic_v1_field_validator
         validator_wrapper_info = _decorators.ValidatorDecoratorInfo(
             fields=fields,
             mode=mode,
             each_item=each_item,
             always=always,
             check_fields=check_fields,
         )
-        return _decorators.PydanticDecoratorMarker(f, validator_wrapper_info, shim=wrap)
+        return _decorators.PydanticDescriptorProxy(f, validator_wrapper_info, shim=wrap)
 
     return dec  # type: ignore[return-value]
 
 
 @overload
 def field_validator(
     __field: str,
@@ -209,64 +203,63 @@
     *fields: str,
     mode: Literal['wrap'],
     check_fields: bool | None = ...,
 ) -> Callable[[_V2WrapValidatorType], _V2WrapValidatorType]:
     ...
 
 
+FieldValidatorModes: TypeAlias = Literal['before', 'after', 'wrap', 'plain']
+
+
 def field_validator(
     __field: str,
     *fields: str,
-    mode: Literal['before', 'after', 'wrap', 'plain'] = 'after',
+    mode: FieldValidatorModes = 'after',
     check_fields: bool | None = None,
 ) -> Callable[[Any], Any]:
     """
     Decorate methods on the class indicating that they should be used to validate fields.
 
     Args:
-        __field (str): The first field the field_validator should be called on; this is separate
+        __field: The first field the field_validator should be called on; this is separate
             from `fields` to ensure an error is raised if you don't pass at least one.
-        *fields (str): Additional field(s) the field_validator should be called on.
-        mode (Literal['before', 'after', 'wrap', 'plain'], optional): TODO. Defaults to 'after'.
-        check_fields (bool | None, optional): Whether to check that the fields actually exist on
-            the model. Defaults to None.
+        *fields: Additional field(s) the field_validator should be called on.
+        mode: Defaults to 'after'.
+        check_fields: Whether to check that the fields actually exist on the model. Defaults to None.
 
     Returns:
-        Callable[[Any], Any]: A decorator that can be used to decorate a function to be used as a field_validator.
+        A decorator that can be used to decorate a function to be used as a field_validator.
     """
-    fields = tuple((__field, *fields))
-    if isinstance(fields[0], FunctionType):
+    if isinstance(__field, FunctionType):
         raise PydanticUserError(
             'field_validators should be used with fields and keyword arguments, not bare. '
             "E.g. usage should be `@validator('<field_name>', ...)`",
             code='validator-no-fields',
         )
-    elif not all(isinstance(field, str) for field in fields):
+    fields = __field, *fields
+    if not all(isinstance(field, str) for field in fields):
         raise PydanticUserError(
             'field_validator fields should be passed as separate string args. '
             "E.g. usage should be `@validator('<field_name_1>', '<field_name_2>', ...)`",
             code='validator-invalid-fields',
         )
 
     def dec(
         f: Callable[..., Any] | staticmethod[Any, Any] | classmethod[Any, Any, Any]
-    ) -> _decorators.PydanticDecoratorMarker[Any]:
+    ) -> _decorators.PydanticDescriptorProxy[Any]:
         if _decorators.is_instance_method_from_sig(f):
             raise PydanticUserError(
                 '`@field_validator` cannot be applied to instance methods', code='validator-instance-method'
             )
-        # auto apply the @classmethod decorator and warn users if we had to do so
-        f = _decorators.ensure_classmethod_based_on_signature(f)
 
-        wrap = partial(_decorators.make_generic_validator, mode=mode)
+        # auto apply the @classmethod decorator
+        f = _decorators.ensure_classmethod_based_on_signature(f)
 
-        validator_wrapper_info = _decorators.FieldValidatorDecoratorInfo(
-            fields=fields, mode=mode, check_fields=check_fields
-        )
-        return _decorators.PydanticDecoratorMarker(f, validator_wrapper_info, shim=wrap)
+        dec_info = _decorators.FieldValidatorDecoratorInfo(fields=fields, mode=mode, check_fields=check_fields)
+        return _decorators.PydanticDescriptorProxy(f, dec_info)
 
     return dec
 
 
 @overload
 def root_validator(
     *,
@@ -327,47 +320,34 @@
     mode: Literal['before', 'after'] = 'before' if pre is True else 'after'
     if pre is False and skip_on_failure is not True:
         raise PydanticUserError(
             'If you use `@root_validator` with pre=False (the default) you MUST specify `skip_on_failure=True`.',
             code='root-validator-pre-skip',
         )
 
-    wrap = partial(_decorators.make_v1_generic_root_validator, pre=pre)
+    wrap = partial(_decorators_v1.make_v1_generic_root_validator, pre=pre)
 
     def dec(f: Callable[..., Any] | classmethod[Any, Any, Any] | staticmethod[Any, Any]) -> Any:
         if _decorators.is_instance_method_from_sig(f):
             raise TypeError('`@root_validator` cannot be applied to instance methods')
-        # auto apply the @classmethod decorator and warn users if we had to do so
+        # auto apply the @classmethod decorator
         res = _decorators.ensure_classmethod_based_on_signature(f)
-        validator_wrapper_info = _decorators.RootValidatorDecoratorInfo(mode=mode)
-        return _decorators.PydanticDecoratorMarker(res, validator_wrapper_info, shim=wrap)
+        dec_info = _decorators.RootValidatorDecoratorInfo(mode=mode)
+        return _decorators.PydanticDescriptorProxy(res, dec_info, shim=wrap)
 
     return dec
 
 
-_PlainSerializationFunction = Union[
-    _core_schema.GeneralPlainSerializerFunction,
-    _core_schema.FieldPlainSerializerFunction,
-    _decorators.GenericPlainSerializerFunctionWithoutInfo,
-    _decorators.FieldPlainSerializerFunctionWithoutInfo,
-    _PartialClsOrStaticMethod,
-]
-
-
-_WrapSerializationFunction = Union[
-    _core_schema.GeneralWrapSerializerFunction,
-    _core_schema.FieldWrapSerializerFunction,
-    _decorators.GeneralWrapSerializerFunctionWithoutInfo,
-    _decorators.FieldWrapSerializerFunctionWithoutInfo,
-    _PartialClsOrStaticMethod,
-]
+if TYPE_CHECKING:
+    _PlainSerializationFunction = Union[_core_schema.SerializerFunction, _PartialClsOrStaticMethod]
 
+    _WrapSerializationFunction = Union[_core_schema.WrapSerializerFunction, _PartialClsOrStaticMethod]
 
-_PlainSerializeMethodType = TypeVar('_PlainSerializeMethodType', bound=_PlainSerializationFunction)
-_WrapSerializeMethodType = TypeVar('_WrapSerializeMethodType', bound=_WrapSerializationFunction)
+    _PlainSerializeMethodType = TypeVar('_PlainSerializeMethodType', bound=_PlainSerializationFunction)
+    _WrapSerializeMethodType = TypeVar('_WrapSerializeMethodType', bound=_WrapSerializationFunction)
 
 
 @overload
 def field_serializer(
     __field: str,
     *fields: str,
     json_return_type: _core_schema.JsonReturnTypes | None = ...,
@@ -427,38 +407,33 @@
         json_return_type (str): The type that the function returns if the serialization mode is JSON.
         when_used (str): When the function should be called.
         check_fields (bool): Whether to check that the fields actually exist on the model.
     """
 
     def dec(
         f: Callable[..., Any] | staticmethod[Any, Any] | classmethod[Any, Any, Any]
-    ) -> _decorators.PydanticDecoratorMarker[Any]:
-        type_: Literal['field', 'general'] = 'field' if _decorators.is_instance_method_from_sig(f) else 'general'
-
+    ) -> _decorators.PydanticDescriptorProxy[Any]:
         dec_info = _decorators.FieldSerializerDecoratorInfo(
             fields=fields,
             mode=mode,
-            type=type_,
             json_return_type=json_return_type,
             when_used=when_used,
             check_fields=check_fields,
         )
-        return _decorators.PydanticDecoratorMarker(
-            f, dec_info, shim=partial(_decorators.make_generic_serializer, mode=mode, type=type_)
-        )
+        return _decorators.PydanticDescriptorProxy(f, dec_info)
 
     return dec
 
 
 def model_serializer(
     __f: Callable[..., Any] | None = None,
     *,
     mode: Literal['plain', 'wrap'] = 'plain',
     json_return_type: _core_schema.JsonReturnTypes | None = None,
-) -> Callable[[Any], _decorators.PydanticDecoratorMarker[Any]] | _decorators.PydanticDecoratorMarker[Any]:
+) -> Callable[[Any], _decorators.PydanticDescriptorProxy[Any]] | _decorators.PydanticDescriptorProxy[Any]:
     """
     Decorator to add a function which will be called to serialize the model.
 
     (`when_used` is not permitted here since it makes no sense.)
 
     Args:
         __f (Callable[..., Any] | None): The function to be decorated.
@@ -469,27 +444,17 @@
             serialization mode is JSON.
 
     Returns:
         Callable[[Any], _decorators.PydanticDecoratorMarker[Any]] | _decorators.PydanticDecoratorMarker[Any]:
             The decorated function.
     """
 
-    def dec(f: Callable[..., Any]) -> _decorators.PydanticDecoratorMarker[Any]:
-        if isinstance(f, (staticmethod, classmethod)) or not _decorators.is_instance_method_from_sig(f):
-            raise PydanticUserError(
-                '`@model_serializer` must be applied to instance methods', code='model-serializer-instance-method'
-            )
-
-        dec_info = _decorators.ModelSerializerDecoratorInfo(
-            mode=mode,
-            json_return_type=json_return_type,
-        )
-        return _decorators.PydanticDecoratorMarker(
-            f, dec_info, shim=partial(_decorators.make_generic_model_serializer, mode=mode)
-        )
+    def dec(f: Callable[..., Any]) -> _decorators.PydanticDescriptorProxy[Any]:
+        dec_info = _decorators.ModelSerializerDecoratorInfo(mode=mode, json_return_type=json_return_type)
+        return _decorators.PydanticDescriptorProxy(f, dec_info)
 
     if __f is None:
         return dec
     else:
         return dec(__f)
 
 
@@ -562,59 +527,47 @@
     def __call__(
         self: ModelType,  # type: ignore
         __info: _core_schema.ValidationInfo,
     ) -> ModelType:
         ...
 
 
-AnyModelWrapValidator = Union[
-    ModelWrapValidator,
-    ModelWrapValidatorWithoutInfo,
-]
-
-AnyModeBeforeValidator = Union[
-    ModelBeforeValidator,
-    ModelBeforeValidatorWithoutInfo,
-]
-
-AnyModeAfterValidator = Union[
-    ModelAfterValidator,
-    ModelAfterValidatorWithoutInfo,
-]
+AnyModelWrapValidator = Union[ModelWrapValidator, ModelWrapValidatorWithoutInfo]
+AnyModeBeforeValidator = Union[ModelBeforeValidator, ModelBeforeValidatorWithoutInfo]
+AnyModeAfterValidator = Union[ModelAfterValidator, ModelAfterValidatorWithoutInfo]
 
 
 @overload
 def model_validator(
     *,
     mode: Literal['wrap'],
-) -> Callable[[AnyModelWrapValidator], _decorators.PydanticDecoratorMarker[_decorators.ModelValidatorDecoratorInfo]]:
+) -> Callable[[AnyModelWrapValidator], _decorators.PydanticDescriptorProxy[_decorators.ModelValidatorDecoratorInfo]]:
     ...
 
 
 @overload
 def model_validator(
     *,
     mode: Literal['before'],
-) -> Callable[[AnyModeBeforeValidator], _decorators.PydanticDecoratorMarker[_decorators.ModelValidatorDecoratorInfo]]:
+) -> Callable[[AnyModeBeforeValidator], _decorators.PydanticDescriptorProxy[_decorators.ModelValidatorDecoratorInfo]]:
     ...
 
 
 @overload
 def model_validator(
     *,
     mode: Literal['after'],
-) -> Callable[[AnyModeAfterValidator], _decorators.PydanticDecoratorMarker[_decorators.ModelValidatorDecoratorInfo]]:
+) -> Callable[[AnyModeAfterValidator], _decorators.PydanticDescriptorProxy[_decorators.ModelValidatorDecoratorInfo]]:
     ...
 
 
 def model_validator(
     *,
     mode: Literal['wrap', 'before', 'after'],
 ) -> Any:
-    def dec(f: Any) -> _decorators.PydanticDecoratorMarker[Any]:
-        dec_info = _decorators.ModelValidatorDecoratorInfo(
-            mode=mode,
-        )
-        shim = partial(_decorators.make_generic_validator, mode=mode)
-        return _decorators.PydanticDecoratorMarker(f, dec_info, shim=shim)
+    def dec(f: Any) -> _decorators.PydanticDescriptorProxy[Any]:
+        # auto apply the @classmethod decorator
+        f = _decorators.ensure_classmethod_based_on_signature(f)
+        dec_info = _decorators.ModelValidatorDecoratorInfo(mode=mode)
+        return _decorators.PydanticDescriptorProxy(f, dec_info)
 
     return dec
```

### Comparing `pydantic-2.0a2/pydantic/json_schema.py` & `pydantic-2.0a3/pydantic/json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -672,21 +672,17 @@
             return self.kw_arguments_schema(kw_or_p_arguments + kw_only_arguments, var_kwargs_schema)
 
         if not prefer_positional:
             positional_possible = not kw_only_arguments and not var_kwargs_schema
             if positional_possible:
                 return self.p_arguments_schema(p_only_arguments + kw_or_p_arguments, var_args_schema)
 
-        return {
-            'type': 'object',
-            'properties': {
-                '__args__': self.p_arguments_schema(p_only_arguments, var_args_schema),
-                '__kwargs__': self.kw_arguments_schema(kw_or_p_arguments + kw_only_arguments, var_args_schema),
-            },
-        }
+        raise PydanticInvalidForJsonSchema(
+            'Unable to generate JSON schema for arguments validator with positional only and keyword only arguments'
+        )
 
     def kw_arguments_schema(
         self, arguments: list[core_schema.ArgumentsParameter], var_kwargs_schema: CoreSchema | None
     ) -> JsonSchemaValue:
         properties: dict[str, JsonSchemaValue] = {}
         required: list[str] = []
         for argument in arguments:
@@ -823,15 +819,15 @@
             if schema['type'] == 'definition-ref':
                 # Referenced schemas should not have titles set for the same reason
                 # schemas with refs should not
                 return False
             return True  # anything else should have title set
 
         else:
-            raise TypeError(f'Unexpected schema type: schema={schema}')
+            raise PydanticInvalidForJsonSchema(f'Unexpected schema type: schema={schema}')
 
     def normalize_name(self, name: str) -> str:
         return re.sub(r'[^a-zA-Z0-9.\-_]', '_', name).replace('.', '__')
 
     def get_defs_ref(self, core_ref: CoreRef) -> DefsRef:
         """
         Override this method to change the way that definitions keys are generated from a core reference.
```

### Comparing `pydantic-2.0a2/pydantic/main.py` & `pydantic-2.0a3/pydantic/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typing
 import warnings
 from abc import ABCMeta
 from copy import copy, deepcopy
 from inspect import getdoc
 from pathlib import Path
 from types import prepare_class, resolve_bases
-from typing import Any, Generic, Mapping, Tuple, cast
+from typing import Any, Callable, Generic, Mapping, Tuple, cast
 
 import pydantic_core
 import typing_extensions
 
 from ._internal import (
     _config,
     _decorators,
@@ -22,27 +22,27 @@
     _generics,
     _model_construction,
     _repr,
     _typing_extra,
     _utils,
 )
 from ._internal._fields import Undefined
+from ._migration import getattr_migration
 from .config import ConfigDict
 from .deprecated import copy_internals as _deprecated_copy_internals
 from .deprecated import parse as _deprecated_parse
 from .errors import PydanticUndefinedAnnotation, PydanticUserError
-from .fields import Field, FieldInfo, ModelPrivateAttr
+from .fields import ComputedFieldInfo, Field, FieldInfo, ModelPrivateAttr
 from .json_schema import DEFAULT_REF_TEMPLATE, GenerateJsonSchema, JsonSchemaValue, model_json_schema
 
 if typing.TYPE_CHECKING:
     from inspect import Signature
 
     from pydantic_core import CoreSchema, SchemaSerializer, SchemaValidator
 
-    from ._internal._generate_schema import GenerateSchema
     from ._internal._utils import AbstractSetIntStr, MappingIntStrAny
 
     AnyClassMethod = classmethod[Any, Any, Any]
     TupleGenerator = typing.Generator[Tuple[str, Any], None, None]
     Model = typing.TypeVar('Model', bound='BaseModel')
     # should be `set[int] | set[str] | dict[int, IncEx] | dict[str, IncEx] | None`, but mypy can't cope
     IncEx: typing_extensions.TypeAlias = 'set[int] | set[str] | dict[int, Any] | dict[str, Any] | None'
@@ -60,15 +60,15 @@
 class _ModelNamespaceDict(dict):  # type: ignore[type-arg]
     """
     Intercept attributes being set on model classes and warn about overriding of decorators (`@field_validator`, etc.)
     """
 
     def __setitem__(self, k: str, v: object) -> None:
         existing: Any = self.get(k, None)
-        if existing and v is not existing and isinstance(existing, _decorators.PydanticDecoratorMarker):
+        if existing and v is not existing and isinstance(existing, _decorators.PydanticDescriptorProxy):
             warnings.warn(f'`{k}` overrides an existing Pydantic `{existing.decorator_info.decorator_repr}` decorator')
 
         return super().__setitem__(k, v)
 
 
 @typing_extensions.dataclass_transform(kw_only_default=True, field_specifiers=(Field,))
 class ModelMetaclass(ABCMeta):
@@ -116,15 +116,15 @@
                 def hash_func(self: Any) -> int:
                     return hash(self.__class__) + hash(tuple(self.__dict__.values()))
 
                 namespace['__hash__'] = hash_func
 
             cls: type[BaseModel] = super().__new__(mcs, cls_name, bases, namespace, **kwargs)  # type: ignore
 
-            cls.__pydantic_decorators__ = _decorators.gather_decorator_functions(cls)
+            cls.__pydantic_decorators__ = _decorators.DecoratorInfos.build(cls)
 
             # Use the getattr below to grab the __parameters__ from the `typing.Generic` parent class
             if __pydantic_generic_metadata__:
                 cls.__pydantic_generic_metadata__ = __pydantic_generic_metadata__
             else:
                 parameters = getattr(cls, '__parameters__', ())
                 parent_parameters = getattr(cls, '__pydantic_generic_metadata__', {}).get('parameters', ())
@@ -157,22 +157,22 @@
                 if callable(set_name):
                     set_name(cls, name)
 
             if __pydantic_reset_parent_namespace__:
                 cls.__pydantic_parent_namespace__ = _typing_extra.parent_frame_namespace()
             parent_namespace = getattr(cls, '__pydantic_parent_namespace__', None)
 
-            types_namespace = _model_construction.get_model_types_namespace(cls, parent_namespace)
+            types_namespace = _typing_extra.get_cls_types_namespace(cls, parent_namespace)
             _model_construction.set_model_fields(cls, bases, types_namespace)
             _model_construction.complete_model_class(
                 cls,
                 cls_name,
                 config_wrapper,
-                types_namespace,
                 raise_errors=False,
+                types_namespace=types_namespace,
             )
             # using super(cls, cls) on the next line ensures we only call the parent class's __pydantic_init_subclass__
             # I believe the `type: ignore` is only necessary because mypy doesn't realize that this code branch is
             # only hit for _proper_ subclasses of BaseModel
             super(cls, cls).__pydantic_init_subclass__(**kwargs)  # type: ignore[misc]
             return cls
         else:
@@ -227,16 +227,27 @@
         Uses something other than `self` for the first arg to allow "self" as a field name.
         """
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
         __pydantic_self__.__pydantic_validator__.validate_python(data, self_instance=__pydantic_self__)
 
     @classmethod
-    def __get_pydantic_core_schema__(cls, source: type[BaseModel], gen_schema: GenerateSchema) -> CoreSchema:
-        return gen_schema.model_schema(cls)
+    def __get_pydantic_core_schema__(
+        cls, __source: type[BaseModel], __handler: Callable[[Any], CoreSchema]
+    ) -> CoreSchema:
+        # Only use the cached value from this _exact_ class; we don't want one from a parent class
+        # This is why we check `cls.__dict__` and don't use `cls.__pydantic_core_schema__` or similar.
+        if '__pydantic_core_schema__' in cls.__dict__:
+            # Due to the way generic classes are built, it's possible that an invalid schema may be temporarily
+            # set on generic classes. I think we could resolve this to ensure that we get proper schema caching
+            # for generics, but for simplicity for now, we just always rebuild if the class has a generic origin.
+            if not cls.__pydantic_generic_metadata__['origin']:
+                return cls.__pydantic_core_schema__
+
+        return __handler(__source)
 
     @classmethod
     def __pydantic_init_subclass__(cls, **kwargs: Any) -> None:
         """
         This is intended to behave just like `__init_subclass__`, but is called by ModelMetaclass
         only after the class is actually fully initialized. In particular, attributes like `model_fields` will
         be present when this is called.
@@ -261,14 +272,21 @@
     @property
     def model_fields_set(self) -> set[str]:
         """
         The set of fields that have been set on this model instance, i.e. that were not filled from defaults.
         """
         return self.__pydantic_fields_set__
 
+    @property
+    def model_computed_fields(self) -> dict[str, ComputedFieldInfo]:
+        """
+        The computed fields of this model instance.
+        """
+        return {k: v.info for k, v in self.__pydantic_decorators__.computed_fields.items()}
+
     @classmethod
     def model_validate_json(
         cls: type[Model],
         json_data: str | bytes | bytearray,
         *,
         strict: bool | None = None,
         context: dict[str, Any] | None = None,
@@ -285,18 +303,23 @@
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name in self.__class_vars__:
             raise AttributeError(
                 f'"{name}" is a ClassVar of `{self.__class__.__name__}` and cannot be set on an instance. '
                 f'If you want to set a value on the class, use `{self.__class__.__name__}.{name} = value`.'
             )
-        if name.startswith('_'):
+        elif name.startswith('_'):
             _object_setattr(self, name, value)
+            return
         elif self.model_config.get('frozen', None):
             raise TypeError(f'"{self.__class__.__name__}" is frozen and does not support item assignment')
+
+        attr = getattr(self.__class__, name, None)
+        if isinstance(attr, property):
+            attr.__set__(self, value)
         elif self.model_config.get('validate_assignment', None):
             self.__pydantic_validator__.validate_assignment(self, name, value)
         elif self.model_config.get('extra') != 'allow' and name not in self.model_fields:
             # TODO - matching error
             raise ValueError(f'"{self.__class__.__name__}" object has no field "{name}"')
         else:
             self.__dict__[name] = value
@@ -449,21 +472,21 @@
                 if _parent_namespace_depth > 0:
                     frame_parent_ns = _typing_extra.parent_frame_namespace(parent_depth=_parent_namespace_depth) or {}
                     cls_parent_ns = cls.__pydantic_parent_namespace__ or {}
                     cls.__pydantic_parent_namespace__ = {**cls_parent_ns, **frame_parent_ns}
 
                 types_namespace = cls.__pydantic_parent_namespace__
 
-                types_namespace = _model_construction.get_model_types_namespace(cls, types_namespace)
+                types_namespace = _typing_extra.get_cls_types_namespace(cls, types_namespace)
             return _model_construction.complete_model_class(
                 cls,
                 cls.__name__,
                 _config.ConfigWrapper(cls.model_config, check=False),
-                types_namespace,
                 raise_errors=raise_errors,
+                types_namespace=types_namespace,
             )
 
     def __iter__(self) -> TupleGenerator:
         """
         so `dict(model)` works
         """
         yield from self.__dict__.items()
@@ -533,19 +556,20 @@
         for name in self.__private_attributes__:
             value = getattr(self, name, Undefined)
             if value is not Undefined:
                 _object_setattr(m, name, deepcopy(value, memo=memo))
         return m
 
     def __repr_args__(self) -> _repr.ReprArgs:
-        return [
+        yield from [
             (k, v)
             for k, v in self.__dict__.items()
             if not k.startswith('_') and (k not in self.model_fields or self.model_fields[k].repr)
         ]
+        yield from [(k, getattr(self, k)) for k, v in self.model_computed_fields.items() if v.repr]
 
     def __class_getitem__(
         cls, typevar_values: type[Any] | tuple[type[Any], ...]
     ) -> type[BaseModel] | _forward_ref.PydanticForwardRef | _forward_ref.PydanticRecursiveRef:
         cached = _generics.get_cached_generic_type_early(cls, typevar_values)
         if cached is not None:
             return cached
@@ -1003,7 +1027,10 @@
     for base in bases:
         if _base_class_defined and issubclass(base, BaseModel) and base != BaseModel:
             # model_fields might not be defined yet in the case of generics, so we use getattr here:
             field_names.update(getattr(base, 'model_fields', {}).keys())
             class_vars.update(base.__class_vars__)
             private_attributes.update(base.__private_attributes__)
     return field_names, class_vars, private_attributes
+
+
+__getattr__ = getattr_migration(__name__)
```

### Comparing `pydantic-2.0a2/pydantic/mypy.py` & `pydantic-2.0a3/pydantic/mypy.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
                 return False
             return True
         if isinstance(expr, CallExpr) and isinstance(expr.callee, RefExpr) and expr.callee.fullname == FIELD_FULLNAME:
             # The "default value" is a call to `Field`; at this point, the field is
             # only required if default is Ellipsis (i.e., `field_name: Annotation = Field(...)`) or if default_factory
             # is specified.
             for arg, name in zip(expr.args, expr.arg_names):
-                # If name is None, then this arg is the default because it is the only positonal argument.
+                # If name is None, then this arg is the default because it is the only positional argument.
                 if name is None or name == 'default':
                     return arg.__class__ is EllipsisExpr
                 if name == 'default_factory':
                     return False
             return True
         # Only required if the "default value" is Ellipsis (i.e., `field_name: Annotation = ...`)
         return isinstance(expr, EllipsisExpr)
```

### Comparing `pydantic-2.0a2/pydantic/networks.py` & `pydantic-2.0a3/pydantic/networks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations as _annotations
 
 import dataclasses as _dataclasses
 import re
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Callable
 
 from pydantic_core import MultiHostUrl, PydanticCustomError, Url, core_schema
 from typing_extensions import Annotated, TypeAlias
 
 from ._internal import _fields, _repr
+from ._migration import getattr_migration
 
 if TYPE_CHECKING:
     import email_validator
 
     NetworkType: TypeAlias = 'str | bytes | int | tuple[str | bytes | int, str | int]'
 
 else:
@@ -129,22 +130,18 @@
 if TYPE_CHECKING:
     EmailStr = Annotated[str, ...]
 else:
 
     class EmailStr:
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, schema: core_schema.CoreSchema | None = None, **_kwargs: Any
+            cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
         ) -> core_schema.CoreSchema:
             import_email_validator()
-            if schema is None:
-                return core_schema.general_after_validator_function(cls.validate, core_schema.str_schema())
-            else:
-                assert schema['type'] == 'str', 'EmailStr must be used with string fields'
-                return core_schema.general_after_validator_function(cls.validate, schema)
+            return core_schema.general_after_validator_function(cls.validate, core_schema.str_schema())
 
         @classmethod
         def __pydantic_modify_json_schema__(cls, field_schema: dict[str, Any]) -> dict[str, Any]:
             field_schema.update(type='string', format='email')
             return field_schema
 
         @classmethod
@@ -164,15 +161,17 @@
 
     @classmethod
     def __pydantic_modify_json_schema__(cls, field_schema: dict[str, Any]) -> dict[str, Any]:
         field_schema.update(type='string', format='name-email')
         return field_schema
 
     @classmethod
-    def __get_pydantic_core_schema__(cls, **_kwargs: Any) -> core_schema.AfterValidatorFunctionSchema:
+    def __get_pydantic_core_schema__(
+        cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
+    ) -> core_schema.CoreSchema:
         import_email_validator()
         return core_schema.general_after_validator_function(
             cls._validate,
             core_schema.union_schema([core_schema.is_instance_schema(cls), core_schema.str_schema()]),
             serialization=core_schema.to_string_ser_schema(),
         )
 
@@ -204,15 +203,17 @@
 
     @classmethod
     def __pydantic_modify_json_schema__(cls, field_schema: dict[str, Any]) -> dict[str, Any]:
         field_schema.update(type='string', format='ipvanyaddress')
         return field_schema
 
     @classmethod
-    def __get_pydantic_core_schema__(cls, **_kwargs: Any) -> core_schema.PlainValidatorFunctionSchema:
+    def __get_pydantic_core_schema__(
+        cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
+    ) -> core_schema.CoreSchema:
         return core_schema.general_plain_validator_function(cls._validate)
 
     @classmethod
     def _validate(cls, __input_value: Any, _: core_schema.ValidationInfo) -> IPv4Address | IPv6Address:
         return cls(__input_value)  # type: ignore[return-value]
 
 
@@ -232,15 +233,17 @@
 
     @classmethod
     def __pydantic_modify_json_schema__(cls, field_schema: dict[str, Any]) -> dict[str, Any]:
         field_schema.update(type='string', format='ipvanyinterface')
         return field_schema
 
     @classmethod
-    def __get_pydantic_core_schema__(cls, **_kwargs: Any) -> core_schema.PlainValidatorFunctionSchema:
+    def __get_pydantic_core_schema__(
+        cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
+    ) -> core_schema.CoreSchema:
         return core_schema.general_plain_validator_function(cls._validate)
 
     @classmethod
     def _validate(cls, __input_value: NetworkType, _: core_schema.ValidationInfo) -> IPv4Interface | IPv6Interface:
         return cls(__input_value)  # type: ignore[return-value]
 
 
@@ -262,15 +265,17 @@
 
     @classmethod
     def __pydantic_modify_json_schema__(cls, field_schema: dict[str, Any]) -> dict[str, Any]:
         field_schema.update(type='string', format='ipvanynetwork')
         return field_schema
 
     @classmethod
-    def __get_pydantic_core_schema__(cls, **_kwargs: Any) -> core_schema.PlainValidatorFunctionSchema:
+    def __get_pydantic_core_schema__(
+        cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
+    ) -> core_schema.CoreSchema:
         return core_schema.general_plain_validator_function(cls._validate)
 
     @classmethod
     def _validate(cls, __input_value: NetworkType, _: core_schema.ValidationInfo) -> IPv4Network | IPv6Network:
         return cls(__input_value)  # type: ignore[return-value]
 
 
@@ -300,7 +305,10 @@
         parts = email_validator.validate_email(email, check_deliverability=False)
     except email_validator.EmailNotValidError as e:
         raise PydanticCustomError(
             'value_error', 'value is not a valid email address: {reason}', {'reason': str(e.args[0])}
         ) from e
 
     return name or parts['local'], parts['email']
+
+
+__getattr__ = getattr_migration(__name__)
```

### Comparing `pydantic-2.0a2/pydantic/tools.py` & `pydantic-2.0a3/pydantic/deprecated/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 from __future__ import annotations
 
 import json
 import warnings
 from typing import Any, Callable, Type, TypeVar, Union
 
-from . import AnalyzedType
+from typing_extensions import deprecated
 
-__all__ = 'parse_obj_as', 'schema_of', 'schema_json_of'
+from ..analyzed_type import AnalyzedType
+from ..json_schema import DEFAULT_REF_TEMPLATE, GenerateJsonSchema
 
-from .json_schema import DEFAULT_REF_TEMPLATE, GenerateJsonSchema
+__all__ = 'parse_obj_as', 'schema_of', 'schema_json_of'
 
 NameFactory = Union[str, Callable[[Type[Any]], str]]
 
 
 T = TypeVar('T')
 
 
+@deprecated('parse_obj_as is deprecated. Use pydantic.AnalyzedType.validate_python instead.')
 def parse_obj_as(type_: type[T], obj: Any, type_name: NameFactory | None = None) -> T:
-    # TODO: add deprecation warning of some sort
+    warnings.warn(
+        'parse_obj_as is deprecated. Use pydantic.AnalyzedType.validate_python instead.',
+        DeprecationWarning,
+        stacklevel=2,
+    )
     if type_name is not None:  # pragma: no cover
         warnings.warn(
             'The type_name parameter is deprecated. parse_obj_as no longer creates temporary models',
             DeprecationWarning,
             stacklevel=2,
         )
     return AnalyzedType(type_).validate_python(obj)
 
 
+@deprecated('schema_of is deprecated. Use pydantic.AnalyzedType.json_schema instead.')
 def schema_of(
     type_: Any,
     *,
     title: NameFactory | None = None,
     by_alias: bool = True,
     ref_template: str = DEFAULT_REF_TEMPLATE,
     schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
 ) -> dict[str, Any]:
     """Generate a JSON schema (as dict) for the passed model or dynamically generated one"""
+    warnings.warn(
+        'schema_of is deprecated. Use pydantic.AnalyzedType.json_schema instead.', DeprecationWarning, stacklevel=2
+    )
     res = AnalyzedType(type_).json_schema(
         by_alias=by_alias,
         schema_generator=schema_generator,
         ref_template=ref_template,
     )
     if title is not None:
         if isinstance(title, str):
@@ -50,21 +60,25 @@
                 DeprecationWarning,
                 stacklevel=2,
             )
             res['title'] = title(type_)
     return res
 
 
+@deprecated('schema_json_of is deprecated. Use pydantic.AnalyzedType.json_schema instead.')
 def schema_json_of(
     type_: Any,
     *,
     title: NameFactory | None = None,
     by_alias: bool = True,
     ref_template: str = DEFAULT_REF_TEMPLATE,
     schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
     **dumps_kwargs: Any,
 ) -> str:
     """Generate a JSON schema (as JSON) for the passed model or dynamically generated one"""
+    warnings.warn(
+        'schema_json_of is deprecated. Use pydantic.AnalyzedType.json_schema instead.', DeprecationWarning, stacklevel=2
+    )
     return json.dumps(
         schema_of(type_, title=title, by_alias=by_alias, ref_template=ref_template, schema_generator=schema_generator),
         **dumps_kwargs,
     )
```

### Comparing `pydantic-2.0a2/pydantic/types.py` & `pydantic-2.0a3/pydantic/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from datetime import date, datetime
 from decimal import Decimal
 from enum import Enum
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     ClassVar,
     FrozenSet,
     Generic,
     Hashable,
     List,
     Set,
     TypeVar,
@@ -22,14 +23,15 @@
 from uuid import UUID
 
 import annotated_types
 from pydantic_core import PydanticCustomError, PydanticKnownError, core_schema
 from typing_extensions import Annotated, Literal
 
 from ._internal import _fields, _validators
+from ._migration import getattr_migration
 
 __all__ = [
     'Strict',
     'StrictStr',
     'conbytes',
     'conlist',
     'conset',
@@ -243,21 +245,23 @@
     class ImportString:
         @classmethod
         def __class_getitem__(cls, item: AnyType) -> AnyType:
             return Annotated[item, cls()]
 
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, schema: core_schema.CoreSchema | None = None, **_kwargs: Any
+            cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
         ) -> core_schema.CoreSchema:
-            if schema is None or schema == {'type': 'any'}:
+            if cls is source:
                 # Treat bare usage of ImportString (`schema is None`) as the same as ImportString[Any]
                 return core_schema.general_plain_validator_function(lambda v, _: _validators.import_string(v))
             else:
-                return core_schema.general_before_validator_function(lambda v, _: _validators.import_string(v), schema)
+                return core_schema.general_before_validator_function(
+                    lambda v, _: _validators.import_string(v), handler(source)
+                )
 
         def __repr__(self) -> str:
             return 'ImportString'
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ DECIMAL TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -293,18 +297,18 @@
 
     def __pydantic_modify_json_schema__(self, field_schema: dict[str, Any]) -> dict[str, Any]:
         field_schema.pop('anyOf', None)  # remove the bytes/str union
         field_schema.update(type='string', format=f'uuid{self.uuid_version}')
         return field_schema
 
     def __get_pydantic_core_schema__(
-        self, schema: core_schema.CoreSchema, **_kwargs: Any
-    ) -> core_schema.AfterValidatorFunctionSchema:
+        self, source: Any, handler: Callable[[Any], core_schema.CoreSchema]
+    ) -> core_schema.CoreSchema:
         return core_schema.general_after_validator_function(
-            cast(core_schema.GeneralValidatorFunction, self.validate), schema
+            cast(core_schema.GeneralValidatorFunction, self.validate), handler(source)
         )
 
     def validate(self, value: UUID, _: core_schema.ValidationInfo) -> UUID:
         if value.version != self.uuid_version:
             raise PydanticCustomError(
                 'uuid_version', 'uuid version {required_version} expected', {'required_version': self.uuid_version}
             )
@@ -326,25 +330,25 @@
 
     def __pydantic_modify_json_schema__(self, field_schema: dict[str, Any]) -> dict[str, Any]:
         format_conversion = {'file': 'file-path', 'dir': 'directory-path'}
         field_schema.update(format=format_conversion.get(self.path_type, 'path'), type='string')
         return field_schema
 
     def __get_pydantic_core_schema__(
-        self, schema: core_schema.CoreSchema, **_kwargs: Any
-    ) -> core_schema.AfterValidatorFunctionSchema:
+        self, source: Any, handler: Callable[[Any], core_schema.CoreSchema]
+    ) -> core_schema.CoreSchema:
         function_lookup = {
             'file': cast(core_schema.GeneralValidatorFunction, self.validate_file),
             'dir': cast(core_schema.GeneralValidatorFunction, self.validate_directory),
             'new': cast(core_schema.GeneralValidatorFunction, self.validate_new),
         }
 
         return core_schema.general_after_validator_function(
             function_lookup[self.path_type],
-            schema,
+            handler(source),
         )
 
     @staticmethod
     def validate_file(path: Path, _: core_schema.ValidationInfo) -> Path:
         if path.is_file():
             return path
         else:
@@ -385,22 +389,20 @@
     class Json:
         @classmethod
         def __class_getitem__(cls, item: AnyType) -> AnyType:
             return Annotated[item, cls()]
 
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, schema: core_schema.CoreSchema | None = None, **_kwargs: Any
-        ) -> core_schema.JsonSchema:
-            return core_schema.json_schema(schema)
-
-        @classmethod
-        def __pydantic_modify_json_schema__(cls, field_schema: dict[str, Any]) -> dict[str, Any]:
-            field_schema.update(type='string', format='json-string')
-            return field_schema
+            cls, source: Any, handler: Callable[[Any], core_schema.CoreSchema]
+        ) -> core_schema.CoreSchema:
+            if cls is source:
+                return core_schema.json_schema(None)
+            else:
+                return core_schema.json_schema(handler(source))
 
         def __repr__(self) -> str:
             return 'Json'
 
         def __hash__(self) -> int:
             return hash(type(self))
 
@@ -419,15 +421,17 @@
     def __init__(self, secret_value: SecretType) -> None:
         self._secret_value: SecretType = secret_value
 
     def get_secret_value(self) -> SecretType:
         return self._secret_value
 
     @classmethod
-    def __get_pydantic_core_schema__(cls, **_kwargs: Any) -> core_schema.AfterValidatorFunctionSchema:
+    def __get_pydantic_core_schema__(
+        cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
+    ) -> core_schema.CoreSchema:
         validator = SecretFieldValidator(cls)
         if issubclass(cls, SecretStr):
             # Use a lambda here so that `apply_metadata` can be called on the validator before the override is generated
             js_cs_override = lambda: core_schema.str_schema(  # noqa E731
                 min_length=validator.min_length,
                 max_length=validator.max_length,
             )
@@ -445,16 +449,16 @@
             validator,
             core_schema.union_schema(
                 [core_schema.is_instance_schema(cls), cls._pre_core_schema()],
                 strict=True,
                 custom_error_type=cls._error_kind,
             ),
             metadata=metadata,
-            serialization=core_schema.general_plain_serializer_function_ser_schema(
-                cls._serialize, json_return_type='str'
+            serialization=core_schema.plain_serializer_function_ser_schema(
+                cls._serialize, info_arg=True, json_return_type='str'
             ),
         )
 
     @classmethod
     def _serialize(
         cls, value: SecretField[SecretType], info: core_schema.SerializationInfo
     ) -> str | SecretField[SecretType]:
@@ -587,15 +591,17 @@
         card_number = self.validate_luhn_check_digit(card_number)
 
         self.bin = card_number[:6]
         self.last4 = card_number[-4:]
         self.brand = self.validate_brand(card_number)
 
     @classmethod
-    def __get_pydantic_core_schema__(cls, **_kwargs: Any) -> core_schema.AfterValidatorFunctionSchema:
+    def __get_pydantic_core_schema__(
+        cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
+    ) -> core_schema.CoreSchema:
         return core_schema.general_after_validator_function(
             cls.validate,
             core_schema.str_schema(
                 min_length=cls.min_length, max_length=cls.max_length, strip_whitespace=cls.strip_whitespace
             ),
         )
 
@@ -689,15 +695,17 @@
 }
 BYTE_SIZES.update({k.lower()[0]: v for k, v in BYTE_SIZES.items() if 'i' not in k})
 byte_string_re = re.compile(r'^\s*(\d*\.?\d+)\s*(\w+)?', re.IGNORECASE)
 
 
 class ByteSize(int):
     @classmethod
-    def __get_pydantic_core_schema__(cls, **_kwargs: Any) -> core_schema.PlainValidatorFunctionSchema:
+    def __get_pydantic_core_schema__(
+        cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
+    ) -> core_schema.CoreSchema:
         # TODO better schema
         return core_schema.general_plain_validator_function(cls.validate)
 
     @classmethod
     def validate(cls, __input_value: Any, _: core_schema.ValidationInfo) -> ByteSize:
         try:
             return cls(int(__input_value))
@@ -755,36 +763,38 @@
     PastDate = Annotated[date, ...]
     FutureDate = Annotated[date, ...]
 else:
 
     class PastDate:
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, schema: core_schema.CoreSchema | None = None, **_kwargs: Any
+            cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
         ) -> core_schema.CoreSchema:
-            if schema is None:
+            if cls is source:
                 # used directly as a type
                 return core_schema.date_schema(now_op='past')
             else:
+                schema = handler(source)
                 assert schema['type'] == 'date'
                 schema['now_op'] = 'past'
                 return schema
 
         def __repr__(self) -> str:
             return 'PastDate'
 
     class FutureDate:
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, schema: core_schema.CoreSchema | None = None, **_kwargs: Any
+            cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
         ) -> core_schema.CoreSchema:
-            if schema is None:
+            if cls is source:
                 # used directly as a type
                 return core_schema.date_schema(now_op='future')
             else:
+                schema = handler(source)
                 assert schema['type'] == 'date'
                 schema['now_op'] = 'future'
                 return schema
 
         def __repr__(self) -> str:
             return 'FutureDate'
 
@@ -810,35 +820,40 @@
     AwareDatetime = Annotated[datetime, ...]
     NaiveDatetime = Annotated[datetime, ...]
 else:
 
     class AwareDatetime:
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, schema: core_schema.CoreSchema | None = None, **_kwargs: Any
+            cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
         ) -> core_schema.CoreSchema:
-            if schema is None:
+            if cls is source:
                 # used directly as a type
                 return core_schema.datetime_schema(tz_constraint='aware')
             else:
+                schema = handler(source)
                 assert schema['type'] == 'datetime'
                 schema['tz_constraint'] = 'aware'
                 return schema
 
         def __repr__(self) -> str:
             return 'AwareDatetime'
 
     class NaiveDatetime:
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, schema: core_schema.CoreSchema | None = None, **_kwargs: Any
+            cls, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
         ) -> core_schema.CoreSchema:
-            if schema is None:
+            if cls is source:
                 # used directly as a type
                 return core_schema.datetime_schema(tz_constraint='naive')
             else:
+                schema = handler(source)
                 assert schema['type'] == 'datetime'
                 schema['tz_constraint'] = 'naive'
                 return schema
 
         def __repr__(self) -> str:
             return 'NaiveDatetime'
+
+
+__getattr__ = getattr_migration(__name__)
```

### Comparing `pydantic-2.0a2/pydantic/version.py` & `pydantic-2.0a3/pydantic/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = 'VERSION', 'version_info'
 
-VERSION = '2.0a2'
+VERSION = '2.0a3'
 
 
 def version_info() -> str:
     import platform
     import sys
     from importlib import import_module
     from pathlib import Path
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_config.py` & `pydantic-2.0a3/pydantic/_internal/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     strict: bool
     # whether instances of models and dataclasses (including subclass instances) should re-validate, default 'never'
     revalidate_instances: Literal['always', 'never', 'subclass-instances']
     ser_json_timedelta: Literal['iso8601', 'float']
     ser_json_bytes: Literal['utf8', 'base64']
     # whether to validate default values during validation, default False
     validate_default: bool
+    validate_return: bool
 
     def __init__(self, config: ConfigDict | dict[str, Any] | type[Any] | None, *, check: bool = True):
         if check:
             self.config_dict = prepare_config(config)
         else:
             self.config_dict = cast(ConfigDict, config)
 
@@ -163,14 +164,15 @@
     ignored_types=(),
     allow_inf_nan=True,
     strict=False,
     revalidate_instances='never',
     ser_json_timedelta='iso8601',
     ser_json_bytes='utf8',
     validate_default=False,
+    validate_return=False,
 )
 
 
 def prepare_config(config: ConfigDict | dict[str, Any] | type[Any] | None) -> ConfigDict:
     """
     Create a `ConfigDict` instance from an existing dict, a class (e.g. old class-based config) or None.
     """
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_core_metadata.py` & `pydantic-2.0a3/pydantic/_internal/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/pydantic/_internal/_core_utils.py` & `pydantic-2.0a3/pydantic/_internal/_core_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         ref: str | None = s.get('ref')  # type: ignore[assignment]
         if ref:
             if ref in refs:
                 return {'type': 'definition-ref', 'schema_ref': ref}
             refs.add(ref)
         return s
 
-    schema = WalkAndApply(_replace_refs, apply_before_recurse=True).walk(schema)
+    schema = WalkCoreSchema(_replace_refs, apply_before_recurse=True).walk(schema)
     return schema
 
 
 def collect_definitions(schema: core_schema.CoreSchema) -> dict[str, core_schema.CoreSchema]:
     # Only collect valid definitions. This is equivalent to collecting all definitions for "valid" schemas,
     # but allows us to reuse this logic while removing "invalid" definitions
     valid_definitions = dict()
@@ -127,15 +127,15 @@
         if ref:
             metadata = s.get('metadata')
             definition_is_invalid = isinstance(metadata, dict) and 'invalid' in metadata
             if not definition_is_invalid:
                 valid_definitions[ref] = s
         return s
 
-    WalkAndApply(_record_valid_refs).walk(schema)
+    WalkCoreSchema(_record_valid_refs).walk(schema)
 
     return valid_definitions
 
 
 def remove_unnecessary_invalid_definitions(schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
     valid_refs = collect_definitions(schema).keys()
 
@@ -157,29 +157,33 @@
                 continue
             # fmt: on
             new_definitions.append(definition)
 
         new_schema['definitions'] = new_definitions
         return new_schema
 
-    return WalkAndApply(_remove_invalid_defs).walk(schema)
+    return WalkCoreSchema(_remove_invalid_defs).walk(schema)
 
 
 def define_expected_missing_refs(
     schema: core_schema.CoreSchema, allowed_missing_refs: set[str]
 ) -> core_schema.CoreSchema:
+    if not allowed_missing_refs:
+        # in this case, there are no missing refs to potentially substitute, so there's no need to walk the schema
+        # this is a common case (will be hit for all non-generic models), so it's worth optimizing for
+        return schema
     refs = set()
 
     def _record_refs(s: core_schema.CoreSchema) -> core_schema.CoreSchema:
         ref: str | None = s.get('ref')  # type: ignore[assignment]
         if ref:
             refs.add(ref)
         return s
 
-    WalkAndApply(_record_refs).walk(schema)
+    WalkCoreSchema(_record_refs).walk(schema)
 
     expected_missing_refs = allowed_missing_refs.difference(refs)
     if expected_missing_refs:
         definitions: list[core_schema.CoreSchema] = [
             # TODO: Replace this with a (new) CoreSchema that, if present at any level, makes validation fail
             core_schema.none_schema(ref=ref, metadata={'pydantic_debug_missing_ref': True, 'invalid': True})
             for ref in expected_missing_refs
@@ -192,19 +196,26 @@
     invalid_schemas: list[core_schema.CoreSchema] = []
 
     def _is_schema_valid(s: core_schema.CoreSchema) -> core_schema.CoreSchema:
         if s.get('metadata', {}).get('invalid'):
             invalid_schemas.append(s)
         return s
 
-    WalkAndApply(_is_schema_valid).walk(schema)
+    WalkCoreSchema(_is_schema_valid).walk(schema)
     return invalid_schemas
 
 
-class WalkAndApply:
+class WalkCoreSchema:
+    """
+    Transforms a CoreSchema by recursively calling the provided function on all (nested) fields of type CoreSchema
+
+    The provided function need not actually modify the schema in any way, but will still be called on all nested
+    fields with type CoreSchema. (This can be useful for collecting information about refs, etc.)
+    """
+
     def __init__(
         self, f: Callable[[core_schema.CoreSchema], core_schema.CoreSchema], apply_before_recurse: bool = True
     ):
         self.f = f
 
         self.apply_before_recurse = apply_before_recurse
 
@@ -336,14 +347,23 @@
         for k, v in schema['fields'].items():
             replaced_field = v.copy()
             replaced_field['schema'] = self._walk(v['schema'])
             replaced_fields[k] = replaced_field
         schema['fields'] = replaced_fields
         return schema
 
+    def handle_dataclass_args_schema(self, schema: core_schema.DataclassArgsSchema) -> CoreSchema:
+        replaced_fields: list[core_schema.DataclassField] = []
+        for field in schema['fields']:
+            replaced_field = field.copy()
+            replaced_field['schema'] = self._walk(field['schema'])
+            replaced_fields.append(replaced_field)
+        schema['fields'] = replaced_fields
+        return schema
+
     def handle_arguments_schema(self, schema: core_schema.ArgumentsSchema) -> CoreSchema:
         replaced_arguments_schema = []
         for param in schema['arguments_schema']:
             replaced_param = param.copy()
             replaced_param['schema'] = self._walk(param['schema'])
             replaced_arguments_schema.append(replaced_param)
         schema['arguments_schema'] = replaced_arguments_schema
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_dataclasses.py` & `pydantic-2.0a3/pydantic/_internal/_dataclasses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,122 @@
 """
 Private logic for creating pydantic dataclasses.
 """
 from __future__ import annotations as _annotations
 
+import dataclasses
 import typing
 import warnings
 from functools import wraps
-from typing import Any, Callable, ClassVar, cast
+from typing import Any, Callable, ClassVar
 
 from pydantic_core import ArgsKwargs, SchemaSerializer, SchemaValidator, core_schema
+from typing_extensions import TypeGuard
 
 from ..errors import PydanticUndefinedAnnotation
 from ..fields import FieldInfo
-from . import _decorators
-from ._core_utils import get_type_ref
-from ._fields import collect_fields
-from ._forward_ref import PydanticForwardRef
-from ._generate_schema import dataclass_schema
+from . import _decorators, _typing_extra
+from ._fields import collect_dataclass_fields
+from ._generate_schema import GenerateSchema
+from ._generics import get_standard_typevars_map
 from ._model_construction import MockValidator
 
-__all__ = 'StandardDataclass', 'PydanticDataclass', 'prepare_dataclass'
-
 if typing.TYPE_CHECKING:
     from ..config import ConfigDict
     from ._config import ConfigWrapper
 
     class StandardDataclass(typing.Protocol):
         __dataclass_fields__: ClassVar[dict[str, Any]]
         __dataclass_params__: ClassVar[Any]  # in reality `dataclasses._DataclassParams`
         __post_init__: ClassVar[Callable[..., None]]
 
         def __init__(self, *args: object, **kwargs: object) -> None:
             pass
 
     class PydanticDataclass(StandardDataclass, typing.Protocol):
-        __pydantic_validator__: typing.ClassVar[SchemaValidator]
         __pydantic_core_schema__: typing.ClassVar[core_schema.CoreSchema]
+        __pydantic_validator__: typing.ClassVar[SchemaValidator]
         __pydantic_serializer__: typing.ClassVar[SchemaSerializer]
         __pydantic_decorators__: typing.ClassVar[_decorators.DecoratorInfos]
         """metadata for `@validator`, `@root_validator` and `@serializer` decorators"""
         __pydantic_fields__: typing.ClassVar[dict[str, FieldInfo]]
         __pydantic_config__: typing.ClassVar[ConfigDict]
 
 
-def prepare_dataclass(
+def set_dataclass_fields(cls: type[StandardDataclass], types_namespace: dict[str, Any] | None = None) -> None:
+    """
+    Collect and set `cls.__pydantic_fields__`
+    """
+    typevars_map = get_standard_typevars_map(cls)
+    fields = collect_dataclass_fields(cls, types_namespace, typevars_map=typevars_map)
+
+    cls.__pydantic_fields__ = fields  # type: ignore
+
+
+def complete_dataclass(
     cls: type[Any],
     config_wrapper: ConfigWrapper,
-    kw_only: bool,
     *,
     raise_errors: bool = True,
     types_namespace: dict[str, Any] | None = None,
 ) -> bool:
     """
     Prepare a raw class to become a pydantic dataclass.
 
     Returns `True` if the validation construction is successfully completed, else `False`.
 
     This logic is called on a class which is yet to be wrapped in `dataclasses.dataclass()`.
     """
+    cls_name = cls.__name__
+
     if hasattr(cls, '__post_init_post_parse__'):
         warnings.warn(
             'Support for `__post_init_post_parse__` has been dropped, the method will not be called', DeprecationWarning
         )
 
-    cls = cast('type[PydanticDataclass]', cls)
-
-    name = cls.__name__
-    bases = cls.__bases__
+    types_namespace = _typing_extra.get_cls_types_namespace(cls, types_namespace)
+    typevars_map = get_standard_typevars_map(cls)
+    gen_schema = GenerateSchema(
+        config_wrapper,
+        types_namespace,
+        typevars_map,
+    )
 
-    dataclass_ref = get_type_ref(cls)
-    self_schema = core_schema.definition_reference_schema(dataclass_ref)
-    types_namespace = {**(types_namespace or {}), name: PydanticForwardRef(self_schema, cls)}
     try:
-        fields, _ = collect_fields(cls, bases, types_namespace, is_dataclass=True, dc_kw_only=kw_only)
+        schema = gen_schema.generate_schema(cls)
     except PydanticUndefinedAnnotation as e:
         if raise_errors:
             raise
-        warning_string = (
-            f'`{name}` is not fully defined, you should define `{e}`, then call TODO! `methods.rebuild({name})`'
-        )
         if config_wrapper.undefined_types_warning:
-            raise UserWarning(warning_string)
-        cls.__pydantic_validator__ = MockValidator(warning_string, code='dataclass-not-fully-defined')  # type: ignore
+            config_warning_string = (
+                f'`{cls_name}` has an undefined annotation: `{e.name}`. '
+                f'It may be possible to resolve this by setting '
+                f'undefined_types_warning=False in the config for `{cls_name}`.'
+            )
+            # FIXME UserWarning should not be raised here, but rather warned!
+            raise UserWarning(config_warning_string)
+        usage_warning_string = (
+            f'`{cls_name}` is not fully defined; you should define `{e.name}`, then call'
+            f' TODO! `methods.rebuild({cls_name})` before the first `{cls_name}` instance is created.'  # <--- TODO
+        )
+        cls.__pydantic_validator__ = MockValidator(  # type: ignore[assignment]
+            usage_warning_string, code='dataclass-not-fully-defined'
+        )
         return False
 
-    decorators = cls.__pydantic_decorators__
-
-    cls.__pydantic_core_schema__ = schema = dataclass_schema(
-        cls,
-        dataclass_ref,
-        fields,
-        decorators,
-        config_wrapper,
-        types_namespace,
-    )
-
     core_config = config_wrapper.core_config(cls)
-    cls.__pydantic_fields__ = fields
+
+    # We are about to set all the remaining required properties expected for this cast;
+    # __pydantic_decorators__ and __pydantic_fields__ should already be set
+    cls = typing.cast('type[PydanticDataclass]', cls)
+    # debug(schema)
+    cls.__pydantic_core_schema__ = schema
     cls.__pydantic_validator__ = validator = SchemaValidator(schema, core_config)
-    # this works because cls has been transformed into a dataclass by the time "cls" is called
     cls.__pydantic_serializer__ = SchemaSerializer(schema, core_config)
+    # dataclasses only:
     cls.__pydantic_config__ = config_wrapper.config_dict
 
     if config_wrapper.validate_assignment:
 
         @wraps(cls.__setattr__)
         def validated_setattr(instance: Any, __field: str, __value: str) -> None:
             validator.validate_assignment(instance, __field, __value)
@@ -119,15 +132,15 @@
 
     __init__.__qualname__ = f'{cls.__qualname__}.__init__'
     cls.__init__ = __init__  # type: ignore
 
     return True
 
 
-def is_builtin_dataclass(_cls: type[Any]) -> bool:
+def is_builtin_dataclass(_cls: type[Any]) -> TypeGuard[type[StandardDataclass]]:
     """
     Whether a class is a stdlib dataclass
     (useful to discriminated a pydantic dataclass that is actually a wrapper around a stdlib dataclass)
 
     we check that
     - `_cls` is a dataclass
     - `_cls` is not a processed pydantic dataclass (with a basemodel attached)
@@ -141,14 +154,16 @@
     @pydantic.dataclasses.dataclass
     class B(A):
         y: int
     ```
     In this case, when we first check `B`, we make an extra check and look at the annotations ('y'),
     which won't be a superset of all the dataclass fields (only the stdlib fields i.e. 'x')
     """
-    import dataclasses
-
     return (
         dataclasses.is_dataclass(_cls)
         and not hasattr(_cls, '__pydantic_validator__')
         and set(_cls.__dataclass_fields__).issuperset(set(getattr(_cls, '__annotations__', {})))
     )
+
+
+def is_pydantic_dataclass(_cls: type[Any]) -> TypeGuard[type[PydanticDataclass]]:
+    return dataclasses.is_dataclass(_cls) and hasattr(_cls, '__pydantic_validator__')
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_decorators.py` & `pydantic-2.0a3/pydantic/_internal/_decorators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,33 @@
 """
 Logic related to validators applied to models etc. via the `@validator` and `@root_validator` decorators.
 """
 from __future__ import annotations as _annotations
 
-from dataclasses import field
+from dataclasses import dataclass, field
 from functools import partial, partialmethod
-from inspect import Parameter, Signature, signature
-from typing import (
-    Any,
-    Callable,
-    ClassVar,
-    Dict,
-    Generic,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-    cast,
-    overload,
-)
+from inspect import Parameter, Signature, isdatadescriptor, ismethoddescriptor, signature
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Generic, TypeVar, Union, cast
 
-from pydantic_core.core_schema import (
-    FieldPlainSerializerFunction,
-    FieldValidationInfo,
-    FieldValidatorFunction,
-    FieldWrapSerializerFunction,
-    FieldWrapValidatorFunction,
-    GeneralPlainSerializerFunction,
-    GeneralWrapSerializerFunction,
-    JsonReturnTypes,
-    SerializationInfo,
-    SerializerFunctionWrapHandler,
-    ValidationInfo,
-    WhenUsed,
-)
-from typing_extensions import Literal, Protocol, TypeAlias
+from pydantic_core import core_schema
+from typing_extensions import Literal, TypeAlias
 
 from ..errors import PydanticUserError
+from ..fields import ComputedFieldInfo
 from ._core_utils import get_type_ref
 from ._internal_dataclass import slots_dataclass
 
-FIELD_VALIDATOR_TAG = '_field_validator'
-ROOT_VALIDATOR_TAG = '_root_validator'
+if TYPE_CHECKING:
+    from ..decorators import FieldValidatorModes
 
-FIELD_SERIALIZER_TAG = '_field_serializer'
+try:
+    from functools import cached_property  # type: ignore
+except ImportError:
+    # python 3.7
+    cached_property = None
 
 
 @slots_dataclass
 class ValidatorDecoratorInfo:
     """
     A container for data from `@validator` so that we can access it
     while building the pydantic-core schema.
@@ -68,15 +48,15 @@
     A container for data from `@field_validator` so that we can access it
     while building the pydantic-core schema.
     """
 
     decorator_repr: ClassVar[str] = '@field_validator'
 
     fields: tuple[str, ...]
-    mode: Literal['before', 'after', 'wrap', 'plain']
+    mode: FieldValidatorModes
     check_fields: bool | None
 
 
 @slots_dataclass
 class RootValidatorDecoratorInfo:
     """
     A container for data from `@root_validator` so that we can access it
@@ -93,30 +73,29 @@
     A container for data from `@field_serializer` so that we can access it
     while building the pydantic-core schema.
     """
 
     decorator_repr: ClassVar[str] = '@field_serializer'
     fields: tuple[str, ...]
     mode: Literal['plain', 'wrap']
-    type: Literal['general', 'field']
-    json_return_type: JsonReturnTypes | None
-    when_used: WhenUsed
+    json_return_type: core_schema.JsonReturnTypes | None
+    when_used: core_schema.WhenUsed
     check_fields: bool | None
 
 
 @slots_dataclass
 class ModelSerializerDecoratorInfo:
     """
     A container for data from `@model_serializer` so that we can access it
     while building the pydantic-core schema.
     """
 
     decorator_repr: ClassVar[str] = '@model_serializer'
     mode: Literal['plain', 'wrap']
-    json_return_type: JsonReturnTypes | None
+    json_return_type: core_schema.JsonReturnTypes | None
 
 
 @slots_dataclass
 class ModelValidatorDecoratorInfo:
     """
     A container for data from `@model_validator` so that we can access it
     while building the pydantic-core schema.
@@ -129,54 +108,63 @@
 DecoratorInfo = Union[
     ValidatorDecoratorInfo,
     FieldValidatorDecoratorInfo,
     RootValidatorDecoratorInfo,
     FieldSerializerDecoratorInfo,
     ModelSerializerDecoratorInfo,
     ModelValidatorDecoratorInfo,
+    ComputedFieldInfo,
 ]
 
 ReturnType = TypeVar('ReturnType')
 DecoratedType: TypeAlias = (
-    'Union[classmethod[Any, Any, ReturnType], staticmethod[Any, ReturnType], Callable[..., ReturnType]]'
+    'Union[classmethod[Any, Any, ReturnType], staticmethod[Any, ReturnType], Callable[..., ReturnType], property]'
 )
 
 
-@slots_dataclass
-class PydanticDecoratorMarker(Generic[ReturnType]):
+@dataclass  # can't use slots here since we set attributes on `__post_init__`
+class PydanticDescriptorProxy(Generic[ReturnType]):
     """
-    Wrap a classmethod, staticmethod or unbound function
+    Wrap a classmethod, staticmethod, property or unbound function
     and act as a descriptor that allows us to detect decorated items
     from the class' attributes.
 
     This class' __get__ returns the wrapped item's __get__ result,
     which makes it transparent for classmethods and staticmethods.
     """
 
     wrapped: DecoratedType[ReturnType]
     decorator_info: DecoratorInfo
-    shim: Callable[[Callable[..., Any]], Callable[..., Any]] | None
+    shim: Callable[[Callable[..., Any]], Callable[..., Any]] | None = None
 
-    @overload
-    def __get__(self, obj: None, objtype: None) -> PydanticDecoratorMarker[ReturnType]:
-        ...
-
-    @overload
-    def __get__(self, obj: object, objtype: type[object]) -> Callable[..., ReturnType]:
-        ...
-
-    def __get__(
-        self, obj: object | None, objtype: type[object] | None = None
-    ) -> Callable[..., ReturnType] | PydanticDecoratorMarker[ReturnType]:
+    def __post_init__(self):
+        for attr in 'setter', 'deleter':
+            if hasattr(self.wrapped, attr):
+                f = partial(self._call_wrapped_attr, name=attr)
+                setattr(self, attr, f)
+
+    def _call_wrapped_attr(self, func: Callable[[Any], None], *, name: str) -> PydanticDescriptorProxy[ReturnType]:
+        self.wrapped = getattr(self.wrapped, name)(func)
+        return self
+
+    def __get__(self, obj: object | None, obj_type: type[object] | None = None) -> PydanticDescriptorProxy[ReturnType]:
         try:
-            return self.wrapped.__get__(obj, objtype)
+            return self.wrapped.__get__(obj, obj_type)
         except AttributeError:
             # not a descriptor, e.g. a partial object
             return self.wrapped  # type: ignore[return-value]
 
+    def __set_name__(self, instance: Any, name: str) -> None:
+        if hasattr(self.wrapped, '__set_name__'):
+            self.wrapped.__set_name__(instance, name)
+
+    def __getattr__(self, __name: str) -> Any:
+        """Forward checks for __isabstractmethod__ and such"""
+        return getattr(self.wrapped, __name)
+
 
 DecoratorInfoType = TypeVar('DecoratorInfoType', bound=DecoratorInfo)
 
 
 @slots_dataclass
 class Decorator(Generic[DecoratorInfoType]):
     """
@@ -191,14 +179,15 @@
     func: Callable[..., Any]
     shim: Callable[[Any], Any] | None
     info: DecoratorInfoType
 
     @staticmethod
     def build(
         cls_: Any,
+        *,
         cls_var_name: str,
         shim: Callable[[Any], Any] | None,
         info: DecoratorInfoType,
     ) -> Decorator[DecoratorInfoType]:
         func = getattr(cls_, cls_var_name)
         if shim is not None:
             func = shim(func)
@@ -220,459 +209,326 @@
 
 
 @slots_dataclass
 class DecoratorInfos:
     # mapping of name in the class namespace to decorator info
     # note that the name in the class namespace is the function or attribute name
     # not the field name!
+    # TODO these all need to be renamed to plural
     validator: dict[str, Decorator[ValidatorDecoratorInfo]] = field(default_factory=dict)
     field_validator: dict[str, Decorator[FieldValidatorDecoratorInfo]] = field(default_factory=dict)
     root_validator: dict[str, Decorator[RootValidatorDecoratorInfo]] = field(default_factory=dict)
     field_serializer: dict[str, Decorator[FieldSerializerDecoratorInfo]] = field(default_factory=dict)
     model_serializer: dict[str, Decorator[ModelSerializerDecoratorInfo]] = field(default_factory=dict)
     model_validator: dict[str, Decorator[ModelValidatorDecoratorInfo]] = field(default_factory=dict)
+    computed_fields: dict[str, Decorator[ComputedFieldInfo]] = field(default_factory=dict)
 
-
-def gather_decorator_functions(cls: type[Any]) -> DecoratorInfos:
-    """
-    We want to collect all DecFunc instances that exist as
-    attributes in the namespace of the class (a BaseModel or dataclass)
-    that called us
-    But we want to collect these in the order of the bases
-    So instead of getting them all from the leaf class (the class that called us),
-    we traverse the bases from root (the oldest ancestor class) to leaf
-    and collect all of the instances as we go, taking care to replace
-    any duplicate ones with the last one we see to mimic how function overriding
-    works with inheritance.
-    If we do replace any functions we put the replacement into the position
-    the replaced function was in; that is, we maintain the order.
-    """
-
-    # reminder: dicts are ordered and replacement does not alter the order
-    res = DecoratorInfos()
-    for base in cls.__bases__[::-1]:
-        existing = cast(Union[DecoratorInfos, None], getattr(base, '__pydantic_decorators__', None))
-        if existing is not None:
-            res.validator.update({k: v.bind_to_cls(cls) for k, v in existing.validator.items()})
-            res.field_validator.update({k: v.bind_to_cls(cls) for k, v in existing.field_validator.items()})
-            res.root_validator.update({k: v.bind_to_cls(cls) for k, v in existing.root_validator.items()})
-            res.field_serializer.update({k: v.bind_to_cls(cls) for k, v in existing.field_serializer.items()})
-            res.model_serializer.update({k: v.bind_to_cls(cls) for k, v in existing.model_serializer.items()})
-
-    for var_name, var_value in vars(cls).items():
-        if isinstance(var_value, PydanticDecoratorMarker):
-            info = var_value.decorator_info
-            if isinstance(info, ValidatorDecoratorInfo):
-                res.validator[var_name] = Decorator.build(cls, cls_var_name=var_name, shim=var_value.shim, info=info)
-            elif isinstance(info, FieldValidatorDecoratorInfo):
-                res.field_validator[var_name] = Decorator.build(
-                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
-                )
-            elif isinstance(info, RootValidatorDecoratorInfo):
-                res.root_validator[var_name] = Decorator.build(
-                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
-                )
-            elif isinstance(info, FieldSerializerDecoratorInfo):
-                # check whether a serializer function is already registered for fields
-                for field_serializer_decorator in res.field_serializer.values():
-                    # check that each field has at most one serializer function.
-                    # serializer functions for the same field in subclasses are allowed,
-                    # and are treated as overrides
-                    if field_serializer_decorator.cls_var_name == var_name:
-                        continue
-                    for f in info.fields:
-                        if f in field_serializer_decorator.info.fields:
-                            raise PydanticUserError(
-                                'Multiple field serializer functions were defined '
-                                f'for field {f!r}, this is not allowed.',
-                                code='multiple-field-serializers',
-                            )
-                res.field_serializer[var_name] = Decorator.build(
-                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
-                )
-            elif isinstance(info, ModelValidatorDecoratorInfo):
-                res.model_validator[var_name] = Decorator.build(
-                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
-                )
-            else:
-                assert isinstance(info, ModelSerializerDecoratorInfo)
-                res.model_serializer[var_name] = Decorator.build(
-                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
-                )
-            setattr(cls, var_name, var_value.wrapped)
-    return res
-
-
-_FUNCS: set[str] = set()
-
-
-AnyDecoratorCallable: TypeAlias = (
-    'Union[classmethod[Any, Any, Any], staticmethod[Any, Any], partialmethod[Any], Callable[..., Any]]'
-)
+    @staticmethod
+    def build(model_dc: type[Any]) -> DecoratorInfos:  # noqa: C901 (ignore complexity)
+        """
+        We want to collect all DecFunc instances that exist as
+        attributes in the namespace of the class (a BaseModel or dataclass)
+        that called us
+        But we want to collect these in the order of the bases
+        So instead of getting them all from the leaf class (the class that called us),
+        we traverse the bases from root (the oldest ancestor class) to leaf
+        and collect all of the instances as we go, taking care to replace
+        any duplicate ones with the last one we see to mimic how function overriding
+        works with inheritance.
+        If we do replace any functions we put the replacement into the position
+        the replaced function was in; that is, we maintain the order.
+        """
+
+        # reminder: dicts are ordered and replacement does not alter the order
+        res = DecoratorInfos()
+        for base in model_dc.__bases__[::-1]:
+            existing = cast(Union[DecoratorInfos, None], getattr(base, '__pydantic_decorators__', None))
+            if existing is not None:
+                res.validator.update({k: v.bind_to_cls(model_dc) for k, v in existing.validator.items()})
+                res.field_validator.update({k: v.bind_to_cls(model_dc) for k, v in existing.field_validator.items()})
+                res.root_validator.update({k: v.bind_to_cls(model_dc) for k, v in existing.root_validator.items()})
+                res.field_serializer.update({k: v.bind_to_cls(model_dc) for k, v in existing.field_serializer.items()})
+                res.model_serializer.update({k: v.bind_to_cls(model_dc) for k, v in existing.model_serializer.items()})
+                res.model_validator.update({k: v.bind_to_cls(model_dc) for k, v in existing.model_validator.items()})
+                res.computed_fields.update({k: v.bind_to_cls(model_dc) for k, v in existing.computed_fields.items()})
+
+        for var_name, var_value in vars(model_dc).items():
+            if isinstance(var_value, PydanticDescriptorProxy):
+                info = var_value.decorator_info
+                if isinstance(info, ValidatorDecoratorInfo):
+                    res.validator[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, FieldValidatorDecoratorInfo):
+                    res.field_validator[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, RootValidatorDecoratorInfo):
+                    res.root_validator[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, FieldSerializerDecoratorInfo):
+                    # check whether a serializer function is already registered for fields
+                    for field_serializer_decorator in res.field_serializer.values():
+                        # check that each field has at most one serializer function.
+                        # serializer functions for the same field in subclasses are allowed,
+                        # and are treated as overrides
+                        if field_serializer_decorator.cls_var_name == var_name:
+                            continue
+                        for f in info.fields:
+                            if f in field_serializer_decorator.info.fields:
+                                raise PydanticUserError(
+                                    'Multiple field serializer functions were defined '
+                                    f'for field {f!r}, this is not allowed.',
+                                    code='multiple-field-serializers',
+                                )
+                    res.field_serializer[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, ModelValidatorDecoratorInfo):
+                    res.model_validator[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, ModelSerializerDecoratorInfo):
+                    res.model_serializer[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                else:
+                    isinstance(var_value, ComputedFieldInfo)
+                    res.computed_fields[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=None, info=info
+                    )
+                setattr(model_dc, var_name, var_value.wrapped)
+        return res
 
 
-def unwrap_wrapped_function(
-    func: Any,
-    *,
-    unwrap_class_static_method: bool = True,
-) -> Any:
+def inspect_validator(validator: Callable[..., Any], mode: FieldValidatorModes) -> bool:
     """
-    Recursively unwraps a wrapped function until the underlying function is reached.
-    This handles functools.partial, functools.partialmethod, staticmethod and classmethod.
+    Look at a field or model validator function and determine if it whether it takes an info argument.
+
+    An error is raised if the function has an invalid signature.
 
     Args:
-        func: The function to unwrap.
-        unwrap_class_static_method: If True (default), also unwrap classmethod and staticmethod
-            decorators. If False, only unwrap partial and partialmethod decorators.
+        validator: The validator function to inspect.
+        mode: The proposed validator mode.
 
     Returns:
-        The underlying function of the wrapped function.
+        Whether the validator takes an info argument.
     """
-    all: tuple[Any, ...]
-    if unwrap_class_static_method:
-        all = (
-            staticmethod,
-            classmethod,
-            partial,
-            partialmethod,
-        )
+    sig = signature(validator)
+    n_positional = count_positional_params(sig)
+    if mode == 'wrap':
+        if n_positional == 3:
+            return True
+        elif n_positional == 2:
+            return False
     else:
-        all = partial, partialmethod
-
-    while isinstance(func, all):
-        if unwrap_class_static_method and isinstance(func, (classmethod, staticmethod)):
-            func = func.__func__
-        elif isinstance(func, (partial, partialmethod)):
-            func = func.func
-
-    return func
+        assert mode in {'before', 'after', 'plain'}, f"invalid mode: {mode!r}, expected 'before', 'after' or 'plain"
+        if n_positional == 2:
+            return True
+        elif n_positional == 1:
+            return False
+
+    raise PydanticUserError(
+        f'Unrecognized field_validator function signature for {validator} with `mode={mode}`:{sig}',
+        code='field-validator-signature',
+    )
 
 
-def get_function_ref(func: Any) -> str:
-    func = unwrap_wrapped_function(func)
-    return (
-        getattr(func, '__module__', '<No __module__>')
-        + '.'
-        + getattr(func, '__qualname__', f'<No __qualname__: id:{id(func)}>')
-    )
+def inspect_field_serializer(serializer: Callable[..., Any], mode: Literal['plain', 'wrap']) -> tuple[bool, bool]:
+    """
+    Look at a field serializer function and determine if it is a field serializer,
+    and whether it takes an info argument.
 
+    An error is raised if the function has an invalid signature.
 
-def is_classmethod_from_sig(function: AnyDecoratorCallable) -> bool:
-    sig = signature(unwrap_wrapped_function(function))
-    first = next(iter(sig.parameters.values()), None)
-    if first and first.name == 'cls':
-        return True
-    return False
+    Args:
+        serializer: The serializer function to inspect.
+        mode: The serializer mode, either 'plain' or 'wrap'.
 
+    Returns:
+        Tuple of (is_field_serializer, info_arg)
+    """
+    sig = signature(serializer)
 
-def is_instance_method_from_sig(function: AnyDecoratorCallable) -> bool:
-    sig = signature(unwrap_wrapped_function(function))
     first = next(iter(sig.parameters.values()), None)
-    if first and first.name == 'self':
-        return True
-    return False
+    is_field_serializer = first is not None and first.name == 'self'
 
+    n_positional = count_positional_params(sig)
+    if is_field_serializer:
+        # -1 to correct for self parameter
+        info_arg = _serializer_info_arg(mode, n_positional - 1)
+    else:
+        info_arg = _serializer_info_arg(mode, n_positional)
 
-def ensure_classmethod_based_on_signature(
-    function: AnyDecoratorCallable,
-) -> Any:
-    if not isinstance(
-        unwrap_wrapped_function(function, unwrap_class_static_method=False), classmethod
-    ) and is_classmethod_from_sig(function):
-        return classmethod(function)  # type: ignore[arg-type]
-    return function
+    if info_arg is None:
+        raise PydanticUserError(
+            f'Unrecognized field_serializer function signature for {serializer} with `mode={mode}`:{sig}',
+            code='field-serializer-signature',
+        )
+    else:
+        return is_field_serializer, info_arg
 
 
-class OnlyValueValidator(Protocol):
-    """
-    A simple validator, supported for V1 validators and V2 validators
+def inspect_annotated_serializer(serializer: Callable[..., Any], mode: Literal['plain', 'wrap']) -> bool:
     """
+    Look at a serializer function used via `Annotated` and determine whether it takes an info argument.
 
-    def __call__(self, __value: Any) -> Any:
-        ...
-
-
-class V1ValidatorWithValues(Protocol):
-    def __call__(self, __value: Any, values: dict[str, Any]) -> Any:
-        ...
-
-
-class V1ValidatorWithValuesKwOnly(Protocol):
-    def __call__(self, __value: Any, *, values: dict[str, Any]) -> Any:
-        ...
+    An error is raised if the function has an invalid signature.
 
+    Args:
+        serializer: The serializer function to check.
+        mode: The serializer mode, either 'plain' or 'wrap'.
 
-class V1ValidatorWithKwargs(Protocol):
-    def __call__(self, __value: Any, **kwargs: Any) -> Any:
-        ...
+    Returns:
+        info_arg
+    """
+    sig = signature(serializer)
+    info_arg = _serializer_info_arg(mode, count_positional_params(sig))
+    if info_arg is None:
+        raise PydanticUserError(
+            f'Unrecognized field_serializer function signature for {serializer} with `mode={mode}`:{sig}',
+            code='field-serializer-signature',
+        )
+    else:
+        return info_arg
 
 
-class V1ValidatorWithValuesAndKwargs(Protocol):
-    def __call__(self, __value: Any, values: dict[str, Any], **kwargs: Any) -> Any:
-        ...
+def inspect_model_serializer(serializer: Callable[..., Any], mode: Literal['plain', 'wrap']) -> bool:
+    """
+    Look at a model serializer function and determine whether it takes an info argument.
 
+    An error is raised if the function has an invalid signature.
 
-V1Validator = Union[
-    V1ValidatorWithValues, V1ValidatorWithValuesKwOnly, V1ValidatorWithKwargs, V1ValidatorWithValuesAndKwargs
-]
+    Args:
+        serializer: The serializer function to check.
+        mode: The serializer mode, either 'plain' or 'wrap'.
 
+    Returns:
+        `info_arg` - whether the function expects an info argument
+    """
 
-def can_be_positional(param: Parameter) -> bool:
-    return param.kind in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD)
+    if isinstance(serializer, (staticmethod, classmethod)) or not is_instance_method_from_sig(serializer):
+        raise PydanticUserError(
+            '`@model_serializer` must be applied to instance methods', code='model-serializer-instance-method'
+        )
 
+    sig = signature(serializer)
+    info_arg = _serializer_info_arg(mode, count_positional_params(sig))
+    if info_arg is None:
+        raise PydanticUserError(
+            f'Unrecognized model_serializer function signature for {serializer} with `mode={mode}`:{sig}',
+            code='model-serializer-signature',
+        )
+    else:
+        return info_arg
 
-def can_be_keyword(param: Parameter) -> bool:
-    return param.kind in (Parameter.POSITIONAL_OR_KEYWORD, Parameter.KEYWORD_ONLY)
 
+def _serializer_info_arg(mode: Literal['plain', 'wrap'], n_positional: int) -> bool | None:
+    if mode == 'plain':
+        if n_positional == 1:
+            # (__input_value: Any) -> Any
+            return False
+        elif n_positional == 2:
+            # (__model: Any, __input_value: Any) -> Any
+            return True
+    else:
+        assert mode == 'wrap', f"invalid mode: {mode!r}, expected 'plain' or 'wrap'"
+        if n_positional == 2:
+            # (__input_value: Any, __serializer: SerializerFunctionWrapHandler) -> Any
+            return False
+        elif n_positional == 3:
+            # (__input_value: Any, __serializer: SerializerFunctionWrapHandler, __info: SerializationInfo) -> Any
+            return True
 
-def make_generic_v1_field_validator(validator: V1Validator) -> FieldValidatorFunction:
-    sig = signature(validator)
+    return None
 
-    needs_values_kw = False
 
-    for param_num, (param_name, parameter) in enumerate(sig.parameters.items()):
-        if can_be_keyword(parameter) and param_name in ('field', 'config'):
-            raise PydanticUserError(
-                'The `field` and `config` parameters are not available in Pydantic V2, '
-                'please use the `info` parameter instead.',
-                code='validator-field-config-info',
-            )
-        if parameter.kind is Parameter.VAR_KEYWORD:
-            needs_values_kw = True
-        elif can_be_keyword(parameter) and param_name == 'values':
-            needs_values_kw = True
-        elif can_be_positional(parameter) and param_num == 0:
-            # value
-            continue
-        elif parameter.default is Parameter.empty:  # ignore params with defaults e.g. bound by functools.partial
-            raise PydanticUserError(
-                f'Unsupported signature for V1 style validator {validator}: {sig} is not supported.',
-                code='validator-v1-signature',
-            )
-
-    if needs_values_kw:
-        # (v, **kwargs), (v, values, **kwargs), (v, *, values, **kwargs) or (v, *, values)
-        val1 = cast(V1ValidatorWithValues, validator)
+AnyDecoratorCallable: TypeAlias = (
+    'Union[classmethod[Any, Any, Any], staticmethod[Any, Any], partialmethod[Any], Callable[..., Any]]'
+)
 
-        def wrapper1(value: Any, info: FieldValidationInfo) -> Any:
-            return val1(value, values=info.data)
 
-        return wrapper1
-    else:
-        val2 = cast(OnlyValueValidator, validator)
+def is_instance_method_from_sig(function: AnyDecoratorCallable) -> bool:
+    sig = signature(unwrap_wrapped_function(function))
+    first = next(iter(sig.parameters.values()), None)
+    if first and first.name == 'self':
+        return True
+    return False
 
-        def wrapper2(value: Any, _: FieldValidationInfo) -> Any:
-            return val2(value)
 
-        return wrapper2
+def ensure_classmethod_based_on_signature(function: AnyDecoratorCallable) -> Any:
+    if not isinstance(
+        unwrap_wrapped_function(function, unwrap_class_static_method=False), classmethod
+    ) and _is_classmethod_from_sig(function):
+        return classmethod(function)  # type: ignore[arg-type]
+    return function
 
 
-def remove_params_with_defaults(sig: Signature) -> Signature:
-    return Signature([p for p in sig.parameters.values() if p.default is Parameter.empty])
+def _is_classmethod_from_sig(function: AnyDecoratorCallable) -> bool:
+    sig = signature(unwrap_wrapped_function(function))
+    first = next(iter(sig.parameters.values()), None)
+    if first and first.name == 'cls':
+        return True
+    return False
 
 
-def make_generic_validator(
-    validator: OnlyValueValidator | FieldValidatorFunction | FieldWrapValidatorFunction, mode: str
+def unwrap_wrapped_function(
+    func: Any,
+    *,
+    unwrap_class_static_method: bool = True,
 ) -> Any:
     """
-    In order to support different signatures, including deprecated validator signatures from v1,
-    we introspect the function signature and wrap it in a parent function that has a signature
-    compatible with pydantic_core
-    """
-    sig = remove_params_with_defaults(signature(validator))
-    if mode in ('before', 'after', 'plain') and len(sig.parameters) == 1:
-        val1 = cast(OnlyValueValidator, validator)
-
-        # allow the (v) -> Any signature as a convenience
-        def wrapper1(value: Any, info: FieldValidationInfo) -> Any:
-            return val1(value)
-
-        return wrapper1
-
-    val2 = cast(Union[FieldValidatorFunction, FieldWrapValidatorFunction], validator)
-    return val2
-
-
-RootValidatorValues = Dict[str, Any]
-RootValidatorFieldsSet = Set[str]
-RootValidatorValuesAndFieldsSet = Tuple[RootValidatorValues, RootValidatorFieldsSet]
-
-
-class V1RootValidatorFunction(Protocol):
-    def __call__(self, __values: RootValidatorValues) -> RootValidatorValues:
-        ...
-
-
-class V2CoreBeforeRootValidator(Protocol):
-    def __call__(self, __values: RootValidatorValues, __info: ValidationInfo) -> RootValidatorValues:
-        ...
-
-
-class V2CoreAfterRootValidator(Protocol):
-    def __call__(
-        self, __values_and_fields_set: RootValidatorValuesAndFieldsSet, __info: ValidationInfo
-    ) -> RootValidatorValuesAndFieldsSet:
-        ...
+    Recursively unwraps a wrapped function until the underlying function is reached.
+    This handles functools.partial, functools.partialmethod, staticmethod and classmethod.
 
+    Args:
+        func: The function to unwrap.
+        unwrap_class_static_method: If True (default), also unwrap classmethod and staticmethod
+            decorators. If False, only unwrap partial and partialmethod decorators.
 
-def make_v1_generic_root_validator(
-    validator: V1RootValidatorFunction, pre: bool
-) -> V2CoreBeforeRootValidator | V2CoreAfterRootValidator:
-    """
-    Wrap a V1 style root validator for V2 compatibility
+    Returns:
+        The underlying function of the wrapped function.
     """
-    if pre is True:
-        # mode='before' for pydantic-core
-        def _wrapper1(values: RootValidatorValues, _: ValidationInfo) -> RootValidatorValues:
-            return validator(values)
-
-        return _wrapper1
+    all: tuple[Any, ...]
+    if unwrap_class_static_method:
+        all = (
+            staticmethod,
+            classmethod,
+            partial,
+            partialmethod,
+        )
+    else:
+        all = partial, partialmethod
 
-    # mode='after' for pydantic-core
-    def _wrapper2(
-        values_and_fields_set: tuple[RootValidatorValues, RootValidatorFieldsSet], _: ValidationInfo
-    ) -> tuple[RootValidatorValues, RootValidatorFieldsSet]:
-        values, fields_set = values_and_fields_set
-        values = validator(values)
-        return (values, fields_set)
+    while isinstance(func, all):
+        if unwrap_class_static_method and isinstance(func, (classmethod, staticmethod)):
+            func = func.__func__
+        elif isinstance(func, (partial, partialmethod)):
+            func = func.func
 
-    return _wrapper2
+    return func
 
 
-GenericPlainSerializerFunctionWithoutInfo = Callable[[Any], Any]
-FieldPlainSerializerFunctionWithoutInfo = Callable[[Any, Any], Any]
-FieldWrapSerializerFunctionWithoutInfo = Callable[[Any, Any, SerializerFunctionWrapHandler], Any]
-GeneralWrapSerializerFunctionWithoutInfo = Callable[[Any, SerializerFunctionWrapHandler], Any]
+def count_positional_params(sig: Signature) -> int:
+    return sum(1 for param in sig.parameters.values() if can_be_positional(param))
 
-AnyCoreSerializer = Union[
-    FieldPlainSerializerFunction,
-    FieldWrapSerializerFunction,
-    GeneralPlainSerializerFunction,
-    GeneralWrapSerializerFunction,
-]
 
-AnySerializerFunction = Union[
-    GenericPlainSerializerFunctionWithoutInfo,
-    GeneralWrapSerializerFunctionWithoutInfo,
-    AnyCoreSerializer,
-]
+def can_be_positional(param: Parameter) -> bool:
+    return param.kind in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD)
 
 
-def make_generic_serializer(
-    serializer: AnySerializerFunction, mode: Literal['plain', 'wrap'], type: Literal['field', 'general']
-) -> Any:
-    """
-    Wrap serializers to allow ignoring the `info` argument as a convenience.
+def ensure_property(f: Any) -> Any:
     """
-    sig = remove_params_with_defaults(signature(serializer))
-    if is_instance_method_from_sig(serializer):
-        # for the errors below to exclude self
-        sig = Signature(parameters=list(sig.parameters.values())[1:])
-
-    n_positional = sum(
-        1
-        for param in sig.parameters.values()
-        if param.kind in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD)
-    )
-    if mode == 'plain':
-        if n_positional == 1:
-            if type == 'general':
-                func1 = cast(GenericPlainSerializerFunctionWithoutInfo, serializer)
-
-                def wrap_generic_serializer_single_argument(value: Any, _: SerializationInfo) -> Any:
-                    return func1(value)
+    Ensure that a function is a `property` or `cached_property`, or is a valid descriptor.
 
-                return wrap_generic_serializer_single_argument
-            else:
-                assert type == 'field'
-                func2 = cast(FieldPlainSerializerFunctionWithoutInfo, serializer)
-
-                def wrap_field_serializer_single_argument(self: Any, value: Any, _: SerializationInfo) -> Any:
-                    return func2(self, value)
-
-                return wrap_field_serializer_single_argument
-        if n_positional != 2:
-            raise PydanticUserError(
-                f'Unrecognized field_serializer signature for {serializer} with `mode={mode}`:{sig}',
-                code='field-serializer-signature',
-            )
-        func = cast(AnyCoreSerializer, serializer)
-        return func
-    else:
-        assert mode == 'wrap'
-        if n_positional == 2:
-            if type == 'general':
-                func3 = cast(GeneralWrapSerializerFunctionWithoutInfo, serializer)
+    Args:
+        f: The function to check.
 
-                def wrap_general_serializer_in_wrap_mode(
-                    value: Any, handler: SerializerFunctionWrapHandler, _: SerializationInfo
-                ) -> Any:
-                    return func3(value, handler)
-
-                return wrap_general_serializer_in_wrap_mode
-            else:
-                assert type == 'field'
-                func4 = cast(FieldWrapSerializerFunctionWithoutInfo, serializer)
-
-                def wrap_field_serializer_in_wrap_mode(
-                    self: Any, value: Any, handler: SerializerFunctionWrapHandler, _: SerializationInfo
-                ) -> Any:
-                    return func4(self, value, handler)
-
-                return wrap_field_serializer_in_wrap_mode
-
-        if n_positional != 3:
-            raise PydanticUserError(
-                f'Unrecognized field_serializer signature for {serializer} with `mode={mode}`:{sig}',
-                code='field-serializer-signature',
-            )
-        func = cast(AnyCoreSerializer, serializer)
-        return func
-
-
-def make_generic_model_serializer(
-    serializer: AnySerializerFunction, mode: Literal['plain', 'wrap']
-) -> AnyCoreSerializer:
-    """
-    Wrap serializers to allow ignoring the `info` argument as a convenience.
+    Returns:
+        The function, or a `property` or `cached_property` instance wrapping the function.
     """
-    sig = signature(serializer)
 
-    n_positional = sum(
-        1
-        for param in sig.parameters.values()
-        if param.kind in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD)
-    )
-    if mode == 'plain':
-        if n_positional == 1:
-            func1 = cast(GenericPlainSerializerFunctionWithoutInfo, serializer)
-
-            def wrap_model_serializer_single_argument(value: Any, _: SerializationInfo) -> Any:
-                return func1(value)
-
-            return wrap_model_serializer_single_argument
-        if n_positional != 2:
-            raise PydanticUserError(
-                f'Unrecognized model_serializer signature for {serializer} with `mode={mode}`:{sig}',
-                code='model-serializer-signature',
-            )
-        func = cast(AnyCoreSerializer, serializer)
-        return func
+    if ismethoddescriptor(f) or isdatadescriptor(f):
+        return f
     else:
-        assert mode == 'wrap'
-        if n_positional == 2:
-            func2 = cast(GeneralWrapSerializerFunctionWithoutInfo, serializer)
-
-            def wrap_model_serializer_in_wrap_mode(
-                value: Any, handler: SerializerFunctionWrapHandler, _: SerializationInfo
-            ) -> Any:
-                return func2(value, handler)
-
-            return wrap_model_serializer_in_wrap_mode
-
-        if n_positional != 3:
-            raise PydanticUserError(
-                f'Unrecognized serializer signature for {serializer} with `mode={mode}`:{sig}',
-                code='model-serializer-signature',
-            )
-        func = cast(AnyCoreSerializer, serializer)
-        return func
+        return property(f)
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_discriminated_union.py` & `pydantic-2.0a3/pydantic/_internal/_discriminated_union.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/pydantic/_internal/_fields.py` & `pydantic-2.0a3/pydantic/_internal/_fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Private logic related to fields (the `Field()` function and `FieldInfo` class), and arguments to `Annotated`.
 """
 from __future__ import annotations as _annotations
 
 import dataclasses
 import sys
-import typing
 from abc import ABC, abstractmethod
 from copy import copy
 from typing import TYPE_CHECKING, Any
 
 from pydantic_core import core_schema
 
+from . import _typing_extra
 from ._forward_ref import PydanticForwardRef
-from ._generics import get_typevars_map, replace_types
 from ._repr import Representation
 from ._typing_extra import get_cls_type_hints_lenient, get_type_hints, is_classvar, is_finalvar
 
 if TYPE_CHECKING:
     from ..fields import FieldInfo
+    from ._dataclasses import StandardDataclass
 
 
 def get_type_hints_infer_globalns(
     obj: Any,
     localns: dict[str, Any] | None = None,
     include_extras: bool = False,
 ) -> dict[str, Any]:
@@ -107,89 +107,60 @@
             setattr(self, k, v)
 
 
 # KW_ONLY is only available in Python 3.10+
 DC_KW_ONLY = getattr(dataclasses, 'KW_ONLY', None)
 
 
-def collect_fields(  # noqa: C901
+def collect_model_fields(  # noqa: C901
     cls: type[Any],
     bases: tuple[type[Any], ...],
     types_namespace: dict[str, Any] | None,
     *,
-    is_dataclass: bool = False,
-    dc_kw_only: bool | None = None,
+    typevars_map: dict[Any, Any] | None = None,
 ) -> tuple[dict[str, FieldInfo], set[str]]:
     """
-    Collect the fields of:
-    * a nascent pydantic model
-    * a nascent pydantic dataclass
-    * or, a standard library dataclass
+    Collect the fields of a nascent pydantic model
+
     Also collect the names of any ClassVars present in the type hints.
 
     The returned value is a tuple of two items: the fields dict, and the set of ClassVar names.
 
     :param cls: BaseModel or dataclass
     :param bases: parents of the class, generally `cls.__bases__`
     :param types_namespace: optional extra namespace to look for types in
-    :param is_dataclass: whether the class is a dataclass, used to decide about kw_only setting
-    :param dc_kw_only: whether the whole dataclass is kw_only
     """
     from ..fields import FieldInfo
 
     type_hints = get_cls_type_hints_lenient(cls, types_namespace)
 
     # https://docs.python.org/3/howto/annotations.html#accessing-the-annotations-dict-of-an-object-in-python-3-9-and-older
     # annotations is only used for finding fields in parent classes
     annotations = cls.__dict__.get('__annotations__', {})
     fields: dict[str, FieldInfo] = {}
 
-    # currently just used for `init=False` dataclass fields, this logic can probably be removed if
-    # we simplify this function to not be "all things to all men"
-    omitted_fields: set[str] | None = getattr(cls, '__pydantic_omitted_fields__', None)
-
     class_vars: set[str] = set()
     for ann_name, ann_type in type_hints.items():
         if is_classvar(ann_type):
             class_vars.add(ann_name)
             continue
         if _is_finalvar_with_default_val(ann_type, getattr(cls, ann_name, Undefined)):
             class_vars.add(ann_name)
             continue
-        if ann_name.startswith('_') or (omitted_fields and ann_name in omitted_fields):
-            continue
-
-        if DC_KW_ONLY and ann_type is DC_KW_ONLY:
-            # all field fields will be kw_only
-            dc_kw_only = True
+        if ann_name.startswith('_'):
             continue
-        kw_only = dc_kw_only
-
-        init_var = False
-        if ann_type is dataclasses.InitVar:
-            if sys.version_info < (3, 8):
-                raise RuntimeError('InitVar is not supported in Python 3.7 as type information is lost')
-
-            init_var = True
-            ann_type = Any
-        elif isinstance(ann_type, dataclasses.InitVar):
-            init_var = True
-            ann_type = ann_type.type
 
         # when building a generic model with `MyModel[int]`, the generic_origin check makes sure we don't get
         # "... shadows an attribute" errors
         generic_origin = getattr(cls, '__pydantic_generic_metadata__', {}).get('origin')
         for base in bases:
             if hasattr(base, ann_name):
                 if base is generic_origin:
                     # Don't error when "shadowing" of attributes in parametrized generics
                     continue
-                if is_dataclass and dataclasses.is_dataclass(base):
-                    # Don't error when shadowing a field in a parent dataclass
-                    continue
                 raise NameError(
                     f'Field name "{ann_name}" shadows an attribute in parent "{base.__qualname__}"; '
                     f'you might want to use a different field name with "alias=\'{ann_name}\'".'
                 )
 
         try:
             default = getattr(cls, ann_name, Undefined)
@@ -210,62 +181,28 @@
                     field_info = copy(model_fields_lookup[ann_name])
                 else:
                     # The field was not found on any base classes; this seems to be caused by fields not getting
                     # generated thanks to models not being fully defined while initializing recursive models.
                     # Nothing stops us from just creating a new FieldInfo for this type hint, so we do this.
                     field_info = FieldInfo.from_annotation(ann_type)
         else:
-            if isinstance(default, dataclasses.Field):
-                if not default.init:
-                    # dataclasses.Field with init=False are not fields
-                    continue
-                if DC_KW_ONLY and default.kw_only is True:  # type: ignore
-                    kw_only = True
-
             field_info = FieldInfo.from_annotated_attribute(ann_type, default)
             # attributes which are fields are removed from the class namespace:
             # 1. To match the behaviour of annotation-only fields
             # 2. To avoid false positives in the NameError check above
             try:
                 delattr(cls, ann_name)
             except AttributeError:
                 pass  # indicates the attribute was on a parent class
 
-            if is_dataclass:
-                # for dataclasses we preserve the default value if it is set
-                # field, e.g. `a: int = 1` gets kept as is
-                # and `a: int = field(default=1, repr=False)` gets converted to the above
-                if isinstance(default, (dataclasses.Field, FieldInfo)):
-                    if default.default not in (
-                        Undefined,
-                        dataclasses.MISSING,
-                    ):
-                        setattr(cls, ann_name, default.default)
-                else:
-                    # not a field default
-                    setattr(cls, ann_name, default)
-
-        if init_var:
-            field_info.init_var = True
-        if kw_only is not None:
-            field_info.kw_only = kw_only
         fields[ann_name] = field_info
 
-    generic_metadata = getattr(cls, '__pydantic_generic_metadata__', None)
-    if generic_metadata:
-        typevars_map = get_typevars_map(generic_metadata['origin'], generic_metadata['args'])
-        if typevars_map:
-            for field in fields.values():
-                try:
-                    field.annotation = typing._eval_type(  # type: ignore[attr-defined]
-                        field.annotation, types_namespace, None
-                    )
-                except NameError:
-                    pass
-                field.annotation = replace_types(field.annotation, typevars_map)
+    if typevars_map:
+        for field in fields.values():
+            field.apply_typevars_map(typevars_map, types_namespace)
 
     return fields, class_vars
 
 
 def _is_finalvar_with_default_val(type_: type[Any], val: Any) -> bool:
     from pydantic.fields import FieldInfo
 
@@ -273,7 +210,43 @@
         return False
     elif val is Undefined:
         return False
     elif isinstance(val, FieldInfo) and (val.default is Undefined and val.default_factory is None):
         return False
     else:
         return True
+
+
+def collect_dataclass_fields(
+    cls: type[StandardDataclass], types_namespace: dict[str, Any] | None, *, typevars_map: dict[Any, Any] | None = None
+) -> dict[str, FieldInfo]:
+    from ..fields import FieldInfo
+
+    fields: dict[str, FieldInfo] = {}
+    dataclass_fields: dict[str, dataclasses.Field] = cls.__dataclass_fields__
+    cls_localns = dict(vars(cls))  # this matches get_cls_type_hints_lenient, but all tests pass with `= None` instead
+
+    for ann_name, dataclass_field in dataclass_fields.items():
+        ann_type = _typing_extra.eval_type_lenient(dataclass_field.type, types_namespace, cls_localns)
+        if is_classvar(ann_type):
+            continue
+
+        if not dataclass_field.init:
+            # TODO: We should probably do something with this so that validate_assignment behaves properly
+            #   See https://github.com/pydantic/pydantic/issues/5470
+            continue
+
+        if isinstance(dataclass_field.default, FieldInfo):
+            field_info = FieldInfo.from_annotated_attribute(ann_type, dataclass_field.default)
+        else:
+            field_info = FieldInfo.from_annotated_attribute(ann_type, dataclass_field)
+        fields[ann_name] = field_info
+
+        if field_info.default is not Undefined:
+            # We need this to fix the default when the "default" from __dataclass_fields__ is a pydantic.FieldInfo
+            setattr(cls, ann_name, field_info.default)
+
+    if typevars_map:
+        for field in fields.values():
+            field.apply_typevars_map(typevars_map, types_namespace)
+
+    return fields
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_forward_ref.py` & `pydantic-2.0a3/pydantic/_internal/_forward_ref.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from __future__ import annotations as _annotations
 
 from dataclasses import dataclass, replace
-from typing import TYPE_CHECKING, Any, Union
+from typing import Any, Union
 
 from pydantic_core import core_schema
 from typing_extensions import Literal, TypedDict
 
 from ._typing_extra import TypeVarType
 
-if TYPE_CHECKING:
-    from pydantic import BaseModel
-    from pydantic._internal._dataclasses import PydanticDataclass
-
 
 class DeferredClassGetitem(TypedDict):
     kind: Literal['class_getitem']
     item: Any
 
 
 class DeferredReplaceTypes(TypedDict):
@@ -45,15 +41,15 @@
     """
     No-op marker class for (recursive) type references.
 
     Most of the logic here exists to handle recursive generics.
     """
 
     schema: core_schema.CoreSchema
-    model: type[BaseModel] | type[PydanticDataclass]
+    model: type[Any]
     deferred_actions: tuple[DeferredAction, ...] = ()
 
     __name__ = 'PydanticForwardRef'
     __hash__ = object.__hash__
 
     def __call__(self) -> None:
         """
@@ -65,18 +61,18 @@
         updated_actions = self.deferred_actions + ({'kind': 'class_getitem', 'item': item},)
         return replace(self, deferred_actions=updated_actions)
 
     def replace_types(self, typevars_map: Any) -> PydanticForwardRef:
         updated_actions = self.deferred_actions + ({'kind': 'replace_types', 'typevars_map': typevars_map},)
         return replace(self, deferred_actions=updated_actions)
 
-    def resolve_model(self) -> type[BaseModel] | type[PydanticDataclass] | PydanticForwardRef:
+    def resolve_model(self) -> type[Any] | PydanticForwardRef:
         from ._generics import replace_types
 
-        model: type[BaseModel] | type[PydanticDataclass] | PydanticForwardRef = self.model
+        model: type[Any] | PydanticForwardRef = self.model
         for action in self.deferred_actions:
             if action['kind'] == 'replace_types':
                 model = replace_types(model, action['typevars_map'])
             elif action['kind'] == 'class_getitem':
                 model = model[action['item']]  # type: ignore[index]
             else:
                 raise ValueError(f'Unexpected action: {action}')
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_generate_schema.py` & `pydantic-2.0a3/pydantic/_internal/_generate_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,85 @@
 """
 Convert python types to pydantic-core schema.
 """
 from __future__ import annotations as _annotations
 
 import collections.abc
 import dataclasses
+import inspect
 import re
 import sys
 import typing
 import warnings
+from functools import partial
+from inspect import Parameter, _ParameterKind, signature
 from itertools import chain
+from types import FunctionType, LambdaType, MethodType
 from typing import TYPE_CHECKING, Any, Callable, ForwardRef, Iterable, Mapping, TypeVar, Union
 
 from annotated_types import BaseMetadata, GroupedMetadata
-from pydantic_core import SchemaError, SchemaValidator, core_schema
+from pydantic_core import CoreSchema, SchemaError, SchemaValidator, core_schema
 from typing_extensions import Annotated, Final, Literal, TypedDict, get_args, get_origin, is_typeddict
 
-from pydantic.annotated_arguments import AfterValidator, BeforeValidator, PlainSerializer, WrapSerializer, WrapValidator
-
 from ..errors import PydanticSchemaGenerationError, PydanticUndefinedAnnotation, PydanticUserError
 from ..fields import FieldInfo
 from ..json_schema import JsonSchemaValue, update_json_schema
 from . import _discriminated_union, _typing_extra
 from ._config import ConfigWrapper
 from ._core_metadata import CoreMetadataHandler, build_metadata_dict
 from ._core_utils import (
     consolidate_refs,
     define_expected_missing_refs,
     get_type_ref,
     is_list_like_schema_with_items_schema,
     remove_unnecessary_invalid_definitions,
 )
 from ._decorators import (
+    ComputedFieldInfo,
     Decorator,
     DecoratorInfos,
     FieldSerializerDecoratorInfo,
     FieldValidatorDecoratorInfo,
     ModelSerializerDecoratorInfo,
     ModelValidatorDecoratorInfo,
     RootValidatorDecoratorInfo,
     ValidatorDecoratorInfo,
-    make_generic_serializer,
-    make_generic_validator,
+    inspect_field_serializer,
+    inspect_model_serializer,
+    inspect_validator,
+)
+from ._fields import (
+    PydanticGeneralMetadata,
+    PydanticMetadata,
+    Undefined,
+    collect_dataclass_fields,
+    get_type_hints_infer_globalns,
 )
-from ._fields import PydanticGeneralMetadata, PydanticMetadata, Undefined, collect_fields, get_type_hints_infer_globalns
 from ._forward_ref import PydanticForwardRef, PydanticRecursiveRef
-from ._generics import recursively_defined_type_refs, replace_types
+from ._generics import get_standard_typevars_map, recursively_defined_type_refs, replace_types
 from ._typing_extra import is_finalvar
+from ._utils import lenient_issubclass
 
 if TYPE_CHECKING:
+    from ..decorators import FieldValidatorModes
     from ..main import BaseModel
     from ._dataclasses import StandardDataclass
 
-__all__ = 'dataclass_schema', 'GenerateSchema'
-
 _SUPPORTS_TYPEDDICT = sys.version_info >= (3, 11)
 
 FieldDecoratorInfo = Union[ValidatorDecoratorInfo, FieldValidatorDecoratorInfo, FieldSerializerDecoratorInfo]
 FieldDecoratorInfoType = TypeVar('FieldDecoratorInfoType', bound=FieldDecoratorInfo)
 AnyFieldDecorator = Union[
     Decorator[ValidatorDecoratorInfo],
     Decorator[FieldValidatorDecoratorInfo],
     Decorator[FieldSerializerDecoratorInfo],
 ]
 
+ModifyCoreSchemaWrapHandler = Callable[[Any], core_schema.CoreSchema]
+
 
 def check_validator_fields_against_field_name(
     info: FieldDecoratorInfo,
     field: str,
 ) -> bool:
     if isinstance(info, ValidatorDecoratorInfo):
         # V1 compat: accept `'*'` as a wildcard that matches all fields
@@ -127,36 +139,14 @@
     elif each_item_validators:
         raise TypeError(
             f"`@validator(..., each_item=True)` cannot be applied to fields with a schema of {schema['type']}"
         )
     return schema
 
 
-def dataclass_schema(
-    cls: type[Any],
-    ref: str,
-    fields: dict[str, FieldInfo],
-    decorators: DecoratorInfos,
-    config_wrapper: ConfigWrapper,
-    types_namespace: dict[str, Any] | None,
-) -> core_schema.CoreSchema:
-    """
-    Generate schema for a dataclass.
-    """
-    # TODO add typevars_map argument when we support generic dataclasses
-    schema_generator = GenerateSchema(config_wrapper, types_namespace)
-    args = [schema_generator.generate_dc_field_schema(k, v, decorators) for k, v in fields.items()]
-    has_post_init = hasattr(cls, '__post_init__')
-    args_schema = core_schema.dataclass_args_schema(cls.__name__, args, collect_init_only=has_post_init)
-    inner_schema = apply_validators(args_schema, decorators.root_validator.values())
-    dc_schema = core_schema.dataclass_schema(cls, inner_schema, post_init=has_post_init, ref=ref)
-    schema = apply_model_serializers(dc_schema, decorators.model_serializer.values())
-    return apply_model_validators(schema, decorators.model_validator.values())
-
-
 class GenerateSchema:
     __slots__ = '_config_wrapper_stack', 'types_namespace', 'typevars_map', 'recursion_cache', 'definitions'
 
     def __init__(
         self,
         config_wrapper: ConfigWrapper,
         types_namespace: dict[str, Any] | None,
@@ -175,15 +165,15 @@
         return self._config_wrapper_stack[-1]
 
     @property
     def arbitrary_types(self) -> bool:
         return self.config_wrapper.arbitrary_types_allowed
 
     def generate_schema(self, obj: Any) -> core_schema.CoreSchema:
-        schema = self._generate_schema(obj)
+        schema = self._generate_schema(obj, from_dunder_get_core_schema=True)
 
         schema = remove_unnecessary_invalid_definitions(schema)
 
         js_modify_function = _get_pydantic_modify_json_schema(obj)
         if js_modify_function is None:
             # Need to do this to handle custom generics:
             if hasattr(obj, '__origin__'):
@@ -197,23 +187,24 @@
             self.definitions[schema_ref] = schema
 
         return schema
 
     def model_schema(self, cls: type[BaseModel]) -> core_schema.CoreSchema:
         """
         Generate schema for a pydantic model.
+
+        Since models generate schemas for themselves this method is public and can be called
+        from within BaseModel's metaclass.
         """
-        from pydantic.main import BaseModel
+        model_ref, schema = self._get_or_cache_recursive_ref(cls)
+        if schema is not None:
+            return schema
 
-        model_ref = get_type_ref(cls)
-        cached_def = self.recursion_cache.get(model_ref)
-        if cached_def is not None:
-            return cached_def
+        from pydantic.main import BaseModel
 
-        self.recursion_cache[model_ref] = core_schema.definition_reference_schema(model_ref)
         fields = cls.model_fields
         decorators = cls.__pydantic_decorators__
         check_decorator_fields_exist(
             chain(
                 decorators.field_validator.values(),
                 decorators.field_serializer.values(),
                 decorators.validator.values(),
@@ -223,15 +214,16 @@
         # TODO: we need to do something similar to this for pydantic dataclasses
         #   This should be straight forward once we expose the pydantic config on the dataclass;
         #   I have done this in my PR for dataclasses JSON schema
         config_wrapper = ConfigWrapper(cls.model_config, check=False)
         self._config_wrapper_stack.append(config_wrapper)
         try:
             fields_schema: core_schema.CoreSchema = core_schema.typed_dict_schema(
-                {k: self.generate_td_field_schema(k, v, decorators) for k, v in fields.items()},
+                {k: self._generate_td_field_schema(k, v, decorators) for k, v in fields.items()},
+                computed_fields=generate_computed_field(decorators.computed_fields),
                 return_fields_set=True,
             )
         finally:
             self._config_wrapper_stack.pop()
         inner_schema = apply_validators(fields_schema, decorators.root_validator.values())
 
         inner_schema = consolidate_refs(inner_schema)
@@ -252,29 +244,42 @@
         return apply_model_validators(schema, decorators.model_validator.values())
 
     def _generate_schema_from_property(self, obj: Any, source: Any) -> core_schema.CoreSchema | None:
         """
         Try to generate schema from either the `__get_pydantic_core_schema__` function or
         `__pydantic_core_schema__` property.
 
-        Note: `__get_pydantic_core_schema__` takes priority so it can decide whether to use a `__pydantic_core_schema__`
-        attribute, or generate a fresh schema.
+        Note: `__get_pydantic_core_schema__` takes priority so it can
+        decide whether to use a `__pydantic_core_schema__` attribute, or generate a fresh schema.
         """
         get_schema = getattr(obj, '__get_pydantic_core_schema__', None)
         if get_schema is not None:
+            # (source) -> CoreSchema
+            if len(inspect.signature(get_schema).parameters) == 1:
+                return get_schema(source)
+
+            # (source, handler) -> CoreSchema
+            def handler(source: Any) -> core_schema.CoreSchema:
+                return self._generate_schema(source, False)
+
             # Can return None to tell pydantic not to override
-            return get_schema(source=source, gen_schema=self)
+            return get_schema(source, handler)
+
+        if _typing_extra.is_dataclass(obj):
+            # For dataclasses, only use the __pydantic_core_schema__ if it is defined on this exact class, not a parent
+            schema_property = obj.__dict__.get('__pydantic_core_schema__')
+        else:
+            schema_property = getattr(obj, '__pydantic_core_schema__', None)
 
-        schema_property = getattr(obj, '__pydantic_core_schema__', None)
         if schema_property is not None:
             return schema_property
 
         return None
 
-    def _generate_schema(self, obj: Any) -> core_schema.CoreSchema:  # noqa: C901
+    def _generate_schema(self, obj: Any, from_dunder_get_core_schema: bool) -> core_schema.CoreSchema:  # noqa: C901
         """
         Recursively generate a pydantic-core schema for any supported python type.
         """
         if isinstance(obj, str):
             return {'type': obj}  # type: ignore[return-value,misc]
         elif isinstance(obj, dict):
             # we assume this is already a valid schema
@@ -295,17 +300,23 @@
             # if obj is still a ForwardRef, it means we can't evaluate it, raise PydanticUndefinedAnnotation
             if isinstance(obj, ForwardRef):
                 raise PydanticUndefinedAnnotation(obj.__forward_arg__, f'Unable to evaluate forward reference {obj}')
 
             if self.typevars_map is not None:
                 obj = replace_types(obj, self.typevars_map)
 
-        from_property = self._generate_schema_from_property(obj, obj)
-        if from_property is not None:
-            return from_property
+        if from_dunder_get_core_schema:
+            from_property = self._generate_schema_from_property(obj, obj)
+            if from_property is not None:
+                return from_property
+
+        from pydantic.main import BaseModel
+
+        if lenient_issubclass(obj, BaseModel):
+            return self.model_schema(obj)
 
         if isinstance(obj, PydanticRecursiveRef):
             return core_schema.definition_reference_schema(schema_ref=obj.type_ref)
 
         if isinstance(obj, PydanticForwardRef):
             if not obj.deferred_actions:
                 return obj.schema
@@ -345,14 +356,16 @@
         elif _typing_extra.is_namedtuple(obj):
             return self._namedtuple_schema(obj)
         elif _typing_extra.is_new_type(obj):
             # NewType, can't use isinstance because it fails <3.7
             return self.generate_schema(obj.__supertype__)
         elif obj == re.Pattern:
             return self._pattern_schema(obj)
+        elif obj is collections.abc.Hashable or obj is typing.Hashable:
+            return self._hashable_schema()
         elif isinstance(obj, type):
             if obj is dict:
                 return self._dict_schema(obj)
             if issubclass(obj, dict):
                 # TODO: We would need to handle generic subclasses of certain typing dict subclasses here
                 #   This includes subclasses of typing.Counter, typing.DefaultDict, and typing.OrderedDict
                 #   Note also that we may do a better job of handling typing.DefaultDict by inspecting its arguments.
@@ -360,33 +373,45 @@
             # probably need to take care of other subclasses here
         elif isinstance(obj, typing.TypeVar):
             return self._unsubstituted_typevar_schema(obj)
         elif is_finalvar(obj):
             if obj is Final:
                 return core_schema.AnySchema(type='any')
             return self.generate_schema(get_args(obj)[0])
+        elif isinstance(obj, (FunctionType, LambdaType, MethodType, partial)):
+            return self._callable_schema(obj)
 
         # TODO: _std_types_schema iterates over the __mro__ looking for an expected schema.
         #   This will catch subclasses of typing.Deque, preventing us from properly supporting user-defined
         #   generic subclasses. (In principle this would also catch typing.OrderedDict, but that is currently
         #   already getting caught in the `issubclass(obj, dict):` check above.
         std_schema = self._std_types_schema(obj)
         if std_schema is not None:
             return std_schema
 
+        if _typing_extra.is_dataclass(obj):
+            return self._dataclass_schema(obj, None)
+
         origin = get_origin(obj)
         if origin is None:
             if self.arbitrary_types:
                 return core_schema.is_instance_schema(obj)
             else:
                 raise PydanticSchemaGenerationError(
                     f'Unable to generate pydantic-core schema for {obj!r}. '
                     f'Setting `arbitrary_types_allowed=True` in the model_config may prevent this error.'
                 )
 
+        # Need to handle generic dataclasses before looking for the schema properties because attribute accesses
+        # on _GenericAlias delegate to the origin type, so lose the information about the concrete parametrization
+        # As a result, currently, there is no way to cache the schema for generic dataclasses. This may be possible
+        # to resolve by modifying the value returned by `Generic.__class_getitem__`, but that is a dangerous game.
+        if _typing_extra.is_dataclass(origin):
+            return self._dataclass_schema(obj, origin)
+
         from_property = self._generate_schema_from_property(origin, obj)
         if from_property is not None:
             return from_property
 
         if _typing_extra.origin_is_union(origin):
             return self._union_schema(obj)
         elif issubclass(origin, Annotated):  # type: ignore[arg-type]
@@ -439,15 +464,15 @@
                 return core_schema.is_instance_schema(origin)
             else:
                 raise PydanticSchemaGenerationError(
                     f'Unable to generate pydantic-core schema for {obj!r} (origin={origin!r}). '
                     f'Setting `arbitrary_types_allowed=True` in the model_config may prevent this error.'
                 )
 
-    def generate_td_field_schema(
+    def _generate_td_field_schema(
         self,
         name: str,
         field_info: FieldInfo,
         decorators: DecoratorInfos,
         *,
         required: bool = True,
     ) -> core_schema.TypedDictField:
@@ -461,15 +486,15 @@
             serialization_exclude=common_field['serialization_exclude'],
             validation_alias=common_field['validation_alias'],
             serialization_alias=common_field['serialization_alias'],
             frozen=common_field['frozen'],
             metadata=common_field['metadata'],
         )
 
-    def generate_dc_field_schema(
+    def _generate_dc_field_schema(
         self,
         name: str,
         field_info: FieldInfo,
         decorators: DecoratorInfos,
     ) -> core_schema.DataclassField:
         """
         Prepare a DataclassField to represent the parameter/field, of a dataclass
@@ -486,19 +511,21 @@
             frozen=common_field['frozen'],
             metadata=common_field['metadata'],
         )
 
     def _common_field_schema(self, name: str, field_info: FieldInfo, decorators: DecoratorInfos) -> _CommonField:
         assert field_info.annotation is not None, 'field_info.annotation should not be None when generating a schema'
 
-        schema = self.generate_schema(field_info.annotation)
+        def generate_schema(source: Any) -> CoreSchema:
+            schema = self.generate_schema(source)
+            if field_info.discriminator is not None:
+                schema = _discriminated_union.apply_discriminator(schema, field_info.discriminator, self.definitions)
+            return schema
 
-        if field_info.discriminator is not None:
-            schema = _discriminated_union.apply_discriminator(schema, field_info.discriminator, self.definitions)
-        schema = apply_annotations(schema, field_info.metadata, self.definitions)
+        schema = apply_annotations(generate_schema, field_info.metadata, self.definitions)(field_info.annotation)
 
         # TODO: remove this V1 compatibility shim once it's deprecated
         # push down any `each_item=True` validators
         # note that this won't work for any Annotated types that get wrapped by a function validator
         # but that's okay because that didn't exist in V1
         this_field_validators = filter_field_decorator_info_by_field(decorators.validator.values(), name)
         if _validators_require_validate_default(this_field_validators):
@@ -561,16 +588,15 @@
         return s
 
     def _annotated_schema(self, annotated_type: Any) -> core_schema.CoreSchema:
         """
         Generate schema for an Annotated type, e.g. `Annotated[int, Field(...)]` or `Annotated[int, Gt(0)]`.
         """
         first_arg, *other_args = get_args(annotated_type)
-        schema = self.generate_schema(first_arg)
-        return apply_annotations(schema, other_args, self.definitions)
+        return apply_annotations(self.generate_schema, other_args, self.definitions)(first_arg)
 
     def _literal_schema(self, literal_type: Any) -> core_schema.LiteralSchema:
         """
         Generate schema for a Literal.
         """
         expected = _typing_extra.all_literal_values(literal_type)
         assert expected, f'literal "expected" cannot be empty, obj={literal_type}'
@@ -588,55 +614,50 @@
         __required_keys__ was added in Python 3.9
         (https://github.com/miss-islington/cpython/blob/1e9939657dd1f8eb9f596f77c1084d2d351172fc/Doc/library/typing.rst?plain=1#L1546-L1548)
         however it is buggy
         (https://github.com/python/typing_extensions/blob/ac52ac5f2cb0e00e7988bae1e2a1b8257ac88d6d/src/typing_extensions.py#L657-L666).
         Hence to avoid creating validators that do not do what users expect we only
         support typing.TypedDict on Python >= 3.11 or typing_extension.TypedDict on all versions
         """
+        typed_dict_ref, schema = self._get_or_cache_recursive_ref(typed_dict_cls)
+        if schema is not None:
+            return schema
+
+        typevars_map = get_standard_typevars_map(typed_dict_cls)
         if origin is not None:
-            typeddict_typevars_map = dict(zip(origin.__parameters__, typed_dict_cls.__args__))
             typed_dict_cls = origin
-        else:
-            typeddict_typevars_map = {}
 
         if not _SUPPORTS_TYPEDDICT and type(typed_dict_cls).__module__ == 'typing':
             raise PydanticUserError(
                 'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.11.',
                 code='typed-dict-version',
             )
 
         required_keys: frozenset[str] = typed_dict_cls.__required_keys__
 
         fields: dict[str, core_schema.TypedDictField] = {}
 
-        obj_ref = f'{typed_dict_cls.__module__}.{typed_dict_cls.__qualname__}:{id(typed_dict_cls)}'
-        if obj_ref in self.recursion_cache:
-            return self.recursion_cache[obj_ref]
-        else:
-            self.recursion_cache[obj_ref] = core_schema.definition_reference_schema(obj_ref)
-
         for field_name, annotation in get_type_hints_infer_globalns(
             typed_dict_cls, localns=self.types_namespace, include_extras=True
         ).items():
-            annotation = replace_types(annotation, typeddict_typevars_map)
+            annotation = replace_types(annotation, typevars_map)
             required = field_name in required_keys
 
             if get_origin(annotation) == _typing_extra.Required:
                 required = True
                 annotation = get_args(annotation)[0]
             elif get_origin(annotation) == _typing_extra.NotRequired:
                 required = False
                 annotation = get_args(annotation)[0]
 
             field_info = FieldInfo.from_annotation(annotation)
-            fields[field_name] = self.generate_td_field_schema(
+            fields[field_name] = self._generate_td_field_schema(
                 field_name, field_info, DecoratorInfos(), required=required
             )
 
-        typed_dict_ref = get_type_ref(typed_dict_cls)
         return core_schema.typed_dict_schema(
             fields,
             extra_behavior='forbid',
             ref=typed_dict_ref,
             metadata=build_metadata_dict(
                 js_modify_function=lambda s: update_json_schema(s, {'title': typed_dict_cls.__name__}),
             ),
@@ -663,29 +684,39 @@
         )
         return core_schema.call_schema(arguments_schema, namedtuple_cls)
 
     def _generate_parameter_schema(
         self,
         name: str,
         annotation: type[Any],
+        default: Any = Parameter.empty,
         mode: Literal['positional_only', 'positional_or_keyword', 'keyword_only'] | None = None,
     ) -> core_schema.ArgumentsParameter:
         """
-        Prepare a ArgumentsParameter to represent a field in a namedtuple, dataclass or function signature.
+        Prepare a ArgumentsParameter to represent a field in a namedtuple or function signature.
         """
-        field = FieldInfo.from_annotation(annotation)
+        if default is Parameter.empty:
+            field = FieldInfo.from_annotation(annotation)
+        else:
+            field = FieldInfo.from_annotated_attribute(annotation, default)
         assert field.annotation is not None, 'field.annotation should not be None when generating a schema'
-        schema = self.generate_schema(field.annotation)
-        schema = apply_annotations(schema, field.metadata, self.definitions)
+        schema = apply_annotations(self.generate_schema, field.metadata, self.definitions)(annotation)
+
+        if not field.is_required():
+            schema = wrap_default(field, schema)
 
         parameter_schema = core_schema.arguments_parameter(name, schema)
         if mode is not None:
             parameter_schema['mode'] = mode
         if field.alias is not None:
             parameter_schema['alias'] = field.alias
+        else:
+            alias_generator = self.config_wrapper.alias_generator
+            if alias_generator:
+                parameter_schema['alias'] = alias_generator(name)
         return parameter_schema
 
     def _generic_collection_schema(
         self, parent_type: type[Any], type_: type[Any], origin: type[Any]
     ) -> core_schema.CoreSchema:
         """
         Generate schema for List, Set, and FrozenSet, possibly parameterized.
@@ -865,16 +896,16 @@
 
         return core_schema.generator_schema(self.generate_schema(item_type))
 
     def _pattern_schema(self, pattern_type: Any) -> core_schema.CoreSchema:
         from . import _serializers, _validators
 
         metadata = build_metadata_dict(js_override={'type': 'string', 'format': 'regex'})
-        ser = core_schema.general_plain_serializer_function_ser_schema(
-            _serializers.pattern_serializer, json_return_type='str'
+        ser = core_schema.plain_serializer_function_ser_schema(
+            _serializers.pattern_serializer, info_arg=True, json_return_type='str'
         )
         if pattern_type == typing.Pattern or pattern_type == re.Pattern:
             # bare type
             return core_schema.general_plain_validator_function(
                 _validators.pattern_either_validator, serialization=ser, metadata=metadata
             )
 
@@ -886,95 +917,193 @@
         elif param == bytes:
             return core_schema.general_plain_validator_function(
                 _validators.pattern_bytes_validator, serialization=ser, metadata=metadata
             )
         else:
             raise PydanticSchemaGenerationError(f'Unable to generate pydantic-core schema for {pattern_type!r}.')
 
+    def _hashable_schema(self) -> core_schema.CoreSchema:
+        return core_schema.custom_error_schema(
+            core_schema.is_instance_schema(collections.abc.Hashable),
+            custom_error_type='is_hashable',
+            custom_error_message='Input should be hashable',
+        )
+
     def _std_types_schema(self, obj: Any) -> core_schema.CoreSchema | None:
         """
         Generate schema for types in the standard library.
         """
         if not isinstance(obj, type):
             return None
 
         # Import here to avoid the extra import time earlier since _std_validators imports lots of things globally
-        import dataclasses
-
         from ._std_types_schema import SCHEMA_LOOKUP
 
         # instead of iterating over a list and calling is_instance, this should be somewhat faster,
         # especially as it should catch most types on the first iteration
         # (same as we do/used to do in json encoding)
         for base in obj.__mro__[:-1]:
             try:
                 encoder = SCHEMA_LOOKUP[base]
             except KeyError:
                 continue
             return encoder(self, obj)
-        if dataclasses.is_dataclass(obj):
-            return self._dataclass_schema(obj)  # type: ignore
         return None
 
-    def _dataclass_schema(self, dataclass: type[StandardDataclass]) -> core_schema.CoreSchema:
+    def _dataclass_schema(
+        self, dataclass: type[StandardDataclass], origin: type[StandardDataclass] | None
+    ) -> core_schema.CoreSchema:
         """
         Generate schema for a dataclass.
         """
-        # FIXME we need a way to make sure kw_only info is propagated through to fields
-        fields, _ = collect_fields(
-            dataclass, dataclass.__bases__, self.types_namespace, dc_kw_only=True, is_dataclass=True
-        )
+        dataclass_ref, schema = self._get_or_cache_recursive_ref(dataclass)
+        if schema is not None:
+            return schema
 
-        return dataclass_schema(
-            dataclass,
-            get_type_ref(dataclass),
-            fields,
-            # FIXME we need to get validators and serializers from the dataclasses
-            DecoratorInfos(),
-            self.config_wrapper,
-            self.types_namespace,
+        typevars_map = get_standard_typevars_map(dataclass)
+        if origin is not None:
+            dataclass = origin
+
+        from ._dataclasses import is_pydantic_dataclass
+
+        if is_pydantic_dataclass(dataclass):
+            fields = dataclass.__pydantic_fields__
+            if typevars_map:
+                for field in fields.values():
+                    field.apply_typevars_map(typevars_map, self.types_namespace)
+        else:
+            fields = collect_dataclass_fields(
+                dataclass,
+                self.types_namespace,
+                typevars_map=typevars_map,
+            )
+        decorators = getattr(dataclass, '__pydantic_decorators__', None) or DecoratorInfos()
+        args = [self._generate_dc_field_schema(k, v, decorators) for k, v in fields.items()]
+        has_post_init = hasattr(dataclass, '__post_init__')
+        args_schema = core_schema.dataclass_args_schema(
+            dataclass.__name__,
+            args,
+            computed_fields=generate_computed_field(decorators.computed_fields),
+            collect_init_only=has_post_init,
+        )
+        inner_schema = apply_validators(args_schema, decorators.root_validator.values())
+        dc_schema = core_schema.dataclass_schema(dataclass, inner_schema, post_init=has_post_init, ref=dataclass_ref)
+        schema = apply_model_serializers(dc_schema, decorators.model_serializer.values())
+        return apply_model_validators(schema, decorators.model_validator.values())
+
+    def _callable_schema(self, function: Callable[..., Any]) -> core_schema.CallSchema:
+        """
+        Generate schema for a Callable.
+
+        TODO support functional validators once we support them in Config
+        """
+        sig = signature(function)
+
+        type_hints = _typing_extra.get_function_type_hints(function)
+
+        mode_lookup: dict[_ParameterKind, Literal['positional_only', 'positional_or_keyword', 'keyword_only']] = {
+            Parameter.POSITIONAL_ONLY: 'positional_only',
+            Parameter.POSITIONAL_OR_KEYWORD: 'positional_or_keyword',
+            Parameter.KEYWORD_ONLY: 'keyword_only',
+        }
+
+        arguments_list: list[core_schema.ArgumentsParameter] = []
+        var_args_schema: core_schema.CoreSchema | None = None
+        var_kwargs_schema: core_schema.CoreSchema | None = None
+
+        for i, (name, p) in enumerate(sig.parameters.items()):
+            if p.annotation is sig.empty:
+                annotation = Any
+            else:
+                annotation = type_hints[name]
+
+            parameter_mode = mode_lookup.get(p.kind)
+            if parameter_mode is not None:
+                arg_schema = self._generate_parameter_schema(name, annotation, p.default, parameter_mode)
+                arguments_list.append(arg_schema)
+            elif p.kind == Parameter.VAR_POSITIONAL:
+                var_args_schema = self.generate_schema(annotation)
+            else:
+                assert p.kind == Parameter.VAR_KEYWORD, p.kind
+                var_kwargs_schema = self.generate_schema(annotation)
+
+        return_schema: core_schema.CoreSchema | None = None
+        config_wrapper = self.config_wrapper
+        if config_wrapper.validate_return:
+            return_hint = type_hints.get('return')
+            if return_hint is not None:
+                return_schema = self.generate_schema(return_hint)
+
+        return core_schema.call_schema(
+            core_schema.arguments_schema(
+                arguments_list,
+                var_args_schema=var_args_schema,
+                var_kwargs_schema=var_kwargs_schema,
+                populate_by_name=config_wrapper.populate_by_name,
+            ),
+            function,
+            return_schema=return_schema,
         )
 
     def _unsubstituted_typevar_schema(self, typevar: typing.TypeVar) -> core_schema.CoreSchema:
         assert isinstance(typevar, typing.TypeVar)
 
         if typevar.__bound__:
             return self.generate_schema(typevar.__bound__)
         elif typevar.__constraints__:
             return self._union_schema(typing.Union[typevar.__constraints__])  # type: ignore
         else:
             return core_schema.AnySchema(type='any')
 
+    def _get_or_cache_recursive_ref(self, cls: type[Any]) -> tuple[str, core_schema.DefinitionReferenceSchema | None]:
+        obj_ref = get_type_ref(cls)
+        if obj_ref in self.recursion_cache:
+            return obj_ref, self.recursion_cache[obj_ref]
+        else:
+            self.recursion_cache[obj_ref] = core_schema.definition_reference_schema(obj_ref)
+            return obj_ref, None
+
 
 _VALIDATOR_F_MATCH: Mapping[
-    tuple[str, bool], Callable[[Callable[..., Any], core_schema.CoreSchema], core_schema.CoreSchema]
+    tuple[FieldValidatorModes, Literal['no-info', 'general', 'field']],
+    Callable[[Callable[..., Any], core_schema.CoreSchema], core_schema.CoreSchema],
 ] = {
-    ('before', True): core_schema.field_before_validator_function,
-    ('after', True): core_schema.field_after_validator_function,
-    ('plain', True): lambda f, _: core_schema.field_plain_validator_function(f),
-    ('wrap', True): core_schema.field_wrap_validator_function,
-    ('before', False): core_schema.general_before_validator_function,
-    ('after', False): core_schema.general_after_validator_function,
-    ('plain', False): lambda f, _: core_schema.general_plain_validator_function(f),
-    ('wrap', False): core_schema.general_wrap_validator_function,
+    ('before', 'no-info'): core_schema.no_info_before_validator_function,
+    ('after', 'no-info'): core_schema.no_info_after_validator_function,
+    ('plain', 'no-info'): lambda f, _: core_schema.no_info_plain_validator_function(f),
+    ('wrap', 'no-info'): core_schema.no_info_wrap_validator_function,
+    ('before', 'general'): core_schema.general_before_validator_function,
+    ('after', 'general'): core_schema.general_after_validator_function,
+    ('plain', 'general'): lambda f, _: core_schema.general_plain_validator_function(f),
+    ('wrap', 'general'): core_schema.general_wrap_validator_function,
+    ('before', 'field'): core_schema.field_before_validator_function,
+    ('after', 'field'): core_schema.field_after_validator_function,
+    ('plain', 'field'): lambda f, _: core_schema.field_plain_validator_function(f),
+    ('wrap', 'field'): core_schema.field_wrap_validator_function,
 }
 
 
 def apply_validators(
     schema: core_schema.CoreSchema,
     validators: Iterable[Decorator[RootValidatorDecoratorInfo]]
     | Iterable[Decorator[ValidatorDecoratorInfo]]
     | Iterable[Decorator[FieldValidatorDecoratorInfo]],
 ) -> core_schema.CoreSchema:
     """
     Apply validators to a schema.
     """
     for validator in validators:
-        is_field = isinstance(validator.info, (FieldValidatorDecoratorInfo, ValidatorDecoratorInfo))
-        schema = _VALIDATOR_F_MATCH[(validator.info.mode, is_field)](validator.func, schema)
+        info_arg = inspect_validator(validator.func, validator.info.mode)
+        if not info_arg:
+            val_type: Literal['no-info', 'general', 'field'] = 'no-info'
+        elif isinstance(validator.info, (FieldValidatorDecoratorInfo, ValidatorDecoratorInfo)):
+            val_type = 'field'
+        else:
+            val_type = 'general'
+        schema = _VALIDATOR_F_MATCH[(validator.info.mode, val_type)](validator.func, schema)
     return schema
 
 
 def _validators_require_validate_default(validators: Iterable[Decorator[ValidatorDecoratorInfo]]) -> bool:
     """
     In v1, if any of the validators for a field had `always=True`, the default value would be validated.
 
@@ -996,158 +1125,134 @@
 ) -> core_schema.CoreSchema:
     """
     Apply field serializers to a schema.
     """
     if serializers:
         # use the last serializer to make it easy to override a serializer set on a parent model
         serializer = serializers[-1]
+        is_field_serializer, info_arg = inspect_field_serializer(serializer.func, serializer.info.mode)
         if serializer.info.mode == 'wrap':
-            sf = (
-                core_schema.field_wrap_serializer_function_ser_schema
-                if serializer.info.type == 'field'
-                else core_schema.general_wrap_serializer_function_ser_schema
-            )
-            schema['serialization'] = sf(  # type: ignore[operator]
+            schema['serialization'] = core_schema.wrap_serializer_function_ser_schema(
                 serializer.func,
+                is_field_serializer=is_field_serializer,
+                info_arg=info_arg,
                 json_return_type=serializer.info.json_return_type,
                 when_used=serializer.info.when_used,
             )
         else:
             assert serializer.info.mode == 'plain'
-            sf = (
-                core_schema.field_plain_serializer_function_ser_schema
-                if serializer.info.type == 'field'
-                else core_schema.general_plain_serializer_function_ser_schema
-            )
-            schema['serialization'] = sf(  # type: ignore[operator]
+            schema['serialization'] = core_schema.plain_serializer_function_ser_schema(
                 serializer.func,
+                is_field_serializer=is_field_serializer,
+                info_arg=info_arg,
                 json_return_type=serializer.info.json_return_type,
                 when_used=serializer.info.when_used,
             )
     return schema
 
 
 def apply_model_serializers(
     schema: core_schema.CoreSchema, serializers: Iterable[Decorator[ModelSerializerDecoratorInfo]]
 ) -> core_schema.CoreSchema:
     """
     Apply model serializers to a schema.
     """
     if serializers:
         serializer = list(serializers)[-1]
-
+        info_arg = inspect_model_serializer(serializer.func, serializer.info.mode)
         if serializer.info.mode == 'wrap':
-            ser_schema: core_schema.SerSchema = core_schema.general_wrap_serializer_function_ser_schema(
+            ser_schema: core_schema.SerSchema = core_schema.wrap_serializer_function_ser_schema(
                 serializer.func,
+                info_arg=info_arg,
                 json_return_type=serializer.info.json_return_type,
             )
         else:
             # plain
-            ser_schema = core_schema.general_plain_serializer_function_ser_schema(
+            ser_schema = core_schema.plain_serializer_function_ser_schema(
                 serializer.func,
+                info_arg=info_arg,
                 json_return_type=serializer.info.json_return_type,
             )
         schema['serialization'] = ser_schema
     return schema
 
 
 def apply_model_validators(
     schema: core_schema.CoreSchema, validators: Iterable[Decorator[ModelValidatorDecoratorInfo]]
 ) -> core_schema.CoreSchema:
     """
     Apply model validators to a schema.
     """
     for validator in validators:
+        info_arg = inspect_validator(validator.func, validator.info.mode)
         if validator.info.mode == 'wrap':
-            schema = core_schema.general_wrap_validator_function(
-                function=validator.func,
-                schema=schema,
-            )
+            if info_arg:
+                schema = core_schema.general_wrap_validator_function(function=validator.func, schema=schema)
+            else:
+                schema = core_schema.no_info_wrap_validator_function(function=validator.func, schema=schema)
         elif validator.info.mode == 'before':
-            schema = core_schema.general_before_validator_function(
-                function=validator.func,
-                schema=schema,
-            )
+            if info_arg:
+                schema = core_schema.general_before_validator_function(function=validator.func, schema=schema)
+            else:
+                schema = core_schema.no_info_before_validator_function(function=validator.func, schema=schema)
         else:
             assert validator.info.mode == 'after'
-            schema = core_schema.general_after_validator_function(
-                function=validator.func,
-                schema=schema,
-            )
+            if info_arg:
+                schema = core_schema.general_after_validator_function(function=validator.func, schema=schema)
+            else:
+                schema = core_schema.no_info_after_validator_function(function=validator.func, schema=schema)
     return schema
 
 
 def apply_annotations(
-    schema: core_schema.CoreSchema, annotations: typing.Iterable[Any], definitions: dict[str, core_schema.CoreSchema]
-) -> core_schema.CoreSchema:
+    get_inner_schema: ModifyCoreSchemaWrapHandler,
+    annotations: typing.Iterable[Any],
+    definitions: dict[str, core_schema.CoreSchema],
+) -> ModifyCoreSchemaWrapHandler:
     """
     Apply arguments from `Annotated` or from `FieldInfo` to a schema.
     """
-    handler = CoreMetadataHandler(schema)
     for metadata in annotations:
-        schema = apply_single_annotation(schema, metadata, definitions)
+        if metadata is None:
+            continue
+        get_inner_schema = get_wrapped_inner_schema(get_inner_schema, metadata, definitions)
 
-        metadata_js_modify_function = _get_pydantic_modify_json_schema(metadata)
-        handler.compose_js_modify_functions(metadata_js_modify_function)
+    return get_inner_schema
 
-    return schema
 
+def get_wrapped_inner_schema(
+    get_inner_schema: ModifyCoreSchemaWrapHandler, metadata: Any, definitions: dict[str, core_schema.CoreSchema]
+) -> Callable[[Any], core_schema.CoreSchema]:
+    metadata_get_schema = getattr(metadata, '__get_pydantic_core_schema__', None) or (
+        lambda source, handler: handler(source)
+    )
 
-def apply_single_annotation(  # noqa C901
-    schema: core_schema.CoreSchema, metadata: Any, definitions: dict[str, core_schema.CoreSchema]
-) -> core_schema.CoreSchema:
-    if metadata is None:
+    def _new_inner_schema_handler(source: Any) -> core_schema.CoreSchema:
+        schema = metadata_get_schema(source, get_inner_schema)
+        schema = apply_single_annotation(schema, metadata, definitions)
+        metadata_js_modify_function = _get_pydantic_modify_json_schema(metadata)
+        CoreMetadataHandler(schema).compose_js_modify_functions(metadata_js_modify_function)
         return schema
 
-    metadata_schema = getattr(metadata, '__pydantic_core_schema__', None)
-    if metadata_schema is not None:
-        return metadata_schema
-
-    metadata_get_schema = getattr(metadata, '__get_pydantic_core_schema__', None)
-    if metadata_get_schema is not None:
-        return metadata_get_schema(schema)
+    return _new_inner_schema_handler
+
 
+def apply_single_annotation(
+    schema: core_schema.CoreSchema, metadata: Any, definitions: dict[str, core_schema.CoreSchema]
+) -> core_schema.CoreSchema:
     if isinstance(metadata, GroupedMetadata):
-        # GroupedMetadata yields `BaseMetadata`s
-        return apply_annotations(schema, metadata, definitions)
+        for a in metadata:
+            schema = apply_single_annotation(schema, a, definitions)
     elif isinstance(metadata, FieldInfo):
-        schema = apply_annotations(schema, metadata.metadata, definitions)
+        for field_metadata in metadata.metadata:
+            schema = apply_single_annotation(schema, field_metadata, definitions)
         if metadata.discriminator is not None:
             schema = _discriminated_union.apply_discriminator(schema, metadata.discriminator, definitions)
         # TODO setting a default here needs to be tested
         return wrap_default(metadata, schema)
-    elif isinstance(metadata, AfterValidator):
-        return core_schema.general_after_validator_function(
-            make_generic_validator(metadata.func, mode='after'),
-            schema=schema,
-        )
-    elif isinstance(metadata, BeforeValidator):
-        return core_schema.general_before_validator_function(
-            make_generic_validator(metadata.func, mode='before'),
-            schema=schema,
-        )
-    elif isinstance(metadata, WrapValidator):
-        return core_schema.general_wrap_validator_function(
-            make_generic_validator(metadata.func, mode='wrap'),
-            schema=schema,
-        )
-    elif isinstance(metadata, PlainSerializer):
-        schema['serialization'] = core_schema.general_plain_serializer_function_ser_schema(
-            function=make_generic_serializer(metadata.func, mode='plain', type='general'),
-            json_return_type=metadata.json_return_type,
-            when_used=metadata.when_used,
-        )
-        return schema
-    elif isinstance(metadata, WrapSerializer):
-        schema['serialization'] = core_schema.general_wrap_serializer_function_ser_schema(
-            function=make_generic_serializer(metadata.func, mode='wrap', type='general'),
-            json_return_type=metadata.json_return_type,
-            when_used=metadata.when_used,
-        )
-        return schema
 
     if isinstance(metadata, PydanticGeneralMetadata):
         metadata_dict = metadata.__dict__
     elif isinstance(metadata, (BaseMetadata, PydanticMetadata)):
         metadata_dict = dataclasses.asdict(metadata)  # type: ignore[call-overload]
     elif isinstance(metadata, type) and issubclass(metadata, PydanticMetadata):
         # also support PydanticMetadata classes being used without initialisation,
@@ -1244,7 +1349,19 @@
         'schema': schema,
         'validation_alias': validation_alias,
         'serialization_alias': serialization_alias,
         'serialization_exclude': serialization_exclude,
         'frozen': frozen,
         'metadata': metadata,
     }
+
+
+def generate_computed_field(d: dict[str, Decorator[ComputedFieldInfo]]) -> list[core_schema.ComputedField] | None:
+    r = [
+        core_schema.computed_field(
+            d.cls_var_name,
+            json_return_type=d.info.json_return_type,
+            alias=d.info.alias,
+        )
+        for d in d.values()
+    ]
+    return r
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_generics.py` & `pydantic-2.0a3/pydantic/_internal/_generics.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,19 +210,43 @@
 def get_origin(v: Any) -> Any:
     pydantic_generic_metadata: PydanticGenericMetadata | None = getattr(v, '__pydantic_generic_metadata__', None)
     if pydantic_generic_metadata:
         return pydantic_generic_metadata.get('origin')
     return typing_extensions.get_origin(v)
 
 
-def get_typevars_map(origin: type[Any] | None, args: tuple[type[Any], ...]) -> dict[TypeVarType, type[Any]]:
+def get_standard_typevars_map(cls: type[Any]) -> dict[TypeVarType, Any] | None:
     """
-    Builds the mapping of typevars to argument values in a manner consistent with how the `typing` library,
-    but correctly handles the case where the origin is a generic BaseModel subclass.
+    Package a generic type's typevars and parametrization (if present) into a dictionary compatible with the
+    `replace_types` function. Specifically, this works with standard typing generics and typing._GenericAlias.
     """
+    origin = get_origin(cls)
+    if origin is None:
+        return None
+
+    # In this case, we know that cls is a _GenericAlias, and origin is the generic type
+    # So it is safe to access cls.__args__ and origin.__parameters__
+    args: tuple[Any, ...] = cls.__args__  # type: ignore
+    parameters: tuple[TypeVarType, ...] = origin.__parameters__  # type: ignore
+    return dict(zip(parameters, args))
+
+
+def get_model_typevars_map(cls: type[BaseModel]) -> dict[TypeVarType, Any] | None:
+    """
+    Package a generic BaseModel's typevars and concrete parametrization (if present) into a dictionary compatible
+    with the `replace_types` function.
+
+    Since BaseModel.__class_getitem__ does not produce a typing._GenericAlias, and the BaseModel generic info is
+    stored in the __pydantic_generic_metadata__ attribute, we need special handling here.
+    """
+    # TODO: This could be unified with `get_standard_typevars_map` if we stored the generic metadata
+    #   in the __origin__, __args__, and __parameters__ attributes of the model.
+    generic_metadata = cls.__pydantic_generic_metadata__
+    origin = generic_metadata['origin']
+    args = generic_metadata['args']
     return dict(zip(iter_contained_typevars(origin), args))
 
 
 def replace_types(type_: Any, type_map: Mapping[Any, Any] | None) -> Any:
     """Return type with all occurrences of `type_map` keys recursively replaced with their values.
 
     :param type_: Any type, class or generic alias
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_model_construction.py` & `pydantic-2.0a3/pydantic/_internal/_model_construction.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,37 @@
 from typing import Any, Callable
 
 from pydantic_core import SchemaSerializer, SchemaValidator
 
 from ..errors import PydanticErrorCodes, PydanticUndefinedAnnotation, PydanticUserError
 from ..fields import FieldInfo, ModelPrivateAttr, PrivateAttr
 from ._config import ConfigWrapper
-from ._decorators import PydanticDecoratorMarker
-from ._fields import Undefined, collect_fields
+from ._decorators import ComputedFieldInfo, PydanticDescriptorProxy
+from ._fields import Undefined, collect_model_fields
 from ._generate_schema import GenerateSchema
-from ._generics import get_typevars_map
-from ._typing_extra import add_module_globals, is_classvar
+from ._generics import get_model_typevars_map
+from ._typing_extra import is_classvar
 from ._utils import ClassAttribute, is_valid_identifier
 
 if typing.TYPE_CHECKING:
     from inspect import Signature
 
     from ..config import ConfigDict
     from ..main import BaseModel
 
-__all__ = 'object_setattr', 'init_private_attributes', 'inspect_namespace', 'MockValidator'
 
-IGNORED_TYPES: tuple[Any, ...] = (FunctionType, property, type, classmethod, staticmethod, PydanticDecoratorMarker)
+IGNORED_TYPES: tuple[Any, ...] = (
+    FunctionType,
+    property,
+    type,
+    classmethod,
+    staticmethod,
+    PydanticDescriptorProxy,
+    ComputedFieldInfo,
+)
 object_setattr = object.__setattr__
 
 
 def init_private_attributes(self: BaseModel, __context: Any) -> None:
     """
     This function is meant to behave like a BaseModel method to initialise private attributes.
 
@@ -69,15 +76,15 @@
             '__root__ models are no longer supported in v2; a migration guide will be added in the near future'
         )
 
     ignored_names: set[str] = set()
     for var_name, value in list(namespace.items()):
         if var_name == 'model_config':
             continue
-        elif isinstance(value, all_ignored_types):
+        elif isinstance(value, all_ignored_types) or value.__class__.__module__ == 'functools':
             ignored_names.add(var_name)
             continue
         elif isinstance(value, ModelPrivateAttr):
             if var_name.startswith('__'):
                 raise NameError(
                     f'Private attributes "{var_name}" must not have dunder names; '
                     'use a single underscore prefix instead.'
@@ -119,66 +126,61 @@
     for ann_name, ann_type in raw_annotations.items():
         if (
             single_underscore(ann_name)
             and ann_name not in private_attributes
             and ann_name not in ignored_names
             and not is_classvar(ann_type)
             and ann_type not in all_ignored_types
+            and ann_type.__module__ != 'functools'
         ):
             private_attributes[ann_name] = PrivateAttr()
 
     return private_attributes
 
 
 def single_underscore(name: str) -> bool:
     return name.startswith('_') and not name.startswith('__')
 
 
-def get_model_types_namespace(cls: type[BaseModel], parent_frame_namespace: dict[str, Any] | None) -> dict[str, Any]:
-    ns = add_module_globals(cls, parent_frame_namespace)
-    ns[cls.__name__] = cls
-    return ns
-
-
 def set_model_fields(cls: type[BaseModel], bases: tuple[type[Any], ...], types_namespace: dict[str, Any]) -> None:
     """
     Collect and set `cls.model_fields` and `cls.__class_vars__`.
     """
-    fields, class_vars = collect_fields(cls, bases, types_namespace)
+    typevars_map = get_model_typevars_map(cls)
+    fields, class_vars = collect_model_fields(cls, bases, types_namespace, typevars_map=typevars_map)
 
     apply_alias_generator(cls.model_config, fields)
     cls.model_fields = fields
     cls.__class_vars__.update(class_vars)
 
 
 def complete_model_class(
     cls: type[BaseModel],
     cls_name: str,
     config_wrapper: ConfigWrapper,
-    types_namespace: dict[str, Any] | None,
     *,
     raise_errors: bool = True,
+    types_namespace: dict[str, Any] | None,
 ) -> bool:
     """
     Finish building a model class.
 
     Returns `True` if the model is successfully completed, else `False`.
 
     This logic must be called after class has been created since validation functions must be bound
     and `get_type_hints` requires a class object.
     """
-    generic_metadata = cls.__pydantic_generic_metadata__
-    typevars_map = get_typevars_map(generic_metadata['origin'], generic_metadata['args'])
+    typevars_map = get_model_typevars_map(cls)
     gen_schema = GenerateSchema(
         config_wrapper,
         types_namespace,
         typevars_map,
     )
     try:
-        schema = gen_schema.generate_schema(cls)
+        schema = cls.__get_pydantic_core_schema__(cls, gen_schema.generate_schema)
     except PydanticUndefinedAnnotation as e:
         if raise_errors:
             raise
         if config_wrapper.undefined_types_warning:
             config_warning_string = (
                 f'`{cls_name}` has an undefined annotation: `{e.name}`. '
                 f'It may be possible to resolve this by setting '
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_repr.py` & `pydantic-2.0a3/pydantic/_internal/_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/pydantic/_internal/_serializers.py` & `pydantic-2.0a3/pydantic/_internal/_serializers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/pydantic/_internal/_std_types_schema.py` & `pydantic-2.0a3/pydantic/_internal/_std_types_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from ._core_utils import get_type_ref
 
 if typing.TYPE_CHECKING:
     from ._generate_schema import GenerateSchema
 
     StdSchemaFunction = Callable[[GenerateSchema, type[Any]], core_schema.CoreSchema]
 
-__all__ = ('SCHEMA_LOOKUP',)
 
 SCHEMA_LOOKUP: dict[type[Any], StdSchemaFunction] = {}
 
 
 def schema_function(type: type[Any]) -> Callable[[StdSchemaFunction], StdSchemaFunction]:
     def wrapper(func: StdSchemaFunction) -> StdSchemaFunction:
         SCHEMA_LOOKUP[type] = func
@@ -60,57 +59,64 @@
 @schema_function(timedelta)
 def timedelta_schema(_schema_generator: GenerateSchema, _t: type[Any]) -> core_schema.TimedeltaSchema:
     return core_schema.TimedeltaSchema(type='timedelta')
 
 
 @schema_function(Enum)
 def enum_schema(_schema_generator: GenerateSchema, enum_type: type[Enum]) -> core_schema.CoreSchema:
+    cases = list(enum_type.__members__.values())
+
+    if not cases:
+        # Use an isinstance check for enums with no cases.
+        # This won't work with serialization or JSON schema, but that's okay -- the most important
+        # use case for this is creating typevar bounds for generics that should be restricted to enums.
+        # This is more consistent than it might seem at first, since you can only subclass enum.Enum
+        # (or subclasses of enum.Enum) if all parent classes have no cases.
+        return core_schema.is_instance_schema(enum_type)
+
+    if len(cases) == 1:
+        expected = repr(cases[0].value)
+    else:
+        expected = ','.join([repr(case.value) for case in cases[:-1]]) + f' or {cases[-1].value!r}'
+
     def to_enum(__input_value: Any, _: core_schema.ValidationInfo) -> Enum:
         try:
             return enum_type(__input_value)
         except ValueError:
-            raise PydanticCustomError('enum', 'Input is not a valid enum member')
+            raise PydanticCustomError('enum', f'Input should be {expected}', {'expected': expected})
 
     enum_ref = get_type_ref(enum_type)
-    literal_schema = core_schema.literal_schema(
-        [m.value for m in enum_type.__members__.values()],
-    )
     description = None if not enum_type.__doc__ else inspect.cleandoc(enum_type.__doc__)
     if description == 'An enumeration.':  # This is the default value provided by enum.EnumMeta.__new__; don't use it
         description = None
     updates = {'title': enum_type.__name__, 'description': description}
     updates = {k: v for k, v in updates.items() if v is not None}
     metadata = build_metadata_dict(
-        js_cs_override=literal_schema.copy(), js_modify_function=lambda s: update_json_schema(s, updates)
+        js_cs_override=core_schema.literal_schema([x.value for x in cases]),
+        js_modify_function=lambda s: update_json_schema(s, updates),
     )
 
-    lax: CoreSchema
-    json_type: Literal['int', 'float', 'str']
+    strict_json_types: set[Literal['int', 'float', 'str']]
+    to_enum_validator = core_schema.general_plain_validator_function(to_enum)
     if issubclass(enum_type, int):
         # this handles `IntEnum`, and also `Foobar(int, Enum)`
         updates['type'] = 'integer'
-        lax = core_schema.chain_schema(
-            [core_schema.int_schema(), literal_schema, core_schema.general_plain_validator_function(to_enum)],
-            metadata=metadata,
-        )
-        json_type = 'int'
+        strict_json_types = {'int'}
+        lax: core_schema.CoreSchema = core_schema.chain_schema([core_schema.int_schema(), to_enum_validator])
     elif issubclass(enum_type, str):
         # this handles `StrEnum` (3.11 only), and also `Foobar(str, Enum)`
         updates['type'] = 'string'
-        lax = core_schema.chain_schema(
-            [core_schema.str_schema(), literal_schema, core_schema.general_plain_validator_function(to_enum)],
-            metadata=metadata,
-        )
-        json_type = 'str'
+        strict_json_types = {'str'}
+        lax = core_schema.chain_schema([core_schema.str_schema(), to_enum_validator])
     else:
-        lax = core_schema.general_after_validator_function(to_enum, literal_schema, metadata=metadata)
-        json_type = 'str'
+        lax = to_enum_validator
+        strict_json_types = {'int', 'float', 'str'}
     return core_schema.lax_or_strict_schema(
         lax_schema=lax,
-        strict_schema=core_schema.is_instance_schema(enum_type, json_types={json_type}),
+        strict_schema=core_schema.is_instance_schema(enum_type, json_types=strict_json_types, json_function=enum_type),
         ref=enum_ref,
         metadata=metadata,
     )
 
 
 @schema_function(Decimal)
 def decimal_schema(_schema_generator: GenerateSchema, _decimal_type: type[Decimal]) -> core_schema.LaxOrStrictSchema:
@@ -211,30 +217,32 @@
         ),
     )
 
 
 def _deque_ser_schema(
     inner_schema: core_schema.CoreSchema | None = None,
 ) -> core_schema.WrapSerializerFunctionSerSchema:
-    return core_schema.general_wrap_serializer_function_ser_schema(
-        _serializers.serialize_deque, schema=inner_schema or core_schema.any_schema()
+    return core_schema.wrap_serializer_function_ser_schema(
+        _serializers.serialize_deque, info_arg=True, schema=inner_schema or core_schema.any_schema()
     )
 
 
 def _deque_any_schema() -> core_schema.LaxOrStrictSchema:
+    metadata = build_metadata_dict(js_cs_override=lambda: core_schema.list_schema(core_schema.any_schema()))
     return core_schema.lax_or_strict_schema(
         lax_schema=core_schema.general_wrap_validator_function(
             _validators.deque_any_validator,
             core_schema.list_schema(),
         ),
         strict_schema=core_schema.general_after_validator_function(
-            lambda x, _: deque(x),
+            lambda x, _: x if isinstance(x, deque) else deque(x),
             core_schema.is_instance_schema(deque, json_types={'list'}),
         ),
         serialization=_deque_ser_schema(),
+        metadata=metadata,
     )
 
 
 @schema_function(deque)
 def deque_schema(schema_generator: GenerateSchema, obj: Any) -> core_schema.CoreSchema:
     if obj == deque:
         # bare `deque` type used as annotation
@@ -250,32 +258,26 @@
         # `Deque[Any]`
         return _deque_any_schema()
     else:
         # `Deque[Something]`
         inner_schema = schema_generator.generate_schema(arg)
         # Use a lambda here so `apply_metadata` is called on the decimal_validator before the override is generated
         metadata = build_metadata_dict(js_cs_override=lambda: core_schema.list_schema(inner_schema))
+        lax_schema = core_schema.general_wrap_validator_function(
+            _validators.deque_typed_validator,
+            core_schema.list_schema(inner_schema, strict=False),
+        )
+
         return core_schema.lax_or_strict_schema(
-            lax_schema=core_schema.general_after_validator_function(
-                _validators.deque_typed_validator,
-                core_schema.list_schema(inner_schema),
-                serialization=_deque_ser_schema(inner_schema),
-                metadata=metadata,
-            ),
+            lax_schema=lax_schema,
             strict_schema=core_schema.chain_schema(
-                [
-                    core_schema.is_instance_schema(deque, json_types={'list'}),
-                    core_schema.list_schema(inner_schema, allow_any_iter=True),
-                    core_schema.general_plain_validator_function(
-                        _validators.deque_typed_validator,
-                    ),
-                ],
-                metadata=metadata,
+                [core_schema.is_instance_schema(deque, json_types={'list'}), lax_schema],
             ),
             serialization=_deque_ser_schema(inner_schema),
+            metadata=metadata,
         )
 
 
 def _ordered_dict_any_schema() -> core_schema.LaxOrStrictSchema:
     return core_schema.lax_or_strict_schema(
         lax_schema=core_schema.general_wrap_validator_function(
             _validators.ordered_dict_any_validator, core_schema.dict_schema()
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_typing_extra.py` & `pydantic-2.0a3/pydantic/_internal/_typing_extra.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,25 @@
 """
 Logic for interacting with type annotations, mostly extensions, shims and hacks to wrap python's typing module.
 """
 from __future__ import annotations as _annotations
 
+import dataclasses
 import sys
 import types
 import typing
 from collections.abc import Callable
+from functools import partial
 from types import GetSetDescriptorType
-from typing import Any, ForwardRef
+from typing import TYPE_CHECKING, Any, ForwardRef
 
-from typing_extensions import Annotated, Final, Literal, get_args, get_origin
+from typing_extensions import Annotated, Final, Literal, TypeGuard, get_args, get_origin
 
-__all__ = (
-    'NoneType',
-    'is_none_type',
-    'is_callable_type',
-    'is_literal_type',
-    'all_literal_values',
-    'is_annotated',
-    'is_namedtuple',
-    'is_new_type',
-    'is_classvar',
-    'is_finalvar',
-    'WithArgsTypes',
-    'typing_base',
-    'origin_is_union',
-    'NotRequired',
-    'Required',
-    'parent_frame_namespace',
-    'get_type_hints',
-    'EllipsisType',
-    'add_module_globals',
-    'get_cls_type_hints_lenient',
-)
+if TYPE_CHECKING:
+    from ._dataclasses import StandardDataclass
 
 try:
     from typing import _TypingBase  # type: ignore[attr-defined]
 except ImportError:
     from typing import _Final as _TypingBase  # type: ignore[attr-defined]
 
 typing_base = _TypingBase
@@ -49,15 +31,15 @@
 else:
     from typing import GenericAlias as TypingGenericAlias  # type: ignore
 
 
 if sys.version_info < (3, 11):
     from typing_extensions import NotRequired, Required
 else:
-    from typing import NotRequired, Required
+    from typing import NotRequired, Required  # noqa: F401
 
 
 if sys.version_info < (3, 10):
 
     def origin_is_union(tp: type[Any] | None) -> bool:
         return tp is typing.Union
 
@@ -71,15 +53,15 @@
     WithArgsTypes = typing._GenericAlias, types.GenericAlias, types.UnionType  # type: ignore[attr-defined]
 
 
 if sys.version_info < (3, 10):
     NoneType = type(None)
     EllipsisType = type(Ellipsis)
 else:
-    from types import EllipsisType as EllipsisType
+    from types import EllipsisType as EllipsisType  # noqa: F401
     from types import NoneType as NoneType
 
 
 NONE_TYPES: tuple[Any, Any, Any] = (None, NoneType, Literal[None])
 
 
 TypeVarType = Any  # since mypy doesn't allow the use of TypeVar as a type
@@ -221,15 +203,15 @@
     # if f_back is None, it's the global module namespace and we don't need to include it here
     if frame.f_back is None:
         return None
     else:
         return frame.f_locals
 
 
-def add_module_globals(obj: Any, globalns: dict[str, Any] | None) -> dict[str, Any]:
+def add_module_globals(obj: Any, globalns: dict[str, Any] | None = None) -> dict[str, Any]:
     module_name = getattr(obj, '__module__', None)
     if module_name:
         try:
             module_globalns = sys.modules[module_name].__dict__
         except KeyError:
             # happens occasionally, see https://github.com/pydantic/pydantic/issues/2363
             pass
@@ -239,41 +221,77 @@
             else:
                 # copy module globals to make sure it can't be updated later
                 return module_globalns.copy()
 
     return globalns or {}
 
 
+def get_cls_types_namespace(cls: type[Any], parent_namespace: dict[str, Any] | None = None) -> dict[str, Any]:
+    ns = add_module_globals(cls, parent_namespace)
+    ns[cls.__name__] = cls
+    return ns
+
+
 def get_cls_type_hints_lenient(obj: Any, globalns: dict[str, Any] | None = None) -> dict[str, Any]:
     """
     Collect annotations from a class, including those from parent classes.
 
-    Unlike `typing.get_type_hints`, this function will not evaluate forward references so won't error if
-    a forward reference is not resolvable.
+    Unlike `typing.get_type_hints`, this function will not error if a forward reference is not resolvable.
     """
     # TODO: Try handling typevars_map here
     hints = {}
     for base in reversed(obj.__mro__):
         ann = base.__dict__.get('__annotations__')
         localns = dict(vars(base))
         if ann is not None and ann is not GetSetDescriptorType:
             for name, value in ann.items():
-                if value is None:
-                    value = NoneType
-                elif isinstance(value, str):
-                    value = _make_forward_ref(value, is_argument=False, is_class=True)  # type: ignore
-
-                try:
-                    hints[name] = typing._eval_type(value, globalns, localns)  # type: ignore[attr-defined]
-                except NameError:
-                    # the point of this function is to be tolerant to this case
-                    hints[name] = value
+                hints[name] = eval_type_lenient(value, globalns, localns)
     return hints
 
 
+def eval_type_lenient(value: Any, globalns: dict[str, Any] | None, localns: dict[str, Any] | None) -> Any:
+    """
+    Behaves like typing._eval_type, except it won't raise an error if a forward reference can't be resolved.
+    """
+    if value is None:
+        value = NoneType
+    elif isinstance(value, str):
+        value = _make_forward_ref(value, is_argument=False, is_class=True)
+
+    try:
+        return typing._eval_type(value, globalns, localns)  # type: ignore
+    except NameError:
+        # the point of this function is to be tolerant to this case
+        return value
+
+
+def get_function_type_hints(function: Callable[..., Any]) -> dict[str, Any]:
+    """
+    Like `typing.get_type_hints`, but doesn't convert `X` to `Optional[X]` if the default value is `None`, also
+    copes with `partial`.
+    """
+
+    if isinstance(function, partial):
+        annotations = function.func.__annotations__
+    else:
+        annotations = function.__annotations__
+
+    globalns = add_module_globals(function)
+    type_hints = {}
+    for name, value in annotations.items():
+        if value is None:
+            value = NoneType
+        elif isinstance(value, str):
+            value = _make_forward_ref(value)
+
+        type_hints[name] = typing._eval_type(value, globalns, None)  # type: ignore
+
+    return type_hints
+
+
 if sys.version_info < (3, 9):
 
     def _make_forward_ref(
         arg: Any,
         is_argument: bool = True,
         *,
         is_class: bool = False,
@@ -441,7 +459,13 @@
 
 else:
 
     def evaluate_fwd_ref(
         ref: ForwardRef, globalns: dict[str, Any] | None = None, localns: dict[str, Any] | None = None
     ) -> Any:
         return ref._evaluate(globalns=globalns, localns=localns, recursive_guard=frozenset())
+
+
+def is_dataclass(_cls: type[Any]) -> TypeGuard[type[StandardDataclass]]:
+    # The dataclasses.is_dataclass function doesn't seem to provide TypeGuard functionality,
+    # so I created this convenience function
+    return dataclasses.is_dataclass(_cls)
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_utils.py` & `pydantic-2.0a3/pydantic/_internal/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,31 +19,14 @@
 from . import _repr, _typing_extra
 
 if typing.TYPE_CHECKING:
     MappingIntStrAny: TypeAlias = 'typing.Mapping[int, Any] | typing.Mapping[str, Any]'
     AbstractSetIntStr: TypeAlias = 'typing.AbstractSet[int] | typing.AbstractSet[str]'
     from ..main import BaseModel
 
-__all__ = (
-    'sequence_like',
-    'lenient_isinstance',
-    'lenient_issubclass',
-    'is_valid_identifier',
-    'deep_update',
-    'update_not_none',
-    'almost_equal_floats',
-    'to_camel',
-    'smart_deepcopy',
-    'ValueItems',
-    'ClassAttribute',
-    'dict_not_none',
-    'AbstractSetIntStr',
-    'MappingIntStrAny',
-    'all_identical',
-)
 
 # these are types that are returned unchanged by deepcopy
 IMMUTABLE_NON_COLLECTIONS_TYPES: set[type[Any]] = {
     int,
     float,
     complex,
     str,
```

### Comparing `pydantic-2.0a2/pydantic/_internal/_validators.py` & `pydantic-2.0a3/pydantic/_internal/_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,16 +332,21 @@
 ) -> deque[Any]:
     if isinstance(__input_value, deque):
         return __input_value
     else:
         return deque(validator(__input_value))
 
 
-def deque_typed_validator(__input_value: list[Any], _: core_schema.ValidationInfo) -> deque[Any]:
-    return deque(__input_value)
+def deque_typed_validator(
+    __input_value: Any, validator: core_schema.ValidatorFunctionWrapHandler, _: core_schema.ValidationInfo
+) -> deque[Any]:
+    if isinstance(__input_value, deque):
+        return deque(validator(__input_value), maxlen=__input_value.maxlen)
+    else:
+        return deque(validator(__input_value))
 
 
 def ordered_dict_any_validator(
     __input_value: Any, validator: core_schema.ValidatorFunctionWrapHandler, _: core_schema.ValidationInfo
 ) -> OrderedDict[Any, Any]:
     if isinstance(__input_value, OrderedDict):
         return __input_value
```

### Comparing `pydantic-2.0a2/pydantic/deprecated/config.py` & `pydantic-2.0a3/pydantic/deprecated/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations as _annotations
 
 import warnings
 from typing import Any
 
+from typing_extensions import deprecated
+
 from .._internal import _config
 
 __all__ = ('BaseConfig',)
 
 
 class _ConfigMetaclass(type):
     def __getattr__(self, item: str) -> Any:
@@ -14,14 +16,15 @@
 
         try:
             return _config.config_defaults[item]
         except KeyError as exc:
             raise AttributeError(f"type object '{self.__name__}' has no attribute {exc}") from exc
 
 
+@deprecated('BaseConfig is deprecated. Use the `pydantic.ConfigDict` instead.')
 class BaseConfig(metaclass=_ConfigMetaclass):
     """
     This class is only retained for backwards compatibility.
 
     The preferred approach going forward is to assign a ConfigDict to the `model_config` attribute of the Model class.
     """
```

### Comparing `pydantic-2.0a2/pydantic/deprecated/copy_internals.py` & `pydantic-2.0a3/pydantic/deprecated/copy_internals.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/pydantic/deprecated/json.py` & `pydantic-2.0a3/pydantic/deprecated/json.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import datetime
+import warnings
 from collections import deque
 from decimal import Decimal
 from enum import Enum
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from pathlib import Path
 from re import Pattern
 from types import GeneratorType
 from typing import Any, Callable, Dict, Type, Union
 from uuid import UUID
 
+from typing_extensions import deprecated
+
 from ..color import Color
 from ..networks import NameEmail
 from ..types import SecretBytes, SecretStr
 
 __all__ = 'pydantic_encoder', 'custom_pydantic_encoder', 'timedelta_isoformat'
 
 
@@ -66,19 +69,21 @@
     SecretBytes: str,
     SecretStr: str,
     set: list,
     UUID: str,
 }
 
 
+@deprecated('pydantic_encoder is deprecated, use pydantic_core.to_jsonable_python instead.')
 def pydantic_encoder(obj: Any) -> Any:
     from dataclasses import asdict, is_dataclass
 
     from ..main import BaseModel
 
+    warnings.warn('pydantic_encoder is deprecated, use BaseModel.model_dump instead.', DeprecationWarning, stacklevel=2)
     if isinstance(obj, BaseModel):
         return obj.model_dump()
     elif is_dataclass(obj):
         return asdict(obj)
 
     # Check the class type and its superclasses for a matching encoder
     for base in obj.__class__.__mro__[:-1]:
@@ -87,27 +92,34 @@
         except KeyError:
             continue
         return encoder(obj)
     else:  # We have exited the for loop without finding a suitable encoder
         raise TypeError(f"Object of type '{obj.__class__.__name__}' is not JSON serializable")
 
 
+# TODO: Add a suggested migration path once there is a way to use custom encoders
+@deprecated('custom_pydantic_encoder is deprecated.')
 def custom_pydantic_encoder(type_encoders: Dict[Any, Callable[[Type[Any]], Any]], obj: Any) -> Any:
     # Check the class type and its superclasses for a matching encoder
+    warnings.warn(
+        'custom_pydantic_encoder is deprecated, use BaseModel.model_dump instead.', DeprecationWarning, stacklevel=2
+    )
     for base in obj.__class__.__mro__[:-1]:
         try:
             encoder = type_encoders[base]
         except KeyError:
             continue
 
         return encoder(obj)
     else:  # We have exited the for loop without finding a suitable encoder
         return pydantic_encoder(obj)
 
 
+@deprecated('timedelta_isoformat is deprecated.')
 def timedelta_isoformat(td: datetime.timedelta) -> str:
     """
     ISO 8601 encoding for Python timedelta object.
     """
+    warnings.warn('timedelta_isoformat is deprecated.', DeprecationWarning, stacklevel=2)
     minutes, seconds = divmod(td.seconds, 60)
     hours, minutes = divmod(minutes, 60)
     return f'{"-" if td.days < 0 else ""}P{abs(td.days)}DT{hours:d}H{minutes:d}M{seconds:d}.{td.microseconds:06d}S'
```

### Comparing `pydantic-2.0a2/pydantic/deprecated/parse.py` & `pydantic-2.0a3/pydantic/deprecated/parse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from __future__ import annotations
 
 import json
 import pickle
+import warnings
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable
 
+from typing_extensions import deprecated
+
 
 class Protocol(str, Enum):
     json = 'json'
     pickle = 'pickle'
 
 
+@deprecated('load_str_bytes is deprecated.')
 def load_str_bytes(
     b: str | bytes,
     *,
     content_type: str | None = None,
     encoding: str = 'utf8',
     proto: Protocol | None = None,
     allow_pickle: bool = False,
     json_loads: Callable[[str], Any] = json.loads,
 ) -> Any:
+    warnings.warn('load_str_bytes is deprecated.', DeprecationWarning, stacklevel=2)
     if proto is None and content_type:
         if content_type.endswith(('json', 'javascript')):
             pass
         elif allow_pickle and content_type.endswith('pickle'):
             proto = Protocol.pickle
         else:
             raise TypeError(f'Unknown content-type: {content_type}')
@@ -40,23 +45,25 @@
             raise RuntimeError('Trying to decode with pickle with allow_pickle=False')
         bb = b if isinstance(b, bytes) else b.encode()
         return pickle.loads(bb)
     else:
         raise TypeError(f'Unknown protocol: {proto}')
 
 
+@deprecated('load_file is deprecated.')
 def load_file(
     path: str | Path,
     *,
     content_type: str | None = None,
     encoding: str = 'utf8',
     proto: Protocol | None = None,
     allow_pickle: bool = False,
     json_loads: Callable[[str], Any] = json.loads,
 ) -> Any:
+    warnings.warn('load_file is deprecated.', DeprecationWarning, stacklevel=2)
     path = Path(path)
     b = path.read_bytes()
     if content_type is None:
         if path.suffix in ('.js', '.json'):
             proto = Protocol.json
         elif path.suffix == '.pkl':
             proto = Protocol.pickle
```

### Comparing `pydantic-2.0a2/requirements/README.md` & `pydantic-2.0a3/requirements/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # requirements
 
 This folder contains requirements files (`*.in` files) that get compiled into lockfiles (`*.txt` files) by [pip-tools].
 
-All of the `*.in` files get collected into `all.in`, which then crates `all.txt`. This `all.txt` functions both as the pip-installable requirements file with all of the requirements and as a [pip constraints file](https://pip.pypa.io/en/stable/user_guide/#constraints-files) for the rest of the lockfiles. This ensures that all of the lockfiles lock to the same version of dependencies and are compatible (that is, you can always install any combination of lockfiles without dependency version conflicts).
-The individual lockfiles, for example `docs.txt`, get produced by combining `docs.in` with `all.txt` via `docs-constrained.in`. This is necessary because pip-tools can only accept lockfiles if they are specified in a requirements file, but we cannot but the reference to `all.txt` in `docs.in` because `docs.in` is used to build `all.txt`.
+All of the `*.in` files get collected into `all.in`, which then creates the `all.txt`. This `all.txt` functions both as the pip-installable requirements file with all of the requirements and as a [pip constraints file](https://pip.pypa.io/en/stable/user_guide/#constraints-files) for the rest of the lockfiles. This ensures that all of the lockfiles lock to the same version of dependencies and are compatible (that is, you can always install any combination of lockfiles without dependency version conflicts).
+The individual lockfiles, for example `docs.txt`, get produced by combining `docs.in` with `all.txt` via `docs-constrained.in`. This is necessary because pip-tools can only accept lockfiles if they are specified in a requirements file, but we cannot reference to `all.txt` in `docs.in` because `docs.in` is used to build `all.txt`.
 
 There are two scripts included: `rebuild.sh` which deletes the lockfiles and rebuilds them from scratch (thus updating all dependencies) and `refresh.sh` which updates the lockfiles to reflect any changes in the `.in` files while minimizing the changes to the lockfiles (i.e. it only updates/changes dependencies that need updating/changing).
 
 [pip-tools]: https://github.com/jazzband/pip-tools
```

### Comparing `pydantic-2.0a2/requirements/all.txt` & `pydantic-2.0a3/requirements/all.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     # via
     #   black
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==2.21.0
     # via -r requirements/linting.in
-pydantic-core==0.23.1
+pydantic-core==0.25.0
     # via
     #   -r requirements/docs.in
     #   -r requirements/linting.in
 pyflakes==3.0.1
     # via autoflake
 pygments==2.14.0
     # via
```

### Comparing `pydantic-2.0a2/requirements/docs.txt` & `pydantic-2.0a3/requirements/docs.txt`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     # via mkdocstrings-python
 mkdocstrings-python==0.9.0
     # via -r requirements/docs.in
 packaging==23.0
     # via
     #   -c requirements/all.txt
     #   mkdocs
-pydantic-core==0.23.1
+pydantic-core==0.25.0
     # via
     #   -c requirements/all.txt
     #   -r requirements/docs.in
 pyflakes==3.0.1
     # via
     #   -c requirements/all.txt
     #   autoflake
```

### Comparing `pydantic-2.0a2/requirements/linting.txt` & `pydantic-2.0a3/requirements/linting.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     #   -c requirements/all.txt
     #   black
     #   virtualenv
 pre-commit==2.21.0
     # via
     #   -c requirements/all.txt
     #   -r requirements/linting.in
-pydantic-core==0.23.1
+pydantic-core==0.25.0
     # via
     #   -c requirements/all.txt
     #   -r requirements/linting.in
 pyupgrade==3.3.1
     # via
     #   -c requirements/all.txt
     #   -r requirements/linting.in
```

### Comparing `pydantic-2.0a2/requirements/pyproject-all.txt` & `pydantic-2.0a3/requirements/pyproject-all.txt`

 * *Files 19% similar despite different names*

```diff
@@ -8,13 +8,13 @@
     # via pydantic (pyproject.toml)
 dnspython==2.3.0
     # via email-validator
 email-validator==1.3.1
     # via pydantic (pyproject.toml)
 idna==3.4
     # via email-validator
-pydantic-core==0.23.1
+pydantic-core==0.25.0
     # via pydantic (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   pydantic (pyproject.toml)
     #   pydantic-core
```

### Comparing `pydantic-2.0a2/requirements/refresh.sh` & `pydantic-2.0a3/requirements/refresh.sh`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/requirements/testing-extra.txt` & `pydantic-2.0a3/requirements/testing-extra.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/requirements/testing-mypy.txt` & `pydantic-2.0a3/requirements/testing-mypy.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/requirements/testing.txt` & `pydantic-2.0a3/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/conftest.py` & `pydantic-2.0a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_abc.py` & `pydantic-2.0a3/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_aliases.py` & `pydantic-2.0a3/tests/test_aliases.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from inspect import signature
 from typing import Any, ContextManager, List, Optional
 
 import pytest
 from dirty_equals import IsStr
 
 from pydantic import BaseModel, ConfigDict, ValidationError
-from pydantic.fields import Field
+from pydantic.fields import AliasChoices, AliasPath, Field
 
 
 def test_alias_generator():
     def to_camel(string: str):
         return ''.join(x.capitalize() for x in string.split('_'))
 
     class MyModel(BaseModel):
@@ -411,7 +411,52 @@
 
     assert Model.model_json_schema() == {
         'properties': {'x_val_alias': {'title': 'X Val Alias', 'type': 'string'}},
         'required': ['x_val_alias'],
         'title': 'Model',
         'type': 'object',
     }
+
+
+@pytest.mark.parametrize(
+    'input,expected',
+    [
+        ('a', 'a'),
+        (AliasPath('a', 'b', 1), ['a', 'b', 1]),
+        (AliasChoices('a', 'b'), [['a'], ['b']]),
+        (AliasChoices('a', AliasPath('b', 1)), [['a'], ['b', 1]]),
+        (AliasChoices(), None),
+    ],
+)
+def test_validation_alias_path(input, expected):
+    class Model(BaseModel):
+        x: str = Field(validation_alias=input)
+
+    assert Model.model_fields['x'].validation_alias == expected
+
+
+def test_validation_alias_invalid_value_type():
+    m = 'Invalid `validation_alias` type. it should be `str`, `AliasChoices`, or `AliasPath`'
+    with pytest.raises(TypeError, match=m):
+
+        class Model(BaseModel):
+            x: str = Field(validation_alias=123)
+
+
+def test_validation_alias_parse_data():
+    class Model(BaseModel):
+        x: str = Field(validation_alias=AliasChoices('a', AliasPath('b', 1), 'c'))
+
+    assert Model.model_fields['x'].validation_alias == [['a'], ['b', 1], ['c']]
+    assert Model.model_validate({'a': 'hello'}).x == 'hello'
+    assert Model.model_validate({'b': ['hello', 'world']}).x == 'world'
+    assert Model.model_validate({'c': 'test'}).x == 'test'
+    with pytest.raises(ValidationError) as exc_info:
+        Model.model_validate({'b': ['hello']})
+    assert exc_info.value.errors() == [
+        {
+            'type': 'missing',
+            'loc': ('a',),
+            'msg': 'Field required',
+            'input': {'b': ['hello']},
+        }
+    ]
```

### Comparing `pydantic-2.0a2/tests/test_assert_in_validators.py` & `pydantic-2.0a3/tests/test_assert_in_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_callable.py` & `pydantic-2.0a3/tests/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_color.py` & `pydantic-2.0a3/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_config.py` & `pydantic-2.0a3/tests/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import re
 import sys
 from contextlib import nullcontext as does_not_raise
-from functools import partial
 from inspect import signature
 from typing import Any, ContextManager, Iterable, NamedTuple, Type, Union, get_type_hints
 
 from dirty_equals import HasRepr
 from pydantic_core import SchemaError
 
 from pydantic import (
     BaseConfig,
     BaseModel,
     Field,
     PrivateAttr,
     PydanticSchemaGenerationError,
     ValidationError,
     create_model,
-    validate_arguments,
+    validate_call,
 )
 from pydantic._internal._config import ConfigWrapper, config_defaults
 from pydantic.config import ConfigDict
 from pydantic.dataclasses import dataclass as pydantic_dataclass
 from pydantic.errors import PydanticUserError
 
 if sys.version_info < (3, 9):
@@ -453,15 +452,15 @@
 
         @pydantic_dataclass(config=config_dict)
         class MyDataclass:
             pass
 
     with pytest.warns(UserWarning, match=re.escape(warning_message)):
 
-        @validate_arguments(config=config_dict)
+        @validate_call(config=config_dict)
         def my_function():
             pass
 
 
 def test_invalid_extra():
     extra_error = re.escape(
         "Input should be 'allow', 'forbid' or 'ignore'"
@@ -479,43 +478,19 @@
 
     with pytest.raises(SchemaError, match='Invalid extra_behavior: `invalid-value`'):
 
         @pydantic_dataclass(config=config_dict)
         class MyDataclass:
             pass
 
-    with pytest.raises(SchemaError, match=extra_error):
-
-        @validate_arguments(config=config_dict)
-        def my_function():
-            pass
-
-    with pytest.raises(SchemaError, match=extra_error):
-        # This case happens when the function passed to `validate_arguments` has no `__name__`.
-        # This is a pretty exotic case, but it has caused issues in the past, so I wanted to add a test.
-        def my_wrapped_function():
-            pass
-
-        my_partial_function = partial(my_wrapped_function)
-        my_partial_function.__annotations__ = my_wrapped_function.__annotations__
-        validate_arguments(config=config_dict)(my_partial_function)
-
 
 def test_invalid_config_keys():
-    with pytest.raises(
-        PydanticUserError,
-        match=re.escape(
-            'Setting the "alias_generator" property on custom Config for'
-            ' @validate_arguments is not yet supported, please remove.'
-        ),
-    ):
-
-        @validate_arguments(config={'alias_generator': lambda x: x})
-        def my_function():
-            pass
+    @validate_call(config={'alias_generator': lambda x: x})
+    def my_function():
+        pass
 
 
 def test_multiple_inheritance_config():
     class Parent(BaseModel):
         model_config = ConfigDict(frozen=True, extra='forbid')
 
     class Mixin(BaseModel):
```

### Comparing `pydantic-2.0a2/tests/test_construction.py` & `pydantic-2.0a3/tests/test_construction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_create_model.py` & `pydantic-2.0a3/tests/test_create_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_dataclasses.py` & `pydantic-2.0a3/tests/test_dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import dataclasses
 import pickle
 import re
 import sys
 from collections.abc import Hashable
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Callable, ClassVar, Dict, FrozenSet, List, Optional, Set, Union
+from typing import Any, Callable, ClassVar, Dict, FrozenSet, Generic, List, Optional, Set, TypeVar, Union
 
 import pytest
+from dirty_equals import HasRepr
 from typing_extensions import Literal
 
 import pydantic
-from pydantic import BaseModel, ConfigDict, FieldValidationInfo, ValidationError
+from pydantic import AnalyzedType, BaseModel, ConfigDict, FieldValidationInfo, ValidationError
 from pydantic.decorators import field_validator
 from pydantic.fields import Field, FieldInfo
 from pydantic.json_schema import model_json_schema
 
 
 def test_simple():
     @pydantic.dataclasses.dataclass
@@ -688,33 +689,47 @@
     class Child(Base):
         b: int
 
     Child(a=1, b=2)
     assert post_init_called
 
 
-@pytest.mark.xfail(reason='support Hashable')
 def test_hashable_required():
     @pydantic.dataclasses.dataclass
     class MyDataclass:
         v: Hashable
 
     MyDataclass(v=None)
     with pytest.raises(ValidationError) as exc_info:
         MyDataclass(v=[])
     assert exc_info.value.errors() == [
-        {'loc': ('v',), 'msg': 'value is not a valid hashable', 'type': 'type_error.hashable'}
+        {'input': [], 'loc': ('v',), 'msg': 'Input should be hashable', 'type': 'is_hashable'}
     ]
-    with pytest.raises(TypeError) as exc_info:
+
+    with pytest.raises(ValidationError) as exc_info:
+        # Should this raise a TypeError instead? https://github.com/pydantic/pydantic/issues/5487
         MyDataclass()
-    assert "__init__() missing 1 required positional argument: 'v'" in str(exc_info.value)
+    assert exc_info.value.errors() == [
+        {'input': HasRepr('ArgsKwargs(())'), 'loc': ('v',), 'msg': 'Field required', 'type': 'missing'}
+    ]
 
 
-@pytest.mark.xfail(reason='support Hashable')
-@pytest.mark.parametrize('default', [1, None, ...])
+@pytest.mark.parametrize(
+    'default',
+    [
+        1,
+        None,
+        pytest.param(
+            ...,
+            marks=pytest.mark.xfail(
+                reason='... makes field required: https://github.com/pydantic/pydantic/issues/5488'
+            ),
+        ),
+    ],
+)
 def test_hashable_optional(default):
     @pydantic.dataclasses.dataclass
     class MyDataclass:
         v: Hashable = default
 
     MyDataclass()
     MyDataclass(v=None)
@@ -962,56 +977,82 @@
     assert restored_obj == obj
 
     # ensure the restored dataclass is still a pydantic dataclass
     with pytest.raises(ValidationError):
         restored_obj.value = 'value of a wrong type'
 
 
-def gen_2162_dataclasses():
-    @dataclasses.dataclass(frozen=True)
-    class StdLibFoo:
-        a: str
-        b: int
+def lazy_cases_for_dataclass_equality_checks():
+    """
+    The reason for the convoluted structure of this function is to avoid
+    creating the classes while collecting tests, which may trigger breakpoints
+    etc. while working on one specific test.
+    """
+    cases = []
 
-    @pydantic.dataclasses.dataclass(frozen=True)
-    class PydanticFoo:
-        a: str
-        b: int
+    def get_cases():
+        if cases:
+            return cases  # cases already "built"
 
-    @dataclasses.dataclass(frozen=True)
-    class StdLibBar:
-        c: StdLibFoo
+        @dataclasses.dataclass(frozen=True)
+        class StdLibFoo:
+            a: str
+            b: int
 
-    @pydantic.dataclasses.dataclass(frozen=True)
-    class PydanticBar:
-        c: PydanticFoo
+        @pydantic.dataclasses.dataclass(frozen=True)
+        class PydanticFoo:
+            a: str
+            b: int
 
-    @dataclasses.dataclass(frozen=True)
-    class StdLibBaz:
-        c: PydanticFoo
+        @dataclasses.dataclass(frozen=True)
+        class StdLibBar:
+            c: StdLibFoo
 
-    @pydantic.dataclasses.dataclass(frozen=True)
-    class PydanticBaz:
-        c: StdLibFoo
+        @pydantic.dataclasses.dataclass(frozen=True)
+        class PydanticBar:
+            c: PydanticFoo
+
+        @dataclasses.dataclass(frozen=True)
+        class StdLibBaz:
+            c: PydanticFoo
+
+        @pydantic.dataclasses.dataclass(frozen=True)
+        class PydanticBaz:
+            c: StdLibFoo
+
+        foo = StdLibFoo(a='Foo', b=1)
+        cases.append((foo, StdLibBar(c=foo)))
+
+        foo = PydanticFoo(a='Foo', b=1)
+        cases.append((foo, PydanticBar(c=foo)))
+
+        foo = PydanticFoo(a='Foo', b=1)
+        cases.append((foo, StdLibBaz(c=foo)))
 
-    foo = StdLibFoo(a='Foo', b=1)
-    yield foo, StdLibBar(c=foo)
+        foo = StdLibFoo(a='Foo', b=1)
+        cases.append((foo, PydanticBaz(c=foo)))
 
-    foo = PydanticFoo(a='Foo', b=1)
-    yield foo, PydanticBar(c=foo)
+        return cases
 
-    foo = PydanticFoo(a='Foo', b=1)
-    yield foo, StdLibBaz(c=foo)
+    case_ids = ['stdlib_stdlib', 'pydantic_pydantic', 'pydantic_stdlib', 'stdlib_pydantic']
 
-    foo = StdLibFoo(a='Foo', b=1)
-    yield foo, PydanticBaz(c=foo)
+    def case(i):
+        def get_foo_bar():
+            return get_cases()[i]
 
+        get_foo_bar.__name__ = case_ids[i]  # get nice names in pytest output
+        return get_foo_bar
 
-@pytest.mark.parametrize('foo,bar', gen_2162_dataclasses())
-def test_issue_2162(foo, bar):
+    return [case(i) for i in range(4)]
+
+
+@pytest.mark.parametrize('foo_bar_getter', lazy_cases_for_dataclass_equality_checks())
+def test_dataclass_equality_for_field_values(foo_bar_getter):
+    # Related to issue #2162
+    foo, bar = foo_bar_getter()
     assert dataclasses.asdict(foo) == dataclasses.asdict(bar.c)
     assert dataclasses.astuple(foo) == dataclasses.astuple(bar.c)
     assert foo == bar.c
 
 
 def test_issue_2383():
     @dataclasses.dataclass
@@ -1365,25 +1406,62 @@
 
     msg = re.escape("Unexpected keyword argument [type=unexpected_keyword_argument, input_value='2', input_type=str]")
 
     with pytest.raises(ValidationError, match=msg):
         Foo(**{'x': '1', 'y': '2'})
 
 
-@pytest.mark.xfail(reason='recursive references need rebuilding?')
+@pytest.mark.xfail(reason='need to make it possible to rebuild dataclasses')
 def test_self_reference_dataclass():
     @pydantic.dataclasses.dataclass
     class MyDataclass:
-        self_reference: 'MyDataclass'
+        self_reference: Optional['MyDataclass'] = None
+
+    # rebuild_pydantic_dataclass(MyDataclass)
+
+    assert MyDataclass.__pydantic_fields__['self_reference'].annotation == Optional[MyDataclass]
+
+    instance = MyDataclass(self_reference=MyDataclass(self_reference=MyDataclass()))
+    assert AnalyzedType(MyDataclass).dump_python(instance) == {
+        'self_reference': {'self_reference': {'self_reference': None}}
+    }
+
+    with pytest.raises(ValidationError) as exc_info:
+        MyDataclass(self_reference=MyDataclass(self_reference=1))
 
-    annotation = MyDataclass.__pydantic_fields__['self_reference'].annotation
-    # Currently, this is true:
-    # assert isinstance(MyDataclass, PydanticForwardRef)
-    # TODO: Probably need a way to "model_rebuild" a dataclass
-    assert annotation is MyDataclass
+    assert exc_info.value.errors() == [
+        {
+            'ctx': {'dataclass_name': 'MyDataclass'},
+            'input': 1,
+            'loc': ('self_reference',),
+            'msg': 'Input should be a dictionary or an instance of MyDataclass',
+            'type': 'dataclass_type',
+        }
+    ]
+
+
+@pytest.mark.xfail(reason='need to make it possible to rebuild dataclasses')
+def test_cyclic_reference_dataclass():
+    @pydantic.dataclasses.dataclass
+    class D1:
+        d2: Optional['D2'] = None
+
+    @pydantic.dataclasses.dataclass
+    class D2:
+        d1: Optional[D1] = None
+
+    # rebuild_pydantic_dataclass(D1)
+
+    instance = D1(d2=D2(d1=D1(d2=D2(d1=D1()))))
+
+    assert AnalyzedType(D1).dump_python(instance) == {...}
+
+    with pytest.raises(ValidationError) as exc_info:
+        D1(d2=D2(d1=D1(d2=D2(d1=D2()))))
+    assert exc_info.value.errors() == [...]
 
 
 @pytest.mark.skipif(sys.version_info < (3, 10), reason='kw_only is not available in python < 3.10')
 def test_kw_only():
     @pydantic.dataclasses.dataclass(kw_only=True)
     class A:
         a: int | None = None
@@ -1663,7 +1741,87 @@
             'ctx': {'error': 'assert -1 > 0'},
             'input': -1,
             'loc': ('x',),
             'msg': 'Assertion failed, assert -1 > 0',
             'type': 'assertion_error',
         }
     ]
+
+
+def dataclass_decorators():
+    def combined(cls):
+        """
+        Should be equivalent to:
+        @pydantic.dataclasses.dataclass
+        @dataclasses.dataclass
+        """
+        return pydantic.dataclasses.dataclass(dataclasses.dataclass(cls))
+
+    decorators = [pydantic.dataclasses.dataclass, dataclasses.dataclass, combined]
+    ids = ['pydantic', 'stdlib', 'combined']
+    # decorators = [pydantic.dataclasses.dataclass]
+    # ids = ['pydantic']
+    # decorators = [dataclasses.dataclass]
+    # ids = ['stdlib']
+    return {'argvalues': decorators, 'ids': ids}
+
+
+@pytest.mark.parametrize('dataclass_decorator', **dataclass_decorators())
+def test_unparametrized_generic_dataclass(dataclass_decorator):
+    T = TypeVar('T')
+
+    @dataclass_decorator
+    class GenericDataclass(Generic[T]):
+        x: T
+
+    # In principle we could call GenericDataclass(...) below, but this won't do validation
+    # for standard dataclasses, so we just use AnalyzedType to get validation for each.
+    validator = pydantic.AnalyzedType(GenericDataclass)
+
+    assert validator.validate_python({'x': None}).x is None
+    assert validator.validate_python({'x': 1}).x == 1
+
+    with pytest.raises(ValidationError) as exc_info:
+        validator.validate_python({'y': None})
+    assert exc_info.value.errors() == [
+        {'input': {'y': None}, 'loc': ('x',), 'msg': 'Field required', 'type': 'missing'}
+    ]
+
+
+@pytest.mark.parametrize('dataclass_decorator', **dataclass_decorators())
+@pytest.mark.parametrize(
+    'annotation,input_value,error,output_value',
+    [
+        (int, 1, False, 1),
+        (str, 'a', False, 'a'),
+        (
+            int,
+            'a',
+            True,
+            [
+                {
+                    'input': 'a',
+                    'loc': ('x',),
+                    'msg': 'Input should be a valid integer, unable to parse string as an ' 'integer',
+                    'type': 'int_parsing',
+                }
+            ],
+        ),
+    ],
+)
+def test_parametrized_generic_dataclass(dataclass_decorator, annotation, input_value, error, output_value):
+    T = TypeVar('T')
+
+    @dataclass_decorator
+    class GenericDataclass(Generic[T]):
+        x: T
+
+    # Need to use AnalyzedType here because GenericDataclass[annotation] will be a GenericAlias, which delegates
+    # method calls to the (non-parametrized) origin class. This is essentially a limitation of typing._GenericAlias.
+    validator = pydantic.AnalyzedType(GenericDataclass[annotation])
+
+    if not error:
+        assert validator.validate_python({'x': input_value}).x == output_value
+    else:
+        with pytest.raises(ValidationError) as exc_info:
+            validator.validate_python({'x': input_value})
+        assert exc_info.value.errors() == output_value
```

### Comparing `pydantic-2.0a2/tests/test_datetime.py` & `pydantic-2.0a3/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_decorator.py` & `pydantic-2.0a3/tests/test_deprecated_validate_arguments.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import asyncio
 import inspect
 import sys
-from datetime import datetime, timezone
 from pathlib import Path
 from typing import List
 
 import pytest
 from dirty_equals import IsInstance
-from typing_extensions import Annotated, TypedDict
+from typing_extensions import Annotated
 
-from pydantic import BaseModel, Field, ValidationError, validate_arguments
-from pydantic.decorator import ValidatedFunction
+from pydantic import BaseModel, Field, ValidationError
+from pydantic.deprecated.decorator import ValidatedFunction
+from pydantic.deprecated.decorator import validate_arguments as validate_arguments_deprecated
 from pydantic.errors import PydanticUserError
 
 skip_pre_38 = pytest.mark.skipif(sys.version_info < (3, 8), reason='testing >= 3.8 behaviour only')
 
 
+def validate_arguments(*args, **kwargs):
+    with pytest.warns(DeprecationWarning, match='^The `validate_arguments` method is deprecated; use `validate_call`'):
+        return validate_arguments_deprecated(*args, **kwargs)
+
+
 def test_args():
     @validate_arguments
     def foo(a: int, b: int):
         return f'{a}, {b}'
 
     assert foo(1, 2) == '1, 2'
     assert foo(*[1, 2]) == '1, 2'
@@ -61,15 +66,15 @@
     @validate_arguments
     def foo_bar(a: int, b: int):
         """This is the foo_bar method."""
         return f'{a}, {b}'
 
     assert foo_bar.__doc__ == 'This is the foo_bar method.'
     assert foo_bar.__name__ == 'foo_bar'
-    assert foo_bar.__module__ == 'tests.test_decorator'
+    assert foo_bar.__module__ == 'tests.test_deprecated_validate_arguments'
     assert foo_bar.__qualname__ == 'test_wrap.<locals>.foo_bar'
     assert isinstance(foo_bar.vd, ValidatedFunction)
     assert callable(foo_bar.raw_function)
     assert foo_bar.vd.arg_mapping == {0: 'a', 1: 'b'}
     assert foo_bar.vd.positional_only_args == set()
     assert issubclass(foo_bar.model, BaseModel)
     assert foo_bar.model.model_fields.keys() == {'a', 'b', 'args', 'kwargs', 'v__duplicate_kwargs'}
@@ -135,36 +140,27 @@
         """mypy is happy with this"""
         return a + b + sum(args)
 
     assert foo(3) == 102
     assert foo(1, 2, 3) == 6
 
 
-@pytest.mark.xfail(reason='Using Annotated to get a field default is not working properly yet')
-def test_annotated_field_can_provide_factory() -> None:
-    @validate_arguments
-    def foo2(a: int, b: Annotated[int, Field(default_factory=lambda: 99)], *args: int) -> int:
-        """mypy reports Incompatible default for argument "b" if we don't supply ANY as default"""
-        return a + b + sum(args)
-
-    assert foo2(1) == 100
-
-
 @skip_pre_38
 def test_positional_only(create_module):
-    module = create_module(
-        # language=Python
-        """
-from pydantic import validate_arguments
+    with pytest.warns(DeprecationWarning):
+        module = create_module(
+            # language=Python
+            """
+from pydantic.deprecated.decorator import validate_arguments
 
 @validate_arguments
 def foo(a, b, /, c=None):
     return f'{a}, {b}, {c}'
 """
-    )
+        )
     assert module.foo(1, 2) == '1, 2, None'
     assert module.foo(1, 2, 44) == '1, 2, 44'
     assert module.foo(1, 2, c=44) == '1, 2, 44'
     with pytest.raises(TypeError, match="positional-only argument passed as keyword argument: 'b'"):
         module.foo(1, b=2)
     with pytest.raises(TypeError, match="positional-only arguments passed as keyword arguments: 'a', 'b'"):
         module.foo(a=1, b=2)
@@ -370,33 +366,14 @@
     func.validate('qwe', 2)
     with pytest.raises(ValidationError):
         func.validate(['qwe'], 2)
 
     stub.assert_not_called()
 
 
-@pytest.mark.xfail(reason='Annotated does not seem to be respected')
-def test_annotated_use_of_alias():
-    @validate_arguments
-    def foo(a: Annotated[int, Field(alias='b')], c: Annotated[int, Field()], d: Annotated[int, Field(alias='')]):
-        return a + c + d
-
-    assert foo(**{'b': 10, 'c': 12, '': 1}) == 23
-
-    with pytest.raises(ValidationError) as exc_info:
-        assert foo(a=10, c=12, d=1) == 10
-
-    assert exc_info.value.errors() == [
-        {'loc': ('b',), 'msg': 'field required', 'type': 'value_error.missing'},
-        {'loc': ('',), 'msg': 'field required', 'type': 'value_error.missing'},
-        {'loc': ('a',), 'msg': 'extra fields not permitted', 'type': 'value_error.extra'},
-        {'loc': ('d',), 'msg': 'extra fields not permitted', 'type': 'value_error.extra'},
-    ]
-
-
 def test_use_of_alias():
     @validate_arguments
     def foo(c: int = Field(default_factory=lambda: 20), a: int = Field(default_factory=lambda: 10, alias='b')):
         return a + c
 
     assert foo(b=10) == 30
 
@@ -405,56 +382,7 @@
     @validate_arguments(config=dict(populate_by_name=True))
     def foo(a: Annotated[int, Field(alias='b')], c: Annotated[int, Field(alias='d')]):
         return a + c
 
     assert foo(a=10, d=1) == 11
     assert foo(b=10, c=1) == 11
     assert foo(a=10, c=1) == 11
-
-
-@pytest.mark.xfail(reason='validate_all')
-def test_validate_all():
-    # TODO remove or rename, validate_all doesn't exist anymore
-    @validate_arguments(config=dict(validate_all=True))
-    def foo(dt: datetime = Field(default_factory=lambda: 946684800)):
-        return dt
-
-    assert foo() == datetime(2000, 1, 1, tzinfo=timezone.utc)
-    assert foo(0) == datetime(1970, 1, 1, tzinfo=timezone.utc)
-
-
-@pytest.mark.xfail(reason='validate_all')
-@skip_pre_38
-def test_validate_all_positional(create_module):
-    # TODO remove or rename, validate_all doesn't exist anymore
-    module = create_module(
-        # language=Python
-        """
-from datetime import datetime
-
-from pydantic import Field, validate_arguments
-
-@validate_arguments(config=dict(validate_all=True))
-def foo(dt: datetime = Field(default_factory=lambda: 946684800), /):
-    return dt
-"""
-    )
-    assert module.foo() == datetime(2000, 1, 1, tzinfo=timezone.utc)
-    assert module.foo(0) == datetime(1970, 1, 1, tzinfo=timezone.utc)
-
-
-@pytest.mark.xfail(reason='config["extra"] does not seem to be respected')
-def test_validate_extra():
-    class TypedTest(TypedDict):
-        y: str
-
-    @validate_arguments(config={'extra': 'allow'})
-    def test(other: TypedTest):
-        return other
-
-    assert test(other={'y': 'b', 'z': 'a'}) == {'y': 'b', 'z': 'a'}
-
-    @validate_arguments(config={'extra': 'ignore'})
-    def test(other: TypedTest):
-        return other
-
-    assert test(other={'y': 'b', 'z': 'a'}) == {'y': 'b'}
```

### Comparing `pydantic-2.0a2/tests/test_deprecated.py` & `pydantic-2.0a3/tests/test_deprecated.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 import platform
 import re
+import sys
+from datetime import timedelta
+from pathlib import Path
 from types import SimpleNamespace
 from typing import Any, Dict, List, Type
 
 import pytest
 from typing_extensions import Literal
 
 from pydantic import BaseModel, ConfigDict, Field, PydanticUserError, ValidationError, model_serializer, root_validator
 from pydantic.config import Extra
+from pydantic.deprecated.decorator import validate_arguments
+from pydantic.deprecated.json import custom_pydantic_encoder, pydantic_encoder, timedelta_isoformat
+from pydantic.deprecated.parse import load_file, load_str_bytes
+from pydantic.deprecated.tools import parse_obj_as, schema_json_of, schema_of
+
+if sys.version_info < (3, 11):
+    from typing_extensions import get_overloads
+else:
+    from typing import get_overloads
 
 
 def deprecated_from_orm(model_type: Type[BaseModel], obj: Any) -> Any:
     with pytest.warns(
         DeprecationWarning,
         match=re.escape(
             'The `from_orm` method is deprecated; set `model_config["from_attributes"]=True` '
@@ -516,7 +528,156 @@
 
         class Model(BaseModel):
             x: str = Field('test', test='test')
 
     assert Model.model_json_schema(by_alias=True)['properties'] == {
         'x': {'default': 'test', 'test': 'test', 'title': 'X', 'type': 'string'}
     }
+
+
+class SimpleModel(BaseModel):
+    x: int
+
+
+def test_dict():
+    m = SimpleModel(x=1)
+    with pytest.warns(DeprecationWarning, match=r'^The `dict` method is deprecated; use `model_dump` instead\.$'):
+        assert m.dict() == {'x': 1}
+
+
+def test_json():
+    m = SimpleModel(x=1)
+    with pytest.warns(DeprecationWarning, match=r'^The `json` method is deprecated; use `model_dump_json` instead\.$'):
+        assert m.json() == '{"x":1}'
+
+    with pytest.warns(DeprecationWarning):
+        with pytest.raises(TypeError, match='The `encoder` argument is no longer supported'):
+            m.json(encoder=1)
+        with pytest.raises(TypeError, match='The `models_as_dict` argument is no longer supported'):
+            m.json(models_as_dict=True)
+        with pytest.raises(TypeError, match='`dumps_kwargs` keyword arguments are no longer supported.'):
+            m.json(foo=4)
+
+
+def test_parse_obj():
+    with pytest.warns(DeprecationWarning, match='^The `parse_obj` method is deprecated; use `model_validate` instead.'):
+        m = SimpleModel.parse_obj({'x': 1})
+
+    assert m.model_dump() == {'x': 1}
+
+
+def test_parse_file(tmp_path):
+    path = tmp_path / 'test.json'
+    path.write_text('{"x": 12}')
+    with pytest.warns(DeprecationWarning, match='^The `parse_file` method is deprecated; load the data from file,'):
+        assert SimpleModel.parse_file(str(path)).model_dump() == {'x': 12}
+
+
+def test_construct():
+    with pytest.warns(DeprecationWarning, match='The `construct` method is deprecated; use `model_construct` instead.'):
+        m = SimpleModel.construct(x='not an int')
+
+    assert m.x == 'not an int'
+
+
+def test_json_schema():
+    m = SimpleModel(x=1)
+    with pytest.warns(DeprecationWarning, match='^The `schema` method is deprecated; use `model_json_schema` instead.'):
+        assert m.schema() == {
+            'title': 'SimpleModel',
+            'type': 'object',
+            'properties': {'x': {'title': 'X', 'type': 'integer'}},
+            'required': ['x'],
+        }
+
+
+def test_validate():
+    with pytest.warns(DeprecationWarning, match='^The `validate` method is deprecated; use `model_validate` instead.'):
+        m = SimpleModel.validate({'x': 1})
+
+    assert m.model_dump() == {'x': 1}
+
+
+def test_update_forward_refs():
+    with pytest.warns(DeprecationWarning, match='^The `update_forward_refs` method is deprecated;'):
+        SimpleModel.update_forward_refs()
+
+
+def test_copy_and_set_values():
+    m = SimpleModel(x=1)
+    with pytest.warns(DeprecationWarning, match='^The private method  `_copy_and_set_values` will be removed and '):
+        m2 = m._copy_and_set_values(values={'x': 2}, fields_set={'x'}, deep=False)
+
+    assert m2.x == 2
+
+
+def test_get_value():
+    m = SimpleModel(x=1)
+    with pytest.warns(DeprecationWarning, match='^The private method  `_get_value` will be removed and '):
+        v = m._get_value(
+            [1, 2, 3],
+            to_dict=False,
+            by_alias=False,
+            include=None,
+            exclude=None,
+            exclude_unset=False,
+            exclude_defaults=False,
+            exclude_none=False,
+        )
+    assert v == [1, 2, 3]
+
+
+def test_deprecated_module(tmp_path: Path) -> None:
+    class Model(BaseModel):
+        x: int
+
+    assert hasattr(parse_obj_as, '__deprecated__')
+    with pytest.warns(
+        DeprecationWarning, match='parse_obj_as is deprecated. Use pydantic.AnalyzedType.validate_python instead.'
+    ):
+        parse_obj_as(Model, {'x': 1})
+
+    assert hasattr(schema_json_of, '__deprecated__')
+    with pytest.warns(
+        DeprecationWarning, match='schema_json_of is deprecated. Use pydantic.AnalyzedType.json_schema instead.'
+    ):
+        schema_json_of(Model)
+
+    assert hasattr(schema_of, '__deprecated__')
+    with pytest.warns(
+        DeprecationWarning, match='schema_of is deprecated. Use pydantic.AnalyzedType.json_schema instead.'
+    ):
+        schema_of(Model)
+
+    assert hasattr(load_str_bytes, '__deprecated__')
+    with pytest.warns(DeprecationWarning, match='load_str_bytes is deprecated.'):
+        load_str_bytes('{"x": 1}')
+
+    assert hasattr(load_file, '__deprecated__')
+    file = tmp_path / 'main.py'
+    file.write_text('{"x": 1}')
+    with pytest.warns(DeprecationWarning, match='load_file is deprecated.'):
+        load_file(file)
+
+    assert hasattr(pydantic_encoder, '__deprecated__')
+    with pytest.warns(DeprecationWarning, match='pydantic_encoder is deprecated, use BaseModel.model_dump instead.'):
+        pydantic_encoder(Model(x=1))
+
+    assert hasattr(custom_pydantic_encoder, '__deprecated__')
+    with pytest.warns(
+        DeprecationWarning, match='custom_pydantic_encoder is deprecated, use BaseModel.model_dump instead.'
+    ):
+        custom_pydantic_encoder({int: lambda x: str(x)}, Model(x=1))
+
+    assert hasattr(timedelta_isoformat, '__deprecated__')
+    with pytest.warns(DeprecationWarning, match='timedelta_isoformat is deprecated.'):
+        timedelta_isoformat(timedelta(seconds=1))
+
+    assert all(hasattr(func, '__deprecated__') for func in get_overloads(validate_arguments))
+    with pytest.warns(
+        DeprecationWarning, match='The `validate_arguments` method is deprecated; use `validate_call` instead.'
+    ):
+
+        def test(a: int, b: int):
+            pass
+
+        validate_arguments()(test)
```

### Comparing `pydantic-2.0a2/tests/test_discriminated_union.py` & `pydantic-2.0a3/tests/test_discriminated_union.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,26 +346,31 @@
 
 
 class FooStrEnum(str, Enum):
     pass
 
 
 ENUM_TEST_CASES = [
-    pytest.param(Enum, {'a': 1, 'b': 2}, marks=pytest.mark.xfail(reason='Plain Enum not yet supported')),
-    pytest.param(Enum, {'a': 'v_a', 'b': 'v_b'}, marks=pytest.mark.xfail(reason='Plain Enum not yet supported')),
+    pytest.param(Enum, {'a': 1, 'b': 2}, marks=pytest.mark.xfail(reason='Plain Enum discriminator not yet supported')),
+    pytest.param(
+        Enum, {'a': 'v_a', 'b': 'v_b'}, marks=pytest.mark.xfail(reason='Plain Enum discriminator not yet supported')
+    ),
     (FooIntEnum, {'a': 1, 'b': 2}),
     (IntEnum, {'a': 1, 'b': 2}),
     (FooStrEnum, {'a': 'v_a', 'b': 'v_b'}),
 ]
 if sys.version_info >= (3, 11):
     from enum import StrEnum
 
     ENUM_TEST_CASES.append((StrEnum, {'a': 'v_a', 'b': 'v_b'}))
 
 
+@pytest.mark.xfail(
+    sys.version_info[:2] == (3, 8), reason='https://github.com/python/cpython/issues/103592', strict=False
+)
 @pytest.mark.parametrize('base_class,choices', ENUM_TEST_CASES)
 def test_discriminated_union_enum(base_class, choices):
     EnumValue = base_class('EnumValue', choices)
 
     class A(BaseModel):
         m: Literal[EnumValue.a]
```

### Comparing `pydantic-2.0a2/tests/test_docs.py` & `pydantic-2.0a3/tests/test_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     def now(cls, *args, **kwargs):
         return datetime(2032, 1, 2, 3, 4, 5, 6)
 
 
 skip_reason = skip_docs_tests()
 
 
+@pytest.mark.filterwarnings('ignore:(parse_obj_as|schema_json_of|schema_of) is deprecated.*:DeprecationWarning')
 @pytest.mark.skipif(bool(skip_reason), reason=skip_reason or 'not skipping')
 @pytest.mark.parametrize('example', find_examples(str(DOCS_ROOT), skip=sys.platform == 'win32'), ids=str)
 def test_docs_examples(example: CodeExample, eval_example: EvalExample, tmp_path: Path, mocker):  # noqa: C901
     global INDEX_MAIN
     if example.path.name == 'index.md':
         if INDEX_MAIN is None:
             INDEX_MAIN = example.source
```

### Comparing `pydantic-2.0a2/tests/test_edge_cases.py` & `pydantic-2.0a3/tests/test_edge_cases.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import importlib.util
 import re
 import sys
+from abc import ABC, abstractmethod
 from collections.abc import Hashable
 from decimal import Decimal
 from enum import Enum
-from typing import Any, Dict, FrozenSet, Generic, List, Optional, Sequence, Set, Tuple, Type, TypeVar, Union
+from typing import Any, Callable, Dict, FrozenSet, Generic, List, Optional, Sequence, Set, Tuple, Type, TypeVar, Union
 
 import pytest
 from dirty_equals import HasRepr, IsStr
-from pydantic_core import core_schema
+from pydantic_core import PydanticSerializationError, core_schema
 from typing_extensions import Annotated, get_args
 
 from pydantic import (
     AnalyzedType,
     BaseModel,
     ConfigDict,
+    PydanticInvalidForJsonSchema,
     PydanticSchemaGenerationError,
     ValidationError,
     constr,
     errors,
 )
-from pydantic.decorators import field_validator
-from pydantic.fields import Field
+from pydantic.decorators import (
+    field_serializer,
+    field_validator,
+    model_serializer,
+    model_validator,
+    root_validator,
+    validator,
+)
+from pydantic.fields import Field, computed_field
 
 
 def test_str_bytes():
     class Model(BaseModel):
         v: Union[str, bytes] = ...
 
     m = Model(v='s')
@@ -1857,15 +1866,15 @@
 
     class MyGen(Generic[T1, T2]):
         def __init__(self, t1: T1, t2: T2):
             self.t1 = t1
             self.t2 = t2
 
         @classmethod
-        def __get_pydantic_core_schema__(cls, source, **kwargs):
+        def __get_pydantic_core_schema__(cls, source: Any, handler: Callable[[Any], core_schema.CoreSchema]):
             schema = core_schema.is_instance_schema(cls)
 
             args = get_args(source)
             if not args:
                 return schema
 
             t1_f = AnalyzedType(args[0]).validate_python
@@ -1985,47 +1994,63 @@
             gen: MyGen[str, bool]
 
 
 def test_hashable_required():
     class Model(BaseModel):
         v: Hashable
 
-        # TODO: Should arbitrary_types_allowed be necessary for Hashable?
-        #   "ideally I guess we should have a validator for this."
-        #   https://github.com/pydantic/pydantic/pull/5151#discussion_r1130684977
-        model_config = dict(arbitrary_types_allowed=True)
-
     Model(v=None)
     with pytest.raises(ValidationError) as exc_info:
         Model(v=[])
     assert exc_info.value.errors() == [
-        {
-            'ctx': {'class': 'Hashable'},
-            'input': [],
-            'loc': ('v',),
-            'msg': 'Input should be an instance of Hashable',
-            'type': 'is_instance_of',
-        }
+        {'input': [], 'loc': ('v',), 'msg': 'Input should be hashable', 'type': 'is_hashable'}
     ]
     with pytest.raises(ValidationError) as exc_info:
         Model()
     assert exc_info.value.errors() == [{'input': {}, 'loc': ('v',), 'msg': 'Field required', 'type': 'missing'}]
 
 
 @pytest.mark.parametrize('default', [1, None])
 def test_hashable_optional(default):
     class Model(BaseModel):
         v: Hashable = default
 
-        model_config = dict(arbitrary_types_allowed=True)
-
     Model(v=None)
     Model()
 
 
+def test_hashable_serialization():
+    class Model(BaseModel):
+        v: Hashable
+
+    class HashableButNotSerializable:
+        def __hash__(self):
+            return 0
+
+    assert Model(v=(1,)).model_dump_json() == '{"v":[1]}'
+    m = Model(v=HashableButNotSerializable())
+    with pytest.raises(
+        PydanticSerializationError, match='Unable to serialize unknown type:.*HashableButNotSerializable'
+    ):
+        m.model_dump_json()
+
+
+def test_hashable_json_schema():
+    class Model(BaseModel):
+        v: Hashable
+
+    with pytest.raises(
+        PydanticInvalidForJsonSchema,
+        match=re.escape(
+            "Cannot generate a JsonSchema for core_schema.IsInstanceSchema (<class 'collections.abc.Hashable'>)"
+        ),
+    ):
+        Model.model_json_schema()
+
+
 def test_default_factory_called_once():
     """It should never call `default_factory` more than once even when `validate_all` is set"""
 
     v = 0
 
     def factory() -> int:
         nonlocal v
@@ -2244,7 +2269,80 @@
     class Child(Parent):
         c: int = 3
 
     c = Child()
     assert c.a == 1
     assert c.b == 2
     assert c.c == 3
+
+
+@pytest.mark.parametrize(
+    'bases',
+    [
+        (BaseModel, ABC),
+        (ABC, BaseModel),
+        (BaseModel,),
+    ],
+)
+def test_abstractmethod_missing_for_all_decorators(bases):
+    class AbstractSquare(*bases):
+        side: float
+
+        @field_validator('side')
+        @classmethod
+        @abstractmethod
+        def my_field_validator(cls, v):
+            raise NotImplementedError
+
+        @model_validator(mode='wrap')
+        @classmethod
+        @abstractmethod
+        def my_model_validator(cls, values, handler, info):
+            raise NotImplementedError
+
+        @root_validator(skip_on_failure=True)
+        @classmethod
+        @abstractmethod
+        def my_root_validator(cls, values):
+            raise NotImplementedError
+
+        with pytest.warns(DeprecationWarning):
+
+            @validator('side')
+            @classmethod
+            @abstractmethod
+            def my_validator(cls, value, **kwargs):
+                raise NotImplementedError
+
+        @model_serializer(mode='wrap')
+        @abstractmethod
+        def my_model_serializer(self, handler, info):
+            raise NotImplementedError
+
+        @field_serializer('side')
+        @abstractmethod
+        def my_serializer(self, v, _info):
+            raise NotImplementedError
+
+        @computed_field
+        @property
+        @abstractmethod
+        def my_computed_field(self):
+            raise NotImplementedError
+
+    class Square(AbstractSquare):
+        pass
+
+    with pytest.raises(
+        TypeError,
+        match=(
+            "Can't instantiate abstract class Square with abstract methods"
+            " my_computed_field,"
+            " my_field_validator,"
+            " my_model_serializer,"
+            " my_model_validator,"
+            " my_root_validator,"
+            " my_serializer,"
+            " my_validator"
+        ),
+    ):
+        Square(side=1.0)
```

### Comparing `pydantic-2.0a2/tests/test_fastapi_json_schema.py` & `pydantic-2.0a3/tests/test_fastapi_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_forward_ref.py` & `pydantic-2.0a3/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_generics.py` & `pydantic-2.0a3/tests/test_generics.py`

 * *Files 1% similar despite different names*

```diff
@@ -2193,7 +2193,103 @@
             'ctx': {'ge': 42},
             'input': 41,
             'loc': ('page',),
             'msg': 'Input should be greater than or equal to 42',
             'type': 'greater_than_equal',
         }
     ]
+
+
+def test_generic_enum_bound():
+    T = TypeVar('T', bound=Enum)
+
+    class MyEnum(Enum):
+        a = 1
+
+    class OtherEnum(Enum):
+        b = 2
+
+    class Model(BaseModel, Generic[T]):
+        x: T
+
+    m = Model(x=MyEnum.a)
+    assert m.x == MyEnum.a
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(x=1)
+    assert exc_info.value.errors() == [
+        {
+            'ctx': {'class': 'Enum'},
+            'input': 1,
+            'loc': ('x',),
+            'msg': 'Input should be an instance of Enum',
+            'type': 'is_instance_of',
+        }
+    ]
+
+    m2 = Model[MyEnum](x=MyEnum.a)
+    assert m2.x == MyEnum.a
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model[MyEnum](x=OtherEnum.b)
+    assert exc_info.value.errors() == [
+        {
+            'ctx': {'expected': '1'},
+            'input': OtherEnum.b,
+            'loc': ('x',),
+            'msg': 'Input should be 1',
+            'type': 'enum',
+        }
+    ]
+
+    assert Model[MyEnum].model_json_schema() == {
+        '$defs': {'MyEnum': {'const': 1, 'title': 'MyEnum'}},
+        'properties': {'x': {'$ref': '#/$defs/MyEnum'}},
+        'required': ['x'],
+        'title': 'Model[test_generic_enum_bound.<locals>.MyEnum]',
+        'type': 'object',
+    }
+
+
+def test_generic_intenum_bound():
+    T = TypeVar('T', bound=IntEnum)
+
+    class MyEnum(IntEnum):
+        a = 1
+
+    class OtherEnum(IntEnum):
+        b = 2
+
+    class Model(BaseModel, Generic[T]):
+        x: T
+
+    m = Model(x=MyEnum.a)
+    assert m.x == MyEnum.a
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(x=1)
+    assert exc_info.value.errors() == [
+        {
+            'ctx': {'class': 'IntEnum'},
+            'input': 1,
+            'loc': ('x',),
+            'msg': 'Input should be an instance of IntEnum',
+            'type': 'is_instance_of',
+        }
+    ]
+
+    m2 = Model[MyEnum](x=MyEnum.a)
+    assert m2.x == MyEnum.a
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model[MyEnum](x=OtherEnum.b)
+    assert exc_info.value.errors() == [
+        {'ctx': {'expected': '1'}, 'input': 2, 'loc': ('x',), 'msg': 'Input should be 1', 'type': 'enum'}
+    ]
+
+    assert Model[MyEnum].model_json_schema() == {
+        '$defs': {'MyEnum': {'const': 1, 'title': 'MyEnum', 'type': 'integer'}},
+        'properties': {'x': {'$ref': '#/$defs/MyEnum'}},
+        'required': ['x'],
+        'title': 'Model[test_generic_intenum_bound.<locals>.MyEnum]',
+        'type': 'object',
+    }
```

### Comparing `pydantic-2.0a2/tests/test_hypothesis_plugin.py` & `pydantic-2.0a3/tests/test_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_json.py` & `pydantic-2.0a3/tests/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 try:
     import email_validator
 except ImportError:
     email_validator = None
 
 
+pytestmark = pytest.mark.filterwarnings('ignore::DeprecationWarning')
+
+
 class MyEnum(Enum):
     foo = 'bar'
     snap = 'crackle'
 
 
 class MyModel(BaseModel):
     a: str = 'b'
```

### Comparing `pydantic-2.0a2/tests/test_json_schema.py` & `pydantic-2.0a3/tests/test_json_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,18 @@
     BaseModel,
     Field,
     ImportString,
     ValidationError,
     field_validator,
 )
 from pydantic._internal._core_metadata import build_metadata_dict
-from pydantic._internal._generate_schema import GenerateSchema
 from pydantic.color import Color
 from pydantic.config import ConfigDict
 from pydantic.dataclasses import dataclass
 from pydantic.errors import PydanticInvalidForJsonSchema
-from pydantic.fields import FieldInfo
 from pydantic.json_schema import (
     DEFAULT_REF_TEMPLATE,
     GenerateJsonSchema,
     PydanticJsonSchemaWarning,
     model_json_schema,
     models_json_schema,
 )
@@ -2274,19 +2272,21 @@
 
         @classmethod
         def validate(cls, v: Any):
             return v
 
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, source: Any, gen_schema: GenerateSchema, **_kwargs: Any
+            cls,
+            source: Any,
+            handler: Callable[[Any], core_schema.CoreSchema],
         ) -> core_schema.PlainValidatorFunctionSchema:
             source_args = getattr(source, '__args__', [Any])
             param = source_args[0]
-            metadata = build_metadata_dict(js_cs_override=gen_schema.generate_schema(param))
+            metadata = build_metadata_dict(js_cs_override=handler(param))
             return core_schema.general_plain_validator_function(
                 GenModel,
                 metadata=metadata,
             )
 
     class Model(BaseModel):
         data: GenModel[str]
@@ -2371,26 +2371,26 @@
 
         @classmethod
         def validate(cls, v: Any):
             return v
 
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, source: Any, gen_schema: GenerateSchema, **_kwargs: Any
-        ) -> core_schema.PlainValidatorFunctionSchema:
+            cls, source: Any, handler: Callable[[Any], core_schema.CoreSchema]
+        ) -> core_schema.CoreSchema:
             if hasattr(source, '__args__'):
                 param = source.__args__[0]
-                metadata = build_metadata_dict(js_cs_override=gen_schema.generate_schema(Optional[param]))
+                metadata = build_metadata_dict(js_cs_override=handler(Optional[param]))
                 return core_schema.general_plain_validator_function(
                     Gen,
                     metadata=metadata,
                 )
 
         @classmethod
-        def __pydantic_modify_json_schema__(cls, field_schema):
+        def __pydantic_modify_json_schema__(cls, field_schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
             the_type = field_schema.pop('anyOf', [{'type': 'string'}])[0]
             field_schema.update(title='Gen title', anyOf=[the_type, {'type': 'array', 'items': the_type}])
             return field_schema
 
     class GenTwoParams(Generic[T, K]):
         def __init__(self, x: str, y: Any):
             self.x = x
@@ -2402,36 +2402,37 @@
 
         @classmethod
         def validate(cls, v: Any):
             return cls(*v)
 
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, source: Any, gen_schema: GenerateSchema, **_kwargs: Any
-        ) -> core_schema.PlainValidatorFunctionSchema:
+            cls, source: Any, handler: Callable[[Any], core_schema.CoreSchema], **_kwargs: Any
+        ) -> core_schema.CoreSchema:
             if hasattr(source, '__args__'):
-                metadata = build_metadata_dict(js_cs_override=gen_schema.generate_schema(Tuple[source.__args__]))
+                metadata = build_metadata_dict(js_cs_override=handler(Tuple[source.__args__]))
                 return core_schema.general_plain_validator_function(
                     GenTwoParams,
                     metadata=metadata,
                 )
+            return handler(source)
 
         @classmethod
-        def __pydantic_modify_json_schema__(cls, field_schema):
+        def __pydantic_modify_json_schema__(cls, field_schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
             field_schema.pop('minItems')
             field_schema.pop('maxItems')
             field_schema.update(examples='examples')
             return field_schema
 
     class CustomType(Enum):
         A = 'a'
         B = 'b'
 
         @classmethod
-        def __pydantic_modify_json_schema__(cls, field_schema):
+        def __pydantic_modify_json_schema__(cls, field_schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
             field_schema.update(title='CustomType title', type='string')
             return field_schema
 
     class Model(BaseModel):
         data0: Gen
         data1: Gen[CustomType] = Field(title='Data1 title', description='Data 1 description')
         data2: GenTwoParams[CustomType, UUID4] = Field(title='Data2 title', description='Data 2')
@@ -2598,41 +2599,14 @@
                 'required': ['uuid'],
             },
         },
         'allOf': [{'$ref': '#/$defs/Model'}],
     }
 
 
-@pytest.mark.xfail(reason='__pydantic_modify_json_schema__ does not receive FieldInfo')
-def test_schema_with_field_parameter():
-    # TODO: Update so that __pydantic_modify_json_schema__ gets called with the FieldInfo when handling fields
-    class RestrictedAlphabetStr(str):
-        @classmethod
-        def __pydantic_modify_json_schema__(cls, field_schema, field: Optional[FieldInfo]):
-            assert isinstance(field, FieldInfo)
-            alphabet = field.json_schema_extra['alphabet']
-            field_schema['examples'] = [c * 3 for c in alphabet]
-            field_schema['title'] = field.title.lower()
-            return field_schema
-
-    class MyModel(BaseModel):
-        value: RestrictedAlphabetStr = Field(title='RESTRICTED_ALPHABET', json_schema_extra={'alphabet': 'ABC'})
-
-        model_config = {'arbitrary_types_allowed': True}
-
-    assert MyModel.model_json_schema() == {
-        'title': 'MyModel',
-        'type': 'object',
-        'properties': {
-            'value': {'title': 'Value', 'alphabet': 'ABC', 'examples': ['AAA', 'BBB', 'CCC'], 'type': 'string'}
-        },
-        'required': ['value'],
-    }
-
-
 def test_modify_schema_dict_keys() -> None:
     class MyType:
         @classmethod
         def __pydantic_modify_json_schema__(cls, schema):
             schema['test'] = 'passed'
             return schema
 
@@ -3454,7 +3428,34 @@
     assert MyModel.model_json_schema() == {
         '$schema': 'https://json-schema.org/draft/2020-12/schema',
         'properties': {'x': {'title': 'X', 'type': 'integer'}},
         'required': ['x'],
         'title': 'MyModel',
         'type': 'object',
     }
+
+
+def test_nested_default_json_schema():
+    class InnerModel(BaseModel):
+        foo: str = 'bar'
+        baz: str = Field(default='foobar', alias='my_alias')
+
+    class OuterModel(BaseModel):
+        nested_field: InnerModel = InnerModel()
+
+    assert OuterModel.model_json_schema() == {
+        '$defs': {
+            'InnerModel': {
+                'properties': {
+                    'foo': {'default': 'bar', 'title': 'Foo', 'type': 'string'},
+                    'my_alias': {'default': 'foobar', 'title': 'My Alias', 'type': 'string'},
+                },
+                'title': 'InnerModel',
+                'type': 'object',
+            }
+        },
+        'properties': {
+            'nested_field': {'allOf': [{'$ref': '#/$defs/InnerModel'}], 'default': {'my_alias': 'foobar', 'foo': 'bar'}}
+        },
+        'title': 'OuterModel',
+        'type': 'object',
+    }
```

### Comparing `pydantic-2.0a2/tests/test_main.py` & `pydantic-2.0a3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_model_signature.py` & `pydantic-2.0a3/tests/test_model_signature.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_model_validator.py` & `pydantic-2.0a3/tests/test_model_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from typing import Any, Dict, cast
 
+import pytest
+
 from pydantic import BaseModel, ValidationInfo
 from pydantic.decorators import ModelWrapValidatorHandler, model_validator
 
 
 def test_model_validator_wrap() -> None:
     class Model(BaseModel):
         x: int
@@ -25,21 +27,22 @@
             self.y += 1
             return self
 
     assert Model(x=1, y=2).model_dump() == {'x': 2, 'y': 3}
     assert Model.model_validate(Model(x=1, y=2)).model_dump() == {'x': 3, 'y': 4}
 
 
-def test_model_validator_before() -> None:
+@pytest.mark.parametrize('classmethod_decorator', [classmethod, lambda x: x])
+def test_model_validator_before(classmethod_decorator: Any) -> None:
     class Model(BaseModel):
         x: int
         y: int
 
         @model_validator(mode='before')
-        @classmethod
+        @classmethod_decorator
         def val_model(cls, values: Any, info: ValidationInfo) -> dict[str, Any] | Model:
             assert not info.context
             if isinstance(values, dict):
                 values = cast(Dict[str, Any], values)
                 values['x'] += 1
                 values['y'] += 1
             else:
@@ -62,7 +65,21 @@
             assert not info.context
             self.x += 1
             self.y += 1
             return self
 
     assert Model(x=1, y=2).model_dump() == {'x': 2, 'y': 3}
     assert Model.model_validate(Model(x=1, y=2)).model_dump() == {'x': 3, 'y': 4}
+
+
+def test_subclass() -> None:
+    class Human(BaseModel):
+        @model_validator(mode='before')
+        @classmethod
+        def run_model_validator(cls, values: dict[str, Any]) -> dict[str, Any]:
+            values['age'] *= 2
+            return values
+
+    class Person(Human):
+        age: int
+
+    assert Person(age=28).age == 56
```

### Comparing `pydantic-2.0a2/tests/test_networks.py` & `pydantic-2.0a3/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_networks_ipaddress.py` & `pydantic-2.0a3/tests/test_networks_ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_parse.py` & `pydantic-2.0a3/tests/test_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,15 @@
         nested: NestedModel
 
     m = MyModel.model_validate({'nested': [{'id': 'foo'}]})
     assert isinstance(m.nested, NestedModel)
     assert isinstance(m.nested.root[0], NestedData)
 
 
+@pytest.mark.filterwarnings('ignore:parse_obj_as is deprecated.*:DeprecationWarning')
 def test_parse_nested_root_tuple():
     class NestedData(BaseModel):
         id: str
 
     class NestedModel(BaseModel):
         root: Tuple[int, NestedData]
```

### Comparing `pydantic-2.0a2/tests/test_private_attributes.py` & `pydantic-2.0a3/tests/test_private_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 import platform
 from typing import ClassVar, Generic, TypeVar
 
 import pytest
 
 from pydantic import BaseModel, ConfigDict, PrivateAttr
 from pydantic.fields import Undefined
@@ -308,7 +309,18 @@
         # The following are included to document existing behavior, and can be updated
         # if the current behavior does not match the desired behavior
         _e: int
         _f: int = 1
         _g = 1  # Note: this is completely ignored, in keeping with v1
 
     assert sorted(MyModel.__private_attributes__.keys()) == ['_e', '_f']
+
+
+@pytest.mark.skipif(not hasattr(functools, 'cached_property'), reason='cached_property is not available')
+def test_ignored_types_are_ignored_cached_property():
+    """Demonstrate the members of functools are ignore here as with fields."""
+
+    class MyModel(BaseModel):
+        _a: functools.cached_property
+        _b: int
+
+    assert set(MyModel.__private_attributes__) == {'_b'}
```

### Comparing `pydantic-2.0a2/tests/test_rich_repr.py` & `pydantic-2.0a3/tests/test_rich_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_serialize.py` & `pydantic-2.0a3/tests/test_serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 
 def test_annotated_customisation():
     def parse_int(s: str, _: Any) -> int:
         return int(s.replace(',', ''))
 
     class CommaFriendlyIntLogic:
         @classmethod
-        def __get_pydantic_core_schema__(cls, _schema):
+        def __get_pydantic_core_schema__(cls, _source, _handler):
             # here we ignore the schema argument (which is just `{'type': 'int'}`) and return our own
             return core_schema.general_before_validator_function(
                 parse_int,
                 core_schema.int_schema(),
                 serialization=core_schema.format_ser_schema(',', when_used='unless-none'),
             )
 
@@ -231,64 +231,64 @@
         'f3': '3,000',
         'f4': '4,000',
     }
     assert m.model_dump_json() == '{"f1":"1,000","f2":"2,000","f3":"3,000","f4":"4,000"}'
 
 
 def test_invalid_signature_no_params() -> None:
-    with pytest.raises(TypeError, match='Unrecognized field_serializer signature'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer function signature'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x')
             def no_args() -> Any:  # pragma: no cover
                 ...
 
 
 def test_invalid_signature_single_params() -> None:
-    with pytest.raises(TypeError, match='Unrecognized field_serializer signature'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer function signature'):
 
         class _(BaseModel):
             x: int
 
             # not caught by type checkers
             @field_serializer('x')
             def no_args(self) -> Any:  # pragma: no cover
                 ...
 
 
 def test_invalid_signature_too_many_params_1() -> None:
-    with pytest.raises(TypeError, match='Unrecognized field_serializer signature'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer function signature'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x')
             def no_args(self, value: Any, nxt: Any, info: Any, extra_param: Any) -> Any:  # pragma: no cover
                 ...
 
 
 def test_invalid_signature_too_many_params_2() -> None:
-    with pytest.raises(TypeError, match='Unrecognized field_serializer signature'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer function signature'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x')
             @staticmethod
             def no_args(not_self: Any, value: Any, nxt: Any, info: Any) -> Any:  # pragma: no cover
                 ...
 
 
 def test_invalid_signature_bad_plain_signature() -> None:
-    with pytest.raises(TypeError, match='Unrecognized field_serializer signature for'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer function signature for'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x', mode='plain')
             def no_args(self, value: Any, nxt: Any, info: Any) -> Any:  # pragma: no cover
@@ -457,15 +457,15 @@
     msg = "^Error serializing to JSON: 'int' object cannot be converted to 'PyString'$"
     with pytest.raises(PydanticSerializationError, match=msg):
         m.model_dump_json()
 
 
 def test_model_serializer_wrong_args():
     m = (
-        r'Unrecognized model_serializer signature for '
+        r'Unrecognized model_serializer function signature for '
         r'<.+MyModel._serialize at 0x\w+> with `mode=plain`:\(self, x, y, z\)'
     )
     with pytest.raises(TypeError, match=m):
 
         class MyModel(BaseModel):
             a: int
 
@@ -621,15 +621,15 @@
 
         @field_serializer('x')
         def ser_x(self, _v: int, _info: SerializationInfo) -> str:
             return 'parent_encoder'
 
     # overriding a serializer with a function / class var
     # of the same name is allowed
-    # to mimick how inheritance works
+    # to mimic how inheritance works
     # the serializer in the child class replaces the parent
     # (without modifying the parent class itself)
     class Child1(Parent):
         @field_serializer('x')
         def ser_x(self, _v: int, _info: SerializationInfo) -> str:
             return 'child1_encoder' + ' ' + super().ser_x(_v, _info)
```

### Comparing `pydantic-2.0a2/tests/test_strict.py` & `pydantic-2.0a3/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_structural_pattern_matching.py` & `pydantic-2.0a3/tests/test_structural_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_tools.py` & `pydantic-2.0a3/tests/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Dict, List, Mapping, Union
 
 import pytest
 
 from pydantic import BaseModel, ValidationError
 from pydantic.dataclasses import dataclass
-from pydantic.tools import parse_obj_as, schema_json_of, schema_of
+from pydantic.deprecated.tools import parse_obj_as, schema_json_of, schema_of
+
+pytestmark = pytest.mark.filterwarnings('ignore::DeprecationWarning')
 
 
 @pytest.mark.parametrize('obj,type_,parsed', [('1', int, 1), (['1'], List[int], [1])])
 def test_parse_obj(obj, type_, parsed):
     assert parse_obj_as(type_, obj) == parsed
```

### Comparing `pydantic-2.0a2/tests/test_types.py` & `pydantic-2.0a3/tests/test_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,24 @@
     TypeVar,
     Union,
 )
 from uuid import UUID
 
 import annotated_types
 import pytest
-from dirty_equals import HasRepr
+from dirty_equals import HasRepr, IsStr
 from pydantic_core._pydantic_core import PydanticCustomError, SchemaError
 from typing_extensions import Annotated, Literal, TypedDict
 
 from pydantic import (
     UUID1,
     UUID3,
     UUID4,
     UUID5,
+    AnalyzedType,
     AwareDatetime,
     BaseModel,
     ByteSize,
     ConfigDict,
     DirectoryPath,
     EmailStr,
     Field,
@@ -59,14 +60,15 @@
     NonNegativeFloat,
     NonNegativeInt,
     NonPositiveFloat,
     NonPositiveInt,
     PastDate,
     PositiveFloat,
     PositiveInt,
+    PydanticInvalidForJsonSchema,
     SecretBytes,
     SecretStr,
     StrictBool,
     StrictBytes,
     StrictFloat,
     StrictInt,
     StrictStr,
@@ -1321,15 +1323,15 @@
 def test_enum_fails(cooking_model):
     FruitEnum, ToolEnum, CookingModel = cooking_model
     with pytest.raises(ValueError) as exc_info:
         CookingModel(tool=3)
     # insert_assert(exc_info.value.errors())
     assert exc_info.value.errors() == [
         {
-            'type': 'literal_error',
+            'type': 'enum',
             'loc': ('tool',),
             'msg': 'Input should be 1 or 2',
             'input': 3,
             'ctx': {'expected': '1 or 2'},
         }
     ]
 
@@ -1337,26 +1339,151 @@
 def test_int_enum_successful_for_str_int(cooking_model):
     FruitEnum, ToolEnum, CookingModel = cooking_model
     m = CookingModel(tool='2')
     assert m.tool == ToolEnum.wrench
     assert repr(m.tool) == '<ToolEnum.wrench: 2>'
 
 
+def test_plain_enum_validate():
+    class MyEnum(Enum):
+        a = 1
+
+    class Model(BaseModel):
+        x: MyEnum
+
+    m = Model(x=MyEnum.a)
+    assert m.x is MyEnum.a
+
+    assert AnalyzedType(MyEnum).validate_python(1) is MyEnum.a
+    with pytest.raises(ValidationError) as exc_info:
+        AnalyzedType(MyEnum).validate_python(1, strict=True)
+    assert exc_info.value.errors() == [
+        {
+            'ctx': {'class': 'test_plain_enum_validate.<locals>.MyEnum'},
+            'input': 1,
+            'loc': (),
+            'msg': IsStr(regex='Input should be an instance of test_plain_enum_validate.<locals>.MyEnum'),
+            'type': 'is_instance_of',
+        }
+    ]
+
+
+def test_plain_enum_validate_json():
+    class MyEnum(Enum):
+        a = 1
+
+    class Model(BaseModel):
+        x: MyEnum
+
+    m = Model.model_validate_json('{"x":1}')
+    assert m.x is MyEnum.a
+
+
 def test_enum_type():
-    with pytest.raises(SchemaError, match='"expected" should have length > 0'):
+    class Model(BaseModel):
+        my_enum: Enum
 
-        class Model(BaseModel):
-            my_int_enum: Enum
+    class MyEnum(Enum):
+        a = 1
+
+    m = Model(my_enum=MyEnum.a)
+    assert m.my_enum == MyEnum.a
+    assert m.model_dump() == {'my_enum': MyEnum.a}
+    assert m.model_dump_json() == '{"my_enum":1}'
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(my_enum=1)
+    assert exc_info.value.errors() == [
+        {
+            'ctx': {'class': 'Enum'},
+            'input': 1,
+            'loc': ('my_enum',),
+            'msg': 'Input should be an instance of Enum',
+            'type': 'is_instance_of',
+        }
+    ]
+
+    with pytest.raises(
+        PydanticInvalidForJsonSchema,
+        match=re.escape("Cannot generate a JsonSchema for core_schema.IsInstanceSchema (<enum 'Enum'>)"),
+    ):
+        Model.model_json_schema()
 
 
 def test_int_enum_type():
-    with pytest.raises(SchemaError, match='"expected" should have length > 0'):
+    class Model(BaseModel):
+        my_enum: IntEnum
 
-        class Model(BaseModel):
-            my_int_enum: IntEnum
+    class MyEnum(Enum):
+        a = 1
+
+    class MyIntEnum(IntEnum):
+        b = 2
+
+    m = Model(my_enum=MyIntEnum.b)
+    assert m.my_enum == MyIntEnum.b
+    assert m.model_dump() == {'my_enum': MyIntEnum.b}
+    assert m.model_dump_json() == '{"my_enum":2}'
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(my_enum=MyEnum.a)
+    assert exc_info.value.errors() == [
+        {
+            'ctx': {'class': 'IntEnum'},
+            'input': MyEnum.a,
+            'loc': ('my_enum',),
+            'msg': 'Input should be an instance of IntEnum',
+            'type': 'is_instance_of',
+        }
+    ]
+
+    with pytest.raises(
+        PydanticInvalidForJsonSchema,
+        match=re.escape("Cannot generate a JsonSchema for core_schema.IsInstanceSchema (<enum 'IntEnum'>)"),
+    ):
+        Model.model_json_schema()
+
+
+@pytest.mark.parametrize('enum_base', [Enum, IntEnum])
+@pytest.mark.parametrize('strict', [True, False])
+def test_enum_from_json(enum_base, strict):
+    class MyEnum(enum_base):
+        a = 1
+
+    class Model(BaseModel):
+        my_enum: MyEnum
+
+    m = Model.model_validate_json('{"my_enum":1}', strict=strict)
+    assert m.my_enum is MyEnum.a
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model.model_validate_json('{"my_enum":2}', strict=strict)
+
+    my_enum_label = MyEnum.__name__ if sys.version_info[:2] <= (3, 8) else MyEnum.__qualname__
+
+    if strict:
+        assert exc_info.value.errors() == [
+            {
+                'ctx': {'error': f'2 is not a valid {my_enum_label}'},
+                'input': 2,
+                'loc': ('my_enum',),
+                'msg': f'Value error, 2 is not a valid {my_enum_label}',
+                'type': 'value_error',
+            }
+        ]
+    else:
+        assert exc_info.value.errors() == [
+            {
+                'ctx': {'expected': '1'},
+                'input': 2,
+                'loc': ('my_enum',),
+                'msg': 'Input should be 1',
+                'type': 'enum',
+            }
+        ]
 
 
 @pytest.mark.parametrize(
     'kwargs,type_',
     [
         ({'max_length': 5}, int),
         ({'min_length': 2}, float),
@@ -3850,48 +3977,84 @@
 def test_deque_json():
     class Model(BaseModel):
         v: Deque[int]
 
     assert Model(v=deque((1, 2, 3))).model_dump_json() == '{"v":[1,2,3]}'
 
 
-@pytest.mark.parametrize('value_type', (None, type(None), None.__class__, Literal[None]))
+def test_deque_any_maxlen():
+    class DequeModel1(BaseModel):
+        field: deque
+
+    assert DequeModel1(field=deque()).field.maxlen is None
+    assert DequeModel1(field=deque(maxlen=8)).field.maxlen == 8
+
+    class DequeModel2(BaseModel):
+        field: deque = deque()
+
+    assert DequeModel2().field.maxlen is None
+    assert DequeModel2(field=deque()).field.maxlen is None
+    assert DequeModel2(field=deque(maxlen=8)).field.maxlen == 8
+
+    class DequeModel3(BaseModel):
+        field: deque = deque(maxlen=5)
+
+    assert DequeModel3().field.maxlen == 5
+    assert DequeModel3(field=deque()).field.maxlen is None
+    assert DequeModel3(field=deque(maxlen=8)).field.maxlen == 8
+
+
+def test_deque_typed_maxlen():
+    class DequeModel1(BaseModel):
+        field: Deque[int]
+
+    assert DequeModel1(field=deque()).field.maxlen is None
+    assert DequeModel1(field=deque(maxlen=8)).field.maxlen == 8
+
+    class DequeModel2(BaseModel):
+        field: Deque[int] = deque()
+
+    assert DequeModel2().field.maxlen is None
+    assert DequeModel2(field=deque()).field.maxlen is None
+    assert DequeModel2(field=deque(maxlen=8)).field.maxlen == 8
+
+    class DequeModel3(BaseModel):
+        field: Deque[int] = deque(maxlen=5)
+
+    assert DequeModel3().field.maxlen == 5
+    assert DequeModel3(field=deque()).field.maxlen is None
+    assert DequeModel3(field=deque(maxlen=8)).field.maxlen == 8
+
+
+@pytest.mark.parametrize('value_type', (None, type(None), None.__class__))
 def test_none(value_type):
     class Model(BaseModel):
         my_none: value_type
         my_none_list: List[value_type]
         my_none_dict: Dict[str, value_type]
         my_json_none: Json[value_type]
 
     Model(
         my_none=None,
         my_none_list=[None] * 3,
         my_none_dict={'a': None, 'b': None},
         my_json_none='null',
     )
 
-    # assert Model.model_json_schema() == {
-    #     'title': 'Model',
-    #     'type': 'object',
-    #     'properties': {
-    #         'my_none': {'title': 'My None', 'type': 'null'},
-    #         'my_none_list': {
-    #             'title': 'My None List',
-    #             'type': 'array',
-    #             'items': {'type': 'null'},
-    #         },
-    #         'my_none_dict': {
-    #             'title': 'My None Dict',
-    #             'type': 'object',
-    #             'additionalProperties': {'type': 'null'},
-    #         },
-    #         'my_json_none': {'title': 'My Json None', 'type': 'null'},
-    #     },
-    #     'required': ['my_none', 'my_none_list', 'my_none_dict', 'my_json_none'],
-    # }
+    assert Model.model_json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {
+            'my_none': {'type': 'null', 'title': 'My None'},
+            'my_none_list': {'type': 'array', 'items': {'type': 'null'}, 'title': 'My None List'},
+            'my_none_dict': {'type': 'object', 'additionalProperties': {'type': 'null'}, 'title': 'My None Dict'},
+            'my_json_none': {'type': 'string', 'format': 'json-string', 'title': 'My Json None'},
+        },
+        'required': ['my_none', 'my_none_list', 'my_none_dict', 'my_json_none'],
+    }
 
     with pytest.raises(ValidationError) as exc_info:
         Model(
             my_none='qwe',
             my_none_list=[1, None, 'qwe'],
             my_none_dict={'a': 1, 'b': None},
             my_json_none='"a"',
@@ -3912,14 +4075,87 @@
             'msg': 'Input should be None',
             'input': 1,
         },
         {'type': 'none_required', 'loc': ('my_json_none',), 'msg': 'Input should be None', 'input': 'a'},
     ]
 
 
+def test_none_literal():
+    class Model(BaseModel):
+        my_none: Literal[None]
+        my_none_list: List[Literal[None]]
+        my_none_dict: Dict[str, Literal[None]]
+        my_json_none: Json[Literal[None]]
+
+    Model(
+        my_none=None,
+        my_none_list=[None] * 3,
+        my_none_dict={'a': None, 'b': None},
+        my_json_none='null',
+    )
+
+    assert Model.model_json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {
+            'my_none': {'const': None, 'title': 'My None'},
+            'my_none_list': {'type': 'array', 'items': {'const': None}, 'title': 'My None List'},
+            'my_none_dict': {'type': 'object', 'additionalProperties': {'const': None}, 'title': 'My None Dict'},
+            'my_json_none': {'type': 'string', 'format': 'json-string', 'title': 'My Json None'},
+        },
+        'required': ['my_none', 'my_none_list', 'my_none_dict', 'my_json_none'],
+    }
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(
+            my_none='qwe',
+            my_none_list=[1, None, 'qwe'],
+            my_none_dict={'a': 1, 'b': None},
+            my_json_none='"a"',
+        )
+    # insert_assert(exc_info.value.errors())
+    assert exc_info.value.errors() == [
+        {
+            'type': 'literal_error',
+            'loc': ('my_none',),
+            'msg': 'Input should be None',
+            'input': 'qwe',
+            'ctx': {'expected': 'None'},
+        },
+        {
+            'type': 'literal_error',
+            'loc': ('my_none_list', 0),
+            'msg': 'Input should be None',
+            'input': 1,
+            'ctx': {'expected': 'None'},
+        },
+        {
+            'type': 'literal_error',
+            'loc': ('my_none_list', 2),
+            'msg': 'Input should be None',
+            'input': 'qwe',
+            'ctx': {'expected': 'None'},
+        },
+        {
+            'type': 'literal_error',
+            'loc': ('my_none_dict', 'a'),
+            'msg': 'Input should be None',
+            'input': 1,
+            'ctx': {'expected': 'None'},
+        },
+        {
+            'type': 'literal_error',
+            'loc': ('my_json_none',),
+            'msg': 'Input should be None',
+            'input': 'a',
+            'ctx': {'expected': 'None'},
+        },
+    ]
+
+
 def test_default_union_types():
     class DefaultModel(BaseModel):
         v: Union[int, bool, str]
 
     # do it this way since `1 == True`
     assert repr(DefaultModel(v=True).v) == 'True'
     assert repr(DefaultModel(v=1).v) == '1'
```

### Comparing `pydantic-2.0a2/tests/test_types_namedtuple.py` & `pydantic-2.0a3/tests/test_types_namedtuple.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_types_payment_card_number.py` & `pydantic-2.0a3/tests/test_types_payment_card_number.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_types_typeddict.py` & `pydantic-2.0a3/tests/test_types_typeddict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_typing.py` & `pydantic-2.0a3/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_utils.py` & `pydantic-2.0a3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_validator.py` & `pydantic-2.0a3/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/test_validators.py` & `pydantic-2.0a3/tests/test_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import sys
 from collections import deque
 from datetime import date, datetime
 from enum import Enum
 from functools import partial, partialmethod
 from itertools import product
 from typing import Any, Callable, Deque, Dict, FrozenSet, List, Optional, Tuple, Type, Union
 from unittest.mock import MagicMock
@@ -1471,14 +1472,17 @@
             return value
 
     m = Model(name='hello')
     m.name = 'goodbye'
     assert validator_calls == 2
 
 
+@pytest.mark.xfail(
+    sys.version_info[:2] == (3, 8), reason='https://github.com/python/cpython/issues/103592', strict=False
+)
 def test_literal_validator():
     class Model(BaseModel):
         a: Literal['foo']
 
     Model(a='foo')
 
     with pytest.raises(ValidationError) as exc_info:
@@ -1490,15 +1494,14 @@
             'msg': "Input should be 'foo'",
             'input': 'nope',
             'ctx': {'expected': "'foo'"},
         }
     ]
 
 
-@pytest.mark.xfail(reason='working on V2 - enum validator bug https://github.com/pydantic/pydantic/issues/5242')
 def test_literal_validator_str_enum():
     class Bar(str, Enum):
         FIZ = 'fiz'
         FUZ = 'fuz'
 
     class Foo(BaseModel):
         bar: Bar
@@ -1514,14 +1517,17 @@
 
     my_foo = Foo.model_validate({'bar': 'fiz', 'barfiz': 'fiz', 'fizfuz': 'fuz'})
     assert my_foo.bar is Bar.FIZ
     assert my_foo.barfiz is Bar.FIZ
     assert my_foo.fizfuz is Bar.FUZ
 
 
+@pytest.mark.xfail(
+    sys.version_info[:2] == (3, 8), reason='https://github.com/python/cpython/issues/103592', strict=False
+)
 def test_nested_literal_validator():
     L1 = Literal['foo']
     L2 = Literal['bar']
 
     class Model(BaseModel):
         a: Literal[L1, L2]
```

### Comparing `pydantic-2.0a2/tests/test_validators_dataclass.py` & `pydantic-2.0a3/tests/test_validators_dataclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import re
 from dataclasses import asdict, is_dataclass
 from typing import Any, List
 
 import pytest
-from dirty_equals import HasRepr, IsStr
+from dirty_equals import HasRepr
 
 from pydantic import ValidationError, root_validator
 from pydantic.dataclasses import dataclass
 from pydantic.decorators import field_validator
 
 
 def test_simple():
@@ -176,13 +175,13 @@
     with pytest.raises(ValidationError) as exc_info:
         MyDataclass(1, b='snap dragon')
     assert root_val_values == [{'a': 123, 'b': 'barbar'}, {'a': 1, 'b': 'snap dragonsnap dragon'}]
 
     assert exc_info.value.errors() == [
         {
             'ctx': {'error': 'foobar'},
-            'input': HasRepr(IsStr(regex=re.escape("ArgsKwargs((1,), {'b': 'snap dragon'})"))),
+            'input': HasRepr("ArgsKwargs((1,), {'b': 'snap dragon'})"),
             'loc': (),
             'msg': 'Value error, foobar',
             'type': 'value_error',
         }
     ]
```

### Comparing `pydantic-2.0a2/tests/test_version.py` & `pydantic-2.0a3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/test_mypy.py` & `pydantic-2.0a3/tests/mypy/test_mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,23 @@
     ('mypy-plugin-strict.ini', 'plugin_success_baseConfig.py', 'plugin-success-strict-baseConfig.txt'),
     ('mypy-plugin-strict.ini', 'plugin_fail_baseConfig.py', 'plugin-fail-strict-baseConfig.txt'),
     ('mypy-default.ini', 'plugin_success_baseConfig.py', 'plugin_success_baseConfig.txt'),
     ('pyproject-plugin.toml', 'plugin_success_baseConfig.py', None),
     ('pyproject-plugin.toml', 'plugin_fail_baseConfig.py', 'plugin-fail-baseConfig.txt'),
     ('pyproject-plugin-strict.toml', 'plugin_success_baseConfig.py', 'plugin-success-strict-baseConfig.txt'),
     ('pyproject-plugin-strict.toml', 'plugin_fail_baseConfig.py', 'plugin-fail-strict-baseConfig.txt'),
+    pytest.param(
+        'pyproject-default.toml',
+        'computed_fields.py',
+        'computed_fields.txt',
+        marks=pytest.mark.skipif(
+            sys.version_info < (3, 8) or MYPY_VERSION_TUPLE < (0, 982),
+            reason='cached_property is only available in Python 3.8+, errors are different with mypy 0.971',
+        ),
+    ),
 ]
 
 
 def build_executable_modules():
     """
     Iterates over the test cases and returns a list of modules that should be executable.
     Specifically, we include any modules that are not expected to produce any typechecking errors.
@@ -197,26 +206,27 @@
     with pytest.raises(ValueError) as e:
         mypy_api.run(command)
 
     assert str(e.value) == 'Configuration value must be a boolean for key: init_forbid_extra'
 
 
 @pytest.mark.parametrize('module', sorted(executable_modules))
+@pytest.mark.filterwarnings('ignore:.*is deprecated.*:DeprecationWarning')
 def test_success_cases_run(module: str) -> None:
     """
     Ensure the "success" files can actually be executed
     """
     importlib.import_module(f'tests.mypy.modules.{module}')
 
 
 def test_explicit_reexports():
     from pydantic import __all__ as root_all
+    from pydantic.deprecated.tools import __all__ as tools
     from pydantic.main import __all__ as main
     from pydantic.networks import __all__ as networks
-    from pydantic.tools import __all__ as tools
     from pydantic.types import __all__ as types
 
     for name, export_all in [('main', main), ('network', networks), ('tools', tools), ('types', types)]:
         for export in export_all:
             assert export in root_all, f'{export} is in {name}.__all__ but missing from re-export in __init__.py'
```

### Comparing `pydantic-2.0a2/tests/mypy/configs/mypy-plugin-strict-no-any.ini` & `pydantic-2.0a3/tests/mypy/configs/mypy-plugin-strict-no-any.ini`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/configs/pyproject-default.toml` & `pydantic-2.0a3/tests/mypy/configs/pyproject-default.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/configs/pyproject-plugin-bad-param.toml` & `pydantic-2.0a3/tests/mypy/configs/pyproject-plugin-bad-param.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/configs/pyproject-plugin-strict.toml` & `pydantic-2.0a3/tests/mypy/configs/pyproject-plugin-strict.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/configs/pyproject-plugin.toml` & `pydantic-2.0a3/tests/mypy/configs/pyproject-plugin.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/modules/fail4.py` & `pydantic-2.0a3/tests/mypy/modules/fail4.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 
-from pydantic import BaseModel, root_validator, validate_arguments
+from pydantic import BaseModel, root_validator, validate_call
 
 
-@validate_arguments
+@validate_call
 def foo(a: int, *, c: str = 'x') -> str:
     return c * a
 
 
 # ok
 x: str = foo(1, c='hello')
 # fails
@@ -15,15 +15,15 @@
 foo(1, c=1)
 foo(1, 2)
 foo(1, d=2)
 # mypy assumes foo is just a function
 callable(foo.raw_function)
 
 
-@validate_arguments
+@validate_call
 def bar() -> str:
     return 'x'
 
 
 # return type should be a string
 y: int = bar()
```

### Comparing `pydantic-2.0a2/tests/mypy/modules/plugin_default_factory.py` & `pydantic-2.0a3/tests/mypy/modules/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/modules/plugin_fail.py` & `pydantic-2.0a3/tests/mypy/modules/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/modules/plugin_fail_baseConfig.py` & `pydantic-2.0a3/tests/mypy/modules/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/modules/plugin_success.py` & `pydantic-2.0a3/tests/mypy/modules/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/modules/plugin_success_baseConfig.py` & `pydantic-2.0a3/tests/mypy/modules/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/modules/success.py` & `pydantic-2.0a3/tests/mypy/modules/success.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     StrictFloat,
     StrictInt,
     StrictStr,
     UrlConstraints,
     field_validator,
     parse_obj_as,
     root_validator,
-    validate_arguments,
+    validate_call,
 )
 from pydantic.fields import Field, PrivateAttr
 from pydantic.networks import AnyUrl
 
 
 class Flags(BaseModel):
     strict_bool: StrictBool = False
@@ -152,25 +152,25 @@
 
 class WithField(BaseModel):
     age: int
     first_name: str = Field('John', max_length=42)
 
 
 # simple decorator
-@validate_arguments
+@validate_call
 def foo(a: int, *, c: str = 'x') -> str:
     return c * a
 
 
 foo(1, c='thing')
 foo(1)
 
 
 # nested decorator should not produce an error
-@validate_arguments(config={'arbitrary_types_allowed': True})
+@validate_call(config={'arbitrary_types_allowed': True})
 def bar(a: int, *, c: str = 'x') -> str:
     return c * a
 
 
 bar(1, c='thing')
 bar(1)
```

### Comparing `pydantic-2.0a2/tests/mypy/outputs/latest/fail4.txt` & `pydantic-2.0a3/tests/mypy/outputs/latest/fail4.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt` & `pydantic-2.0a3/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt` & `pydantic-2.0a3/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-strict.txt` & `pydantic-2.0a3/tests/mypy/outputs/latest/plugin-fail-strict.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail.txt` & `pydantic-2.0a3/tests/mypy/outputs/latest/plugin-fail.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/.gitignore` & `pydantic-2.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/LICENSE` & `pydantic-2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a2/pyproject.toml` & `pydantic-2.0a3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     'Framework :: Pydantic',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 requires-python = '>=3.7'
 dependencies = [
     'typing-extensions>=4.2.0',
-    'pydantic-core==0.23.1',
+    'pydantic-core==0.25.0',
     'annotated-types>=0.4.0',
 ]
 optional-dependencies = { email = ['email-validator>=1.3.0'] }
 dynamic = ['version', 'readme']
 
 entry-points.hypothesis = {_ = 'pydantic._hypothesis_plugin'}
 
@@ -121,15 +121,17 @@
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
     'pragma: no cover',
     'raise NotImplementedError',
     'if TYPE_CHECKING:',
+    'if typing.TYPE_CHECKING:',
     '@overload',
+    '@typing.overload',
     '\(Protocol\):$',
 ]
 
 [tool.coverage.paths]
 source = [
     'pydantic/',
     '/Users/runner/work/pydantic/pydantic/pydantic/',
@@ -141,7 +143,12 @@
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
 
 [tool.pyright]
 include = ['pydantic']
 exclude = ['pydantic/_hypothesis_plugin.py', 'pydantic/mypy.py']
+
+[tool.codespell]
+skip = '.git,env*'
+# `ser` - abbreviation for "ser"ialisation
+ignore-words-list = 'gir,ser'
```

### Comparing `pydantic-2.0a2/PKG-INFO` & `pydantic-2.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic
-Version: 2.0a2
+Version: 2.0a3
 Summary: Data validation using Python type hints
 Project-URL: Homepage, https://github.com/pydantic/pydantic
 Project-URL: Documentation, https://docs.pydantic.dev
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic
 Project-URL: Changelog, https://docs.pydantic.dev/changelog
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Terrence Dorsey <terry@pydantic.dev>, David Montague <david@pydantic.dev>
@@ -31,15 +31,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: annotated-types>=0.4.0
-Requires-Dist: pydantic-core==0.23.1
+Requires-Dist: pydantic-core==0.25.0
 Requires-Dist: typing-extensions>=4.2.0
 Provides-Extra: email
 Requires-Dist: email-validator>=1.3.0; extra == 'email'
 Description-Content-Type: text/markdown
 
 # Pydantic
 
@@ -108,14 +108,20 @@
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/pydantic/security/policy).
 
 ## Changelog
 
+## v2.0a3 (2023-04-20)
+
+Third pre-release of Pydantic V2
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0a3)
+
 ## v2.0a2 (2023-04-12)
 
 Second pre-release of Pydantic V2
 
 See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0a2)
 
 ## v2.0a1 (2023-04-03)
```

