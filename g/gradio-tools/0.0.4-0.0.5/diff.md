# Comparing `tmp/gradio_tools-0.0.4.tar.gz` & `tmp/gradio_tools-0.0.5.tar.gz`

## Comparing `gradio_tools-0.0.4.tar` & `gradio_tools-0.0.5.tar`

### file list

```diff
@@ -1,56 +1,98 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/.DS_Store
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/README.md
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/162952a0-7147-4f52-ab58-f852bc5c0561/captions.json
--rw-r--r--   0        0        0   109150 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg
--rw-r--r--   0        0        0    79996 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg
--rw-r--r--   0        0        0    99128 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg
--rw-r--r--   0        0        0   101966 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/330d40a3-cc6a-41ce-96c2-002bc67df326/captions.json
--rw-r--r--   0        0        0   105846 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg
--rw-r--r--   0        0        0   126760 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg
--rw-r--r--   0        0        0   119178 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg
--rw-r--r--   0        0        0   108581 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/captions.json
--rw-r--r--   0        0        0    99607 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg
--rw-r--r--   0        0        0   131260 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg
--rw-r--r--   0        0        0   116900 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg
--rw-r--r--   0        0        0    80104 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/508529be-bc20-48b9-b0b7-003e7a21db62/captions.json
--rw-r--r--   0        0        0   122753 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg
--rw-r--r--   0        0        0    86812 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg
--rw-r--r--   0        0        0   105885 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg
--rw-r--r--   0        0        0   117917 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/70a06453-f83c-4866-89a1-d8f5c9a052d7/captions.json
--rw-r--r--   0        0        0    77205 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg
--rw-r--r--   0        0        0    92290 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg
--rw-r--r--   0        0        0   120803 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg
--rw-r--r--   0        0        0    89928 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/75c113a2-7d4f-4f14-abe9-23259df50dfb/captions.json
--rw-r--r--   0        0        0    96910 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg
--rw-r--r--   0        0        0    81978 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg
--rw-r--r--   0        0        0   112268 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg
--rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/aa3ee281-8672-4993-bb3e-09335e1de70e/captions.json
--rw-r--r--   0        0        0   122186 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg
--rw-r--r--   0        0        0    93863 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg
--rw-r--r--   0        0        0   121362 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg
--rw-r--r--   0        0        0    80154 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/ac2f6e03-9430-4c22-a559-354225a49357/captions.json
--rw-r--r--   0        0        0    79381 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg
--rw-r--r--   0        0        0   105896 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg
--rw-r--r--   0        0        0    92696 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg
--rw-r--r--   0        0        0   112587 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/examples/langchain/example.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/examples/minichain/example.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/gradio_tools/__init__.py
--rw-r--r--   0        0        0    93174 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/gradio_tools/test_image.jpg
--rw-r--r--   0        0        0    93174 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/gradio_tools/test_image.webp
--rw-r--r--   0        0        0     9642 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/gradio_tools/tools.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/scripts/format.sh
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/scripts/lint.sh
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/LICENSE
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6675 2020-02-02 00:00:00.000000 gradio_tools-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/.DS_Store
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/temp.log
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/captions.json
+-rw-r--r--   0        0        0   109150 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg
+-rw-r--r--   0        0        0    79996 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg
+-rw-r--r--   0        0        0    99128 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg
+-rw-r--r--   0        0        0   101966 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/captions.json
+-rw-r--r--   0        0        0   105846 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg
+-rw-r--r--   0        0        0   126760 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg
+-rw-r--r--   0        0        0   119178 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg
+-rw-r--r--   0        0        0   108581 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/captions.json
+-rw-r--r--   0        0        0    99607 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg
+-rw-r--r--   0        0        0   131260 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg
+-rw-r--r--   0        0        0   116900 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg
+-rw-r--r--   0        0        0    80104 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/captions.json
+-rw-r--r--   0        0        0   122753 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg
+-rw-r--r--   0        0        0    86812 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg
+-rw-r--r--   0        0        0   105885 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg
+-rw-r--r--   0        0        0   117917 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/captions.json
+-rw-r--r--   0        0        0   106965 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpmsy7r5s4.jpg
+-rw-r--r--   0        0        0   126635 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpotr65fvw.jpg
+-rw-r--r--   0        0        0   103678 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpr4__qxcx.jpg
+-rw-r--r--   0        0        0    94221 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpx4p7b1ft.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/captions.json
+-rw-r--r--   0        0        0   135053 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpj6tqr3fx.jpg
+-rw-r--r--   0        0        0   108105 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpodtfruna.jpg
+-rw-r--r--   0        0        0   137541 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmppg3kuayo.jpg
+-rw-r--r--   0        0        0   103154 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmps600nxhc.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/captions.json
+-rw-r--r--   0        0        0    77205 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg
+-rw-r--r--   0        0        0    92290 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg
+-rw-r--r--   0        0        0   120803 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg
+-rw-r--r--   0        0        0    89928 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/captions.json
+-rw-r--r--   0        0        0    96910 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg
+-rw-r--r--   0        0        0    81978 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg
+-rw-r--r--   0        0        0   112268 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg
+-rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/captions.json
+-rw-r--r--   0        0        0    93851 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmp74tk8cfs.jpg
+-rw-r--r--   0        0        0   115711 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpk_wbbklr.jpg
+-rw-r--r--   0        0        0    89571 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpvufkgo26.jpg
+-rw-r--r--   0        0        0   112338 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpz6lir7im.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/captions.json
+-rw-r--r--   0        0        0   122186 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg
+-rw-r--r--   0        0        0    93863 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg
+-rw-r--r--   0        0        0   121362 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg
+-rw-r--r--   0        0        0    80154 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/captions.json
+-rw-r--r--   0        0        0   111564 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmp5myeybsm.jpg
+-rw-r--r--   0        0        0    98332 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpd3ufb_2o.jpg
+-rw-r--r--   0        0        0   112096 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpdlfj8cj_.jpg
+-rw-r--r--   0        0        0   109146 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmps0tx8a8q.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/captions.json
+-rw-r--r--   0        0        0    79381 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg
+-rw-r--r--   0        0        0   105896 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg
+-rw-r--r--   0        0        0    92696 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg
+-rw-r--r--   0        0        0   112587 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/captions.json
+-rw-r--r--   0        0        0    93651 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmp7n9_771q.jpg
+-rw-r--r--   0        0        0    83077 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpgaejg5rz.jpg
+-rw-r--r--   0        0        0   101925 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpl3n0u99v.jpg
+-rw-r--r--   0        0        0   122576 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpuylgwvrf.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/captions.json
+-rw-r--r--   0        0        0    99572 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmphp1_2bwe.jpg
+-rw-r--r--   0        0        0   115349 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmplv4pugrr.jpg
+-rw-r--r--   0        0        0    91136 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpsvh8rgjz.jpg
+-rw-r--r--   0        0        0    91363 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpvtinxpmw.jpg
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/langchain/document_qa.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/langchain/example.py
+-rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/langchain/florida-drivers-license.jpeg
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/minichain/agent.pmpt.tpl
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/minichain/agent.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/minichain/example.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/clip_interrogator.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/document_qa.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/gradio_tool.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/image_captioning.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/image_to_music.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/prompt_generator.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/stable_diffusion.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/text_to_video.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/whisper.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/scripts/format.sh
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/scripts/lint.sh
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/PKG-INFO
```

### Comparing `gradio_tools-0.0.4/.DS_Store` & `gradio_tools-0.0.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/README.md` & `gradio_tools-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,68 @@
 # Gradio Tools: Gradio 🤝 LLM Agents
 
-Any [Gradio](https://github.com/gradio-app/gradio) application at the tips of your LLM's fingers 🦾
+There are many 1000s of [Gradio](https://github.com/gradio-app/gradio) apps on [Hugging Face Spaces](https://huggingface.co/spaces). This library puts them at the tips of your LLM's fingers 🦾
 
-[gradio_tool](https://github.com/freddyaboulton/gradio-tool) can turn any [Gradio](https://github.com/gradio-app/gradio) application into a [tool](https://python.langchain.com/en/latest/modules/agents/tools.html) that an
-LLM agent can use to complete its task.
+Specifically, [`gradio-tools`](https://pypi.org/project/gradio-tools/) is a Python library for converting Gradio apps into [tools](https://python.langchain.com/en/latest/modules/agents/tools.html) that can be leveraged by a large language model (LLM)-based agent to complete its task. For example, an LLM could use a Gradio tool to transcribe a voice recording it finds online and then summarize it for you. Or it could use a different Gradio tool to apply OCR to a document on your Google Drive and then answer questions about it.
 
-Currently supported are:
-- [LangChain agents](https://docs.langchain.com/docs/components/agents/agent) can use to complete its task.
+Currently supported libraries for agents are:
+- [LangChain](https://docs.langchain.com/docs/components/agents/agent)
 - [MiniChain](https://github.com/srush/MiniChain/tree/main)
 
+`gradio-tools` comes with a set of pre-built tools you can leverage immediately! These include:
+
+1. StableDiffusionTool - Generate an image from a given prompt using the open source stable diffusion demo hosted on [HuggingFace spaces](https://huggingface.co/spaces/stabilityai/stable-diffusion)
+2. ImageCaptionTool - Caption an image by providing a filepath based on Niels Rogge's [HuggingFace Space](https://huggingface.co/spaces/nielsr/comparing-captioning-models)
+3. ImageToMusicTool - Create an audio clip that matches the style of a given image file based on Sylvain Filoni's [HuggingFace Space](https://huggingface.co/spaces/fffiloni/img-to-music)
+4. StableDiffusionPromptGeneratorTool - Use this tool to improve a prompt for stable diffusion and other image generators based on this [HuggingFace Space](https://huggingface.co/spaces/microsoft/Promptist)
+5. TextToVideoTool - A tool for creating short videos from text. Based on this [HuggingFace Space](https://huggingface.co/spaces/damo-vilab/modelscope-text-to-video-synthesis)
+6. WhisperAudioTranscriptionTool - A tool for transcribing audio with Whisper. Based on this [HuggingFace Space](https://huggingface.co/spaces/abidlabs/whisper)
+7. ClipInterrogatorTool - A tool for reverse engineering a prompt from a source image. Based on this [HuggingFace Space](https://huggingface.co/spaces/pharma/CLIP-Interrogator)
+8. DocQueryDocumentAnsweringTool - A tool for answering questions about a document from the from the image of the document. Based on this [HuggingFace Space](https://huggingface.co/spaces/abidlabs/docquery)
+
+We welcome more contributions!
+
 ## Example Usage
 
 Simply import the desired tools from `gradio_tool` (or create your own!) and pass to `initialize_agent` from LangChain.
 
-In this example, we use some pre-built tools to generate images, caption them, and create a music clip to match its artistic style!
+In this example, we use some pre-built tools to generate images, caption them, and create a video!
 
 Read the [How It Works](#how-it-works) section to learn how to create your own tools! We welcome any new tools to the library!
 
 ```python
-os.environ["OPENAI_API_KEY"] = "<Secret Key>"
+import os
+
+if not os.getenv("OPENAI_API_KEY"):
+    raise ValueError("OPENAI_API_KEY must be set")
 
 from langchain.agents import initialize_agent
 from langchain.llms import OpenAI
-import os
-from gradio_tool.tool import StableDiffusionTool, ImageCaptioningTool, ImageToMusicTool
+from gradio_tools import (StableDiffusionTool, ImageCaptioningTool, StableDiffusionPromptGeneratorTool,
+                          TextToVideoTool)
+
 from langchain.memory import ConversationBufferMemory
 
 llm = OpenAI(temperature=0)
 memory = ConversationBufferMemory(memory_key="chat_history")
-tools = [StableDiffusionTool().langchain, ImageCaptioningTool().langchain, ImageToMusicTool().langchain]
+tools = [StableDiffusionTool().langchain, ImageCaptioningTool().langchain,
+         StableDiffusionPromptGeneratorTool().langchain, TextToVideoTool().langchain]
 
 
 agent = initialize_agent(tools, llm, memory=memory, agent="conversational-react-description", verbose=True)
-output = agent.run(input=("I would please like a photo of a dog riding a skateboard. "
-                          "Please caption this image and create a song for it."))
+output = agent.run(input=("Please create a photo of a dog riding a skateboard "
+                          "but improve my prompt prior to using an image generator."
+                          "Please caption the generated image and create a video for it using the improved prompt."))
 ```
 
-![gradio_langchain](https://user-images.githubusercontent.com/41651716/231012932-ce989347-db21-41be-8971-ab278d689b2d.gif)
+https://user-images.githubusercontent.com/41651716/233391796-49c3f762-bd58-41d7-b399-629e3c1661b2.mp4
 
 
+See the `/examples` directory for more complete code examples. 
+
 ## How it works
 
 The core abstraction is the `GradioTool`, which lets you define a new tool for your LLM as long as you implement a standard interface:
 
 ```python
 class GradioTool(BaseTool):
 
@@ -60,25 +80,20 @@
 The requirements are:
 1. The name for your tool
 2. The description for your tool. This is crucial! Agents decide which tool to use based on their description. Be precise and be sure to inclue example of what the input and the output of the tool should look like.
 3. The url or space id, e.g. `freddyaboulton/calculator`, of the Gradio application. Based on this value, `gradio_tool` will create a [gradio client](https://github.com/gradio-app/gradio/blob/main/client/python/README.md) instance to query the upstream application via API. Be sure to click the link and learn more about the gradio client library if you are not familiar with it.
 4. create_job - Given a string, this method should parse that string and return a job from the client. Most times, this is as simple as passing the string to the `submit` function of the client. More info on creating jobs [here](https://github.com/gradio-app/gradio/blob/main/client/python/README.md#making-a-prediction)
 5. postprocess - Given the result of the job, convert it to a string the LLM can display to the user.
 6. *Optional* - Some libraries, e.g. [MiniChain](https://github.com/srush/MiniChain/tree/main), may need some info about the underlying gradio input and output types used by the tool. By default, this will return gr.Textbox() but 
-if you'd like to provide more accurate info, implement the `_block_input(self)` and `_block_output(self)` methods of the tool.
+if you'd like to provide more accurate info, implement the `_block_input(self, gr)` and `_block_output(self, gr)` methods of the tool. The `gr` variable is the gradio module (the result of `import gradio as gr`). It will be
+automatically imported by the `GradiTool` parent class and passed to the `_block_input` and `_block_output` methods.
 
 And that's it!
 
-## Pre-built tools
-
-gradio_tool comes with a set of pre-built tools you can leverage immediately! These are
 
-1. StableDiffusionTool - Generate an image from a given prompt using the open source stable diffusion demo hosted on [HuggingFace spaces](https://huggingface.co/spaces/stabilityai/stable-diffusion)
-2. ImageCaptionTool - Caption an image by providing a filepath based on Niels Rogge's [HuggingFace Space](https://huggingface.co/spaces/nielsr/comparing-captioning-models)
-3. ImageToMusicTool - Create an audio clip that matches the style of a given image file based on Sylvain Filoni's [HuggingFace Space](https://huggingface.co/spaces/fffiloni/img-to-music)
 
 ## Appendix
 
 ### What are agents?
 
 A [LangChain agent](https://docs.langchain.com/docs/components/agents/agent) is a Large Language Model (LLM) that takes user input and reports an output based on using one of many tools at its disposal.
```

### Comparing `gradio_tools-0.0.4/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg` & `gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg` & `gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg` & `gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg` & `gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg` & `gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg` & `gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg` & `gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg` & `gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg` & `gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg` & `gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg` & `gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg` & `gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg` & `gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg` & `gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg` & `gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg` & `gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg` & `gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg` & `gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg` & `gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg` & `gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg` & `gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg` & `gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg` & `gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg` & `gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg` & `gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg` & `gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg` & `gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg` & `gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg` & `gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg` & `gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg` & `gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg` & `gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/examples/langchain/example.py` & `gradio_tools-0.0.5/examples/langchain/example.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import os
 
 if not os.getenv("OPENAI_API_KEY"):
     raise ValueError("OPENAI_API_KEY must be set")
 
 from langchain.agents import initialize_agent
 from langchain.llms import OpenAI
-from gradio_tools.tools import StableDiffusionTool, ImageCaptioningTool, ImageToMusicTool
+from gradio_tools.tools import (StableDiffusionTool, ImageCaptioningTool, StableDiffusionPromptGeneratorTool,
+                                TextToVideoTool)
+
 from langchain.memory import ConversationBufferMemory
 
 llm = OpenAI(temperature=0)
 memory = ConversationBufferMemory(memory_key="chat_history")
-tools = [StableDiffusionTool().langchain, ImageCaptioningTool().langchain]
+tools = [StableDiffusionTool().langchain, ImageCaptioningTool().langchain,
+         StableDiffusionPromptGeneratorTool().langchain, TextToVideoTool().langchain]
 
 
 agent = initialize_agent(tools, llm, memory=memory, agent="conversational-react-description", verbose=True)
-output = agent.run(input=("I would please like a photo of a dog riding a skateboard. "
-                          "Please caption this image and create a song for it."))
+output = agent.run(input=("Please create a photo of a dog riding a skateboard "
+                          "but improve my prompt prior to using an image generator."
+                          "Please caption the generated image and create a video for it using the improved prompt."))
```

### Comparing `gradio_tools-0.0.4/examples/minichain/example.py` & `gradio_tools-0.0.5/examples/minichain/example.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-from minichain import show, prompt, OpenAI, OpenAIStream
+
+from minichain import show, prompt, OpenAI, GradioConf
 import gradio as gr
 from gradio_tools.tools import StableDiffusionTool, ImageCaptioningTool
 
-@prompt(OpenAIStream(), stream=True)
+@prompt(OpenAI())
 def picture(model, query):
-    out = ""
-    for r in model.stream(query):
-        out += r
-        yield out
+    return model(query)
 
-@prompt(StableDiffusionTool(), stream=True, block_input=lambda: gr.Textbox(label=""))
+@prompt(StableDiffusionTool(),
+        gradio_conf=GradioConf(
+            block_output= lambda: gr.Image(),
+            block_input= lambda: gr.Textbox(show_label=False)))
 def gen(model, query):
-    for r in model.stream(query):
-        # Show a blue cube while waiting.
-        yield "https://htmlcolorcodes.com/assets/images/colors/baby-blue-color-solid-background-1920x1080.png"
-    yield r
+    return model(query)
 
-@prompt(ImageCaptioningTool(), block_output=lambda: gr.Textbox(label=""))
+@prompt(ImageCaptioningTool(),
+        gradio_conf=GradioConf(
+            block_input= lambda: gr.Image(),
+            block_output=lambda: gr.Textbox(show_label=False)))
 def caption(model, img_src):
     return model(img_src)
 
 def gradio_example(query):
     return caption(gen(picture(query)))
 
-
 desc = """
 ### Gradio Tool
 
-Examples using the gradio tool in Minichain. Example creates an image and then captions it.
+Examples using the gradio tool [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/srush/MiniChain/blob/master/examples/gradio_example.ipynb)
 
 """
 
-
 gradio = show(gradio_example,
               subprompts=[picture, gen, caption],
               examples=['Describe a one-sentence fantasy scene.',
                         'Describe a one-sentence scene happening on the moon.'],
               out_type="markdown",
               description=desc,
-              css="#advanced {display: none}"
-
+              show_advanced=False
               )
 if __name__ == "__main__":
     gradio.queue().launch()
```

### Comparing `gradio_tools-0.0.4/LICENSE` & `gradio_tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.4/pyproject.toml` & `gradio_tools-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt", "hatch-fancy-pypi-readme>=22.5.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_tools"
-version = "0.0.4"
+version = "0.0.5"
 description = "Use Gradio Apps as tools for LLM Agents"
 requires-python = ">=3.8"
 license = "MIT"
 authors = [
     { name = "Freddy Boulton", email = "alfonsoboulton@gmail.com" },
 ]
 classifiers = [
@@ -32,17 +32,18 @@
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["readme"]
 dependencies = [
     "gradio_client>=0.1.2",
 ]
 [project.optional-dependencies]
-minichain = ["gradio", "minichain"]
+minichain = ["gradio", "minichain>=0.3.3"]
 langchain = ["langchain", "openai"]
 all = ["gradio_tools[langchain]", "gradio_tools[minichain]"]
 test = ["ruff==0.0.260", "pyright==1.1.298", "isort >=5.0.6,<6.0.0", "black==22.6.0"]
+dev = ["gradio_tools[all]", "gradio_tools[test]"]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 fragments = [
   { path = "README.md"},
 ]
```

### Comparing `gradio_tools-0.0.4/PKG-INFO` & `gradio_tools-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Use Gradio Apps as tools for LLM Agents
 Author-email: Freddy Boulton <alfonsoboulton@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -24,68 +24,91 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: gradio-client>=0.1.2
 Provides-Extra: all
 Requires-Dist: gradio-tools[langchain]; extra == 'all'
 Requires-Dist: gradio-tools[minichain]; extra == 'all'
+Provides-Extra: dev
+Requires-Dist: gradio-tools[all]; extra == 'dev'
+Requires-Dist: gradio-tools[test]; extra == 'dev'
 Provides-Extra: langchain
 Requires-Dist: langchain; extra == 'langchain'
 Requires-Dist: openai; extra == 'langchain'
 Provides-Extra: minichain
 Requires-Dist: gradio; extra == 'minichain'
-Requires-Dist: minichain; extra == 'minichain'
+Requires-Dist: minichain>=0.3.3; extra == 'minichain'
 Provides-Extra: test
 Requires-Dist: black==22.6.0; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: pyright==1.1.298; extra == 'test'
 Requires-Dist: ruff==0.0.260; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Gradio Tools: Gradio 🤝 LLM Agents
 
-Any [Gradio](https://github.com/gradio-app/gradio) application at the tips of your LLM's fingers 🦾
+There are many 1000s of [Gradio](https://github.com/gradio-app/gradio) apps on [Hugging Face Spaces](https://huggingface.co/spaces). This library puts them at the tips of your LLM's fingers 🦾
 
-[gradio_tool](https://github.com/freddyaboulton/gradio-tool) can turn any [Gradio](https://github.com/gradio-app/gradio) application into a [tool](https://python.langchain.com/en/latest/modules/agents/tools.html) that an
-LLM agent can use to complete its task.
+Specifically, [`gradio-tools`](https://pypi.org/project/gradio-tools/) is a Python library for converting Gradio apps into [tools](https://python.langchain.com/en/latest/modules/agents/tools.html) that can be leveraged by a large language model (LLM)-based agent to complete its task. For example, an LLM could use a Gradio tool to transcribe a voice recording it finds online and then summarize it for you. Or it could use a different Gradio tool to apply OCR to a document on your Google Drive and then answer questions about it.
 
-Currently supported are:
-- [LangChain agents](https://docs.langchain.com/docs/components/agents/agent) can use to complete its task.
+Currently supported libraries for agents are:
+- [LangChain](https://docs.langchain.com/docs/components/agents/agent)
 - [MiniChain](https://github.com/srush/MiniChain/tree/main)
 
+`gradio-tools` comes with a set of pre-built tools you can leverage immediately! These include:
+
+1. StableDiffusionTool - Generate an image from a given prompt using the open source stable diffusion demo hosted on [HuggingFace spaces](https://huggingface.co/spaces/stabilityai/stable-diffusion)
+2. ImageCaptionTool - Caption an image by providing a filepath based on Niels Rogge's [HuggingFace Space](https://huggingface.co/spaces/nielsr/comparing-captioning-models)
+3. ImageToMusicTool - Create an audio clip that matches the style of a given image file based on Sylvain Filoni's [HuggingFace Space](https://huggingface.co/spaces/fffiloni/img-to-music)
+4. StableDiffusionPromptGeneratorTool - Use this tool to improve a prompt for stable diffusion and other image generators based on this [HuggingFace Space](https://huggingface.co/spaces/microsoft/Promptist)
+5. TextToVideoTool - A tool for creating short videos from text. Based on this [HuggingFace Space](https://huggingface.co/spaces/damo-vilab/modelscope-text-to-video-synthesis)
+6. WhisperAudioTranscriptionTool - A tool for transcribing audio with Whisper. Based on this [HuggingFace Space](https://huggingface.co/spaces/abidlabs/whisper)
+7. ClipInterrogatorTool - A tool for reverse engineering a prompt from a source image. Based on this [HuggingFace Space](https://huggingface.co/spaces/pharma/CLIP-Interrogator)
+8. DocQueryDocumentAnsweringTool - A tool for answering questions about a document from the from the image of the document. Based on this [HuggingFace Space](https://huggingface.co/spaces/abidlabs/docquery)
+
+We welcome more contributions!
+
 ## Example Usage
 
 Simply import the desired tools from `gradio_tool` (or create your own!) and pass to `initialize_agent` from LangChain.
 
-In this example, we use some pre-built tools to generate images, caption them, and create a music clip to match its artistic style!
+In this example, we use some pre-built tools to generate images, caption them, and create a video!
 
 Read the [How It Works](#how-it-works) section to learn how to create your own tools! We welcome any new tools to the library!
 
 ```python
-os.environ["OPENAI_API_KEY"] = "<Secret Key>"
+import os
+
+if not os.getenv("OPENAI_API_KEY"):
+    raise ValueError("OPENAI_API_KEY must be set")
 
 from langchain.agents import initialize_agent
 from langchain.llms import OpenAI
-import os
-from gradio_tool.tool import StableDiffusionTool, ImageCaptioningTool, ImageToMusicTool
+from gradio_tools import (StableDiffusionTool, ImageCaptioningTool, StableDiffusionPromptGeneratorTool,
+                          TextToVideoTool)
+
 from langchain.memory import ConversationBufferMemory
 
 llm = OpenAI(temperature=0)
 memory = ConversationBufferMemory(memory_key="chat_history")
-tools = [StableDiffusionTool().langchain, ImageCaptioningTool().langchain, ImageToMusicTool().langchain]
+tools = [StableDiffusionTool().langchain, ImageCaptioningTool().langchain,
+         StableDiffusionPromptGeneratorTool().langchain, TextToVideoTool().langchain]
 
 
 agent = initialize_agent(tools, llm, memory=memory, agent="conversational-react-description", verbose=True)
-output = agent.run(input=("I would please like a photo of a dog riding a skateboard. "
-                          "Please caption this image and create a song for it."))
+output = agent.run(input=("Please create a photo of a dog riding a skateboard "
+                          "but improve my prompt prior to using an image generator."
+                          "Please caption the generated image and create a video for it using the improved prompt."))
 ```
 
-![gradio_langchain](https://user-images.githubusercontent.com/41651716/231012932-ce989347-db21-41be-8971-ab278d689b2d.gif)
+https://user-images.githubusercontent.com/41651716/233391796-49c3f762-bd58-41d7-b399-629e3c1661b2.mp4
 
 
+See the `/examples` directory for more complete code examples. 
+
 ## How it works
 
 The core abstraction is the `GradioTool`, which lets you define a new tool for your LLM as long as you implement a standard interface:
 
 ```python
 class GradioTool(BaseTool):
 
@@ -103,25 +126,20 @@
 The requirements are:
 1. The name for your tool
 2. The description for your tool. This is crucial! Agents decide which tool to use based on their description. Be precise and be sure to inclue example of what the input and the output of the tool should look like.
 3. The url or space id, e.g. `freddyaboulton/calculator`, of the Gradio application. Based on this value, `gradio_tool` will create a [gradio client](https://github.com/gradio-app/gradio/blob/main/client/python/README.md) instance to query the upstream application via API. Be sure to click the link and learn more about the gradio client library if you are not familiar with it.
 4. create_job - Given a string, this method should parse that string and return a job from the client. Most times, this is as simple as passing the string to the `submit` function of the client. More info on creating jobs [here](https://github.com/gradio-app/gradio/blob/main/client/python/README.md#making-a-prediction)
 5. postprocess - Given the result of the job, convert it to a string the LLM can display to the user.
 6. *Optional* - Some libraries, e.g. [MiniChain](https://github.com/srush/MiniChain/tree/main), may need some info about the underlying gradio input and output types used by the tool. By default, this will return gr.Textbox() but 
-if you'd like to provide more accurate info, implement the `_block_input(self)` and `_block_output(self)` methods of the tool.
+if you'd like to provide more accurate info, implement the `_block_input(self, gr)` and `_block_output(self, gr)` methods of the tool. The `gr` variable is the gradio module (the result of `import gradio as gr`). It will be
+automatically imported by the `GradiTool` parent class and passed to the `_block_input` and `_block_output` methods.
 
 And that's it!
 
-## Pre-built tools
-
-gradio_tool comes with a set of pre-built tools you can leverage immediately! These are
 
-1. StableDiffusionTool - Generate an image from a given prompt using the open source stable diffusion demo hosted on [HuggingFace spaces](https://huggingface.co/spaces/stabilityai/stable-diffusion)
-2. ImageCaptionTool - Caption an image by providing a filepath based on Niels Rogge's [HuggingFace Space](https://huggingface.co/spaces/nielsr/comparing-captioning-models)
-3. ImageToMusicTool - Create an audio clip that matches the style of a given image file based on Sylvain Filoni's [HuggingFace Space](https://huggingface.co/spaces/fffiloni/img-to-music)
 
 ## Appendix
 
 ### What are agents?
 
 A [LangChain agent](https://docs.langchain.com/docs/components/agents/agent) is a Large Language Model (LLM) that takes user input and reports an output based on using one of many tools at its disposal.
```

