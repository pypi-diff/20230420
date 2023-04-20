# Comparing `tmp/sentry_cli-2.17.3.tar.gz` & `tmp/sentry_cli-2.17.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.17.3.tar", last modified: Wed Apr 19 10:09:30 2023, max compression
+gzip compressed data, was "sentry_cli-2.17.4.tar", last modified: Thu Apr 20 09:59:23 2023, max compression
```

## Comparing `sentry_cli-2.17.3.tar` & `sentry_cli-2.17.4.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/
--rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:29.996271 sentry_cli-2.17.3/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-19 10:09:29.000000 sentry_cli-2.17.3/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-19 10:09:29.000000 sentry_cli-2.17.3/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:09:29.000000 sentry_cli-2.17.3/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:09:29.000000 sentry_cli-2.17.3/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:29.996271 sentry_cli-2.17.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)    87341 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.000271 sentry_cli-2.17.3/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.000271 sentry_cli-2.17.3/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.000271 sentry_cli-2.17.3/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.000271 sentry_cli-2.17.3/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.008271 sentry_cli-2.17.3/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.008271 sentry_cli-2.17.3/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.008271 sentry_cli-2.17.3/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.012271 sentry_cli-2.17.3/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36190 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.657736 sentry_cli-2.17.4/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-20 09:59:23.000000 sentry_cli-2.17.4/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-20 09:59:23.000000 sentry_cli-2.17.4/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:59:23.000000 sentry_cli-2.17.4/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:59:23.000000 sentry_cli-2.17.4/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.657736 sentry_cli-2.17.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    87341 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.657736 sentry_cli-2.17.4/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.657736 sentry_cli-2.17.4/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.665736 sentry_cli-2.17.4/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.665736 sentry_cli-2.17.4/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.665736 sentry_cli-2.17.4/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36190 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.17.3/Cargo.lock` & `sentry_cli-2.17.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2155,51 +2155,51 @@
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "sentry"
-version = "0.29.3"
+version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6f8ce69326daef9d845c3fd17149bd3dbd7caf5dc65dbbad9f5441a40ee407f"
+checksum = "6c3d7f8bf7373e75222452fcdd9347d857452a92d0eec738f941bc4656c5b5df"
 dependencies = [
  "curl",
  "httpdate",
  "sentry-anyhow",
  "sentry-contexts",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-anyhow"
-version = "0.29.3"
+version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a80510663e6b711de2eed521a95dc38435a0e5858397d1acec79185e4a44215b"
+checksum = "9ef7f47c57a1146d553b4976f20e8bba370195a88858bdf6945a63c529549236"
 dependencies = [
  "anyhow",
  "sentry-backtrace",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-backtrace"
-version = "0.29.3"
+version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ed6c0254d4cce319800609aa0d41b486ee57326494802045ff27434fc9a2030"
+checksum = "03b7cdefbdca51f1146f0f24a3cb4ecb6428951f030ff5c720cfb5c60bd174c0"
 dependencies = [
  "backtrace",
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.17.3"
+version = "2.17.4"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
@@ -2261,44 +2261,44 @@
  "which",
  "winapi 0.3.9",
  "zip",
 ]
 
 [[package]]
 name = "sentry-contexts"
-version = "0.29.3"
+version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3277dc5d2812562026f2095c7841f3d61bbe6789159b7da54f41d540787f818"
+checksum = "6af4cb29066e0e8df0cc3111211eb93543ccb09e1ccbe71de6d88b4bb459a2b1"
 dependencies = [
  "hostname",
  "libc",
  "os_info",
  "rustc_version 0.4.0",
  "sentry-core",
  "uname",
 ]
 
 [[package]]
 name = "sentry-core"
-version = "0.29.3"
+version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5acbd3da4255938cf0384b6b140e6c07ff65919c26e4d7a989d8d90ee88fa91"
+checksum = "5e781b55761e47a60d1ff326ae8059de22b0e6b0cee68eab1c5912e4fb199a76"
 dependencies = [
  "once_cell",
  "rand",
  "sentry-types",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "sentry-types"
-version = "0.29.3"
+version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10d8587b12c0b8211bb3066979ee57af6e8657e23cf439dc6c8581fd86de24e8"
+checksum = "d642a04657cc77d8de52ae7c6d93a15cb02284eb219344a89c1e2b26bbaf578c"
 dependencies = [
  "debugid",
  "getrandom",
  "hex",
  "serde",
  "serde_json",
  "thiserror",
```

### Comparing `sentry_cli-2.17.3/Cargo.toml` & `sentry_cli-2.17.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.17.3"
+version = "2.17.4"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
@@ -53,15 +53,15 @@
 proguard = { version = "5.0.0", features = ["uuid"] }
 r2d2 = "0.8.10"
 rayon = "1.6.1"
 regex = "1.7.1"
 runas = "1.0.0"
 rust-ini = "0.18.0"
 semver = "1.0.16"
-sentry = { version = "0.29.3", default-features = false, features = [
+sentry = { version = "0.31.0", default-features = false, features = [
   "anyhow",
   "curl",
   "contexts",
 ] }
 serde = { version = "1.0.152", features = ["derive"] }
 serde_json = "1.0.93"
 sha1_smol = { version = "1.0.0", features = ["serde"] }
```

### Comparing `sentry_cli-2.17.3/LICENSE` & `sentry_cli-2.17.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/PKG-INFO` & `sentry_cli-2.17.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.17.3
+Version: 2.17.4
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.17.3 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.17.4 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.3/README.md` & `sentry_cli-2.17.4/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/build.rs` & `sentry_cli-2.17.4/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.17.4/sentry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-cli
-Version: 2.17.3
+Version: 2.17.4
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.17.3 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.17.4 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.3/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.17.4/sentry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/setup.cfg` & `sentry_cli-2.17.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/setup.py` & `sentry_cli-2.17.4/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/api.rs` & `sentry_cli-2.17.4/src/api.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/bashsupport.sh` & `sentry_cli-2.17.4/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/bash_hook.rs` & `sentry_cli-2.17.4/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.17.4/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.17.4/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/debug_files/check.rs` & `sentry_cli-2.17.4/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/debug_files/find.rs` & `sentry_cli-2.17.4/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/debug_files/mod.rs` & `sentry_cli-2.17.4/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.17.4/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/debug_files/upload.rs` & `sentry_cli-2.17.4/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/deploys/list.rs` & `sentry_cli-2.17.4/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/deploys/mod.rs` & `sentry_cli-2.17.4/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/deploys/new.rs` & `sentry_cli-2.17.4/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/events/list.rs` & `sentry_cli-2.17.4/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/events/mod.rs` & `sentry_cli-2.17.4/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/files/delete.rs` & `sentry_cli-2.17.4/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/files/list.rs` & `sentry_cli-2.17.4/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/files/mod.rs` & `sentry_cli-2.17.4/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/files/upload.rs` & `sentry_cli-2.17.4/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/info.rs` & `sentry_cli-2.17.4/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/issues/mod.rs` & `sentry_cli-2.17.4/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/issues/mute.rs` & `sentry_cli-2.17.4/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/issues/resolve.rs` & `sentry_cli-2.17.4/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/issues/unresolve.rs` & `sentry_cli-2.17.4/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/login.rs` & `sentry_cli-2.17.4/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/mod.rs` & `sentry_cli-2.17.4/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/monitors/list.rs` & `sentry_cli-2.17.4/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/monitors/mod.rs` & `sentry_cli-2.17.4/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/monitors/run.rs` & `sentry_cli-2.17.4/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/organizations/list.rs` & `sentry_cli-2.17.4/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/organizations/mod.rs` & `sentry_cli-2.17.4/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/projects/list.rs` & `sentry_cli-2.17.4/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/projects/mod.rs` & `sentry_cli-2.17.4/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/react_native/appcenter.rs` & `sentry_cli-2.17.4/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/react_native/gradle.rs` & `sentry_cli-2.17.4/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/react_native/mod.rs` & `sentry_cli-2.17.4/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/react_native/xcode.rs` & `sentry_cli-2.17.4/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/releases/archive.rs` & `sentry_cli-2.17.4/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/releases/delete.rs` & `sentry_cli-2.17.4/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/releases/finalize.rs` & `sentry_cli-2.17.4/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/releases/info.rs` & `sentry_cli-2.17.4/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/releases/list.rs` & `sentry_cli-2.17.4/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/releases/mod.rs` & `sentry_cli-2.17.4/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/releases/new.rs` & `sentry_cli-2.17.4/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/releases/restore.rs` & `sentry_cli-2.17.4/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/releases/set_commits.rs` & `sentry_cli-2.17.4/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/repos/list.rs` & `sentry_cli-2.17.4/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/repos/mod.rs` & `sentry_cli-2.17.4/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/send_envelope.rs` & `sentry_cli-2.17.4/src/commands/send_envelope.rs`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             Arg::new("raw")
                 .long("raw")
                 .action(ArgAction::SetTrue)
                 .help("Send envelopes without attempting to parse their contents."),
         )
 }
 
-fn send_raw_envelope(envelope: Envelope, dsn: Dsn) {
+pub fn send_raw_envelope(envelope: Envelope, dsn: Dsn) {
     debug!("{:?}", envelope);
     with_sentry_client(dsn, |c| c.send_envelope(envelope));
 }
 
 pub fn execute(matches: &ArgMatches) -> Result<()> {
     let config = Config::current();
     let dsn = config.get_dsn()?;
```

### Comparing `sentry_cli-2.17.3/src/commands/send_event.rs` & `sentry_cli-2.17.4/src/commands/send_event.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 use std::borrow::Cow;
 use std::env;
-use std::fs::File;
-use std::io::BufReader;
 use std::path::PathBuf;
 use std::time::SystemTime;
 
 use anyhow::{format_err, Result};
 use chrono::{DateTime, Utc};
 use clap::{Arg, ArgAction, ArgMatches, Command};
 use glob::{glob_with, MatchOptions};
 use itertools::Itertools;
 use log::{debug, warn};
 use sentry::protocol::{Event, Level, LogEntry, User};
 use sentry::types::{Dsn, Uuid};
+use sentry::Envelope;
 use serde_json::Value;
 use username::get_user_name;
 
+use crate::commands::send_envelope::send_raw_envelope;
 use crate::config::Config;
 use crate::utils::args::{get_timestamp, validate_distribution};
 use crate::utils::event::{attach_logfile, get_sdk_info, with_sentry_client};
 use crate::utils::releases::detect_release_name;
 
 pub fn make_command(command: Command) -> Command {
     command.about("Send a manual event to Sentry.")
@@ -33,14 +33,20 @@
         .arg(
             Arg::new("path")
                 .value_name("PATH")
                 .required(false)
                 .help("The path or glob to the file(s) in JSON format to send as event(s). When provided, all other arguments are ignored."),
         )
         .arg(
+            Arg::new("raw")
+                .long("raw")
+                .action(ArgAction::SetTrue)
+                .help("Send events using an envelope without attempting to parse their contents."),
+        )
+        .arg(
             Arg::new("level")
                 .value_name("LEVEL")
                 .long("level")
                 .short('l')
                 .help("Optional event severity/log level. (debug|info|warning|error|fatal) [defaults to 'error']"),
         )
         .arg(Arg::new("timestamp")
@@ -157,33 +163,55 @@
     debug!("{:?}", event);
     with_sentry_client(dsn, |c| c.capture_event(event, None))
 }
 
 pub fn execute(matches: &ArgMatches) -> Result<()> {
     let config = Config::current();
     let dsn = config.get_dsn()?;
+    let raw = matches.get_flag("raw");
 
     if let Some(path) = matches.get_one::<String>("path") {
         let collected_paths: Vec<PathBuf> = glob_with(path, MatchOptions::new())
             .unwrap()
             .flatten()
             .collect();
 
         if collected_paths.is_empty() {
             warn!("Did not match any .json files for pattern: {}", path);
             return Ok(());
         }
 
         for path in collected_paths {
-            let p = path.as_path();
-            let file = File::open(p)?;
-            let reader = BufReader::new(file);
-            let event: Event = serde_json::from_reader(reader)?;
-            let id = send_raw_event(event, dsn.clone());
-            println!("Event from file {} dispatched: {}", p.display(), id);
+            let raw_event = std::fs::read(&path)?;
+
+            let id = if raw {
+                use std::io::Write;
+
+                // Its a bit unfortunate that we still need to parse the whole JSON,
+                // but envelopes need an `event_id`, which we also want to report.
+                let json: Value = serde_json::from_slice(&raw_event)?;
+                let id = json
+                    .as_object()
+                    .and_then(|event| event.get("event_id"))
+                    .and_then(|val| val.as_str())
+                    .and_then(|id| Uuid::parse_str(id).ok())
+                    .unwrap_or_default();
+                let mut buf = Vec::new();
+                writeln!(buf, r#"{{"event_id":"{id}"}}"#)?;
+                writeln!(buf, r#"{{"type":"event","length":{}}}"#, raw_event.len())?;
+                buf.extend(raw_event);
+                let envelope = Envelope::from_bytes_raw(buf)?;
+                send_raw_envelope(envelope, dsn.clone());
+                id
+            } else {
+                let event: Event = serde_json::from_slice(&raw_event)?;
+                send_raw_event(event, dsn.clone())
+            };
+
+            println!("Event from file {} dispatched: {}", path.display(), id);
         }
 
         return Ok(());
     }
 
     let mut event = Event {
         sdk: Some(get_sdk_info()),
```

### Comparing `sentry_cli-2.17.3/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.17.4/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.17.4/src/commands/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.17.4/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.17.4/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.17.4/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/uninstall.rs` & `sentry_cli-2.17.4/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/update.rs` & `sentry_cli-2.17.4/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/commands/upload_proguard.rs` & `sentry_cli-2.17.4/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/config.rs` & `sentry_cli-2.17.4/src/config.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/constants.rs` & `sentry_cli-2.17.4/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/android.rs` & `sentry_cli-2.17.4/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/appcenter.rs` & `sentry_cli-2.17.4/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/args.rs` & `sentry_cli-2.17.4/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/chunks.rs` & `sentry_cli-2.17.4/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/codepush.rs` & `sentry_cli-2.17.4/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/cordova.rs` & `sentry_cli-2.17.4/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/dif.rs` & `sentry_cli-2.17.4/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/dif_upload.rs` & `sentry_cli-2.17.4/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/enc.rs` & `sentry_cli-2.17.4/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/event.rs` & `sentry_cli-2.17.4/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/file_search.rs` & `sentry_cli-2.17.4/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/file_upload.rs` & `sentry_cli-2.17.4/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/formatting.rs` & `sentry_cli-2.17.4/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/fs.rs` & `sentry_cli-2.17.4/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/http.rs` & `sentry_cli-2.17.4/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/logging.rs` & `sentry_cli-2.17.4/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/progress.rs` & `sentry_cli-2.17.4/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/releases.rs` & `sentry_cli-2.17.4/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/retry.rs` & `sentry_cli-2.17.4/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.17.4/src/utils/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/sourcemaps.rs` & `sentry_cli-2.17.4/src/utils/sourcemaps.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/system.rs` & `sentry_cli-2.17.4/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/ui.rs` & `sentry_cli-2.17.4/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/update.rs` & `sentry_cli-2.17.4/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/vcs.rs` & `sentry_cli-2.17.4/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.3/src/utils/xcode.rs` & `sentry_cli-2.17.4/src/utils/xcode.rs`

 * *Files identical despite different names*

