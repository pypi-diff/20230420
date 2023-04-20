# Comparing `tmp/snaik-0.1.0.tar.gz` & `tmp/snaik-0.1.1.tar.gz`

## Comparing `snaik-0.1.0.tar` & `snaik-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 snaik-0.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 snaik-0.1.0/Dockerfile
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 snaik-0.1.0/requirements-pinned.txt
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 snaik-0.1.0/windist.Dockerfile
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/__main__.py
--rw-r--r--   0        0        0    12734 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/brain.py
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/food.py
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/game.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/leaderboard.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/snake.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/staterecorder.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/utils.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/window.py
--rw-r--r--   0        0        0   171676 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/resources/Roboto-Regular.ttf
--rw-r--r--   0        0        0     8502 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/resources/logo.svg
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 snaik-0.1.0/snaik/resources/sample_external.cpp
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 snaik-0.1.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snaik-0.1.0/README.md
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 snaik-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 snaik-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 snaik-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 snaik-0.1.1/Dockerfile
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snaik-0.1.1/requirements-pinned.txt
+-rw-r--r--   0        0        0   114502 2020-02-02 00:00:00.000000 snaik-0.1.1/states_homepage_gif - Copy.json
+-rw-r--r--   0        0        0   114502 2020-02-02 00:00:00.000000 snaik-0.1.1/states_homepage_gif.json
+-rw-r--r--   0        0        0    44937 2020-02-02 00:00:00.000000 snaik-0.1.1/tmp.png
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 snaik-0.1.1/windist.Dockerfile
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/__init__.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/__main__.py
+-rw-r--r--   0        0        0    12844 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/brain.py
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/food.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/game.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/leaderboard.py
+-rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/snake.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/staterecorder.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/utils.py
+-rw-r--r--   0        0        0     8095 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/window.py
+-rw-r--r--   0        0        0   171676 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/resources/Roboto-Regular.ttf
+-rw-r--r--   0        0        0     8502 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/resources/logo.svg
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 snaik-0.1.1/snaik/resources/sample_external.cpp
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 snaik-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 snaik-0.1.1/README.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 snaik-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11790 2020-02-02 00:00:00.000000 snaik-0.1.1/PKG-INFO
```

### Comparing `snaik-0.1.0/.gitlab-ci.yml` & `snaik-0.1.1/.gitlab-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 stages:
     - build
 
 .on_tagged_commit: &on_tagged_commit
     rules:
-#        - if: "$CI_COMMIT_TAG"
-        - when: always
+        - if: "$CI_COMMIT_TAG"
+#        - when: always
 
 .default_variables: &default_variables
     IMAGE_NAME: snaik
     IMAGE_TAG: latest
     DOCKERFILE: Dockerfile
 
 .docker-build-template: &docker-build-template
```

### Comparing `snaik-0.1.0/requirements-pinned.txt` & `snaik-0.1.1/requirements-pinned.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --extra=full --output-file=requirements-pinned.txt pyproject.toml
 #
-click==8.1.3
-    # via snaik (pyproject.toml)
-colorama==0.4.6
-    # via click
 darkdetect==0.7.1
     # via pyqtdarktheme
 imageio==2.27.0
     # via snaik (pyproject.toml)
 numpy==1.24.2
     # via
     #   imageio
```

### Comparing `snaik-0.1.0/snaik/__init__.py` & `snaik-0.1.1/snaik/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,10 +15,10 @@
             if depth == 0:
                 font.setPointSize(self.pointSize() + 1)
             self.setFont(c, font)
         self.titleChanged()
 
     GroupParameterItem.updateDepth = updateDepth
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 from snaik.game import Game
 from snaik.window import SnaikWindow
```

### Comparing `snaik-0.1.0/snaik/brain.py` & `snaik-0.1.1/snaik/brain.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         nsew_keys
             Keys to use for changing direction, can be any standard keyboard key, i.e.,
             "Up", "A", "Left", etc. Order should match which key should be pressed to
             go north, south, east, and west, respectively.
         """
         super().__init__(None)
         Key = QtCore.Qt.Key
+        nsew_keys = [k.upper() if len(k) == 1 else k for k in nsew_keys]
         qt_keys = [getattr(Key, f"Key_{key}") for key in nsew_keys]
         self.key_map = dict(zip(qt_keys, Direction))
         self.current_direction: Direction | None = None
         key_str = "".join(nsew_keys)
         self.__name__ = f"Keys `{key_str}`"
 
     def eventFilter(self, _obj: QtCore.QObject, event: QtCore.QEvent) -> bool:
@@ -338,26 +339,26 @@
 
 def get_external_brain(brain_name: str):
     try:
         return ExternalBrain(*brain_name.split(" "))
     except FileNotFoundError:
         raise ValueError(
             f"Brain `{brain_name}` not found, must be one of: "
-            f"{brain_factory.keys()} or a valid executable"
+            f"{brain_name_factory_map.keys()} or a valid executable"
         )
 
 
-brain_factory = {
+brain_name_factory_map = {
     "greedy": GreedyBrain,
     "random": lambda: random_brain,
     "keyboard": get_keyboard_brain,
 }
 
 
 def get_brain(brain_args: str):
     brain_key = brain_args.split()[0]
-    if brain_key in brain_factory:
+    if brain_key in brain_name_factory_map:
         string_kwargs = brain_args[len(brain_key) + 1 :]
         kwargs = eval(f"dict({string_kwargs})")
-        return brain_factory[brain_key](**kwargs)
+        return brain_name_factory_map[brain_key](**kwargs)
     else:
         return get_external_brain(brain_args)
```

### Comparing `snaik-0.1.0/snaik/food.py` & `snaik-0.1.1/snaik/food.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         ]
         n_posistions_needed = n_points - len(existing_points)
 
         collision_points = data.get_points()
         collision_points = np.row_stack((collision_points, existing_points)).astype(int)
         collision_points = collision_points[(collision_points >= 0).all(axis=1)]
 
-        board_positions = np.mgrid[0 : grid_size[1], 0 : grid_size[0]].reshape(2, -1).T
+        board_positions = np.mgrid[0 : grid_size[0], 0 : grid_size[1]].reshape(2, -1).T
         del_idxs = np.ravel_multi_index(collision_points.T, dims=grid_size, mode="clip")
         board_positions = np.delete(board_positions, del_idxs, axis=0)
 
         if not len(board_positions):
             # Snake has filled the board, so no new food can be added
             return
         new_points = board_positions[
```

### Comparing `snaik-0.1.0/snaik/game.py` & `snaik-0.1.1/snaik/game.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,22 +79,21 @@
 
         self.snake_manager.set_snakes(brains)
         self.restart()
 
     def tick(self):
         state = self.get_board_state()
         if self._game_over or self.maybe_end_game(state):
+            self.pause()
             return
         for priority in sorted(self._priority_tick_map):
             ticker = self._priority_tick_map[priority]
-            # User code is untrutsed, pass deep copy of
             state = ticker.tick(state)
         return state
 
-    @bind(title="Playback History")
     def playback_history_gui(self):
         states = self.recorder.json_states
 
         def set_tick_number(tick_number: int = len(states) - 1):
             self.set_board_state(states[tick_number])
 
         param = ParameterEditor.defaultInteractor(
@@ -107,15 +106,14 @@
         if states:
             self.set_board_state(states[-1])
 
     def maybe_end_game(self, new_board_state):
         snake_won = any(s.is_winner() for s in self.snake_manager)
         if snake_won or pg_eq(new_board_state, self._last_board_state):
             self._game_over = True
-            self.pause()
             return True
         self._last_board_state = new_board_state
         return False
 
     def register_tick_callback(
         self, callback: TickProtocol, priority: int | None = None
     ):
```

### Comparing `snaik-0.1.0/snaik/leaderboard.py` & `snaik-0.1.1/snaik/leaderboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,22 @@
 
     def refresh(self, board_state: dict = None):
         self.clear()
         all_scores = [snake.get_score() for snake in self.snakes]
         min_score = min(all_scores)
         score_ptp = max(all_scores) - min_score
         base_font_size = 12
+        z_values = sorted([snake.zValue() for snake in self.snakes])
         # Negative id in key means 0 is sorted first
         for snake in reversed(
             sorted(self.snakes, key=lambda s: (s.is_alive(), s.get_score(), -s.id))
         ):
+            # Make sure high-scoring snakes are always on top
+            snake.setZValue(z_values.pop())
+
             if score_ptp > 0:
                 font_size = (
                     base_font_size + (snake.get_score() - min_score) / score_ptp * 7
                 )
             else:
                 font_size = base_font_size
             color = snake.primary_color
```

### Comparing `snaik-0.1.0/snaik/snake.py` & `snaik-0.1.1/snaik/snake.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,17 +271,14 @@
         self._score += increment
 
     def set_status(self, status: Status):
         self._status = status
         opacity = 1.0 if status != Status.DEAD else 0.175
         self.setOpacity(opacity)
 
-    def die(self):
-        self.set_status(Status.DEAD)
-
     def is_alive(self):
         return self._status in [Status.ALIVE, Status.WINNER]
 
     def is_winner(self):
         return self._status == Status.WINNER
 
     def increment_food_indexes(self):
@@ -486,14 +483,16 @@
         for condition, message in self.death_condition_log_map.items():
             dead_ids = condition(board_state["snake_data"])
             if len(dead_ids):
                 logging.getLogger(__name__).info(message.format(ids=dead_ids))
                 all_dead_ids.extend(dead_ids)
         for snake_id in all_dead_ids:
             self[snake_id].set_status(Status.DEAD)
+            board_state["snake_data"][snake_id]["status"] = Status.DEAD
+        return board_state
 
     def check_for_winner(self, board_state: dict):
         data: SnakeData = board_state["snake_data"]
         living = data.get_living_subset()
 
         if len(data) > 1 and len(living) == 1:
             winner = next(iter(living))
@@ -504,15 +503,15 @@
         return board_state
 
     def tick(self, board_state: dict):
         out_state = board_state.copy()
         self.move_snakes(board_state)
         # Update with new snake positions
         out_state["snake_data"] = self.get_snake_data()
-        self.kill_invalid_snakes(out_state)
+        out_state = self.kill_invalid_snakes(out_state)
         out_state = self.check_for_winner(out_state)
         eaten_food_idxs = self.feed_snakes(out_state)
         out_state["food"] = np.delete(board_state["food"], eaten_food_idxs, axis=0)
         return out_state
 
     def restart(self, board_state: dict | None = None):
         if board_state is None:
```

### Comparing `snaik-0.1.0/snaik/staterecorder.py` & `snaik-0.1.1/snaik/staterecorder.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     def __init__(
         self,
         scene_items: QtWidgets.QGraphicsItem | list[QtWidgets.QGraphicsItem],
         json_path: str | Path | None = None,
         frames_path: str | Path | None = None,
         gif_path: str | Path | None = None,
         gif_update_ms: int = 150,
-        include_leaderboard=False,
         initial_board_state: dict | None = None,
     ):
         self.json_path = self.frames_path = self.gif_path = None
         self.gif_writer = DummyWriter()
         self.board_state_hook: t.Callable | None = (
             value_converter_json_hook(initial_board_state)
             if initial_board_state
@@ -47,15 +46,14 @@
         self.json_states = []
         if self.frames_path:
             self.frames_path.mkdir(exist_ok=True)
         self.scene_items = (
             scene_items if isinstance(scene_items, list) else [scene_items]
         )
         self.gif_update_ms = gif_update_ms
-        self.include_leaderboard = include_leaderboard
 
         try:
             import imageio
         except ImportError:
             imageio = None
         self.imageio = imageio
```

### Comparing `snaik-0.1.0/snaik/utils.py` & `snaik-0.1.1/snaik/utils.py`

 * *Files identical despite different names*

### Comparing `snaik-0.1.0/snaik/resources/Roboto-Regular.ttf` & `snaik-0.1.1/snaik/resources/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `snaik-0.1.0/snaik/resources/logo.svg` & `snaik-0.1.1/snaik/resources/logo.svg`

 * *Files identical despite different names*

### Comparing `snaik-0.1.0/pyproject.toml` & `snaik-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,14 @@
   { name = "Nathan Jessurun", email = "ntjessu@gmail.com" },
 ]
 dependencies = [
     "numpy",
     "pyqtgraph     >= 0.13.1",
     "qtextras      >= 0.6.6",
     "qtpy          >= 1.11.0",
-    "click         >= 7.1.2",
     "pyqtdarktheme >= 2.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 full = [
     "PySide6 ~= 6.4.0",
```

