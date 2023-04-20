# Comparing `tmp/xllabelme-5.1.4.tar.gz` & `tmp/xllabelme-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xllabelme-5.1.4.tar", last modified: Fri Apr 14 09:39:52 2023, max compression
+gzip compressed data, was "xllabelme-5.1.5.tar", last modified: Thu Apr 20 12:48:18 2023, max compression
```

## Comparing `xllabelme-5.1.4.tar` & `xllabelme-5.1.5.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.746422 xllabelme-5.1.4/
--rw-rw-rw-   0        0        0      707 2020-11-09 02:22:17.000000 xllabelme-5.1.4/LICENSE
--rw-rw-rw-   0        0        0       19 2020-08-05 08:41:43.000000 xllabelme-5.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0    11738 2023-04-14 09:39:52.745425 xllabelme-5.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     9202 2022-04-20 05:38:39.000000 xllabelme-5.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.659174 xllabelme-5.1.4/docs/
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.665365 xllabelme-5.1.4/docs/man/
--rw-rw-rw-   0        0        0     2148 2020-08-05 08:41:43.000000 xllabelme-5.1.4/docs/man/labelme.1
--rw-rw-rw-   0        0        0       42 2023-04-14 09:39:52.746422 xllabelme-5.1.4/setup.cfg
--rw-rw-rw-   0        0        0     5290 2023-04-04 11:32:18.000000 xllabelme-5.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.674341 xllabelme-5.1.4/xllabelme/
--rw-rw-rw-   0        0        0     1072 2023-04-14 09:39:50.000000 xllabelme-5.1.4/xllabelme/__init__.py
--rw-rw-rw-   0        0        0     7419 2023-04-13 14:13:41.000000 xllabelme-5.1.4/xllabelme/__main__.py
--rw-rw-rw-   0        0        0    78177 2023-04-14 09:19:03.000000 xllabelme-5.1.4/xllabelme/app.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.683909 xllabelme-5.1.4/xllabelme/cli/
--rw-rw-rw-   0        0        0      129 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/cli/__init__.py
--rw-rw-rw-   0        0        0     1404 2022-04-20 05:42:00.000000 xllabelme-5.1.4/xllabelme/cli/draw_json.py
--rw-rw-rw-   0        0        0      667 2021-06-08 03:21:06.000000 xllabelme-5.1.4/xllabelme/cli/draw_label_png.py
--rw-rw-rw-   0        0        0     2473 2022-04-20 05:42:14.000000 xllabelme-5.1.4/xllabelme/cli/json_to_dataset.py
--rw-rw-rw-   0        0        0     2851 2022-04-20 05:42:22.000000 xllabelme-5.1.4/xllabelme/cli/on_docker.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.686904 xllabelme-5.1.4/xllabelme/config/
--rw-rw-rw-   0        0        0     2784 2021-06-08 03:21:07.000000 xllabelme-5.1.4/xllabelme/config/__init__.py
--rw-rw-rw-   0        0        0     2320 2023-04-04 02:59:12.000000 xllabelme-5.1.4/xllabelme/config/default_config.yaml
--rw-rw-rw-   0        0        0    48869 2023-04-14 09:20:52.000000 xllabelme-5.1.4/xllabelme/config/xllabellib.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.725477 xllabelme-5.1.4/xllabelme/icons/
--rw-rw-rw-   0        0        0     2136 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/cancel.png
--rw-rw-rw-   0        0        0     3111 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/close.png
--rw-rw-rw-   0        0        0     2368 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/color-line.png
--rw-rw-rw-   0        0        0     1461 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/color.png
--rw-rw-rw-   0        0        0      646 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/copy.png
--rw-rw-rw-   0        0        0     1486 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/delete.png
--rw-rw-rw-   0        0        0     2198 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/done.png
--rw-rw-rw-   0        0        0    22632 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/done.svg
--rw-rw-rw-   0        0        0     1092 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/edit.png
--rw-rw-rw-   0        0        0     7718 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/expert.png
--rw-rw-rw-   0        0        0     1264 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/eye.png
--rw-rw-rw-   0        0        0     8059 2019-01-15 04:29:26.000000 xllabelme-5.1.4/xllabelme/icons/feBlend-icon.png
--rw-rw-rw-   0        0        0      765 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/file.png
--rw-rw-rw-   0        0        0     1365 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/fit-width.png
--rw-rw-rw-   0        0        0     1102 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/fit-window.png
--rw-rw-rw-   0        0        0     2262 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/fit.png
--rw-rw-rw-   0        0        0     1587 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/help.png
--rw-rw-rw-   0        0        0   183198 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/icon.ico
--rw-rw-rw-   0        0        0    44771 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/icon.png
--rw-rw-rw-   0        0        0    38362 2023-04-04 10:35:02.000000 xllabelme-5.1.4/xllabelme/icons/icon2.ico
--rw-rw-rw-   0        0        0    34213 2023-04-04 10:24:55.000000 xllabelme-5.1.4/xllabelme/icons/icon2.png
--rw-rw-rw-   0        0        0     2381 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/labels.png
--rw-rw-rw-   0        0        0    37512 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/labels.svg
--rw-rw-rw-   0        0        0      977 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/new.png
--rw-rw-rw-   0        0        0    30288 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/next.png
--rw-rw-rw-   0        0        0     1103 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/objects.png
--rw-rw-rw-   0        0        0     2073 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/open.png
--rw-rw-rw-   0        0        0    18773 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/open.svg
--rw-rw-rw-   0        0        0    30665 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/prev.png
--rw-rw-rw-   0        0        0     1915 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/quit.png
--rw-rw-rw-   0        0        0     2811 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/save-as.png
--rw-rw-rw-   0        0        0    65363 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/save-as.svg
--rw-rw-rw-   0        0        0     1187 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/save.png
--rw-rw-rw-   0        0        0    31292 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/save.svg
--rw-rw-rw-   0        0        0     2004 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/undo-cross.png
--rw-rw-rw-   0        0        0     2018 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/undo.png
--rw-rw-rw-   0        0        0     1099 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/zoom-in.png
--rw-rw-rw-   0        0        0     1074 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/zoom-out.png
--rw-rw-rw-   0        0        0     1139 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/zoom.png
--rw-rw-rw-   0        0        0     7004 2023-04-13 14:18:20.000000 xllabelme-5.1.4/xllabelme/label_file.py
--rw-rw-rw-   0        0        0     1907 2023-03-31 08:56:10.000000 xllabelme-5.1.4/xllabelme/logger.py
--rw-rw-rw-   0        0        0     9649 2022-04-26 01:24:19.000000 xllabelme-5.1.4/xllabelme/shape.py
--rw-rw-rw-   0        0        0      886 2021-06-08 03:21:06.000000 xllabelme-5.1.4/xllabelme/testing.py
--rw-rw-rw-   0        0        0    44799 2023-04-04 12:30:43.000000 xllabelme-5.1.4/xllabelme/ts.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.730464 xllabelme-5.1.4/xllabelme/utils/
--rw-rw-rw-   0        0        0      749 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/utils/__init__.py
--rw-rw-rw-   0        0        0      698 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/utils/_io.py
--rw-rw-rw-   0        0        0     2468 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/utils/image.py
--rw-rw-rw-   0        0        0     6290 2023-04-04 09:31:32.000000 xllabelme-5.1.4/xllabelme/utils/qt.py
--rw-rw-rw-   0        0        0     3764 2021-06-08 03:21:06.000000 xllabelme-5.1.4/xllabelme/utils/shape.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.744428 xllabelme-5.1.4/xllabelme/widgets/
--rw-rw-rw-   0        0        0      554 2022-04-20 05:44:54.000000 xllabelme-5.1.4/xllabelme/widgets/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-03-31 14:44:05.000000 xllabelme-5.1.4/xllabelme/widgets/brightness_contrast_dialog.py
--rw-rw-rw-   0        0        0    35438 2023-03-31 14:49:37.000000 xllabelme-5.1.4/xllabelme/widgets/canvas.py
--rw-rw-rw-   0        0        0     1231 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/widgets/color_dialog.py
--rw-rw-rw-   0        0        0      290 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/widgets/escapable_qlist_widget.py
--rw-rw-rw-   0        0        0     2451 2023-03-24 09:08:22.000000 xllabelme-5.1.4/xllabelme/widgets/file_dialog_preview.py
--rw-rw-rw-   0        0        0    19741 2022-10-24 08:25:25.000000 xllabelme-5.1.4/xllabelme/widgets/label_dialog.py
--rw-rw-rw-   0        0        0     6194 2023-03-31 08:45:59.000000 xllabelme-5.1.4/xllabelme/widgets/label_list_widget.py
--rw-rw-rw-   0        0        0      998 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/widgets/tool_bar.py
--rw-rw-rw-   0        0        0     1666 2023-03-31 08:47:05.000000 xllabelme-5.1.4/xllabelme/widgets/unique_label_qlist_widget.py
--rw-rw-rw-   0        0        0      735 2023-04-04 11:11:05.000000 xllabelme-5.1.4/xllabelme/widgets/zoom_widget.py
--rw-rw-rw-   0        0        0    11756 2023-04-14 09:15:35.000000 xllabelme-5.1.4/xllabelme/xlapp.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.679327 xllabelme-5.1.4/xllabelme.egg-info/
--rw-rw-rw-   0        0        0    11738 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      281 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      116 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.285127 xllabelme-5.1.5/
+-rw-rw-rw-   0        0        0      707 2020-11-09 02:22:17.000000 xllabelme-5.1.5/LICENSE
+-rw-rw-rw-   0        0        0       19 2020-08-05 08:41:43.000000 xllabelme-5.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    11738 2023-04-20 12:48:18.285127 xllabelme-5.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9202 2022-04-20 05:38:39.000000 xllabelme-5.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.212321 xllabelme-5.1.5/docs/
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.217308 xllabelme-5.1.5/docs/man/
+-rw-rw-rw-   0        0        0     2148 2020-08-05 08:41:43.000000 xllabelme-5.1.5/docs/man/labelme.1
+-rw-rw-rw-   0        0        0       42 2023-04-20 12:48:18.286124 xllabelme-5.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     5290 2023-04-20 12:13:49.000000 xllabelme-5.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.224289 xllabelme-5.1.5/xllabelme/
+-rw-rw-rw-   0        0        0     1074 2023-04-20 12:48:16.000000 xllabelme-5.1.5/xllabelme/__init__.py
+-rw-rw-rw-   0        0        0     7602 2023-04-18 02:03:52.000000 xllabelme-5.1.5/xllabelme/__main__.py
+-rw-rw-rw-   0        0        0    78564 2023-04-20 11:53:57.000000 xllabelme-5.1.5/xllabelme/app.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.232268 xllabelme-5.1.5/xllabelme/cli/
+-rw-rw-rw-   0        0        0      129 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/cli/__init__.py
+-rw-rw-rw-   0        0        0     1404 2022-04-20 05:42:00.000000 xllabelme-5.1.5/xllabelme/cli/draw_json.py
+-rw-rw-rw-   0        0        0      667 2021-06-08 03:21:06.000000 xllabelme-5.1.5/xllabelme/cli/draw_label_png.py
+-rw-rw-rw-   0        0        0     2473 2022-04-20 05:42:14.000000 xllabelme-5.1.5/xllabelme/cli/json_to_dataset.py
+-rw-rw-rw-   0        0        0     2851 2022-04-20 05:42:22.000000 xllabelme-5.1.5/xllabelme/cli/on_docker.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.234263 xllabelme-5.1.5/xllabelme/config/
+-rw-rw-rw-   0        0        0     2784 2021-06-08 03:21:07.000000 xllabelme-5.1.5/xllabelme/config/__init__.py
+-rw-rw-rw-   0        0        0     2340 2023-04-16 08:40:27.000000 xllabelme-5.1.5/xllabelme/config/default_config.yaml
+-rw-rw-rw-   0        0        0    54316 2023-04-20 11:30:13.000000 xllabelme-5.1.5/xllabelme/config/xllabellib.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.272162 xllabelme-5.1.5/xllabelme/icons/
+-rw-rw-rw-   0        0        0     2136 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/cancel.png
+-rw-rw-rw-   0        0        0     3111 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/close.png
+-rw-rw-rw-   0        0        0     2368 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/color-line.png
+-rw-rw-rw-   0        0        0     1461 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/color.png
+-rw-rw-rw-   0        0        0      646 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/copy.png
+-rw-rw-rw-   0        0        0     1486 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/delete.png
+-rw-rw-rw-   0        0        0     2198 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/done.png
+-rw-rw-rw-   0        0        0    22632 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/done.svg
+-rw-rw-rw-   0        0        0     1092 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/edit.png
+-rw-rw-rw-   0        0        0     7718 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/expert.png
+-rw-rw-rw-   0        0        0     1264 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/eye.png
+-rw-rw-rw-   0        0        0     8059 2019-01-15 04:29:26.000000 xllabelme-5.1.5/xllabelme/icons/feBlend-icon.png
+-rw-rw-rw-   0        0        0      765 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/file.png
+-rw-rw-rw-   0        0        0     1365 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/fit-width.png
+-rw-rw-rw-   0        0        0     1102 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/fit-window.png
+-rw-rw-rw-   0        0        0     2262 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/fit.png
+-rw-rw-rw-   0        0        0     1587 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/help.png
+-rw-rw-rw-   0        0        0   183198 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/icon.ico
+-rw-rw-rw-   0        0        0    44771 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/icon.png
+-rw-rw-rw-   0        0        0    38362 2023-04-04 10:35:02.000000 xllabelme-5.1.5/xllabelme/icons/icon2.ico
+-rw-rw-rw-   0        0        0    34213 2023-04-04 10:24:55.000000 xllabelme-5.1.5/xllabelme/icons/icon2.png
+-rw-rw-rw-   0        0        0     2381 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/labels.png
+-rw-rw-rw-   0        0        0    37512 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/labels.svg
+-rw-rw-rw-   0        0        0      977 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/new.png
+-rw-rw-rw-   0        0        0    30288 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/next.png
+-rw-rw-rw-   0        0        0     1103 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/objects.png
+-rw-rw-rw-   0        0        0     2073 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/open.png
+-rw-rw-rw-   0        0        0    18773 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/open.svg
+-rw-rw-rw-   0        0        0    30665 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/prev.png
+-rw-rw-rw-   0        0        0     1915 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/quit.png
+-rw-rw-rw-   0        0        0     2811 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/save-as.png
+-rw-rw-rw-   0        0        0    65363 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/save-as.svg
+-rw-rw-rw-   0        0        0     1187 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/save.png
+-rw-rw-rw-   0        0        0    31292 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/save.svg
+-rw-rw-rw-   0        0        0     2004 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/undo-cross.png
+-rw-rw-rw-   0        0        0     2018 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/undo.png
+-rw-rw-rw-   0        0        0     1099 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/zoom-in.png
+-rw-rw-rw-   0        0        0     1074 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/zoom-out.png
+-rw-rw-rw-   0        0        0     1139 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/zoom.png
+-rw-rw-rw-   0        0        0     7120 2023-04-20 09:45:20.000000 xllabelme-5.1.5/xllabelme/label_file.py
+-rw-rw-rw-   0        0        0     1907 2023-03-31 08:56:10.000000 xllabelme-5.1.5/xllabelme/logger.py
+-rw-rw-rw-   0        0        0     9649 2022-04-26 01:24:19.000000 xllabelme-5.1.5/xllabelme/shape.py
+-rw-rw-rw-   0        0        0      886 2021-06-08 03:21:06.000000 xllabelme-5.1.5/xllabelme/testing.py
+-rw-rw-rw-   0        0        0    44799 2023-04-04 12:30:43.000000 xllabelme-5.1.5/xllabelme/ts.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.275153 xllabelme-5.1.5/xllabelme/utils/
+-rw-rw-rw-   0        0        0      749 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/utils/__init__.py
+-rw-rw-rw-   0        0        0      698 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/utils/_io.py
+-rw-rw-rw-   0        0        0     2468 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/utils/image.py
+-rw-rw-rw-   0        0        0     6290 2023-04-04 09:31:32.000000 xllabelme-5.1.5/xllabelme/utils/qt.py
+-rw-rw-rw-   0        0        0     3764 2021-06-08 03:21:06.000000 xllabelme-5.1.5/xllabelme/utils/shape.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.284129 xllabelme-5.1.5/xllabelme/widgets/
+-rw-rw-rw-   0        0        0      554 2022-04-20 05:44:54.000000 xllabelme-5.1.5/xllabelme/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-03-31 14:44:05.000000 xllabelme-5.1.5/xllabelme/widgets/brightness_contrast_dialog.py
+-rw-rw-rw-   0        0        0    35438 2023-04-20 08:18:28.000000 xllabelme-5.1.5/xllabelme/widgets/canvas.py
+-rw-rw-rw-   0        0        0     1231 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/widgets/color_dialog.py
+-rw-rw-rw-   0        0        0      290 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/widgets/escapable_qlist_widget.py
+-rw-rw-rw-   0        0        0     2451 2023-04-15 14:50:00.000000 xllabelme-5.1.5/xllabelme/widgets/file_dialog_preview.py
+-rw-rw-rw-   0        0        0    19741 2022-10-24 08:25:25.000000 xllabelme-5.1.5/xllabelme/widgets/label_dialog.py
+-rw-rw-rw-   0        0        0     6194 2023-03-31 08:45:59.000000 xllabelme-5.1.5/xllabelme/widgets/label_list_widget.py
+-rw-rw-rw-   0        0        0      998 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/widgets/tool_bar.py
+-rw-rw-rw-   0        0        0     1666 2023-03-31 08:47:05.000000 xllabelme-5.1.5/xllabelme/widgets/unique_label_qlist_widget.py
+-rw-rw-rw-   0        0        0      735 2023-04-04 11:11:05.000000 xllabelme-5.1.5/xllabelme/widgets/zoom_widget.py
+-rw-rw-rw-   0        0        0    11774 2023-04-20 09:48:46.000000 xllabelme-5.1.5/xllabelme/xlapp.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.229276 xllabelme-5.1.5/xllabelme.egg-info/
+-rw-rw-rw-   0        0        0    11738 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      281 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      116 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/top_level.txt
```

### Comparing `xllabelme-5.1.4/LICENSE` & `xllabelme-5.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/PKG-INFO` & `xllabelme-5.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xllabelme
-Version: 5.1.4
+Version: 5.1.5
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada
 Author-email: 877362867@qq.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xllabelme Version: 5.1.4 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: xllabelme Version: 5.1.5 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada Author-email: 877362867@qq.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `xllabelme-5.1.4/README.md` & `xllabelme-5.1.5/README.md`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/docs/man/labelme.1` & `xllabelme-5.1.5/docs/man/labelme.1`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/setup.py` & `xllabelme-5.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def get_install_requires():
     PY3 = sys.version_info[0] == 3
     PY2 = sys.version_info[0] == 2
     assert PY3 or PY2
 
     # 试了py3.6、py3.8，都是能编译exe成功的
     install_requires = [
-        "pyxllib>=0.3.24",
+        "pyxllib>=0.3.38",
         # "imgviz==1.2.1",  # 这个限定不用，新版imgviz又兼容了
         "imgviz>=0.11",
         "matplotlib<3.3",  # for PyInstaller
         # "matplotlib",  # 这个版本确实不能升，会有问题，先不要改
 		"natsort>=7.1.0",
         "numpy",
         "Pillow>=2.8",
```

### Comparing `xllabelme-5.1.4/xllabelme/__init__.py` & `xllabelme-5.1.5/xllabelme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 # Semantic Versioning 2.0.0: https://semver.org/
 # 1. MAJOR version when you make incompatible API changes;
 # 2. MINOR version when you add functionality in a backwards-compatible manner;
 # 3. PATCH version when you make backwards-compatible bug fixes.
 
 # 每当官方有第2位版本号更新，比如5.2、5.3时，我会尽力做个源码的同步
 # 然后我个人功能，会在第3位上自增，比如5.1.2、5.1.3
-__version__ = "5.1.4"
+__version__ = "5.1.5"
 
 # 2 扩展的更灵活的labelme，兼容官方的功能，但有更强的可视化效果，能查看shape的多个属性值
 __appname__ = f"xllabelme v{__version__}"
 
 QT4 = QT_VERSION[0] == "4"
 QT5 = QT_VERSION[0] == "5"
 del QT_VERSION
 
 PY2 = sys.version[0] == "2"
 PY3 = sys.version[0] == "3"
 del sys
 
 from xllabelme.label_file import LabelFile
-from xllabelme import testing
+# from xllabelme import testing
 from xllabelme import utils
```

### Comparing `xllabelme-5.1.4/xllabelme/__main__.py` & `xllabelme-5.1.5/xllabelme/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         else:
             output_dir = output
 
     translator = QtCore.QTranslator()
     # 写不存在的值也没影响，默认就是变成英文
     # translator.load(osp.dirname(osp.abspath(__file__)) + "/translate/" + 'zh_CN.qm')
     translator.loadFromData(getattr(xllabelme.ts, args.lang))
-    app = QtWidgets.QApplication(sys.argv)
+    # app = QtWidgets.QApplication(sys.argv)
     app.setApplicationName(__appname__)
     app.setWindowIcon(newIcon("icon.png"))
     app.installTranslator(translator)
     win = mainwin(
         config=config,
         filename=filename,
         output_file=output_file,
@@ -204,13 +204,16 @@
         sys.exit(0)
 
     win.show()
     win.raise_()
     sys.exit(app.exec_())
 
 
+def handle_exception(exc_type, exc_value, exc_traceback):
+    show_message_box(format_exception(exc_value), '程序跑路了，给管理员发这个截图让他来破案吧！')
+
+
 # this main block is required to generate executable by pyinstaller
 if __name__ == "__main__":
-    try:
-        main(XlMainWindow)
-    except Exception as e:
-        show_message_box(format_exception(e), '程序跑路了，给管理员发这个截图让他来破案吧！')
+    app = QtWidgets.QApplication(sys.argv)
+    sys.excepthook = handle_exception  # 全局异常捕获。既能获得错误，也能防止软件崩溃。
+    main(XlMainWindow)
```

### Comparing `xllabelme-5.1.4/xllabelme/app.py` & `xllabelme-5.1.5/xllabelme/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -454,18 +454,18 @@
             functools.partial(self.togglePolygons, True),
             icon="eye",
             tip=self.tr("Show all polygons"),
             enabled=False,
         )
 
         help = action(
-            self.tr("&Tutorial"),
+            self.tr("通用教程"),
             self.tutorial,
             icon="help",
-            tip=self.tr("Show tutorial page"),
+            tip=self.tr("打开通用的xllabelme使用教程"),
         )
 
         zoom = QtWidgets.QWidgetAction(self)
         zoom.setDefaultWidget(self.zoomWidget)
         self.zoomWidget.setWhatsThis(
             str(
                 self.tr(
@@ -567,15 +567,15 @@
         )
 
         clear_label = action(
             self.tr("清空所有标注"),
             self.clearLabel,
             None,
             "delete",
-            self.tr("Modify the label of the selected polygon"),
+            self.tr("清空所有标注，但是保留空json文件"),
             enabled=True,
         )
 
         fill_drawing = action(
             self.tr("Fill Drawing Polygon"),
             self.canvas.setFillDrawing,
             None,
@@ -642,15 +642,15 @@
                 undo,
                 undoLastPoint,
                 None,
                 removePoint,
                 None,
                 toggle_keep_prev_mode,
             ),
-            # menu shown at right click
+            # menu shown at right click，canvas里的右键菜单
             menu=(
                 createMode,
                 createRectangleMode,
                 createCircleMode,
                 createLineMode,
                 createPointMode,
                 createLineStripMode,
@@ -739,16 +739,16 @@
         self.menus.file.aboutToShow.connect(self.updateFileMenu)
 
         # Custom context menu for the canvas widget:
         utils.addActions(self.canvas.menus[0], self.actions.menu)
         utils.addActions(
             self.canvas.menus[1],
             (
-                action("&Copy here", self.copyShape),
-                action("&Move here", self.moveShape),
+                action("复制到这里", self.copyShape),
+                action("移动到这里", self.moveShape),
             ),
         )
 
         self.tools = self.toolbar("Tools")
         # Menu buttons on Left
         self.actions.tool = (
             # open_,
@@ -797,24 +797,25 @@
             Qt.Horizontal: {},
             Qt.Vertical: {},
         }  # key=filename, value=scroll_value
 
         if filename is not None and osp.isdir(filename):
             self.importDirImages(filename, load=False)
         else:
-            self.filename = filename
+            self.filename = filename  # 当前打开的文件
 
         if config["file_search"]:
             self.fileSearch.setText(config["file_search"])
             self.fileSearchChanged()
 
         # XXX: Could be completely declarative.
         # Restore application settings.
         self.settings = QtCore.QSettings("labelme", "labelme")  # 这个配置好像是写到注册表中的~
         self.recentFiles = self.settings.value("recentFiles", []) or []
+        self.recentFiles = [str(f) for f in self.recentFiles]
         size = self.settings.value("window/size", QtCore.QSize(600, 500))
         position = self.settings.value("window/position", QtCore.QPoint(0, 0))
         state = self.settings.value("window/state", QtCore.QByteArray())
         self.resize(size)
         self.move(position)
         # or simply:
         # self.restoreGeometry(settings['window/geometry']
@@ -882,26 +883,26 @@
             2，需要保存图片数据
         :return:
         """
         # Even if we autosave the file, we keep the ability to undo
         self.actions.undo.setEnabled(self.canvas.isShapeRestorable)
 
         if self._config["auto_save"] or self.actions.saveAuto.isChecked():
-            label_file = osp.splitext(self.imagePath)[0] + ".json"
-            if self.output_dir:
-                label_file_without_path = osp.basename(label_file)
-                label_file = osp.join(self.output_dir, label_file_without_path)
-            self.saveLabels(label_file)
-            return
-        self.dirty = self.dirty | dirty
-        self.actions.save.setEnabled(True)
-        title = f'{__appname__}'
-        if self.filename is not None:
-            title = "{} - {}*".format(title, self.filename)
-        self.setWindowTitle(title)
+            self.saveLabels(str(self.get_label_path()))
+
+            if dirty & 2:  # 需要保存图片
+                self.canvas.pixmap.save(self.imagePath, osp.splitext(self.imagePath)[1][1:])
+            self.dirty = 0
+        else:
+            self.dirty = self.dirty | dirty
+            self.actions.save.setEnabled(True)
+            title = f'{__appname__}'
+            if self.filename is not None:
+                title = "{} - {}*".format(title, self.filename)
+            self.setWindowTitle(title)
 
     def setClean(self):
         self.dirty = False
         self.actions.save.setEnabled(False)
         self.actions.createMode.setEnabled(True)
         self.actions.createRectangleMode.setEnabled(True)
         self.actions.createCircleMode.setEnabled(True)
@@ -956,17 +957,18 @@
     # Callbacks
 
     def undoShapeEdit(self):
         self.canvas.restoreShape()
         self.labelList.clear()
         self.loadShapes(self.canvas.shapes)
         self.actions.undo.setEnabled(self.canvas.isShapeRestorable)
+        self.setDirty()
 
     def tutorial(self):
-        url = "https://github.com/wkentaro/labelme/tree/main/examples/tutorial"  # NOQA
+        url = "https://www.yuque.com/xlpr/pyxllib/xllabelme"  # NOQA
         webbrowser.open(url)
 
     def toggleDrawingSensitive(self, drawing=True):
         """Toggle drawing sensitive.
 
         In the middle of drawing, toggling between modes should be disabled.
         """
@@ -1043,15 +1045,15 @@
 
         menu = self.menus.recentFiles
         menu.clear()
         files = [f for f in self.recentFiles if f != current and exists(f)]
         for i, f in enumerate(files):
             icon = utils.newIcon("labels")
             action = QtWidgets.QAction(
-                icon, "&%d %s" % (i + 1, QtCore.QFileInfo(f).fileName()), self
+                icon, "&%d %s" % (i + 1, QtCore.QFileInfo(str(f)).fileName()), self
             )
             action.triggered.connect(functools.partial(self.loadRecent, f))
             menu.addAction(action)
 
     def popLabelListMenu(self, point):
         self.menus.labelList.exec_(self.labelList.mapToGlobal(point))
 
@@ -1160,14 +1162,15 @@
             self.labelList.scrollToItem(item)
         self._noSelectionSlot = False
         n_selected = len(selected_shapes)
         self.actions.delete.setEnabled(n_selected)
         self.actions.duplicate.setEnabled(n_selected)
         self.actions.copy.setEnabled(n_selected)
         self.actions.edit.setEnabled(n_selected == 1)
+        self.project.shapeSelectionChanged(n_selected)
 
     def addLabel(self, shape):
         if shape.group_id is None:
             text = shape.label
         else:
             text = "{} ({})".format(shape.label, shape.group_id)
         label_list_item = LabelListWidgetItem(text, shape)
@@ -1297,16 +1300,15 @@
             item = self.flag_widget.item(i)
             key = item.text()
             flag = item.checkState() == Qt.Checked
             flags[key] = flag
         try:
             imagePath = osp.relpath(self.imagePath, osp.dirname(filename))
             imageData = self.imageData if self._config["store_data"] else None
-            if osp.dirname(filename) and not osp.exists(osp.dirname(filename)):
-                os.makedirs(osp.dirname(filename))
+            filename.parent.mkdir(parents=True, exist_ok=True)
             lf.save(
                 filename=filename,
                 shapes=shapes,
                 imagePath=imagePath,
                 imageData=imageData,
                 imageHeight=self.image.height(),
                 imageWidth=self.image.width(),
@@ -1463,50 +1465,46 @@
     def togglePolygons(self, value):
         for item in self.labelList:
             item.setCheckState(Qt.Checked if value else Qt.Unchecked)
 
     def loadFile(self, filename=None):
         """Load the specified file, or the last opened file if None."""
         # changing fileListWidget loads file
+        imageList = self.imageList
         if filename in self.imageList and (
-                self.fileListWidget.currentRow() != self.imageList.index(filename)
+                self.fileListWidget.currentRow() != imageList.index(filename)
         ):
-            self.fileListWidget.setCurrentRow(self.imageList.index(filename))
+            self.fileListWidget.setCurrentRow(imageList.index(filename))
             self.fileListWidget.repaint()
             return
 
         self.resetState()
         self.canvas.setEnabled(False)
         if filename is None:
             filename = self.settings.value("filename", "")
         # filename = str(filename)
-        filename = osp.join(self.lastOpenDir, str(filename))
-        if not QtCore.QFile.exists(filename):
+        filename = self.get_image_path(filename)
+        if not filename.is_file():
             self.errorMessage(
                 self.tr("Error opening file"),  # 打开文件发生错误
                 self.tr("No such file: <b>%s</b>") % filename,
             )
             return False
         # assumes same name, but json extension
         self.status(
-            str(self.tr("Loading %s...")) % osp.basename(str(filename))
+            str(self.tr("Loading %s...")) % filename.name
         )
-        label_file = osp.splitext(filename)[0] + ".json"
-        if self.output_dir:
-            label_file_without_path = osp.basename(label_file)
-            label_file = osp.join(self.output_dir, label_file_without_path)
-        if QtCore.QFile.exists(label_file) and LabelFile.is_label_file(
-                label_file
-        ):
+        label_file = self.get_label_path(self.get_image_path2(filename))
+        if label_file.is_file() and LabelFile.is_label_file(label_file):
             try:
                 self.labelFile = LabelFile(label_file, filename)
             except LabelFileError as e:
                 self.errorMessage(
-                    self.tr("Error opening file"),
-                    self.tr(
+                    self.tr("Error opening file"),  # 打开文件发生错误
+                    self.tr(  # 请确认 是一个合法的标签文件
                         "<p><b>%s</b></p>"
                         "<p>Make sure <i>%s</i> is a valid label file."
                     )
                     % (e, label_file),
                 )
                 self.status(self.tr("Error reading %s") % label_file)
                 return False
@@ -1515,15 +1513,15 @@
                 osp.dirname(label_file),
                 self.labelFile.imagePath,
             )
             self.otherData = self.labelFile.otherData
         else:
             self.imageData = LabelFile.load_image_file(filename)
             if self.imageData:
-                self.imagePath = filename
+                self.imagePath = str(filename)
             self.labelFile = None
         image = QtGui.QImage.fromData(self.imageData)
         if self.imageData:  # ckz: 新增存储cv2的图片数据
             self.arr_image = utils.img_data_to_arr(self.imageData)
 
         if image.isNull():
             formats = [
@@ -1692,15 +1690,17 @@
 
         if len(self.imageList) <= 0:
             return
 
         if self.filename is None:
             return
 
-        currIndex = self.imageList.index(self.filename)
+        fn = XlPath(self.filename).relpath(self.lastOpenDir).as_posix()
+        currIndex = self.imageList.index(fn)
+        # currIndex = self.imageList.index(self.filename)
         if currIndex - 1 >= 0:
             filename = self.imageList[currIndex - 1]
             if filename:
                 self.loadFile(filename)
 
         self._config["keep_prev"] = keep_prev
 
@@ -1729,15 +1729,15 @@
                 else:
                     filename = imageList[-1]
             except ValueError:  # 找不到则默认用第1个
                 filename = imageList[0]
         self.filename = XlPath(self.lastOpenDir, filename)
 
         if self.filename and load:
-            self.loadFile(self.filename)
+            self.loadFile(filename)
 
         self._config["keep_prev"] = keep_prev
 
     def openFile(self, _value=False):
         if not self.mayContinue():
             return
         path = osp.dirname(str(self.filename)) if self.filename else "."
@@ -1800,77 +1800,86 @@
 
     def saveFile(self, _value=False):
         assert not self.image.isNull(), "cannot save empty image"
 
         if self.dirty & 2:  # 需要保存图片
             self.canvas.pixmap.save(self.imagePath, osp.splitext(self.imagePath)[1][1:])
 
-        if self.labelFile:
-            # DL20180323 - overwrite when in directory
-            self._saveFile(self.labelFile.filename)
-        elif self.output_file:
-            self._saveFile(self.output_file)
-            self.close()
-        else:
-            self._saveFile(self.saveFileDialog())
+        if self.dirty & 1:
+            if self.labelFile:
+                # DL20180323 - overwrite when in directory
+                self._saveFile(self.labelFile.filename)
+            elif self.output_file:
+                self._saveFile(self.output_file)
+                self.close()
+            else:
+                self._saveFile(self.saveFileDialog())
 
     def saveFileAs(self, _value=False):
         assert not self.image.isNull(), "cannot save empty image"
         self._saveFile(self.saveFileDialog())
 
     def saveFileDialog(self):
-        caption = self.tr("%s - Choose File") % __appname__
-        filters = self.tr("Label files (*%s)") % LabelFile.suffix
-        if self.output_dir:
-            dlg = QtWidgets.QFileDialog(
-                self, caption, self.output_dir, filters
-            )
-        else:
-            dlg = QtWidgets.QFileDialog(
-                self, caption, self.currentPath(), filters
-            )
-        dlg.setDefaultSuffix(LabelFile.suffix[1:])
-        dlg.setAcceptMode(QtWidgets.QFileDialog.AcceptSave)
-        dlg.setOption(QtWidgets.QFileDialog.DontConfirmOverwrite, False)
-        dlg.setOption(QtWidgets.QFileDialog.DontUseNativeDialog, False)
-        basename = osp.basename(osp.splitext(self.filename)[0])
-        if self.output_dir:
-            default_labelfile_name = osp.join(
-                self.output_dir, basename + LabelFile.suffix
-            )
+        if self.savefile_without_dialog_action.isChecked():
+            filename = str(XlPath(self.imagePath).with_suffix('.json'))
         else:
-            default_labelfile_name = osp.join(
-                self.currentPath(), basename + LabelFile.suffix
+            caption = self.tr("%s - Choose File") % __appname__
+            filters = self.tr("Label files (*%s)") % LabelFile.suffix
+            if self.output_dir:
+                dlg = QtWidgets.QFileDialog(
+                    self, caption, self.output_dir, filters
+                )
+            else:
+                dlg = QtWidgets.QFileDialog(
+                    self, caption, self.currentPath(), filters
+                )
+            dlg.setDefaultSuffix(LabelFile.suffix[1:])
+            dlg.setAcceptMode(QtWidgets.QFileDialog.AcceptSave)
+            dlg.setOption(QtWidgets.QFileDialog.DontConfirmOverwrite, False)
+            dlg.setOption(QtWidgets.QFileDialog.DontUseNativeDialog, False)
+            basename = osp.basename(osp.splitext(self.filename)[0])
+            if self.output_dir:
+                default_labelfile_name = osp.join(
+                    self.output_dir, basename + LabelFile.suffix
+                )
+            else:
+                default_labelfile_name = osp.join(
+                    self.currentPath(), basename + LabelFile.suffix
+                )
+            filename = dlg.getSaveFileName(
+                self,
+                self.tr("Choose File"),
+                default_labelfile_name,
+                self.tr("Label files (*%s)") % LabelFile.suffix,
             )
-        filename = dlg.getSaveFileName(
-            self,
-            self.tr("Choose File"),
-            default_labelfile_name,
-            self.tr("Label files (*%s)") % LabelFile.suffix,
-        )
+
         if isinstance(filename, tuple):
             filename, _ = filename
         return filename
 
     def _saveFile(self, filename):
-        if filename and self.saveLabels(filename):
-            self.addRecentFile(filename)
-            self.setClean()
+        if filename:
+            image_path = self.get_image_path2()
+            if self.saveLabels(filename):
+                item = self.fileListWidget.findItems(image_path, Qt.MatchExactly)[0]
+                item.setCheckState(Qt.Checked)
+                self.addRecentFile(filename)
+                self.setClean()
 
     def closeFile(self, _value=False):
         if not self.mayContinue():
             return
         self.resetState()
         self.setClean()
         self.toggleActions(False)
         self.canvas.setEnabled(False)
         self.actions.saveAs.setEnabled(False)
 
     def getLabelFile(self):
-        if self.filename.lower().endswith(".json"):
+        if str(self.filename).lower().endswith(".json"):
             label_file = self.filename
         else:
             label_file = osp.splitext(self.filename)[0] + ".json"
 
         return label_file
 
     def deleteFile(self):
@@ -2013,37 +2022,63 @@
     def imageList(self):
         lst = []
         for i in range(self.fileListWidget.count()):
             item = self.fileListWidget.item(i)
             lst.append(item.text())
         return lst
 
+    def get_image_path(self, fn=None):
+        """ label里的路径处理太乱了，统一一个处理接口
+        图片绝对路径，返回XlPath
+
+        :param fn: 可以输入一个参考名称，没输入时，默认获取"文件列表"中选中的item
+        """
+        if fn:
+            return XlPath.init(fn, self.lastOpenDir)
+        else:
+            return XlPath.init(self.imagePath, self.lastOpenDir)
+
+    def get_label_path(self, fn=None):
+        """ json绝对路径，返回XlPath """
+        outdir = self.output_dir or self.lastOpenDir
+
+        if fn:
+            p = XlPath.init(fn, outdir)
+        else:
+            p = XlPath.init(self.labelFile.filename if self.labelFile else self.get_image_path2(), outdir)
+
+        return p.with_suffix('.json')
+
+    def get_image_path2(self, fn=None):
+        """ 图片相对路径，返回str """
+        p = self.get_image_path(fn)
+        return p.relpath(self.lastOpenDir).as_posix()
+
+    def get_label_path2(self, fn=None):
+        """ json相对路径，返回str """
+        p = self.get_label_path(fn)
+        return p.relpath(self.lastOpenDir).as_posix()
+
     def importDroppedImageFiles(self, imageFiles):
         extensions = [
             ".%s" % fmt.data().decode().lower()
             for fmt in QtGui.QImageReader.supportedImageFormats()
         ]
 
         self.filename = None
+        imageList = self.imageList
         for file in imageFiles:
-            if file in self.imageList or not file.lower().endswith(
+            if file in imageList or not file.lower().endswith(
                     tuple(extensions)
             ):
                 continue
-            # label_file = osp.splitext(file)[0] + ".json"
-            if self.output_dir:
-                label_file_without_path = osp.basename(label_file)
-                label_file = osp.join(self.output_dir, label_file_without_path)
-            else:
-                label_file = osp.join(self.lastOpenDir, label_file)
+            label_file = self.get_label_path(file)
             item = QtWidgets.QListWidgetItem(file)
             item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsSelectable)
-            if QtCore.QFile.exists(label_file) and LabelFile.is_label_file(
-                    label_file
-            ):
+            if label_file.is_file() and LabelFile.is_label_file(label_file):
                 item.setCheckState(Qt.Checked)
             else:
                 item.setCheckState(Qt.Unchecked)
             self.fileListWidget.addItem(item)
 
         if len(self.imageList) > 1:
             self.actions.openNextImg.setEnabled(True)
@@ -2058,48 +2093,26 @@
         if not self.mayContinue() or not dirpath:
             return
 
         self.lastOpenDir = dirpath
         self.filename = filename
         self.fileListWidget.clear()
 
-        image_root = self.xllabel.image_root or dirpath
-        for filename in self.scanAllImages(image_root):
+        for filename in self.scanAllImages(dirpath):
             if pattern and pattern not in filename:
                 continue
-            label_file = osp.splitext(filename)[0] + ".json"
-            # label_file = osp.join(self.lastOpenDir, osp.basename(filename) + ".json")
-            if self.output_dir:
-                label_file_without_path = osp.basename(label_file)
-                label_file = osp.join(self.output_dir, label_file_without_path)
-            else:
-                label_file = osp.join(self.lastOpenDir, label_file)
+            label_file = self.get_label_path(filename)
             item = QtWidgets.QListWidgetItem(filename)
             item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsSelectable)
-            if QtCore.QFile.exists(label_file) and LabelFile.is_label_file(
-                    label_file
-            ):
+            if label_file.is_file() and LabelFile.is_label_file(label_file):
                 item.setCheckState(Qt.Checked)
             else:
                 item.setCheckState(Qt.Unchecked)
             self.fileListWidget.addItem(item)
 
-        # else:  # ckz，我要扩展一个读取json来展示图片的功能
-        #     root = self.xllabel.image_root
-        #     for label_file in XlPath(dirpath).rglob('*.json'):
-        #         data = label_file.read_json()
-        #         if 'imagePath' in data:
-        #             filename = str(label_file.relpath(dirpath))
-        #         else:
-        #             continue
-        #         item = QtWidgets.QListWidgetItem(filename)
-        #         item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsSelectable)
-        #         item.setCheckState(Qt.Checked)
-        #         self.fileListWidget.addItem(item)
-
         self.openNextImg(load=load, offset=offset)
 
     def scanAllImages(self, folderPath):
         extensions = [
             ".%s" % fmt.data().decode().lower()
             for fmt in QtGui.QImageReader.supportedImageFormats()
         ]
```

### Comparing `xllabelme-5.1.4/xllabelme/cli/draw_json.py` & `xllabelme-5.1.5/xllabelme/cli/draw_json.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/cli/draw_label_png.py` & `xllabelme-5.1.5/xllabelme/cli/draw_label_png.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/cli/json_to_dataset.py` & `xllabelme-5.1.5/xllabelme/cli/json_to_dataset.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/cli/on_docker.py` & `xllabelme-5.1.5/xllabelme/cli/on_docker.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/config/__init__.py` & `xllabelme-5.1.5/xllabelme/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/config/default_config.yaml` & `xllabelme-5.1.5/xllabelme/config/default_config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -91,16 +91,16 @@
 
   zoom_in: [Ctrl++, Ctrl+=]
   zoom_out: Ctrl+-
   zoom_to_original: Ctrl+0
   fit_window: Ctrl+F
   fit_width: Ctrl+Shift+F
 
-  create_polygon: Ctrl+N
-  create_rectangle: Ctrl+R
+  create_polygon: [Ctrl+N, Ctrl+1]
+  create_rectangle: [Ctrl+R, Ctrl+3]
   create_circle: null
   create_line: null
   create_point: null
   create_linestrip: null
   edit_polygon: Ctrl+J
   delete_polygon: Delete
   duplicate_polygon: Ctrl+D
```

### Comparing `xllabelme-5.1.4/xllabelme/config/xllabellib.py` & `xllabelme-5.1.5/xllabelme/config/xllabellib.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,49 +4,55 @@
 import os.path as osp
 import re
 from statistics import mean
 import time
 import sys
 
 import requests
+import webbrowser
+
+import numpy as np
 
 from PyQt5.QtCore import QPointF, QTranslator, QLocale, QLibraryInfo
 from PyQt5.QtWidgets import QMenu, QAction, QFileDialog, QMessageBox, QActionGroup, QApplication
 from qtpy import QtGui
 from qtpy.QtCore import Qt
+from PyQt5.QtGui import QImage, QPixmap, QColor
 
 from pyxllib.file.specialist import XlPath
 from pyxllib.algo.geo import rect_bounds
 from pyxllib.algo.pupil import make_index_function
 from pyxllib.prog.pupil import DictTool
 from pyxlpr.ai.clientlib import XlAiClient
 from pyxllib.algo.shapelylib import ShapelyPolygon
+# from pyxllib.xlcv import xlcv
 
 from xllabelme import utils
 from xllabelme.widgets import LabelListWidgetItem
 from xllabelme.shape import Shape
 
 _CONFIGS = {
     '原版labelme': {},
     'xllabelme': {},
     'm2302中科院题库':  # 这是比较旧的一套配置字段名
         {'_attrs':
              [['line_id', 1, 'int'],
               ['content_type', 1, 'str', ('印刷体', '手写体')],
-              ["content_class", 1, "str", ("文本", "公式", "图片", "表格")],
+              ["content_class", 1, "str", ("文本", "公式", "图片", "表格", "删除")],
               ['text', 1, 'str'],
               ],
          'label_shape_color': 'content_type,content_class'.split(','),
          'label_shape_color2': ['line_id'],
          'default_label': json.dumps({'line_id': 1,
                                       'content_type': '印刷体',
                                       'content_class': '文本',
                                       'text': ''}, ensure_ascii=False),
          },
     'm2303表格标注': {},
+    'm2303表格标注二阶段': {},
     # '渊亭OCR':  # 这是比较旧的一套配置字段名
     #     {'_attrs':
     #          [['content_type', 1, 'str', ('印刷体', '手写体', '印章', '其它')],
     #           ['content_kv', 1, 'str', ('key', 'value')],
     #           ["content_class", 1, "str", ("姓名", "身份证号", "联系方式", "采样时间", "检测时间", "核酸结果", "其它类")],
     #           ['text', 1, 'str'],
     #           ],
@@ -112,14 +118,44 @@
     #           ['sroie_class', 1, 'str', ('other', 'company', 'address', 'date', 'total')],
     #           ['sroie_kv', 1, 'str', ('other', 'key', 'value')],
     #           ]
     #      },
 }
 
 
+def q_pixmap_to_np_array(qpixmap):
+    qimage = qpixmap.toImage()
+    width, height = qimage.width(), qimage.height()
+    channel_count = qimage.pixelFormat().channelCount()
+    buffer = qimage.constBits().asarray(width * height * channel_count)
+    np_array = np.frombuffer(buffer, dtype=np.uint8).reshape((height, width, channel_count))
+    return np_array
+
+
+def np_array_to_q_pixmap(np_array):
+    if len(np_array.shape) == 2:
+        height, width = np_array.shape
+        channel_count = 1
+    else:
+        height, width, channel_count = np_array.shape
+    bytes_per_line = channel_count * width
+
+    if channel_count == 1:
+        format = QImage.Format_Grayscale8
+    elif channel_count == 3:
+        format = QImage.Format_RGB888
+    elif channel_count == 4:
+        format = QImage.Format_RGBA8888
+    else:
+        raise ValueError("Unsupported channel count: {}".format(channel_count))
+
+    qimage = QImage(np_array.data, width, height, bytes_per_line, format)
+    return QPixmap.fromImage(qimage)
+
+
 def __1_自定义项目():
     pass
 
 
 class 原版labelme:
     """ 不同项目任务可以继承这个类，进行一些功能的定制
     这里设计默认是labelme原版功能
@@ -179,15 +215,15 @@
             def func(x):
                 xllabel.auto_rec_text = x
 
                 if xllabel.auto_rec_text:
                     os.environ['XlAiAccounts'] = 'eyJwcml1IjogeyJ0b2tlbiI6ICJ4bGxhYmVsbWV5XipBOXlraiJ9fQ=='
                     try:
                         xllabel.xlapi = XlAiClient()
-                    except ConnectionError:
+                    except requests.exceptions.ConnectionError:
                         # 没有网络
                         xllabel.xlapi = None
                         a.setChecked(False)
                         # 提示
                         msg_box = QMessageBox(QMessageBox.Information, "xllabelme标注工具：连接自动识别的API失败",
                                               "尝试连接xmutpriu.com的api失败，请检查网络问题，比如关闭梯子。\n"
                                               '如果仍然连接不上，可能是服务器的问题，请联系"管理员"。')
@@ -225,18 +261,32 @@
                                       "注意，需要重启软件才能生效。")
                 msg_box.setStandardButtons(QMessageBox.Ok)
                 msg_box.exec_()
 
             a.triggered.connect(func)
             return a
 
+        def create_savefile_without_dialog_action():
+            a = utils.newAction(mainwin,
+                                mainwin.tr("关闭保存标注文件的弹窗"),
+                                lambda x: a.setChecked(x),
+                                None,  # 快捷键
+                                None,  # 图标
+                                mainwin.tr("无json标注文件情况下，保存时不启用dialog而是自动生成标注文件"),  # 左下角的提示
+                                checkable=True,
+                                checked=True,
+                                )
+            mainwin.savefile_without_dialog_action = a
+            return a
+
         settings_menu = self.mainwin.menus.settings
         settings_menu.addMenu(create_project_menu())
         settings_menu.addSeparator()
         settings_menu.addAction(create_auto_rec_text_action())
+        settings_menu.addAction(create_savefile_without_dialog_action())
         # 关闭该功能，发现原本就有类似的功能，是我重复造轮子了
         # settings_menu.addAction(create_set_image_root_action())
         settings_menu.addSeparator()
         settings_menu.addAction(create_reset_config_action())
 
     def convert_to_rectangle_action(self):
         """ 将shape形状改为四边形 """
@@ -253,15 +303,16 @@
 
         mainwin = self.mainwin
         a = utils.newAction(mainwin,
                             mainwin.tr("Convert to Rectangle"),
                             func,
                             None,  # 快捷键
                             None,  # 图标
-                            mainwin.tr("将当前shape形状转为Rectangle矩形")  # 左下角的提示
+                            mainwin.tr("将当前shape形状转为Rectangle矩形"),  # 左下角的提示
+                            enabled=False,
                             )
         return a
 
     def rotate_image_action(self):
         """ 旋转图片 """
 
         def flip_points(sp, h):
@@ -300,14 +351,15 @@
                 flip_points(sp, h)
 
             # 2 旋转图片
             mainwin.updateShapes(shapes)
             transform = QTransform()
             transform.rotate(90)
             canvas.pixmap = canvas.pixmap.transformed(transform)
+            mainwin.image = canvas.pixmap.toImage()
 
             # 3 end
             canvas.repaint()
             mainwin.setDirty(3)
 
         mainwin = self.mainwin
         a = utils.newAction(mainwin,
@@ -317,14 +369,35 @@
                             None,  # 图标
                             mainwin.tr("将图片和当前标注的形状，顺时针旋转90度，可以多次操作调整到合适方向。"
                                        "注意1：软件中操作并未改变原始图片，需要保存标注文件后，外部图片文件才会更新。"
                                        "注意2：图片操作目前是撤销不了的，不过可以不保存再重新打开文件恢复初始状态。")  # 左下角的提示
                             )
         return a
 
+    # def deskew_image_action(self):
+    #     def func():
+    #         canvas = mainwin.canvas
+    #         image = q_pixmap_to_np_array(canvas.pixmap)
+    #         image = xlcv.deskew_image(image)
+    #         canvas.pixmap = np_array_to_q_pixmap(image)
+    #         canvas.repaint()
+    #         mainwin.setDirty(2)
+    #
+    #     mainwin = self.mainwin
+    #     a = utils.newAction(mainwin,
+    #                         mainwin.tr("歪斜图片矫正"),
+    #                         func,
+    #                         None,  # 快捷键
+    #                         None,  # 图标
+    #                         mainwin.tr("歪斜比较严重的图片，可以尝试使用该功能矫正。"
+    #                                    "注意1：软件中操作并未改变原始图片，需要保存标注文件后，外部图片文件才会更新。"
+    #                                    "注意2：图片操作目前是撤销不了的，不过可以不保存再重新打开文件恢复初始状态。")  # 左下角的提示
+    #                         )
+    #     return a
+
     def create(self):
         mainwin = self.mainwin
 
         # 1 设置菜单
         self.config_settings_menu()
 
         # 2 帮助菜单
@@ -351,19 +424,26 @@
         # 4 右键菜单增加功能
         mainwin.actions.menu = list(mainwin.actions.menu) + [
             None,
             self.convert_to_rectangle_action(),
             self.xllabel.split_shape_action(),
             None,
             self.rotate_image_action(),
+            # self.deskew_image_action(),  # 歪斜矫正
         ]
 
         # 5 一些操作习惯
         mainwin.populateModeActions()
 
+    def shapeSelectionChanged(self, n_selected):
+        """ 选中shape时会激活的功能 """
+        menu = self.mainwin.actions.menu
+        menu[-4].setEnabled(n_selected)
+        menu[-3].setEnabled(n_selected)
+
     def destroy(self):
         """ 销毁项目相关配置 """
         self.mainwin.menus.settings.clear()
         self.mainwin.actions.editMenu = self.mainwin.actions.editMenu[:-3]
         self.mainwin.actions.menu = self.mainwin.actions.menu[:-5]
 
     def update_shape(self, shape, label_list_item=None):
@@ -671,45 +751,97 @@
 
 class m2302中科院题库(增强版xllabelme):
     def get_default_label(self, shape=None):
         from pyxllib.cv.xlcvlib import xlcv
         from pyxlpr.data.imtextline import TextlineShape
 
         # 1 获得基本内容。如果开了识别接口，要调api。
-        xllabel = self.mainwin.xllabel
+        mainwin = self.mainwin
+        xllabel = mainwin.xllabel
         points = [(p.x(), p.y()) for p in shape.points]
         d = None
         if xllabel.auto_rec_text and xllabel.xlapi and shape:
             # 识别指定的points区域
 
-            im = xlcv.get_sub(xllabel.mainwin.arr_image, points, warp_quad=True)
+            im = xlcv.get_sub(mainwin.arr_image, points, warp_quad=True)
             try:
-                d = xllabel.xlapi.priu_api('content_ocr', im, filename=xllabel.mainwin.filename)
+                d = xllabel.xlapi.priu_api('content_ocr', im, filename=str(mainwin.filename))
             except requests.exceptions.ConnectionError:
                 pass
         if d is None:  # 设默认值
             d = {'line_id': 1, 'content_type': '印刷体', 'content_class': '文本', 'text': ''}
 
         # 2 获得line_id
         line_id = 1
-        shapes = xllabel.mainwin.canvas.shapes  # 最后一个框
+        shapes = mainwin.canvas.shapes  # 最后一个框
         if len(shapes) > 1:
             sp = shapes[-2]  # 当前框会变成shapes[-1]，所以要取shapes[-2]才是上一次建立的框
             line_id0 = json.loads(sp.label).get('line_id', 1)
             if TextlineShape(points).in_the_same_line(TextlineShape([(p.x(), p.y()) for p in sp.points])):
                 line_id = line_id0
             else:
                 line_id = line_id0 + 1
         d['line_id'] = line_id
 
         return json.dumps(d, ensure_ascii=False)
 
 
 class m2303表格标注(原版labelme):
     def get_default_label(self, shape=None):
+        return '表格'
+
+    def move_file(self, dst):
+        # 0 准备
+        m = self.mainwin
+        fw = self.fileListWidget
+        item = fw.currentItem()
+        t = item.text()
+
+        if t.startswith(dst + '/'):
+            # 已经是分好类的，不处理
+            return
+
+        dst_path = XlPath.init(dst, m.lastOpenDir)
+        dst_path.mkdir(exist_ok=True)
+
+        # 1 移动文件
+        p = m.get_image_path()
+        p.move(dst_path / p.name)
+        p2 = m.get_label_path()
+        p2.move(dst_path / p2.name)
+
+        # 2 更新标签
+        item.setText(dst + '/' + p.name)
+
+    def create(self):
+        super().create()
+
+        # 1 帮助文档
+        mainwin = self.mainwin
+        self.help_action = utils.newAction(mainwin,
+                                           mainwin.tr("表格标注文档"),
+                                           lambda: webbrowser.open("https://docs.qq.com/doc/DUnZJQnN1YkZMZkpx"))
+        mainwin.menus.help.addAction(self.help_action)
+
+        # 2 文件列表的右键菜单
+        fileListWidget = self.fileListWidget = mainwin.fileListWidget
+        self.menu = QMenu(self.fileListWidget)
+        self.menu.addAction('移到"无表格"', lambda: self.move_file('无表格'))
+        self.menu.addAction('移到"重复图"', lambda: self.move_file('重复图'))
+        fileListWidget.setContextMenuPolicy(Qt.CustomContextMenu)
+        fileListWidget.customContextMenuRequested.connect(lambda pos: self.menu.exec_(fileListWidget.mapToGlobal(pos)))
+
+    def destroy(self):
+        self.mainwin.menus.help.removeAction(self.help_action)
+        self.fileListWidget.customContextMenuRequested.disconnect()
+        super().destroy()
+
+
+class m2303表格标注二阶段(m2303表格标注):
+    def get_default_label(self, shape=None):
         """ 这个识别可以做的更精细的，不过这个项目不一定接，现在只做一个最基础性的功能 """
         # 表格, 可见横线, 可见竖线, 不可见横线, 不可见竖线
 
         poly = ShapelyPolygon.gen([(p.x(), p.y()) for p in shape.points])
         bounds = poly.bounds
         width = bounds[2] - bounds[0]
         height = bounds[3] - bounds[1]
@@ -861,15 +993,15 @@
             def func(x):
                 self.auto_rec_text = x
 
                 if self.auto_rec_text:
                     os.environ['XlAiAccounts'] = 'eyJwcml1IjogeyJ0b2tlbiI6ICJ4bGxhYmVsbWV5XipBOXlraiJ9fQ=='
                     try:
                         self.xlapi = XlAiClient()
-                    except ConnectionError:
+                    except requests.exceptions.ConnectionError:
                         # 没有网络
                         self.xlapi = None
                         a.setChecked(False)
                         # 提示
                         msg_box = QMessageBox(QMessageBox.Information, "xllabelme标注工具：连接自动识别的API失败",
                                               "尝试连接xmutpriu.com的api失败，请检查网络问题，比如关闭梯子。\n"
                                               '如果仍然连接不上，可能是服务器的问题，请联系"管理员"。')
@@ -1181,15 +1313,16 @@
 
         mainwin = self.mainwin
         a = utils.newAction(mainwin,
                             mainwin.tr("Split Shape"),
                             func,
                             None,  # shortcut
                             None,  # icon
-                            mainwin.tr("在当前鼠标点击位置，将一个shape拆成两个shape（注意，该功能会强制拆出两个矩形框）")
+                            mainwin.tr("在当前鼠标点击位置，将一个shape拆成两个shape（注意，该功能会强制拆出两个矩形框）"),
+                            enabled=False,
                             )
         return a
 
     def change_check(self, update=True):
         """ 设置不同的高亮格式 """
         if update:
             self.default_shape_color_mode += 1
```

### Comparing `xllabelme-5.1.4/xllabelme/icons/cancel.png` & `xllabelme-5.1.5/xllabelme/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/close.png` & `xllabelme-5.1.5/xllabelme/icons/close.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/color-line.png` & `xllabelme-5.1.5/xllabelme/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/color.png` & `xllabelme-5.1.5/xllabelme/icons/color.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/copy.png` & `xllabelme-5.1.5/xllabelme/icons/copy.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/delete.png` & `xllabelme-5.1.5/xllabelme/icons/delete.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/done.png` & `xllabelme-5.1.5/xllabelme/icons/done.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/done.svg` & `xllabelme-5.1.5/xllabelme/icons/done.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/edit.png` & `xllabelme-5.1.5/xllabelme/icons/edit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/expert.png` & `xllabelme-5.1.5/xllabelme/icons/expert.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/eye.png` & `xllabelme-5.1.5/xllabelme/icons/eye.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/feBlend-icon.png` & `xllabelme-5.1.5/xllabelme/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/file.png` & `xllabelme-5.1.5/xllabelme/icons/file.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/fit-width.png` & `xllabelme-5.1.5/xllabelme/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/fit-window.png` & `xllabelme-5.1.5/xllabelme/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/fit.png` & `xllabelme-5.1.5/xllabelme/icons/fit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/help.png` & `xllabelme-5.1.5/xllabelme/icons/help.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/icon.ico` & `xllabelme-5.1.5/xllabelme/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/icon.png` & `xllabelme-5.1.5/xllabelme/icons/icon.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/icon2.ico` & `xllabelme-5.1.5/xllabelme/icons/icon2.ico`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/icon2.png` & `xllabelme-5.1.5/xllabelme/icons/icon2.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/labels.png` & `xllabelme-5.1.5/xllabelme/icons/labels.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/labels.svg` & `xllabelme-5.1.5/xllabelme/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/new.png` & `xllabelme-5.1.5/xllabelme/icons/new.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/next.png` & `xllabelme-5.1.5/xllabelme/icons/next.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/objects.png` & `xllabelme-5.1.5/xllabelme/icons/objects.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/open.png` & `xllabelme-5.1.5/xllabelme/icons/open.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/open.svg` & `xllabelme-5.1.5/xllabelme/icons/open.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/prev.png` & `xllabelme-5.1.5/xllabelme/icons/prev.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/quit.png` & `xllabelme-5.1.5/xllabelme/icons/quit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/save-as.png` & `xllabelme-5.1.5/xllabelme/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/save-as.svg` & `xllabelme-5.1.5/xllabelme/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/save.png` & `xllabelme-5.1.5/xllabelme/icons/save.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/save.svg` & `xllabelme-5.1.5/xllabelme/icons/save.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/undo-cross.png` & `xllabelme-5.1.5/xllabelme/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/undo.png` & `xllabelme-5.1.5/xllabelme/icons/undo.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/zoom-in.png` & `xllabelme-5.1.5/xllabelme/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/zoom-out.png` & `xllabelme-5.1.5/xllabelme/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/icons/zoom.png` & `xllabelme-5.1.5/xllabelme/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/label_file.py` & `xllabelme-5.1.5/xllabelme/label_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,43 +11,46 @@
 from xllabelme import PY2
 from xllabelme import QT4
 from xllabelme import utils
 
 PIL.Image.MAX_IMAGE_PIXELS = None
 
 
-@contextlib.contextmanager
-def open(name, mode):
-    assert mode in ["r", "w"]
-    if PY2:
-        mode += "b"
-        encoding = None
-    else:
-        encoding = "utf-8"
-    yield io.open(name, mode, encoding=encoding)
-    return
+# @contextlib.contextmanager
+# def open(name, mode):
+#     assert mode in ["r", "w"]
+#     if PY2:
+#         mode += "b"
+#         encoding = None
+#     else:
+#         encoding = "utf-8"
+#     f = io.open(name, mode, encoding=encoding)
+#     try:
+#         yield f
+#     finally:
+#         f.close()
 
 
 class LabelFileError(Exception):
     pass
 
 
 class LabelFile(object):
     suffix = ".json"
 
     def __init__(self, filename=None, image_file=None):
         self.shapes = []
         self.imagePath = None
         self.imageData = None
 
-        self.image_file = image_file
+        self.image_file = str(image_file)
 
         if filename is not None:
             self.load(filename)
-        self.filename = filename
+        self.filename = str(filename)
 
     @staticmethod
     def load_image_file(filename):
         try:
             image_pil = PIL.Image.open(filename)
         except IOError:
             logger.error("Failed opening image file: {}".format(filename))
@@ -85,15 +88,15 @@
             "label",
             "points",
             "group_id",
             "shape_type",
             "flags",
         ]
         try:
-            with open(filename, "r") as f:
+            with open(filename, "r", encoding='utf8') as f:
                 data = json.load(f)
             version = data.get("version")
             if version is None:
                 logger.warning(
                     "Loading JSON file ({}) of unknown version".format(
                         filename
                     )
@@ -197,15 +200,15 @@
             imageHeight=imageHeight,
             imageWidth=imageWidth,
         )
         for key, value in otherData.items():
             assert key not in data
             data[key] = value
         try:
-            with open(filename, "w") as f:
+            with open(filename, "w", encoding='utf8') as f:
                 json.dump(data, f, ensure_ascii=False, indent=2)
             self.filename = filename
         except Exception as e:
             raise LabelFileError(e)
 
     @staticmethod
     def is_label_file(filename):
```

### Comparing `xllabelme-5.1.4/xllabelme/logger.py` & `xllabelme-5.1.5/xllabelme/logger.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/shape.py` & `xllabelme-5.1.5/xllabelme/shape.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/testing.py` & `xllabelme-5.1.5/xllabelme/testing.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/ts.py` & `xllabelme-5.1.5/xllabelme/ts.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/utils/__init__.py` & `xllabelme-5.1.5/xllabelme/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/utils/_io.py` & `xllabelme-5.1.5/xllabelme/utils/_io.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/utils/image.py` & `xllabelme-5.1.5/xllabelme/utils/image.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/utils/qt.py` & `xllabelme-5.1.5/xllabelme/utils/qt.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/utils/shape.py` & `xllabelme-5.1.5/xllabelme/utils/shape.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/__init__.py` & `xllabelme-5.1.5/xllabelme/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/brightness_contrast_dialog.py` & `xllabelme-5.1.5/xllabelme/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/canvas.py` & `xllabelme-5.1.5/xllabelme/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/color_dialog.py` & `xllabelme-5.1.5/xllabelme/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/file_dialog_preview.py` & `xllabelme-5.1.5/xllabelme/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/label_dialog.py` & `xllabelme-5.1.5/xllabelme/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/label_list_widget.py` & `xllabelme-5.1.5/xllabelme/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/tool_bar.py` & `xllabelme-5.1.5/xllabelme/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/unique_label_qlist_widget.py` & `xllabelme-5.1.5/xllabelme/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/widgets/zoom_widget.py` & `xllabelme-5.1.5/xllabelme/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.4/xllabelme/xlapp.py` & `xllabelme-5.1.5/xllabelme/xlapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
                 otherData=self.otherData,
                 flags=flags,
             )
 
             # 2 fileList里可能原本没有标记json文件的，现在可以标记
             self.labelFile = lf
             items = self.fileListWidget.findItems(
-                self.imagePath, Qt.MatchExactly
+                self.get_image_path2(self.imagePath), Qt.MatchExactly
             )
             if len(items) > 0:
                 if len(items) != 1:
                     raise RuntimeError("There are duplicate files.")
                 items[0].setCheckState(Qt.Checked)
             # disable allows next and previous image to proceed
             # self.filename = filename
@@ -301,12 +301,12 @@
     def open_last_workspace(self):
         """ 打开上一次退出软件的工作空间状态 """
         # 如果保存了目录和文件，打开上次工作状态
         if 'lastOpenDir' in self.xllabel.meta_cfg:
             d = XlPath(self.xllabel.meta_cfg['lastOpenDir'])
             if d.is_dir():
                 if 'filename' in self.xllabel.meta_cfg:
-                    p = XlPath(self.xllabel.meta_cfg['filename'])
+                    p = d / self.xllabel.meta_cfg['filename']
                     if p.is_file():
                         self.importDirImages(d, filename=str(p), offset=0)
                         return
                 self.importDirImages(d)
```

### Comparing `xllabelme-5.1.4/xllabelme.egg-info/PKG-INFO` & `xllabelme-5.1.5/xllabelme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xllabelme
-Version: 5.1.4
+Version: 5.1.5
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada
 Author-email: 877362867@qq.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xllabelme Version: 5.1.4 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: xllabelme Version: 5.1.5 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada Author-email: 877362867@qq.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `xllabelme-5.1.4/xllabelme.egg-info/SOURCES.txt` & `xllabelme-5.1.5/xllabelme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

