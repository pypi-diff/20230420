# Comparing `tmp/pipelime_python-1.4.1.tar.gz` & `tmp/pipelime_python-1.5.0.tar.gz`

## Comparing `pipelime_python-1.4.1.tar` & `pipelime_python-1.5.0.tar`

### file list

```diff
@@ -1,115 +1,116 @@
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/__init__.py
--rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/xconfig.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/ast/__init__.py
--rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/ast/nodes.py
--rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/ast/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/utils/__init__.py
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/utils/common.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/utils/imports.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/utils/io.py
--rw-r--r--   0        0        0    13100 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/utils/rand.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/visitors/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/visitors/decoder.py
--rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/visitors/inspector.py
--rw-r--r--   0        0        0    13127 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/visitors/processor.py
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/visitors/unparser.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/choixe/visitors/walker.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/cli/__init__.py
--rw-r--r--   0        0        0    25204 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/cli/main.py
--rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/cli/parser.py
--rw-r--r--   0        0        0    15042 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/cli/pretty_print.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/cli/subcommands.py
--rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/cli/utils.py
--rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/cli/wizard.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/commands/__init__.py
--rw-r--r--   0        0        0    26693 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/commands/general.py
--rw-r--r--   0        0        0    28071 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/commands/interfaces.py
--rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/commands/piper.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/commands/shell.py
--rw-r--r--   0        0        0    13586 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/commands/split_ops.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/commands/toy_dataset.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/items/__init__.py
--rw-r--r--   0        0        0    30704 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/items/base.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/items/binary_item.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/items/image_item.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/items/metadata_item.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/items/model3d_item.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/items/numpy_item.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/items/pickle_item.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/__init__.py
--rw-r--r--   0        0        0    18226 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/graph.py
--rw-r--r--   0        0        0    15533 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/drawing/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/drawing/base.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/drawing/factory.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/drawing/graphviz.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/drawing/mermaid.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/executors/__init__.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/executors/base.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/executors/factory.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/executors/naive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/parsers/__init__.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/parsers/base.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/parsers/choixe_parser.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/parsers/factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/__init__.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/estimator/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/estimator/base.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/estimator/factory.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/estimator/naive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/listener/__init__.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/listener/base.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/listener/factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/listener/callbacks/__init__.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/listener/callbacks/file.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/listener/callbacks/rich_table.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/listener/callbacks/tqdm_bars.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/listener/receiver/__init__.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/listener/receiver/zmq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/tracker/__init__.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/tracker/base.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/tracker/direct.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/tracker/factory.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/tracker/loguru.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/piper/progress/tracker/zmq.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/remotes/__init__.py
--rw-r--r--   0        0        0    12825 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/remotes/base.py
--rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/remotes/s3_remote.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/remotes/shared_folder_remote.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/direct_access.py
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/grabber.py
--rw-r--r--   0        0        0     8682 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/sample.py
--rw-r--r--   0        0        0    22718 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/samples_sequence.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/torch.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/pipes/__init__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/pipes/base.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/pipes/mapping.py
--rw-r--r--   0        0        0    14098 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/pipes/operations.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/pipes/validation.py
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/pipes/writers.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/sources/__init__.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/sources/from_callable.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/sources/raw.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/sources/readers.py
--rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/sequences/sources/toy_dataset.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/stages/__init__.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/stages/augmentations.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/stages/base.py
--rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/stages/entities.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/stages/item_info.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/stages/item_replacement.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/stages/item_sources.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/stages/key_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/utils/__init__.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/utils/context_managers.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/utils/inspection.py
--rw-r--r--   0        0        0    23458 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pipelime/utils/pydantic_types.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/LICENSE
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/README.md
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 pipelime_python-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/__init__.py
+-rw-r--r--   0        0        0    10465 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/xconfig.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/ast/__init__.py
+-rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/ast/nodes.py
+-rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/ast/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/utils/__init__.py
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/utils/common.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/utils/imports.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/utils/io.py
+-rw-r--r--   0        0        0    13100 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/utils/rand.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/visitors/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/visitors/decoder.py
+-rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/visitors/inspector.py
+-rw-r--r--   0        0        0    13803 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/visitors/processor.py
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/visitors/unparser.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/choixe/visitors/walker.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/cli/__init__.py
+-rw-r--r--   0        0        0    26097 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/cli/main.py
+-rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/cli/parser.py
+-rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/cli/pretty_print.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/cli/subcommands.py
+-rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/cli/utils.py
+-rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/cli/wizard.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/commands/__init__.py
+-rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/commands/general.py
+-rw-r--r--   0        0        0    28216 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/commands/interfaces.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/commands/piper.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/commands/shell.py
+-rw-r--r--   0        0        0    13525 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/commands/split_ops.py
+-rw-r--r--   0        0        0     9219 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/commands/tempman.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/commands/toy_dataset.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/items/__init__.py
+-rw-r--r--   0        0        0    30747 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/items/base.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/items/binary_item.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/items/image_item.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/items/metadata_item.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/items/model3d_item.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/items/numpy_item.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/items/pickle_item.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/__init__.py
+-rw-r--r--   0        0        0    18226 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/graph.py
+-rw-r--r--   0        0        0    15533 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/drawing/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/drawing/base.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/drawing/factory.py
+-rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/drawing/graphviz.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/drawing/mermaid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/executors/__init__.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/executors/base.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/executors/factory.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/executors/naive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/parsers/__init__.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/parsers/base.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/parsers/choixe_parser.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/parsers/factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/__init__.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/estimator/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/estimator/base.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/estimator/factory.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/estimator/naive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/listener/__init__.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/listener/base.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/listener/factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/listener/callbacks/__init__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/listener/callbacks/file.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/listener/callbacks/rich_table.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/listener/callbacks/tqdm_bars.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/listener/receiver/__init__.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/listener/receiver/zmq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/tracker/__init__.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/tracker/base.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/tracker/direct.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/tracker/factory.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/tracker/loguru.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/piper/progress/tracker/zmq.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/remotes/__init__.py
+-rw-r--r--   0        0        0    12825 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/remotes/base.py
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/remotes/s3_remote.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/remotes/shared_folder_remote.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/direct_access.py
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/grabber.py
+-rw-r--r--   0        0        0     8682 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/sample.py
+-rw-r--r--   0        0        0    22718 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/samples_sequence.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/torch.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/pipes/__init__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/pipes/base.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/pipes/mapping.py
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/pipes/operations.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/pipes/validation.py
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/pipes/writers.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/sources/__init__.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/sources/from_callable.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/sources/raw.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/sources/readers.py
+-rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/sequences/sources/toy_dataset.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/stages/__init__.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/stages/augmentations.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/stages/base.py
+-rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/stages/entities.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/stages/item_info.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/stages/item_replacement.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/stages/item_sources.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/stages/key_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/utils/__init__.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/utils/context_managers.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/utils/inspection.py
+-rw-r--r--   0        0        0    23458 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pipelime/utils/pydantic_types.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/LICENSE
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/README.md
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 pipelime_python-1.5.0/PKG-INFO
```

### Comparing `pipelime_python-1.4.1/pipelime/choixe/xconfig.py` & `pipelime_python-1.5.0/pipelime/choixe/xconfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -222,43 +222,80 @@
             List[Tuple[List[Union[str, int]], Any]]: The walk output.
         """
         return walk(self.parse())
 
     def _process(
         self, context: Optional[Dict[str, Any]] = None, allow_branching: bool = True
     ) -> List[XConfig]:
-        data = process(
+        data = self._unsafe_process(context=context, allow_branching=allow_branching)
+        return [
+            XConfig(data=x, cwd=self.get_cwd(), schema=self.get_schema()) for x in data
+        ]
+
+    def _unsafe_process(
+        self, context: Optional[Dict[str, Any]] = None, allow_branching: bool = True
+    ) -> List[Any]:
+        return process(
             self.parse(),
             context=context,
             cwd=self.get_cwd(),
             allow_branching=allow_branching,
         )
-        return [
-            XConfig(data=x, cwd=self.get_cwd(), schema=self.get_schema()) for x in data
-        ]
 
     def process(self, context: Optional[Dict[str, Any]] = None) -> XConfig:
         """Process this XConfig without branching.
 
         Args:
             context (Optional[Dict[str, Any]], optional): Optional data structure
                 containing all variables values. Defaults to None.
 
         Returns:
             XConfig: The processed XConfig.
         """
         return self._process(context=context, allow_branching=False)[0]
 
+    def unsafe_process(self, context: Optional[Dict[str, Any]] = None) -> Any:
+        """Process this XConfig without branching and return the result, without
+        wrapping it in an XConfig to allow for more flexibility in the result.
+
+        No guarantees can be made about the result type, so it is up to the user to
+        handle it properly.
+
+        Args:
+            context (Optional[Dict[str, Any]], optional): Optional data structure
+                containing all variables values. Defaults to None.
+
+        Returns:
+            Any: The processed result.
+        """
+        return self._unsafe_process(context=context, allow_branching=False)[0]
+
     def process_all(self, context: Optional[Dict[str, Any]] = None) -> List[XConfig]:
         """Process this XConfig with branching.
 
         Args:
             context (Optional[Dict[str, Any]], optional): Optional data structure
                 containing all variables values. Defaults to None.
 
         Returns:
             List[XConfig]: A list of all processing outcomes.
         """
         return self._process(context=context, allow_branching=True)
 
+    def unsafe_process_all(self, context: Optional[Dict[str, Any]] = None) -> List[Any]:
+        """Process this XConfig with branching and return the results, without
+        wrapping them in XConfigs to allow for more flexibility in the result.
+
+        No guarantees can be made about the result types, so it is up to the user to
+        handle them properly.
+
+        Args:
+            context (Optional[Dict[str, Any]], optional): Optional data structure
+                containing all variables values. Defaults to None.
+
+        Returns:
+            List[Any]: A list of all processing outcomes.
+        """
+        return self._unsafe_process(context=context, allow_branching=True)
+
     def inspect(self) -> Inspection:
         return inspect(self.parse(), cwd=self.get_cwd())
```

### Comparing `pipelime_python-1.4.1/pipelime/choixe/ast/nodes.py` & `pipelime_python-1.5.0/pipelime/choixe/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/choixe/ast/parser.py` & `pipelime_python-1.5.0/pipelime/choixe/ast/parser.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/choixe/utils/common.py` & `pipelime_python-1.5.0/pipelime/choixe/utils/common.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/choixe/utils/imports.py` & `pipelime_python-1.5.0/pipelime/choixe/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/choixe/utils/rand.py` & `pipelime_python-1.5.0/pipelime/choixe/utils/rand.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/choixe/visitors/decoder.py` & `pipelime_python-1.5.0/pipelime/choixe/visitors/decoder.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/choixe/visitors/inspector.py` & `pipelime_python-1.5.0/pipelime/choixe/visitors/inspector.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/choixe/visitors/processor.py` & `pipelime_python-1.5.0/pipelime/choixe/visitors/processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import os
-import tempfile
 import uuid
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from itertools import product
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional
 
 import pydash as py_
 
 import pipelime.choixe.ast.nodes as ast
 from pipelime.choixe.ast.parser import parse
 from pipelime.choixe.utils.imports import import_symbol
-from pipelime.choixe.utils.io import load
+from pipelime.choixe.utils.io import load, PipelimeTmp
 from pipelime.choixe.utils.rand import rand
 from pipelime.choixe.visitors.unparser import unparse
 
 
 class ChoixeProcessingError(Exception):
     pass
 
@@ -52,15 +51,14 @@
         super().__init__()
         self._context = context if context is not None else {}
         self._cwd = cwd if cwd is not None else Path(os.getcwd())
         self._allow_branching = allow_branching
 
         self._loop_data: Dict[str, LoopInfo] = {}
         self._current_loop: Optional[str] = None
-        self._tmp_name = uuid.uuid1().hex
 
     def _branches(self, *branches: List[Any]) -> List[Any]:
         if len(branches) == 1:
             return branches[0]
         return list(product(*branches))
 
     def _repeat(self, data: Any, n: int) -> List[Any]:
@@ -250,26 +248,44 @@
 
         all_branches = self._branches(
             value_branches, *set_branches, *body_branches, default_branches
         )
 
         branches = []
         for branch in all_branches:
-            value = py_.get(self._context, branch[0])
+            varname = branch[0]
+
+            # If the variable is not in the context, raise an error
+            if not py_.has(self._context, varname):
+                msg = f"Switch variable `{varname}` not found in context"
+                raise ChoixeProcessingError(msg)
+
+            # Get the value of the variable
+            value = py_.get(self._context, varname)
+
+            # Match the value to the correct case
             for i in range(len(node.cases)):
                 set_ = branch[i + 1]
+
+                # If the set is not iterable, make it a list
                 if not isinstance(set_, Iterable) or isinstance(set_, str):
                     set_ = [set_]
 
+                # If the value is in the set, use the corresponding branch and break
                 if value in set_:
                     branches.append(branch[i + 1 + len(node.cases)])
                     break
+
+            # If no case matched, use the default if available, otherwise raise an error
             else:
                 if node.default is not None:
                     branches.append(branch[-1])
+                else:
+                    msg = f"Switch variable `{varname}`={value} did not match any case"
+                    raise ChoixeProcessingError(msg)
 
         return branches
 
     def visit_index(self, node: ast.IndexNode) -> List[Any]:
         branches = (
             node.identifier.accept(self) if node.identifier else [self._current_loop]
         )
@@ -305,19 +321,18 @@
             subp = os.popen(str(branch))
             stdout = subp.read()
             stdouts.append(stdout)
         return stdouts
 
     def visit_tmp_dir(self, node: ast.TmpDirNode) -> Any:
         paths = []
-        branches = node.name.accept(self) if node.name else [self._tmp_name]
+        branches = node.name.accept(self) if node.name else [""]
         for branch in branches:
-            path = Path(tempfile.gettempdir()) / str(branch)
-            path.parent.mkdir(exist_ok=True, parents=True)
-            paths.append(str(path))
+            path = PipelimeTmp.make_subdir(str(branch))
+            paths.append(path.resolve().absolute().as_posix())
         return paths
 
     def visit_rand(self, node: ast.RandNode) -> Any:
         args_branches = [
             node.args[i].accept(self) if i < len(node.args) else [...] for i in range(3)
         ]
         n_branches = node.n.accept(self) if node.n else [...]
```

### Comparing `pipelime_python-1.4.1/pipelime/choixe/visitors/unparser.py` & `pipelime_python-1.5.0/pipelime/choixe/visitors/unparser.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import pipelime.choixe.ast.nodes as ast
 from pipelime.choixe.ast.parser import DIRECTIVE_PREFIX
 
 
 class Unparser(ast.NodeVisitor):
     """`NodeVisitor` for the `unparse` operation."""
 
+    def __init__(self):
+        self._allow_compact = True
+
     def visit_dict(self, node: ast.DictNode) -> Dict:
         data = {}
         for k, v in node.nodes.items():
             data[k.accept(self)] = v.accept(self)
         return data
 
     def visit_list(self, node: ast.ListNode) -> List:
@@ -25,15 +28,26 @@
     def visit_dict_bundle(self, node: ast.DictBundleNode) -> Any:
         data = {}
         for x in node.nodes:
             data.update(x.accept(self))
         return data
 
     def visit_str_bundle(self, node: ast.StrBundleNode) -> str:
-        return "".join(x.accept(self) for x in node.nodes)
+        # Disable compact mode for the duration of the bundle
+        # Because we don't want compact directives the middle of a string
+        # (e.g. "aaa$tmp()bbb" getting unparsed as "aaa$tmpbbb") and
+        # causing a parsing error.
+        old_allow_compact = self._allow_compact
+        self._allow_compact = False
+
+        result = "".join(x.accept(self) for x in node.nodes)
+
+        # Restore compact mode to its previous state
+        self._allow_compact = old_allow_compact
+        return result
 
     def visit_sweep(self, node: ast.SweepNode) -> Union[Dict, str]:
         return self._unparse_auto("sweep", *node.cases)
 
     def visit_var(self, node: ast.VarNode) -> Union[Dict, str]:
         kwargs = {}
         if node.default is not None:
@@ -139,24 +153,31 @@
 
     def _unparse_as_args(self, *nodes: ast.Node) -> str:
         return ", ".join([self._unparse_as_arg(x) for x in nodes])
 
     def _unparse_as_kwargs(self, **nodes: ast.Node) -> str:
         return ", ".join([f"{k}={self._unparse_as_arg(v)}" for k, v in nodes.items()])
 
-    def _unparse_compact(self, name: str) -> str:
+    def _directive_name(self, name: str) -> str:
         return f"{DIRECTIVE_PREFIX}{name}"
 
+    def _unparse_compact(self, name: str) -> str:
+        # If compact mode is not allowed, fall back to call syntax.
+        if not self._allow_compact:
+            return self._unparse_call(name)
+
+        return self._directive_name(name)
+
     def _unparse_call(self, name: str, *args: ast.Node, **kwargs: ast.Node) -> str:
         parts = []
         if len(args) > 0:
             parts.append(self._unparse_as_args(*args))
         if len(kwargs) > 0:
             parts.append(self._unparse_as_kwargs(**kwargs))
-        return f"{self._unparse_compact(name)}({', '.join(parts)})"
+        return f"{self._directive_name(name)}({', '.join(parts)})"
 
     def _unparse_extended(
         self, name: str, *args: ast.Node, **kwargs: ast.Node
     ) -> Dict[str, Any]:
         return {
             "$directive": name,
             "$args": [x.accept(self) for x in args],
```

### Comparing `pipelime_python-1.4.1/pipelime/choixe/visitors/walker.py` & `pipelime_python-1.5.0/pipelime/choixe/visitors/walker.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/cli/__init__.py` & `pipelime_python-1.5.0/pipelime/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/cli/main.py` & `pipelime_python-1.5.0/pipelime/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     cfg_name: str,
     run_all: t.Optional[bool],
     output: t.Optional[Path],
     exit_on_error: bool,
     verbose: bool,
     print_all: bool,
 ) -> t.List["XConfig"]:
-    from pipelime.cli.pretty_print import print_error, print_info
+    from pipelime.cli.pretty_print import print_error, print_info, print_warning
     from pipelime.choixe.visitors.processor import ChoixeProcessingError
 
     if verbose:
         print_info(f"> Processing {cfg_name}...")
 
     try:
         effective_configs = (
@@ -107,14 +107,20 @@
     except ChoixeProcessingError as e:
         if exit_on_error:
             print_error(
                 f"Invalid {cfg_name}! {e}\nRun with -vv or more to get more info."
             )
             raise typer.Exit(1)
         raise e
+    except RecursionError:
+        print_error(f"Recursion detected while processing {cfg_name}!")
+        print_warning(
+            "Please check your context for self-references, eg, `myvar: $var(myvar)`."
+        )
+        raise typer.Exit(1)
 
     if verbose:
         pls = "s" if len(effective_configs) != 1 else ""
         print_info(f"> Found {len(effective_configs)} {cfg_name}{pls}")
 
     if len(effective_configs) > 1 and run_all is None:
         if not typer.confirm(
@@ -227,15 +233,15 @@
         readable=True,
         resolve_path=True,
         help=(
             "One or more yaml/json files with some or "
             "all the arguments required by the command.\n\n"
             "`++opt` or `+opt` command line options update and override them.\n\n "
         ),
-        autocompletion=_complete_yaml,
+        # autocompletion=_complete_yaml,
     ),
     context: t.List[Path] = typer.Option(
         None,
         "--context",
         "-x",
         exists=True,
         file_okay=True,
@@ -248,15 +254,21 @@
             "If `--config` is set and `--context` is not, all files matching "
             "`*context*.[yaml|yml|json]` in the folders of all the "
             "configuration files will be loaded as the context. "
             "Use `--no-ctx-autoload` to disable this behavior.\n\n"
             "`@@opt` or `@opt` command line options update and override them.\n\n"
             "After a `//` token, `++opt` and `+opt` are accepted as well.\n\n "
         ),
-        autocompletion=_complete_yaml,
+        # autocompletion=_complete_yaml,
+    ),
+    keep_tmp: bool = typer.Option(
+        False,
+        "--keep-tmp",
+        "-t",
+        help="DO NOT remove temporary folders, if any, after running this command.",
     ),
     ctx_autoload: bool = typer.Option(
         True,
         help=(
             "Enable/disable context auto-loading when "
             "`--config` is set and `--context` is not."
         ),
@@ -301,20 +313,20 @@
             (
                 "A command, ie, a `command-name`, "
                 "a `package.module.ClassName` class path or "
                 "a `path/to/module.py:ClassName` uri (use with care).\n\n"
             )
             + subc.get_help()
         ),
-        autocompletion=PipelimeSymbolsHelper.complete_name(
-            is_cmd=True,
-            is_seq_op=False,
-            is_stage=False,
-            additional_names=subc.get_autocompletions(),
-        ),
+        # autocompletion=PipelimeSymbolsHelper.complete_name(
+        #     is_cmd=True,
+        #     is_seq_op=False,
+        #     is_stage=False,
+        #     additional_names=subc.get_autocompletions(),
+        # ),
     ),
     command_args: t.Optional[t.List[str]] = typer.Argument(
         None,
         help=(
             "\b\nExpected command line:\n"
             "- `++opt` and `+opt` are command parameters\n"
             "- `@@opt` and `@opt` are context parameters\n"
@@ -540,14 +552,16 @@
 
                 effective_ctx.extend(new_ctxs)
 
         if effective_ctx:
             effective_ctx = functools.reduce(
                 lambda acc, curr: _deep_update_fn(acc, curr, verbose > 3), effective_ctx
             )
+            if output_ctx:
+                effective_ctx.save_to(output_ctx)
         else:
             effective_ctx = XConfig()
 
         if verbose > 1:
             print_info("\nFinal effective context:")
             print_info(effective_ctx.to_dict(), pretty=True)
 
@@ -644,32 +658,41 @@
                         print_warning(
                             "You should use the `run` command to process a dag."
                         )
                         raise typer.Exit(1)
                     cmd_name = next(iter(cfg_dict))
                     cfg_dict = next(iter(cfg_dict.values()))
 
-                run_command(cmd_name, cfg_dict, verbose, dry_run)
+                run_command(cmd_name, cfg_dict, verbose, dry_run, keep_tmp)
     else:
         from pipelime.cli.pretty_print import print_error
 
         print_error("No command specified.")
         raise typer.Exit(1)
 
 
-def run_command(command: str, cmd_args: t.Mapping, verbose: int, dry_run: bool):
+def run_command(
+    command: str, cmd_args: t.Mapping, verbose: int, dry_run: bool, keep_tmp: bool
+):
     """
     Run a pipelime command.
     """
 
     import time
     from pydantic.error_wrappers import ValidationError
 
+    from pipelime.choixe.utils.io import PipelimeTmp
+    from pipelime.commands import TempCommand
+
     from pipelime.cli.pretty_print import print_info, print_command_outputs
-    from pipelime.cli.utils import get_pipelime_command_cls, time_to_str, show_field_alias_valerr
+    from pipelime.cli.utils import (
+        get_pipelime_command_cls,
+        time_to_str,
+        show_field_alias_valerr,
+    )
 
     try:
         cmd_cls = get_pipelime_command_cls(command)
     except ValueError:
         raise typer.Exit(1)
 
     if verbose > 2:
@@ -694,14 +717,18 @@
         cmd_obj()
     end_time = time.perf_counter_ns()
     print_info("\nCommand executed in " + time_to_str(end_time - start_time))
 
     print_info(f"\n`{command}` outputs:")
     print_command_outputs(cmd_obj)
 
+    if not keep_tmp and PipelimeTmp.SESSION_TMP_DIR:
+        print_info("\nCleaning temporary files...")
+        TempCommand(name=PipelimeTmp.SESSION_TMP_DIR.stem, force=True)()  # type: ignore
+
 
 def _create_typer_app(
     *,
     app_name: str = "Pipelime",
     entry_point: t.Optional[str] = None,
     app_description: t.Optional[str] = None,
     version: t.Optional[str] = None,
```

### Comparing `pipelime_python-1.4.1/pipelime/cli/parser.py` & `pipelime_python-1.5.0/pipelime/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/cli/pretty_print.py` & `pipelime_python-1.5.0/pipelime/cli/pretty_print.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         *([Column(overflow="fold") for _ in range(2 + int(show_class_path))]),
         padding=(0, 1),
     )
     for m in model_cls:
         col_vals = [escape(get_model_title(m))]
         if show_class_path:
             col_vals.append(f"[italic grey50]{escape(get_model_classpath(m))}[/]")
-        col_vals.append(escape(inspect.getdoc(m) or ""))
+        col_vals.append(escape((inspect.getdoc(m) or "").partition("\n")[0]))
         grid.add_row(*col_vals)
     rprint(grid)
 
 
 def print_model_info(
     model_cls: t.Type[BaseModel],
     *,
@@ -222,14 +222,16 @@
     field,
     indent: int,
     indent_offs: int,
     show_piper_port: bool,
     show_description: bool,
     recursive: bool,
 ):
+    from enum import Enum
+
     is_model = _is_model(field.outer_type_) and not inspect.isabstract(
         field.outer_type_
     )
 
     if show_description:
         # NB: docs should not come from the inner __root__ type
         if field.field_info.description:
@@ -287,15 +289,18 @@
     )
 
     # Piper port
     if show_piper_port:
         line.append(fport)  # type: ignore
 
     # Default value
-    line.append("[red]✗[/]" if field.required else f"[green]{field.get_default()}[/]")
+    field_default = field.get_default()
+    if isinstance(field_default, Enum):
+        field_default = field_default.value
+    line.append("[red]✗[/]" if field.required else f"[green]{field_default}[/]")
 
     grid.add_row(*line)
 
     if recursive:
         if is_model and not has_root_item:
             _iterate_model_fields(
                 model_cls=field_outer_type,
```

### Comparing `pipelime_python-1.4.1/pipelime/cli/subcommands.py` & `pipelime_python-1.5.0/pipelime/cli/subcommands.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/cli/utils.py` & `pipelime_python-1.5.0/pipelime/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/cli/wizard.py` & `pipelime_python-1.5.0/pipelime/cli/wizard.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/commands/__init__.py` & `pipelime_python-1.5.0/pipelime/commands/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,16 +7,18 @@
     AddRemoteCommand,
     RemoveRemoteCommand,
     ValidateCommand,
     MapCommand,
     SortCommand,
     FilterCommand,
     SliceCommand,
+    SetMetadataCommand,
 )
 from pipelime.commands.shell import ShellCommand
 from pipelime.commands.split_ops import (
     SplitByQueryCommand,
     SplitByValueCommand,
     SplitCommand,
 )
 from pipelime.commands.toy_dataset import ToyDatasetCommand
 from pipelime.commands.piper import RunCommand, DrawCommand, WatchCommand
+from pipelime.commands.tempman import TempCommand
```

### Comparing `pipelime_python-1.4.1/pipelime/commands/general.py` & `pipelime_python-1.5.0/pipelime/commands/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,16 +188,19 @@
             keep_order=False,
             parent_cmd=self,
             track_message=f"Writing results ({len(seq)} samples)",
         )
 
 
 class CloneCommand(PipelimeCommand, title="clone"):
-    """Clone a dataset. You can use this command to create a local copy of a dataset
-    hosted on a remote data lake by disabling the `REMOTE_FILE` serialization option."""
+    """Clone a dataset.
+
+    You can use this command to create a local copy of a dataset
+    hosted on a remote data lake by disabling the `REMOTE_FILE` serialization option.
+    """
 
     input: pl_interfaces.InputDatasetInterface = (
         pl_interfaces.InputDatasetInterface.pyd_field(
             alias="i", piper_port=PiperPortType.INPUT
         )
     )
 
@@ -386,14 +389,15 @@
             parent_cmd=self,
             track_message=message,
         )
 
 
 class AddRemoteCommand(RemoteCommandBase, title="remote-add"):
     """Upload samples to one or more remotes.
+
     Slicing and key options filter the samples to upload,
     but the whole dataset is always written out.
     """
 
     def run(self):
         from pipelime.stages import StageUploadToRemote
 
@@ -404,16 +408,18 @@
             ),
             "Uploading data",
         )
 
 
 class RemoveRemoteCommand(RemoteCommandBase, title="remote-remove"):
     """Remove one or more remote from a dataset.
+
     Slicing and key options filter the samples,
     but the whole dataset is always written out.
+
     NB: data is not removed from the remote data lake.
     """
 
     def run(self):
         from pipelime.stages import StageForgetSource
 
         remotes = [r.get_url() for r in self.remotes]  # type: ignore
@@ -706,27 +712,31 @@
         )
     )
 
     grabber: pl_interfaces.GrabberInterface = pl_interfaces.GrabberInterface.pyd_field(
         alias="g"
     )
 
+    @pyd.validator("filter_fn", always=True)
+    def _check_filters(
+        cls, v: t.Optional[pl_types.CallableDef], values: t.Mapping[str, t.Any]
+    ) -> t.Optional[pl_types.CallableDef]:
+        fquery = values.get("filter_query", None)
+        if (v is None) == (fquery is None):
+            raise ValueError("You should define either `filter_query` or `filter_fn`")
+        return v
+
     def _filter_key_fn(self, x):
         return x.match(self.filter_query)
 
     def run(self):
         from pipelime.sequences import DataStream
 
-        if (self.filter_query is None) == (self.filter_fn is None):
-            raise ValueError("You should define either `filter_query` or `filter_fn`")
-
         filter_fn = (
-            self._filter_key_fn
-            if self.filter_query is not None
-            else self.filter_fn.value  # type: ignore
+            self._filter_key_fn if self.filter_fn is None else self.filter_fn.value
         )
 
         # multi-processing friendly filtering
         class _WriterHelper:
             def __init__(self, output_pipe):
                 self.stream = DataStream(output_pipe=output_pipe)
                 self.curr_idx = 0
@@ -796,7 +806,57 @@
         self.grabber.grab_all(
             seq,
             grab_context_manager=self.output.serialization_cm(),
             keep_order=False,
             parent_cmd=self,
             track_message=f"Slicing dataset ({len(seq)} samples)",
         )
+
+
+class SetMetadataCommand(FilterCommand, title="set-meta"):
+    """Set a metadata for some or all samples in a dataset.
+
+    The metadata is set only on samples selected by a dictquery or a filter function.
+    """
+
+    filter_fn: t.Optional[pl_types.CallableDef] = pyd.Field(
+        None,
+        alias="f",
+        description=(
+            "A `class.path.to.func` (or `file.py:func`) to "
+            "a callable returning True for any valid sample.\n"
+            "Accepted signatures:\n"
+            "  `() -> bool`\n"
+            "  `(index: int) -> bool`\n"
+            "  `(index: int, sample: Sample) -> bool`\n"
+            "  `(index: int, sample: Sample, source: SamplesSequence) -> bool`."
+        ),
+    )
+
+    key_path: str = pyd.Field(
+        ..., alias="k", description="The metadata key in pydash dot notation."
+    )
+    value: pl_types.YamlInput = pyd.Field(
+        None, alias="v", description="The value to set, ie, any valid yaml/json value."
+    )
+
+    def _filter_key_fn(self, idx, x):
+        return x.match(self.filter_query)
+
+    def run(self) -> None:
+        from pipelime.stages import StageSetMetadata
+
+        seq = self.input.create_reader()
+        seq = seq.map_if(
+            stage=StageSetMetadata(key_path=self.key_path, value=self.value),
+            condition=(
+                self._filter_key_fn if self.filter_fn is None else self.filter_fn.value
+            ),
+        )
+        seq = self.output.append_writer(seq)
+        self.grabber.grab_all(
+            seq,
+            grab_context_manager=self.output.serialization_cm(),
+            keep_order=False,
+            parent_cmd=self,
+            track_message=f"Setting metadata ({len(seq)} samples)",
+        )
```

### Comparing `pipelime_python-1.4.1/pipelime/commands/interfaces.py` & `pipelime_python-1.5.0/pipelime/commands/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,22 +312,26 @@
                 )
             value = data
 
         if isinstance(value, t.Mapping):
             return InputDatasetInterface(**value)
         raise ValueError("Invalid input dataset definition.")
 
+    @staticmethod
+    def is_empty_fn(x):
+        return not all(i.is_shared for i in x.values())
+
     def create_reader(self):
         from pipelime.sequences import SamplesSequence
 
         reader = SamplesSequence.from_underfolder(
             folder=self.folder, merge_root_items=self.merge_root_items, must_exist=True
         )
         if self.skip_empty:
-            reader = reader.filter(lambda x: not all(i.is_shared for i in x.values()))
+            reader = reader.filter(InputDatasetInterface.is_empty_fn)
         if self.schema_ is not None:
             reader = self.schema_.append_validator(reader)
         return reader
 
     def __repr__(self) -> str:
         return self.__piper_repr__()
 
@@ -705,19 +709,24 @@
     """
 
     _default_type_description: t.ClassVar[t.Optional[str]] = "An interval of indexes."
     _compact_form: t.ClassVar[t.Optional[str]] = "<start>[:<stop>]"
 
     start: t.Optional[int] = pyd.Field(
         None,
-        description="The first index (included), defaults to the first element (can be negative).",
+        description=(
+            "The first index (included), defaults to the first element "
+            "(can be negative)."
+        ),
     )
     stop: t.Optional[int] = pyd.Field(
         None,
-        description="The last index (excluded), defaults to the last element (can be negative).",
+        description=(
+            "The last index (excluded), defaults to the last element (can be negative)."
+        ),
     )
 
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
```

### Comparing `pipelime_python-1.4.1/pipelime/commands/piper.py` & `pipelime_python-1.5.0/pipelime/commands/piper.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,16 @@
 
                 graph_image = drawer.draw(graph=graph, **extra)
                 img = Image.fromarray(graph_image, "RGB")
                 img.show("Graph")
 
 
 class WatchCommand(PipelimeCommand, title="watch"):
+    """Show the progress of a running DAG."""
+
     token: t.Optional[str] = Field(
         None,
         alias="t",
         description=(
             "The token of the DAG you want to monitor. "
             "Defaults to any DAG if not specified."
         ),
```

### Comparing `pipelime_python-1.4.1/pipelime/commands/shell.py` & `pipelime_python-1.5.0/pipelime/commands/shell.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,16 +40,17 @@
 
     def get_inputs(self) -> Dict[str, Any]:
         return self.inputs
 
     def get_outputs(self) -> Dict[str, Any]:
         return self.outputs
 
+    @PipelimeCommand.command_name.getter
     def command_name(self) -> str:
-        return self.command
+        return self.command_title() + ":" + self.command.partition(" ")[0]
 
     def _to_command_chunk(self, key: str, value: Any) -> str:
         cmd = ""
         if isinstance(value, Sequence):
             cmd += f" --{key} {value[0]} {self._to_command_chunk(key, value[1:])}"
         elif isinstance(value, Mapping):
             raise NotImplementedError("Mapping values are not supported")
@@ -66,8 +67,10 @@
         args = {**self.inputs, **self.outputs}
         cmd = cmd.format(**args)
 
         for key in set(args.keys()).difference(fields):
             value = args[key]
             cmd += self._to_command_chunk(key, value)
 
-        subprocess.run(cmd, shell=True)
+        with self.create_task(1, "Executing") as t:
+            subprocess.run(cmd, shell=True)
+            t.advance()
```

### Comparing `pipelime_python-1.4.1/pipelime/commands/split_ops.py` & `pipelime_python-1.5.0/pipelime/commands/split_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,16 +300,15 @@
             keep_order=False,
             parent_cmd=self,
             track_message=f"Writing {message} ({len(seq)} samples)",
         )
 
 
 class SplitByValueCommand(PipelimeCommand, title="split-value"):
-    """Split a dataset into multiple sequences,
-    one for each unique value of a given key."""
+    """Creates a new sequence for each unique value of a given key."""
 
     input: pl_interfaces.InputDatasetInterface = (
         pl_interfaces.InputDatasetInterface.pyd_field(
             alias="i", piper_port=PiperPortType.INPUT
         )
     )
 
@@ -358,23 +357,22 @@
                             if np.issubdtype(value.dtype, np.integer)
                             else float(value)
                         )
                     else:
                         value = tuple(value)
                 return (
                     str(value)
-                    .replace(", ", "„")
-                    .replace(",", "„")
-                    .replace(" ", "_")
-                    .replace("/", "-")
-                    .replace("\\", "-")
+                    .replace(",", "‚")
+                    .replace(" ", "·")
+                    .replace("/", "∕")
+                    .replace("\\", "∖")
                     .replace("<", "‹")
                     .replace(">", "›")
                     .replace(":", "⁚")
-                    .replace('"', "'")
+                    .replace('"', "″")
                     .replace("|", "¦")
                     .replace("?", "⁇")
                     .replace("*", "⁎")
                 )
 
             def __call__(self, x: Sample):
                 value = x.deep_get(self._value_key)
```

### Comparing `pipelime_python-1.4.1/pipelime/commands/toy_dataset.py` & `pipelime_python-1.5.0/pipelime/commands/toy_dataset.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/items/__init__.py` & `pipelime_python-1.5.0/pipelime/items/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/items/base.py` & `pipelime_python-1.5.0/pipelime/items/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,14 +376,15 @@
 
         class MyItem(Item, default_concrete=MyItemConcrete):
             pass
 
         class MyOtherItem(Item):
             @deferred_classattr
             def default_concrete(cls):
+                return MyOtherItemConcrete
     """
 
     _data_cache: t.Optional[T]
     _file_sources: t.List[Path]
     _remote_sources: t.List[ParseResult]
     _cache_data: t.Optional[bool]
     _shared: bool
```

### Comparing `pipelime_python-1.4.1/pipelime/items/binary_item.py` & `pipelime_python-1.5.0/pipelime/items/binary_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/items/image_item.py` & `pipelime_python-1.5.0/pipelime/items/image_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/items/metadata_item.py` & `pipelime_python-1.5.0/pipelime/items/metadata_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/items/model3d_item.py` & `pipelime_python-1.5.0/pipelime/items/model3d_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/items/numpy_item.py` & `pipelime_python-1.5.0/pipelime/items/numpy_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/graph.py` & `pipelime_python-1.5.0/pipelime/piper/graph.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/model.py` & `pipelime_python-1.5.0/pipelime/piper/model.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/drawing/base.py` & `pipelime_python-1.5.0/pipelime/piper/drawing/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/drawing/factory.py` & `pipelime_python-1.5.0/pipelime/piper/drawing/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/drawing/graphviz.py` & `pipelime_python-1.5.0/pipelime/piper/drawing/graphviz.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/drawing/mermaid.py` & `pipelime_python-1.5.0/pipelime/piper/drawing/mermaid.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/executors/base.py` & `pipelime_python-1.5.0/pipelime/piper/executors/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/executors/factory.py` & `pipelime_python-1.5.0/pipelime/piper/executors/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/executors/naive.py` & `pipelime_python-1.5.0/pipelime/piper/executors/naive.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/parsers/base.py` & `pipelime_python-1.5.0/pipelime/piper/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/parsers/choixe_parser.py` & `pipelime_python-1.5.0/pipelime/piper/parsers/choixe_parser.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/parsers/factory.py` & `pipelime_python-1.5.0/pipelime/piper/parsers/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/model.py` & `pipelime_python-1.5.0/pipelime/piper/progress/model.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/estimator/base.py` & `pipelime_python-1.5.0/pipelime/piper/progress/estimator/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/estimator/naive.py` & `pipelime_python-1.5.0/pipelime/piper/progress/estimator/naive.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/listener/base.py` & `pipelime_python-1.5.0/pipelime/piper/progress/listener/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/listener/factory.py` & `pipelime_python-1.5.0/pipelime/piper/progress/listener/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/listener/callbacks/file.py` & `pipelime_python-1.5.0/pipelime/piper/progress/listener/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/listener/callbacks/rich_table.py` & `pipelime_python-1.5.0/pipelime/piper/progress/listener/callbacks/rich_table.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/listener/callbacks/tqdm_bars.py` & `pipelime_python-1.5.0/pipelime/piper/progress/listener/callbacks/tqdm_bars.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/listener/receiver/zmq.py` & `pipelime_python-1.5.0/pipelime/piper/progress/listener/receiver/zmq.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/tracker/base.py` & `pipelime_python-1.5.0/pipelime/piper/progress/tracker/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/tracker/direct.py` & `pipelime_python-1.5.0/pipelime/piper/progress/tracker/direct.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/tracker/factory.py` & `pipelime_python-1.5.0/pipelime/piper/progress/tracker/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/tracker/loguru.py` & `pipelime_python-1.5.0/pipelime/piper/progress/tracker/loguru.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/piper/progress/tracker/zmq.py` & `pipelime_python-1.5.0/pipelime/piper/progress/tracker/zmq.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/remotes/base.py` & `pipelime_python-1.5.0/pipelime/remotes/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/remotes/s3_remote.py` & `pipelime_python-1.5.0/pipelime/remotes/s3_remote.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/remotes/shared_folder_remote.py` & `pipelime_python-1.5.0/pipelime/remotes/shared_folder_remote.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/direct_access.py` & `pipelime_python-1.5.0/pipelime/sequences/direct_access.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/grabber.py` & `pipelime_python-1.5.0/pipelime/sequences/grabber.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
-import multiprocessing
+import billiard.context
+import billiard.pool
 import pydantic as pyd
 import typing as t
 from enum import Enum, auto
 
 import pipelime.sequences as pls
 
 
@@ -72,41 +73,50 @@
         self._sequence = sequence
         self._return_type = return_type
         self._size = size
         self._pool = None
         self._worker_init_fn = (None, ()) if worker_init_fn is None else worker_init_fn
 
     @staticmethod
-    def wrk_init(extra_modules, user_init_fn):
+    def wrk_init(extra_modules, session_temp_dir, user_init_fn):
+        from pipelime.choixe.utils.io import PipelimeTmp
         from pipelime.cli.utils import PipelimeSymbolsHelper
 
+        PipelimeTmp.SESSION_TMP_DIR = session_temp_dir
+
         PipelimeSymbolsHelper.set_extra_modules(extra_modules)
         PipelimeSymbolsHelper.import_everything()
 
         if user_init_fn[0] is not None:
             user_init_fn[0](*user_init_fn[1])
 
     def __enter__(self):
+        from pipelime.choixe.utils.io import PipelimeTmp
         from pipelime.cli.utils import PipelimeSymbolsHelper
 
         if self._grabber.num_workers == 0:
             # SINGLE PROCESS
             self._pool = None
             it = iter(self._sequence)
             if self._worker_init_fn[0] is not None:
                 self._worker_init_fn[0](*self._worker_init_fn[1])
             if self._return_type == ReturnType.SAMPLE_AND_INDEX:
                 return enumerate(it)
             return it
 
         # MULTIPLE PROCESSES
-        self._pool = multiprocessing.Pool(
+        self._pool = billiard.pool.Pool(
             self._grabber.num_workers if self._grabber.num_workers > 0 else None,
             initializer=_GrabContext.wrk_init,
-            initargs=(PipelimeSymbolsHelper.extra_modules, self._worker_init_fn),
+            initargs=(
+                PipelimeSymbolsHelper.extra_modules,
+                PipelimeTmp.SESSION_TMP_DIR,
+                self._worker_init_fn,
+            ),
+            context=billiard.context.SpawnContext(),
         )
         runner = self._pool.__enter__()
 
         worker = _GrabWorker(self._sequence)
         if self._return_type == ReturnType.NO_RETURN:
             fn = worker._worker_fn_no_return
         elif self._return_type == ReturnType.SAMPLE:
@@ -181,13 +191,13 @@
             sequence,
             return_type=return_type,
             size=size,
             worker_init_fn=worker_init_fn,
         )
         if return_type == ReturnType.SAMPLE_AND_INDEX:
             with ctx as gseq:
-                for idx, sample in track_fn(gseq):
+                for idx, sample in track_fn(gseq):  # type: ignore
                     sample_fn(sample, idx)  # type: ignore
         else:
             with ctx as gseq:
-                for sample in track_fn(gseq):
+                for sample in track_fn(gseq):  # type: ignore
                     sample_fn(sample)  # type: ignore
```

### Comparing `pipelime_python-1.4.1/pipelime/sequences/sample.py` & `pipelime_python-1.5.0/pipelime/sequences/sample.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/samples_sequence.py` & `pipelime_python-1.5.0/pipelime/sequences/samples_sequence.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/utils.py` & `pipelime_python-1.5.0/pipelime/sequences/utils.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/pipes/base.py` & `pipelime_python-1.5.0/pipelime/sequences/pipes/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/pipes/mapping.py` & `pipelime_python-1.5.0/pipelime/sequences/pipes/mapping.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/pipes/operations.py` & `pipelime_python-1.5.0/pipelime/sequences/pipes/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 class CachedSequence(PipedSequenceBase, title="cache"):
     """Caches the input Samples the first time they are accessed."""
 
     cache_folder: t.Optional[Path] = pyd.Field(
         None,
         description=(
             "The cache folder path. Leave empty to use a temporary folder "
-            "which will be deleted when exiting the process."
+            "which will be deleted when the object will be garbage collected."
         ),
     )
     reuse_cache: bool = pyd.Field(
         False,
         description=(
             "If `cache_folder` exists, use it anyway if true, "
             "otherwise raise a FileExistsError."
@@ -328,17 +328,17 @@
     )
 
     _temp_folder = pyd.PrivateAttr(None)
 
     def __init__(self, cache_folder: t.Optional[Path] = None, **data):
         super().__init__(cache_folder=cache_folder, **data)  # type: ignore
         if self.cache_folder is None:
-            from tempfile import TemporaryDirectory
+            from pipelime.choixe.utils.io import PipelimeTemporaryDirectory as PlTmpDir
 
-            self._temp_folder = TemporaryDirectory()
+            self._temp_folder = PlTmpDir()
             self.cache_folder = Path(self._temp_folder.name)
         else:
             if not self.reuse_cache and self.cache_folder.exists():
                 raise FileExistsError(
                     f"The cache folder `{self.cache_folder}` already exists."
                 )
             self.cache_folder.mkdir(parents=True, exist_ok=True)
```

### Comparing `pipelime_python-1.4.1/pipelime/sequences/pipes/validation.py` & `pipelime_python-1.5.0/pipelime/sequences/pipes/validation.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/pipes/writers.py` & `pipelime_python-1.5.0/pipelime/sequences/pipes/writers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing as t
 from pathlib import Path
 import re
 
 import pydantic as pyd
 from filelock import FileLock, Timeout
-from tempfile import TemporaryDirectory
 
 import pipelime.sequences as pls
 from pipelime.items import Item, SerializationMode
 from pipelime.sequences.pipes import PipedSequenceBase
 
 
 class _serialization_mode_override:
@@ -43,37 +42,41 @@
     ] = pyd.Field(None, description="Forced serialization mode for each key.")
     exists_ok: bool = pyd.Field(
         False, description="If False raises an error when `folder` exists."
     )
 
     _data_folder: Path
     _effective_zfill: int
-    _temp_folder: TemporaryDirectory
+    _temp_folder: t.Any
 
     @pyd.validator("exists_ok", always=True)
     def _check_folder_exists(cls, v: bool, values: t.Mapping[str, t.Any]) -> bool:
         if not v and "folder" in values and values["folder"].exists():
             raise ValueError(
                 f"Trying to overwrite an existing dataset: `{values['folder']}`. "
                 "Please use `exists_ok=True` to overwrite."
             )
         return v
 
     def __init__(self, folder: Path, **data):
+        from pipelime.choixe.utils.io import PipelimeTemporaryDirectory
+
         super().__init__(folder=folder, **data)  # type: ignore
 
         self._data_folder = self.folder / "data"
         self._effective_zfill = (
             self.source.best_zfill() if self.zfill is None else self.zfill
         )
         if self.key_serialization_mode is None:
             self.key_serialization_mode = {}
 
         self._data_folder.mkdir(parents=True, exist_ok=True)
-        self._temp_folder = TemporaryDirectory()  # will be automatically deleted
+
+        # will be automatically deleted
+        self._temp_folder = PipelimeTemporaryDirectory()
 
     def get_sample(self, idx: int) -> pls.Sample:
         sample = self.source[idx]
 
         id_str_nofill = str(idx)
         id_str = id_str_nofill.zfill(self._effective_zfill)
```

### Comparing `pipelime_python-1.4.1/pipelime/sequences/sources/from_callable.py` & `pipelime_python-1.5.0/pipelime/sequences/sources/from_callable.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/sources/raw.py` & `pipelime_python-1.5.0/pipelime/sequences/sources/raw.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/sources/readers.py` & `pipelime_python-1.5.0/pipelime/sequences/sources/readers.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/sequences/sources/toy_dataset.py` & `pipelime_python-1.5.0/pipelime/sequences/sources/toy_dataset.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/stages/__init__.py` & `pipelime_python-1.5.0/pipelime/stages/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-from pipelime.stages.base import SampleStage, StageCompose, StageIdentity, StageLambda, StageInput
+from pipelime.stages.base import (
+    SampleStage,
+    StageCompose,
+    StageIdentity,
+    StageLambda,
+    StageInput,
+)
 from pipelime.stages.augmentations import StageAlbumentations
-from pipelime.stages.item_replacement import StageReplaceItem
+from pipelime.stages.item_replacement import StageReplaceItem, StageSetMetadata
 from pipelime.stages.item_sources import StageForgetSource, StageUploadToRemote
 from pipelime.stages.key_transformations import (
     StageDuplicateKey,
     StageKeyFormat,
     StageKeysFilter,
     StageRemap,
 )
```

### Comparing `pipelime_python-1.4.1/pipelime/stages/augmentations.py` & `pipelime_python-1.5.0/pipelime/stages/augmentations.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/stages/base.py` & `pipelime_python-1.5.0/pipelime/stages/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/stages/entities.py` & `pipelime_python-1.5.0/pipelime/stages/entities.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/stages/item_info.py` & `pipelime_python-1.5.0/pipelime/stages/item_info.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/stages/item_sources.py` & `pipelime_python-1.5.0/pipelime/stages/item_sources.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/stages/key_transformations.py` & `pipelime_python-1.5.0/pipelime/stages/key_transformations.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/utils/context_managers.py` & `pipelime_python-1.5.0/pipelime/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/utils/inspection.py` & `pipelime_python-1.5.0/pipelime/utils/inspection.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pipelime/utils/pydantic_types.py` & `pipelime_python-1.5.0/pipelime/utils/pydantic_types.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/.gitignore` & `pipelime_python-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/LICENSE` & `pipelime_python-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/README.md` & `pipelime_python-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.4.1/pyproject.toml` & `pipelime_python-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     "pydash",
     "pydantic>=1.10",
     "schema",
     "pyzmq",
     "dictquery",
     "minio",
     "requests",
+    "billiard",
 ]
 dynamic = [ "version" ]
 
 [project.optional-dependencies]
 draw = ["pygraphviz"]
 tests = [
     "pytest",
```

### Comparing `pipelime_python-1.4.1/PKG-INFO` & `pipelime_python-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelime-python
-Version: 1.4.1
+Version: 1.5.0
 Summary: Data workflows, cli and dataflow automation.
 Project-URL: Source, https://github.com/eyecan-ai/pipelime-python
 Project-URL: Issues, https://github.com/eyecan-ai/pipelime-python/issues
 Project-URL: Documentation, http://pipelime-python.readthedocs.io/
 Author-email: "Eyecan.ai" <info@eyecan.ai>
 License: GNU General Public License v3 (GPLv3)
 License-File: LICENSE
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Requires-Dist: albumentations>=1.0.0
 Requires-Dist: astunparse
+Requires-Dist: billiard
 Requires-Dist: deepdiff
 Requires-Dist: dictquery
 Requires-Dist: filelock
 Requires-Dist: imageio>=2.17.0
 Requires-Dist: loguru
 Requires-Dist: minio
 Requires-Dist: numpy
```

