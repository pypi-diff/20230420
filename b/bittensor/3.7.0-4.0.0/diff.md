# Comparing `tmp/bittensor-3.7.0.tar.gz` & `tmp/bittensor-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-3.7.0.tar", last modified: Thu Mar 23 20:50:38 2023, max compression
+gzip compressed data, was "bittensor-4.0.0.tar", last modified: Thu Apr 20 17:18:38 2023, max compression
```

## Comparing `bittensor-3.7.0.tar` & `bittensor-4.0.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.560555 bittensor-3.7.0/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1087 2022-07-09 15:48:08.000000 bittensor-3.7.0/LICENSE
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11585 2023-03-23 20:50:38.028385 bittensor-3.7.0/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10559 2023-03-23 20:47:08.000000 bittensor-3.7.0/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.548555 bittensor-3.7.0/benchmarks/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11819 2023-03-23 20:47:08.000000 bittensor-3.7.0/benchmarks/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2251 2022-10-11 20:17:46.000000 bittensor-3.7.0/benchmarks/core_server.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2392 2022-07-09 15:48:08.000000 bittensor-3.7.0/benchmarks/multitron_server.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2404 2022-07-09 15:48:08.000000 bittensor-3.7.0/benchmarks/template_miner.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.548555 bittensor-3.7.0/bin/
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1297 2022-10-11 20:24:30.000000 bittensor-3.7.0/bin/btcli
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.548555 bittensor-3.7.0/bittensor/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8756 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.548555 bittensor-3.7.0/bittensor/_axon/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    27767 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_axon/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    44809 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_axon/axon_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.548555 bittensor-3.7.0/bittensor/_cli/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7347 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4316 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/cli_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.548555 bittensor-3.7.0/bittensor/_cli/commands/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      741 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    24295 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/delegates.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7578 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/inspect.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3911 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/list.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7197 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/metagraph.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6973 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/misc.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    16251 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/overview.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5434 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/query.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7587 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/register.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6979 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/run.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11039 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/stake.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4349 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/transfer.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11771 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/unstake.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6583 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/utils.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    17528 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/wallets.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7587 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/commands/weights.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    45041 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_cli/naka_cli_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.548555 bittensor-3.7.0/bittensor/_config/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6080 2022-11-24 17:43:32.000000 bittensor-3.7.0/bittensor/_config/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6168 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_config/config_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.548555 bittensor-3.7.0/bittensor/_dataset/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10966 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_dataset/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26969 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_dataset/dataset_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5467 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_dataset/dataset_mock.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3623 2022-10-11 20:17:46.000000 bittensor-3.7.0/bittensor/_dataset/thread_queue.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.548555 bittensor-3.7.0/bittensor/_dendrite/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9507 2022-12-13 00:25:39.000000 bittensor-3.7.0/bittensor/_dendrite/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    61529 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_dendrite/dendrite_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    37034 2022-10-11 20:17:46.000000 bittensor-3.7.0/bittensor/_dendrite/dendrite_mock.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2906 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/_dendrite/manager_server.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_endpoint/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7561 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_endpoint/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6780 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_endpoint/endpoint_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_ipfs/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/_ipfs/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2907 2023-02-21 20:04:30.000000 bittensor-3.7.0/bittensor/_ipfs/ipfs_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_keyfile/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1894 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/_keyfile/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    22266 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_keyfile/keyfile_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_logging/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    13273 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_logging/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_metagraph/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11783 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_metagraph/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18406 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_metagraph/metagraph_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8650 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_metagraph/metagraph_mock.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26417 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_metagraph/naka_metagraph_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_neuron/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1665 2022-10-11 20:17:46.000000 bittensor-3.7.0/bittensor/_neuron/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_neuron/audio/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1150 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/_neuron/audio/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_neuron/text/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1114 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/_neuron/text/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_neuron/text/core_server/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    33808 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_neuron/text/core_server/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      143 2022-10-11 20:17:46.000000 bittensor-3.7.0/bittensor/_neuron/text/core_server/main.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    34918 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_neuron/text/core_server/nucleus_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_neuron/text/core_validator/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    87279 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_neuron/text/core_validator/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1357 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/_neuron/text/core_validator/main.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26915 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_neuron/text/log_utilities.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11272 2022-10-11 20:17:46.000000 bittensor-3.7.0/bittensor/_neuron/text/neuron_utilities.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_prometheus/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8118 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_prometheus/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_proto/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/_proto/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    58390 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_proto/bittensor_pb2.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4168 2022-11-22 20:12:34.000000 bittensor-3.7.0/bittensor/_proto/bittensor_pb2_grpc.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_receptor/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3881 2022-11-24 17:43:32.000000 bittensor-3.7.0/bittensor/_receptor/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    36988 2022-12-13 00:25:39.000000 bittensor-3.7.0/bittensor/_receptor/receptor_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    17491 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_receptor/receptor_pool_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.552555 bittensor-3.7.0/bittensor/_serializer/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5910 2022-10-11 20:17:46.000000 bittensor-3.7.0/bittensor/_serializer/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11375 2022-10-11 20:17:46.000000 bittensor-3.7.0/bittensor/_serializer/serializer_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.556555 bittensor-3.7.0/bittensor/_subtensor/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14546 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26242 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/chain_data.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2351 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/errors.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.556555 bittensor-3.7.0/bittensor/_subtensor/extrinsics/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1126 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/extrinsics/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    17164 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/extrinsics/delegation.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6056 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/extrinsics/prometheus.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14404 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/extrinsics/registration.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10091 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/extrinsics/serving.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6243 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/extrinsics/set_weights.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18046 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/extrinsics/staking.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7596 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/extrinsics/transfer.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    15089 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/extrinsics/unstaking.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    85974 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/naka_subtensor_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    46360 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/subtensor_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14153 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_subtensor/subtensor_mock.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.556555 bittensor-3.7.0/bittensor/_synapse/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14697 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_synapse/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14073 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_synapse/synapse_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11996 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_synapse/text_causallm_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11623 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_synapse/text_causallmnext_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    15284 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_synapse/text_lasthiddenstate_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    13066 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_synapse/text_seq2seq_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.556555 bittensor-3.7.0/bittensor/_threadpool/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4618 2022-10-11 20:24:30.000000 bittensor-3.7.0/bittensor/_threadpool/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8631 2022-11-24 17:43:32.000000 bittensor-3.7.0/bittensor/_threadpool/priority_thread_pool_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.556555 bittensor-3.7.0/bittensor/_tokenizer/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2500 2022-10-11 20:17:46.000000 bittensor-3.7.0/bittensor/_tokenizer/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.556555 bittensor-3.7.0/bittensor/_wallet/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7408 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_wallet/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    37669 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_wallet/naka_wallet_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    41712 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/_wallet/wallet_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2287 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/_wallet/wallet_mock.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.556555 bittensor-3.7.0/bittensor/_wandb/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7739 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/_wandb/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.556555 bittensor-3.7.0/bittensor/utils/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8544 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/utils/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8711 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/utils/balance.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4277 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/utils/codes.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8017 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/utils/networking.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3241 2022-10-11 20:24:56.000000 bittensor-3.7.0/bittensor/utils/register_cuda.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    36240 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/utils/registration.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    33186 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/utils/registratrion_old.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3373 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/utils/stats.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      630 2022-07-09 15:48:08.000000 bittensor-3.7.0/bittensor/utils/test_utils.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    75481 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/utils/tokenizer_utils.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5908 2023-03-23 20:47:08.000000 bittensor-3.7.0/bittensor/utils/weight_utils.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:50:38.028385 bittensor-3.7.0/bittensor.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11585 2023-03-23 20:50:37.000000 bittensor-3.7.0/bittensor.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5657 2023-03-23 20:50:37.000000 bittensor-3.7.0/bittensor.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-03-23 20:50:37.000000 bittensor-3.7.0/bittensor.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1046 2023-03-23 20:50:37.000000 bittensor-3.7.0/bittensor.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       27 2023-03-23 20:50:37.000000 bittensor-3.7.0/bittensor.egg-info/top_level.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-03-23 20:50:38.028385 bittensor-3.7.0/setup.cfg
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3436 2023-03-23 20:47:08.000000 bittensor-3.7.0/setup.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.556555 bittensor-3.7.0/tests/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-3.7.0/tests/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6049 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/helpers.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.560555 bittensor-3.7.0/tests/integration_tests/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-3.7.0/tests/integration_tests/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      183 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/constant.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    82396 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/test_cli.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10989 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/test_cli_no_network.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3535 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/test_dataset.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    21138 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/test_dendrite.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      925 2023-02-21 14:16:57.000000 bittensor-3.7.0/tests/integration_tests/test_ipfs.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7593 2022-07-09 15:48:08.000000 bittensor-3.7.0/tests/integration_tests/test_keyfile.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2640 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/test_metagraph.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1566 2022-07-09 15:48:08.000000 bittensor-3.7.0/tests/integration_tests/test_priority_thread_pool.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1589 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/test_prometheus.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    20112 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/test_server_compression.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    27891 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/test_subtensor.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10005 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/integration_tests/test_wallet.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.560555 bittensor-3.7.0/tests/unit_tests/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-3.7.0/tests/unit_tests/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.560555 bittensor-3.7.0/tests/unit_tests/bittensor_tests/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    62356 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_axon.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    15186 2022-12-09 22:03:09.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_balance.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5426 2022-10-31 21:50:09.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_config.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6658 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_endpoint.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14448 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_forward_backward.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_metagraph.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14798 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_neuron.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    37744 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_receptor.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18650 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_receptor_pool.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    13476 2022-10-11 20:17:46.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_serialization.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6471 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_subtensor.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8103 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_synapse.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10781 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_wallet.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1666 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_wandb.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-03-23 20:48:00.560555 bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4938 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/test_network_utils.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    37677 2022-12-06 18:07:11.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/test_tokenizer_utils.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    23823 2023-03-23 20:47:08.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/test_utils.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2948 2022-12-06 18:07:11.000000 bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.120097 bittensor-4.0.0/
+-rw-rw-r--   0 root         (0) root         (0)     1087 2022-07-09 15:48:08.000000 bittensor-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14522 2023-04-20 17:18:38.120097 bittensor-4.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    10559 2023-03-23 20:47:08.000000 bittensor-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.108097 bittensor-4.0.0/benchmarks/
+-rw-rw-r--   0 root         (0) root         (0)    11819 2023-03-23 20:47:08.000000 bittensor-4.0.0/benchmarks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2251 2022-10-11 20:17:46.000000 bittensor-4.0.0/benchmarks/core_server.py
+-rw-rw-r--   0 root         (0) root         (0)     2392 2022-07-09 15:48:08.000000 bittensor-4.0.0/benchmarks/multitron_server.py
+-rw-rw-r--   0 root         (0) root         (0)     2404 2022-07-09 15:48:08.000000 bittensor-4.0.0/benchmarks/template_miner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.108097 bittensor-4.0.0/bin/
+-rwxrwxr-x   0 root         (0) root         (0)     1297 2022-10-11 20:24:30.000000 bittensor-4.0.0/bin/btcli
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.108097 bittensor-4.0.0/bittensor/
+-rw-rw-r--   0 root         (0) root         (0)     8756 2023-04-20 17:12:16.000000 bittensor-4.0.0/bittensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_axon/
+-rw-rw-r--   0 root         (0) root         (0)    27767 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_axon/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    44809 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_axon/axon_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_cli/
+-rw-rw-r--   0 root         (0) root         (0)     7347 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4316 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/cli_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_cli/commands/
+-rw-rw-r--   0 root         (0) root         (0)      741 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    24295 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/delegates.py
+-rw-rw-r--   0 root         (0) root         (0)     7578 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/inspect.py
+-rw-rw-r--   0 root         (0) root         (0)     3911 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/list.py
+-rw-rw-r--   0 root         (0) root         (0)     7197 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/metagraph.py
+-rw-rw-r--   0 root         (0) root         (0)     6973 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    16251 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/overview.py
+-rw-rw-r--   0 root         (0) root         (0)     5434 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/query.py
+-rw-rw-r--   0 root         (0) root         (0)     7587 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/register.py
+-rw-rw-r--   0 root         (0) root         (0)     6979 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/run.py
+-rw-rw-r--   0 root         (0) root         (0)    11039 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/stake.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/transfer.py
+-rw-rw-r--   0 root         (0) root         (0)    11142 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/unstake.py
+-rw-rw-r--   0 root         (0) root         (0)     6583 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    17528 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/wallets.py
+-rw-rw-r--   0 root         (0) root         (0)     7587 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/weights.py
+-rw-rw-r--   0 root         (0) root         (0)    45041 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/naka_cli_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_config/
+-rw-rw-r--   0 root         (0) root         (0)     6080 2022-11-24 17:43:32.000000 bittensor-4.0.0/bittensor/_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6168 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_config/config_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_dataset/
+-rw-rw-r--   0 root         (0) root         (0)    10966 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_dataset/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    26969 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_dataset/dataset_impl.py
+-rw-rw-r--   0 root         (0) root         (0)     5467 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_dataset/dataset_mock.py
+-rw-rw-r--   0 root         (0) root         (0)     3623 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_dataset/thread_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_dendrite/
+-rw-rw-r--   0 root         (0) root         (0)     9507 2022-12-13 00:25:39.000000 bittensor-4.0.0/bittensor/_dendrite/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    61529 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_dendrite/dendrite_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    37034 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_dendrite/dendrite_mock.py
+-rw-rw-r--   0 root         (0) root         (0)     2906 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_dendrite/manager_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_endpoint/
+-rw-rw-r--   0 root         (0) root         (0)     7561 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_endpoint/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6780 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_endpoint/endpoint_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_ipfs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_ipfs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2907 2023-02-21 20:04:30.000000 bittensor-4.0.0/bittensor/_ipfs/ipfs_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_keyfile/
+-rw-rw-r--   0 root         (0) root         (0)     1894 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_keyfile/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22266 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_keyfile/keyfile_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_logging/
+-rw-rw-r--   0 root         (0) root         (0)    13273 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_metagraph/
+-rw-rw-r--   0 root         (0) root         (0)    11783 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_metagraph/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    18406 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_metagraph/metagraph_impl.py
+-rw-rw-r--   0 root         (0) root         (0)     8650 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_metagraph/metagraph_mock.py
+-rw-rw-r--   0 root         (0) root         (0)    26417 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_metagraph/naka_metagraph_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/
+-rw-rw-r--   0 root         (0) root         (0)     1665 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_neuron/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/audio/
+-rw-rw-r--   0 root         (0) root         (0)     1150 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_neuron/audio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/text/
+-rw-rw-r--   0 root         (0) root         (0)     1114 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_neuron/text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/text/core_server/
+-rw-rw-r--   0 root         (0) root         (0)    33808 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_neuron/text/core_server/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      143 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_neuron/text/core_server/main.py
+-rw-rw-r--   0 root         (0) root         (0)    34918 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_neuron/text/core_server/nucleus_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/text/core_validator/
+-rw-rw-r--   0 root         (0) root         (0)    87279 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_neuron/text/core_validator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1357 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_neuron/text/core_validator/main.py
+-rw-rw-r--   0 root         (0) root         (0)    26915 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_neuron/text/log_utilities.py
+-rw-rw-r--   0 root         (0) root         (0)    11272 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_neuron/text/neuron_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_prometheus/
+-rw-rw-r--   0 root         (0) root         (0)     8118 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_prometheus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_proto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_proto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    58390 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_proto/bittensor_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     4168 2022-11-22 20:12:34.000000 bittensor-4.0.0/bittensor/_proto/bittensor_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_receptor/
+-rw-rw-r--   0 root         (0) root         (0)     3881 2022-11-24 17:43:32.000000 bittensor-4.0.0/bittensor/_receptor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    36988 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_receptor/receptor_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    17491 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_receptor/receptor_pool_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_serializer/
+-rw-rw-r--   0 root         (0) root         (0)     5910 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_serializer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11375 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_serializer/serializer_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_subtensor/
+-rw-rw-r--   0 root         (0) root         (0)    14546 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    26242 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/chain_data.py
+-rw-rw-r--   0 root         (0) root         (0)     2351 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_subtensor/extrinsics/
+-rw-rw-r--   0 root         (0) root         (0)     1126 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17164 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/delegation.py
+-rw-rw-r--   0 root         (0) root         (0)     6056 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/prometheus.py
+-rw-rw-r--   0 root         (0) root         (0)    14404 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/registration.py
+-rw-rw-r--   0 root         (0) root         (0)    10091 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/serving.py
+-rw-rw-r--   0 root         (0) root         (0)     6243 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/set_weights.py
+-rw-rw-r--   0 root         (0) root         (0)    18046 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/staking.py
+-rw-rw-r--   0 root         (0) root         (0)     7596 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/transfer.py
+-rw-rw-r--   0 root         (0) root         (0)    15089 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/unstaking.py
+-rw-rw-r--   0 root         (0) root         (0)    85974 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/naka_subtensor_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    46360 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/subtensor_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    14153 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/subtensor_mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_synapse/
+-rw-rw-r--   0 root         (0) root         (0)    14697 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14073 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/synapse_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    11996 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/text_causallm_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    11623 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/text_causallmnext_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    15284 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/text_lasthiddenstate_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    13066 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/text_seq2seq_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_threadpool/
+-rw-rw-r--   0 root         (0) root         (0)     4618 2022-10-11 20:24:30.000000 bittensor-4.0.0/bittensor/_threadpool/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8631 2022-11-24 17:43:32.000000 bittensor-4.0.0/bittensor/_threadpool/priority_thread_pool_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_tokenizer/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_tokenizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_wallet/
+-rw-rw-r--   0 root         (0) root         (0)     7408 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_wallet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    37669 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_wallet/naka_wallet_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    41712 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_wallet/wallet_impl.py
+-rw-rw-r--   0 root         (0) root         (0)     2287 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_wallet/wallet_mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_wandb/
+-rw-rw-r--   0 root         (0) root         (0)     7739 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_wandb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/utils/
+-rw-rw-r--   0 root         (0) root         (0)     8544 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8711 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/utils/balance.py
+-rw-rw-r--   0 root         (0) root         (0)     4277 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/utils/codes.py
+-rw-rw-r--   0 root         (0) root         (0)     8017 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/utils/networking.py
+-rw-rw-r--   0 root         (0) root         (0)     3241 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/register_cuda.py
+-rw-rw-r--   0 root         (0) root         (0)    36240 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/registration.py
+-rw-rw-r--   0 root         (0) root         (0)    33186 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/registratrion_old.py
+-rw-rw-r--   0 root         (0) root         (0)     3373 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/utils/stats.py
+-rw-rw-r--   0 root         (0) root         (0)      630 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/utils/test_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    75481 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/utils/tokenizer_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5908 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/weight_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.108097 bittensor-4.0.0/bittensor.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)    14522 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5657 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)     1046 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       27 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 17:18:38.120097 bittensor-4.0.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3436 2023-03-23 20:47:08.000000 bittensor-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6049 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/tests/integration_tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/integration_tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      183 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/constant.py
+-rw-rw-r--   0 root         (0) root         (0)    82396 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_cli.py
+-rw-rw-r--   0 root         (0) root         (0)    10989 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_cli_no_network.py
+-rw-rw-r--   0 root         (0) root         (0)     3535 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/test_dataset.py
+-rw-rw-r--   0 root         (0) root         (0)    21138 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/test_dendrite.py
+-rw-rw-r--   0 root         (0) root         (0)      925 2023-02-21 14:16:57.000000 bittensor-4.0.0/tests/integration_tests/test_ipfs.py
+-rw-rw-r--   0 root         (0) root         (0)     7593 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/integration_tests/test_keyfile.py
+-rw-rw-r--   0 root         (0) root         (0)     2640 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_metagraph.py
+-rw-rw-r--   0 root         (0) root         (0)     1566 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/integration_tests/test_priority_thread_pool.py
+-rw-rw-r--   0 root         (0) root         (0)     1589 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_prometheus.py
+-rw-rw-r--   0 root         (0) root         (0)    20112 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/test_server_compression.py
+-rw-rw-r--   0 root         (0) root         (0)    27891 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_subtensor.py
+-rw-rw-r--   0 root         (0) root         (0)    10005 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/test_wallet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/tests/unit_tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.120097 bittensor-4.0.0/tests/unit_tests/bittensor_tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    62356 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_axon.py
+-rw-rw-r--   0 root         (0) root         (0)    15186 2022-12-09 22:03:09.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_balance.py
+-rw-rw-r--   0 root         (0) root         (0)     5426 2022-10-31 21:50:09.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6658 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_endpoint.py
+-rw-rw-r--   0 root         (0) root         (0)    14448 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_forward_backward.py
+-rw-rw-r--   0 root         (0) root         (0)     2136 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_metagraph.py
+-rw-rw-r--   0 root         (0) root         (0)    14798 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_neuron.py
+-rw-rw-r--   0 root         (0) root         (0)    37744 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_receptor.py
+-rw-rw-r--   0 root         (0) root         (0)    18650 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_receptor_pool.py
+-rw-rw-r--   0 root         (0) root         (0)    13476 2022-10-11 20:17:46.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_serialization.py
+-rw-rw-r--   0 root         (0) root         (0)     6471 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_subtensor.py
+-rw-rw-r--   0 root         (0) root         (0)     8103 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_synapse.py
+-rw-rw-r--   0 root         (0) root         (0)    10781 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     1666 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.120097 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4938 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_network_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    37677 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_tokenizer_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    23823 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2948 2022-12-06 18:07:11.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py
```

### Comparing `bittensor-3.7.0/LICENSE` & `bittensor-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/PKG-INFO` & `bittensor-4.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: bittensor
-Version: 3.7.0
-Summary: bittensor
-Home-page: https://github.com/opentensor/bittensor
-Author: bittensor.com
-Author-email: 
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
 
 # **Bittensor** <!-- omit in toc -->
 [![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
 [![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `bittensor-3.7.0/README.md` & `bittensor-4.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,366 +1,393 @@
-<div align="center">
-
-# **Bittensor** <!-- omit in toc -->
-[![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
-[![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
-
----
-
-### Internet-scale Neural Networks <!-- omit in toc -->
-
-[Discord](https://discord.gg/bittensor) • [Docs](https://docs.bittensor.com/) • [Network](https://www.bittensor.com/network) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU) • [Code](https://github.com/opentensor/BitTensor)
-
-</div>
-
-This repository contains Bittensor's Python API, which can be used for the following purposes:
-
-1. Querying the Bittensor network as a [client](https://github.com/opentensor/bittensor#31-client).
-2. Running and building Bittensor miners and validators for [mining TAO](https://github.com/opentensor/bittensor#43-running-a-template-miner).
-3. Pulling network [state information](https://github.com/opentensor/bittensor#3-using-bittensor).
-4. Managing [TAO wallets](https://github.com/opentensor/bittensor#41-cli), balances, transfers, etc.
-
-Bittensor is a mining network, similar to Bitcoin, that includes built-in incentives designed to encourage miners to provide value by hosting trained or training machine learning models. These models can be queried by clients seeking inference over inputs, such as token-based text generations or numerical embeddings from a large foundation model like GPT-NeoX-20B.
-
-Token-based incentives are designed to drive the network's growth and distribute the value generated by the network directly to the individuals producing that value, without intermediaries. The network is open to all participants, and no individual or group has full control over what is learned, who can profit from it, or who can access it.
-
-To learn more about Bittensor, please read our [paper](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU/view).
-
-- [1. Documentation](#1-documentation)
-- [2. Install](#2-install)
-- [3. Using Bittensor](#3-using-bittensor)
-  - [3.1. Client](#31-client)
-  - [3.2. Server](#32-server)
-  - [3.3. Validator](#33-validator)
-- [4. Features](#4-features)
-  - [4.1. Using the CLI](#41-cli)
-  - [4.2. Selecting the network to join](#42-selecting-the-network-to-join)
-  - [4.3. Running a template miner](#43-running-a-template-miner)
-  - [4.4. Running a template server](#44-running-a-template-server)
-  - [4.5. Syncing with the chain/ Finding the ranks/stake/uids of other nodes](#46-syncing-with-the-chain-finding-the-ranksstakeuids-of-other-nodes)
-  - [4.6. Finding and creating the endpoints for other nodes in the network](#47-finding-and-creating-the-endpoints-for-other-nodes-in-the-network)
-  - [4.7. Querying others in the network](#48-querying-others-in-the-network)
-- [5. Release](#5-release)
-- [6. License](#6-license)
-- [7. Acknowledgments](#7-acknowledgments)
-
-## 1. Documentation
-
-https://docs.bittensor.com/
-
-## 2. Install
-Three ways to install Bittensor
-
-1. Through the installer:
-```
-$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"
-```
-
-2. With pip:
-```bash
-$ pip3 install bittensor
-```
-
-3. From source:
-```
-$ git clone https://github.com/opentensor/bittensor.git
-$ python3 -m pip install -e bittensor/
-```
-
-## 3. Using Bittensor
-
-The following examples showcase how to use the Bittensor API for 3 separate purposes.
-
-### 3.1. Client 
-
-Querying the network for generations.
-
-```python
-import bittensor
-wallet = bittensor.wallet().create_if_non_existent()
-graph = bittensor.metagraph().sync()
-print ( bittensor.dendrite( wallet = wallet ).generate
-        ( 
-            endpoints = graph.endpoints[graph.incentive.sort()[1][-1]],  // The highest ranked peer.
-            prompt = "The quick brown fox jumped over the lazy dog", 
-            num_to_generate = 20
+Metadata-Version: 2.1
+Name: bittensor
+Version: 4.0.0
+Summary: bittensor
+Home-page: https://github.com/opentensor/bittensor
+Author: bittensor.com
+Author-email: 
+License: MIT
+Description: <div align="center">
+        
+        # **Bittensor** <!-- omit in toc -->
+        [![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
+        [![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
+        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
+        
+        ---
+        
+        ### Internet-scale Neural Networks <!-- omit in toc -->
+        
+        [Discord](https://discord.gg/bittensor) • [Docs](https://docs.bittensor.com/) • [Network](https://www.bittensor.com/network) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU) • [Code](https://github.com/opentensor/BitTensor)
+        
+        </div>
+        
+        This repository contains Bittensor's Python API, which can be used for the following purposes:
+        
+        1. Querying the Bittensor network as a [client](https://github.com/opentensor/bittensor#31-client).
+        2. Running and building Bittensor miners and validators for [mining TAO](https://github.com/opentensor/bittensor#43-running-a-template-miner).
+        3. Pulling network [state information](https://github.com/opentensor/bittensor#3-using-bittensor).
+        4. Managing [TAO wallets](https://github.com/opentensor/bittensor#41-cli), balances, transfers, etc.
+        
+        Bittensor is a mining network, similar to Bitcoin, that includes built-in incentives designed to encourage miners to provide value by hosting trained or training machine learning models. These models can be queried by clients seeking inference over inputs, such as token-based text generations or numerical embeddings from a large foundation model like GPT-NeoX-20B.
+        
+        Token-based incentives are designed to drive the network's growth and distribute the value generated by the network directly to the individuals producing that value, without intermediaries. The network is open to all participants, and no individual or group has full control over what is learned, who can profit from it, or who can access it.
+        
+        To learn more about Bittensor, please read our [paper](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU/view).
+        
+        - [1. Documentation](#1-documentation)
+        - [2. Install](#2-install)
+        - [3. Using Bittensor](#3-using-bittensor)
+          - [3.1. Client](#31-client)
+          - [3.2. Server](#32-server)
+          - [3.3. Validator](#33-validator)
+        - [4. Features](#4-features)
+          - [4.1. Using the CLI](#41-cli)
+          - [4.2. Selecting the network to join](#42-selecting-the-network-to-join)
+          - [4.3. Running a template miner](#43-running-a-template-miner)
+          - [4.4. Running a template server](#44-running-a-template-server)
+          - [4.5. Syncing with the chain/ Finding the ranks/stake/uids of other nodes](#46-syncing-with-the-chain-finding-the-ranksstakeuids-of-other-nodes)
+          - [4.6. Finding and creating the endpoints for other nodes in the network](#47-finding-and-creating-the-endpoints-for-other-nodes-in-the-network)
+          - [4.7. Querying others in the network](#48-querying-others-in-the-network)
+        - [5. Release](#5-release)
+        - [6. License](#6-license)
+        - [7. Acknowledgments](#7-acknowledgments)
+        
+        ## 1. Documentation
+        
+        https://docs.bittensor.com/
+        
+        ## 2. Install
+        Three ways to install Bittensor
+        
+        1. Through the installer:
+        ```
+        $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"
+        ```
+        
+        2. With pip:
+        ```bash
+        $ pip3 install bittensor
+        ```
+        
+        3. From source:
+        ```
+        $ git clone https://github.com/opentensor/bittensor.git
+        $ python3 -m pip install -e bittensor/
+        ```
+        
+        ## 3. Using Bittensor
+        
+        The following examples showcase how to use the Bittensor API for 3 separate purposes.
+        
+        ### 3.1. Client 
+        
+        Querying the network for generations.
+        
+        ```python
+        import bittensor
+        wallet = bittensor.wallet().create_if_non_existent()
+        graph = bittensor.metagraph().sync()
+        print ( bittensor.dendrite( wallet = wallet ).generate
+                ( 
+                    endpoints = graph.endpoints[graph.incentive.sort()[1][-1]],  // The highest ranked peer.
+                    prompt = "The quick brown fox jumped over the lazy dog", 
+                    num_to_generate = 20
+                )
         )
-)
-```
-
-Querying the network for representations.
-
-```python
-import bittensor
-wallet = bittensor.wallet().create_if_non_existent()
-graph = bittensor.metagraph().sync()
-print ( bittensor.dendrite( wallet = wallet ).text_last_hidden_state
-        (
-            endpoints = graph.endpoints[graph.incentive.sort()[1][-1]],  // The highest ranked peer.
-            inputs = "The quick brown fox jumped over the lazy dog"
+        ```
+        
+        Querying the network for representations.
+        
+        ```python
+        import bittensor
+        wallet = bittensor.wallet().create_if_non_existent()
+        graph = bittensor.metagraph().sync()
+        print ( bittensor.dendrite( wallet = wallet ).text_last_hidden_state
+                (
+                    endpoints = graph.endpoints[graph.incentive.sort()[1][-1]],  // The highest ranked peer.
+                    inputs = "The quick brown fox jumped over the lazy dog"
+                )
         )
-)
-...
-// Apply model. 
-...
-loss.backward() // Accumulate gradients on endpoints.
-```
-
-### 3.2. Server
-
-Serving a custom model.
-
-```python
-import bittensor
-import torch
-from transformers import GPT2Model, GPT2Config
-
-model = GPT2Model( GPT2Config(vocab_size = bittensor.__vocab_size__, n_embd = bittensor.__network_dim__ , n_head = 8))
-optimizer = torch.optim.SGD( [ {"params": model.parameters()} ], lr = 0.01 )
-
-def forward_text( pubkey, inputs_x ):
-    return model( inputs_x )
-  
-def backward_text( pubkey, inputs_x, grads_dy ):
-    with torch.enable_grad():
-        outputs_y = model( inputs_x.to(device) ).last_hidden_state
-        torch.autograd.backward (
-            tensors = [ outputs_y.to(device) ],
-            grad_tensors = [ grads_dy.to(device) ]
+        ...
+        // Apply model. 
+        ...
+        loss.backward() // Accumulate gradients on endpoints.
+        ```
+        
+        ### 3.2. Server
+        
+        Serving a custom model.
+        
+        ```python
+        import bittensor
+        import torch
+        from transformers import GPT2Model, GPT2Config
+        
+        model = GPT2Model( GPT2Config(vocab_size = bittensor.__vocab_size__, n_embd = bittensor.__network_dim__ , n_head = 8))
+        optimizer = torch.optim.SGD( [ {"params": model.parameters()} ], lr = 0.01 )
+        
+        def forward_text( pubkey, inputs_x ):
+            return model( inputs_x )
+          
+        def backward_text( pubkey, inputs_x, grads_dy ):
+            with torch.enable_grad():
+                outputs_y = model( inputs_x.to(device) ).last_hidden_state
+                torch.autograd.backward (
+                    tensors = [ outputs_y.to(device) ],
+                    grad_tensors = [ grads_dy.to(device) ]
+                )
+                optimizer.step()
+                optimizer.zero_grad() 
+        
+        wallet = bittensor.wallet().create().register()
+        axon = bittensor.axon (
+            wallet = wallet,
+            forward_text = forward_text,
+            backward_text = backward_text
+        ).start().serve()
+        ```
+        
+        ### 3.3. Validator 
+        
+        Validating models by setting weights.
+        
+        ```python
+        import bittensor
+        import torch
+        
+        graph = bittensor.metagraph().sync()
+        dataset = bittensor.dataset()
+        chain_weights = torch.ones( [graph.n.item()], dtype = torch.float32 )
+        
+        for batch in dataset.dataloader( 10 ):
+            ...
+            // Train chain_weights.
+            ...
+        bittensor.subtensor().set_weights (
+            weights = chain_weights,
+            uids = graph.uids,
+            wait_for_inclusion = True,
+            wallet = bittensor.wallet(),
         )
-        optimizer.step()
-        optimizer.zero_grad() 
-
-wallet = bittensor.wallet().create().register()
-axon = bittensor.axon (
-    wallet = wallet,
-    forward_text = forward_text,
-    backward_text = backward_text
-).start().serve()
-```
-
-### 3.3. Validator 
-
-Validating models by setting weights.
-
-```python
-import bittensor
-import torch
-
-graph = bittensor.metagraph().sync()
-dataset = bittensor.dataset()
-chain_weights = torch.ones( [graph.n.item()], dtype = torch.float32 )
-
-for batch in dataset.dataloader( 10 ):
-    ...
-    // Train chain_weights.
-    ...
-bittensor.subtensor().set_weights (
-    weights = chain_weights,
-    uids = graph.uids,
-    wait_for_inclusion = True,
-    wallet = bittensor.wallet(),
-)
-```
-## 4. Features
-
-### 4.1. CLI
-
-Creating a new wallet.
-```bash
-$ btcli new_coldkey
-$ btcli new_hotkey
-```
-
-Listing your wallets
-```bash
-$ btcli list
-```
-
-Registering a wallet
-```bash
-$ btcli register
-```
-
-Running a miner
-```bash
-$ btcli run
-```
-
-Checking balances
-```bash
-$ btcli overview
-```
-
-Checking the incentive mechanism.
-```bash
-$ btcli metagraph
-```
-
-Transfering funds
-```bash
-$ btcli transfer
-```
-
-Staking/Unstaking from a hotkey
-```bash
-$ btcli stake
-$ btcli unstake
-```
-
-### 4.2. Selecting the network to join 
-There are two open Bittensor networks: staging (Nobunaga) and main (Nakamoto, Local).
-
-- Nobunaga (staging)
-- Nakamoto (main)
-- Local (localhost, mirrors nakamoto)
-
-```bash
-$ export NETWORK=local 
-$ python (..) --subtensor.network $NETWORK
-or
->> btcli run --subtensor.network $NETWORK
-```
-
-### 4.3. Running a template miner
-
-The following command will run Bittensor's template miner
-
-```bash
-$ cd bittensor
-$ python ./bittensor/_neuron/text/template_miner/main.py
-```
-or 
-```python3
->> import bittensor
->> bittensor.neurons.text.template_miner.neuron().run()
-```
-
-OR with customized settings
-
-```bash
-$ cd bittensor
-$ python3 ./bittensor/_neuron/text/template_miner/main.py --wallet.name <WALLET NAME> --wallet.hotkey <HOTKEY NAME>
-```
-
-For the full list of settings, please run
-
-```bash
-$ python3 ~/.bittensor/bittensor/bittensor/_neuron/neurons/text/template_miner/main.py --help
-```
-
-### 4.4. Running a template server
-
-The template server follows a similar structure as the template miner. 
-
-```bash
-$ cd bittensor
-$ python3 ./bittensor/_neuron/text/core_server/main.py --wallet.name <WALLET NAME> --wallet.hotkey <HOTKEY NAME>
-```
-or 
-```python3
->> import bittensor
->> bittensor.neurons.text.core_server.neuron().run()
-```
-
-For the full list of settings, please run
-
-```bash
-$ cd bittensor
-$ python3 ./bittensor/_neuron/text/core_server/main.py --help
-```
-
-
-###  4.5. Serving an endpoint on the network
-
-Endpoints are served to the bittensor network through the axon. The axon is instantiated via a wallet which holds an account on the Bittensor network.
-
-```python
-import bittensor
-
-wallet = bittensor.wallet().create().register()
-axon = bittensor.axon (
-    wallet = wallet,
-    forward_text = forward_text,
-    backward_text = backward_text
-).start().serve()
-```
-
-### 4.6. Syncing with the chain/ Finding the ranks/stake/uids of other nodes
-
-Information from the chain is collected/formated by the metagraph.
-
-```bash
-btcli metagraph
-```
-and
-```python
-import bittensor
-
-meta = bittensor.metagraph()
-meta.sync()
-
-# --- uid ---
-print(meta.uids)
-
-# --- hotkeys ---
-print(meta.hotkeys)
-
-# --- ranks ---
-print(meta.R)
-
-# --- stake ---
-print(meta.S)
-
-```
-
-### 4.7. Finding and creating the endpoints for other nodes in the network
-
-```python
-import bittensor
-
-meta = bittensor.metagraph()
-meta.sync()
-
-### Address for the node uid 0
-endpoint_as_tensor = meta.endpoints[0]
-endpoint_as_object = meta.endpoint_objs[0]
-```
-
-### 4.8. Querying others in the network
-
-```python
-import bittensor
-
-meta = bittensor.metagraph()
-meta.sync()
-
-### Address for the node uid 0
-endpoint_0 = meta.endpoints[0]
-
-### Creating the wallet, and dendrite
-wallet = bittensor.wallet().create().register()
-den = bittensor.dendrite(wallet = wallet)
-representations, _, _ = den.forward_text (
-    endpoints = endpoint_0,
-    inputs = "Hello World"
-)
-
-```
-
-## 5. Release
-The release manager should follow the instructions of the [RELEASE_GUIDELINES.md](./RELEASE_GUIDELINES.md) document.
-
-## 6. License
-The MIT License (MIT)
-Copyright © 2021 Yuma Rao
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-## 7. Acknowledgments
-**learning-at-home/hivemind**
+        ```
+        ## 4. Features
+        
+        ### 4.1. CLI
+        
+        Creating a new wallet.
+        ```bash
+        $ btcli new_coldkey
+        $ btcli new_hotkey
+        ```
+        
+        Listing your wallets
+        ```bash
+        $ btcli list
+        ```
+        
+        Registering a wallet
+        ```bash
+        $ btcli register
+        ```
+        
+        Running a miner
+        ```bash
+        $ btcli run
+        ```
+        
+        Checking balances
+        ```bash
+        $ btcli overview
+        ```
+        
+        Checking the incentive mechanism.
+        ```bash
+        $ btcli metagraph
+        ```
+        
+        Transfering funds
+        ```bash
+        $ btcli transfer
+        ```
+        
+        Staking/Unstaking from a hotkey
+        ```bash
+        $ btcli stake
+        $ btcli unstake
+        ```
+        
+        ### 4.2. Selecting the network to join 
+        There are two open Bittensor networks: staging (Nobunaga) and main (Nakamoto, Local).
+        
+        - Nobunaga (staging)
+        - Nakamoto (main)
+        - Local (localhost, mirrors nakamoto)
+        
+        ```bash
+        $ export NETWORK=local 
+        $ python (..) --subtensor.network $NETWORK
+        or
+        >> btcli run --subtensor.network $NETWORK
+        ```
+        
+        ### 4.3. Running a template miner
+        
+        The following command will run Bittensor's template miner
+        
+        ```bash
+        $ cd bittensor
+        $ python ./bittensor/_neuron/text/template_miner/main.py
+        ```
+        or 
+        ```python3
+        >> import bittensor
+        >> bittensor.neurons.text.template_miner.neuron().run()
+        ```
+        
+        OR with customized settings
+        
+        ```bash
+        $ cd bittensor
+        $ python3 ./bittensor/_neuron/text/template_miner/main.py --wallet.name <WALLET NAME> --wallet.hotkey <HOTKEY NAME>
+        ```
+        
+        For the full list of settings, please run
+        
+        ```bash
+        $ python3 ~/.bittensor/bittensor/bittensor/_neuron/neurons/text/template_miner/main.py --help
+        ```
+        
+        ### 4.4. Running a template server
+        
+        The template server follows a similar structure as the template miner. 
+        
+        ```bash
+        $ cd bittensor
+        $ python3 ./bittensor/_neuron/text/core_server/main.py --wallet.name <WALLET NAME> --wallet.hotkey <HOTKEY NAME>
+        ```
+        or 
+        ```python3
+        >> import bittensor
+        >> bittensor.neurons.text.core_server.neuron().run()
+        ```
+        
+        For the full list of settings, please run
+        
+        ```bash
+        $ cd bittensor
+        $ python3 ./bittensor/_neuron/text/core_server/main.py --help
+        ```
+        
+        
+        ###  4.5. Serving an endpoint on the network
+        
+        Endpoints are served to the bittensor network through the axon. The axon is instantiated via a wallet which holds an account on the Bittensor network.
+        
+        ```python
+        import bittensor
+        
+        wallet = bittensor.wallet().create().register()
+        axon = bittensor.axon (
+            wallet = wallet,
+            forward_text = forward_text,
+            backward_text = backward_text
+        ).start().serve()
+        ```
+        
+        ### 4.6. Syncing with the chain/ Finding the ranks/stake/uids of other nodes
+        
+        Information from the chain is collected/formated by the metagraph.
+        
+        ```bash
+        btcli metagraph
+        ```
+        and
+        ```python
+        import bittensor
+        
+        meta = bittensor.metagraph()
+        meta.sync()
+        
+        # --- uid ---
+        print(meta.uids)
+        
+        # --- hotkeys ---
+        print(meta.hotkeys)
+        
+        # --- ranks ---
+        print(meta.R)
+        
+        # --- stake ---
+        print(meta.S)
+        
+        ```
+        
+        ### 4.7. Finding and creating the endpoints for other nodes in the network
+        
+        ```python
+        import bittensor
+        
+        meta = bittensor.metagraph()
+        meta.sync()
+        
+        ### Address for the node uid 0
+        endpoint_as_tensor = meta.endpoints[0]
+        endpoint_as_object = meta.endpoint_objs[0]
+        ```
+        
+        ### 4.8. Querying others in the network
+        
+        ```python
+        import bittensor
+        
+        meta = bittensor.metagraph()
+        meta.sync()
+        
+        ### Address for the node uid 0
+        endpoint_0 = meta.endpoints[0]
+        
+        ### Creating the wallet, and dendrite
+        wallet = bittensor.wallet().create().register()
+        den = bittensor.dendrite(wallet = wallet)
+        representations, _, _ = den.forward_text (
+            endpoints = endpoint_0,
+            inputs = "Hello World"
+        )
+        
+        ```
+        
+        ## 5. Release
+        The release manager should follow the instructions of the [RELEASE_GUIDELINES.md](./RELEASE_GUIDELINES.md) document.
+        
+        ## 6. License
+        The MIT License (MIT)
+        Copyright © 2021 Yuma Rao
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+        
+        ## 7. Acknowledgments
+        **learning-at-home/hivemind**
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `bittensor-3.7.0/benchmarks/__init__.py` & `bittensor-4.0.0/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/benchmarks/core_server.py` & `bittensor-4.0.0/benchmarks/core_server.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/benchmarks/multitron_server.py` & `bittensor-4.0.0/benchmarks/multitron_server.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/benchmarks/template_miner.py` & `bittensor-4.0.0/benchmarks/template_miner.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bin/btcli` & `bittensor-4.0.0/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/__init__.py` & `bittensor-4.0.0/bittensor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from rich.traceback import install
 from prometheus_client import Info
 
 import nest_asyncio
 nest_asyncio.apply()
 
 # Bittensor code and protocol version.
-__version__ = '3.7.0'
+__version__ = '4.0.0'
 version_split = __version__.split(".")
 __version_as_int__ = (100 * int(version_split[0])) + (10 * int(version_split[1])) + (1 * int(version_split[2]))
 __new_signature_version__ = 360
 
 # Turn off rich console locals trace.
 from rich.traceback import install
 install(show_locals=False)
```

### Comparing `bittensor-3.7.0/bittensor/_axon/__init__.py` & `bittensor-4.0.0/bittensor/_axon/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_axon/axon_impl.py` & `bittensor-4.0.0/bittensor/_axon/axon_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/__init__.py` & `bittensor-4.0.0/bittensor/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/cli_impl.py` & `bittensor-4.0.0/bittensor/_cli/cli_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/__init__.py` & `bittensor-4.0.0/bittensor/_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/delegates.py` & `bittensor-4.0.0/bittensor/_cli/commands/delegates.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/inspect.py` & `bittensor-4.0.0/bittensor/_cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/list.py` & `bittensor-4.0.0/bittensor/_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/metagraph.py` & `bittensor-4.0.0/bittensor/_cli/commands/metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/misc.py` & `bittensor-4.0.0/bittensor/_cli/commands/misc.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/overview.py` & `bittensor-4.0.0/bittensor/_cli/commands/overview.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/query.py` & `bittensor-4.0.0/bittensor/_cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/register.py` & `bittensor-4.0.0/bittensor/_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/run.py` & `bittensor-4.0.0/bittensor/_cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/stake.py` & `bittensor-4.0.0/bittensor/_cli/commands/stake.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/transfer.py` & `bittensor-4.0.0/bittensor/_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/unstake.py` & `bittensor-4.0.0/bittensor/_cli/commands/unstake.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,25 +176,14 @@
             assert cli.config.wallet.hotkey is not None
             hotkeys_to_unstake_from = [ (None, bittensor.wallet( config = cli.config ).hotkey.ss58_address) ]
         
         final_hotkeys: List[Tuple[str, str]] = [] 
         final_amounts: List[Union[float, Balance]] = []
         for hotkey in tqdm(hotkeys_to_unstake_from):
             hotkey: Tuple[Optional[str], str] # (hotkey_name (or None), hotkey_ss58)
-            if not subtensor.is_hotkey_registered_any( hotkey_ss58 = hotkey[1] ):
-                # Hotkey is not registered.
-                if (len(hotkeys_to_unstake_from) == 1):
-                    # Only one hotkey, error
-                    bittensor.__console__.print(f"[red]Hotkey [bold]{hotkey[1]}[/bold] is not registered. Aborting.[/red]")
-                    return None
-                else:
-                    # Otherwise, print warning and skip
-                    bittensor.__console__.print(f"[yellow]Hotkey [bold]{hotkey[1]}[/bold] is not registered. Skipping.[/yellow]")
-                    continue
-        
             unstake_amount_tao: float = cli.config.get('amount') # The amount specified to unstake.
             hotkey_stake: Balance = subtensor.get_stake_for_coldkey_and_hotkey( hotkey_ss58 = hotkey[1], coldkey_ss58 = wallet.coldkeypub.ss58_address )
             if unstake_amount_tao == None:
                 unstake_amount_tao = hotkey_stake.tao
             if cli.config.get('max_stake'):
                 # Get the current stake of the hotkey from this coldkey.
                 unstake_amount_tao: float = hotkey_stake.tao - cli.config.get('max_stake')
```

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/utils.py` & `bittensor-4.0.0/bittensor/_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/wallets.py` & `bittensor-4.0.0/bittensor/_cli/commands/wallets.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/commands/weights.py` & `bittensor-4.0.0/bittensor/_cli/commands/weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_cli/naka_cli_impl.py` & `bittensor-4.0.0/bittensor/_cli/naka_cli_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_config/__init__.py` & `bittensor-4.0.0/bittensor/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_config/config_impl.py` & `bittensor-4.0.0/bittensor/_config/config_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_dataset/__init__.py` & `bittensor-4.0.0/bittensor/_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_dataset/dataset_impl.py` & `bittensor-4.0.0/bittensor/_dataset/dataset_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_dataset/dataset_mock.py` & `bittensor-4.0.0/bittensor/_dataset/dataset_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_dataset/thread_queue.py` & `bittensor-4.0.0/bittensor/_dataset/thread_queue.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_dendrite/__init__.py` & `bittensor-4.0.0/bittensor/_dendrite/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_dendrite/dendrite_impl.py` & `bittensor-4.0.0/bittensor/_dendrite/dendrite_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_dendrite/dendrite_mock.py` & `bittensor-4.0.0/bittensor/_dendrite/dendrite_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_dendrite/manager_server.py` & `bittensor-4.0.0/bittensor/_dendrite/manager_server.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_endpoint/__init__.py` & `bittensor-4.0.0/bittensor/_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_endpoint/endpoint_impl.py` & `bittensor-4.0.0/bittensor/_endpoint/endpoint_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_ipfs/ipfs_impl.py` & `bittensor-4.0.0/bittensor/_ipfs/ipfs_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_keyfile/__init__.py` & `bittensor-4.0.0/bittensor/_keyfile/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_keyfile/keyfile_impl.py` & `bittensor-4.0.0/bittensor/_keyfile/keyfile_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_logging/__init__.py` & `bittensor-4.0.0/bittensor/_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_metagraph/__init__.py` & `bittensor-4.0.0/bittensor/_metagraph/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_metagraph/metagraph_impl.py` & `bittensor-4.0.0/bittensor/_metagraph/metagraph_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_metagraph/metagraph_mock.py` & `bittensor-4.0.0/bittensor/_metagraph/metagraph_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_metagraph/naka_metagraph_impl.py` & `bittensor-4.0.0/bittensor/_metagraph/naka_metagraph_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_neuron/__init__.py` & `bittensor-4.0.0/bittensor/_neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_neuron/audio/__init__.py` & `bittensor-4.0.0/bittensor/_neuron/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_neuron/text/__init__.py` & `bittensor-4.0.0/bittensor/_neuron/text/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_neuron/text/core_server/__init__.py` & `bittensor-4.0.0/bittensor/_neuron/text/core_server/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_neuron/text/core_server/nucleus_impl.py` & `bittensor-4.0.0/bittensor/_neuron/text/core_server/nucleus_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_neuron/text/core_validator/__init__.py` & `bittensor-4.0.0/bittensor/_neuron/text/core_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_neuron/text/core_validator/main.py` & `bittensor-4.0.0/bittensor/_neuron/text/core_validator/main.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_neuron/text/log_utilities.py` & `bittensor-4.0.0/bittensor/_neuron/text/log_utilities.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_neuron/text/neuron_utilities.py` & `bittensor-4.0.0/bittensor/_neuron/text/neuron_utilities.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_prometheus/__init__.py` & `bittensor-4.0.0/bittensor/_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_proto/bittensor_pb2.py` & `bittensor-4.0.0/bittensor/_proto/bittensor_pb2.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_proto/bittensor_pb2_grpc.py` & `bittensor-4.0.0/bittensor/_proto/bittensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_receptor/__init__.py` & `bittensor-4.0.0/bittensor/_receptor/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_receptor/receptor_impl.py` & `bittensor-4.0.0/bittensor/_receptor/receptor_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_receptor/receptor_pool_impl.py` & `bittensor-4.0.0/bittensor/_receptor/receptor_pool_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_serializer/__init__.py` & `bittensor-4.0.0/bittensor/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_serializer/serializer_impl.py` & `bittensor-4.0.0/bittensor/_serializer/serializer_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/__init__.py` & `bittensor-4.0.0/bittensor/_subtensor/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/chain_data.py` & `bittensor-4.0.0/bittensor/_subtensor/chain_data.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/errors.py` & `bittensor-4.0.0/bittensor/_subtensor/errors.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/extrinsics/__init__.py` & `bittensor-4.0.0/bittensor/_subtensor/extrinsics/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/extrinsics/delegation.py` & `bittensor-4.0.0/bittensor/_subtensor/extrinsics/delegation.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/extrinsics/prometheus.py` & `bittensor-4.0.0/bittensor/_subtensor/extrinsics/prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/extrinsics/registration.py` & `bittensor-4.0.0/bittensor/_subtensor/extrinsics/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/extrinsics/serving.py` & `bittensor-4.0.0/bittensor/_subtensor/extrinsics/serving.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/extrinsics/set_weights.py` & `bittensor-4.0.0/bittensor/_subtensor/extrinsics/set_weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/extrinsics/staking.py` & `bittensor-4.0.0/bittensor/_subtensor/extrinsics/staking.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/extrinsics/transfer.py` & `bittensor-4.0.0/bittensor/_subtensor/extrinsics/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/extrinsics/unstaking.py` & `bittensor-4.0.0/bittensor/_subtensor/extrinsics/unstaking.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/naka_subtensor_impl.py` & `bittensor-4.0.0/bittensor/_subtensor/naka_subtensor_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/subtensor_impl.py` & `bittensor-4.0.0/bittensor/_subtensor/subtensor_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_subtensor/subtensor_mock.py` & `bittensor-4.0.0/bittensor/_subtensor/subtensor_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_synapse/__init__.py` & `bittensor-4.0.0/bittensor/_synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_synapse/synapse_impl.py` & `bittensor-4.0.0/bittensor/_synapse/synapse_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_synapse/text_causallm_impl.py` & `bittensor-4.0.0/bittensor/_synapse/text_causallm_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_synapse/text_causallmnext_impl.py` & `bittensor-4.0.0/bittensor/_synapse/text_causallmnext_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_synapse/text_lasthiddenstate_impl.py` & `bittensor-4.0.0/bittensor/_synapse/text_lasthiddenstate_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_synapse/text_seq2seq_impl.py` & `bittensor-4.0.0/bittensor/_synapse/text_seq2seq_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_threadpool/__init__.py` & `bittensor-4.0.0/bittensor/_threadpool/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_threadpool/priority_thread_pool_impl.py` & `bittensor-4.0.0/bittensor/_threadpool/priority_thread_pool_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_tokenizer/__init__.py` & `bittensor-4.0.0/bittensor/_tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_wallet/__init__.py` & `bittensor-4.0.0/bittensor/_wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_wallet/naka_wallet_impl.py` & `bittensor-4.0.0/bittensor/_wallet/naka_wallet_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_wallet/wallet_impl.py` & `bittensor-4.0.0/bittensor/_wallet/wallet_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_wallet/wallet_mock.py` & `bittensor-4.0.0/bittensor/_wallet/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/_wandb/__init__.py` & `bittensor-4.0.0/bittensor/_wandb/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/__init__.py` & `bittensor-4.0.0/bittensor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/balance.py` & `bittensor-4.0.0/bittensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/codes.py` & `bittensor-4.0.0/bittensor/utils/codes.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/networking.py` & `bittensor-4.0.0/bittensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/register_cuda.py` & `bittensor-4.0.0/bittensor/utils/register_cuda.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/registration.py` & `bittensor-4.0.0/bittensor/utils/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/registratrion_old.py` & `bittensor-4.0.0/bittensor/utils/registratrion_old.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/stats.py` & `bittensor-4.0.0/bittensor/utils/stats.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/test_utils.py` & `bittensor-4.0.0/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/tokenizer_utils.py` & `bittensor-4.0.0/bittensor/utils/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor/utils/weight_utils.py` & `bittensor-4.0.0/bittensor/utils/weight_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor.egg-info/SOURCES.txt` & `bittensor-4.0.0/bittensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/bittensor.egg-info/requires.txt` & `bittensor-4.0.0/bittensor.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,57 @@
+ansible_vault>=2.1
 argparse==1.4.0
-base58==2.0.1
 backoff==2.1.0
+base58==2.0.1
 certifi==2020.11.8
 cryptography==39.0.0
-idna==2.10
-jinja2==3.0
 fuzzywuzzy==0.18.0
 google-api-python-client==2.6.0
-python-levenshtein==0.12.1
-grpcio==1.42.0
 grpcio-tools==1.42.0
+grpcio==1.42.0
 hypothesis==6.47.4
+idna==2.10
+jinja2==3.0
+jsonschema[format-nongpl]<=4.17.0,>=4.14.0
 loguru==0.6.0
-msgpack==1.0.4
-msgpack-numpy==0.4.7.1
+markupsafe==2.0.1
 miniupnpc==2.0.2
+msgpack-numpy==0.4.7.1
+msgpack==1.0.4
 munch==2.5.0
 nest_asyncio==1.5.6
 netaddr==0.8.0
+numpy==1.21.6
 pandas==1.5.2
-psutil==5.9.4
 password_strength==0.0.3.post2
-protobuf==3.19.5
 prometheus_client==0.14.1
-pycryptodome==3.11.0
-py-sr25519-bindings<1,>=0.1.4
-py-ed25519-bindings<2,>=1.0
+protobuf==3.19.5
+psutil==5.9.4
 py-bip39-bindings<1,>=0.1.9
+py-ed25519-bindings<2,>=1.0
+py-sr25519-bindings<1,>=0.1.4
+pycryptodome==3.11.0
+python-levenshtein==0.12.1
 pyyaml==6.0
-rich==12.5.1
-retry==0.9.2
+qqdm==0.0.7
 requests==2.25.0
+retry==0.9.2
+rich==12.5.1
 scalecodec==1.2.0
 sentencepiece==0.1.97
+substrate-interface==1.5.0
 termcolor==2.1.1
 torch==1.13.1
-transformers==4.20.1
-numpy==1.21.6
-wheel==0.37.1
 tqdm==4.64.1
-qqdm==0.0.7
+transformers==4.20.1
 wandb<0.13.4,>=0.11.1
-ansible_vault>=2.1
-substrate-interface==1.5.0
-jsonschema[format-nongpl]<=4.17.0,>=4.14.0
-markupsafe==2.0.1
+wheel==0.37.1
 
 [dev]
-pytest==7.2.0
-pytest-split==0.8.0
-pytest-xdist==3.0.2
-pytest-rerunfailures==10.2
-coveralls==3.3.1
-pytest-cov==4.0.0
 codecov==2.1.12
+coveralls==3.3.1
 ddt==1.6.0
+pytest-cov==4.0.0
+pytest-rerunfailures==10.2
+pytest-split==0.8.0
+pytest-xdist==3.0.2
+pytest==7.2.0
```

### Comparing `bittensor-3.7.0/setup.py` & `bittensor-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/helpers.py` & `bittensor-4.0.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_cli.py` & `bittensor-4.0.0/tests/integration_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_cli_no_network.py` & `bittensor-4.0.0/tests/integration_tests/test_cli_no_network.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_dataset.py` & `bittensor-4.0.0/tests/integration_tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_dendrite.py` & `bittensor-4.0.0/tests/integration_tests/test_dendrite.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_ipfs.py` & `bittensor-4.0.0/tests/integration_tests/test_ipfs.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_keyfile.py` & `bittensor-4.0.0/tests/integration_tests/test_keyfile.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_metagraph.py` & `bittensor-4.0.0/tests/integration_tests/test_metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_priority_thread_pool.py` & `bittensor-4.0.0/tests/integration_tests/test_priority_thread_pool.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_prometheus.py` & `bittensor-4.0.0/tests/integration_tests/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_server_compression.py` & `bittensor-4.0.0/tests/integration_tests/test_server_compression.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_subtensor.py` & `bittensor-4.0.0/tests/integration_tests/test_subtensor.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/integration_tests/test_wallet.py` & `bittensor-4.0.0/tests/integration_tests/test_wallet.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_axon.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_axon.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_balance.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_config.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_endpoint.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_forward_backward.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_forward_backward.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_metagraph.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_neuron.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_neuron.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_receptor.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_receptor.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_receptor_pool.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_receptor_pool.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_serialization.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_subtensor.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_subtensor.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_synapse.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_wallet.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_wallet.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/test_wandb.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_wandb.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/test_network_utils.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_network_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/test_tokenizer_utils.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/test_utils.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-3.7.0/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py` & `bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py`

 * *Files identical despite different names*

