# Comparing `tmp/tinymovr-1.3.0.tar.gz` & `tmp/tinymovr-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinymovr-1.3.0.tar", last modified: Mon Apr 17 16:52:37 2023, max compression
+gzip compressed data, was "tinymovr-1.3.1.tar", last modified: Thu Apr 20 17:25:49 2023, max compression
```

## Comparing `tinymovr-1.3.0.tar` & `tinymovr-1.3.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.496353 tinymovr-1.3.0/
--rw-r--r--   0 yanconst   (501) staff       (20)       87 2023-04-10 19:14:46.000000 tinymovr-1.3.0/MANIFEST.in
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-17 16:52:37.496191 tinymovr-1.3.0/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.3.0/README.md
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.490282 tinymovr-1.3.0/resources/
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.491283 tinymovr-1.3.0/resources/icons/
--rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-08 07:47:15.000000 tinymovr-1.3.0/resources/icons/call.png
--rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-17 16:52:37.496399 tinymovr-1.3.0/setup.cfg
--rw-r--r--   0 yanconst   (501) staff       (20)     2334 2023-04-17 16:47:58.000000 tinymovr-1.3.0/setup.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.492837 tinymovr-1.3.0/tinymovr/
--rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3529 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/channel.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2882 2023-04-10 19:03:18.000000 tinymovr-1.3.0/tinymovr/cli.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.494371 tinymovr-1.3.0/tinymovr/codec/
--rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.3.0/tinymovr/codec/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/codec/codec.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.494898 tinymovr-1.3.0/tinymovr/config/
--rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/config/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3358 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/config/config.py
--rw-r--r--   0 yanconst   (501) staff       (20)    15484 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/config/device.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/constants.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/discovery.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.495977 tinymovr-1.3.0/tinymovr/gui/
--rw-r--r--   0 yanconst   (501) staff       (20)      411 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/gui/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1718 2023-04-17 16:47:58.000000 tinymovr-1.3.0/tinymovr/gui/gui.py
--rw-r--r--   0 yanconst   (501) staff       (20)     8904 2023-04-17 16:47:58.000000 tinymovr-1.3.0/tinymovr/gui/helpers.py
--rw-r--r--   0 yanconst   (501) staff       (20)    12207 2023-04-17 16:47:58.000000 tinymovr-1.3.0/tinymovr/gui/window.py
--rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-17 16:47:58.000000 tinymovr-1.3.0/tinymovr/gui/worker.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3088 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/tee.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.493975 tinymovr-1.3.0/tinymovr.egg-info/
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)      614 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/SOURCES.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/dependency_links.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/entry_points.txt
--rw-r--r--   0 yanconst   (501) staff       (20)      166 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/requires.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/top_level.txt
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.371284 tinymovr-1.3.1/
+-rw-r--r--   0 yanconst   (501) staff       (20)      185 2023-04-20 17:24:50.000000 tinymovr-1.3.1/MANIFEST.in
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-20 17:25:49.371103 tinymovr-1.3.1/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.3.1/README.md
+-rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-20 17:25:49.371333 tinymovr-1.3.1/setup.cfg
+-rw-r--r--   0 yanconst   (501) staff       (20)     2334 2023-04-17 16:47:58.000000 tinymovr-1.3.1/setup.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.367184 tinymovr-1.3.1/tinymovr/
+-rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3529 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2845 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/cli.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.368698 tinymovr-1.3.1/tinymovr/codec/
+-rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.3.1/tinymovr/codec/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/codec/codec.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.369262 tinymovr-1.3.1/tinymovr/config/
+-rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/config/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3358 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/config/config.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    15484 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/config/device.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/constants.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/discovery.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.370190 tinymovr-1.3.1/tinymovr/gui/
+-rw-r--r--   0 yanconst   (501) staff       (20)      431 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/gui/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1582 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/gui/gui.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     9660 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/gui/helpers.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    12203 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/gui/window.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-17 16:47:58.000000 tinymovr-1.3.1/tinymovr/gui/worker.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.365294 tinymovr-1.3.1/tinymovr/resources/
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.370838 tinymovr-1.3.1/tinymovr/resources/icons/
+-rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/resources/icons/call.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    12497 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/resources/icons/empty.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    30143 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/resources/icons/empty@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)     3088 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/tee.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.368297 tinymovr-1.3.1/tinymovr.egg-info/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)      696 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/SOURCES.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/dependency_links.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/entry_points.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)      166 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/requires.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/top_level.txt
```

### Comparing `tinymovr-1.3.0/PKG-INFO` & `tinymovr-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.3.0/README.md` & `tinymovr-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/resources/icons/call.png` & `tinymovr-1.3.1/tinymovr/resources/icons/call.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/setup.py` & `tinymovr-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/tinymovr/channel.py` & `tinymovr-1.3.1/tinymovr/channel.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/tinymovr/cli.py` & `tinymovr-1.3.1/tinymovr/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,12 +79,11 @@
     print(app_name + " " + str(version))
 
     init_tee(can.Bus(**params))
     dsc = Discovery(node_appeared, node_disappeared, logger)
     print("Listening for nodes...")
 
     c = Config()
-    c.InteractiveShellApp.gui = "tk"
     c.TerminalIPythonApp.display_banner = False
     IPython.start_ipython(argv=[], config=c, user_ns=user_ns)
     logger.debug("Exiting...")
     destroy_tee()
```

### Comparing `tinymovr-1.3.0/tinymovr/codec/codec.py` & `tinymovr-1.3.1/tinymovr/codec/codec.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/tinymovr/config/config.py` & `tinymovr-1.3.1/tinymovr/config/config.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/tinymovr/config/device.yaml` & `tinymovr-1.3.1/tinymovr/config/device.yaml`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/tinymovr/constants.py` & `tinymovr-1.3.1/tinymovr/constants.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/tinymovr/discovery.py` & `tinymovr-1.3.1/tinymovr/discovery.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/tinymovr/gui/gui.py` & `tinymovr-1.3.1/tinymovr/gui/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,14 @@
 This program is distributed in the hope that it will be useful, but WITHOUT
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
-# https://www.loekvandenouweland.com/content/pyside2-big-sur-does-not-show-window.html
-import os
-os.environ['QT_MAC_WANTS_LAYER'] = '1'
 
 def spawn():
     version = pkg_resources.require("tinymovr")[0].version
     arguments = docopt(__doc__, version=app_name + " " + str(version))
     app = QApplication(sys.argv)
     app.setStyleSheet(app_stylesheet)
     w = MainWindow(app, arguments)
```

### Comparing `tinymovr-1.3.0/tinymovr/gui/helpers.py` & `tinymovr-1.3.1/tinymovr/gui/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import time
 import os
 import enum
 import pint
-from PySide6 import QtGui, QtCore
-from PySide6.QtWidgets import QMessageBox, QFileDialog
+from PySide6 import QtGui
+from PySide6.QtWidgets import QMessageBox, QFileDialog, QTreeWidget
 from avlos.definitions import RemoteAttribute
+import tinymovr
 
 
 app_stylesheet = """
 
 /* --------------------------------------- QPushButton -----------------------------------*/
 
     QPushButton {
@@ -172,37 +173,61 @@
     QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical
     {
         background: none;
     }
 """
 
 
+class OurQTreeWidget(QTreeWidget):
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        self.placeholder_image = load_pixmap("empty.png")
+
+    def paintEvent(self, event):
+        if self.topLevelItemCount() == 0:
+            painter = QtGui.QPainter(self.viewport())
+            painter.setOpacity(0.5)  # Adjust the opacity of the placeholder image
+            painter.drawPixmap(
+                (self.viewport().width() - self.placeholder_image.width()) / 2,
+                (self.viewport().height() - self.placeholder_image.height()) / 2,
+                self.placeholder_image,
+            )
+        else:
+            super().paintEvent(event)
+
+
 def format_value(value, include_unit=True):
     """
     Format a numeric value according to its
     type and return the formatted string
     """
     if isinstance(value, enum.IntFlag):
         return str(value) if value > 0 else "(no flags)"
     if not include_unit and isinstance(value, pint.Quantity):
         return str(value.magnitude)
     if isinstance(value, float):
         return "{0:.6g}".format(value)
     return str(value)
 
 
+def load_pixmap(fname_pixmap):
+    """
+    Load an image from a file and return it as a QPixmap
+    """
+    file_path = os.path.join(
+        os.path.dirname(tinymovr.__file__), "resources", "icons", fname_pixmap
+    )
+    return QtGui.QPixmap(file_path)
+
+
 def load_icon(fname_icon):
     """
-    Load an image from a file and return it
-    as a QIcon
+    Load an image from a file and return it as a QIcon
     """
-    path_this_dir = os.path.dirname(os.path.abspath(__file__))
-    path_icons = os.path.join(path_this_dir, "..", "..", "resources", "icons")
-    path_icon = os.path.join(path_icons, fname_icon)
-    pixmap = QtGui.QPixmap(path_icon)
+    pixmap = load_pixmap(fname_icon)
     icon = QtGui.QIcon()
     icon.addPixmap(pixmap, QtGui.QIcon.Normal)
     icon.addPixmap(pixmap, QtGui.QIcon.Disabled)
     return icon
 
 
 def magnitude_of(val):
```

### Comparing `tinymovr-1.3.0/tinymovr/gui/window.py` & `tinymovr-1.3.1/tinymovr/gui/window.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,27 +27,27 @@
     QMenuBar,
     QWidget,
     QFrame,
     QHBoxLayout,
     QVBoxLayout,
     QHeaderView,
     QLabel,
-    QTreeWidget,
     QTreeWidgetItem,
     QPushButton,
 )
 from PySide6.QtGui import QAction
 import pyqtgraph as pg
 from tinymovr.constants import app_name
 from tinymovr.channel import ResponseError as ChannelResponseError
 from tinymovr.config import get_bus_config, configure_logging
 from avlos import get_registry
 from avlos.json_codec import AvlosEncoder
 from tinymovr.gui import (
     Worker,
+    OurQTreeWidget,
     format_value,
     load_icon,
     display_file_open_dialog,
     display_file_save_dialog,
     magnitude_of,
     check_selected_items,
 )
@@ -84,15 +84,15 @@
         self.file_menu.addAction(self.export_action)
         self.file_menu.addAction(self.import_action)
 
         self.menu_bar.addMenu(self.file_menu)
         self.setMenuBar(self.menu_bar)
 
         # Setup the tree widget
-        self.tree_widget = QTreeWidget()
+        self.tree_widget = OurQTreeWidget()
         self.tree_widget.itemChanged.connect(self.item_changed)
         self.tree_widget.itemDoubleClicked.connect(self.double_click)
         self.tree_widget.setHeaderLabels(["Attribute", "Value"])
 
         self.status_label = QLabel()
         self.status_label.setStyleSheet("margin: 5px;")
 
@@ -294,15 +294,15 @@
             column == 1
             and hasattr(item, "_tm_attribute")
             and hasattr(item._tm_attribute, "setter_name")
             and item._tm_attribute.setter_name != None
         ):
             item.setFlags(item.flags() | QtCore.Qt.ItemIsEditable)
             item._editing = True
-        elif int(item._orig_flags) != int(item.flags()):
+        elif item._orig_flags != item.flags():
             item.setFlags(item._orig_flags)
 
     def on_export(self):
         selected_items = self.tree_widget.selectedItems()
         if check_selected_items(selected_items):
             root_node = selected_items[0]._tm_attribute.root
             values_object = root_node.export_values()
```

### Comparing `tinymovr-1.3.0/tinymovr/gui/worker.py` & `tinymovr-1.3.1/tinymovr/gui/worker.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/tinymovr/tee.py` & `tinymovr-1.3.1/tinymovr/tee.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.0/tinymovr.egg-info/PKG-INFO` & `tinymovr-1.3.1/tinymovr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.3.0/tinymovr.egg-info/SOURCES.txt` & `tinymovr-1.3.1/tinymovr.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 MANIFEST.in
 README.md
 setup.py
-resources/icons/call.png
 tinymovr/__init__.py
 tinymovr/channel.py
 tinymovr/cli.py
 tinymovr/constants.py
 tinymovr/discovery.py
 tinymovr/tee.py
 tinymovr.egg-info/PKG-INFO
@@ -19,8 +18,11 @@
 tinymovr/config/__init__.py
 tinymovr/config/config.py
 tinymovr/config/device.yaml
 tinymovr/gui/__init__.py
 tinymovr/gui/gui.py
 tinymovr/gui/helpers.py
 tinymovr/gui/window.py
-tinymovr/gui/worker.py
+tinymovr/gui/worker.py
+tinymovr/resources/icons/call.png
+tinymovr/resources/icons/empty.png
+tinymovr/resources/icons/empty@2x.png
```

