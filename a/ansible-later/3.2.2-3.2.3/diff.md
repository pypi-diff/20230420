# Comparing `tmp/ansible_later-3.2.2.tar.gz` & `tmp/ansible_later-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_later-3.2.2.tar", max compression
+gzip compressed data, was "ansible_later-3.2.3.tar", max compression
```

## Comparing `ansible_later-3.2.2.tar` & `ansible_later-3.2.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1123 2023-04-03 08:49:14.098684 ansible_later-3.2.2/LICENSE
--rw-r--r--   0        0        0     3173 2023-04-03 08:49:14.098684 ansible_later-3.2.2/README.md
--rw-r--r--   0        0        0      120 2023-04-03 08:49:30.486751 ansible_later-3.2.2/ansiblelater/__init__.py
--rwxr-xr-x   0        0        0     2892 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/__main__.py
--rw-r--r--   0        0        0     9843 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/candidate.py
--rw-r--r--   0        0        0      666 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/exceptions.py
--rw-r--r--   0        0        0     5180 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/logger.py
--rw-r--r--   0        0        0      834 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckBecomeUser.py
--rw-r--r--   0        0        0     1636 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckBracesSpaces.py
--rw-r--r--   0        0        0     2345 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckChangedInWhen.py
--rw-r--r--   0        0        0     1079 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckCommandHasChanges.py
--rw-r--r--   0        0        0     2650 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckCommandInsteadOfArgument.py
--rw-r--r--   0        0        0     1895 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckCommandInsteadOfModule.py
--rw-r--r--   0        0        0     1227 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckCompareToEmptyString.py
--rw-r--r--   0        0        0     1229 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckCompareToLiteralBool.py
--rw-r--r--   0        0        0      952 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckDeprecated.py
--rw-r--r--   0        0        0     3764 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckFilePermissionMissing.py
--rw-r--r--   0        0        0     3105 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckFilePermissionOctal.py
--rw-r--r--   0        0        0     1156 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckFilterSeparation.py
--rw-r--r--   0        0        0     1920 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckGitHasVersion.py
--rw-r--r--   0        0        0     1162 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckInstallUseLatest.py
--rw-r--r--   0        0        0      941 2023-04-03 08:49:14.098684 ansible_later-3.2.2/ansiblelater/rules/CheckLiteralBoolFormat.py
--rw-r--r--   0        0        0      737 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckLocalAction.py
--rw-r--r--   0        0        0     1182 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckMetaChangeFromDefault.py
--rw-r--r--   0        0        0     1201 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckMetaMain.py
--rw-r--r--   0        0        0      892 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckNameFormat.py
--rw-r--r--   0        0        0      897 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckNamedTask.py
--rw-r--r--   0        0        0     1679 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckNativeYaml.py
--rw-r--r--   0        0        0     2179 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckNestedJinja.py
--rw-r--r--   0        0        0     1235 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckRelativeRolePaths.py
--rw-r--r--   0        0        0      700 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckScmInSrc.py
--rw-r--r--   0        0        0     1321 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckShellInsteadCommand.py
--rw-r--r--   0        0        0     1601 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckTaskSeparation.py
--rw-r--r--   0        0        0      904 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckUniqueNamedTask.py
--rw-r--r--   0        0        0      590 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckVersion.py
--rw-r--r--   0        0        0      891 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckWhenFormat.py
--rw-r--r--   0        0        0      518 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckYamlColons.py
--rw-r--r--   0        0        0      517 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckYamlDocumentEnd.py
--rw-r--r--   0        0        0      525 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckYamlDocumentStart.py
--rw-r--r--   0        0        0      524 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckYamlEmptyLines.py
--rw-r--r--   0        0        0      684 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckYamlFile.py
--rw-r--r--   0        0        0      627 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckYamlHasContent.py
--rw-r--r--   0        0        0      521 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckYamlHyphens.py
--rw-r--r--   0        0        0      526 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/rules/CheckYamlIndent.py
--rw-r--r--   0        0        0     7899 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/settings.py
--rw-r--r--   0        0        0    11321 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/standard.py
--rw-r--r--   0        0        0        0 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/test/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/test/unit/__init__.py
--rw-r--r--   0        0        0     2337 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/test/unit/test_logger.py
--rw-r--r--   0        0        0      527 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/test/unit/test_settings.py
--rw-r--r--   0        0        0     2475 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/utils/__init__.py
--rw-r--r--   0        0        0    19003 2023-04-03 08:49:14.102684 ansible_later-3.2.2/ansiblelater/utils/yamlhelper.py
--rw-r--r--   0        0        0     3488 2023-04-03 08:49:30.474751 ansible_later-3.2.2/pyproject.toml
--rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 ansible_later-3.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-04-20 07:50:50.803852 ansible_later-3.2.3/LICENSE
+-rw-r--r--   0        0        0     3173 2023-04-20 07:50:50.803852 ansible_later-3.2.3/README.md
+-rw-r--r--   0        0        0      120 2023-04-20 07:51:04.080358 ansible_later-3.2.3/ansiblelater/__init__.py
+-rwxr-xr-x   0        0        0     2892 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/__main__.py
+-rw-r--r--   0        0        0     9843 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/candidate.py
+-rw-r--r--   0        0        0      666 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/exceptions.py
+-rw-r--r--   0        0        0     5180 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/logger.py
+-rw-r--r--   0        0        0      834 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckBecomeUser.py
+-rw-r--r--   0        0        0     1636 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckBracesSpaces.py
+-rw-r--r--   0        0        0     2345 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckChangedInWhen.py
+-rw-r--r--   0        0        0     1079 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCommandHasChanges.py
+-rw-r--r--   0        0        0     2650 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCommandInsteadOfArgument.py
+-rw-r--r--   0        0        0     2031 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCommandInsteadOfModule.py
+-rw-r--r--   0        0        0     1227 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCompareToEmptyString.py
+-rw-r--r--   0        0        0     1229 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCompareToLiteralBool.py
+-rw-r--r--   0        0        0      952 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckDeprecated.py
+-rw-r--r--   0        0        0     3764 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckFilePermissionMissing.py
+-rw-r--r--   0        0        0     3105 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckFilePermissionOctal.py
+-rw-r--r--   0        0        0     1156 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckFilterSeparation.py
+-rw-r--r--   0        0        0     1920 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckGitHasVersion.py
+-rw-r--r--   0        0        0     1162 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckInstallUseLatest.py
+-rw-r--r--   0        0        0      941 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckLiteralBoolFormat.py
+-rw-r--r--   0        0        0      737 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckLocalAction.py
+-rw-r--r--   0        0        0     1182 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckMetaChangeFromDefault.py
+-rw-r--r--   0        0        0     1201 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckMetaMain.py
+-rw-r--r--   0        0        0      892 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckNameFormat.py
+-rw-r--r--   0        0        0      897 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckNamedTask.py
+-rw-r--r--   0        0        0     1679 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckNativeYaml.py
+-rw-r--r--   0        0        0     2179 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckNestedJinja.py
+-rw-r--r--   0        0        0     1235 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckRelativeRolePaths.py
+-rw-r--r--   0        0        0      700 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckScmInSrc.py
+-rw-r--r--   0        0        0     1064 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckShellInsteadCommand.py
+-rw-r--r--   0        0        0     1601 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckTaskSeparation.py
+-rw-r--r--   0        0        0      904 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckUniqueNamedTask.py
+-rw-r--r--   0        0        0      590 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckVersion.py
+-rw-r--r--   0        0        0      891 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckWhenFormat.py
+-rw-r--r--   0        0        0      518 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlColons.py
+-rw-r--r--   0        0        0      517 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlDocumentEnd.py
+-rw-r--r--   0        0        0      525 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlDocumentStart.py
+-rw-r--r--   0        0        0      524 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlEmptyLines.py
+-rw-r--r--   0        0        0      684 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlFile.py
+-rw-r--r--   0        0        0      627 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlHasContent.py
+-rw-r--r--   0        0        0      521 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlHyphens.py
+-rw-r--r--   0        0        0      526 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlIndent.py
+-rw-r--r--   0        0        0     7899 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/settings.py
+-rw-r--r--   0        0        0    11943 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/standard.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/test/unit/__init__.py
+-rw-r--r--   0        0        0     2337 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/test/unit/test_logger.py
+-rw-r--r--   0        0        0      527 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/test/unit/test_settings.py
+-rw-r--r--   0        0        0     2475 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/utils/__init__.py
+-rw-r--r--   0        0        0    19003 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/utils/yamlhelper.py
+-rw-r--r--   0        0        0     3475 2023-04-20 07:51:04.080358 ansible_later-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 ansible_later-3.2.3/PKG-INFO
```

### Comparing `ansible_later-3.2.2/LICENSE` & `ansible_later-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/README.md` & `ansible_later-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/__main__.py` & `ansible_later-3.2.3/ansiblelater/__main__.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/candidate.py` & `ansible_later-3.2.3/ansiblelater/candidate.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/exceptions.py` & `ansible_later-3.2.3/ansiblelater/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/logger.py` & `ansible_later-3.2.3/ansiblelater/logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckBecomeUser.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckBecomeUser.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckBracesSpaces.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckBracesSpaces.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckChangedInWhen.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckChangedInWhen.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckCommandHasChanges.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckCommandHasChanges.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckCommandInsteadOfArgument.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckCommandInsteadOfArgument.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckCommandInsteadOfModule.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckCommandInsteadOfModule.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,17 +35,20 @@
         }
 
         if not errors:
             for task in tasks:
                 if task["action"]["__ansible_module__"] in commands:
                     first_cmd_arg = self.get_first_cmd_arg(task)
                     executable = os.path.basename(first_cmd_arg)
+                    cmd = cmd = self.get_safe_cmd(task)
+
                     if (
                         first_cmd_arg and executable in modules
                         and task["action"].get("warn", True) and "register" not in task
+                        and not any(ch in cmd for ch in self.SHELL_PIPE_CHARS)
                     ):
                         errors.append(
                             self.Error(
                                 task["__line__"],
                                 self.helptext.format(exec=executable, module=modules[executable])
                             )
                         )
```

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckCompareToEmptyString.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckCompareToEmptyString.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckCompareToLiteralBool.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckCompareToLiteralBool.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckDeprecated.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckDeprecated.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckFilePermissionMissing.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckFilePermissionMissing.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckFilePermissionOctal.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckFilePermissionOctal.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckFilterSeparation.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckFilterSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckGitHasVersion.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckGitHasVersion.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckInstallUseLatest.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckInstallUseLatest.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckLiteralBoolFormat.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckLiteralBoolFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckLocalAction.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckLocalAction.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckMetaChangeFromDefault.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckMetaChangeFromDefault.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckMetaMain.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckMetaMain.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckNameFormat.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckNameFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckNamedTask.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckNativeYaml.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckNativeYaml.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckNestedJinja.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckNestedJinja.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckRelativeRolePaths.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckRelativeRolePaths.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckScmInSrc.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckScmInSrc.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckShellInsteadCommand.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckShellInsteadCommand.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import re
-
 from ansiblelater.standard import StandardBase
 
 
 class CheckShellInsteadCommand(StandardBase):
 
     sid = "ANSIBLE0010"
     description = "Shell should only be used when essential"
@@ -18,17 +16,12 @@
             for task in tasks:
                 if task["action"]["__ansible_module__"] == "shell":
                     # skip processing if args.executable is used as this
                     # parameter is no longer support by command module
                     if "executable" in task["action"]:
                         continue
 
-                    if "cmd" in task["action"]:
-                        cmd = task["action"].get("cmd", [])
-                    else:
-                        cmd = " ".join(task["action"].get("__ansible_arguments__", []))
-
-                    unjinja = re.sub(r"\{\{[^\}]*\}\}", "JINJA_VAR", cmd)
-                    if not any(ch in unjinja for ch in "&|<>;$\n*[]{}?"):
+                    cmd = self.get_safe_cmd(task)
+                    if not any(ch in cmd for ch in self.SHELL_PIPE_CHARS):
                         errors.append(self.Error(task["__line__"], self.helptext))
 
         return self.Result(candidate.path, errors)
```

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckTaskSeparation.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckTaskSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckUniqueNamedTask.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckUniqueNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckVersion.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckVersion.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckWhenFormat.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckWhenFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckYamlColons.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckYamlColons.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckYamlDocumentEnd.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckYamlDocumentEnd.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckYamlDocumentStart.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckYamlDocumentStart.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckYamlEmptyLines.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckYamlEmptyLines.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckYamlFile.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckYamlFile.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckYamlHasContent.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckYamlHasContent.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckYamlHyphens.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckYamlHyphens.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/rules/CheckYamlIndent.py` & `ansible_later-3.2.3/ansiblelater/rules/CheckYamlIndent.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/settings.py` & `ansible_later-3.2.3/ansiblelater/settings.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/standard.py` & `ansible_later-3.2.3/ansiblelater/standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import importlib
 import inspect
 import os
 import pathlib
 import re
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
+from urllib.parse import urlparse
 
 import toolz
 import yaml
 from yamllint import linter
 from yamllint.config import YamlLintConfig
 
 from ansiblelater.exceptions import LaterAnsibleError, LaterError
@@ -40,14 +41,16 @@
 
 class StandardExtendedMeta(StandardMeta, ABCMeta):
     pass
 
 
 class StandardBase(metaclass=StandardExtendedMeta):
 
+    SHELL_PIPE_CHARS = "&|<>;$\n*[]{}?"
+
     @property
     @abstractmethod
     def sid(self):
         pass
 
     @abstractmethod
     def check(self, candidate, settings):
@@ -242,14 +245,30 @@
         elif "argv" in task["action"]:
             first_cmd_arg = task["action"]["argv"][0]
         else:
             first_cmd_arg = task["action"]["__ansible_arguments__"][0]
 
         return first_cmd_arg
 
+    @staticmethod
+    def get_safe_cmd(task):
+        if "cmd" in task["action"]:
+            cmd = task["action"].get("cmd", "")
+        else:
+            cmd = " ".join(task["action"].get("__ansible_arguments__", []))
+
+        cmd = re.sub(r"{{.+?}}", "JINJA_EXPRESSION", cmd)
+        cmd = re.sub(r"{%.+?%}", "JINJA_STATEMENT", cmd)
+        cmd = re.sub(r"{#.+?#}", "JINJA_COMMENT", cmd)
+
+        parts = cmd.split()
+        parts = [p if not urlparse(p.strip('"').strip("'")).scheme else "URL" for p in parts]
+
+        return " ".join(parts)
+
     class Error:
         """Default error object created if a rule failed."""
 
         def __init__(self, lineno, message, **kwargs):
             """
             Initialize a new error object and returns None.
```

### Comparing `ansible_later-3.2.2/ansiblelater/test/unit/test_logger.py` & `ansible_later-3.2.3/ansiblelater/test/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/test/unit/test_settings.py` & `ansible_later-3.2.3/ansiblelater/test/unit/test_settings.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/utils/__init__.py` & `ansible_later-3.2.3/ansiblelater/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/ansiblelater/utils/yamlhelper.py` & `ansible_later-3.2.3/ansiblelater/utils/yamlhelper.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.2/pyproject.toml` & `ansible_later-3.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 license = "MIT"
 name = "ansible-later"
 packages = [
   {include = "ansiblelater"},
 ]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/ansible-later/"
-version = "3.2.2"
+version = "3.2.3"
 
 [tool.poetry.dependencies]
 PyYAML = "6.0"
 ansible = {version = "7.4.0", optional = true}
 ansible-core = {version = "2.14.4", optional = true}
 anyconfig = "0.13.0"
 appdirs = "1.4.4"
@@ -52,28 +52,28 @@
 ansible = ["ansible"]
 ansible-core = ["ansible-core"]
 
 [tool.poetry.scripts]
 ansible-later = "ansiblelater.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.0.260"
-pytest = "7.2.2"
+ruff = "0.0.261"
+pytest = "7.3.1"
 pytest-mock = "3.10.0"
 pytest-cov = "4.0.0"
 toml = "0.10.2"
 yapf = "0.32.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
 
 [tool.pytest.ini_options]
-addopts = "ansiblelater --cov=ansiblelater --cov-report=xml:coverage.xml --cov-report=term --cov-append --no-cov-on-fail"
+addopts = "ansiblelater --cov=ansiblelater --cov-report=xml:coverage.xml --cov-report=term --no-cov-on-fail"
 filterwarnings = [
   "ignore::FutureWarning",
   "ignore::DeprecationWarning",
   "ignore:.*pep8.*:FutureWarning",
 ]
 
 [tool.coverage.run]
```

### Comparing `ansible_later-3.2.2/PKG-INFO` & `ansible_later-3.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-later
-Version: 3.2.2
+Version: 3.2.3
 Summary: Reviews ansible playbooks, roles and inventories and suggests improvements.
 Home-page: https://ansible-later.geekdocs.de/
 License: MIT
 Keywords: ansible,code,review
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.9.0,<4.0.0
```

