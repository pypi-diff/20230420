# Comparing `tmp/VisionFive.gpio-1.2.7.tar.gz` & `tmp/VisionFive.gpio-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionFive.gpio-1.2.7.tar", last modified: Thu Apr  6 06:31:47 2023, max compression
+gzip compressed data, was "VisionFive.gpio-1.2.8.tar", last modified: Thu Apr 20 07:21:45 2023, max compression
```

## Comparing `VisionFive.gpio-1.2.7.tar` & `VisionFive.gpio-1.2.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.673470 VisionFive.gpio-1.2.7/
--rw-r--r--   0 sz        (1000) sz        (1000)      942 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/CHANGELOG.txt
--rw-r--r--   0 sz        (1000) sz        (1000)      430 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/INSTALL.txt
--rw-r--r--   0 sz        (1000) sz        (1000)     1060 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/LICENCE.txt
--rw-r--r--   0 sz        (1000) sz        (1000)       50 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/MANIFEST.in
--rw-rw-r--   0 sz        (1000) sz        (1000)     2449 2023-04-06 06:31:47.673470 VisionFive.gpio-1.2.7/PKG-INFO
--rw-r--r--   0 sz        (1000) sz        (1000)      757 2023-04-06 06:31:23.000000 VisionFive.gpio-1.2.7/README.txt
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.661470 VisionFive.gpio-1.2.7/VisionFive/
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.665470 VisionFive.gpio-1.2.7/VisionFive/boardtype/
--rw-r--r--   0 sz        (1000) sz        (1000)     1241 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/boardtype/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.665470 VisionFive.gpio-1.2.7/VisionFive/gpio/
--rw-r--r--   0 sz        (1000) sz        (1000)     1226 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/gpio/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.665470 VisionFive.gpio-1.2.7/VisionFive/i2c/
--rw-r--r--   0 sz        (1000) sz        (1000)     1225 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/i2c/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.665470 VisionFive.gpio-1.2.7/VisionFive/sample-code/
--rw-r--r--   0 sz        (1000) sz        (1000)     3760 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/I2C_Sense_Hat.py
--rw-r--r--   0 sz        (1000) sz        (1000)     2569 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/LED_Matrix.py
--rw-r--r--   0 sz        (1000) sz        (1000)      946 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/RPi_demo_#GPIO_basic#_run_on_VisionFive.py
--rw-r--r--   0 sz        (1000) sz        (1000)      826 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/RPi_demo_#PWM#_run_on_VisionFive.py
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/__init__.py
--rw-r--r--   0 sz        (1000) sz        (1000)     2156 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/basic_edge_detection.py
--rw-r--r--   0 sz        (1000) sz        (1000)     1730 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/buzzer.py
--rw-r--r--   0 sz        (1000) sz        (1000)     4829 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/edge_detection_with_LED_Matrix.py
--rw-r--r--   0 sz        (1000) sz        (1000)     2817 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/edge_detection_with_waiting_time.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.665470 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/
--rw-r--r--   0 sz        (1000) sz        (1000)       86 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/READEME.txt
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.665470 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/
--rw-r--r--   0 sz        (1000) sz        (1000)     2598 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/2.4inch_LCD_demo.py
--rw-r--r--   0 sz        (1000) sz        (1000)    31487 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/LCD_2inch.jpg
--rw-r--r--   0 sz        (1000) sz        (1000)   153656 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/LCD_2inch4_parrot.bmp
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/__init__.py
--rw-r--r--   0 sz        (1000) sz        (1000)   230454 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/visionfive.bmp
--rw-r--r--   0 sz        (1000) sz        (1000)   230454 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/visionfive2.bmp
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.669470 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/lib/
--rw-r--r--   0 sz        (1000) sz        (1000)     7733 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/lib/LCD2inch4_lib.py
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/lib/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.669470 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/lib/example/
--rw-r--r--   0 sz        (1000) sz        (1000)      417 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/lib/example/LCD_2intest.py
--rw-r--r--   0 sz        (1000) sz        (1000)      925 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/led.py
--rw-r--r--   0 sz        (1000) sz        (1000)     1390 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/pud_test.py
--rw-r--r--   0 sz        (1000) sz        (1000)     1150 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/pwm_led.py
--rw-r--r--   0 sz        (1000) sz        (1000)     8642 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/sample-code/uart_gps_demo.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.669470 VisionFive.gpio-1.2.7/VisionFive/spi/
--rw-r--r--   0 sz        (1000) sz        (1000)     1225 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/VisionFive/spi/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.661470 VisionFive.gpio-1.2.7/VisionFive.gpio.egg-info/
--rw-r--r--   0 sz        (1000) sz        (1000)     2449 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.7/VisionFive.gpio.egg-info/PKG-INFO
--rw-r--r--   0 sz        (1000) sz        (1000)     2019 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.7/VisionFive.gpio.egg-info/SOURCES.txt
--rw-r--r--   0 sz        (1000) sz        (1000)        1 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.7/VisionFive.gpio.egg-info/dependency_links.txt
--rw-r--r--   0 sz        (1000) sz        (1000)       11 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.7/VisionFive.gpio.egg-info/top_level.txt
--rw-r--r--   0 sz        (1000) sz        (1000)       38 2023-04-06 06:31:47.673470 VisionFive.gpio-1.2.7/setup.cfg
--rw-r--r--   0 sz        (1000) sz        (1000)     3747 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/setup.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.661470 VisionFive.gpio-1.2.7/source/
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.669470 VisionFive.gpio-1.2.7/source/boardtype/
--rw-r--r--   0 sz        (1000) sz        (1000)     1340 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/boardtype/py_boardtype.c
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.669470 VisionFive.gpio-1.2.7/source/gpio/
--rw-r--r--   0 sz        (1000) sz        (1000)    10302 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/c_gpio.c
--rw-r--r--   0 sz        (1000) sz        (1000)    21693 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/c_gpio.h
--rw-r--r--   0 sz        (1000) sz        (1000)     1510 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/cpuinfo.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1394 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/cpuinfo.h
--rw-r--r--   0 sz        (1000) sz        (1000)    15109 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/event_gpio.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1703 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/event_gpio.h
--rw-r--r--   0 sz        (1000) sz        (1000)     9596 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/gpio-utils.c
--rw-r--r--   0 sz        (1000) sz        (1000)     2097 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/gpio-utils.h
--rw-r--r--   0 sz        (1000) sz        (1000)     2866 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/py_constants.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1615 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/py_constants.h
--rw-r--r--   0 sz        (1000) sz        (1000)    22867 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/gpio/py_gpio.c
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.669470 VisionFive.gpio-1.2.7/source/i2c/
--rw-r--r--   0 sz        (1000) sz        (1000)     1845 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/i2c/c_i2c.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1345 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/i2c/c_i2c.h
--rw-r--r--   0 sz        (1000) sz        (1000)     4369 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/i2c/py_i2c.c
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.673470 VisionFive.gpio-1.2.7/source/pwm/
--rw-r--r--   0 sz        (1000) sz        (1000)     6174 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/pwm/py_pwm.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1190 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/pwm/py_pwm.h
--rw-r--r--   0 sz        (1000) sz        (1000)     5188 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/pwm/soft_pwm.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1334 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/pwm/soft_pwm.h
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.673470 VisionFive.gpio-1.2.7/source/spi/
--rw-r--r--   0 sz        (1000) sz        (1000)     6105 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/spi/py_spi.c
--rw-r--r--   0 sz        (1000) sz        (1000)     3831 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/spi/spi_dev.c
--rw-r--r--   0 sz        (1000) sz        (1000)      407 2023-04-06 06:27:26.000000 VisionFive.gpio-1.2.7/source/spi/spi_dev.h
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1003 2023-04-20 07:12:09.000000 VisionFive.gpio-1.2.8/CHANGELOG.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)      430 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/INSTALL.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)     1060 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/LICENCE.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)       50 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/MANIFEST.in
+-rw-rw-r--   0 sz        (1000) sz        (1000)     2510 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/PKG-INFO
+-rw-r--r--   0 sz        (1000) sz        (1000)      757 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/README.txt
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive/
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive/boardtype/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1241 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/boardtype/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive/gpio/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1226 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/gpio/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive/i2c/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1225 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/i2c/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.913627 VisionFive.gpio-1.2.8/VisionFive/sample-code/
+-rw-r--r--   0 sz        (1000) sz        (1000)     3760 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/I2C_Sense_Hat.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     2569 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/LED_Matrix.py
+-rw-r--r--   0 sz        (1000) sz        (1000)      946 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/RPi_demo_#GPIO_basic#_run_on_VisionFive.py
+-rw-r--r--   0 sz        (1000) sz        (1000)      826 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/RPi_demo_#PWM#_run_on_VisionFive.py
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/__init__.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     2156 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/basic_edge_detection.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     1730 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/buzzer.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     4829 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/edge_detection_with_LED_Matrix.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     2817 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/edge_detection_with_waiting_time.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.913627 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/
+-rw-r--r--   0 sz        (1000) sz        (1000)       86 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/READEME.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.913627 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/
+-rw-r--r--   0 sz        (1000) sz        (1000)     2598 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/2.4inch_LCD_demo.py
+-rw-r--r--   0 sz        (1000) sz        (1000)    31487 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/LCD_2inch.jpg
+-rw-r--r--   0 sz        (1000) sz        (1000)   153656 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/LCD_2inch4_parrot.bmp
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/__init__.py
+-rw-r--r--   0 sz        (1000) sz        (1000)   230454 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/visionfive.bmp
+-rw-r--r--   0 sz        (1000) sz        (1000)   230454 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/visionfive2.bmp
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/
+-rw-r--r--   0 sz        (1000) sz        (1000)     7733 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/LCD2inch4_lib.py
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/example/
+-rw-r--r--   0 sz        (1000) sz        (1000)      417 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/example/LCD_2intest.py
+-rw-r--r--   0 sz        (1000) sz        (1000)      925 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/led.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     1390 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/pud_test.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     1150 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/pwm_led.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     8642 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/uart_gps_demo.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/VisionFive/spi/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1225 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/spi/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/
+-rw-rw-r--   0 sz        (1000) sz        (1000)     2510 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/PKG-INFO
+-rw-rw-r--   0 sz        (1000) sz        (1000)     2019 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/SOURCES.txt
+-rw-rw-r--   0 sz        (1000) sz        (1000)        1 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/dependency_links.txt
+-rw-rw-r--   0 sz        (1000) sz        (1000)       11 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/top_level.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)       38 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/setup.cfg
+-rw-r--r--   0 sz        (1000) sz        (1000)     3747 2023-04-20 07:21:22.000000 VisionFive.gpio-1.2.8/setup.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.905627 VisionFive.gpio-1.2.8/source/
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/source/boardtype/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1340 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/boardtype/py_boardtype.c
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/source/gpio/
+-rw-r--r--   0 sz        (1000) sz        (1000)    10302 2023-04-20 07:19:24.000000 VisionFive.gpio-1.2.8/source/gpio/c_gpio.c
+-rw-r--r--   0 sz        (1000) sz        (1000)    21693 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/c_gpio.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     1510 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/cpuinfo.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1394 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/cpuinfo.h
+-rw-r--r--   0 sz        (1000) sz        (1000)    15109 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/event_gpio.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1703 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/event_gpio.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     9596 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/gpio-utils.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     2097 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/gpio-utils.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     2866 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/py_constants.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1615 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/py_constants.h
+-rw-r--r--   0 sz        (1000) sz        (1000)    22867 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/py_gpio.c
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/source/i2c/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1845 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/i2c/c_i2c.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1345 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/i2c/c_i2c.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     4369 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/i2c/py_i2c.c
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/source/pwm/
+-rw-r--r--   0 sz        (1000) sz        (1000)     6174 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/pwm/py_pwm.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1190 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/pwm/py_pwm.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     5188 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/pwm/soft_pwm.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1334 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/pwm/soft_pwm.h
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/source/spi/
+-rw-r--r--   0 sz        (1000) sz        (1000)     6105 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/spi/py_spi.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     3831 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/spi/spi_dev.c
+-rw-r--r--   0 sz        (1000) sz        (1000)      407 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/spi/spi_dev.h
```

### Comparing `VisionFive.gpio-1.2.7/CHANGELOG.txt` & `VisionFive.gpio-1.2.8/CHANGELOG.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 Change Log
 ==========
+1.2.8
+-------
+-Fix gpio issue
+
+1.2.7
+-------
+-Fix pud issue
+
 1.2.6
 -------
 - Support GPIO edge detection
 - Add GPIO edge detection demo
 
 1.2.5
 -------
```

### Comparing `VisionFive.gpio-1.2.7/LICENCE.txt` & `VisionFive.gpio-1.2.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/PKG-INFO` & `VisionFive.gpio-1.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionFive.gpio
-Version: 1.2.7
+Version: 1.2.8
 Summary: A module to control VisionFive GPIO ports
 Home-page: http://gitlab.starfivetech.com/Product/Software AE/VisionFive-python-gpio/starfive_gpio
 Author: VisionFive
 Author-email: support@starfivetech.com
 License: MIT
 Keywords: VisionFive GPIO
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,14 +32,22 @@
 edge_with_waiting_time about edge detection with specific time, 
 edge_with_LED_Matrix about trigger LED display by button, 
 RPi_demo_#GPIO_basic#_run_on_VisionFive about running RPi GPIO demo on VisionFive board, 
 RPi_demo_#PWM#_run_on_VisionFive about running RPi PWM demo on VisionFive board.
 
 Change Log
 ==========
+1.2.8
+-------
+-Fix gpio issue
+
+1.2.7
+-------
+-Fix pud issue
+
 1.2.6
 -------
 - Support GPIO edge detection
 - Add GPIO edge detection demo
 
 1.2.5
 -------
```

### Comparing `VisionFive.gpio-1.2.7/README.txt` & `VisionFive.gpio-1.2.8/README.txt`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/boardtype/__init__.py` & `VisionFive.gpio-1.2.8/VisionFive/boardtype/__init__.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/gpio/__init__.py` & `VisionFive.gpio-1.2.8/VisionFive/gpio/__init__.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/i2c/__init__.py` & `VisionFive.gpio-1.2.8/VisionFive/i2c/__init__.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/I2C_Sense_Hat.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/I2C_Sense_Hat.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/LED_Matrix.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/LED_Matrix.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/RPi_demo_#GPIO_basic#_run_on_VisionFive.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/RPi_demo_#GPIO_basic#_run_on_VisionFive.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/RPi_demo_#PWM#_run_on_VisionFive.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/RPi_demo_#PWM#_run_on_VisionFive.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/basic_edge_detection.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/basic_edge_detection.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/buzzer.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/buzzer.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/edge_detection_with_LED_Matrix.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/edge_detection_with_LED_Matrix.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/edge_detection_with_waiting_time.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/edge_detection_with_waiting_time.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/2.4inch_LCD_demo.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/2.4inch_LCD_demo.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/LCD_2inch.jpg` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/LCD_2inch.jpg`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/LCD_2inch4_parrot.bmp` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/LCD_2inch4_parrot.bmp`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/visionfive.bmp` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/visionfive.bmp`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/example/visionfive2.bmp` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/visionfive2.bmp`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/lcddemo/lib/LCD2inch4_lib.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/LCD2inch4_lib.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/led.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/led.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/pud_test.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/pud_test.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/pwm_led.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/pwm_led.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/sample-code/uart_gps_demo.py` & `VisionFive.gpio-1.2.8/VisionFive/sample-code/uart_gps_demo.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive/spi/__init__.py` & `VisionFive.gpio-1.2.8/VisionFive/spi/__init__.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/VisionFive.gpio.egg-info/PKG-INFO` & `VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionFive.gpio
-Version: 1.2.7
+Version: 1.2.8
 Summary: A module to control VisionFive GPIO ports
 Home-page: http://gitlab.starfivetech.com/Product/Software AE/VisionFive-python-gpio/starfive_gpio
 Author: VisionFive
 Author-email: support@starfivetech.com
 License: MIT
 Keywords: VisionFive GPIO
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,14 +32,22 @@
 edge_with_waiting_time about edge detection with specific time, 
 edge_with_LED_Matrix about trigger LED display by button, 
 RPi_demo_#GPIO_basic#_run_on_VisionFive about running RPi GPIO demo on VisionFive board, 
 RPi_demo_#PWM#_run_on_VisionFive about running RPi PWM demo on VisionFive board.
 
 Change Log
 ==========
+1.2.8
+-------
+-Fix gpio issue
+
+1.2.7
+-------
+-Fix pud issue
+
 1.2.6
 -------
 - Support GPIO edge detection
 - Add GPIO edge detection demo
 
 1.2.5
 -------
```

### Comparing `VisionFive.gpio-1.2.7/VisionFive.gpio.egg-info/SOURCES.txt` & `VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/setup.py` & `VisionFive.gpio-1.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 module_boardtype = Extension('VisionFive._boardtype',
                            [
                             'source/gpio/cpuinfo.c',
                             'source/boardtype/py_boardtype.c'])
 
 setup(name             = 'VisionFive.gpio',
-      version          = '1.2.7',
+      version          = '1.2.8',
       author           = 'VisionFive',
       author_email     = 'support@starfivetech.com',
       description      = 'A module to control VisionFive GPIO ports',
       long_description = open('README.txt').read() + open('CHANGELOG.txt').read(),
       license          = 'MIT',
       keywords         = 'VisionFive GPIO',
       url              = 'http://gitlab.starfivetech.com/Product/Software AE/VisionFive-python-gpio/starfive_gpio',
```

### Comparing `VisionFive.gpio-1.2.7/source/boardtype/py_boardtype.c` & `VisionFive.gpio-1.2.8/source/boardtype/py_boardtype.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/c_gpio.c` & `VisionFive.gpio-1.2.8/source/gpio/c_gpio.c`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
    -1,  -1,  -1,  -1,  -1,  -1,  -1,  46,  -1,  -1,  -1,  44,  -1,  22,  -1,  20,  21,  -1,  19,  -1,  -1,
 // 21   22   23   24   25   26   27   28    29   30   31  32    33  34   35   36   37   38   39  40
    -1,  17,  -1,  -1,  -1,  -1,   9,  10,   8,   -1,  6,  -1,   -1,  -1,  3,   4,   1,   2,  -1,  0
   };
 
 const int GPIO2line_VisionFive_v2[41] = {
 //   0    1    2    3    4    5   6   7     8    9  10    11   12   13   14   15   16   17   18  19  20
-    -1,  -1,  -1,  -1,  -1,  -1, -1,  55,  -1,  -1, -1,   42,  38,  43,  -1,  47,  54,  -1,  21, -1, -1,
+    -1,  -1,  -1,  -1,  -1,  -1, -1,  55,  -1,  -1, -1,   42,  38,  43,  -1,  47,  54,  -1,  51, -1, -1,
 //  21   22   23    24  25  26   27   28   29   30   31   32   33   34   35   36   37   38   39   40
 	-1,  50,  -1,  -1, -1,  56,  45,  40,  37,  -1,  39,  -1,  -1,  -1,  63,  36,  60,  61,  -1,  44
 	};
 
 int gpio_direction[41] = {
 	-1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1,
 	-1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1,
```

### Comparing `VisionFive.gpio-1.2.7/source/gpio/c_gpio.h` & `VisionFive.gpio-1.2.8/source/gpio/c_gpio.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/cpuinfo.c` & `VisionFive.gpio-1.2.8/source/gpio/cpuinfo.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/cpuinfo.h` & `VisionFive.gpio-1.2.8/source/gpio/cpuinfo.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/event_gpio.c` & `VisionFive.gpio-1.2.8/source/gpio/event_gpio.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/event_gpio.h` & `VisionFive.gpio-1.2.8/source/gpio/event_gpio.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/gpio-utils.c` & `VisionFive.gpio-1.2.8/source/gpio/gpio-utils.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/gpio-utils.h` & `VisionFive.gpio-1.2.8/source/gpio/gpio-utils.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/py_constants.c` & `VisionFive.gpio-1.2.8/source/gpio/py_constants.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/py_constants.h` & `VisionFive.gpio-1.2.8/source/gpio/py_constants.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/gpio/py_gpio.c` & `VisionFive.gpio-1.2.8/source/gpio/py_gpio.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/i2c/c_i2c.c` & `VisionFive.gpio-1.2.8/source/i2c/c_i2c.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/i2c/c_i2c.h` & `VisionFive.gpio-1.2.8/source/i2c/c_i2c.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/i2c/py_i2c.c` & `VisionFive.gpio-1.2.8/source/i2c/py_i2c.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/pwm/py_pwm.c` & `VisionFive.gpio-1.2.8/source/pwm/py_pwm.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/pwm/py_pwm.h` & `VisionFive.gpio-1.2.8/source/pwm/py_pwm.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/pwm/soft_pwm.c` & `VisionFive.gpio-1.2.8/source/pwm/soft_pwm.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/pwm/soft_pwm.h` & `VisionFive.gpio-1.2.8/source/pwm/soft_pwm.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/spi/py_spi.c` & `VisionFive.gpio-1.2.8/source/spi/py_spi.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.7/source/spi/spi_dev.c` & `VisionFive.gpio-1.2.8/source/spi/spi_dev.c`

 * *Files identical despite different names*

