# Comparing `tmp/flet_core-0.6.0.dev1322.tar.gz` & `tmp/flet_core-0.6.0.dev1336.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_core-0.6.0.dev1322.tar", max compression
+gzip compressed data, was "flet_core-0.6.0.dev1336.tar", max compression
```

## Comparing `flet_core-0.6.0.dev1322.tar` & `flet_core-0.6.0.dev1336.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0      189 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/README.md
--rw-r--r--   0        0        0      723 2023-04-17 18:18:47.733178 flet_core-0.6.0.dev1322/pyproject.toml
--rw-r--r--   0        0        0     6035 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/__init__.py
--rw-r--r--   0        0        0     6774 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/alert_dialog.py
--rw-r--r--   0        0        0      407 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/alignment.py
--rw-r--r--   0        0        0     7226 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/animated_switcher.py
--rw-r--r--   0        0        0     2806 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/animation.py
--rw-r--r--   0        0        0     5403 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/app_bar.py
--rw-r--r--   0        0        0     7301 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/audio.py
--rw-r--r--   0        0        0     5446 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/banner.py
--rw-r--r--   0        0        0     1079 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/border.py
--rw-r--r--   0        0        0      930 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/border_radius.py
--rw-r--r--   0        0        0     2826 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/bottom_sheet.py
--rw-r--r--   0        0        0     2202 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/buttons.py
--rw-r--r--   0        0        0     3036 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/callable_control.py
--rw-r--r--   0        0        0     5639 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/card.py
--rw-r--r--   0        0        0     9855 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/bar_chart.py
--rw-r--r--   0        0        0     2061 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/bar_chart_group.py
--rw-r--r--   0        0        0     6837 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0        0        0     1949 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0        0        0     2924 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/chart_axis.py
--rw-r--r--   0        0        0     1293 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/chart_axis_label.py
--rw-r--r--   0        0        0      338 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0        0        0      286 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/chart_point_line.py
--rw-r--r--   0        0        0     1006 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/chart_point_shape.py
--rw-r--r--   0        0        0    11228 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/line_chart.py
--rw-r--r--   0        0        0     8258 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/line_chart_data.py
--rw-r--r--   0        0        0     5496 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0        0        0     5888 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/pie_chart.py
--rw-r--r--   0        0        0     3824 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/charts/pie_chart_section.py
--rw-r--r--   0        0        0     7122 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/checkbox.py
--rw-r--r--   0        0        0     6739 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/circle_avatar.py
--rw-r--r--   0        0        0     3085 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/client_storage.py
--rw-r--r--   0        0        0     1002 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/clipboard.py
--rw-r--r--   0        0        0    10627 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/colors.py
--rw-r--r--   0        0        0     7305 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/column.py
--rw-r--r--   0        0        0     1132 2023-04-17 18:18:07.057538 flet_core-0.6.0.dev1322/src/flet_core/connection.py
--rw-r--r--   0        0        0     6848 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/constrained_control.py
--rw-r--r--   0        0        0    13650 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/container.py
--rw-r--r--   0        0        0    14172 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/control.py
--rw-r--r--   0        0        0      260 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/control_event.py
--rw-r--r--   0        0        0    20740 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/datatable.py
--rw-r--r--   0        0        0     2263 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/divider.py
--rw-r--r--   0        0        0     6270 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/drag_target.py
--rw-r--r--   0        0        0     6063 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/draggable.py
--rw-r--r--   0        0        0     9121 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/dropdown.py
--rw-r--r--   0        0        0     8066 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/elevated_button.py
--rw-r--r--   0        0        0     2166 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/embed_json_encoder.py
--rw-r--r--   0        0        0      166 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/event.py
--rw-r--r--   0        0        0     1839 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/event_handler.py
--rw-r--r--   0        0        0     9777 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/file_picker.py
--rw-r--r--   0        0        0     2505 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/filled_button.py
--rw-r--r--   0        0        0     2639 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/filled_tonal_button.py
--rw-r--r--   0        0        0     2542 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/flet_app.py
--rw-r--r--   0        0        0     6556 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/floating_action_button.py
--rw-r--r--   0        0        0    13925 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/form_field_control.py
--rw-r--r--   0        0        0    27963 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/gesture_detector.py
--rw-r--r--   0        0        0     1531 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/gradients.py
--rw-r--r--   0        0        0     6301 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/grid_view.py
--rw-r--r--   0        0        0     2134 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/haptic_feedback.py
--rw-r--r--   0        0        0     3375 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/icon.py
--rw-r--r--   0        0        0     7700 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/icon_button.py
--rw-r--r--   0        0        0   362652 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/icons.py
--rw-r--r--   0        0        0     6530 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/image.py
--rw-r--r--   0        0        0     7805 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/list_tile.py
--rw-r--r--   0        0        0     6206 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/list_view.py
--rw-r--r--   0        0        0     8668 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/local_connection.py
--rw-r--r--   0        0        0      235 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/locks.py
--rw-r--r--   0        0        0      583 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/margin.py
--rw-r--r--   0        0        0     5165 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/markdown.py
--rw-r--r--   0        0        0     5125 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/matplotlib_chart.py
--rw-r--r--   0        0        0     8322 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/navigation_bar.py
--rw-r--r--   0        0        0    11986 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/navigation_rail.py
--rw-r--r--   0        0        0     6751 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/outlined_button.py
--rw-r--r--   0        0        0      587 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/padding.py
--rw-r--r--   0        0        0    52348 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/page.py
--rw-r--r--   0        0        0     4355 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/plotly_chart.py
--rw-r--r--   0        0        0     6756 2023-04-17 18:18:07.061538 flet_core-0.6.0.dev1322/src/flet_core/popup_menu_button.py
--rw-r--r--   0        0        0     4237 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/progress_bar.py
--rw-r--r--   0        0        0     4435 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/progress_ring.py
--rw-r--r--   0        0        0     4100 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/protocol.py
--rw-r--r--   0        0        0     3470 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/querystring.py
--rw-r--r--   0        0        0     5731 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/radio.py
--rw-r--r--   0        0        0     2389 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/radio_group.py
--rw-r--r--   0        0        0      291 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/ref.py
--rw-r--r--   0        0        0     6354 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/responsive_row.py
--rw-r--r--   0        0        0     7289 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/row.py
--rw-r--r--   0        0        0     1637 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/semantics.py
--rw-r--r--   0        0        0      576 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/session_storage.py
--rw-r--r--   0        0        0     5318 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/shader_mask.py
--rw-r--r--   0        0        0      572 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/shadow.py
--rw-r--r--   0        0        0     2919 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/shake_detector.py
--rw-r--r--   0        0        0     7326 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/slider.py
--rw-r--r--   0        0        0     3971 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/snack_bar.py
--rw-r--r--   0        0        0     4833 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/stack.py
--rw-r--r--   0        0        0     8092 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/switch.py
--rw-r--r--   0        0        0     6776 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/tabs.py
--rw-r--r--   0        0        0      632 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/template_route.py
--rw-r--r--   0        0        0    10042 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/text.py
--rw-r--r--   0        0        0     6724 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/text_button.py
--rw-r--r--   0        0        0      594 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/text_style.py
--rw-r--r--   0        0        0    15388 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/textfield.py
--rw-r--r--   0        0        0     1482 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/theme.py
--rw-r--r--   0        0        0     8345 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/tooltip.py
--rw-r--r--   0        0        0      544 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/transform.py
--rw-r--r--   0        0        0     2753 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/transparent_pointer.py
--rw-r--r--   0        0        0     5134 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/types.py
--rw-r--r--   0        0        0      684 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/user_control.py
--rw-r--r--   0        0        0      409 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/utils.py
--rw-r--r--   0        0        0     2337 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/vertical_divider.py
--rw-r--r--   0        0        0     6225 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/view.py
--rw-r--r--   0        0        0     4049 2023-04-17 18:18:07.065538 flet_core-0.6.0.dev1322/src/flet_core/window_drag_area.py
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.6.0.dev1322/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/README.md
+-rw-r--r--   0        0        0      723 2023-04-19 23:41:11.935766 flet_core-0.6.0.dev1336/pyproject.toml
+-rw-r--r--   0        0        0     6035 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/__init__.py
+-rw-r--r--   0        0        0     6774 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/alert_dialog.py
+-rw-r--r--   0        0        0      407 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/alignment.py
+-rw-r--r--   0        0        0     7226 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/animated_switcher.py
+-rw-r--r--   0        0        0     2806 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/animation.py
+-rw-r--r--   0        0        0     5403 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/app_bar.py
+-rw-r--r--   0        0        0     7301 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/audio.py
+-rw-r--r--   0        0        0     5446 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/banner.py
+-rw-r--r--   0        0        0     1079 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/border.py
+-rw-r--r--   0        0        0      930 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/border_radius.py
+-rw-r--r--   0        0        0     2826 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/bottom_sheet.py
+-rw-r--r--   0        0        0     2202 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/buttons.py
+-rw-r--r--   0        0        0     3044 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/callable_control.py
+-rw-r--r--   0        0        0     5639 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/card.py
+-rw-r--r--   0        0        0     9855 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/bar_chart.py
+-rw-r--r--   0        0        0     2061 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0        0        0     6837 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0        0        0     1949 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0        0        0     2924 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/chart_axis.py
+-rw-r--r--   0        0        0     1293 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0        0        0      338 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0        0        0      286 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/chart_point_line.py
+-rw-r--r--   0        0        0     1006 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0        0        0    11228 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/line_chart.py
+-rw-r--r--   0        0        0     8258 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/line_chart_data.py
+-rw-r--r--   0        0        0     5496 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0        0        0     5888 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/pie_chart.py
+-rw-r--r--   0        0        0     3824 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0        0        0     7122 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/checkbox.py
+-rw-r--r--   0        0        0     6739 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/circle_avatar.py
+-rw-r--r--   0        0        0     3085 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/client_storage.py
+-rw-r--r--   0        0        0     1002 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/clipboard.py
+-rw-r--r--   0        0        0    10627 2023-04-19 23:40:35.334384 flet_core-0.6.0.dev1336/src/flet_core/colors.py
+-rw-r--r--   0        0        0     7305 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/column.py
+-rw-r--r--   0        0        0     1132 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/connection.py
+-rw-r--r--   0        0        0     6848 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/constrained_control.py
+-rw-r--r--   0        0        0    13660 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/container.py
+-rw-r--r--   0        0        0    14162 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/control.py
+-rw-r--r--   0        0        0      260 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/control_event.py
+-rw-r--r--   0        0        0    20740 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/datatable.py
+-rw-r--r--   0        0        0     2263 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/divider.py
+-rw-r--r--   0        0        0     6270 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/drag_target.py
+-rw-r--r--   0        0        0     6063 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/draggable.py
+-rw-r--r--   0        0        0     9121 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/dropdown.py
+-rw-r--r--   0        0        0     8066 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/elevated_button.py
+-rw-r--r--   0        0        0     2166 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/embed_json_encoder.py
+-rw-r--r--   0        0        0      166 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/event.py
+-rw-r--r--   0        0        0     1839 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/event_handler.py
+-rw-r--r--   0        0        0     9777 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/file_picker.py
+-rw-r--r--   0        0        0     2505 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/filled_button.py
+-rw-r--r--   0        0        0     2639 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/filled_tonal_button.py
+-rw-r--r--   0        0        0     2542 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/flet_app.py
+-rw-r--r--   0        0        0     6556 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/floating_action_button.py
+-rw-r--r--   0        0        0    13925 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/form_field_control.py
+-rw-r--r--   0        0        0    27963 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/gesture_detector.py
+-rw-r--r--   0        0        0     1531 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/gradients.py
+-rw-r--r--   0        0        0     6301 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/grid_view.py
+-rw-r--r--   0        0        0     2134 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/haptic_feedback.py
+-rw-r--r--   0        0        0     3375 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/icon.py
+-rw-r--r--   0        0        0     7700 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/icon_button.py
+-rw-r--r--   0        0        0   362652 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/icons.py
+-rw-r--r--   0        0        0     6530 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/image.py
+-rw-r--r--   0        0        0     7805 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/list_tile.py
+-rw-r--r--   0        0        0     6206 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/list_view.py
+-rw-r--r--   0        0        0     8644 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/local_connection.py
+-rw-r--r--   0        0        0      223 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/locks.py
+-rw-r--r--   0        0        0      583 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/margin.py
+-rw-r--r--   0        0        0     5165 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/markdown.py
+-rw-r--r--   0        0        0     5125 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/matplotlib_chart.py
+-rw-r--r--   0        0        0     8322 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/navigation_bar.py
+-rw-r--r--   0        0        0    11986 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/navigation_rail.py
+-rw-r--r--   0        0        0     6751 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/outlined_button.py
+-rw-r--r--   0        0        0      587 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/padding.py
+-rw-r--r--   0        0        0    52360 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/page.py
+-rw-r--r--   0        0        0     4355 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/plotly_chart.py
+-rw-r--r--   0        0        0     6756 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/popup_menu_button.py
+-rw-r--r--   0        0        0     4237 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/progress_bar.py
+-rw-r--r--   0        0        0     4435 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/progress_ring.py
+-rw-r--r--   0        0        0     4088 2023-04-19 23:40:35.338384 flet_core-0.6.0.dev1336/src/flet_core/protocol.py
+-rw-r--r--   0        0        0     3419 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/querystring.py
+-rw-r--r--   0        0        0     5731 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/radio.py
+-rw-r--r--   0        0        0     2389 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/radio_group.py
+-rw-r--r--   0        0        0      291 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/ref.py
+-rw-r--r--   0        0        0     6354 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/responsive_row.py
+-rw-r--r--   0        0        0     7289 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/row.py
+-rw-r--r--   0        0        0     1637 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/semantics.py
+-rw-r--r--   0        0        0      576 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/session_storage.py
+-rw-r--r--   0        0        0     5318 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/shader_mask.py
+-rw-r--r--   0        0        0      572 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/shadow.py
+-rw-r--r--   0        0        0     2919 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/shake_detector.py
+-rw-r--r--   0        0        0     7326 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/slider.py
+-rw-r--r--   0        0        0     3971 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/snack_bar.py
+-rw-r--r--   0        0        0     4833 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/stack.py
+-rw-r--r--   0        0        0     8092 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/switch.py
+-rw-r--r--   0        0        0     6776 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/tabs.py
+-rw-r--r--   0        0        0      632 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/template_route.py
+-rw-r--r--   0        0        0    10042 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/text.py
+-rw-r--r--   0        0        0     6724 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/text_button.py
+-rw-r--r--   0        0        0      594 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/text_style.py
+-rw-r--r--   0        0        0    15388 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/textfield.py
+-rw-r--r--   0        0        0     1482 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/theme.py
+-rw-r--r--   0        0        0     8345 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/tooltip.py
+-rw-r--r--   0        0        0      544 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/transform.py
+-rw-r--r--   0        0        0     2753 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/transparent_pointer.py
+-rw-r--r--   0        0        0     5134 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/types.py
+-rw-r--r--   0        0        0      684 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/user_control.py
+-rw-r--r--   0        0        0      409 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/utils.py
+-rw-r--r--   0        0        0     2337 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/vertical_divider.py
+-rw-r--r--   0        0        0     6225 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/view.py
+-rw-r--r--   0        0        0     4049 2023-04-19 23:40:35.342384 flet_core-0.6.0.dev1336/src/flet_core/window_drag_area.py
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.6.0.dev1336/PKG-INFO
```

### Comparing `flet_core-0.6.0.dev1322/pyproject.toml` & `flet_core-0.6.0.dev1336/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-core"
-version = "0.6.0.dev1322"
+version = "0.6.0.dev1336"
 description = "Flet core library"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_core", from = "src" },
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/__init__.py` & `flet_core-0.6.0.dev1336/src/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/alert_dialog.py` & `flet_core-0.6.0.dev1336/src/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/animated_switcher.py` & `flet_core-0.6.0.dev1336/src/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/animation.py` & `flet_core-0.6.0.dev1336/src/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/app_bar.py` & `flet_core-0.6.0.dev1336/src/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/audio.py` & `flet_core-0.6.0.dev1336/src/flet_core/audio.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/banner.py` & `flet_core-0.6.0.dev1336/src/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/border.py` & `flet_core-0.6.0.dev1336/src/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/border_radius.py` & `flet_core-0.6.0.dev1336/src/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/bottom_sheet.py` & `flet_core-0.6.0.dev1336/src/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/buttons.py` & `flet_core-0.6.0.dev1336/src/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/callable_control.py` & `flet_core-0.6.0.dev1336/src/flet_core/callable_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,17 @@
         assert evt is not None
         if not evt.wait(5):
             del self.__calls[m.i]
             raise Exception(
                 f"Timeout waiting for {self.__class__.__name__}.{name}({params}) method call"
             )
         result, err = self.__results.pop(evt)
-        if err != None:
+        if err is not None:
             raise Exception(err)
-        if result == None:
+        if result is None:
             return None
         return json.loads(result)
 
     async def _call_method_async(
         self, name: str, params: List[str], wait_for_result=True
     ) -> Any:
         m = ControlMethodCall(i=self.__call_counter, n=name, p=params)
@@ -92,21 +92,21 @@
         except TimeoutError:
             del self.__calls[m.i]
             raise Exception(
                 f"Timeout waiting for {self.__class__.__name__}.{name}({params}) method call"
             )
 
         result, err = self.__results.pop(evt)
-        if err != None:
+        if err is not None:
             raise Exception(err)
-        if result == None:
+        if result is None:
             return None
         return json.loads(result)
 
     def _on_result(self, e):
         d = json.loads(e.data)
         result = ControlMethodResults(**d)
         evt = self.__calls.pop(result.i, None)
-        if evt == None:
+        if evt is None:
             return
         self.__results[evt] = (result.r, result.e)
         evt.set()
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/card.py` & `flet_core-0.6.0.dev1336/src/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/bar_chart.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/bar_chart_group.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/bar_chart_rod.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/chart_axis.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/chart_axis_label.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/chart_point_shape.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/line_chart.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/line_chart_data.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/line_chart_data_point.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/pie_chart.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/charts/pie_chart_section.py` & `flet_core-0.6.0.dev1336/src/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/checkbox.py` & `flet_core-0.6.0.dev1336/src/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/circle_avatar.py` & `flet_core-0.6.0.dev1336/src/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/client_storage.py` & `flet_core-0.6.0.dev1336/src/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/clipboard.py` & `flet_core-0.6.0.dev1336/src/flet_core/clipboard.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/colors.py` & `flet_core-0.6.0.dev1336/src/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/column.py` & `flet_core-0.6.0.dev1336/src/flet_core/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,17 +223,17 @@
         self.__scroll = value
         if isinstance(value, ScrollMode):
             self._set_attr("scroll", value.value)
         else:
             self.__set_scroll(value)
 
     def __set_scroll(self, value: Optional[ScrollModeString]):
-        if value == True:
+        if value is True:
             value = "auto"
-        elif value == False:
+        elif value is False:
             value = None
         self._set_attr("scroll", value)
 
     # auto_scroll
     @property
     def auto_scroll(self) -> Optional[bool]:
         return self._get_attr("autoScroll")
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/connection.py` & `flet_core-0.6.0.dev1336/src/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/constrained_control.py` & `flet_core-0.6.0.dev1336/src/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/container.py` & `flet_core-0.6.0.dev1336/src/flet_core/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ResponsiveNumber,
     RotateValue,
     ScaleValue,
 )
 
 try:
     from typing import Literal
-except:
+except Exception:
     from typing_extensions import Literal
 
 
 class BlurTileMode(Enum):
     CLAMP = "clamp"
     DECAL = "decal"
     MIRROR = "mirror"
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/control.py` & `flet_core-0.6.0.dev1336/src/flet_core/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             return value
         return {"": value}
 
     def __str__(self):
         attrs = {}
         for k, v in self.__attrs.items():
             attrs[k] = v[0]
-        return "{} {}".format(self._get_control_name(), attrs)
+        return f"{self._get_control_name()} {attrs}"
 
     # event_handlers
     @property
     def event_handlers(self):
         return self.__event_handlers
 
     # _previous_children
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/datatable.py` & `flet_core-0.6.0.dev1336/src/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/divider.py` & `flet_core-0.6.0.dev1336/src/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/drag_target.py` & `flet_core-0.6.0.dev1336/src/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/draggable.py` & `flet_core-0.6.0.dev1336/src/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/dropdown.py` & `flet_core-0.6.0.dev1336/src/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/elevated_button.py` & `flet_core-0.6.0.dev1336/src/flet_core/elevated_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/embed_json_encoder.py` & `flet_core-0.6.0.dev1336/src/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/event_handler.py` & `flet_core-0.6.0.dev1336/src/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/file_picker.py` & `flet_core-0.6.0.dev1336/src/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/filled_button.py` & `flet_core-0.6.0.dev1336/src/flet_core/filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/filled_tonal_button.py` & `flet_core-0.6.0.dev1336/src/flet_core/filled_tonal_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/flet_app.py` & `flet_core-0.6.0.dev1336/src/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/floating_action_button.py` & `flet_core-0.6.0.dev1336/src/flet_core/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/form_field_control.py` & `flet_core-0.6.0.dev1336/src/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/gesture_detector.py` & `flet_core-0.6.0.dev1336/src/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/gradients.py` & `flet_core-0.6.0.dev1336/src/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/grid_view.py` & `flet_core-0.6.0.dev1336/src/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/haptic_feedback.py` & `flet_core-0.6.0.dev1336/src/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/icon.py` & `flet_core-0.6.0.dev1336/src/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/icon_button.py` & `flet_core-0.6.0.dev1336/src/flet_core/icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/icons.py` & `flet_core-0.6.0.dev1336/src/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/image.py` & `flet_core-0.6.0.dev1336/src/flet_core/image.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/list_tile.py` & `flet_core-0.6.0.dev1336/src/flet_core/list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/list_view.py` & `flet_core-0.6.0.dev1336/src/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/local_connection.py` & `flet_core-0.6.0.dev1336/src/flet_core/local_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,30 +70,30 @@
             sessionID=self._client_details.sessionId,
             eventTarget="page",
             eventName="change",
             eventData=json.dumps(msg.payload["props"], separators=(",", ":")),
         )
 
     def _process_command(self, command: Command):
-        logger.debug("_process_command: {}".format(command))
+        logger.debug(f"_process_command: {command}")
         if command.name == "get":
             return self._process_get_command(command.values)
         elif command.name == "add":
             return self._process_add_command(command)
         elif command.name == "set":
             return self._process_set_command(command.values, command.attrs)
         elif command.name == "remove":
             return self._process_remove_command(command.values)
         elif command.name == "clean":
             return self._process_clean_command(command.values)
         elif command.name == "invokeMethod":
             return self._process_invoke_method_command(command.values, command.attrs)
         elif command.name == "error":
             return self._process_error_command(command.values)
-        raise Exception("Unsupported command: {}".format(command.name))
+        raise Exception(f"Unsupported command: {command.name}")
 
     def _process_add_command(self, command: Command):
 
         top_parent_id = command.attrs.get("to", "page")
         top_parent_at = int(command.attrs.get("at", "-1"))
 
         batch: List[Command] = []
@@ -127,15 +127,15 @@
             # parent wasn't found - use the topmost one
             if parent_id == "":
                 parent_id = top_parent_id
                 parent_at = top_parent_at
 
             id = cmd.attrs.get("id", "")
             if not id:
-                id = "_{}".format(self._control_id)
+                id = f"_{self._control_id}"
                 self._control_id += 1
                 cmd.attrs["id"] = id
 
             ids.append(id)
 
             control = {"t": control_type, "i": id, "p": parent_id, "c": []}
             controls.append(control)
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/margin.py` & `flet_core-0.6.0.dev1336/src/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/markdown.py` & `flet_core-0.6.0.dev1336/src/flet_core/markdown.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/matplotlib_chart.py` & `flet_core-0.6.0.dev1336/src/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/navigation_bar.py` & `flet_core-0.6.0.dev1336/src/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/navigation_rail.py` & `flet_core-0.6.0.dev1336/src/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/outlined_button.py` & `flet_core-0.6.0.dev1336/src/flet_core/outlined_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/padding.py` & `flet_core-0.6.0.dev1336/src/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/page.py` & `flet_core-0.6.0.dev1336/src/flet_core/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
 
         return commands, added_controls, removed_controls
 
     def __validate_controls_page(self, added_controls):
         for ctrl in added_controls:
             if ctrl.page and ctrl.page != self:
                 raise Exception(
-                    "Control has already been added to another page: {}".format(ctrl)
+                    f"Control has already been added to another page: {ctrl}"
                 )
 
     def __update_control_ids(self, added_controls, results):
         if len(results) > 0:
             n = 0
             for line in results:
                 for id in line.split(" "):
@@ -482,30 +482,30 @@
             id = props["i"]
             if id in self._index:
                 for name in props:
                     if name != "i":
                         self._index[id]._set_attr(name, props[name], dirty=False)
 
     def go(self, route, **kwargs):
-        self.route = route if kwargs == {} else route + self.query.post(kwargs)
+        self.route = route if not kwargs else route + self.query.post(kwargs)
 
         self.__on_route_change.get_sync_handler()(
             ControlEvent(
                 target="page",
                 name="route_change",
                 data=self.route,
                 page=self,
                 control=self,
             )
         )
         self.update()
         self.query()  # Update query url (required when using go)
 
     async def go_async(self, route, **kwargs):
-        self.route = route if kwargs == {} else route + self.query.post(kwargs)
+        self.route = route if not kwargs else route + self.query.post(kwargs)
 
         await self.__on_route_change.get_handler()(
             ControlEvent(
                 target="page",
                 name="route_change",
                 data=self.route,
                 page=self,
@@ -772,21 +772,21 @@
         url: str,
         web_window_name: Optional[str] = None,
         web_popup_window: bool = False,
         window_width: Optional[int] = None,
         window_height: Optional[int] = None,
     ):
         args = {"url": url}
-        if web_window_name != None:
+        if web_window_name is not None:
             args["web_window_name"] = web_window_name
-        if web_popup_window != None:
+        if web_popup_window is not None:
             args["web_popup_window"] = str(web_popup_window)
-        if window_width != None:
+        if window_width is not None:
             args["window_width"] = str(window_width)
-        if window_height != None:
+        if window_height is not None:
             args["window_height"] = str(window_height)
         return args
 
     def can_launch_url(self, url: str):
         args = {"url": url}
         return self.invoke_method("canLaunchUrl", args, wait_for_result=True) == "true"
 
@@ -841,17 +841,17 @@
         if not evt.wait(5):
             del self.__method_calls[method_id]
             raise Exception(
                 f"Timeout waiting for invokeMethod {method_name}({arguments}) call"
             )
 
         result, err = self.__method_call_results.pop(evt)
-        if err != None:
+        if err is not None:
             raise Exception(err)
-        if result == None:
+        if result is None:
             return None
         return result
 
     async def invoke_method_async(
         self,
         method_name: str,
         arguments: Optional[Dict[str, str]] = None,
@@ -885,25 +885,25 @@
         except TimeoutError:
             del self.__method_calls[method_id]
             raise Exception(
                 f"Timeout waiting for invokeMethod {method_name}({arguments}) call"
             )
 
         result, err = self.__method_call_results.pop(evt)
-        if err != None:
+        if err is not None:
             raise Exception(err)
-        if result == None:
+        if result is None:
             return None
         return result
 
     def __on_invoke_method_result(self, e):
         d = json.loads(e.data)
         result = InvokeMethodResults(**d)
         evt = self.__method_calls.pop(result.method_id, None)
-        if evt == None:
+        if evt is None:
             return
         self.__method_call_results[evt] = (result.result, result.error)
         evt.set()
 
     def show_snack_bar(self, snack_bar: SnackBar):
         self.__offstage.snack_bar = snack_bar
         self.__offstage.update()
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/plotly_chart.py` & `flet_core-0.6.0.dev1336/src/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/popup_menu_button.py` & `flet_core-0.6.0.dev1336/src/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/progress_bar.py` & `flet_core-0.6.0.dev1336/src/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/progress_ring.py` & `flet_core-0.6.0.dev1336/src/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/protocol.py` & `flet_core-0.6.0.dev1336/src/flet_core/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     indent: int
     name: Optional[str]
     values: List[str] = field(default_factory=list)
     attrs: Dict[str, str] = field(default_factory=dict)
     commands: List[Any] = field(default_factory=list)
 
     def __str__(self):
-        return "{} {} {}".format(self.name, self.values, self.attrs)
+        return f"{self.name} {self.values} {self.attrs}"
 
 
 @dataclass
 class Message:
     id: str
     action: str
     payload: Any
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/querystring.py` & `flet_core-0.6.0.dev1336/src/flet_core/querystring.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,20 +24,18 @@
     def _is_encoded(self) -> bool:
         """
         Function returns True if URL is already encoded
         """
         if "?" in self.url:
             q_result = self._querystring_part()
             return (
-                True
-                if self._decode_url_component(
+                self._decode_url_component(
                     self.url[q_result.start() + 1 : q_result.end()]
                 )
                 != self.url[q_result.start() + 1 : q_result.end()]
-                else False
             )
 
     def _querystring_part(self, url_string: bool = False):
         """
         Function sliced url part and returns querystring part.\n
         Use case: checking querystring part for encode, assiging decoded value
         """
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/radio.py` & `flet_core-0.6.0.dev1336/src/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/radio_group.py` & `flet_core-0.6.0.dev1336/src/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/responsive_row.py` & `flet_core-0.6.0.dev1336/src/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/row.py` & `flet_core-0.6.0.dev1336/src/flet_core/row.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,17 +226,17 @@
         self.__scroll = value
         if isinstance(value, ScrollMode):
             self._set_attr("scroll", value.value)
         else:
             self.__set_scroll(value)
 
     def __set_scroll(self, value: Optional[ScrollModeString]):
-        if value == True:
+        if value is True:
             value = "auto"
-        elif value == False:
+        elif value is False:
             value = None
         self._set_attr("scroll", value)
 
     # auto_scroll
     @property
     def auto_scroll(self) -> Optional[bool]:
         return self._get_attr("autoScroll")
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/semantics.py` & `flet_core-0.6.0.dev1336/src/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/session_storage.py` & `flet_core-0.6.0.dev1336/src/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/shader_mask.py` & `flet_core-0.6.0.dev1336/src/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/shadow.py` & `flet_core-0.6.0.dev1336/src/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/shake_detector.py` & `flet_core-0.6.0.dev1336/src/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/slider.py` & `flet_core-0.6.0.dev1336/src/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/snack_bar.py` & `flet_core-0.6.0.dev1336/src/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/stack.py` & `flet_core-0.6.0.dev1336/src/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/switch.py` & `flet_core-0.6.0.dev1336/src/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/tabs.py` & `flet_core-0.6.0.dev1336/src/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/template_route.py` & `flet_core-0.6.0.dev1336/src/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/text.py` & `flet_core-0.6.0.dev1336/src/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/text_button.py` & `flet_core-0.6.0.dev1336/src/flet_core/text_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/text_style.py` & `flet_core-0.6.0.dev1336/src/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/textfield.py` & `flet_core-0.6.0.dev1336/src/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/theme.py` & `flet_core-0.6.0.dev1336/src/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/tooltip.py` & `flet_core-0.6.0.dev1336/src/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/transform.py` & `flet_core-0.6.0.dev1336/src/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/transparent_pointer.py` & `flet_core-0.6.0.dev1336/src/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/types.py` & `flet_core-0.6.0.dev1336/src/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/user_control.py` & `flet_core-0.6.0.dev1336/src/flet_core/user_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/vertical_divider.py` & `flet_core-0.6.0.dev1336/src/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/view.py` & `flet_core-0.6.0.dev1336/src/flet_core/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,17 +189,17 @@
         self.__scroll = value
         if isinstance(value, ScrollMode):
             self._set_attr("scroll", value.value)
         else:
             self.__set_scroll(value)
 
     def __set_scroll(self, value: Optional[ScrollModeString]):
-        if value == True:
+        if value is True:
             value = "auto"
-        elif value == False:
+        elif value is False:
             value = None
         self._set_attr("scroll", value)
 
     # auto_scroll
     @property
     def auto_scroll(self) -> Optional[bool]:
         return self._get_attr("autoScroll")
```

### Comparing `flet_core-0.6.0.dev1322/src/flet_core/window_drag_area.py` & `flet_core-0.6.0.dev1336/src/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1322/PKG-INFO` & `flet_core-0.6.0.dev1336/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-core
-Version: 0.6.0.dev1322
+Version: 0.6.0.dev1336
 Summary: Flet core library
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

