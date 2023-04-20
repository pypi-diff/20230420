# Comparing `tmp/Warg-1.1.3.tar.gz` & `tmp/Warg-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Warg-1.1.3.tar", last modified: Tue Feb 28 15:39:10 2023, max compression
+gzip compressed data, was "Warg-1.1.4.tar", last modified: Thu Apr 20 06:13:50 2023, max compression
```

## Comparing `Warg-1.1.3.tar` & `Warg-1.1.4.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.738595 Warg-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.718595 Warg-1.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-02-28 15:38:55.000000 Warg-1.1.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 15:38:55.000000 Warg-1.1.3/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-28 15:38:55.000000 Warg-1.1.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-28 15:38:55.000000 Warg-1.1.3/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-02-28 15:38:55.000000 Warg-1.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-28 15:38:55.000000 Warg-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-02-28 15:39:10.738595 Warg-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-02-28 15:38:55.000000 Warg-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-28 15:38:55.000000 Warg-1.1.3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.722595 Warg-1.1.3/Warg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-02-28 15:39:10.000000 Warg-1.1.3/Warg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-02-28 15:39:10.000000 Warg-1.1.3/Warg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 15:39:10.000000 Warg-1.1.3/Warg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-28 15:39:10.000000 Warg-1.1.3/Warg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-28 15:39:10.000000 Warg-1.1.3/Warg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.722595 Warg-1.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-28 15:38:55.000000 Warg-1.1.3/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-28 15:38:55.000000 Warg-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-28 15:38:55.000000 Warg-1.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-28 15:39:10.738595 Warg-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-02-28 15:38:55.000000 Warg-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.722595 Warg-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_ast_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_collective.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_gdkc.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_nod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-28 15:38:55.000000 Warg-1.1.3/tests/test_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.726595 Warg-1.1.3/warg/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.726595 Warg-1.1.3/warg/ast_ops/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/ast_ops/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/ast_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/ast_ops/arg_indentifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/ast_ops/first_arg_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.730595 Warg-1.1.3/warg/bases/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/bases/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/bases/property_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/boolean_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/business.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.730595 Warg-1.1.3/warg/colors/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/colors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/colors/color_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/colors/css_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/colors/label_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/config_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/context_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.730595 Warg-1.1.3/warg/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/data_structures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/data_structures/auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/data_structures/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/data_structures/named_ordered_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/data_structures/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/data_structures/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.730595 Warg-1.1.3/warg/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.734595 Warg-1.1.3/warg/decorators/caching/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/caching/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/caching/look_up_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/caching/property_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/exporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13097 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/decorators/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/gdkc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.734595 Warg-1.1.3/warg/generators/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/generators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/generators/cyclic_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/generators/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/generators/mapping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/generators/zipping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/map_itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.734595 Warg-1.1.3/warg/math_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/math_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/math_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/math_utilities/multiples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/math_utilities/ordinals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/math_utilities/powers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.734595 Warg-1.1.3/warg/metas/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/metas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/metas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/metas/post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/metas/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.734595 Warg-1.1.3/warg/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/mixins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/mixins/dict_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/mixins/ordinal_index_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/mixins/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/ode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:39:10.738595 Warg-1.1.3/warg/os_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/os_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/os_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/os_utilities/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/os_utilities/os_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/os_utilities/path_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/os_utilities/path_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/os_utilities/platform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-02-28 15:38:55.000000 Warg-1.1.3/warg/typing_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.401847 Warg-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.389846 Warg-1.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-20 06:13:41.000000 Warg-1.1.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:41.000000 Warg-1.1.4/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 06:13:41.000000 Warg-1.1.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 06:13:41.000000 Warg-1.1.4/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-20 06:13:41.000000 Warg-1.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-20 06:13:41.000000 Warg-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-20 06:13:50.401847 Warg-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-04-20 06:13:41.000000 Warg-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-20 06:13:41.000000 Warg-1.1.4/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.389846 Warg-1.1.4/Warg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-20 06:13:50.000000 Warg-1.1.4/Warg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-20 06:13:50.000000 Warg-1.1.4/Warg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:13:50.000000 Warg-1.1.4/Warg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-20 06:13:50.000000 Warg-1.1.4/Warg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 06:13:50.000000 Warg-1.1.4/Warg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.389846 Warg-1.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 06:13:41.000000 Warg-1.1.4/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-20 06:13:41.000000 Warg-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 06:13:41.000000 Warg-1.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 06:13:50.401847 Warg-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-20 06:13:41.000000 Warg-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.389846 Warg-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_ast_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_gdkc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_nod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 06:13:41.000000 Warg-1.1.4/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.393847 Warg-1.1.4/warg/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.393847 Warg-1.1.4/warg/ast_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/ast_ops/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/ast_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/ast_ops/arg_indentifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/ast_ops/first_arg_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.393847 Warg-1.1.4/warg/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/bases/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/bases/property_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/boolean_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/business.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.397847 Warg-1.1.4/warg/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/colors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/colors/color_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/colors/css_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/colors/label_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/config_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/context_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.397847 Warg-1.1.4/warg/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/data_structures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/data_structures/auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/data_structures/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16677 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/data_structures/named_ordered_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/data_structures/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/data_structures/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.397847 Warg-1.1.4/warg/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.397847 Warg-1.1.4/warg/decorators/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/caching/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/caching/look_up_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/caching/property_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/exporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/decorators/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/gdkc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.397847 Warg-1.1.4/warg/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/generators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/generators/cyclic_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/generators/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/generators/mapping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/generators/zipping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/map_itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.397847 Warg-1.1.4/warg/math_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/math_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/math_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/math_utilities/multiples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/math_utilities/ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/math_utilities/powers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.401847 Warg-1.1.4/warg/metas/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/metas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/metas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/metas/post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/metas/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.401847 Warg-1.1.4/warg/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/mixins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/mixins/dict_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/mixins/ordinal_index_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/mixins/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/ode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:50.401847 Warg-1.1.4/warg/os_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/os_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/os_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/os_utilities/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/os_utilities/os_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/os_utilities/path_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/os_utilities/path_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/os_utilities/platform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-20 06:13:41.000000 Warg-1.1.4/warg/typing_extension.py
```

### Comparing `Warg-1.1.3/.github/CODE_OF_CONDUCT.md` & `Warg-1.1.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/LICENSE.md` & `Warg-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/PKG-INFO` & `Warg-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.3
+Version: 1.1.4
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,17 +19,17 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: dev
+Provides-Extra: tests
 Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
```

### Comparing `Warg-1.1.3/README.md` & `Warg-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/SECURITY.md` & `Warg-1.1.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/Warg.egg-info/PKG-INFO` & `Warg-1.1.4/Warg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.3
+Version: 1.1.4
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,17 +19,17 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: dev
+Provides-Extra: tests
 Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
```

### Comparing `Warg-1.1.3/Warg.egg-info/SOURCES.txt` & `Warg-1.1.4/Warg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/Warg.egg-info/requires.txt` & `Warg-1.1.4/Warg.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 setuptools>=60.9.3
 
 [all]
-pytest-runner
-sphinxcontrib-programoutput
+pytest-cov>=2.6.1
 pytest>=4.3.0
+tox
 black>=18.9b0
+wheel>=0.33.0
 setuptools>=60.9.3
+pytest-runner
+sphinxcontrib-programoutput
 pip>=19.0.3
 coveralls>=1.6.0
-wheel>=0.33.0
-tox
-twine>=1.13.0
-warg
 sphinx
-pytest-cov>=2.6.1
 apppath
+twine>=1.13.0
+warg
 
 [dev]
-sphinx
-pytest-runner
-sphinxcontrib-programoutput
+pytest-cov>=2.6.1
 pytest>=4.3.0
+tox
 black>=18.9b0
+wheel>=0.33.0
 setuptools>=60.9.3
+pytest-runner
+sphinxcontrib-programoutput
+pip>=19.0.3
 coveralls>=1.6.0
-wheel>=0.33.0
-tox
+sphinx
+apppath
 twine>=1.13.0
 warg
-pip>=19.0.3
-pytest-cov>=2.6.1
-apppath
 
 [docs]
 sphinxcontrib-programoutput
-warg
 sphinx
 apppath
+warg
 
 [setup]
 pytest-runner
 
 [tests]
 pytest-cov>=2.6.1
-tox
 pytest>=4.3.0
+tox
```

### Comparing `Warg-1.1.3/pyproject.toml` & `Warg-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/setup.py` & `Warg-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_arguments.py` & `Warg-1.1.4/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_ast_ops.py` & `Warg-1.1.4/tests/test_ast_ops.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_auto_dict.py` & `Warg-1.1.4/tests/test_auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_collective.py` & `Warg-1.1.4/tests/test_collective.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_gdkc.py` & `Warg-1.1.4/tests/test_gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_imports.py` & `Warg-1.1.4/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_kw_passing.py` & `Warg-1.1.4/tests/test_kw_passing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_nod.py` & `Warg-1.1.4/tests/test_nod.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_post_init.py` & `Warg-1.1.4/tests/test_post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/tests/test_singleton.py` & `Warg-1.1.4/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/__init__.py` & `Warg-1.1.4/warg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from warnings import warn
 
 import pkg_resources
 
 __project__ = "Warg"
 
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 __doc__ = r"""
 Created on 27/04/2019
 
 @author: cnheider
 
 """
```

### Comparing `Warg-1.1.3/warg/arguments.py` & `Warg-1.1.4/warg/arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/ast_ops/arg_indentifier.py` & `Warg-1.1.4/warg/ast_ops/arg_indentifier.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/ast_ops/first_arg_identifier.py` & `Warg-1.1.4/warg/ast_ops/first_arg_identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,18 @@
                 else:
                     iter_name = "iterable"
             self.result[node.func.id][node.lineno] = iter_name
         self.generic_visit(node)  # visit the children
 
 
 def get_first_arg_name(
-    func_name: str, *, verbose=False, max_num_intermediate_unnamed_elements=-1  # recurse = -1
+    func_name: str,
+    *,
+    verbose=False,
+    max_num_intermediate_unnamed_elements=-1,  # recurse = -1
 ) -> Optional[str]:
     """description"""
     import inspect
     import textwrap
     import ast
 
     caller_frame = inspect.currentframe().f_back.f_back
```

### Comparing `Warg-1.1.3/warg/bases/property_settings.py` & `Warg-1.1.4/warg/bases/property_settings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/boolean_tests.py` & `Warg-1.1.4/warg/boolean_tests.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/business.py` & `Warg-1.1.4/warg/business.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/colors/color_conversion.py` & `Warg-1.1.4/warg/colors/color_conversion.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/colors/css_colors.py` & `Warg-1.1.4/warg/colors/css_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/colors/label_colors.py` & `Warg-1.1.4/warg/colors/label_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/config_shell.py` & `Warg-1.1.4/warg/config_shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,15 +112,20 @@
                     deleter = lambda *e: prop.fdel(ps)
                     deleter.__doc__ = prop.fdel.__doc__
                 else:
                     deleter = None
                 self.add_option(p, getter=getter, setter=setter, deleter=deleter)
 
     def add_option(
-        self, key: str, *, getter: callable, setter: callable, deleter: Optional[callable] = None
+        self,
+        key: str,
+        *,
+        getter: callable,
+        setter: callable,
+        deleter: Optional[callable] = None,
     ) -> None:
         """
 
         :param key:
         :type key:
         :param getter:
         :type getter:
```

### Comparing `Warg-1.1.3/warg/context_wrapper.py` & `Warg-1.1.4/warg/context_wrapper.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/contexts.py` & `Warg-1.1.4/warg/contexts.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/data_structures/auto_dict.py` & `Warg-1.1.4/warg/data_structures/auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/data_structures/mappings.py` & `Warg-1.1.4/warg/data_structures/mappings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/data_structures/named_ordered_dictionary.py` & `Warg-1.1.4/warg/data_structures/named_ordered_dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     assert nodict.paramA == 20
     """
 
     # __slots__ = ('_unnamed_arg_i','__dict__')
 
     # _unnamed_arg_i = 0
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         # super().__init__(**kwargs)
         if len(args) == 1 and isinstance(args[0], dict):
             args_dict = args[0]
         else:
             args_dict = {}
             if len(args) == 1 and isinstance(args[0], Iterable):
                 args = args[0]
@@ -350,36 +350,36 @@
         if len(items) > 0:
             for key, value in items:
                 print_str += f"'{key}': {value}, "
             print_str = print_str[:-2]
         print_str += ")"
         return print_str
 
-    def update(self, *args: Sequence, **kwargs: MutableMapping) -> T:
+    def update(self, *args: Any, **kwargs: Any) -> T:
         """
         Merge two attributes, overriding any repeated keys from
         the `items` parameter.
 
         :returns self
 
         Args:
         items (dict): Python dictionary containing updated values."""
 
         if len(args) == 1 and isinstance(args[0], Mapping):
-            a = args[0]
+            a: Mapping = args[0]
             if RECURSE_MAPPING_CONVERSION and True:
                 l = {}
                 for k, v in a.items():
                     l[k] = recurse_conversion(self, v)
                 a = l
 
             args_dict = a
         elif len(args):
             args_dict = {}
-            a = list(self.__dict__.keys())
+            a: List = list(self.__dict__.keys())
             if True:  # be same length guard
                 assert len(a) == len(args)
             for arg, key in zip(args, a):
                 if RECURSE_MAPPING_CONVERSION and True:
                     arg = recurse_conversion(self, arg)
 
                 args_dict[key] = arg
```

### Comparing `Warg-1.1.3/warg/data_structures/ordered_set.py` & `Warg-1.1.4/warg/data_structures/ordered_set.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/data_structures/sequences.py` & `Warg-1.1.4/warg/data_structures/sequences.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/datetimes.py` & `Warg-1.1.4/warg/datetimes.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/debug.py` & `Warg-1.1.4/warg/debug.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/decorators/caching/look_up_table.py` & `Warg-1.1.4/warg/decorators/caching/look_up_table.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/decorators/caching/property_caching.py` & `Warg-1.1.4/warg/decorators/caching/property_caching.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/decorators/exporting.py` & `Warg-1.1.4/warg/decorators/exporting.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/decorators/hashing.py` & `Warg-1.1.4/warg/decorators/hashing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/decorators/kw_passing.py` & `Warg-1.1.4/warg/decorators/kw_passing.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,22 @@
     :param receiver_func:
     :type receiver_func:
     :param keep_from_var_kw:
     :type keep_from_var_kw:
     :return:
     :rtype:"""
     passing_params: dict = dict(passing_sig.parameters)
-    receiver_params = inspect.signature(receiver_func).parameters
+    # if inspect.isfunction()
+    # if inspect.ismethod()
+    # arg_spec_sig = inspect.getfullargspec(receiver_func)[0]
+
+    receiver_params = inspect.signature(
+        receiver_func
+    ).parameters  # TODO: Sometime no signature is found resulting in
+    # a ValueError exception
 
     var_kw_key = None
     var_kw = None
     for k, v in passing_params.items():
         if v.kind == inspect._ParameterKind.VAR_KEYWORD:
             var_kw_key = k
 
@@ -218,15 +225,19 @@
     - {
         "__annotations__",
     }
 )
 
 
 def pack_args(
-    f: callable, *, pack_name: str = "arg_pack", allow_passing: bool = True, verbose: bool = False
+    f: callable,
+    *,
+    pack_name: str = "arg_pack",
+    allow_passing: bool = True,
+    verbose: bool = False,
 ) -> callable:
     """
 
     :param pack_name:
     :type pack_name:
     :param f:
     :type f:
@@ -258,15 +269,19 @@
                 new_kwargs[pack_name] = args
         return f(*args, **new_kwargs)
 
     return wrapper
 
 
 def pack_kws(
-    f: callable, *, pack_name: str = "kw_pack", allow_passing: bool = True, verbose: bool = False
+    f: callable,
+    *,
+    pack_name: str = "kw_pack",
+    allow_passing: bool = True,
+    verbose: bool = False,
 ) -> callable:
     """
 
     :param pack_name:
     :type pack_name:
     :param f:
     :type f:
@@ -298,15 +313,19 @@
                 new_kwargs[pack_name] = kwargs
         return f(*args, **new_kwargs)
 
     return wrapper
 
 
 def pack_args_and_kws(
-    f: callable, *, pack_name: str = "arg_kw_pack", allow_passing: bool = True, verbose: bool = False
+    f: callable,
+    *,
+    pack_name: str = "arg_kw_pack",
+    allow_passing: bool = True,
+    verbose: bool = False,
 ) -> callable:
     """
 
     :param pack_name:
     :type pack_name:
     :param f:
     :type f:
```

### Comparing `Warg-1.1.3/warg/decorators/timing.py` & `Warg-1.1.4/warg/decorators/timing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/exceptions.py` & `Warg-1.1.4/warg/exceptions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/functions.py` & `Warg-1.1.4/warg/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,25 @@
     "last_key",
 ]
 
 import operator
 from collections import defaultdict
 from copy import deepcopy
 from functools import reduce
-from typing import Any, Callable, Dict, Iterable, Iterator, Mapping, Sequence, Tuple, List
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    Mapping,
+    Sequence,
+    Tuple,
+    List,
+)
 
 from warg import Number, drop_unused_kws
 
 
 def list_keys(d: Dict) -> List[Any]:
     return list(d.keys())
```

### Comparing `Warg-1.1.3/warg/gdkc.py` & `Warg-1.1.4/warg/gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/generators/cyclic_generators.py` & `Warg-1.1.4/warg/generators/cyclic_generators.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/generators/filtering.py` & `Warg-1.1.4/warg/generators/filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 class FilterModeEnum(Enum):
     """
     Filter Mode
     """
 
     # exclude_postfix, exclude_prefix, exclude_fully = assigned_names()
     # TODO: Include variants
-    exclude_postfix, exclude_prefix, exclude_fully = "exclude_postfix", "exclude_prefix", "exclude_fully"
+    exclude_postfix, exclude_prefix, exclude_fully = (
+        "exclude_postfix",
+        "exclude_prefix",
+        "exclude_fully",
+    )
 
 
 def symbol_filter(
     string_stream: Iterable,
     symbol: str = "#",
     *,
     exclusion_mode: FilterModeEnum = FilterModeEnum.exclude_postfix,
```

### Comparing `Warg-1.1.3/warg/generators/mapping_generator.py` & `Warg-1.1.4/warg/generators/mapping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/generators/zipping_generator.py` & `Warg-1.1.4/warg/generators/zipping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/importing.py` & `Warg-1.1.4/warg/importing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/manipulation.py` & `Warg-1.1.4/warg/manipulation.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/map_itertools.py` & `Warg-1.1.4/warg/map_itertools.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/math_utilities/ordinals.py` & `Warg-1.1.4/warg/math_utilities/ordinals.py`

 * *Files 11% similar despite different names*

```diff
@@ -105,9 +105,18 @@
 
 if __name__ == "__main__":
     from warg.ast_ops import cprint
     import numpy
 
     for a in numpy.arange(-1.0, 10.0, 0.5):
         cprint(a)
-        for f in (ceil_odd, ceil_even, floor_even, floor_odd, next_even, next_odd, prev_even, prev_odd):
+        for f in (
+            ceil_odd,
+            ceil_even,
+            floor_even,
+            floor_odd,
+            next_even,
+            next_odd,
+            prev_even,
+            prev_odd,
+        ):
             print(f.__name__, f(a))
```

### Comparing `Warg-1.1.3/warg/math_utilities/powers.py` & `Warg-1.1.4/warg/math_utilities/powers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/metas/post_init.py` & `Warg-1.1.4/warg/metas/post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/metas/singleton.py` & `Warg-1.1.4/warg/metas/singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/mixins/dict_mixins.py` & `Warg-1.1.4/warg/mixins/dict_mixins.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/mixins/ordinal_index_mixin.py` & `Warg-1.1.4/warg/mixins/ordinal_index_mixin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/ode.py` & `Warg-1.1.4/warg/ode.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/os_utilities/filtering.py` & `Warg-1.1.4/warg/os_utilities/filtering.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/os_utilities/os_platform.py` & `Warg-1.1.4/warg/os_utilities/os_platform.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,9 +63,10 @@
     """
     test if display is available, if other than linux system atm it returns true
 
     :return:
     :rtype:
     """
     if is_nix():
-        return os.environ["DISPLAY"] != ""
+        return "DISPLAY" in os.environ and os.environ["DISPLAY"] != ""
+
     return True
```

### Comparing `Warg-1.1.3/warg/os_utilities/path_functions.py` & `Warg-1.1.4/warg/os_utilities/path_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,52 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 08/03/2020
            """
 
-__all__ = ["ensure_existence", "path_rmtree", "sanitise_path"]
+__all__ = ["ensure_existence", "path_rmtree", "sanitise_path", "path_join"]
 
 import os
 from itertools import cycle
 from pathlib import Path
 from shutil import rmtree
 from typing import Iterable, Union
 
+from warg.decorators import passes_kws_to
 
-# from warg import passes_kws_to
 
+def path_join(*p: Union[Path, str]) -> Path:
+    """
+    drop-in replacement for os.path.join, returning a Path instead
+
+    :param p: Sequence of path components to be joined
+    :type p:  Union[Path,str]
+    :return: Joined path
+    :rtype: Path
+    """
+    p, *rest = p
+    p = Path(p)
+    for r in rest:
+        p /= r
+    return p
 
-# @passes_kws_to(rmtree) Throws error due to import issues
+
+@passes_kws_to(rmtree)
 def path_rmtree(path: Path, **kwargs) -> None:
     """
     asses_kws_to rmtree from shutil
     :param path:
-    :type path:
+    :type path: Path
     :param kwargs:
-    :type kwargs:"""
+    :type kwargs:
+    :return: None
+    :rtype: None
+    """
     rmtree(str(path), **kwargs)
 
 
 def sanitise_path(
     path: Path,
     naughty_directory_symbols: Iterable[str] = (
         " ",
```

### Comparing `Warg-1.1.3/warg/os_utilities/path_utilities.py` & `Warg-1.1.4/warg/os_utilities/path_utilities.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/os_utilities/platform_selection.py` & `Warg-1.1.4/warg/os_utilities/platform_selection.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/plugin.py` & `Warg-1.1.4/warg/plugin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/replication.py` & `Warg-1.1.4/warg/replication.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/strings.py` & `Warg-1.1.4/warg/strings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/styling.py` & `Warg-1.1.4/warg/styling.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/text.py` & `Warg-1.1.4/warg/text.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.3/warg/typing_extension.py` & `Warg-1.1.4/warg/typing_extension.py`

 * *Files identical despite different names*

