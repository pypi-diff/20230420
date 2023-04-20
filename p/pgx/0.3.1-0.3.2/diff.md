# Comparing `tmp/pgx-0.3.1.tar.gz` & `tmp/pgx-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.3.1.tar", last modified: Mon Apr 17 08:49:23 2023, max compression
+gzip compressed data, was "pgx-0.3.2.tar", last modified: Thu Apr 20 11:48:47 2023, max compression
```

## Comparing `pgx-0.3.1.tar` & `pgx-0.3.2.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.199586 pgx-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 08:49:10.000000 pgx-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 08:49:23.199586 pgx-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-17 08:49:10.000000 pgx-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.187586 pgx-0.3.1/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 11106175 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.191586 pgx-0.3.1/pgx/_dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.191586 pgx-0.3.1/pgx/_dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.191586 pgx-0.3.1/pgx/_dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.195586 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_dwg/tictactoe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.195586 pgx-0.3.1/pgx/_flax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_flax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_flax/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_flax/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.195586 pgx-0.3.1/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27595 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    44105 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28934 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.195586 pgx-0.3.1/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/experimental/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.199586 pgx-0.3.1/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25917 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-17 08:49:10.000000 pgx-0.3.1/pgx/tic_tac_toe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.187586 pgx-0.3.1/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 08:49:23.000000 pgx-0.3.1/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-17 08:49:10.000000 pgx-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:49:23.199586 pgx-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-17 08:49:10.000000 pgx-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:23.199586 pgx-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61258 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-17 08:49:10.000000 pgx-0.3.1/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.836676 pgx-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 11:48:35.000000 pgx-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 11:48:47.836676 pgx-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-20 11:48:35.000000 pgx-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.820675 pgx-0.3.2/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 11106175 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.824675 pgx-0.3.2/pgx/_dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.824675 pgx-0.3.2/pgx/_dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.824675 pgx-0.3.2/pgx/_dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.828676 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/tictactoe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.828676 pgx-0.3.2/pgx/_flax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_flax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_flax/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_flax/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.828676 pgx-0.3.2/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27595 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44184 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28934 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.832676 pgx-0.3.2/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.832676 pgx-0.3.2/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25917 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.820675 pgx-0.3.2/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-20 11:48:35.000000 pgx-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:48:47.836676 pgx-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-20 11:48:35.000000 pgx-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.836676 pgx-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61403 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.3.1/LICENSE` & `pgx-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/README.md` & `pgx-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
 
 <div align="center">
-<img src="fig/logo.svg" width="40%">
+<img src="docs/assets/logo.svg" width="40%">
 </div>
 
 A collection of GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 
 <div align="center">
-<img src="fig/go_dark.gif#gh-dark-mode-only" width="30%"><img src="fig/go_dark.gif#gh-dark-mode-only" width="30%" style="transform:rotate(270deg);"><img src="fig/go_dark.gif#gh-dark-mode-only" width="30%" style="transform:rotate(90deg);">
-<img src="fig/go_light.gif#gh-light-mode-only" width="30%"><img src="fig/go_light.gif#gh-light-mode-only" width="30%" style="transform:rotate(270deg);"><img src="fig/go_light.gif#gh-light-mode-only" width="30%" style="transform:rotate(90deg);">
+<img src="docs/assets/go_dark.gif#gh-dark-mode-only" width="30%"><img src="docs/assets/go_dark.gif#gh-dark-mode-only" width="30%" style="transform:rotate(270deg);"><img src="docs/assets/go_dark.gif#gh-dark-mode-only" width="30%" style="transform:rotate(90deg);">
+<img src="docs/assets/go_light.gif#gh-light-mode-only" width="30%"><img src="docs/assets/go_light.gif#gh-light-mode-only" width="30%" style="transform:rotate(270deg);"><img src="docs/assets/go_light.gif#gh-light-mode-only" width="30%" style="transform:rotate(90deg);">
 </div>
 
 ## Why Pgx?
 
 <!--- 
 throughput: https://colab.research.google.com/drive/1gIWHYLKBxE2XKDhAlEYKVecz3WG4czdz#scrollTo=V1QZhRXoGL8K
 --->
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/badge.svg)]
 (https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
-                                [fig/logo.svg]
+                            [docs/assets/logo.svg]
 A collection of GPU/TPU-accelerated parallel game simulators for reinforcement
 learning (RL)
-  [fig/go_dark.gif#gh-dark-mode-only][fig/go_dark.gif#gh-dark-mode-only][fig/
-   go_dark.gif#gh-dark-mode-only] [fig/go_light.gif#gh-light-mode-only][fig/
-     go_light.gif#gh-light-mode-only][fig/go_light.gif#gh-light-mode-only]
+ [docs/assets/go_dark.gif#gh-dark-mode-only][docs/assets/go_dark.gif#gh-dark-
+      mode-only][docs/assets/go_dark.gif#gh-dark-mode-only] [docs/assets/
+ go_light.gif#gh-light-mode-only][docs/assets/go_light.gif#gh-light-mode-only]
+                 [docs/assets/go_light.gif#gh-light-mode-only]
 ## Why Pgx?  [Brax](https://github.com/google/brax), a [JAX](https://
 github.com/google/jax)-native physics engine, provides extremely high-speed
 parallel simulation for RL in *continuous* state space. Then, what about RL in
 *discrete* state spaces like Chess, Shogi, and Go? **Pgx** provides a wide
 variety of JAX-native game simulators! Highlighted features include: - **JAX-
 native.** All `step` functions are *JIT-able* - **Super fast** in parallel
 execution on accelerators - **Various game support** including **Backgammon**,
```

### Comparing `pgx-0.3.1/pgx/_cache.py` & `pgx-0.3.2/pgx/_cache.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_chess_utils.py` & `pgx-0.3.2/pgx/_chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/animalshogi.py` & `pgx-0.3.2/pgx/_dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/backgammon.py` & `pgx-0.3.2/pgx/_dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/bridge_bidding.py` & `pgx-0.3.2/pgx/_dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/chess.py` & `pgx-0.3.2/pgx/_dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/connect_four.py` & `pgx-0.3.2/pgx/_dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/go.py` & `pgx-0.3.2/pgx/_dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/hex.py` & `pgx-0.3.2/pgx/_dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/LICENSE` & `pgx-0.3.2/pgx/_dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/bBishop.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/bKing.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/bKnight.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/bPawn.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/bQueen.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/bRook.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/wBishop.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/wKing.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/wKnight.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/wPawn.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/wQueen.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/chess/wRook.svg` & `pgx-0.3.2/pgx/_dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/b.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/kuhn_poker.py` & `pgx-0.3.2/pgx/_dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/leduc_holdem.py` & `pgx-0.3.2/pgx/_dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/othello.py` & `pgx-0.3.2/pgx/_dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/play2048.py` & `pgx-0.3.2/pgx/_dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/shogi.py` & `pgx-0.3.2/pgx/_dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/sparrow_mahjong.py` & `pgx-0.3.2/pgx/_dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_dwg/tictactoe.py` & `pgx-0.3.2/pgx/_dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_flax/serialization.py` & `pgx-0.3.2/pgx/_flax/serialization.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,209 +14,194 @@
 
 """Serialization utilities for Jax.
 
 All Flax classes that carry state (e.g. ,Optimizer) can be turned into a
 state dict of numpy arrays for easy serialization.
 """
 import enum
+from typing import Any, Dict, List
 import threading
 from contextlib import contextmanager
-from typing import Any, Dict, List
 
 import jax
 import msgpack  # type: ignore
 import numpy as np
 
+
 _STATE_DICT_REGISTRY: Dict[Any, Any] = {}
 
 
 class _ErrorContext(threading.local):
-    """Context for deserialization error messages."""
-
-    def __init__(self):
-        self.path = []
+  """Context for deserialization error messages."""
 
+  def __init__(self):
+    self.path = []
 
 _error_context = _ErrorContext()
 
 
 @contextmanager
 def _record_path(name):
-    try:
-        _error_context.path.append(name)
-        yield
-    finally:
-        _error_context.path.pop()
+  try:
+    _error_context.path.append(name)
+    yield
+  finally:
+    _error_context.path.pop()
 
 
 def current_path():
-    """Current state_dict path during deserialization for error messages."""
-    return "/".join(_error_context.path)
+  """Current state_dict path during deserialization for error messages."""
+  return '/'.join(_error_context.path)
 
 
 class _NamedTuple:
-    """Fake type marker for namedtuple for registry."""
-
-    pass
+  """Fake type marker for namedtuple for registry."""
+  pass
 
 
 def _is_namedtuple(x):
-    """Duck typing test for namedtuple factory-generated objects."""
-    return isinstance(x, tuple) and hasattr(x, "_fields")
+  """Duck typing test for namedtuple factory-generated objects."""
+  return isinstance(x, tuple) and hasattr(x, '_fields')
 
 
-def from_state_dict(target, state: Dict[str, Any], name: str = "."):
-    """Restores the state of the given target using a state dict.
+def from_state_dict(target, state: Dict[str, Any], name: str = '.'):
+  """Restores the state of the given target using a state dict.
 
-    This function takes the current target as an argument. This
-    lets us know the exact structure of the target,
-    as well as lets us add assertions that shapes and dtypes don't change.
-
-    In practice, none of the leaf values in `target` are actually
-    used. Only the tree structure, shapes and dtypes.
-
-    Args:
-      target: the object of which the state should be restored.
-      state: a dictionary generated by `to_state_dict` with the desired new
-             state for `target`.
-      name: name of branch taken, used to improve deserialization error messages.
-    Returns:
-      A copy of the object with the restored state.
-    """
-    if _is_namedtuple(target):
-        ty = _NamedTuple
-    else:
-        ty = type(target)
-    if ty not in _STATE_DICT_REGISTRY:
-        return state
-    ty_from_state_dict = _STATE_DICT_REGISTRY[ty][1]
-    with _record_path(name):
-        return ty_from_state_dict(target, state)
+  This function takes the current target as an argument. This
+  lets us know the exact structure of the target,
+  as well as lets us add assertions that shapes and dtypes don't change.
+
+  In practice, none of the leaf values in `target` are actually
+  used. Only the tree structure, shapes and dtypes.
+
+  Args:
+    target: the object of which the state should be restored.
+    state: a dictionary generated by `to_state_dict` with the desired new
+           state for `target`.
+    name: name of branch taken, used to improve deserialization error messages.
+  Returns:
+    A copy of the object with the restored state.
+  """
+  if _is_namedtuple(target):
+    ty = _NamedTuple
+  else:
+    ty = type(target)
+  if ty not in _STATE_DICT_REGISTRY:
+    return state
+  ty_from_state_dict = _STATE_DICT_REGISTRY[ty][1]
+  with _record_path(name):
+    return ty_from_state_dict(target, state)
 
 
 def to_state_dict(target) -> Dict[str, Any]:
-    """Returns a dictionary with the state of the given target."""
-    if _is_namedtuple(target):
-        ty = _NamedTuple
-    else:
-        ty = type(target)
-    if ty not in _STATE_DICT_REGISTRY:
-        return target
-
-    ty_to_state_dict = _STATE_DICT_REGISTRY[ty][0]
-    state_dict = ty_to_state_dict(target)
-    assert isinstance(state_dict, dict), "A state dict must be a Python dict."
-    for key in state_dict.keys():
-        assert isinstance(key, str), "A state dict must only have string keys."
-    return state_dict
-
-
-def register_serialization_state(
-    ty, ty_to_state_dict, ty_from_state_dict, override=False
-):
-    """Register a type for serialization.
-
-    Args:
-      ty: the type to be registered
-      ty_to_state_dict: a function that takes an instance of ty and
-        returns its state as a dictionary.
-      ty_from_state_dict: a function that takes an instance of ty and
-        a state dict, and returns a copy of the instance with the restored state.
-      override: override a previously registered serialization handler
-        (default: False).
-    """
-    if ty in _STATE_DICT_REGISTRY and not override:
-        raise ValueError(
-            f'a serialization handler for "{ty.__name__}"'
-            " is already registered"
-        )
-    _STATE_DICT_REGISTRY[ty] = (ty_to_state_dict, ty_from_state_dict)
+  """Returns a dictionary with the state of the given target."""
+  if _is_namedtuple(target):
+    ty = _NamedTuple
+  else:
+    ty = type(target)
+  if ty not in _STATE_DICT_REGISTRY:
+    return target
+
+  ty_to_state_dict = _STATE_DICT_REGISTRY[ty][0]
+  state_dict = ty_to_state_dict(target)
+  assert isinstance(state_dict, dict), 'A state dict must be a Python dict.'
+  for key in state_dict.keys():
+    assert isinstance(key, str), 'A state dict must only have string keys.'
+  return state_dict
+
+
+def register_serialization_state(ty, ty_to_state_dict, ty_from_state_dict,
+                                 override=False):
+  """Register a type for serialization.
+
+  Args:
+    ty: the type to be registered
+    ty_to_state_dict: a function that takes an instance of ty and
+      returns its state as a dictionary.
+    ty_from_state_dict: a function that takes an instance of ty and
+      a state dict, and returns a copy of the instance with the restored state.
+    override: override a previously registered serialization handler
+      (default: False).
+  """
+  if ty in _STATE_DICT_REGISTRY and not override:
+    raise ValueError(f'a serialization handler for "{ty.__name__}"'
+                     ' is already registered')
+  _STATE_DICT_REGISTRY[ty] = (ty_to_state_dict, ty_from_state_dict)
 
 
 def _list_state_dict(xs: List[Any]) -> Dict[str, Any]:
-    return {str(i): to_state_dict(x) for i, x in enumerate(xs)}
+  return {str(i): to_state_dict(x) for i, x in enumerate(xs)}
 
 
 def _restore_list(xs, state_dict: Dict[str, Any]) -> List[Any]:
-    if len(state_dict) != len(xs):
-        raise ValueError(
-            "The size of the list and the state dict do not match,"
-            f" got {len(xs)} and {len(state_dict)} "
-            f"at path {current_path()}"
-        )
-    ys = []
-    for i in range(len(state_dict)):
-        y = from_state_dict(xs[i], state_dict[str(i)], name=str(i))
-        ys.append(y)
-    return ys
+  if len(state_dict) != len(xs):
+    raise ValueError('The size of the list and the state dict do not match,'
+                     f' got {len(xs)} and {len(state_dict)} '
+                     f'at path {current_path()}')
+  ys = []
+  for i in range(len(state_dict)):
+    y = from_state_dict(xs[i], state_dict[str(i)], name=str(i))
+    ys.append(y)
+  return ys
 
 
 def _dict_state_dict(xs: Dict[str, Any]) -> Dict[str, Any]:
-    str_keys = set(str(k) for k in xs.keys())
-    if len(str_keys) != len(xs):
-        raise ValueError(
-            "Dict keys do not have a unique string representation: "
-            f"{str_keys} vs given: {xs}"
-        )
-    return {str(key): to_state_dict(value) for key, value in xs.items()}
+  str_keys = set(str(k) for k in xs.keys())
+  if len(str_keys) != len(xs):
+    raise ValueError(
+        'Dict keys do not have a unique string representation: '
+        f'{str_keys} vs given: {xs}'
+    )
+  return {str(key): to_state_dict(value) for key, value in xs.items()}
 
 
 def _restore_dict(xs, states: Dict[str, Any]) -> Dict[str, Any]:
-    diff = set(map(str, xs.keys())).difference(states.keys())
-    if diff:
-        raise ValueError(
-            "The target dict keys and state dict keys do not match,"
-            f" target dict contains keys {diff} which are not present in state dict "
-            f"at path {current_path()}"
-        )
-
-    return {
-        key: from_state_dict(value, states[str(key)], name=str(key))
-        for key, value in xs.items()
-    }
+  diff = set(map(str, xs.keys())).difference(states.keys())
+  if diff:
+    raise ValueError('The target dict keys and state dict keys do not match,'
+                   f' target dict contains keys {diff} which are not present in state dict '
+                   f'at path {current_path()}')
+
+  return {key: from_state_dict(value, states[str(key)], name=str(key))
+          for key, value in xs.items()}
 
 
 def _namedtuple_state_dict(nt) -> Dict[str, Any]:
-    return {key: to_state_dict(getattr(nt, key)) for key in nt._fields}
+  return {key: to_state_dict(getattr(nt, key)) for key in nt._fields}
 
 
 def _restore_namedtuple(xs, state_dict: Dict[str, Any]):
-    """Rebuild namedtuple from serialized dict."""
-    if set(state_dict.keys()) == {"name", "fields", "values"}:
-        # TODO(jheek): remove backward compatible named tuple restoration early 2022
-        state_dict = {
-            state_dict["fields"][str(i)]: state_dict["values"][str(i)]
-            for i in range(len(state_dict["fields"]))
-        }
-
-    sd_keys = set(state_dict.keys())
-    nt_keys = set(xs._fields)
-
-    if sd_keys != nt_keys:
-        raise ValueError(
-            "The field names of the state dict and the named tuple do not match,"
-            f" got {sd_keys} and {nt_keys} at path {current_path()}"
-        )
-    fields = {
-        k: from_state_dict(getattr(xs, k), v, name=k)
-        for k, v in state_dict.items()
-    }
-    return type(xs)(**fields)
+  """Rebuild namedtuple from serialized dict."""
+  if set(state_dict.keys()) == {'name', 'fields', 'values'}:
+    # TODO(jheek): remove backward compatible named tuple restoration early 2022
+    state_dict = {state_dict['fields'][str(i)]: state_dict['values'][str(i)]
+                  for i in range(len(state_dict['fields']))}
+
+  sd_keys = set(state_dict.keys())
+  nt_keys = set(xs._fields)
+
+  if sd_keys != nt_keys:
+    raise ValueError(
+        'The field names of the state dict and the named tuple do not match,'
+        f' got {sd_keys} and {nt_keys} at path {current_path()}')
+  fields = {
+      k: from_state_dict(getattr(xs, k), v, name=k)
+      for k, v in state_dict.items()
+  }
+  return type(xs)(**fields)
 
 
 register_serialization_state(dict, _dict_state_dict, _restore_dict)
 register_serialization_state(list, _list_state_dict, _restore_list)
 register_serialization_state(
-    tuple,
-    _list_state_dict,
-    lambda xs, state_dict: tuple(_restore_list(list(xs), state_dict)),
-)
-register_serialization_state(
-    _NamedTuple, _namedtuple_state_dict, _restore_namedtuple
-)
+    tuple, _list_state_dict,
+    lambda xs, state_dict: tuple(_restore_list(list(xs), state_dict)))
+register_serialization_state(_NamedTuple,
+                             _namedtuple_state_dict,
+                             _restore_namedtuple)
 
 register_serialization_state(
     jax.tree_util.Partial,
     lambda x: (
         {
             "args": to_state_dict(x.args),
             "keywords": to_state_dict(x.keywords),
@@ -239,226 +224,217 @@
 #   Note: only simple ndarray types are supported, no objects or fields.
 #
 # - native complex scalars are converted to nested msgpack-encoded tuples
 #   (real, imag).
 
 
 def _ndarray_to_bytes(arr) -> bytes:
-    """Save ndarray to simple msgpack encoding."""
-    if isinstance(arr, jax.Array):
-        arr = np.array(arr)
-    if arr.dtype.hasobject or arr.dtype.isalignedstruct:
-        raise ValueError(
-            "Object and structured dtypes not supported "
-            "for serialization of ndarrays."
-        )
-    tpl = (arr.shape, arr.dtype.name, arr.tobytes("C"))
-    return msgpack.packb(tpl, use_bin_type=True)
+  """Save ndarray to simple msgpack encoding."""
+  if isinstance(arr, jax.Array):
+    arr = np.array(arr)
+  if arr.dtype.hasobject or arr.dtype.isalignedstruct:
+    raise ValueError('Object and structured dtypes not supported '
+                     'for serialization of ndarrays.')
+  tpl = (arr.shape, arr.dtype.name, arr.tobytes('C'))
+  return msgpack.packb(tpl, use_bin_type=True)
 
 
 def _dtype_from_name(name: str):
-    """Handle JAX bfloat16 dtype correctly."""
-    if name == b"bfloat16":
-        return jax.numpy.bfloat16
-    else:
-        return np.dtype(name)
+  """Handle JAX bfloat16 dtype correctly."""
+  if name == b'bfloat16':
+    return jax.numpy.bfloat16
+  else:
+    return np.dtype(name)
 
 
 def _ndarray_from_bytes(data: bytes) -> np.ndarray:
-    """Load ndarray from simple msgpack encoding."""
-    shape, dtype_name, buffer = msgpack.unpackb(data, raw=True)
-    return np.frombuffer(
-        buffer, dtype=_dtype_from_name(dtype_name), count=-1, offset=0
-    ).reshape(shape, order="C")
+  """Load ndarray from simple msgpack encoding."""
+  shape, dtype_name, buffer = msgpack.unpackb(data, raw=True)
+  return np.frombuffer(buffer,
+                       dtype=_dtype_from_name(dtype_name),
+                       count=-1,
+                       offset=0).reshape(shape, order='C')
 
 
 class _MsgpackExtType(enum.IntEnum):
-    """Messagepack custom type ids."""
-
-    ndarray = 1
-    native_complex = 2
-    npscalar = 3
+  """Messagepack custom type ids."""
+  ndarray = 1
+  native_complex = 2
+  npscalar = 3
 
 
 def _msgpack_ext_pack(x):
-    """Messagepack encoders for custom types."""
-    # TODO(_flax-dev): Array here only work when they are fully addressable.
-    # If they are not fully addressable, use the GDA path for checkpointing.
-    if isinstance(x, (np.ndarray, jax.Array)):
-        return msgpack.ExtType(_MsgpackExtType.ndarray, _ndarray_to_bytes(x))
-    if np.issctype(type(x)):
-        # pack scalar as ndarray
-        return msgpack.ExtType(
-            _MsgpackExtType.npscalar, _ndarray_to_bytes(np.asarray(x))
-        )
-    elif isinstance(x, complex):
-        return msgpack.ExtType(
-            _MsgpackExtType.native_complex, msgpack.packb((x.real, x.imag))
-        )
-    return x
+  """Messagepack encoders for custom types."""
+  # TODO(flax-dev): Array here only work when they are fully addressable.
+  # If they are not fully addressable, use the GDA path for checkpointing.
+  if isinstance(x, (np.ndarray, jax.Array)):
+    return msgpack.ExtType(_MsgpackExtType.ndarray, _ndarray_to_bytes(x))
+  if np.issctype(type(x)):
+    # pack scalar as ndarray
+    return msgpack.ExtType(_MsgpackExtType.npscalar,
+                           _ndarray_to_bytes(np.asarray(x)))
+  elif isinstance(x, complex):
+    return msgpack.ExtType(_MsgpackExtType.native_complex,
+                           msgpack.packb((x.real, x.imag)))
+  return x
 
 
 def _msgpack_ext_unpack(code, data):
-    """Messagepack decoders for custom types."""
-    if code == _MsgpackExtType.ndarray:
-        return _ndarray_from_bytes(data)
-    elif code == _MsgpackExtType.native_complex:
-        complex_tuple = msgpack.unpackb(data)
-        return complex(complex_tuple[0], complex_tuple[1])
-    elif code == _MsgpackExtType.npscalar:
-        ar = _ndarray_from_bytes(data)
-        return ar[()]  # unpack ndarray to scalar
-    return msgpack.ExtType(code, data)
+  """Messagepack decoders for custom types."""
+  if code == _MsgpackExtType.ndarray:
+    return _ndarray_from_bytes(data)
+  elif code == _MsgpackExtType.native_complex:
+    complex_tuple = msgpack.unpackb(data)
+    return complex(complex_tuple[0], complex_tuple[1])
+  elif code == _MsgpackExtType.npscalar:
+    ar = _ndarray_from_bytes(data)
+    return ar[()]  # unpack ndarray to scalar
+  return msgpack.ExtType(code, data)
 
 
 # Chunking array leaves
 
 # msgpack has a hard limit of 2**31 - 1 bytes per object leaf.  To circumvent
 # this limit for giant arrays (e.g. embedding tables), we traverse the tree
 # and break up arrays near the limit into flattened array chunks.
 
 # True limit is 2**31 - 1, but leave a margin for encoding padding.
 MAX_CHUNK_SIZE = 2**30
 
 
 def _np_convert_in_place(d):
-    """Convert any jax devicearray leaves to numpy arrays in place."""
-    if isinstance(d, dict):
-        for k, v in d.items():
-            if isinstance(v, jax.Array):
-                d[k] = np.array(v)
-            elif isinstance(v, dict):
-                _np_convert_in_place(v)
-    elif isinstance(d, jax.Array):
-        return np.array(d)
-    return d
+  """Convert any jax devicearray leaves to numpy arrays in place."""
+  if isinstance(d, dict):
+    for k, v in d.items():
+      if isinstance(v, jax.Array):
+        d[k] = np.array(v)
+      elif isinstance(v, dict):
+        _np_convert_in_place(v)
+  elif isinstance(d, jax.Array):
+    return np.array(d)
+  return d
 
 
 _tuple_to_dict = lambda tpl: {str(x): y for x, y in enumerate(tpl)}
 _dict_to_tuple = lambda dct: tuple(dct[str(i)] for i in range(len(dct)))
 
 
 def _chunk(arr) -> Dict[str, Any]:
-    """Convert array to a canonical dictionary of chunked arrays."""
-    chunksize = max(1, int(MAX_CHUNK_SIZE / arr.dtype.itemsize))
-    data = {
-        "__msgpack_chunked_array__": True,
-        "shape": _tuple_to_dict(arr.shape),
-    }
-    flatarr = arr.reshape(-1)
-    chunks = [
-        flatarr[i : i + chunksize] for i in range(0, flatarr.size, chunksize)
-    ]
-    data["chunks"] = _tuple_to_dict(chunks)
-    return data
+  """Convert array to a canonical dictionary of chunked arrays."""
+  chunksize = max(1, int(MAX_CHUNK_SIZE / arr.dtype.itemsize))
+  data = {'__msgpack_chunked_array__': True,
+          'shape': _tuple_to_dict(arr.shape)}
+  flatarr = arr.reshape(-1)
+  chunks = [flatarr[i:i + chunksize] for i in range(0, flatarr.size, chunksize)]
+  data['chunks'] = _tuple_to_dict(chunks)
+  return data
 
 
 def _unchunk(data: Dict[str, Any]):
-    """Convert canonical dictionary of chunked arrays back into array."""
-    assert "__msgpack_chunked_array__" in data
-    shape = _dict_to_tuple(data["shape"])
-    flatarr = np.concatenate(_dict_to_tuple(data["chunks"]))
-    return flatarr.reshape(shape)
+  """Convert canonical dictionary of chunked arrays back into array."""
+  assert '__msgpack_chunked_array__' in data
+  shape = _dict_to_tuple(data['shape'])
+  flatarr = np.concatenate(_dict_to_tuple(data['chunks']))
+  return flatarr.reshape(shape)
 
 
 def _chunk_array_leaves_in_place(d):
-    """Convert oversized array leaves to safe chunked form in place."""
-    if isinstance(d, dict):
-        for k, v in d.items():
-            if isinstance(v, np.ndarray):
-                if v.size * v.dtype.itemsize > MAX_CHUNK_SIZE:
-                    d[k] = _chunk(v)
-            elif isinstance(v, dict):
-                _chunk_array_leaves_in_place(v)
-    elif isinstance(d, np.ndarray):
-        if d.size * d.dtype.itemsize > MAX_CHUNK_SIZE:
-            return _chunk(d)
-    return d
+  """Convert oversized array leaves to safe chunked form in place."""
+  if isinstance(d, dict):
+    for k, v in d.items():
+      if isinstance(v, np.ndarray):
+        if v.size * v.dtype.itemsize > MAX_CHUNK_SIZE:
+          d[k] = _chunk(v)
+      elif isinstance(v, dict):
+        _chunk_array_leaves_in_place(v)
+  elif isinstance(d, np.ndarray):
+    if d.size * d.dtype.itemsize > MAX_CHUNK_SIZE:
+      return _chunk(d)
+  return d
 
 
 def _unchunk_array_leaves_in_place(d):
-    """Convert chunked array leaves back into array leaves, in place."""
-    if isinstance(d, dict):
-        if "__msgpack_chunked_array__" in d:
-            return _unchunk(d)
-        else:
-            for k, v in d.items():
-                if isinstance(v, dict) and "__msgpack_chunked_array__" in v:
-                    d[k] = _unchunk(v)
-                elif isinstance(v, dict):
-                    _unchunk_array_leaves_in_place(v)
-    return d
+  """Convert chunked array leaves back into array leaves, in place."""
+  if isinstance(d, dict):
+    if '__msgpack_chunked_array__' in d:
+      return _unchunk(d)
+    else:
+      for k, v in d.items():
+        if isinstance(v, dict) and '__msgpack_chunked_array__' in v:
+          d[k] = _unchunk(v)
+        elif isinstance(v, dict):
+          _unchunk_array_leaves_in_place(v)
+  return d
 
 
 # User-facing API calls:
 
 
 def msgpack_serialize(pytree, in_place: bool = False) -> bytes:
-    """Save data structure to bytes in msgpack format.
+  """Save data structure to bytes in msgpack format.
 
-    Low-level function that only supports python trees with array leaves,
-    for custom objects use `to_bytes`.  It splits arrays above MAX_CHUNK_SIZE into
-    multiple chunks.
-
-    Args:
-      pytree: python tree of dict, list, tuple with python primitives
-        and array leaves.
-      in_place: boolean specifyng if pytree should be modified in place.
-
-    Returns:
-      msgpack-encoded bytes of pytree.
-    """
-    if not in_place:
-        pytree = jax.tree_util.tree_map(lambda x: x, pytree)
-    pytree = _np_convert_in_place(pytree)
-    pytree = _chunk_array_leaves_in_place(pytree)
-    return msgpack.packb(pytree, default=_msgpack_ext_pack, strict_types=True)
+  Low-level function that only supports python trees with array leaves,
+  for custom objects use `to_bytes`.  It splits arrays above MAX_CHUNK_SIZE into
+  multiple chunks.
+
+  Args:
+    pytree: python tree of dict, list, tuple with python primitives
+      and array leaves.
+    in_place: boolean specifyng if pytree should be modified in place.
+
+  Returns:
+    msgpack-encoded bytes of pytree.
+  """
+  if not in_place:
+    pytree = jax.tree_util.tree_map(lambda x: x, pytree)
+  pytree = _np_convert_in_place(pytree)
+  pytree = _chunk_array_leaves_in_place(pytree)
+  return msgpack.packb(pytree, default=_msgpack_ext_pack, strict_types=True)
 
 
 def msgpack_restore(encoded_pytree: bytes):
-    """Restore data structure from bytes in msgpack format.
+  """Restore data structure from bytes in msgpack format.
 
-    Low-level function that only supports python trees with array leaves,
-    for custom objects use `from_bytes`.
+  Low-level function that only supports python trees with array leaves,
+  for custom objects use `from_bytes`.
 
-    Args:
-      encoded_pytree: msgpack-encoded bytes of python tree.
+  Args:
+    encoded_pytree: msgpack-encoded bytes of python tree.
 
-    Returns:
-      Python tree of dict, list, tuple with python primitive
-      and array leaves.
-    """
-    state_dict = msgpack.unpackb(
-        encoded_pytree, ext_hook=_msgpack_ext_unpack, raw=False
-    )
-    return _unchunk_array_leaves_in_place(state_dict)
+  Returns:
+    Python tree of dict, list, tuple with python primitive
+    and array leaves.
+  """
+  state_dict = msgpack.unpackb(
+      encoded_pytree, ext_hook=_msgpack_ext_unpack, raw=False)
+  return _unchunk_array_leaves_in_place(state_dict)
 
 
 def from_bytes(target, encoded_bytes: bytes):
-    """Restore optimizer or other object from msgpack-serialized state-dict.
+  """Restore optimizer or other object from msgpack-serialized state-dict.
 
-    Args:
-      target: template object with state-dict registrations that matches
-        the structure being deserialized from `encoded_bytes`.
-      encoded_bytes: msgpack serialized object structurally isomorphic to
-        `target`.  Typically a _flax model or optimizer.
-
-    Returns:
-      A new object structurally isomorphic to `target` containing the updated
-      leaf data from saved data.
-    """
-    state_dict = msgpack_restore(encoded_bytes)
-    return from_state_dict(target, state_dict)
+  Args:
+    target: template object with state-dict registrations that matches
+      the structure being deserialized from `encoded_bytes`.
+    encoded_bytes: msgpack serialized object structurally isomorphic to
+      `target`.  Typically a flax model or optimizer.
+
+  Returns:
+    A new object structurally isomorphic to `target` containing the updated
+    leaf data from saved data.
+  """
+  state_dict = msgpack_restore(encoded_bytes)
+  return from_state_dict(target, state_dict)
 
 
 def to_bytes(target) -> bytes:
-    """Save optimizer or other object as msgpack-serialized state-dict.
+  """Save optimizer or other object as msgpack-serialized state-dict.
 
-    Args:
-      target: template object with state-dict registrations to be
-        serialized to msgpack format.  Typically a _flax model or optimizer.
-
-    Returns:
-      Bytes of msgpack-encoded state-dict of `target` object.
-    """
-    state_dict = to_state_dict(target)
-    return msgpack_serialize(state_dict, in_place=True)
+  Args:
+    target: template object with state-dict registrations to be
+      serialized to msgpack format.  Typically a flax model or optimizer.
+
+  Returns:
+    Bytes of msgpack-encoded state-dict of `target` object.
+  """
+  state_dict = to_state_dict(target)
+  return msgpack_serialize(state_dict, in_place=True)
```

### Comparing `pgx-0.3.1/pgx/_flax/struct.py` & `pgx-0.3.2/pgx/_flax/struct.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The Flax Authors.
+# Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,221 +12,214 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utilities for defining custom classes that can be used with jax transformations.
 """
 
 import dataclasses
-import typing
-from typing import Any, Callable, Tuple, TypeVar, Union
+from typing import TypeVar, Callable, Tuple, Union, Any
+
+from . import serialization
 
 import jax
-from typing_extensions import (  # pytype: disable=not-supported-yet
-    dataclass_transform,
-)
+from typing_extensions import dataclass_transform  # pytype: disable=not-supported-yet
 
-from . import serialization
 
 _T = TypeVar("_T")
 
 
 def field(pytree_node=True, **kwargs):
-    return dataclasses.field(metadata={"pytree_node": pytree_node}, **kwargs)
+  return dataclasses.field(metadata={'pytree_node': pytree_node}, **kwargs)
 
 
-@dataclass_transform(field_descriptors=(field,))
+@dataclass_transform(field_descriptors=(field,)) # type: ignore[literal-required]
 def dataclass(clz: _T) -> _T:
-    """Create a class which can be passed to functional transformations.
-
-    NOTE: Inherit from ``PyTreeNode`` instead to avoid type checking issues when
-    using PyType.
+  """Create a class which can be passed to functional transformations.
 
-    Jax transformations such as `jax.jit` and `jax.grad` require objects that are
-    immutable and can be mapped over using the `jax.tree_util` methods.
-    The `dataclass` decorator makes it easy to define custom classes that can be
-    passed safely to Jax. For example::
-
-      from _flax import struct
-
-      @struct.dataclass
-      class Model:
-        params: Any
-        # use pytree_node=False to indicate an attribute should not be touched
-        # by Jax transformations.
-        apply_fn: FunctionType = struct.field(pytree_node=False)
-
-        def __apply__(self, *args):
-          return self.apply_fn(*args)
-
-      model = Model(params, apply_fn)
-
-      model.params = params_b  # Model is immutable. This will raise an error.
-      model_b = model.replace(params=params_b)  # Use the replace method instead.
-
-      # This class can now be used safely in Jax to compute gradients w.r.t. the
-      # parameters.
-      model = Model(params, apply_fn)
-      model_grad = jax.grad(some_loss_fn)(model)
-
-    Note that dataclasses have an auto-generated ``__init__`` where
-    the arguments of the constructor and the attributes of the created
-    instance match 1:1. This correspondence is what makes these objects
-    valid containers that work with JAX transformations and
-    more generally the `jax.tree_util` library.
-
-    Sometimes a "smart constructor" is desired, for example because
-    some of the attributes can be (optionally) derived from others.
-    The way to do this with Flax dataclasses is to make a static or
-    class method that provides the smart constructor.
-    This way the simple constructor used by `jax.tree_util` is
-    preserved. Consider the following example::
-
-      @struct.dataclass
-      class DirectionAndScaleKernel:
-        direction: Array
-        scale: Array
-
-        @classmethod
-        def create(cls, kernel):
-          scale = jax.numpy.linalg.norm(kernel, axis=0, keepdims=True)
-          directin = direction / scale
-          return cls(direction, scale)
-
-    Args:
-      clz: the class that will be transformed by the decorator.
-    Returns:
-      The new class.
-    """
-    # check if already a _flax dataclass
-    if "_flax_dataclass" in clz.__dict__:
-        return clz
-
-    data_clz = dataclasses.dataclass(frozen=True)(clz)  # type: ignore
-    meta_fields = []
-    data_fields = []
-    for field_info in dataclasses.fields(data_clz):
-        is_pytree_node = field_info.metadata.get("pytree_node", True)
-        if is_pytree_node:
-            data_fields.append(field_info.name)
-        else:
-            meta_fields.append(field_info.name)
-
-    def replace(self, **updates):
-        """ "Returns a new object replacing the specified fields with new values."""
-        return dataclasses.replace(self, **updates)
-
-    data_clz.replace = replace
-
-    def iterate_clz(x):
-        meta = tuple(getattr(x, name) for name in meta_fields)
-        data = tuple(getattr(x, name) for name in data_fields)
-        return data, meta
-
-    def clz_from_iterable(meta, data):
-        meta_args = tuple(zip(meta_fields, meta))
-        data_args = tuple(zip(data_fields, data))
-        kwargs = dict(meta_args + data_args)
-        return data_clz(**kwargs)
+  NOTE: Inherit from ``PyTreeNode`` instead to avoid type checking issues when
+  using PyType.
 
-    jax.tree_util.register_pytree_node(
-        data_clz, iterate_clz, clz_from_iterable
+  Jax transformations such as `jax.jit` and `jax.grad` require objects that are
+  immutable and can be mapped over using the `jax.tree_util` methods.
+  The `dataclass` decorator makes it easy to define custom classes that can be
+  passed safely to Jax. For example::
+
+    from flax import struct
+
+    @struct.dataclass
+    class Model:
+      params: Any
+      # use pytree_node=False to indicate an attribute should not be touched
+      # by Jax transformations.
+      apply_fn: FunctionType = struct.field(pytree_node=False)
+
+      def __apply__(self, *args):
+        return self.apply_fn(*args)
+
+    model = Model(params, apply_fn)
+
+    model.params = params_b  # Model is immutable. This will raise an error.
+    model_b = model.replace(params=params_b)  # Use the replace method instead.
+
+    # This class can now be used safely in Jax to compute gradients w.r.t. the
+    # parameters.
+    model = Model(params, apply_fn)
+    model_grad = jax.grad(some_loss_fn)(model)
+
+  Note that dataclasses have an auto-generated ``__init__`` where
+  the arguments of the constructor and the attributes of the created
+  instance match 1:1. This correspondence is what makes these objects
+  valid containers that work with JAX transformations and
+  more generally the `jax.tree_util` library.
+
+  Sometimes a "smart constructor" is desired, for example because
+  some of the attributes can be (optionally) derived from others.
+  The way to do this with Flax dataclasses is to make a static or
+  class method that provides the smart constructor.
+  This way the simple constructor used by `jax.tree_util` is
+  preserved. Consider the following example::
+
+    @struct.dataclass
+    class DirectionAndScaleKernel:
+      direction: Array
+      scale: Array
+
+      @classmethod
+      def create(cls, kernel):
+        scale = jax.numpy.linalg.norm(kernel, axis=0, keepdims=True)
+        directin = direction / scale
+        return cls(direction, scale)
+
+  Args:
+    clz: the class that will be transformed by the decorator.
+  Returns:
+    The new class.
+  """
+  # check if already a flax dataclass
+  if '_flax_dataclass' in clz.__dict__:
+    return clz
+
+  data_clz = dataclasses.dataclass(frozen=True)(clz) # type: ignore
+  meta_fields = []
+  data_fields = []
+  for field_info in dataclasses.fields(data_clz):
+    is_pytree_node = field_info.metadata.get('pytree_node', True)
+    if is_pytree_node:
+      data_fields.append(field_info.name)
+    else:
+      meta_fields.append(field_info.name)
+
+  def replace(self, **updates):
+    """"Returns a new object replacing the specified fields with new values."""
+    return dataclasses.replace(self, **updates)
+
+  data_clz.replace = replace
+
+  def iterate_clz(x):
+    meta = tuple(getattr(x, name) for name in meta_fields)
+    data = tuple(getattr(x, name) for name in data_fields)
+    return data, meta
+
+  def iterate_clz_with_keys(x):
+    meta = tuple(getattr(x, name) for name in meta_fields)
+    data = tuple(
+        (jax.tree_util.GetAttrKey(name), getattr(x, name))
+        for name in data_fields
     )
+    return data, meta
 
-    if tuple(map(int, jax.version.__version__.split("."))) >= (0, 3, 1):
-
-        def keypaths(_):
-            return [
-                jax.tree_util.AttributeKeyPathEntry(name)
-                for name in data_fields
-            ]
-
-        jax.tree_util.register_keypaths(data_clz, keypaths)
-
-    def to_state_dict(x):
-        state_dict = {
-            name: serialization.to_state_dict(getattr(x, name))
-            for name in data_fields
-        }
-        return state_dict
-
-    def from_state_dict(x, state):
-        """Restore the state of a data class."""
-        state = (
-            state.copy()
-        )  # copy the state so we can pop the restored fields.
-        updates = {}
-        for name in data_fields:
-            if name not in state:
-                raise ValueError(
-                    f"Missing field {name} in state dict while restoring"
-                    f" an instance of {clz.__name__},"
-                    f" at path {serialization.current_path()}"
-                )
-            value = getattr(x, name)
-            value_state = state.pop(name)
-            updates[name] = serialization.from_state_dict(
-                value, value_state, name=name
-            )
-        if state:
-            names = ",".join(state.keys())
-            raise ValueError(
-                f'Unknown field(s) "{names}" in state dict while'
-                f" restoring an instance of {clz.__name__}"
-                f" at path {serialization.current_path()}"
-            )
-        return x.replace(**updates)
-
-    serialization.register_serialization_state(
-        data_clz, to_state_dict, from_state_dict
+  def clz_from_iterable(meta, data):
+    meta_args = tuple(zip(meta_fields, meta))
+    data_args = tuple(zip(data_fields, data))
+    kwargs = dict(meta_args + data_args)
+    return data_clz(**kwargs)
+
+  if hasattr(jax.tree_util, 'register_pytree_with_keys'):
+    jax.tree_util.register_pytree_with_keys(
+        data_clz, iterate_clz_with_keys, clz_from_iterable
     )
+  else:
+    jax.tree_util.register_pytree_node(data_clz, iterate_clz, clz_from_iterable)
+    def keypaths(_):
+      return [
+          jax.tree_util.AttributeKeyPathEntry(name) for name in data_fields
+      ]
+    jax.tree_util.register_keypaths(data_clz, keypaths)
+
+  def to_state_dict(x):
+    state_dict = {name: serialization.to_state_dict(getattr(x, name))
+                  for name in data_fields}
+    return state_dict
+
+  def from_state_dict(x, state):
+    """Restore the state of a data class."""
+    state = state.copy()  # copy the state so we can pop the restored fields.
+    updates = {}
+    for name in data_fields:
+      if name not in state:
+        raise ValueError(f'Missing field {name} in state dict while restoring'
+                         f' an instance of {clz.__name__},'
+                         f' at path {serialization.current_path()}')
+      value = getattr(x, name)
+      value_state = state.pop(name)
+      updates[name] = serialization.from_state_dict(value, value_state, name=name)
+    if state:
+      names = ','.join(state.keys())
+      raise ValueError(f'Unknown field(s) "{names}" in state dict while'
+                       f' restoring an instance of {clz.__name__}'
+                       f' at path {serialization.current_path()}')
+    return x.replace(**updates)
+
+  serialization.register_serialization_state(
+      data_clz, to_state_dict, from_state_dict)
+
+  # add a _flax_dataclass flag to distinguish from regular dataclasses
+  data_clz._flax_dataclass = True # type: ignore[attr-defined]
 
-    # add a _flax_dataclass flag to distinguish from regular dataclasses
-    data_clz._flax_dataclass = True  # type: ignore[attr-defined]
-
-    return data_clz  # type: ignore
+  return data_clz # type: ignore
 
 
-TNode = TypeVar("TNode", bound="PyTreeNode")
+TNode = TypeVar('TNode', bound='PyTreeNode')
 
 
-@dataclass_transform(field_descriptors=(field,))
+@dataclass_transform(field_descriptors=(field,)) # type: ignore[literal-required]
 class PyTreeNode:
-    """Base class for dataclasses that should act like a JAX pytree node.
+  """Base class for dataclasses that should act like a JAX pytree node.
 
-    See ``_flax.struct.dataclass`` for the ``jax.tree_util`` behavior.
-    This base class additionally avoids type checking errors when using PyType.
+  See ``flax.struct.dataclass`` for the ``jax.tree_util`` behavior.
+  This base class additionally avoids type checking errors when using PyType.
 
-    Example::
+  Example::
 
-      from _flax import struct
+    from flax import struct
 
-      class Model(struct.PyTreeNode):
-        params: Any
-        # use pytree_node=False to indicate an attribute should not be touched
-        # by Jax transformations.
-        apply_fn: FunctionType = struct.field(pytree_node=False)
+    class Model(struct.PyTreeNode):
+      params: Any
+      # use pytree_node=False to indicate an attribute should not be touched
+      # by Jax transformations.
+      apply_fn: FunctionType = struct.field(pytree_node=False)
 
-        def __apply__(self, *args):
-          return self.apply_fn(*args)
+      def __apply__(self, *args):
+        return self.apply_fn(*args)
 
-      model = Model(params, apply_fn)
+    model = Model(params, apply_fn)
 
-      model.params = params_b  # Model is immutable. This will raise an error.
-      model_b = model.replace(params=params_b)  # Use the replace method instead.
+    model.params = params_b  # Model is immutable. This will raise an error.
+    model_b = model.replace(params=params_b)  # Use the replace method instead.
 
-      # This class can now be used safely in Jax to compute gradients w.r.t. the
-      # parameters.
-      model = Model(params, apply_fn)
-      model_grad = jax.grad(some_loss_fn)(model)
+    # This class can now be used safely in Jax to compute gradients w.r.t. the
+    # parameters.
+    model = Model(params, apply_fn)
+    model_grad = jax.grad(some_loss_fn)(model)
 
-    """
+  """
 
-    def __init_subclass__(cls):
-        dataclass(cls)  # pytype: disable=wrong-arg-types
+  def __init_subclass__(cls):
+    dataclass(cls)  # pytype: disable=wrong-arg-types
 
-    def __init__(self, *args, **kwargs):
-        # stub for pytype
-        raise NotImplementedError
+  def __init__(self, *args, **kwargs):
+    # stub for pytype
+    raise NotImplementedError
 
-    def replace(self: TNode, **overrides) -> TNode:
-        # stub for pytype
-        raise NotImplementedError
+  def replace(self: TNode, **overrides) -> TNode:
+    # stub for pytype
+    raise NotImplementedError
```

### Comparing `pgx-0.3.1/pgx/_mahjong/_hand.py` & `pgx-0.3.2/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_shogi_utils.py` & `pgx-0.3.2/pgx/_shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/_test.py` & `pgx-0.3.2/pgx/_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     prev_state = state
     if not state.terminated:
         return
     action = 0
     state = step_fn(state, action)
     assert (state.reward == 0).all()
     for field in fields(state):
-        if field.name in ["reward", "steps"]:
+        if field.name in ["reward", "steps", "_info"]:
             continue
         assert (
             getattr(state, field.name) == getattr(prev_state, field.name)
         ).all(), f"{field.name} : \n{getattr(state, field.name)}\n{getattr(prev_state, field.name)}"
 
 
 def _validate_init_reward(state: State):
```

### Comparing `pgx-0.3.1/pgx/_visualizer.py` & `pgx-0.3.2/pgx/_visualizer.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/animal_shogi.py` & `pgx-0.3.2/pgx/animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/backgammon.py` & `pgx-0.3.2/pgx/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/bridge_bidding.py` & `pgx-0.3.2/pgx/bridge_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 def duplicate(
     init_state: State,
 ) -> State:
     """Make duplicated state where NSplayer and EWplayer are swapped"""
     duplicated_state = copy.deepcopy(init_state)
     ix = jnp.array([1, 0, 3, 2])
     # fmt: off
-    duplicated_state = duplicated_state.replace(shuffled_players=duplicated_state.shuffled_players[ix])  # type: ignore
+    duplicated_state = duplicated_state.replace(shuffled_players=duplicated_state.shuffled_players[ix], current_player=duplicated_state.shuffled_players[ix][duplicated_state.dealer])  # type: ignore
     # fmt: on
     return duplicated_state
 
 
 @jax.jit
 def _terminated_step(
     state: State,
```

### Comparing `pgx-0.3.1/pgx/chess.py` & `pgx-0.3.2/pgx/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/connect_four.py` & `pgx-0.3.2/pgx/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/core.py` & `pgx-0.3.2/pgx/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
-from typing import Literal, Optional, Tuple, get_args
+from typing import Any, Dict, Literal, Optional, Tuple, get_args
 
 import jax
 import jax.numpy as jnp
 
-from pgx._flax.struct import dataclass
+from pgx._flax.struct import dataclass, field
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 
 # Pgx environments are versioned like OpenAI Gym or Brax.
 # OpenAI Gym forces user to specify version (e.g., `MountainCar-v0`); while Brax does not (e.g., `ant`)
@@ -67,14 +67,15 @@
     legal_action_mask: jnp.ndarray
     # NOTE: _rng_key is
     #   - used for stochastic env and auto reset
     #   - updated only when actually used
     #   - supposed NOT to be used by agent
     _rng_key: jax.random.KeyArray
     _step_count: jnp.ndarray
+    _info: Dict[str, Any] = field(default_factory=dict)  # experimental
 
     @property
     @abc.abstractmethod
     def env_id(self) -> EnvId:
         ...
 
     def _repr_html_(self) -> str:
```

### Comparing `pgx-0.3.1/pgx/experimental/gym.py` & `pgx-0.3.2/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/experimental/pettingzoo.py` & `pgx-0.3.2/pgx/experimental/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/experimental/visualize.py` & `pgx-0.3.2/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/experimental/wrappers.py` & `pgx-0.3.2/pgx/experimental/wrappers.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/go.py` & `pgx-0.3.2/pgx/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/hex.py` & `pgx-0.3.2/pgx/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/kuhn_poker.py` & `pgx-0.3.2/pgx/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/leduc_holdem.py` & `pgx-0.3.2/pgx/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/minatar/asterix.py` & `pgx-0.3.2/pgx/minatar/asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/minatar/breakout.py` & `pgx-0.3.2/pgx/minatar/breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/minatar/freeway.py` & `pgx-0.3.2/pgx/minatar/freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/minatar/seaquest.py` & `pgx-0.3.2/pgx/minatar/seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/minatar/space_invaders.py` & `pgx-0.3.2/pgx/minatar/space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/minatar/utils.py` & `pgx-0.3.2/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/othello.py` & `pgx-0.3.2/pgx/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/play2048.py` & `pgx-0.3.2/pgx/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/shogi.py` & `pgx-0.3.2/pgx/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/sparrow_mahjong.py` & `pgx-0.3.2/pgx/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx/tic_tac_toe.py` & `pgx-0.3.2/pgx/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/pgx.egg-info/SOURCES.txt` & `pgx-0.3.2/pgx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 pgx/_flax/__init__.py
 pgx/_flax/serialization.py
 pgx/_flax/struct.py
 pgx/_mahjong/__init__.py
 pgx/_mahjong/_action.py
 pgx/_mahjong/_hand.py
 pgx/experimental/__init__.py
+pgx/experimental/bridge_bidding.py
 pgx/experimental/gym.py
 pgx/experimental/pettingzoo.py
 pgx/experimental/utils.py
 pgx/experimental/visualize.py
 pgx/experimental/wrappers.py
 pgx/minatar/__init__.py
 pgx/minatar/asterix.py
```

### Comparing `pgx-0.3.1/setup.py` & `pgx-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pgx",
-    version="0.3.1",
+    version="0.3.2",
     long_description_content_type="text/markdown",
     description="",
     url="",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
     packages=find_packages(),
```

### Comparing `pgx-0.3.1/tests/minatar_utils.py` & `pgx-0.3.2/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_animal_shogi.py` & `pgx-0.3.2/tests/test_animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_asterix.py` & `pgx-0.3.2/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_backgammon.py` & `pgx-0.3.2/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_breakout.py` & `pgx-0.3.2/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_bridge_bidding.py` & `pgx-0.3.2/tests/test_bridge_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,18 @@
 def test_duplicate():
     key = jax.random.PRNGKey(0)
     for i in range(1000):
         key, subkey = jax.random.split(key)
         init_state = init(subkey)
         duplicated_state = duplicate(init_state)
         assert (
+            duplicated_state.current_player
+            == duplicated_state.shuffled_players[duplicated_state.dealer]
+        )
+        assert (
             init_state.shuffled_players[0]
             == duplicated_state.shuffled_players[1]
         )
         assert (
             init_state.shuffled_players[1]
             == duplicated_state.shuffled_players[0]
         )
```

### Comparing `pgx-0.3.1/tests/test_chess.py` & `pgx-0.3.2/tests/test_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_connect_four.py` & `pgx-0.3.2/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_freeway.py` & `pgx-0.3.2/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_go.py` & `pgx-0.3.2/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_hex.py` & `pgx-0.3.2/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_kuhn_poker.py` & `pgx-0.3.2/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_leduc_holdem.py` & `pgx-0.3.2/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_mahjong.py` & `pgx-0.3.2/tests/test_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_othello.py` & `pgx-0.3.2/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_play2048.py` & `pgx-0.3.2/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_seaquest.py` & `pgx-0.3.2/tests/test_seaquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,16 @@
     N = 100
     for _ in range(N):
         env.reset()
         s = extract_state(env, state_keys)
         s_pgx = _init_det()
         s_pgx2 = minatar2pgx(s, seaquest.State)
         for field in fields(s_pgx):
+            if field.name == '_info':
+                continue
             assert jnp.allclose(getattr(s_pgx, field.name), getattr(s_pgx2, field.name))
 
 
 def test_observe():
     env = Environment("seaquest", sticky_action_prob=0.0)
     num_actions = env.num_actions()
```

### Comparing `pgx-0.3.1/tests/test_shogi.py` & `pgx-0.3.2/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_space_invaders.py` & `pgx-0.3.2/tests/test_space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_sparrow_mahjong.py` & `pgx-0.3.2/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.1/tests/test_tic_tac_toe.py` & `pgx-0.3.2/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

