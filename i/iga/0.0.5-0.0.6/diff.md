# Comparing `tmp/iga-0.0.5.tar.gz` & `tmp/iga-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-0.0.5.tar", last modified: Tue Apr 11 00:15:28 2023, max compression
+gzip compressed data, was "iga-0.0.6.tar", last modified: Thu Apr 20 01:00:51 2023, max compression
```

## Comparing `iga-0.0.5.tar` & `iga-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-11 00:15:28.032966 iga-0.0.5/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.5/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-11 00:15:28.033045 iga-0.0.5/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    24828 2023-04-06 20:04:04.000000 iga-0.0.5/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-11 00:15:28.030262 iga-0.0.5/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-04-11 00:11:34.000000 iga-0.0.5/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.5/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    31130 2023-04-10 21:10:55.000000 iga-0.0.5/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.5/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.5/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1069 2023-04-07 18:13:39.000000 iga-0.0.5/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.5/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    12795 2023-04-10 21:12:02.000000 iga-0.0.5/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3192 2023-03-28 22:54:00.000000 iga-0.0.5/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14934 2023-04-10 21:13:20.000000 iga-0.0.5/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2054 2023-04-08 02:43:59.000000 iga-0.0.5/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.5/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    68275 2023-04-10 23:14:29.000000 iga-0.0.5/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    13434 2023-04-08 03:10:23.000000 iga-0.0.5/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.5/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.5/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.5/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.5/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-11 00:15:28.031036 iga-0.0.5/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      904 2023-04-11 00:15:28.000000 iga-0.0.5/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-04-11 00:15:27.000000 iga-0.0.5/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-04-11 00:15:28.000000 iga-0.0.5/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-04-11 00:15:28.033381 iga-0.0.5/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.5/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-11 00:15:28.032872 iga-0.0.5/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     5701 2023-04-08 01:24:41.000000 iga-0.0.5/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.5/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.5/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.5/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.5/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.5/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.5/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2149 2023-03-02 15:19:42.000000 iga-0.0.5/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.5/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.5/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    51703 2023-04-07 00:07:41.000000 iga-0.0.5/tests/test_name_parsing.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1821 2023-03-02 23:15:31.000000 iga-0.0.5/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.5/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.5/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.5/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.5/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.5/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-20 01:00:51.687296 iga-0.0.6/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.6/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-20 01:00:51.687407 iga-0.0.6/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    24828 2023-04-20 00:49:26.000000 iga-0.0.6/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-20 01:00:51.656158 iga-0.0.6/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-04-20 01:00:03.000000 iga-0.0.6/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.6/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    31130 2023-04-10 21:10:55.000000 iga-0.0.6/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.6/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.6/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1069 2023-04-07 18:13:39.000000 iga-0.0.6/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.6/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15031 2023-04-20 00:58:38.000000 iga-0.0.6/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3192 2023-03-28 22:54:00.000000 iga-0.0.6/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14934 2023-04-10 21:13:20.000000 iga-0.0.6/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-0.0.6/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.6/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    69392 2023-04-20 00:58:38.000000 iga-0.0.6/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14559 2023-04-20 00:58:38.000000 iga-0.0.6/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.6/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.6/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.6/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.6/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-20 01:00:51.670452 iga-0.0.6/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-04-20 01:00:51.687837 iga-0.0.6/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.6/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-20 01:00:51.687134 iga-0.0.6/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     5732 2023-04-20 00:58:38.000000 iga-0.0.6/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.6/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.6/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.6/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.6/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.6/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.6/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2149 2023-03-02 15:19:42.000000 iga-0.0.6/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.6/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-0.0.6/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.6/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-0.0.6/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-0.0.6/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.6/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.6/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.6/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.6/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.6/tests/test_text_utils.py
```

### Comparing `iga-0.0.5/LICENSE` & `iga-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/PKG-INFO` & `iga-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.5
+Version: 0.0.6
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
```

### Comparing `iga-0.0.5/README.md` & `iga-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/__init__.py` & `iga-0.0.6/iga/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '0.0.5'
+__version__     = '0.0.6'
 __description__ = 'InvenioRDM GitHub Archiver'
 __url__         = 'https://github.com/caltechlibrary/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-0.0.5/iga/__main__.py` & `iga-0.0.6/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/cli.py` & `iga-0.0.6/iga/cli.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/data_utils.py` & `iga-0.0.6/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/doi.py` & `iga-0.0.6/iga/doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/exceptions.py` & `iga-0.0.6/iga/exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/exit_codes.py` & `iga-0.0.6/iga/exit_codes.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/github.py` & `iga-0.0.6/iga/github.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,19 @@
 
 from iga.exceptions import GitHubError, InternalError
 
 
 # Constants.
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-# 2023-03-27 used to include "bot" (no brackets) in this list, but then
-# discovered a real person whose last name is "Bot".
+_BASE_URL = 'https://api.github.com'
+'''Base URL for GitHub's API endpoints.'''
+
+# 2023-03-27 the following used to include "bot" (no brackets) in this list,
+# but then I discovered a real person whose last name is "Bot"!
 
 _BOT_NAME_WORDS = ['daemon', 'dependabot', 'dependabot[bot]']
 '''List of words such that, if one of the words is the last word in an account
 name, mean the account will be assumed to be a software bot of some kind.'''
 
 
 # Classes.
@@ -96,38 +99,38 @@
 
 
 # Exported module functions.
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 def github_release(account_name, repo_name, tag_name):
     '''Return a Release object corresponding to the tagged release in GitHub.'''
-    endpoint = ('https://api.github.com/repos/' + account_name
-                + '/' + repo_name + '/releases/tags/' + tag_name)
+    endpoint = (_BASE_URL + '/repos/' + account_name + '/' + repo_name
+                + '/releases/tags/' + tag_name)
     log('getting GitHub data for release at ' + endpoint)
     result = _object_for_github(endpoint, GitHubRelease)
     if not result:
         raise GitHubError(f'Can\'t get GitHub release data for {tag_name} in'
                           f' repository {repo_name} of account {account_name}')
     return result
 
 
 def github_repo(account_name, repo_name):
     '''Return a Repo object corresponding to the named repo in GitHub.'''
-    endpoint = 'https://api.github.com/repos/' + account_name + '/' + repo_name
+    endpoint = _BASE_URL + '/repos/' + account_name + '/' + repo_name
     log('getting GitHub data for repo at ' + endpoint)
     result = _object_for_github(endpoint, GitHubRepo)
     if not result:
         raise GitHubError('Can\'t get GitHub repository data for'
                           f' {account_name}/{repo_name}')
     return result
 
 
 def github_account(account_name):
     '''Return an Account object corresponding to the GitHub user account.'''
-    endpoint = 'https://api.github.com/users/' + account_name
+    endpoint = _BASE_URL + '/users/' + account_name
     log('getting GitHub data for user at ' + endpoint)
     result = _object_for_github(endpoint, GitHubAccount)
     if not result:
         raise GitHubError(f'Can\'t get GitHub account data for {account_name}')
     return result
 
 
@@ -140,41 +143,86 @@
         assets.append(release.tarball_url)
         for asset in release.assets:
             assets.append(asset.browser_download_url)
     log(f'found {len(assets)} assets for release "{tag_name}"')
     return assets
 
 
-def github_repo_filenames(repo):
-    '''Return a list of file information objects for the given repo object.'''
+def github_repo_filenames(repo, tag_name):
+    '''Return a list of file information objects for the given repo object.
+
+    The tag_name must be a release tag, and is used to find the version of
+    the repository corresponding to that tag.
+    '''
     if getattr(repo, '_filenames', None):
         return repo._filenames
-    log('asking GitHub for list of files at ' + repo.api_url)
-    files_url = repo.api_url + '/git/trees/' + repo.default_branch
-    response = _github_get(files_url)
+
+    # We need to find the SHA for the file tree corresponding to the tag. There
+    # is no direct API, so we have to start by getting info about all the tags.
+    tags_endpoint = repo.api_url + '/git/refs/tags'
+    response = _github_get(tags_endpoint)
+    if not response:
+        log(f'failed to get tags data using {tags_endpoint} – something is wrong')
+        raise GitHubError('Unable to get list of tags for GitHub repository')
+
+    # Next, we look up the specific commit by tag, then get the commit object.
+    for tag_ref in response.json():     # The json in this case is a list.
+        if tag_ref.get('ref', '').endswith(tag_name):
+            tag_commit_url = tag_ref.get('object', {}).get('url', '')
+            break
+    else:
+        log(f'failed to find tag {tag_name} in repo tag refs')
+        return []
+    response = _github_get(tag_commit_url)
+    if not response:
+        log(f'failed to get tag commit {tag_commit_url} – something is wrong')
+        raise GitHubError(f'Unable to get needed GitHub data for release {tag_name}')
+
+    # Next, we have to get the git commit object from that tag object. There
+    # are two cases: one direct, and one with ane extra level of indirection.
+    json_dict = response.json()
+    if 'tree' not in json_dict:
+        # We have to do one more lookup.
+        git_commit_url = json_dict.get('object', {}).get('url', '')
+        response = _github_get(git_commit_url)
+        if not response:
+            log(f'failed to get git commit {git_commit_url} – something is wrong')
+            raise GitHubError(f'Unable to get needed GitHub data for release {tag_name}')
+        json_dict = response.json()
+
+    # Now we can finally get the file tree.
+    tree_url = json_dict.get('tree', {}).get('url')
+    response = _github_get(tree_url)
+    if not response:
+        log(f'failed to get file tree using {tree_url} – something is wrong')
+        raise GitHubError('Unable to get list of files for GitHub repository')
     if not response:
         log(f'did not get a list of file names for {repo}')
         return []
     json_dict = response.json()
     files = [GitHubFile(data) for data in json_dict['tree']]
     log(f'GitHub returned a list of {len(files)} files in repo')
     # Cache the results on the repo object, so we don't have to recompute it.
     repo._files = files
     repo._filenames = [file.path for file in files]
     return repo._filenames
 
 
-def github_repo_file(repo, filename):
-    '''Return the text contents of the named file in the repo object.'''
-    if filename not in github_repo_filenames(repo):
-        log(f'{filename} not found in the files of {repo}')
-        return ''
+def github_repo_file(repo, tag_name, filename):
+    '''Return the text contents of the named file in the repo object.
+
+    The tag_name must be a release tag, and is used to find the version of
+    the repository corresponding to that tag.
+    '''
     if filename in getattr(repo, '_files_contents', {}):
         log(f'{filename} found in the files of {repo}')
         return repo._files_contents[filename]
+    if filename not in github_repo_filenames(repo, tag_name):
+        log(f'{filename} not found in the files of {repo}')
+        return ''
     log(f'getting contents of file {filename} from GitHub repo {repo.full_name}')
     file = next(f for f in repo._files if f.path == filename)
     response = _github_get(file.url)
     if not response:
         log(f'got no content for file {filename} or it does not exist')
         return ''
     json_dict = response.json()
@@ -221,18 +269,19 @@
     return contributors
 
 
 def github_account_repo_tag(release_url):
     '''Return tuple (account, repo name, tag) based on the given web URL.'''
     # Example URL: https://github.com/mhucka/taupe/releases/tag/v1.2.0
     # Note this is not the same as the "release url" below.
-    _, _, _, account, repo, _, _, tag = release_url.split('/')
-    return (account, repo, tag)
+    _, _, _, account_name, repo_name, _, _, tag_name = release_url.split('/')
+    return (account_name, repo_name, tag_name)
 
 
+# FIXME
 def github_file_url(repo, filename):
     '''Return a URL that can be used to download the given file from the repo.'''
     return repo.html_url + '/blob/' + repo.default_branch + '/' + filename
 
 
 def valid_github_release_url(url):
     '''Return True if the given URL appears to be a valid GitHub release URL.'''
@@ -289,15 +338,15 @@
 def _github_get(endpoint):
     headers = {'Accept': 'application/vnd.github.v3+json'}
     using_token = 'GITHUB_TOKEN' in os.environ
     if using_token:
         headers['Authorization'] = f'token {os.environ["GITHUB_TOKEN"]}'
     try:
         response = network('get', endpoint, headers=headers)
-        return response
+        return response                 # noqa PIE787
     except KeyboardInterrupt:
         raise
     except commonpy.exceptions.NoContent:
         log(f'got no content for {endpoint}')
     except commonpy.exceptions.AuthenticationFailure:
         # GitHub is unusual in returning 403 when you hit the rate limit.
         # https://docs.github.com/en/rest/overview/resources-in-the-rest-api
```

### Comparing `iga-0.0.5/iga/id_utils.py` & `iga-0.0.6/iga/id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/invenio.py` & `iga-0.0.6/iga/invenio.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/json_utils.py` & `iga-0.0.6/iga/json_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     JSON, so the result of using this function may be an empty JSON.
     '''
     if skip_line:
         log(f'skipping line {skip_line} in JSON content and retrying')
         # This is an embarrassingly simple-minded approach. Maybe someday we
         # can make something better and more performant, but for now ...
         content = content.split('\n')
-        content = content[:skip_line - 1] + content[skip_line:]
+        content = content[:skip_line - 2] + content[skip_line - 1:]
         content = '\n'.join(content)
     try:
         return dict(dirtyjson.loads(content))
     except KeyboardInterrupt:
         raise
     except dirtyjson.error.Error as ex:
         # Do we have a line number?
```

### Comparing `iga-0.0.5/iga/licenses.py` & `iga-0.0.6/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/metadata.py` & `iga-0.0.6/iga/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,32 +181,32 @@
     repo = github_repo(account_name, repo_name)
     release = github_release(account_name, repo_name, tag)
 
     # We use codemeta.json & CITATION.cff often. Get them now & augment the
     # repo object with them so that field extraction functions can access them.
     repo.codemeta = {}
     repo.cff = {}
-    filenames = github_repo_filenames(repo)
+    filenames = github_repo_filenames(repo, tag)
     if 'codemeta.json' in filenames:
-        codemeta_file = github_repo_file(repo, 'codemeta.json')
+        codemeta_file = github_repo_file(repo, tag, 'codemeta.json')
         try:
             repo.codemeta = json5.loads(codemeta_file)
         except KeyboardInterrupt:
             raise
         except ValueError:
             from iga.json_utils import partial_json
             log('CodeMeta content has syntactic errors; trying alternate parser')
             repo.codemeta = partial_json(codemeta_file)
         except Exception as ex:         # noqa PIE786
             log('ignoring codemeta.json file because of error: ' + str(ex))
     for name in ['CITATION.cff', 'CITATION.CFF', 'citation.cff']:
         if name in filenames:
             import yaml
             try:
-                repo.cff = yaml.safe_load(github_repo_file(repo, name))
+                repo.cff = yaml.safe_load(github_repo_file(repo, tag, name))
             except KeyboardInterrupt:
                 raise
             except Exception as ex:     # noqa PIE786
                 log(f'ignoring {name} file because of error: ' + str(ex))
             break
 
     _load_vocabularies()
@@ -875,14 +875,30 @@
     # indicates the item’s identity." Note that relative to a release stored
     # in InvenioRDM, it is not "same as"; rather it's closer to "a version of".
     # There's no equivalent in CFF or the GitHub repo data structure.
     if sameas_url := repo.codemeta.get('sameAs', ''):
         log('adding CodeMeta "sameAs" to "related_identifiers"')
         identifiers.append(id_dict(sameas_url, 'isversionof', 'software'))
 
+    # CodeMeta's "downloadURL" and CFF's "repository-artifact" are equivalent.
+    # Watch out that CM defines it as one URL, but some people make it a list.
+    if download_url := repo.codemeta.get('downloadUrl', ''):
+        log('adding CodeMeta "downloadUrl" to "related_identifiers"')
+    elif download_url := repo.cff.get('repository-artifact', ''):
+        log('adding CFF "repository-artifact" to "related_identifiers"')
+    for url in filter(validators.url, listified(download_url)):
+        identifiers.append(id_dict(url, 'isvariantformof', 'software'))
+
+    # CodeMeta "installUrl" is often used to point to (when working w/ Python)
+    # the PyPI location for a program. That's basically like downloadUrl.
+    if install_url := listified(repo.codemeta.get('installUrl', '')):
+        log('adding CodeMeta "installUrl" to "related_identifiers"')
+        for url in filter(validators.url, install_url):
+            identifiers.append(id_dict(url, 'isvariantformof', 'software'))
+
     # CodeMeta softwareHelp type is CreativeWork but sometimes people use URLs.
     for help in listified(repo.codemeta.get('softwareHelp', '')):  # noqa A001
         if isinstance(help, str) and validators.url(help):
             url = help
         elif isinstance(help, dict):
             if help_url := help.get('url', ''):
                 url = normalized_url(help_url)
@@ -918,32 +934,32 @@
     # web pages"; however, in the codemeta.json file, we get zero info about
     # what the links are meant to be. Worse, relatedLink has no direct
     # equivalent in the relations CV in InvenioRDM. Since the direction is
     # "this release" --> relatedLink --> "something", the closest relationship
     # term seems to be "references", as in "this release references this link".
     if links := listified(repo.codemeta.get('relatedLink')):
         log('adding CodeMeta "relatedLink" URL value(s) to "related_identifiers"')
-        for url in filter(lambda x: validators.url(x), links):
+        for url in filter(validators.url, links):
             url = normalized_url(url)
             # We don't add URLs we've already added (possibly as another type).
             # The list needs to be recreated in the loop b/c we're adding to it.
             added_urls = [item['identifier'] for item in identifiers]
             # We compare URLs loosely b/c people frequently put https in one
             # place and http in another, or add an extraneous trailing slash.
             if any(similar_urls(url, added) for added in added_urls):
                 continue
             # There's no good way to know what the resource type actually is.
             identifiers.append(id_dict(url, 'references', 'other'))
 
-    # We add CodeMeta & CFF "references" values to InvenioRDM "references" but
-    # formatted as references. Here, add the id's alone.
+    # We add CodeMeta & CFF "references" to InvenioRDM "references" elsewhere
+    # (c.f. function references()). Here we add just the identifiers.
     if reference_ids := _codemeta_reference_ids(repo) | _cff_reference_ids(repo):
         log('adding id\'s of CodeMeta & CFF references to "related_identifiers"')
     for id in reference_ids:            # noqa A001
-        # Adding id's => must recreate the list in this test each iteration.
+        # Adding id's => must recreate the list in the test on each iteration.
         if id not in [detected_id(item['identifier']) for item in identifiers]:
             identifiers.append({'identifier': id,
                                 'relation_type': {'id': 'isreferencedby'},
                                 'scheme': recognized_scheme(id)})
 
     # Final step: remove things that have urls not in our allowed list.
     filtered_identifiers = []
@@ -1036,15 +1052,15 @@
                 rights['description'] = {'en': LICENSES[spdx_id].description}
         return [rights]
     else:
         log('GitHub did not provide license info for this repo')
 
     # GitHub didn't fill in the license info -- maybe it didn't recognize
     # the license or its format. Try to look for a license file ourselves.
-    filenames = github_repo_filenames(repo)
+    filenames = github_repo_filenames(repo, release.tag_name)
     for basename in ['LICENSE', 'License', 'license',
                      'LICENCE', 'Licence', 'licence',
                      'COPYING', 'COPYRIGHT', 'Copyright', 'copyright']:
         for ext in ['', '.txt', '.md', '.html']:
             if basename + ext in filenames:
                 log('found a license file in the repo: "' + basename + ext + '"')
                 # There's no safe way to summarize arbitrary license text,
@@ -1073,16 +1089,16 @@
     subjects = CaseFoldSet()
 
     # Add values from CodeMeta field "keywords". If the whole value is one
     # string, it may contain multiple terms separated by a comma or semicolon.
     if keywords := repo.codemeta.get('keywords', []):
         log('adding CodeMeta "keywords" value(s) to "subjects"')
     if isinstance(keywords, str):
-        # Trying the ';' first, alone, is deliberate in case the values
-        # separated by semicolons have commas within them.
+        # Try the ';' first, alone, before trying ',', in case the values
+        # separated by semicolons are subject terms containing commas.
         if ';' in keywords:
             subjects.update(keywords.split(';'))
         elif ',' in keywords:
             subjects.update(keywords.split(','))
         else:
             subjects.update(keywords.split())
     else:
@@ -1097,19 +1113,15 @@
         log('adding CFF "keywords" value(s) to "subjects"')
     for item in keywords:
         if isinstance(item, str):
             subjects.add(item)
         else:
             log(f'skipping item with unexpected format: {item}')
 
-    # Add languages as topics too.
-    if languages := github_repo_languages(repo):
-        log('adding GitHub repo languages to "subjects"')
-    for lang in languages:
-        subjects.add(lang)
+    # Add the languages listed in the CodeMeta file.
     if cm_langs := listified(repo.codemeta.get('programmingLanguage', [])):
         log('adding CodeMeta "programmingLanguage" value(s) to "subjects"')
     for item in cm_langs:
         if isinstance(item, str):
             subjects.add(item)
         elif isinstance(item, dict):
             if lang := (item.get('name', '') or item.get('@name', '')):
@@ -1119,14 +1131,20 @@
                 ' in codemeta.json: ' + str(item))
             break
 
     if include_all:
         log('adding GitHub topics to "subjects"')
         subjects.update(repo.topics)
 
+        # Add repo languages as topics too.
+        if languages := github_repo_languages(repo):
+            log('adding GitHub repo languages to "subjects"')
+        for lang in languages:
+            subjects.add(lang)
+
     return [{'subject': x} for x in sorted(subjects, key=str.lower)]
 
 
 def title(repo, release, include_all):
     '''Return InvenioRDM "title".
     https://inveniordm.docs.cern.ch/reference/metadata/#title-1
     '''
```

### Comparing `iga-0.0.5/iga/name_utils.py` & `iga-0.0.6/iga/name_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,19 +49,43 @@
     ' — ',                              # em-dash
 }
 '''Items used as part of a filter to rule out person names.'''
 
 _NLP = {}
 '''Cache for the spaCy model so that we don't have to load it more than once.'''
 
-_ORGANIZATIONS = CaseFoldSet()
-'''Set of well-known company names.'''
+_ORGANIZATIONS = {}
+'''Cache for the set of well-known company names.'''
 
-_ORGANIZATIONS_FILENAMES = ['famous-orgs.txt', 'github-orgs.txt']
-'''List of files in iga/data containing organization names.'''
+_ORGANIZATIONS_FILENAME = 'org-names.p'
+'''Pickled CaseFoldSet in iga/data containing organization names.'''
+
+_COMMON_PREFIXES = [
+    '',
+    'Dame',
+    'Dr',
+    'Fr',
+    'Imām',
+    'Lady',
+    'Lord',
+    'Messrs',
+    'Miss',
+    'Mr',
+    'Mrs',
+    'Ms',
+    'Mx',
+    'Pr',
+    'Prof',
+    'Professor',
+    'Rabbi',
+    'Revd',
+    'Roshi',
+    'Sensei',
+    'Sir',
+]
 
 
 # Exported module functions.
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 # https://stackoverflow.com/questions/54334304/spacy-cant-find-model-en-core-web-sm-on-windows-10-and-python-3-5-3-anacon
 # import spacy.cli
@@ -198,50 +222,67 @@
         log('treating single name as the family name')
         given = ''
         surname = name
     else:
         try:
             log('trying to split name using probablepeople')
             import probablepeople as pp
-            from_pp = pp.tag(name)
+
             # PP gets better results if you DON'T supply the 'type' parameter.
-            # (I don't know why.) Use that 1st, unless it guesses wrong about
-            # the type, in which case, we run it again using type=person.
-            if from_pp[1] != 'Person':
-                from_pp = pp.tag(_cleaned_name(name), type='person')
+            # (I don't know why.) Try it that way first, let it guess the type,
+            # and if it guesses wrong, try it again but with the type that time.
+            from_pp = pp.tag(name)
+            log(f'probablepeople initial result: {str(from_pp)}')
+            guessed_type = from_pp[1]
+            guessed_prefix = from_pp[0].get('PrefixOther', '')
+            has_bad_prefix = guessed_prefix not in _COMMON_PREFIXES
+            has_corp_key = any(key.startswith('Corp') for key in from_pp[0].keys())
+            if guessed_type != 'Person' or has_bad_prefix or has_corp_key:
+                from_pp = pp.tag(name, type='person')
+                log(f'probablepeople 2nd result: {str(from_pp)}')
+                guessed_prefix = from_pp[0].get('PrefixOther', '')
+                if guessed_prefix not in _COMMON_PREFIXES:
+                    # This is a sign something is still wrong. Give up on PP.
+                    raise Exception
             parsed = from_pp[0]
+
             # If it found initials instead of full names, use those.
-            if parsed.get('FirstInitial', ''):
+            if parsed.get('FirstInitial'):
                 given = parsed.get('FirstInitial')
             else:
                 # Get rid of periods at the end, in case someone got cute.
                 given = parsed.get('GivenName', '').rstrip('.')
 
-            # For some reason, it seems the InvenioRDM records include the
-            # middle names as part of the first/given names, so:
-            if parsed.get('MiddleInitial', ''):
-                given += (' ' + parsed.get('MiddleInitial'))
-            elif parsed.get('MiddleName', ''):
-                given += (' ' + parsed.get('MiddleName'))
-
-            if parsed.get('LastInitial', '') and not parsed.get('Surname', ''):
-                surname = parsed.get('LastInitial').title()
+            # InvenioRDM wants middle names to be part of the first/given names:
+            if middle := (parsed.get('MiddleInitial') or parsed.get('MiddleName')):
+                given += (' ' + middle)
+
+            # If we only have a last initial, then that's all we can use.
+            if parsed.get('LastInitial') and not parsed.get('Surname'):
+                surname = parsed.get('LastInitial', '').title()
             else:
                 surname = parsed.get('Surname', '')
+
+            # If we didn't find a given name but the surname has a space, use
+            # it as a split point & take all but last word as the given name.
+            if not given and ' ' in surname:
+                split = surname.split(' ')
+                surname = split.pop()
+                given = ' '.join(split)
         except KeyboardInterrupt:
             raise
         except Exception:                   # noqa: PIE786
             log(f'switching to nameparser b/c probablepeople failed on "{name}"')
             from nameparser import HumanName
             parsed = HumanName(name)
             # (Noted above) InvenioRDM includes middle name as part of 1st name:
             given = parsed.first + ' ' + parsed.middle
             surname = parsed.last
 
-    given = _upcase_first_letters(given)
+    given = _first_letters_upcased(given)
     if _plain_word(surname):
         surname = surname.title()
     surname = surname.strip()
 
     log(f'final name splitting result: ({given}, {surname})')
     return (given, surname)
 
@@ -289,28 +330,28 @@
 def _plain_word(name):
     return (' ' not in name
             and not any(str.isdigit(c) for c in name)
             and (all(str.isupper(c) for c in name)
                  or not any(str.isupper(c) for c in name[1:])))
 
 
-def _upcase_first_letters(name):
+def _first_letters_upcased(name):
     # Python's .title() will downcase the letters after the 1st letter, which
     # is undesired behavior for the situation where we need this.
     return ' '.join(word[0].upper() + word[1:] for word in name.split())
 
 
 def _load_organizations():
+    global _ORGANIZATIONS
     from os.path import dirname, abspath, join
+    import pickle
+    log(f'loading data/{_ORGANIZATIONS_FILENAME} – this may take some time')
     here = dirname(abspath(__file__))
-    for file in _ORGANIZATIONS_FILENAMES:
-        log(f'loading data/{file} – this may take a little while')
-        with open(join(here, f'data/{file}'), 'r') as f:
-            for line in f.readlines():
-                _ORGANIZATIONS.add(_cleaned_name(line))
+    with open(join(here, f'data/{_ORGANIZATIONS_FILENAME}'), 'rb') as f:
+        _ORGANIZATIONS = pickle.load(f)
 
 
 def _load_spacy(charset):
     global _NLP
     import spacy
     model = 'zh_core_web_trf' if charset == 'cjk' else 'en_core_web_trf'
     try:
```

### Comparing `iga-0.0.5/iga/orcid.py` & `iga-0.0.6/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/reference.py` & `iga-0.0.6/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/ror.py` & `iga-0.0.6/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga/text_utils.py` & `iga-0.0.6/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/iga.egg-info/PKG-INFO` & `iga-0.0.6/iga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.5
+Version: 0.0.6
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
```

### Comparing `iga-0.0.5/iga.egg-info/SOURCES.txt` & `iga-0.0.6/iga.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 tests/test_doi.py
 tests/test_exceptions.py
 tests/test_exit_codes.py
 tests/test_github.py
 tests/test_github_mocks.py
 tests/test_id_utils.py
 tests/test_init.py
+tests/test_is_person.py
 tests/test_licenses.py
-tests/test_name_parsing.py
+tests/test_name_splitting.py
 tests/test_name_utils.py
 tests/test_orcid.py
 tests/test_record_from_codemeta.py
 tests/test_reference.py
 tests/test_ror.py
 tests/test_text_utils.py
```

### Comparing `iga-0.0.5/iga.egg-info/requires.txt` & `iga-0.0.6/iga.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/setup.cfg` & `iga-0.0.6/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 0.0.5
+version = 0.0.6
 description = InvenioRDM GitHub Archiver
 author = Michael Hucka
 author_email = helpdesk@library.caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-0.0.5/setup.py` & `iga-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_cli.py` & `iga-0.0.6/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,31 +36,31 @@
         return GitHubAccount(json5.loads(f.read()))
 
 
 def mocked_github_repo(account_name, repo_name):
     log(f'returing mocked GitHubRepo for {repo_name}')
     with open(path.join(repo_dir, 'repo.json'), 'r') as f:
         repo = GitHubRepo(json5.loads(f.read()))
-        repo._files = mocked_github_repo_filenames(repo_name)
+        repo._files = mocked_github_repo_filenames(repo_name, 'faketag')
         return repo
 
 
 def mocked_github_release(account_name, repo_name, tag_name):
     log(f'returing mocked GitHubRelease for {tag_name}')
     with open(path.join(repo_dir, 'release.json'), 'r') as f:
         return GitHubRelease(json5.loads(f.read()))
 
 
-def mocked_github_repo_filenames(repo):
+def mocked_github_repo_filenames(repo, tag_name):
     log('returing mocked filenames list')
     with open(path.join(repo_dir, 'filenames.json'), 'r') as f:
         return json5.loads(f.read())
 
 
-def mocked_github_repo_file(repo, filename):
+def mocked_github_repo_file(repo, tag_name, filename):
     log(f'returing mocked file contents for {filename}')
     with open(path.join(repo_dir, filename), 'r') as f:
         return f.read()
 
 
 def mocked_github_repo_contributors(repo):
     log('returing mocked contributors')
```

### Comparing `iga-0.0.5/tests/test_data_utils.py` & `iga-0.0.6/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_doi.py` & `iga-0.0.6/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_exceptions.py` & `iga-0.0.6/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_github.py` & `iga-0.0.6/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_github_mocks.py` & `iga-0.0.6/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_id_utils.py` & `iga-0.0.6/tests/test_id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_init.py` & `iga-0.0.6/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_licenses.py` & `iga-0.0.6/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_name_parsing.py` & `iga-0.0.6/tests/test_is_person.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # =============================================================================
-# @file    test_name_parsing.py
-# @brief   Py.test cases for parts of record.py
+# @file    test_is_person.py
+# @brief   Py.test cases for parts of name_utils.py
 # @created 2022-12-23
 # @license Please see the file named LICENSE in the project directory
 # @website https://github.com/caltechlibrary/iga
 # =============================================================================
 
 from collections import namedtuple
 from iga.name_utils import (
     split_name,
     is_person,
 )
 
-# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Name = namedtuple('Name', 'first last')
-
 # Some of these names came from the following gist accessed on 2023-01-17:
 # https://gist.github.com/paulmillr/2657075/a31455729440672467ada20ac10452d74a871e54
 
 # Some real-life examples that we can't handle.
 #
 # * Ingy döt Net -- someone being cute, but it's not a real name
 #
@@ -41,58 +37,14 @@
 # companies is to *always* ignore PP's tag if it comes out as company
 # -- which means we always fail on these:
 #
 # * Account for Github research
 # * Practical Arduino - The Book
 # * Sony Xperia Developer World
 
-PARSED_NAMES = [
-    ('Mike Hucka', Name(first='Mike', last='Hucka')),
-    ('Rafael França', Name(first='Rafael', last='França')),
-    ('Wladimir J. van der Laan', Name(first='Wladimir J.', last='van der Laan')),
-    ('Iuri de Silvio', Name(first='Iuri', last='de Silvio')),
-    ('Ian Storm Taylor', Name(first='Ian Storm', last='Taylor')),
-    ("Matthew Weier O'Phinney", Name(first='Matthew', last="Weier O'Phinney")),
-    ('Martin Luther King, Jr.', Name(first='Martin Luther', last='King')),
-    ('J. Robert Oppenheimer', Name(first='J. Robert', last='Oppenheimer')),
-    ('Lukas Kahwe Smith', Name(first='Lukas Kahwe', last='Smith')),
-    ('Philip (flip) Kromer', Name(first='Philip', last='Kromer')),
-    ('Weibin Yao(姚伟斌)', Name(first='Weibin', last='Yao')),
-    ('Dr Nic Williams', Name(first='Nic', last='Williams')),
-    ('cho45', Name(first='', last='cho45')),
-    ('王爵nice', Name(first='', last='Nice')),
-    ('TZ | 天猪', Name(first='', last='Tz')),
-    ('TJ Holowaychuk', Name(first='TJ', last='Holowaychuk')),
-    ('PatrickJS [tipe.io]', Name(first='', last='PatrickJS')),
-    ('Mu-An ✌️ Chiou', Name(first='Mu-An', last='Chiou')),
-    ('Jean-Jacques Rousseau', Name(first='Jean-Jacques', last='Rousseau')),
-    ('Jose Diaz-Gonzalez', Name(first='Jose', last='Diaz-Gonzalez')),
-    ('Miguel de Val-Borro', Name(first='Miguel', last='de Val-Borro')),
-    ('Carla Rodriguez de García', Name(first='Carla', last='Rodriguez de García')),
-    ('R. Tyler Croy', Name(first='R. Tyler', last='Croy')),
-    ('Mr.doob', Name(first='', last='Doob')),
-    ('Yukihiro &quot;Matz&quot; Matsumoto', Name(first='Yukihiro', last='Matsumoto')),
-    ("Adam 'Atomic' Saltsman", Name(first='Adam', last='Saltsman')),
-    ('Andrey “A.I” Sitnik', Name(first='Andrey', last='Sitnik')),
-    ("Ching-Lan 'digdog' HUANG 黃 青嵐", Name(first='Ching-Lan', last='Huang')),
-    ('Fuji, Goro', Name(first='Fuji', last='Goro')),
-    ('Christian Van Der Henst S.', Name(first='Christian', last='Van Der Henst S.')),
-    ('R.I.Pienaar', Name(first='R. I.', last='Pienaar')),
-    ('ara.t.howard', Name(first='Ara T.', last='Howard')),
-    # ('', Name(first='', last='')),
-]
-
-
-def test_name_parsing():
-    for original, parsed in PARSED_NAMES:
-        (first, last) = split_name(original)
-        assert first == parsed.first
-        assert last == parsed.last
-
-
 PEOPLE = [
     "Martin Luther King, Jr.",
     "Yihui Xie",
     "José Valim",
     "Kevin Sawicki",
     "Jordan Sissel",
     "Alon Zakai",
```

### Comparing `iga-0.0.5/tests/test_name_utils.py` & `iga-0.0.6/tests/test_name_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @license Please see the file named LICENSE in the project directory
 # @website https://github.com/caltechlibrary/iga
 # =============================================================================
 
 from iga.name_utils import (
     _cleaned_name,
     _plain_word,
-    _upcase_first_letters,
+    _first_letters_upcased,
     contains_cjk,
     flattened_name,
 )
 
 RAW_NAMES = [
     ('偏右', ''),
     ('王爵nice', 'nice'),
@@ -47,14 +47,14 @@
     assert _plain_word('FOO')
     assert _plain_word('Foo')
     assert not _plain_word('foo bar')
     assert not _plain_word('foo1')
 
 
 def test_upcase_first_letter():
-    assert _upcase_first_letters('aBC dEF') == 'ABC DEF'
-    assert _upcase_first_letters('Abc Def') == 'Abc Def'
-    assert _upcase_first_letters('abc def') == 'Abc Def'
-    assert _upcase_first_letters('abc DEF') == 'Abc DEF'
-    assert _upcase_first_letters('abc dEF') == 'Abc DEF'
-    assert _upcase_first_letters('a') == 'A'
-    assert _upcase_first_letters('A') == 'A'
+    assert _first_letters_upcased('aBC dEF') == 'ABC DEF'
+    assert _first_letters_upcased('Abc Def') == 'Abc Def'
+    assert _first_letters_upcased('abc def') == 'Abc Def'
+    assert _first_letters_upcased('abc DEF') == 'Abc DEF'
+    assert _first_letters_upcased('abc dEF') == 'Abc DEF'
+    assert _first_letters_upcased('a') == 'A'
+    assert _first_letters_upcased('A') == 'A'
```

### Comparing `iga-0.0.5/tests/test_orcid.py` & `iga-0.0.6/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_record_from_codemeta.py` & `iga-0.0.6/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_reference.py` & `iga-0.0.6/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_ror.py` & `iga-0.0.6/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.5/tests/test_text_utils.py` & `iga-0.0.6/tests/test_text_utils.py`

 * *Files identical despite different names*

