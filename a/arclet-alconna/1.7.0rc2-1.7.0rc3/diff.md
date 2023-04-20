# Comparing `tmp/arclet-alconna-1.7.0rc2.tar.gz` & `tmp/arclet-alconna-1.7.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.0rc2.tar", last modified: Thu Apr 13 10:49:38 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.0rc3.tar", last modified: Thu Apr 20 13:16:09 2023, max compression
```

## Comparing `arclet-alconna-1.7.0rc2.tar` & `arclet-alconna-1.7.0rc3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc2/LICENSE
--rw-r--r--   0        0        0     2934 2023-04-12 14:50:52.114697 arclet-alconna-1.7.0rc2/pyproject.toml
--rw-r--r--   0        0        0     5110 2023-04-13 04:57:01.774375 arclet-alconna-1.7.0rc2/README-EN.md
--rw-r--r--   0        0        0      986 2023-04-13 03:53:01.217815 arclet-alconna-1.7.0rc2/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0     3419 2023-04-09 14:04:25.832070 arclet-alconna-1.7.0rc2/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    15690 2023-04-13 03:53:01.241816 arclet-alconna-1.7.0rc2/src/arclet/alconna/analyser.py
--rw-r--r--   0        0        0    11073 2023-04-13 03:53:01.202851 arclet-alconna-1.7.0rc2/src/arclet/alconna/args.py
--rw-r--r--   0        0        0    12635 2023-04-13 03:53:01.266816 arclet-alconna-1.7.0rc2/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0     6728 2023-04-13 03:53:01.232845 arclet-alconna-1.7.0rc2/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     4383 2023-02-22 15:46:15.071359 arclet-alconna-1.7.0rc2/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     3506 2023-04-13 03:56:31.540007 arclet-alconna-1.7.0rc2/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     3086 2023-04-13 04:07:03.467875 arclet-alconna-1.7.0rc2/src/arclet/alconna/config.py
--rw-r--r--   0        0        0     6293 2023-04-13 03:56:31.510993 arclet-alconna-1.7.0rc2/src/arclet/alconna/container.py
--rw-r--r--   0        0        0    13398 2023-04-13 03:56:31.527968 arclet-alconna-1.7.0rc2/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     9715 2023-04-01 15:40:45.569486 arclet-alconna-1.7.0rc2/src/arclet/alconna/default.lang
--rw-r--r--   0        0        0     2498 2023-03-31 19:18:40.743939 arclet-alconna-1.7.0rc2/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-03-31 14:01:42.790537 arclet-alconna-1.7.0rc2/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0      823 2023-04-08 10:00:51.776731 arclet-alconna-1.7.0rc2/src/arclet/alconna/executor.py
--rw-r--r--   0        0        0     9771 2023-04-13 03:35:02.154387 arclet-alconna-1.7.0rc2/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0    19282 2023-04-13 03:59:55.614916 arclet-alconna-1.7.0rc2/src/arclet/alconna/handlers.py
--rw-r--r--   0        0        0     5828 2023-04-12 12:26:51.391339 arclet-alconna-1.7.0rc2/src/arclet/alconna/header.py
--rw-r--r--   0        0        0     2487 2023-04-13 10:49:13.979099 arclet-alconna-1.7.0rc2/src/arclet/alconna/lang.py
--rw-r--r--   0        0        0    13354 2023-04-13 03:59:55.575869 arclet-alconna-1.7.0rc2/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1505 2023-04-13 03:35:02.200010 arclet-alconna-1.7.0rc2/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1144 2023-04-12 12:33:00.784350 arclet-alconna-1.7.0rc2/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     2942 2023-02-22 15:46:15.130357 arclet-alconna-1.7.0rc2/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-04-08 09:18:05.731268 arclet-alconna-1.7.0rc2/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     4805 2023-02-22 15:46:15.253359 arclet-alconna-1.7.0rc2/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     2397 2023-03-31 14:01:42.844114 arclet-alconna-1.7.0rc2/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0      895 2023-04-11 10:30:01.832860 arclet-alconna-1.7.0rc2/src/arclet/alconna/util.py
--rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc3/LICENSE
+-rw-r--r--   0        0        0     2934 2023-04-17 06:25:04.271711 arclet-alconna-1.7.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     5108 2023-04-17 05:33:14.505606 arclet-alconna-1.7.0rc3/README-EN.md
+-rw-r--r--   0        0        0      928 2023-04-20 13:14:50.371493 arclet-alconna-1.7.0rc3/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0     3419 2023-04-09 14:04:25.832070 arclet-alconna-1.7.0rc3/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    13932 2023-04-20 13:00:01.793211 arclet-alconna-1.7.0rc3/src/arclet/alconna/analyser.py
+-rw-r--r--   0        0        0    11060 2023-04-20 09:42:19.098735 arclet-alconna-1.7.0rc3/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     6768 2023-04-20 12:31:38.881196 arclet-alconna-1.7.0rc3/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    12639 2023-04-17 05:44:49.700466 arclet-alconna-1.7.0rc3/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0     6734 2023-04-17 05:44:49.658976 arclet-alconna-1.7.0rc3/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     4384 2023-04-17 05:41:18.628904 arclet-alconna-1.7.0rc3/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     3515 2023-04-20 12:31:38.882195 arclet-alconna-1.7.0rc3/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     3348 2023-04-20 13:07:02.615788 arclet-alconna-1.7.0rc3/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    13657 2023-04-20 12:48:50.977968 arclet-alconna-1.7.0rc3/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2498 2023-03-31 19:18:40.743939 arclet-alconna-1.7.0rc3/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-03-31 14:01:42.790537 arclet-alconna-1.7.0rc3/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0      823 2023-04-08 10:00:51.776731 arclet-alconna-1.7.0rc3/src/arclet/alconna/executor.py
+-rw-r--r--   0        0        0     9772 2023-04-20 12:48:50.996903 arclet-alconna-1.7.0rc3/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0    18374 2023-04-20 13:00:17.125966 arclet-alconna-1.7.0rc3/src/arclet/alconna/handlers.py
+-rw-r--r--   0        0        0     6033 2023-04-20 12:53:16.998627 arclet-alconna-1.7.0rc3/src/arclet/alconna/header.py
+-rw-r--r--   0        0        0       65 2023-04-17 05:01:09.559175 arclet-alconna-1.7.0rc3/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3217 2023-04-17 05:01:09.583116 arclet-alconna-1.7.0rc3/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3200 2023-04-17 05:01:09.575993 arclet-alconna-1.7.0rc3/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    14589 2023-04-20 12:31:38.884196 arclet-alconna-1.7.0rc3/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1505 2023-04-13 03:35:02.200010 arclet-alconna-1.7.0rc3/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1144 2023-04-12 12:33:00.784350 arclet-alconna-1.7.0rc3/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     2942 2023-02-22 15:46:15.130357 arclet-alconna-1.7.0rc3/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:18:05.731268 arclet-alconna-1.7.0rc3/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     4805 2023-02-22 15:46:15.253359 arclet-alconna-1.7.0rc3/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     2401 2023-04-20 12:43:09.501490 arclet-alconna-1.7.0rc3/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0      895 2023-04-11 10:30:01.832860 arclet-alconna-1.7.0rc3/src/arclet/alconna/util.py
+-rw-r--r--   0        0        0     5909 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc3/PKG-INFO
```

### Comparing `arclet-alconna-1.7.0rc2/LICENSE` & `arclet-alconna-1.7.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/pyproject.toml` & `arclet-alconna-1.7.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 name = "arclet-alconna"
 description = "A High-performance, Generality, Humane Command Line Arguments Parser Library."
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
-    "nepattern<0.6.0, >=0.5.2",
-    "tarina>=0.2.3",
+    "nepattern<0.6.0, >=0.5.3",
+    "tarina>=0.3.0",
 ]
 dynamic = []
 requires-python = ">=3.8"
 readme = "README-EN.md"
 keywords = [
     "command",
     "argparse",
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.0rc2"
+version = "1.7.0rc3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.0rc2/README-EN.md` & `arclet-alconna-1.7.0rc3/README-EN.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 ```
 
 Output as follows:
 ```
 value=None args={'pak_name': 'numpy'} options={'upgrade': value=Ellipsis args={}} subcommands={}
 ```
 
-
 ## Communication
 
 QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 ## Features
 
 * High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Alconna 概览"""
 
 from nepattern import AllParam as AllParam, AnyOne as AnyOne  # noqa
 from tarina import Empty as Empty # noqa
+from .config import config, namespace, Namespace
 from .typing import MultiVar, KeyWordVar, Kw, Nargs
 from .args import Args, Field, ArgFlag, Arg
 from .base import CommandNode, Option, Subcommand
 from .completion import CompInterface
 from .exceptions import ParamsUnmatched, NullMessage, InvalidParam
 from .analyser import Analyser
-from .container import DataCollectionContainer
+from .argv import Argv
 from .core import Alconna, CommandMeta
 from .arparma import Arparma, ArparmaBehavior
 from .manager import command_manager, ShortcutArgs
-from .config import config, namespace, Namespace
-from .lang import load_lang_file
 
 from .builtin import store_value, set_default, store_true, store_false
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.0rc2"
+__version__ = "1.7.0rc3"
 
 Arpamar = Arparma
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/action.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/analyser.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/analyser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,114 @@
 from __future__ import annotations
 
 import re
 import traceback
 from re import Match
 from typing import TYPE_CHECKING, Any, Generic, Callable
-from dataclasses import dataclass, field, InitVar
-from typing_extensions import Self, TypeVar
+from dataclasses import dataclass, field
+from typing_extensions import Self, TypeAlias
+from tarina.lang import lang
 
 from .manager import command_manager, ShortcutArgs
 from .exceptions import (
     ParamsUnmatched,
     ArgumentMissing,
     FuzzyMatchSuccess,
     PauseTriggered,
-    SpecialOptionTriggered,
-    NullMessage
+    SpecialOptionTriggered
 )
 from .args import Args
 from .header import Header
 from .base import Option, Subcommand
 from .completion import comp_ctx
 from .model import Sentence, HeadResult, OptionResult, SubcommandResult
 from .arparma import Arparma
 from .typing import TDataCollection
 from .config import Namespace
-from .lang import lang
 from .output import output_manager
-from .handlers import analyse_args, analyse_param, analyse_header, handle_help, handle_shortcut, handle_completion, prompt
-from .container import DataCollectionContainer, TContainer
+from .handlers import (
+    analyse_args, analyse_param, analyse_header, handle_help, handle_shortcut, handle_completion, prompt
+)
+from .argv import Argv
 
 if TYPE_CHECKING:
     from .core import Alconna
 
+_SPECIAL = {
+    "help": handle_help,
+    "shortcut": handle_shortcut,
+    "completion": handle_completion
+}
+
 
 def _compile_opts(option: Option, data: dict[str, Sentence | list[Option] | SubAnalyser]):
     for alias in option.aliases:
         if (li := data.get(alias)) and isinstance(li, list):
             li.append(option)  # type: ignore
             li.sort(key=lambda x: x.priority, reverse=True)
         else:
             data[alias] = [option]
 
 
-def default_compiler(analyser: SubAnalyser, _config: Namespace):
+def default_compiler(analyser: SubAnalyser, _config: Namespace, pids: set[str]):
     require_len = 0
     for opts in analyser.command.options:
         if isinstance(opts, Option):
             _compile_opts(opts, analyser.compile_params)  # type: ignore
-            analyser.container.param_ids.update(opts.aliases)
+            pids.update(opts.aliases)
         elif isinstance(opts, Subcommand):
-            sub = SubAnalyser(opts, analyser.container, _config, analyser.fuzzy_match)
+            sub = SubAnalyser(opts)
             analyser.compile_params[opts.name] = sub
-            analyser.container.param_ids.add(opts.name)
-            default_compiler(sub, _config)
-        if not set(analyser.container.separators).issuperset(opts.separators):
-            analyser.container.default_separate &= False
+            pids.add(opts.name)
+            default_compiler(sub, _config, pids)
+        if not set(analyser.command.separators).issuperset(opts.separators):
+            analyser.default_separate &= False
         if opts.requires:
-            analyser.container.param_ids.update(opts.requires)
+            pids.update(opts.requires)
             require_len = max(len(opts.requires), require_len)
             for k in opts.requires:
                 analyser.compile_params.setdefault(k, Sentence(name=k))
     analyser.part_len = range(
         len(analyser.command.options) + analyser.need_main_args + require_len
     )
 
 
 @dataclass
-class SubAnalyser(Generic[TContainer]):
+class SubAnalyser(Generic[TDataCollection]):
     command: Subcommand
-    container: TContainer
-    namespace: InitVar[Namespace]
-
-    fuzzy_match: bool = field(default=False)
     default_main_only: bool = field(default=False)  # 默认只有主参数
     part_len: range = field(default=range(0))  # 分段长度
     need_main_args: bool = field(default=False)  # 是否需要主参数
-
-    compile_params: dict[str, Sentence | list[Option] | SubAnalyser[TContainer]] = field(default_factory=dict)
+    default_separate: bool = field(default=True)
+    compile_params: dict[str, Sentence | list[Option] | SubAnalyser[TDataCollection]] = field(default_factory=dict)
 
     self_args: Args = field(init=False)  # 自身参数
     subcommands_result: dict[str, SubcommandResult] = field(init=False)
     options_result: dict[str, OptionResult] = field(init=False)  # 存放解析到的所有选项
     args_result: dict[str, Any] = field(init=False)  # 参数的解析结果
     header_result: HeadResult | None = field(init=False)
     value_result: Any = field(init=False)
     sentences: list[str] = field(init=False)  # 存放解析到的所有句子
 
     def _clr(self):
         self.reset()
-        self.container.reset()
         ks = list(self.__dict__.keys())
         for k in ks:
             delattr(self, k)
 
-    def __post_init__(self, namespace: Namespace):
+    def __post_init__(self):
         self.reset()
-        self.container.reset()
-        self.special = {}
-        self.special.update(
-            [(i, handle_help) for i in namespace.builtin_option_name['help']] +
-            [(i, handle_completion) for i in namespace.builtin_option_name['completion']] +
-            [(i, handle_shortcut) for i in namespace.builtin_option_name['shortcut']]
-        )
-        self.completion_names = namespace.builtin_option_name['completion']
         self.self_args = self.command.args
-        self.__handle_args__()
+        if self.command.nargs > 0 and self.command.nargs > self.self_args.optional_count:
+            self.need_main_args = True  # 如果need_marg那么match的元素里一定得有main_argument
+        _de_count = sum(arg.field.default_gen is not None for arg in self.self_args.argument)
+        if _de_count and _de_count == self.command.nargs:
+            self.default_main_only = True
 
-    def export(self) -> SubcommandResult:
+    def result(self) -> SubcommandResult:
         res = SubcommandResult(
             self.value_result, self.args_result.copy(), self.options_result.copy(), self.subcommands_result.copy()
         )
         self.reset()
         return res
 
     def reset(self):
@@ -118,245 +116,224 @@
         self.args_result = {}
         self.options_result = {}
         self.subcommands_result = {}
         self.sentences = []
         self.value_result = None
         self.header_result = None
 
-    def __handle_args__(self):
-        if self.command.nargs > 0 and self.command.nargs > self.self_args.optional_count:
-            self.need_main_args = True  # 如果need_marg那么match的元素里一定得有main_argument
-        _de_count = sum(arg.field.default_gen is not None for arg in self.self_args.argument)
-        if _de_count and _de_count == self.command.nargs:
-            self.default_main_only = True
-
-    def process(self) -> Self:
-        param = self.container.context = self.command
+    def process(self, argv: Argv[TDataCollection]) -> Self:
+        param = argv.context = self.command
         if param.requires and self.sentences != param.requires:
             raise ParamsUnmatched(f"{param.name}'s required is not '{' '.join(self.sentences)}'")
         self.sentences = []
         if param.is_compact:
-            name, _ = self.container.popitem()
+            name, _ = argv.popitem()
             if not name.startswith(param.name):
                 raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
-            self.container.pushback(name.lstrip(param.name), replace=True)
+            argv.pushback(name.lstrip(param.name), replace=True)
         else:
-            name, _ = self.container.popitem(param.separators)
+            name, _ = argv.popitem(param.separators)
             if name != param.name:  # 先匹配选项名称
                 raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
 
         if self.part_len.stop == 0:
             self.value_result = Ellipsis
             return self
-        return self.analyse()
+        return self.analyse(argv)
 
-    def analyse(self) -> Self:
+    def analyse(self, argv: Argv[TDataCollection]) -> Self:
         for _ in self.part_len:
-            analyse_param(self, *self.container.popitem(self.command.separators, move=False))
+            analyse_param(self, argv, *argv.popitem(self.command.separators, move=False))
         if self.default_main_only and not self.args_result:
-            self.args_result = analyse_args(self, self.self_args)
+            self.args_result = analyse_args(argv, self.self_args)
         if not self.args_result and self.need_main_args:
             raise ArgumentMissing(lang.subcommand.args_missing.format(name=self.command.dest))
         return self
 
-    def get_sub_analyser(self, target: Subcommand) -> SubAnalyser[TContainer] | None:
+    def get_sub_analyser(self, target: Subcommand) -> SubAnalyser[TDataCollection] | None:
         if target == self.command:
             return self
         for param in self.compile_params.values():
             if isinstance(param, SubAnalyser):
                 return param.get_sub_analyser(target)
 
 
-class Analyser(SubAnalyser[TContainer], Generic[TContainer, TDataCollection]):
+class Analyser(SubAnalyser[TDataCollection], Generic[TDataCollection]):
     command: Alconna  # Alconna实例
     used_tokens: set[int]  # 已使用的token
     # 命令头部
     command_header: Header
-    _global_container_type = DataCollectionContainer
 
-    def __init__(self, alconna: Alconna, container_type: type[TContainer] | None = None):
-        _type: type[TContainer] = container_type or self.__class__._global_container_type  # type: ignore
-        super().__init__(
-            alconna,
-            _type(
-                to_text=alconna.namespace_config.to_text,
-                separators=alconna.separators,
-                message_cache=alconna.namespace_config.enable_message_cache,
-                filter_crlf=not alconna.meta.keep_crlf,
-            ),
-            alconna.namespace_config
-        )
+    def __init__(self, alconna: Alconna[TDataCollection], compiler: TCompile | None = None):
+        super().__init__(alconna)
         self.fuzzy_match = alconna.meta.fuzzy_match
         self.used_tokens = set()
-        self.command_header = Header.generate(alconna.command, alconna.headers)
-
-    @classmethod
-    def default_container(cls, __t: type[TContainer] | None = None) -> type[Analyser[TContainer, TDataCollection]]:
-        """配置 Analyser 的默认容器"""
-        if __t is not None:
-            cls._global_container_type = __t
-        return cls
+        self.command_header = Header.generate(alconna.command, alconna.prefixes)
+        compiler = compiler or default_compiler
+        compiler(
+            self,
+            alconna.namespace_config,
+            command_manager.resolve(self.command).param_ids
+        )
 
     def _clr(self):
         self.used_tokens.clear()
         super()._clr()
 
     @staticmethod
     def converter(command: str) -> TDataCollection:
         return command  # type: ignore
 
     def __repr__(self):
         return f"<{self.__class__.__name__} of {self.command.path}>"
 
-    def shortcut(self, data: list[Any], short: Arparma | ShortcutArgs, reg: Match | None) -> Arparma[TDataCollection]:
+    def shortcut(
+        self,
+        argv: Argv[TDataCollection],
+        data: list[Any], short: Arparma | ShortcutArgs,
+        reg: Match | None
+    ) -> Arparma[TDataCollection]:
         if isinstance(short, Arparma):
             return short
-        self.container.build(short.get('command', self.command.command or self.command.name))
+        argv.build(short.get('command', self.command.command or self.command.name))
+        if not short.get('fuzzy') and data:
+            exc = ParamsUnmatched(lang.analyser.param_unmatched.format(target=data[0]))
+            if self.command.meta.raise_exception:
+                raise exc
+            return self.export(argv, True, exc)
         data_index = 0
-        for i, unit in enumerate(self.container.raw_data):
+        for i, unit in enumerate(argv.raw_data):
             if not data:
                 break
             if not isinstance(unit, str):
                 continue
             if unit == f"{{%{data_index}}}":
-                self.container.raw_data[i] = data.pop(0)
+                argv.raw_data[i] = data.pop(0)
                 data_index += 1
             elif f"{{%{data_index}}}" in unit:
-                self.container.raw_data[i] = unit.replace(f"{{%{data_index}}}", str(data.pop(0)))
+                argv.raw_data[i] = unit.replace(f"{{%{data_index}}}", str(data.pop(0)))
                 data_index += 1
             elif mat := re.search(r"\{\*(.*)\}", unit, re.DOTALL):
                 sep = mat[1]
-                self.container.raw_data[i] = unit.replace(f"{{*{sep}}}", (sep or ' ').join(map(str, data)))
+                argv.raw_data[i] = unit.replace(f"{{*{sep}}}", (sep or ' ').join(map(str, data)))
                 data.clear()
 
-        self.container.bak_data = self.container.raw_data.copy()
-        self.container.rebuild(*data).rebuild(*short.get('args', []))
+        argv.bak_data = argv.raw_data.copy()
+        argv.rebuild(*data).rebuild(*short.get('args', []))
         if reg:
             groups: tuple[str, ...] = reg.groups()
             gdict: dict[str, str] = reg.groupdict()
-            for j, unit in enumerate(self.container.raw_data):
+            for j, unit in enumerate(argv.raw_data):
                 if not isinstance(unit, str):
                     continue
                 for i, c in enumerate(groups):
                     unit = unit.replace(f"{{{i}}}", c)
                 for k, v in gdict.items():
                     unit = unit.replace(f"{{{k}}}", v)
-                self.container.raw_data[j] = unit
-        if self.container.message_cache:
-            self.container.temp_token = self.container.generate_token(self.container.raw_data)
-        return self.process()
+                argv.raw_data[j] = unit
+        if argv.message_cache:
+            argv.token = argv.generate_token(argv.raw_data)
+        return self.process(argv)
 
-    def process(self, message: TDataCollection | None = None) -> Arparma[TDataCollection]:
+    def process(self, argv: Argv[TDataCollection]) -> Arparma[TDataCollection]:
         """主体解析函数, 应针对各种情况进行解析"""
-        if self.container.ndata == 0:
-            if not message:
-                raise NullMessage(lang.analyser.handle_null_message.format(target=message))
-            try:
-                self.container.build(message)
-            except Exception as e:
-                return self.export(fail=True, exception=e)
         if (
-            self.container.message_cache and
-            self.container.temp_token in self.used_tokens and
-            (res := command_manager.get_record(self.container.temp_token))
+            argv.message_cache and
+            argv.token in self.used_tokens and
+            (res := command_manager.get_record(argv.token))
         ):
             return res
         try:
-            self.header_result = analyse_header(self)
+            self.header_result = analyse_header(self.command_header, argv)
         except ParamsUnmatched as e:
-            self.container.raw_data = self.container.bak_data.copy()
-            self.container.current_index = 0
+            argv.raw_data = argv.bak_data.copy()
+            argv.current_index = 0
             try:
-                _res = command_manager.find_shortcut(self.command, self.container.popitem(move=False)[0])
+                _res = command_manager.find_shortcut(self.command, argv.popitem(move=False)[0])
             except ValueError as exc:
                 if self.command.meta.raise_exception:
                     raise e from exc
-                return self.export(fail=True, exception=e)
+                return self.export(argv, True, e)
             else:
-                self.container.popitem()
-                data = self.container.release()
+                argv.popitem()
+                data = argv.release()
                 self.reset()
-                self.container.reset()
-                return self.shortcut(data, *_res)
+                argv.reset()
+                return self.shortcut(argv, data, *_res)
 
         except FuzzyMatchSuccess as Fuzzy:
             output_manager.send(self.command.name, lambda: str(Fuzzy))
-            return self.export(fail=True)
+            return self.export(argv, True)
 
-        if fail := self.analyse():
+        if fail := self.analyse(argv):
             return fail
 
-        if self.container.done and (not self.need_main_args or self.args_result):
-            return self.export()
+        if argv.done and (not self.need_main_args or self.args_result):
+            return self.export(argv)
 
-        rest = self.container.release()
+        rest = argv.release()
         if len(rest) > 0:
-            if isinstance(rest[-1], str) and rest[-1] in self.completion_names:
-                last = self.container.bak_data[-1]
-                self.container.bak_data[-1] = last[:last.rfind(rest[-1])]
-                return handle_completion(self, rest[-2])
-            exc = ParamsUnmatched(lang.analyser.param_unmatched.format(target=self.container.popitem(move=False)[0]))
+            if isinstance(rest[-1], str) and rest[-1] in argv.completion_names:
+                last = argv.bak_data[-1]
+                argv.bak_data[-1] = last[:last.rfind(rest[-1])]
+                return handle_completion(self, argv, rest[-2])
+            exc = ParamsUnmatched(lang.analyser.param_unmatched.format(target=argv.popitem(move=False)[0]))
         else:
             exc = ArgumentMissing(lang.analyser.param_missing)
         if isinstance(exc, ArgumentMissing) and comp_ctx.get(None):
-            raise PauseTriggered(prompt(self))
+            raise PauseTriggered(prompt(self, argv))
         if self.command.meta.raise_exception:
             raise exc
-        return self.export(fail=True, exception=exc)
+        return self.export(argv, True, exc)
 
-    def analyse(self) -> Arparma[TDataCollection] | None:
+    def analyse(self, argv: Argv[TDataCollection]) -> Arparma[TDataCollection] | None:
         for _ in self.part_len:
             try:
-                analyse_param(self, *self.container.popitem(move=False))
+                analyse_param(self, argv, *argv.popitem(move=False))
             except FuzzyMatchSuccess as e:
                 output_manager.send(self.command.name, lambda: str(e))
-                return self.export(fail=True)
+                return self.export(argv, True)
             except SpecialOptionTriggered as sot:
-                return sot.args[0](self)
+                return _SPECIAL[sot.args[0]](self, argv)
             except (ParamsUnmatched, ArgumentMissing) as e1:
-                if (rest := self.container.release()) and isinstance(rest[-1], str):
-                    if rest[-1] in self.completion_names:
-                        last = self.container.bak_data[-1]
-                        self.container.bak_data[-1] = last[:last.rfind(rest[-1])]
-                        return handle_completion(self)
-                    if handler := self.special.get(rest[-1]):
-                        return handler(self)
+                if (rest := argv.release()) and isinstance(rest[-1], str):
+                    if rest[-1] in argv.completion_names:
+                        last = argv.bak_data[-1]
+                        argv.bak_data[-1] = last[:last.rfind(rest[-1])]
+                        return handle_completion(self, argv)
+                    if handler := argv.special.get(rest[-1]):
+                        return _SPECIAL[handler](self, argv)
                 if isinstance(e1, ArgumentMissing) and comp_ctx.get(None):
-                    raise PauseTriggered(prompt(self)) from e1
+                    raise PauseTriggered(prompt(self, argv)) from e1
                 if self.command.meta.raise_exception:
                     raise
-                return self.export(fail=True, exception=e1)
-            if self.container.done:
+                return self.export(argv, True, e1)
+            if argv.done:
                 break
 
         if self.default_main_only and not self.args_result:
-            self.args_result = analyse_args(self, self.self_args)
+            self.args_result = analyse_args(argv, self.self_args)
 
-    def export(self, exception: BaseException | None = None, fail: bool = False) -> Arparma[TDataCollection]:
+    def export(
+        self,
+        argv: Argv[TDataCollection],
+        fail: bool = False,
+        exception: BaseException | None = None,
+    ) -> Arparma[TDataCollection]:
         """创建arpamar, 其一定是一次解析的最后部分"""
-        result = Arparma(self.command.path, self.container.origin, not fail, self.header_result)
+        result = Arparma(self.command.path, argv.origin, not fail, self.header_result)
         if fail:
             result.error_info = repr(exception or traceback.format_exc(limit=1))
-            result.error_data = self.container.release()
+            result.error_data = argv.release()
         else:
             result.main_args = self.args_result
             result.options = self.options_result
             result.subcommands = self.subcommands_result
             result.unpack()
-            if self.container.message_cache:
-                command_manager.record(self.container.temp_token, result)
-                self.used_tokens.add(self.container.temp_token)
+            if argv.message_cache:
+                command_manager.record(argv.token, result)
+                self.used_tokens.add(argv.token)
         self.reset()
         return result  # type: ignore
 
-    @classmethod
-    def compile(
-        cls: type[TAnalyser],
-        command: Alconna[Any],
-        compiler: Callable[[TAnalyser, Namespace], None] = default_compiler
-    ) -> TAnalyser:
-        _analyser = cls(command)
-        compiler(_analyser, command.namespace_config)
-        return _analyser
-
 
-TAnalyser = TypeVar("TAnalyser", bound=Analyser, default=Analyser)
+TCompile: TypeAlias = "Callable[[SubAnalyser, Namespace, set[str]], None]"
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/args.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import inspect
 import re
 from copy import deepcopy
 from dataclasses import field as dc_field
 from enum import Enum
 from functools import partial
 from typing import Any, Callable, Generic, Iterable, Sequence, TypeVar, Union, TYPE_CHECKING
-from tarina import Empty
+from tarina import Empty, get_signature
+from tarina.lang import lang
 from nepattern import AllParam, AnyOne, BasePattern, UnionPattern, type_parser
 from typing_extensions import Self
-from tarina import get_signature
 
-from .lang import lang
 from .exceptions import InvalidParam
 from .typing import KeyWordVar, MultiVar
 
 if TYPE_CHECKING:
     from dataclasses import dataclass
 else:
     from .util import dataclass
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/arparma.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from abc import ABCMeta, abstractmethod
 from contextlib import suppress
 from dataclasses import dataclass, field
 from functools import lru_cache
 from types import MappingProxyType
 from typing import Any, Callable, Generic, Mapping, TypeVar, overload
 from tarina import get_signature, generic_isinstance, Empty
-
+from tarina.lang import lang
 from typing_extensions import Self
 
-from .lang import lang
 from .exceptions import BehaveCancelled, OutBoundsBehave
 from .model import HeadResult, OptionResult, SubcommandResult
 from .typing import TDataCollection
 
 T = TypeVar('T')
 D = TypeVar('D')
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/base.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Alconna 的基础内容相关"""
 from __future__ import annotations
 
 from functools import reduce
 from typing import Callable, Iterable, Sequence, overload
 from typing_extensions import Self
+from tarina.lang import lang
 
 from .action import ArgAction
 from .args import Arg, Args
-from .lang import lang
 from .exceptions import InvalidParam
 
 
 class CommandNode:
     """命令体基类, 规定基础命令的参数"""
     name: str
     dest: str
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/builtin.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .arparma import Arparma, ArparmaBehavior
 from .exceptions import BehaveCancelled
 from .model import OptionResult, SubcommandResult
 
 __all__ = ["set_default", "store_value", "store_true", "store_false"]
 
 
-class _MISSING_TYPE:pass
+class _MISSING_TYPE: pass
 MISSING = _MISSING_TYPE()
 
 
 class _StoreValue(ArgAction):
     def __init__(self, value: Any):
         super().__init__(lambda: value)
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/completion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, TYPE_CHECKING
 from tarina import ContextModel
+from tarina.lang import lang
 
 from .exceptions import PauseTriggered
 from .manager import command_manager
 from .output import output_manager
-from .lang import lang
+
 
 if TYPE_CHECKING:
     from .core import Alconna
 
 
 @dataclass(eq=True, frozen=True, unsafe_hash=True)
 class Prompt:
@@ -59,31 +60,32 @@
         if not self.prompts:
             raise ValueError("No prompt available.")
         self.index += offset
         self.index %= len(self.prompts)
         return self.prompts[self.index].text
 
     def enter(self, content: Any | None = None):
+        argv = command_manager.resolve(self.source.command)
         if content:
-            self.source.container.rebuild(content)
+            argv.rebuild(content)
             self.clear()
-            return self.source.process()
+            return self.source.process(argv)
         if not self.prompts:
             raise ValueError("No prompt available.")
         prompt = self.prompts[self.index]
         if not prompt.can_use:
             raise ValueError("This prompt cannot be used.")
         if prompt.removal_prefix:
-            last = self.source.container.bak_data[-1]
-            self.source.container.bak_data[-1] = last[
+            last = argv.bak_data[-1]
+            argv.bak_data[-1] = last[
                 : last.rfind(prompt.removal_prefix)
             ]
-        self.source.container.rebuild(prompt.text)
+        argv.rebuild(prompt.text)
         self.clear()
-        return self.source.process()
+        return self.source.process(argv)
 
     def push(self, *suggests: Prompt):
         self.prompts.extend(suggests)
         return self
 
     def clear(self):
         self.index = 0
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/config.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import ContextManager, TypedDict, Callable, Any, TYPE_CHECKING
-from .typing import THeader
+from tarina.lang import lang
+from pathlib import Path
+
+from .typing import TPrefixes
 
 if TYPE_CHECKING:
     from .formatter import TextFormatter
 
 
 class OptionNames(TypedDict):
     help: set[str]
     shortcut: set[str]
     completion: set[str]
 
 
 @dataclass(init=True, repr=True)
 class Namespace:
     name: str
-    headers: THeader = field(default_factory=list)
+    prefixes: TPrefixes = field(default_factory=list)
     separators: tuple[str, ...] = field(default_factory=lambda: (" ",))
     formatter_type: type[TextFormatter] | None = field(default=None)  # type: ignore
     fuzzy_match: bool = field(default=False)
     raise_exception: bool = field(default=False)
     enable_message_cache: bool = field(default=True)
     builtin_option_name: OptionNames = field(
         default_factory=lambda: {
@@ -34,14 +37,22 @@
 
     def __eq__(self, other):
         return isinstance(other, Namespace) and other.name == self.name
 
     def __hash__(self):
         return hash(self.name)
 
+    @property
+    def headers(self):
+        return self.prefixes
+
+    @headers.setter
+    def headers(self, value):
+        self.prefixes = value
+
 
 class namespace(ContextManager[Namespace]):
     """
     新建一个命名空间配置并暂时作为默认命名空间
 
     with namespace("xxx") as np:
         np.headers = [aaa]
@@ -63,17 +74,14 @@
             return False
         config.default_namespace = self.old
         config.namespaces[self.name] = self.np
         del self.old
         del self.np
 
 
-
-
-
 class _AlconnaConfig:
     command_max_count: int = 200
     message_max_cache: int = 100
     fuzzy_threshold: float = 0.6
     _default_namespace = "Alconna"
     namespaces: dict[str, Namespace] = {_default_namespace: Namespace(_default_namespace)}
 
@@ -91,10 +99,10 @@
             self._default_namespace = np
         else:
             self._default_namespace = np.name
             self.namespaces[np.name] = np
 
 
 config = _AlconnaConfig()
+lang.load(Path(__file__).parent / "i18n")
 
-
-__all__ = ["config", "Namespace", "namespace"]
+__all__ = ["config", "Namespace", "namespace", "lang"]
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/container.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/argv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
-from typing import Any, Callable, TypeVar
+from dataclasses import dataclass, field, InitVar
+from typing import Any, Callable, Generic
 from typing_extensions import Self
 from tarina import split, split_once
+from tarina.lang import lang
 
 from .args import Arg
+from .config import Namespace, config
 from .base import Option, Subcommand
-from .lang import lang
 from .exceptions import NullMessage
-from .typing import DataCollection
+from .typing import TDataCollection
 
 _cache: dict[type, dict[str, Any]] = {}
 
 
 @dataclass(repr=True)
-class DataCollectionContainer:
+class Argv(Generic[TDataCollection]):
+    namespace: InitVar[Namespace] = field(default=config.default_namespace)
+    fuzzy_match: bool = field(default=False)
     preprocessors: dict[str, Callable[..., Any]] = field(default_factory=dict)
     to_text: Callable[[Any], str | None] = field(default=lambda x: x if isinstance(x, str) else None)
     separators: tuple[str, ...] = field(default=(' ',))  # 分隔符
     filter_out: list[str] = field(default_factory=list)  # 元素黑名单
-    default_separate: bool = field(default=True)
     filter_crlf: bool = field(default=True)
     message_cache: bool = field(default=True)
     param_ids: set[str] = field(default_factory=set)
 
     context: Arg | Subcommand | Option | None = field(init=False)
     current_index: int = field(init=False)  # 当前数据的index
     ndata: int = field(init=False)  # 原始数据的长度
     bak_data: list[str | Any] = field(init=False)
     raw_data: list[str | Any] = field(init=False)
-    temp_token: int = field(init=False)  # 临时token
-    origin: DataCollection[Any] = field(init=False)
+    token: int = field(init=False)  # 临时token
+    origin: TDataCollection = field(init=False)
     _sep: tuple[str, ...] | None = field(init=False)
 
     @classmethod
     def config(
         cls,
         preprocessors: dict[str, Callable[..., Any]] | None = None,
         to_text: Callable[[Any], str | None] | None = None,
         filter_out: list[str] | None = None
     ):
         _cache.setdefault(cls, {}).update(locals())
 
-    def __post_init__(self):
+    def __post_init__(self, namespace: Namespace):
         self.reset()
+        self.special: dict[str, str] = {}
+        self.special.update(
+            [(i, "help") for i in namespace.builtin_option_name['help']] +
+            [(i, "completion") for i in namespace.builtin_option_name['completion']] +
+            [(i, "shortcut") for i in namespace.builtin_option_name['shortcut']]
+        )
+        self.completion_names = namespace.builtin_option_name['completion']
         if __cache := _cache.get(self.__class__, {}):
             self.preprocessors.update(__cache["preprocessors"] or {})
             self.filter_out.extend(__cache["filter_out"] or [])
             self.to_text = __cache["to_text"] or self.to_text
 
     def reset(self):
         self.current_index = 0
         self.ndata = 0
         self.bak_data = []
         self.raw_data = []
-        self.temp_token = 0
+        self.token = 0
         self.origin = "None"
         self._sep = None
         self.context = None
 
     @staticmethod
     def generate_token(data: list[Any | list[str]]) -> int:
         return hash(str(data))
 
     @property
     def done(self) -> bool:
         return self.current_index == self.ndata
 
-    def build(self, data: DataCollection[str | Any]) -> Self:
+    def build(self, data: TDataCollection) -> Self:
         """命令分析功能, 传入字符串或消息链"""
         self.reset()
         self.origin = data
         if isinstance(data, str):
             data = [data]
         i, raw_data = 0, self.raw_data
         for unit in data:
@@ -88,15 +97,15 @@
                 raw_data.append(res)
             i += 1
         if i < 1:
             raise NullMessage(lang.analyser_handle_null_message.format(target=data))
         self.ndata = i
         self.bak_data = raw_data.copy()
         if self.message_cache:
-            self.temp_token = self.generate_token(raw_data)
+            self.token = self.generate_token(raw_data)
         return self
 
     def rebuild(self, *data: str | Any) -> Self:
         self.raw_data = self.bak_data.copy()
         for i, d in enumerate(data):
             if not d:
                 continue
@@ -104,27 +113,27 @@
                 self.raw_data[-1] += f"{self.separators[0]}{d}"
             else:
                 self.raw_data.append(d)
                 self.ndata += 1
         self.current_index = 0
         self.bak_data = self.raw_data.copy()
         if self.message_cache:
-            self.temp_token = self.generate_token(self.raw_data)
+            self.token = self.generate_token(self.raw_data)
         return self
 
     def popitem(self, separate: tuple[str, ...] | None = None, move: bool = True) -> tuple[str | Any, bool]:
         """获取解析需要的下个数据"""
         if self._sep:
             self._sep = None
         if self.current_index == self.ndata:
             return "", True
         separate = separate or self.separators
         _current_data = self.raw_data[self.current_index]
-        if isinstance(_current_data, str):
-            _text, _rest_text = split_once(_current_data, separate, self.filter_crlf)
+        if _current_data.__class__ == str:
+            _text, _rest_text = split_once(_current_data, separate, self.filter_crlf)  # type: ignore
             if move:
                 if _rest_text:
                     self._sep = separate
                     self.raw_data[self.current_index] = _rest_text
                 else:
                     self.current_index += 1
             return _text, True
@@ -157,10 +166,7 @@
 
     def data_set(self):
         return self.raw_data.copy(), self.current_index
 
     def data_reset(self, data: list[str | Any], index: int):
         self.raw_data = data
         self.current_index = index
-
-
-TContainer = TypeVar("TContainer", bound=DataCollectionContainer)
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/core.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Alconna 主体"""
 from __future__ import annotations
 
 import sys
 from dataclasses import InitVar, dataclass, field
-from functools import reduce
+from functools import reduce, partial
 from typing import Any, Callable, Generic, Sequence, TypeVar, overload
 
 from tarina import init_spec
+from tarina.lang import lang
 from typing_extensions import Self
 
 from .action import ArgAction, exec_, exec_args
-from .analyser import Analyser
+from .analyser import TCompile, Analyser
 from .args import Arg, Args
 from .arparma import Arparma, ArparmaBehavior
 from .base import Option, Subcommand
 from .config import Namespace, config
-from .lang import lang
 from .duplication import Duplication
 from .exceptions import NullMessage
 from .executor import ArparmaExecutor, T
 from .formatter import TextFormatter
 from .manager import ShortcutArgs, command_manager
-from .typing import TDataCollection, THeader
+from .typing import TDataCollection, TPrefixes
 
 T_Duplication = TypeVar('T_Duplication', bound=Duplication)
 
 
 @dataclass
 class ActionHandler(ArparmaBehavior):
     source: InitVar[Alconna]
@@ -71,48 +71,49 @@
     更加精确的命令解析
 
     Examples:
 
         >>> from arclet.alconna import Alconna
         >>> alc = Alconna(
         ...     "name",
-        ...     ["h1", "h2"],
+        ...     ["p1", "p2"],
         ...     Option("opt", Args["opt_arg", "opt_arg"]),
         ...     Subcommand(
         ...         "sub_name",
         ...         Option("sub_opt", Args["sub_arg", "sub_arg"]),
         ...         Args["sub_main_args", "sub_main_args"]
         ...     ),
         ...     Args["main_args", "main_args"],
         ...  )
         >>> alc.parse("name opt opt_arg")
     """
-    headers: THeader
+    prefixes: TPrefixes
     command: str | Any
     analyser_type: type[Analyser]
     formatter: TextFormatter
     namespace: str
     meta: CommandMeta
     behaviors: list[ArparmaBehavior]
 
     global_analyser_type: type[Analyser] = Analyser
 
-    def compile(self) -> Analyser:
-        return self.analyser_type.compile(self)
+    @property
+    def compile(self) -> Callable[[TCompile | None], Analyser[TDataCollection]]:
+        return partial(self.analyser_type, self)
 
     @classmethod
     def default_analyser(cls, __t: type[Analyser] | None = None):
         """配置 Alconna 的默认解析器"""
         if __t is not None:
             cls.global_analyser_type = __t
         return cls
 
     def __init__(
         self,
-        *args: Option | Subcommand | str | THeader | Any | Args | Arg,
+        *args: Option | Subcommand | str | TPrefixes | Any | Args | Arg,
         action: ArgAction | Callable | None = None,
         meta: CommandMeta | None = None,
         namespace: str | Namespace | None = None,
         separators: str | set[str] | Sequence[str] | None = None,
         analyser_type: type[Analyser] | None = None,
         behaviors: list[ArparmaBehavior] | None = None,
         formatter_type: type[TextFormatter] | None = None
@@ -132,19 +133,19 @@
         """
         if not namespace:
             np_config = config.default_namespace
         elif isinstance(namespace, Namespace):
             np_config = config.namespaces.setdefault(namespace.name, namespace)
         else:
             np_config = config.namespaces.setdefault(namespace, Namespace(namespace))
-        self.headers = next(filter(lambda x: isinstance(x, list), args + (np_config.headers.copy(),)))  # type: ignore
+        self.prefixes = next(filter(lambda x: isinstance(x, list), args + (np_config.prefixes.copy(),)))  # type: ignore
         try:
             self.command = next(filter(lambda x: not isinstance(x, (list, Option, Subcommand, Args, Arg)), args))
         except StopIteration:
-            self.command = "" if self.headers else sys.argv[0]
+            self.command = "" if self.prefixes else sys.argv[0]
         self.namespace = np_config.name
         self.analyser_type = analyser_type or self.__class__.global_analyser_type  # type: ignore
         self.formatter = (formatter_type or np_config.formatter_type or TextFormatter)()
         self.meta = meta or CommandMeta()
         self.meta.fuzzy_match = self.meta.fuzzy_match or np_config.fuzzy_match
         self.meta.raise_exception = self.meta.raise_exception or np_config.raise_exception
         options = [i for i in args if isinstance(i, (Option, Subcommand))]
@@ -159,15 +160,15 @@
             )
         )
         options.append(
             Option(
                 "|".join(np_config.builtin_option_name['completion']), help_text=lang.builtin.option_completion
             )
         )
-        name = f"{self.command or self.headers[0]}".replace(command_manager.sign, "")  # type: ignore
+        name = f"{self.command or self.prefixes[0]}".replace(command_manager.sign, "")  # type: ignore
         self.path = f"{self.namespace}::{name}"
         super().__init__(
             "ALCONNA::",
             reduce(lambda x, y: x + y, [Args()] + [i for i in args if isinstance(i, (Arg, Args))]),  # type: ignore
             *options,
             dest=name,
             action=action,
@@ -188,15 +189,15 @@
         """重新设置命名空间"""
         command_manager.delete(self)
         if isinstance(namespace, str):
             namespace = config.namespaces.setdefault(namespace, Namespace(namespace))
         self.namespace = namespace.name
         self.path = f"{self.namespace}::{self.name}"
         if header:
-            self.headers = namespace.headers.copy()
+            self.prefixes = namespace.prefixes.copy()
         self.options[-3] = Option(
             "|".join(namespace.builtin_option_name['help']), help_text=lang.builtin.option_help
         )
         self.options[-2] = Option(
             "|".join(namespace.builtin_option_name['shortcut']),
             Args["delete;?", "delete"]["name", str]["command", str, "_"],
             help_text=lang.builtin.option_shortcut
@@ -260,21 +261,22 @@
 
     @init_spec(Subcommand, True)
     def subcommand(self, sub: Subcommand) -> Self:
         return self.add(sub)
 
     def _parse(self, message: TDataCollection) -> Arparma[TDataCollection]:
         if self.union:
-            for ana in command_manager.requires(*self.union):
-                ana.container.build(message)
-                if (res := ana.process()).matched:
+            for ana, argv in command_manager.requires(*self.union):
+                argv.build(message)
+                if (res := ana.process(argv)).matched:
                     return res
         analyser = command_manager.require(self)
-        analyser.container.build(message)
-        return analyser.process()
+        argv = command_manager.resolve(self)
+        argv.build(message)
+        return analyser.process(argv)
 
     @overload
     def parse(self, message: TDataCollection) -> Arparma[TDataCollection]:
         ...
 
     @overload
     def parse(self, message, *, duplication: type[T_Duplication]) -> T_Duplication:
@@ -324,12 +326,15 @@
 
     def __or__(self, other: Alconna) -> Self:
         self.union.add(other.path)
         return self
 
     def _calc_hash(self):
         return hash(
-            (self.path + str(self.headers), self.meta, *self.options, *self.args.argument)
+            (self.path + str(self.prefixes), self.meta, *self.options, *self.args.argument)
         )
 
+    def __call__(self, *args, **kwargs):
+        return self.parse(list(args)) if args else self.parse(sys.argv[1:])
+
 
 __all__ = ["Alconna", "CommandMeta"]
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/duplication.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/executor.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/executor.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/formatter.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,17 +60,17 @@
     body: list[Option | Subcommand]
 
     def union(self, others: list[Trace]):
         if not others:
             return self
         if others[0] == self:
             return self.union(others[1:])
-        hds = self.head.copy()
-        hds['header'] = list({*self.head['header'], *others[0].head['header']})
-        return Trace(hds, self.args, self.separators, list({*self.body, *others[0].body})).union(others[1:])
+        pfs = self.head.copy()
+        pfs['prefix'] = list({*self.head['prefix'], *others[0].head['prefix']})
+        return Trace(pfs, self.args, self.separators, list({*self.body, *others[0].body})).union(others[1:])
 
 
 class TextFormatter:
     """帮助文档格式化器
 
     该格式化器负责将传入的命令节点字典解析并生成帮助文档字符串
     """
@@ -79,20 +79,20 @@
         self.data = {}
         self.ignore_names = set()
 
     def add(self, base: Alconna):
         self.ignore_names.update(base.namespace_config.builtin_option_name['help'])
         self.ignore_names.update(base.namespace_config.builtin_option_name['shortcut'])
         self.ignore_names.update(base.namespace_config.builtin_option_name['completion'])
-        hds = base.headers.copy()
-        if base.name in hds:
-            hds.remove(base.name)  # type: ignore
+        pfs = base.prefixes.copy()
+        if base.name in pfs:
+            pfs.remove(base.name)  # type: ignore
         res = Trace(
             {
-                'name': base.name, 'header': hds or [], 'description': base.meta.description,
+                'name': base.name, 'prefix': pfs or [], 'description': base.meta.description,
                 'usage': base.meta.usage, 'example': base.meta.example
             },
             base.args, base.separators, base.options.copy()
         )
         self.data.setdefault(base.path, []).append(res)
         return self
 
@@ -125,37 +125,37 @@
                     for k, i in _cache.items():
                         if isinstance(i, dict):
                             _opts.append(Option(k, requires=_parts))
                         elif i not in _visited:
                             _opts.append(i)
                             _visited.add(i)
                     return self.format(Trace(
-                        {"name": _parts[-1], 'header': [], 'description': _parts[-1]}, Args(), trace.separators,
+                        {"name": _parts[-1], 'prefix': [], 'description': _parts[-1]}, Args(), trace.separators,
                         _opts
                     ))
             if isinstance(_cache, Option):
                 return self.format(Trace(
-                    {"name": "", "header": list(_cache.aliases), "description": _cache.help_text}, _cache.args,
+                    {"name": "", "prefix": list(_cache.aliases), "description": _cache.help_text}, _cache.args,
                     _cache.separators, []
                 ))
             if isinstance(_cache, Subcommand):
                 return self.format(Trace(
-                    {"name": _cache.name, "header": [], "description": _cache.help_text}, _cache.args,
+                    {"name": _cache.name, "prefix": [], "description": _cache.help_text}, _cache.args,
                     _cache.separators, _cache.options  # type: ignore
                 ))
             return self.format(trace)
 
         return "\n".join([_handle(v) for v in self.data.values()])
 
     def format(self, trace: Trace) -> str:
         """help text的生成入口"""
-        header = self.header(trace.head, trace.separators)
+        prefix = self.header(trace.head, trace.separators)
         param = self.parameters(trace.args)
         body = self.body(trace.body)
-        return header % (param, body)
+        return prefix % (param, body)
 
     def param(self, parameter: Arg) -> str:
         """对单个参数的描述"""
         name = parameter.name
         arg = f"[{name}" if parameter.optional else f"<{name}"
         if not parameter.hidden:
             if parameter.value is AllParam:
@@ -183,16 +183,16 @@
         return f"{res}\n## 注释\n  " + "\n  ".join([f"{v[0]}: {v[1]}" for v in notice]) if notice else res
 
     def header(self, root: dict[str, Any], separators: tuple[str, ...]) -> str:
         """头部节点的描述"""
         help_string = f"\n{desc}" if (desc := root.get('description')) else ""
         usage = f"\n用法:\n{usage}" if (usage := root.get('usage')) else ""
         example = f"\n使用示例:\n{example}" if (example := root.get('example')) else ""
-        headers = f"[{''.join(map(str, headers))}]" if (headers := root.get('header', [])) != [] else ""
-        cmd = f"{headers}{root.get('name', '')}"
+        prefixs = f"[{''.join(map(str, prefixs))}]" if (prefixs := root.get('prefix', [])) != [] else ""
+        cmd = f"{prefixs}{root.get('name', '')}"
         command_string = cmd or (root['name'] + separators[0])
         return f"{command_string} %s{help_string}{usage}\n%s{example}"
 
     def part(self, node: Subcommand | Option) -> str:
         """每个子节点的描述"""
         if isinstance(node, Subcommand):
             name = " ".join(node.requires) + (' ' if node.requires else '') + node.name
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/handlers.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,203 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Any, Iterable
 from tarina import Empty, split_once
+from tarina.lang import lang
 from nepattern import AllParam, BasePattern
 from nepattern.util import TPattern
 
 from .args import Arg, Args
-from .header import Double
+from .header import Double, Header
 from .base import Option, Subcommand
 from .config import config
-from .lang import lang
 from .completion import Prompt, comp_ctx
 from .exceptions import ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, SpecialOptionTriggered, PauseTriggered
 from .model import OptionResult, Sentence, HeadResult
 from .output import output_manager
 from .typing import KeyWordVar, MultiVar
 from .util import levenshtein_norm
 
 if TYPE_CHECKING:
-    from .analyser import SubAnalyser, DataCollectionContainer, Analyser
+    from .argv import Argv
+    from .analyser import SubAnalyser, Analyser
 
 
 def _handle_keyword(
-    container: DataCollectionContainer,
+    argv: Argv,
     value: KeyWordVar,
     may_arg: Any,
     seps: tuple[str, ...],
     result_dict: dict[str, Any],
     default_val: Any,
     optional: bool,
     key: str | None = None,
     fuzzy: bool = False,
 ):
     if _kwarg := re.match(fr'^([^{value.sep}]+){value.sep}(.*?)$', may_arg):
         key = key or _kwarg[1]
         if (_key := _kwarg[1]) != key:
-            container.pushback(may_arg)
+            argv.pushback(may_arg)
             if fuzzy and levenshtein_norm(_key, key) >= config.fuzzy_threshold:
                 raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_key, target=key))
             if default_val is None:
                 raise ParamsUnmatched(lang.common.fuzzy_matched.format(source=_key, target=key))
             result_dict[_key] = None if default_val is Empty else default_val
             return
         if not (_m_arg := _kwarg[2]):
-            _m_arg, _ = container.popitem(seps)
+            _m_arg, _ = argv.popitem(seps)
         res = value.base(_m_arg, default_val)
         if res.flag != 'valid':
-            container.pushback(may_arg)
+            argv.pushback(may_arg)
         if res.flag == 'error':
             if optional:
                 return
             raise ParamsUnmatched(*res.error.args)
         result_dict[_kwarg[1]] = res._value  # type: ignore
         return
-    container.pushback(may_arg)
+    argv.pushback(may_arg)
     raise ParamsUnmatched(lang.args.key_missing.format(target=may_arg, key=key))
 
 
 def _loop_kw(
-    container: DataCollectionContainer,
+    argv: Argv,
     _loop: int,
     seps: tuple[str, ...],
     value: MultiVar,
     default: Any
 ):
     result = {}
     for _ in range(_loop):
-        _m_arg, _m_str = container.popitem(seps)
+        _m_arg, _m_str = argv.popitem(seps)
         if not _m_arg:
             continue
-        if _m_str and _m_arg in container.param_ids:
-            container.pushback(_m_arg)
+        if _m_str and _m_arg in argv.param_ids:
+            argv.pushback(_m_arg)
             break
         try:
-            _handle_keyword(container, value.base, _m_arg, seps, result, default, False)  # type: ignore
+            _handle_keyword(argv, value.base, _m_arg, seps, result, default, False)  # type: ignore
         except ParamsUnmatched:
             break
     if not result:
         if value.flag == '+':
             raise ParamsUnmatched
         result = [default] if default else []
     return result
 
 
 def _loop(
-    container: DataCollectionContainer,
+    argv: Argv,
     _loop: int,
     seps: tuple[str, ...],
     value: MultiVar,
     default: Any,
     args: Args
 ):
     kw = args[args.var_keyword].value.base if args.var_keyword else None
     result = []
     for _ in range(_loop):
-        _m_arg, _m_str = container.popitem(seps)
+        _m_arg, _m_str = argv.popitem(seps)
         if not _m_arg:
             continue
         if _m_str and (
-            _m_arg in container.param_ids or
+            _m_arg in argv.param_ids or
             (kw and re.match(fr'^([^{kw.sep}]+){kw.sep}(.*?)$', _m_arg))
         ):
-            container.pushback(_m_arg)
+            argv.pushback(_m_arg)
             break
         if (res := value.base(_m_arg)).flag != 'valid':
-            container.pushback(_m_arg)
+            argv.pushback(_m_arg)
             break
         result.append(res._value)  # type: ignore
     if not result:
         if value.flag == '+':
             raise ParamsUnmatched
         result = [default] if default else []
     return tuple(result)
 
 
 def multi_arg_handler(
-    analyser: SubAnalyser,
+    argv: Argv,
     args: Args,
     arg: Arg,
     result_dict: dict[str, Any],
 ):
     seps = arg.separators
     value = arg.value
     key = arg.name
     default = arg.field.default_gen
     kw = value.base.__class__ == KeyWordVar
     _m_rest_arg = len(args) - len(result_dict)
-    _m_rest_all_param_count = len(analyser.container.release(seps))
+    _m_rest_all_param_count = len(argv.release(seps))
     if not kw and not args.var_keyword or kw and not args.var_positional:
         loop = _m_rest_all_param_count - _m_rest_arg + 1
     elif not kw:
         loop = _m_rest_all_param_count - (_m_rest_arg - 2*(args[args.var_keyword].value.flag == "*"))
     else:
         loop = _m_rest_all_param_count - (_m_rest_arg - 2*(args[args.var_positional].value.flag == "*"))
     if value.length > 0:
         loop = min(loop, value.length)
     result_dict[key] = (
-        _loop_kw(analyser.container, loop, seps, value, default) if kw
-        else _loop(analyser.container, loop, seps, value, default, args)
+        _loop_kw(argv, loop, seps, value, default) if kw
+        else _loop(argv, loop, seps, value, default, args)
     )
 
 
-def analyse_args(analyser: SubAnalyser, args: Args) -> dict[str, Any]:
+def analyse_args(argv: Argv, args: Args) -> dict[str, Any]:
     """
     分析 Args 部分
 
     Args:
-        analyser: 使用的分析器
+        argv: 使用的分析器
         args: 目标Args
 
     Returns:
         Dict: 解析结果
     """
     result: dict[str, Any] = {}
     for arg in args.argument:
-        analyser.container.context = arg
+        argv.context = arg
         key = arg.name
         value = arg.value
         default_val = arg.field.default_gen
         optional = arg.optional
         seps = arg.separators
-        may_arg, _str = analyser.container.popitem(seps)
-        if _str and may_arg in analyser.special:
-            raise SpecialOptionTriggered(analyser.special[may_arg])
-        if (
-            (not may_arg or (_str and may_arg in analyser.container.param_ids))
-            and (value.__class__ != MultiVar or value.__class__ is MultiVar and value.flag == '+')
-        ):
-            analyser.container.pushback(may_arg)
+        may_arg, _str = argv.popitem(seps)
+        if _str and may_arg in argv.special:
+            raise SpecialOptionTriggered(argv.special[may_arg])
+        if not may_arg or (_str and may_arg in argv.param_ids):
+            argv.pushback(may_arg)
             if default_val is not None:
                 result[key] = None if default_val is Empty else default_val
+            elif value.__class__ is MultiVar and value.flag == '*':
+                result[key] = ()
             elif not optional:
                 raise ArgumentMissing(lang.args.missing.format(key=key))
             continue
         if value.__class__ is MultiVar:
-            analyser.container.pushback(may_arg)
-            multi_arg_handler(analyser, args, arg, result)  # type: ignore
+            argv.pushback(may_arg)
+            multi_arg_handler(argv, args, arg, result)  # type: ignore
         elif value.__class__ is KeyWordVar:
             _handle_keyword(
-                analyser.container, value, may_arg, seps, result, default_val, optional, key, analyser.fuzzy_match  # type: ignore
+                argv, value, may_arg, seps, result, default_val, optional, key, argv.fuzzy_match  # type: ignore
             )
         elif value is AllParam:
-            analyser.container.pushback(may_arg)
-            result[key] = analyser.container.release(seps)
-            analyser.container.current_index = analyser.container.ndata
+            argv.pushback(may_arg)
+            result[key] = argv.release(seps)
+            argv.current_index = argv.ndata
             return result
         else:
             res = (
                 value.invalidate(may_arg, default_val)
                 if value.anti
                 else value.validate(may_arg, default_val)
             )
             if res.flag != 'valid':
-                analyser.container.pushback(may_arg)
+                argv.pushback(may_arg)
             if res.flag == 'error':
                 if optional:
                     continue
                 raise ParamsUnmatched(*res.error.args)
             if not arg.anonymous:
                 result[key] = res._value  # type: ignore
     if args.var_keyword:
@@ -210,185 +210,186 @@
         if not isinstance(varargs, Iterable):
             varargs = [varargs]
         elif not isinstance(varargs, list):
             varargs = list(varargs)
         result['$varargs'] = (varargs, args.var_positional)
     if args.keyword_only:
         result['$kwonly'] = {k: v for k, v in result.items() if k in args.keyword_only}
-    analyser.container.context = None
+    argv.context = None
     return result
 
 
-def analyse_unmatch_params(analyser: SubAnalyser, text: str):
+def analyse_unmatch_params(analyser: SubAnalyser, argv: Argv, text: str):
     for _p in analyser.compile_params.values():
         if isinstance(_p, list):
             res = []
             for _o in _p:
                 _may_param, _ = split_once(text, _o.separators)
                 if _may_param in _o.aliases or any(map(_may_param.startswith, _o.aliases)):
                     analyser.compile_params.setdefault(text, res)
                     res.append(_o)
                     continue
-                if analyser.fuzzy_match and levenshtein_norm(_may_param, _o.name) >= config.fuzzy_threshold:
+                if argv.fuzzy_match and levenshtein_norm(_may_param, _o.name) >= config.fuzzy_threshold:
                     raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_may_param, target=_o.name))
             if res:
                 return res
         elif isinstance(_p, Sentence):
             if (_may_param := split_once(text, _p.separators)[0]) == _p.name:
                 analyser.compile_params.setdefault(text, _p)
                 return _p
-            if analyser.fuzzy_match and levenshtein_norm(_may_param, _p.name) >= config.fuzzy_threshold:
+            if argv.fuzzy_match and levenshtein_norm(_may_param, _p.name) >= config.fuzzy_threshold:
                 raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_may_param, target=_p.name))
         else:
             _may_param, _ = split_once(text, _p.command.separators)
             if _may_param == _p.command.name or _may_param.startswith(_p.command.name):
                 analyser.compile_params.setdefault(text, _p)
                 return _p
-            if analyser.fuzzy_match and levenshtein_norm(_may_param, _p.command.name) >= config.fuzzy_threshold:
+            if argv.fuzzy_match and levenshtein_norm(_may_param, _p.command.name) >= config.fuzzy_threshold:
                 raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_may_param, target=_p.command.name))
 
 
-def analyse_option(analyser: SubAnalyser, param: Option) -> tuple[str, OptionResult]:
+def analyse_option(analyser: SubAnalyser, argv: Argv, param: Option) -> tuple[str, OptionResult]:
     """
     分析 Option 部分
 
     Args:
         analyser: 使用的分析器
         param: 目标Option
     """
-    analyser.container.context = param
+    argv.context = param
     if param.requires and analyser.sentences != param.requires:
         raise ParamsUnmatched(f"{param.name}'s required is not '{' '.join(analyser.sentences)}'")
     analyser.sentences = []
     if param.is_compact:
-        name, _ = analyser.container.popitem()
+        name, _ = argv.popitem()
         for al in param.aliases:
             if mat := re.fullmatch(f"{al}(?P<rest>.*?)", name):
-                analyser.container.pushback(mat.groupdict()['rest'], replace=True)
+                argv.pushback(mat.groupdict()['rest'], replace=True)
                 break
         else:
             raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
     else:
-        name, _ = analyser.container.popitem(param.separators)
+        name, _ = argv.popitem(param.separators)
         if name not in param.aliases:  # 先匹配选项名称
             raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
     name = param.dest
     if param.nargs == 0:
         return name, OptionResult()
-    return name, OptionResult(None, analyse_args(analyser, param.args))
+    return name, OptionResult(None, analyse_args(argv, param.args))
 
 
-def analyse_param(analyser: SubAnalyser, _text: Any, _str: bool):
-    if _str and _text in analyser.special:
-        if _text in analyser.completion_names:
-            if analyser.container.current_index < analyser.container.ndata:
-                analyser.container.bak_data = analyser.container.bak_data[:analyser.container.current_index+1]
-            last = analyser.container.bak_data[-1]
-            analyser.container.bak_data[-1] = last[:last.rfind(_text)]
-        raise SpecialOptionTriggered(analyser.special[_text])
+def analyse_param(analyser: SubAnalyser, argv: Argv, _text: Any, _str: bool):
+    if _str and _text in argv.special:
+        if _text in argv.completion_names:
+            if argv.current_index < argv.ndata:
+                argv.bak_data = argv.bak_data[:argv.current_index+1]
+            last = argv.bak_data[-1]
+            argv.bak_data[-1] = last[:last.rfind(_text)]
+        raise SpecialOptionTriggered(argv.special[_text])
     if not _str or not _text:
         _param = None
     elif _text in analyser.compile_params:
         _param = analyser.compile_params[_text]
     else:
-        _param = None if analyser.container.default_separate else analyse_unmatch_params(analyser, _text)
+        _param = None if analyser.default_separate else analyse_unmatch_params(analyser, argv, _text)
     if not _param and not analyser.args_result:
-        analyser.args_result = analyse_args(analyser, analyser.self_args)
+        analyser.args_result = analyse_args(argv, analyser.self_args)
     elif isinstance(_param, list):
         for opt in _param:
-            _data, _index = analyser.container.data_set()
+            _data, _index = argv.data_set()
             try:
-                opt_n, opt_v = analyse_option(analyser, opt)
+                opt_n, opt_v = analyse_option(analyser, argv, opt)
                 analyser.options_result[opt_n] = opt_v
                 _data.clear()
                 break
             except Exception as e:
                 exc = e
-                analyser.container.data_reset(_data, _index)
+                argv.data_reset(_data, _index)
                 continue
         else:
             raise exc  # type: ignore  # noqa
     elif isinstance(_param, Sentence):
-        analyser.sentences.append(analyser.container.popitem()[0])
+        analyser.sentences.append(argv.popitem()[0])
     elif _param:
-        _param.process()
-        analyser.subcommands_result.setdefault(_param.command.dest, _param.export())
-    analyser.container.context = None
+        _param.process(argv)
+        analyser.subcommands_result.setdefault(_param.command.dest, _param.result())
+    argv.context = None
 
 
-def analyse_header(analyser: Analyser) -> HeadResult:
-    header = analyser.command_header
+def analyse_header(header: Header, argv: Argv) -> HeadResult:
     content = header.content
     mapping = header.mapping
-    head_text, _str = analyser.container.popitem()
+    head_text, _str = argv.popitem()
     if isinstance(content, TPattern) and _str and (mat := content.fullmatch(head_text)):
         return HeadResult(head_text, head_text, True, mat.groupdict(), mapping)
     elif isinstance(content, BasePattern) and (val := content(head_text, Empty)).success:
         return HeadResult(head_text, val.value, True, fixes=mapping)
 
-    may_command, _m_str = analyser.container.popitem()
+    may_command, _m_str = argv.popitem()
     if isinstance(content, list) and _m_str:
         for pair in content:
             if res := pair.match(head_text, may_command):
                 return HeadResult(*res, fixes=mapping)
     if isinstance(content, Double) and (
-        res := content.match(head_text, may_command, _str, _m_str, analyser.container.pushback)
+        res := content.match(head_text, may_command, _str, _m_str, argv.pushback)
     ):
         return HeadResult(*res, fixes=mapping)
 
-    if _str and analyser.fuzzy_match:
+    if _str and argv.fuzzy_match:
+        command, prefixes = header.origin
         headers_text = []
-        if analyser.command.headers and analyser.command.headers != [""]:
-            headers_text.extend(f"{i}{analyser.command.command}" for i in analyser.command.headers)
-        elif analyser.command.command:
-            headers_text.append(str(analyser.command.command))
+        if prefixes and prefixes != [""]:
+            headers_text.extend(f"{i}{command}" for i in prefixes)
+        elif command:
+            headers_text.append(str(command))
         if isinstance(content, (TPattern, BasePattern)):
             source = head_text
         else:
-            source = head_text + analyser.container.separators[0] + str(may_command)
-        if source == analyser.command.command:
-            analyser.header_result = HeadResult(source, source, False)
+            source = head_text + argv.separators[0] + str(may_command)
+        if source == command:
             raise ParamsUnmatched(lang.header.error.format(target=head_text))
         for ht in headers_text:
             if levenshtein_norm(source, ht) >= config.fuzzy_threshold:
-                analyser.header_result = HeadResult(source, ht, True)
                 raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(target=source, source=ht))
     raise ParamsUnmatched(lang.header.error.format(target=head_text))
 
 
-def handle_help(analyser: Analyser):
-    _help_param = [str(i) for i in analyser.container.release(recover=True) if str(i) not in analyser.special]
+def handle_help(analyser: Analyser, argv: Argv):
+    _help_param = [str(i) for i in argv.release(recover=True) if str(i) not in argv.special]
     output_manager.send(
         analyser.command.name,
         lambda: analyser.command.formatter.format_node(_help_param),
     )
-    return analyser.export(fail=True)
+    return analyser.export(argv, True)
+
+
+_args = Args["delete;?", "delete"]["name", str]["command", str, "_"]
 
 
-def handle_shortcut(analyser: Analyser):
-    analyser.container.popitem()
-    opt_v = analyse_args(analyser, Args["delete;?", "delete"]["name", str]["command", str, "_"])
+def handle_shortcut(analyser: Analyser, argv: Argv):
+    argv.popitem()
+    opt_v = analyse_args(argv, _args)
     try:
         msg = analyser.command.shortcut(
             opt_v["name"],
             None if opt_v["command"] == "_" else {"command": analyser.converter(opt_v["command"])},
             bool(opt_v.get("delete"))
         )
         output_manager.send(analyser.command.name, lambda: msg)
     except Exception as e:
         output_manager.send(analyser.command.name, lambda: str(e))
-    return analyser.export(fail=True)
+    return analyser.export(argv, True)
 
 
-def _prompt_unit(analyser: Analyser, trigger: Arg):
+def _prompt_unit(argv: Argv, trigger: Arg):
     if trigger.field.completion:
         comp = trigger.field.completion()
         if isinstance(comp, str):
             return [Prompt(comp, False)]
-        releases = analyser.container.release(recover=True)
+        releases = argv.release(recover=True)
         target = str(releases[-1]) or str(releases[-2])
         o = list(filter(lambda x: target in x, comp)) or comp
         return [Prompt(i, False, target) for i in o]
     default = trigger.field.default_gen
     o = f"[{trigger.name}]{trigger.value}{'' if default is None else f' default:({None if default is Empty else default})'}"
     return [Prompt(o, False)]
 
@@ -403,62 +404,62 @@
         if len(opt.requires) > s_len:
             res.append(opt.requires[s_len])
         else:
             res.extend(opt.aliases if isinstance(opt, Option) else [opt.name])
     return [Prompt(i) for i in res]
 
 
-def _prompt_none(analyser: Analyser, got: list[str]):
+def _prompt_none(analyser: Analyser, argv: Argv, got: list[str]):
     res: list[Prompt] = []
     if not analyser.args_result and analyser.self_args.argument:
         unit = analyser.self_args.argument[0]
         if gen := unit.field.completion:
             res.extend([Prompt(comp, False)] if isinstance(comp := gen(), str) else [Prompt(i, False) for i in comp])
         else:
             default = unit.field.default_gen
             res.append(
                 Prompt(
                     f"[{unit.name}]{unit.value}{'' if default is None else f' ({None if default is Empty else default})'}",
                     False
                 )
             )
     for opt in filter(
-        lambda x: x.name not in analyser.completion_names,
+        lambda x: x.name not in argv.completion_names,
         analyser.command.options,
     ):
         if opt.requires and all(opt.requires[0] not in i for i in got):
             res.append(Prompt(opt.requires[0]))
         elif opt.dest not in got:
             res.extend([Prompt(al) for al in opt.aliases] if isinstance(opt, Option) else [Prompt(opt.name)])
     return res
 
 
-def prompt(analyser: Analyser, trigger: str | None = None):
-    trigger = trigger or analyser.container.context
+def prompt(analyser: Analyser, argv: Argv, trigger: str | None = None):
+    trigger = trigger or argv.context
     got = [*analyser.options_result.keys(), *analyser.subcommands_result.keys(), *analyser.sentences]
     if isinstance(trigger, Arg):
-        return _prompt_unit(analyser, trigger)
+        return _prompt_unit(argv, trigger)
     elif isinstance(trigger, Subcommand):
         return [Prompt(i) for i in analyser.get_sub_analyser(trigger).compile_params]
     elif isinstance(trigger, str):
         res = list(filter(lambda x: trigger in x, analyser.compile_params))
         if not res:
             return []
         out = [i for i in res if i not in got]
         return [Prompt(i, True, trigger) for i in (out or res)]
-    releases = analyser.container.release(recover=True)
+    releases = argv.release(recover=True)
     target = str(releases[-1]) or str(releases[-2])
     if _res := list(filter(lambda x: target in x and target != x, analyser.compile_params)):
         out = [i for i in _res if i not in got]
         return [Prompt(i, True, target) for i in (out or _res)]
-    return _prompt_sentence(analyser) if analyser.sentences else _prompt_none(analyser, got)
+    return _prompt_sentence(analyser) if analyser.sentences else _prompt_none(analyser, argv, got)
 
 
-def handle_completion(analyser: Analyser, trigger: str | None = None):
-    if res := prompt(analyser, trigger):
+def handle_completion(analyser: Analyser, argv: Argv, trigger: str | None = None):
+    if res := prompt(analyser, argv, trigger):
         if comp_ctx.get(None):
             raise PauseTriggered(res)
         output_manager.send(
             analyser.command.name,
             lambda: f"{lang.common.completion_node}\n* " + "\n* ".join([i.text for i in res]),
         )
-    return analyser.export(fail=True, exception='NoneType: None\n')  # type: ignore
+    return analyser.export(argv, True, 'NoneType: None\n')  # type: ignore
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/header.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/header.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from inspect import isclass
 from typing import Any, Callable
 
 from nepattern import BasePattern, UnionPattern, all_patterns, type_parser
 from nepattern.util import TPattern
 from tarina import Empty
 
+from .typing import TPrefixes
+
 
 def handle_bracket(name: str):
     pattern_map = all_patterns()
     mapping = {}
     if len(parts := re.split(r"(\{.*?})", name)) <= 1:
         return name, mapping
     for i, part in enumerate(parts):
@@ -106,57 +108,60 @@
             and (_val := self.command(command, Empty)).success
         ):
             return (_po, command), (_pr, _val.value), True
 
 
 @dataclass
 class Header:
+    origin: tuple[str | type | BasePattern, TPrefixes]
     content: TPattern | BasePattern | list[Pair] | Double
     mapping: dict[str, BasePattern] = field(default_factory=dict)
 
     @classmethod
     def generate(
         cls,
         command: str | type | BasePattern,
-        headers: list[Any] | list[tuple[Any, str]],
+        prefixes: TPrefixes,
     ):
         mapping = {}
         if isinstance(command, str):
             command, mapping = handle_bracket(command)
         _cmd_name: TPattern | BasePattern
         _cmd_str: str
         _cmd_name, _cmd_str = (
             (re.compile(command), command)
             if isinstance(command, str)
             else (deepcopy(type_parser(command)), str(command))
         )
-        if not headers:
-            return cls(_cmd_name, mapping)
-        if isinstance(headers[0], tuple):
+        if not prefixes:
+            return cls((command, prefixes), _cmd_name, mapping)
+        if isinstance(prefixes[0], tuple):
             return cls(
-                [Pair(h[0], re.compile(re.escape(h[1]) + _cmd_str)) for h in headers],
+                (command, prefixes),
+                [Pair(h[0], re.compile(re.escape(h[1]) + _cmd_str)) for h in prefixes],
                 mapping,
             )
         elements = []
         patterns = []
         ch_text = ""
-        for h in headers:
+        for h in prefixes:
             if isinstance(h, str):
                 ch_text += f"{re.escape(h)}|"
             elif isinstance(h, BasePattern):
                 patterns.append(h)
             else:
                 elements.append(h)
         if not elements and not patterns:
             if isinstance(_cmd_name, TPattern):
-                return cls(re.compile(f"(?:{ch_text[:-1]}){_cmd_str}"), mapping)
+                return cls((command, prefixes), re.compile(f"(?:{ch_text[:-1]}){_cmd_str}"), mapping)
             _cmd_name.pattern = f"(?:{ch_text[:-1]}){_cmd_name.pattern}"  # type: ignore
             _cmd_name.regex_pattern = re.compile(_cmd_name.pattern)  # type: ignore
-            return cls(_cmd_name)
+            return cls((command, prefixes), _cmd_name)
         return cls(
+            (command, prefixes),
             Double(
                 elements,
                 UnionPattern(patterns) if patterns else None,
                 re.compile(f"(?:{ch_text[:-1]})") if ch_text else None,
                 _cmd_name,
             ),
             mapping,
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,35 +7,38 @@
 import shelve
 import weakref
 from copy import copy
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Match, TypedDict, Union, overload, Generic
 from typing_extensions import NotRequired
 from tarina import LRU
+from tarina.lang import lang
 from weakref import WeakKeyDictionary, WeakValueDictionary
 
+from .argv import Argv
 from .arparma import Arparma
 from .config import Namespace, config
-from .lang import lang
 from .exceptions import ExceedMaxCount
 from .typing import DataCollection, TDataCollection
 
 
 if TYPE_CHECKING:
     from .analyser import Analyser
     from .core import Alconna, CommandMeta
 
 
     class ShortcutArgs(TypedDict, Generic[TDataCollection]):
         command: NotRequired[TDataCollection]
         args: NotRequired[list[Any]]
+        fuzzy: NotRequired[bool]
 else:
     class ShortcutArgs(TypedDict):
         command: NotRequired[DataCollection[Any]]
         args: NotRequired[list[Any]]
+        fuzzy: NotRequired[bool]
 
 
 class CommandManager:
     """
     Alconna 命令管理器
 
     命令管理器负责记录命令, 并存储快捷指令。
@@ -43,25 +46,27 @@
 
     sign: str
     current_count: int
     max_count: int
 
     __commands: dict[str, WeakValueDictionary[str, Alconna]]
     __analysers: WeakKeyDictionary[Alconna, Analyser]
+    __argv: WeakKeyDictionary[Alconna, Argv]
     __abandons: list[Alconna]
     __record: LRU[int, Arparma]
     __shortcuts: dict[str, Union[Arparma, ShortcutArgs]]
 
     def __init__(self):
         self.cache_path = f"{__file__.replace('manager.py', '')}manager_cache.db"
         self.sign = "ALCONNA::"
         self.max_count = config.command_max_count
         self.current_count = 0
 
         self.__commands = {}
+        self.__argv = WeakKeyDictionary()
         self.__analysers = WeakKeyDictionary()
         self.__abandons = []
         self.__shortcuts = {}
         self.__record = LRU(config.message_max_cache)
 
         def _del():
             self.__commands.clear()
@@ -105,44 +110,65 @@
             return
         return config.namespaces.get(name)
 
     def register(self, command: Alconna) -> None:
         """注册命令解析器, 会同时记录解析器对应的命令"""
         if self.current_count >= self.max_count:
             raise ExceedMaxCount
+        self.__argv.pop(command, None)
+        self.__argv[command] = Argv(
+            command.namespace_config,
+            fuzzy_match=command.meta.fuzzy_match,
+            to_text=command.namespace_config.to_text,
+            separators=command.separators,
+            message_cache=command.namespace_config.enable_message_cache,
+            filter_crlf=not command.meta.keep_crlf,
+        )
         self.__analysers.pop(command, None)
-        self.__analysers[command] = command.compile()
+        self.__analysers[command] = command.compile(None)
         namespace = self.__commands.setdefault(command.namespace, WeakValueDictionary())
         if _cmd := namespace.get(command.name):
             if _cmd == command:
                 return
             _cmd.formatter.add(command)
             command.formatter = _cmd.formatter
         else:
             command.formatter.add(command)
             namespace[command.name] = command
             self.current_count += 1
 
-    def require(self, command: Alconna) -> Analyser:
+    def resolve(self, command: Alconna[TDataCollection]) -> Argv[TDataCollection]:
+        """获取命令解析器的参数解析器"""
+        try:
+            return self.__argv[command]
+        except KeyError as e:
+            namespace, name = self._command_part(command.path)
+            raise ValueError(lang.manager.undefined_command.format(target=f"{namespace}.{name}")) from e
+
+    def require(self, command: Alconna[TDataCollection]) -> Analyser[TDataCollection]:
         """获取命令解析器"""
         try:
             return self.__analysers[command]  # type: ignore
         except KeyError as e:
             namespace, name = self._command_part(command.path)
             raise ValueError(lang.manager.undefined_command.format(target=f"{namespace}.{name}")) from e
 
-    def requires(self, *paths: str) -> list[Analyser]:
-        return [v for k, v in self.__analysers.items() if k.path in paths]
+    def requires(self, *paths: str) -> zip[tuple[Analyser, Argv]]:  # type: ignore
+        return zip(
+            [v for k, v in self.__analysers.items() if k.path in paths],
+            [v for k, v in self.__argv.items() if k.path in paths],
+        )
 
     def delete(self, command: Alconna | str) -> None:
         """删除命令"""
         namespace, name = self._command_part(command if isinstance(command, str) else command.path)
         try:
             base = self.__commands[namespace][name]
             base.formatter.remove(base)
+            del self.__argv[base]
             del self.__analysers[base]
             del self.__commands[namespace][name]
             self.current_count -= 1
         finally:
             if self.__commands.get(namespace) == {}:
                 del self.__commands[namespace]
             return None
@@ -160,14 +186,15 @@
             self.__abandons.append(command)
 
     def add_shortcut(self, target: Alconna, key: str, source: Arparma | ShortcutArgs):
         """添加快捷命令"""
         namespace, name = self._command_part(target.path)
         if isinstance(source, dict):
             source['command'] = source.get('command', target.command or target.name)
+            source.setdefault('fuzzy', True)
             self.__shortcuts[f"{namespace}.{name}::{key}"] = source
         elif source.matched:
             self.__shortcuts[f"{namespace}.{name}::{key}"] = source
         else:
             raise ValueError(lang.manager.incorrect_shortcut.format(target=f"{key}"))
 
     @overload
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/model.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/output.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Alconna 参数相关"""
 from __future__ import annotations
 
 from typing import TypeVar, Iterator, runtime_checkable, Protocol, Union, Any, Literal, Tuple, Dict, List
 from nepattern import BasePattern, type_parser, MatchMode
 
-THeader = Union[List[Union[str, object]], List[Tuple[object, str]]]
+TPrefixes = Union[List[Union[str, object]], List[Tuple[object, str]]]
 DataUnit = TypeVar("DataUnit", covariant=True)
 
 
 @runtime_checkable
 class DataCollection(Protocol[DataUnit]):
     """数据集合协议"""
     def __repr__(self) -> str: ...
@@ -67,8 +67,8 @@
     def __repr__(self):
         return self.alias
 
 
 Nargs = MultiVar
 Kw = _Kw()
 
-__all__ = ["DataCollection", "TDataCollection", "MultiVar", "Nargs", "Kw", "KeyWordVar", "THeader"]
+__all__ = ["DataCollection", "TDataCollection", "MultiVar", "Nargs", "Kw", "KeyWordVar", "TPrefixes"]
```

### Comparing `arclet-alconna-1.7.0rc2/src/arclet/alconna/util.py` & `arclet-alconna-1.7.0rc3/src/arclet/alconna/util.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc2/PKG-INFO` & `arclet-alconna-1.7.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.0rc2
+Version: 1.7.0rc3
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -75,15 +75,14 @@
 ```
 
 Output as follows:
 ```
 value=None args={'pak_name': 'numpy'} options={'upgrade': value=Ellipsis args={}} subcommands={}
 ```
 
-
 ## Communication
 
 QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 ## Features
 
 * High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
```

