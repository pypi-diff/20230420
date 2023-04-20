# Comparing `tmp/rugosa-0.7.1.tar.gz` & `tmp/rugosa-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rugosa-0.7.1.tar", last modified: Wed Mar  1 13:04:16 2023, max compression
+gzip compressed data, was "rugosa-0.7.2.tar", last modified: Thu Apr 20 21:37:34 2023, max compression
```

## Comparing `rugosa-0.7.1.tar` & `rugosa-0.7.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.436585 rugosa-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-03-01 13:04:04.000000 rugosa-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-01 13:04:04.000000 rugosa-0.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-01 13:04:04.000000 rugosa-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-01 13:04:16.436585 rugosa-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-01 13:04:04.000000 rugosa-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.396586 rugosa-0.7.1/rugosa/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/disassembly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.404585 rugosa-0.7.1/rugosa/emulation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.408586 rugosa-0.7.1/rugosa/emulation/ARM/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/ARM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/ARM/instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)   106639 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/ARM/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/ARM/operands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/ARM/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/ARM/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.408586 rugosa-0.7.1/rugosa/emulation/call_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.408586 rugosa-0.7.1/rugosa/emulation/call_hooks/stdlib/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/stdlib/libc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.408586 rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/advapi32.py
--rw-r--r--   0 runner    (1001) docker     (123)    18628 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/kernel32.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/shell32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/shlwapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/win_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/ws2_32.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25677 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/cpu_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    37394 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/flowchart.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    27380 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/operands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.412586 rugosa-0.7.1/rugosa/emulation/x86_64/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/x86_64/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/x86_64/fpu_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/x86_64/instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    79547 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/x86_64/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/x86_64/operands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/emulation/x86_64/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/func_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/function_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.412586 rugosa-0.7.1/rugosa/ghidra_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.424585 rugosa-0.7.1/rugosa/ghidra_plugin/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/call_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/function_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/operands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/components/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.424585 rugosa-0.7.1/rugosa/ghidra_plugin/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/gui/context_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/gui/error_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/gui/mouse_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/gui/program_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/gui/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.384586 rugosa-0.7.1/rugosa/ghidra_plugin/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.428585 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/EmulatorForm.form
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/EmulatorForm.java
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/GoToListingAction.java
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaActionListener.java
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaChangeListener.java
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaComponentProvider.java
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaContextMenuEntry.java
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaDockingAction.java
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaPlugin.java
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaProgramListener.java
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaTabbedPane.java
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaTask.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.432585 rugosa-0.7.1/rugosa/ida_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.436585 rugosa-0.7.1/rugosa/ida_plugin/components/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/call_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/function_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/operands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/components/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.436585 rugosa-0.7.1/rugosa/ida_plugin/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/gui/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/rugosa.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/ida_plugin/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/re.py
--rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-03-01 13:04:04.000000 rugosa-0.7.1/rugosa/yara.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.400586 rugosa-0.7.1/rugosa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-01 13:04:16.000000 rugosa-0.7.1/rugosa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-01 13:04:16.000000 rugosa-0.7.1/rugosa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 13:04:16.000000 rugosa-0.7.1/rugosa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-01 13:04:16.000000 rugosa-0.7.1/rugosa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-01 13:04:16.000000 rugosa-0.7.1/rugosa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-01 13:04:16.000000 rugosa-0.7.1/rugosa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-01 13:04:16.440585 rugosa-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-01 13:04:04.000000 rugosa-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:04:16.436585 rugosa-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-03-01 13:04:04.000000 rugosa-0.7.1/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-01 13:04:04.000000 rugosa-0.7.1/tests/test_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-03-01 13:04:04.000000 rugosa-0.7.1/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-01 13:04:04.000000 rugosa-0.7.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-01 13:04:04.000000 rugosa-0.7.1/tests/test_yara.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.111405 rugosa-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-20 21:37:23.000000 rugosa-0.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-20 21:37:23.000000 rugosa-0.7.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 21:37:23.000000 rugosa-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-20 21:37:34.111405 rugosa-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-20 21:37:23.000000 rugosa-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.067406 rugosa-0.7.2/rugosa/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/disassembly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.075405 rugosa-0.7.2/rugosa/emulation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.075405 rugosa-0.7.2/rugosa/emulation/ARM/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/ARM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/ARM/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106639 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/ARM/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/ARM/operands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/ARM/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/ARM/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.075405 rugosa-0.7.2/rugosa/emulation/call_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.079405 rugosa-0.7.2/rugosa/emulation/call_hooks/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/stdlib/libc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.083406 rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/advapi32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18628 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/kernel32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/shell32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/shlwapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/win_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/ws2_32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25677 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/cpu_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37394 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/flowchart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27380 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/operands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.091405 rugosa-0.7.2/rugosa/emulation/x86_64/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/x86_64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/x86_64/fpu_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/x86_64/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78477 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/x86_64/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/x86_64/operands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/emulation/x86_64/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/func_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/function_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.091405 rugosa-0.7.2/rugosa/ghidra_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.095405 rugosa-0.7.2/rugosa/ghidra_plugin/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/call_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/function_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/operands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/components/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.095405 rugosa-0.7.2/rugosa/ghidra_plugin/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/gui/context_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/gui/error_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/gui/mouse_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/gui/program_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/gui/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.059405 rugosa-0.7.2/rugosa/ghidra_plugin/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.099405 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/EmulatorForm.form
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/EmulatorForm.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/GoToListingAction.java
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaActionListener.java
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaChangeListener.java
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaComponentProvider.java
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaContextMenuEntry.java
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaDockingAction.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaPlugin.java
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaProgramListener.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaTabbedPane.java
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaTask.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.099405 rugosa-0.7.2/rugosa/ida_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.111405 rugosa-0.7.2/rugosa/ida_plugin/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/call_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/function_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/operands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/components/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.111405 rugosa-0.7.2/rugosa/ida_plugin/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/gui/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/rugosa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/ida_plugin/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-20 21:37:23.000000 rugosa-0.7.2/rugosa/yara.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.067406 rugosa-0.7.2/rugosa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-20 21:37:34.000000 rugosa-0.7.2/rugosa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-20 21:37:34.000000 rugosa-0.7.2/rugosa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:37:34.000000 rugosa-0.7.2/rugosa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 21:37:34.000000 rugosa-0.7.2/rugosa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-20 21:37:34.000000 rugosa-0.7.2/rugosa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 21:37:34.000000 rugosa-0.7.2/rugosa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 21:37:34.115405 rugosa-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 21:37:23.000000 rugosa-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:34.111405 rugosa-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-20 21:37:23.000000 rugosa-0.7.2/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 21:37:23.000000 rugosa-0.7.2/tests/test_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-20 21:37:23.000000 rugosa-0.7.2/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-20 21:37:23.000000 rugosa-0.7.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-20 21:37:23.000000 rugosa-0.7.2/tests/test_yara.py
```

### Comparing `rugosa-0.7.1/CHANGELOG.md` & `rugosa-0.7.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 
+## [0.7.2] - 2023-04-19
+- Fixed implementation of `div` opcode.
+
+
 ## [0.7.1] - 2023-02-21
 - Fixed emulation of floating point opcodes.
 - Fixed bug in Ghidra plugin setup handling.
 
 
 ## [0.7.0] - 2023-01-26
 - Add `movsq` opcode support (@ddash-ct)
@@ -95,15 +99,16 @@
 
 
 ## 0.1.0 - 2022-02-04
 - Initial release.
 - Migrated the majority of Kordesii functionality to work with Dragodis.
 
 
-[Unreleased]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.7.1...HEAD
+[Unreleased]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.7.2...HEAD
+[0.7.2]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.7.1...0.7.2
 [0.7.1]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.7.0...0.7.1
 [0.7.0]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.6.1...0.7.0
 [0.6.1]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.6.0...0.6.1
 [0.6.0]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.5.1...0.6.0
 [0.5.1]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.5.0...0.5.1
 [0.5.0]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.4.0...0.5.0
 [0.4.0]: https://github.com/dod-cyber-crime-center/rugosa/compare/0.3.0...0.4.0
```

### Comparing `rugosa-0.7.1/LICENSE.txt` & `rugosa-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/PKG-INFO` & `rugosa-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rugosa
-Version: 0.7.1
+Version: 0.7.2
 Summary: The next generation of kordesii. This is a library for managing emulation and provides utilities for interfacing with decompiled malware samples using dragodis.
 Home-page: https://github.com/Defense-Cyber-Crime-Center/rugosa
 Author: DC3
 License: MIT
 Keywords: malware,ida,ghidra,emulation,strings
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rugosa-0.7.1/README.md` & `rugosa-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/disassembly.py` & `rugosa-0.7.2/rugosa/disassembly.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/ARM/__init__.py` & `rugosa-0.7.2/rugosa/emulation/ARM/__init__.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/ARM/instruction.py` & `rugosa-0.7.2/rugosa/emulation/ARM/instruction.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/ARM/opcodes.py` & `rugosa-0.7.2/rugosa/emulation/ARM/opcodes.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/ARM/operands.py` & `rugosa-0.7.2/rugosa/emulation/ARM/operands.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/ARM/registers.py` & `rugosa-0.7.2/rugosa/emulation/ARM/registers.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/ARM/utils.py` & `rugosa-0.7.2/rugosa/emulation/ARM/utils.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/actions.py` & `rugosa-0.7.2/rugosa/emulation/actions.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/call_hooks/__init__.py` & `rugosa-0.7.2/rugosa/emulation/call_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/call_hooks/stdlib/libc.py` & `rugosa-0.7.2/rugosa/emulation/call_hooks/stdlib/libc.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/advapi32.py` & `rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/advapi32.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/kernel32.py` & `rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/kernel32.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/shell32.py` & `rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/shell32.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/shlwapi.py` & `rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/shlwapi.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/win_constants.py` & `rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/win_constants.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/call_hooks/win_api/ws2_32.py` & `rugosa-0.7.2/rugosa/emulation/call_hooks/win_api/ws2_32.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/constants.py` & `rugosa-0.7.2/rugosa/emulation/constants.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/cpu_context.py` & `rugosa-0.7.2/rugosa/emulation/cpu_context.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/emulator.py` & `rugosa-0.7.2/rugosa/emulation/emulator.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/flowchart.py` & `rugosa-0.7.2/rugosa/emulation/flowchart.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/functions.py` & `rugosa-0.7.2/rugosa/emulation/functions.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/instruction.py` & `rugosa-0.7.2/rugosa/emulation/instruction.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/memory.py` & `rugosa-0.7.2/rugosa/emulation/memory.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/objects.py` & `rugosa-0.7.2/rugosa/emulation/objects.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/operands.py` & `rugosa-0.7.2/rugosa/emulation/operands.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/registers.py` & `rugosa-0.7.2/rugosa/emulation/registers.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/registry.py` & `rugosa-0.7.2/rugosa/emulation/registry.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/utils.py` & `rugosa-0.7.2/rugosa/emulation/utils.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/variables.py` & `rugosa-0.7.2/rugosa/emulation/variables.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/x86_64/__init__.py` & `rugosa-0.7.2/rugosa/emulation/x86_64/__init__.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/x86_64/fpu_opcodes.py` & `rugosa-0.7.2/rugosa/emulation/x86_64/fpu_opcodes.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/x86_64/instruction.py` & `rugosa-0.7.2/rugosa/emulation/x86_64/instruction.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/x86_64/opcodes.py` & `rugosa-0.7.2/rugosa/emulation/x86_64/opcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,110 +385,77 @@
     if cpu_context.emulator.branch_tracking:
         cpu_context.jcccontext.update_flag_opnds(["af", "zf", "sf", "of", "pf"], operands)
 
     logger.debug("0x%X - 1 = 0x%X", opvalue1, result)
     operands[0].value = result & mask
 
 
-@opcode
-def DIV(cpu_context: ProcessorContext, instruction: Instruction):
-    """
-    Divide
-
-    rax / op1 -> rax (rdx holds remainder)
-    """
-    RAX_REG_SIZE_MAP = {8: "rax", 4: "eax", 2: "ax", 1: "al"}
-    RDX_REG_SIZE_MAP = {8: "rdx", 4: "edx", 2: "dx"}
-
-    operands = instruction.operands
-    divisor = operands[0].value
-    width = operands[0].width
-    if divisor == 0:
-        # Log the instruction for a DIV / 0 error
-        logger.debug("DIV / 0")
-        return
-
-    # We actually need to do some doctoring with DIV as operand 0 is implied as the EAX register of
-    # a certain size.
-    rax_str = RAX_REG_SIZE_MAP[width]
-    dividend = cpu_context.registers[rax_str]
-
-    result = (dividend // divisor) & utils.get_mask(width)
-    remainder = (dividend % divisor) & utils.get_mask(width)
-    logger.debug("0x%X / 0x%X = 0x%X", dividend, divisor, result)
-    if width == 1:
-        # Result stored in AL, remainder stored in AH
-        cpu_context.registers.al = result
-        cpu_context.registers.ah = remainder
-    else:
-        rdx_str = RDX_REG_SIZE_MAP[width]
-        cpu_context.registers[rax_str] = result
-        cpu_context.registers[rdx_str] = remainder
-
-
-@opcode
-def IDIV(cpu_context: ProcessorContext, instruction: Instruction):
-    """
-    Signed Division
-    """
+@opcode("div")
+@opcode("idiv")
+def _div(cpu_context: ProcessorContext, instruction: Instruction):
+    signed = instruction.mnem == "idiv"
     RAX_REG_SIZE_MAP = {8: "rax", 4: "eax", 2: "ax", 1: "al"}
     RDX_REG_SIZE_MAP = {8: "rdx", 4: "edx", 2: "dx"}
 
     operands = instruction.operands
     # Need to obtain the width of the divisor, to determine the width of the dividend
     width = operands[-1].width
-    divisor = utils.signed(operands[-1].value, width)
+    divisor = operands[-1].value
+    if signed:
+        divisor = utils.signed(divisor, width)
     if divisor == 0:
         logger.debug("DIV / 0")
         return
 
     if width == 1:
         # When dividing by a 8-bit value, use AX
-        dividend = utils.signed(cpu_context.registers.ax, 2)
+        dividend = cpu_context.registers.ax
+        if signed:
+            dividend = utils.signed(dividend, 2)
         result_reg = "al"
         remainder_reg = "ah"
 
     else:
         # When dividing by 16-bits -> combine DX:AX
         # When dividing by 32-bits -> combine EDX:EAX
         # When dividing by 64-bits -> combine RDX:RAX
         rax_str = RAX_REG_SIZE_MAP[width]
         rdx_str = RDX_REG_SIZE_MAP[width]
-        dividend = utils.signed(
-            (cpu_context.registers[rdx_str] << (width * 8)) | cpu_context.registers[rax_str],
-            width * 2
-        )
+        dividend = (cpu_context.registers[rdx_str] << (width * 8)) | cpu_context.registers[rax_str]
+        if signed:
+            dividend = utils.signed(dividend, width * 2)
         result_reg = rax_str
         remainder_reg = rdx_str
 
-    result = int(dividend / divisor) & utils.get_mask(width)
-    remainder = (dividend - (int(dividend / divisor) * divisor)) & utils.get_mask(width)
-    logger.debug("0x%X / 0x%X = 0x%X", dividend, divisor, result)
+    result = (dividend // divisor) & utils.get_mask(width)
+    remainder = (dividend % divisor) & utils.get_mask(width)
+    logger.debug("0x%X / 0x%X = 0x%X R 0x%X", dividend, divisor, result, remainder)
+
     cpu_context.registers[result_reg] = result
     cpu_context.registers[remainder_reg] = remainder
 
 
 @opcode
 def DIVSD(cpu_context: ProcessorContext, instruction: Instruction):
     """
     Divide Scalar Double-Precision Floating-Point Value
 
     op1 / op2 -> op1
     """
     operands = instruction.operands
-    opvalue1 = utils.int_to_float(operands[0].value)
-    opvalue2 = utils.int_to_float(operands[1].value)
+    dividend = utils.int_to_float(operands[0].value)
+    divisor = utils.int_to_float(operands[1].value)
     # Because there is no guarantee that the registers/memory have been properly initialized, ignore DIV / 0 errors.
-    if opvalue2 == 0:
+    if divisor == 0:
         # Log DIV / 0 error
         logger.debug("DIV / 0")
         return
 
-    result = opvalue1 // opvalue2
-    logger.debug("0x%X / 0x%X = 0x%X", opvalue1, opvalue2, result)
+    result = dividend / divisor
+    logger.debug("%f / %f = %f", dividend, divisor, result)
     result = utils.float_to_int(result)
     operands[0].value = result
 
 
 def _mul(cpu_context: ProcessorContext, instruction: Instruction):
     """
     Handle MUL instruction and 1-operand IMUL instruction as the same.
```

### Comparing `rugosa-0.7.1/rugosa/emulation/x86_64/operands.py` & `rugosa-0.7.2/rugosa/emulation/x86_64/operands.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/emulation/x86_64/registers.py` & `rugosa-0.7.2/rugosa/emulation/x86_64/registers.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/func_utils.py` & `rugosa-0.7.2/rugosa/func_utils.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/components/actions.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/components/actions.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/components/call_history.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/components/call_history.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/components/emulator.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/components/emulator.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/components/function_arguments.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/components/function_arguments.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/components/memory.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/components/memory.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/components/operands.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/components/operands.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/components/registers.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/components/registers.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/components/stdout.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/components/stdout.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/components/variables.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/components/variables.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/gui/context_menu.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/gui/context_menu.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/gui/error_msg.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/gui/error_msg.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/gui/mouse_listener.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/gui/mouse_listener.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/gui/program_listener.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/gui/program_listener.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/gui/table.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/gui/table.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/install.py` & `rugosa-0.7.2/rugosa/ghidra_plugin/install.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/EmulatorForm.form` & `rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/EmulatorForm.form`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/EmulatorForm.java` & `rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/EmulatorForm.java`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/GoToListingAction.java` & `rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/GoToListingAction.java`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaComponentProvider.java` & `rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaComponentProvider.java`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaContextMenuEntry.java` & `rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaContextMenuEntry.java`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaPlugin.java` & `rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaPlugin.java`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ghidra_plugin/java/plugin/RugosaTabbedPane.java` & `rugosa-0.7.2/rugosa/ghidra_plugin/java/plugin/RugosaTabbedPane.java`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/components/actions.py` & `rugosa-0.7.2/rugosa/ida_plugin/components/actions.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/components/call_history.py` & `rugosa-0.7.2/rugosa/ida_plugin/components/call_history.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/components/emulator.py` & `rugosa-0.7.2/rugosa/ida_plugin/components/emulator.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/components/function_arguments.py` & `rugosa-0.7.2/rugosa/ida_plugin/components/function_arguments.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/components/memory.py` & `rugosa-0.7.2/rugosa/ida_plugin/components/memory.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/components/operands.py` & `rugosa-0.7.2/rugosa/ida_plugin/components/operands.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/components/registers.py` & `rugosa-0.7.2/rugosa/ida_plugin/components/registers.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/components/stdout.py` & `rugosa-0.7.2/rugosa/ida_plugin/components/stdout.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/components/variables.py` & `rugosa-0.7.2/rugosa/ida_plugin/components/variables.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/gui/emulator.py` & `rugosa-0.7.2/rugosa/ida_plugin/gui/emulator.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/install.py` & `rugosa-0.7.2/rugosa/ida_plugin/install.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/plugin.py` & `rugosa-0.7.2/rugosa/ida_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/ida_plugin/util.py` & `rugosa-0.7.2/rugosa/ida_plugin/util.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/re.py` & `rugosa-0.7.2/rugosa/re.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/strings.py` & `rugosa-0.7.2/rugosa/strings.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa/yara.py` & `rugosa-0.7.2/rugosa/yara.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/rugosa.egg-info/PKG-INFO` & `rugosa-0.7.2/rugosa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rugosa
-Version: 0.7.1
+Version: 0.7.2
 Summary: The next generation of kordesii. This is a library for managing emulation and provides utilities for interfacing with decompiled malware samples using dragodis.
 Home-page: https://github.com/Defense-Cyber-Crime-Center/rugosa
 Author: DC3
 License: MIT
 Keywords: malware,ida,ghidra,emulation,strings
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rugosa-0.7.1/rugosa.egg-info/SOURCES.txt` & `rugosa-0.7.2/rugosa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/setup.cfg` & `rugosa-0.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/tests/test_issues.py` & `rugosa-0.7.2/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/tests/test_strings.py` & `rugosa-0.7.2/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/tests/test_utils.py` & `rugosa-0.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rugosa-0.7.1/tests/test_yara.py` & `rugosa-0.7.2/tests/test_yara.py`

 * *Files identical despite different names*

