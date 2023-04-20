# Comparing `tmp/gaboost-1.6.8.tar.gz` & `tmp/gaboost-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaboost-1.6.8.tar", last modified: Wed Mar 29 07:13:51 2023, max compression
+gzip compressed data, was "gaboost-1.6.9.tar", last modified: Thu Apr 20 03:26:07 2023, max compression
```

## Comparing `gaboost-1.6.8.tar` & `gaboost-1.6.9.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.325048 gaboost-1.6.8/
--rw-rw-rw-   0        0        0    11558 2022-08-02 07:14:48.000000 gaboost-1.6.8/LICENSE
--rw-rw-rw-   0        0        0       68 2023-03-29 06:23:28.000000 gaboost-1.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0      811 2023-03-29 07:13:51.324070 gaboost-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0    22983 2023-03-28 12:34:36.000000 gaboost-1.6.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.102463 gaboost-1.6.8/funboost/
--rw-rw-rw-   0        0        0    20775 2023-03-29 02:17:21.000000 gaboost-1.6.8/funboost/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.103440 gaboost-1.6.8/funboost/assist/
--rw-rw-rw-   0        0        0     2858 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/assist/user_custom_broker_register.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.105398 gaboost-1.6.8/funboost/beggar_version_implementation/
--rw-rw-rw-   0        0        0     3930 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/beggar_version_implementation/beggar_redis_consumer.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.122007 gaboost-1.6.8/funboost/concurrent_pool/
--rw-rw-rw-   0        0        0      628 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/concurrent_pool/__init__.py
--rw-rw-rw-   0        0        0     3256 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/concurrent_pool/async_helper.py
--rw-rw-rw-   0        0        0     7227 2023-03-29 02:20:08.000000 gaboost-1.6.8/funboost/concurrent_pool/async_pool_executor.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.126893 gaboost-1.6.8/funboost/concurrent_pool/backup/
--rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/concurrent_pool/backup/__init__.py
--rw-rw-rw-   0        0        0     9548 2023-03-29 02:20:08.000000 gaboost-1.6.8/funboost/concurrent_pool/backup/async_pool_executor0223.py
--rw-rw-rw-   0        0        0     9568 2023-03-29 02:20:08.000000 gaboost-1.6.8/funboost/concurrent_pool/backup/async_pool_executor_back.py
--rw-rw-rw-   0        0        0     5728 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/concurrent_pool/backup/async_pool_executor_janus.py
--rw-rw-rw-   0        0        0     4723 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py
--rw-rw-rw-   0        0        0     3011 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/concurrent_pool/bounded_processpoolexcutor_py36.py
--rw-rw-rw-   0        0        0     1571 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/concurrent_pool/bounded_threadpoolexcutor.py
--rw-rw-rw-   0        0        0     1693 2022-08-02 08:43:39.000000 gaboost-1.6.8/funboost/concurrent_pool/concurrent_pool_with_multi_process.py
--rw-rw-rw-   0        0        0        0 2023-03-28 13:05:23.000000 gaboost-1.6.8/funboost/concurrent_pool/custom_evenlet_pool_executor.py
--rw-rw-rw-   0        0        0        0 2023-03-28 13:05:32.000000 gaboost-1.6.8/funboost/concurrent_pool/custom_gevent_pool_executor.py
--rw-rw-rw-   0        0        0    11273 2022-08-02 08:43:39.000000 gaboost-1.6.8/funboost/concurrent_pool/custom_threadpool_executor.py
--rw-rw-rw-   0        0        0     9317 2022-08-02 08:43:39.000000 gaboost-1.6.8/funboost/concurrent_pool/custom_threadpool_executor000.py
--rw-rw-rw-   0        0        0      373 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/concurrent_pool/single_thread_executor.py
--rw-rw-rw-   0        0        0     5631 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/constant.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.177776 gaboost-1.6.8/funboost/consumers/
--rw-rw-rw-   0        0        0      126 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/__init__.py
--rw-rw-rw-   0        0        0    91580 2023-03-29 02:23:37.000000 gaboost-1.6.8/funboost/consumers/base_consumer.py
--rw-rw-rw-   0        0        0     5644 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/confirm_mixin.py
--rw-rw-rw-   0        0        0     2045 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/http_consumer.py
--rw-rw-rw-   0        0        0     4463 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/http_consumer000.py
--rw-rw-rw-   0        0        0     1058 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/httpsqs_consumer.py
--rw-rw-rw-   0        0        0     3963 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/kafka_consumer.py
--rw-rw-rw-   0        0        0     6640 2022-08-08 08:45:32.000000 gaboost-1.6.8/funboost/consumers/kafka_consumer_manually_commit.py
--rw-rw-rw-   0        0        0     5082 2023-03-29 02:23:37.000000 gaboost-1.6.8/funboost/consumers/kombu_consumer.py
--rw-rw-rw-   0        0        0     1328 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/local_python_queue_consumer.py
--rw-rw-rw-   0        0        0     1069 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/mongomq_consumer.py
--rw-rw-rw-   0        0        0     2208 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/mqtt_consumer.py
--rw-rw-rw-   0        0        0     1054 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/consumers/nats_consumer.py
--rw-rw-rw-   0        0        0     1440 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/nsq_consumer.py
--rw-rw-rw-   0        0        0     1221 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/peewee_conusmer.py
--rw-rw-rw-   0        0        0      982 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/persist_queue_consumer.py
--rw-rw-rw-   0        0        0     1796 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/pulsar_consumer.py
--rw-rw-rw-   0        0        0     1776 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/rabbitmq_amqpstorm_consumer.py
--rw-rw-rw-   0        0        0     5412 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/rabbitmq_pika_consumer.py
--rw-rw-rw-   0        0        0     4653 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/rabbitmq_pika_consumerv0.py
--rw-rw-rw-   0        0        0     1239 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/rabbitmq_rabbitpy_consumer.py
--rw-rw-rw-   0        0        0     3067 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/redis_brpoplpush_consumer.py
--rw-rw-rw-   0        0        0     2843 2023-03-29 02:03:02.000000 gaboost-1.6.8/funboost/consumers/redis_consumer.py
--rw-rw-rw-   0        0        0     4338 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/redis_consumer_ack_able.py
--rw-rw-rw-   0        0        0     1109 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/redis_consumer_simple.py
--rw-rw-rw-   0        0        0     7190 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/redis_filter.py
--rw-rw-rw-   0        0        0     1184 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/redis_pubsub_consumer.py
--rw-rw-rw-   0        0        0     6572 2022-09-01 07:50:53.000000 gaboost-1.6.8/funboost/consumers/redis_stream_consumer.py
--rw-rw-rw-   0        0        0     1633 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/rocketmq_consumer.py
--rw-rw-rw-   0        0        0     1289 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/sqlachemy_consumer.py
--rw-rw-rw-   0        0        0     2025 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/tcp_consumer.py
--rw-rw-rw-   0        0        0     1322 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/txt_file_consumer.py
--rw-rw-rw-   0        0        0     1625 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/udp_consumer.py
--rw-rw-rw-   0        0        0     4137 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/consumers/zeromq_consumer.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.182663 gaboost-1.6.8/funboost/contrib/
--rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/contrib/__init__.py
--rw-rw-rw-   0        0        0     4702 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/contrib/queue2queue.py
--rw-rw-rw-   0        0        0     1817 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/contrib/redis_consume_latest_msg_broker.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.186574 gaboost-1.6.8/funboost/factories/
--rw-rw-rw-   0        0        0      178 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/factories/__init__.py
--rw-rw-rw-   0        0        0     2500 2023-03-28 13:04:26.000000 gaboost-1.6.8/funboost/factories/consumer_factory.py
--rw-rw-rw-   0        0        0     4417 2023-03-28 13:10:00.000000 gaboost-1.6.8/funboost/factories/publisher_factotry.py
--rw-rw-rw-   0        0        0     6670 2023-03-29 02:23:37.000000 gaboost-1.6.8/funboost/funboost_config_deafult.py
--rw-rw-rw-   0        0        0    14118 2023-03-29 07:13:34.000000 gaboost-1.6.8/funboost/helpers.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.229565 gaboost-1.6.8/funboost/publishers/
--rw-rw-rw-   0        0        0      131 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/__init__.py
--rw-rw-rw-   0        0        0    14972 2023-03-29 02:23:37.000000 gaboost-1.6.8/funboost/publishers/base_publisher.py
--rw-rw-rw-   0        0        0     3541 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/confluent_kafka_publisher.py
--rw-rw-rw-   0        0        0      777 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/http_publisher.py
--rw-rw-rw-   0        0        0     2783 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/httpsqs_publisher.py
--rw-rw-rw-   0        0        0     2160 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/kafka_publisher.py
--rw-rw-rw-   0        0        0     4567 2023-03-29 02:23:37.000000 gaboost-1.6.8/funboost/publishers/kombu_publisher.py
--rw-rw-rw-   0        0        0     1365 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/local_python_queue_publisher.py
--rw-rw-rw-   0        0        0     1874 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/mongomq_publisher.py
--rw-rw-rw-   0        0        0     3050 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/mqtt_publisher.py
--rw-rw-rw-   0        0        0     6254 2023-03-29 02:28:13.000000 gaboost-1.6.8/funboost/publishers/msg_result_getter.py
--rw-rw-rw-   0        0        0      776 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/publishers/nats_publisher.py
--rw-rw-rw-   0        0        0     1302 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/nsq_publisher.py
--rw-rw-rw-   0        0        0     1095 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/peewee_publisher.py
--rw-rw-rw-   0        0        0     2540 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/persist_queue_publisher.py
--rw-rw-rw-   0        0        0     1085 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/pulsar_publisher.py
--rw-rw-rw-   0        0        0     2673 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/rabbitmq_amqpstorm_publisher.py
--rw-rw-rw-   0        0        0     2343 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/rabbitmq_pika_publisher.py
--rw-rw-rw-   0        0        0     1953 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/rabbitmq_rabbitpy_publisher.py
--rw-rw-rw-   0        0        0     3950 2023-03-29 02:04:48.000000 gaboost-1.6.8/funboost/publishers/redis_publisher.py
--rw-rw-rw-   0        0        0      278 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/redis_publisher_lpush.py
--rw-rw-rw-   0        0        0      872 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/redis_publisher_simple.py
--rw-rw-rw-   0        0        0      721 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/redis_pubsub_publisher.py
--rw-rw-rw-   0        0        0     2141 2022-09-01 07:50:53.000000 gaboost-1.6.8/funboost/publishers/redis_stream_publisher.py
--rw-rw-rw-   0        0        0     2343 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/rocketmq_publisher.py
--rw-rw-rw-   0        0        0     1215 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/sqla_queue_publisher.py
--rw-rw-rw-   0        0        0     1359 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/tcp_publisher.py
--rw-rw-rw-   0        0        0     1380 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/txt_file_publisher.py
--rw-rw-rw-   0        0        0     1218 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/publishers/udp_publisher.py
--rw-rw-rw-   0        0        0     1002 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/publishers/zeromq_publisher.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.234175 gaboost-1.6.8/funboost/queues/
--rw-rw-rw-   0        0        0        0 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/queues/__init__.py
--rw-rw-rw-   0        0        0     4982 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/queues/peewee_queue.py
--rw-rw-rw-   0        0        0    11186 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/queues/sqla_queue.py
--rw-rw-rw-   0        0        0     9134 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/set_frame_config.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.240039 gaboost-1.6.8/funboost/timing_job/
--rw-rw-rw-   0        0        0     4098 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/timing_job/__init__.py
--rw-rw-rw-   0        0        0      273 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/timing_job/apscheduler_use_mysql_store.py
--rw-rw-rw-   0        0        0      868 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/timing_job/apscheduler_use_redis_store.py
--rw-rw-rw-   0        0        0      996 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/timing_job/push_fun_for_apscheduler_use_db.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.265443 gaboost-1.6.8/funboost/utils/
--rw-rw-rw-   0        0        0     1951 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/__init__.py
--rw-rw-rw-   0        0        0     3124 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/apscheduler_monkey.py
--rw-rw-rw-   0        0        0       96 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/block_exit.py
--rw-rw-rw-   0        0        0    10063 2022-08-09 01:46:39.000000 gaboost-1.6.8/funboost/utils/bulk_operation.py
--rw-rw-rw-   0        0        0     5923 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/custom_pysnooper.py
--rw-rw-rw-   0        0        0    24284 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/decorators.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.267399 gaboost-1.6.8/funboost/utils/dependency_packages/
--rw-rw-rw-   0        0        0        0 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/dependency_packages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.274236 gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/
--rw-rw-rw-   0        0        0      131 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/__init__.py
--rw-rw-rw-   0        0        0     2486 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/lock.py
--rw-rw-rw-   0        0        0     7902 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/mongomq.py
--rw-rw-rw-   0        0        0     7867 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/mongomq0000.py
--rw-rw-rw-   0        0        0     4811 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/test.py
--rw-rw-rw-   0        0        0      377 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.276190 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.277172 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/__pycache__/
--rw-rw-rw-   0        0        0      324 2023-03-29 02:15:53.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-310.pyc
--rw-rw-rw-   0        0        0      341 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.289870 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/
--rw-rw-rw-   0        0        0     1282 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.298665 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/
--rw-rw-rw-   0        0        0     1214 2023-03-29 02:15:56.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0   156125 2023-03-29 02:15:56.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-310.pyc
--rw-rw-rw-   0        0        0      358 2023-03-29 02:15:56.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-310.pyc
--rw-rw-rw-   0        0        0    42622 2023-03-29 02:15:56.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-310.pyc
--rw-rw-rw-   0        0        0     2907 2023-03-29 02:15:56.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-310.pyc
--rw-rw-rw-   0        0        0    10275 2023-03-29 02:15:56.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-310.pyc
--rw-rw-rw-   0        0        0     2053 2023-03-29 02:15:56.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0   187456 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py
--rw-rw-rw-   0        0        0      191 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py
--rw-rw-rw-   0        0        0    63907 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py
--rw-rw-rw-   0        0        0     1682 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py
--rw-rw-rw-   0        0        0    11957 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py
--rw-rw-rw-   0        0        0      442 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/log.py
--rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/py.typed
--rw-rw-rw-   0        0        0      617 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md
--rw-rw-rw-   0        0        0    12865 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py
--rw-rw-rw-   0        0        0     1345 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.305505 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/
--rw-rw-rw-   0        0        0     5379 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py
--rw-rw-rw-   0        0        0      603 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.311367 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/
--rw-rw-rw-   0        0        0     5094 2023-03-29 02:20:11.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-310.pyc
--rw-rw-rw-   0        0        0      775 2023-03-29 02:20:11.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     7995 2023-03-29 02:20:11.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-310.pyc
--rw-rw-rw-   0        0        0     3742 2023-03-29 02:20:11.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-310.pyc
--rw-rw-rw-   0        0        0      315 2023-03-29 02:20:11.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-310.pyc
--rw-rw-rw-   0        0        0     9531 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py
--rw-rw-rw-   0        0        0     4072 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py
--rw-rw-rw-   0        0        0      176 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py
--rw-rw-rw-   0        0        0      287 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py
--rw-rw-rw-   0        0        0      545 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/readme.md
--rw-rw-rw-   0        0        0      251 2022-08-02 08:43:39.000000 gaboost-1.6.8/funboost/utils/develop_log.py
--rw-rw-rw-   0        0        0     2847 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/mongo_util.py
--rw-rw-rw-   0        0        0     7367 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/monkey_color_log.py
--rw-rw-rw-   0        0        0     2882 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/monkey_patches.py
--rw-rw-rw-   0        0        0     3199 2022-08-02 08:43:39.000000 gaboost-1.6.8/funboost/utils/mqtt_util.py
--rw-rw-rw-   0        0        0     4901 2022-08-02 08:43:39.000000 gaboost-1.6.8/funboost/utils/paramiko_util.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.317233 gaboost-1.6.8/funboost/utils/pysnooper_ydf/
--rw-rw-rw-   0        0        0      909 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/pysnooper_ydf/__init__.py
--rw-rw-rw-   0        0        0     2243 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/pysnooper_ydf/pycompat.py
--rw-rw-rw-   0        0        0    19131 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/pysnooper_ydf/tracer.py
--rw-rw-rw-   0        0        0     2753 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/pysnooper_ydf/utils.py
--rw-rw-rw-   0        0        0     3693 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/pysnooper_ydf/variables.py
--rw-rw-rw-   0        0        0     2963 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/rabbitmq_factory.py
--rw-rw-rw-   0        0        0     4844 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/redis_manager.py
--rw-rw-rw-   0        0        0     5532 2023-03-28 12:34:36.000000 gaboost-1.6.8/funboost/utils/resource_monitoring.py
--rw-rw-rw-   0        0        0     1418 2023-03-29 02:20:08.000000 gaboost-1.6.8/funboost/utils/restart_python.py
--rw-rw-rw-   0        0        0     1204 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/simple_data_class.py
--rw-rw-rw-   0        0        0     5407 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/time_util.py
--rw-rw-rw-   0        0        0      408 2022-08-02 07:14:48.000000 gaboost-1.6.8/funboost/utils/un_strict_json_dumps.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:13:51.323093 gaboost-1.6.8/gaboost.egg-info/
--rw-rw-rw-   0        0        0      811 2023-03-29 07:13:50.000000 gaboost-1.6.8/gaboost.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8221 2023-03-29 07:13:51.000000 gaboost-1.6.8/gaboost.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 07:13:50.000000 gaboost-1.6.8/gaboost.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      319 2023-03-29 07:13:50.000000 gaboost-1.6.8/gaboost.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-29 07:13:50.000000 gaboost-1.6.8/gaboost.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 07:13:51.325048 gaboost-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     4000 2023-03-29 07:13:46.000000 gaboost-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.485848 gaboost-1.6.9/
+-rw-rw-rw-   0        0        0    11558 2022-08-02 07:14:48.000000 gaboost-1.6.9/LICENSE
+-rw-rw-rw-   0        0        0       68 2023-03-29 06:23:28.000000 gaboost-1.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      811 2023-04-20 03:26:07.484870 gaboost-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0    22066 2023-04-20 03:18:22.000000 gaboost-1.6.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.253472 gaboost-1.6.9/funboost/
+-rw-rw-rw-   0        0        0    20805 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.254449 gaboost-1.6.9/funboost/assist/
+-rw-rw-rw-   0        0        0     2858 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/assist/user_custom_broker_register.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.255425 gaboost-1.6.9/funboost/beggar_version_implementation/
+-rw-rw-rw-   0        0        0     3930 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/beggar_version_implementation/beggar_redis_consumer.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.269150 gaboost-1.6.9/funboost/concurrent_pool/
+-rw-rw-rw-   0        0        0      628 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/concurrent_pool/__init__.py
+-rw-rw-rw-   0        0        0     3256 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/concurrent_pool/async_helper.py
+-rw-rw-rw-   0        0        0     7227 2023-03-29 02:20:08.000000 gaboost-1.6.9/funboost/concurrent_pool/async_pool_executor.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.274026 gaboost-1.6.9/funboost/concurrent_pool/backup/
+-rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/concurrent_pool/backup/__init__.py
+-rw-rw-rw-   0        0        0     9548 2023-03-29 02:20:08.000000 gaboost-1.6.9/funboost/concurrent_pool/backup/async_pool_executor0223.py
+-rw-rw-rw-   0        0        0     9568 2023-03-29 02:20:08.000000 gaboost-1.6.9/funboost/concurrent_pool/backup/async_pool_executor_back.py
+-rw-rw-rw-   0        0        0     5728 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/concurrent_pool/backup/async_pool_executor_janus.py
+-rw-rw-rw-   0        0        0     4723 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py
+-rw-rw-rw-   0        0        0     3011 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/concurrent_pool/bounded_processpoolexcutor_py36.py
+-rw-rw-rw-   0        0        0     1571 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/concurrent_pool/bounded_threadpoolexcutor.py
+-rw-rw-rw-   0        0        0     1693 2022-08-02 08:43:39.000000 gaboost-1.6.9/funboost/concurrent_pool/concurrent_pool_with_multi_process.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 13:05:23.000000 gaboost-1.6.9/funboost/concurrent_pool/custom_evenlet_pool_executor.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 13:05:32.000000 gaboost-1.6.9/funboost/concurrent_pool/custom_gevent_pool_executor.py
+-rw-rw-rw-   0        0        0    11273 2022-08-02 08:43:39.000000 gaboost-1.6.9/funboost/concurrent_pool/custom_threadpool_executor.py
+-rw-rw-rw-   0        0        0     9317 2022-08-02 08:43:39.000000 gaboost-1.6.9/funboost/concurrent_pool/custom_threadpool_executor000.py
+-rw-rw-rw-   0        0        0      373 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/concurrent_pool/single_thread_executor.py
+-rw-rw-rw-   0        0        0     5631 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/constant.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.317056 gaboost-1.6.9/funboost/consumers/
+-rw-rw-rw-   0        0        0      126 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/__init__.py
+-rw-rw-rw-   0        0        0    91581 2023-04-20 03:21:25.000000 gaboost-1.6.9/funboost/consumers/base_consumer.py
+-rw-rw-rw-   0        0        0     5877 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/consumers/confirm_mixin.py
+-rw-rw-rw-   0        0        0     2045 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/http_consumer.py
+-rw-rw-rw-   0        0        0     4463 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/http_consumer000.py
+-rw-rw-rw-   0        0        0     1058 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/httpsqs_consumer.py
+-rw-rw-rw-   0        0        0     4295 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/consumers/kafka_consumer.py
+-rw-rw-rw-   0        0        0     6640 2022-08-08 08:45:32.000000 gaboost-1.6.9/funboost/consumers/kafka_consumer_manually_commit.py
+-rw-rw-rw-   0        0        0     5082 2023-03-29 02:23:37.000000 gaboost-1.6.9/funboost/consumers/kombu_consumer.py
+-rw-rw-rw-   0        0        0     1328 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/local_python_queue_consumer.py
+-rw-rw-rw-   0        0        0     1069 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/mongomq_consumer.py
+-rw-rw-rw-   0        0        0     2208 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/mqtt_consumer.py
+-rw-rw-rw-   0        0        0     1054 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/consumers/nats_consumer.py
+-rw-rw-rw-   0        0        0     1440 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/nsq_consumer.py
+-rw-rw-rw-   0        0        0     1218 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/consumers/peewee_conusmer.py
+-rw-rw-rw-   0        0        0      982 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/persist_queue_consumer.py
+-rw-rw-rw-   0        0        0     1791 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/consumers/pulsar_consumer.py
+-rw-rw-rw-   0        0        0     1776 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/rabbitmq_amqpstorm_consumer.py
+-rw-rw-rw-   0        0        0     5412 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/rabbitmq_pika_consumer.py
+-rw-rw-rw-   0        0        0     4653 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/rabbitmq_pika_consumerv0.py
+-rw-rw-rw-   0        0        0     1239 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/rabbitmq_rabbitpy_consumer.py
+-rw-rw-rw-   0        0        0     3067 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/redis_brpoplpush_consumer.py
+-rw-rw-rw-   0        0        0     2843 2023-03-29 02:03:02.000000 gaboost-1.6.9/funboost/consumers/redis_consumer.py
+-rw-rw-rw-   0        0        0     4338 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/redis_consumer_ack_able.py
+-rw-rw-rw-   0        0        0     1109 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/redis_consumer_simple.py
+-rw-rw-rw-   0        0        0     7190 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/redis_filter.py
+-rw-rw-rw-   0        0        0     1184 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/redis_pubsub_consumer.py
+-rw-rw-rw-   0        0        0     6572 2022-09-01 07:50:53.000000 gaboost-1.6.9/funboost/consumers/redis_stream_consumer.py
+-rw-rw-rw-   0        0        0     1633 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/rocketmq_consumer.py
+-rw-rw-rw-   0        0        0     1289 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/sqlachemy_consumer.py
+-rw-rw-rw-   0        0        0     2025 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/tcp_consumer.py
+-rw-rw-rw-   0        0        0     1322 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/txt_file_consumer.py
+-rw-rw-rw-   0        0        0     1625 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/udp_consumer.py
+-rw-rw-rw-   0        0        0     4137 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/consumers/zeromq_consumer.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.319986 gaboost-1.6.9/funboost/contrib/
+-rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/contrib/__init__.py
+-rw-rw-rw-   0        0        0     4703 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/contrib/queue2queue.py
+-rw-rw-rw-   0        0        0     1817 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/contrib/redis_consume_latest_msg_broker.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.324884 gaboost-1.6.9/funboost/factories/
+-rw-rw-rw-   0        0        0      178 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/factories/__init__.py
+-rw-rw-rw-   0        0        0     2500 2023-03-28 13:04:26.000000 gaboost-1.6.9/funboost/factories/consumer_factory.py
+-rw-rw-rw-   0        0        0     4417 2023-03-28 13:10:00.000000 gaboost-1.6.9/funboost/factories/publisher_factotry.py
+-rw-rw-rw-   0        0        0     6684 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/funboost_config_deafult.py
+-rw-rw-rw-   0        0        0    14118 2023-04-20 03:21:07.000000 gaboost-1.6.9/funboost/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.367562 gaboost-1.6.9/funboost/publishers/
+-rw-rw-rw-   0        0        0      131 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/__init__.py
+-rw-rw-rw-   0        0        0    14972 2023-04-20 03:20:54.000000 gaboost-1.6.9/funboost/publishers/base_publisher.py
+-rw-rw-rw-   0        0        0     3541 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/confluent_kafka_publisher.py
+-rw-rw-rw-   0        0        0      777 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/http_publisher.py
+-rw-rw-rw-   0        0        0     2783 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/httpsqs_publisher.py
+-rw-rw-rw-   0        0        0     2160 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/publishers/kafka_publisher.py
+-rw-rw-rw-   0        0        0     4567 2023-03-29 02:23:37.000000 gaboost-1.6.9/funboost/publishers/kombu_publisher.py
+-rw-rw-rw-   0        0        0     1365 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/local_python_queue_publisher.py
+-rw-rw-rw-   0        0        0     1874 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/mongomq_publisher.py
+-rw-rw-rw-   0        0        0     3050 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/mqtt_publisher.py
+-rw-rw-rw-   0        0        0     7875 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/publishers/msg_result_getter.py
+-rw-rw-rw-   0        0        0      776 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/publishers/nats_publisher.py
+-rw-rw-rw-   0        0        0     1302 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/nsq_publisher.py
+-rw-rw-rw-   0        0        0     1095 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/peewee_publisher.py
+-rw-rw-rw-   0        0        0     2540 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/persist_queue_publisher.py
+-rw-rw-rw-   0        0        0     1085 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/pulsar_publisher.py
+-rw-rw-rw-   0        0        0     2687 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/publishers/rabbitmq_amqpstorm_publisher.py
+-rw-rw-rw-   0        0        0     2343 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/rabbitmq_pika_publisher.py
+-rw-rw-rw-   0        0        0     1953 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/rabbitmq_rabbitpy_publisher.py
+-rw-rw-rw-   0        0        0     3950 2023-03-29 02:04:48.000000 gaboost-1.6.9/funboost/publishers/redis_publisher.py
+-rw-rw-rw-   0        0        0      278 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/redis_publisher_lpush.py
+-rw-rw-rw-   0        0        0      872 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/redis_publisher_simple.py
+-rw-rw-rw-   0        0        0      721 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/redis_pubsub_publisher.py
+-rw-rw-rw-   0        0        0     2141 2022-09-01 07:50:53.000000 gaboost-1.6.9/funboost/publishers/redis_stream_publisher.py
+-rw-rw-rw-   0        0        0     2343 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/rocketmq_publisher.py
+-rw-rw-rw-   0        0        0     1215 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/sqla_queue_publisher.py
+-rw-rw-rw-   0        0        0     1359 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/tcp_publisher.py
+-rw-rw-rw-   0        0        0     1380 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/txt_file_publisher.py
+-rw-rw-rw-   0        0        0     1218 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/publishers/udp_publisher.py
+-rw-rw-rw-   0        0        0     1002 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/publishers/zeromq_publisher.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.372446 gaboost-1.6.9/funboost/queues/
+-rw-rw-rw-   0        0        0        0 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/queues/__init__.py
+-rw-rw-rw-   0        0        0     4982 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/queues/peewee_queue.py
+-rw-rw-rw-   0        0        0    11186 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/queues/sqla_queue.py
+-rw-rw-rw-   0        0        0     9134 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/set_frame_config.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.377323 gaboost-1.6.9/funboost/timing_job/
+-rw-rw-rw-   0        0        0     4098 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/timing_job/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/timing_job/apscheduler_use_mysql_store.py
+-rw-rw-rw-   0        0        0      868 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/timing_job/apscheduler_use_redis_store.py
+-rw-rw-rw-   0        0        0      996 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/timing_job/push_fun_for_apscheduler_use_db.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.406453 gaboost-1.6.9/funboost/utils/
+-rw-rw-rw-   0        0        0     1951 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/__init__.py
+-rw-rw-rw-   0        0        0     3124 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/apscheduler_monkey.py
+-rw-rw-rw-   0        0        0       96 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/block_exit.py
+-rw-rw-rw-   0        0        0    10063 2022-08-09 01:46:39.000000 gaboost-1.6.9/funboost/utils/bulk_operation.py
+-rw-rw-rw-   0        0        0     5923 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/custom_pysnooper.py
+-rw-rw-rw-   0        0        0    24284 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/decorators.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.408516 gaboost-1.6.9/funboost/utils/dependency_packages/
+-rw-rw-rw-   0        0        0        0 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/dependency_packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.418297 gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/
+-rw-rw-rw-   0        0        0      131 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/__init__.py
+-rw-rw-rw-   0        0        0     2486 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/lock.py
+-rw-rw-rw-   0        0        0     7902 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/mongomq.py
+-rw-rw-rw-   0        0        0     7867 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/mongomq0000.py
+-rw-rw-rw-   0        0        0     4811 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/test.py
+-rw-rw-rw-   0        0        0      377 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.421225 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.422198 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/__pycache__/
+-rw-rw-rw-   0        0        0      324 2023-03-29 02:15:53.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-310.pyc
+-rw-rw-rw-   0        0        0      341 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.441487 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/
+-rw-rw-rw-   0        0        0     1282 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.453368 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/
+-rw-rw-rw-   0        0        0     1214 2023-03-29 02:15:56.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0   156125 2023-03-29 02:15:56.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-310.pyc
+-rw-rw-rw-   0        0        0      358 2023-03-29 02:15:56.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-310.pyc
+-rw-rw-rw-   0        0        0    42622 2023-03-29 02:15:56.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2907 2023-03-29 02:15:56.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-310.pyc
+-rw-rw-rw-   0        0        0    10275 2023-03-29 02:15:56.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2053 2023-03-29 02:15:56.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0   187456 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py
+-rw-rw-rw-   0        0        0      191 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py
+-rw-rw-rw-   0        0        0    63907 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py
+-rw-rw-rw-   0        0        0     1682 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py
+-rw-rw-rw-   0        0        0    11957 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py
+-rw-rw-rw-   0        0        0      442 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/log.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/py.typed
+-rw-rw-rw-   0        0        0      617 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md
+-rw-rw-rw-   0        0        0    12865 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py
+-rw-rw-rw-   0        0        0     1345 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.462154 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/
+-rw-rw-rw-   0        0        0     5379 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py
+-rw-rw-rw-   0        0        0      603 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.470968 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/
+-rw-rw-rw-   0        0        0     5094 2023-03-29 02:20:11.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-310.pyc
+-rw-rw-rw-   0        0        0      775 2023-03-29 02:20:11.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7995 2023-03-29 02:20:11.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3742 2023-03-29 02:20:11.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-310.pyc
+-rw-rw-rw-   0        0        0      315 2023-03-29 02:20:11.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9531 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py
+-rw-rw-rw-   0        0        0     4072 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py
+-rw-rw-rw-   0        0        0      176 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py
+-rw-rw-rw-   0        0        0      287 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py
+-rw-rw-rw-   0        0        0      545 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/readme.md
+-rw-rw-rw-   0        0        0      251 2022-08-02 08:43:39.000000 gaboost-1.6.9/funboost/utils/develop_log.py
+-rw-rw-rw-   0        0        0     2984 2023-04-20 03:18:22.000000 gaboost-1.6.9/funboost/utils/mongo_util.py
+-rw-rw-rw-   0        0        0     7367 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/monkey_color_log.py
+-rw-rw-rw-   0        0        0     2882 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/monkey_patches.py
+-rw-rw-rw-   0        0        0     3199 2022-08-02 08:43:39.000000 gaboost-1.6.9/funboost/utils/mqtt_util.py
+-rw-rw-rw-   0        0        0     4901 2022-08-02 08:43:39.000000 gaboost-1.6.9/funboost/utils/paramiko_util.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.476831 gaboost-1.6.9/funboost/utils/pysnooper_ydf/
+-rw-rw-rw-   0        0        0      909 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/pysnooper_ydf/__init__.py
+-rw-rw-rw-   0        0        0     2243 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/pysnooper_ydf/pycompat.py
+-rw-rw-rw-   0        0        0    19131 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/pysnooper_ydf/tracer.py
+-rw-rw-rw-   0        0        0     2753 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/pysnooper_ydf/utils.py
+-rw-rw-rw-   0        0        0     3693 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/pysnooper_ydf/variables.py
+-rw-rw-rw-   0        0        0     2963 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/rabbitmq_factory.py
+-rw-rw-rw-   0        0        0     4844 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/redis_manager.py
+-rw-rw-rw-   0        0        0     5532 2023-03-28 12:34:36.000000 gaboost-1.6.9/funboost/utils/resource_monitoring.py
+-rw-rw-rw-   0        0        0     1418 2023-03-29 02:20:08.000000 gaboost-1.6.9/funboost/utils/restart_python.py
+-rw-rw-rw-   0        0        0     1204 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/simple_data_class.py
+-rw-rw-rw-   0        0        0     5407 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/time_util.py
+-rw-rw-rw-   0        0        0      408 2022-08-02 07:14:48.000000 gaboost-1.6.9/funboost/utils/un_strict_json_dumps.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:26:07.483899 gaboost-1.6.9/gaboost.egg-info/
+-rw-rw-rw-   0        0        0      811 2023-04-20 03:26:07.000000 gaboost-1.6.9/gaboost.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8221 2023-04-20 03:26:07.000000 gaboost-1.6.9/gaboost.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 03:26:07.000000 gaboost-1.6.9/gaboost.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      319 2023-04-20 03:26:07.000000 gaboost-1.6.9/gaboost.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 03:26:07.000000 gaboost-1.6.9/gaboost.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 03:26:07.485848 gaboost-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     4000 2023-04-20 03:25:33.000000 gaboost-1.6.9/setup.py
```

### Comparing `gaboost-1.6.8/LICENSE` & `gaboost-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/PKG-INFO` & `gaboost-1.6.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaboost
-Version: 1.6.8
+Version: 1.6.9
 Summary: fork funboost
 Author: ziko
 License: BSD License
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `gaboost-1.6.8/README.md` & `gaboost-1.6.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
 
 ## 1.0 github地址和文档地址
 
 ### 1.0.1 [分布式函数调度框架文档地址](https://funboost.readthedocs.io/zh/latest/index.html)
 [查看分布式函数调度框架文档](https://funboost.readthedocs.io/zh/latest/index.html)
 
+[funboost依赖的nb_log日志文档](https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2)
+
 ```
 文档很长，但归根结底只需要学习 1.3 里面的这1个例子就行，主要是修改下@boost的各种参数，
 通过不同的入参，实践测试下各种控制功能。
 
 对比 celery 有20种改善，其中之一是无依赖文件夹层级和文件夹名字 文件名字。
 首先能把  https://github.com/ydf0509/celery_demo
 这个例子的已经写好的不规则目录层级和文件名字的函数用celery框架玩起来，才能说是了解celery，
@@ -60,33 +62,21 @@
 [//]: # (现在新建一个qq群 189603256)
 
 [//]:# ([点击加入 python万能分布式函数调度框架qq群]&#40;https://qm.qq.com/cgi-bin/qm/qr?k=unA_o_L3sv5yushJzYGUTAwSzZ7GhUhq&jump_from=webapi&#41;)
 
 
 ### 1.0.3 funboost 框架 和 function_scheduling_distributed_framework 框架 关系说明
 
-<p style="color: crimson;font-size: larger">funboost框架取名说明:</p>
-<pre style="color: darkorchid ;font-size:medium">
-funboost是function_scheduling_distributed_framework框架的新名字,把框架名字长度减小.
-funboost名字是两个单词,fun是function指的是python函数,boost是加速的意思,合一起是加速函数并发运行.
-</pre>
-
-<p style="color: crimson;font-size: larger">两个框架的兼容性说明:</p>
-<pre style="color: darkorchid;font-size:medium">
-funboost 和 function_scheduling_distributed_framework 项目的代码一模一样,以后新代码只更新funboost项目。
-from funboost import xx 和  from function_scheduling_distributed_framework import xx 是完全一模一样的.
-boost是task_deco的别名，两个都可以使用。在消费函数上写@boost 和 @task_deco是一模一样的，两个都可以使用。
-所以在有的文档或者截图中如果写 
-from  function_scheduling_distributed_framework import task_deco , @task_deco
-用户需要知道效果和from funboost import boost , @boost 是一模一样的。兼容性100%
-</pre>
+```
+funboost 是 function_scheduling_distributed_framework的包名更新版本
+```
 
 
 
-<span style="font-size:25px">旧框架地址：<span><a href="https://github.com/ydf0509/distributed_framework" style="font-size: 25px">function_scheduling_distributed_framework框架地址链接</a>
+<span style="font-size:15px">旧框架地址：<span><a href="https://github.com/ydf0509/distributed_framework" style="font-size: 15px">function_scheduling_distributed_framework框架地址链接</a>
 
 
 ## 1.1 安装方式
 
 pip install funboost --upgrade
```

### Comparing `gaboost-1.6.8/funboost/__init__.py` & `gaboost-1.6.9/funboost/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from funboost.utils.paramiko_util import ParamikoFolderUploader
 from funboost.consumers.base_consumer import (ExceptionForRequeue, ExceptionForRetry, ExceptionForPushToDlxqueue,
                                               AbstractConsumer, ConsumersManager,
                                               FunctionResultStatusPersistanceConfig,
                                               wait_for_possible_has_finish_all_tasks_by_conusmer_list,
                                               ActiveCousumerProcessInfoGetter, FunctionResultStatus)
 from funboost.publishers.base_publisher import (PriorityConsumingControlConfig,
-                                                AbstractPublisher, AsyncResult, HasNotAsyncResult, AioAsyncResult)
+                                                AbstractPublisher, AsyncResult, HasNotAsyncResult, AioAsyncResult,ResultFromMongo)
 from funboost.factories.publisher_factotry import get_publisher
 from funboost.factories.consumer_factory import get_consumer
 
 # noinspection PyUnresolvedReferences
 from funboost.utils import nb_print, patch_print, LogManager, get_logger, LoggerMixin
 from funboost.timing_job import fsdf_background_scheduler, timing_publish_deco
 from funboost.constant import BrokerEnum, ConcurrentModeEnum
@@ -217,15 +217,15 @@
     :param user_custom_record_process_info_func  提供一个用户自定义的保存消息处理记录到某个地方例如mysql数据库的函数，函数仅仅接受一个入参，入参类型是 FunctionResultStatus，用户可以打印参数
     :param is_using_rpc_mode 是否使用rpc模式，可以在发布端获取消费端的结果回调，但消耗一定性能，使用async_result.result时候会等待阻塞住当前线程。。
     :param broker_exclusive_config 加上一个不同种类中间件非通用的配置,不同中间件自身独有的配置，不是所有中间件都兼容的配置，因为框架支持30种消息队列，消息队列不仅仅是一般的先进先出queue这么简单的概念，
             例如kafka支持消费者组，rabbitmq也支持各种独特概念例如各种ack机制 复杂路由机制，每一种消息队列都有独特的配置参数意义，可以通过这里传递。
     :param broker_kind:中间件种类，支持30种消息队列。 入参见 BrokerEnum枚举类的属性。
     :param boost_decorator_default_params: oostDecoratorDefaultParams是
             @boost装饰器默认的全局入参。如果boost没有亲自指定某个入参，就自动使用funboost_config.py的BoostDecoratorDefaultParams中的配置。
-            除非你嫌弃每个 boost 装饰器相同入参太多了，可以在 funboost_config.py 文件中设置boost装饰器的全局默认值。
+                    如果你嫌弃每个 boost 装饰器相同入参太多重复了，可以在 funboost_config.py 文件中设置boost装饰器的全局默认值。
             BoostDecoratorDefaultParams() 实例化时候也可以传递这个boost装饰器任何的入参，BoostDecoratorDefaultParams是个数据类，百度python3.7dataclass的概念，类似。
 
             funboost.funboost_config_deafult.BoostDecoratorDefaultParams 的值会自动被你项目根目录下的funboost_config.BoostDecoratorDefaultParams的值覆盖
     """
 
     """
     这是此框架最重要的一个函数，必须看懂里面的入参有哪些。
```

### Comparing `gaboost-1.6.8/funboost/assist/user_custom_broker_register.py` & `gaboost-1.6.9/funboost/assist/user_custom_broker_register.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/beggar_version_implementation/beggar_redis_consumer.py` & `gaboost-1.6.9/funboost/beggar_version_implementation/beggar_redis_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/__init__.py` & `gaboost-1.6.9/funboost/concurrent_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/async_helper.py` & `gaboost-1.6.9/funboost/concurrent_pool/async_helper.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/async_pool_executor.py` & `gaboost-1.6.9/funboost/concurrent_pool/async_pool_executor.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/backup/async_pool_executor0223.py` & `gaboost-1.6.9/funboost/concurrent_pool/backup/async_pool_executor0223.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/backup/async_pool_executor_back.py` & `gaboost-1.6.9/funboost/concurrent_pool/backup/async_pool_executor_back.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/backup/async_pool_executor_janus.py` & `gaboost-1.6.9/funboost/concurrent_pool/backup/async_pool_executor_janus.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py` & `gaboost-1.6.9/funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/bounded_processpoolexcutor_py36.py` & `gaboost-1.6.9/funboost/concurrent_pool/bounded_processpoolexcutor_py36.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/bounded_threadpoolexcutor.py` & `gaboost-1.6.9/funboost/concurrent_pool/bounded_threadpoolexcutor.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/concurrent_pool_with_multi_process.py` & `gaboost-1.6.9/funboost/concurrent_pool/concurrent_pool_with_multi_process.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/custom_threadpool_executor.py` & `gaboost-1.6.9/funboost/concurrent_pool/custom_threadpool_executor.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/concurrent_pool/custom_threadpool_executor000.py` & `gaboost-1.6.9/funboost/concurrent_pool/custom_threadpool_executor000.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/constant.py` & `gaboost-1.6.9/funboost/constant.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/base_consumer.py` & `gaboost-1.6.9/funboost/consumers/base_consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1025,15 +1025,15 @@
                 function_only_params):  # 对函数的参数进行检查，过滤已经执行过并且成功的任务。
             self.logger.warning(f'redis的 [{self._redis_filter_key_name}] 键 中 过滤任务 {kw["body"]}')
             self._confirm_consume(kw)
             return
         publish_time = _get_publish_time(kw['body'])
         msg_expire_senconds_priority = self._get_priority_conf(kw, 'msg_expire_senconds')
         dis = round(time.time() - publish_time, 4)
-        if msg_expire_senconds_priority and dis > 5:
+        if msg_expire_senconds_priority and dis > 20:
             self.alert.info(f'延时报警：{self.queue_name} 消息发布时间距离现在 {dis} 秒,请检查服务器状态')
         if msg_expire_senconds_priority and dis > msg_expire_senconds_priority:
             self.logger.warning(
                 f'消息发布时戳是 {publish_time} {kw["body"].get("publish_time_format", "")},距离现在 {dis} 秒 ,'
                 f'超过了指定的 {msg_expire_senconds_priority} 秒，丢弃任务')
             self._confirm_consume(kw)
             return 0
```

### Comparing `gaboost-1.6.8/funboost/consumers/confirm_mixin.py` & `gaboost-1.6.9/funboost/consumers/confirm_mixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,21 +70,24 @@
         with decorators.RedisDistributedLockContextManager(self.redis_db_frame, lock_key, ).set_log_level(30) as lock:
             if lock.has_aquire_lock:
                 self._distributed_consumer_statistics.send_heartbeat()
                 current_queue_hearbeat_ids = self._distributed_consumer_statistics.get_queue_heartbeat_ids(without_time=True)
                 current_queue_unacked_msg_queues = self.redis_db_frame.scan(0, f'{self._queue_name}__unack_id_*', self.SCAN_COUNT) # 不要在funboost的队列所在db放弃他缓存keys，要保持db的keys少于1000，否则要多次scan。
                 # print(current_queue_unacked_msg_queues)
                 for current_queue_unacked_msg_queue in current_queue_unacked_msg_queues[1]:
-                    current_queue_unacked_msg_queue_str = current_queue_unacked_msg_queue.decode()
+                    current_queue_unacked_msg_queue_name = current_queue_unacked_msg_queue.decode()
                     if time.time() - self._last_show_unacked_msg_num_log > 600:
-                        self.logger.info(f'{current_queue_unacked_msg_queue_str} 中有待确认消费任务的数量是'
-                                         f' {self.redis_db_frame.zcard(current_queue_unacked_msg_queue_str)}')
+                        self.logger.info(f'{current_queue_unacked_msg_queue_name} 中有待确认消费任务的数量是'
+                                         f' {self.redis_db_frame.zcard(current_queue_unacked_msg_queue_name)}')
                         self._last_show_unacked_msg_num_log = time.time()
-                    if current_queue_unacked_msg_queue_str.split(f'{self._queue_name}__unack_id_')[1] not in current_queue_hearbeat_ids:
-                        self.logger.warning(f'{current_queue_unacked_msg_queue_str} 是掉线或关闭消费者的')
-                        for unacked_task_str in self.redis_db_frame.zrevrange(current_queue_unacked_msg_queue_str, 0, 1000):
-                            self.logger.warning(f'从 {current_queue_unacked_msg_queue_str} 向 {self._queue_name} 重新放入掉线消费者未消费确认的任务 {unacked_task_str.decode()}')
-                            self.redis_db_frame.lpush(self._queue_name, unacked_task_str)
-                            self.redis_db_frame.zrem(current_queue_unacked_msg_queue_str, unacked_task_str)
+                    if current_queue_unacked_msg_queue_name.split(f'{self._queue_name}__unack_id_')[1] not in current_queue_hearbeat_ids:
+                        self.logger.warning(f'{current_queue_unacked_msg_queue_name} 是掉线或关闭消费者的')
+                        while 1:
+                            if self.redis_db_frame.exists(current_queue_unacked_msg_queue_name):
+                                for unacked_task_str in self.redis_db_frame.zrevrange(current_queue_unacked_msg_queue_name, 0, 1000):
+                                    self.logger.warning(f'从 {current_queue_unacked_msg_queue_name} 向 {self._queue_name} 重新放入掉线消费者未消费确认的任务'
+                                                        f' {unacked_task_str.decode()}')
+                                    self.redis_db_frame.lpush(self._queue_name, unacked_task_str)
+                                    self.redis_db_frame.zrem(current_queue_unacked_msg_queue_name, unacked_task_str)
                     else:
                         pass
                         # print('是活跃消费者')
```

### Comparing `gaboost-1.6.8/funboost/consumers/http_consumer.py` & `gaboost-1.6.9/funboost/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/http_consumer000.py` & `gaboost-1.6.9/funboost/consumers/http_consumer000.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/httpsqs_consumer.py` & `gaboost-1.6.9/funboost/consumers/httpsqs_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/kafka_consumer.py` & `gaboost-1.6.9/funboost/consumers/kafka_consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,29 +10,36 @@
 from kafka.errors import TopicAlreadyExistsError
 
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
 from ga_log import get_logger, LogManager
 
 # LogManager('kafka').get_logger_and_add_handlers(30)
-get_logger('kafka', log_level_int=20)
+get_logger('kafka', log_level_int=30)
 
 
 class KafkaConsumer(AbstractConsumer):
     """
     kafka作为中间件实现的。自动确认消费，最多消费一次，随意重启会丢失正在大批正在运行的任务。推荐使用 confluent_kafka 中间件，kafka_consumer_manually_commit.py。
 
     可以让消费函数内部 sleep60秒，突然停止消费代码，使用 kafka-consumer-groups.sh --bootstrap-server 127.0.0.1:9092 --describe --group funboost 来证实自动确认消费和手动确认消费的区别。
     """
     BROKER_KIND = 8
     KAFKA_GROUP_ID = 'funboost_kafka'
     AUTO_OFFSET_RESET = 'earliest'
 
     BROKER_EXCLUSIVE_CONFIG_KEYS = ['group_id','auto_offset_reset']
     # not_all_brokers_general_settings配置 ，支持独立的中间件配置参数是 group_id 和 auto_offset_reset
+    """
+    auto_offset_reset 介绍
+      auto_offset_reset (str): A policy for resetting offsets on
+            OffsetOutOfRange errors: 'earliest' will move to the oldest
+            available message, 'latest' will move to the most recent. Any
+            other value will raise the exception. Default: 'latest'.
+    """
 
     def _shedual_task(self):
         try:
             admin_client = KafkaAdminClient(bootstrap_servers=funboost_config_deafult.KAFKA_BOOTSTRAP_SERVERS)
             admin_client.create_topics([NewTopic(self._queue_name, 10, 1)])
             # admin_client.create_partitions({self._queue_name: NewPartitions(total_count=16)})
         except TopicAlreadyExistsError:
```

### Comparing `gaboost-1.6.8/funboost/consumers/kafka_consumer_manually_commit.py` & `gaboost-1.6.9/funboost/consumers/kafka_consumer_manually_commit.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/kombu_consumer.py` & `gaboost-1.6.9/funboost/consumers/kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/local_python_queue_consumer.py` & `gaboost-1.6.9/funboost/consumers/local_python_queue_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/mongomq_consumer.py` & `gaboost-1.6.9/funboost/consumers/mongomq_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/mqtt_consumer.py` & `gaboost-1.6.9/funboost/consumers/mqtt_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/nats_consumer.py` & `gaboost-1.6.9/funboost/consumers/nats_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/nsq_consumer.py` & `gaboost-1.6.9/funboost/consumers/nsq_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/peewee_conusmer.py` & `gaboost-1.6.9/funboost/consumers/peewee_conusmer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from funboost import funboost_config_deafult
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.queues.peewee_queue import PeeweeQueue,TaskStatus
 
 
 class PeeweeConsumer(AbstractConsumer):
     """
-    sqlachemy实现的操作5种数据库模拟消息队列，支持消费确认。
+    peewee实现的操作5种数据库模拟消息队列，支持消费确认。
     """
     BROKER_KIND = 26
 
     def _shedual_task(self):
         self.queue = PeeweeQueue(self.queue_name)
         while True:
             task_dict = self.queue.get()
```

### Comparing `gaboost-1.6.8/funboost/consumers/persist_queue_consumer.py` & `gaboost-1.6.9/funboost/consumers/persist_queue_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/pulsar_consumer.py` & `gaboost-1.6.9/funboost/consumers/pulsar_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 class PulsarConsumer(AbstractConsumer, ):
     """
     pulsar作为中间件实现的。
     """
     BROKER_KIND = 20
     BROKER_EXCLUSIVE_CONFIG_KEYS = ['subscription_name']
-    SUBSCRIPTION_NAME = 'funboost_subc'
+    SUBSCRIPTION_NAME = 'funboost'
 
     def custom_init(self):
         try:
             import pulsar  # 需要用户自己 pip install pulsar-client ，目前20221206只支持linux安装此python包。
         except ImportError:
             raise ImportError('需要用户自己 pip install pulsar-client ，目前20221206只支持linux安装此python包,win不支持。')
         self._client = pulsar.Client(funboost_config_deafult.PULSAR_URL)
```

### Comparing `gaboost-1.6.8/funboost/consumers/rabbitmq_amqpstorm_consumer.py` & `gaboost-1.6.9/funboost/consumers/rabbitmq_amqpstorm_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/rabbitmq_pika_consumer.py` & `gaboost-1.6.9/funboost/consumers/rabbitmq_pika_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/rabbitmq_pika_consumerv0.py` & `gaboost-1.6.9/funboost/consumers/rabbitmq_pika_consumerv0.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/rabbitmq_rabbitpy_consumer.py` & `gaboost-1.6.9/funboost/consumers/rabbitmq_rabbitpy_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/redis_brpoplpush_consumer.py` & `gaboost-1.6.9/funboost/consumers/redis_brpoplpush_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/redis_consumer.py` & `gaboost-1.6.9/funboost/consumers/redis_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/redis_consumer_ack_able.py` & `gaboost-1.6.9/funboost/consumers/redis_consumer_ack_able.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/redis_consumer_simple.py` & `gaboost-1.6.9/funboost/consumers/redis_consumer_simple.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/redis_filter.py` & `gaboost-1.6.9/funboost/consumers/redis_filter.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/redis_pubsub_consumer.py` & `gaboost-1.6.9/funboost/consumers/redis_pubsub_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/redis_stream_consumer.py` & `gaboost-1.6.9/funboost/consumers/redis_stream_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/rocketmq_consumer.py` & `gaboost-1.6.9/funboost/consumers/rocketmq_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/sqlachemy_consumer.py` & `gaboost-1.6.9/funboost/consumers/sqlachemy_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/tcp_consumer.py` & `gaboost-1.6.9/funboost/consumers/tcp_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/txt_file_consumer.py` & `gaboost-1.6.9/funboost/consumers/txt_file_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/udp_consumer.py` & `gaboost-1.6.9/funboost/consumers/udp_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/consumers/zeromq_consumer.py` & `gaboost-1.6.9/funboost/consumers/zeromq_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/contrib/queue2queue.py` & `gaboost-1.6.9/funboost/contrib/queue2queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         # print(kwargs)
         nonlocal msg_cnt
         target_publisher.publish(kwargs)
         with msg_cnt_lock:
             msg_cnt += 1
 
     source_consumer = get_consumer(source_queue_name, broker_kind=source_broker_kind, consuming_function=_task_fun, log_level=log_level_int)
-    source_consumer.set_do_not_delete_extra_from_msg()
+    source_consumer._set_do_not_delete_extra_from_msg()
     source_consumer.start_consuming_message()
     if exit_script_when_finish:
         source_consumer.wait_for_possible_has_finish_all_tasks(2)
         print(f'消息转移完成，结束脚本,累计从 {source_queue_name} 转移消息到 {target_queue_name} 队列 总数是 {msg_cnt}')
         os._exit(888)  # 结束脚本
```

### Comparing `gaboost-1.6.8/funboost/contrib/redis_consume_latest_msg_broker.py` & `gaboost-1.6.9/funboost/contrib/redis_consume_latest_msg_broker.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/factories/consumer_factory.py` & `gaboost-1.6.9/funboost/factories/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/factories/publisher_factotry.py` & `gaboost-1.6.9/funboost/factories/publisher_factotry.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/funboost_config_deafult.py` & `gaboost-1.6.9/funboost/funboost_config_deafult.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,21 @@
 
 # ga_log包的第几个日志模板，内置了7个模板，可以在你当前项目根目录下的ga_log_config.py文件扩展模板。
 NB_LOG_FORMATER_INDEX_FOR_CONSUMER_AND_PUBLISHER = 11  # 7是简短的不可跳转，5是可点击跳转的，11是可显示ip 进程 线程的模板。
 FSDF_DEVELOP_LOG_LEVEL = 50  # 作者开发时候的调试代码的日志，仅供我自己用，所以日志级别跳到最高，用户不需要管。
 
 TIMEZONE = 'Asia/Shanghai'
 
+
+
+
+
+
+
+
 # *********************************************** 以下是 boost装饰器的默认全局配置 *******************************************
 """
 BoostDecoratorDefaultParams是@boost装饰器默认的全局入参。如果boost没有亲自指定某个入参，就自动使用这里的配置。
 这里的值不用配置，在boost装饰器中可以为每个消费者指定不同的入参，除非你嫌弃每个 boost 装饰器相同入参太多了，那么可以设置这里的全局默认值。
 
 例如用户不想每次在boost装饰器指定broker_kind为哪种消息队列，可以设置broker_kind为用户自己希望的默认消息队列类型
```

### Comparing `gaboost-1.6.8/funboost/helpers.py` & `gaboost-1.6.9/funboost/helpers.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/base_publisher.py` & `gaboost-1.6.9/funboost/publishers/base_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/confluent_kafka_publisher.py` & `gaboost-1.6.9/funboost/publishers/confluent_kafka_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/http_publisher.py` & `gaboost-1.6.9/funboost/publishers/http_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/httpsqs_publisher.py` & `gaboost-1.6.9/funboost/publishers/httpsqs_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/kafka_publisher.py` & `gaboost-1.6.9/funboost/publishers/kafka_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """
 
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         self._producer = KafkaProducer(bootstrap_servers=funboost_config_deafult.KAFKA_BOOTSTRAP_SERVERS)
         self._admin_client = KafkaAdminClient(bootstrap_servers=funboost_config_deafult.KAFKA_BOOTSTRAP_SERVERS)
         try:
-            self._admin_client.create_topics([NewTopic(self._queue_name, 10, 1)])
+            self._admin_client.create_topics([NewTopic(self._queue_name, 10, 2)])
             # admin_client.create_partitions({self._queue_name: NewPartitions(total_count=16)})
         except TopicAlreadyExistsError:
             pass
         except BaseException as e:
             self.logger.exception(e)
         atexit.register(self.close)  # 程序退出前不主动关闭，会报错。
```

### Comparing `gaboost-1.6.8/funboost/publishers/kombu_publisher.py` & `gaboost-1.6.9/funboost/publishers/kombu_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/local_python_queue_publisher.py` & `gaboost-1.6.9/funboost/publishers/local_python_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/mongomq_publisher.py` & `gaboost-1.6.9/funboost/publishers/mongomq_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/mqtt_publisher.py` & `gaboost-1.6.9/funboost/publishers/mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/nats_publisher.py` & `gaboost-1.6.9/funboost/publishers/nats_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/nsq_publisher.py` & `gaboost-1.6.9/funboost/publishers/nsq_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/peewee_publisher.py` & `gaboost-1.6.9/funboost/publishers/peewee_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/persist_queue_publisher.py` & `gaboost-1.6.9/funboost/publishers/persist_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/pulsar_publisher.py` & `gaboost-1.6.9/funboost/publishers/pulsar_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/rabbitmq_amqpstorm_publisher.py` & `gaboost-1.6.9/funboost/publishers/rabbitmq_amqpstorm_publisher.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     # noinspection PyAttributeOutsideInit
     # @decorators.synchronized
     def init_broker(self):
         # username=app_config.RABBITMQ_USER, password=app_config.RABBITMQ_PASS, host=app_config.RABBITMQ_HOST, port=app_config.RABBITMQ_PORT, virtual_host=app_config.RABBITMQ_VIRTUAL_HOST, heartbeat=60 * 10
         self.logger.warning(f'使用AmqpStorm包 链接mq')
         self.connection = amqpstorm.UriConnection(
-            f'amqp://{funboost_config_deafult.RABBITMQ_USER}:{funboost_config_deafult.RABBITMQ_PASS}@{funboost_config_deafult.RABBITMQ_HOST}:{funboost_config_deafult.RABBITMQ_PORT}/{funboost_config_deafult.RABBITMQ_VIRTUAL_HOST}?heartbeat={60 * 10}'
+            f'amqp://{funboost_config_deafult.RABBITMQ_USER}:{funboost_config_deafult.RABBITMQ_PASS}@{funboost_config_deafult.RABBITMQ_HOST}:{funboost_config_deafult.RABBITMQ_PORT}/{funboost_config_deafult.RABBITMQ_VIRTUAL_HOST}?heartbeat={60 * 10}&timeout=20000'
         )
         self.channel = self.connection.channel()  # type:amqpstorm.Channel
         self.channel_wrapper_by_ampqstormbaic = AmqpStormBasic(self.channel)
         self.queue = AmqpStormQueue(self.channel)
         self.queue.declare(queue=self._queue_name, durable=True)
 
     # @decorators.tomorrow_threads(10)
```

### Comparing `gaboost-1.6.8/funboost/publishers/rabbitmq_pika_publisher.py` & `gaboost-1.6.9/funboost/publishers/rabbitmq_pika_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/rabbitmq_rabbitpy_publisher.py` & `gaboost-1.6.9/funboost/publishers/rabbitmq_rabbitpy_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/redis_publisher.py` & `gaboost-1.6.9/funboost/publishers/redis_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/redis_publisher_simple.py` & `gaboost-1.6.9/funboost/publishers/redis_publisher_simple.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/redis_pubsub_publisher.py` & `gaboost-1.6.9/funboost/publishers/redis_pubsub_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/redis_stream_publisher.py` & `gaboost-1.6.9/funboost/publishers/redis_stream_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/rocketmq_publisher.py` & `gaboost-1.6.9/funboost/publishers/rocketmq_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/sqla_queue_publisher.py` & `gaboost-1.6.9/funboost/publishers/sqla_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/tcp_publisher.py` & `gaboost-1.6.9/funboost/publishers/tcp_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/txt_file_publisher.py` & `gaboost-1.6.9/funboost/publishers/txt_file_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/udp_publisher.py` & `gaboost-1.6.9/funboost/publishers/udp_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/publishers/zeromq_publisher.py` & `gaboost-1.6.9/funboost/publishers/zeromq_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/queues/peewee_queue.py` & `gaboost-1.6.9/funboost/queues/peewee_queue.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/queues/sqla_queue.py` & `gaboost-1.6.9/funboost/queues/sqla_queue.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/set_frame_config.py` & `gaboost-1.6.9/funboost/set_frame_config.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/timing_job/__init__.py` & `gaboost-1.6.9/funboost/timing_job/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/timing_job/apscheduler_use_redis_store.py` & `gaboost-1.6.9/funboost/timing_job/apscheduler_use_redis_store.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/timing_job/push_fun_for_apscheduler_use_db.py` & `gaboost-1.6.9/funboost/timing_job/push_fun_for_apscheduler_use_db.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/__init__.py` & `gaboost-1.6.9/funboost/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/apscheduler_monkey.py` & `gaboost-1.6.9/funboost/utils/apscheduler_monkey.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/bulk_operation.py` & `gaboost-1.6.9/funboost/utils/bulk_operation.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/custom_pysnooper.py` & `gaboost-1.6.9/funboost/utils/custom_pysnooper.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/decorators.py` & `gaboost-1.6.9/funboost/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/lock.py` & `gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/lock.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/mongomq.py` & `gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/mongomq.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/mongomq0000.py` & `gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/mongomq0000.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages/mongomq/test.py` & `gaboost-1.6.9/funboost/utils/dependency_packages/mongomq/test.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-310.pyc` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/dependency_packages_in_pythonpath/readme.md` & `gaboost-1.6.9/funboost/utils/dependency_packages_in_pythonpath/readme.md`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/mongo_util.py` & `gaboost-1.6.9/funboost/utils/mongo_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,42 +30,42 @@
 
 class MongoMixin:
     """
     mixin类被继承，也可以直接实例化。
 
     这个是修改后的，当使用f.multi_process_connsume() + linux +  保存结果到mongo + pymongo.0.2 时候不再报错了。
 
-    在linux上 即使写 connect=False，如果在主进程操作了collection，那么久破坏了 connect=False，在子进程中继续操作这个collection全局变量就会报错。
+    在linux上 即使写 connect=False，如果在主进程操作了collection，那么就破坏了 connect=False，在子进程中继续操作这个collection全局变量就会报错。
+    设计了多进程+fork 每次都 get_mongo_collection() 是最保险的
     """
     processid__client_map = {}
     processid__db_map = {}
     processid__col_map = {}
 
     @property
     def mongo_client(self) -> pymongo.MongoClient:
         pid = os.getpid()
-        if pid not in MongoMixin.processid__client_map:
-            MongoMixin.processid__client_map[pid] = pymongo.MongoClient(funboost_config_deafult.MONGO_CONNECT_URL,
-                                                                        connect=False,maxIdleTimeMS=60*1000,minPoolSize=3,maxPoolSize=20)
-        return MongoMixin.processid__client_map[pid]
+        key = pid
+        if key not in MongoMixin.processid__client_map:
+            MongoMixin.processid__client_map[key] = pymongo.MongoClient(funboost_config_deafult.MONGO_CONNECT_URL,
+                                                                        connect=False, maxIdleTimeMS=60 * 1000, minPoolSize=3, maxPoolSize=20)
+        return MongoMixin.processid__client_map[key]
 
     @property
     def mongo_db_task_status(self):
         pid = os.getpid()
-        key = (pid,'task_status')
+        key = (pid, 'task_status')
         if key not in MongoMixin.processid__db_map:
             MongoMixin.processid__db_map[key] = self.mongo_client.get_database('task_status')
         return MongoMixin.processid__db_map[key]
 
-    def get_mongo_collection(self,database_name,colleciton_name):
+    def get_mongo_collection(self, database_name, colleciton_name) -> pymongo.collection.Collection:
         pid = os.getpid()
         key = (pid, database_name, colleciton_name)
         if key not in MongoMixin.processid__col_map:
             MongoMixin.processid__col_map[key] = self.mongo_client.get_database(database_name).get_collection(colleciton_name)
         return MongoMixin.processid__col_map[key]
 
 
-
-
 if __name__ == '__main__':
-    print(MongoMixin().get_mongo_collection('db2','col2'))
-    print(MongoMixin().get_mongo_collection('db2', 'col3'))
+    print(MongoMixin().get_mongo_collection('db2', 'col2'))
+    print(MongoMixin().get_mongo_collection('db2', 'col3'))
```

### Comparing `gaboost-1.6.8/funboost/utils/monkey_color_log.py` & `gaboost-1.6.9/funboost/utils/monkey_color_log.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/monkey_patches.py` & `gaboost-1.6.9/funboost/utils/monkey_patches.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/mqtt_util.py` & `gaboost-1.6.9/funboost/utils/mqtt_util.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/paramiko_util.py` & `gaboost-1.6.9/funboost/utils/paramiko_util.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/pysnooper_ydf/__init__.py` & `gaboost-1.6.9/funboost/utils/pysnooper_ydf/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/pysnooper_ydf/pycompat.py` & `gaboost-1.6.9/funboost/utils/pysnooper_ydf/pycompat.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/pysnooper_ydf/tracer.py` & `gaboost-1.6.9/funboost/utils/pysnooper_ydf/tracer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/pysnooper_ydf/utils.py` & `gaboost-1.6.9/funboost/utils/pysnooper_ydf/utils.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/pysnooper_ydf/variables.py` & `gaboost-1.6.9/funboost/utils/pysnooper_ydf/variables.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/rabbitmq_factory.py` & `gaboost-1.6.9/funboost/utils/rabbitmq_factory.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/redis_manager.py` & `gaboost-1.6.9/funboost/utils/redis_manager.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/resource_monitoring.py` & `gaboost-1.6.9/funboost/utils/resource_monitoring.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/restart_python.py` & `gaboost-1.6.9/funboost/utils/restart_python.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/simple_data_class.py` & `gaboost-1.6.9/funboost/utils/simple_data_class.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/funboost/utils/time_util.py` & `gaboost-1.6.9/funboost/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/gaboost.egg-info/PKG-INFO` & `gaboost-1.6.9/gaboost.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaboost
-Version: 1.6.8
+Version: 1.6.9
 Summary: fork funboost
 Author: ziko
 License: BSD License
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `gaboost-1.6.8/gaboost.egg-info/SOURCES.txt` & `gaboost-1.6.9/gaboost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaboost-1.6.8/setup.py` & `gaboost-1.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='gaboost',  #
-    version='1.6.8',
+    version='1.6.9',
     description=(
         'fork funboost'
     ),
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     # keywords=["funboost", "distributed-framework", "function-scheduling", "rabbitmq", "rocketmq", "kafka", "nsq", "redis", "disk",
     #           "sqlachemy", "consume-confirm", "timing", "task-scheduling", "apscheduler", "pulsar", "mqtt", "kombu"],
     #long_description_content_type="text/markdown",
```

