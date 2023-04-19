# Comparing `tmp/atri_react-1.0.0a13.tar.gz` & `tmp/atri_react-1.0.0a26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atri_react-1.0.0a13.tar", last modified: Wed Mar 29 11:39:12 2023, max compression
+gzip compressed data, was "atri_react-1.0.0a26.tar", last modified: Wed Apr 19 22:16:38 2023, max compression
```

## Comparing `atri_react-1.0.0a13.tar` & `atri_react-1.0.0a26.tar`

### file list

```diff
@@ -1,75 +1,78 @@
-drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-03-29 11:39:12.290452 atri_react-1.0.0a13/
--rw-r--r--   0 shyamswaroop   (501) staff       (20)      331 2023-03-29 11:39:12.289867 atri_react-1.0.0a13/PKG-INFO
--rw-r--r--   0 shyamswaroop   (501) staff       (20)       80 2023-03-12 04:38:00.000000 atri_react-1.0.0a13/pyproject.toml
--rw-r--r--   0 shyamswaroop   (501) staff       (20)       38 2023-03-29 11:39:12.290786 atri_react-1.0.0a13/setup.cfg
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1072 2023-03-27 19:17:10.000000 atri_react-1.0.0a13/setup.py
-drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-03-29 11:39:12.210456 atri_react-1.0.0a13/src/
-drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-03-29 11:39:12.283763 atri_react-1.0.0a13/src/atri_react/
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4005 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Accordion.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4201 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Alert.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4073 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Anchor.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4173 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/AreaChart.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     5914 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Badge.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4514 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/BarChart.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1722 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Breadcrumb.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3929 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Button.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3836 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/CandleStick.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3708 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Card.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2792 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Carousel.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     8620 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Cascader.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1679 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Checkbox.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)    13818 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/CodeMirror.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3780 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Countdown.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1726 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Countup.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2079 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/DatePicker.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1011 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Div.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1859 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Dropdown.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1015 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Flex.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     5190 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Form.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4486 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/GanttChart.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3848 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/HistogramChart.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1305 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Icon.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1606 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Image.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     6801 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Input.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     6666 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/InputNumber.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4173 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/LineChart.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1971 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Link.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4822 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Menu.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     5914 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Modal.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1774 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Overlay.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3419 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/PieChart.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2321 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Radio.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3591 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Rating.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2532 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Repeating.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4506 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/ScatterChart.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     6364 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Search.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2517 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Select.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4496 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Slider.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4694 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Statistic.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4161 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Step.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3569 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Table.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3831 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Tabs.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3716 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Tag.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2215 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Testimonial.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1329 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/TextBox.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     4599 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Textarea.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3423 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/TimePicker.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2705 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Timeline.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2160 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Toggle.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3466 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Tree.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2448 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/TreemapChart.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     7908 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/UnorderedList.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     3543 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Upload.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1409 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/VerticalMenu.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     7273 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/Video.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1684 2023-03-28 18:48:45.000000 atri_react-1.0.0a13/src/atri_react/__init__.py
-drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-03-29 11:39:12.288162 atri_react-1.0.0a13/src/atri_react.egg-info/
--rw-r--r--   0 shyamswaroop   (501) staff       (20)      331 2023-03-29 11:39:12.000000 atri_react-1.0.0a13/src/atri_react.egg-info/PKG-INFO
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     1821 2023-03-29 11:39:12.000000 atri_react-1.0.0a13/src/atri_react.egg-info/SOURCES.txt
--rw-r--r--   0 shyamswaroop   (501) staff       (20)        1 2023-03-29 11:39:12.000000 atri_react-1.0.0a13/src/atri_react.egg-info/dependency_links.txt
--rw-r--r--   0 shyamswaroop   (501) staff       (20)        1 2023-03-13 04:01:34.000000 atri_react-1.0.0a13/src/atri_react.egg-info/not-zip-safe
--rw-r--r--   0 shyamswaroop   (501) staff       (20)       10 2023-03-29 11:39:12.000000 atri_react-1.0.0a13/src/atri_react.egg-info/requires.txt
--rw-r--r--   0 shyamswaroop   (501) staff       (20)       18 2023-03-29 11:39:12.000000 atri_react-1.0.0a13/src/atri_react.egg-info/top_level.txt
-drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-03-29 11:39:12.289253 atri_react-1.0.0a13/src/config/
--rw-r--r--   0 shyamswaroop   (501) staff       (20)        0 2023-03-28 18:48:35.000000 atri_react-1.0.0a13/src/config/__init__.py
--rw-r--r--   0 shyamswaroop   (501) staff       (20)     2489 2023-03-28 18:48:35.000000 atri_react-1.0.0a13/src/config/package.json
+drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-04-19 22:16:38.008670 atri_react-1.0.0a26/
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)      331 2023-04-19 22:16:38.008169 atri_react-1.0.0a26/PKG-INFO
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)       80 2023-03-12 04:38:00.000000 atri_react-1.0.0a26/pyproject.toml
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)       38 2023-04-19 22:16:38.008834 atri_react-1.0.0a26/setup.cfg
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1072 2023-03-27 19:17:10.000000 atri_react-1.0.0a26/setup.py
+drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-04-19 22:16:37.935983 atri_react-1.0.0a26/src/
+drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-04-19 22:16:37.999641 atri_react-1.0.0a26/src/atri_react/
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4145 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Accordion.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4341 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Alert.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4213 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Anchor.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4313 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/AreaChart.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     6054 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Badge.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4654 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/BarChart.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1862 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Breadcrumb.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4378 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Button.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3976 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/CandleStick.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4193 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Card.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2932 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Carousel.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     8760 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Cascader.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2902 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Checkbox.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)    13958 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/CodeMirror.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3920 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Countdown.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1866 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Countup.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4634 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/DatePicker.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1151 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Div.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     5470 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Drawer.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1999 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Dropdown.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1155 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Flex.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     5330 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Form.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4626 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/GanttChart.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3988 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/HistogramChart.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1445 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Icon.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3479 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Iframe.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1746 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Image.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     6941 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Input.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     6806 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/InputNumber.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4313 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/LineChart.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2111 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Link.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4962 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Menu.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     5819 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Modal.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1914 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Overlay.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3559 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/PieChart.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3973 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Radio.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3731 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Rating.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2689 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Repeating.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4646 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/ScatterChart.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     6504 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Search.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2657 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Select.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4636 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Slider.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4834 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Statistic.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3932 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Step.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3709 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Table.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4424 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Tabs.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3856 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Tag.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2355 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Testimonial.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1469 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/TextBox.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4739 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Textarea.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     4325 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/TimePicker.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2845 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Timeline.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     6737 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/TinyMCE.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2300 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Toggle.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3606 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Tree.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2588 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/TreemapChart.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     8048 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/UnorderedList.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     3683 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Upload.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1549 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/VerticalMenu.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     7413 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/Video.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1767 2023-04-19 22:16:10.000000 atri_react-1.0.0a26/src/atri_react/__init__.py
+drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-04-19 22:16:38.005756 atri_react-1.0.0a26/src/atri_react.egg-info/
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)      331 2023-04-19 22:16:37.000000 atri_react-1.0.0a26/src/atri_react.egg-info/PKG-INFO
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     1897 2023-04-19 22:16:37.000000 atri_react-1.0.0a26/src/atri_react.egg-info/SOURCES.txt
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)        1 2023-04-19 22:16:37.000000 atri_react-1.0.0a26/src/atri_react.egg-info/dependency_links.txt
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)        1 2023-03-13 04:01:34.000000 atri_react-1.0.0a26/src/atri_react.egg-info/not-zip-safe
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)       10 2023-04-19 22:16:37.000000 atri_react-1.0.0a26/src/atri_react.egg-info/requires.txt
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)       18 2023-04-19 22:16:37.000000 atri_react-1.0.0a26/src/atri_react.egg-info/top_level.txt
+drwxr-xr-x   0 shyamswaroop   (501) staff       (20)        0 2023-04-19 22:16:38.007401 atri_react-1.0.0a26/src/config/
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)        0 2023-04-19 22:16:01.000000 atri_react-1.0.0a26/src/config/__init__.py
+-rw-r--r--   0 shyamswaroop   (501) staff       (20)     2504 2023-04-19 22:16:01.000000 atri_react-1.0.0a26/src/config/package.json
```

### Comparing `atri_react-1.0.0a13/setup.py` & `atri_react-1.0.0a26/setup.py`

 * *Files identical despite different names*

### Comparing `atri_react-1.0.0a13/src/atri_react/Accordion.py` & `atri_react-1.0.0a26/src/atri_react/Accordion.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,24 +80,25 @@
 		return self._items
 	@items.setter
 	def items(self, state):
 		self._setter_access_tracker["items"] = {}
 		self._items = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"size": self._size,
 			"expandIconPosition": self._expandIconPosition,
 			"collapse": self._collapse,
 			"bordered": self._bordered,
 			"ghost": self._ghost,
 			"defaultActiveKey": self._defaultActiveKey,
 			"expandIcon": self._expandIcon,
 			"items": self._items
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Accordion(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -114,11 +115,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = AccordionCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Alert.py` & `atri_react-1.0.0a26/src/atri_react/Card.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class AlertCustomClass():
+class CardCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
+		self.type: Union[Any, None] = state["type"] if state != None and "type" in state else None
 		self.text: Union[Any, None] = state["text"] if state != None and "text" in state else None
 		self.description: Union[Any, None] = state["description"] if state != None and "description" in state else None
-		self.alertType: Union[Any, None] = state["alertType"] if state != None and "alertType" in state else None
-		self.showIcon: Union[Any, None] = state["showIcon"] if state != None and "showIcon" in state else None
-		self.icon: Union[Any, None] = state["icon"] if state != None and "icon" in state else None
-		self.isClosable: Union[Any, None] = state["isClosable"] if state != None and "isClosable" in state else None
-		self.closeText: Union[Any, None] = state["closeText"] if state != None and "closeText" in state else None
-		self.closeIcon: Union[Any, None] = state["closeIcon"] if state != None and "closeIcon" in state else None
-		self.banner: Union[Any, None] = state["banner"] if state != None and "banner" in state else None
+		self.size: Union[Any, None] = state["size"] if state != None and "size" in state else None
+		self.loading: Union[Any, None] = state["loading"] if state != None and "loading" in state else None
+		self.hoverable: Union[Any, None] = state["hoverable"] if state != None and "hoverable" in state else None
+		self.bordered: Union[Any, None] = state["bordered"] if state != None and "bordered" in state else None
+		self.cover: Union[Any, None] = state["cover"] if state != None and "cover" in state else None
+		self.avatar: Union[Any, None] = state["avatar"] if state != None and "avatar" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
+	def type(self):
+		self._getter_access_tracker["type"] = {}
+		return self._type
+	@type.setter
+	def type(self, state):
+		self._setter_access_tracker["type"] = {}
+		self._type = state
+	@property
 	def text(self):
 		self._getter_access_tracker["text"] = {}
 		return self._text
 	@text.setter
 	def text(self, state):
 		self._setter_access_tracker["text"] = {}
 		self._text = state
@@ -32,103 +40,97 @@
 		self._getter_access_tracker["description"] = {}
 		return self._description
 	@description.setter
 	def description(self, state):
 		self._setter_access_tracker["description"] = {}
 		self._description = state
 	@property
-	def alertType(self):
-		self._getter_access_tracker["alertType"] = {}
-		return self._alertType
-	@alertType.setter
-	def alertType(self, state):
-		self._setter_access_tracker["alertType"] = {}
-		self._alertType = state
-	@property
-	def showIcon(self):
-		self._getter_access_tracker["showIcon"] = {}
-		return self._showIcon
-	@showIcon.setter
-	def showIcon(self, state):
-		self._setter_access_tracker["showIcon"] = {}
-		self._showIcon = state
-	@property
-	def icon(self):
-		self._getter_access_tracker["icon"] = {}
-		return self._icon
-	@icon.setter
-	def icon(self, state):
-		self._setter_access_tracker["icon"] = {}
-		self._icon = state
-	@property
-	def isClosable(self):
-		self._getter_access_tracker["isClosable"] = {}
-		return self._isClosable
-	@isClosable.setter
-	def isClosable(self, state):
-		self._setter_access_tracker["isClosable"] = {}
-		self._isClosable = state
-	@property
-	def closeText(self):
-		self._getter_access_tracker["closeText"] = {}
-		return self._closeText
-	@closeText.setter
-	def closeText(self, state):
-		self._setter_access_tracker["closeText"] = {}
-		self._closeText = state
-	@property
-	def closeIcon(self):
-		self._getter_access_tracker["closeIcon"] = {}
-		return self._closeIcon
-	@closeIcon.setter
-	def closeIcon(self, state):
-		self._setter_access_tracker["closeIcon"] = {}
-		self._closeIcon = state
-	@property
-	def banner(self):
-		self._getter_access_tracker["banner"] = {}
-		return self._banner
-	@banner.setter
-	def banner(self, state):
-		self._setter_access_tracker["banner"] = {}
-		self._banner = state
+	def size(self):
+		self._getter_access_tracker["size"] = {}
+		return self._size
+	@size.setter
+	def size(self, state):
+		self._setter_access_tracker["size"] = {}
+		self._size = state
+	@property
+	def loading(self):
+		self._getter_access_tracker["loading"] = {}
+		return self._loading
+	@loading.setter
+	def loading(self, state):
+		self._setter_access_tracker["loading"] = {}
+		self._loading = state
+	@property
+	def hoverable(self):
+		self._getter_access_tracker["hoverable"] = {}
+		return self._hoverable
+	@hoverable.setter
+	def hoverable(self, state):
+		self._setter_access_tracker["hoverable"] = {}
+		self._hoverable = state
+	@property
+	def bordered(self):
+		self._getter_access_tracker["bordered"] = {}
+		return self._bordered
+	@bordered.setter
+	def bordered(self, state):
+		self._setter_access_tracker["bordered"] = {}
+		self._bordered = state
+	@property
+	def cover(self):
+		self._getter_access_tracker["cover"] = {}
+		return self._cover
+	@cover.setter
+	def cover(self, state):
+		self._setter_access_tracker["cover"] = {}
+		self._cover = state
+	@property
+	def avatar(self):
+		self._getter_access_tracker["avatar"] = {}
+		return self._avatar
+	@avatar.setter
+	def avatar(self, state):
+		self._setter_access_tracker["avatar"] = {}
+		self._avatar = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
+			"type": self._type,
 			"text": self._text,
 			"description": self._description,
-			"alertType": self._alertType,
-			"showIcon": self._showIcon,
-			"icon": self._icon,
-			"isClosable": self._isClosable,
-			"closeText": self._closeText,
-			"closeIcon": self._closeIcon,
-			"banner": self._banner
+			"size": self._size,
+			"loading": self._loading,
+			"hoverable": self._hoverable,
+			"bordered": self._bordered,
+			"cover": self._cover,
+			"avatar": self._avatar
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class Alert(AtriComponent):
+class Card(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "Alert"
+		self.compKey = "Card"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		self.onClick = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = AlertCustomClass(state)
+		self._custom = CardCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Anchor.py` & `atri_react-1.0.0a26/src/atri_react/Anchor.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,25 +89,26 @@
 		return self._disabled
 	@disabled.setter
 	def disabled(self, state):
 		self._setter_access_tracker["disabled"] = {}
 		self._disabled = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"href": self._href,
 			"download": self._download,
 			"referrerPolicy": self._referrerPolicy,
 			"rel": self._rel,
 			"target": self._target,
 			"hreflang": self._hreflang,
 			"ping": self._ping,
 			"type": self._type,
 			"disabled": self._disabled
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Anchor(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -124,11 +125,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = AnchorCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/AreaChart.py` & `atri_react-1.0.0a26/src/atri_react/LineChart.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class AreaChartCustomClass():
+class LineChartCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
 		self.cartesianGrid: Union[Any, None] = state["cartesianGrid"] if state != None and "cartesianGrid" in state else None
 		self.data: Union[Any, None] = state["data"] if state != None and "data" in state else None
 		self.options: Union[Any, None] = state["options"] if state != None and "options" in state else None
 		self.toolTip: Union[Any, None] = state["toolTip"] if state != None and "toolTip" in state else None
@@ -89,46 +89,48 @@
 		return self._chartWidth
 	@chartWidth.setter
 	def chartWidth(self, state):
 		self._setter_access_tracker["chartWidth"] = {}
 		self._chartWidth = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"cartesianGrid": self._cartesianGrid,
 			"data": self._data,
 			"options": self._options,
 			"toolTip": self._toolTip,
 			"legend": self._legend,
 			"xAxis": self._xAxis,
 			"yAxis": self._yAxis,
 			"chartHeight": self._chartHeight,
 			"chartWidth": self._chartWidth
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class AreaChart(AtriComponent):
+class LineChart(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "AreaChart"
+		self.compKey = "LineChart"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = AreaChartCustomClass(state)
+		self._custom = LineChartCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Badge.py` & `atri_react-1.0.0a26/src/atri_react/Badge.py`

 * *Files 8% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 		return self._ribbonColor
 	@ribbonColor.setter
 	def ribbonColor(self, state):
 		self._setter_access_tracker["ribbonColor"] = {}
 		self._ribbonColor = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"title": self._title,
 			"status": self._status,
 			"color": self._color,
 			"dot": self._dot,
 			"count": self._count,
 			"countIcon": self._countIcon,
 			"text": self._text,
@@ -150,14 +150,15 @@
 			"showZero": self._showZero,
 			"overflowCount": self._overflowCount,
 			"ribbon": self._ribbon,
 			"ribbonText": self._ribbonText,
 			"ribbonPlacement": self._ribbonPlacement,
 			"ribbonColor": self._ribbonColor
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Badge(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -174,11 +175,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = BadgeCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/BarChart.py` & `atri_react-1.0.0a26/src/atri_react/GanttChart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class BarChartCustomClass():
+class GanttChartCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
 		self.cartesianGrid: Union[Any, None] = state["cartesianGrid"] if state != None and "cartesianGrid" in state else None
 		self.data: Union[Any, None] = state["data"] if state != None and "data" in state else None
 		self.options: Union[Any, None] = state["options"] if state != None and "options" in state else None
 		self.toolTip: Union[Any, None] = state["toolTip"] if state != None and "toolTip" in state else None
 		self.legend: Union[Any, None] = state["legend"] if state != None and "legend" in state else None
+		self.keys: Union[Any, None] = state["keys"] if state != None and "keys" in state else None
 		self.xAxis: Union[Any, None] = state["xAxis"] if state != None and "xAxis" in state else None
 		self.yAxis: Union[Any, None] = state["yAxis"] if state != None and "yAxis" in state else None
-		self.stacked: Union[Any, None] = state["stacked"] if state != None and "stacked" in state else None
 		self.chartHeight: Union[Any, None] = state["chartHeight"] if state != None and "chartHeight" in state else None
 		self.chartWidth: Union[Any, None] = state["chartWidth"] if state != None and "chartWidth" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def cartesianGrid(self):
@@ -57,14 +57,22 @@
 		self._getter_access_tracker["legend"] = {}
 		return self._legend
 	@legend.setter
 	def legend(self, state):
 		self._setter_access_tracker["legend"] = {}
 		self._legend = state
 	@property
+	def keys(self):
+		self._getter_access_tracker["keys"] = {}
+		return self._keys
+	@keys.setter
+	def keys(self, state):
+		self._setter_access_tracker["keys"] = {}
+		self._keys = state
+	@property
 	def xAxis(self):
 		self._getter_access_tracker["xAxis"] = {}
 		return self._xAxis
 	@xAxis.setter
 	def xAxis(self, state):
 		self._setter_access_tracker["xAxis"] = {}
 		self._xAxis = state
@@ -73,22 +81,14 @@
 		self._getter_access_tracker["yAxis"] = {}
 		return self._yAxis
 	@yAxis.setter
 	def yAxis(self, state):
 		self._setter_access_tracker["yAxis"] = {}
 		self._yAxis = state
 	@property
-	def stacked(self):
-		self._getter_access_tracker["stacked"] = {}
-		return self._stacked
-	@stacked.setter
-	def stacked(self, state):
-		self._setter_access_tracker["stacked"] = {}
-		self._stacked = state
-	@property
 	def chartHeight(self):
 		self._getter_access_tracker["chartHeight"] = {}
 		return self._chartHeight
 	@chartHeight.setter
 	def chartHeight(self, state):
 		self._setter_access_tracker["chartHeight"] = {}
 		self._chartHeight = state
@@ -98,47 +98,49 @@
 		return self._chartWidth
 	@chartWidth.setter
 	def chartWidth(self, state):
 		self._setter_access_tracker["chartWidth"] = {}
 		self._chartWidth = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"cartesianGrid": self._cartesianGrid,
 			"data": self._data,
 			"options": self._options,
 			"toolTip": self._toolTip,
 			"legend": self._legend,
+			"keys": self._keys,
 			"xAxis": self._xAxis,
 			"yAxis": self._yAxis,
-			"stacked": self._stacked,
 			"chartHeight": self._chartHeight,
 			"chartWidth": self._chartWidth
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class BarChart(AtriComponent):
+class GanttChart(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "BarChart"
+		self.compKey = "GanttChart"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = BarChartCustomClass(state)
+		self._custom = GanttChartCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Breadcrumb.py` & `atri_react-1.0.0a26/src/atri_react/Breadcrumb.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 		return self._items
 	@items.setter
 	def items(self, state):
 		self._setter_access_tracker["items"] = {}
 		self._items = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"separator": self._separator,
 			"items": self._items
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Breadcrumb(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -54,11 +55,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = BreadcrumbCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Button.py` & `atri_react-1.0.0a26/src/atri_react/Button.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 		self.block: Union[Any, None] = state["block"] if state != None and "block" in state else None
 		self.danger: Union[Any, None] = state["danger"] if state != None and "danger" in state else None
 		self.disabled: Union[Any, None] = state["disabled"] if state != None and "disabled" in state else None
 		self.icon: Union[Any, None] = state["icon"] if state != None and "icon" in state else None
 		self.loading: Union[Any, None] = state["loading"] if state != None and "loading" in state else None
 		self.shape: Union[Any, None] = state["shape"] if state != None and "shape" in state else None
 		self.size: Union[Any, None] = state["size"] if state != None and "size" in state else None
+		self.href: Union[Any, None] = state["href"] if state != None and "href" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def text(self):
 		self._getter_access_tracker["text"] = {}
 		return self._text
@@ -87,27 +88,37 @@
 	def size(self):
 		self._getter_access_tracker["size"] = {}
 		return self._size
 	@size.setter
 	def size(self, state):
 		self._setter_access_tracker["size"] = {}
 		self._size = state
+	@property
+	def href(self):
+		self._getter_access_tracker["href"] = {}
+		return self._href
+	@href.setter
+	def href(self, state):
+		self._setter_access_tracker["href"] = {}
+		self._href = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"text": self._text,
 			"type": self._type,
 			"block": self._block,
 			"danger": self._danger,
 			"disabled": self._disabled,
 			"icon": self._icon,
 			"loading": self._loading,
 			"shape": self._shape,
-			"size": self._size
+			"size": self._size,
+			"href": self._href
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Button(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -124,11 +135,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = ButtonCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/CandleStick.py` & `atri_react-1.0.0a26/src/atri_react/CandleStick.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,24 +80,25 @@
 		return self._chartWidth
 	@chartWidth.setter
 	def chartWidth(self, state):
 		self._setter_access_tracker["chartWidth"] = {}
 		self._chartWidth = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"cartesianGrid": self._cartesianGrid,
 			"data": self._data,
 			"toolTip": self._toolTip,
 			"legend": self._legend,
 			"xAxis": self._xAxis,
 			"yAxis": self._yAxis,
 			"chartHeight": self._chartHeight,
 			"chartWidth": self._chartWidth
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class CandleStick(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -114,11 +115,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = CandleStickCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Card.py` & `atri_react-1.0.0a26/src/atri_react/Iframe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,124 +1,116 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class CardCustomClass():
+class IframeCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.type: Union[Any, None] = state["type"] if state != None and "type" in state else None
-		self.text: Union[Any, None] = state["text"] if state != None and "text" in state else None
-		self.description: Union[Any, None] = state["description"] if state != None and "description" in state else None
-		self.size: Union[Any, None] = state["size"] if state != None and "size" in state else None
-		self.hoverable: Union[Any, None] = state["hoverable"] if state != None and "hoverable" in state else None
-		self.bordered: Union[Any, None] = state["bordered"] if state != None and "bordered" in state else None
-		self.cover: Union[Any, None] = state["cover"] if state != None and "cover" in state else None
-		self.avatar: Union[Any, None] = state["avatar"] if state != None and "avatar" in state else None
+		self.src: Union[Any, None] = state["src"] if state != None and "src" in state else None
+		self.id: Union[Any, None] = state["id"] if state != None and "id" in state else None
+		self.title: Union[Any, None] = state["title"] if state != None and "title" in state else None
+		self.allow: Union[Any, None] = state["allow"] if state != None and "allow" in state else None
+		self.referrerPolicy: Union[Any, None] = state["referrerPolicy"] if state != None and "referrerPolicy" in state else None
+		self.sandbox: Union[Any, None] = state["sandbox"] if state != None and "sandbox" in state else None
+		self.loading: Union[Any, None] = state["loading"] if state != None and "loading" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def type(self):
-		self._getter_access_tracker["type"] = {}
-		return self._type
-	@type.setter
-	def type(self, state):
-		self._setter_access_tracker["type"] = {}
-		self._type = state
-	@property
-	def text(self):
-		self._getter_access_tracker["text"] = {}
-		return self._text
-	@text.setter
-	def text(self, state):
-		self._setter_access_tracker["text"] = {}
-		self._text = state
-	@property
-	def description(self):
-		self._getter_access_tracker["description"] = {}
-		return self._description
-	@description.setter
-	def description(self, state):
-		self._setter_access_tracker["description"] = {}
-		self._description = state
-	@property
-	def size(self):
-		self._getter_access_tracker["size"] = {}
-		return self._size
-	@size.setter
-	def size(self, state):
-		self._setter_access_tracker["size"] = {}
-		self._size = state
-	@property
-	def hoverable(self):
-		self._getter_access_tracker["hoverable"] = {}
-		return self._hoverable
-	@hoverable.setter
-	def hoverable(self, state):
-		self._setter_access_tracker["hoverable"] = {}
-		self._hoverable = state
-	@property
-	def bordered(self):
-		self._getter_access_tracker["bordered"] = {}
-		return self._bordered
-	@bordered.setter
-	def bordered(self, state):
-		self._setter_access_tracker["bordered"] = {}
-		self._bordered = state
-	@property
-	def cover(self):
-		self._getter_access_tracker["cover"] = {}
-		return self._cover
-	@cover.setter
-	def cover(self, state):
-		self._setter_access_tracker["cover"] = {}
-		self._cover = state
-	@property
-	def avatar(self):
-		self._getter_access_tracker["avatar"] = {}
-		return self._avatar
-	@avatar.setter
-	def avatar(self, state):
-		self._setter_access_tracker["avatar"] = {}
-		self._avatar = state
+	def src(self):
+		self._getter_access_tracker["src"] = {}
+		return self._src
+	@src.setter
+	def src(self, state):
+		self._setter_access_tracker["src"] = {}
+		self._src = state
+	@property
+	def id(self):
+		self._getter_access_tracker["id"] = {}
+		return self._id
+	@id.setter
+	def id(self, state):
+		self._setter_access_tracker["id"] = {}
+		self._id = state
+	@property
+	def title(self):
+		self._getter_access_tracker["title"] = {}
+		return self._title
+	@title.setter
+	def title(self, state):
+		self._setter_access_tracker["title"] = {}
+		self._title = state
+	@property
+	def allow(self):
+		self._getter_access_tracker["allow"] = {}
+		return self._allow
+	@allow.setter
+	def allow(self, state):
+		self._setter_access_tracker["allow"] = {}
+		self._allow = state
+	@property
+	def referrerPolicy(self):
+		self._getter_access_tracker["referrerPolicy"] = {}
+		return self._referrerPolicy
+	@referrerPolicy.setter
+	def referrerPolicy(self, state):
+		self._setter_access_tracker["referrerPolicy"] = {}
+		self._referrerPolicy = state
+	@property
+	def sandbox(self):
+		self._getter_access_tracker["sandbox"] = {}
+		return self._sandbox
+	@sandbox.setter
+	def sandbox(self, state):
+		self._setter_access_tracker["sandbox"] = {}
+		self._sandbox = state
+	@property
+	def loading(self):
+		self._getter_access_tracker["loading"] = {}
+		return self._loading
+	@loading.setter
+	def loading(self, state):
+		self._setter_access_tracker["loading"] = {}
+		self._loading = state
 
 	def _to_json_fields(self):
-		return {
-			"type": self._type,
-			"text": self._text,
-			"description": self._description,
-			"size": self._size,
-			"hoverable": self._hoverable,
-			"bordered": self._bordered,
-			"cover": self._cover,
-			"avatar": self._avatar
+		all_fields = {
+			"src": self._src,
+			"id": self._id,
+			"title": self._title,
+			"allow": self._allow,
+			"referrerPolicy": self._referrerPolicy,
+			"sandbox": self._sandbox,
+			"loading": self._loading
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class Card(AtriComponent):
+class Iframe(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "Card"
+		self.compKey = "Iframe"
 		self.nodePkg = "@atrilabs/react-component-manifests"
-		self.onClick = False
+		
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = CardCustomClass(state)
+		self._custom = IframeCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Carousel.py` & `atri_react-1.0.0a26/src/atri_react/Carousel.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,21 +53,22 @@
 		return self._items
 	@items.setter
 	def items(self, state):
 		self._setter_access_tracker["items"] = {}
 		self._items = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"autoplay": self._autoplay,
 			"dots": self._dots,
 			"dotPosition": self._dotPosition,
 			"effect": self._effect,
 			"items": self._items
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Carousel(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -86,11 +87,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = CarouselCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Cascader.py` & `atri_react-1.0.0a26/src/atri_react/Cascader.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 		return self._notFoundContent
 	@notFoundContent.setter
 	def notFoundContent(self, state):
 		self._setter_access_tracker["notFoundContent"] = {}
 		self._notFoundContent = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"options": self._options,
 			"placeholder": self._placeholder,
 			"allowClear": self._allowClear,
 			"multiple": self._multiple,
 			"showCheckedStrategy": self._showCheckedStrategy,
 			"maxTagCount": self._maxTagCount,
 			"maxTagTextLength": self._maxTagTextLength,
@@ -210,14 +210,15 @@
 			"removeIcon": self._removeIcon,
 			"clearIcon": self._clearIcon,
 			"expandIcon": self._expandIcon,
 			"expandTrigger": self._expandTrigger,
 			"status": self._status,
 			"notFoundContent": self._notFoundContent
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Cascader(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -234,11 +235,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = CascaderCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Checkbox.py` & `atri_react-1.0.0a26/src/atri_react/Checkbox.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,41 +3,72 @@
 
 
 
 class CheckboxCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.checked: Union[Any, None] = state["checked"] if state != None and "checked" in state else None
-		self.text: Union[Any, None] = state["text"] if state != None and "text" in state else None
+		self.defaultValue: Union[Any, None] = state["defaultValue"] if state != None and "defaultValue" in state else None
+		self.disabled: Union[Any, None] = state["disabled"] if state != None and "disabled" in state else None
+		self.name: Union[Any, None] = state["name"] if state != None and "name" in state else None
+		self.value: Union[Any, None] = state["value"] if state != None and "value" in state else None
+		self.options: Union[Any, None] = state["options"] if state != None and "options" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def checked(self):
-		self._getter_access_tracker["checked"] = {}
-		return self._checked
-	@checked.setter
-	def checked(self, state):
-		self._setter_access_tracker["checked"] = {}
-		self._checked = state
-	@property
-	def text(self):
-		self._getter_access_tracker["text"] = {}
-		return self._text
-	@text.setter
-	def text(self, state):
-		self._setter_access_tracker["text"] = {}
-		self._text = state
+	def defaultValue(self):
+		self._getter_access_tracker["defaultValue"] = {}
+		return self._defaultValue
+	@defaultValue.setter
+	def defaultValue(self, state):
+		self._setter_access_tracker["defaultValue"] = {}
+		self._defaultValue = state
+	@property
+	def disabled(self):
+		self._getter_access_tracker["disabled"] = {}
+		return self._disabled
+	@disabled.setter
+	def disabled(self, state):
+		self._setter_access_tracker["disabled"] = {}
+		self._disabled = state
+	@property
+	def name(self):
+		self._getter_access_tracker["name"] = {}
+		return self._name
+	@name.setter
+	def name(self, state):
+		self._setter_access_tracker["name"] = {}
+		self._name = state
+	@property
+	def value(self):
+		self._getter_access_tracker["value"] = {}
+		return self._value
+	@value.setter
+	def value(self, state):
+		self._setter_access_tracker["value"] = {}
+		self._value = state
+	@property
+	def options(self):
+		self._getter_access_tracker["options"] = {}
+		return self._options
+	@options.setter
+	def options(self, state):
+		self._setter_access_tracker["options"] = {}
+		self._options = state
 
 	def _to_json_fields(self):
-		return {
-			"checked": self._checked,
-			"text": self._text
+		all_fields = {
+			"defaultValue": self._defaultValue,
+			"disabled": self._disabled,
+			"name": self._name,
+			"value": self._value,
+			"options": self._options
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Checkbox(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -54,11 +85,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = CheckboxCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/CodeMirror.py` & `atri_react-1.0.0a26/src/atri_react/CodeMirror.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 		return self._lintKeymap
 	@lintKeymap.setter
 	def lintKeymap(self, state):
 		self._setter_access_tracker["lintKeymap"] = {}
 		self._lintKeymap = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"extensions": self._extensions,
 			"value": self._value,
 			"theme": self._theme,
 			"autoFocus": self._autoFocus,
 			"editable": self._editable,
 			"placeholder": self._placeholder,
 			"lineNumbers": self._lineNumbers,
@@ -310,14 +310,15 @@
 			"defaultKeymap": self._defaultKeymap,
 			"searchKeymap": self._searchKeymap,
 			"historyKeymap": self._historyKeymap,
 			"foldKeymap": self._foldKeymap,
 			"completionKeymap": self._completionKeymap,
 			"lintKeymap": self._lintKeymap
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class CodeMirror(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -334,11 +335,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = CodeMirrorCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Countdown.py` & `atri_react-1.0.0a26/src/atri_react/Countdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,24 +80,25 @@
 		return self._suffixIcon
 	@suffixIcon.setter
 	def suffixIcon(self, state):
 		self._setter_access_tracker["suffixIcon"] = {}
 		self._suffixIcon = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"title": self._title,
 			"format": self._format,
 			"inputType": self._inputType,
 			"value": self._value,
 			"prefix": self._prefix,
 			"prefixIcon": self._prefixIcon,
 			"suffix": self._suffix,
 			"suffixIcon": self._suffixIcon
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Countdown(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -114,11 +115,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = CountdownCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Countup.py` & `atri_react-1.0.0a26/src/atri_react/Countup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 		return self._duration
 	@duration.setter
 	def duration(self, state):
 		self._setter_access_tracker["duration"] = {}
 		self._duration = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"itemCount": self._itemCount,
 			"duration": self._duration
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Countup(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -54,11 +55,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = CountupCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/DatePicker.py` & `atri_react-1.0.0a26/src/atri_react/Testimonial.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class DatePickerCustomClass():
+class TestimonialCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.picker: Union[Any, None] = state["picker"] if state != None and "picker" in state else None
-		self.showTime: Union[Any, None] = state["showTime"] if state != None and "showTime" in state else None
-		self.disabled: Union[Any, None] = state["disabled"] if state != None and "disabled" in state else None
+		self.startTile: Union[Any, None] = state["startTile"] if state != None and "startTile" in state else None
+		self.intervalTime: Union[Any, None] = state["intervalTime"] if state != None and "intervalTime" in state else None
+		self.testimonials: Union[Any, None] = state["testimonials"] if state != None and "testimonials" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def picker(self):
-		self._getter_access_tracker["picker"] = {}
-		return self._picker
-	@picker.setter
-	def picker(self, state):
-		self._setter_access_tracker["picker"] = {}
-		self._picker = state
+	def startTile(self):
+		self._getter_access_tracker["startTile"] = {}
+		return self._startTile
+	@startTile.setter
+	def startTile(self, state):
+		self._setter_access_tracker["startTile"] = {}
+		self._startTile = state
 	@property
-	def showTime(self):
-		self._getter_access_tracker["showTime"] = {}
-		return self._showTime
-	@showTime.setter
-	def showTime(self, state):
-		self._setter_access_tracker["showTime"] = {}
-		self._showTime = state
+	def intervalTime(self):
+		self._getter_access_tracker["intervalTime"] = {}
+		return self._intervalTime
+	@intervalTime.setter
+	def intervalTime(self, state):
+		self._setter_access_tracker["intervalTime"] = {}
+		self._intervalTime = state
 	@property
-	def disabled(self):
-		self._getter_access_tracker["disabled"] = {}
-		return self._disabled
-	@disabled.setter
-	def disabled(self, state):
-		self._setter_access_tracker["disabled"] = {}
-		self._disabled = state
+	def testimonials(self):
+		self._getter_access_tracker["testimonials"] = {}
+		return self._testimonials
+	@testimonials.setter
+	def testimonials(self, state):
+		self._setter_access_tracker["testimonials"] = {}
+		self._testimonials = state
 
 	def _to_json_fields(self):
-		return {
-			"picker": self._picker,
-			"showTime": self._showTime,
-			"disabled": self._disabled
+		all_fields = {
+			"startTile": self._startTile,
+			"intervalTime": self._intervalTime,
+			"testimonials": self._testimonials
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class DatePicker(AtriComponent):
+class Testimonial(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "DatePicker"
+		self.compKey = "Testimonial"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		self.onClick = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = DatePickerCustomClass(state)
+		self._custom = TestimonialCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Div.py` & `atri_react-1.0.0a26/src/atri_react/Flex.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class DivCustomClass():
+class FlexCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
 		
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class Div(AtriComponent):
+class Flex(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "Div"
+		self.compKey = "Flex"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		self.onClick = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = DivCustomClass(state)
+		self._custom = FlexCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Dropdown.py` & `atri_react-1.0.0a26/src/atri_react/Image.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class DropdownCustomClass():
+class ImageCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.selectedValue: Union[Any, None] = state["selectedValue"] if state != None and "selectedValue" in state else None
-		self.dropdownItems: Union[Any, None] = state["dropdownItems"] if state != None and "dropdownItems" in state else None
+		self.alt: Union[Any, None] = state["alt"] if state != None and "alt" in state else None
+		self.src: Union[Any, None] = state["src"] if state != None and "src" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def selectedValue(self):
-		self._getter_access_tracker["selectedValue"] = {}
-		return self._selectedValue
-	@selectedValue.setter
-	def selectedValue(self, state):
-		self._setter_access_tracker["selectedValue"] = {}
-		self._selectedValue = state
+	def alt(self):
+		self._getter_access_tracker["alt"] = {}
+		return self._alt
+	@alt.setter
+	def alt(self, state):
+		self._setter_access_tracker["alt"] = {}
+		self._alt = state
 	@property
-	def dropdownItems(self):
-		self._getter_access_tracker["dropdownItems"] = {}
-		return self._dropdownItems
-	@dropdownItems.setter
-	def dropdownItems(self, state):
-		self._setter_access_tracker["dropdownItems"] = {}
-		self._dropdownItems = state
+	def src(self):
+		self._getter_access_tracker["src"] = {}
+		return self._src
+	@src.setter
+	def src(self, state):
+		self._setter_access_tracker["src"] = {}
+		self._src = state
 
 	def _to_json_fields(self):
-		return {
-			"selectedValue": self._selectedValue,
-			"dropdownItems": self._dropdownItems
+		all_fields = {
+			"alt": self._alt,
+			"src": self._src
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class Dropdown(AtriComponent):
+class Image(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "Dropdown"
+		self.compKey = "Image"
 		self.nodePkg = "@atrilabs/react-component-manifests"
-		self.onChange = False
+		self.onClick = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = DropdownCustomClass(state)
+		self._custom = ImageCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Flex.py` & `atri_react-1.0.0a26/src/atri_react/Div.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class FlexCustomClass():
+class DivCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
 		
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class Flex(AtriComponent):
+class Div(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "Flex"
+		self.compKey = "Div"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		self.onClick = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = FlexCustomClass(state)
+		self._custom = DivCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Form.py` & `atri_react-1.0.0a26/src/atri_react/Form.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,26 +98,27 @@
 		return self._disabled
 	@disabled.setter
 	def disabled(self, state):
 		self._setter_access_tracker["disabled"] = {}
 		self._disabled = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"autocomplete": self._autocomplete,
 			"form": self._form,
 			"showSubmitButton": self._showSubmitButton,
 			"showResetButton": self._showResetButton,
 			"submitButtonBgColor": self._submitButtonBgColor,
 			"submitButtonColor": self._submitButtonColor,
 			"resetButtonBgColor": self._resetButtonBgColor,
 			"resetButtonColor": self._resetButtonColor,
 			"target": self._target,
 			"disabled": self._disabled
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Form(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -134,11 +135,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = FormCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/GanttChart.py` & `atri_react-1.0.0a26/src/atri_react/ScatterChart.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class GanttChartCustomClass():
+class ScatterChartCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
 		self.cartesianGrid: Union[Any, None] = state["cartesianGrid"] if state != None and "cartesianGrid" in state else None
 		self.data: Union[Any, None] = state["data"] if state != None and "data" in state else None
 		self.options: Union[Any, None] = state["options"] if state != None and "options" in state else None
 		self.toolTip: Union[Any, None] = state["toolTip"] if state != None and "toolTip" in state else None
 		self.legend: Union[Any, None] = state["legend"] if state != None and "legend" in state else None
-		self.keys: Union[Any, None] = state["keys"] if state != None and "keys" in state else None
 		self.xAxis: Union[Any, None] = state["xAxis"] if state != None and "xAxis" in state else None
 		self.yAxis: Union[Any, None] = state["yAxis"] if state != None and "yAxis" in state else None
+		self.zAxis: Union[Any, None] = state["zAxis"] if state != None and "zAxis" in state else None
 		self.chartHeight: Union[Any, None] = state["chartHeight"] if state != None and "chartHeight" in state else None
 		self.chartWidth: Union[Any, None] = state["chartWidth"] if state != None and "chartWidth" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def cartesianGrid(self):
@@ -57,22 +57,14 @@
 		self._getter_access_tracker["legend"] = {}
 		return self._legend
 	@legend.setter
 	def legend(self, state):
 		self._setter_access_tracker["legend"] = {}
 		self._legend = state
 	@property
-	def keys(self):
-		self._getter_access_tracker["keys"] = {}
-		return self._keys
-	@keys.setter
-	def keys(self, state):
-		self._setter_access_tracker["keys"] = {}
-		self._keys = state
-	@property
 	def xAxis(self):
 		self._getter_access_tracker["xAxis"] = {}
 		return self._xAxis
 	@xAxis.setter
 	def xAxis(self, state):
 		self._setter_access_tracker["xAxis"] = {}
 		self._xAxis = state
@@ -81,14 +73,22 @@
 		self._getter_access_tracker["yAxis"] = {}
 		return self._yAxis
 	@yAxis.setter
 	def yAxis(self, state):
 		self._setter_access_tracker["yAxis"] = {}
 		self._yAxis = state
 	@property
+	def zAxis(self):
+		self._getter_access_tracker["zAxis"] = {}
+		return self._zAxis
+	@zAxis.setter
+	def zAxis(self, state):
+		self._setter_access_tracker["zAxis"] = {}
+		self._zAxis = state
+	@property
 	def chartHeight(self):
 		self._getter_access_tracker["chartHeight"] = {}
 		return self._chartHeight
 	@chartHeight.setter
 	def chartHeight(self, state):
 		self._setter_access_tracker["chartHeight"] = {}
 		self._chartHeight = state
@@ -98,47 +98,49 @@
 		return self._chartWidth
 	@chartWidth.setter
 	def chartWidth(self, state):
 		self._setter_access_tracker["chartWidth"] = {}
 		self._chartWidth = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"cartesianGrid": self._cartesianGrid,
 			"data": self._data,
 			"options": self._options,
 			"toolTip": self._toolTip,
 			"legend": self._legend,
-			"keys": self._keys,
 			"xAxis": self._xAxis,
 			"yAxis": self._yAxis,
+			"zAxis": self._zAxis,
 			"chartHeight": self._chartHeight,
 			"chartWidth": self._chartWidth
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class GanttChart(AtriComponent):
+class ScatterChart(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "GanttChart"
+		self.compKey = "ScatterChart"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = GanttChartCustomClass(state)
+		self._custom = ScatterChartCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/HistogramChart.py` & `atri_react-1.0.0a26/src/atri_react/HistogramChart.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,24 +80,25 @@
 		return self._chartWidth
 	@chartWidth.setter
 	def chartWidth(self, state):
 		self._setter_access_tracker["chartWidth"] = {}
 		self._chartWidth = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"cartesianGrid": self._cartesianGrid,
 			"data": self._data,
 			"toolTip": self._toolTip,
 			"legend": self._legend,
 			"xAxis": self._xAxis,
 			"yAxis": self._yAxis,
 			"chartHeight": self._chartHeight,
 			"chartWidth": self._chartWidth
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class HistogramChart(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -114,11 +115,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = HistogramChartCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Icon.py` & `atri_react-1.0.0a26/src/atri_react/Icon.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 		return self._svg
 	@svg.setter
 	def svg(self, state):
 		self._setter_access_tracker["svg"] = {}
 		self._svg = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"svg": self._svg
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Icon(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -44,11 +45,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = IconCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Input.py` & `atri_react-1.0.0a26/src/atri_react/Input.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 		return self._suffix
 	@suffix.setter
 	def suffix(self, state):
 		self._setter_access_tracker["suffix"] = {}
 		self._suffix = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"defaultValue": self._defaultValue,
 			"value": self._value,
 			"placeholder": self._placeholder,
 			"isPasswordField": self._isPasswordField,
 			"size": self._size,
 			"addonAfter": self._addonAfter,
 			"addonBefore": self._addonBefore,
@@ -170,14 +170,15 @@
 			"id": self._id,
 			"maxLength": self._maxLength,
 			"showCount": self._showCount,
 			"status": self._status,
 			"prefix": self._prefix,
 			"suffix": self._suffix
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Input(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -195,11 +196,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = InputCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/InputNumber.py` & `atri_react-1.0.0a26/src/atri_react/InputNumber.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 		return self._readOnly
 	@readOnly.setter
 	def readOnly(self, state):
 		self._setter_access_tracker["readOnly"] = {}
 		self._readOnly = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"defaultValue": self._defaultValue,
 			"value": self._value,
 			"max": self._max,
 			"min": self._min,
 			"step": self._step,
 			"placeholder": self._placeholder,
 			"size": self._size,
@@ -170,14 +170,15 @@
 			"addonAfter": self._addonAfter,
 			"addonBefore": self._addonBefore,
 			"prefix": self._prefix,
 			"suffix": self._suffix,
 			"keyboard": self._keyboard,
 			"readOnly": self._readOnly
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class InputNumber(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -198,11 +199,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = InputNumberCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/LineChart.py` & `atri_react-1.0.0a26/src/atri_react/AreaChart.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class LineChartCustomClass():
+class AreaChartCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
 		self.cartesianGrid: Union[Any, None] = state["cartesianGrid"] if state != None and "cartesianGrid" in state else None
 		self.data: Union[Any, None] = state["data"] if state != None and "data" in state else None
 		self.options: Union[Any, None] = state["options"] if state != None and "options" in state else None
 		self.toolTip: Union[Any, None] = state["toolTip"] if state != None and "toolTip" in state else None
@@ -89,46 +89,48 @@
 		return self._chartWidth
 	@chartWidth.setter
 	def chartWidth(self, state):
 		self._setter_access_tracker["chartWidth"] = {}
 		self._chartWidth = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"cartesianGrid": self._cartesianGrid,
 			"data": self._data,
 			"options": self._options,
 			"toolTip": self._toolTip,
 			"legend": self._legend,
 			"xAxis": self._xAxis,
 			"yAxis": self._yAxis,
 			"chartHeight": self._chartHeight,
 			"chartWidth": self._chartWidth
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class LineChart(AtriComponent):
+class AreaChart(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "LineChart"
+		self.compKey = "AreaChart"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = LineChartCustomClass(state)
+		self._custom = AreaChartCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Link.py` & `atri_react-1.0.0a26/src/atri_react/Link.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,20 @@
 		return self._disabled
 	@disabled.setter
 	def disabled(self, state):
 		self._setter_access_tracker["disabled"] = {}
 		self._disabled = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"text": self._text,
 			"url": self._url,
 			"disabled": self._disabled
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Link(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -64,11 +65,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = LinkCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Menu.py` & `atri_react-1.0.0a26/src/atri_react/Menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,26 +98,27 @@
 		return self._items
 	@items.setter
 	def items(self, state):
 		self._setter_access_tracker["items"] = {}
 		self._items = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"mode": self._mode,
 			"theme": self._theme,
 			"multiple": self._multiple,
 			"selectable": self._selectable,
 			"selectedKeys": self._selectedKeys,
 			"defaultOpenKeys": self._defaultOpenKeys,
 			"defaultSelectedKeys": self._defaultSelectedKeys,
 			"expandIcon": self._expandIcon,
 			"openKeys": self._openKeys,
 			"items": self._items
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Menu(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -136,11 +137,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = MenuCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Modal.py` & `atri_react-1.0.0a26/src/atri_react/Modal.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,32 +3,39 @@
 
 
 
 class ModalCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
+		self.open: Union[Any, None] = state["open"] if state != None and "open" in state else None
 		self.text: Union[Any, None] = state["text"] if state != None and "text" in state else None
 		self.content: Union[Any, None] = state["content"] if state != None and "content" in state else None
-		self.cancelText: Union[Any, None] = state["cancelText"] if state != None and "cancelText" in state else None
-		self.okText: Union[Any, None] = state["okText"] if state != None and "okText" in state else None
 		self.centered: Union[Any, None] = state["centered"] if state != None and "centered" in state else None
 		self.icon: Union[Any, None] = state["icon"] if state != None and "icon" in state else None
 		self.closable: Union[Any, None] = state["closable"] if state != None and "closable" in state else None
 		self.closeIcon: Union[Any, None] = state["closeIcon"] if state != None and "closeIcon" in state else None
 		self.destroyOnClose: Union[Any, None] = state["destroyOnClose"] if state != None and "destroyOnClose" in state else None
 		self.keyboard: Union[Any, None] = state["keyboard"] if state != None and "keyboard" in state else None
 		self.mask: Union[Any, None] = state["mask"] if state != None and "mask" in state else None
 		self.maskClosable: Union[Any, None] = state["maskClosable"] if state != None and "maskClosable" in state else None
 		self.zIndex: Union[Any, None] = state["zIndex"] if state != None and "zIndex" in state else None
-		self.open: Union[Any, None] = state["open"] if state != None and "open" in state else None
+		self.confirmLoading: Union[Any, None] = state["confirmLoading"] if state != None and "confirmLoading" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
+	def open(self):
+		self._getter_access_tracker["open"] = {}
+		return self._open
+	@open.setter
+	def open(self, state):
+		self._setter_access_tracker["open"] = {}
+		self._open = state
+	@property
 	def text(self):
 		self._getter_access_tracker["text"] = {}
 		return self._text
 	@text.setter
 	def text(self, state):
 		self._setter_access_tracker["text"] = {}
 		self._text = state
@@ -37,30 +44,14 @@
 		self._getter_access_tracker["content"] = {}
 		return self._content
 	@content.setter
 	def content(self, state):
 		self._setter_access_tracker["content"] = {}
 		self._content = state
 	@property
-	def cancelText(self):
-		self._getter_access_tracker["cancelText"] = {}
-		return self._cancelText
-	@cancelText.setter
-	def cancelText(self, state):
-		self._setter_access_tracker["cancelText"] = {}
-		self._cancelText = state
-	@property
-	def okText(self):
-		self._getter_access_tracker["okText"] = {}
-		return self._okText
-	@okText.setter
-	def okText(self, state):
-		self._setter_access_tracker["okText"] = {}
-		self._okText = state
-	@property
 	def centered(self):
 		self._getter_access_tracker["centered"] = {}
 		return self._centered
 	@centered.setter
 	def centered(self, state):
 		self._setter_access_tracker["centered"] = {}
 		self._centered = state
@@ -125,60 +116,63 @@
 		self._getter_access_tracker["zIndex"] = {}
 		return self._zIndex
 	@zIndex.setter
 	def zIndex(self, state):
 		self._setter_access_tracker["zIndex"] = {}
 		self._zIndex = state
 	@property
-	def open(self):
-		self._getter_access_tracker["open"] = {}
-		return self._open
-	@open.setter
-	def open(self, state):
-		self._setter_access_tracker["open"] = {}
-		self._open = state
+	def confirmLoading(self):
+		self._getter_access_tracker["confirmLoading"] = {}
+		return self._confirmLoading
+	@confirmLoading.setter
+	def confirmLoading(self, state):
+		self._setter_access_tracker["confirmLoading"] = {}
+		self._confirmLoading = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
+			"open": self._open,
 			"text": self._text,
 			"content": self._content,
-			"cancelText": self._cancelText,
-			"okText": self._okText,
 			"centered": self._centered,
 			"icon": self._icon,
 			"closable": self._closable,
 			"closeIcon": self._closeIcon,
 			"destroyOnClose": self._destroyOnClose,
 			"keyboard": self._keyboard,
 			"mask": self._mask,
 			"maskClosable": self._maskClosable,
 			"zIndex": self._zIndex,
-			"open": self._open
+			"confirmLoading": self._confirmLoading
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Modal(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
 		self.compKey = "Modal"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		self.onClick = False
+		self.onCancel = False
+		self.afterClose = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = ModalCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Overlay.py` & `atri_react-1.0.0a26/src/atri_react/Overlay.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 		return self._open
 	@open.setter
 	def open(self, state):
 		self._setter_access_tracker["open"] = {}
 		self._open = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"closeOverlayAfter": self._closeOverlayAfter,
 			"open": self._open
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Overlay(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -54,11 +55,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = OverlayCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/PieChart.py` & `atri_react-1.0.0a26/src/atri_react/PieChart.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,23 +71,24 @@
 		return self._chartWidth
 	@chartWidth.setter
 	def chartWidth(self, state):
 		self._setter_access_tracker["chartWidth"] = {}
 		self._chartWidth = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"data": self._data,
 			"options": self._options,
 			"toolTip": self._toolTip,
 			"legend": self._legend,
 			"keys": self._keys,
 			"chartHeight": self._chartHeight,
 			"chartWidth": self._chartWidth
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class PieChart(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -104,11 +105,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = PieChartCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Radio.py` & `atri_react-1.0.0a26/src/atri_react/TextBox.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,56 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class RadioCustomClass():
+class TextBoxCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.name: Union[Any, None] = state["name"] if state != None and "name" in state else None
-		self.label: Union[Any, None] = state["label"] if state != None and "label" in state else None
-		self.checked: Union[Any, None] = state["checked"] if state != None and "checked" in state else None
-		self.radius: Union[Any, None] = state["radius"] if state != None and "radius" in state else None
+		self.text: Union[Any, None] = state["text"] if state != None and "text" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def name(self):
-		self._getter_access_tracker["name"] = {}
-		return self._name
-	@name.setter
-	def name(self, state):
-		self._setter_access_tracker["name"] = {}
-		self._name = state
-	@property
-	def label(self):
-		self._getter_access_tracker["label"] = {}
-		return self._label
-	@label.setter
-	def label(self, state):
-		self._setter_access_tracker["label"] = {}
-		self._label = state
-	@property
-	def checked(self):
-		self._getter_access_tracker["checked"] = {}
-		return self._checked
-	@checked.setter
-	def checked(self, state):
-		self._setter_access_tracker["checked"] = {}
-		self._checked = state
-	@property
-	def radius(self):
-		self._getter_access_tracker["radius"] = {}
-		return self._radius
-	@radius.setter
-	def radius(self, state):
-		self._setter_access_tracker["radius"] = {}
-		self._radius = state
+	def text(self):
+		self._getter_access_tracker["text"] = {}
+		return self._text
+	@text.setter
+	def text(self, state):
+		self._setter_access_tracker["text"] = {}
+		self._text = state
 
 	def _to_json_fields(self):
-		return {
-			"name": self._name,
-			"label": self._label,
-			"checked": self._checked,
-			"radius": self._radius
+		all_fields = {
+			"text": self._text
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class Radio(AtriComponent):
+class TextBox(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "Radio"
+		self.compKey = "TextBox"
 		self.nodePkg = "@atrilabs/react-component-manifests"
-		self.onChange = False
+		self.onClick = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = RadioCustomClass(state)
+		self._custom = TextBoxCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Rating.py` & `atri_react-1.0.0a26/src/atri_react/Rating.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,23 +71,24 @@
 		return self._count
 	@count.setter
 	def count(self, state):
 		self._setter_access_tracker["count"] = {}
 		self._count = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"allowHalf": self._allowHalf,
 			"defaultValue": self._defaultValue,
 			"disabled": self._disabled,
 			"allowClear": self._allowClear,
 			"character": self._character,
 			"toolTipInfo": self._toolTipInfo,
 			"count": self._count
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Rating(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -104,11 +105,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = RatingCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Repeating.py` & `atri_react-1.0.0a26/src/atri_react/Repeating.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 	@property
 	def data(self):
 		self._getter_access_tracker["data"] = {}
 		return self._data
 	@data.setter
 	def data(self, state):
 		self._setter_access_tracker["data"] = {}
-		if type(state) == "list":
-			self._data = [self._WrapperClass(i) for i in state]
+		if type(state) == list:
+			self._data = [self._WrapperClass(state[i]) for i in range(len(state))]
 		else:
 			self._data = []
 	@property
 	def start(self):
 		self._getter_access_tracker["start"] = {}
 		return self._start
 	@start.setter
@@ -47,20 +47,21 @@
 		return self._image
 	@image.setter
 	def image(self, state):
 		self._setter_access_tracker["image"] = {}
 		self._image = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"data": self._data,
 			"start": self._start,
 			"end": self._end,
 			"image": self._image
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Repeating(AtriComponent, Generic[T]):
 	def __init__(self, state: Union[Any, None], WrapperClass: T):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		self._WrapperClass = WrapperClass
@@ -77,11 +78,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = RepeatingCustomClass[T](state, self._WrapperClass)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/ScatterChart.py` & `atri_react-1.0.0a26/src/atri_react/BarChart.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class ScatterChartCustomClass():
+class BarChartCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
 		self.cartesianGrid: Union[Any, None] = state["cartesianGrid"] if state != None and "cartesianGrid" in state else None
 		self.data: Union[Any, None] = state["data"] if state != None and "data" in state else None
 		self.options: Union[Any, None] = state["options"] if state != None and "options" in state else None
 		self.toolTip: Union[Any, None] = state["toolTip"] if state != None and "toolTip" in state else None
 		self.legend: Union[Any, None] = state["legend"] if state != None and "legend" in state else None
 		self.xAxis: Union[Any, None] = state["xAxis"] if state != None and "xAxis" in state else None
 		self.yAxis: Union[Any, None] = state["yAxis"] if state != None and "yAxis" in state else None
-		self.zAxis: Union[Any, None] = state["zAxis"] if state != None and "zAxis" in state else None
+		self.stacked: Union[Any, None] = state["stacked"] if state != None and "stacked" in state else None
 		self.chartHeight: Union[Any, None] = state["chartHeight"] if state != None and "chartHeight" in state else None
 		self.chartWidth: Union[Any, None] = state["chartWidth"] if state != None and "chartWidth" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def cartesianGrid(self):
@@ -73,21 +73,21 @@
 		self._getter_access_tracker["yAxis"] = {}
 		return self._yAxis
 	@yAxis.setter
 	def yAxis(self, state):
 		self._setter_access_tracker["yAxis"] = {}
 		self._yAxis = state
 	@property
-	def zAxis(self):
-		self._getter_access_tracker["zAxis"] = {}
-		return self._zAxis
-	@zAxis.setter
-	def zAxis(self, state):
-		self._setter_access_tracker["zAxis"] = {}
-		self._zAxis = state
+	def stacked(self):
+		self._getter_access_tracker["stacked"] = {}
+		return self._stacked
+	@stacked.setter
+	def stacked(self, state):
+		self._setter_access_tracker["stacked"] = {}
+		self._stacked = state
 	@property
 	def chartHeight(self):
 		self._getter_access_tracker["chartHeight"] = {}
 		return self._chartHeight
 	@chartHeight.setter
 	def chartHeight(self, state):
 		self._setter_access_tracker["chartHeight"] = {}
@@ -98,47 +98,49 @@
 		return self._chartWidth
 	@chartWidth.setter
 	def chartWidth(self, state):
 		self._setter_access_tracker["chartWidth"] = {}
 		self._chartWidth = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"cartesianGrid": self._cartesianGrid,
 			"data": self._data,
 			"options": self._options,
 			"toolTip": self._toolTip,
 			"legend": self._legend,
 			"xAxis": self._xAxis,
 			"yAxis": self._yAxis,
-			"zAxis": self._zAxis,
+			"stacked": self._stacked,
 			"chartHeight": self._chartHeight,
 			"chartWidth": self._chartWidth
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class ScatterChart(AtriComponent):
+class BarChart(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "ScatterChart"
+		self.compKey = "BarChart"
 		self.nodePkg = "@atrilabs/react-component-manifests"
 		
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = ScatterChartCustomClass(state)
+		self._custom = BarChartCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Search.py` & `atri_react-1.0.0a26/src/atri_react/Search.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 		return self._suffix
 	@suffix.setter
 	def suffix(self, state):
 		self._setter_access_tracker["suffix"] = {}
 		self._suffix = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"defaultValue": self._defaultValue,
 			"placeholder": self._placeholder,
 			"value": self._value,
 			"size": self._size,
 			"addonAfter": self._addonAfter,
 			"addonBefore": self._addonBefore,
 			"allowClear": self._allowClear,
@@ -160,14 +160,15 @@
 			"id": self._id,
 			"maxLength": self._maxLength,
 			"showCount": self._showCount,
 			"status": self._status,
 			"prefix": self._prefix,
 			"suffix": self._suffix
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Search(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -185,11 +186,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = SearchCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Select.py` & `atri_react-1.0.0a26/src/atri_react/Select.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,20 +44,21 @@
 		return self._disabled
 	@disabled.setter
 	def disabled(self, state):
 		self._setter_access_tracker["disabled"] = {}
 		self._disabled = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"placeholder": self._placeholder,
 			"defaultValue": self._defaultValue,
 			"options": self._options,
 			"disabled": self._disabled
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Select(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -74,11 +75,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = SelectCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Slider.py` & `atri_react-1.0.0a26/src/atri_react/Slider.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,26 +98,27 @@
 		return self._marks
 	@marks.setter
 	def marks(self, state):
 		self._setter_access_tracker["marks"] = {}
 		self._marks = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"range": self._range,
 			"value": self._value,
 			"min": self._min,
 			"max": self._max,
 			"defaultValue": self._defaultValue,
 			"disabled": self._disabled,
 			"vertical": self._vertical,
 			"draggableTrack": self._draggableTrack,
 			"reverse": self._reverse,
 			"marks": self._marks
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Slider(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -135,11 +136,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = SliderCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Statistic.py` & `atri_react-1.0.0a26/src/atri_react/Statistic.py`

 * *Files 15% similar despite different names*

```diff
@@ -98,26 +98,27 @@
 		return self._loading
 	@loading.setter
 	def loading(self, state):
 		self._setter_access_tracker["loading"] = {}
 		self._loading = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"title": self._title,
 			"value": self._value,
 			"groupSeparator": self._groupSeparator,
 			"decimalSeparator": self._decimalSeparator,
 			"precision": self._precision,
 			"prefix": self._prefix,
 			"prefixIcon": self._prefixIcon,
 			"suffix": self._suffix,
 			"suffixIcon": self._suffixIcon,
 			"loading": self._loading
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Statistic(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -134,11 +135,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = StatisticCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Step.py` & `atri_react-1.0.0a26/src/atri_react/Step.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
 		self.current: Union[Any, None] = state["current"] if state != None and "current" in state else None
 		self.size: Union[Any, None] = state["size"] if state != None and "size" in state else None
 		self.direction: Union[Any, None] = state["direction"] if state != None and "direction" in state else None
 		self.dotStyle: Union[Any, None] = state["dotStyle"] if state != None and "dotStyle" in state else None
-		self.clickable: Union[Any, None] = state["clickable"] if state != None and "clickable" in state else None
 		self.type: Union[Any, None] = state["type"] if state != None and "type" in state else None
 		self.percent: Union[Any, None] = state["percent"] if state != None and "percent" in state else None
 		self.labelPlacement: Union[Any, None] = state["labelPlacement"] if state != None and "labelPlacement" in state else None
 		self.items: Union[Any, None] = state["items"] if state != None and "items" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
@@ -48,22 +47,14 @@
 		self._getter_access_tracker["dotStyle"] = {}
 		return self._dotStyle
 	@dotStyle.setter
 	def dotStyle(self, state):
 		self._setter_access_tracker["dotStyle"] = {}
 		self._dotStyle = state
 	@property
-	def clickable(self):
-		self._getter_access_tracker["clickable"] = {}
-		return self._clickable
-	@clickable.setter
-	def clickable(self, state):
-		self._setter_access_tracker["clickable"] = {}
-		self._clickable = state
-	@property
 	def type(self):
 		self._getter_access_tracker["type"] = {}
 		return self._type
 	@type.setter
 	def type(self, state):
 		self._setter_access_tracker["type"] = {}
 		self._type = state
@@ -89,25 +80,25 @@
 		return self._items
 	@items.setter
 	def items(self, state):
 		self._setter_access_tracker["items"] = {}
 		self._items = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"current": self._current,
 			"size": self._size,
 			"direction": self._direction,
 			"dotStyle": self._dotStyle,
-			"clickable": self._clickable,
 			"type": self._type,
 			"percent": self._percent,
 			"labelPlacement": self._labelPlacement,
 			"items": self._items
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Step(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -124,11 +115,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = StepCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Table.py` & `atri_react-1.0.0a26/src/atri_react/Table.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,23 +71,24 @@
 		return self._selection
 	@selection.setter
 	def selection(self, state):
 		self._setter_access_tracker["selection"] = {}
 		self._selection = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"rows": self._rows,
 			"cols": self._cols,
 			"checkboxSelection": self._checkboxSelection,
 			"autoHeight": self._autoHeight,
 			"numRows": self._numRows,
 			"rowHeight": self._rowHeight,
 			"selection": self._selection
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Table(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -104,11 +105,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = TableCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Tabs.py` & `atri_react-1.0.0a26/src/atri_react/Tabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 		
 		self.centered: Union[Any, None] = state["centered"] if state != None and "centered" in state else None
 		self.animated: Union[Any, None] = state["animated"] if state != None and "animated" in state else None
 		self.addIcon: Union[Any, None] = state["addIcon"] if state != None and "addIcon" in state else None
 		self.tabPosition: Union[Any, None] = state["tabPosition"] if state != None and "tabPosition" in state else None
 		self.size: Union[Any, None] = state["size"] if state != None and "size" in state else None
 		self.type: Union[Any, None] = state["type"] if state != None and "type" in state else None
+		self.inActiveTabColor: Union[Any, None] = state["inActiveTabColor"] if state != None and "inActiveTabColor" in state else None
 		self.activeTabColor: Union[Any, None] = state["activeTabColor"] if state != None and "activeTabColor" in state else None
 		self.items: Union[Any, None] = state["items"] if state != None and "items" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def centered(self):
@@ -63,14 +64,22 @@
 		self._getter_access_tracker["type"] = {}
 		return self._type
 	@type.setter
 	def type(self, state):
 		self._setter_access_tracker["type"] = {}
 		self._type = state
 	@property
+	def inActiveTabColor(self):
+		self._getter_access_tracker["inActiveTabColor"] = {}
+		return self._inActiveTabColor
+	@inActiveTabColor.setter
+	def inActiveTabColor(self, state):
+		self._setter_access_tracker["inActiveTabColor"] = {}
+		self._inActiveTabColor = state
+	@property
 	def activeTabColor(self):
 		self._getter_access_tracker["activeTabColor"] = {}
 		return self._activeTabColor
 	@activeTabColor.setter
 	def activeTabColor(self, state):
 		self._setter_access_tracker["activeTabColor"] = {}
 		self._activeTabColor = state
@@ -80,24 +89,26 @@
 		return self._items
 	@items.setter
 	def items(self, state):
 		self._setter_access_tracker["items"] = {}
 		self._items = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"centered": self._centered,
 			"animated": self._animated,
 			"addIcon": self._addIcon,
 			"tabPosition": self._tabPosition,
 			"size": self._size,
 			"type": self._type,
+			"inActiveTabColor": self._inActiveTabColor,
 			"activeTabColor": self._activeTabColor,
 			"items": self._items
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Tabs(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -114,11 +125,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = TabsCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Tag.py` & `atri_react-1.0.0a26/src/atri_react/Tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,57 +4,33 @@
 
 
 class TagCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
 		self.text: Union[Any, None] = state["text"] if state != None and "text" in state else None
-		self.closable: Union[Any, None] = state["closable"] if state != None and "closable" in state else None
-		self.link: Union[Any, None] = state["link"] if state != None and "link" in state else None
-		self.color: Union[Any, None] = state["color"] if state != None and "color" in state else None
 		self.variant: Union[Any, None] = state["variant"] if state != None and "variant" in state else None
 		self.icon: Union[Any, None] = state["icon"] if state != None and "icon" in state else None
 		self.iconVariant: Union[Any, None] = state["iconVariant"] if state != None and "iconVariant" in state else None
+		self.closable: Union[Any, None] = state["closable"] if state != None and "closable" in state else None
 		self.closeIcon: Union[Any, None] = state["closeIcon"] if state != None and "closeIcon" in state else None
+		self.link: Union[Any, None] = state["link"] if state != None and "link" in state else None
+		self.color: Union[Any, None] = state["color"] if state != None and "color" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def text(self):
 		self._getter_access_tracker["text"] = {}
 		return self._text
 	@text.setter
 	def text(self, state):
 		self._setter_access_tracker["text"] = {}
 		self._text = state
 	@property
-	def closable(self):
-		self._getter_access_tracker["closable"] = {}
-		return self._closable
-	@closable.setter
-	def closable(self, state):
-		self._setter_access_tracker["closable"] = {}
-		self._closable = state
-	@property
-	def link(self):
-		self._getter_access_tracker["link"] = {}
-		return self._link
-	@link.setter
-	def link(self, state):
-		self._setter_access_tracker["link"] = {}
-		self._link = state
-	@property
-	def color(self):
-		self._getter_access_tracker["color"] = {}
-		return self._color
-	@color.setter
-	def color(self, state):
-		self._setter_access_tracker["color"] = {}
-		self._color = state
-	@property
 	def variant(self):
 		self._getter_access_tracker["variant"] = {}
 		return self._variant
 	@variant.setter
 	def variant(self, state):
 		self._setter_access_tracker["variant"] = {}
 		self._variant = state
@@ -71,33 +47,58 @@
 		self._getter_access_tracker["iconVariant"] = {}
 		return self._iconVariant
 	@iconVariant.setter
 	def iconVariant(self, state):
 		self._setter_access_tracker["iconVariant"] = {}
 		self._iconVariant = state
 	@property
+	def closable(self):
+		self._getter_access_tracker["closable"] = {}
+		return self._closable
+	@closable.setter
+	def closable(self, state):
+		self._setter_access_tracker["closable"] = {}
+		self._closable = state
+	@property
 	def closeIcon(self):
 		self._getter_access_tracker["closeIcon"] = {}
 		return self._closeIcon
 	@closeIcon.setter
 	def closeIcon(self, state):
 		self._setter_access_tracker["closeIcon"] = {}
 		self._closeIcon = state
+	@property
+	def link(self):
+		self._getter_access_tracker["link"] = {}
+		return self._link
+	@link.setter
+	def link(self, state):
+		self._setter_access_tracker["link"] = {}
+		self._link = state
+	@property
+	def color(self):
+		self._getter_access_tracker["color"] = {}
+		return self._color
+	@color.setter
+	def color(self, state):
+		self._setter_access_tracker["color"] = {}
+		self._color = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"text": self._text,
-			"closable": self._closable,
-			"link": self._link,
-			"color": self._color,
 			"variant": self._variant,
 			"icon": self._icon,
 			"iconVariant": self._iconVariant,
-			"closeIcon": self._closeIcon
+			"closable": self._closable,
+			"closeIcon": self._closeIcon,
+			"link": self._link,
+			"color": self._color
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Tag(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -114,11 +115,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = TagCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Testimonial.py` & `atri_react-1.0.0a26/src/atri_react/Timeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,96 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class TestimonialCustomClass():
+class TimelineCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.startTile: Union[Any, None] = state["startTile"] if state != None and "startTile" in state else None
-		self.intervalTime: Union[Any, None] = state["intervalTime"] if state != None and "intervalTime" in state else None
-		self.testimonials: Union[Any, None] = state["testimonials"] if state != None and "testimonials" in state else None
+		self.items: Union[Any, None] = state["items"] if state != None and "items" in state else None
+		self.mode: Union[Any, None] = state["mode"] if state != None and "mode" in state else None
+		self.pending: Union[Any, None] = state["pending"] if state != None and "pending" in state else None
+		self.pendingDot: Union[Any, None] = state["pendingDot"] if state != None and "pendingDot" in state else None
+		self.reverse: Union[Any, None] = state["reverse"] if state != None and "reverse" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def startTile(self):
-		self._getter_access_tracker["startTile"] = {}
-		return self._startTile
-	@startTile.setter
-	def startTile(self, state):
-		self._setter_access_tracker["startTile"] = {}
-		self._startTile = state
-	@property
-	def intervalTime(self):
-		self._getter_access_tracker["intervalTime"] = {}
-		return self._intervalTime
-	@intervalTime.setter
-	def intervalTime(self, state):
-		self._setter_access_tracker["intervalTime"] = {}
-		self._intervalTime = state
-	@property
-	def testimonials(self):
-		self._getter_access_tracker["testimonials"] = {}
-		return self._testimonials
-	@testimonials.setter
-	def testimonials(self, state):
-		self._setter_access_tracker["testimonials"] = {}
-		self._testimonials = state
+	def items(self):
+		self._getter_access_tracker["items"] = {}
+		return self._items
+	@items.setter
+	def items(self, state):
+		self._setter_access_tracker["items"] = {}
+		self._items = state
+	@property
+	def mode(self):
+		self._getter_access_tracker["mode"] = {}
+		return self._mode
+	@mode.setter
+	def mode(self, state):
+		self._setter_access_tracker["mode"] = {}
+		self._mode = state
+	@property
+	def pending(self):
+		self._getter_access_tracker["pending"] = {}
+		return self._pending
+	@pending.setter
+	def pending(self, state):
+		self._setter_access_tracker["pending"] = {}
+		self._pending = state
+	@property
+	def pendingDot(self):
+		self._getter_access_tracker["pendingDot"] = {}
+		return self._pendingDot
+	@pendingDot.setter
+	def pendingDot(self, state):
+		self._setter_access_tracker["pendingDot"] = {}
+		self._pendingDot = state
+	@property
+	def reverse(self):
+		self._getter_access_tracker["reverse"] = {}
+		return self._reverse
+	@reverse.setter
+	def reverse(self, state):
+		self._setter_access_tracker["reverse"] = {}
+		self._reverse = state
 
 	def _to_json_fields(self):
-		return {
-			"startTile": self._startTile,
-			"intervalTime": self._intervalTime,
-			"testimonials": self._testimonials
+		all_fields = {
+			"items": self._items,
+			"mode": self._mode,
+			"pending": self._pending,
+			"pendingDot": self._pendingDot,
+			"reverse": self._reverse
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class Testimonial(AtriComponent):
+class Timeline(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "Testimonial"
+		self.compKey = "Timeline"
 		self.nodePkg = "@atrilabs/react-component-manifests"
-		self.onClick = False
+		
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = TestimonialCustomClass(state)
+		self._custom = TimelineCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/TextBox.py` & `atri_react-1.0.0a26/src/atri_react/TreemapChart.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,86 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class TextBoxCustomClass():
+class TreemapChartCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.text: Union[Any, None] = state["text"] if state != None and "text" in state else None
+		self.data: Union[Any, None] = state["data"] if state != None and "data" in state else None
+		self.treemap: Union[Any, None] = state["treemap"] if state != None and "treemap" in state else None
+		self.chartHeight: Union[Any, None] = state["chartHeight"] if state != None and "chartHeight" in state else None
+		self.chartWidth: Union[Any, None] = state["chartWidth"] if state != None and "chartWidth" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def text(self):
-		self._getter_access_tracker["text"] = {}
-		return self._text
-	@text.setter
-	def text(self, state):
-		self._setter_access_tracker["text"] = {}
-		self._text = state
+	def data(self):
+		self._getter_access_tracker["data"] = {}
+		return self._data
+	@data.setter
+	def data(self, state):
+		self._setter_access_tracker["data"] = {}
+		self._data = state
+	@property
+	def treemap(self):
+		self._getter_access_tracker["treemap"] = {}
+		return self._treemap
+	@treemap.setter
+	def treemap(self, state):
+		self._setter_access_tracker["treemap"] = {}
+		self._treemap = state
+	@property
+	def chartHeight(self):
+		self._getter_access_tracker["chartHeight"] = {}
+		return self._chartHeight
+	@chartHeight.setter
+	def chartHeight(self, state):
+		self._setter_access_tracker["chartHeight"] = {}
+		self._chartHeight = state
+	@property
+	def chartWidth(self):
+		self._getter_access_tracker["chartWidth"] = {}
+		return self._chartWidth
+	@chartWidth.setter
+	def chartWidth(self, state):
+		self._setter_access_tracker["chartWidth"] = {}
+		self._chartWidth = state
 
 	def _to_json_fields(self):
-		return {
-			"text": self._text
+		all_fields = {
+			"data": self._data,
+			"treemap": self._treemap,
+			"chartHeight": self._chartHeight,
+			"chartWidth": self._chartWidth
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class TextBox(AtriComponent):
+class TreemapChart(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "TextBox"
+		self.compKey = "TreemapChart"
 		self.nodePkg = "@atrilabs/react-component-manifests"
-		self.onClick = False
+		
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = TextBoxCustomClass(state)
+		self._custom = TreemapChartCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Textarea.py` & `atri_react-1.0.0a26/src/atri_react/Textarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,26 +98,27 @@
 		return self._showCount
 	@showCount.setter
 	def showCount(self, state):
 		self._setter_access_tracker["showCount"] = {}
 		self._showCount = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"defaultValue": self._defaultValue,
 			"placeholder": self._placeholder,
 			"value": self._value,
 			"size": self._size,
 			"allowClear": self._allowClear,
 			"bordered": self._bordered,
 			"disabled": self._disabled,
 			"id": self._id,
 			"maxLength": self._maxLength,
 			"showCount": self._showCount
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Textarea(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -135,11 +136,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = TextareaCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/TimePicker.py` & `atri_react-1.0.0a26/src/atri_react/Upload.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,119 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class TimePickerCustomClass():
+class UploadCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.use12Hours: Union[Any, None] = state["use12Hours"] if state != None and "use12Hours" in state else None
-		self.size: Union[Any, None] = state["size"] if state != None and "size" in state else None
-		self.format: Union[Any, None] = state["format"] if state != None and "format" in state else None
-		self.bordered: Union[Any, None] = state["bordered"] if state != None and "bordered" in state else None
+		self.text: Union[Any, None] = state["text"] if state != None and "text" in state else None
+		self.listType: Union[Any, None] = state["listType"] if state != None and "listType" in state else None
+		self.dragger: Union[Any, None] = state["dragger"] if state != None and "dragger" in state else None
+		self.maxCount: Union[Any, None] = state["maxCount"] if state != None and "maxCount" in state else None
+		self.multiple: Union[Any, None] = state["multiple"] if state != None and "multiple" in state else None
 		self.disabled: Union[Any, None] = state["disabled"] if state != None and "disabled" in state else None
-		self.status: Union[Any, None] = state["status"] if state != None and "status" in state else None
-		self.range: Union[Any, None] = state["range"] if state != None and "range" in state else None
+		self.directory: Union[Any, None] = state["directory"] if state != None and "directory" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def use12Hours(self):
-		self._getter_access_tracker["use12Hours"] = {}
-		return self._use12Hours
-	@use12Hours.setter
-	def use12Hours(self, state):
-		self._setter_access_tracker["use12Hours"] = {}
-		self._use12Hours = state
-	@property
-	def size(self):
-		self._getter_access_tracker["size"] = {}
-		return self._size
-	@size.setter
-	def size(self, state):
-		self._setter_access_tracker["size"] = {}
-		self._size = state
-	@property
-	def format(self):
-		self._getter_access_tracker["format"] = {}
-		return self._format
-	@format.setter
-	def format(self, state):
-		self._setter_access_tracker["format"] = {}
-		self._format = state
-	@property
-	def bordered(self):
-		self._getter_access_tracker["bordered"] = {}
-		return self._bordered
-	@bordered.setter
-	def bordered(self, state):
-		self._setter_access_tracker["bordered"] = {}
-		self._bordered = state
+	def text(self):
+		self._getter_access_tracker["text"] = {}
+		return self._text
+	@text.setter
+	def text(self, state):
+		self._setter_access_tracker["text"] = {}
+		self._text = state
+	@property
+	def listType(self):
+		self._getter_access_tracker["listType"] = {}
+		return self._listType
+	@listType.setter
+	def listType(self, state):
+		self._setter_access_tracker["listType"] = {}
+		self._listType = state
+	@property
+	def dragger(self):
+		self._getter_access_tracker["dragger"] = {}
+		return self._dragger
+	@dragger.setter
+	def dragger(self, state):
+		self._setter_access_tracker["dragger"] = {}
+		self._dragger = state
+	@property
+	def maxCount(self):
+		self._getter_access_tracker["maxCount"] = {}
+		return self._maxCount
+	@maxCount.setter
+	def maxCount(self, state):
+		self._setter_access_tracker["maxCount"] = {}
+		self._maxCount = state
+	@property
+	def multiple(self):
+		self._getter_access_tracker["multiple"] = {}
+		return self._multiple
+	@multiple.setter
+	def multiple(self, state):
+		self._setter_access_tracker["multiple"] = {}
+		self._multiple = state
 	@property
 	def disabled(self):
 		self._getter_access_tracker["disabled"] = {}
 		return self._disabled
 	@disabled.setter
 	def disabled(self, state):
 		self._setter_access_tracker["disabled"] = {}
 		self._disabled = state
 	@property
-	def status(self):
-		self._getter_access_tracker["status"] = {}
-		return self._status
-	@status.setter
-	def status(self, state):
-		self._setter_access_tracker["status"] = {}
-		self._status = state
-	@property
-	def range(self):
-		self._getter_access_tracker["range"] = {}
-		return self._range
-	@range.setter
-	def range(self, state):
-		self._setter_access_tracker["range"] = {}
-		self._range = state
+	def directory(self):
+		self._getter_access_tracker["directory"] = {}
+		return self._directory
+	@directory.setter
+	def directory(self, state):
+		self._setter_access_tracker["directory"] = {}
+		self._directory = state
 
 	def _to_json_fields(self):
-		return {
-			"use12Hours": self._use12Hours,
-			"size": self._size,
-			"format": self._format,
-			"bordered": self._bordered,
+		all_fields = {
+			"text": self._text,
+			"listType": self._listType,
+			"dragger": self._dragger,
+			"maxCount": self._maxCount,
+			"multiple": self._multiple,
 			"disabled": self._disabled,
-			"status": self._status,
-			"range": self._range
+			"directory": self._directory
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class TimePicker(AtriComponent):
+class Upload(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "TimePicker"
+		self.compKey = "Upload"
 		self.nodePkg = "@atrilabs/react-component-manifests"
-		self.onClick = False
+		self.onChange = False
+		self.beforeUpload = False
+		self.onDrop = False
+		self.onPreview = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = TimePickerCustomClass(state)
+		self._custom = UploadCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Timeline.py` & `atri_react-1.0.0a26/src/atri_react/Dropdown.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,66 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class TimelineCustomClass():
+class DropdownCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.items: Union[Any, None] = state["items"] if state != None and "items" in state else None
-		self.mode: Union[Any, None] = state["mode"] if state != None and "mode" in state else None
-		self.pending: Union[Any, None] = state["pending"] if state != None and "pending" in state else None
-		self.pendingDot: Union[Any, None] = state["pendingDot"] if state != None and "pendingDot" in state else None
-		self.reverse: Union[Any, None] = state["reverse"] if state != None and "reverse" in state else None
+		self.selectedValue: Union[Any, None] = state["selectedValue"] if state != None and "selectedValue" in state else None
+		self.dropdownItems: Union[Any, None] = state["dropdownItems"] if state != None and "dropdownItems" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def items(self):
-		self._getter_access_tracker["items"] = {}
-		return self._items
-	@items.setter
-	def items(self, state):
-		self._setter_access_tracker["items"] = {}
-		self._items = state
-	@property
-	def mode(self):
-		self._getter_access_tracker["mode"] = {}
-		return self._mode
-	@mode.setter
-	def mode(self, state):
-		self._setter_access_tracker["mode"] = {}
-		self._mode = state
-	@property
-	def pending(self):
-		self._getter_access_tracker["pending"] = {}
-		return self._pending
-	@pending.setter
-	def pending(self, state):
-		self._setter_access_tracker["pending"] = {}
-		self._pending = state
-	@property
-	def pendingDot(self):
-		self._getter_access_tracker["pendingDot"] = {}
-		return self._pendingDot
-	@pendingDot.setter
-	def pendingDot(self, state):
-		self._setter_access_tracker["pendingDot"] = {}
-		self._pendingDot = state
-	@property
-	def reverse(self):
-		self._getter_access_tracker["reverse"] = {}
-		return self._reverse
-	@reverse.setter
-	def reverse(self, state):
-		self._setter_access_tracker["reverse"] = {}
-		self._reverse = state
+	def selectedValue(self):
+		self._getter_access_tracker["selectedValue"] = {}
+		return self._selectedValue
+	@selectedValue.setter
+	def selectedValue(self, state):
+		self._setter_access_tracker["selectedValue"] = {}
+		self._selectedValue = state
+	@property
+	def dropdownItems(self):
+		self._getter_access_tracker["dropdownItems"] = {}
+		return self._dropdownItems
+	@dropdownItems.setter
+	def dropdownItems(self, state):
+		self._setter_access_tracker["dropdownItems"] = {}
+		self._dropdownItems = state
 
 	def _to_json_fields(self):
-		return {
-			"items": self._items,
-			"mode": self._mode,
-			"pending": self._pending,
-			"pendingDot": self._pendingDot,
-			"reverse": self._reverse
+		all_fields = {
+			"selectedValue": self._selectedValue,
+			"dropdownItems": self._dropdownItems
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class Timeline(AtriComponent):
+class Dropdown(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "Timeline"
+		self.compKey = "Dropdown"
 		self.nodePkg = "@atrilabs/react-component-manifests"
-		
+		self.onChange = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = TimelineCustomClass(state)
+		self._custom = DropdownCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Toggle.py` & `atri_react-1.0.0a26/src/atri_react/Toggle.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,19 +35,20 @@
 		return self._inactiveColor
 	@inactiveColor.setter
 	def inactiveColor(self, state):
 		self._setter_access_tracker["inactiveColor"] = {}
 		self._inactiveColor = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"active": self._active,
 			"activeColor": self._activeColor,
 			"inactiveColor": self._inactiveColor
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Toggle(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -64,11 +65,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = ToggleCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Tree.py` & `atri_react-1.0.0a26/src/atri_react/Tree.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,22 +62,23 @@
 		return self._defaultExpandParent
 	@defaultExpandParent.setter
 	def defaultExpandParent(self, state):
 		self._setter_access_tracker["defaultExpandParent"] = {}
 		self._defaultExpandParent = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"treeData": self._treeData,
 			"checkable": self._checkable,
 			"showLine": self._showLine,
 			"multiple": self._multiple,
 			"defaultExpandAll": self._defaultExpandAll,
 			"defaultExpandParent": self._defaultExpandParent
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Tree(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -97,11 +98,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = TreeCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/UnorderedList.py` & `atri_react-1.0.0a26/src/atri_react/UnorderedList.py`

 * *Files 8% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 		return self._xxl
 	@xxl.setter
 	def xxl(self, state):
 		self._setter_access_tracker["xxl"] = {}
 		self._xxl = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"size": self._size,
 			"itemLayout": self._itemLayout,
 			"bordered": self._bordered,
 			"split": self._split,
 			"items": self._items,
 			"actionAdd": self._actionAdd,
 			"actionUpdate": self._actionUpdate,
@@ -210,14 +210,15 @@
 			"xs": self._xs,
 			"sm": self._sm,
 			"md": self._md,
 			"lg": self._lg,
 			"xl": self._xl,
 			"xxl": self._xxl
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class UnorderedList(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -234,11 +235,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = UnorderedListCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Upload.py` & `atri_react-1.0.0a26/src/atri_react/TimePicker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,136 @@
 from typing import Any, Union
 from atri_core import AtriComponent
 
 
 
-class UploadCustomClass():
+class TimePickerCustomClass():
 	def __init__(self, state: Union[Any, None]):
 		self._setter_access_tracker = {}
 		
-		self.text: Union[Any, None] = state["text"] if state != None and "text" in state else None
-		self.listType: Union[Any, None] = state["listType"] if state != None and "listType" in state else None
-		self.dragger: Union[Any, None] = state["dragger"] if state != None and "dragger" in state else None
-		self.maxCount: Union[Any, None] = state["maxCount"] if state != None and "maxCount" in state else None
-		self.multiple: Union[Any, None] = state["multiple"] if state != None and "multiple" in state else None
+		self.use12Hours: Union[Any, None] = state["use12Hours"] if state != None and "use12Hours" in state else None
+		self.size: Union[Any, None] = state["size"] if state != None and "size" in state else None
+		self.placement: Union[Any, None] = state["placement"] if state != None and "placement" in state else None
+		self.format: Union[Any, None] = state["format"] if state != None and "format" in state else None
+		self.placeholder: Union[Any, None] = state["placeholder"] if state != None and "placeholder" in state else None
+		self.bordered: Union[Any, None] = state["bordered"] if state != None and "bordered" in state else None
 		self.disabled: Union[Any, None] = state["disabled"] if state != None and "disabled" in state else None
-		self.directory: Union[Any, None] = state["directory"] if state != None and "directory" in state else None
+		self.status: Union[Any, None] = state["status"] if state != None and "status" in state else None
+		self.range: Union[Any, None] = state["range"] if state != None and "range" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
-	def text(self):
-		self._getter_access_tracker["text"] = {}
-		return self._text
-	@text.setter
-	def text(self, state):
-		self._setter_access_tracker["text"] = {}
-		self._text = state
-	@property
-	def listType(self):
-		self._getter_access_tracker["listType"] = {}
-		return self._listType
-	@listType.setter
-	def listType(self, state):
-		self._setter_access_tracker["listType"] = {}
-		self._listType = state
-	@property
-	def dragger(self):
-		self._getter_access_tracker["dragger"] = {}
-		return self._dragger
-	@dragger.setter
-	def dragger(self, state):
-		self._setter_access_tracker["dragger"] = {}
-		self._dragger = state
-	@property
-	def maxCount(self):
-		self._getter_access_tracker["maxCount"] = {}
-		return self._maxCount
-	@maxCount.setter
-	def maxCount(self, state):
-		self._setter_access_tracker["maxCount"] = {}
-		self._maxCount = state
-	@property
-	def multiple(self):
-		self._getter_access_tracker["multiple"] = {}
-		return self._multiple
-	@multiple.setter
-	def multiple(self, state):
-		self._setter_access_tracker["multiple"] = {}
-		self._multiple = state
+	def use12Hours(self):
+		self._getter_access_tracker["use12Hours"] = {}
+		return self._use12Hours
+	@use12Hours.setter
+	def use12Hours(self, state):
+		self._setter_access_tracker["use12Hours"] = {}
+		self._use12Hours = state
+	@property
+	def size(self):
+		self._getter_access_tracker["size"] = {}
+		return self._size
+	@size.setter
+	def size(self, state):
+		self._setter_access_tracker["size"] = {}
+		self._size = state
+	@property
+	def placement(self):
+		self._getter_access_tracker["placement"] = {}
+		return self._placement
+	@placement.setter
+	def placement(self, state):
+		self._setter_access_tracker["placement"] = {}
+		self._placement = state
+	@property
+	def format(self):
+		self._getter_access_tracker["format"] = {}
+		return self._format
+	@format.setter
+	def format(self, state):
+		self._setter_access_tracker["format"] = {}
+		self._format = state
+	@property
+	def placeholder(self):
+		self._getter_access_tracker["placeholder"] = {}
+		return self._placeholder
+	@placeholder.setter
+	def placeholder(self, state):
+		self._setter_access_tracker["placeholder"] = {}
+		self._placeholder = state
+	@property
+	def bordered(self):
+		self._getter_access_tracker["bordered"] = {}
+		return self._bordered
+	@bordered.setter
+	def bordered(self, state):
+		self._setter_access_tracker["bordered"] = {}
+		self._bordered = state
 	@property
 	def disabled(self):
 		self._getter_access_tracker["disabled"] = {}
 		return self._disabled
 	@disabled.setter
 	def disabled(self, state):
 		self._setter_access_tracker["disabled"] = {}
 		self._disabled = state
 	@property
-	def directory(self):
-		self._getter_access_tracker["directory"] = {}
-		return self._directory
-	@directory.setter
-	def directory(self, state):
-		self._setter_access_tracker["directory"] = {}
-		self._directory = state
+	def status(self):
+		self._getter_access_tracker["status"] = {}
+		return self._status
+	@status.setter
+	def status(self, state):
+		self._setter_access_tracker["status"] = {}
+		self._status = state
+	@property
+	def range(self):
+		self._getter_access_tracker["range"] = {}
+		return self._range
+	@range.setter
+	def range(self, state):
+		self._setter_access_tracker["range"] = {}
+		self._range = state
 
 	def _to_json_fields(self):
-		return {
-			"text": self._text,
-			"listType": self._listType,
-			"dragger": self._dragger,
-			"maxCount": self._maxCount,
-			"multiple": self._multiple,
+		all_fields = {
+			"use12Hours": self._use12Hours,
+			"size": self._size,
+			"placement": self._placement,
+			"format": self._format,
+			"placeholder": self._placeholder,
+			"bordered": self._bordered,
 			"disabled": self._disabled,
-			"directory": self._directory
+			"status": self._status,
+			"range": self._range
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
-class Upload(AtriComponent):
+class TimePicker(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
-		self.compKey = "Upload"
+		self.compKey = "TimePicker"
 		self.nodePkg = "@atrilabs/react-component-manifests"
-		self.onChange = False
-		self.beforeUpload = False
-		self.onDrop = False
-		self.onPreview = False
+		self.onClick = False
 		self.custom = state["custom"] if state != None and "custom" in state else None
 		self._setter_access_tracker = {}
 		self._getter_access_tracker = {}
 
 	@property
 	def custom(self):
 		self._getter_access_tracker["custom"] = {}
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
-		self._custom = UploadCustomClass(state)
+		self._custom = TimePickerCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/VerticalMenu.py` & `atri_react-1.0.0a26/src/atri_react/VerticalMenu.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 		return self._menuItems
 	@menuItems.setter
 	def menuItems(self, state):
 		self._setter_access_tracker["menuItems"] = {}
 		self._menuItems = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"menuItems": self._menuItems
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class VerticalMenu(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -44,11 +45,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = VerticalMenuCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/Video.py` & `atri_react-1.0.0a26/src/atri_react/Video.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 		return self._config
 	@config.setter
 	def config(self, state):
 		self._setter_access_tracker["config"] = {}
 		self._config = state
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"playing": self._playing,
 			"url": self._url,
 			"light": self._light,
 			"loop": self._loop,
 			"controls": self._controls,
 			"volume": self._volume,
 			"muted": self._muted,
@@ -170,14 +170,15 @@
 			"playIcon": self._playIcon,
 			"previewTabIndex": self._previewTabIndex,
 			"pip": self._pip,
 			"stopOnUnmount": self._stopOnUnmount,
 			"fallback": self._fallback,
 			"config": self._config
 			}
+		return {k: v for k, v in all_fields.items() if v is not None}
 
 
 class Video(AtriComponent):
 	def __init__(self, state: Union[Any, None]):
 		super().__init__(state)
 		self._setter_access_tracker = {}
 		
@@ -214,11 +215,12 @@
 		return self._custom
 	@custom.setter
 	def custom(self, state):
 		self._setter_access_tracker["custom"] = {}
 		self._custom = VideoCustomClass(state)
 
 	def _to_json_fields(self):
-		return {
+		all_fields = {
 			"styles": self._styles,
 			"custom": self._custom,
-			}
+			}
+		return {k: v for k, v in all_fields.items() if v is not None}
```

### Comparing `atri_react-1.0.0a13/src/atri_react/__init__.py` & `atri_react-1.0.0a26/src/atri_react/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,58 @@
+from .Accordion import Accordion
 from .Alert import Alert
 from .Anchor import Anchor
+from .Badge import Badge
+from .Card import Card
 from .Breadcrumb import Breadcrumb
 from .Button import Button
-from .Card import Card
-from .Carousel import Carousel
 from .Cascader import Cascader
+from .Carousel import Carousel
 from .Checkbox import Checkbox
 from .CodeMirror import CodeMirror
-from .Countup import Countup
+from .Div import Div
 from .Countdown import Countdown
+from .Countup import Countup
 from .DatePicker import DatePicker
+from .Drawer import Drawer
 from .Dropdown import Dropdown
-from .Flex import Flex
 from .Form import Form
+from .Flex import Flex
 from .Icon import Icon
-from .Image import Image
+from .Iframe import Iframe
 from .Input import Input
-from .Badge import Badge
 from .Link import Link
 from .Menu import Menu
-from .Modal import Modal
 from .Overlay import Overlay
-from .Radio import Radio
+from .Modal import Modal
 from .Rating import Rating
+from .Radio import Radio
+from .InputNumber import InputNumber
+from .Image import Image
 from .Repeating import Repeating
-from .Accordion import Accordion
+from .Search import Search
 from .Select import Select
-from .Slider import Slider
-from .Statistic import Statistic
 from .Step import Step
-from .Div import Div
-from .InputNumber import InputNumber
-from .Search import Search
-from .Tabs import Tabs
+from .Slider import Slider
+from .Table import Table
 from .Tag import Tag
-from .Testimonial import Testimonial
+from .Statistic import Statistic
 from .TextBox import TextBox
+from .Testimonial import Testimonial
 from .Textarea import Textarea
+from .Tabs import Tabs
 from .TimePicker import TimePicker
 from .Timeline import Timeline
+from .TinyMCE import TinyMCE
 from .Toggle import Toggle
 from .Tree import Tree
 from .UnorderedList import UnorderedList
 from .Upload import Upload
-from .VerticalMenu import VerticalMenu
 from .Video import Video
-from .Table import Table
+from .VerticalMenu import VerticalMenu
 from .AreaChart import AreaChart
 from .BarChart import BarChart
 from .CandleStick import CandleStick
 from .GanttChart import GanttChart
 from .HistogramChart import HistogramChart
 from .LineChart import LineChart
 from .PieChart import PieChart
```

### Comparing `atri_react-1.0.0a13/src/atri_react.egg-info/SOURCES.txt` & `atri_react-1.0.0a26/src/atri_react.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 src/atri_react/Cascader.py
 src/atri_react/Checkbox.py
 src/atri_react/CodeMirror.py
 src/atri_react/Countdown.py
 src/atri_react/Countup.py
 src/atri_react/DatePicker.py
 src/atri_react/Div.py
+src/atri_react/Drawer.py
 src/atri_react/Dropdown.py
 src/atri_react/Flex.py
 src/atri_react/Form.py
 src/atri_react/GanttChart.py
 src/atri_react/HistogramChart.py
 src/atri_react/Icon.py
+src/atri_react/Iframe.py
 src/atri_react/Image.py
 src/atri_react/Input.py
 src/atri_react/InputNumber.py
 src/atri_react/LineChart.py
 src/atri_react/Link.py
 src/atri_react/Menu.py
 src/atri_react/Modal.py
@@ -46,14 +48,15 @@
 src/atri_react/Tabs.py
 src/atri_react/Tag.py
 src/atri_react/Testimonial.py
 src/atri_react/TextBox.py
 src/atri_react/Textarea.py
 src/atri_react/TimePicker.py
 src/atri_react/Timeline.py
+src/atri_react/TinyMCE.py
 src/atri_react/Toggle.py
 src/atri_react/Tree.py
 src/atri_react/TreemapChart.py
 src/atri_react/UnorderedList.py
 src/atri_react/Upload.py
 src/atri_react/VerticalMenu.py
 src/atri_react/Video.py
```

### Comparing `atri_react-1.0.0a13/src/config/package.json` & `atri_react-1.0.0a26/src/config/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.892510775862069%*

 * *Differences: {"'dependencies'": "{'@atrilabs/app-design-forest': '^1.0.0-alpha.26', '@atrilabs/commands': "*

 * *                   "'^1.0.0-alpha.26', '@atrilabs/component-icon-manifest-schema': "*

 * *                   "'^1.0.0-alpha.26', '@atrilabs/core': '^1.0.0-alpha.26', "*

 * *                   "'@atrilabs/design-system': '^1.0.0-alpha.26', '@atrilabs/layer-types': "*

 * *                   "'^1.0.0-alpha.26', '@atrilabs/react-component-manifest-schema': "*

 * *                   "'^1.0.0-alpha.26', '@tinymce/tinymce-react': '^4.3.0',  […]*

```diff
@@ -3,38 +3,40 @@
         "pythonPackageName": "atri_react"
     },
     "author": "cruxcode <swaroopshyam0@gmail.com>",
     "bugs": {
         "url": "https://github.com/cruxcode/atrilabs-engine/issues"
     },
     "dependencies": {
-        "@atrilabs/app-design-forest": "^1.0.0-alpha.13",
-        "@atrilabs/commands": "^1.0.0-alpha.13",
-        "@atrilabs/component-icon-manifest-schema": "^1.0.0-alpha.13",
-        "@atrilabs/core": "^1.0.0-alpha.13",
-        "@atrilabs/design-system": "^1.0.0-alpha.13",
-        "@atrilabs/layer-types": "^1.0.0-alpha.13",
-        "@atrilabs/react-component-manifest-schema": "^1.0.0-alpha.13",
+        "@atrilabs/app-design-forest": "^1.0.0-alpha.26",
+        "@atrilabs/commands": "^1.0.0-alpha.26",
+        "@atrilabs/component-icon-manifest-schema": "^1.0.0-alpha.26",
+        "@atrilabs/core": "^1.0.0-alpha.26",
+        "@atrilabs/design-system": "^1.0.0-alpha.26",
+        "@atrilabs/layer-types": "^1.0.0-alpha.26",
+        "@atrilabs/react-component-manifest-schema": "^1.0.0-alpha.26",
         "@codemirror/lang-css": "^6.0.2",
         "@codemirror/lang-html": "^6.4.2",
         "@codemirror/lang-java": "^6.0.1",
         "@codemirror/lang-javascript": "^6.1.4",
         "@codemirror/lang-json": "^6.0.1",
         "@codemirror/lang-php": "^6.0.1",
         "@codemirror/lang-python": "^6.1.1",
         "@codemirror/lang-rust": "^6.0.1",
         "@codemirror/lang-sql": "^6.4.0",
         "@codemirror/lang-xml": "^6.0.2",
         "@emotion/react": "^11.10.0",
         "@emotion/styled": "^11.10.0",
         "@mui/material": "^5.10.0",
         "@mui/x-data-grid": "^5.15.2",
+        "@tinymce/tinymce-react": "^4.3.0",
         "@uiw/react-codemirror": "^4.19.9",
         "antd": "^5.3.0",
         "color": "^4.2.3",
+        "postcss-js": "^4.0.1",
         "react-player": "2.11.2",
         "recharts": "^2.1.13",
         "typescript": "^4.6.4"
     },
     "description": "> TODO: description",
     "devDependencies": {
         "@babel/cli": "^7.17.10",
@@ -54,25 +56,24 @@
         "react-router-dom": "^6.6.2"
     },
     "files": [
         "src",
         "dist/manifests.bundle.js",
         "dist/manifests.bundle.js.map"
     ],
-    "gitHead": "1e8d3a363d72346146d46969323f6ee1fc5fb18c",
     "homepage": "https://github.com/cruxcode/atrilabs-engine#readme",
     "license": "ISC",
     "main": "./src/manifest.config.js",
     "name": "@atrilabs/react-component-manifests",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "git+https://github.com/cruxcode/atrilabs-engine.git"
     },
     "scripts": {
-        "build": "gen-py-classes -n ../../node_modules -i '@atrilabs/utils' -a '@atrilabs/utils'",
+        "build": "gen-py-classes -n ../../node_modules -i \"@atrilabs/utils\" -a \"@atrilabs/utils\"",
         "prepublishOnly": "yarn build"
     },
-    "version": "1.0.0-alpha.13"
+    "version": "1.0.0-alpha.26"
 }
```

